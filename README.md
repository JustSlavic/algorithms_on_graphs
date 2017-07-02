# Задание 3: Прыгающая лягушка

## Тема задания: поиск надежного пути, топологическая сортировка

### Условие задачи:

Лягушка прыгает с кочки на кочку. При этом кочки после дождя достаточно скользкие и она имеет шанс упасть в воду. Вероятность того, что лягушка не соскользнет при прыжке с `i`-ой кочки на `j`-ую кочку равна `p[i][j]`. Кочки нумеруются от `0` до `N-1`, где `N` – количество кочек.
Требуется написать программу, которая определяет маршрут от кочки `0` до кочки `N-1`, прыгая по которому, вероятность соскользнуть для лягушки минимальна, причем известно, что как бы лягушка не прыгала, она никогда не может попасть на кочку, на которой уже была.

### Формат входного файла

Первая строка содержит число `N` – количество кочек. Следующие `N` строк содержат по `N` вещественных значений `p[i][j]`, при этом строка с номером `i+2` описывает вероятности прыжка с кочки с номером `i` до всех кочек с номерами `j`. Если `p[i][j] = 0`, то лягушка не может прыгнуть с кочки `i` на кочку `j`. Вероятность задается числом с двумя знаками после запятой.

### Формат выходного файла

В первой строке нужно указать два числа разделенных одиночным пробелом. Первое - вероятность успеха лягушки на самом надежном пути, представленное вещественным числом с точностью до сотых `(0.01)`. Второе - целое число, описывающее количество кочек на которых придется побывать лягушке на своем самом надежном пути.
Во второй строке выходного файла должна содержаться последовательность номеров кочек, разделенных одиночными пробелами, описывающая самый надежный маршрут. То есть маршрут, по которому лягушке стоит прыгать, чтобы упасть с наименьшей вероятностью.