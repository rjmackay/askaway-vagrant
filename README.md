Vagrant + Puppet Development Setup for Askaway
==============================================

Requires vagrant and virtualbox

1. Change this line in the Vagrantfile to point to the askaway codebase
   `config.vm.synced_folder "../askaway", "/var/www", id: "askaway-root", :nfs => true`
2. Run `vagrant up`

Hopefully this should work for many rails sites.