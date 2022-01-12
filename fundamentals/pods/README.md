# Pods
Pod is a single container to is runs with an image

## Commands
Runs an nginx image with a pod name nginx
```bash
kubectl run nginx --image nginx
```

Gets the list of pods available in the kube cluster.
```bash
kubectl get pods
```

Generates a yaml file of the nginx image.
```bash
kubectl run nginx --image nginx -o yaml --dry-run=client
```

Describe the pod nginx
```bash
kubectl describe pod nginx
```

Delete pod nginx
```bash
kubectl delete pod nginx
```

Create the pod with apply command
```bash
kubectl apply -f pod.yaml
```

Shows all information about the pod and more details like nodes
```bash
k get pods --all-namespaces -o wide
```