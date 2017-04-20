# -*- mode: ruby -*-
# vi: set ft=ruby :

# All Vagrant configuration is done below. The "2" in Vagrant.configure
# configures the configuration version (we support older styles for
# backwards compatibility). Please don't change it unless you know what
# you're doing.
BOX_IMAGE = "bento/centos-7.2"
Vagrant.configure("2") do |config|

    # Multi-Machine config
    # Loadbalancer VM
    config.vm.define "lbcer", primary: true do |lbcer|
        lbcer.vm.box= BOX_IMAGE
        lbcer.vm.hostname = "lbcer."
        lbcer.vm.network "private_network", ip: "10.0.1.10"
        
    end
    
    # Dev01 VM
    config.vm.define "dev01" do |dev01|
        dev01.vm.box= BOX_IMAGE
        dev01.vm.hostname = "dev01"
        dev01.vm.network "private_network", ip: "10.0.1.11"
        
    end

    # Dev02 VM
    config.vm.define "dev02" do |dev02|
        dev02.vm.box= BOX_IMAGE
        dev02.vm.hostname = "dev02"
        dev02.vm.network "private_network", ip: "10.0.1.12"
        
    end

    # DB01 VM
    config.vm.define "db01" do |db01|
        db01.vm.box= BOX_IMAGE
        db01.vm.hostname = "db01"
        db01.vm.network "private_network", ip: "10.0.1.13"
        
    end

    # DB02 VM
    config.vm.define "db02" do |db02|
        db02.vm.box= BOX_IMAGE
        db02.vm.hostname = "db02"
        db02.vm.network "private_network", ip: "10.0.1.14"
        
    end

end
