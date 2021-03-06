Учебный план
============

- Примитивные и ссылочные типы
- Способы кодирования чисел
- Функции (передача аргументов и пр.)
- Объекты, система типов Java
- Методы класса Object
- Инкапсуляция, наследование, полиморфизм
- Стандартные коллекции
- Stream API

Задачи
------

### Примитивные и ссылочные типы

1. Написать функцию `Integer sum(Integer[] xs)`.
2. Написать функцию `int sum(int[] xs)`.

Выполнить функции для массивов из 100000 элементов (все элементы должны быть больше 10000).
Какая функция работает быстрее? Почему?

3. Объяснить результаты следующих операций: `new Integer(100) == new Integer(100)`; `Integer.valueOf(100) == Integer.valueOf(100)`; `Integer.valueOf(100000) == Integer.valueOf(100000)`.
4. В программе возникает ошибка `NullPointerException` в такой функции:

```
Integer sum(Integer x, Integer y) {
    return x + y;
}
```

Объяснить причину ошибки и возможные способы исправления.

### Способы кодирования чисел

Справочный материал: https://habrahabr.ru/post/124395/

Контрольные вопросы:

1. Перечислите виды систем счисления, которые вы знаете
2. Перечислите несколько конкретных систем счисления, кроме десятичной, которые используются в информатике
3. Какие из этих форм доступны в языке Java?
4. Что означает запись `0xFF`?
5. Имеется число 256 в десятичной системе. Распечатайте его в шестнадцатеричной системе, пользуясь стандартной функциональностью языка Java (свой конвертер систем счисления писать не нужно).
6. Напишите функцию, которая принимает на вход целое число `n` и возвращает строковое представление этого числа в восьмеричной системе (написать свой конвертер).

### Функции, передача аргументов

1. Реализовать функцию `String concat(String[] x)` (конкатенирует строки, возвращает новую строку)
2. Реализовать функцию `int sum(int[] x)` (складывает числа, возвращает результат)
3. Реализовать функцию `void sort(int[] x)` (сортирует числа в переданном массиве)
4. Реализовать функцию `void sort(String x)` (сортирует символы в переданной строке)
    — **эту функцию написать не получится. Почему?**

5. Реализовать функцию `int[] sort(int[] x)` (сортирует числа, возвращает новый массив с отсортированным результатом)
6. Реализовать функцию `String sort(String x)` (сортирует символы в строке, возвращает строку с отсортированными символами)

### Методы класса Object

1. Реализовать класс с несколькими полями ("свидетельство", поля "номер", "серия").
2. Использовать класс в качестве ключа в `Map`. Пояснить результаты.
3. Перегрузить у него методы `equals` и `hashCode`, попробовать ещё раз. Пояснить результаты.
