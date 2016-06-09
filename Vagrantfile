Vagrant.configure(2) do |config|
  config.vm.box = "ubuntu/trusty64"
  config.vm.synced_folder ".", "/home/vagrant/project"
  config.vm.network "private_network", ip: "192.168.10.10"

  config.vm.provider :virtualbox do |vb|
    vb.customize ["setextradata", :id, "VBoxInternal2/SharedFoldersEnableSymlinksCreate/.", "1"]
  end

  config.vm.provision "shell", inline: <<-SHELL
      # update APT repositories before installing anything else
      sudo apt-get update

      # install node.js the usual way (will also install npm this time)
      sudo apt-get install -y nodejs npm

      sudo rm /usr/bin/node
      sudo rm /usr/sbin/node
      sudo ln -s /usr/bin/nodejs /usr/bin/node

      # let's get "node_modules" out of the synced folder
      mkdir /home/vagrant/node_modules
      cd /home/vagrant/project/slides
      ln -s /home/vagrant/node_modules/ node_modules

      # grunt
      sudo npm install -g grunt-cli
    SHELL
end
