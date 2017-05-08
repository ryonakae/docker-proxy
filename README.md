# docker-proxy
Reverse proxy server by Docker

## ネットワーク作成
リバースプロキシとサービスのWebサーバ(Apache, Nginx)とを繋ぐためのネットワークを作成
サービス内の各コンテナは別のネットワークで繋ぐ

```
$ docker network create --driver bridge front
```