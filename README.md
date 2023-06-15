# Docker Compose
#### 起動の方法
```
docker compose up -d
```
- コンテナの作成と実行を行う
- yamlファイルがある階層で実行
- composeの時はrunではなく<font color="red">「up」</font>
#### コンテナ確認
```
<!-- 実行中のコンテナを一覧表示 -->
docker container ls
<!-- すべてのコンテナを一覧表示 -->
docker container ls -a
```
#### プロジェクト一覧表示
```
docker compose ls
```
#### コンテナの起動・停止
```
docker compose start
docker compose stop
```
#### コンテナのコピー
```
<!-- コンテナへファイルをコピー -->
docker compose cp ホストのファイルパス コンテナ名:コンテナ内のファイルパス
<!-- Dockerホストへファイルをコピー -->
docker compose cp コンテナ名:コンテナ内のファイルパス ホストのファイルパス
<!-- 例:DockerからPCへコピー -->
docker compose cp web:/usr/local/apache2/htdocs/index.html .
```
#### コンテナの削除
```
<!-- コンテナとネットワークを一度に削除 -->
docker compose down
<!-- イメージ削除 -->
docker compose down --rmi all
<!-- イメージの一覧表示 -->
docker image ls
<!-- 「volume」に記載されたボリュームと匿名ボリュームを削除 -->
docker compose down -v
```
#### コンテナ内でコマンド実行
```
docker compose exec コンテナ名 コンテナで実行したいコマンド
```
#### コンテナ内でシェルの立ち上げ
```
docker compose exec コンテナ名 /bin/bash
```
<br>
#### README機能
※言語別でコードも書ける
↓↓指定あり
```java
int num = 10;
```
↓↓指定なし
```
int num = 10;
```