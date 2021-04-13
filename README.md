# развернуть Redis

`kubectl apply -f welltory-redis.yaml`

развернуть Prometheus

kubectl apply -f welltory-prom.yaml

будет создан 
manespace: welltory
redis cluster statefulset: 3 nodes
prometheus: 

Deploy redis exporter
helm install --namespace welltory --name redis-monitoring-prometheus-redis-exporter stable/prometheus-redis-exporter --set redisAddress=redis://redis-cluster:6379

Задача для middle

1 Применить манифесты
Task:
Применить манифесты
HowTo

git clone bla
или
git pull в репозитории
развернуть Redis
kubectl apply -f welltory-redis.yaml
развернуть Prometheus
kubectl apply -f welltory-prom.yaml

2 Обновить версию прометеуса
Task:
Обновить версию прометеуса
HowTo:
в welltory-prom.yaml d cnhjrt 136 заменить v2.10.0 на последнюю с dockerhub
затем
kubectl apply -f welltory-prom.yaml передеплоить стек

