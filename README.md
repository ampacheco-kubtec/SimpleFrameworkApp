![Build and Deploy](https://github.com/timheuer/SimpleFrameworkApp/workflows/Build%20and%20Deploy/badge.svg?branch=master)

# SimpleFrameworkApp
Sample repo for showing how to use GitHub Actions for a .NET Framework app.

Blog post: https://timheuer.com/blog/building-net-framework-apps-using-github-actions/

## Steps to Build the Webapp Resource on Azure
```sh
az login
az group create --name devops-rg --location eastus
az configure --defaults group=devops-rg location=eastus
az appservice plan create --name devops-plan --sku F1
az webapp create --name devops-webapp --plan devops-plan
az webapp list
az webapp browse -n devops-webapp
```

## Get Publishing Profile as XML


## Store Publishing Profile as a Secret in Github Repository Settings
