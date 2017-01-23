# install-vagrant-on-windows
This manual enables you to use Vagrant on your Windows machine.

## Install VirtualBox
1. Download VirtualBox: https://www.virtualbox.org/wiki/Downloads
2. Install VirtualBox

## Install Git
The Windows Commandline doesn't know Linux commands, but you need them to have a working Vagrant environment and Git will install a bundle of needed commands for you.

1. Download Git here: https://git-scm.com/download/win
2. Install Git

## Install Vagrant
1. Download Vagrant here: https://releases.hashicorp.com/vagrant/1.8.7/vagrant_1.8.7.msi
2. Install Vagrant
3. Reboot your Windows

## Install Vagrant Plugins
1. Open your Powershell
2. vagrant plugin install vagrant-winnfsd # used for fast NFS shares
3. vagrant plugin install vagrant-vbguest # used for automatic VirtualBox guest addition updates

## Test your new environment
1. Open your Powershell
2. mkdir test-vagrant
3. cd test-vagrant
4. wget https://github.com/neikei/install-vagrant-on-windows/blob/master/Vagrantfile
5. vagrant up
6. ... wait ...
7. vagrant ssh

## Have fun! :)
