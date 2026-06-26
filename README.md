# 🛒 Online Shopping Portal - DevOps Deployment Project

## 📌 Project Overview

This project demonstrates the end-to-end deployment of a React-based Online Shopping Portal using modern DevOps practices.

The frontend application is containerized using Docker, orchestrated with Docker Compose, integrated with Jenkins for Continuous Integration and Continuous Deployment (CI/CD), and deployed on a Google Cloud Platform (GCP) Virtual Machine using Nginx.

This repository focuses on implementing production-style DevOps workflows rather than developing new application features.

---

# 🚀 Live Demo

**Application URL**

```
http://shubham-shop.duckdns.org
```

---

# 🏗️ Architecture

```
Developer
     │
     ▼
 GitHub Repository
     │
     ▼
 Jenkins Pipeline
     │
     ├── Checkout Source Code
     ├── Build Docker Image
     ├── Push Image to Docker Hub
     └── Deploy using Docker Compose
               │
               ▼
        Google Cloud VM
               │
               ▼
        Docker Container
               │
               ▼
            Nginx
               │
               ▼
     Online Shopping Portal
```

---

# ⚙️ Tech Stack

* React (Vite)
* Docker
* Docker Compose
* Jenkins
* Nginx
* Google Cloud Platform (GCP)
* Docker Hub
* Git & GitHub
* DuckDNS

---

# 📂 Project Structure

```
.
├── Dockerfile
├── docker-compose.yml
├── Jenkinsfile
├── nginx.conf
├── README.md
├── src/
├── public/
└── package.json
```

---

# 🐳 Docker Implementation

* Multi-stage Docker Build
* Lightweight Nginx Production Image
* Optimized Image Size
* Production Build using Vite

---

# 📦 Docker Compose

Docker Compose is used to

* Build the application
* Manage containers
* Configure networking
* Restart containers automatically
* Simplify deployment using a single command

---

# 🔄 Jenkins CI/CD Pipeline

Pipeline Stages

* Checkout Source Code
* Build Docker Image
* Push Docker Image to Docker Hub
* Deploy using Docker Compose

This enables automated application deployment from GitHub to the target server.

---

# 🌐 Nginx Configuration

Nginx is used as the production web server.

Implemented:

* Static file hosting
* SPA Routing using `try_files`
* Production-ready container deployment

---

# ☁️ Google Cloud Deployment

The application is deployed on a Google Cloud Platform VM.

Deployment includes:

* Docker installation
* Docker Compose
* Jenkins
* Firewall configuration
* Public IP access
* DuckDNS domain mapping

---

# 📸 Screenshots

> Screenshots will be added.

* Home Page
* Docker Containers
* Jenkins Successful Pipeline
* Docker Hub Repository
* GCP VM
* Live Website

---

# 📈 Key DevOps Features

* Multi-stage Docker Build
* Docker Compose Deployment
* Jenkins CI/CD Pipeline
* Docker Hub Integration
* GCP Deployment
* DuckDNS Domain Mapping
* Nginx Production Server
* SPA Routing Configuration

---

# 🛠️ Future Improvements

* HTTPS using Let's Encrypt
* Reverse Proxy Configuration
* Kubernetes Deployment
* GitHub Webhooks
* GitOps Deployment using ArgoCD

---

# 🙏 Acknowledgements

The frontend application used in this repository is based on a learning project created during the **Train With Shubham** program.

The DevOps implementation, containerization, CI/CD pipeline, deployment workflow, project restructuring, and documentation have been independently implemented by **Shubham Srivastava** for learning and portfolio purposes.

---



