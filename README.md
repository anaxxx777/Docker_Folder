#### 起動の方法
```
docker compose up -d
```
- yamlファイルがある階層で実行
- composeの時はrunではなく<font color="red">「up」</font>
<br>
#### MariaDB
| 環境変数              | 意味                       | 
| --------------------- | -------------------------- | 
| MARIADB_ROOT_PASSWORD | ルートユーザーのパスワード | 
| MARIADB_DATABASE      | データベース名             | 
| MARIADB_USER          | データベースのユーザー名   | 
| MARIADB_PASSWORD      | データベースのパスワード   | 
[DockerHub:mariadb](https://hub.docker.com/_/mariadb)
<br>
※言語別でコードも書ける
↓↓指定あり
```java
int num = 10;
```
↓↓指定なし
```
int num = 10;
```