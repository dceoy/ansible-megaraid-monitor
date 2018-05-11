ansible-megaraid-monitor
========================

Version: v0.2.2

Physical disk monitor using Ansible and Slack for MegaRAID

Requirements of remote servers
------------------------------

This tool's operation was checked using StorCli SAS Customization Utility Ver 1.23.02.

- StorCLI

Preparation
-----------

```sh
$ git clone https://github.com/dceoy/ansible-megaraid-monitor.git
$ cd ansible-megaraid-monitor
$ cp example_hosts hosts
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
