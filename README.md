Role: cns.ansible
========

This role installs and configures ansible from source for specific users

Requirements
------------

Nothing, it runs out of the box.

Role Variables
--------------

In the current version, you can specify the following variables:

| Name               | Default |                                                              |
|--------------------|---------|--------------------------------------------------------------|
| admin_users        |   ---   | List containing all users that require ansible environment.  |
| ansible_user       |   ---   | Default user to use for playbooks if user is not specified.  |
| ansible_ssh_key    |   ---   | If set, always use this private key file for authentication. |


Dependencies
------------

This package has no dependencies.

License
-------

GPLv2

Author Information
------------------

Created by Sam Morrison [@samcns](https://www.twitter.com/samcns)

Examples
--------

```yaml
---
- name: common role test
  hosts: all
  roles:
    - cns.ansible
```
