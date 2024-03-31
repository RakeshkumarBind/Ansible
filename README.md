# Ansible
Ansible is used to configure multiple server or system , deploy software , orchestrate(plan or project) , do sysytem updates.

Advantages : Agentless : If you have hundreds of servers or system ypu dont need to configure all by installing ansible you just neeed one ansible server and you can manage them all.

# ACCESSING REMOTE SERVER FROM MAIN SERVER WITHOUT PASSWORD:

   MAIN SERVER :sudo dnf install epel-release
                sudo dnf install ansible
                ansible --version (to check whether it is installed)
                ansible localhost -m ping (This is a adhoc process to check whether ansible is working or not by using ping module to ping liocalhost)

                Make sure that your remote server has ssh enabled
                

                ssh-keygen
                ssh-copy-id remote server ip
                password 

                now you have suuccessfully configured your main server to remote server
# Some configuration files :
                              /etc/ansible/ansible.cfg
                              /etc/ansible/playbook ------------->main configuration file for doing tasks
                              /etc/ansible/hosts   --------------> inventory files having ip address of the server you can also add groups of ip adrress with [group 1]
                              /etc/ansible/roles

# Modules : small progran to do a task 
                              ping
                              file
                              service : state ---> present , absent
                              copy --------->src , dest
                              yum ----------->
                              shell
                              cron
                              user
                              firewalld
                              get_url
                              
                              
  
