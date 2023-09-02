mailhog
=======

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
    mailhog_release: v1.0.1

By setting the following additional variables, you can proxy mailhog behind apache

    mailhog_proxy_apache: true
    mailhog_proxy_domain: _your.mailghog.domain_
    mailhog_proxy_port: 80

or nginx

    mailhog_proxy_nginx: true
    mailhog_proxy_domain: _your.mailghog.domain_
    mailhog_proxy_port: 80    

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
