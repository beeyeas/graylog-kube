# graylog-kube
# graylog cluster in kubernetes
# Steps to install graylog cluster 

### 1. Make sure kubectl is up and working , connecting to kubenetes
### 2. Run graylog cluster 
```
 kubectl create -f elasticsearch-deployment.yaml,elasticsearch-service.yaml,graylog-service.yaml,graylog-deployment.yaml,mongo-service.yaml,mongo-deployment.yaml
```
### 3. Forward port 9000 
```
 kubectl port-forward graylog-3226681439-97w36 9000:9000
```