Ansible Cobalt Strike (Docker)
=========

[![CI](https://github.com/warhorse/ansible-role-evilginx2-docker/workflows/CI/badge.svg?event=push)](https://github.com/warhorse/ansible-role-evilginx2-docker/actions?query=workflow%3ACI)
[![Release](https://github.com/warhorse/ansible-role-evilginx2-docker/actions/workflows/release.yml/badge.svg)](https://github.com/warhorse/ansible-role-evilginx2-docker/actions/workflows/release.yml)
[![warhorse.evilginx2_docker](https://img.shields.io/ansible/role/57563)](https://galaxy.ansible.com/warhorse/evilginx2_docker)
[![warhorse.cobaltstrike_docker](https://img.shields.io/ansible/quality/57563)](https://galaxy.ansible.com/warhorse/evilginx2_docker)
[![warhorse.cobaltstrike_docker](https://img.shields.io/ansible/role/d/57563)](https://galaxy.ansible.com/warhorse/evilginx2_docker)
![License](https://img.shields.io/github/license/warhorse/ansible-role-evilginx2-docker)
![Commit](https://img.shields.io/github/last-commit/warhorse/ansible-role-evilginx2-docker)

![Evilginx2 Logo](./images/evilginx2_logo.png "Evilginx2 Logo")

Install evilginx2 in (Docker)

This role is part of the Warhorse Automation Framework. This role can be used with Warhorse or as a standalone role.

Docker Image
-------------

[ghcr.io/stevesec/docker-evilginx2](https://github.com/stevesec/docker-evilginx2)

Role Variables
--------------

A list of all the variables can be found in ./defaults/main.yml.

`evilginx2_dir` - Cobalt Strike container directory 

`evilginx2_ports` - Cobalt Strike container ports

`evilginx2_hostname` - Cobalt Strike container hostname

`evilginx2_container_name` - Cobalt Strike container name 

`evilginx2_docker_network` Cobalt Strike container docker network


Dependencies
------------

```shell
ansible-galaxy install geerlingguy.docker geerlingguy.pip
```

Install
------------

```shell
ansible-galaxy install stevesec.evilginx2_docker
```

Example Playbook
----------------

```yaml
- hosts: servers
  roles:
      - { role: stevesec.evilginx2_docker }
```

License
-------

MIT/BSD

Author Information
------------------

Steve Nelson
