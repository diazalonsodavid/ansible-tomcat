Role Tomcat
============

This role installs and configure Tomcat Server.


Use
---

Role install Tomcat in /opt via tar.gz package 


Port variables are in default/main.yml

Users will be defined in default/main.yml
```yml
tomcat_users:
  - name: 
    password: 
    roles: 
```




Example Playbook
----------------
```yaml
---
    - hosts: servers
      roles:
         - { role: tomcat, become: yes }
```        

```console
ansible-playbook playbook.yml -i inventory
```