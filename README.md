[![Build Status](https://drone.kiwi-labs.net/api/badges/Diesel-Net/rt-ax88u/status.svg)](https://drone.kiwi-labs.net/Diesel-Net/rt-ax88u)

# rt-ax88u
Automation for Asus RT-AX88U Router running Asuswrt-Merlin

# Dependencies
- Asus Router RT-AX88U running Asuswrt-Merlin firmware
- Ansible 2.10+

# Renew TLS Certificates
1. Update certificate data in [certificates.yaml](.ansible/inventory/production/group_vars/rt-ax88u/certificates.yaml)

2. Deploy new certificates
```bash
ansible-playbook .ansible/update_certificate.yaml -i .ansible/inventory/production/hosts --vault-id ~/.tokens/master_id
```
