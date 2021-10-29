# Описание настроек для торгового бота криптовалютой HFbot


| Параметр | Описание | Тип | Параметр по-умолчанию |
| ------- | ----------- | ---- | ------- |
| language | Язык интрефейса (ru или en) <br> **language="ru"** | sting | en |
| exchange | Биржа (binance, ftm, kucoin) <br> **exchange="binance"** | string | - |
| market   | Торгуемая пара <br> BTC/USDT, ETH/BUSD, ... <br> **market="BTC/USDT"** | string | - |
| algorithm| Стратегия для выбранной пары <br> short, long <br> **algorithm="long"** | string | - |
| grow_first | Накапливаемя валюта (true/false) <br> **grow_first="false"** | boolean | - |
| percent_of_amout | Выбирает процент от депозита, либо фиксированный депозит <br> **percent_of_amount="false"** | boolean | - |
| can_spend | Депозит выделяемый для торгуемой пары <br> **can_spend="1000.0"** | float | - |
| first_step | Покупка ордера по рынку - 0 или по лимиту от 0.01 и выше <br> **first_step="0.0"** | float | - |
| lift_step | Если не сработал ордер, то сдвигаем его на указанный процент <br> **lift_step="0.2"** | float | - |
| range_cover | Шаг страховочного ордера <br> **range_cover="2.2"** | float | - |
| orders_total | Количество базовых оредров + страховочных <br> **orders_total="4"** | integer | - |
| one_or_more | Сколько выставлять на бирже страховочных ордеров, при дСО устанавливаем "true" (true/false)<br> **one_or_more="true"** | boolean | - |
| free_dynamic_co | Включить множитель для страховочных ордеров <br> **free_dynamic_co="true"** | boolean | - |
| dynamic_co_koeff | Коэффициент множителя страховочного ордера <br> **dynamic_co_koeff="1.3"** | float | - |
| trailing | Включить трейлинг (true/false)<br> **trailing="true"** | boolean | false |
| squeeze_profit | Сквиз для трейлинга <br> **squeeze_profit="2.0"** | float | - |
| trailing_stop | Трейлинг стоп <br> **trailing_stop="0.4"** | float | - |
| limit_stop | Лимит стоп <br> **limit_stop="0.6"** | float | - |
| log_distribution | Включить логирование бота (true/false) <br> **log_distribution="true"** | boolean | false |
| time_sleep | Опрос биржи в секундах (от 20.0 до бесконечности) <br> **time_sleep="40.0"** | float | 20.0 |
| martingale | Мартингейл, если не стоит вход по индикаторам <br> **martingale="80.0"** | float | - |
| profit | Тейк-профит, если не стоит вход по индикаторам <br> **profit="2.0"** | float | - |
| back_profit | С каждым страховочным ордером тейк-профит понижается, если не 0 <br> **back_profit="0.0"** | float | 0.0 |
| use_indicators | Включить индикаторы для дСО <br> **use_indicators="true"** | boolean | false |
| co_safety_price | Отступ, при котором бот не будет усреднять, после последнего сработанного страховочного ордера, чем больше тейк-профит, тем больше процент. <br> **co_safety_price="1"** | integer | 0 |
| new_order_time | Задержка в секундах, чтобы не было ложных сработок страховочных ордеров <br> **new_order_time="200"** | integer | - |
