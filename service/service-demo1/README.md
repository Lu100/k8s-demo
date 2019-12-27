+ create pod
```
kubectl apply -f webapp-rc.yaml
```
+ expose service
```
kubectl expose rc webapp
```
+ query service

```
kubectl get service
```

+ testing

```
curl x.x.x.x:8080
```

or:
+ query service
```
kubectl apply -f webapp-svc.yaml
curl x.x.x.x:8081
```
