# Ingress

One of the way to get cluster load balancer and public IP.
Plusserver https://docs.plusserver.com/en/container/managed-kubernetes/tutorials/lb_configuration/[load balancer docs].

```shell
helm repo add ingress-nginx https://kubernetes.github.io/ingress-nginx
```


```shell
helm repo update

```


```shell
helm install ingress-nginx ingress-nginx/ingress-nginx \
  --namespace ingress-nginx --create-namespace \
  -f ./utilities/ingress/values.yaml

```

```shell
helm upgrade --install ingress-nginx ingress-nginx/ingress-nginx \
  --namespace ingress-nginx --create-namespace \
  -f ./utilities/ingress/values.yaml
```