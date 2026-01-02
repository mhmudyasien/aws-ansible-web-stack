# aws-ansible-web-stack

# aws-ansible-web-stack

Automated deployment of a secure Nginx web server on AWS using Ansible.

> 🔧 **DevOps focus**: Infrastructure-as-Code, idempotency, security, and reproducibility.

---

## ✨ Features
- Provisions EC2 instance
- Creates minimal security group (HTTP + SSH)
- Installs and configures Nginx
- Deploys a dynamic welcome page
- Fully idempotent and CLI-driven

---

## 🚀 Quick Start

### Prerequisites
- AWS CLI configured (`~/.aws/credentials`)
- Ansible ≥ 6.0
- Python 3.8+
- An existing SSH key in AWS named `ansible-web-key` (or update `playbooks/deploy-web-server.yml`)

### Run
```bash
# Install dependencies
pip install -r requirements.txt

# Run playbook
ansible-playbook playbooks/deploy-web-server.yml
