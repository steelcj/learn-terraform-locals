# Terraform Patterns for Identifying Project Infrastructure

Implements solutions proposed in Learn Terraform locals tutorial (see link below)

In a nutshell allows for the creation (and renaming) of "name/tagged" infrastructure using a pattern like this from the command line:

```shell
terraform apply -var "environment=prod" -var "project_name=alpha-001"
```

if -var option not used for one or more vars then defaults will be provided as set at end of variables.tf

(Original README content below)

# Learn Terraform locals

This repo is a companion repo to the [Learn Terraform locals](https://developer.hashicorp.com/terraform/tutorials/configuration-language/locals) tutorial.

Terraform locals allow you to simplify your Terraform configuration and avoid
repetition. Local values can also help you write more readable configuration by
using meaningful names rather than hard-coding values. 

## Terraform Patterns for Well Named Cloud Infrastructure
