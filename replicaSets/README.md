# Pods
* Replicasets contains multiple pods which provides High Availability
* Replication Controller is the older technology that was replcaed by Replicasets
* ReplicaSet contains selectors but ReplciationController does not

## Labels and Selectors
* Labels are useful for selectors to select the labels.

## Commands
How to scale replica sets?
```bash
kubectl scale --replicas=6 -f replicaset-definition.yml
kubectl scale --replicas=6 replicaset myapp-replicaset
```

How to get replicaset
```bash
kubectl get rs
kubectl get replicaset
```

How to describe replicaset
```bash
kubectl describe rs myapp-replicaset
```

How to remove replicaset
```bash
kubectl delete rs myapp-replicaset
```