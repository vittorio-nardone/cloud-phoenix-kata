# Phoenix Application Problem
This problem is about to create a production ready infrastructure for the Phoenix Application.

## Problem

The development team has released the phoenix application code.
Your task is to create the production infrastructure
for the Phoenix application.
The application has two particularly troubling endpoints:

- `GET /crash` kill the application process
- `GET /generatecert` is not optimized and creates resource consumption peaks

You can't block those endpoints because the universe really wants them to be exposed but at the same time 
you need to guarantee that the application is always available.

## General Requirements

- You may use whatever programming language/platform you prefer. Use something that you know well.
- You must release your work with an OSI-approved open source license of your choice.
- You must deliver the sources, with a README that explains how to run it.
- Add the code to your own Github/GitLab/.. account and send us the link.

## Application Requirements

- Runs on Node.js 8.11.1 LTS
- MongoDB as Database
- Environment variables:
    - PORT - Application HTTP Exposed Port
    - DB_CONNECTION_STRING - Database connection string `mongodb://[username:password@]host1[:port1][,host2[:port2],...[,hostN[:portN]]][/[database][?options]]`

## Run Application
- Install dependencies `npm install`
- Run `npm start`
- Connect to `http://<hostname|IP>:<ENV.PORT>`

## Problem Requirements

1. Automate the creation of the infrastructure and the setup of the application.
2. Recover from crashes. Implement an autorestart mechanism.
3. Backup the logs and database with a rotation of 7 days
4. Notify any CPU peak
5. Implements a CI/CD pipeline for the code
6. Scale when the number of requests is greater than 10 req /sec
