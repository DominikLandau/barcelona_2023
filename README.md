# ansible_netapp_explore_2023

The code for the presentation at the VMware Explore for NetApp.

## Setup ansible
### Create virtual environment
python3 -m venv virt

### Activate virtual environment
. virt/bin/activate

### Install packages
pip install ansible-core

### Install ansible collections
#### VMware community collection
ansible-galaxy collection install community.vmware
#### Official NetApp collection
ansible-galaxy collection install netapp.ontap
#### Ansible collection for mounting NFS share
ansible-galaxy collection install ansible.posix

## Run the code
### Rename
<b>dynamic.vmware.yml.template</b> to <b>dynamic.vmware.yml</b>  
and  
<b>vars.yml.template</b> to <b>vars.yml</b>  

### Set variables
Populate the files with a <b>user</b> and a <b>password</b>  

### Execute
ansible-playbook main.yaml

<br>
Author: Dominik Landau