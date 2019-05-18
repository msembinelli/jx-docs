---
date: 2019-05-18T11:02:42Z
title: "jx promote"
slug: jx_promote
url: /commands/jx_promote/
---
## jx promote

Promotes a version of an application to an Environment

### Synopsis

Promotes a version of an application to zero to many permanent environments. 

For more documentation see: https://jenkins-x.io/about/features/#promotion

```
jx promote [application] [flags]
```

### Examples

```
  # Promote a version of the current application to staging
  # discovering the application name from the source code
  jx promote --version 1.2.3 --env staging
  
  # Promote a version of the myapp application to production
  jx promote myapp --version 1.2.3 --env production
  
  # To search for all the available charts for a given name use -f.
  # e.g. to find a redis chart to install
  jx promote -f redis
  
  # To promote a postgres chart using an alias
  jx promote -f postgres --alias mydb
  
  # To create or update a Preview Environment please see the 'jx preview' command
  jx preview
```

### Options

```
      --alias string                    The optional alias used in the 'requirements.yaml' file
      --all-auto                        Promote to all automatic environments in order
  -a, --app string                      The Application to promote
      --build string                    The Build number which is used to update the PipelineActivity. If not specified its defaulted from  the '$BUILD_NUMBER' environment variable
  -e, --env string                      The Environment to promote to
  -f, --filter string                   The search filter to find charts to promote
  -r, --helm-repo-name string           The name of the helm repository that contains the app (default "releases")
  -u, --helm-repo-url string            The Helm Repository URL to use for the App (default "http://jenkins-x-chartmuseum:8080")
  -h, --help                            help for promote
      --ignore-local-file               Ignores the local file system when deducing the Git repository
  -n, --namespace string                The Namespace to promote to
      --no-helm-update                  Allows the 'helm repo update' command if you are sure your local helm cache is up to date with the version you wish to promote
      --no-merge                        Disables automatic merge of promote Pull Requests
      --no-poll                         Disables polling for Pull Request or Pipeline status
      --no-wait                         Disables waiting for completing promotion after the Pull request is merged
      --pipeline string                 The Pipeline string in the form 'folderName/repoName/branch' which is used to update the PipelineActivity. If not specified its defaulted from  the '$BUILD_NUMBER' environment variable
      --pull-request-poll-time string   Poll time when waiting for a Pull Request to merge (default "20s")
      --release string                  The name of the helm release
  -t, --timeout string                  The timeout to wait for the promotion to succeed in the underlying Environment. The command fails if the timeout is exceeded or the promotion does not complete (default "1h")
  -v, --version string                  The Version to promote
```

### Options inherited from parent commands

```
  -b, --batch-mode                Runs in batch mode without prompting for user input (default true)
      --install-dependencies      Enables automatic dependencies installation when required
      --log-level string          Sets the logging level (panic, fatal, error, warning, info, debug) (default "info")
      --no-brew                   Disables brew package manager on MacOS when installing binary dependencies
      --skip-auth-secrets-merge   Skips merging the secrets from local files with the secrets from Kubernetes cluster
      --verbose                   Enables verbose output
```

### SEE ALSO

* [jx](/commands/jx/)	 - jx is a command line tool for working with Jenkins X

###### Auto generated by spf13/cobra on 18-May-2019