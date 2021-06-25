Ansible Docker install role
=========

Simple role to install docker follwing official guide.

Requirements
------------

* debian based distribution

Example Playbook
----------------

```yaml
---
- name: Playbook for docker servers
  hosts: dockers
  remote_user: ansible
  become: true
  vars:
    ansible_python_interpreter: /usr/bin/python3
  roles:
    - role: docker
```

License
-------

MIT

Author Information
------------------

Jindrich Skupa
