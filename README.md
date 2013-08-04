# Ubuntu Auto-upgrades Ansible role

A very simple Ansible role that will enable Ubuntu automatic upgrades.

In the works, options to allow you to choose package upgrades etc rather than just security upgrades, and also the periods to check for these.

For now though, just security upgrades, checked daily.

## Usage

Clone the repo to your Ansible roles directory.

In your playbook, just add `ubuntu-upgrades` to your roles list. For example:

	- hosts: yourservers
	  sudo: yes
	  roles:
	  	- ubuntu-upgrades
	  	