# kubernetes-reloader

[Reloader](https://github.com/stakater/Reloader) can watch changes in ConfigMap and Secret and do rolling upgrades on Pods with their associated DeploymentConfigs, Deployments, Daemonsets Statefulsets and Rollouts.

## Installing the Chart
To install the chart with the release name `reloader`:
```bash
kubectl create ns reloader
helm install reloader . -f values.yaml -n reloader
```

## Uninstalling the Chart
To uninstall the `reloader` deployment:
```bash
helm uninstall reloader -n reloader
kubectl delete ns reloader
```
The command removes all the Kubernetes components associated with the chart and deletes the release.