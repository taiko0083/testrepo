# Docker��Spring boot�𓮂����菇
�y�Q�l�zhttps://qiita.com/A-Kira/items/beaf79a0d39d9839e61e
1. Docker_test��clone�܂��̓_�E�����[�h����
2. �R�}���h�v�����v�g�ňȉ������s
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
3. http://localhost:8080/�@�ɃA�N�Z�X���遨Hello World���\�������