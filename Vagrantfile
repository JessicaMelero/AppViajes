# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|  
	config.vm.provider "virtualbox" do |v|
		v.name="Viajes_Apache_Mysql"
	end
	config.vm.box="ubuntu/xenial64"
	config.vm.provision "shell", path:"script.sh"
	config.vm.network :forwarded_port, guest: 3306, host: 3306
	config.vm.network :forwarded_port, guest: 80, host: 8080
end
