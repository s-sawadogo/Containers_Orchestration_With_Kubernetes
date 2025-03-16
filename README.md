# Start minikube 
```
minikube start
```

# Deploy K8s resource
```
kubectl apply -f lab
```

# Create secret
```
kubectl create secret generic db-secrets --from-env-file=lab/env -n vote
```

# Test services
```
minikube service --all -n vote
```
