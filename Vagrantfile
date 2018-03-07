# -*- mode: ruby -*-
 
# vi: set ft=ruby :
 
hosts = {
 
  "word" => "192.168.88.10" 
}
 
Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/xenial64"

 hosts.each do |name, ip|
 
    config.vm.define name do |machine|
 
      machine.vm.network "private_network", ip: ip
 
      machine.vm.provider "virtualbox" do |v|
 
        v.name = name
 
      end
 
    end
 
  end
 
end
