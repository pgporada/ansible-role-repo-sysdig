# Ansible Role: Sysdig Repository
This role will install and configure the [Sysdig](https://github.com/draios) repository.

## Role Variables

## Example Playbook
```
---
- hosts: localhost
  connection: local
  become: true
  become_method: sudo
  roles:
    - ansible-role-repo-draios
```

### Usage
```
ansible-playbook -i localhost -c local example_playbook.yml
```
