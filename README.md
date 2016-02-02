# ansible-role-interfaces
Quick and dirty ansible role to configure multiple sequential ip addresses on ubuntu...

## example
### playbook
```YAML
---
- hosts: myhosts
  sudo: true
  roles:
    - interfaces
```

### host_vars
```YAML
---
ext_ip: 10.0.0.2
ext_ip_netmask: 255.255.255.0
ext_ip_gw: 10.0.0.1
ext_ip_bcast: 10.0.0.255
ext_ip_dns: 10.0.1.10 10.0.2.10
ext_ip_net: 10.0.0.0/24
extra_ip_addresses: 5
```
