#create a nginx pod with port forwarding


kubectl run my-nginx --image=nginx:alpine ==> creates a pod with nginx container

kubectl get pods ==> lists pods

kubectl port-forward my-nginx 8080:80 ==> port forwarding from 80 (internal port of nginx) to 8080 (external port that we can access from a browser)

kubectl delete pod my-nginx ==> deletes pod
