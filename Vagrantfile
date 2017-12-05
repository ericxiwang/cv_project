Vagrant.configure("2") do |config|
  config.vm.define "jenkins" do |jenkins|
    jenkins.vm.box = "centos/7"
    jenkins.vm.network "public_network", ip: "192.168.0.160"
    
    jenkins.vm.provider "virtualbox" do |v|
       v.memory = 4096
       v.cpus = 2
    end
    #config.vm.provision "shell", path: "inst.sh"
  end

  config.vm.define "dev-server" do |dev-server|
    dev-server.vm.box = "centos/7"
    dev-server.vm.network "public_network", ip: "192.168.0.161"

    dev-server.vm.provider "virtualbox" do |v|
       v.memory = 8192
       v.cpus = 4
    end


  end
end