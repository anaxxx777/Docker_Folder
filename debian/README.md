#### Debianコンテナ
- コンテナを起動させたいのに、すぐに終了してしまう場合はyamlファイルに記述する
※コンテナはフォアグラウンドで実行されるプロセスが無いと起動後すぐに終了する
```
tty: true
```