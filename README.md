# 🚀 Cloud Native DevOps Platform

## About this project

This repository is a practical DevOps portfolio project focused on building and managing a cloud-native deployment workflow.

The main goal of this project is to gain practical experience with modern DevOps technologies and approaches:

- Containerization
- Kubernetes orchestration
- Infrastructure as Code
- CI/CD automation
- Monitoring
- GitOps-based deployments

The project was created for educational purposes and represents a production-like environment.

---

# 🏗 Architecture Overview

```
Developer
    |
    v
GitHub Repository
    |
    v
GitHub Actions
    |
    +----------------+
    |                |
    v                v
Terraform          Docker
    |                |
    v                |
AWS Resources       |
                    |
                    v
              Kubernetes Cluster
                    |
        +-----------+-----------+
        |                       |
       Helm                  Argo CD
        |                       |
        +-----------+-----------+
                    |
                    v
              Nginx Application
                    |
                    v
            Prometheus + Grafana
```

---

# 🛠 Technology Stack

## Containerization

- Docker
- Docker Images
- Dockerfile

## Kubernetes

- Kubernetes
- Minikube
- kubectl
- Pods
- Deployments
- ReplicaSets
- Services
- ConfigMaps
- Secrets
- Persistent Volumes (PV)
- Persistent Volume Claims (PVC)
- Ingress Controller
- RBAC

## Package Management

- Helm
- Helm Charts
- Helm Releases
- Helm Upgrade
- Helm Rollback

## Infrastructure as Code

- Terraform
- AWS Provider
- Terraform Modules
- Infrastructure provisioning

## CI/CD

- GitHub Actions
- Docker build workflows
- Kubernetes validation
- Terraform validation

## Monitoring

- Prometheus
- Grafana
- Metrics collection
- Monitoring dashboards

## GitOps

- Argo CD
- Declarative deployments
- Git as a single source of truth
- Automated synchronization
- Self-healing deployments

---

# 📁 Project Structure

```
.
├── .github/
│   └── workflows/
│
├── argocd/
│   ├── applications/
│   │   └── nginx-application.yaml
│   │
│   └── projects/
│       └── devops-lab-project.yaml
│
├── docker/
│   └── nginx/
│       ├── Dockerfile
│       └── index.html
│
├── helm/
│   └── nginx-chart/
│
├── kubernetes/
│
├── monitoring-manual/
│
├── rbac/
│
└── terraform/
    ├── modules/
    ├── main.tf
    ├── providers.tf
    └── variables.tf
```

---

# 🚀 Kubernetes Deployment

Start Minikube:

```bash
minikube start
```

Check cluster:

```bash
kubectl get nodes
```

Check resources:

```bash
kubectl get pods
kubectl get deployments
kubectl get services
kubectl get ingress
kubectl get pvc
```

---

# 📦 Helm Deployment

Helm is used to package and manage Kubernetes applications.

Install application:

```bash
helm install nginx ./helm/nginx-chart
```

Check releases:

```bash
helm list
```

Upgrade:

```bash
helm upgrade nginx ./helm/nginx-chart
```

Rollback:

```bash
helm rollback nginx
```

Remove:

```bash
helm uninstall nginx
```

---

# 🔄 GitOps with Argo CD

Argo CD manages Kubernetes deployments using Git as the source of truth.

Workflow:

```
GitHub Repository
        |
        v
     Argo CD
        |
        v
    Helm Chart
        |
        v
 Kubernetes Cluster
```

Implemented:

- Declarative deployments
- Git-based configuration management
- Automated synchronization
- Self-healing Kubernetes resources

---

# 📊 Monitoring

Monitoring architecture:

```
Application
     |
     v
Prometheus
     |
     v
Grafana Dashboard
```

Implemented:

- Metrics collection
- Kubernetes monitoring
- Visualization dashboards

---

# 🌩 Infrastructure as Code

Terraform manages cloud infrastructure.

Implemented:

- AWS Provider configuration
- Terraform modules
- Network resources
- Compute resources
- Storage resources
- IAM configuration

---

# 🎯 Project Goals

This project demonstrates practical knowledge of:

✅ Kubernetes administration  
✅ Docker containerization  
✅ Helm package management  
✅ GitHub Actions CI/CD  
✅ Terraform Infrastructure as Code  
✅ AWS cloud fundamentals  
✅ Prometheus and Grafana monitoring  
✅ GitOps with Argo CD  

---

# 🇷🇺 Русский

## О проекте

Этот репозиторий — практический DevOps-проект, направленный на создание и управление cloud-native инфраструктурой.

Основная цель проекта — получить практический опыт работы с современными DevOps технологиями:

- контейнеризация
- Kubernetes orchestration
- Infrastructure as Code
- CI/CD автоматизация
- мониторинг
- GitOps подход

Проект создан в учебных целях и представляет собой приближённую к production среду.

---

# Используемые технологии

- Docker
- Kubernetes
- Minikube
- kubectl
- Helm
- Terraform
- AWS
- GitHub Actions
- Prometheus
- Grafana
- Argo CD

---

# Цель проекта

Получить практические навыки:

✅ Kubernetes  
✅ Docker  
✅ Helm  
✅ Terraform  
✅ Cloud Infrastructure  
✅ CI/CD  
✅ Monitoring  
✅ GitOps  

Проект является частью самостоятельного изучения DevOps и Cloud технологий.