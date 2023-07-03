### bankly-helm-chart

- [repo](https://github.com/acesso-bankly/bankly-helm-chart)
- [usage link chart](https://acesso-bankly.github.io/bankly-helm-chart)

execute these commands to generate helm chart

```sh
helm lint bankly-curity

helm package bankly-curity

helm repo index --url https://acesso-bankly.github.io/bankly-helm-chart .

```

### test locally

```sh

helm install deploy-bankly-product ./bankly-product --dry-run --debug

```

### upgrade 

```sh

helm upgrade -f .\stepllader-values.yaml --set isCanary=false,enviroment="production" -i "namespace.service-name" bankly-helm/bankly-product --dry-run --debug

```

### repository 

````sh

helm repo add bankly-helm https://acesso-bankly.github.io/bankly-helm-chart

```