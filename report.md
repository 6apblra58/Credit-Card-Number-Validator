# Отчёт о тестировании Credit Card Number Validator

## Краткое описание

Начало тестирования 18.01.2021 - 18.01.2021

Было проведено функциональное тестирование (метод черного ящика) поля ввода номера карты приложения *Credit Card Number Validator*.

На тестирование затрачено: 2 часа

*В результате тестирования выявлены следующие дефекты:*

Баг-репорт №1 (Ввод валидных значений в поле ввода номера карт) приложения Credit Card Number Validator

Описание процесса тестирования
Тест №1 - Ввод 16-значного номерка карты "0000000000000000"

**Ожидаемый результат** - "Result is FAIL"

**Фактический результат** - "Result is FAIL"



Тест №2 - Ввод 14-значного валидного номера карты "36283208288670" платежной системы Diners Club - International

**Ожидаемый результат** - ""Result is OK""

**Фактический результат** - "Result is FAIL"

[Ответ приложения(Credit Card Number Validator) "FAIL" на ввод валидного ключа платежной системы Diners Club - International](https://github.com/6apblra58/Credit-Card-Number-Validator/issues/1#issue-787827658)

Тест №3 Ввод 17-значного валидного номера карты "36283208288670" платежной системы American Express (AMEX)

**Ожидаемый результат** - ""Result is OK""

**Фактический результат** - "Result is FAIL"

[Ответ приложения(Credit Card Number Validator) "FAIL" на ввод валидного ключа платежной системы American Express (AMEX)](https://github.com/6apblra58/Credit-Card-Number-Validator/issues/2#issue-788134029)


Тест №4 - Ввод 16-значного валидного номера карты "5188985381044119" платежной системы MasterCard

**Ожидаемый результат** - "Result is OK"

**Фактический результат** - "Result is OK"



Тест №5 - Ввод 17-значного номера карты "4485855163207296" платежной системы Visa

**Ожидаемый результат** - ""Result is FAIL""

**Фактический результат** - "Result is FAIL"



Тест №6 - Ввод 21-значного номера карты "3536138310452150673" платежной системы JSB

**Ожидаемый результат** - ""Result is OK""

**Фактический результат** - "Result is FAIL"

[Ответ приложения(Credit Card Number Validator) "FAIL" на ввод валидного ключа платежной системы JSB](https://github.com/6apblra58/Credit-Card-Number-Validator/issues/3#issue-788154331)


Тест №7 - Оставляем поле пустым

**Ожидаемый результат** - ""Result is FAIL""

**Фактический результат** - "Result is FAIL"



Тест №8 - Ввод 16 значений на латинице "QWERTYASDFZXCVTYUI"

**Ожидаемый результат** - ""Result is FAIL""

**Фактический результат** - "Result is FAIL"



В качестве тестовых данных использовались номера карт из веб-сайта https://www.freeformatter.com/credit-card-number-generator-validator.html:

**Тестирование производилось в следующем окружении:**

Windows 10 Home Edition x64

java version "11.0.9.1" 2020-11-04

Google Crome Версия 87.0.4280.141 (Официальная сборка), (64 бит)

IntelliJ IDEA 2020.2.3 (Community Edition)
