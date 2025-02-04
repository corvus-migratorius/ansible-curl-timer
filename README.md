curl-scheduled
=========

Configure curl to run on schedule by deploying a systemd service + timer. Useful for sending heartbeats.

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

Because the role uses host-specific `kuma_token` variable, it have to be defined in inventory.yml file. For example:

```yaml
testtest:
  hosts:
    test-node:
      ansible_host: xxx.xxx.xxx.xxx
      ansible_user: ubuntu
      kuma_token: "testtesttesttesttest1"
    test-node2:
      ansible_host: xxx.xxx.xxx.xxx
      ansible_user: ubuntu
      kuma_token: "testtesttesttesttest2"
```

License
-------

BSD

Author Information
------------------

corvus-migratorius@proton.me
