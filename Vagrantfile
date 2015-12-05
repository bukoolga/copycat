# -*- mode: ruby -*-
# vi: set ft=ruby :

host_path_dev = "../copycat/copycat"
ang_host_path_dev = "../copycat/catangular"

vm_path_dev = "/vagrant/copycat/copycat"
ang_vm_path_dev = "/vagrant/copycat/catangular"

Vagrant.configure(2) do |config|
  config.vm.box = "ubuntu/trusty64"

  config.vm.network "private_network", ip: "192.168.33.56"

  config.vm.host_name = "copycat.dev"

  config.vm.synced_folder ".", "/vagrant", disabled: true
  config.vm.synced_folder host_path_dev, vm_path_dev
  config.vm.synced_folder ang_host_path_dev, ang_vm_path_dev

end
