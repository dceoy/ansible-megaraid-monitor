ansible-megaraid-monitor
========================

Physical disk monitor using Ansible and Slack for MegaRAID

Preparation
-----------

```sh
$ git clone https://github.com/dceoy/ansible-megaraid-monitor.git
$ cd ansible-megaraid-monitor
$ cp templates/template_vars.yml vars.yml
$ vim vars.yml  # => edit
$ cp templates/template_hosts.yml hosts.yml
$ vim hosts.yml  # => edit
```

Usage
-----

Monitor physical disks

```sh
$ ansible-playbook -i hosts monitor_drives.yml
```

Clear previous cache

```sh
$ ansible-playbook -i hosts clear_monitor_cache.yml
```