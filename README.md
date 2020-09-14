ansible-role-win-kms
====================

[![Ansible Role: bit_kitchen.win_kms](https://img.shields.io/ansible/role/50686.svg)](https://galaxy.ansible.com/bit_kitchen/win_kms)
[![Build Status](https://travis-ci.org/bit-kitchen/ansible-role-win-kms.svg?branch=master)](https://travis-ci.org/bit-kitchen/ansible-role-win-kms)

Set the name and/or the port of the KMS host to use and activate Windows.

    ansible-galaxy install bit_kitchen.win_kms

Requirements
------------

None.

Role Variables
--------------

Variable | Default   | Comment
-------- | --------- | -------
kms_host | undefined | Name and/or the port for the KMS computer the target machine will use. <br> IPv6 address must be specified in the format `[hostname]:port`.

Dependencies
------------

None.

Example Playbook
----------------

```yml
- hosts: windows
  roles:
  - name: bit_kitchen.win_kms
    kms_host: kms.example.com
```

License
-------

[MIT](LICENSE)

Author Information
------------------

[bit.kitchen](https://github.com/bit-kitchen)
