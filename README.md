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



helm repo index --url https://raw.githubusercontent.com/sacloudworld/helmfile/master/ .    (master is  branch)

helm repo list


https://raw.githubusercontent.com/username/repository/main/path/to/file


curl -O https://raw.githubusercontent.com/sacloudworld/helmfile/master/user-app-0.1.0.tgz
