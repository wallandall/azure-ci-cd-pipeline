# azure-ci-cd-pipeline
# Overview
This project demponstrates the steps on how to build a CI/CD pipeline using Azure Devops and Github to deploy a Pyhon Machine Learning Application to Azure App Services
Technolog

[![Python application test with Github Actions](https://github.com/wallandall/azure-ci-cd-pipeline/actions/workflows/pythonapp.yml/badge.svg)](https://github.com/wallandall/azure-ci-cd-pipeline/actions/workflows/pythonapp.yml)


## Project Plan
Click on the below links to view the Trello Board and Project Plan

* [Trello board](https://trello.com/b/DKIrIpDZ/deploy-cicd-pipeline-in-azure)
* [Project Plan](https://docs.google.com/spreadsheets/d/1X-_tgCsTntOpF15eZHiBT_9kV8qnpq180sBZ4QrkGVM/edit#gid=1348135932)

## Instructions


### Architectural Diagram
  
![alt text](https://github.com/wallandall/azure-ci-cd-pipeline/blob/main/images/architecture.png "Architecture Diagram")

This project uses a number of technologies as well as the following platforms to implement a CI/CD Pipeline [Azure](https://portal.azure.com), [Azure DevOps](https://dev.azure.com) and [GitHub](https://github.com), therefore the relevant accounts are required. The below steps detail the steps for implementing a CD/CD Pipeline, Configuring our Python Machine Leaarning Application and Deployment to Azure App Services:

## Development Environment
For our development environment we will use Azure Shell and push our code to a GitHub repository. To implement this the following steps need to be performed:

![alt text](https://github.com/wallandall/azure-ci-cd-pipeline/blob/main/images/cloud-dev.png "Development Environment")


1. Log into Azure Portal and access the cloud shell as per the below image


   ![alt text](https://github.com/wallandall/azure-ci-cd-pipeline/blob/main/images/cloud-shell.png "Cloud Shell")


2. Generate an SSH Key by running the following command from the Azure Cloud Shell : ``` ssh-keygen -t rsa ```. The passphrase blank.


   ![alt text](https://github.com/wallandall/azure-ci-cd-pipeline/blob/main/images/ssh-key-gen.png "Generate SSH Key")


3. Once the Key has been generated run the following command from the Cloud Shell: ``` cat ~/.ssh/id_rsa.pub ```
4. 

* Project running on Azure App Service

* Project cloned into Azure Cloud Shell

* Passing tests that are displayed after running the `make all` command from the `Makefile`

* Output of a test run

* Successful deploy of the project in Azure Pipelines.  [Note the official documentation should be referred to and double checked as you setup CI/CD](https://docs.microsoft.com/en-us/azure/devops/pipelines/ecosystems/python-webapp?view=azure-devops).

* Running Azure App Service from Azure Pipelines automatic deployment

* Successful prediction from deployed flask app in Azure Cloud Shell.  [Use this file as a template for the deployed prediction](https://github.com/udacity/nd082-Azure-Cloud-DevOps-Starter-Code/blob/master/C2-AgileDevelopmentwithAzure/project/starter_files/flask-sklearn/make_predict_azure_app.sh).
The output should look similar to this:

```bash
udacity@Azure:~$ ./make_predict_azure_app.sh
Port: 443
{"prediction":[20.35373177134412]}
```

* Output of streamed log files from deployed application

> 

## Enhancements

<TODO: A short description of how to improve the project in the future>

## Demo 

<TODO: Add link Screencast on YouTube>
