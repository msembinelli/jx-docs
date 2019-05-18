---
date: 2019-05-18T11:02:42Z
title: "jx delete chat server"
slug: jx_delete_chat_server
url: /commands/jx_delete_chat_server/
---
## jx delete chat server

Deletes one or more chat server(s)

### Synopsis

Deletes one or more chat servers from your local settings

```
jx delete chat server [flags]
```

### Examples

```
  # Deletes an chat server
  jx delete chat server MyProvider
```

### Options

```
  -h, --help             help for server
  -i, --ignore-missing   Silently ignore attempts to remove an chat server name that does not exist
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

* [jx delete chat](/commands/jx_delete_chat/)	 - Deletes one or more chat services resources

###### Auto generated by spf13/cobra on 18-May-2019