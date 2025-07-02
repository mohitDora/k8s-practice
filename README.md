# Kubernetes & Helm Command Reference

## Basic kubectl Commands

```sh
kubectl apply -f <file_name>
kubectl get <resource_name> [name]
# ex: kubectl get pods, kubectl get pod <name>, kubectl get all, kubectl get pods -n <namespace>
kubectl describe <resource_name> <name>
kubectl logs <pod_name> | -c <container_name>
kubectl exex -it <pod_name> [ -c container_name ] --command 
kubectl delete <resource_name> <name> | -f <file_name>
```

## Node Taints

```sh
# taint
tkubectl taint nodes <node_name> <key>=<value>:<effect>
# untaint
kubectl taint nodes <node_name> <key>=<value>:<effect>-
```

## Helm Commands

```sh
# Add a repo
helm repo add <repo_name>
# Search repo
helm serach repo <repo_name>
# Install a release
helm install <release_name> <chart_name>
```

### Upgrade a Release

```sh
helm upgrade <release_name> <chart_name> --version <some_version>
```

### Show Helm History

```sh
helm history <release_name>
```

### Rollback a Release

```sh
helm rollback <release_name> <revision>
```

### Uninstall a Release

```sh
helma unistall <release_name>
``` 