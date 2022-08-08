# deploy

Deployments provide declarative update capabilities for Pods and ReplicaSets.
![Minion](../../../assets/images/workload/deploy-list-en.jpg)
## deploy operations

![Minion](../../../assets/images/workload/deploy-operation-en.jpg)
The following interface graphical operations are supported:
* Pause rolling updates
* Service public
* Expansion
* reboot
* Image upgrade
* rollback
* other configuration
* pod network
* Affinity
* Tolerate
* Strategy
* Safety
* Label
* Notes
* Yaml/Json editing

### Create
Create a deployment, click the "Create Deployment" button, enter the Create Deployment page, and fill in the necessary parameters
![Minion](../../../assets/images/workload/deploy-create1-en.jpg)
parameter
name: deployment name
Number of replicas: The number of replicas of the deployment control pod
![Minion](../../../assets/images/workload/deploy-create2-en.jpg)
parameter
Image name: Deployment image name
Mirror address: deployment mirror warehouse address
![Minion](../../../assets/images/workload/deploy-create3-en.jpg)
parameter
Update strategy: deploy image rolling upgrade strategy
Click "Create" to do so.
### Deployment Details
Click the link of the deployment name to enter the deployment details page
Overview information
![Minion](../../../assets/images/workload/deploy-info1-en.jpg)
topology information
![Minion](../../../assets/images/workload/deploy-info2-en.jpg)
Yaml information
![Minion](../../../assets/images/workload/deploy-info3-en.jpg)
container information
![Minion](../../../assets/images/workload/deploy-info4-en.jpg)
Revision log information
![Minion](../../../assets/images/workload/deploy-info5-en.jpg)
Pod information
![Minion](../../../assets/images/workload/deploy-info6-en.jpg)
Storage volume information
![Minion](../../../assets/images/workload/deploy-info7-en.jpg)
Environmental information
![Minion](../../../assets/images/workload/deploy-info8-en.jpg)
event information
![Minion](../../../assets/images/workload/deploy-info9-en.jpg)

### delete
Select the deployment to be deleted, click the multi-select box to select, click the "Delete button", and enter "yes" in the confirmation input box to complete the deletion operation.
### refresh
Click "Refresh" to complete the refresh of the deployment list.