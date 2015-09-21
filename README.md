MariaDB Galera Clusterを試す
============================

MariaDB Galera Clusterを試すためのVagrantfile一式

## Description

MariaDB Galera Clusterを使ったシステム構成を試すためのVagrantfile一式です。  
このVagrantfileではWeb(確認用)用VM1台、DB用VM3台の構成です。

## Requirement

- Vagrant
    - plugins
        - vagrant-hostmanager
- VirtualBox
- Ansible
- Memory > 4GB

## Usage

```bash
$ vagrant up
```

### web

```bash
$ vagrant ssh web
$ mysql
or
$ mysql -h 127.0.0.1 -P 3306 -u client
```

### db[1-3]

```bash
$ vagrant ssh db[1-3]
```

## Licence

[MIT](./LICENSE)

## Author

[n.matayoshi](https://github.com/matayoshi)
