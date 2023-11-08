# Spinning up and configuring Kind cluster

This installs:
* Docker
* kubectl
* Kind with local Docker registry
* MetallLb load balancer

After the script is done, you should be seeing something like this:
```
kubectl get pods -A
NAMESPACE            NAME                                         READY   STATUS    RESTARTS        AGE
kube-system          coredns-5d78c9869d-8w7qm                     1/1     Running   1 (8m7s ago)    115m
kube-system          coredns-5d78c9869d-vm6r5                     1/1     Running   1 (8m7s ago)    115m
kube-system          etcd-kind-control-plane                      1/1     Running   1 (8m7s ago)    115m
kube-system          kindnet-bvv22                                1/1     Running   1 (8m7s ago)    115m
kube-system          kube-apiserver-kind-control-plane            1/1     Running   1 (8m7s ago)    115m
kube-system          kube-controller-manager-kind-control-plane   1/1     Running   2 (8m7s ago)    115m
kube-system          kube-proxy-qgzvg                             1/1     Running   1 (8m7s ago)    115m
kube-system          kube-scheduler-kind-control-plane            1/1     Running   1 (8m7s ago)    115m
local-path-storage   local-path-provisioner-6bc4bddd6b-vjv62      1/1     Running   2 (6m57s ago)   115m
metallb-system       controller-789c75c689-x9z7g                  1/1     Running   2 (6m56s ago)   110m
metallb-system       speaker-7llsn                                1/1     Running   2 (6m56s ago)   110m
```