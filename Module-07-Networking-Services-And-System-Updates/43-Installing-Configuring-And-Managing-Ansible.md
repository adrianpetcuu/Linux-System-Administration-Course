## Installing, Configuring and Managing Ansible

Ansible is an automation
tool used for configuration
management, application
deployment, and orchestration.

### Key Features
- Agentless architecture
- Uses SSH for communication
- Written in YAML (playbooks)
- Simple and powerful automation

### Install Ansible
```bash
dnf install ansible -y
```

### Verify Installation
```bash
ansible --version
```

### Ansible Configuration Files
- `/etc/ansible/ansible.cfg`
- `/etc/ansible/hosts`

### Inventory File Example
```text
[servers]
server1
server2
```

### Test Connectivity
```bash
ansible all -m ping
```

### Basic Playbook Example
```yaml
- name: Install Apache
  hosts: servers
  become: yes
  tasks:
    - name: Install httpd
      dnf:
        name: httpd
        state: present
```

### Run Playbook
```bash
ansible-playbook playbook.yml
```

### Summary
Ansible simplifies system
administration by automating
tasks consistently across
multiple Linux servers.
