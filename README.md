## DevOps Internship Task 1 - CI/CD Pipeline using GitHub Actions and Docker
## Task Title : Automate Code Deployment Using CI/CD Pipeline (GitHub Actions)

## Objective :
The objective of this task is to create a CI/CD pipeline that automatically builds and deploys a Node.js application using GitHub Actions and Docker.

## Tools Used :
* GitHub
* GitHub Actions
* Node.js
* Docker
* Docker Hub
* Visual Studio Code

## Project Description
A simple Node.js web application was created using Express.js.
The CI/CD pipeline was configured using GitHub Actions. Whenever code is pushed to the `main` branch, the workflow automatically:
1. Checks out the source code
2. Installs Node.js dependencies
3. Runs the build/test process
4. Logs in to Docker Hub
5. Builds a Docker image
6. Pushes the image to Docker Hub

## Project Structure
```text
.github/workflows/main.yml
Dockerfile
server.js
package.json
README.md
```
## Running the Application Locally
Install dependencies:
```bash
npm install
```
Start the application:
```bash
npm start
```
Open:
```text
http://localhost:3000
```
## Docker Commands
Build image:
```bash
docker build -t nodejs-demo-app .
```
Run container:
```bash
docker run -p 3000:3000 nodejs-demo-app
```
## GitHub Actions Workflow
Workflow file location:
```text
.github/workflows/main.yml
```
Trigger:
```yaml
on:
  push:
    branches:
      - main
```

## Screenshots Included
* Application running locally
* Successful GitHub Actions workflow
* Docker Hub repository/image
* vs code project structure

## Learning Outcomes
Through this task I learned:
* CI/CD concepts
* GitHub Actions workflow creation
* Docker containerization
* Docker image deployment
* GitHub Secrets management
* Automated software delivery pipelines

## Repository Link



## Docker Hub Link



## Conclusion

This project successfully demonstrates an automated CI/CD pipeline using GitHub Actions and Docker for a Node.js application.
