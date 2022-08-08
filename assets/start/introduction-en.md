# Architecture

The HyperKuber container management platform consists of four components, namely front-end web service, back-end API service, database service (MySQL) and cache (Redis) service.

![hykuber-arc](/assets/images/hyperkuber-arc.png)


HyperKuber supports flexible deployment methods, and all its components support containerized deployment. All components can be deployed either in the cluster or separately outside the cluster, such as using docker compose.
Both HyperKuber Web services and API Server services are stateless services, which can be scaled horizontally and support multiple copies to provide high availability and offloading. When deployed in a production environment, external high-availability MySQL clusters and Redis clusters can be configured.

## component list

| Name | Description |
| ------ | ------------- |
| hyperkuber-web | Front-end UX service, providing user interface. |
| hyperkuebr-server | Backend API service, providing API and business logic functions. |
| mysql | Database Services, mysql 8+. It can be configured to connect to existing external services. |
| redis | Cache service, which can be configured to connect to existing external services. |


## Dependency Services
| Name | Description |
| ------ | ------------- |
| kuernetes* | Managed kubernetes cluster. |
| prometheus* | Monitoring services, prometheus and alertmanager. |
| harbor | Image repository service. |
| argocd | Gitops service. |
| elasticsearch | Log query service. |

> `*` are required services, others are optional services, and the corresponding functions are unavailable when they do not exist.


# Features

## Overview

The core functions of HyperKuber can be summarized in the following six dimensions:

![concept](/assets/images/hyperkuber-arc-concept.png)


The feature set included in each dimension is as follows:


![funcset](/assets/images/hyperkuber-arc-func.png)



## Features

+ ### Multi-cluster management

HyperKuber supports unified management of multiple clusters, and one-click release of applications for multiple clusters. HyperKuber can manage clusters regardless of whether they are in an on-premises data center or public cloud, as long as the network is reachable. At the same time, HyperKuber provides platform-level RBAC functions. In a multi-cluster environment, it is no longer necessary to rely on Kubernetes' RBAC to maintain user roles and permission assignments, reduce operation and maintenance pressure, and improve security and maintainability.

+ ### Real-time observability

HyperKuber supports real-time monitoring of cluster resources, events, logs, etc. Real-time control of cluster resource status for debugging and problem investigation.

+ ### Resource topology

HyperKuber supports Kubernetes resource topology display, resource dependencies and status can be seen at a glance. Application topology, resource topology and namespace topology are supported.

+ ### Powerful and easy to use

HyperKuber provides rich resource creation wizard functions. For beginners, you can operate and manage resources even if you don’t know YAML. For Kubernetes senior managers, while providing wizards and forms to create resources, the YAML editing function is still retained, and resources can still be managed through YAML. The life cycle.

+ ### Tenant Support

HyperKuber provides two-level multi-tenant management functions. The first level is the namespace level. Based on the namespace, it provides two-level multi-tenant resource management and control, and tenant resources can be managed and allocated across clusters.


+ ### Agentless

HyperKuber adopts an agentless implementation method in its architecture design, that is, it does not need to deploy any agent component services on the managed cluster, and does not occupy the resources of the managed cluster. Except for some usage scenarios (such as webhook authentication, which is not required), the managed cluster does not need to make any configuration changes, and only needs to ensure the network connectivity between the API Server service and the managed cluster.

+ ### Security Compliance

When the new version of HyperKuber is released, its Web service image and API Server image have been scanned to ensure that it has no CVE vulnerability. TLS encrypted communication is supported when the API Server service communicates with the Kubernetes cluster. HyperKuber supports offline deployment and installation, and all its components can work normally in offline mode. HyperKuber does not collect any customer data during installation or operation, except for the data required for license activation, and is fully GDPR compliant. For details, please refer to our [Privacy Policy](https://www.sheencloud.com/privacy-policy/).


---