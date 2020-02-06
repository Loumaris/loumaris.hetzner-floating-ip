# loumaris.hetzner-floating-ip

A small playbook to setup the floating ip on hetzner cloud.

## usage

Example inside a playbook:

```yaml
- name: apply common configuration to all nodes
  hosts: all
  roles:
    - { role: loumaris.hetzner-floating-ip, ip_v4: '1.1.1.1', ip_v6: '1:2:3:4 }
```
## configuration

Possible parameter with default:

* `interface`: _eth0_
* `ip_v4`
* `ip_v6`