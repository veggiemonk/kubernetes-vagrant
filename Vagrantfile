# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  # Specify your hostname if you like
  # config.vm.hostname = "name"
  config.vm.box = "bento/ubuntu-16.04"
  config.vm.network "private_network", type: "dhcp"
  # config.vm.provision "shell", path: "install_k8s_crio"
  config.vm.provision "shell", path: "install_k8s_docker"
end
