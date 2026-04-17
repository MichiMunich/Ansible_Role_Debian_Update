# Debian Update Ansible Role

A simple and reliable Ansible role for updating Debian-based systems.

## Overview

This role automates the process of updating packages on Debian-based systems. It handles package cache refresh, system updates, and optionally removes unnecessary packages to keep your systems clean and secure.

## Functionality
The debian_update role performs the following tasks:

- Update package cache — Refreshes the APT package index
- Install available updates — Upgrades all packages to their latest versions
- Reboot if required — Optionally restarts the system if kernel updates are applied
- Remove unnecessary packages — Optionally cleans up unused dependencies (autoremove)

## Further information
https://blog.doenselmann.com/linux-server-mit-ansible-aktualisieren/

## Prerequisites

- **Ansible** >= 2.9
- **Target systems** running Debian or Debian-based distributions (Ubuntu, etc.)
- **SSH access** to target hosts with appropriate privileges (sudo)

## Installation
### Clone the repository:
```bash
git clone https://github.com/MichiMunich/Ansible_Role_Debian_Update.git
cd Ansible_Role_Debian_Update
```

## Running the Playbook

Execute the playbook using the following command:
```bash
ansible-playbook -i inventory/hosts.yml playbooks/role_debian_update.yml -vv
```

