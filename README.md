Role Name
=========

This is ansible automation to install and use mysql 5.7 on Ubuntu Server.\
Role name is install-mysql.\
To use this ansible-playbook, first create a role directory and clone this repo.\
Then, copy hosts file and mysqlsetup.yml from templates folder in outside of the roles directory.

Requirements
------------

This mysql setup has been tested and applied in ubuntu 16.04 and 18.04.


Role Variables
--------------

vars/main.yml contains the root user name and password.


Dependencies
------------

templates folder has also the information of root password in file (root-my.cnf.j2) which then will be copied after running the playbook as /root/.my.cnf. The module of mysql will attempt to read the credentials from ~/.my.cnf to login.

Example Playbook
----------------

T

Author Information
------------------

Sushan Kunwar\
System Engineer/DevOps Engineer
