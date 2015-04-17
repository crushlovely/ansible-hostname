# Ansible Role to edit server hostname

[![Current Version](https://circleci.com/gh/crushlovely/ansible-hostname.png?circle-token=ef759a78c1d03411214d35ca2a958962f7fdce0c)](https://circleci.com/gh/crushlovely/ansible-hostname)
[![Current Version](http://img.shields.io/github/release/crushlovely/ansible-hostname.svg?style=flat)](https://galaxy.ansible.com/list#/users/3804)

This Ansible role installs AWS EC2 API tools and edits the server hostname.  It will grep the EC2 API for the server `tag_Name` and use that as the server hostname.  This role assumes that you have provisioned your severs with a tag name.

## Installation

``` bash
$ ansible-galaxy install https://github.com/crushlovely/ansible-hostname.git, v1.0.0
```

## Variables

  ``` yaml
aws:
  access_key: 1234567890
  secret_key: 1234567890

  ```

## Usage

Once this role is installed on your system, include it in the roles list of your playbook.

``` yaml
- hosts: localhost
  roles:
    - ansible-hostname
```

## Dependencies

None

## License

MIT