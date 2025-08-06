# jenkins-ci-cd-pipeline
# Task: Jenkins CI/CD Pipeline

## 📌 Objective

Set up a basic Jenkins pipeline to automate the process of building and deploying an application.

---

## 🛠 Tools & Technologies Used

- Jenkins (Pipeline as Code)
- GitHub (with HTTPS and Personal Access Token)
- Docker
- Node.js
- Git (Windows)

---

## 📁 Folder Contents

- `Jenkinsfile` – Jenkins pipeline script for CI/CD
- `Dockerfile` – Docker instructions to build the app
- `app.js` – Basic Node.js application
- `package.json` – Project dependencies
- `test/basic.test.js` – Sample test case
- `README.md` – This file

---

## 🚀 What I Did

1. Set up Jenkins on Windows (installed plugins, created a pipeline job).
2. Created a GitHub repo and pushed project files.
3. Configured GitHub token in Jenkins (used HTTPS, not SSH).
4. Wrote a `Jenkinsfile` to define the build, test, and deploy stages.
5. Connected the repo with Jenkins using "Pipeline script from SCM".
6. Verified automatic pipeline trigger on GitHub push.
7. Successfully deployed the Node.js app using Docker.

---

## 🔧 How to Run

### Clone the Repo

```bash
git clone https://github.com/your-username/jenkins-ci-cd-pipeline.git
cd jenkins-ci-cd-pipeline
----------

##  Build Docker Image
docker build -t node-webapp

--------------

##   Run the App
docker run -d -p 3000:3000 node-webapp.

