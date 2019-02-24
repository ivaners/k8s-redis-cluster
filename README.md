# k8s-redis-cluster

kubectl create -f persistentvolume

kubectl create -f persistentvolumeclaims

kubectl create configmap redis-conf --from-file=redis.conf

kubectl apply -f redis-headless.yaml

kubectl apply -f redis.yaml

#### 使用redis-trib激活集群，如：
```
docker run --rm -it inem0o/redis-trib create --replicas 1 172.19.165.222:8001 172.19.165.222:8002 172.19.165.222:8003 172.19.165.222:8004 172.19.165.222:8005 172.19.165.222:8006
```
