# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|
    config.vm.box = "bento/ubuntu-20.04"
    config.vm.box_check_update = false
    config.vm.hostname = "nginx.local.dev"

    config.vm.network :private_network, ip: "12.34.56.78"
    config.vm.network :forwarded_port, guest: 80, host: 8080

    config.vm.provider "virtualbox" do |vb|
        vb.name = "NgiServer"
        vb.memory = "4096"
        vb.cpus = "2"
    end
end
