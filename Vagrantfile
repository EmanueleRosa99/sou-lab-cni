Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/focal64"
  
  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "playbook.yaml"
  end

  config.vm.define "soufe1" do |soufe1|
    soufe1.vm.hostname = "soufe1"
    soufe1.vm.network "private_network", ip: "192.168.50.11"
    soufe1.vm.provider "virtualbox" do |vb|
      vb.memory = "1024"
      vb.cpus = 1
    end
  end

  config.vm.define "soube2" do |soube2|
    soube2.vm.hostname = "soube2"
    soube2.vm.network "private_network", ip: "192.168.50.12"
    soube2.vm.provider "virtualbox" do |vb|
      vb.memory = "1024"
      vb.cpus = 1
    end
  end
end
