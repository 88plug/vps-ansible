# vps-ansible
Meticulously crafted Ansible playbooks designed to streamline the process of setting up VPS servers with speed and precision. Whether you prefer Vultr, DigitalOcean, OVH, or other providers, our versatile playbooks are your key to hassle-free server provisioning.

## Requirements
```
apt-get update
apt-get install -y ansible-playbook
git clone https://github.com/88plug/vps-ansible ; cd vps-ansible
```
**You must edit inventory.ini with the new VPS/SSH host.**

## Run
```
ansible-playbook -i inventory.ini playbook.yml
```

Run and install optional Docker and docker-compose
```
ansible-playbook -i inventory.ini playbook.yml -e "install_docker=true"
```
