# Operator
## install by Operator
```
apiVersion: operator.hyperkuber.io/v1
kind: Hkcmp
metadata:
  name: hkcmp-sample
  namespace : default
spec:
  namespace: default
  managed: true
  strategy: demo 
```

```
apiVersion: operator.hyperkuber.io/v1
kind: Hkcmp
metadata:
  name: hkcmp-sample
  namespace : default
spec:
  namespace: default
  config:
    mysql:
      host: "127.0.0.1"
      port: 3306
      username: "root"
      password: "Kingsoft123"
      database: "hyperkuber"
      migerate: true
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
    image: sheencloud/hyperkuber-server:v1
    serviceType: NodePort
  web:
    replicas: 1
    image: sheencloud/hyperkuber-web:v1
    serviceType: NodePort
  ingress:
    hosts:
      - hyperkuber.cloud.local
    tls:
      - hosts:
          - hyperkuber.cloud.local
        secretName: hyperkuber-cloud-local-tls

```