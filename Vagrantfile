```
Vagrant.configure("2") do |config|
  config.vm.define "kube-master-1" do |vm1|
    vm1.vm.box = "centos/7"
    vm1.vm.hostname = "kube-master-1"
    vm1.vm.network "public_network", bridge: 'en0: Wi-Fi (Wireless)', ip: "192.168.0.109"

    vm1.vm.provider "virtualbox" do |vb|
       vb.gui = false
       vb.memory = "2048"
       vb.customize ["modifyvm", :id, "--cpus", "2"]
    end
  end

  config.vm.define "kube-worker-1" do |vm2|
    vm2.vm.box = "centos/7"
    vm2.vm.hostname = "kube-worker-1"

    vm2.vm.network "public_network", bridge: 'en0: Wi-Fi (Wireless)', ip: "192.168.0.110"

    vm2.vm.provider "virtualbox" do |vb|
       vb.gui = false
       vb.memory = "2048"
       vb.customize ["modifyvm", :id, "--cpus", "2"]
    end
  end

  config.vm.define "kube-worker-2" do |vm3|
    vm3.vm.box = "centos/7"
    vm3.vm.hostname = "kube-worker-2"

    vm3.vm.network "public_network", bridge: 'en0: Wi-Fi (Wireless)', ip: "192.168.0.111"

    vm3.vm.provider "virtualbox" do |vb|
       vb.gui = false
       vb.memory = "2048"
       vb.customize ["modifyvm", :id, "--cpus", "2"]
    end
  end
end
```
