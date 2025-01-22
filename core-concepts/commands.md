# Kubernetes Commands

## Namespace Operations
`kubectl create namespace test` - Creates a new namespace named test

`kubectl get namespace` - Lists all available namespaces

`kubectl delete namespace test` - Deletes specified namespace

## Pod Operations
`kubectl run nginx --image=nginx` - Creates a pod running nginx

`kubectl get pods` - Shows all running pods

`kubectl describe pod nginx` - Displays detailed pod information

`kubectl delete pod nginx` - Removes specified pod

`kubectl logs nginx` - Shows pod's container logs

`kubectl exec -it nginx -- bash` - Opens shell inside pod

## Deployment Operations
`kubectl create deployment web --image=nginx` - Creates new deployment

`kubectl get deployments` - Lists all deployments

`kubectl scale deployment web --replicas=3` - Scales deployment replicas

`kubectl rollout undo deployment/web` - Reverts last deployment

`kubectl set image deployment/web nginx=1.9` - Updates container image

## ReplicaSet Operations
`kubectl get rs` - Shows all replicasets

`kubectl scale rs web --replicas=3` - Changes replicaset size

`kubectl delete rs web` - Removes replicaset

## Quota Operations
`kubectl create quota dev-quota --hard=cpu=2` - Sets resource quota

`kubectl get quota` - Lists all quotas

`kubectl describe quota dev-quota` - Shows quota details

`kubectl delete quota dev-quota` - Removes quota
