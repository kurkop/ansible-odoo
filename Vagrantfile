# -*- mode: ruby -*-
# vi: set ft=ruby :

# Vagrantfile API/syntax version. Don't touch unless you know what you're doing!
VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  NAME = "odoo"
  config.vm.define "odoo" do |odoo|
      odoo.vm.box = "precise32"
      odoo.vm.host_name = NAME

      odoo.vm.network :private_network, ip: "192.168.33.2"
      odoo.vm.provider "virtualbox" do |vb|
        vb.customize ["modifyvm", :id, "--memory", "2048"]
        vb.customize ["modifyvm", :id, "--name", NAME ]
      end
  end
end
