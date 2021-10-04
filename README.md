# elk-k8s
kubectl create configmap log-manual-pipeline --from-file ./logstash.conf -n elastic-dev

# Other

kubectl create configmap beat-manual-config --from-file ./other/filebeat.yaml -n elastic-dev

kubectl create -f ./other/deployment.yaml -n elastic-dev
