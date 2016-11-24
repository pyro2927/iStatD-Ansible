# iStatD Ansible Script

![](https://bjango.com/images/mac/istat3/istat-macbook.png)

This Ansible script is meant to target Linux (specifically Debian/Ubuntu at this time) hosts and install [istatserver](https://bjango.com/help/istat3/linuxpackages/) on them, for use with iStat for [macOS](https://bjango.com/mac/istat/) and [iOS](https://bjango.com/ios/istat/).

## Setup

You'll need to create a `hosts` file according to the Ansible [inventory](http://docs.ansible.com/ansible/intro_inventory.html) guide.

## Run

```
$ ansible-playbook playbook.yml
```

## Get Configs

You'll want the see the config in order to know what the automatically generated server code is.

```
$ ansible all -m shell -a "cat /usr/local/etc/istatserver/istatserver.conf | grep code"
```