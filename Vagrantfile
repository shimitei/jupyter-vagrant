Vagrant.configure("2") do |config|
  config.vm.box = "ubuntu/xenial64"
  config.vm.network :forwarded_port, host: 8888, guest: 8888
  config.vm.provider "virtualbox" do |v|
    v.customize ["modifyvm", :id, "--ostype", "Ubuntu_64", "--ioapic", "on"]
    v.cpus = 2
    v.memory = 512
  end
  config.vm.provision "docker"
  config.vm.provision :shell, path: "pull_image.sh"
  config.vm.provision :shell, path: "run.sh"
end
