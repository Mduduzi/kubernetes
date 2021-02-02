# Kubernetes notes

## kubectl commands

[Set up Ingress on Minikube with the NGINX Ingress Controller](https://kubernetes.io/docs/tasks/access-application-cluster/ingress-minikube/)


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

## Start Minikube
### Start Minikube itself
```shell
minikube start
```

## Pod
### Create a new pod
```shell
kubectl run hello-minikube --image=gcr.io/google_containers/echoserver:1.4 --port=8080
```

### List pods
```shell
kubectl get pod
```
### Delete Pods
```shell
kubectl delete pods hello-minikube
```

## Deployment



## shell session
```console
foo@bar:~$ whoami
foo
```

## Some shell samples:
```
Shell:      console, shell
Bash:       bash, sh, zsh
PowerShell: powershell, ps
DOS:        dos, bat, cmd
```

#### Example:

```bat
cd \
copy a b
ping 192.168.0.1
```

```javascript
var s = "JavaScript syntax highlighting";
alert(s);
```
 
```python
s = "Python syntax highlighting"
print s
```
 
```
No language indicated, so no syntax highlighting. 
But let's throw in a <b>tag</b>.
```
