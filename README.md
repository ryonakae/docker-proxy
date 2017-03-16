# brdr-proxy
Reverse proxy server for brdr.jp

## ネットワーク作成
リバースプロキシとサービスのWebサーバ(Apache, Nginx)とを繋ぐためのネットワークを作成
サービス内の各コンテナは別のネットワークで繋ぐ

```
$ docker network create --driver bridge front
```