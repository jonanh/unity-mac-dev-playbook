Vagrant.configure("2") do |config|
  
  config.vm.box = "jonan/macOS_10.13"
  
  config.vm.provider "virtualbox" do |v|
    v.gui = true
    v.linked_clone = true
  end

  config.vm.synced_folder ".", "/vagrant", disabled: true
  
  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "main.yml"
  end

end

