# Ansible_learn
Learning ansible by doing hands-on


## Ad-hoc Commands 
ansible all -i inventory -m ping   \
ansible -i inventory webservers -m "shell" -a "df"   
ansible all -i inventory -b -m apt -a "name=nginx state=present"


## Run Playbooks
ansible-playbook -i inventory playbook.yml

## Use Tags
ansible-playbook playbook.yml --tags nginx    
ansible-playbook playbook.yml --skip-tags docker

<img width="600" height="700" alt="Screenshot (7)" src="https://github.com/user-attachments/assets/49b11590-0a1e-4d83-be7a-35f165d7661d" />
