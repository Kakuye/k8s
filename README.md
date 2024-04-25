sudo kubectl get pods --no-headers | grep 'gitlab' | awk '{print $1}' | xargs kubectl delete pod

kubectl get statefulsets

kubectl get deployments

kubectl apply -f https://raw.githubusercontent.com/metallb/metallb/v0.11.0/manifests/namespace.yaml
kubectl apply -f https://raw.githubusercontent.com/metallb/metallb/v0.11.0/manifests/metallb.yaml
