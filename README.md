# Phoenix Application Problem - Solution 

This is my AWS implementation of required infrastructure to solve Phoenix Application Problem.
Original GitHub repo is [here](https://github.com/claranet-coast/cloud-phoenix-kata)

## Problem Summary

The development team has released the phoenix application code.
Your task is to create the production infrastructure
for the Phoenix application.

1. Automate the creation of the infrastructure and the setup of the application.
2. Recover from crashes. Implement an autorestart mechanism.
3. Backup the logs and database with a rotation of 7 days
4. Notify any CPU peak
5. Implements a CI/CD pipeline for the code
6. Scale when the number of requests is greater than 10 req /sec

# Infrastructure Overview

Infrastructure is hosted by AWS. CloudFormation templates are provided in order to build infrastructure and automatic CI/CD pipeline. 

![Architecture](aws/Phoenix-App-Layout.png)
