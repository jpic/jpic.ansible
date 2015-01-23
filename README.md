Ansibleenv
==========

Ansibleenv enables the same workflows as with virtualenv and pip, by
making an ansible.cfg with a configurable root for plugins, roles, modules
etc ...

Role Variables
--------------

- ansibleenv_cfg: path to the configuration file to write (default:
  ~/.ansible.cfg)
- ansibleenv_root: path to the ansibleenv root (default: ~/ansibleenv)


Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      roles:
         - role: jpic.ansibleenv
           ansibleenv_cfg: ~/.ansible.cfg
           ansibleenv_root: ~/ansibleenv

License
-------

BSD
