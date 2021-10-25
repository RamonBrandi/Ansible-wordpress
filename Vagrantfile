Vagrant.configure("2") do |config|

  config.vm.box = "ubuntu/trusty64"

  config.vm.provider "virtualbox" do |vb|
    vb.memory = 1024
  end

  config.vm.define "wordpress" do |wp|
    wp.vm.network "private_network", ip: "172.17.177.40"
  end

  config.vm.define "database" do |db|
    db.vm.network "private_network", ip: "172.17.177.42"
  end

end