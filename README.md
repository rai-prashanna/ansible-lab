# ansible-lab

#to run playbook in local instance 
   ansible-playbook playbook.yml --connection=local

#or you can edit your inventory file as follows
  [local]                                    |             [local]
   127.0.0.1                                 |             127.0.0.1   ansible_connection=local
                                             |
  [local:vars]                               |
  ansible_connection=local                   |
  
#or you can edit your playbook as follows
   - hosts: local
     connection: local
  
