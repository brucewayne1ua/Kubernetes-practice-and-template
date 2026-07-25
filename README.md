# 🚀 Kubernetes Practice Project

## 🇬🇧 English

## About this project

This repository is a practical Kubernetes learning project.

The project was created **only for educational purposes** and is not a production application.

The main goal of this project is to gain practical experience with Kubernetes, Docker, Helm and DevOps workflows.

During this project the following technologies and concepts were practiced:

- Kubernetes cluster management
- Pods
- Deployments
- ReplicaSets
- Services
- ConfigMaps
- Secrets
- Persistent Volumes (PV)
- Persistent Volume Claims (PVC)
- Ingress Controller
- Helm Charts
- Helm Releases
- Helm Upgrade and Rollback
- Docker containers
- Local Kubernetes development using Minikube


---

# 🛠 Technology Stack

- Docker
- Docker Desktop
- Kubernetes
- Minikube
- kubectl
- Helm
- Nginx


---

# 📁 Project Structure

```
kubernetes-practice/

│
├── kubectl/
│   ├── deployment.yaml
│   ├── service.yaml
│   ├── ingress.yaml
│   ├── pvc.yaml
│   ├── configmap.yaml
│   └── secret.yaml
│
└── helm/
    └── nginx-chart/
        ├── Chart.yaml
        ├── values.yaml
        └── templates/
            ├── deployment.yaml
            ├── service.yaml
            └── ingress.yaml
```


---

# ▶️ Kubernetes Setup

## Start Minikube

```bash
minikube start
```

Check cluster status:

```bash
minikube status
```

Check Kubernetes nodes:

```bash
kubectl get nodes
```


---

# Kubernetes Deployment

Apply Kubernetes manifests:

```bash
kubectl apply -f deployment.yaml
kubectl apply -f service.yaml
kubectl apply -f ingress.yaml
kubectl apply -f pvc.yaml
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

# Docker

Docker was used as the container runtime environment.

Check Docker:

```bash
docker info
```

List containers:

```bash
docker ps
```

List images:

```bash
docker images
```


---

# Helm

Helm was used to package and manage Kubernetes applications.

Helm allows creating reusable Kubernetes templates:

```
values.yaml
      |
      v
templates/
      |
      v
Kubernetes resources
```


## Create Helm Chart

```bash
helm create nginx-chart
```


## Check generated Kubernetes manifests

```bash
helm template nginx-chart .
```


## Install application

```bash
helm install my-nginx .
```


## Check Helm releases

```bash
helm list
```


## Upgrade application

```bash
helm upgrade my-nginx .
```


## Check release history

```bash
helm history my-nginx
```


## Remove release

```bash
helm uninstall my-nginx
```


---

# Application Request Flow

```
User
 |
 v
Ingress
 |
 v
Service
 |
 v
Deployment
 |
 v
Pod
 |
 v
Container
```


---

# 🇩🇪 Deutsch

## Über dieses Projekt

Dieses Repository ist ein praktisches Kubernetes-Lernprojekt.

Das Projekt wurde **nur zu Lernzwecken erstellt** und ist keine produktive Anwendung.

Das Hauptziel dieses Projekts ist es, praktische Erfahrungen mit Kubernetes, Docker, Helm und DevOps-Workflows zu sammeln.

Während dieses Projekts wurden folgende Themen geübt:

- Verwaltung eines Kubernetes-Clusters
- Pods
- Deployments
- ReplicaSets
- Services
- ConfigMaps
- Secrets
- Persistent Volumes (PV)
- Persistent Volume Claims (PVC)
- Ingress Controller
- Helm Charts
- Helm Releases
- Helm Updates und Rollbacks
- Docker Container
- Lokale Kubernetes-Umgebung mit Minikube


---

# 🛠 Technologie-Stack

- Docker
- Docker Desktop
- Kubernetes
- Minikube
- kubectl
- Helm
- Nginx


---

# ▶️ Kubernetes starten

Minikube starten:

```bash
minikube start
```

Cluster prüfen:

```bash
kubectl get nodes
```


---

# Helm verwenden

Helm Chart erstellen:

```bash
helm create nginx-chart
```


Templates prüfen:

```bash
helm template nginx-chart .
```


Installation:

```bash
helm install my-nginx .
```


Update:

```bash
helm upgrade my-nginx .
```


Release löschen:

```bash
helm uninstall my-nginx
```


---

# Anfragefluss

```
Benutzer
 |
 v
Ingress
 |
 v
Service
 |
 v
Deployment
 |
 v
Pod
 |
 v
Container
```


---

# 🇷🇺 Русский

## О проекте

Этот репозиторий — практический учебный проект по Kubernetes.

Проект создан **исключительно для обучения** и не является production-приложением.

Основная цель проекта — получить практический опыт работы с Kubernetes, Docker, Helm и DevOps-процессами.

В проекте были изучены и применены:

- управление Kubernetes кластером
- Pods
- Deployments
- ReplicaSets
- Services
- ConfigMaps
- Secrets
- Persistent Volumes (PV)
- Persistent Volume Claims (PVC)
- Ingress Controller
- Helm Charts
- Helm Releases
- обновление и откат приложений через Helm
- Docker контейнеры
- локальная Kubernetes среда через Minikube


---

# 🛠 Используемый стек

- Docker
- Docker Desktop
- Kubernetes
- Minikube
- kubectl
- Helm
- Nginx


---

# ▶️ Запуск Kubernetes

Запуск Minikube:

```bash
minikube start
```


Проверка кластера:

```bash
kubectl get nodes
```


---

# Работа через kubectl

Применение Kubernetes конфигураций:

```bash
kubectl apply -f deployment.yaml

kubectl apply -f service.yaml

kubectl apply -f ingress.yaml

kubectl apply -f pvc.yaml
```


Проверка ресурсов:

```bash
kubectl get pods

kubectl get deployments

kubectl get services

kubectl get ingress

kubectl get pvc
```


---

# Работа через Helm

Создание Helm Chart:

```bash
helm create nginx-chart
```


Проверка шаблонов:

```bash
helm template nginx-chart .
```


Установка приложения:

```bash
helm install my-nginx .
```


Обновление приложения:

```bash
helm upgrade my-nginx .
```


История релизов:

```bash
helm history my-nginx
```


Удаление:

```bash
helm uninstall my-nginx
```


---

# Цель проекта

Получить практические навыки:

✅ Kubernetes  
✅ Docker  
✅ Helm  
✅ Container Orchestration  
✅ DevOps Workflow  
✅ Infrastructure as Code подход  


Проект является частью самостоятельного изучения DevOps и Cloud технологий.