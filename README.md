# Ansible role: rbenv

[![Build Status](https://travis-ci.org/danbohea/ansible-role-rbenv.svg?branch=master)](https://travis-ci.org/danbohea/ansible-role-rbenv)

Installs rbenv on macOS.


## Requirements

- macOS 10.10, 10.11 or 10.12


## Role Variables

```YAML
# The default version of Ruby to be initially installed via rbenv.
rbenv_default_ruby_version: "2.1.2"

# Any global gems to be installed with the default Ruby version.
rbenv_global_gems:
  - "bundler"
  - "travis"

# Whether the role should add the line `eval \"$(rbenv init -)\"` to .bash_profile.
# If set to false you'll want to consider adding this line yourself.
rbenv_update_bash_profile: false
```


## Dependencies

- [danbohea.homebrew](https://galaxy.ansible.com/danbohea/homebrew)


## Example Playbook

```YAML
- hosts: macbook
  connection: local

  roles:
    - role: ansible-role-rbenv
```


## License

MIT


## Author Information

This role was created by [Dan Bohea](https://bohea.uk).
