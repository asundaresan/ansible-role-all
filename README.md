# Meta package for ansible roles

This package contains all the ansible roles for different components as sub-modules.

Use the following code in an ansible YAML file to install required components. 

```
---
- name: Install and configure all components
  hosts: all
  become: yes
  become_method: sudo
  roles: 
  - base
  - timezone
  - ntp
  - ros 
```

