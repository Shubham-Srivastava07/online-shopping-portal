Online Shopping Portal 

A production-style DevOps project demonstrating the complete deployment lifecycle of a React-based Online Shopping Portal.

The application is containerized using Docker with a multi-stage build, orchestrated using Docker Compose, automated through Jenkins CI/CD, and deployed on a Google Cloud Platform (GCP) Virtual Machine with Nginx serving as the web server.

The project demonstrates modern DevOps practices including containerization, CI/CD automation, cloud deployment, Nginx configuration, and automated application hosting.

---

Architecture

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

Tech Stack

| Category | Technology |
|-----------|------------|
| Frontend | React (Vite) |
| Containerization | Docker |
| Container Management | Docker Compose |
| CI/CD | Jenkins |
| Web Server | Nginx |
| Cloud Platform | Google Cloud Platform (GCP) |
| Image Registry | Docker Hub |
| Version Control | Git & GitHub |

---

Project Structure

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

Docker Implementation

The application is containerized using a **Multi-Stage Docker Build** to separate the build environment from the production environment.

Features

- Multi-stage Docker Build
- Optimized Docker Image
- Lightweight Nginx Runtime Image
- Optimized Build using Vite
- Reduced Final Image Size
- Clean Dockerfile Structure

---

Docker Compose

Docker Compose is used to automate the complete deployment process.

Features

- Build Docker Image
- Create Container
- Automatic Restart Policy
- Container Networking
- One-command Deployment

```bash
docker compose up -d --build
```

Jenkins CI/CD Pipeline

Jenkins is used to automate the complete deployment workflow.

Pipeline Stages

- Checkout Source Code
- Build Docker Image
- Push Docker Image to Docker Hub
- Deploy using Docker Compose

Pipeline Flow

```
GitHub Push
   │
   ▼
Webhook Trigger
   │
   ▼
Jenkins
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

Docker Hub

The Docker image is automatically pushed to Docker Hub after a successful Jenkins build.

Docker images are published with Jenkins build-based version tags alongside the latest tag, enabling traceable and consistent deployments.

<img width="1368" height="754" alt="Screenshot (489)" src="https://github.com/user-attachments/assets/04cdee62-ccf7-465a-bee7-4fd7a1fc7086" />

---

Nginx Configuration

Nginx is used as the web server and handles static file serving and SPA routing.

Implemented

- Static File Hosting
- SPA Routing using try_files
- Custom Nginx Configuration

The custom **nginx.conf** prevents **404 errors** during page refresh by redirecting unknown routes back to the application entry point.


<img width="1363" height="800" alt="Screenshot (487)" src="https://github.com/user-attachments/assets/534a3663-3613-4f30-a75c-94afd6fde5d8" />

---

Deployment

The application is deployed on a Google Cloud Platform Virtual Machine with automated deployment through Jenkins and Docker Compose.

Deployment includes:

- Docker Installation
- Docker Compose
- Jenkins
- Firewall Configuration
- Public IP Access
- Nginx Deployment

Deployment Flow

```
Browser
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

Project Screenshots


<img width="1359" height="800" alt="Screenshot (485)" src="https://github.com/user-attachments/assets/e702481e-e305-45af-8898-13a5b2f97a81" />


<img width="1368" height="800" alt="Screenshot (486)" src="https://github.com/user-attachments/assets/c888a46f-a31b-4896-b81d-5a5be1c209b7" />



---

Key DevOps Features

-  Multi-stage Docker Build
-  Docker Compose Deployment
-  Jenkins CI/CD Pipeline
-  Docker Hub Integration
-  Nginx web Server
-  SPA Routing Configuration
-  Google Cloud VM Deployment
-  Health Check Configuration
-  Custom Docker Network
-  Optimized Containerization

---

Challenges Faced

During this project, I solved several real-world deployment challenges including:

- Designing Multi-stage Docker Builds
- Building Production Images using Vite
- Configuring Nginx for SPA Routing
- Configuring Google Cloud Firewall Rules
- Creating an Automated Jenkins CI/CD Pipeline
- Deploying Docker Containers on Cloud Infrastructure

---

Learning Outcomes

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


---



AWS metrics update 10
AWS metrics update 11
AWS metrics update 12
AWS metrics update 13
AWS metrics update 14
AWS metrics update 15
AWS metrics update 16
AWS metrics update 17
AWS metrics update 18
EKS architecture update 05
EKS architecture update 06
EKS architecture update 07
EKS architecture update 08
EKS architecture update 09
EKS architecture update 10
EKS architecture update 11
EKS architecture update 12
Core Infrastructure architecture blueprint update 1 on day 12
Core Infrastructure architecture blueprint update 2 on day 12
Core Infrastructure architecture blueprint update 1 on day 13
Core Infrastructure architecture blueprint update 2 on day 13
Core Infrastructure architecture blueprint update 1 on day 14
Core Infrastructure architecture blueprint update 2 on day 14
Core Infrastructure architecture blueprint update 1 on day 15
Core Infrastructure architecture blueprint update 2 on day 15
Core Infrastructure architecture blueprint update 1 on day 16
Core Infrastructure architecture blueprint update 2 on day 16
Core Infrastructure architecture blueprint update 1 on day 17
Core Infrastructure architecture blueprint update 2 on day 17
Core Infrastructure architecture blueprint update 1 on day 18
Core Infrastructure architecture blueprint update 2 on day 18
Staging optimization logs update 1 on day 22
Staging optimization logs update 2 on day 22
Staging optimization logs update 1 on day 23
Staging optimization logs update 2 on day 23
Staging optimization logs update 1 on day 24
Staging optimization logs update 2 on day 24
Staging optimization logs update 1 on day 25
Staging optimization logs update 2 on day 25
Application component refactoring logs 1 on day 14
Application component refactoring logs 2 on day 14
Application component refactoring logs 1 on day 15
Application component refactoring logs 2 on day 15
Jenkins workflow and staging configuration update 1 on day 12
Jenkins workflow and staging configuration update 2 on day 12
Jenkins workflow and staging configuration update 1 on day 13
Jenkins workflow and staging configuration update 2 on day 13
Jenkins workflow and staging configuration update 1 on day 14
Jenkins workflow and staging configuration update 2 on day 14
Jenkins workflow and staging configuration update 1 on day 15
Jenkins workflow and staging configuration update 2 on day 15
Docker layer optimization logs update 1 on day 28
Docker layer optimization logs update 2 on day 28
Docker layer optimization logs update 1 on day 29
Docker layer optimization logs update 2 on day 29
Docker layer optimization logs update 1 on day 30
Docker layer optimization logs update 2 on day 30
Nginx proxy configuration polish update 1 on day 12
Nginx proxy configuration polish update 2 on day 12
Nginx proxy configuration polish update 1 on day 13
Nginx proxy configuration polish update 2 on day 13
Nginx proxy configuration polish update 1 on day 14
Nginx proxy configuration polish update 2 on day 14
Nginx proxy configuration polish update 1 on day 15
Nginx proxy configuration polish update 2 on day 15
Nginx proxy configuration polish update 1 on day 16
Nginx proxy configuration polish update 2 on day 16
AWS architecture initial draft 1 on day 14
AWS architecture initial draft 2 on day 14
AWS architecture initial draft 1 on day 15
AWS architecture initial draft 2 on day 15
CloudWatch dashboard metrics integration 1 on day 22
CloudWatch dashboard metrics integration 2 on day 22
CloudWatch dashboard metrics integration 1 on day 23
CloudWatch dashboard metrics integration 2 on day 23
CloudWatch dashboard metrics integration 1 on day 24
CloudWatch dashboard metrics integration 2 on day 24
CloudWatch dashboard metrics integration 1 on day 25
CloudWatch dashboard metrics integration 2 on day 25
EKS routing and service maps update 1 on day 14
EKS routing and service maps update 2 on day 14
EKS routing and service maps update 1 on day 15
EKS routing and service maps update 2 on day 15
EKS routing and service maps update 1 on day 16
EKS routing and service maps update 2 on day 16
EKS routing and service maps update 1 on day 17
EKS routing and service maps update 2 on day 17
EKS routing and service maps update 1 on day 18
EKS routing and service maps update 2 on day 18
Production optimization review log 1 on day 07
Production optimization review log 2 on day 07
Production optimization review log 1 on day 08
Production optimization review log 2 on day 08
