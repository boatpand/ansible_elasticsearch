step
 define host in /etc/hosts on controller machine
 verify python is installed -> python --version
 generate ssh keygen "ssh-keygen -t rsa" at controller machine (root user)
 copy ssh key from root user to all nodes -> ssh-copy-id node01

 install ansible -> yum install ansible
 adjust config -> vi /etc/ansible/ansible.cfg -> callback_whitelist = profile_tasks (for show timestamp on each task)
 create inventory -> touch inventory.ini
 create playbook -> playbook.yaml

 run playbook -> ansible-playbook playbook.yaml -i inventory.ini
