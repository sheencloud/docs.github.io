# Prerequests

Basicly HyperKuber can be installed independently without any software, But for the monitoring works properly, the prometheus or prometheus stack is needed. 

A list of service that can be installed for more functionality, (Not Required, but recommended).

+ ## Prometheus
  For metrics and monitoring system
```
# install by helm (https://artifacthub.io/packages/helm/prometheus-community/kube-prometheus-stack)

helm repo add prometheus-community https://prometheus-community.github.io/helm-charts
helm install my-kube-prometheus-stack prometheus-community/kube-prometheus-stack --version 39.9.0 -n monitoring --create-namespace
```

+ ## ArgoCD
   For GitOps system.
   
```
# install by helm (https://artifacthub.io/packages/helm/argo/argo-cd)

helm repo add argo https://argoproj.github.io/argo-helm
helm install my-argo-cd argo/argo-cd --version 5.3.6 -n argo-cd --create-namespace
```

+ ## ElasticSearch
  For Logging system.
```
# install elasticsearch by helm (https://artifacthub.io/packages/helm/elastic/elasticsearch)

helm repo add elastic https://helm.elastic.co
helm install my-elasticsearch elastic/elasticsearch --version 7.17.3 -n logging --create-namespace

# install kibana by helm (https://artifacthub.io/packages/helm/elastic/kibana)

helm repo add elastic https://helm.elastic.co
helm install my-kibana elastic/kibana --version 7.17.3 -n logging --create-namespace

# install filebeat by helm (https://artifacthub.io/packages/helm/elastic/filebeat)

helm repo add elastic https://helm.elastic.co
helm install my-filebeat elastic/filebeat --version 7.17.3
```


+ ## Harbor
+ For registry management.
```
# install by helm (https://artifacthub.io/packages/helm/harbor/harbor)

helm repo add harbor https://helm.goharbor.io
helm install my-harbor harbor/harbor --version 1.9.3 -n harbor --create-namespace
```



