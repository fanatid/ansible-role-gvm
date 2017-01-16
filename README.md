# gvm

[![Build Status](https://img.shields.io/travis/fanatid/ansible-role-gvm.svg?branch=master&style=flat-square)](https://travis-ci.org/fanatid/ansible-role-gvm)

## Requirements

git, bison, mercurial

## Role Variables

  - `gvm.user` remote user
  - `gvm.version` gvm version tag, or HEAD
  - `gvm.go_version` go version

You can find default values in [defaults/main.yml](https://github.com/fanatid/ansible-role-gvm/blob/master/defaults/main.yml)

## Dependencies

No depedencies.

## Example Playbook

```
- hosts: servers
  roles:
    - role: fanatid.gvm
      gvm:
        user: deploy
        version: '1.0.22'
        go_version: 'go1.7'
```

## LICENSE

This library is free and open-source software released under the MIT license.
