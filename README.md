Ansible Role: MariaDB(pkg)
================================================================================
Install and configure MariaDB

- Install MariaDB 5.* using yum at CentOS 7
- Configure /etc/my.cnf
- Close tcp/3306

Requirements
--------------------------------------------------------------------------------
None

Role Variables
--------------------------------------------------------------------------------
The following variables are defined in defaults/main.yml file.

```yaml
mariadb:
  enabled: true
  started: true
  serverroot: "/var/lib/mysql"
  configroot: "/etc"
  workingdir: "/usr/local/src"
```

Dependencies
--------------------------------------------------------------------------------
None

Example Playbook
--------------------------------------------------------------------------------
```yaml
- hosts: servers
  roles:
     - { role: azumakuniyuki.ar-mariadb-pkg }
```

License
--------------------------------------------------------------------------------
BSD

Author Information
--------------------------------------------------------------------------------
[azumakuniyuki](http://nyaan.jp)

