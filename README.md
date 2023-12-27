opendkim
=================

Setup OpenDKIM

OS Platform
-----------------

### Debian

- bookworm
- bullseye

Role Variables
--------------

設定方法の詳細については[defaults/main.yml](defaults/main.yml)のサンプルコードを参照してください。

### `opendkim_packages`

インストールするパッケージ

### `opedkim_domains`

設定するドメイン

Example Playbook
--------------

```yaml
- hosts: servers
  roles:
    - role: opendkim
```

License
--------------

Apache License 2.0
