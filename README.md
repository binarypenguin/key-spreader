# Key Spreader
A simple ansible playbook the distributes your ssh keys to a list of hosts. This is intended to be ran by the end user and is not for bulk user key deployment.

# Dependencies
* Ansible Core 2.17.4

# Getting Started
* Clone this repo
* ```cd key-spreader```
* ```python3 -m virtualenv .venv```
* ```source .venv/bin/activate```
* ```pip install -r requirements.txt```
* Copy ```hosts.example``` to ```hosts```
* Update ```hosts``` with machines you would like to provision. (See [Ansible Inventory](http://docs.ansible.com/ansible/intro_inventory.html))
  * Setting ```ansible_user``` will define which user to use.
* Copy your public keys (id_rsa.pub and id_ed25519.pub for example) to the keys folder.
* Run ```./distribute.sh``` to distribute your keys :)
