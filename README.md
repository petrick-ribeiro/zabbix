# Zabbix
Ansible Provisioning Zabbix for CentOS/7

## Prerequisites
- Disable SElinux
- Disable Firewall

 
Install Ansible:
```
sudo yum install epel-release
sudo yum install ansible
```

Install Ansible Galaxy dependencies for MariaDB:

```
ansible-galaxy collection install community.mysql
```

Run playbook:
```
ansible-playbook -i hosts install_zabbix.yaml
```
