#Helm Chart

## Install hyperkuber via Helm chart
1. Add hyperkuber chart repo
````
helm repo add harbor https://sheencloud.com/charts
````
2, Download the chart package
````
helm pull sheencloud/hyperkuber

````
3. Modify the default value of Values.yaml
````
# Currently hyperkuber's chart depends on mysql, redis components, and the chart comes from bitnami. Please modify the default configuration of values during installation
# mysql: https://raw.githubusercontent.com/bitnami/charts/master/bitnami/mysql/values.yaml
# redis: https://raw.githubusercontent.com/bitnami/charts/master/bitnami/redis/values.yaml
````

4. Install Chart
````
helm install hkcmp -f hyperkuber-0.1.0.tgz -n hyperkuber --create-namespace
````