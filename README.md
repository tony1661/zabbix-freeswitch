# freeswitch-zabbix
A monitoring template for Freeswitch via Zabbix

This repo has the monitoring scripts and templates for monitoring Freeswitch via Zabbix.

Currently, it will
  - automatically discover all gateways on your freeswitch system
  - log the inbound and outbound calls for each gateway
  - detect the status of the freeswitch service via systemd
  - log all registrations on the system (this includes gateways) in a single item
  - log all configured extensions (FusionPBX only)

## Install
### Step 1
To install, take the freeswitch.conf file in this repo and save it to the /etc/zabbix/zabbix_agentd.d/ folder.

### Step 2
Next, upload the zabbix templates in this repo to your Zabbix server. This can be done by doing to **Configuration>Templates** and clicking the **Import** butto

## Sample Dashboard
![image](https://github.com/tony1661/freeswitch-zabbix/assets/5287266/78e96d3c-4657-4b6a-9d06-2aec12b9a3fa)
