# kubeadm-installation (v1.22)

## server (K8 v1.22.6)
 ```bash
curl https://raw.githubusercontent.com/JosephYostos/kubeadm-installation/main/master.sh |bash
 ```
 
## Worker (K8 v1.22.6)
 ```bash
curl https://raw.githubusercontent.com/JosephYostos/kubeadm-installation/main/worker.sh |bash
 ```
 
## install calico CNI (v3.22)

 ```bash
kubectl create -f https://projectcalico.docs.tigera.io/archive/v3.22/manifests/tigera-operator.yaml
kubectl create -f https://projectcalico.docs.tigera.io/archive/v3.22/manifests/custom-resources.yaml
 ```

# kubeadm-installation (v1.25)

## server (K8 v1.25.6)
 ```bash
curl https://raw.githubusercontent.com/JosephYostos/kubeadm-installation/main/master_125.sh |bash
 ```
 
## Worker (K8 v1.25.6)
 ```bash
curl https://raw.githubusercontent.com/JosephYostos/kubeadm-installation/main/worker_125.sh |bash
 ```
 
## install calico CNI (v3.24)

 ```bash
kubectl create -f https://raw.githubusercontent.com/projectcalico/calico/v3.24.5/manifests/tigera-operator.yaml
kubectl create -f https://raw.githubusercontent.com/projectcalico/calico/v3.24.5/manifests/custom-resources.yaml
 ```





## Troubleshooting claico installation

 ```bash
kubectl get installer default --namespace calico-cloud -o jsonpath --template '{.status}'
kubectl get tigerastatus 
 ```
