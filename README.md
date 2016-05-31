# Ansible Role - Teamspeak3 for Docker

[![Build Status](https://travis-ci.org/elnebuloso/ansible-role-docker-teamspeak3.svg?branch=master)](https://travis-ci.org/elnebuloso/ansible-role-docker-teamspeak3)

## Requirements

This role requires Ansible 2.0 or higher, and platform requirements are listed in the metadata file.

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

```
docker_teamspeak3_state: "started"
docker_teamspeak3_version: "latest"
docker_teamspeak3_container_name: "teamspeak3"
docker_teamspeak3_container_volume_base: "/opt/docker"
docker_teamspeak3_container_port_9987: "9987"
docker_teamspeak3_container_port_10011: "10011"
docker_teamspeak3_container_port_30033: "30033"
```

## Example Playbook

```
- hosts: localhost
  roles:
    - { role: elnebuloso.docker-teamspeak3 }
```

## Dependencies

- `docker` should be installed and working (you can use the `elnebuloso.docker` role to install).

##  License

MIT

##  Author Information

This role was created in 2016 by [elnebuloso](https://github.com/elnebuloso/)