```shell
kubectl create secret generic awssm-secret \
  --from-literal=access-key=XXXXX \
  --from-literal=secret-access-key=XXXXX

kubectl apply -f secretstore.yaml
kubectl get secretstore

kubectl apply -f externalsecret.yaml
kubectl get externalsecret

kubectl get secret

kubectl get secret aws-secret -o yaml | grep secret-key | head -n1

echo dmFsdWU= | base64 -d
```
