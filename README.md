[![Build Status](https://travis-ci.org/AdrianGPrado/ansible-role-etc-hosts.svg?branch=master)](https://travis-ci.org/AdrianGPrado/ansible-role-etc-hosts)

Role Name
=========

When working with `Ansible` and `Vagrant` together, this role will write,

    vm_ip   vm_hostname

inside `/etc/hosts`.

Requirements
------------

If you are using `CoreOS` or `Fedora >= 22`, please make sure that the OS has _python 2.4_ installed. You can use the role:

    $ ansible-galaxy install AdrianGPrado.os-info

or

    $ ansible-galaxy install AdrianGPrado.coreos-bootstrap

Role Variables
--------------

None.

Dependencies
------------

None.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: all
      become: yes
      vars:
        - public_iface: "{{ ansible_default_ipv4.interface }}"
      roles:
        - hosts-file

License
-------

BSD, MIT
