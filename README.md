# iStatD Ansible Script

## Install

```
$ ansible-playbook playbook.yml
```

## Get Configs

```
$ ansible all -m shell -a "cat /usr/local/etc/istatserver/istatserver.conf"
```