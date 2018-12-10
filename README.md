[![Build Status](https://www.travis-ci.org/securCom/ansible-role_repo-epel.svg?branch=master)](https://www.travis-ci.org/securCom/ansible-role_repo-epel)
[![GitHub release](https://img.shields.io/github/release/securCom/ansible-role_repo-epel.svg)](https://github.com/securCom/ansible-role_repo-epel)


# Repo: EPEL

Manage Extra Packages for Enterprise Linux (or EPEL) repository.

# Requirements

For supported systems  see https://fedoraproject.org/wiki/EPEL. If your system is not supported,
the role tasks will be skipped.

For supported system by this role, see the `vars/os-<system>` files.

Feel free to add any new linux distribution and version if missing.

# Role Variables

- `epel_repo_package_state`: the epel package presence  state

# Dependencies

There no external dependencies.

# Example Playbook

To install role, add following line to **ansible-galaxy** requirements file
```
- src: https://github.com/securCom/ansible-role_repo-epel
  version: master
  name: securcom.repo_epel
```

```
- hosts: servers
  roles:
     - securcom.repo_epel
```

# License

BSD

# Author Information


- Peter Hudec (@hudecof)