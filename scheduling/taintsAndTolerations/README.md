# Taints & Tolerations
* A taint is to spray a node with a protection.
* A toleration is making the taint useless.

## Commands
This command will taint the node.
```bash
kubectl taint nodes node-name key=value:taint-effect
kubectl taint nodes node1 app=blue:NoSchedule
```

This command will untaint the node.
```bash
kubectl taint nodes node-name key=value:taint-effect-
kubectl taint nodes node1 app=blue:NoSchedule-
```

Taint Effects
* NoSchedule
* PreferNoSchedule
* NoExecute
