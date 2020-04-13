# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
  config.vm.box = "generic/debian10"
  # config.vm.synced_folder "/Users/stefanpapp/workspace", "/workspace"
  config.vm.hostname = "devserver" 
  config.vm.provider "parallels" do |v|
        v.memory = 4096
        v.cpus = 2
        v.name = "devserver"
  end

  config.vm.provision "shell", path: "./provision.sh"
end
