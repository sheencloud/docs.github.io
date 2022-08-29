# Helm Chart

## Install hyperkuber via Helm chart
1. Add hyperkuber chart repo
````
helm repo add hyperkuber https://charts.sheencloud.com
````
2, Download the chart package
````
helm pull sheencloud/hyperkuber
````
1. Modify the default value of Values.yaml
````
# Currently hyperkuber's chart depends on mysql, redis components, and the chart comes from bitnami. Please modify the default configuration of values during installation
# mysql: https://raw.githubusercontent.com/bitnami/charts/master/bitnami/mysql/values.yaml
# redis: https://raw.githubusercontent.com/bitnami/charts/master/bitnami/redis/values.yaml
````

4. Install Chart
````
helm install hyperkuber hyperkuber/hyperkuber -n hyperkuber --create-namespace
````