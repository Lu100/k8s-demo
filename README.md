#  一些k8s的配置文件 参考《Kubernetes权威指南》
---
+ deploy Deployment配置
+ ds DaemonSet 配置
+ ha-mongodb 高可用的mongodb，由于glusterFS集群没做，暂时搁置
+ hpa 自动扩容，k8s版本升级后，metric监控的配置改变，1.5.1版本k8s无法获取到CPU状态，所以暂时搁置
+ job 简单的 job pod 
+ src ConfigMap liveness可用状态检查等简单配置

+ busybox.yaml 简单的pod，可用于pod调试
