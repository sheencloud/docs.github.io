# App release

HyperKuber supports a variety of application publishing methods. Publish the application to multiple clusters in the form of configurable parameters.

## apply template

An application template is a collection of kubernetes resources. The resources required for application deployment, such as deployment, service, configmap, etc., are made into a unified template. Through configurable parameter variables, applications can be easily and quickly deployed to different clusters. middle. The application template supports both public and private modes. The private template can only be seen by the currently created user. When the application template is tested and stabilized, it can be set to public and used as a middleware service for other teams to use.

The application template supports template parameter configuration and one-click publishing to multiple clusters when publishing.

### Applications

An application instance is an application instance management object generated after the template is deployed. Instances can manage the life cycle of the application. On the instance topology page, you can easily view the status of the application in all deployed clusters.

> Application templates are fully compatible with OpenShift Templates.


##Helm

HyperKuber provides a complete deployment solution for Helm applications. Helm warehouse management provides the docking synchronization function for remote Helm warehouses, and synchronizes Chart packages in the remote warehouse to the local, which is convenient for rapid deployment. The Chart can be quickly published to multiple clusters through the Chart Publishing Wizard. It also supports providing configuration parameters for each cluster individually. Through the Helm instance, you can easily view, update, and manage the life cycle of the chart package in all clusters.

## Operator


HyperKuber supports Operator-type application deployment methods. Whether it is the community's OLM or the OCP's Operatorhub, HyperKuber supports the docking and deployment of operators. Create a resource object supported by the operator and manage the operator life cycle.

___