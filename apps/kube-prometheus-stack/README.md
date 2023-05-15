
```shell
# Add the prometheus-community helm registry
helm repo add prometheus-community https://prometheus-community.github.io/helm-charts
helm repo update

# Install/upgrade kube-prometheus-stack
helm upgrade --install kps prometheus-community/kube-prometheus-stack -f values.yaml -n monitoring
```
