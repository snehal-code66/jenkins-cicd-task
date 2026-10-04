# Task 2 — Create a Simple Jenkins Pipeline for CI/CD

## 📌 Objective

The objective of this task was to create a simple **Jenkins CI/CD pipeline** to build, test, and deploy a web application.

## 🛠️ Tools Used

* Jenkins
* Git
* GitHub
* Docker
* Java
* Git Bash

## 🔧 Work Performed

1. Installed and configured Jenkins locally.
2. Created a `Jenkinsfile` in the project repository.
3. Configured the Jenkins pipeline with the following stages:

   * **Build** – Builds the Docker image.
   * **Test** – Verifies the Docker image.
   * **Deploy** – Deploys the application using a Docker container.
4. Connected the Jenkins project with the GitHub repository.
5. Configured the pipeline to detect changes made to the repository.
6. Pushed changes to the `main` branch to test the pipeline.
7. Checked the Jenkins dashboard and verified the pipeline execution.
8. Verified the deployed web application in the browser.

## 📂 Important Files

```text
Dockerfile
Jenkinsfile
index.html
README.md
```

## 🔄 CI/CD Pipeline

```text
GitHub Repository
       ↓
Jenkins Pipeline
       ↓
Build
       ↓
Test
       ↓
Deploy
       ↓
Web Application
```

## ✅ Result

The Jenkins CI/CD pipeline was successfully created and tested. The **Build, Test, and Deploy** stages executed successfully, and the deployed web application was verified through the browser.
