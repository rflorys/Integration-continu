Vagrant.configure("2") do |config|
  config.vm.box = "debian/buster64"
	config.vm.provision "shell", inline: <<-SHELL
		apt-get update
		apt-get install -y git
	SHELL
end
