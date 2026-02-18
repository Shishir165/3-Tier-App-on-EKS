# 3-Tier Application on Amazon EKS

This project deploys a 3-tier application on Amazon EKS using Kubernetes.

## Architecture
- Frontend: Nginx (UI)
- Backend: .NET API
- Database: PostgreSQL
- Ingress: NGINX Ingress Controller

## Kubernetes Resources
- Deployments for UI, API, Postgres
- ClusterIP Services
- Ingress for external access

## How to Deploy
```bash
kubectl apply -f postgres-deployment.yaml
kubectl apply -f api-deployment.yaml
kubectl apply -f ui-deployment.yaml
kubectl apply -f ui-ingress.yaml
