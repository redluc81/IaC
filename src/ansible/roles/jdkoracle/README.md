JDK 8 Ansible Playbook
=========

This role downloads and installs Oracle JDK 8

Requirements
------------

None

Role Variables
--------------

This role requires the following variables to be defined elsewhere in the playbook that uses it:
```yaml
  - jdk_basedir            # Installation directory
```

Dependencies
------------

None

Example Playbook
----------------

Register the role in requirements.yml:
```yaml
- src: capitanh.oraclejdk-ansible-role
  name: oraclejdk
```
Include it in your playbooks:
```yaml
- hosts: servers
  roles:
    - oraclejdk
```


License
-------

BSD

