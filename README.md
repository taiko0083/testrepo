# DockerでSpring bootを動かす手順
【参考】https://qiita.com/A-Kira/items/beaf79a0d39d9839e61e
1. Docker_testをcloneまたはダウンロードする
2. コマンドプロンプトで以下を実行
```
C:\> cd Docker_test
C:\Docker_test> docker-compose build
C:\Docker_test> docker-compose up -d
C:\Docker_test> docker-compose exec java bash

root@48eae2d25f8b:~# cd /srv/api/
root@48eae2d25f8b:/srv/api# sh gradlew build
root@48eae2d25f8b:/srv/api# cd /srv/
root@48eae2d25f8b:/srv# java -jar build/libs/api-0.0.1-SNAPSHOT.jar
```
3. http://localhost:8080/　にアクセスする→Hello Worldが表示される