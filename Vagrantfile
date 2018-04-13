# -*- mode: ruby -*-
# vi: set ft=ruby :

# All Vagrant configuration is done below. The "2" in Vagrant.configure
# configures the configuration version (we support older styles for
# backwards compatibility). Please don't change it unless you know what
# you're doing.
Vagrant.configure("2") do |config|

  config.vm.box       = "ubuntu/xenial64"
  config.vm.hostname  = "rails"
  config.vm.provision :shell, path: 'bootstrap.sh', keep_color: true, privileged: false
  config.vm.network :forwarded_port, guest: 3001, host: 3001,auto_correct: true

  config.vm.provider 'virtualbox' do |v|
    v.memory = 2048
    v.cpus = 2
  end
end
