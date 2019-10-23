netbox
======

Setup NetBox on Debian.

Role Variables
--------------

```yaml
netbox_version: NETBOX_VERSION
netbox_db_name: DB_NAME
netbox_db_user: DB_USER
netbox_db_password: DB_PASSWORD
```

Dependencies
------------

- pylabs.python3
- pylabs.nginx

Example Playbook
----------------

```yaml
- hosts: servers
  roles:
    - pylabs.netbox
  vars:
    netbox_version: "2.6.6"
    netbox_db_name: netbox
    netbox_db_user: netbox
    netbox_db_password: netboxpa$$
```

License
-------

MIT

Author Information
------------------

William Wu <william@pylabs.org>
