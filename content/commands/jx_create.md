---
date: 2019-05-18T11:02:42Z
title: "jx create"
slug: jx_create
url: /commands/jx_create/
---
## jx create

Create a new resource

### Synopsis

Creates a new resource.
  
  Valid resource types include:
  
  * archetype  
  * cluster  
  * env  
  * git  
  * spring (aka 'springboot')

```
jx create [flags]
```

### Options

```
  -h, --help   help for create
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
* [jx create addon](/commands/jx_create_addon/)	 - Creates an addon
* [jx create archetype](/commands/jx_create_archetype/)	 - Create a new app from a Maven Archetype and import the generated code into Git and Jenkins for CI/CD
* [jx create branchpattern](/commands/jx_create_branchpattern/)	 - Create a git branch pattern for your team
* [jx create camel](/commands/jx_create_camel/)	 - Create a new Camel based application and import the generated code into Git and Jenkins for CI/CD
* [jx create chat](/commands/jx_create_chat/)	 - Creates a chat server resource
* [jx create cluster](/commands/jx_create_cluster/)	 - Create a new Kubernetes cluster
* [jx create codeship](/commands/jx_create_codeship/)	 - Creates a build on Codeship to create/update JX clusters
* [jx create devpod](/commands/jx_create_devpod/)	 - Creates a DevPod for running builds and tests inside the cluster
* [jx create docker](/commands/jx_create_docker/)	 - Create/update Docker auth for a given host and user in the config.json file
* [jx create docs](/commands/jx_create_docs/)	 - Creates the documentation files
* [jx create environment](/commands/jx_create_environment/)	 - Create a new Environment which is used to promote your Team's Applications via Continuous Delivery
* [jx create etc-hosts](/commands/jx_create_etc-hosts/)	 - Creates a new Git server URL
* [jx create git](/commands/jx_create_git/)	 - Creates a Git resource
* [jx create gke-service-account](/commands/jx_create_gke-service-account/)	 - Creates a GKE service account
* [jx create issue](/commands/jx_create_issue/)	 - Create an issue on the git project for the current directory
* [jx create jenkins](/commands/jx_create_jenkins/)	 - Creates a Jenkins resource
* [jx create jhipster](/commands/jx_create_jhipster/)	 - Create a new JHipster based application and import the generated code into Git and Jenkins for CI/CD
* [jx create lile](/commands/jx_create_lile/)	 - Create a new Lile based application and import the generated code into Git and Jenkins for CI/CD
* [jx create micro](/commands/jx_create_micro/)	 - Create a new micro based application and import the generated code into Git and Jenkins for CI/CD
* [jx create mlquickstart](/commands/jx_create_mlquickstart/)	 - Create a new machine learning app from a set of quickstarts and import the generated code into Git and Jenkins for CI/CD
* [jx create post](/commands/jx_create_post/)	 - Create a job which is triggered after a Preview is created
* [jx create project](/commands/jx_create_project/)	 - Create a new Project by importing code, using a Quickstart or custom wizard for Spring or Camel
* [jx create pullrequest](/commands/jx_create_pullrequest/)	 - Create a Pull Request on the git project for the current directory
* [jx create quickstart](/commands/jx_create_quickstart/)	 - Create a new app from a Quickstart and import the generated code into Git and Jenkins for CI/CD
* [jx create quickstartlocation](/commands/jx_create_quickstartlocation/)	 - Create a location of quickstarts for your team
* [jx create spring](/commands/jx_create_spring/)	 - Create a new Spring Boot application and import the generated code into Git and Jenkins for CI/CD
* [jx create step](/commands/jx_create_step/)	 - Creates a step in the Jenkins X Pipeline
* [jx create team](/commands/jx_create_team/)	 - Create a new Team which is then provisioned later on
* [jx create terraform](/commands/jx_create_terraform/)	 - Creates a Jenkins X Terraform plan
* [jx create token](/commands/jx_create_token/)	 - Creates a new user token for a service
* [jx create tracker](/commands/jx_create_tracker/)	 - Creates an issue tracker resource
* [jx create user](/commands/jx_create_user/)	 - Create a new User which is then provisioned by the user controller
* [jx create variable](/commands/jx_create_variable/)	 - Creates an environment variable in the Jenkins X Pipeline
* [jx create vault](/commands/jx_create_vault/)	 - Create a new Vault using the vault-operator

###### Auto generated by spf13/cobra on 18-May-2019