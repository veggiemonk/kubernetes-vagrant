# Kubernetes Vagrant

Spin up a single kubernetes node in a VM and use kubectl to manage it.

Based on [this article](https://medium.com/@lizrice/kubernetes-in-vagrant-with-kubeadm-21979ded6c63) written by [Liz Rice](https://github.com/lizrice)

This repo will try to automate things in order to provide fast feedback when testing something on kubernetes.



## Start

```bash
vagrant up
```


1. Search for vagrant logs for: `This VM has IP address`
2. SSH into the vagrant box: `vagrant ssh`
3. Copy the kubeconfig to the local filesystem: `cp /home/vagrant/.kube/config /vagrant/kubeconfig`
4. Modify the server IP address of the kubeconfig file
5. `export KUBECONFIG=$PWD/kubeconfig`
6. Test with: `kubectl get nodes -n kube-system`





Feedback and contributions are more than welcome.
