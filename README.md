Role Name
=========

* This is ansible automation to install and use mysql 5.7 on Ubuntu Server.\
* Role name is install-mysql.\
* To use this ansible-playbook, first create a role directory and clone this repo.\
* Then, copy hosts file and mysqlsetup.yml from templates folder in outside of the roles directory.
* Templates folder has also the information of root password in file (root-my.cnf.j2) which then will be copied after running the playbook as /root/.my.cnf. The module of mysql will attempt to read the credentials from ~/.my.cnf to login.

Requirements
------------

This mysql setup has been tested and applied in ubuntu 16.04 and 18.04.


Role Variables
--------------

vars/main.yml contains the root user name and password.


Example Playbook
----------------

Then execute following command from outside the roles directory.\
ansible-playbook mysqlsetup.yml

Also, the following command will list the tags and run the tags accordingly.\
ansible-playbook mysqlsetup.yml --list-tags

For example to run the listed tags, execute the following command:\
ansible-playbook mysqlsetup.yml -t Add_user\
\
-t flag let you use the tags. The above playbook will only add the new mysql user using the tags.

Author Information
------------------

Sushan Kunwar\
System Engineer/DevOps Engineer
