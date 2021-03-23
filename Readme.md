# Отчёт о тестировании Credit Card Number Validator

## Краткое описание

21.03.21 - 22.03.21 было проведено функциональное тестирование приложения Credit Card Number Validator.

На тестирование затрачено: 3

В результате тестирования выявлены следующие дефекты:
* https://github.com/anfimova/1.1.CreditCardNumberValidator/issues/1 - 
  Валидное значение карты из более чем 16 символов считается невалидным

## Описание процесса тестирования

В процессе тестирования использовались следующие артефакты:
* https://www.freeformatter.com/credit-card-number-generator-validator.html

В качестве тестовых данных использовались данные:
* 5351719427810741 - Result is OK
* 4240481985838543 - Result is OK
* 5266462038841870 - Result is OK
* 5020602515347126 - Result is OK
* 4929548810661998978 - Result is OK
* 50206025153471261 - Result is FAIL
* 502060251534712 - Result is FAIL
* 1234567890123456 - Result is FAIL
* Пустое значение - Result is FAIL
* 1 - Result is FAIL
* йцукенгшщзфывапр - Result is FAIL
* qwertyuiopasdfgh - Result is FAIL
* !@#$%^&*()_+=-; - Result is FAIL

Тестирование производилось в следующем окружении:
* Windows 10 x64
* Java 11