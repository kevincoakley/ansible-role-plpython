ansible-role-plpython
=====================
![](https://github.com/kevincoakley/ansible-role-plpython/workflows/Molecule%20Test/badge.svg)

Installs and enables plpython for PostgreSQL 10, 11 and 12. Tested with plpython on CentOS 7, 8 and Ubuntu 18.04. 

Requirements
------------

None

Role Variables
--------------

See defaults/main.yml and the example inventory below

Dependencies
------------

PostgreSQL 10, 11 or 12 installed. kevincoakley.postgres can be used.

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