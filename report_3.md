# Отчет о тестировании приложения KeyValidator

## Краткое описание

3 марта 2012 было проведено функциональное тестирование приложения KeyValidator
На тестирование затрачено: 1 час

## Описание процесса тестирования

### Проверка валидных ключей

1. Открыть терминал и перейти в папку с приложением:
 
![](https://downloader.disk.yandex.ru/preview/659595f5fa1b3f0ed683d4592dcce6ab2bb194884fddafb5dcbe5431e42b6a01/603fa559/pq3Vt3AEqTUtJh63Jofcvg-f839fXNwPWo613nj_wxqA4kTlOXVgWUq-ICLFAFRfRXRvvKDF81NzTitv3A5Fgg%3D%3D?uid=0&filename=terminal.png&disposition=inline&hash=&limit=0&content_type=image%2Fpng&owner_uid=0&tknv=v2&size=2048x2048)

2. Ввести команду:

java KeyValidator 8f05e6a7-70e9-33d7-bfe7-b19eae0d8998 80b427f8-92cd-3aae-ba04-3927fbe17c6 b295bc63-9f03-3b4b-af80-969b39f8c262 387eedc6-12e9-3b32-9881-63b6b5e85317 c19a8cf9-5c3a-37c5-b7f3-d16d38a0c180

* ОР:
Result for 8f05e6a7-70e9-33d7-bfe7-b19eae0d8998: ОК
Result for 80b427f8-92cd-3aae-ba04-3927fbe17c6 : ОК
Result for b295bc63-9f03-3b4b-af80-969b39f8c262: ОК
Result for 387eedc6-12e9-3b32-9881-63b6b5e85317: ОК
Result for c19a8cf9-5c3a-37c5-b7f3-d16d38a0c180: ОК

* ФР:
Result for 8f05e6a7-70e9-33d7-bfe7-b19eae0d8998: ОК
Result for 80b427f8-92cd-3aae-ba04-3927fbe17c6 : FAIL
Result for b295bc63-9f03-3b4b-af80-969b39f8c262: ОК
Result for 387eedc6-12e9-3b32-9881-63b6b5e85317: FAIL
Result for c19a8cf9-5c3a-37c5-b7f3-d16d38a0c180: ОК

### Проверка невалидных ключей

1. Открыть терминал и перейти в папку с приложением:
 
![](https://downloader.disk.yandex.ru/preview/659595f5fa1b3f0ed683d4592dcce6ab2bb194884fddafb5dcbe5431e42b6a01/603fa559/pq3Vt3AEqTUtJh63Jofcvg-f839fXNwPWo613nj_wxqA4kTlOXVgWUq-ICLFAFRfRXRvvKDF81NzTitv3A5Fgg%3D%3D?uid=0&filename=terminal.png&disposition=inline&hash=&limit=0&content_type=image%2Fpng&owner_uid=0&tknv=v2&size=2048x2048)

2. Ввести команду:

java KeyValidator 18252235-78e0-44a5-8720-556f0c7da17a e66075b6-ddad-445e-baf6-161b3289522b b6d53250-f07e-4352-a293-6102ddf7f1ca c2bc778a-1cb9-46c6-b435-0489649d2a42 2fb98b44-93e7-3bdd-a2ad-79347bfe4ad1

* ОР:
Result for 8f05e6a7-70e9-33d7-bfe7-b19eae0d8998: FAIL
Result for 80b427f8-92cd-3aae-ba04-3927fbe17c6 : FAIL
Result for b295bc63-9f03-3b4b-af80-969b39f8c262: FAIL
Result for 387eedc6-12e9-3b32-9881-63b6b5e85317: FAIL
Result for c19a8cf9-5c3a-37c5-b7f3-d16d38a0c180: ОК

* ФР:
Result for 18252235-78e0-44a5-8720-556f0c7da17a: FAIL
Result for e66075b6-ddad-445e-baf6-161b3289522b: FAIL
Result for b6d53250-f07e-4352-a293-6102ddf7f1ca: FAIL
Result for c2bc778a-1cb9-46c6-b435-0489649d2a42: FAIL
Result for 2fb98b44-93e7-3bdd-a2ad-79347bfe4ad1: OK

## Тестирование проводилось в следующем окружении
Версия и разрядность ОС: Windows 10 Pro, 64 bit
Версия Java: Version 8 Java (build 1.8.0_281-b09)