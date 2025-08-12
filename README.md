# 📦 Ansible Package Installer Playbook

## 📖 Overview
This Ansible playbook automates:
- Installing **Terraform**.
- Creating a dedicated **Ansible automation user**.
- Configuring **SSH key-based access** for the user.
- Setting up **secure sudo privileges**.

It ensures a controlled, repeatable, and secure environment for running infrastructure automation tasks.

---

## 🛠 Prerequisites
Before running this playbook:
1. **Ansible installed** on your control node.
2. Target server accessible via **SSH**.
3. Terraform binary (`terraform.zip`) placed in `/tmp` on the target server.
4. SSH public key file (`ansible-cloud-user.pub`) inside a `files/` directory in the project folder.
5. Sudoers configuration file (`sudoer_ansible-cloud-user`) inside the same project folder.

---

