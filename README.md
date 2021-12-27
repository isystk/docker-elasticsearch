🌙 docker-elasticsearch
====

![GitHub issues](https://img.shields.io/github/issues/isystk/docker-elasticsearch)
![GitHub forks](https://img.shields.io/github/forks/isystk/docker-elasticsearch)
![GitHub stars](https://img.shields.io/github/stars/isystk/docker-elasticsearch)
![GitHub license](https://img.shields.io/github/license/isystk/docker-elasticsearch)

## 📗 プロジェクトの概要

ElasticSearch のサンプルです。Dockerを起動するとElasticSearch を利用する為の環境が整います。

## 🌐 Demo

![Swagger](./swagger.png "Swagger")


## 🔧 開発環境の構築

```
# Docker起動時にエラーが発生する場合は仮想メモリを増やす設定をする
sysctl -w vm.max_map_count=262144
```



## 💬 使い方

```
# Docker でSwaggerを起動します。
$ docker-compose up -d

# Docker を停止します。
$ docker-compose down
```

http://localhost:9200




## 🎨 参考

| プロジェクト| 概要|
| :---------------------------------------| :-------------------------------|
| [Elasticsearch 超入門](https://qiita.com/bbbks9/items/7695262be0befb94897f)| Elasticsearch 超入門|
| [Elasticserachをlocalhost以外で起動する方法](https://qiita.com/TomatoCastle/items/12474753aa8b002db9ca)| Elasticserachをlocalhost以外で起動する方法|


## 🎫 Licence

[MIT](https://github.com/isystk/docker-elasticsearch/blob/master/LICENSE)

## 👀 Author

[isystk](https://github.com/isystk)

