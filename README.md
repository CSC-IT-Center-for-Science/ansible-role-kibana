ansible-role-kibana4
=========

Installs and configures Kibana4

Requirements
------------

 - ES 2.3
 - Kibana 4.6

Role Variables
--------------

see defaults/main.yml

The two important ones:

 - kibana4_tar: False
 - kibana4_yum: True
 - kibana_branch: "4.6"

This is the default and means that kibana version kibana_branch is installed from yum.

Dependencies
------------


Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - { role: ansible-role-kibana4 }

License
-------

MIT

Author Information
------------------
