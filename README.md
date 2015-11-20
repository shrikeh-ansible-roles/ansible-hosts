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
#### [`hosts_file_directory`][hosts_file_directory]
Default: `/etc`
Directory of the hosts file. "Building block" variable, useful in testing.

#### [`hosts_file_name`][hosts_file_name]
Default: `hosts`
Name of the hosts file. "Building block" variable used as component of `hosts_file_path`, useful really only in testing.

#### [`hosts_file_path`][hosts_file_path]
Default: `{{ hosts_file_directory }}/{{ hosts_file_name }}`
Full path to the hosts file. Change this rather than `hosts_file_name` or `hosts_file_directory`.

#### `hosts_file_owner`
Default: `none`
User ownership of `hosts_file_path`. Omitted if unpopulated.

#### `hosts_file_group`
Default: `none`
Group ownership of `hosts_file_path`. Omitted if unpopulated.

#### `hosts_file_group`
Default: `none`
Group ownership of `hosts_file_path`. Omitted if unpopulated.

#### `hosts_file_mode`
Default: `none`
File mode of `hosts_file_path`. Omitted if unpopulated.

## Dependencies
------------

None.

## Example Playbook
----------------

```YAML
---
    - hosts: servers
      vars:
        hosts_file_path: '/etc/foo'
        hosts_file_owner: 'root'
        hosts_file_group: 'devs'
        hosts_entries_local_loopback_ipv4_hostnames:
          - pugh
          - hugh # yes I know it's actually pugh again, but....
          - barney_mcgrew
          - cuthbert
          - dibble
          - grup
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

[hosts_file_directory]: https://github.com/shrikeh-ansible-roles/ansible-hosts/blob/master/defaults/main.yml#L3 "Link to the variable definition in defaults.yml"
[hosts_file_name]: https://github.com/shrikeh-ansible-roles/ansible-hosts/blob/master/defaults/main.yml#L4
[hosts_file_path]: https://github.com/shrikeh-ansible-roles/ansible-hosts/blob/master/defaults/main.yml#L5
[licence]: https://raw.githubusercontent.com/shrikeh-ansible-roles/ansible-hosts/master/LICENSE "Link to the license in the repository"
[twitter]: https://twitter.com/barney_hanlon "Link to my Twitter page"
