Vagrant.configure("2") do |config|
  config.vm.box = "cisco/asa-lab"

  # Dont try to change the insecure public key 
  config.ssh.insert_key = false

  # Disable default host to guest synced folder
  config.vm.synced_folder ".", "/vagrant", disabled: true

  # Give the VM time to boot as Vagrant cannot tell when it is booted
  config.vm.boot_timeout = 120

  # Additional interfaces 
  config.vm.network "private_network", ip: "169.254.1.11", auto_config: false 
  config.vm.network "private_network", ip: "169.254.1.12", auto_config: false 
  config.vm.network "private_network", ip: "169.254.1.13", auto_config: false 
  config.vm.network "private_network", ip: "169.254.1.14", auto_config: false 

end
            
