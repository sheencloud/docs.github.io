# service account

A service account provides an identity to a process running in a Pod.
![Minion](../../../assets/images/resource/sa-list-en.jpg)
## Service account operations

![Minion](../../../assets/images/resource/sa-operation-en.jpg)
The following interface graphical operations are supported:

* Label
* Notes
* Yaml/Json editing

### Create
Create a service account, click the "Create Service Account" button, enter the Create Service Account page, and fill in the necessary parameters
![Minion](../../../assets/images/resource/sa-create1-en.jpg)
parameter
Name: Service account name
Choose a key: The key that pods running with this service account are allowed to use.
Select: A reference to a secret in the same namespace used to pull any images in pods that reference this service account.

Click "Create" to do so.

### Yaml create
Service accounts can be created directly from Yaml files
![Minion](../../../assets/images/resource/sa-create-yaml-en.jpg)
### Service Account Details
Click the link of the service account name to go to the details page of the service account
Overview information
![Minion](../../../assets/images/resource/sa-info1-en.jpg)

Yaml information
![Minion](../../../assets/images/resource/sa-info2-en.jpg)


### delete
Select the service account to be deleted, click the multi-select box to select, click the "Delete button", and enter "yes" in the confirmation input box to complete the deletion operation.
### refresh
Click "Refresh" to complete the refresh of the service account list.