# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|
  config.vm.box = "bento/centos-7.1"

  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "ansible/playbook.yml"
  end

  config.vm.provider :virtualbox do |vb|
    vb.name = "docker-demo"
  end

  config.vm.network "private_network", type: "dhcp"
end
