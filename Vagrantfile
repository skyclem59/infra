Vagrant.configure("2") do |config|
  
  config.vm.provision "shell", inline: "echo Hello"
  config.vm.network "private_network", type: "dhcp"
  config.vm.hostname = "m2i"

  config.vm.provider "virtualbox" do |v|
    v.memory = 4096
    v.cpus = 2
  end
  config.vm.define "outils" do |outils|
    outils.vm.box = "ubuntu/bionic64" 
  end
  config.vm.define "gestion" do |gestion|
    gestion.vm.box = "ubuntu/bionic64"
  end
  config.vm.define "prod" do |prod|
    prod.vm.box = "ubuntu/bionic64"
  end
end