Vagrant + Puppet Development Setup for Askaway
==============================================

Requires vagrant and virtualbox

1. Change this line in the Vagrantfile to point to the askaway codebase
   `config.vm.synced_folder "../askaway", "/var/www", id: "askaway-root", :nfs => true`
2. Run `vagrant up`
3. Go to http://192.168.33.201

You may need to manually start `rails server`..

4. Run `vagrant ssh`
5. Run `cd /var/www/`
6. Run `bundle exec rails server -d`
7. Run `exit`

Hopefully this should work for many rails sites.