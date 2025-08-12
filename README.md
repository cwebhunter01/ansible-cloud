# 🛠 Ansible Cloud Setup Automation

This repository contains Ansible playbooks and configuration files for automating the setup of an Ansible environment, installing Terraform, creating a dedicated Ansible user, configuring SSH access, and granting sudo privileges.

---

## 📌 Overview

The playbooks in this repository will:

1. Install **Terraform** on target servers.
2. Create an **Ansible Cloud user**.
3. Set up **SSH keys** for passwordless access.
4. Configure **sudo privileges** for the Ansible Cloud user.
5. Provide a rollback playbook to remove all installed components.

---

## 📂 Repository Structure

```plaintext
ansible-cloud/
│
├── ansible.cfg                   # Ansible configuration
├── inventory.ini                  # Target host inventory
├── package_installer.yml          # Main setup playbook
├── remove_package_installer.yml   # Rollback / uninstall playbook
├── package_installer.yml.save     # Backup of main playbook
├── files/
│   ├── ansible-cloud-user.pub     # Public SSH key for Ansible Cloud user
│   └── sudoer_ansible-cloud-user  # Sudoers file for Ansible Cloud user
└── README.md
