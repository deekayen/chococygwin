jefg60.chococygwin
=========

Uses chocolatey package manager to install cygwin on windows and manage which parts of cygwin are installed.

Requirements
------------

Role Variables
--------------

optional variables:
    cyg_get_packages: list of packages to install inside cygwin
    cyg_upgrade: set to true if you want to automatically upgrade all cygwin packages

Dependencies
------------

Example Playbook
----------------

    - hosts: windows
      roles:
         - { role: jefg60.chococygwin, cyg_get_packages: ["rsync", "vim"], cyg_upgrade: true }

License
-------

GPLv3

Author Information
------------------

jeff@jeffhibberd.com
