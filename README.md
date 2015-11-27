Ansible Role for MySQL Database
===============================

[![Build Status](https://travis-ci.org/pantarei/ansible-role-mysql-db.svg?branch=master)](https://travis-ci.org/pantarei/ansible-role-mysql-db)
 [![GitHub tag](https://img.shields.io/github/tag/pantarei/ansible-role-mysql-db.svg)](https://github.com/pantarei/ansible-role-mysql-db)
 [![GitHub license](https://img.shields.io/github/license/pantarei/ansible-role-mysql-db.svg)](https://github.com/pantarei/ansible-role-mysql-db/blob/master/LICENSE)
 [![Ansible Role](https://img.shields.io/ansible/role/5978.svg)](https://galaxy.ansible.com/detail#/role/5978)

Ansible Role for MySQL Database Management.

Requirements
------------

This role require Ansible 1.9 or higher.

This role was designed for Ubuntu Server 14.04 LTS.

Role Variables
--------------

<table>
<colgroup>
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
<col width="20%" />
</colgroup>
<thead>
<tr class="header">
<th align="left">parameter</th>
<th align="left">required</th>
<th align="left">default</th>
<th align="left">choices</th>
<th align="left">comments</th>
</tr>
</thead>
<tbody>
<tr class="odd">
<td align="left">mysql_db_collation</td>
<td align="left">yes</td>
<td align="left">utf8_general_ci</td>
<td align="left"></td>
<td align="left">Pass value as <code>collation</code> to <a href="http://docs.ansible.com/ansible/mysql_db_module.html">mysql_db module</a>.</td>
</tr>
<tr class="even">
<td align="left">mysql_db_encoding</td>
<td align="left">yes</td>
<td align="left">utf8</td>
<td align="left"></td>
<td align="left">Pass value as <code>encoding</code> to <a href="http://docs.ansible.com/ansible/mysql_db_module.html">mysql_db module</a>.</td>
</tr>
<tr class="odd">
<td align="left">mysql_db_name</td>
<td align="left">yes</td>
<td align="left">example</td>
<td align="left"></td>
<td align="left">Pass value as <code>name</code> to <a href="http://docs.ansible.com/ansible/mysql_db_module.html">mysql_db module</a>.</td>
</tr>
</tbody>
</table>

Dependencies
------------

-   [hswong3i.mysql\_user](https://github.com/pantarei/ansible-role-mysql-user)

Example Playbook
----------------

    - hosts: servers
      roles:
        - { role: hswong3i.mysql_db, mysql_db_collation: 'utf8_general_ci', mysql_db_encoding: 'utf8', mysql_db_name: 'example' }

License
-------

-   Code released under [MIT](https://github.com/pantarei/ansible-role-mysql-db/blob/master/LICENSE)
-   Docs released under [CC BY 4.0](http://creativecommons.org/licenses/by/4.0/)

Author Information
------------------

-   Wong Hoi Sing Edison
    -   <https://twitter.com/hswong3i>
    -   <https://github.com/hswong3i>

