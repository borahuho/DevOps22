# DevOps22

This vagrant will install 4 Linux Ubuntu machines in a test cluster on Vagrant, 1 manager Docker node and 2 worker Docker nodes. 1 server will be a HAproxy server. This DevOps is to practice Docker swarm networking and high availability.
It will add some default users, groups and directory's. It will install Docker-ce by default with Ansible and the user vagrant is in the Docker group.
This Vagrant is to practice Docker swarm, commands on Docker swarm and deploy application over the Docker cluster.
This repository is intended for educational purpose only.


## Prerequisites

Works on Windows 10 and tested on macOS (macOS needs the Virtualbox extension pack).

Software needed:
* Virtualbox 5.0 or higher
* Git bash for Windows
* Vagrant 2.2.6 or higher
* DevNet account at Cisco 


## Demo installation && use Vagrant

Youtube: https://youtu.be/KABnIuaA8SM


## Demo Docker Swarm networking and high availability

Youtube: 


## Installation

* Install Virtualbox: https://www.virtualbox.org/wiki/Downloads
* Install Git bash for Windows: https://gitforwindows.org/
* Install Vagrant for Windows: https://www.vagrantup.com/downloads.html
* Create an free account at DevNet: https://developer.cisco.com/

## Run this Vagrant VM
Open **Git Bash** in Windows
```
cd Documents
mkdir vagrant && cd vagrant
git clone https://github.com/borahuho/DevOps22
cd DevOps22
vagrant up
vagrant ssh manager
```
## Mission

Read your mission in the directory "Opdracht"

## Network
Vagrant VM will be set up with 2 network adapters
```
Nat : DHCP
Localhost (manager): 192.168.10.200

Nat : DHCP
Localhost (worker1): 192.168.10.201

Nat : DHCP
Localhost (worker2): 192.168.10.202

Nat : DHCP
Localhost (HAproxy): 192.168.10.205
```
## Vagrant commands
Start VM's with Vagrant
```
vagrant up
```
Pause a VM
```
vagrant suspend
```
Restart a paused VM
```
vagrant resume
```
Stop and shutdown a VM
```
vagrant halt
```
Remove a VM
```
vagrant destroy
```
ssh in to the VM
```
vagrant ssh manager
vagrant ssh worker1
vagrant ssh worker2
vagrant ssh HAproxy
```

