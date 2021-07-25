Vagrant.configure("2") do |config|
    # configure the box: ubuntu 20.04 libvirt
    config.vm.box = "generic/ubuntu2004"

    # libvirt config
    config.vm.provider :libvirt do |libvirt|
        libvirt.cpus = 1
        libvirt.memory = 1024
    end

    # set hostname
    config.vm.hostname = "dev.mcgraw.test"

    # forward port 80
    config.vm.network "forwarded_port", guest: 80, host: 8080
end