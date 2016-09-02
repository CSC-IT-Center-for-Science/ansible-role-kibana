ansible-role-kibana4
=========

Installs and configures Kibana4

Tested With
------------

 - ES 2.3-2.4
 - Kibana 4.5-4.6

Role Variables
--------------

see defaults/main.yml

The important ones:

 - kibana4_tar: False
 - kibana4_yum: True
 - kibana_branch: "4.6"

This is the default and means that kibana version kibana_branch is installed from yum.

Related Roles
------------

<pre>
# sets up a curator cronjob (retention handling)
- src: https://github.com/CSC-IT-Center-for-Science/ansible-role-elasticsearch-curator

# elasticsearch role configures elasticsearch
- src: https://github.com/CSC-IT-Center-for-Science/ansible-role-elasticsearch

# installs elastic repos and then installs software from there - logstash and elasticsearch
- src: https://github.com/CSC-IT-Center-for-Science/ansible-role-elk
</pre>



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
