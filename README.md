Disk readahead settings
=========

This role can be used to set up modified readahead settings for
(virtual machine) block devices.

[![Build Status](https://github.com/Rheinwerk/ansible-role-readahead_setup/actions/workflows/ci.yml/badge.svg)](https://github.com/Rheinwerk/ansible-role-readahead_setup/actions/workflows/ci.yml)

Requirements
------------

None.

Role Variables
--------------

There is one main variable that drives this role: `_readahead_setup`. It is a map that contains all configuration and settings for this role.
Please see `defaults/main.yml` for details.

Dependencies
------------

None.


Example Playbook
----------------

The general contract of this role is to take the variables map `_readahead_setup` from `defaults/main.yml` as a template for your configuration and pass that configuration as a parameter to this role.

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers
      var:
        readahead_setup:
          ...
      roles:
         - { role: readahead_setup, tags: [ 'readahead_setup' ], _readahead_setup: "{{ readahead_setup }}" }

License
-------

Please see LICENSE.

Author Information
------------------

Original author is [Daniel Schneller](https://github.com/dschneller) as member of the [Rheinwerk](https://github.com/Rheinwerk) project.

