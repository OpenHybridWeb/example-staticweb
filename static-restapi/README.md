# Example - static website plus rest api
Example of Hybrid Web with static components plus rest api.

Combine two example static component and rest api
1. [Theme](https://github.com/OpenHybridWeb/example-component-theme)
2. [Homepage](https://github.com/OpenHybridWeb/example-component-homepage)

Create REST API manually:
```shell
kubectl -n static-restapi-dev create deployment hello-app1 --image=lkrzyzanek/helloworld-restapi
kubectl -n static-restapi-dev expose deployment hello-app1 --type=NodePort --port=8080

kubectl -n static-restapi-dev create deployment hello-app2 --image=lkrzyzanek/helloworld-restapi:1.0
kubectl -n static-restapi-dev expose deployment hello-app2 --type=NodePort --port=8080
```
