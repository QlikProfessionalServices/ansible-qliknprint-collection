Ansible Role: Qlik NPrinting setup
=========

An Ansible Role that installs Qlik NPrinting server and engine.

Requirements
------------

None.

Role Variables
--------------

```yaml
server_setup_path: '{{ ansible_env.HOME }}\Downloads\QlikNPrintingServer_x64.exe'
engine_setup_path: '{{ ansible_env.HOME }}\Downloads\QlikNPrintingEngine_x64.exe'
service_username: np-service
service_password: Qlik1234
admin_email: npadmin@domain.tld
admin_username: npadmin
admin_password: Qlik1234
database_password: Qlik1234
engine_certs_password: Qlik1234
server_hostname: "{{ ansible_host }}"
```

Dependencies
------------

None.

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

- hosts: nprint_servers
  roles:
    - role: qlik.nprinting.setup
      server_setup_path: '{{ ansible_env.HOME }}\Downloads\QlikNPrintingServer_x64.exe'
      engine_setup_path: '{{ ansible_env.HOME }}\Downloads\QlikNPrintingEngine_x64.exe'
      service_username: np-service
      service_password: Qlik1234
      admin_email: npadmin@domain.tld
      admin_username: npadmin
      admin_password: Qlik1234
      database_password: Qlik1234
      engine_certs_password: Qlik1234
      server_hostname: "{{ ansible_host }}"

License
-------

MIT

Author Information
------------------

This role was created by [Adam Haydon](https://github.com/ahaydon) of [Qlik Customer Success](https://github.com/QlikProfessionalServices)
