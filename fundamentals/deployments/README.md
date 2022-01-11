# Deployments
Deployment is somehow similar to replica sets but it has rollback features and rolling update features.

## Commands
Gets the list of deployments available in the kube cluster.
```bash
kubectl get deployments
```

Create the deployment 
```bash
kubectl create deployment --image=nginx nginx
```

Create the deployment without running the command and in yaml format
```bash
kubectl create deployment --image=nginx nginx --dry-run=client -o yaml
```

Generate deployment with 4 replicas
```bash
kubectl create deployment nginx --image=nginx --replicas=4
```

Scale your deployment
```bash
kubectl scale deployment nginx --replicas=4
```

Export deployment into a yaml file
```bash
kubectl create deployment nginx --image=nginx --dry-run=client -o yaml > nginx-deployment.yaml
```

Describe the deployment named 'myapp-deployment'
```bash
kubectl describe deployment myapp-deployment
```

Delete the deployment named 'myapp-deployment'
```bash
kubectl delete deployment myapp-deployment
```