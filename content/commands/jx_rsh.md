---
date: 2019-05-18T11:02:42Z
title: "jx rsh"
slug: jx_rsh
url: /commands/jx_rsh/
---
## jx rsh

Opens a terminal in a pod or runs a command in the pod

### Synopsis

Opens a terminal or runs a command in a pods container

```
jx rsh [deploymentOrPodName] [flags]
```

### Examples

```
  # Open a terminal in the first container of the foo deployment's latest pod
  jx rsh foo
  
  # Opens a terminal in the cheese container in the latest pod in the foo deployment
  jx rsh -c cheese foo
  
  # To connect to one of your DevPods use:
  jx rsh -d
  
  # To execute something in the remote shell (like classic rsh or ssh commands)
  jx rsh -e 'do something'
```

### Options

```
  -c, --container string     The name of the container to log
  -d, --devpod               Connect to a DevPod
      --environment string   The environment in which to look for the Deployment. Defaults to the current environment
  -e, --execute string       Execute this command on the remote container (default "bash")
  -h, --help                 help for rsh
  -n, --namespace string     the namespace to look for the Deployment. Defaults to the current namespace
  -p, --pod string           the pod name to use
  -s, --shell string         Path to the shell command
      --username string      The username to create the DevPod. If not specified defaults to the current operating system user or $USER'
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