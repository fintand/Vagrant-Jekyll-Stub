# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure("2") do |config|

    config.vm.box = "scotch/box"
    config.vm.network "private_network", ip: "192.168.33.10"
    config.vm.network "forwarded_port", guest: 8000, host: 8000, auto_correct: true
    config.vm.network "forwarded_port", guest: 8080, host: 8080, auto_correct: true
    config.vm.hostname = "scotchbox"
    config.vm.provision "shell", privileged: false, path: "bootstrap.sh"

    # Optional NFS. Make sure to remove other synced_folder line too
    config.vm.synced_folder "./jekyll", "/home/vagrant/jekyll", :nfs => { :mount_options => ["dmode=777","fmode=666"] }
    config.vm.provider "virtualbox" do |vb|
      vb.memory = "1024"
    end

end
