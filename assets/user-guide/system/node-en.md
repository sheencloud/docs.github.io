# node

## node
Nodes are worker machines in Kubernetes. Nodes may be virtual machines or physical machines.

## Node operations
![Minion](../../../assets/images/system/node-list-en.jpg)
### Node details
Node overview information
![Minion](../../../assets/images/system/node-info1-en.jpg)
Yaml information of the node
![Minion](../../../assets/images/system/node-info2-en.jpg)
Mirror information of the node
![Minion](../../../assets/images/system/node-info3-en.jpg)
Pod information running on the node
![Minion](../../../assets/images/system/node-info4-en.jpg)
Node's event information
![Minion](../../../assets/images/system/node-info5-en.jpg)
### Terminal
Use cloudshell to connect to nodes remotely. For cloudshell images, see Platform Management - Global Configuration
### Stain
![Minion](../../../assets/images/system/node-taints-en.jpg)
Add the taint information of the changed node


### Eviction
![Minion](../../../assets/images/system/node-cordon-en.jpg)
Evict Pods running on this node

### delete
Select the node to be deleted, click the multi-select box to select, click the "Delete" button, and enter "yes" in the confirmation input box to complete the deletion operation.
### refresh
Click "Refresh" to complete the refresh of the node list.