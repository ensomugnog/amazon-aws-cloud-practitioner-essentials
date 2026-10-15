# AACPE - Amazon AWS Cloud Practitioner Essentials

In a digital-first world, cloud knowledge is a career advantage. This refreshed course takes you through the fundamentals of AWS—services, pricing, security, monitoring, and architecture—so you can confidently step into cloud, lead technical teams, or expand your expertise. Stay relevant. Stay current. Start with AWS.

**Course**: [https://skillbuilder.aws/learn/94T2BEN85A/aws-cloud-practitioner-essentials/8D79F3AVR7](https://skillbuilder.aws/learn/94T2BEN85A/aws-cloud-practitioner-essentials/8D79F3AVR7)

## Course Progress: 30%

- [x] 00 - How to Use Each Module

- [x] 01 - Module 1: Introduction to the Cloud
  
  - [x] 01.01 - How to Use Each Module

  - [x] 01.02 - Module 1 Introduction
  
    - [x] 01.02.01 - Welcome to AWS Cloud Practitioner Essentials
  
  - [x] 01.03 - The AWS Cloud
    
    - [x] 01.03.01 - What is Cloud Computing?
    
    - [x] 01.03.02 - Benefits of the AWS Cloud
    
    - [x] 01.03.03 - Introduction to AWS Global Infrastructure
    
    - [x] 01.03.04 - The AWS Shared Responsibility Model
  
  - [x] 01.04 - Cloud in Real Life
  
    - [x] 01.04.01 - Applying Cloud Concepts to Real Life Use Cases
  
  - [x] 01.05 - Module 1 Conclusion

    - [x] 01.05.01 - Assessment

    - [x] 01.05.02 - Module Summary

- [x] 02 - Module 2 - Compute in the Cloud

  - [x] 02.01 - Module 2 Introduction
  
    - [x] 02.01.01 - Introduction to Amazon EC2
    
  - [x] 02.02 - Compute in the Cloud
  
    - [x] 02.02.01 - Amazon EC2 Instance Types
    
    - [x] 02.02.02 - How to Provision AWS Resources
    
    - [x] 02.02.03 - Demo: Launching an Amazon EC2 Instance
    
    - [x] 02.02.04 - Amazon EC2 Pricing
  
  - [x] 02.03 - Auto Scaling and Load Balancing
  
    - [x] 02.03.01 - Scaling Amazon EC2
    
    - [x] 02.03.02 - Directing Traffic with Elastic Load Balancing
    
    - [x] 02.03.03 - Messaging and Queuing
  
  - [x] 02.04 - Module 2 Conclusion
  
    - [x] 02.04.01 - Assessment
    
    - [x] 02.04.02 - Module Summary

- [x] 03 - Module 3: Exploring Compute Services

  - [x] 03.01 - Module 3 Introduction
  
    - [x] 03.01.01 - Introduction to Serverless Computing

  - [x] 03.02 - AWS Serverless, Containers, and Solutions Overview
  
    - [x] 03.02.01 - AWS Lambda
    
    - [x] 03.02.02 - Containers and Orchestration on AWS
    
    - [x] 03.02.03 - Additional Compute Services
  
  - [x] 03.03 - Module 3 Conclusion
    
    - [x] 03.03.01 - Assessment
    
    - [x] 03.03.02 - Module Summary

- [x] 04 - Module 4 - Going Global
  
  - [x] 04.01 - Module 4 Introduction
  
    - [x] 04.01.01 - Introduction to Going Global
  
  - [x] 04.02 - AWS Global Infrastructure
  
    - [x] 04.02.01 - Choosing AWS Regions
    
    - [x] 04.02.02 - Diving Deeper into AWS Global Infrastructure
    
    - [x] 04.02.03 - Infrastructure and Automation
  
  - [x] 04.03 - Module 4 Conclusion
  
    - [x] 04.03.01 - Assessment
  
    - [x] 04.03.02 - Module Summary

- [x] 05 - Module 5 - Networking

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