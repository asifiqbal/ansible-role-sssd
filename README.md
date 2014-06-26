marklee77.sssd
==============


Requirements
------------

LDAP server supporting ssl/tls.

Role Variables
--------------

- ldap_uri: ldap://127.0.0.1/

- sssd_password: password
- sssd_password_hash: "{SSHA}eJNTYUqAuakTkuNFr04V1Y0Sh88PPBIn"

- sssd_enable_mkhomedir: true

Example Playbook
-------------------------

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

http://stillwell.me/

