---
date: 2019-05-18T11:02:42Z
title: "jx start protection"
slug: jx_start_protection
url: /commands/jx_start_protection/
---
## jx start protection

Starts protection

### Synopsis

Starts protection checking on an app

```
jx start protection [flags]
```

### Examples

```
  # Start protection
  jx start protection <context> <org/repo>
  
  # For example, to enable compliance on a repopository called "example" in the "acme" organization
  jx start protection compliance-check acme/example
```

### Options

```
  -h, --help   help for protection
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

* [jx start](/commands/jx_start/)	 - Starts a process such as a pipeline

###### Auto generated by spf13/cobra on 18-May-2019