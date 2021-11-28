kibana-role
=========

Роль  установки kibana на rpm-системы

Requirements
------------

Role Variables
--------------
| Variable name | Default | Description |
|-----------------------|----------|-------------------------|
| kibana_version | "7.15.0" | Версия Kibana |
| supported_systems |  | Список поддерживаемых ОС |


Dependencies
------------

Example Playbook
----------------


    - hosts: servers
      roles:
         - { role: kibana-role, kibana_version: 7.15.1 }

License
-------

BSD

Author Information
------------------

MaxNelipin