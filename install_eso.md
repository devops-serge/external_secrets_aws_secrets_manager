```shell
helm repo add external-secrets https://charts.external-secrets.io

helm repo update

helm install external-secrets external-secrets/external-secrets

kubectl get pod -w
```
