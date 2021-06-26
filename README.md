Ansible Docker install role
=========

Simple role to install docker and docker-compose following official guide.

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
    - role: jindrichskupa.ansible_docker
      vars:
        docker_compose_version: 1.29.2
```

License
-------

MIT

Author Information
------------------

Jindrich Skupa
