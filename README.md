
# Ansible Apache Web Server Automation

## Project Overview
This project uses Ansible to automatically install and configure Apache on an AWS EC2 Ubuntu server and deploy a website.

## Architecture
- Control Node: AWS EC2 Ubuntu with Ansible installed.
- Managed Node: AWS EC2 Ubuntu running Apache.
- Connection: SSH.

## Technologies
- AWS EC2
- Ubuntu Linux
- Ansible
- YAML
- Apache HTTP Server

## Project Structure

```text
ansible-level2/
├── ansible.cfg
├── inventory/
│   └── hosts.ini.example
├── playbooks/
│   └── install_apache.yml
├── files/
│   └── index.html
├── templates/
└── .gitignore
```

## Deployment Steps

1. Install Ansible on the control node.
2. Configure the inventory.
3. Configure SSH access to the managed node.
4. Run the playbook:

```bash
ansible-playbook playbooks/install_apache.yml
```

## Result

Apache is installed and enabled automatically, and the website is deployed to:

`/var/www/html/index.html`

## Author
Sachin Santhosh
