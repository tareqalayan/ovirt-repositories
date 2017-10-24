
oVirt Repositories
==================

The `ovirt-repositories` role is used to set the repositories required for oVirt engine installation.
Currently it works only when you provide the release RPM.

Requirements
------------

 * oVirt Python SDK version 4
 * Ansible version 2.4

Role Variables
--------------

| Name                  | Default value         |  Description                              |
|-----------------------|-----------------------|-------------------------------------------|
| ovirt_rpm_repo        | UNDEF                 | URL of RPM package with repository files. |


Dependencies
------------

No.

Example Playbook
----------------

```yaml
---
- name:  install RPM with repository files
  hosts: localhost

  vars:
    ovirt_rpm_repo: http://resources.ovirt.org/pub/yum-repo/ovirt-master-release.rpm

  roles:
    - role: ovirt-common
```

License
-------

Apache License 2.0
