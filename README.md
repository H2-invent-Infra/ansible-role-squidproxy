squidproxy
=========

Ansible scripts to install squid3 proxy server, squidguard redirector with custom blacklists and squidclient that is used by zabbix to get that stuff monitored. Role to install zabbix agent is not included in that pack, but it was there in the past.

Due to some limitations of the current workflow, templates for configuration files have not been made. So, all configuration files must be preconfigured and put on files/ directory of every role. This strategy works well for me, but couldn't be suitable for somebody else.

WARNING! Put your own configuration files and blacklists into specified directories (see group_vars), otherwise these scripts wont work correctly. (As an example I put default configs to files/ directories).

Requirements
------------

Ansible > 1.8

Debian Jessie

Role Variables
--------------

All self-explanatory variables are located at group_vars directory. They are linked to 'proxy' group in /etc/ansible/hosts.

Dependencies
------------

No. But it wouldn't be harmful to play a role which installs zabbix agent.

License
-------

BSD

Author Information
------------------

Andrew Nazarov
