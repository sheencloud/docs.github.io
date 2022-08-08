# persistent storage application

A persistent storage request (pvcC) is a user's storage request.
![Minion](../../../assets/images/storage/pvc-list-en.jpg)
## Persistent storage request operation

![Minion](../../../assets/images/storage/pvc-operation-en.jpg)
The following interface graphical operations are supported:

* Label
* Notes
* Yaml/Json editing

### Create
Create a persistent storage application, click the "Create persistent storage application" button, enter the create persistent storage application page, and fill in the necessary parameters
![Minion](../../../assets/images/storage/pvc-create1-en.jpg)
parameter
Name: persistent storage application name
Select storage class: Specify the storage class to create
Persistent storage application access mode:
* Multiple reading and writing
* Single read and write
* read only
Persistent storage application size: storage capacity size
Storage volume name: Specify the storage volume to create

### Yaml create
Persistent storage applications can be created directly through Yaml files
![Minion](../../../assets/images/storage/pvc-create-yaml-en.jpg)
### Persistent storage application details
Click the link of the persistent storage application name to enter the details page of the persistent storage application
Overview information
![Minion](../../../assets/images/storage/pvc-info1-en.jpg)

Yaml information
![Minion](../../../assets/images/storage/pvc-info2-en.jpg)
event information
![Minion](../../../assets/images/storage/pvc-info3-en.jpg)

### delete
Select the persistent storage application to be deleted, click the multi-select box to select, click the "Delete button", and enter "yes" in the confirmation input box to complete the deletion operation.
### refresh
Click "Refresh" to refresh the persistent storage application list.