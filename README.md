squid3-squidguard
=========

Ansible scripts to install squid3 proxy server, squidguard redirector with custom blacklists and zabbix agent with squidclient to get that stuff monitored.

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

No

License
-------

BSD

Author Information
------------------

Andrew Nazarov
