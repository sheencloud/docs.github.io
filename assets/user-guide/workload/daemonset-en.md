# daemon set

DaemonSet (daemon process set) is similar to the daemon process, it deploys a Pod on each node that meets the matching conditions
![Minion](../../../assets/images/workload/ds-list-en.jpg)
## Daemon set operations

![Minion](../../../assets/images/workload/ds-operation-en.jpg)
The following interface graphical operations are supported:
* Service public
* rollback
* Image upgrade
* reboot
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
Create a daemon process set, click the "Create daemon process set" button, enter the create daemon process set page, and fill in the necessary parameters
![Minion](../../../assets/images/workload/ds-create1-en.jpg)
parameter
name: daemon set name

![Minion](../../../assets/images/workload/ds-create2-en.jpg)
parameter
image name: daemon set image name
Mirror address: daemon set mirror warehouse address
exposed port: daemon set service exposed port
![Minion](../../../assets/images/workload/ds-create3-en.jpg)
Optional parameters:
Pod Security
Pod network
other
Click "Create" to do so.

### Yaml create
Daemon sets can be created directly from Yaml files
![Minion](../../../assets/images/workload/ds-create-yaml-en.jpg)
### Daemon set details
Click the link of the daemon set name to enter the details page of the daemon set
Overview information
![Minion](../../../assets/images/workload/ds-info1-en.jpg)

Yaml information
![Minion](../../../assets/images/workload/ds-info2-en.jpg)
container information
![Minion](../../../assets/images/workload/ds-info3-en.jpg)
Revision log information
![Minion](../../../assets/images/workload/ds-info4-en.jpg)
Pod information
![Minion](../../../assets/images/workload/ds-info5-en.jpg)
Storage volume information
![Minion](../../../assets/images/workload/ds-info6-en.jpg)
Environmental information
![Minion](../../../assets/images/workload/ds-info7-en.jpg)
event information
![Minion](../../../assets/images/workload/ds-info8-en.jpg)

### delete
Select the daemon process set to be deleted, click the multi-select box to select, click the "Delete button", and enter "yes" in the confirmation input box to complete the deletion operation.
### refresh
Click "Refresh" to complete the refresh of the daemon set list.