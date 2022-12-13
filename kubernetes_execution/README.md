# Kubernetes resources

In this folder you will find the basic resources to deploy an application that displays an ngnix hello world image. Just copy this folder & execute below commands

You can deploy the application in your cluster with:

```bash
kubectl apply -f deployment.yaml
kubectl apply -f service-nodeport.yaml
kubectl apply -f ingress.yaml
```
