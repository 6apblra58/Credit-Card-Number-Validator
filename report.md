# Отчёт о тестировании Credit Card Number Validator

## Краткое описание

Начало тестирования 18.01.2021 - 18.01.2021

Было проведено функциональное тестирование (метод черного ящика) поля ввода номера карты приложения *Credit Card Number Validator*.

На тестирование затрачено: 2 часа

*В результате тестирования выявлены следующие дефекты:*

[Ответ Credit Card Number Validator "FAIL" на ввод валидного ключа платежной системы Diners Club - International](https://github.com/6apblra58/Credit-Card-Number-Validator/issues/1#issue-787827658)

[Ответ Credit Card Number Validator "FAIL" на ввод валидного ключа платежной системы American Express (AMEX)](https://github.com/6apblra58/Credit-Card-Number-Validator/issues/2#issue-788134029)

[Ответ Credit Card Number Validator "FAIL" на ввод валидного ключа платежной системы JSB](https://github.com/6apblra58/Credit-Card-Number-Validator/issues/3#issue-788154331)

## Описание процесса тестирования

Тест №1 - Ввод 16-значного номерка карты "0000000000000000"


Тест №2 - Ввод 14-значного валидного номера карты "36283208288670" платежной системы Diners Club - International

Тест №3 - Ввод 14-значного валидного номера карты "30262931447692" платежной системы Diners Club - Carte Blanche

[Ответ Credit Card Number Validator "FAIL" на ввод валидных 14-значных номеров карт](https://github.com/6apblra58/Credit-Card-Number-Validator/issues/1#issue-787827658)

Тест №4 Ввод 17-значного валидного номера карты "377967621265664" платежной системы American Express (AMEX)

Тест №5 Ввод 17-значного валидного номера карты "371954845156362" платежной системы American Express (AMEX)

Тест №6 Ввод 17-значного валидного номера карты "377407362041297" платежной системы American Express (AMEX)

[Ответ Credit Card Number Validator "FAIL" на ввод валидных 17-значных номеров карт ](https://github.com/6apblra58/Credit-Card-Number-Validator/issues/2#issue-788134029)


Тест №7 - Ввод 16-значного валидного номера карты "5188985381044119" платежной системы MasterCard

Тест №8 - Ввод 16-значного номера карты "4485855163207296" платежной системы Visa

Тест №9 - Ввод 16-значного номера карты "4024007164051327" платежной системы Visa

Тест №10 - Ввод 19-значного номера карты "4929754379190944399" платежной системы Visa

Тест №11 - Ввод 19-значного номера карты "3536138310452150673" платежной системы JSB


[Ответ Credit Card Number Validator "FAIL" на ввод валидных 19-значных ключей](https://github.com/6apblra58/Credit-Card-Number-Validator/issues/3#issue-788154331)


Тест №12 - Оставляем поле пустым


Тест №13 - Ввод 16-значного номера карты "6759773749753705" платежной системы Maestro


В качестве тестовых данных использовались номера карт из веб-сайта https://www.freeformatter.com/credit-card-number-generator-validator.html:

## Тестирование производилось в следующем окружении:

Windows 10 Home Edition x64

java version "11.0.9.1" 2020-11-04

Google Chrome Версия 87.0.4280.141 (Официальная сборка), (64 бит)

IntelliJ IDEA 2020.2.3 (Community Edition)
