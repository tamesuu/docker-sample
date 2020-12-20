# まだ途中

```
$ docker-compose build
$ docker-compose up -d
```

TODO: これを起動スクリプトに組み込む

master

```
CREATE USER 'repl'@'%';
GRANT REPLICATION SLAVE ON *.* TO 'repl'@'%';
```

slave

```
CHANGE MASTER TO MASTER_HOST='db-master', MASTER_USER='repl', MASTER_LOG_FILE='hogehoge', MASTER_LOG_POS=xxx;
START SLAVE;
```

master

```
CREATE DATABASE sample;
```
