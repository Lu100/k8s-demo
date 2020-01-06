# 如何使用

## 1、安装HELM
```
curl https://raw.githubusercontent.com/helm/helm/master/scripts/get-helm-3 | bash
```
## 2、安装仓库
```
helm repo add stable https://kubernetes-charts.storage.googleapis.com/
```
## 3、设置NFS存储地址
### 需要自己创建一个NFS存储
```
helm install stable/nfs-client-provisioner --set nfs.server=x.x.x.x --set nfs.path=xxx --generate-name
```

## 4、启动

```
kubectl apply -f .
```

## 5、验证

去对应的NFS存储节点，可以看到创建了一个文件夹，并且添加了一个文件
