![CI/CD Pipeline](https://github.com/shashimpally/ci-cd-github-actions-docker/actions/workflows/ci-cd.yml/badge.svg)


#  CI/CD Pipeline with GitHub Actions & Docker

This is a real-time DevOps project that demonstrates how to set up a full *CI/CD pipeline* using *GitHub Actions, **Docker, and **Localhost* (for localhost:4000 deployment). No cloud is needed — everything runs locally.

---

##  Project Objective

The main goal of this project is to:

- Automate the process of building and testing code using GitHub Actions.
- Create a Docker image and push it to Docker Hub.
- Pull the Docker image and deploy it using Localhost (browser).

This setup mimics how real-world CI/CD pipelines work — just without relying on any cloud infrastructure.

---

## 🛠 Tools & Technologies Used

| Tool/Technology    | Purpose                                           |
|--------------------|--------------------------------------------------|
| *GitHub Actions* | Automate build, test, and Docker deployment      |
| *Docker*         | Containerize the Node.js app                     |
| *Docker Hub*     | Host and pull the Docker image                   |
| *Localhost*       | Run localhost 4000                              |
| *Node.js + Express* | Build a simple backend server app              |

---

## 📁 Project Folder Structure



ci-cd-github-actions-docker/
├── .github/workflows/ci-cd.yml   # GitHub Actions workflow
├── Screenshots
         ├──  Ci-cd pipeline working.png
         └── workflow.png
         └──Ci-Cd all Working flow.png
├── docker/Dockerfile             # Dockerfile for the Node.js app
├── k8s/
│   ├── deployment.yaml           # Kubernetes Deployment manifest
│   └── service.yaml              # Kubernetes Service manifest
├── src/
│   └── server.js                 # Node.js backend code
├── README.md                     # You're reading it!
├── REPORT.pdf                    # Final 2-page report
├── screenshots/                  # Output images of CI/CD flow
│   ├── GitHub-repo-with-workflows.png
│   ├── Docker image link.png
│   ├── CI/CD workflow results.png 
    └── Screenshots of the deployed app.pngs

`

---

## ⚙ How the CI/CD Workflow Works

### 🔹 1. Code Push to GitHub
Triggers the GitHub Actions workflow.

### 🔹 2. GitHub Actions (ci-cd.yml)
- ✅ Checkout code
- ✅ Login to Docker Hub (using secrets)
- ✅ Build Docker image
- ✅ Push image to Docker Hub

### 🔹 3. Local Deployment with localhost:4000
- Pull image from Docker Hub
- Run and expose the app localhost

---

## 🐳 Docker Hub Image

Pull the Docker image from my Docker Hub account:

bash
docker pull shashikumar02/ci-cd-demo:latest


---

## 📷 Screenshots

| Screenshot             | Description                     |
| ---------------------- | ------------------------------- |
| GitHub repo with workflows.png | GitHub Actions pipeline success |
| Docker image link.png | Docker image |
| CI/CD workflow results.png   | ci-cd working in browser|
| Screenshots of the deployed app.pngs  | Deployed app |deployed Healthy | Deployed api users |

Screenshots are available in the Screenshots /Folder

---

## ✅ Result

* Fully automated CI/CD pipeline without using cloud.
* Code tested, built into Docker image, and pushed to Docker Hub.
* Image deployed locally using Kubernetes (Minikube).
