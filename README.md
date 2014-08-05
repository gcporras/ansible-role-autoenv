ansible-role-autoenv
========

An [Ansible](http://www.ansible.com/home) Role that installs and configures
[autoenv](https://github.com/kennethreitz/autoenv).

[![Build Status](https://travis-ci.org/gcporras/ansible-role-autoenv.png?branch=master)](https://travis-ci.org/gcporras/ansible-role-autoenv)


Requirements
------------

The following tools are required:
- [pip](https://pip.pypa.io/en/latest/installing.html) a tool for installing and managing Python packages.


Role Variables
--------------

Available variables are listed below, along with default values (see `defaults/main.yml`):

`autoenv_shell_rc_file` per default set to `{{ ansible_env['HOME'] }}/.{{ ansible_env['SHELL'] | replace('/bin/','') }}rc`

The shell's configuration file for which autoenv variables will be set.


Dependencies
------------

None.

Example Playbook
-------------------------

    - hosts: servers
      roles:
         - { role: gcporras.autoenv }

License
-------

MIT

Author Information
------------------

This role was created in 2014 by Gerardo Cepeda Porras.