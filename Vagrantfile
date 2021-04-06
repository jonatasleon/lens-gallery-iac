# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/focal64"
  config.vm.provider "virtualbox" do |vb|
    vb.cpus = 1
    vb.memory = 1024
  end

  config.vm.define "webapp" do |m|
    m.vm.network "private_network", ip: "172.17.177.40"
  end

  config.vm.define "database" do |m|
    m.vm.network "private_network", ip: "172.17.177.42"
  end

end
