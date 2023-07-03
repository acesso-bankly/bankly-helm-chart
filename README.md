# bankly-helm-chart

# https://github.com/acesso-bankly/bankly-helm-chart
# https://acesso-bankly.github.io/bankly-helm-chart

execute these commands to generate helm chart

```sh
helm lint bankly-curity

helm package bankly-curity

helm repo index --url https://acesso-bankly.github.io/bankly-helm-chart .

```

# test locally

```sh
helm install deploy-bankly-product ./bankly-product --dry-run --debug
```