# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  # Specify your hostname if you like
  # config.vm.hostname = "name"
  
  config.vm.box = "bento/ubuntu-18.04"
  
  # Virtualbox
  config.vm.provider "virtualbox" do |v|
    v.memory = 4096
    v.cpus = 2
  end
  
  config.vm.network "private_network", type: "dhcp"
  config.vm.provision "shell", path: "snap_microk8s"
end
