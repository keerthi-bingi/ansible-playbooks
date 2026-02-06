# ansible-playbooks
This repo is created for storing playbooks !!

# Ansible commands for listing hosts
- ansible all -i <IP>, -e ansible_user=ec2-user -e ansible_password=DevOps321 -m ping
- ansible all -i <IP>, -e ansible_user=ec2-user -e ansible_password=DevOps321 -b -m dnf -a "name=nginx state=installed"
- ansible frontend -i inventory.ini --list-hosts
- ansible ungrouped -i inventory.ini --list-hosts

# Commands for running ansible-playbooks
- ansible-playbook -i <inventory.ini> <01-playbook.yaml> -e ansible_user=<user_name> -e  ansible_password=<Password> -b
# running in local machine
- ansible-playbook -i <inventory.ini> <01-playbook.yaml> 
