
VAGRANTFILE_API_VERSION = "2"

Vagrant.configure(VAGRANTFILE_API_VERSION) do |config|
  config.vm.box = 'cdaf/CentOSLVM'
  config.vm.provider "virtualbox" do | p |
    p.customize ["modifyvm", :id, "--cpus", "2"]
    p.customize ["modifyvm", :id, "--memory", "2000"]
    disk = 'extra_disk.vdi'
    unless File.exist?(disk)
      p.customize ['createhd', '--filename', disk, '--size', 5 * 1024]
    end
    p.customize ['storageattach', :id, '--storagectl', 'SATA', '--port', 1, '--device', 0, '--type', 'hdd', '--medium', disk]
   
    disk = 'extra_disk2.vdi'
    unless File.exist?(disk)
      p.customize ['createhd', '--filename', disk, '--size', 5 * 1024]
    end
    p.customize ['storageattach', :id, '--storagectl', 'SATA', '--port', 2, '--device', 0, '--type', 'hdd', '--medium', disk]

  end
end
