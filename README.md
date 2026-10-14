# 🚀 DevOps Project Templates

A collection of **production-ready DevOps & Cloud project templates** designed for  
**DevOps Engineers, Cloud Engineers, and Platform Engineers**.

This repository is a **GitHub Template Repository** — use it to quickly bootstrap real-world DevOps projects with best practices.

---
# 🎥 StreamHive - Distributed Video Streaming Platform (YouTube Clone)

> A scalable, YouTube-like video platform built with Next.js 14, Go, HLS streaming, and Polyglot Persistence.

![Next.js](https://img.shields.io/badge/Next.js-14-black)
![Go](https://img.shields.io/badge/Go-1.22-blue)
![FFmpeg](https://img.shields.io/badge/FFmpeg-HLS-green)
![Kafka](https://img.shields.io/badge/Kafka-Upstash-orange)

## ⚡ Architecture Overview

```mermaid
graph TD
    A[User Upload] --> B[Go Backend - Gin]
    B --> C[FFmpeg Worker - Goroutine]
    C --> D[HLS.ts +.m3u8]
    D --> E[MinIO / AWS S3]
    E --> F[Kafka Event]
    F --> G[PostgreSQL + TimescaleDB]
    F --> H[MongoDB Atlas]
    H --> I[Next.js 14 Frontend + Video.js]

---

## 🎯 Purpose

This repo helps you:
- Start DevOps projects **faster**
- Follow **industry-standard folder structures**
- Practice **real-world DevOps workflows**
- Build **portfolio-ready projects**
- Prepare for **DevOps / Cloud interviews**

---

## 🧩 What’s Included

- ✅ Docker & Docker Compose templates  
- ✅ CI/CD pipelines (GitHub Actions)  
- ✅ Kubernetes manifests  
- ✅ Terraform infrastructure templates  
- ✅ Helm charts  
- ✅ Monitoring & logging setup  
- ✅ Security & scanning examples  
- ✅ Documentation templates  

---

## 📁 Repository Structure

```text
devops-project-templates/
├── templates/
│   ├── docker-only/
│   ├── ci-cd-github-actions/
│   ├── kubernetes-app/
│   ├── terraform-aws-infra/
│   └── full-devops-pipeline/
├── .github/
│   └── workflows/
├── scripts/
├── docs/
└── README.md
```

---

## 🚀 Quick Start

### Option 1: Use GitHub Template (Recommended)
1. Click **"Use this template"** button at the top
2. Create a new repository
3. Choose a template folder
4. Customize variables & configs
5. Deploy 🚀

### Option 2: Clone Repository
```bash
git clone https://github.com/NotHarshhaa/devops-project-templates.git
cd devops-project-templates

# Run setup script
chmod +x scripts/setup.sh
./scripts/setup.sh
```

---

## 📋 Template Overview

### 🐳 Docker-Only Template
**Perfect for:** Simple containerized applications
- Multi-stage Dockerfile with security best practices
- Docker Compose with development and production configs
- Nginx reverse proxy configuration
- Health checks and monitoring setup

**Quick Start:**
```bash
cd templates/docker-only
docker-compose up -d
```

### 🔄 CI/CD GitHub Actions Template
**Perfect for:** Automated testing and deployment
- Complete CI pipeline (lint, test, security scan, build)
- CD pipeline with multi-environment deployment
- Blue-green deployment strategy
- Automated cleanup and maintenance

**Features:**
- Parallel test execution
- Docker image building and pushing
- Security vulnerability scanning
- Slack/email notifications
- Rollback capabilities

### ☸️ Kubernetes Application Template
**Perfect for:** Container orchestration
- Production-ready Kubernetes manifests
- Helm charts for templated deployments
- Horizontal Pod Autoscaling
- Service monitoring with Prometheus
- Ingress configuration with TLS
te subnets
- Emi
