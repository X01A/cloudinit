Cloudinit
=========

Installs cloud-init

Role Variables
--------------

* `cloud_cfg` can optionally be supplied, this template file overrides the default role
centos.cfg and ubuntu.cfg files.

Example Playbook
----------------

    - hosts: all
      roles:
        - cloudinit
      post_tasks:
        - reboot: # Recommend way to run cloud-init
