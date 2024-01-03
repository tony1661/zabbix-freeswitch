# freeswitch-zabbix
A monitoring template for Freeswitch via Zabbix

This repo has the monitoring scripts and templates for monitoring Freeswitch via Zabbix.

Currently, it will detect the active calls on a gateway as well as if the freeswitch systemd service is running.

## Install
### Step 1
To install, take the freeswitch.conf file in this repo and save it to the /etc/zabbix/zabbix_agentd.d/ folder.

### Step 2
Next, upload the zabbix template in this repo to your Zabbix server. This can be done by doing to **Configuration>Templates** and clicking the **Import** button.

### Step 3
Go to your `/etc/zabbix/agentd.conf` file and add the following line: `AllowKey=system.run["systemctl status freeswitch | grep -q running;echo $?"]`

## Sample Dashboard
![image](https://github.com/tony1661/freeswitch-zabbix/assets/5287266/78e96d3c-4657-4b6a-9d06-2aec12b9a3fa)
