# Git application

Create GitOps applications and manage GitOps applications

## Git application operations
Click the "GitOps" menu on the left to enter the GitOps application page to perform related operations
![Minion](../../../assets/images/gitops/app-list-en.jpg)
### Create application

Click the "Create Git Application" button to enter the connection Git application creation page, fill in the necessary parameters, and save.

![Minion](../../../assets/images/gitops/app-create-en.jpg)
parameter settings:
* Git application name
* Git applies sync strategy:
Manual: need to manually click the page to trigger
Automatic: Triggered automatically when Git changes
* Git repository used by Git application
* The version, branch, tag or commitID of the Git repository used by the Git application
* The path to the Git repository used by the Git application
* Select the target cluster where the Git application is installed
* Select the namespace of the target cluster where the Git application is installed


### Application Details
Click the link in the "Git Applications" list to enter the Git application details page.
![Minion](../../../assets/images/gitops/app-info1-en.jpg)
Git application topology
![Minion](../../../assets/images/gitops/app-info2-en.jpg)
Git application resources
![Minion](../../../assets/images/gitops/app-info3-en.jpg)
Git repository information
![Minion](../../../assets/images/gitops/app-info4-en.jpg)
Git application sync state with Git repository
![Minion](../../../assets/images/gitops/app-info5-en.jpg)
Git application yaml information
![Minion](../../../assets/images/gitops/app-info7-en.jpg)
Yaml support operations
* update
* apply
* merge

Git application event information
![Minion](../../../assets/images/gitops/app-info6-en.jpg)
### delete
Select the Git application to be deleted, click the multi-select box to select, click the "Delete" button, and enter "yes" in the confirmation input box to complete the deletion operation.
### refresh
Click "Refresh" to complete the refresh of the Git application list.