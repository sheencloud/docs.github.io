# Quick Start

## Install via kubernetes yaml file
### Demo 
For quick start and demo try out, run the following command as a cluster admin:

```console
kubectl apply -f https://manifests.sheencloud.com/manifests/manifest.yaml

or

kubectl apply -f https://manifests.sheencloud.com/manifests/manifest-psp.yaml  #for psp enabled clusters
```
Check out pod status in namespace hyperkuber

```console
kubectl get po -n hyperkuber
```

When all pods are running and ready, access the console ingress created by default,

```console
kubectl get ing -n hyperkuber
```

Open the ingress in your favourite browser and login with default user/password: admin/hyperkuber@1314

For other installation methods, such as [helm installation](https://charts.sheencloud.com) or [operator installation](https://operator.sheencloud.com), checkout our [online documents](https://docs.sheencloud.com) for more details.

### Production (persistent volume)
* Install persistent storage environment, persistent storage PV or StorageClass exists in the cluster
````
kubectl apply -f https://manifests.sheencloud.com/manifests/manifest-persistent.yaml
````
checkout pod status.
````
kubectl get po -n hyperkuber
````
when all are in ready status, get the Ingress address and access it through a browser
````
kubectl get ing -n hyperkuber
````
### Change setting

````
kubectl get cm -n hyperkuber
````
Modify the configuration information of redis and mysql in the ConfigMap of hyperkuber-configmap