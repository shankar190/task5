# Task 5 - Build a Kubernetes Cluster Locally with Minikube

## Objective
Deploy and manage an application in Kubernetes using Minikube.

## Tools Used
- Docker
- Minikube
- kubectl

## Files
- deployment.yaml
- service.yaml

## Steps

### Start Minikube
```bash
minikube start
```

### Deploy the application
```bash
kubectl apply -f deployment.yaml
```

### Verify deployment
```bash
kubectl get deployments
kubectl get pods
```

### Create the service
```bash
kubectl apply -f service.yaml
```

### Verify service
```bash
kubectl get services
```

### Open the application
```bash
minikube service nginx-service
```

### Scale the deployment
```bash
kubectl scale deployment nginx-deployment --replicas=4
```

### Check pods
```bash
kubectl get pods
```

### Describe deployment
```bash
kubectl describe deployment nginx-deployment
```

### View logs
```bash
kubectl logs <pod-name>
```

## Output
- Kubernetes cluster started successfully.
- Nginx deployed.
- Service exposed using NodePort.
- Deployment scaled to 4 replicas.
