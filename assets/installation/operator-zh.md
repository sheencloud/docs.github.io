# Operator
## 通过Operator安装 hyperkuber

### 安装hyperkuber-controller

```
kubectl apply -f https://manifests.sheencloud.com/manifest/operator.yaml
```
### demo模式安装hyperkuber
```
apiVersion: operator.hyperkuber.io/v1
kind: Hkcmp
metadata:
  name: hkcmp-sample
spec:
  managed: true
  strategy: demo 
```
注释：
managed： true表示hyperkuber的组件由operator管理整个生命周期
strategy：目前支持两种：demo，prod。
demo使用emptyDir存储，创建hyperkuber相关组件。
prod需配置hyperkuber组件（hyperkuber-server）使用存储，以及配置集群外的Mysql，Redis集群，Ingress方式Hosts名称


### prod模式安装hyperkuber
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
      password: "hyper ku b er"
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
注释：
spec.config
Mysql配置
```
host: "127.0.0.1" ## mysql地址
port: 3306 ##mysql端口
username: "root" ##mysql登陆用户名
password: "hyperkuber" ##mysql登陆密码
database: "hyperkuber" ##mysql数据库名称
migerate: true ##默认为true，自动创建mysql数据库表以及导入mysql数据
log: "DEBUG" ##golang gorm操作mysql日志级别
```
Redis配置
```
addr: "127.0.0.1:6379" ## redis地址
password: "" ## redis密码
```
hyperkuber组件配置
```
 storage: ##存储配置，参照k8s volume配置
    emptyDir: {}
  server: ## hyperkuber-server配置
    replicas: 1
    image: sheencloud/hyperkuber-server:latest
    serviceType: NodePort
  web: ## hyperkuber-server配置
    replicas: 1
    image: sheencloud/hyperkuber-web:latest
    serviceType: NodePort
  ingress: ## hyperkuber ingress 配置
    hosts:
      - console.hyperkuber.io
    tls:
      - hosts:
          - console.hyperkuber.io
        secretName: hyperkuber-cloud-local-tls ## hyperkuber ingress证书配置
```