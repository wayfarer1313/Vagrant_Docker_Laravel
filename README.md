# A LAMP Stack with Laravel Support using Vagrant and Docker

<br>
## Pre-Requisites
- Have [Virtual Box](https://www.virtualbox.org) installed
- Have [Vagrant](https://www.vagrantup.com) installed

<br>
## Setup
1. Run ````git clone https://github.com/MetalCowRobotics/Vagrant_Docker-LAMP.git```` in the Directory you want to Create your Project Directory in
2. Change the name of the ````Vagrant_Docker-LAMP```` Directory to ````Your Project Name````
3. Enter the Directory
4. Run ````vagrant up````
5. Wait for the VM to Start Up ....
6. Happy Coding + Testing

<br>
## General How to Use
Follow the Setup Above. Then change whatever you would like in the ````src```` directory. It is currently a Laravel Project. Then in your browser open  [localhost:8080](http://localhost:8080) or [127.0.0.1:8080](http://127.0.0.1:8080) to see the live web pages.

<br>
## Files

### Config Files
- ````Vagrantfile````

This is the config file for the Vagrant VM. It is where all the ports, vm setup, shared directories, and etc are setup.
- ````docker-compose.yml````

This is the config file for the Docker Containers. It is where all the containers are defined in a similar manner to vagrant. With configuration of port mapping, shared directories, and etc.

### Directories
- ````data```` Directory

This is where the MySQL Database is stored
- ````src```` Directory

This is where all the Laravel Project files are stored. You want to modify things in this directory. All modifications are automatically synced with the VM. 

### Scripts
- ````docker_start.sh````

This is the start script for the docker containers. It runs when the VM is provisioned / first started.

<br>
## Other Useful Notes
### Commands

- ````vagrant up````

This command starts up the VM

- ````vagrant halt````

This command will shutdown the VM and preserve the last state

- ````vagrant destroy````

This command will destroy all traces of the VM ( generally not be run )

- ````vagrant ssh````

This command allows the user to SSH into the VM
