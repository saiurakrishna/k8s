# k8s
K8s configuration files

##### Commands #####
kubectl label node <node-name> key=value   

kubectl describe pod elephant  | grep -A5 State: 

kubectl replace -f elephant.yaml --force {This command will delete the existing one first and recreate a new one from the YAML file}

kubectl top node { To check memory and cpu of nodes } 

kubectl top node --sort-by='memory' --no-headers | head -1 

kubectl top pod { to view the perfomance metrics } 

kubectl top pod --sort-by='cpu' --no-headers | tail -1 {Here we have used tail -1 to list the last pod in the list, which is the pod that uses the least CPU(cores) }
