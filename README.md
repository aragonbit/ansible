# 🧰 Ansible Playbooks for User Management & Server Automation

This repository contains ready-to-use Ansible playbooks for managing Linux servers in a structured environment. It was created for semi-automated user provisioning, key rotation, and deprovisioning in a secure and reproducible way.

---

## 📦 What's Inside?

This repository provides:

- ✅ **User onboarding** with SSH key & sudo rights
- 🔐 **SSH key rotation** for secure access maintenance
- ❌ **Offboarding** of users incl. access revocation
- 📂 YAML inventories for different network zones (DMZ, MGMT, INTRA)
- 🧩 Integration-ready for [Ansible Semaphore](https://github.com/ansible-semaphore/semaphore)

---

## 📁 File Structure

```bash
playbooks/
├── onboarding.yml       # Add a new user with SSH key and optional sudo
├── offboarding.yml      # Remove a user from one or more servers
├── key_rotation.yml     # Rotate SSH key for existing user
