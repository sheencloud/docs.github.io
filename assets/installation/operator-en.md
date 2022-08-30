# Operator
## Install hyperkuber via Operator

### Install hyperkuber-controller

```
kubectl apply -f https://manifests.sheencloud.com/manifest/operator.yaml
```
### Install hyperkuber in demo mode
```
apiVersion: operator.hyperkuber.io/v1
kind: Hkcmp
metadata:
  name: hkcmp-sample
spec:
  managed: true
  strategy: demo
```
Notes:
managed: true indicates that the components of hyperkuber are managed by the operator throughout the life cycle
strategy: Currently supports two kinds: demo, prod.
The demo uses emptyDir storage to create hyperkuber related components.
Prod needs to configure the hyperkuber component (hyperkuber-server) to use storage, and configure the name of Mysql, Redis cluster, and Ingress mode Hosts outside the cluster


### install hyperkuber in prod mode
```
apiVersion: operator.hyperkuber.io/v1
kind: Hkcmp
metadata:
  name: hkcmp-sample
spec:
  config:
    mysql:
      host: "127.0.0.1"
      port: 3306
      username: "root"
      password: "hyperkuber"
      database: "hyperkuber"
      migrate: true
      log: "DEBUG"
    redis:
      addr: "127.0.0.1:6379"
      password: ""
  managed: true
  strategy: prod
  storage:
    emptyDir: {}
  server:
    replicas: 1
    image: sheencloud/hyperkuber-server:latest
    serviceType: NodePort
  web:
    replicas: 1
    image: sheencloud/hyperkuber-web:latest
    serviceType: NodePort
  ingress:
    hosts:
      - console.hyperkuber.io
    tls:
      - hosts:
          - console.hyperkuber.io
        secretName: hyperkuber-cloud-local-tls
```
Notes:
spec.config
Mysql configuration
```
host: "127.0.0.1" ##mysql address
port: 3306 ##mysql port
username: "root" ##mysql login username
password: "hyperkuber" ##mysql login password
database: "hyperkuber" ##mysql database name
migrate: true ##default is true, automatically create mysql database table and import mysql data
log: "DEBUG" ##golang gorm operates mysql log level
```
Redis configuration
```
addr: "127.0.0.1:6379" ## redis address
password: "" ## redis password
```
hyperkuber component configuration
```
 storage: ##Storage configuration, refer to k8s volume configuration
    emptyDir: {}
  server: ## hyperkuber-server configuration
    replicas: 1
    image: sheencloud/hyperkuber-server:latest
    serviceType: NodePort
  web: ## hyperkuber-server configuration
    replicas: 1
    image: sheencloud/hyperkuber-web:latest
    serviceType: NodePort
  ingress: ## hyperkuber ingress configuration
    hosts:
      - console.hyperkuber.io
    tls:
      - hosts:
          - console.hyperkuber.io
        secretName: hyperkuber-cloud-local-tls ## hyperkuber ingress certificate configuration
```