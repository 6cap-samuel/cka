# Node Selector
* Select which node should the pods go to.
* You cannot place pods in nodes with multiple condition.

## Commands
This command will label the node so that the pod with node selector can join the node
```bash
kubectl label nodes <node-name> <label-key>=<label-value>
kubectl label nodes node-1 size=Large
``` 