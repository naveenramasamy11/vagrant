Vagrant.configure("2") do |config|
  config.vm.define "kube-master" do |vm1|
    vm1.vm.box = "centos/7"
    vm1.vm.hostname = "kube-master"
  
     vm1.vm.network "private_network", ip: "192.168.50.4"
  
     vm1.vm.provider "virtualbox" do |vb|
       vb.gui = false
       vb.memory = "512"
     end
  end
  
  config.vm.define "kube-worker-1" do |vm2|
    vm2.vm.box = "centos/7"
    vm2.vm.hostname = "kube-worker-1"
  
     vm2.vm.network "private_network", ip: "192.168.50.5"
  
     vm2.vm.provider "virtualbox" do |vb|
       vb.gui = false
       vb.memory = "512"
     end
  end

  config.vm.define "kube-worker-2" do |vm3|
    vm3.vm.box = "centos/7"
    vm3.vm.hostname = "kube-worker-2"

     vm3.vm.network "private_network", ip: "192.168.50.6"

     vm3.vm.provider "virtualbox" do |vb|
       vb.gui = false
       vb.memory = "512"
     end
  end
end
