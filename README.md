# devops-demo1
First demo project in course Devops and Kubernetes (https://prometheus.org.ua/prometheus-plus/devops_and_kubernetes/)

Small web application with one page that represents DevOps main therms

This application was build into docker image and pushed into my Dockerhub repository - https://hub.docker.com/repository/docker/viktormazepa/devops-demo1/general

To deploy application to Kubernates execute command:
```
kubectl create deploy devops-demo1 --image viktormazepa/devops-demo1:v1.0.0
```

Don't forget to add port-forwarding:
```
kubectl port-forward deploy/devops-demo1 8080
```
