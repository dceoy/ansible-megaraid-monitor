ansible-megaraid-monitor
========================

Physical disk monitor using Ansible and Slack for MegaRAID

Preparation
-----------

```sh
$ git clone https://github.com/dceoy/ansible-megaraid-monitor.git
$ cd ansible-megaraid-monitor
$ cp examples/example_vars.yml vars.yml
$ vim vars.yml  # => edit
$ cp examples/example_hosts hosts
$ vim hosts     # => edit
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
