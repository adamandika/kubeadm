Vagrant.configure("2") do |config|


  config.vm.define "master" do |master|
      master.vm.box =  'ubuntu/xenial64'
      master.vm.network "private_network", ip: "192.168.100.5"
          master.vm.provider "virtualbox" do |v|
              v.memory = 4094
              v.cpus = 4
       end
    end

    config.vm.define "worker" do |worker|
      worker.vm.box = "ubuntu/xenial64"
      worker.vm.network "private_network", ip: "192.168.100.6"
          worker.vm.provider "virtualbox" do |v|
              v.memory = 2094
              v.cpus = 2
       end
    end

  end