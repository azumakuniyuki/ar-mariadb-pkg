Ansible Role: Apache(pkg)
================================================================================
Install and configure Apache as an HTTP Server

- Install Apache 2.4.* using yum at CentOS 7
- Configure files in /etc/httpd
- Open tcp/80 and tcp/443

Requirements
--------------------------------------------------------------------------------
None

Role Variables
--------------------------------------------------------------------------------
The following variables are defined in defaults/main.yml file.

```yaml
apache:
  enabled: true
  started: true
  configroot: "/etc/httpd"
  serverroot: "/usr"
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
     - { role: azumakuniyuki.ar-apache-pkg }
```

License
--------------------------------------------------------------------------------
BSD

Author Information
--------------------------------------------------------------------------------
[azumakuniyuki](http://nyaan.jp)

