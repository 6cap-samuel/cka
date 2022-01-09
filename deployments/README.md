# Deployments
Deployment is somehow similar to replica sets but it has rollback features and rolling update features.

## Commands
Gets the list of pods available in the kube cluster.
```bash
kubectl get deployments
```

Describe the pod nginx
```bash
kubectl describe deployment myapp-deployment
```

Delete pod nginx
```bash
kubectl delete deployment myapp-deployment
```