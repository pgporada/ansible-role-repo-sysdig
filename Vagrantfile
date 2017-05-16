# -*- mode: ruby -*-
# vi: set ft=ruby :

# All Vagrant configuration is done below. The "2" in Vagrant.configure
# configures the configuration version (we support older styles for
# backwards compatibility). Please don't change it unless you know what
# you're doing.
Vagrant.configure(2) do |config|
  config.vm.box = "geerlingguy/centos7"
  config.vm.synced_folder ".", "/vagrant"

  config.vm.provider "virtualbox" do |vb|
     vb.memory = "512"
  end

  config.vm.provision "shell", inline: <<-SHELL
    sudo yum install -y python-devel python-pip libffi libffi-devel openssl-devel gcc
    sudo pip install backports.ssl_match_hostname
    sudo pip install ansible
    sudo pip install --upgrade setuptools
    sudo ansible-playbook /vagrant/hacking.yml
    sudo yum install -y sysdig
  SHELL
end
