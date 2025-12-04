Ansible Role: Qlik NPrinting download
=========

An Ansible Role that downloads Qlik NPrinting setup files from GitHub.

Requirements
------------

None.

Role Variables
--------------

```yaml
release_name: February 2025 SR3
download_path: "{{ lookup('ansible.builtin.env', 'HOME') }}/Downloads"
server_setup_path: "{{ download_path }}/{{ release_name }}/QlikNPrintingServer_x64.exe"
engine_setup_path: "{{ download_path }}/{{ release_name }}/QlikNPrintingEngine_x64.exe"
```

Dependencies
------------

None.

Example Playbook
----------------

```yaml
- hosts: servers
  roles:
    - role: qlik.nprinting.download
      release_name: February 2025 SR3
```

License
-------

MIT

Author Information
------------------

This role was created by [Adam Haydon](https://github.com/ahaydon) of [Qlik Customer Success](https://github.com/QlikProfessionalServices)