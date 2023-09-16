Vagrant.configure("2") do |config|
  # Configuration de la machine virtuelle serveur DNS
  config.vm.define "serveur" do |serveur|
    serveur.vm.box = "ubuntu/bionic64"
    serveur.vm.network "private_network", type: "static", ip: "10.0.0.126"
    serveur.vm.hostname = "serveurdns"
  end

  # Configuration de la machine virtuelle de test
  config.vm.define "testclient" do |testclient|
    testclient.vm.box = "ubuntu/bionic64"
    testclient.vm.network "private_network", type: "static", ip: "10.0.0.127"
    testclient.vm.hostname = "machinetest"
  end
end
