#### 09.02-CI-CD </br>
====================================</br>
В fail.py, в def increment(index):, путалось имя локальной и глобальной переменной, исправил имя переменной и добавил сложение с глобальной.</br>
Далее убрал - pass, т.к нигде не используется. После исправления стало - No Issues. Hooray! </br>
Скрипт: [fail.py](https://github.com/murzinvit/09.02-CI-CD/blob/e1bf567b91e3defa4a93ca47d90cf817b5a05ac3/maven-metadata.xml)</br>
##### sonatype/nexus3:
Не понятно почему контейнер с sonatype/nexus3:latest не запускается на Ubuntu 20.04 LTS, 6Gb ОЗУ. Просто падает и логи в nexus-data/logs не пишет.</br>
На Debian 10 + Docker 20.10.6 - работает.</br>
### Maven-metadata.xml </br>
[Maven-metadata.xml](https://github.com/murzinvit/09.02-CI-CD/blob/e1bf567b91e3defa4a93ca47d90cf817b5a05ac3/maven-metadata.xml)</br>
## sonarscanner result:   
![screen](https://github.com/murzinvit/screen/blob/1f99feec1840c70c0dc50f596ffc7e189f1efe75/Hooray_Ho_Issue.jpg) </br>

