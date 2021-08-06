#### 09.02-CI-CD </br>
====================================</br>
В fail.py, в def increment(index):, путалось имя локальной и глобальной переменной, исправил имя переменной и добавил сложение с глобальной.</br>
Далее убрал - pass, т.к нигде не используется. После исправления стало - No Issues. Hooray! </br>
`def increment(i):`</br>
: `index = i + 1`</br>
`   return index`</br>
`def get_square(numb):`</br>
`    return numb*numb`</br>
`def print_numb(numb):`</br>
`   print("Number is {}".format(numb))`</br>
</br>
`index = 0`</br>
`while (index < 10):`</br>
`   index = increment(index)`</br>
`   print(get_square(index))`</br>
##### sonatype/nexus3:
Не понятно почему контейнер с sonatype/nexus3:latest не запускается на Ubuntu 20.04 LTS, 6Gb ОЗУ. Просто падает и логи в nexus-data/logs не пишет.</br>
На Debian 10 + Docker 20.10.6 - работает.</br>
### Maven-metadata.xml </br>
`<metadata modelVersion="1.1.0">`</br>
`<groupId>netology</groupId>`</br>
`<artifactId>java</artifactId>`</br>
`<versioning>`</br>
`<latest>8_282</latest>`</br>
`<release>8_282</release>`</br>
`<versions>`</br>
`<version>8_102</version>`</br>
`<version>8_282</version>`</br>
`</versions>`</br>
`<lastUpdated>20210806115554</lastUpdated>`</br>
`</versioning>`</br>
`</metadata>`</br>
## sonarscanner result:   
![screen](https://github.com/murzinvit/screen/blob/1f99feec1840c70c0dc50f596ffc7e189f1efe75/Hooray_Ho_Issue.jpg) </br>

