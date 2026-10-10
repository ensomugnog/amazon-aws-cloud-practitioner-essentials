# AACPE - Amazon AWS Cloud Practitioner Essentials

In a digital-first world, cloud knowledge is a career advantage. This refreshed course takes you through the fundamentals of AWS—services, pricing, security, monitoring, and architecture—so you can confidently step into cloud, lead technical teams, or expand your expertise. Stay relevant. Stay current. Start with AWS.

**Course**: [https://skillbuilder.aws/learn/94T2BEN85A/aws-cloud-practitioner-essentials/8D79F3AVR7](https://skillbuilder.aws/learn/94T2BEN85A/aws-cloud-practitioner-essentials/8D79F3AVR7)

## Course Progress: 0%

- [x] 01 - How to Use Each Module

- [x] 02 - Module 1: Introduction to the Cloud
  
  - [x] 02.01 - How to Use Each Module

## Course content

## Repository configuration

Each submodule in this repository contains the code examples of the original course.

### Create new submodules

Create a new repository on Github, then execute the following commands to link the new repository as a submodule of the main repository:

```
$ cd amazon-aws-cloud-practitioner-essentials
$ git submodule add -b main git@github.com:ensomugnog/aacpe-submodule
```

Using the **-b** argument means we want to follow the main branch of the new repository, and after running this command we’ll have a new directory named `aacpe-submodule/`, this directory will automaticaly checkout the main branch for you to be ready to make changes.

### Update main repository with latest submodule changes

First make sure the submodule changes have been commited and pushed to the orign repository, then run the following commands:

```
$ git status
$ git stage .
$ git commit -m 'aacpe-submodule'
$ git push
```

### Clone Repository with submodules

If you want to clone a repository including its submodules you can use the --recursive parameter, use the --jobs parameter to fetch multiple submodules at the same time, download up to 8 submodules at once use --jobs 8

```
$ git clone --recursive --jobs 8 git@github.com:ensomugnog/amazon-aws-cloud-practitioner-essentials.git
```

### Delete a submodule from a repository

Currently Git provides no standard interface to delete a submodule. To remove a submodule `aacpe-submodule` you need to:

```
$ git submodule deinit -f aacpe-submodule
$ rm -rf .git/modules/aacpe-submodule
$ git rm -f aacpe-submodule
```

### Checkout a commit

To checkout a Git commit, you will need the commit hash.

```
$ git checkout 4aa03973d004286558465a8d86bcccfdc7b46505
$ git reset --hard
$ git checkout main
```