# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|

  config.vm.box = "janihur/ubuntu-1404-desktop"

  config.vm.provider "virtualbox"

  #config.vm.network "public_network", bridge: 'en1: Wi-Fi (AirPort)'

  #config.vm.hostname = "aspnet-env.local"

  config.vm.provider :virtualbox do |vb|
    vb.gui = true
    vb.name = "aspnet-env"
    vb.customize ["modifyvm", :id, "--memory", 2048]
    vb.customize ["modifyvm", :id, "--vram", 64]
    vb.customize ["modifyvm", :id, "--accelerate3d", "on"]
    vb.customize ["modifyvm", :id, "--natdnshostresolver1", "on"]
  end

  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "playbook.yml"
  end

end
