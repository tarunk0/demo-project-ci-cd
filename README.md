# demo-project-ci-cd
A complete CI/CD pipeline using ansible git github jenkins ..

Events of actions:
1. The code is firstly pushed to the github. Github is inegrated with jenkins, as soon as the code is changed and pushed to the main branch, the job is triggered on jenkins.
2. The jenkin server sends the code to the ansible server. 
3. Then on ansible, a playbook-has been written that copies the related files on the web server. 
4. This is how the code is deployed on to the webserver. 
