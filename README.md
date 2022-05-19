# Project 2:

### Deploy a high-availability web app using CloudFormation

- By:   
    - Robert Kazirut
- Date: 
    - May 2022

## Scenario

Your company is creating an Instagram clone called Udagram. Developers want to deploy a new application to the AWS infrastructure. You have been tasked with provisioning the required infrastructure and deploying a dummy application, along with the necessary supporting software. This needs to be automated so that the infrastructure can be discarded as soon as the testing team finishes their tests and gathers their results.

## Infrastructure Diagram

![Diagram](/diagram/lucid-diagram.png)

## Creation of Infrastructure

Use the appropriate scripts to create, update, or delete infrastructure as needed. See below example for creation of network and server infrasturcture.

### Bash
```
./scripts/bash/create.sh networkInfra ./cloudformation/network.yml ./cloudformation/network-parameters.json
```

```
./scripts/bash/create.sh serverInfra ./cloudformation/server.yml ./cloudformation/server-parameters.json
```

### Powershell
```
./scripts/powershell/create.sh networkInfra ./cloudformation/network.yml ./cloudformation/network-parameters.json
```

```
./scripts/powershell/create.sh serverInfra ./cloudformation/server.yml ./cloudformation/server-parameters.json
```

## Demo of Udagram

![Demo](/output/udagram.png)

[http://rkser-webse-zlcy4ljg3gas-647052830.us-east-1.elb.amazonaws.com/](http://rkser-webse-zlcy4ljg3gas-647052830.us-east-1.elb.amazonaws.com/)