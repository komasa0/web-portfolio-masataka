# web-portfolio-masataka
このプロジェクトは、ポートフォリオのソースコードです。

##　コンテナの起動

起動する際には以下のコマンドを実施します。
プロジェクトルートでのコマンドの実行の必要があります。

```sh
#start
$ docker run -dit --rm --name portfolio1 -v "$PWD/public":/usr/local/apache2/htdocs/ -p 3000:80 httpd:2.4-alpine
```

##　アクセス

コンテナ起動中は以下のURLにアクセス可能です。

<http://localhost:3000/>

## コンテナ終了

制作終了時に以下のコマンドでコンテナを終了します。

```sh
$ docker stop portfolio1
```