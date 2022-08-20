# demo-project-ci-cd
A complete CI/CD pipeline using ansible git github jenkins .....

Events of actions:
1. The code is firstly pushed to the github. Github is inegrated with jenkins, as soon as the code is changed and pushed to the main branch, the job is triggered on jenkins.
2. The jenkin server sends the code to the ansible server. 
3. Then on ansible, a playbook-has been written that copies the related files on the web server. 
4. This is how the code is deployed on to the webserver. 



After installing ansible using yum or apt..
Do the following:
1. add the group and ips into hosts .. vim /etc/ansible/hosts
2. make the connection between client and server password less between ansible and nodes. using ssh-keygen and then copying ssh key to hosts. Allow root login in nodes by going inside vim /etc./ssh/sshd_onfig set password of root using --- passwd root
4. key generate -- ssh-keygen
5. ssh-copy-id -i root@pvt_ip
6. Make the similar connection between jenkins and ansible
