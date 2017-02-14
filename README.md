# Ansible role: rbenv

[![Build Status](https://travis-ci.org/danbohea/ansible-role-rbenv.svg?branch=master)](https://travis-ci.org/danbohea/ansible-role-rbenv)

Installs rbenv on macOS.


## Requirements

- macOS 10.10, 10.11 or 10.12


## Role Variables

```
rbenv_default_ruby_version: "2.1.2"

rbenv_global_gems:
  - "bundler"
  - "travis"
```


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

This role was created by [Dan Bohea](https://bohea.uk) primarily for use with [Macsible](https://github.com/macsible/macsible).
