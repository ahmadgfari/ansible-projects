# Ansible with Molecule Stack Roles
Roles is folder which contains the specific job or multiple jobs

Maintainer @ahmadgfari
## Getting Started
Install ansible
Install molecule

### Create playbook.yml
For Example we want to run job inject pubkey:
```
---
- hosts: all
  roles:
    - role: injectKey  # this stack of folder
```
### Run Command
```ansible-playbook playbook.yml --extra-vars "new_user=otten" --private-key```
