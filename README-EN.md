# Description of the settings for HFbot (cryptocurrency trading bot)


| Setting | Description | Type | default |
| ------- | ----------- | ---- | ------- |
| language | The language of the interface (ru or en) <br> **language="ru"** | string | en |
| exchange | The choice of the exchange. (binance, ftm, kucoin) <br> **exchange="binance"** | string | - |
| market   | Trading pair <br> BTC/USDT, ETH/BUSD <br> **market="BTC/USDT"** | string | - |
| algorithm| Strategy for a chosen traiding pair <br> short, long <br> **algorithm="long"** | string | - |
| grow_first | Accumulated currency <br> **grow_first="false"** | boolean | - |
| percent_of_amout | Select a percentage of the deposit or a fixed deposit <br> **percent_of_amount="false"** | boolean | - |
| can_spend | Deposit allocated for the bot <br> **can_spend="1000.0"** | float | - |
| first_step | Buying an order at market 0, or at a limit of 0.01 and higher <br> **first_step="0.0"** | float | - |
| lift_step | If the order did not work, then we lift it by this percentage <br> **lift_step="0.2"** | float | - |
| range_cover | Safety order step scale <br> **range_cover="2.2"** | float | - |
| orders_total | Number of orders from base orders + safety orders <br> **orders_total="4"** | integer | - |
| one_or_more | How many safety orders to place on the exchange with a dynamic safety order, if dCO enabled, set to "true" <br> **one_or_more="true"** | boolean | - |
| free_dynamic_co | Enable the safety order multiplier <br> **free_dynamic_co="true"** | boolean | - |
| dynamic_co_koeff | Safety orders multiplier factor <br> **dynamic_co_koeff="1.3"** | float | - |
| trailing | Enable trailing <br> **trailing="true"** | boolean | false |
| squeeze_profit | Squeeze for trailing <br> **squeeze_profit="2.0"** | float | - |
| trailing_stop | Trailing stop <br> **trailing_stop="0.4"** | float | - |
| limit_stop | Limit stop <br> **limit_stop="0.6"** | float | - |
| log_distribution | Enable bot logging (true/false) <br> **log_distribution="true"** | boolean | false |
| time_sleep | Time of exchange polling (from 20.0 ms to infinite) <br> **time_sleep="40.0"** | float | 20.0 |
| martingale | Martingale if you don't use indicator entry <br> **martingale="80.0"** | float | - |
| profit | Take profit if you don't use indicators <br> **profit="2.0"** | float | - |
| back_profit | With each safety order, the take profit decreases, unless the value is set to 0.0 <br> **back_profit="0.0"** | float | 0.0 |
| use_indicators | Enable the use of indicators for dynamic safety orders <br> **use_indicators="true"** | boolean | false |
| co_safety_price | The indent at which the bot will not average after the last triggered safety order. The larger take profit, the greater the percentage <br> **co_safety_price="1"** | integer | 0 |
| new_order_time | Delay in seconds to prevent false triggering of safety orders <br> **new_order_time="200"** | integer | - |
