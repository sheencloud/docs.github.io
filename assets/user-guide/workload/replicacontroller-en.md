# replica controller

The replica controller ensures that the specified number of pod replicas are running at all times.
![Minion](../../../assets/images/workload/rc-list-en.jpg)
## replica controller action

![Minion](../../../assets/images/workload/rc-operation-en.jpg)
The following interface graphical operations are supported:
* Service public
* Expansion
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
Create a replica controller, click the "Create a replica controller" button, enter the create replica controller page, and fill in the necessary parameters
![Minion](../../../assets/images/workload/rc-create1-en.jpg)
parameter
name: replica controller name

![Minion](../../../assets/images/workload/rc-create2-en.jpg)
parameter
Image name: Replica controller image name
Mirror address: the mirror warehouse address of the replica controller
Exposed port: The replica controller service exposes the port
![Minion](../../../assets/images/workload/rc-create3-en.jpg)
Optional parameters:
Pod Security
Pod network
other
Click "Create" to do so.

### Yaml create
Replica controllers can be created directly from Yaml files
![Minion](../../../assets/images/workload/rc-create-yaml-en.jpg)
### Replica Controller Details
Click the link of the replica controller name to enter the details page of the replica controller
Overview information
![Minion](../../../assets/images/workload/rc-info1-en.jpg)

Yaml information
![Minion](../../../assets/images/workload/rc-info2-en.jpg)
container information
![Minion](../../../assets/images/workload/rc-info3-en.jpg)
Pod information
![Minion](../../../assets/images/workload/rc-info4-en.jpg)
Storage volume information
![Minion](../../../assets/images/workload/rc-info5-en.jpg)
Environmental information
![Minion](../../../assets/images/workload/rc-info6-en.jpg)
event information
![Minion](../../../assets/images/workload/rc-info7-en.jpg)

### delete
Select the copy controller to be deleted, click the multi-select box to select, click the "Delete button", and enter "yes" in the confirmation input box to complete the deletion operation.
### refresh
Click "Refresh" to complete the refresh of the replica controller list.