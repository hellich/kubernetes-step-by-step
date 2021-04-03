# Useful commands

kubectl version  ==> check kubernetes version

kubectl cluster-info ==> view cluster information

kubectl get all ==> retrieve information about kubernetes pods, deployments, services and more
kubectl run [container-name] --image=[image-name] ==> simple way to create a deployment for a pod

kubectl port-forward [pod] [ports] ==> forward a port to allow external access

kubectl expose ... ==> expose a port for a deployment/pod

kubectl create [resource] ==> create a resource

kubectl apply [resource] ==> create or modify a resource


# kuberenetes web ui dashboard

kubectl describe secret -n kube-system ==> get tokens

kubectl apply -f https://raw.githubusercontent.com/kubernetes/dashboard/v2.0.0/aio/deploy/recommended.yaml ==> run a pod with ui dashboard
kubectl proxy ==> Kubectl will make Dashboard available at http://localhost:8001/api/v1/namespaces/kubernetes-dashboard/services/https:kubernetes-dashboard:/proxy/.
