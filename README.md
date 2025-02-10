### Паранраф 26 
1) Компьюютерная арифмеетика, техническая дисциплина, предметом исследования которой являются представление чисел в ЭВМ, алгоритмы вычисления элементарных функций, арифметических операций и другие, а также реализующая их аппаратура.

2) В компьютерах вещественные числа хранятся в регистрах и ячейках памяти с ограниченным количеством разрядов. Поэтому точность представления вещественных чисел является конечной, а диапозон ограничен.

3) При сложении может возникнуть ситуация, когда старшие разряды результата операции не помещаются в отведенной для него области памяти. Такая ситуация называется переполнением разрядной сетки формата числа.

4) Дробная часть числа ограничена, поэтому любое число, имеющее более трёх цифр после запятой, не может быть представлено точно: младшие цифры придётся отбрасывать.

5) Антипереполнение — это ситуация, когда результат операции становится настолько близким к нулю, что порядок числа выходит за пределы разрядной сетки. По мнению некоторых источников, переполнение более опасно для вычислений, так как оно приводит к значительным ошибкам и некорректным результатам. Антипереполнение, хотя и вызывает неточности, обычно не столь критично для большинства задач.

6) Антипереполнение может сделать дальнейшие вычисления невозможными, если полученный результат нужно разделить на него.

7) Знаковый разряд несёт один бит информации, поскольку он имеет два допустимых значения: 0 и 1

8) Примеры величин, которые по своему смыслу могут иметь только целые значения: Год рождения, Номер квартиры.

9) Деление

10) Временем исполнения команды, и размером операндов.

11) Разделение в компьютере целых и вещественных (дробей) чисел даёт следующие преимущества: Экономичное использование компьютерной памяти. Целые числа занимают меньше места в памяти, чем вещественные. Например, целые числа в интервале от 0 до 255 в языке Паскаль можно хранить в переменных типа byte, которые занимают всего один байт. Ускорение операций. Операции с целыми числами, как правило, выполняются значительно быстрее, чем с вещественными. В ядре современных процессоров реализованы только целочисленные арифметические действия, а для вещественной арифметики используется специализированный встроенный блок. Удобство в определённых задачах. Только для целых чисел определены операции деления нацело и нахождения остатка. В некоторых задачах они удобнее, чем простое деление с получением дробного (к тому же не совсем точного) результата. Например, без них не обойтись при вычислении наибольшего общего делителя двух чисел.

12) Дискретные величины — это те, множество значений которых состоит из отдельных чисел, не сливающихся в интервалы или отрезки. Например, в большинстве случаев это будет некоторое конечное подмножество целых чисел.
Непрерывные величины — это те, у которых множество возможных значений представляет собой непрерывный отрезок или несколько отрезков на числовой прямой. Иногда этим множеством будет вся числовая прямая. 1
В математике переменная может быть дискретной в одних диапазонах числовой строки и непрерывной в других.
Обоснование: в некоторых контекстах для любого значения в диапазоне, который разрешено принимать переменной, существует положительное минимальное расстояние до ближайшего другого другого допустимого значения.

13) Во-первых, непрерывность бывает разной: в точке, справа и слева от этой точки f(c+0), f(c),f(c-0) на промежутке (открытом или закрытом), на бесконечности или в ООФ
Во-вторых, справедливо другое: если функция непрерывна и ограничена, то такая функция необходимо стремится к пределу.

14) Да, можно увеличить разрядность обрабатываемых чисел по сравнению с аппаратной разрядностью компьютера.


### Задачи.

255, 999
2^16 – 1 = 65 535, 2^32 – 1 = 4 294 967 295
2^-16 = 0,0000152587890625; 1,234567 1,234568
‐32767
Например, факториал числа 9, т.е. 1⋅2⋅3⋅…⋅9 = 362880 > 2^16


### Параграф 27 
1) Представление целых чисел со знаком и без знака в компьютере отличается способом, которым отводится бит для обозначения знака числа. В числах со знаком старший бит (знаковый бит) используется для указания знака числа - 0 для положительных чисел и 1 для отрицательных чисел. В числах без знака все биты отводятся для представления самого числа, и они могут принимать только неотрицательные значения.

2) Примеры величин, которые всегда имеют целые неотрицательные значения, включают количество предметов, количество денег, количество людей и т.д. Такие величины никогда не могут быть отрицательными.

3) Целые числа без знака в компьютере представляются прямым кодом. Каждый бит в таком числе отображает определенную степень двойки (от 2^0 до 2^(n-1)), и значение числа получается путем сложения всех этих степеней двойки, которым соответствуют установленные биты.

4) Диапазон представления чисел увеличивается с увеличением количества разрядов. Если увеличить количество разрядов на 1, то диапазон будет увеличен в два раза (возможность хранения большего числа), так как каждый новый разряд может принимать значения либо 0, либо 1. Аналогично, если увеличить количество разрядов на 2 или n, то диапазон увеличится соответственно в 4 или в 2^n раз.

5) Максимальное целое беззнаковое число, которое можно записать с K двоичных разрядов, равно (2^K - 1), так как все разряды заполнены единицами. Если прибавить единицу к этому максимальному значению, то произойдет переполнение и получится число 0.

6) При переполнении процессор обычно отбрасывает старшие разряды результата, оставляя только младшие разряды. Это может привести к искажениям данных и неправильным результатам операций.

7) Максимальное положительное и минимальное отрицательное значения у целых двоичных чисел со знаком имеют разные абсолютные значения, так как старший бит (знаковый бит) в отрицательных числах отводится для обозначения знака, а не для представления значения числа. Это приводит к смещению диапазона значений в отрицательную сторону.

8) Нет, положительные числа не кодируются одинаково в знаковом и беззнаковом форматах. В знаковом формате старший бит используется для обозначения знака числа, в то время как в беззнаковом формате все биты отводятся для представления самого числа.

9) Существуют различные алгоритмы получения дополнительного кода для отрицательного числа. Например, можно инвертировать все биты положительного числа и затем прибавить к нему единицу, чтобы получить дополнительный код этого числа.

10) Алгоритмы Al, A2 и A3 дают один и тот же результат, так как они все основаны на применении операции инверсии (побитового отрицания) и операции сложения к положительному числу.

11) Минимальное отрицательное значение, которое можно записать с K двоичных разрядов, равно -2^(K-1), так как старший бит отведен для обозначения знака (равен 1).

12) Переполнение может возникнуть при сложении двух отрицательных чисел и в этом случае знак результата будет положительным. Например, если сложить -2 и -3, то получится -5, что превышает допустимый диапазон отрицательных чисел.

13) Если правила перевода в дополнительный код применить к отрицательному числу, то получится обратный код числа с добавлением к младшему разряду единицы.

14) Чтобы проверить правильность перевода отрицательного числа в дополнительный код, можно воспользоваться следующим алгоритмом:

15) Если старший (знаковый) разряд числа, записанного в прямом коде, равен 0, то число положительное и никаких преобразований не делается.

16) Если старший (знаковый) разряд числа, записанного в прямом коде, равен 1, то число отрицательное, все разряды числа, кроме знакового, инвертируются, а к результату прибавляется 1.

17) Его преимущество заключается в том, что он позволяет:

18) Заменить операцию вычитания на операцию сложения;

19) Сделать операции сложения и вычитания одинаковыми для знаковых и беззнаковых чисел, что упрощает архитектуру ЭВМ.

В источнике говорится, что вместо вычитания в компьютере используется сложение с дополнительным кодом вычитаемого.
