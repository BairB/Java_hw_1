# Отчет о тестировании OpenJDK11

## Краткое описание

3 марта 2012 было проведено тестирование установки приложения OpenJDK11
На тестирование затрачено: 1 час

## Описание процесса тестирования

Шаг 1. Перейти на сайт [adoptopenjdk.net](https://adoptopenjdk.net). 

Шаг 2. Выбрать опции как на скриншоте ниже и нажать на кнопку скачивания:

![](https://github.com/netology-code/javaqa-homeworks/raw/master/intro/pic/win-adoptopenjdk.png)


Шаг 3. Запустить на установку скачанный MSI-файл и нажать кнопку "Next":

![](https://github.com/netology-code/javaqa-homeworks/raw/master/intro/pic/win-step1.png)

Шаг 4. Прочитать и согласиться с условиями лицензии:

![](https://github.com/netology-code/javaqa-homeworks/raw/master/intro/pic/win-step2.png)

Шаг 5. Выбрать опции как на экране (удостовеится, что установка происходит в `Program Files` и опция `Add to PATH` выбрана):

![](https://github.com/netology-code/javaqa-homeworks/raw/master/intro/pic/win-step3.png)

Шаг 6. Нажать на кнопку "Install":

![](https://github.com/netology-code/javaqa-homeworks/raw/master/intro/pic/win-step4.png)

Шаг 7. Дождаться окончания установки и нажать на кнопку "Finish":

![](https://github.com/netology-code/javaqa-homeworks/raw/master/intro/pic/win-step5.png)

Шаг 8. Открыть терминал и выполнить команду:

java -version

ОР: 
На экране терминала появляется надпись:
openjdk version "11.0.5" 2019-10-15
OpenJDK Runtime Environment AdoptOpenJDK (build 11.0.5+10)
OpenJDK 64-Bit Server VM AdoptOpenJDK (build 11.0.5+10, mixed mode)

ФР:
На экране терманала появляется надпись: 
C:\Users\User>java -version
openjdk version "11.0.10" 2021-01-19
OpenJDK Runtime Environment AdoptOpenJDK (build 11.0.10+9)
OpenJDK 64-Bit Server VM AdoptOpenJDK (build 11.0.10+9, mixed mode)



## Тестирование проводилось в следующем окружении
Версия и разрядность ОС: Windows 10 Pro, 64 bit
Версия Java: Version 8 Java (build 1.8.0_281-b09)


