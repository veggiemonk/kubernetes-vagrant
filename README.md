# Kubernetes Vagrant

Spin up a single kubernetes node in a VM and use kubectl to manage it.

~~Based on [this article](https://medium.com/@lizrice/kubernetes-in-vagrant-with-kubeadm-21979ded6c63) written by [Liz Rice](https://github.com/lizrice)~~

Just use https://microk8s.io/


## Start

```bash
# start the VM
$ vagrant up
# SSH into the VM
$ vagrant ssh
# Try kubectl
$ microk8s.kubectl get nodes
# list addons, there are lots of them :D
$ microk8s.status
```


Feedback and contributions are more than welcome.
