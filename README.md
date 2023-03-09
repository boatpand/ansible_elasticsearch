step 
<br />
 define host in /etc/hosts on controller machine
 <br />
 verify python is installed -> python --version
 <br />
 generate ssh keygen "ssh-keygen -t rsa" at controller machine (root user)
 <br />
 copy ssh key from root user to all nodes -> ssh-copy-id node01
<br />
 install ansible -> yum install ansible
 <br />
 adjust config -> vi /etc/ansible/ansible.cfg -> callback_whitelist = profile_tasks (for show timestamp on each task)
 <br />
 create inventory -> touch inventory.ini
 <br />
 create playbook -> playbook.yaml
<br />
 run playbook -> ansible-playbook playbook.yaml -i inventory.ini
