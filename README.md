<!-- This was created with Claude Code -->

# Inventory Automation

[![Contribute](https://img.shields.io/badge/OpenShift-Dev%20Spaces-525C86?logo=redhatopenshift&labelColor=EE0000)](https://devspaces.apps.ocp.shadowman.dev/#https://github.com/shadowman-lab/Ansible-Inventory)


This directory contains Ansible automation for inventory management and operations.

## Overview

The Inventory automation provides playbooks and roles for managing and configuring
inventory infrastructure and services.

## Usage

### Running with ansible-navigator

```bash
# Run a playbook
ansible-navigator run <playbook>.yml

# Run in stdout mode
ansible-navigator run <playbook>.yml -m stdout
```

### Using roles

```yaml
- hosts: target_hosts
  roles:
    - role_name
```

## Requirements

- Ansible 2.9 or higher (via ansible-navigator)
- Required collections (see `collections/requirements.yml` if present)
- Appropriate access credentials configured via environment variables

## Directory Structure

```
Ansible-Inventory/
├── collections/        # Collection dependencies (if present)
└── ansible-navigator.yml  # Navigator configuration
```
