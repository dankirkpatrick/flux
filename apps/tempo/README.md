Test
```shell
# Add the grafana helm registry
helm repo add grafana https://grafana.github.io/helm-charts
helm repo update

# Install/upgrade kube-prometheus-stack
helm upgrade --install tempo grafana/tempo-distributed -f base/values.base.yaml -f truenas/values.yaml -n tempo
```
