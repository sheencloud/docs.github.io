# Pod

A Pod is the smallest deployable unit of computing that can be created and managed in Kubernetes.
![Minion](../../../assets/images/workload/pod-list-en.jpg)
## Pod operations

![Minion](../../../assets/images/workload/pod-operation-en.jpg)
The following interface graphical operations are supported:
* Debug Pod
* Service public
* Image upgrade
* Tolerate
* Label
* Notes
* Yaml/Json editing

### Status selection
Pod supports the following state selections

![Minion](../../../assets/images/workload/pod-status-en.jpg)

### Command Line
Pod clicks the "Command Line" button, and the "Command Line" window pops up, and you can execute shell commands in the "Command Line" window
![Minion](../../../assets/images/workload/pod-terminal-en.jpg)

### log
Pod clicks the "Log" button to view the Container log in the Pod
![Minion](../../../assets/images/workload/pod-log-en.jpg)

### Create
Create a Pod, click the "Create Pod" button, enter the Create Pod page, and fill in the necessary parameters
![Minion](../../../assets/images/workload/pod-create1-en.jpg)
parameter
Name: Pod name

![Minion](../../../assets/images/workload/pod-create2-en.jpg)
parameter
Image name: Pod image name
Mirror address: Pod mirror warehouse address
Exposed port: Service exposed port
![Minion](../../../assets/images/workload/pod-create3-en.jpg)
Optional parameters:
Pod Security
Pod network
other
Click "Create" to do so.

### Yaml create
Pods can be created directly from Yaml files
![Minion](../../../assets/images/workload/pod-create-yaml-en.jpg)
### Pod Details
Click the link of the Pod name to enter the details page of the Pod
Overview information
![Minion](../../../assets/images/workload/pod-info1-en.jpg)

Yaml information
![Minion](../../../assets/images/workload/pod-info2-en.jpg)
container information
![Minion](../../../assets/images/workload/pod-info3-en.jpg)
Storage volume information
![Minion](../../../assets/images/workload/pod-info4-en.jpg)
Environmental information
![Minion](../../../assets/images/workload/pod-info5-en.jpg)
log
![Minion](../../../assets/images/workload/pod-info6-en.jpg)
terminal
![Minion](../../../assets/images/workload/pod-info7-en.jpg)
event information
![Minion](../../../assets/images/workload/pod-info8-en.jpg)
Pod monitoring information
![Minion](../../../assets/images/workload/pod-info9-en.jpg)
### delete
Select the Pod to be deleted, click the multi-select box to select, click the "Delete button", and enter "yes" in the confirmation input box to complete the deletion operation.
### refresh
Click "Refresh" to complete the refresh of the Pod list.