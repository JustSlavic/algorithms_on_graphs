# Задание 1: Опасные повороты

## Тема задания: поиск кратчайшего пути, алгоритм Дейкстры

### Условие задачи:

Винтик и Шпунтик наконец доделали второй автомобиль и теперь планируют ездить друг к другу в гости. Но проезд в Солнечном городе оказался не столь безопасным.
Для удобства будем считать, что в Солнечном городе все дороги являются отрезками прямых. Перекрестки - это пересечения двух и более дорог. Дома Винтика и Шпунтика расположены на отрезках дорог, но не на перекрестках.
Итак, Винтик собрался ехать к Шпунтику. Из своего дома Винтик может поехать в одном из двух направлений. Доехав до перекрестка, он может поехать дальше по текущей дороге или свернуть на другую. Определим степень опасности поворота как угол поворота с одной улицы на другую в градусах (от `0` до `180`). Чем круче поворот, тем Винтик сильнее подвержен опасности.
Опасность всего пути равна сумме опасностей на каждом повороте.
Требуется написать программу, которая определяет маршрут с наименьшей опасностью для Винтика.

### Формат входного файла

Первая строка содержит число `N` – количество дорог. Следующие `N` строк содержат по `4` целых числа `x[i][1]`, `y[i][1]`, `x[i][2]` и `y[i][2]` разделенных одиночными пробелами. Эти четыре числа задают две точки на плоскости, через которые проходит дорога (прямая). В следующих двух строках заданы координаты домов Винтика и Шпунтика, в виде пар целых чисел разделенных одиночным пробелом.
Гарантируется, что совпадающих дорог нет, что дома Винтика и Шпунтика не лежат на перекрестках, но лежат на дорогах. Кроме того, координаты домов разные.

### Формат выходного файла

В первой строке нужно указать величину наименьшей возможной опасности на пути Винтика к дому Шпунтику. В случае, если никакого пути не существует, вывести `-1`.
