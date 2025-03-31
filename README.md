# Ansible Role: Docker Engine

An Ansible Role that installs docker engine on linux for [LUDUS](https://ludus.cloud/).

## Requirements

- Linux server
- Internet connection

Check on :

- Debian 11
- Debian 12
- Rocky 8
- Rocky 9
- Ubuntu 20.04
- Ubuntu 24.04

## Role Variables

Available variables are listed below, along with default values (see `defaults/main.yml`):

```yaml
ludus_docker_engine_add_localuser: false
```

## Dependencies

## Example Playbook

## Example Ludus Range Config

```yaml
ludus:
  - vm_name: "{{ range_id }}-linux"
    hostname: "{{ range_id }}-linux"
    template: ubuntu-24.04-x64-server-template
    vlan: 99
    ip_last_octet: 2
    ram_gb: 12
    cpus: 4
    linux: true
    roles:
      - frack113.ludus_docker_engine
```

## License

[//]: # (If you change the License type, be sure to change the actual LICENSE file as well)
GPLv3

## Author Information

This role was created by [frack113](https://github.com/frack113), for [Ludus](https://ludus.cloud/).
