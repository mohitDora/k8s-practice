kubectl apply -f <file_name>
kubectl get <resource_name> [name]
ex : kubectl get pods, kubectl get pod <name>, kubectl get all, kubectl get pods -n <namespace>
kubectl describe <resource_name> <name>
kubectl logs <pod_name> | -c <container_name>
kubectl exex -it <pod_name> [ -c container_name ] --command 
kubectl delete <resource_name> <name> | -f <file_name>

#taint
kubectl taint nodes <node_name> <key>=<value>:<effect>
#untaint
kubectl taint nodes <node_name> <key>=<value>:<effect>-

#helm
helm repo add <repo_name>
helm serach repo <repo_name>
helm install <release_name> <chart_name>

#upgrade a release
helm upgrade <release_name> <chart_name> --version <some_version>

#show helm history
helm history <release_name>

#rollback a release
helm rollback <release_name> <revision>

#unistall a release
helma unistall <release_name>