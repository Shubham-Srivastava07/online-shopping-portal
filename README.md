# 🛒 Online Shopping Portal 

A production-style DevOps project demonstrating the complete deployment lifecycle of a React-based Online Shopping Portal.

The application is containerized using Docker with a multi-stage build, orchestrated using Docker Compose, automated through Jenkins CI/CD, and deployed on a Google Cloud Platform (GCP) Virtual Machine using Nginx as the production web server.

The primary objective of this project is to implement modern DevOps practices including containerization, CI/CD automation, cloud deployment, reverse proxy configuration, and production-ready application hosting.

---

# 🚀 Live Demo

### 🌐 Application URL

http://shubham-shop.duckdns.org

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
      Google Cloud Platform VM
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

# ⚙️ Tech Stack

| Category | Technology |
|-----------|------------|
| Frontend | React (Vite) |
| Containerization | Docker |
| Orchestration | Docker Compose |
| CI/CD | Jenkins |
| Web Server | Nginx |
| Cloud Platform | Google Cloud Platform (GCP) |
| Image Registry | Docker Hub |
| DNS | DuckDNS |
| Version Control | Git & GitHub |

---

# 📂 Project Structure

```
.
├── Dockerfile
├── docker-compose.yml
├── Jenkinsfile
├── nginx.conf
├── .dockerignore
├── README.md
├── public/
├── src/
├── package.json
└── package-lock.json
```

# 🐳 Docker Implementation

The application is containerized using a **Multi-Stage Docker Build** to separate the build environment from the production environment.

### Features

- Multi-stage Docker Build
- Production-ready Docker Image
- Lightweight Nginx Runtime Image
- Optimized Build using Vite
- Reduced Final Image Size
- Clean Dockerfile Structure

---

# 📦 Docker Compose

Docker Compose is used to automate the complete deployment process.

### Features

- Build Docker Image
- Create Container
- Automatic Restart Policy
- Container Networking
- One-command Deployment

```bash
docker compose up -d --build
```

# 🔄 Jenkins CI/CD Pipeline

Jenkins is used to automate the complete deployment workflow.

### Pipeline Stages

- Checkout Source Code
- Build Docker Image
- Push Docker Image to Docker Hub
- Deploy using Docker Compose

Pipeline Flow

```
GitHub
   │
   ▼
Checkout
   │
   ▼
Docker Build
   │
   ▼
Docker Hub Push
   │
   ▼
Docker Compose Deployment
```


<img width="1359" height="754" alt="Screenshot (488)" src="https://github.com/user-attachments/assets/c808474e-5b93-4271-8d2c-0ce22d3cbfa9" />

---

# 🐳 Docker Hub

The Docker image is automatically pushed to Docker Hub after a successful Jenkins build.

This enables consistent deployments using versioned container images.


<img width="1368" height="754" alt="Screenshot (489)" src="https://github.com/user-attachments/assets/04cdee62-ccf7-465a-bee7-4fd7a1fc7086" />

---

# 🌐 Nginx Configuration

Nginx is used as the production web server.

### Implemented

- Static File Hosting
- Reverse Proxy Configuration
- SPA Routing using `try_files`
- Production-ready Configuration

The custom **nginx.conf** prevents **404 errors** during page refresh by redirecting unknown routes back to the application entry point.


<img width="1363" height="800" alt="Screenshot (487)" src="https://github.com/user-attachments/assets/534a3663-3613-4f30-a75c-94afd6fde5d8" />

---

# Deployment

The application is deployed on a Google Cloud Platform Virtual Machine.

Deployment includes:

- Docker Installation
- Docker Compose
- Jenkins
- Firewall Configuration
- Public IP Access
- DuckDNS Domain Mapping
- Nginx Deployment

Deployment Flow

```
Browser
     │
     ▼
Local DNS
     │
     ▼
DuckDNS
     │
     ▼
Google Cloud Firewall
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
React Application
```


<img width="1363" height="800" alt="Screenshot (484)" src="https://github.com/user-attachments/assets/72af5234-43cc-42a0-8616-5c216ed82dae" />


---

# 📸 Project Screenshots


<img width="1359" height="800" alt="Screenshot (485)" src="https://github.com/user-attachments/assets/e702481e-e305-45af-8898-13a5b2f97a81" />


<img width="1368" height="800" alt="Screenshot (486)" src="https://github.com/user-attachments/assets/c888a46f-a31b-4896-b81d-5a5be1c209b7" />



---

# 📈 Key DevOps Features

- ✅ Multi-stage Docker Build
- ✅ Docker Compose Deployment
- ✅ Jenkins CI/CD Pipeline
- ✅ Docker Hub Integration
- ✅ Nginx Production Server
- ✅ SPA Routing Configuration
- ✅ Google Cloud VM Deployment
- ✅ DuckDNS Domain Mapping
- ✅ Health Check Configuration
- ✅ Custom Docker Network
- ✅ Production-ready Containerization

---

# 💡 Challenges Faced

During this project, I solved several real-world deployment challenges including:

- Understanding Multi-stage Docker Builds
- Building Production Images using Vite
- Configuring Nginx for SPA Routing
- Mapping DuckDNS with GCP VM
- Configuring Google Cloud Firewall Rules
- Creating an Automated Jenkins CI/CD Pipeline
- Deploying Docker Containers on Cloud Infrastructure

---

# 📚 Learning Outcomes

Through this project, I gained hands-on experience with:

- Docker Image Optimization
- Docker Multi-stage Builds
- Docker Compose
- Jenkins CI/CD
- Nginx Configuration
- Google Cloud Platform
- Docker Hub
- Production Deployment Workflow
- Cloud Networking
- DNS Mapping

---


