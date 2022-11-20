## ANSIBLE REFACTORING AND STATIC ASSIGNMENTS (IMPORTS AND ROLES)

### INRODUCTION

Refactoring is a general term used in computer programming which means changes to source code without changing the expected behaviour of the software. Refactoring enhances code readability, increases maintainability and extensibility, reduce complexity and allows for the addition of proper comments without affecting the logic.

This project is a continuum of the *ansible-config-mgt* repository implemented in project 11. Here, I made some improvement on my code by refactoring my Ansible code, create new assignments and used the imports functionality; allowing the usage of previously created playbooks in a new playbook.

### JENKINS JOB ENHANCEMENT
The current jenkins job configuration is such that every change in code creates a separate directory. This would be inconvenient when running commands from one place and also consumes space on Jenkins servers with each subsequent change.

I created a new directory named ansible-config-artifact and changed the permission of folder to allow Jenkins save files in the directory. 

![image](images/img1.png)

I installed the *copy artifact* from the Jenkins Manage plugin page without restarting Jenkins.

![image](images/img2.png)




