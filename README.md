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
#### [`hosts_file_path`][hosts_file_path]
Default: `/etc/hosts`
The path to the host file to update.

#### [`hosts_file_owner`][hosts_file_group]
Default: `root`
User ownership of `hosts_file_path`.

#### [`hosts_file_group`][hosts_file_group]
Default: `root`
Group ownership of `hosts_file_path`.

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

[hosts_file_path]: https://github.com/shrikeh-ansible-roles/ansible-hosts/blob/master/defaults/main.yml#L3 "Link to the variable definition in defaults.yml"
[hosts_file_owner]: https://github.com/shrikeh-ansible-roles/ansible-hosts/blob/master/defaults/main.yml#L4
[hosts_file_group]: https://github.com/shrikeh-ansible-roles/ansible-hosts/blob/master/defaults/main.yml#L5
[licence]: https://raw.githubusercontent.com/shrikeh-ansible-roles/ansible-hosts/master/LICENSE "Link to the license in the repository"
[twitter]: https://twitter.com/barney_hanlon "Link to my Twitter page"
