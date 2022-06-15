# Zabbix
Ansible Provisioning Zabbix for CentOS/7 :rocket:	

```
git clone https://github.com/bedrigue02/zabbix.git ~/zabbix
```

## Prerequisites
- Disable SElinux
- Disable Firewall

 
Install Ansible:
```
sudo yum install epel-release

sudo yum update && \
sudo yum install ansible
```

Install Ansible Galaxy dependencies for MariaDB:

```
ansible-galaxy collection install community.mysql
```

## Install Zabbix
Run playbook:
```
ansible-playbook -i hosts install_zabbix.yaml
```
