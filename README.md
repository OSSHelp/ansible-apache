# Apache

[![Build Status](https://drone.osshelp.ru/api/badges/ansible/apache/status.svg)](https://drone.osshelp.ru/ansible/apache)

Ansible Role for Apache 2.4 installation

## Deploy example

```yaml
    - role: apache
      listen_port: 8080
      remove_default_vhost: true
      mods_enabled:
        - rewrite.load
      mods_disabled: []
```

## Available parameters

### Main

Short description here.

| Param | Default | Description |
| -------- | -------- | -------- |
| `listen_port` | `8080` | Default port to listen on |
| `remove_default_vhost` | `false` | Whether to delete default vhost |
| `mods_enabled` | `[rewrite.load]` | List of modules to enable |
| `mods_disabled` | `[]` | List of modules to disable |

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
