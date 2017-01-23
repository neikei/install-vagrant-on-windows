# install-vagrant-on-windows
This manual enables you to use Vagrant on your Windows machine.

## Install VirtualBox
1. Download VirtualBox: https://www.virtualbox.org/wiki/Downloads
2. Install VirtualBox

## Install Git
The Windows Commandline doesn't know Linux commands, but you need them to access your VM with the vagrant ssh commands.

1. Download Git here: https://git-scm.com/download/win 
2. Install Git

## Install Vagrant
1. Download Vagrant here: https://releases.hashicorp.com/vagrant/1.8.7/vagrant_1.8.7.msi
2. Install Vagrant

## Test your new environment
1. Open your Git Bash
2. git clone https://github.com/neikei/vagrant-centos7-ansible-lemp.git
3. cd vagrant-centos7-ansible-lemp
4. vagrant up
5. ... wait ...
6. Check the webserver: http://192.168.56.123/
7. Access the box: vagrant ssh

## Have fun! :)
