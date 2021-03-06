## [![DebOps project](http://debops.org/images/debops-small.png)](http://debops.org) smstools

[![Travis CI](http://img.shields.io/travis/debops/ansible-smstools.svg?style=flat)](http://travis-ci.org/debops/ansible-smstools) [![test-suite](http://img.shields.io/badge/test--suite-ansible--smstools-blue.svg?style=flat)](https://github.com/debops/test-suite/tree/master/ansible-smstools/)  [![Ansible Galaxy](http://img.shields.io/badge/galaxy-debops.smstools-660198.svg?style=flat)](https://galaxy.ansible.com/list#/roles/1601)

This is an Ansible role which configures
[smstools](http://smstools3.kekekasvi.com/) package and sets up a TCP -> SMS
and mail -> SMS gateway. This role has been tested on Debian and should
work on Debian-based systems.

Several other roles from [DebOps](http://debops.org/) project are used to
configure various parts of the SMS gateway (`debops.postfix` role is used
to create mail -> SMS gateway, `debops.etc_services`, `debops.ferm` and
`debops.tcpwrappers` are used to configure TCP service which can be used
by other hosts to send SMS messages over the network).

### Installation

This role requires at least Ansible `v1.7.0`. To install it, run:

    ansible-galaxy install debops.smstools

### Documentation

More information about `debops.smstools` can be found in the
[official debops.smstools documentation](http://docs.debops.org/en/latest/ansible/roles/debops.smstools.html).


### Role dependencies

- `debops.ferm`
- `debops.etc_services`
- `debops.postfix`
- `debops.tcpwrappers`
- `debops.rsyslog`

### Are you using this as a standalone role without DebOps?

You may need to include missing roles from the [DebOps common
playbook](https://github.com/debops/debops-playbooks/blob/master/playbooks/common.yml)
into your playbook.

[Try DebOps now](https://github.com/debops/debops) for a complete solution to run your Debian-based infrastructure.





### Authors and license

`smstools` role was written by:
- Maciej Delmanowski | [e-mail](mailto:drybjed@gmail.com) | [Twitter](https://twitter.com/drybjed) | [GitHub](https://github.com/drybjed)

License: [GPLv3](https://tldrlegal.com/license/gnu-general-public-license-v3-%28gpl-3%29)

***

This role is part of the [DebOps](http://debops.org/) project. README generated by [ansigenome](https://github.com/nickjj/ansigenome/).
