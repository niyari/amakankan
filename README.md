# amakankan [![Build Status](https://travis-ci.org/amakan/amakankan.svg?branch=master)](https://travis-ci.org/amakan/amakankan)

amakankanは、[amakan.net](https://amakan.net) のための公式ブラウザ拡張です。

## インストール

### Google Chrome

~~[amakankan - Chromeウェブストア](https://chrome.google.com/webstore/detail/amakankan/cbbcooiceghdbkklnkdahccnbbfleoll)~~ 登録取消のため再申請中

### Firefox, Opera, Edge

登録申請中 :bow:

## 使い方

### Amazonの注文履歴からインポート

Amazonの [注文履歴ページ](https://www.amazon.co.jp/gp/css/order-history) でボタンを押すと、読んだ本をamakanに一括登録できます。

![demo](/images/demo.gif)

### Amazonの商品ページからamakanに移動

Amazonの商品ページでボタンを押すと、amakanの対応する書籍のページを開きます。

### ブクログの本棚からインポート

[ブクログ](http://booklog.jp/) の本棚ページでボタンを押すと、読んだ本をamakanに一括登録できます。

### 読書メーターの読んだ本からインポート

[読書メーター](http://bookmeter.com/) の読んだ本のページでボタンを押すと、読んだ本をamakanに一括登録できます。

### TSUTAYA LOG の履歴ストックからインポート

[TSUTAYA LOG](https://log.tsutaya.co.jp/) の履歴ストックページでボタンを押すと、読んだ本をamakanに一括登録できます。

### amakanに移動

上記以外のページでボタンを押すと、[amakan.net](https://amakan.net) を開きます。

## 開発者用ドキュメント

### 準備

このリポジトリは、Dockerを利用して開発することを想定しています。
手元の環境でDockerを動かせるように準備を行ってください。

https://docs.docker.com/

### watch

ファイルの変更を監視して継続的にビルドを行うには、以下のスクリプトを実行してください。

```bash
docker-compose up
```

### build

1度だけビルドを行うには、以下のスクリプトを実行してください。

```bash
docker-compose run --rm node yarn run build
```

### pack

拡張用のファイルを生成するには、以下のスクリプトを実行してください。

```bash
docker-compose run --rm node yarn run pack
```
