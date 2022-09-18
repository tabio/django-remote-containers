### 概要

VSCodeのRemote Containersを試すためのサンプルリポジトリ

### 使い方

vscodeを起動して、コマンドパレットから`Remote-Containers: Reopen`を実行するだけ
.devcontainer配下のdevcontainer.jsonの指示に従って開発環境用のDockerをビルドしてくれる
そのDocker内にVScodeもインストールしてくれる仕組みになっている
Docker内の修正はホスト側に反映されるように設定している
ホストのマシンを汚さないで済むことや複数のメンバーでの開発環境に差がでないことが利点

### Django

dockerを立ち上げただけではDjangoは起動してないので手動で起動させる必要がある

```sh
python manage.py runserver
```