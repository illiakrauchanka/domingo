## Warning
During the playbook execution target server(s) will be rebooted, it means a prior downtime should be scheduled.  

## Run the Playbook
ansible-playbook playbooks/playbook.yml -i inventory/production --ask-vault-pass

### Verify CPU settings
because of EC2 instance was running as a target host, there is no options to tune CPU's settings.  
cat /sys/devices/system/cpu/cpu*/cpufreq/scaling_governor
