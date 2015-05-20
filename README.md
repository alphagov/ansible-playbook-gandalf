Gandalf
=========

An ansible role to install a [gandalf](https://gandalf.readthedocs.org/en/latest/) server.

Requirements
------------

Only tested on Ubuntu 14.04.

Role Variables
--------------

`gandalf_port` port that gandalf listens on.

`gandalf_git_template_dir` directory where git templates are stored.

Dependencies
------------

* None

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: gandalf-server
      roles:
         - { role: gandalf, gandalf_port: 8080, gandalf_git_template_dir: /home/git/bare-template }

License
-------

See `LICENSE` file.
