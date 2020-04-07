General utilities ansible role
=========
This role installs sdorra scmmanager

Requirements
------------
None

Role Variables
--------------
This role requires the following variables to be defined elsewhere in the playbook that uses it:
```yaml
  scmmanager_admin_user:        admin      # Webconsole admin user name
  vault_scmmanager_password                # Webconsole admin user password. It should be encryted in vault
```

All of them are already defined in /defaults/main.yml, feel free to overwrite them

Dependencies
------------
None

Example Playbook
----------------
Register the role in requirements.yml:
```yaml
    - src: capitanh.scmmanager_ansible_role
      name: scmmanager
```
Include it in your playbooks:
```yaml
    - hosts: servers
      roles:
      - scmmanager
```
License
-------
BSD
