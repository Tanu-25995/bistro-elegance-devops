# CI/CD Pipeline for Static Website Deployment

## 📌 Project Overview
This project demonstrates a complete CI/CD pipeline to deploy a static website (Tooplate "Bistro Elegance" template) using Jenkins and Docker on AWS EC2.

Whenever code is pushed to GitHub, Jenkins automatically:
- Pulls the latest code
- Builds a Docker image
- Redeploys the container on EC2

## 🛠️ Tech Stack
- GitHub (Source Code Management)
- Jenkins (CI/CD)
- Docker (Containerization)
- Nginx (Web Server)
- AWS EC2 (Hosting)
- Linux (Ubuntu)

## ⚙️ Pipeline Stages
1. **Checkout** – Jenkins pulls code from GitHub  
2. **Build** – Jenkins builds a Docker image using Dockerfile  
3. **Deploy** – Old container is removed and a new container is started  

## 🚀 How to Access the Website
Open in browser:
http://your-ec2-public-ip

## 📂 Project Structure
- index.html
- css/
- js/
- images/
- Dockerfile
- Jenkinsfile

## ✅ Features
- Automated build and deployment using Jenkins
- Dockerized static website using Nginx
- GitHub webhook for auto-triggering pipeline
- Visual pipeline using Jenkins Blue Ocean / Stage View
