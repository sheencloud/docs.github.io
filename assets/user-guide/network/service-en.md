# Serve

A service is an instance that provides network services inside and outside the cluster
![Minion](../../../assets/images/network/svc-list-en.jpg)
## service operation

![Minion](../../../assets/images/network/svc-operation-en.jpg)
The following interface graphical operations are supported:

* Label
* Notes
* Yaml/Json editing

### Create
To create a service, click the "Create Service" button to enter the create service page and fill in the necessary parameters
![Minion](../../../assets/images/network/svc-create1-en.jpg)
parameter
name: service name
Service Type: Supports Cluster IP, Node Port, Load Balancer, External Name
Session affinity: whether to keep the session
Pod selector: Select the Pods forwarded by the service
Exposed port: The port number of the service

### Yaml create
Services can be created directly from Yaml files
![Minion](../../../assets/images/network/svc-create-yaml-en.jpg)
### Service Details
Click the link of the service name to enter the service details page
Overview information
![Minion](../../../assets/images/network/svc-info1-en.jpg)

Yaml information
![Minion](../../../assets/images/network/svc-info2-en.jpg)
event information
![Minion](../../../assets/images/network/svc-info3-en.jpg)

### edit
Select the service to be edited, click the "Edit" button, enter the edit service page, and modify the necessary parameters to complete the deletion operation.
* Support graphical modification of service parameters
![Minion](../../../assets/images/network/svc-edit1-en.jpg)
* Support Yaml modification
![Minion](../../../assets/images/network/svc-edit-yaml-en.jpg)
### delete
Select the service to be deleted, click the multi-select box to select, click the "Delete button", and enter "yes" in the confirmation input box to complete the deletion operation.
### refresh
Click "Refresh" to complete the refresh of the service list.