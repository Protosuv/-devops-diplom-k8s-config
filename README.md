# devops-diplom-k8s-config

1. Для развёртывания и запуска использован пакет [kube-prometheus](https://github.com/prometheus-operator/kube-prometheus.git). Для возможности обращаться к веб интерфейсу Grafana, в манифест сервиса был добавлен NodePort. Этот порт был раннее описан и открыт в конфигурации VPC в Terraform.  
```
# kubectl create -f manifests/setup/
# kubectl create -f manifests/
```

2. Для развёртывания и запуска приложения используется отдельная папка с deployment и service.
```
# kubectl create -f application/

```
