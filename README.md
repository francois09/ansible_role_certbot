CERTBOT Ansible role
========================

Role to manage CERTBOT.

For the moment, this role use already running HTTP server, and you must have write access to the root directory.
It uses the `--webroot` and `-w <DIR>` options.

Requirements
------------

Read/Write access to `certbot__config.rootdir` where certbot places `.well-known` challenge/response directory.

Role Variables
--------------

* `certbot__install` For install only (default: False)
* `certbot__configure` For configuration  (default: False)
* `certbot__config.alert_email` email address used by let's encrypt for alerts about renewing
* `certbot__config.domain` Certificate domain name
* `certbot__config.rootdir` Location of challenge/response files

Dependencies
------------

None

Example Playbooks
-----------------

License
-------

GPL v3

Author Information
------------------

François TOURDE
