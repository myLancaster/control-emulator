# Control theory based emulator
## Описание проекта
Данный проект представляет собой эмулятор работы технологического объекта, с возможностью управления протекающими процессами.

В ходе разработки программного приложения используется метод [пространства состояний](https://en.wikipedia.org/wiki/State-space_representation) для описания поведения динамической системы. Таким образом, технологический объект представлен в виде набора матриц.

Проект включает в себя возможность управления объектом с помощью [линейно-квадратичного регулятора](https://en.wikipedia.org/wiki/Linear%E2%80%93quadratic_regulator), а также ручной режим управления путем изменения заданий технологического процесса.

## Решаемые проблемы
Эмулятор позволяет выполнять предварительную оценку динамики системы. Также может применяться для тестирования работы регуляторов перед внедрением в физическую модель.

## Используемые пакеты
Как и любое другое приложение, эмулятор использует внешние пакеты для упрощения процесса разработки. Одними из таковых являются:
- JAMA - библиотека для выполнения матричных операций;
- JFreeChart - фреймфорк, позволяющий строить графики различных видов;
- Spring Core - ядро Spring, в качестве основы использует [dependency injection](https://en.wikipedia.org/wiki/Dependency_injection) технику, для разрежения зависимостей между классами.

## Задачи на будущие этапы разработки
Поскольку на выходе ожидается полноценный эмулятор для анализа динамики работы различных технологических объектов, предлагаются следующие задания на будущие модификации:
- расширение методов управления (например, [ПИ-регулятор](https://en.wikipedia.org/wiki/PID_controller));
- загрузка конфигурационных файлов из файловой системы;
- GUI-инструменты для изменения модели объекта;
- мультиязычный интерфейс.
