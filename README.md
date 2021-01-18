# rt-ax88u
Automation for Asus RT-AX88U Router running Asuswrt-Merlin

# Dependencies
- Asus Router RT-AX88U running Asuswrt-Merlin firmware
- Ansible 2.10+

# Renew TLS Certificates
1. Update certificate data at [group_vars/all/certificates.yaml](group_vars/all/certificates.yaml)

2. Deploy new certificates
```bash
ansible-playbook renew_certificates.yaml -i inventory/prod/hosts --vault-id ~/.tokens/master_id
```
