sudo kubectl get pods --no-headers | grep 'gitlab' | awk '{print $1}' | xargs kubectl delete pod

kubectl get statefulsets

kubectl get deployments

kubectl apply -f https://raw.githubusercontent.com/metallb/metallb/v0.11.0/manifests/namespace.yaml

kubectl apply -f https://raw.githubusercontent.com/metallb/metallb/v0.11.0/manifests/metallb.yaml




sudo kubeadm init phase certs all --config=kubeadm-config.yaml


kubectl label nodes <node-name> node-role.kubernetes.io/worker=worker



kubectl taint nodes masternode node-role.kubernetes.io/master:NoSchedule


kubectl proxy --address 0.0.0.0 --accept-hosts '.*'
