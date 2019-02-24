# k8s-redis-cluster

kubectl create -f persistentvolume

kubectl create -f persistentvolumeclaims

kubectl create configmap redis-conf --from-file=redis.conf

kubectl apply -f redis-headless.yaml

kubectl apply -f redis.yaml
