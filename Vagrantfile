# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "debian/jessie64"
  config.vm.box_check_update = false

  config.vm.provider "virtualbox" do |vb|
     vb.memory = "1024"
  end
  config.vm.provision "shell", inline: <<-SHELL
      apt-get update
      apt-get install -y debhelper dh-autoreconf devscripts git
  SHELL
end
