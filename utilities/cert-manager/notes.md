# Cert manager

https://cert-manager.io/docs/installation/helm/


## Installing with Helm


### Install


```shell
helm install example ./utilities/cert-manager/helm  --namespace cert-manager --create-namespace
```

```shell
helm dependency update

```

```shell
kubectl apply -f utilities/cert-manager/clusterissuer.yaml
```

### Install simulation

helm install simulation ./../landing-pages/simulation  --create-namespace --namespace simulation

helm upgrade --install simulation ./../landing-pages/simulation --create-namespace --namespace simulation