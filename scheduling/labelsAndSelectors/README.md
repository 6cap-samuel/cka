# Labels and Selectors
* Standard to group things together.

# Annotations


## Commands
Find the pods that has a label of app that contains the value of App1
```bash
kubectl get pods --selector app=App1
```

Find the pods that has multiple labels
```bash
kubectl get pods --selector app=App1,env=prod,tier=frontend
```

