# *Exceptions in Programming and Their Handling (seminars)*

## Урок 1. Обработка ошибок в программировании

### **Задание 1**
**Методы с исключениями**

Реализуйте 3 метода, чтобы в каждом из них получить разные исключения.

1. Метод *arrayOutOfBoundsException* - Ошибка, связанная с выходом за пределы массива

2. Метод *divisionByZero* - Деление на 0

3. Метод *numberFormatException* - Ошибка преобразования строки в число

Важно: они не должны принимать никаких аргументов

### **Задание 2**
**Разность двух массивов**

Реализуйте метод *subArrays*, принимающий в качестве аргументов два целочисленных массива *a* и *b*, и возвращающий новый массив *c*, каждый элемент которого равен разности элементов двух входящих массивов в той же ячейке.

Если длины массивов не равны - верните нулевой массив длины 1.

Напишите свой код в методе *subArrays* класса *Answer*. Метод *subArrays* принимает на вход два параметра:

int[] a - первый массив

int[] b - второй массив


### **Задание 3**
**Частное двух массивов**

Реализуйте метод *divArrays*, принимающий в качестве аргументов два целочисленных массива *a* и *b*, и возвращающий новый массив *с*, каждый элемент которого равен частному элементов двух входящих массивов в той же ячейке.

Если длины массивов не равны - верните нулевой массив длины 1.

Важно: При выполнении метода единственное исключение, которое пользователь может увидеть - *RuntimeException*, т.е. ваше.

Напишите свой код в методе *divArrays* класса *Answer*. Метод *divArrays* принимает на вход два параметра:

int[] a - первый массив

int[] b - второй массив

## Урок 2. Исключения и их обработка

1. Реализуйте метод, который запрашивает у пользователя ввод дробного числа (типа float), и возвращает введенное значение. Ввод текста вместо числа не должно приводить к падению приложения, вместо этого, необходимо повторно запросить у пользователя ввод данных.

2. Если необходимо, исправьте данный код (задание 2 https://docs.google.com/document/d/17EaA1lDxzD5YigQ5OAal60fOFKVoCbEJqooB9XfhT7w/edit)

3. Дан следующий код, исправьте его там, где требуется (задание 3 https://docs.google.com/document/d/17EaA1lDxzD5YigQ5OAal60fOFKVoCbEJqooB9XfhT7w/edit)

4. Разработайте программу, которая выбросит Exception, когда пользователь вводит пустую строку. Пользователю должно показаться сообщение, что пустые строки вводить нельзя.

## Урок 3. Продвинутая работа с исключениями в Java

Напишите приложение, которое будет запрашивать у пользователя следующие данные в произвольном порядке, разделенные пробелом:
Фамилия Имя Отчество датарождения номертелефона пол

Форматы данных:
фамилия, имя, отчество - строки
датарождения - строка формата dd.mm.yyyy
номертелефона - целое беззнаковое число без форматирования
пол - символ латиницей f или m.

Приложение должно проверить введенные данные по количеству. Если количество не совпадает с требуемым, вернуть код ошибки, обработать его и показать пользователю сообщение, что он ввел меньше и больше данных, чем требуется.

Приложение должно попытаться распарсить полученные значения и выделить из них требуемые параметры. Если форматы данных не совпадают, нужно бросить исключение, соответствующее типу проблемы. Можно использовать встроенные типы java и создать свои. Исключение должно быть корректно обработано, пользователю выведено сообщение с информацией, что именно неверно.

Если всё введено и обработано верно, должен создаться файл с названием, равным фамилии, в него в одну строку должны записаться полученные данные, вида

<Фамилия><Имя><Отчество><датарождения> <номертелефона><пол>

Однофамильцы должны записаться в один и тот же файл, в отдельные строки.

Не забудьте закрыть соединение с файлом.

При возникновении проблемы с чтением-записью в файл, исключение должно быть корректно обработано, пользователь должен увидеть стектрейс ошибки.

Данная промежуточная аттестация оценивается по системе "зачет" / "не зачет"

"Зачет" ставится, если слушатель успешно выполнил
"Незачет"" ставится, если слушатель успешно выполнил

Критерии оценивания:
Слушатель напишите приложение, которое будет запрашивать у пользователя следующие данные в произвольном порядке, разделенные пробелом