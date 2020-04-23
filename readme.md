# Bitwarden(rs) VPS

![Ansible CI](https://github.com/eliseomartelli/bitwarden_vps_docker/workflows/Ansible%20CI/badge.svg)

Setups a machine to serve bitwarden(rs) using caddy as a proxy.
Powered by ansible.

## Prerequisites

1. A server
2. Ansible installed on your machine.

## Install

```bash 
# Clone the repo
git clone https://github.com/eliseomartelli/bitwarden_vps_docker

# Enter the repo directory
cd bitwarden_vps_docker

# Copy the default variable file
cp variables/default.yaml.stub variables/default.yaml

# Edit the default variable file
vi variables/default.yaml # Put your domain name here

# Copy the inventory file
cp inventory.stub inventory

# Edit the inventory file
vi inventory # Put your inventory here

# Run the playbook
ansible-playbook -i inventory -k playbook.yaml
```
