# Namespace
Namespace is a way to control which environment does each pod lives in. 

## Commands
Create a pod with dev namespace
```bash
kubectl run nginx --image nginx --namespace dev
```

Get all pods with dev namespace
```bash
kubectl get pods --namespace dev
```

Get all pods from all namespace
```bash
kubectl get pods --all=namespace
```

Set dev namespace as current working environment
```bash
kubectl config set-context $(kubecrl config current-context) --namespace=dev
```
