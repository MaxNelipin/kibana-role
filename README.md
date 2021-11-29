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
| el_instance_ip | "{{hostvars['el-instance']['ansible_facts']['default_ipv4']['address']}}" | IP-адрес сервера Elasticsearch |
| supported_systems |  | Список поддерживаемых ОС |


Dependencies
------------

Example Playbook
----------------


    - hosts: servers
      roles:
         - { role: kibana-role, kibana_version: 7.15.1, el_instance_ip: 10.1.1.1 }

License
-------

BSD

Author Information
------------------

MaxNelipin