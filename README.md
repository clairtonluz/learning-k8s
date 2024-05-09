# Learning K8S

# Inicializar minikube

[Minikube Readme](MINIKUBE.md)

## Creating example

* `-k` bellow is because I using [kustomizer](https://kustomizer.dev/). 
* if you are using macOS you need open another terminal e run `sudo minikube tunnel` to allow minikube use the ports `80` and `443`

```shell
kubectl apply -k example
```

edit you `etc/hosts` and add the follow line `127.0.0.1       hello-world.local`
now access [http://hello-world.local](http://hello-world.local) and [http://hello-world.local/v2](http://hello-world.local/v2)