# ansible-playbooks
This repo is created for storing playbooks !!

# Ansible commands for listing hosts
- ansible frontend -i inventory.ini --list-hosts
- ansible ungrouped -i inventory.ini --list-hosts

# Commands for running ansible-playbooks
- ansible-playbook -i <inventory.ini> <01-playbook.yaml> -e ansible_user=<user_name> -e  ansible_password=<Password> -b
# running in local machine
- ansible-playbook -i <inventory.ini> <01-playbook.yaml> 
