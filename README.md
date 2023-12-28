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

### `opendkim_selector`

DKIMセレクター

### `opendkim_domains`

設定するドメイン

### `opendkim_rsa_keylen`

opendkim-gkeygenで鍵を生成する時のキー長

### `opendkim_mta`

連携させるMTA

### `opendkim_run_dir`

OpenDKIMの動作ディレクトリ

### `opendkim_cfg`

OpenDKIMの設定

### `opendkim_trusted_hosts`

接続を許可するホストの設定  
※1つ以上設定されている場合はInternalHosts/ExternalIgnoreListの設定を設定ファイルに自動で追加します

### `opendkim_postfix_cfg`

Postfixの連携設定

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
