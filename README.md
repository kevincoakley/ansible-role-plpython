ansible-role-plpython
=====================
[![Build Status](https://travis-ci.org/kevincoakley/ansible-role-plpython.svg?branch=master)](https://travis-ci.org/kevincoakley/ansible-role-plpython)

Installs and enables plpython for PostgreSQL 10 and 11. Tested with plpython on CentOS and Ubuntu 18.04 and plpython3 on Ubuntu 18.04. 

Requirements
------------

None

Role Variables
--------------

See defaults/main.yml and the example inventory below

Dependencies
------------

PostgreSQL 10 or 11 installed. kevincoakley.ansible_role_postgres can be used.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

        - name: Converge
          hosts: all
          become: true
        
          vars:
            - postgres_major_version: 11
        
          roles:
            - role: ansible-role-plpython

License
-------

BSD

Author Information
------------------

Kevin Coakley (https://github.com/kevincoakley)