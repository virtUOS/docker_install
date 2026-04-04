Ansible: Install Docker Role
============================

This Ansible role installs the Docker CE repository and Docker itself on EL8/9/10.
It will start and enable the service so that the host is ready to run containers.

Supported Linux Distributions
-----------------------------use

This role supports:

- RHEL
- CentOS Stream
- Rocky Linux
- AlmaLinux OS

Version support:

- 10 (experimental)
- 9
- 8 (deprecated)

Example Playbook
----------------

Example of how to use the role:

```yaml
- hosts: all
  become: true
  roles:
    - role: docker_install
```

Example `requirements.yml`:
```yaml
---
roles:
  - src: https://github.com/virtUOS/docker_install.git
    scm: git
    version: 0.1.0
```
