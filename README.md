HZLF Base sytem role
====================

A minimal Ansible role that configures our servers...


Requirements
------------

 - Debian 8.x
   + Debian < 8.x: We don't have any reasons to support older versions. Most things actually should work fine, but `wheezy`does not include `nodejs`/`npm`
   + ubuntu: Should/could work as well, but has never been tested.

Role Variables
--------------

- `system_base_rsyslog_server`: rsyslog server to use, defasults to `no`



Example Playbook
----------------

Minimal usage example:

    - hosts: all
      roles:
        - {
            role: hzlf.system-base,
            system_base_rsyslog_server: "my.local.proxy.example.com",
          }


License
-------

BSD
