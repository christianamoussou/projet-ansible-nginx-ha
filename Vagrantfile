# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
# Configuration de la machine vm1
  config.vm.define "vm1" do |vm1_config|
    vm1_config.vm.box = "bento/ubuntu-22.04"
    vm1_config.vm.hostname = "vm1"

    vm1_config.vm.network "public_network", bridge: "Carte de bouclage Microsoft KM-TEST", ip: "192.168.30.11"
    vm1_config.vm.provider "virtualbox" do |vb|
      vb.memory = "1024"
      vb.cpus = "1"
    end
  end

  # Configuration de la machine vm2
  config.vm.define "vm2" do |vm2_config|
    vm2_config.vm.box = "bento/ubuntu-22.04"
    vm2_config.vm.hostname = "vm2"

    vm2_config.vm.network "public_network", bridge: "Carte de bouclage Microsoft KM-TEST", ip: "192.168.30.12"
    vm2_config.vm.provider "virtualbox" do |vb|
      vb.memory = "1024"
      vb.cpus = "1"
    end
  end
end