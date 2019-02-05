Role Name
=========

Transport logs to our elks cluster

Requirements
------------

a working elks cluster

Role Variables
--------------

InjestIP
InjestPort
InJestProto

Dependencies
------------

none

Example Playbook
----------------

---
- name: Push logs to elks stack
  hosts: elks
  become: true
  become_user: root
  roles:
    - role: weaselkeeper.logging

License
-------

BSD

Author Information
------------------

Jim Richardson <weaselkeeper@gmail.com>
