Слова Дика для ПСП длины n.
*Правильная скобочная последовательность* &mdash; последовательность из открывающих (кодируется нулём) и закрывающих (кодируется единицей) скобок, в которой количество открывающих скобок равно количеству закрывающих, при этом в любом префиксе последовательности количество закрывающих скобок не превосходит количества открывающих.

Автор: Константин Челпанов.

OEIS: [A000108](https://oeis.org/A000108) (Catalan numbers) &mdash; количество слов Дика для ПСП длины n.
Здесь n-ое число Каталана равно количеству правильных скобочных последовательностей длины 2 * n.

Ссылки:
[Wikipedia](https://en.wikipedia.org/wiki/Catalan_number),
[Wikipedia 2](https://en.wikipedia.org/wiki/Dyck_language),
[MathWorld](http://mathworld.wolfram.com/CatalanNumber.html).

Альтернативные описания:

1. количество триангуляций выпуклого (n+2)-угольника непересекающимися диагоналями;
2. количество способок соединить 2 * n точек на окружности n непересекающимися хордами;
3. количество таблиц Юнга 2 * n (в таблице числа от 1 до 2 * n, при этом в строках последовательности возрастают и любое число первой строки меньше соответствующего числа второй строки);
4. количество последовательностей из (2n+1) чисел, каждое из которых равно +1 или -1, при этом их сумма равна 1, а все частичные суммы положительны.

Количество способов в каждом случае равно n-ому числу Каталана.

Предподсчёт: O(N^2), где N=70 &mdash; максимальное число, для которого N-ое число Каталана вмещается в `int64_t`.

Функция `generate_all`: O(n * answer).

Функция `is_valid`: O(n).

Функция `number_by_object`: O(n).

Функция `object_by_number`: O(n).

Функция `next`: O(n), амортизированно за O(1).

Функция `prev`: O(n), амортизированно за O(1).
