# sofware requirements

Debian GNU/Linux 9 (stretch) or Centos 7

ansible 2.2.1.0

Vagrant 1.9.1

# Content description

Create and start 4 Vagrant boxes

 - apache01
 - db02
 - eao03
 - jcr04

and install/configure with Ansible
  
 - Apache HTTP server in apache01
 - MySql server in db02
 - WildFly 10.0.0-Final  in eap03
 - Jackrabbit  in jcr04

# Notes

To connect with the Vagrant boxex you have to create your SSH private and public key
and the change the path at those 2 lines
server01.ssh.private_key_path = ["/home/luca/.ssh/id_rsa", "~/.vagrant.d/insecure_private_key"]
server01.vm.provision "file", source: "/home/luca/.ssh/id_rsa.pub", destination: "~/.ssh/authorized_keys"



