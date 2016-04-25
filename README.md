# Key Spreader
A simple ansible playbook the distributes your ssh keys to a list of hosts.

#Dependencies
* Ansible 2.0

#Getting Started
* Clone this repo
* Copy ```hosts.example``` to ```hosts```
* Update ```hosts``` with machines you would like to provision. (See [Ansible Inventory](http://docs.ansible.com/ansible/intro_inventory.html))
* Copy your public keys (id_rsa.pub for example) to the keys folder.
* Run ```./distribute.sh``` to distribute your keys :)
