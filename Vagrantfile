# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure(2) do |config|

  config.vm.box = "ubuntu/trusty64"

  config.vm.network "forwarded_port", guest: 8000, host: 8000

  config.vm.synced_folder ".", "/vagrant", type: "virtualbox"
  config.vm.synced_folder "./projects", "/projects", type: "virtualbox"

  config.vm.provider "virtualbox" do |vb|
    # Display the VirtualBox GUI when booting the machine
    vb.gui = false
    vb.memory = "1024"
  end

  config.vm.provision "shell", inline: <<-SHELL
    sudo apt-get update
    sudo apt-get install python-pip -y
    sudo pip install cactus
    sudo apt-get install yui-compressor -y
    sudo ln -s /usr/bin/yui-compressor /usr/bin/yuicompressor
    sudo apt-get install closure-compiler -y
    sudo pip install awscli
  SHELL

end