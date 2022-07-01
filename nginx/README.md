# Nginx Example

## Imperative Approach

This is a quick way to start Nginx using imperative commands:

```
kubectl create deployment --image nginx my-nginx
kubectl scale deployment --replicas 2 my-nginx
kubectl expose deployment my-nginx --port=80 --type=LoadBalancer
```

See results:

```
kubectl get pods,deploy,svc
```

Cleanup:

```
kubectl delete deployment my-nginx
```

## Declarative Approach

The remaining examples in this folder demonstrate YAML config files to create an Nginx application.


## Sources
https://github.com/kubernetes/examples/blob/master/staging/simple-nginx.md
https://kubernetes.io/docs/tasks/configure-pod-container/configure-persistent-volume-storage/