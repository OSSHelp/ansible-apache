# Apache

[![Build Status](https://drone.osshelp.ru/api/badges/ansible/apache/status.svg)](https://drone.osshelp.ru/ansible/apache)

An Ansible Role that installs Apache 2.4

## Requirements

No special requirements.

## Deploy example

```yaml
    - role: apache
      listen_port: 8080
      remove_default_vhost: true
      mods_enabled:
        - rewrite.load
      mods_disabled: []
```
