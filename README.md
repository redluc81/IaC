# sofware requirements in the Control machine

tested with Debian GNU/Linux 9 (stretch) but should work also with Centos 7  

ansible 2.2.1.0

Vagrant 1.9.1

# command to run

cd fsp-install/vagrant/centos

vagrant up

cd fsp-install/ansible

ansible-playbook apache.yml

ansible-playbook mysql.yml


# TEST: go inside a vagrant box (for example the server where has been installed MySql)
# and run mysql -u root -p 
# the password is admin1234

ssh vagrant@192.168.33.24 


