kubectl create -f .\nginx.pod.yml --dry-run=client --validate=true ==> dry run mode

kubectl create -f .\nginx.pod.yml ==> creates a pod / will fail if the pod already exists

kubectl create -f .\nginx.pod.yml ==> creates a pod and store its config/state annotations. So we can use apply after

kubectl apply -f .\nginx.pod.yml ==> creates a pod or update it if already exist

kubectl delete -f .\nginx.pod.yml ==> delete pod using yaml file

kubectl exec my-nginx -it sh ==> enter to the container

kubectl edit -f .\create_nginx_pod_with_yaml\nginx.pod.yml ==> edit a pod's yaml file live