# install-vagrant-on-windows
This manual enables you to use Vagrant on your Windows machine.

## Install VirtualBox
1. Download VirtualBox: https://www.virtualbox.org/wiki/Downloads
2. Install VirtualBox with the default settings

## Install Git
The Windows Commandline doesn't know Linux commands, but you need them to have a working Vagrant environment and Git will install a bundle of needed commands for you.

1. Download Git: https://git-scm.com/download/win
2. Install Git
 - Select "Use Git and optional Unix tools from the Windows Command Promt" in the section for the adjustment of your PATH environment

## Install Vagrant
1. Download Vagrant: https://releases.hashicorp.com/vagrant/1.8.7/vagrant_1.8.7.msi
2. Install Vagrant with the default settings
3. Reboot your Windows

## Install Vagrant Plugins
1. Open your Powershell
2. vagrant plugin install vagrant-winnfsd # used for fast NFS shares
3. vagrant plugin install vagrant-vbguest # used for automatic VirtualBox guest addition updates

## Test your new environment
1. Open your Powershell
2. git clone https://github.com/neikei/install-vagrant-on-windows.git
3. cd install-vagrant-on-windows
4. vagrant up
5. ... wait ...
6. vagrant ssh

## Have fun! :)
