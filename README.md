# ansible-hosts

[![Ansible Role](https://img.shields.io/ansible/role/ansible-6104.svg)](https://galaxy.ansible.com/detail#/role/6104)
[![Build Status](https://travis-ci.org/shrikeh-ansible-roles/ansible-hosts.svg)](https://travis-ci.org/shrikeh-ansible-roles/ansible-hosts)
[![GitHub Stars](https://img.shields.io/github/stars/shrikeh-ansible-roles/ansible-hosts.svg)](https://github.com/shrikeh-ansible-roles/ansible-hosts)

Add grouped or ungrouped host entries to your hosts file.

## Requirements
------------

None.

## Role Variables
--------------
#### [`hosts_pkg_install_latest`][hosts_pkg_install_latest]
Default: `no`
Controls whether to use 'present' or 'latest' for package installation.

## Dependencies
------------

A list of other roles hosted on Galaxy should go here, plus any details in regards to parameters that may need to be set for other roles, or variables that are used from other roles.

## Example Playbook
----------------

```YAML
---
    - hosts: servers
      roles:
         - { role: shrikeh.hosts }
...
```

## License
-------

[MIT][licence]

## Author Information
------------------
Contact me on Twitter @[barney_hanlon][twitter]

[hosts_pkg_install_latest]: https://github.com/shrikeh-ansible-roles/ansible-hosts/blob/master/defaults/main.yml#L3 "Link to the variable definition in defaults.yml"
[licence]: https://raw.githubusercontent.com/shrikeh-ansible-roles/ansible-hosts/master/LICENSE "Link to the license in the repository"
[twitter]: https://twitter.com/barney_hanlon "Link to my Twitter page"
