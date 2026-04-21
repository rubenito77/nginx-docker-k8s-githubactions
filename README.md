🚀 Nginx Docker + K3s + GitHub Actions + Traefik (Ingress)
🧠 Overview

Este proyecto implementa un flujo completo tipo DevOps / GitOps-ready:

🐳 Build de imagen Docker
📦 Push a Docker Hub
⚙️ Deploy automático con GitHub Actions
☸️ Despliegue en Kubernetes (K3s)
🌐 Exposición mediante Traefik Ingress
🔁 Rolling updates automáticos
🏗️ Arquitectura
GitHub Push
   ↓
GitHub Actions (CI/CD)
   ↓
Docker Hub (imagen)
   ↓
K3s Cluster
   ↓
Deployment → Pods
   ↓
Service (ClusterIP)
   ↓
Ingress (Traefik)
   ↓
http://nginx.platform.local
📁 Estructura del proyecto
.
├── Dockerfile
├── k8s/
│   ├── deployment.yaml
│   ├── service.yaml
│   └── ingress.yaml
└── .github/
    └── workflows/
        └── deploy.yml
