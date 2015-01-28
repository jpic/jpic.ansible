Ansible
=======

Ansible role enables the same workflows as with virtualenv and pip, by making
an ansible.cfg with a configurable root for plugins, roles, modules etc ...

Role Variables
--------------

- ansible_cfg: path to the configuration file to write (default:
  ~/.ansible.cfg)
- ansible_root: path to the ansible root (default: ~/ansible)
- ansible_libraries: list of git repositories to clone in 
  ``{{ ansible_root }}/libraries``.


Example Playbook
----------------

Example to create an ansible environment in ~/.ansible

    - hosts: servers
      roles:
      - role: jpic.ansible
        ansible_cfg: ~/.ansible.cfg
        ansible_root: ~/ansible
        ansible_libraries:
        - https://github.com:robparrott/ansible-vagrant.git


License
-------

BSD
