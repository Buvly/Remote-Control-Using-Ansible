# Remote-Control-Using-Ansible
Ansible project

Steps:
1- create a keypair
2- create ubuntu ec2 instance
3- open inboud port 3000 for my ec2 instance
4- create inventory.txt file including the ec2 instance global ipv4
5- Create a new Playbook file named main-remote.yml
6- Create a simple web server file in NodeJS - `roles/setup/files/index.js
7- Add a new task file - roles/setup/tasks/main.yml
8-  run the Playbook using your inventory file and udacity.pem:
  ansible-playbook main-remote.yml -i inventory --private-key udacity.pem
9- delete the ec2 instance after finishing



Errors I faced:
1- forgot to change the mod for the .pem file to 400
2- typo in the taks main.yml file (apt --> changed to npm)
