Основы языка Python для аналитиков (семинары)

Урок 1. Оформление ноутбука и закрепление функций и генераторов
Условие 1:
Оформляйте ноутбук, используя эти советы:
Номер задачи - заголовок 2
Номер подзадачи - заголовок 3
Предоставленные наборы данных оформляйте, как код
Рекомендации для преподавателей по оценке задания:
Смотреть, чтобы студент красиво оформлял ноутбук, использовал ячейки с текстом, указывал номера заданий

Условие 2:
На складе лежат разные фрукты в разном количестве.
Нужно написать функцию, которая на вход принимает любое количество названий фруктов и их количество, а возвращает общее количество фруктов на складе
Условие 2:
На складе лежат разные фрукты в разном количестве.
Нужно написать функцию, которая на вход принимает любое количество названий фруктов и их количество, а возвращает общее количество фруктов на складе
Условие 3:
Дан список с затратами на рекламу. Но в данных есть ошибки, некоторые затраты имеют отрицательную величину. Удалите такие значения из списка и посчитайте суммарные затраты
[100, 125, -90, 345, 655, -1, 0, 200]
Используйте list comprehensions
Условие 4.1:
Даны два списка.
Дата покупки
['2021-09-14', '2021-12-15', '2021-09-08', '2021-12-05', '2021-10-09', '2021-09-30', '2021-12-22', '2021-11-29', '2021-12-24', '2021-11-26', '2021-10-27', '2021-12-18', '2021-11-09', '2021-11-23', '2021-09-27', '2021-10-02', '2021-12-27', '2021-09-20', '2021-12-13', '2021-11-01', '2021-11-09', '2021-12-06', '2021-12-08', '2021-10-09', '2021-10-31', '2021-09-30', '2021-11-09', '2021-12-13', '2021-10-26', '2021-12-09']
Суммы покупок по датам
[1270, 8413, 9028, 3703, 5739, 4095, 295, 4944, 5723, 3701, 4471, 651, 7037, 4274, 6275, 4988, 6930, 2971, 6592, 2004, 2822, 519, 3406, 2732, 5015, 2008, 316, 6333, 5700, 2887]
4.1 Найдите, какая выручка у компании в ноябре
Используйте list comprehensions
4.2 Найдите выручку компании в зависимости от месяца
Для этого напишите функцию, которая на вход принимает список с датами и список с выручкой, а на выходе словарь, где ключи - это месяцы, а значения - это выручка.
Используйте аннотирование типов.

Урок 2. Анализ датасета с помощью Pandas

Условие 1: 1 задача
Скачать файл в уроке
Считать данные с помощью pandas
Вывести на экран первые 5 строк
Посмотреть на описание признаков и на их содержание
Условие 2: 2 задача
Проведите первичный анализ данных
Изучите типы данных
Найдите количество пропущенных ячеек в данных
Посчитайте основные статистики по всем признакам и поизучайте их
Пишите выводы
Условие 3: 3 задача
Ответьте на несколько вопросов
3.1 В каком диапазоне изменяются стоимости недвижимости?
3.2 Какую долю в среднем занимают жилая площадь от всей площади по всем домам?
3.3 Как много домов с разными этажами в данных?
3.4 Насколько хорошие состояния у домов в данных?
3.5 Найдите года, когда построили первый дом, когда построили последний дом в данных?
Условие 4: 4 задача
Ответьте на несколько вопросов

4.1 Сколько в среднем стоят дома, у которых 2 спальни?
4.2 Какая в среднем общая площадь домов, у которых стоимость больше 600 000?
4.3 Как много домов коснулся ремонт?
4.4 Насколько в среднем стоимость домов с оценкой grade домов выше 10 отличается от стоимости домов с оценкой grade меньше 4?
Условие 5: 5 задача
Ответьте на несколько вопросов
5.1 Выберите дом клиенту
Клиент хочет дом с видом на набережную, как минимум с тремя ванными и с подвалом. Сколько вариантов есть у клиента?
5.2 Выберите дом клиенту
Клиент хочет дом либо с очень красивым видом из окна, либо с видом на набережную, в очень хорошем состоянии и год постройки не меньше 1980 года. В какой ценовом диапазоне будут дома?
5.3 Выберите дом клиенту
Клиент хочет дом без подвала, с двумя этажами, стоимостью до 150000. Какая оценка по состоянию у таких домов в среднем?


Урок 3. Изменение таблиц в Pandas
Условие 1: Задача 1
Скачать данные по ссылке https://www.kaggle.com/datasets/ionaskel/laptop-prices
Считать данные с помощью pandas
Вывести на экран первые 5 строк
1.1 Создать новый признак price_per_sq_lot, который будет содержать среднюю стоимость за один кв. метр общей площади
1.2 Создать новый признак delta_renovated, который будет содержать разницу в годах между годом реновацией дома и годом постройки дома
Если реновации дома не было, то в новом признаке поставьте 0
1.3 Создайте признаки года продажи, месяца продажи
1.4 Удалите признаки date, zipcode, lat, long

Условие 2: 2 задача
Создайте датафрейм с клиентами:
clients = pd.DataFrame({
'client_id': [1459, 4684, 3498, 3942, 4535, 2308, 2866, 2765, 1472, 4236, 2295,
939, 3840, 280, 20, 4332, 3475, 4213, 3113, 4809, 2134, 2242,
2068, 4929, 1384, 1589, 3317, 2260, 1727, 1764, 1611, 1474],
'house_id': [8965450190, 6823100225, 5104540330, 2131701075, 1522700060,
1189000207, 6821600300, 7137950720, 9510920050, 6131600255,
5428000070, 1788800910, 8100400160, 3123049142, 6306800010,
5083000375, 7920100025, 1951600150, 809001400, 339600110,
1622049154, 1099600250, 8563000110, 2768100205, 3995700435,
8861700030, 3303980210, 7731100066, 8146100580, 825069097,
3889100029, 9524100196]
})
2.1 Присоедините к таблице clients данные по домам через метод join
2.2 Присоедините к таблице clients данные по домам через метод merge
Это нужно, чтобы понимать, какие дома покупались клиентами
house_id - это индексы датафрейма с домами
Условие 3: 3 задача
Составьте несколько сводных таблиц
3.1 Найдите среднюю стоимость домов в зависимости от количества спален
Отсортируйте от меньшей стоимости к большей
3.2 Найдите минимальную, среднюю и максимальную стоимости домов в зависимости от состояния дома
3.3 Постройте таблицу с подсчетом количества домов в данных в зависимости от вида на набережную и оценкой вида
3.4 Каких домов в зависимости от этажности и количества спален больше?
3.5 Постройте таблицу с подсчетом медианной стоимости домов в данных в зависимости от состояния дома и оценки дома

Урок 4. Визуальный анализ данных
Условие 1: Задача 1
Постройте график
Назовите график
Сделайте именование оси x и оси y
Сделайте выводы

1.1. Скачать данные в закрепе к уроку
1.2 Изучите стоимости недвижимости
1.3 Изучите распределение квадратуры жилой
2.1.4 Изучите распределение года постройки

Условие 2: 2 задача

2.1 Изучите распределение домов от наличия вида на набережную
Постройте график
Сделайте выводы
2.2 Изучите распределение этажей домов
2.2 Изучите распределение состояния домов

Условие 3: 3 задача
Исследуйте, какие характеристики недвижимости влияют на стоимость недвижимости, с применением не менее 5 диаграмм из урока.
Анализ сделайте в формате storytelling: дополнить каждый график письменными выводами и наблюдениями.

