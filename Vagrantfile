# -*- mode: ruby -*-
# vi: set ft=ruby :
Vagrant.configure(2) do |config|
  config.vm.provider 'virtualbox' do |vb|
    vb.cpus = 1
    vb.memory = 1024
  end

  config.vm.define "db1" do |db1|
    db1.vm.box = 'nodejs-box'
    db1.vm.network 'private_network', ip: '192.168.33.100'
    db1.vm.box_url = 'https://s3-ap-northeast-1.amazonaws.com/doridoridoriand/nodejs-vm.box'
  end

  config.vm.define "db2" do |db2|
    db2.vm.box = 'nodejs-box'
    db2.vm.network 'private_network', ip: '192.168.33.110'
    db2.vm.box_url = 'https://s3-ap-northeast-1.amazonaws.com/doridoridoriand/nodejs-vm.box'
  end
end
