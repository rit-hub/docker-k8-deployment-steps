## configure with Access key 

```
aws configure
```

## connecting EKS cluster from EC2 instance

```
aws eks update-kubeconfig --name ritam-eks-cluster
kubectl get nodes
```

## creating kubernates deployment and services

```
cd files-k8/home-insurance-k8
ls

kubectl apply -f db.yaml
kubectl apply -f app.yaml

kubectl get pods
kubectl get svc
```

now connect with external ip
e.g. http://adeb375d4d1b84e29afd911bf6a9b982-1648485156.us-east-1.elb.amazonaws.com:7090/

## connect postgreSQL DB from k8s

-h service name -U username

```
kubectl exec -it postgres-db-754b7c5f84-wp2xj -- bash
PGPASSWORD=admin psql -h postgres-db -U postgres
\l
```
