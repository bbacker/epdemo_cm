# _*_ mode: ruby _*_

VAGRANT_API_VERSION = "2"

Vagrant.configure(VAGRANT_API_VERSION) do |config|
  config.vm.box = "bento/centos-6.7"

  config.vm.hostname = "egdemo"
  config.vm.define "egdemo"

  # 8080 so we can see nginx on vagrant vm from vagrant host
  config.vm.network "forwarded_port", guest: 80, host: 8080

  config.vm.provision "ansible" do |ansible|
    ansible.playbook = "ansible/playbook.yml"
  end

end
