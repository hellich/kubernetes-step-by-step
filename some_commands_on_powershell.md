# Useful commands

kubectl version  ==> check kubernetes version

kubectl cluster-info ==> view cluster information

kubectl get all ==> retrieve information about kubernetes pods, deployments, services and more
kubectl run [container-name] --image=[image-name] ==> simple way to create a deployment for a pod

kubectl port-forward [pod] [ports] ==> forward a port to allow external access

kubectl expose ... ==> expose a port for a deployment/pod

kubectl create [resource] ==> create a resource

kubectl apply [resource] ==> create or modify a resource

kubectl run [podname] --image=nginx:alpine ==> run the nginx:alpine container in a pod

kubectl port-forward [podname] 8080:80 ==> enable pod container to be called externally. 8080 is the external port to call from a web browser (for instance), 80 is the internal port used by the application running inside the container

kubectl get pods ==> lists pods

kubectl delete pod [podname] ==> will cause pod to be recreated (il will kill the running pod and create a new one since kubernetes maintain the current state)

kubectl delete deployment [name-of-deployment] ==> delete deployment that manages the pod

kubectl get pod my-nginx -o yaml ==> get details of the pod my-nginx

kubectl describe pod my-nginx ==> get details of the pod (with a list of events)

# kuberenetes web ui dashboard

kubectl describe secret -n kube-system ==> get tokens

kubectl apply -f https://raw.githubusercontent.com/kubernetes/dashboard/v2.0.0/aio/deploy/recommended.yaml ==> run a pod with ui dashboard
kubectl proxy ==> Kubectl will make Dashboard available at http://localhost:8001/api/v1/namespaces/kubernetes-dashboard/services/https:kubernetes-dashboard:/proxy/.
