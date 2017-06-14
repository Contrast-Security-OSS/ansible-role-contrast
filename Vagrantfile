# -*- mode: ruby -*-
# vi: set ft=ruby :

Vagrant.configure('2') do |config|
  config.vm.define 'ansible-role-contrast' do |c|
    c.vm.box = 'ubuntu/trusty64'
    c.vm.hostname = 'ansible-role-contrast'
    c.vm.provision 'ansible' do |ansible|
      ansible.playbook = 'test.yml'
      ansible.verbose = 'v'
      #ansible.extra_vars = 'test_vars.yml'
      #ansible.inventory_path = 'vagrant-inventory'
      ansible.host_key_checking = false
    end
  end
end
