Ansible Role: Qlik NPrinting settings
=========

An Ansible role that configures Qlik NPrinting server settings.

Requirements
------------

None.

Role Variables
--------------

```yaml
settings_validate_certs: true
settings_hostname: "{{ ansible_host }}"
settings_license_key: AAAnfwebnfl...
```

Dependencies
------------

None.

Example Playbook
----------------

```yaml
- hosts: nprint_servers
  roles:
    - role: qlik.nprinting.settings
      settings_validate_certs: false
      settings_hostname: nprint.domain.tld
      settings_license_key: AAAnfwebnfl...
```

License
-------

MIT

Author Information
------------------

This role was created by [Adam Haydon](https://github.com/ahaydon) of [Qlik Customer Success](https://github.com/QlikProfessionalServices)
