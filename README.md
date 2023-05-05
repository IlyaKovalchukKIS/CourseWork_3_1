# CourseWork_3_1
Для установки зависимостей использовать команду: poetry install

пример ввода данных:
[
  {
    "id": 441945886,
    "state": "EXECUTED",
    "date": "2019-08-26T10:50:58.294041",
    "operationAmount": {
      "amount": "31957.58",
      "currency": {
        "name": "руб.",
        "code": "RUB"
      }
    },
    "description": "Перевод организации",
    "from": "Maestro 1596837868705199",
    "to": "Счет 64686473678894779589"
  }
 ]

пример вывода операций:

08.12.2019 Открытие вклада
Нет данных -> Счет **5907
41096.24 USD


Фича для отображение последних 5 
успехных банковских операций

разработка основного кода велась в ветке develop
написание тестов происходило в ветке test/testing

в директории src хранится основной код программы
в src/main содаржатся 2 файла:
main.py - основной код
ClassOperations.py - класс операции и 3 метода
для корректного отображения счетов и даты

в директории src/utils содержатся 2 файла:
operations.json - список произведенных операций
utils.py - набор функций для открытия файла operation.json
и функции сортировки по дате и статусу операции

тест происходил с помощью pytest,
хранится в директории tests
