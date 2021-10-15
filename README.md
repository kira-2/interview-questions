# Вопросы с собесов

## Контекст стрелочной функции

В отличие от других функций, стрелочные функции не имеют собственного контекста выполнения.

На практике это означает, что они наследуют сущности this и arguments от родительской функции.

## области видимости у let и const

### что делает super у класса

- При переопределении конструктора:
  - Обязателен вызов конструктора родителя super() в конструкторе Child до обращения к this.
- При переопределении другого метода:
  - Мы можем вызвать super.method() в методе Child для обращения к методу родителя Parent.

### чем отличаются коллекции set и map

у Set уникальные значения, у Map ключ-значение

### демонизация node.js

nodemon

## Рассказать об опыте на ноде 1

- среда выполнения для js. по сути — движок V8 + ряд механизмов, позволяющих выполнять js-код вне браузера
- позволяет с помощью кода, написанного на js, взаимодействовать с файловой системой компьютера, системой ввода/вывода и другими сущностями, которые недоступны из браузера
- поддержка модульности;
- возможность не только слать запросы, но и получать и обрабатывать;
- менеджер зависимостей (npm);
============================================================================
"контекст стрелочной функции (стрелочные функции не имеют собственного контекста выполнения. На практике это означает, что они наследуют сущности this и arguments от родительской функции.)

области видимости у let и const (Область видимости переменной let – блок {...}.
Переменная let видна только после объявления.
При использовании в цикле, для каждой итерации создаётся своя переменная.
Переменная var – одна на все итерации цикла и видна даже после цикла)
что делает super у класса)

============================================================================

<a id="top"></a>

| #   | Вопрос                                                                |
| --- | --------------------------------------------------------------------- |
| 1   | [Что такое Singleton](#1)                                             |
| 2   | [Классы и строки являются ссылочным типом?](#2)                       |
| 3   | [Демонизация Node.js](#3)                                             |
| 4   | [Чем отличаются коллекции `Set` и `Map`](#4)                          |
| 5   | [Oбласти видимости у `let` и `const`](#5)                             |
| 99  | [javascript, паттерны и принципы проектирования, браузерное апи](#99) |

## <a id="1"></a> Что такое Singleton

Паттерн программирования, должен гарантированно иметь лишь один объект, и к этому объекту должен быть предоставлен глобальный доступ.

[↑ scroll up](#top)

## <a id="2"></a> Классы и строки являются ссылочным типом?

Классы - да, строки нет.

Строки примитивный тип данных, в них ссылок нет, а вот объекты - это ссылочный тип.

[↑ scroll up](#top)

## <a id="3"></a> Демонизация Node.js

nodemon, supervisor, …

[↑ scroll up](#top)

## <a id="4"></a> Чем отличаются коллекции **Set** и **Map**

У `Set` уникальные значения, у `Map` ключ-значение.

[↑ scroll up](#top)

## <a id="5"></a> Oбласти видимости у `let` и `const`

1. Область видимости переменной let – блок {...}.
2. Переменная let видна только после объявления.
3. При использовании в цикле, для каждой итерации создаётся своя переменная.
    - Переменная var – одна на все итерации цикла и видна даже после цикла:

[↑ scroll up](#top)
