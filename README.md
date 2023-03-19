# HG Homelab

Homelab configurations and setup using Ansible.

Note: Ansible's vault lookup requires the env `OBJC_DISABLE_INITIALIZE_FORK_SAFETY=YES` to be set.

![Homelab](homelab.jpg)

Install requirements:
```
ansible-galaxy collection install -r collections.yaml
```

Run a playbook:
```
ansible-playbook -i hosts.ini playbooks/software.yaml --tags pihole
```