# Learning K8S

## Creating a deployment

```shell
kubectl create deployment web --image=gcr.io/google-samples/hello-app:1.0
kubectl get deployment web
kubectl expose deployment web --type=NodePort --port=8080
kubectl get service web
minikube service web --url
```


## Creating a Ingress
```shell
kubectl apply -f https://k8s.io/examples/service/networking/example-ingress.yaml
```