# ansible-ssh-port
## Description
Detect the host's SSH port between a primary (22) and alternate (variable) and update the listening port as needed.

# (WIP)

## Usage
playbook.yaml
```
---
- name: Playbook Name
  hosts: MyHosts
  become: yes
  gather_facts: no
  
  roles:
    - role: notmycloud.ssh-port
      vars:
        ssh_port_change: false    # Specify true if you want this role to update the SSH listening port to the specified ansible_port.
        ansible_port: 22          # Specify which port SSH "should" be listening on.
```

## Support
For support, please raise an issue and provide the following items
- Sample task/playbook to replicate your issue
- Resultant file that is created.
- If modifying an existing file, please provide the unmodified version as well.
