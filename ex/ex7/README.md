####コンテナ作成
```
docker container run --name my_tomcat -p 8088:8080 -d tomcat
```
####コンテナに入る(yamlなしのコンテナ)
```
docker exec -it my_tomcat bash
```
####tomcat内のwebappsフォルダに空のフォルダを作成(tomcatはwebapps内のフォルダを読み取ってwebページを出力するらしい)
```
cd webapps
mkdir hello
```
####ubuntu内にhtmlをscp送信してをそれをtomcatにコピーする
```
docker cp ~/hello.html my_tomcat:/usr/local/tomcat/webapps/hello
// ~直下にあるファイル
```
<br>
####アクセス例
http://3.86.191.5:8088/hello/hello.html
<br>
####composeなしコンテナ削除
```
docker rm -f my_tomcat
```