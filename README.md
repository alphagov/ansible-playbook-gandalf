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

`tsuru_api_endpoint` uri to tsuru api, defaults to `http://localhost:8080`

`archive_server_version` version of the archive server you wish to install, defaults to `latest`

`gandalf_server_version` version of the gandalf server you wish to install, defaults to `latest`

`tsuru_repo` repo argument for Ansible's [`apt_repository`](http://docs.ansible.com/ansible/apt_repository_module.html) module, defaults to `ppa:tsuru/ppa`

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
