# Quota

Resource quotas provide constraints that limit aggregate resource consumption per namespace.
![Minion](../../../assets/images/resource/quota-list-en.jpg)
## Quota operations

![Minion](../../../assets/images/resource/quota-operation-en.jpg)
The following interface graphical operations are supported:

* Label
* Notes
* Yaml/Json editing

### Create
To create a quota, click the "Create Quota" button to enter the quota creation page and fill in the necessary parameters
![Minion](../../../assets/images/resource/quota-create1-en.jpg)
parameter
name: Quota name
![Minion](../../../assets/images/resource/quota-create2-en.jpg)
Computing resources: Set the size of the computing resources used
Storage resources: Set the storage size used
Object Resources: Set the total number of objects used

Click "Create" to do so.

### Yaml create
Quotas can be created directly from Yaml files
![Minion](../../../assets/images/resource/quota-create-yaml-en.jpg)
### Quota Details
Click the link of the quota name to enter the quota details page
Overview information
![Minion](../../../assets/images/resource/quota-info1-en.jpg)

### delete
Select the quota to be deleted, click the multi-select box to select, click the "Delete button", and enter "yes" in the confirmation input box to complete the deletion operation.
### refresh
Click "Refresh" to refresh the quota list.