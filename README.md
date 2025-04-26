# Ansible Playbooks

This repository contains Ansible playbooks, roles, and inventory files to automate server configurations and deployments.

## Structure
- `inventories/` : Hosts grouped into dev, prod environments.
- `playbooks/` : Main playbooks to install and configure services.
- `roles/` : Reusable Ansible roles for modular design.
- `group_vars/` and `host_vars/` : Variables specific to groups or hosts.
- `ansible.cfg` : Ansible configuration file.

## Requirements
- Ansible 2.9+ installed
- SSH access to target servers

## Basic Usage
Run a playbook:
```bash
ansible-playbook -i inventories/dev/hosts playbooks/site.yml
