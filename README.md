# Ansible Role: Ovirt Guest Agent

[![Build Status](https://travis-ci.org/sbaerlocher/ansible.ovirt-guest-agent.svg?branch=master)](https://travis-ci.org/sbaerlocher/ansible.ovirt-guest-agent) [![license](https://img.shields.io/github/license/mashape/apistatus.svg)](https://sbaerlo.ch/licence) [![Ansible Galaxy](http://img.shields.io/badge/ansible--galaxy-ovirt--guest--agent-blue.svg)](https://galaxy.ansible.com/sbaerlocher/ovirt-guest-agent)
## Description

Ansible role for installing Ovirt Guest Agent on installs RHEL/CentOS.

## Installation

```bash
ansible-galaxy install sbaerlocher.ovirt-guest-agent
```

## Requirements

This role requires Ansible 2 or higher, and platform requirements are listed
in the metadata file.

## Role Variables

| Variable             | Default     | Comments (type)                                   |
| :---                 | :---        | :---                                              |
| ovirt_win_iso_url | <http://resources.ovirt.org/pub/ovirt-4.2/iso/oVirt-toolsSetup/4.2-1.el7.centos/oVirt-toolsSetup-4.2-1.el7.centos.iso> | |
| ovirt_win_iso_name | oVirt-toolsSetup.iso | |

## Dependencies

To install the agent for Windows, the role sbaerlocher.virtio must be installed.

## Example Playbook

```yml
    - hosts: all
      roles:
        - sbaerlocher.ovirt-guest-agent
```

## Changelog

### 1.3

* add windows support

### 1.2

* add new role ckeck
* remove eple repo

### 1.1

* add debian support
* add new syntax
* add tags
* fix bugs

### 1.0

* initial release

## Author

* [Simon Bärlocher](https://sbaerlocher.ch)

## License

MIT