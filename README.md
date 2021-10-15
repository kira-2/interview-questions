# Вопросы с собесов

<a id="top"></a>

| уу | #   | Вопрос                                                                              |
| - | --- | ----------------------------------------------------------------------------------- |
| - [x] | 1   | [Что такое singleton](#1)                                                           |
| - [ ] | 2   | [Есть ли ссылки у класса и у строк / Классы и строки являются ссылочным типом?](#2) |

- [ x ]
- [x]
- [-]

## Есть ли ссылки у класса и у строк / Классы и строки являются ссылочным типом? <a id="2"></a>

Классы - да, строки нет.Rkfccs - lf^ cnhjrb ytn&

Строки примитивный тип данных, в них ссылок нет, а вот объекты - это ссылочный тип

## Контекст стрелочной функции

В отличие от других функций, стрелочные функции не имеют собственного контекста выполнения.

На практике это означает, что они наследуют сущности this и arguments от родительской функции.

## области видимости у let и const

1. Область видимости переменной let – блок {...}.
2. Переменная let видна только после объявления.
3. При использовании в цикле, для каждой итерации создаётся своя переменная.
    1. Переменная var – одна на все итерации цикла и видна даже после цикла:

## Sec 2.2

### что делает super у класса

- При переопределении конструктора:
  - Обязателен вызов конструктора родителя super() в конструкторе Child до обращения к this.
- При переопределении другого метода:
  - Мы можем вызвать super.method() в методе Child для обращения к методу родителя Parent.

### чем отличаются коллекции set и map

у Set уникальные значения, у Map ключ-значение

## <a id="1"></a> что такое singleton

паттерн программирования

[∧ top](#top)<br>
[⤒ top](#top)<br>
[↑ top](#top)<br>
[⬆ top](#top)<br>

### демонизация node.js

nodemon

## Рассказать об опыте на ноде 1

- среда выполнения для js. по сути — движок V8 + ряд механизмов, позволяющих выполнять js-код вне браузера
- позволяет с помощью кода, написанного на js, взаимодействовать с файловой системой компьютера, системой ввода/вывода и другими сущностями, которые недоступны из браузера
- поддержка модульности;
- возможность не только слать запросы, но и получать и обрабатывать;
- менеджер зависимостей (npm);
