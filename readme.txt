kubectl apply -f <file_name>
kubectl get <resource_name> [name]
ex : kubectl get pods, kubectl get pod <name>, kubectl get all, kubectl get pods -n <namespace>
kubectl describe <resource_name> <name>
kubectl logs <pod_name> | -c <container_name>
kubectl exex -it <pod_name> [ -c container_name ] --command 
kubectl delete <resource_name> <name> | -f <file_name>
