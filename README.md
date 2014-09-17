marklee77.sssd
==============

[![Build Status](https://travis-ci.org/marklee77/ansible-role-sssd.svg?branch=master)](https://travis-ci.org/marklee77/ansible-role-sssd)

Ansible role to install sssd auth.

Requirements
------------

LDAP server supporting ssl/tls.

Role Variables
--------------

- sssd_tls_cipher_suite: SECURE256:!AES-128-CBC:!ARCFOUR-128:!CAMELLIA-128-CBC:!3DES-CBC:!CAMELLIA-128-CBC
- sssd_verify_cert: true

- sssd_enable_modify_hosts: false
- sssd_enable_mkhomedir: true

Example Playbook
----------------

    - hosts: all
      sudo: True
      roles:
        - marklee77.slapd-auth
        - marklee77.sssd

License
-------

GPLv2

Author Information
------------------

http://stillwell.me

