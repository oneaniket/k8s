# k8s commands

| Command | Description |
| ------------- | ------------- |
| kubectl cluser-info | Get kubernetes cluster information |
| kubectl config veiw | View the config of cluster |
| kubectl get namespaces | View the config of cluster |
| kubectl create namespace name | Create a namespace |
| kubectl delete namespace name | delete namespace |
| kubectl get nodes | Get information about nodes which are part of the cluster |
| kubectl get pods  | Get all pods running in a current namespace |
| kubectl get pods -o wide | Get information about nodes which are part of the cluster |
| kubectl get pods --all-namespaces | Get information about nodes which are part of the cluster |
| kubectl run podname --image=<image_name> | Create a pod |
| kubectl logs -f podsname | View logs of running pod |
| kubectl exec -it podname -- /bin/bash | Interactive shell access to a running pod |  
| Kubectl delete pods podname | Delete a pod |  
| kubectl create deployment nginx --image=nginx | Create deployment object with command |
| kubectl scale deployment nginx --replicas=2 | Scale replicas of a deployment |  
| kubectl set image deployment nginx nginx=nginx:1.18.0-alpine | Rolling udpate for nginx deployment |  
| kubectl rollout undo deployment nginx | Rollback to previous deployment |
| kubectl apply -f filename | Deploy objects defined in the file|
| kubectl delete -f filename | Delete objects defined in the file |
| kubectl expose deployment nginx --type NodePort --port 80 --target-port 80 | Expose deployment nginx with NodePort service |
| kubectl get pods --selector app=apache | Get all pods with label app=apache | 
| kuebctl create configmap myconfig --from-literal=env=dev | Create configmap imperative command |
| kubectl create secret generic mysecret1 --from-literal=username=admin | Create secret with imperative command |
| kubectl get pods/nodes --show-labels | View lables on object |
| kubectl lable nodes name_of_node key=value | Add label to specified node |



