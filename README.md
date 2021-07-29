Mythic
=========

Install Mythic

Role Variables
--------------

A list of all the variables can be found in ./defaults/main.yml.

## Base Configs
`mythic_repo` - Path to the repo you'd like to install. Useful if using a fork of Mythic

`mythic_version` - Branch to pull from repo

`installation_path` - Path to install Mythic

## Service Configs
`server_header` - Mythic HTTP server header

`admin_username` - Admin username for Mythic

`default_password` - Admin password for Mythic

`operation_name` - Default operation name

## Agents
`agents[].repo` - Git repository to pull agent

`agents[].branch` - Branch to pull from repository

Dependencies
------------

ansible-galaxy install geerlingguy.docker
ansible-galaxy install geerlingguy.pip

Example Playbook
----------------

```yaml
- hosts: servers
  roles:
      - { role: t94j0.mythic }
```

License
-------

BSD

Author Information
------------------

Max Harley <mharley@specterops.io>