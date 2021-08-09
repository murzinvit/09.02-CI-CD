#### 09.02-CI-CD </br>
====================================</br>
#### Работа с SONARQUBE:
SONARQUBE - инструмент тестирования исходного кода, доступен с web интерфейсом на localhost:9000. </br> 
После зупуска sonarcanner в папке с исходником результаты отображаются на localhost:9000 </br>
В fail.py(тестируемый скрипт), в функции - def increment(index), путалось имя локальной и глобальной переменной(index), исправил имя переменной c index на i,</br>
и добавил сложение с глобальной - index</br>
Далее убрал из кода поле - pass, т.к нигде оно не используется. После исправления и прогохода теста, рузультат в web стал - No Issues. Hooray! </br>
Скрипт: [fail.py](https://github.com/murzinvit/09.02-CI-CD/blob/b49874a342957742ba3170c918b91350e7fc5395/fail.py)</br>
</br>
#### Работа с sonatype/nexus3: </br>
sonatype/nexus3 - платформа для хранения и работы с зависимостями для систем сборки - maven, ant, образами Docker и т.п [статья](https://habr.com/ru/post/473358/)</br>
Не понятно почему контейнер с sonatype/nexus3:latest не запускается на Ubuntu 20.04 LTS, 6Gb ОЗУ. Просто падает и логи в nexus-data/logs не пишет.</br>
На Debian 10 + Docker 20.10.6 - работает.</br>
[Maven-metadata.xml](https://github.com/murzinvit/09.02-CI-CD/blob/e1bf567b91e3defa4a93ca47d90cf817b5a05ac3/maven-metadata.xml)</br>
</br>
#### Работа с maven:
В Debian 10 ставиться, но не работает java из apt, удалось поставить только из [openjdk](https://openjdk.java.net/) + export PATH=$PATH:/opt/java/bin</br>
Установка maven: скачать [maven](https://maven.apache.org/download.cgi), распаковать tar xvf, добавть - export PATH=$PATH:/opt/maven/bin</br>
Конфиг mvn: [pom.xml](https://github.com/murzinvit/09.02-CI-CD/blob/a323d6c91127bd7f7e032089fd0a5d229a33380a/pom.xml)</br>
</br>
#### Результат работы sonarscanner:</br>   
![screen](https://github.com/murzinvit/screen/blob/1f99feec1840c70c0dc50f596ffc7e189f1efe75/Hooray_Ho_Issue.jpg) </br>
#### Результат работы maven:</br> 
![screen](https://github.com/murzinvit/screen/blob/bd80d33e9dbd00fb269ebfdf7d32850ec8f04be0/Maven_build.png) </br>


