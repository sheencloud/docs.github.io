# Quick Start

## Install via kubernetes yaml file
### empty volume
* Install the demo demo environment, there is no persistent storage in the cluster, all storage uses emptyDir
````
kubectl apply -f https://raw.githubusercontent.com/sheencloud/hyperkuber/main/manifests/hkcmp/manifest.yaml
````
Determine if it is installed by looking at the pod status.
````
kubectl get po -n hyperkuber
````
View the Ingress address and access it through a browser
````
kubectl get ing -n hyperkuber
````

### persistent volume
* Install persistent storage environment, persistent storage PV or StorageClass exists in the cluster
````
kubectl apply -f https://raw.githubusercontent.com/sheencloud/hyperkuber/main/manifests/hkcmp/manifest-persistent.yaml
````
Determine if it is installed by looking at the pod status.
````
kubectl get po -n hyperkuber
````
View the Ingress address and access it through a browser
````
kubectl get ing -n hyperkuber
````
### Change setting

````
kubectl get cm -n hyperkuber
````
Modify the configuration information of redis and mysql in the ConfigMap of hyperkuber-configmap