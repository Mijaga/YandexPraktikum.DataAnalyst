Прогнозы и предсказания
Сеть фитнес-центров «Культурист-датасаентист» разрабатывает стратегию взаимодействия с клиентами на основе аналитических данных.

Чтобы бороться с оттоком, отдел по работе с клиентами «Культуриста-датасаентиста» перевёл в электронный вид множество клиентских анкет. Задача — провести анализ и подготовить план действий по удержанию клиентов.

А именно:

научиться прогнозировать вероятность оттока (на уровне следующего месяца) для каждого клиента;
сформировать типичные портреты клиентов: выделить несколько наиболее ярких групп и охарактеризовать их основные свойства;
проанализировать основные признаки, наиболее сильно влияющие на отток;
сформулировать основные выводы и разработать рекомендации по повышению качества работы с клиентами:

1) выделить целевые группы клиентов;

2) предложить меры по снижению оттока;

3) определить другие особенности взаимодействия с клиентами.

Выводы

Полученная модель прогнозирования оттока клиентов довольно точная. Общая точность свыше 92%. Очевидных зависимостей между отдельными признаками и фактом оттока клиента нет.

Результаты анализа:

Большинство клиентов (85%) живет или работает рядом с фитнес-клубом
Примерно половина клиентов являются сотрудниками партнерских организаций
Около 30% клиентов пришли по программе "Приведи друга"
Известны мобильные номера примерно 90% клиентов
Средняя длительность абонементов клиентов - 4.6 месяцев
Около 40% клиентов посещают групповые занятия
Средний возраст клиентов 29 лет
Средние дополнительные расходы на клиента - 146
Средний срок до окончания договора - 4.3 месяцев
Среднее время с момента первого обращения в фитнес-центр - 3.7 месяцев
Средняя частота посещений за все время - 1.87 раз в неделю
Средняя частота посещений за последний месяц - 1.76 раз в неделю
Доля оттока - 27%
Особенности:

Ближе живущие или работающие клиенты реже попадают в отток, что вполне логично
Сотрудники компаний-партнеров реже перестают посещать фитнесс-клуб чем остальные клиенты
Клиенты, пришедшие по акции "Приведи друга" в два раза реже уходят в отток
Наличие мобильного номера клиента не отличается в группах
Оставшиеся пользователи чаще ходят на групповые занятия (хотя возможно, что в отток попали те, кто еще не успел начать ходить на них)
У групп есть разница в среднем возрасте клиентов
Есть небольшое различие в выручке от других услуг фитнес-центра
У клиентов в оттоке меньше среднее количество посещений в неделю за всё время
Количество посещений в предыдущий месяц в два раза ниже у клиентов в оттоке
Рекомендации:

Стимулировать покупку абонементов по акции "приведи друга". Например, давать дополнительные плюши другу.
Стимулировать привлечение клиентов, которые живут и работают поблизости. Например, за счёт наружней рекламы.
Стимулировать привлечение клиентов через партнёров. Например, выпустить для них персонифицированные карты/браслеты. Или сделать корпоративные команды по кроссфиты, пауэрлифтингу или боевым искусствам.
Стимулировать покупку абонементов на более долгий период. Например, давать бесплтаную заморозку или дополнительные месяцы за более длительные абонементы.

Выводы по проекту

Загрузил необзодимые библиотеки и датасет. Посмотрел данные и основную информацию о них. Пропусков и дублей не обнаружил.

Проанализировал средние значения признаков по всей выгрузке, а таже отдельно по ушедшим и оставшимся клиентам. Среди оставшихся на 18% больше парнёрских клиентов и на 12% больше пришёдших по акции "приведи друга". Средний срок абонемента у оставшихся выше в 3 раза, и также такие клиенты немного старше -- почти 30 лет против 27 у ушедших. Чаще уходят те, у кого осталось меньше времени действия абонемента (1,6 месяца против 5,2). Лайфтайм ушедших близок к одному месяцу. Оставшиеся ходят на занятия в два раза чаще.

Построил графики распределения признаков по группам, а также тепловую карту корреляции признаков. Сравнение выборок ушедких и оставшихся клиентов показал, что чаще всего клиенты уходят в течение первого месяца посещений фитнеса. Те же, кто остаётся, продолжает заниматься в среднем в три раза дольше. Если клиент живёт не в районе расположения зала -- у него больше шансов уйти. Анализ матрицы коррелиций показал явную зависимость только между сроком абонемента с числом оставшихся по абонементу месяцев.

Построенная модель прогнозирования оттока клиентов показала достаточно высокую точность как для логистической регрессии, так и для случайного леса, но первая всё же оказалась точнее.

Кластеризировал клиентов на 5 кластеров, их анализ показал следующие особенности:

Нулевой -- Самый долгий срок абонемента, почти 11 месяцев. Отток 3%
Первый -- Среднячки без номеров телефона. Отток 27%.
Второй -- Живут в других районах, далеко от фитнес зала. Отток 44%.
Третий -- Живут рядом в фитнес залом. Отток 51%.
Четвертый -- Похожи на первых, но взяли абонемент на меньший срок. Отток 7%.
Построил графики распределения признаков для каждого кластера и сделал выводы. Привёл рекомендации по уменьшению процента оттока клиентов.
