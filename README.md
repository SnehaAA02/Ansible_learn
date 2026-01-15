# Ansible_learn
Learning ansible by doing hands-on


## Ad-hoc Commands 
ansible -i inventory webservers -m "shell" -a "df"   
ansible all -i inventory -b -m apt -a "name=nginx state=present"


## Run Playbooks
ansible-playbook -i inventory playbook.yml

## Use Tags
ansible-playbook playbook.yml --tags nginx    
ansible-playbook playbook.yml --skip-tags docker
