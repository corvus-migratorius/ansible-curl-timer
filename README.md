template
=========

Template for Ansible role monorepos.

⚠️ Do not forget to update:

- `meta/main.yml`
- Conda/Mamba manifests
- this README =)

Requirements
------------

None

Role Variables
--------------

`kuma_port`

`kuma_server_ip`

Dependencies
------------

None

Example Playbook
----------------

```yaml
roles:
    - role: genlab.kuma_curl_timer
      kuma_port: 3001
      kuma_server_ip: xxx.xxx.xxx
```

License
-------

BSD

Author Information
------------------

corvus-migratorius@proton.me
