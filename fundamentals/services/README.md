# Services
## Node Port
* This service allows the port accessible from the client node. (Available port numbers 30000 - 32767)

## Cluster IP
* This service allows the cluster to interact with each other.

## Load Balancer
* Load balanced service helps to load balance the service to different nodes in the kubernetes clusters.

## Commands
how to get all services that is listed in kube
```bash
kubectl get services
```

Create a Service named redis-service of type ClusterIP to expose pod redis on port 6379
```bash
kubectl expose pod redis --port=6379 --name redis-service --dry-run=client -o yaml

kubectl create service clusterip redis --tcp=6379:6379 --dry-run=client -o yaml
```

Create a Service named nginx of type NodePort to expose pod nginx's port 80 on port 30080 on the nodes:
```bash
kubectl expose pod nginx --type=NodePort --port=80 --name=nginx-service --dry-run=client -o yaml

kubectl create service nodeport nginx --tcp=80:80 --node-port=30080 --dry-run=client -o yaml
```