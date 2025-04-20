# System Updater

This repo is a mirror repo to hold just the system updater role from [mshafer1/ansible_configs](/mshafer1/ansible_configs/playbooks/roles/system_updater)

## Customization

To customize the settings, create an Ansible inventory file and specify the veriables for the current system.

```yaml
# example /etc/ansible/hosts
all:
  hosts:
    localhost:
      # use weekday variable to specify what day to do updates on
      # update_job_weekday: MON
      grub_handled: false
      ansible_connection: local
```
