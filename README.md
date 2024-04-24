sudo kubectl get pods --no-headers | grep 'gitlab' | awk '{print $1}' | xargs kubectl delete pod
