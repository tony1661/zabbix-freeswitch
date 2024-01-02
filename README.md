# freeswitch-zabbix
A monitoring template for Freeswitch via Zabbix

This repo has the monitoring scripts and templates for monitoring Freeswitch via Zabbix.

Currently, it will detect the active calls on a gateway as well as if the freeswitch systemd service is running.

## Install
To install, take the freeswitch.conf file in this repo and save it to the /etc/zabbix/zabbix_agentd.d/ folder.

Next, upload the zabbix template in this repo to your Zabbix server. This can be done by doing to **Configuration>Templates** and clicking the **Import** button.
