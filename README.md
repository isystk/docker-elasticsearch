🌙 docker-elasticsearch
====

![GitHub issues](https://img.shields.io/github/issues/isystk/docker-elasticsearch)
![GitHub forks](https://img.shields.io/github/forks/isystk/docker-elasticsearch)
![GitHub stars](https://img.shields.io/github/stars/isystk/docker-elasticsearch)
![GitHub license](https://img.shields.io/github/license/isystk/docker-elasticsearch)

## 📗 プロジェクトの概要

ElasticSearch のサンプルです。Dockerを起動するとElasticSearch を利用する為の環境が整います。

## 🌐 Demo

![Kibana](./kibana.png "Kibana")


## 🔧 開発環境の構築

```
# Docker起動時にエラーが発生する場合は仮想メモリを増やす設定をする
sysctl -w vm.max_map_count=262144
```



## 💬 使い方

```
# Docker でSwaggerを起動します。
$ docker-compose up -d

# サンプルデータを投稿する
$ unzip accounts.zip
$ curl -H 'Content-Type: application/x-ndjson' -XPOST 'http://localhost:9200/bank/account/_bulk?pretty' --data-binary @accounts.json

# データを確認する
$ curl -XGET 'http://localhost:9200/_cat/indices?v'
health status index    uuid                   pri rep docs.count docs.deleted store.size pri.store.size
yellow open   bank     wxooemXLSJqIraatTDJM6Q   1   1       1000            0    414.2kb        414.2kb

# Docker を停止します。
$ docker-compose down
```

# Kibana 
http://localhost:5601/




## 🎨 参考

| プロジェクト| 概要|
| :---------------------------------------| :-------------------------------|
| [Elasticsearch 超入門](https://qiita.com/bbbks9/items/7695262be0befb94897f)| Elasticsearch 超入門|
| [Elasticserachをlocalhost以外で起動する方法](https://qiita.com/TomatoCastle/items/12474753aa8b002db9ca)| Elasticserachをlocalhost以外で起動する方法|


## 🎫 Licence

[MIT](https://github.com/isystk/docker-elasticsearch/blob/master/LICENSE)

## 👀 Author

[isystk](https://github.com/isystk)

