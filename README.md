# My Kubernetes Minikube Project

This project deploys an Nginx app using Kubernetes Minikube on EC2.

## Files
- `deployment.yaml` → Deployment instructions
- `service.yaml` → Expose Nginx on NodePort
- `screenshots/` → Output screenshots

## How to run
1. Start Minikube: `minikube start --driver=docker`
2. Apply deployment: `kubectl apply -f deployment.yaml`
3. Apply service: `kubectl apply -f service.yaml`
4. Check pods: `kubectl get pods`
5. Check service: `kubectl get svc`
6. Access app: `http://<public id>:30007`
