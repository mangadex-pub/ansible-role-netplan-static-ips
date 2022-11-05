# ansible-role-netplan-static-ips

###### Status: Unstable

(Persistently) add extra IPs to network interfaces using netplan.

## Example

```yaml
- name: Ensure extra IP addresses
  ansible.builtin.include_role: mangadex.netplan_static_ips
  vars:
    netplan_static_ips:
      lo: [ 1.2.3.4/32, 1.2.3.5/32 ]
      eth0: [ 5.6.7.8/26 ]
```
