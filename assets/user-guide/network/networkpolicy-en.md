# network policy

Network policies are specifications on how groups of pods are allowed to communicate with each other and with other network endpoints
![Minion](../../../assets/images/network/np-list-en.jpg)
## Network Policy Actions

![Minion](../../../assets/images/network/np-operation-en.jpg)
The following interface graphical operations are supported:

* Label
* Notes
* Yaml/Json editing

### Create
Create a network policy, click the "Create Network Policy" button, enter the Create Network Policy page, and fill in the necessary parameters
![Minion](../../../assets/images/network/np-create1-en.jpg)
parameter
Name: Network Policy Name
Network Policy Template:
* Allow all ingress traffic
* Deny all ingress traffic
* Allow all egress traffic
* Deny all egress traffic
* Deny all ingress and egress traffic
* Custom: Users can customize the network traffic limit

### Yaml create
Network policies can be created directly from Yaml files
![Minion](../../../assets/images/network/np-create-yaml-en.jpg)
### Network Policy Details
Click the link of the network policy name to enter the details page of the network policy
Overview information
![Minion](../../../assets/images/network/np-info1-en.jpg)

Yaml information
![Minion](../../../assets/images/network/np-info2-en.jpg)
event information
![Minion](../../../assets/images/network/np-info3-en.jpg)

### edit
Select the network policy to be edited, click the "Edit" button, enter the edit network policy page, and modify the necessary parameters to complete the deletion operation.
* Support graphical modification of network policy parameters
![Minion](../../../assets/images/network/np-edit1-en.jpg)
* Support Yaml modification
![Minion](../../../assets/images/network/np-edit-yaml-en.jpg)
### delete
Select the network policy to be deleted, click the multi-select box to select, click the "Delete button", and enter "yes" in the confirmation input box to complete the deletion operation.
### refresh
Click "Refresh" to complete the refresh of the network policy list.