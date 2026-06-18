# 🚀 AWS DevOps Platform

A complete end-to-end DevOps project demonstrating Infrastructure as Code (IaC), Containerization, Kubernetes Deployment, and Continuous Integration/Continuous Deployment (CI/CD) on AWS.

![AWS](https://img.shields.io/badge/AWS-Cloud-orange)
![Terraform](https://img.shields.io/badge/Terraform-IaC-purple)
![Docker](https://img.shields.io/badge/Docker-Containerization-blue)
![Kubernetes](https://img.shields.io/badge/Kubernetes-K3s-326CE5)
![GitHub Actions](https://img.shields.io/badge/GitHub_Actions-CI/CD-black)
![Status](https://img.shields.io/badge/Status-Active-success)

---

# 📌 Project Overview

This project automates the deployment of a containerized web application on AWS using modern DevOps practices.

The complete workflow includes:

- Infrastructure provisioning using Terraform
- EC2 instance deployment on AWS
- Docker image creation and management
- Docker Hub image registry integration
- Kubernetes (K3s) deployment
- GitHub Actions based CI/CD pipeline
- Automated application updates through Git push

---

# 🏗️ Architecture

```text
Developer
    │
    ▼
GitHub Repository
    │
    ▼
GitHub Actions CI/CD
    │
    ├── Build Docker Image
    ├── Push Image to Docker Hub
    └── Deploy to Kubernetes
                │
                ▼
          AWS EC2 Instance
                │
                ▼
            K3s Cluster
                │
                ▼
        Containerized Web App
```

---

# ⚙️ Tech Stack

| Category | Technology |
|-----------|------------|
| Cloud | AWS EC2 |
| IaC | Terraform |
| Containerization | Docker |
| Container Registry | Docker Hub |
| Orchestration | Kubernetes (K3s) |
| CI/CD | GitHub Actions |
| Version Control | Git & GitHub |
| Operating System | Ubuntu Server |
| Web Server | Nginx |

---

# 📂 Project Structure

```text
aws-devops-platform/
│
├── .github/
│   └── workflows/
│       └── ci-cd.yml
│
├── app/
│   ├── Dockerfile
│   └── index.html
│
├── kubernetes/
│   ├── deployment.yaml
│   └── service.yaml
│
├── terraform/
│   ├── provider.tf
│   ├── variables.tf
│   ├── outputs.tf
│   └── main.tf
│
├── .gitignore
└── README.md
```

---

# 🚀 Infrastructure Provisioning

Infrastructure is provisioned using Terraform.

### Resources Created

- AWS EC2 Instance
- Security Group
- Public Networking Configuration

### Terraform Commands

```bash
terraform init
terraform validate
terraform plan
terraform apply
```

---

# 🐳 Docker Implementation

The application is containerized using Docker.

### Build Image

```bash
docker build -t puneet8580/devops-app-123:latest ./app
```

### Push Image

```bash
docker push puneet8580/devops-app-123:latest
```

---

# ☸️ Kubernetes Deployment

K3s lightweight Kubernetes cluster is used for deployment.

### Deployment

```bash
kubectl apply -f deployment.yaml
```

### Service

```bash
kubectl apply -f service.yaml
```

### Verify

```bash
kubectl get deployments
kubectl get pods
kubectl get svc
```

---

# 🔄 CI/CD Pipeline

GitHub Actions automates the complete deployment process.

### Pipeline Workflow

```text
Git Push
   │
   ▼
GitHub Actions
   │
   ├── Checkout Source Code
   ├── Docker Build
   ├── Docker Push
   ├── Connect to EC2 via SSH
   └── Restart Kubernetes Deployment
            │
            ▼
       Updated Application
```

### Trigger

Pipeline automatically runs on:

```text
Push to Main Branch
```

---

# 📸 Screenshots

## AWS EC2 Instance

_Add Screenshot Here_

---

## Terraform Infrastructure State

_Add Screenshot Here_

---

## Docker Image Build

_Add Screenshot Here_

---

## Kubernetes Deployment

_Add Screenshot Here_

---

## Application Running

_Add Screenshot Here_

---

## GitHub Actions Success

_Add Screenshot Here_

---

# 🎯 Key Features

✅ Infrastructure as Code (Terraform)

✅ Automated AWS Provisioning

✅ Dockerized Application

✅ Kubernetes Deployment using K3s

✅ Docker Hub Integration

✅ GitHub Actions CI/CD

✅ Automated Deployment Workflow

✅ Production-Oriented DevOps Practices

---

# 📊 Project Workflow

```text
Terraform
    │
    ▼
AWS EC2
    │
    ▼
Docker Build
    │
    ▼
Docker Hub
    │
    ▼
K3s Kubernetes
    │
    ▼
Application Deployment
    │
    ▼
GitHub Actions CI/CD
```

---

# 🧠 Learning Outcomes

Through this project I gained hands-on experience with:

- Infrastructure as Code (IaC)
- AWS Cloud Deployment
- Docker Containerization
- Kubernetes Workloads
- CI/CD Pipeline Automation
- GitHub Actions
- Linux Administration
- DevOps Workflow Design

---

# 👨‍💻 Author

**Punnet Choudhary**

GitHub: :contentReference[oaicite:0]{index=0}

---

# ⭐ Support

If you found this project useful, consider giving it a ⭐ on GitHub.

It helps others discover the project and supports future improvements.

---

## 🚀 DevOps | Cloud | Kubernetes | Terraform | AWS | CI/CD
