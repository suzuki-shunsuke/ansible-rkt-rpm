# ansible-rkt-rpm

ansible role to install rkt with rpm package.

https://galaxy.ansible.com/suzuki-shunsuke/rkt-rpm/

## Requirements

Nothing.

## Role Variables

name | required |  description
--- | --- | ---
rkt_version | yes | installed rkt version
rkt_rpm | yes | rpm file name

https://github.com/rkt/rkt/releases

## Dependencies

Nothing.

## Example Playbook

```yaml
- hosts: servers
  roles:
    - role: suzuki-shunsuke.rkt-rpm
      rkt_version: v1.29.0
      rkt_rpm: rkt-1.29.0-1.x86_64.rpm
      become: yes
```

## License

[MIT](LICENSE)
