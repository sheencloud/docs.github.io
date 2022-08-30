# 安装

基本上HyperKuber可以独立安装，不需要任何软件，但是要正常监控，需要prometheus或者prometheus stack。

可以安装以获得更多功能的服务列表（不是必需的，但推荐）。

+ ## Prometheus
   对于指标和监控系统
```
# helm安装 (https://artifacthub.io/packages/helm/prometheus-community/kube-prometheus-stack)

helm repo add prometheus-community https://prometheus-community.github.io/helm-charts
helm install my-kube-prometheus-stack prometheus-community/kube-prometheus-stack --version 39.9.0 -n monitoring --create-namespace
```
+ ## ArgoCD
    对于 GitOps 系统。
```
# helm安装 (https://artifacthub.io/packages/helm/argo/argo-cd)

helm repo add argo https://argoproj.github.io/argo-helm
helm install my-argo-cd argo/argo-cd --version 5.3.6
```
+ ## ElasticSearch
   用于日志系统。
```
# helm安装 elasticsearch (https://artifacthub.io/packages/helm/elastic/elasticsearch)

helm repo add elastic https://helm.elastic.co
helm install my-elasticsearch elastic/elasticsearch --version 7.17.3 -n logging --create-namespace

# helm安装 kibana (https://artifacthub.io/packages/helm/elastic/kibana)

helm repo add elastic https://helm.elastic.co
helm install my-kibana elastic/kibana --version 7.17.3 -n logging --create-namespace

# helm安装 filebeat (https://artifacthub.io/packages/helm/elastic/filebeat)

helm repo add elastic https://helm.elastic.co
helm install my-filebeat elastic/filebeat --version 7.17.3
```

+ ## Harbor
  用于仓库管理。
```
# helm安装  (https://artifacthub.io/packages/helm/harbor/harbor)

helm repo add harbor https://helm.goharbor.io
helm install my-harbor harbor/harbor --version 1.9.3 -n harbor --create-namespace
```