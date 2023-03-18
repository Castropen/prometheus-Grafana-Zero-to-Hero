# Install using Helm

## Add helm repo

`helm repo add grafana https://grafana.github.io/helm-charts`

## Update helm repo

`helm repo update`

## Install helm 

`helm install grafana grafana/grafana`

## Expose Grafana Service

`kubectl expose service grafana --ype=NodePort --target-port=3000 --name=grafana-ext`
# To expose to browser 
'minikube sevice grafana-ext'
