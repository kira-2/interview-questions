# Вопросы с собесов

<a id="top"></a>

| #   | Вопрос                                                                |
| --- | --------------------------------------------------------------------- |
| 1   | [Что такое Singleton](#1)                                             |
| 2   | [Классы и строки являются ссылочным типом?](#2)                       |
| 3   | [Демонизация Node.js](#3)                                             |
| 4   | [Чем отличаются коллекции `Set` и `Map`](#4)                          |
| 5   | [Oбласти видимости у `let` и `const`](#5)                             |
| 6   | [Контекст стрелочной функции](#6)                                     |
| 7   | [Особенности Node.js](#7)                                             |
| 8   | [Что делает super у класса?](#8)                                      |
| 99  | [javascript, паттерны и принципы проектирования, браузерное апи](#99) |

## <a id="8"></a> Что делает super у класса?

- При переопределении конструктора:
  - Обязателен вызов конструктора родителя `super()` в конструкторе Child до обращения к `this`.
- При переопределении другого метода:
  - Мы можем вызвать `super.method()` в методе Child для обращения к методу родителя Parent.

[`↑ scroll up`](#top)

## <a id="7"></a> Особенности Node.js

- среда выполнения для js; по сути — движок V8 + ряд механизмов, позволяющих выполнять js-код вне браузера
- позволяет с помощью кода, написанного на js, взаимодействовать с файловой системой компьютера, системой ввода/вывода и другими сущностями, которые недоступны из браузера
- поддержка модульности;
- возможность не только слать запросы, но и получать и обрабатывать;
- менеджер зависимостей (npm);

[`↑ scroll up`](#top)

## <a id="1"></a> Что такое Singleton

Паттерн программирования, должен гарантированно иметь лишь один объект, и к этому объекту должен быть предоставлен глобальный доступ.

[`↑ scroll up`](#top)

## <a id="2"></a> Классы и строки являются ссылочным типом?

Классы - да, строки нет.

Строки примитивный тип данных, в них ссылок нет, а вот объекты - это ссылочный тип.

[`↑ scroll up`](#top)

## <a id="3"></a> Демонизация Node.js

nodemon, supervisor, …

[`↑ scroll up`](#top)

## <a id="4"></a> Чем отличаются коллекции **Set** и **Map**

У `Set` уникальные значения, у `Map` ключ-значение.

[`↑ scroll up`](#top)

## <a id="5"></a> Oбласти видимости у `let` и `const`

ОВ переменных:

- `let`, `const` – блочная { … }. Видны только после объявления. При использовании в цикле, для каждой итерации создаётся своя переменная.
- `var` – глобальная. Доступ из любого места в коде. Переменная var – одна на все итерации цикла и видна даже после цикла:

```javascript
// С var прокатит:
console.log(hello) // undefined
var hello = "Hello"

// C let и const — нет:
console.log(hello) // Reference error
let hello = "Hello"

console.log(bye) // Reference error
const bye = "Bye"
```

[`↑ scroll up`](#top)

## <a id="6"></a> Контекст стрелочной функции

Стрелочные функции не имеют собственного контекста выполнения. На практике это означает, что они наследуют сущности `this` и `arguments` от родительской функции.

[`↑ scroll up`](#top)
