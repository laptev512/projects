Перед нами даннные взаимодействии с рекламными объявлениями на некоторой площадке за 6 дней.
И таблица с характеристиками рекламных клиентов (тех, кто разместил эти объявления).

#### Описание данных:
date - дата\
time - время\
event - действие (просмотр/клик)\
platform - платформа\
ad_id - id объявления\
client_union_id - id рекламного кабинета\
campain_union_id - id рекламной компании\
ad_cost_type - тип оплаты\
ad_cost - цена\
has_video - есть ли видео\
target_audience_count - размер аудитории\

ads_clients_data.csv характеристики рекламных клиентов:\
date - дата\
client_union_id - id рекламного кабинета\
community_id - id сообщества\
create_date - дата создания рекламного клиента\

#### Задачи
1.Разберемся с распределением количества показов и кликов. Посчитаем среднее количество показов и среднее количество кликов на объявления за весь период\ (округлим до целых).\
2.Нарисуем график распределения показов на объявление за весь период.\
3.Посчитаем скользящее среднее показов с окном 2. Какое значение скользящего среднего получим за 6 апреля 2019 года (ответ округлим до целых)?\
4.Скользящее среднее часто используется для поиска аномалий в данных. Давайте попробуем нанести на один график значения арифметического среднего по дням и\
скользящего среднего количества показов. В какой день наблюдается наибольшая разница по модулю между арифметическим средним и скользящим средним? Дни,  в\ которых скользящее среднее равно NaN, не учитываем.\
5.Напишите функцию, которая найдет проблемное объявление (с наибольшим/наименьшим количеством показов) в день, в который была замечена самая большая по\ модулю аномалия.\
6.Теперь подгрузим данные по рекламным клиентам и найдем среднее количество дней от даты создания рекламного клиента и первым запуском рекламного\ объявления этим клиентом.\
7.Вычислим конверсию из создания рекламного клиента в запуск первой рекламы в течение не более 365 дней. Ответ дайте в процентах и округлите до сотых.\
8.Давайте разобъем наших клиентов по промежуткам от создания до запуска рекламного объявления, равным 30. Определите, сколько уникальных клиентов запустили свое первое объявление в первый месяц своего существования (от 0 до 30 дней). Список промежутков для метода pd.cut – [0, 30, 90, 180, 365]\
9. А теперь – выведем на интерактивный график эти категории с количеством уникальных клиентов в них.\
