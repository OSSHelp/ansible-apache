# Apache

[![Build Status](https://drone.osshelp.ru/api/badges/ansible/apache/status.svg)](https://drone.osshelp.ru/ansible/apache)

Ansible Role for Apache 2.4 installation

## Deploy example

```yaml
    - role: apache
      apache_additional_modules:
        - libapache2-mpm-itk
        - libapache2-mod-php
      apache_listen_port: 8080
      apache_remove_default_vhost: true
      apache_mods_enabled:
        - rewrite.load
      apache_mods_disabled: []
```

## Available parameters

### Main

Short description here.

| Param | Default | Description |
| -------- | -------- | -------- |
| `apache_listen_port` | `8080` | Default port to listen on |
| `apache_additional_modules` | `[]` | List of additional modules to install |
| `apache_remove_default_vhost` | `false` | Whether to delete default vhost |
| `apache_mods_enabled` | `[rewrite.load]` | List of modules to enable |
| `apache_mods_disabled` | `[]` | List of modules to disable |

## FAQ

...

## Useful links

- [Official documentation](https://httpd.apache.org/docs/)

## TODO

...

## License

GPL3

## Author

OSSHelp Team, see <https://oss.help>
