# sofware requirements in the Control machine

Debian GNU/Linux 9 (stretch) or Centos 7

ansible 2.2.1.0

Vagrant 1.9.1

# command to run

cd IaC/vagrant/centos

vagrant up

cd IaC/ansible

ansible-playbook apache.yml

ansible-playbook mysql.yml

# to test go inside a vagrant box (for example the server where has been installed MySql)
ssh vagrant@192.168.33.24 
# and run 
mysql -u root -p
# the password is admin1234


