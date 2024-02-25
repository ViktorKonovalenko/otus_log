# -*- mode: ruby -*- 
# vi: set ft=ruby : vsa
Vagrant.configure(2) do |config| 
  config.vm.box = "centos/7" 
# config.vm.box_version = "2004.01" 
  config.vm.provider "virtualbox" do |v| 
  v.memory = 512 
  v.cpus = 1 
  end 
  config.vm.define "web" do |web| 
   web.vm.network "private_network", ip: "192.168.56.10",  virtualbox__intnet: "net1" 
   web.vm.hostname = "web" 
   web.vm.network "forwarded_port", guest: 80, host: 8080
  end
  config.vm.define "log" do |log|
   log.vm.network "private_network", ip: "192.168.56.11",  virtualbox__intnet: "net1"
   log.vm.hostname = "log"
  end
   config.vm.provision "ansible" do |ansible|
   ansible.playbook = "web.yml"
   ansible.become = "true"
   end
end
