# Ansible role: rbenv

Installs rbenv on macOS.


## Requirements

- macOS 10.10, 10.11 or 10.12


## Role Variables

See defaults/main.yml


## Dependencies

- [danbohea.homebrew](https://galaxy.ansible.com/danbohea/homebrew)


## Example Playbook

```
- hosts: macbook
  connection: local

  roles:
    - role: ansible-role-rbenv
```

## License

MIT


## Author Information

This role was created by [Dan Bohea](http://bohea.co.uk) primarily for use with [Macsible](https://github.com/macsible/macsible).
