apt-http-proxy
=========

Very minimalistic role to manage apt HTTP-proxy


Role Variables
--------------

Variable | Function
--- | ---
apt_http_proxy | URL of Proxy Server
apt_http_proxy_direct | List of Servers without proxy


Dependencies
------------

None


Example Playbook
----------------

```yaml
- hosts: servers
  vars:
    apt_http_proxy: "http://10.10.10.10:3128"
    apt_http_proxy_direct:
      - deb.example.com
  roles:
    - clutterbox.apt-http-proxy
```

License
-------

MIT Licsense

Author Information
------------------

Alexander Zielke - mail@alexander.zielke.name
