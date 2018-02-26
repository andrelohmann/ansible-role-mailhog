mailhog
=======

[![Build Status](https://travis-ci.org/andrelohmann/ansible-role-mailhog.svg?branch=master)](https://travis-ci.org/andrelohmann/ansible-role-mailhog)

Use this role to install mailhog and run it as a deamon in the backgroud using systemd.

Requirements
------------

This role requires ubuntu.

Role Variables
--------------

The default set of variables defines the the settings, mailhog will be started with

    mailhog_smtp_port: 1025
    mailhog_web_port: 8025
    mailhog_path: /opt/mailhog
    mailhog_release: v1.0.0

Example Playbook
----------------

    - hosts: mailhog
      roles:
         - { role: andrelohmann.mailhog }

License
-------

MIT

Author Information
------------------

https://github.com/andrelohmann
