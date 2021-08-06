#### 09.02-CI-CD </br>
====================================</br>
В fail.py, в def increment(index):, путалось имя локальной и глобальной переменной, исправил имя переменной и добавил сложение с глобальной.</br>
Далее убрал - pass, т.к нигде не используется. После исправления стало - No Issues. Hooray! </br>
`def increment(i):
    index = i + 1
    return index
def get_square(numb):
    return numb*numb
def print_numb(numb):
    print("Number is {}".format(numb))

index = 0
while (index < 10):
    index = increment(index)
    print(get_square(index))`</br>


### successed:   
![screen](https://github.com/murzinvit/screen/blob/1f99feec1840c70c0dc50f596ffc7e189f1efe75/Hooray_Ho_Issue.jpg) </br>
