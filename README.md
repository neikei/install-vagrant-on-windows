# install-vagrant-on-windows

This manual enables you to use Vagrant on your Windows machine.

<!-- TOC -->

- [install-vagrant-on-windows](#install-vagrant-on-windows)
    - [Manual installation](#manual-installation)
        - [Install VirtualBox](#install-virtualbox)
        - [Install Git](#install-git)
        - [Install Vagrant](#install-vagrant)
        - [Install Vagrant Plugins](#install-vagrant-plugins)
    - [Installation via Chocolatey](#installation-via-chocolatey)
    - [Test your new environment](#test-your-new-environment)
    - [Have fun! :)](#have-fun-)

<!-- /TOC -->

## Manual installation

### Install VirtualBox

1. Download VirtualBox and the corresponding Extension Pack: https://www.virtualbox.org/wiki/Downloads
2. Install VirtualBox with the default settings
3. Add the Extension Pack to VirtualBox (File -> Preferences -> Extensions)

### Install Git

1. Download Git: https://git-scm.com/download/win
2. Install Git with the default settings

### Install Vagrant

1. Download Vagrant: https://releases.hashicorp.com/vagrant/2.3.7/vagrant_2.3.6_windows_amd64.msi
2. Install Vagrant with the default settings
3. Reboot Windows

### Install Vagrant Plugins

1. Open your Git Bash or your Powershell, which should also work
2. vagrant plugin install vagrant-winnfsd # used for fast NFS shares
3. vagrant plugin install vagrant-vbguest # used for automatic VirtualBox guest addition updates

## Installation via Chocolatey

[Chocolatey](https://chocolatey.org/) is a package manager for Windows.

```powershell
# Start Powershell as administrator

# Install chocolatey if it isn't installed yet
Set-ExecutionPolicy Bypass -Scope Process -Force; iex ((New-Object System.Net.WebClient).DownloadString('https://chocolatey.org/install.ps1'))

# Install Git VirtualBox and Vagrant
choco install git virtualbox vagrant

# Refresh environment variables
refreshenv

# Install Vagrant Plugins
vagrant plugin install vagrant-winnfsd
vagrant plugin install vagrant-vbguest

# Reboot Windows
```

## Test your new environment

1. Open your Git Bash or your Powershell, which should also work
2. git clone https://github.com/neikei/install-vagrant-on-windows.git
3. cd install-vagrant-on-windows
4. vagrant up
5. ... wait ...
6. vagrant ssh

## Have fun! :)
