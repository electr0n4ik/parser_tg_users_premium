# Анализ собственных движений цены фьючерса ETHUSDT, исключая влияние цены BTCUSDT

Определение собственных движений цены фьючерса ETHUSDT, исключая влияние цены BTCUSDT, может быть сложной задачей, но это возможно с использованием статистических методов и анализа корреляции. Ниже приведены шаги и методика:

## Получение исторических данных цен:

Сначала потребуются исторические данные по ценам для фьючерса ETHUSDT и BTCUSDT. Эти данные могут быть загружены с биржи или из финансовых источников.

## Расчет процентного изменения цен:

Расчет процентного изменения цены для обоих фьючерсов ETHUSDT и BTCUSDT на каждом временном интервале (например, час, день и т. д.). Это можно сделать с помощью следующей формулы:

Процентное изменение цены = (Текущая цена - Предыдущая цена) × 100


## Рассчет корреляции:

После того как у меня есть процентные изменения цен для обоих фьючерсов, рассчитываю корреляцию между двумя наборами данных. Корреляция позволит определить, насколько движения цен ETHUSDT и BTCUSDT взаимосвязаны. Использую коэффициент корреляции, такой как коэффициент Пирсона или Спирмана.

Если корреляция близка к 1, это означает, что цены ETHUSDT и BTCUSDT сильно коррелируют, и движения цены ETHUSDT могут сильно зависеть от движения цены BTCUSDT. Если корреляция близка к 0 или отрицательна, это означает, что движения цен не коррелируют или имеют обратную зависимость.

## Исключение влияния BTCUSDT:

Если корреляция между ценами ETHUSDT и BTCUSDT высока, это может указывать на влияние BTCUSDT на ETHUSDT. Чтобы исключить влияние BTCUSDT, можно рассмотреть разные методы, такие как:

- Корреляция остатков: Рассчитать корреляцию между остатками (разницей между фактической ценой и предсказанной моделью) ETHUSDT и BTCUSDT. Если она близка к нулю, это может свидетельствовать об отсутствии влияния BTCUSDT на ETHUSDT.

## Анализ остатков:

Анализирую остатки модели или корреляцию остатков, чтобы определить собственные движения цены ETHUSDT, исключив влияние BTCUSDT.

Методы анализа:
Расчет корреляции:

Шаг 1: Сначала необходимо подготовить исторические данные по ценам ETHUSDT и BTCUSDT для одного и того же временного интервала. Обычно используются ежедневные, ежечасные или другие интервалы в зависимости от конкретных целей анализа.

Шаг 2: Рассчитать процентное изменение цен для обоих фьючерсов на выбранном временном интервале, используя формулу:

Процентное изменение цены = (Текущая цена - Предыдущая цена) / Предыдущая цена * 100

Шаг 3: После того, как у меня есть процентные изменения цен для обоих активов, использую коэффициент корреляции, такой как коэффициент Пирсона или Спирмана, для расчета корреляции между двумя активами. Можно использовать статистические пакеты, такие как Python с библиотекой Pandas, чтобы выполнить этот расчет.

Шаг 4: Интерпретирую результат корреляции. Если коэффициент корреляции близок к 1, это указывает на сильную положительную корреляцию между двумя активами, что означает, что движения цен ETHUSDT и BTCUSDT сильно взаимосвязаны. Если коэффициент корреляции близок к 0 или отрицателен, это указывает на низкую корреляцию или отрицательную зависимость.

Регрессионный анализ:

Шаг 1: Подготовить исторические данные по ценам ETHUSDT и BTCUSDT, а также временной интервал, для которого проводится анализ.

Шаг 2: Построить модель регрессии, где цена ETHUSDT будет зависеть от цены BTCUSDT. Это может быть линейная или нелинейная модель в зависимости от данных и гипотезы.

Шаг 3: Оценить параметры модели с использованием статистических методов, таких как метод наименьших квадратов.

Шаг 4: Проанализировать остатки модели. Остатки представляют разницу между фактической ценой ETHUSDT и ценой, предсказанной моделью. Если остатки имеют случайный характер и не показывают систематических закономерностей, это может указывать на успешное исключение влияния цены BTCUSDT на ETHUSDT.

Шаг 5: Интерпретировать результаты. Если модель успешно исключает влияние BTCUSDT, можно считать остатки как собственные движения цены ETHUSDT.

Чтобы определить собственную цену ETH на основе ETHUSDT, выполняю следующий расчет:

Собственная цена ETH = Цена ETHUSDT

Например, если текущая цена ETHUSDT составляет 4,000 USD, то это означает, что 1 ETH эквивалентно 4,000 USD.

Для рассчета корреляции между остатками (разницей между фактической ценой и предсказанной моделью) ETHUSDT и BTCUSDT, можно использовать библиотеку Python, такую как NumPy и Pandas, для обработки данных. Также понадобится набор данных с фактическими ценами ETHUSDT и BTCUSDT, а также предсказанными моделью ценами.

Предположим, есть два списка с данными: 

actual_eth_prices (фактические цены ETHUSDT) и actual_btc_prices (фактические цены BTCUSDT), 

а также два списка с остатками: 

residuals_eth (остатки для ETHUSDT) и residuals_btc (остатки для BTCUSDT).
