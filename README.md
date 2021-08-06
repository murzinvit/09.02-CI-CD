#### 09.02-CI-CD </br>
====================================</br>
#### Работа с SONARQUBE:
В fail.py, в def increment(index):, путалось имя локальной и глобальной переменной, исправил имя переменной и добавил сложение с глобальной.</br>
Далее убрал - pass, т.к нигде не используется. После исправления стало - No Issues. Hooray! </br>
Скрипт: [fail.py](https://github.com/murzinvit/09.02-CI-CD/blob/b49874a342957742ba3170c918b91350e7fc5395/fail.py)</br>
</br>
#### Работа с sonatype/nexus3: </br>
Не понятно почему контейнер с sonatype/nexus3:latest не запускается на Ubuntu 20.04 LTS, 6Gb ОЗУ. Просто падает и логи в nexus-data/logs не пишет.</br>
На Debian 10 + Docker 20.10.6 - работает.</br>
[Maven-metadata.xml](https://github.com/murzinvit/09.02-CI-CD/blob/e1bf567b91e3defa4a93ca47d90cf817b5a05ac3/maven-metadata.xml)</br>
</br>
#### Работа с maven:
В Debian 10 ставиться, но не работает java из apt, удалось поставить только из [openjdk](https://openjdk.java.net/) + export PATH=$PATH:/opt/java/bin</br>
Конфиг mvn: [pom.xml](https://github.com/murzinvit/09.02-CI-CD/blob/a323d6c91127bd7f7e032089fd0a5d229a33380a/pom.xml)</br>
</br>
#### Результат работы sonarscanner:</br>   
![screen](https://github.com/murzinvit/screen/blob/1f99feec1840c70c0dc50f596ffc7e189f1efe75/Hooray_Ho_Issue.jpg) </br>
#### Результат работы maven:</br> 
![screen](https://github.com/murzinvit/screen/blob/bd80d33e9dbd00fb269ebfdf7d32850ec8f04be0/Maven_build.png) </br>


