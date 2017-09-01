Role Name
=========

Installs php-fpm

Role Variables
--------------

php_fpm should be path to UNIX socket

Dependencies
------------

Depends on nobreach.php_handlers to (re-)start php-fpm

Example Playbook
----------------

How to use role:

    - hosts: servers
      roles:
         - role: nobreach.php

License
-------

BSD
