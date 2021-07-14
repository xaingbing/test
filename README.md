cd busybox-helm-master
helm install --name zetian --namespace devops .
helm upgrade zetian --namespace devops .
kubectl delete job demo-hook -n devops
# kubectl delete job db-init -n devops
helm delete zetian --purge --key XXX
