# Kubernetes notes

## kubectl commands

https://kubernetes.io/docs/tasks/access-application-cluster/ingress-minikube/


```shell
kubectl apply -f example-ingress.yaml example-ingress.yaml
```

or

```shell
kubectl apply -f https://k8s.io/examples/service/networking/example-ingress.yaml
```
## DNS entries

```shell
# /etc/hosts

192.168.39.82   hello-world.info
192.168.49.2    dashboard.com
10.111.216.221  dashboard.com
```

```shell
kubectl apply -f dashboard-ingress.yaml 
```

```shell
kubectl get ingress -n kubernetes-dashboard
```

```shell
kubectl describe ingress dashboard-ingress -n kubernetes-dashboard
```

https://dashboard.com/api/v1/namespaces/kubernetes-dashboard/services/http:kubernetes-dashboard:/proxy/
https://dashboard.com:41149/api/v1/namespaces/kubernetes-dashboard/services/http:kubernetes-dashboard:/proxy/
http://127.0.0.1:41149/api/v1/namespaces/kubernetes-dashboard/services/http:kubernetes-dashboard:/proxy/