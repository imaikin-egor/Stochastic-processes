# Stochastic-processes
Задание
1) Создать модель для симуляции 3 скоррелированных между собой риск-факторов:

Мгновенная процентная ставка для валюты Рубль

Мгновенная процентная ставка для валюты Доллар США

Обменный курс Рубль-Доллар

Для симуляции процентных ставок использовать модель Кокса-Ингерсолла-Росса (CIR)

Для симуляции обменного курса использовать логарифмическую модель (будет дана на ближайшей лекции)

Симуляции провести для расчетной даты 10.12.2021

Необходимы комментарии - обоснования для выборов параметров моделей (волатильность, уровень среднего, скорость возврата к среднему и т.д.)

Выбор шага симуляции и количества симуляций обосновать (используя 2 задачу проекта)

Для симуляций могут быть выбраны с обоснованиями за дополнительный балл и другие симуляционные модели, основанные на стохдиффурах


2) На основании симуляций динамики обменного курса для пары рубль-долллар оценить справедливую стоимость для продукта Range Accrual

Для прайсинга необходимо создать отдельный модуль, который будет принимать на вход список параметров продукта:

Верхняя граница диапазона (или ее отсутствие)

Нижняя граница диапазона (или ее отсутствие)

Номинал сделки (максимальную выплату, доступную в случае нахождения внутри диапазона в течение всего срока жизни сделки)

Дата начала действия контракта

Дата окончания действия контракта

Модуль прайсинга вызывает модель симуляции процентных ставок и обменного курса и принимает обратно симуляции с началом в дату начала действия контракта (для простоты считаем, что расчеты проводим в динь заключения). В качестве результата выдаем справедливую стоимость дериватива
