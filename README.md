Vagrant.configure("2") do |config|
  config.vm.box = "debian/buster64"
	config.vm.provision "shell", inline: <<-SHELL
		apt-get update
		apt-get install -y git
	SHELL
end



| config.vm.box = "debian/buster64" | Permet de créer une vm debian/ Vas recuperer sur vagrant cloud la box debian (version : v10.20231211.1)


|	config.vm.provision "shell", inline: <<-SHELL
		apt-get update
		apt-get install -y git
	SHELL | Ouvre un terminal sur la vm et il vas exécuter les commandes  : 
	- apt-get update | Permet de mettre a jour tous les packets du système
	- apt-get install -y git | Install le packet git, -y permet d'accepter automatiquement des qu'un prompt vas s'afficher pendant l'exécution du ap-get install
