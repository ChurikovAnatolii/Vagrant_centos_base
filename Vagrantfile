# -*- mode: ruby -*-
# vi: set ft=ruby :

$script = <<-'SCRIPT'
yum install -y mc
uname -r
SCRIPT

Vagrant.configure("2") do |config|

  config.vm.box = "Kazay/centos-Kz"
  config.vm.box_check_update = false
  config.vm.network "public_network"
  config.vm.provision "shell", inline: $script
  config.vm.provider "virtualbox" do |vb|
    vb.gui = true
    vb.memory = "512"
  end
end
