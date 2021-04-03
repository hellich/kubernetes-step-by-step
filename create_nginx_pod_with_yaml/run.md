kubectl create -f .\nginx.pod.yml --dry-run=client --validate=true ==> dry run mode

kubectl create -f .\nginx.pod.yml ==> creates a pod / will fail if the pod already exists

kubectl create -f .\nginx.pod.yml ==> creates a pod and store its config/state annotations. So we can use apply after

kubectl apply -f .\nginx.pod.yml ==> creates a pod or update it if already exist

kubectl apply -f .\nginx.pod.yml ==> delete pod using yaml file
