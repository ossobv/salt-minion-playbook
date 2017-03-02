salt-minion-playbook
=========

Ansible playbook which installs the latest version of the salt-minion and adds an entry to the `/etc/hosts` file.

Requirements
------------

None.

Role Variables
--------------

Please configure the following variables:

- saltmaster.ip
- saltmaster.hostname

If these are not set, the playbook will use the defaults!

Dependencies
------------

None.

Example Playbook
----------------

    - hosts: servers
      vars:
        saltmaster:
          ip: 10.10.10.15
          hostname: salt
      roles:
         - ossobv.salt-minion-playbook


License
-------

GNU GPLv3

Author Information
------------------

Jordi de Wal | OSSO B.V. <jdwal@osso.nl>
