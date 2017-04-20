# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/xenial64"
  config.vm.box_check_update = false

  # copy current directory to vagrant machine
  config.vm.synced_folder ".", "/home/vagrant/irclogparser"

  # install IRCLogParser and its dependencies
  config.vm.provision :shell, privileged: true, path: "ext/vagrant.sh"


end
