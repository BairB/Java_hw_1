# Отчет о тестировании приложения KeyValidator

## Краткое описание

3 марта 2012 было проведено тестирование совместимости приложени KeyValidator с Java 11
На тестирование затрачено: 1 час

## Описание процесса тестирования

1. Открыть терминал и перейти в папку с приложением:
 
![](https://downloader.disk.yandex.ru/preview/659595f5fa1b3f0ed683d4592dcce6ab2bb194884fddafb5dcbe5431e42b6a01/603fa559/pq3Vt3AEqTUtJh63Jofcvg-f839fXNwPWo613nj_wxqA4kTlOXVgWUq-ICLFAFRfRXRvvKDF81NzTitv3A5Fgg%3D%3D?uid=0&filename=terminal.png&disposition=inline&hash=&limit=0&content_type=image%2Fpng&owner_uid=0&tknv=v2&size=2048x2048)

2. Ввести команду:

java KeyValidator 00000000-0000-0000-0000-000000000000 00000000-0000-0000-0000-000000000001

где 00000000-0000-0000-0000-000000000000, 00000000-0000-0000-0000-000000000001 - передаваемые для валидации ключи.

![](https://downloader.disk.yandex.ru/preview/038e3846cc3490dff165dd1256b07524b9609eb9156febd907ca8c2714e37145/603fa57d/RWkz1DqQNwWKL_V1eywOW7UV7M50CGRvuqypIX6acHd1vG0GnPN5C8ASRhih3mEuQUE_tkJ2sGSR9jfV0cmF2w%3D%3D?uid=0&filename=keyValidator.png&disposition=inline&hash=&limit=0&content_type=image%2Fpng&owner_uid=0&tknv=v2&size=2048x2048)

* ОР:
В результате выполнения команды в окне термаинала выводится сообщение:
Result for 00000000-0000-0000-0000-000000000000: OK
Result for 00000000-0000-0000-0000-000000000001: FAIL
где OK означает, что ключ валидный, FAIL - невалидный.

* ФР:
В результате выполнения команды в окне термаинала выводится сообщение:
Result for 00000000-0000-0000-0000-000000000000: OK
Result for 00000000-0000-0000-0000-000000000001: FAIL

## Тестирование проводилось в следующем окружении
Версия и разрядность ОС: Windows 10 Pro, 64 bit
Версия Java: Version 8 Java (build 1.8.0_281-b09)