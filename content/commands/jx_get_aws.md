---
date: 2019-05-18T11:02:42Z
title: "jx get aws"
slug: jx_get_aws
url: /commands/jx_get_aws/
---
## jx get aws

Displays AWS account information

### Synopsis

Display the AWS information for the current user

```
jx get aws info [flags]
```

### Examples

```
  # Get the AWS account information
  jx get aws info
```

### Options

```
  -h, --help            help for aws
  -o, --output string   The output format such as 'yaml'
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

* [jx get](/commands/jx_get/)	 - Display one or more resources

###### Auto generated by spf13/cobra on 18-May-2019