#user app
Link:
https://github.com/helm/helm/releases




helm create user-app

Connect to eks cluster:  aws eks --region us-east-1 update-kubeconfig --name sa-cluster

helm install user-app-release user-app

helm list -a


helm status user-app-release

kubectl get service

helm uninstall user-app-release user-app

helm install user-app-release --debug  --dry-run user-app


helm upgrade user-app-release user-app



helm repo index --url https://github.com/sacloudworld/helmfile/master/ .    (master is  branch)

https://raw.githubusercontent.com/sacloudworld/helmfile/master/