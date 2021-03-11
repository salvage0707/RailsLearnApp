# README

This README would normally document whatever steps are necessary to get the
application up and running.

Things you may want to cover:

* Ruby version

* System dependencies

* Configuration

* Database creation

* Database initialization

* How to run the test suite

* Services (job queues, cache servers, search engines, etc.)

* Deployment instructions

* ...

## postgresql
### 起動
```sh
$ pg_ctl start -D /usr/local/var/postgresql@12
```

### 接続
```sh
$ psql -d postgres
```

### ユーザー
```sh
$ # create user taskleaf;
$ # \password tasklaf
  Enter new password: password
  Enter it again: password
```


権限設定をした。
参考：http://php.o0o0.jp/article/postgres-role
`ALTER ROLE taskleaf CREATEDB;` // データベース作成権限
