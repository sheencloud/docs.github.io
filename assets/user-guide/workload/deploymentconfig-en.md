# deploy configuration

DeploymentConfig is Openshift's deployment configuration, an extension of Kubernetes deployment that provides fine-grained management of common user applications.
![Minion](../../../assets/images/workload/dc-list-en.jpg)
## deploy configuration operations

![Minion](../../../assets/images/workload/dc-operation-en.jpg)
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
Create a deployment configuration, click the "Create Deployment Configuration" button, enter the Create Deployment Configuration page, and fill in the necessary parameters
![Minion](../../../assets/images/workload/dc-create1-en.jpg)
parameter
name: Deployment configuration name
Number of replicas: The deployment configuration controls the number of replicas of the Pod
![Minion](../../../assets/images/workload/dc-create2-en.jpg)
parameter
Image name: Deployment configuration image name
Mirror address: deployment configuration mirror warehouse address
![Minion](../../../assets/images/workload/dc-create3-en.jpg)
parameter
Update strategy: Deployment configuration mirror rolling upgrade strategy
trigger:
* imageChange: When the image changes, trigger a rolling upgrade
* configChange: When the configuration changes, trigger a rolling upgrade

Click "Create" to do so.
### Deployment configuration details
Click the link of the deployment configuration name to enter the details page of the deployment configuration
Overview information
![Minion](../../../assets/images/workload/dc-info1-en.jpg)
Yaml information
![Minion](../../../assets/images/workload/dc-info2-en.jpg)
container information
![Minion](../../../assets/images/workload/dc-info3-en.jpg)
Revision log information
![Minion](../../../assets/images/workload/dc-info4-en.jpg)
Pod information
![Minion](../../../assets/images/workload/dc-info5-en.jpg)
Storage volume information
![Minion](../../../assets/images/workload/dc-info6-en.jpg)
Environmental information
![Minion](../../../assets/images/workload/dc-info7-en.jpg)
log information
![Minion](../../../assets/images/workload/dc-info8-en.jpg)
event information
![Minion](../../../assets/images/workload/dc-info9-en.jpg)

### delete
Select the deployment configuration to be deleted, click the multi-select box to select, click the "Delete button", and enter "yes" in the confirmation input box to complete the deletion operation.
### refresh
Click "Refresh" to complete the refresh of the deployment configuration list.