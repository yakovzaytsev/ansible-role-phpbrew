Role Name
=========

Installs phpbrew

Example Playbook
----------------

How to use role:

    - hosts: servers
      roles:
         - role: ysz.php

then add task like this somewhere

    - name: phpbrew quick start
      shell: |
        phpbrew init
        echo "[[ -e ~/.phpbrew/bashrc ]] && source ~/.phpbrew/bashrc" >> ~/.bashrc
        source ~/.phpbrew/bashrc
        phpbrew update
        phpbrew --debug install --stdout 7.0 as 7.0-dev +default +intl
    
      become: yes
      become_user: "vagrant"


License
-------

BSD
