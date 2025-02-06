## Run the Playbook
ansible-playbook playbooks/playbook.yml -i inventory/production --ask-vault-pass

### Verify CPU settings

cat /sys/devices/system/cpu/cpu*/cpufreq/scaling_governor