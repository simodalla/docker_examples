# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/bionic64"

  # config.vm.box_check_update = false
  # config.vm.network "forwarded_port", guest: 80, host: 8080

  # Create a private network, which allows host-only access to the machine
  # using a specific IP.
  # config.vm.network "private_network", ip: "192.168.33.10"

  config.vm.synced_folder ".", "/project", SharedFoldersEnableSymlinksCreate: false

  # config.vm.provider "virtualbox" do |vb|
  #   vb.memory = "1024"
  # end
end
