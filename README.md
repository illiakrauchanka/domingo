## Warning
During the playbook execution target server(s) will be rebooted, it means a prior downtime should be scheduled.  

## Vault secret
`group_vars/all/secrets.yml`
https://eu.onetimesecret.com/secret/1foa0ohutb04ww16nnj6p0sz0aw5sjw

## Run the Playbook
`ansible-playbook playbooks/playbook.yml -i inventory/production --ask-vault-pass`

### Verify CPU settings
because of EC2 instance was running as a target host, there is no options to tune CPU's settings.  
cat /sys/devices/system/cpu/cpu*/cpufreq/scaling_governor
