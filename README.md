# base-statistics
Задание на тему: "Основы статистики". 

В этом задании нужно убедиться, что ЦПТ действительно работает. Создайте случайную величину из любого выбранного вами распределения, для разных значений n сгенерируйте 1000 выборок размера n. Постройте гистрограммы средних этих выборок и сделайте выводы.

Решение.
1. Загрузила библиотеки: matplotlib, scipy, numpy, pandas.
2. Выбрала экспоненциальное распределение с параметрами 15 и 1.3: sts.expon(loc=15,scale=1.3). Сгенерировала 1 000 выборок с помощью метода rvs.
3. Построила гистограмму с помощью функционала matplotlib.
4. Указала размеры трех выборок через созданные переменные, создала массивы для сохранения средних по выборкам через array. Указала количество повторов генерации в переменной. На каждом цикле сгенерировала выборки указанных размеров через rvs, посчитала среднее по каждой выборке и добавила в массив средних.
5. Построила график средних выборок n1, n2 и n3.
6. Итог. Мы видим на построенном графике, что распределение случайных величин выборок n1, n2 и n3 стало близко к нормальному.
