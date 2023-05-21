# Comparing `tmp/backtrader_binance-1.0.4.tar.gz` & `tmp/backtrader_binance-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backtrader_binance-1.0.4.tar", last modified: Sun Apr 30 08:27:33 2023, max compression
+gzip compressed data, was "backtrader_binance-1.0.5.tar", last modified: Sun May 21 12:45:05 2023, max compression
```

## Comparing `backtrader_binance-1.0.4.tar` & `backtrader_binance-1.0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 08:27:33.818684 backtrader_binance-1.0.4/
--rw-rw-rw-   0        0        0     1090 2023-04-07 12:36:18.000000 backtrader_binance-1.0.4/LICENSE
--rw-rw-rw-   0        0        0    23941 2023-04-30 08:27:33.818684 backtrader_binance-1.0.4/PKG-INFO
--rw-rw-rw-   0        0        0    22689 2023-04-30 08:26:04.000000 backtrader_binance-1.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-30 08:27:33.813684 backtrader_binance-1.0.4/backtrader_binance/
--rw-rw-rw-   0        0        0       40 2021-06-25 01:58:20.000000 backtrader_binance-1.0.4/backtrader_binance/__init__.py
--rw-rw-rw-   0        0        0     6397 2023-04-05 12:42:51.000000 backtrader_binance-1.0.4/backtrader_binance/binance_broker.py
--rw-rw-rw-   0        0        0     5048 2023-04-05 03:54:03.000000 backtrader_binance-1.0.4/backtrader_binance/binance_feed.py
--rw-rw-rw-   0        0        0     6586 2023-04-30 07:50:22.000000 backtrader_binance-1.0.4/backtrader_binance/binance_store.py
-drwxrwxrwx   0        0        0        0 2023-04-30 08:27:33.817685 backtrader_binance-1.0.4/backtrader_binance.egg-info/
--rw-rw-rw-   0        0        0    23941 2023-04-30 08:27:33.000000 backtrader_binance-1.0.4/backtrader_binance.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      384 2023-04-30 08:27:33.000000 backtrader_binance-1.0.4/backtrader_binance.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 08:27:33.000000 backtrader_binance-1.0.4/backtrader_binance.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       33 2023-04-30 08:27:33.000000 backtrader_binance-1.0.4/backtrader_binance.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-04-30 08:27:33.000000 backtrader_binance-1.0.4/backtrader_binance.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-30 08:27:33.819686 backtrader_binance-1.0.4/setup.cfg
--rw-rw-rw-   0        0        0     2163 2023-04-30 08:27:08.000000 backtrader_binance-1.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-21 12:45:05.364984 backtrader_binance-1.0.5/
+-rw-rw-rw-   0        0        0     1090 2023-04-07 12:36:18.000000 backtrader_binance-1.0.5/LICENSE
+-rw-rw-rw-   0        0        0    25436 2023-05-21 12:45:05.364984 backtrader_binance-1.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0    24174 2023-05-21 12:43:42.000000 backtrader_binance-1.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-21 12:45:05.359984 backtrader_binance-1.0.5/backtrader_binance/
+-rw-rw-rw-   0        0        0       40 2021-06-25 01:58:20.000000 backtrader_binance-1.0.5/backtrader_binance/__init__.py
+-rw-rw-rw-   0        0        0     6397 2023-04-05 12:42:51.000000 backtrader_binance-1.0.5/backtrader_binance/binance_broker.py
+-rw-rw-rw-   0        0        0     5048 2023-04-05 03:54:03.000000 backtrader_binance-1.0.5/backtrader_binance/binance_feed.py
+-rw-rw-rw-   0        0        0     6586 2023-04-30 07:50:22.000000 backtrader_binance-1.0.5/backtrader_binance/binance_store.py
+drwxrwxrwx   0        0        0        0 2023-05-21 12:45:05.363985 backtrader_binance-1.0.5/backtrader_binance.egg-info/
+-rw-rw-rw-   0        0        0    25436 2023-05-21 12:45:05.000000 backtrader_binance-1.0.5/backtrader_binance.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      384 2023-05-21 12:45:05.000000 backtrader_binance-1.0.5/backtrader_binance.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-21 12:45:05.000000 backtrader_binance-1.0.5/backtrader_binance.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       33 2023-05-21 12:45:05.000000 backtrader_binance-1.0.5/backtrader_binance.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-05-21 12:45:05.000000 backtrader_binance-1.0.5/backtrader_binance.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-21 12:45:05.366489 backtrader_binance-1.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     2163 2023-05-21 12:41:26.000000 backtrader_binance-1.0.5/setup.py
```

### Comparing `backtrader_binance-1.0.4/LICENSE` & `backtrader_binance-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `backtrader_binance-1.0.4/PKG-INFO` & `backtrader_binance-1.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backtrader_binance
-Version: 1.0.4
+Version: 1.0.5
 Summary: Binance API integration with Backtrader
 Home-page: https://github.com/WISEPLAT/backtrader_binance
 Author: wiseplat
 Author-email: oshpagin@gmail.com
 License: MIT License
 Project-URL: Documentation, https://github.com/WISEPLAT/backtrader_binance/blob/master/README.md
 Keywords: trading,development
@@ -87,15 +87,19 @@
 * **01 - Symbol.py** - trading strategy for obtaining historical and "live" data of one ticker for one timeframe
 * **02 - Symbol data to DF.py** - export to csv file of historical data of one ticker for one timeframe
 * **03 - Symbols.py** - trading strategy for multiple tickers on the same timeframe
 * **04 - Resample.py** - trading strategy for obtaining data from one ticker for different timeframes by converting a smaller timeframe into a larger one
 * **05 - Replay.py** - launching a trading strategy on a smaller timeframe, with processing on a larger one and displaying a larger interval chart
 * **06 - Rollover.py** - launch of a trading strategy based on gluing data from a file with historical data and the last downloaded history from the broker
 * **07 - Get Asset Balance.py** - getting the ticker balance directly through the Binance API
-* **08 - Timeframes.py** - trading strategy for one ticker on different timeframes
+* **08 - Timeframes.py** - trading strategy is running on different timeframes.
+* **09 - Get Asset Info.py** - getting info about asset: balance, lot size, min price step, min value to buy and etc.
+* **09 - Get Asset Info - no Decimal.py** - getting info about asset: balance, lot size, min price step, min value to buy and etc.
+* **09 - Get Asset Info - through client.py** - getting info about asset: balance, lot size, min price step, min value to buy and etc.
+* **10 - Get Historical Data.py** - getting historical data through binance client for asset.
 * **Strategy.py** - An example of a trading strategy that only outputs data of the OHLCV for ticker/tickers
 
 The **StrategyExamplesBinance** folder contains the code of sample strategies.
 
 * **01 - Live Trade.py** - An example of a live trading strategy for two BTC and ETH tickers on the base USDT ticker.
   * The strategy shows how to apply indicators (SMA, RSI) to several tickers at the same time.
   * Example of placing and cancel orders on the Binance exchange.
@@ -263,14 +267,20 @@
   * Стратегия показывает, как покупать по цене закрытия и продавать по рыночной небольшое количество ETH через 3 бара.
   * Пример размещения ордеров на бирже Binance.
     * **Не забудьте отменить выставленные ордера с биржи после тестирования!**
 * **07 - Offline Backtest Indicators.py** - Пример торговой стратегии для теста на истории с использованием индикаторов SMA и RSI - не live режим - для двух тикеров BTC и ETH на базовом тикере USDT. 
   * В стратегии показано как применять индикаторы (SMA, RSI) к нескольким тикерам одновременно.
     * генерит 177% дохода на момент записи видео )) 
     * Не live режим - для тестирования стратегий без отправки заявок на биржу!
+* **08 - Timeframes.py** - торговая стратегия работает на разных таймфреймах.
+* **09 - Get Asset Info.py* - получение информации об активе: баланс, размер лота, минимальный шаг цены, минимальная стоимость покупки и т.д.
+* **09 - Get Asset Info - no Decimal.py** - получение информации об активе: баланс, размер лота, минимальный шаг цены, минимальная стоимость покупки и т.д.
+* **09 - Get Asset Info - through client.py** - получение информации об активе: баланс, размер лота, минимальный шаг цены, минимальная стоимость покупки и т.д.
+* **10 - Get Historical Data.py** - получение исторических данных через клиент binance для актива.
+
 ## Спасибо
 - backtrader: очень простая и классная библиотека!
 - [python-binance](https://github.com/sammchardy/python-binance ): Для создания оболочки Binance API, сокращающей большую часть работы.
 - lindomar-oliveira за некоторый код
 
 ## Важно
 Исправление ошибок, доработка и развитие библиотеки осуществляется автором и сообществом!
```

### Comparing `backtrader_binance-1.0.4/README.md` & `backtrader_binance-1.0.5/backtrader_binance.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,267 +1,301 @@
-# backtrader_binance
-Binance API integration with [Backtrader](https://github.com/WISEPLAT/backtrader).
-
-With this integration you can do:
- - Backtesting your strategy on historical data from the exchange [Binance](https://www.binance.com/?ref=CPA_004RZBKQWK ) + [Backtrader](https://github.com/WISEPLAT/backtrader )  // Backtesting 
- - Launch trading systems for automatic trading on the exchange [Binance](https://www.binance.com/?ref=CPA_004RZBKQWK) + [Backtrader](https://github.com/WISEPLAT/backtrader ) // Live trading
- - Download historical data for cryptocurrencies from the exchange [Binance](https://www.binance.com/?ref=CPA_004RZBKQWK)
-
-For API connection we are using library [python-binance](https://github.com/sammchardy/python-binance).
-
-## Installation
-1) The simplest way:
-```shell
-pip install backtrader_binance
-```
-or
-```shell
-git clone https://github.com/WISEPLAT/backtrader_binance
-```
-or
-```shell
-pip install git+https://github.com/WISEPLAT/backtrader_binance.git
-```
-
-2) Please use backtrader from my repository (as your can push your commits in it). Install it:
-```shell
-pip install git+https://github.com/WISEPLAT/backtrader.git
-```
--- Can I use your binance interface with original backtrader?
-
--- Yes, you can use original backtrader, as the author of original backtrader had approved all my changes. 
-
-Here is the link: [mementum/backtrader#472](https://github.com/mementum/backtrader/pull/472)
-
-3) We have some dependencies, you need to install them: 
-```shell
-pip install python-binance pandas matplotlib
-```
-
-### Getting started
-To make it easier to figure out how everything works, many examples have been made in the folders **DataExamplesBinance** and **StrategyExamplesBinance**.
-
-Before running the example, you need to get your API key and Secret key, and put them in the file **ConfigBinance\Config.py:**
-
-```python
-# content of ConfigBinance\Config.py 
-class Config:
-    BINANCE_API_KEY = "YOUR_API_KEY"
-    BINANCE_API_SECRET = "YOUR_SECRET_KEY"
-```
-
-#### How to get a Binance API token:
-1. Register your account on [Binance](https://www.binance.com/?ref=CPA_004RZBKQWK )
-2. Go to the ["API Management"](https://www.binance.com/en/my/settings/api-management?ref=CPA_004RZBKQWK ) 
-3. Then click the "Create API" button and select "System Generated".
-4. In the "API Restrictions" section, enable "Enable Spot and Margin Trading".
-5. Copy and paste to the file **ConfigBinance\Config.py ** received **"API key"** and **"Secret key"**
-
-#### Now you can run examples
-
-The **DataExamplesBinance** folder contains the code of examples for working with exchange data via the [Binance](https://www.binance.com/?ref=CPA_004RZBKQWK ) API.
-
-* **01 - Symbol.py** - trading strategy for obtaining historical and "live" data of one ticker for one timeframe
-* **02 - Symbol data to DF.py** - export to csv file of historical data of one ticker for one timeframe
-* **03 - Symbols.py** - trading strategy for multiple tickers on the same timeframe
-* **04 - Resample.py** - trading strategy for obtaining data from one ticker for different timeframes by converting a smaller timeframe into a larger one
-* **05 - Replay.py** - launching a trading strategy on a smaller timeframe, with processing on a larger one and displaying a larger interval chart
-* **06 - Rollover.py** - launch of a trading strategy based on gluing data from a file with historical data and the last downloaded history from the broker
-* **07 - Get Asset Balance.py** - getting the ticker balance directly through the Binance API
-* **08 - Timeframes.py** - trading strategy for one ticker on different timeframes
-* **Strategy.py** - An example of a trading strategy that only outputs data of the OHLCV for ticker/tickers
-
-The **StrategyExamplesBinance** folder contains the code of sample strategies.
-
-* **01 - Live Trade.py** - An example of a live trading strategy for two BTC and ETH tickers on the base USDT ticker.
-  * The strategy shows how to apply indicators (SMA, RSI) to several tickers at the same time.
-  * Example of placing and cancel orders on the Binance exchange.
-    * Please be aware! This is Live order - if market has a big change down in value of price more than 5% - the order will be completed.... 
-    * **Do not forget to cancel the submitted orders from the exchange after the test!**
-* **02 - Live Trade MultiPortfolio.py** - An example of a live trading strategy for a set of tickers that can be transferred to the strategy in a list (BTC, ETH, BNB) on the base USDT ticker.
-  * The strategy shows how to apply indicators (SMA, RSI) to several tickers at the same time.
-  * Example of placing and cancel orders on the Binance exchange.
-    * Please be aware! This is Live order - if market has a big change down in value of price more than 5% - the order will be completed.... 
-    * **Do not forget to cancel the submitted orders from the exchange after the test!**
-* **03 - Live Trade ETH.py** - An example of a live trading strategy for two BNB and XMR tickers on the basic ETH ticker.
-  * The strategy shows how to apply indicators (SMA, RSI) to several tickers at the same time.
-  * Example of placing and cancel orders on the Binance exchange.
-    * Please be aware! This is Live order - if market has a big change down in value of price more than 5% - the order will be completed.... 
-    * **Do not forget to cancel the submitted orders from the exchange after the test!**
-* **04 - Offline Backtest.py** - An example of a trading strategy on a historical data - not live mode - for two BTC and ETH tickers on the base USDT ticker.
-  * The strategy shows how to apply indicators (SMA, RSI) to several tickers at the same time.
-    * Not a live mode - for testing strategies without sending orders to the exchange!
-* **05 - Offline Backtest MultiPortfolio.py** - An example of a trading strategy on a historical data - not live mode - for a set of tickers that can be transferred to the strategy in a list (BTC, ETH, BNB) on the base USDT ticker.
-  * The strategy shows how to apply indicators (SMA, RSI) to several tickers at the same time.
-    * Not a live mode - for testing strategies without sending orders to the exchange!
-* **06 - Live Trade Just Buy and Close by Market.py** - An example of a live trading strategy for ETH ticker on the base USDT ticker.
-  * The strategy shows how to buy by close price and sell by market a little value of ETH after 3 bars.
-  * Example of placing orders on the Binance exchange.
-    * **Do not forget to cancel the submitted orders from the exchange after the test!**
-* **07 - Offline Backtest Indicators.py** - An example of a trading strategy for a history test using SMA and RSI indicators - not live mode - for two BTC and ETH tickers on the base USDT ticker.
-  * The strategy shows how to apply indicators (SMA, RSI) to several tickers at the same time.
-    * generates 177% of revenue at the time of video recording))
-    * Non-live mode - for testing strategies without sending orders to the exchange!
-
-## Thanks
-- backtrader: Very simple and cool library!
-- [python-binance](https://github.com/sammchardy/python-binance): For creating Binance API wrapper, shortening a lot of work.
-- lindomar-oliveira for some code
-
-## License
-[MIT](https://choosealicense.com/licenses/mit)
-
-## Important
-Error correction, revision and development of the library is carried out by the author and the community!
-
-**Push your commits!**
-
-## Terms of Use
-The backtrader_binance library, which allows you to integrate Backtrader and Binance API, is the **Program** created solely for the convenience of work.
-When using the **Program**, the User is obliged to comply with the provisions of the current legislation of his country.
-Using the **Program** are offered on an "AS IS" basis. No guarantees, either oral or written, are attached and are not provided.
-The author and the community does not guarantee that all errors of the **Program** have been eliminated, respectively, the author and the community do not bear any responsibility for
-the consequences of using the **Program**, including, but not limited to, any damage to equipment, computers, mobile devices,
-User software caused by or related to the use of the **Program**, as well as for any financial losses
-incurred by the User as a result of using the **Program**.
-No one is responsible for data loss, losses, damages, including accidental or indirect, lost profits, loss of revenue or any other losses
-related to the use of the **Program**.
-
-The **Program** is distributed under the terms of the [MIT](https://choosealicense.com/licenses/mit ) license.
-
-## Star History
-
-Please put a Star 🌟 for this code
-
-[![Star History Chart](https://api.star-history.com/svg?repos=WISEPLAT/backtrader_binance&type=Timeline)](https://star-history.com/#WISEPLAT/backtrader_binance&Timeline)
-
-Пожалуйста поставьте Звезду 🌟 этому коду
-
-==========================================================================
-
-# backtrader_binance
-
-Интеграция Binance API с [Backtrader](https://github.com/WISEPLAT/backtrader ).
-
-С помощью этой интеграции вы можете делать:
-- Тестирование вашей стратегии на исторических данных с биржи [Binance](https://www.binance.com/?ref=CPA_004RZBKQWK ) + [Backtrader](https://github.com/WISEPLAT/backtrader )
-- Запускать торговые системы для автоматической торговли на бирже [Binance](https://www.binance.com/?ref=CPA_004RZBKQWK ) + [Backtrader](https://github.com/WISEPLAT/backtrader ) 
-- Загружать исторические данные по криптовалютам с биржи [Binance](https://www.binance.com/?ref=CPA_004RZBKQWK )
-
-Для подключения к API мы используем библиотеку [python-binance](https://github.com/sammchardy/python-binance ).
-
-
-## Установка
-1) Самый простой способ:
-```shell
-pip install backtrader_binance
-```
-или
-```shell
-git clone https://github.com/WISEPLAT/backtrader_binance
-```
-или
-```shell
-pip install git+https://github.com/WISEPLAT/backtrader_binance.git
-```
-
-2) Пожалуйста, используйте backtrader из моего репозитория (так как вы можете размещать в нем свои коммиты). Установите его:
-```shell
-pip install git+https://github.com/WISEPLAT/backtrader.git
-```
--- Могу ли я использовать ваш интерфейс binance с оригинальным backtrader?
-
--- Да, вы можете использовать оригинальный backtrader, так как автор оригинального backtrader одобрил все мои изменения.
-
-Вот ссылка: [mementum/backtrader#472](https://github.com/mementum/backtrader/pull/472)
-
-3) У нас есть некоторые зависимости, вам нужно их установить:
-```shell
-pip install python-binance pandas matplotlib
-```
-
-### Начало работы
-Чтобы было легче разобраться как всё работает, сделано множество примеров в папках **DataExamplesBinance_ru** и **StrategyExamplesBinance_ru**.
-
-Перед запуском примера, необходимо получить свой API ключ и Secret ключ, и прописать их в файле **ConfigBinance\Config.py:**
-
-```python
-# content of ConfigBinance\Config.py 
-class Config:
-    BINANCE_API_KEY = "YOUR_API_KEY"
-    BINANCE_API_SECRET = "YOUR_SECRET_KEY"
-```
-
-####  Как получить токен Binance API:
-1. Зарегистрируйте свой аккаунт на [Binance](https://www.binance.com/?ref=CPA_004RZBKQWK )
-2. Перейдите в раздел ["Управление API"](https://www.binance.com/en/my/settings/api-management?ref=CPA_004RZBKQWK )
-3. Затем нажмите кнопку "Создать API" и выберите "Сгенерированный системой".
-4. В разделе "Ограничения API" включите "Включить спотовую и маржинальную торговлю".
-5. Скопируйте и вставьте в файл **ConfigBinance\Config.py** полученные **"Ключ API"** и **"Секретный ключ"**
-
-#### Теперь можно запускать примеры
-
-В папке **DataExamplesBinance_ru** находится код примеров по работе с биржевыми данными через API интерфейс [Binance](https://www.binance.com/?ref=CPA_004RZBKQWK ).
-
-* **01 - Symbol.py** - торговая стратегия для получения исторических и "живых" данных одного тикера по одному таймфрейму
-* **02 - Symbol data to DF.py** - экспорт в csv файл исторических данных одного тикера по одному таймфрейму
-* **03 - Symbols.py** - торговая стратегия для нескольких тикеров по одному таймфрейму
-* **04 - Resample.py** - торговая стратегия для получения данных одного тикера по разным таймфреймам методом конвертации меньшего таймфрейма в больший
-* **05 - Replay.py** - запуск торговой стратегии на меньшем таймфрейме, с обработкой на большем и выводом графика большего интервала
-* **06 - Rollover.py** - запуск торговой стратегии на склейке данных из файла с историческими данными и последней загруженной истории с брокера
-* **07 - Get Asset Balance.py** - получение баланса тикера напрямую через API Binance
-* **08 - Timeframes.py** - торговая стратегия для одного тикера по разным таймфреймам
-* **Strategy.py** - Пример торговой стратегии, которая только выводит данные по тикеру/тикерам OHLCV
-
-В папке **StrategyExamplesBinance_ru** находится код примеров стратегий.  
-
-* **01 - Live Trade.py** - Пример торговой стратегии в live режиме для двух тикеров BTC и ETH на базовом тикере USDT. 
-  * В стратегии показано как применять индикаторы (SMA, RSI) к нескольким тикерам одновременно. 
-  * Пример выставления заявок на биржу Binance и их снятие.
-    * Пожалуйста, имейте в виду! Это live режим - если на рынке произойдет значительное изменение цены в сторону понижения более чем на 5% - ордер может быть выполнен.... 
-    * **Не забудьте после теста снять с биржи выставленные заявки!**
-* **02 - Live Trade MultiPortfolio.py** - Пример торговой стратегии в live режиме для множества тикеров, которые можно передавать в стратегию списком (BTC, ETH, BNB) на базовом тикере USDT. 
-  * В стратегии показано как применять индикаторы (SMA, RSI) к нескольким тикерам одновременно. 
-  * Пример выставления заявок на биржу Binance и их снятие.
-    * Пожалуйста, имейте в виду! Это live режим - если на рынке произойдет значительное изменение цены в сторону понижения более чем на 5% - ордер может быть выполнен....
-    * **Не забудьте после теста снять с биржи выставленные заявки!**
-* **03 - Live Trade ETH.py** - Пример торговой стратегии в live режиме для двух тикеров BNB и XMR на базовом тикере ETH. 
-  * В стратегии показано как применять индикаторы (SMA, RSI) к нескольким тикерам одновременно. 
-  * Пример выставления заявок на биржу Binance и их снятие.
-    * Пожалуйста, имейте в виду! Это live режим - если на рынке произойдет значительное изменение цены в сторону понижения более чем на 5% - ордер может быть выполнен....
-    * **Не забудьте после теста снять с биржи выставленные заявки!**
-* **04 - Offline Backtest.py** - Пример торговой стратегии для теста на истории - не live режим - для двух тикеров BTC и ETH на базовом тикере USDT. 
-  * В стратегии показано как применять индикаторы (SMA, RSI) к нескольким тикерам одновременно.
-    * Не live режим - для тестирования стратегий без отправки заявок на биржу!
-* **05 - Offline Backtest MultiPortfolio.py** - Пример торговой стратегии для теста на истории - не live режим - для множества тикеров, которые можно передавать в стратегию списком (BTC, ETH, BNB) на базовом тикере USDT. 
-  * В стратегии показано как применять индикаторы (SMA, RSI) к нескольким тикерам одновременно.
-    * Не live режим - для тестирования стратегий без отправки заявок на биржу!
-* **06 - Live Trade Just Buy and Close by Market.py** - Пример торговой стратегии в live для тикера ETH на базовом тикере USDT.
-  * Стратегия показывает, как покупать по цене закрытия и продавать по рыночной небольшое количество ETH через 3 бара.
-  * Пример размещения ордеров на бирже Binance.
-    * **Не забудьте отменить выставленные ордера с биржи после тестирования!**
-* **07 - Offline Backtest Indicators.py** - Пример торговой стратегии для теста на истории с использованием индикаторов SMA и RSI - не live режим - для двух тикеров BTC и ETH на базовом тикере USDT. 
-  * В стратегии показано как применять индикаторы (SMA, RSI) к нескольким тикерам одновременно.
-    * генерит 177% дохода на момент записи видео )) 
-    * Не live режим - для тестирования стратегий без отправки заявок на биржу!
-## Спасибо
-- backtrader: очень простая и классная библиотека!
-- [python-binance](https://github.com/sammchardy/python-binance ): Для создания оболочки Binance API, сокращающей большую часть работы.
-- lindomar-oliveira за некоторый код
-
-## Важно
-Исправление ошибок, доработка и развитие библиотеки осуществляется автором и сообществом!
-
-**Пушьте ваши коммиты!** 
-
-# Условия использования
-Библиотека backtrader_binance позволяющая делать интеграцию Backtrader и Binance API - это **Программа** созданная исключительно для удобства работы.
-При использовании **Программы** Пользователь обязан соблюдать положения действующего законодательства Российской Федерации или своей страны.
-Использование **Программы** предлагается по принципу «Как есть» («AS IS»). Никаких гарантий, как устных, так и письменных не прилагается и не предусматривается.
-Автор и сообщество не дает гарантии, что все ошибки **Программы** были устранены, соответственно автор и сообщество не несет никакой ответственности за
-последствия использования **Программы**, включая, но, не ограничиваясь любым ущербом оборудованию, компьютерам, мобильным устройствам, 
-программному обеспечению Пользователя вызванным или связанным с использованием **Программы**, а также за любые финансовые потери,
-понесенные Пользователем в результате использования **Программы**.
-Никто не ответственен за потерю данных, убытки, ущерб, включаю случайный или косвенный, упущенную выгоду, потерю доходов или любые другие потери,
-связанные с использованием **Программы**.
-
-**Программа** распространяется на условиях лицензии [MIT](https://choosealicense.com/licenses/mit).
+Metadata-Version: 2.1
+Name: backtrader-binance
+Version: 1.0.5
+Summary: Binance API integration with Backtrader
+Home-page: https://github.com/WISEPLAT/backtrader_binance
+Author: wiseplat
+Author-email: oshpagin@gmail.com
+License: MIT License
+Project-URL: Documentation, https://github.com/WISEPLAT/backtrader_binance/blob/master/README.md
+Keywords: trading,development
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Financial and Insurance Industry
+Classifier: Topic :: Software Development
+Classifier: Topic :: Office/Business :: Financial
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# backtrader_binance
+Binance API integration with [Backtrader](https://github.com/WISEPLAT/backtrader).
+
+With this integration you can do:
+ - Backtesting your strategy on historical data from the exchange [Binance](https://www.binance.com/?ref=CPA_004RZBKQWK ) + [Backtrader](https://github.com/WISEPLAT/backtrader )  // Backtesting 
+ - Launch trading systems for automatic trading on the exchange [Binance](https://www.binance.com/?ref=CPA_004RZBKQWK) + [Backtrader](https://github.com/WISEPLAT/backtrader ) // Live trading
+ - Download historical data for cryptocurrencies from the exchange [Binance](https://www.binance.com/?ref=CPA_004RZBKQWK)
+
+For API connection we are using library [python-binance](https://github.com/sammchardy/python-binance).
+
+## Installation
+1) The simplest way:
+```shell
+pip install backtrader_binance
+```
+or
+```shell
+git clone https://github.com/WISEPLAT/backtrader_binance
+```
+or
+```shell
+pip install git+https://github.com/WISEPLAT/backtrader_binance.git
+```
+
+2) Please use backtrader from my repository (as your can push your commits in it). Install it:
+```shell
+pip install git+https://github.com/WISEPLAT/backtrader.git
+```
+-- Can I use your binance interface with original backtrader?
+
+-- Yes, you can use original backtrader, as the author of original backtrader had approved all my changes. 
+
+Here is the link: [mementum/backtrader#472](https://github.com/mementum/backtrader/pull/472)
+
+3) We have some dependencies, you need to install them: 
+```shell
+pip install python-binance pandas matplotlib
+```
+
+### Getting started
+To make it easier to figure out how everything works, many examples have been made in the folders **DataExamplesBinance** and **StrategyExamplesBinance**.
+
+Before running the example, you need to get your API key and Secret key, and put them in the file **ConfigBinance\Config.py:**
+
+```python
+# content of ConfigBinance\Config.py 
+class Config:
+    BINANCE_API_KEY = "YOUR_API_KEY"
+    BINANCE_API_SECRET = "YOUR_SECRET_KEY"
+```
+
+#### How to get a Binance API token:
+1. Register your account on [Binance](https://www.binance.com/?ref=CPA_004RZBKQWK )
+2. Go to the ["API Management"](https://www.binance.com/en/my/settings/api-management?ref=CPA_004RZBKQWK ) 
+3. Then click the "Create API" button and select "System Generated".
+4. In the "API Restrictions" section, enable "Enable Spot and Margin Trading".
+5. Copy and paste to the file **ConfigBinance\Config.py ** received **"API key"** and **"Secret key"**
+
+#### Now you can run examples
+
+The **DataExamplesBinance** folder contains the code of examples for working with exchange data via the [Binance](https://www.binance.com/?ref=CPA_004RZBKQWK ) API.
+
+* **01 - Symbol.py** - trading strategy for obtaining historical and "live" data of one ticker for one timeframe
+* **02 - Symbol data to DF.py** - export to csv file of historical data of one ticker for one timeframe
+* **03 - Symbols.py** - trading strategy for multiple tickers on the same timeframe
+* **04 - Resample.py** - trading strategy for obtaining data from one ticker for different timeframes by converting a smaller timeframe into a larger one
+* **05 - Replay.py** - launching a trading strategy on a smaller timeframe, with processing on a larger one and displaying a larger interval chart
+* **06 - Rollover.py** - launch of a trading strategy based on gluing data from a file with historical data and the last downloaded history from the broker
+* **07 - Get Asset Balance.py** - getting the ticker balance directly through the Binance API
+* **08 - Timeframes.py** - trading strategy is running on different timeframes.
+* **09 - Get Asset Info.py** - getting info about asset: balance, lot size, min price step, min value to buy and etc.
+* **09 - Get Asset Info - no Decimal.py** - getting info about asset: balance, lot size, min price step, min value to buy and etc.
+* **09 - Get Asset Info - through client.py** - getting info about asset: balance, lot size, min price step, min value to buy and etc.
+* **10 - Get Historical Data.py** - getting historical data through binance client for asset.
+* **Strategy.py** - An example of a trading strategy that only outputs data of the OHLCV for ticker/tickers
+
+The **StrategyExamplesBinance** folder contains the code of sample strategies.
+
+* **01 - Live Trade.py** - An example of a live trading strategy for two BTC and ETH tickers on the base USDT ticker.
+  * The strategy shows how to apply indicators (SMA, RSI) to several tickers at the same time.
+  * Example of placing and cancel orders on the Binance exchange.
+    * Please be aware! This is Live order - if market has a big change down in value of price more than 5% - the order will be completed.... 
+    * **Do not forget to cancel the submitted orders from the exchange after the test!**
+* **02 - Live Trade MultiPortfolio.py** - An example of a live trading strategy for a set of tickers that can be transferred to the strategy in a list (BTC, ETH, BNB) on the base USDT ticker.
+  * The strategy shows how to apply indicators (SMA, RSI) to several tickers at the same time.
+  * Example of placing and cancel orders on the Binance exchange.
+    * Please be aware! This is Live order - if market has a big change down in value of price more than 5% - the order will be completed.... 
+    * **Do not forget to cancel the submitted orders from the exchange after the test!**
+* **03 - Live Trade ETH.py** - An example of a live trading strategy for two BNB and XMR tickers on the basic ETH ticker.
+  * The strategy shows how to apply indicators (SMA, RSI) to several tickers at the same time.
+  * Example of placing and cancel orders on the Binance exchange.
+    * Please be aware! This is Live order - if market has a big change down in value of price more than 5% - the order will be completed.... 
+    * **Do not forget to cancel the submitted orders from the exchange after the test!**
+* **04 - Offline Backtest.py** - An example of a trading strategy on a historical data - not live mode - for two BTC and ETH tickers on the base USDT ticker.
+  * The strategy shows how to apply indicators (SMA, RSI) to several tickers at the same time.
+    * Not a live mode - for testing strategies without sending orders to the exchange!
+* **05 - Offline Backtest MultiPortfolio.py** - An example of a trading strategy on a historical data - not live mode - for a set of tickers that can be transferred to the strategy in a list (BTC, ETH, BNB) on the base USDT ticker.
+  * The strategy shows how to apply indicators (SMA, RSI) to several tickers at the same time.
+    * Not a live mode - for testing strategies without sending orders to the exchange!
+* **06 - Live Trade Just Buy and Close by Market.py** - An example of a live trading strategy for ETH ticker on the base USDT ticker.
+  * The strategy shows how to buy by close price and sell by market a little value of ETH after 3 bars.
+  * Example of placing orders on the Binance exchange.
+    * **Do not forget to cancel the submitted orders from the exchange after the test!**
+* **07 - Offline Backtest Indicators.py** - An example of a trading strategy for a history test using SMA and RSI indicators - not live mode - for two BTC and ETH tickers on the base USDT ticker.
+  * The strategy shows how to apply indicators (SMA, RSI) to several tickers at the same time.
+    * generates 177% of revenue at the time of video recording))
+    * Non-live mode - for testing strategies without sending orders to the exchange!
+
+## Thanks
+- backtrader: Very simple and cool library!
+- [python-binance](https://github.com/sammchardy/python-binance): For creating Binance API wrapper, shortening a lot of work.
+- lindomar-oliveira for some code
+
+## License
+[MIT](https://choosealicense.com/licenses/mit)
+
+## Important
+Error correction, revision and development of the library is carried out by the author and the community!
+
+**Push your commits!**
+
+## Terms of Use
+The backtrader_binance library, which allows you to integrate Backtrader and Binance API, is the **Program** created solely for the convenience of work.
+When using the **Program**, the User is obliged to comply with the provisions of the current legislation of his country.
+Using the **Program** are offered on an "AS IS" basis. No guarantees, either oral or written, are attached and are not provided.
+The author and the community does not guarantee that all errors of the **Program** have been eliminated, respectively, the author and the community do not bear any responsibility for
+the consequences of using the **Program**, including, but not limited to, any damage to equipment, computers, mobile devices,
+User software caused by or related to the use of the **Program**, as well as for any financial losses
+incurred by the User as a result of using the **Program**.
+No one is responsible for data loss, losses, damages, including accidental or indirect, lost profits, loss of revenue or any other losses
+related to the use of the **Program**.
+
+The **Program** is distributed under the terms of the [MIT](https://choosealicense.com/licenses/mit ) license.
+
+## Star History
+
+Please put a Star 🌟 for this code
+
+[![Star History Chart](https://api.star-history.com/svg?repos=WISEPLAT/backtrader_binance&type=Timeline)](https://star-history.com/#WISEPLAT/backtrader_binance&Timeline)
+
+Пожалуйста поставьте Звезду 🌟 этому коду
+
+==========================================================================
+
+# backtrader_binance
+
+Интеграция Binance API с [Backtrader](https://github.com/WISEPLAT/backtrader ).
+
+С помощью этой интеграции вы можете делать:
+- Тестирование вашей стратегии на исторических данных с биржи [Binance](https://www.binance.com/?ref=CPA_004RZBKQWK ) + [Backtrader](https://github.com/WISEPLAT/backtrader )
+- Запускать торговые системы для автоматической торговли на бирже [Binance](https://www.binance.com/?ref=CPA_004RZBKQWK ) + [Backtrader](https://github.com/WISEPLAT/backtrader ) 
+- Загружать исторические данные по криптовалютам с биржи [Binance](https://www.binance.com/?ref=CPA_004RZBKQWK )
+
+Для подключения к API мы используем библиотеку [python-binance](https://github.com/sammchardy/python-binance ).
+
+
+## Установка
+1) Самый простой способ:
+```shell
+pip install backtrader_binance
+```
+или
+```shell
+git clone https://github.com/WISEPLAT/backtrader_binance
+```
+или
+```shell
+pip install git+https://github.com/WISEPLAT/backtrader_binance.git
+```
+
+2) Пожалуйста, используйте backtrader из моего репозитория (так как вы можете размещать в нем свои коммиты). Установите его:
+```shell
+pip install git+https://github.com/WISEPLAT/backtrader.git
+```
+-- Могу ли я использовать ваш интерфейс binance с оригинальным backtrader?
+
+-- Да, вы можете использовать оригинальный backtrader, так как автор оригинального backtrader одобрил все мои изменения.
+
+Вот ссылка: [mementum/backtrader#472](https://github.com/mementum/backtrader/pull/472)
+
+3) У нас есть некоторые зависимости, вам нужно их установить:
+```shell
+pip install python-binance pandas matplotlib
+```
+
+### Начало работы
+Чтобы было легче разобраться как всё работает, сделано множество примеров в папках **DataExamplesBinance_ru** и **StrategyExamplesBinance_ru**.
+
+Перед запуском примера, необходимо получить свой API ключ и Secret ключ, и прописать их в файле **ConfigBinance\Config.py:**
+
+```python
+# content of ConfigBinance\Config.py 
+class Config:
+    BINANCE_API_KEY = "YOUR_API_KEY"
+    BINANCE_API_SECRET = "YOUR_SECRET_KEY"
+```
+
+####  Как получить токен Binance API:
+1. Зарегистрируйте свой аккаунт на [Binance](https://www.binance.com/?ref=CPA_004RZBKQWK )
+2. Перейдите в раздел ["Управление API"](https://www.binance.com/en/my/settings/api-management?ref=CPA_004RZBKQWK )
+3. Затем нажмите кнопку "Создать API" и выберите "Сгенерированный системой".
+4. В разделе "Ограничения API" включите "Включить спотовую и маржинальную торговлю".
+5. Скопируйте и вставьте в файл **ConfigBinance\Config.py** полученные **"Ключ API"** и **"Секретный ключ"**
+
+#### Теперь можно запускать примеры
+
+В папке **DataExamplesBinance_ru** находится код примеров по работе с биржевыми данными через API интерфейс [Binance](https://www.binance.com/?ref=CPA_004RZBKQWK ).
+
+* **01 - Symbol.py** - торговая стратегия для получения исторических и "живых" данных одного тикера по одному таймфрейму
+* **02 - Symbol data to DF.py** - экспорт в csv файл исторических данных одного тикера по одному таймфрейму
+* **03 - Symbols.py** - торговая стратегия для нескольких тикеров по одному таймфрейму
+* **04 - Resample.py** - торговая стратегия для получения данных одного тикера по разным таймфреймам методом конвертации меньшего таймфрейма в больший
+* **05 - Replay.py** - запуск торговой стратегии на меньшем таймфрейме, с обработкой на большем и выводом графика большего интервала
+* **06 - Rollover.py** - запуск торговой стратегии на склейке данных из файла с историческими данными и последней загруженной истории с брокера
+* **07 - Get Asset Balance.py** - получение баланса тикера напрямую через API Binance
+* **08 - Timeframes.py** - торговая стратегия для одного тикера по разным таймфреймам
+* **Strategy.py** - Пример торговой стратегии, которая только выводит данные по тикеру/тикерам OHLCV
+
+В папке **StrategyExamplesBinance_ru** находится код примеров стратегий.  
+
+* **01 - Live Trade.py** - Пример торговой стратегии в live режиме для двух тикеров BTC и ETH на базовом тикере USDT. 
+  * В стратегии показано как применять индикаторы (SMA, RSI) к нескольким тикерам одновременно. 
+  * Пример выставления заявок на биржу Binance и их снятие.
+    * Пожалуйста, имейте в виду! Это live режим - если на рынке произойдет значительное изменение цены в сторону понижения более чем на 5% - ордер может быть выполнен.... 
+    * **Не забудьте после теста снять с биржи выставленные заявки!**
+* **02 - Live Trade MultiPortfolio.py** - Пример торговой стратегии в live режиме для множества тикеров, которые можно передавать в стратегию списком (BTC, ETH, BNB) на базовом тикере USDT. 
+  * В стратегии показано как применять индикаторы (SMA, RSI) к нескольким тикерам одновременно. 
+  * Пример выставления заявок на биржу Binance и их снятие.
+    * Пожалуйста, имейте в виду! Это live режим - если на рынке произойдет значительное изменение цены в сторону понижения более чем на 5% - ордер может быть выполнен....
+    * **Не забудьте после теста снять с биржи выставленные заявки!**
+* **03 - Live Trade ETH.py** - Пример торговой стратегии в live режиме для двух тикеров BNB и XMR на базовом тикере ETH. 
+  * В стратегии показано как применять индикаторы (SMA, RSI) к нескольким тикерам одновременно. 
+  * Пример выставления заявок на биржу Binance и их снятие.
+    * Пожалуйста, имейте в виду! Это live режим - если на рынке произойдет значительное изменение цены в сторону понижения более чем на 5% - ордер может быть выполнен....
+    * **Не забудьте после теста снять с биржи выставленные заявки!**
+* **04 - Offline Backtest.py** - Пример торговой стратегии для теста на истории - не live режим - для двух тикеров BTC и ETH на базовом тикере USDT. 
+  * В стратегии показано как применять индикаторы (SMA, RSI) к нескольким тикерам одновременно.
+    * Не live режим - для тестирования стратегий без отправки заявок на биржу!
+* **05 - Offline Backtest MultiPortfolio.py** - Пример торговой стратегии для теста на истории - не live режим - для множества тикеров, которые можно передавать в стратегию списком (BTC, ETH, BNB) на базовом тикере USDT. 
+  * В стратегии показано как применять индикаторы (SMA, RSI) к нескольким тикерам одновременно.
+    * Не live режим - для тестирования стратегий без отправки заявок на биржу!
+* **06 - Live Trade Just Buy and Close by Market.py** - Пример торговой стратегии в live для тикера ETH на базовом тикере USDT.
+  * Стратегия показывает, как покупать по цене закрытия и продавать по рыночной небольшое количество ETH через 3 бара.
+  * Пример размещения ордеров на бирже Binance.
+    * **Не забудьте отменить выставленные ордера с биржи после тестирования!**
+* **07 - Offline Backtest Indicators.py** - Пример торговой стратегии для теста на истории с использованием индикаторов SMA и RSI - не live режим - для двух тикеров BTC и ETH на базовом тикере USDT. 
+  * В стратегии показано как применять индикаторы (SMA, RSI) к нескольким тикерам одновременно.
+    * генерит 177% дохода на момент записи видео )) 
+    * Не live режим - для тестирования стратегий без отправки заявок на биржу!
+* **08 - Timeframes.py** - торговая стратегия работает на разных таймфреймах.
+* **09 - Get Asset Info.py* - получение информации об активе: баланс, размер лота, минимальный шаг цены, минимальная стоимость покупки и т.д.
+* **09 - Get Asset Info - no Decimal.py** - получение информации об активе: баланс, размер лота, минимальный шаг цены, минимальная стоимость покупки и т.д.
+* **09 - Get Asset Info - through client.py** - получение информации об активе: баланс, размер лота, минимальный шаг цены, минимальная стоимость покупки и т.д.
+* **10 - Get Historical Data.py** - получение исторических данных через клиент binance для актива.
+
+## Спасибо
+- backtrader: очень простая и классная библиотека!
+- [python-binance](https://github.com/sammchardy/python-binance ): Для создания оболочки Binance API, сокращающей большую часть работы.
+- lindomar-oliveira за некоторый код
+
+## Важно
+Исправление ошибок, доработка и развитие библиотеки осуществляется автором и сообществом!
+
+**Пушьте ваши коммиты!** 
+
+# Условия использования
+Библиотека backtrader_binance позволяющая делать интеграцию Backtrader и Binance API - это **Программа** созданная исключительно для удобства работы.
+При использовании **Программы** Пользователь обязан соблюдать положения действующего законодательства Российской Федерации или своей страны.
+Использование **Программы** предлагается по принципу «Как есть» («AS IS»). Никаких гарантий, как устных, так и письменных не прилагается и не предусматривается.
+Автор и сообщество не дает гарантии, что все ошибки **Программы** были устранены, соответственно автор и сообщество не несет никакой ответственности за
+последствия использования **Программы**, включая, но, не ограничиваясь любым ущербом оборудованию, компьютерам, мобильным устройствам, 
+программному обеспечению Пользователя вызванным или связанным с использованием **Программы**, а также за любые финансовые потери,
+понесенные Пользователем в результате использования **Программы**.
+Никто не ответственен за потерю данных, убытки, ущерб, включаю случайный или косвенный, упущенную выгоду, потерю доходов или любые другие потери,
+связанные с использованием **Программы**.
+
+**Программа** распространяется на условиях лицензии [MIT](https://choosealicense.com/licenses/mit).
```

### Comparing `backtrader_binance-1.0.4/backtrader_binance/binance_broker.py` & `backtrader_binance-1.0.5/backtrader_binance/binance_broker.py`

 * *Files identical despite different names*

### Comparing `backtrader_binance-1.0.4/backtrader_binance/binance_feed.py` & `backtrader_binance-1.0.5/backtrader_binance/binance_feed.py`

 * *Files identical despite different names*

### Comparing `backtrader_binance-1.0.4/backtrader_binance/binance_store.py` & `backtrader_binance-1.0.5/backtrader_binance/binance_store.py`

 * *Files identical despite different names*

### Comparing `backtrader_binance-1.0.4/backtrader_binance.egg-info/PKG-INFO` & `backtrader_binance-1.0.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,291 +1,277 @@
-Metadata-Version: 2.1
-Name: backtrader-binance
-Version: 1.0.4
-Summary: Binance API integration with Backtrader
-Home-page: https://github.com/WISEPLAT/backtrader_binance
-Author: wiseplat
-Author-email: oshpagin@gmail.com
-License: MIT License
-Project-URL: Documentation, https://github.com/WISEPLAT/backtrader_binance/blob/master/README.md
-Keywords: trading,development
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Financial and Insurance Industry
-Classifier: Topic :: Software Development
-Classifier: Topic :: Office/Business :: Financial
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# backtrader_binance
-Binance API integration with [Backtrader](https://github.com/WISEPLAT/backtrader).
-
-With this integration you can do:
- - Backtesting your strategy on historical data from the exchange [Binance](https://www.binance.com/?ref=CPA_004RZBKQWK ) + [Backtrader](https://github.com/WISEPLAT/backtrader )  // Backtesting 
- - Launch trading systems for automatic trading on the exchange [Binance](https://www.binance.com/?ref=CPA_004RZBKQWK) + [Backtrader](https://github.com/WISEPLAT/backtrader ) // Live trading
- - Download historical data for cryptocurrencies from the exchange [Binance](https://www.binance.com/?ref=CPA_004RZBKQWK)
-
-For API connection we are using library [python-binance](https://github.com/sammchardy/python-binance).
-
-## Installation
-1) The simplest way:
-```shell
-pip install backtrader_binance
-```
-or
-```shell
-git clone https://github.com/WISEPLAT/backtrader_binance
-```
-or
-```shell
-pip install git+https://github.com/WISEPLAT/backtrader_binance.git
-```
-
-2) Please use backtrader from my repository (as your can push your commits in it). Install it:
-```shell
-pip install git+https://github.com/WISEPLAT/backtrader.git
-```
--- Can I use your binance interface with original backtrader?
-
--- Yes, you can use original backtrader, as the author of original backtrader had approved all my changes. 
-
-Here is the link: [mementum/backtrader#472](https://github.com/mementum/backtrader/pull/472)
-
-3) We have some dependencies, you need to install them: 
-```shell
-pip install python-binance pandas matplotlib
-```
-
-### Getting started
-To make it easier to figure out how everything works, many examples have been made in the folders **DataExamplesBinance** and **StrategyExamplesBinance**.
-
-Before running the example, you need to get your API key and Secret key, and put them in the file **ConfigBinance\Config.py:**
-
-```python
-# content of ConfigBinance\Config.py 
-class Config:
-    BINANCE_API_KEY = "YOUR_API_KEY"
-    BINANCE_API_SECRET = "YOUR_SECRET_KEY"
-```
-
-#### How to get a Binance API token:
-1. Register your account on [Binance](https://www.binance.com/?ref=CPA_004RZBKQWK )
-2. Go to the ["API Management"](https://www.binance.com/en/my/settings/api-management?ref=CPA_004RZBKQWK ) 
-3. Then click the "Create API" button and select "System Generated".
-4. In the "API Restrictions" section, enable "Enable Spot and Margin Trading".
-5. Copy and paste to the file **ConfigBinance\Config.py ** received **"API key"** and **"Secret key"**
-
-#### Now you can run examples
-
-The **DataExamplesBinance** folder contains the code of examples for working with exchange data via the [Binance](https://www.binance.com/?ref=CPA_004RZBKQWK ) API.
-
-* **01 - Symbol.py** - trading strategy for obtaining historical and "live" data of one ticker for one timeframe
-* **02 - Symbol data to DF.py** - export to csv file of historical data of one ticker for one timeframe
-* **03 - Symbols.py** - trading strategy for multiple tickers on the same timeframe
-* **04 - Resample.py** - trading strategy for obtaining data from one ticker for different timeframes by converting a smaller timeframe into a larger one
-* **05 - Replay.py** - launching a trading strategy on a smaller timeframe, with processing on a larger one and displaying a larger interval chart
-* **06 - Rollover.py** - launch of a trading strategy based on gluing data from a file with historical data and the last downloaded history from the broker
-* **07 - Get Asset Balance.py** - getting the ticker balance directly through the Binance API
-* **08 - Timeframes.py** - trading strategy for one ticker on different timeframes
-* **Strategy.py** - An example of a trading strategy that only outputs data of the OHLCV for ticker/tickers
-
-The **StrategyExamplesBinance** folder contains the code of sample strategies.
-
-* **01 - Live Trade.py** - An example of a live trading strategy for two BTC and ETH tickers on the base USDT ticker.
-  * The strategy shows how to apply indicators (SMA, RSI) to several tickers at the same time.
-  * Example of placing and cancel orders on the Binance exchange.
-    * Please be aware! This is Live order - if market has a big change down in value of price more than 5% - the order will be completed.... 
-    * **Do not forget to cancel the submitted orders from the exchange after the test!**
-* **02 - Live Trade MultiPortfolio.py** - An example of a live trading strategy for a set of tickers that can be transferred to the strategy in a list (BTC, ETH, BNB) on the base USDT ticker.
-  * The strategy shows how to apply indicators (SMA, RSI) to several tickers at the same time.
-  * Example of placing and cancel orders on the Binance exchange.
-    * Please be aware! This is Live order - if market has a big change down in value of price more than 5% - the order will be completed.... 
-    * **Do not forget to cancel the submitted orders from the exchange after the test!**
-* **03 - Live Trade ETH.py** - An example of a live trading strategy for two BNB and XMR tickers on the basic ETH ticker.
-  * The strategy shows how to apply indicators (SMA, RSI) to several tickers at the same time.
-  * Example of placing and cancel orders on the Binance exchange.
-    * Please be aware! This is Live order - if market has a big change down in value of price more than 5% - the order will be completed.... 
-    * **Do not forget to cancel the submitted orders from the exchange after the test!**
-* **04 - Offline Backtest.py** - An example of a trading strategy on a historical data - not live mode - for two BTC and ETH tickers on the base USDT ticker.
-  * The strategy shows how to apply indicators (SMA, RSI) to several tickers at the same time.
-    * Not a live mode - for testing strategies without sending orders to the exchange!
-* **05 - Offline Backtest MultiPortfolio.py** - An example of a trading strategy on a historical data - not live mode - for a set of tickers that can be transferred to the strategy in a list (BTC, ETH, BNB) on the base USDT ticker.
-  * The strategy shows how to apply indicators (SMA, RSI) to several tickers at the same time.
-    * Not a live mode - for testing strategies without sending orders to the exchange!
-* **06 - Live Trade Just Buy and Close by Market.py** - An example of a live trading strategy for ETH ticker on the base USDT ticker.
-  * The strategy shows how to buy by close price and sell by market a little value of ETH after 3 bars.
-  * Example of placing orders on the Binance exchange.
-    * **Do not forget to cancel the submitted orders from the exchange after the test!**
-* **07 - Offline Backtest Indicators.py** - An example of a trading strategy for a history test using SMA and RSI indicators - not live mode - for two BTC and ETH tickers on the base USDT ticker.
-  * The strategy shows how to apply indicators (SMA, RSI) to several tickers at the same time.
-    * generates 177% of revenue at the time of video recording))
-    * Non-live mode - for testing strategies without sending orders to the exchange!
-
-## Thanks
-- backtrader: Very simple and cool library!
-- [python-binance](https://github.com/sammchardy/python-binance): For creating Binance API wrapper, shortening a lot of work.
-- lindomar-oliveira for some code
-
-## License
-[MIT](https://choosealicense.com/licenses/mit)
-
-## Important
-Error correction, revision and development of the library is carried out by the author and the community!
-
-**Push your commits!**
-
-## Terms of Use
-The backtrader_binance library, which allows you to integrate Backtrader and Binance API, is the **Program** created solely for the convenience of work.
-When using the **Program**, the User is obliged to comply with the provisions of the current legislation of his country.
-Using the **Program** are offered on an "AS IS" basis. No guarantees, either oral or written, are attached and are not provided.
-The author and the community does not guarantee that all errors of the **Program** have been eliminated, respectively, the author and the community do not bear any responsibility for
-the consequences of using the **Program**, including, but not limited to, any damage to equipment, computers, mobile devices,
-User software caused by or related to the use of the **Program**, as well as for any financial losses
-incurred by the User as a result of using the **Program**.
-No one is responsible for data loss, losses, damages, including accidental or indirect, lost profits, loss of revenue or any other losses
-related to the use of the **Program**.
-
-The **Program** is distributed under the terms of the [MIT](https://choosealicense.com/licenses/mit ) license.
-
-## Star History
-
-Please put a Star 🌟 for this code
-
-[![Star History Chart](https://api.star-history.com/svg?repos=WISEPLAT/backtrader_binance&type=Timeline)](https://star-history.com/#WISEPLAT/backtrader_binance&Timeline)
-
-Пожалуйста поставьте Звезду 🌟 этому коду
-
-==========================================================================
-
-# backtrader_binance
-
-Интеграция Binance API с [Backtrader](https://github.com/WISEPLAT/backtrader ).
-
-С помощью этой интеграции вы можете делать:
-- Тестирование вашей стратегии на исторических данных с биржи [Binance](https://www.binance.com/?ref=CPA_004RZBKQWK ) + [Backtrader](https://github.com/WISEPLAT/backtrader )
-- Запускать торговые системы для автоматической торговли на бирже [Binance](https://www.binance.com/?ref=CPA_004RZBKQWK ) + [Backtrader](https://github.com/WISEPLAT/backtrader ) 
-- Загружать исторические данные по криптовалютам с биржи [Binance](https://www.binance.com/?ref=CPA_004RZBKQWK )
-
-Для подключения к API мы используем библиотеку [python-binance](https://github.com/sammchardy/python-binance ).
-
-
-## Установка
-1) Самый простой способ:
-```shell
-pip install backtrader_binance
-```
-или
-```shell
-git clone https://github.com/WISEPLAT/backtrader_binance
-```
-или
-```shell
-pip install git+https://github.com/WISEPLAT/backtrader_binance.git
-```
-
-2) Пожалуйста, используйте backtrader из моего репозитория (так как вы можете размещать в нем свои коммиты). Установите его:
-```shell
-pip install git+https://github.com/WISEPLAT/backtrader.git
-```
--- Могу ли я использовать ваш интерфейс binance с оригинальным backtrader?
-
--- Да, вы можете использовать оригинальный backtrader, так как автор оригинального backtrader одобрил все мои изменения.
-
-Вот ссылка: [mementum/backtrader#472](https://github.com/mementum/backtrader/pull/472)
-
-3) У нас есть некоторые зависимости, вам нужно их установить:
-```shell
-pip install python-binance pandas matplotlib
-```
-
-### Начало работы
-Чтобы было легче разобраться как всё работает, сделано множество примеров в папках **DataExamplesBinance_ru** и **StrategyExamplesBinance_ru**.
-
-Перед запуском примера, необходимо получить свой API ключ и Secret ключ, и прописать их в файле **ConfigBinance\Config.py:**
-
-```python
-# content of ConfigBinance\Config.py 
-class Config:
-    BINANCE_API_KEY = "YOUR_API_KEY"
-    BINANCE_API_SECRET = "YOUR_SECRET_KEY"
-```
-
-####  Как получить токен Binance API:
-1. Зарегистрируйте свой аккаунт на [Binance](https://www.binance.com/?ref=CPA_004RZBKQWK )
-2. Перейдите в раздел ["Управление API"](https://www.binance.com/en/my/settings/api-management?ref=CPA_004RZBKQWK )
-3. Затем нажмите кнопку "Создать API" и выберите "Сгенерированный системой".
-4. В разделе "Ограничения API" включите "Включить спотовую и маржинальную торговлю".
-5. Скопируйте и вставьте в файл **ConfigBinance\Config.py** полученные **"Ключ API"** и **"Секретный ключ"**
-
-#### Теперь можно запускать примеры
-
-В папке **DataExamplesBinance_ru** находится код примеров по работе с биржевыми данными через API интерфейс [Binance](https://www.binance.com/?ref=CPA_004RZBKQWK ).
-
-* **01 - Symbol.py** - торговая стратегия для получения исторических и "живых" данных одного тикера по одному таймфрейму
-* **02 - Symbol data to DF.py** - экспорт в csv файл исторических данных одного тикера по одному таймфрейму
-* **03 - Symbols.py** - торговая стратегия для нескольких тикеров по одному таймфрейму
-* **04 - Resample.py** - торговая стратегия для получения данных одного тикера по разным таймфреймам методом конвертации меньшего таймфрейма в больший
-* **05 - Replay.py** - запуск торговой стратегии на меньшем таймфрейме, с обработкой на большем и выводом графика большего интервала
-* **06 - Rollover.py** - запуск торговой стратегии на склейке данных из файла с историческими данными и последней загруженной истории с брокера
-* **07 - Get Asset Balance.py** - получение баланса тикера напрямую через API Binance
-* **08 - Timeframes.py** - торговая стратегия для одного тикера по разным таймфреймам
-* **Strategy.py** - Пример торговой стратегии, которая только выводит данные по тикеру/тикерам OHLCV
-
-В папке **StrategyExamplesBinance_ru** находится код примеров стратегий.  
-
-* **01 - Live Trade.py** - Пример торговой стратегии в live режиме для двух тикеров BTC и ETH на базовом тикере USDT. 
-  * В стратегии показано как применять индикаторы (SMA, RSI) к нескольким тикерам одновременно. 
-  * Пример выставления заявок на биржу Binance и их снятие.
-    * Пожалуйста, имейте в виду! Это live режим - если на рынке произойдет значительное изменение цены в сторону понижения более чем на 5% - ордер может быть выполнен.... 
-    * **Не забудьте после теста снять с биржи выставленные заявки!**
-* **02 - Live Trade MultiPortfolio.py** - Пример торговой стратегии в live режиме для множества тикеров, которые можно передавать в стратегию списком (BTC, ETH, BNB) на базовом тикере USDT. 
-  * В стратегии показано как применять индикаторы (SMA, RSI) к нескольким тикерам одновременно. 
-  * Пример выставления заявок на биржу Binance и их снятие.
-    * Пожалуйста, имейте в виду! Это live режим - если на рынке произойдет значительное изменение цены в сторону понижения более чем на 5% - ордер может быть выполнен....
-    * **Не забудьте после теста снять с биржи выставленные заявки!**
-* **03 - Live Trade ETH.py** - Пример торговой стратегии в live режиме для двух тикеров BNB и XMR на базовом тикере ETH. 
-  * В стратегии показано как применять индикаторы (SMA, RSI) к нескольким тикерам одновременно. 
-  * Пример выставления заявок на биржу Binance и их снятие.
-    * Пожалуйста, имейте в виду! Это live режим - если на рынке произойдет значительное изменение цены в сторону понижения более чем на 5% - ордер может быть выполнен....
-    * **Не забудьте после теста снять с биржи выставленные заявки!**
-* **04 - Offline Backtest.py** - Пример торговой стратегии для теста на истории - не live режим - для двух тикеров BTC и ETH на базовом тикере USDT. 
-  * В стратегии показано как применять индикаторы (SMA, RSI) к нескольким тикерам одновременно.
-    * Не live режим - для тестирования стратегий без отправки заявок на биржу!
-* **05 - Offline Backtest MultiPortfolio.py** - Пример торговой стратегии для теста на истории - не live режим - для множества тикеров, которые можно передавать в стратегию списком (BTC, ETH, BNB) на базовом тикере USDT. 
-  * В стратегии показано как применять индикаторы (SMA, RSI) к нескольким тикерам одновременно.
-    * Не live режим - для тестирования стратегий без отправки заявок на биржу!
-* **06 - Live Trade Just Buy and Close by Market.py** - Пример торговой стратегии в live для тикера ETH на базовом тикере USDT.
-  * Стратегия показывает, как покупать по цене закрытия и продавать по рыночной небольшое количество ETH через 3 бара.
-  * Пример размещения ордеров на бирже Binance.
-    * **Не забудьте отменить выставленные ордера с биржи после тестирования!**
-* **07 - Offline Backtest Indicators.py** - Пример торговой стратегии для теста на истории с использованием индикаторов SMA и RSI - не live режим - для двух тикеров BTC и ETH на базовом тикере USDT. 
-  * В стратегии показано как применять индикаторы (SMA, RSI) к нескольким тикерам одновременно.
-    * генерит 177% дохода на момент записи видео )) 
-    * Не live режим - для тестирования стратегий без отправки заявок на биржу!
-## Спасибо
-- backtrader: очень простая и классная библиотека!
-- [python-binance](https://github.com/sammchardy/python-binance ): Для создания оболочки Binance API, сокращающей большую часть работы.
-- lindomar-oliveira за некоторый код
-
-## Важно
-Исправление ошибок, доработка и развитие библиотеки осуществляется автором и сообществом!
-
-**Пушьте ваши коммиты!** 
-
-# Условия использования
-Библиотека backtrader_binance позволяющая делать интеграцию Backtrader и Binance API - это **Программа** созданная исключительно для удобства работы.
-При использовании **Программы** Пользователь обязан соблюдать положения действующего законодательства Российской Федерации или своей страны.
-Использование **Программы** предлагается по принципу «Как есть» («AS IS»). Никаких гарантий, как устных, так и письменных не прилагается и не предусматривается.
-Автор и сообщество не дает гарантии, что все ошибки **Программы** были устранены, соответственно автор и сообщество не несет никакой ответственности за
-последствия использования **Программы**, включая, но, не ограничиваясь любым ущербом оборудованию, компьютерам, мобильным устройствам, 
-программному обеспечению Пользователя вызванным или связанным с использованием **Программы**, а также за любые финансовые потери,
-понесенные Пользователем в результате использования **Программы**.
-Никто не ответственен за потерю данных, убытки, ущерб, включаю случайный или косвенный, упущенную выгоду, потерю доходов или любые другие потери,
-связанные с использованием **Программы**.
-
-**Программа** распространяется на условиях лицензии [MIT](https://choosealicense.com/licenses/mit).
+# backtrader_binance
+Binance API integration with [Backtrader](https://github.com/WISEPLAT/backtrader).
+
+With this integration you can do:
+ - Backtesting your strategy on historical data from the exchange [Binance](https://www.binance.com/?ref=CPA_004RZBKQWK ) + [Backtrader](https://github.com/WISEPLAT/backtrader )  // Backtesting 
+ - Launch trading systems for automatic trading on the exchange [Binance](https://www.binance.com/?ref=CPA_004RZBKQWK) + [Backtrader](https://github.com/WISEPLAT/backtrader ) // Live trading
+ - Download historical data for cryptocurrencies from the exchange [Binance](https://www.binance.com/?ref=CPA_004RZBKQWK)
+
+For API connection we are using library [python-binance](https://github.com/sammchardy/python-binance).
+
+## Installation
+1) The simplest way:
+```shell
+pip install backtrader_binance
+```
+or
+```shell
+git clone https://github.com/WISEPLAT/backtrader_binance
+```
+or
+```shell
+pip install git+https://github.com/WISEPLAT/backtrader_binance.git
+```
+
+2) Please use backtrader from my repository (as your can push your commits in it). Install it:
+```shell
+pip install git+https://github.com/WISEPLAT/backtrader.git
+```
+-- Can I use your binance interface with original backtrader?
+
+-- Yes, you can use original backtrader, as the author of original backtrader had approved all my changes. 
+
+Here is the link: [mementum/backtrader#472](https://github.com/mementum/backtrader/pull/472)
+
+3) We have some dependencies, you need to install them: 
+```shell
+pip install python-binance pandas matplotlib
+```
+
+### Getting started
+To make it easier to figure out how everything works, many examples have been made in the folders **DataExamplesBinance** and **StrategyExamplesBinance**.
+
+Before running the example, you need to get your API key and Secret key, and put them in the file **ConfigBinance\Config.py:**
+
+```python
+# content of ConfigBinance\Config.py 
+class Config:
+    BINANCE_API_KEY = "YOUR_API_KEY"
+    BINANCE_API_SECRET = "YOUR_SECRET_KEY"
+```
+
+#### How to get a Binance API token:
+1. Register your account on [Binance](https://www.binance.com/?ref=CPA_004RZBKQWK )
+2. Go to the ["API Management"](https://www.binance.com/en/my/settings/api-management?ref=CPA_004RZBKQWK ) 
+3. Then click the "Create API" button and select "System Generated".
+4. In the "API Restrictions" section, enable "Enable Spot and Margin Trading".
+5. Copy and paste to the file **ConfigBinance\Config.py ** received **"API key"** and **"Secret key"**
+
+#### Now you can run examples
+
+The **DataExamplesBinance** folder contains the code of examples for working with exchange data via the [Binance](https://www.binance.com/?ref=CPA_004RZBKQWK ) API.
+
+* **01 - Symbol.py** - trading strategy for obtaining historical and "live" data of one ticker for one timeframe
+* **02 - Symbol data to DF.py** - export to csv file of historical data of one ticker for one timeframe
+* **03 - Symbols.py** - trading strategy for multiple tickers on the same timeframe
+* **04 - Resample.py** - trading strategy for obtaining data from one ticker for different timeframes by converting a smaller timeframe into a larger one
+* **05 - Replay.py** - launching a trading strategy on a smaller timeframe, with processing on a larger one and displaying a larger interval chart
+* **06 - Rollover.py** - launch of a trading strategy based on gluing data from a file with historical data and the last downloaded history from the broker
+* **07 - Get Asset Balance.py** - getting the ticker balance directly through the Binance API
+* **08 - Timeframes.py** - trading strategy is running on different timeframes.
+* **09 - Get Asset Info.py** - getting info about asset: balance, lot size, min price step, min value to buy and etc.
+* **09 - Get Asset Info - no Decimal.py** - getting info about asset: balance, lot size, min price step, min value to buy and etc.
+* **09 - Get Asset Info - through client.py** - getting info about asset: balance, lot size, min price step, min value to buy and etc.
+* **10 - Get Historical Data.py** - getting historical data through binance client for asset.
+* **Strategy.py** - An example of a trading strategy that only outputs data of the OHLCV for ticker/tickers
+
+The **StrategyExamplesBinance** folder contains the code of sample strategies.
+
+* **01 - Live Trade.py** - An example of a live trading strategy for two BTC and ETH tickers on the base USDT ticker.
+  * The strategy shows how to apply indicators (SMA, RSI) to several tickers at the same time.
+  * Example of placing and cancel orders on the Binance exchange.
+    * Please be aware! This is Live order - if market has a big change down in value of price more than 5% - the order will be completed.... 
+    * **Do not forget to cancel the submitted orders from the exchange after the test!**
+* **02 - Live Trade MultiPortfolio.py** - An example of a live trading strategy for a set of tickers that can be transferred to the strategy in a list (BTC, ETH, BNB) on the base USDT ticker.
+  * The strategy shows how to apply indicators (SMA, RSI) to several tickers at the same time.
+  * Example of placing and cancel orders on the Binance exchange.
+    * Please be aware! This is Live order - if market has a big change down in value of price more than 5% - the order will be completed.... 
+    * **Do not forget to cancel the submitted orders from the exchange after the test!**
+* **03 - Live Trade ETH.py** - An example of a live trading strategy for two BNB and XMR tickers on the basic ETH ticker.
+  * The strategy shows how to apply indicators (SMA, RSI) to several tickers at the same time.
+  * Example of placing and cancel orders on the Binance exchange.
+    * Please be aware! This is Live order - if market has a big change down in value of price more than 5% - the order will be completed.... 
+    * **Do not forget to cancel the submitted orders from the exchange after the test!**
+* **04 - Offline Backtest.py** - An example of a trading strategy on a historical data - not live mode - for two BTC and ETH tickers on the base USDT ticker.
+  * The strategy shows how to apply indicators (SMA, RSI) to several tickers at the same time.
+    * Not a live mode - for testing strategies without sending orders to the exchange!
+* **05 - Offline Backtest MultiPortfolio.py** - An example of a trading strategy on a historical data - not live mode - for a set of tickers that can be transferred to the strategy in a list (BTC, ETH, BNB) on the base USDT ticker.
+  * The strategy shows how to apply indicators (SMA, RSI) to several tickers at the same time.
+    * Not a live mode - for testing strategies without sending orders to the exchange!
+* **06 - Live Trade Just Buy and Close by Market.py** - An example of a live trading strategy for ETH ticker on the base USDT ticker.
+  * The strategy shows how to buy by close price and sell by market a little value of ETH after 3 bars.
+  * Example of placing orders on the Binance exchange.
+    * **Do not forget to cancel the submitted orders from the exchange after the test!**
+* **07 - Offline Backtest Indicators.py** - An example of a trading strategy for a history test using SMA and RSI indicators - not live mode - for two BTC and ETH tickers on the base USDT ticker.
+  * The strategy shows how to apply indicators (SMA, RSI) to several tickers at the same time.
+    * generates 177% of revenue at the time of video recording))
+    * Non-live mode - for testing strategies without sending orders to the exchange!
+
+## Thanks
+- backtrader: Very simple and cool library!
+- [python-binance](https://github.com/sammchardy/python-binance): For creating Binance API wrapper, shortening a lot of work.
+- lindomar-oliveira for some code
+
+## License
+[MIT](https://choosealicense.com/licenses/mit)
+
+## Important
+Error correction, revision and development of the library is carried out by the author and the community!
+
+**Push your commits!**
+
+## Terms of Use
+The backtrader_binance library, which allows you to integrate Backtrader and Binance API, is the **Program** created solely for the convenience of work.
+When using the **Program**, the User is obliged to comply with the provisions of the current legislation of his country.
+Using the **Program** are offered on an "AS IS" basis. No guarantees, either oral or written, are attached and are not provided.
+The author and the community does not guarantee that all errors of the **Program** have been eliminated, respectively, the author and the community do not bear any responsibility for
+the consequences of using the **Program**, including, but not limited to, any damage to equipment, computers, mobile devices,
+User software caused by or related to the use of the **Program**, as well as for any financial losses
+incurred by the User as a result of using the **Program**.
+No one is responsible for data loss, losses, damages, including accidental or indirect, lost profits, loss of revenue or any other losses
+related to the use of the **Program**.
+
+The **Program** is distributed under the terms of the [MIT](https://choosealicense.com/licenses/mit ) license.
+
+## Star History
+
+Please put a Star 🌟 for this code
+
+[![Star History Chart](https://api.star-history.com/svg?repos=WISEPLAT/backtrader_binance&type=Timeline)](https://star-history.com/#WISEPLAT/backtrader_binance&Timeline)
+
+Пожалуйста поставьте Звезду 🌟 этому коду
+
+==========================================================================
+
+# backtrader_binance
+
+Интеграция Binance API с [Backtrader](https://github.com/WISEPLAT/backtrader ).
+
+С помощью этой интеграции вы можете делать:
+- Тестирование вашей стратегии на исторических данных с биржи [Binance](https://www.binance.com/?ref=CPA_004RZBKQWK ) + [Backtrader](https://github.com/WISEPLAT/backtrader )
+- Запускать торговые системы для автоматической торговли на бирже [Binance](https://www.binance.com/?ref=CPA_004RZBKQWK ) + [Backtrader](https://github.com/WISEPLAT/backtrader ) 
+- Загружать исторические данные по криптовалютам с биржи [Binance](https://www.binance.com/?ref=CPA_004RZBKQWK )
+
+Для подключения к API мы используем библиотеку [python-binance](https://github.com/sammchardy/python-binance ).
+
+
+## Установка
+1) Самый простой способ:
+```shell
+pip install backtrader_binance
+```
+или
+```shell
+git clone https://github.com/WISEPLAT/backtrader_binance
+```
+или
+```shell
+pip install git+https://github.com/WISEPLAT/backtrader_binance.git
+```
+
+2) Пожалуйста, используйте backtrader из моего репозитория (так как вы можете размещать в нем свои коммиты). Установите его:
+```shell
+pip install git+https://github.com/WISEPLAT/backtrader.git
+```
+-- Могу ли я использовать ваш интерфейс binance с оригинальным backtrader?
+
+-- Да, вы можете использовать оригинальный backtrader, так как автор оригинального backtrader одобрил все мои изменения.
+
+Вот ссылка: [mementum/backtrader#472](https://github.com/mementum/backtrader/pull/472)
+
+3) У нас есть некоторые зависимости, вам нужно их установить:
+```shell
+pip install python-binance pandas matplotlib
+```
+
+### Начало работы
+Чтобы было легче разобраться как всё работает, сделано множество примеров в папках **DataExamplesBinance_ru** и **StrategyExamplesBinance_ru**.
+
+Перед запуском примера, необходимо получить свой API ключ и Secret ключ, и прописать их в файле **ConfigBinance\Config.py:**
+
+```python
+# content of ConfigBinance\Config.py 
+class Config:
+    BINANCE_API_KEY = "YOUR_API_KEY"
+    BINANCE_API_SECRET = "YOUR_SECRET_KEY"
+```
+
+####  Как получить токен Binance API:
+1. Зарегистрируйте свой аккаунт на [Binance](https://www.binance.com/?ref=CPA_004RZBKQWK )
+2. Перейдите в раздел ["Управление API"](https://www.binance.com/en/my/settings/api-management?ref=CPA_004RZBKQWK )
+3. Затем нажмите кнопку "Создать API" и выберите "Сгенерированный системой".
+4. В разделе "Ограничения API" включите "Включить спотовую и маржинальную торговлю".
+5. Скопируйте и вставьте в файл **ConfigBinance\Config.py** полученные **"Ключ API"** и **"Секретный ключ"**
+
+#### Теперь можно запускать примеры
+
+В папке **DataExamplesBinance_ru** находится код примеров по работе с биржевыми данными через API интерфейс [Binance](https://www.binance.com/?ref=CPA_004RZBKQWK ).
+
+* **01 - Symbol.py** - торговая стратегия для получения исторических и "живых" данных одного тикера по одному таймфрейму
+* **02 - Symbol data to DF.py** - экспорт в csv файл исторических данных одного тикера по одному таймфрейму
+* **03 - Symbols.py** - торговая стратегия для нескольких тикеров по одному таймфрейму
+* **04 - Resample.py** - торговая стратегия для получения данных одного тикера по разным таймфреймам методом конвертации меньшего таймфрейма в больший
+* **05 - Replay.py** - запуск торговой стратегии на меньшем таймфрейме, с обработкой на большем и выводом графика большего интервала
+* **06 - Rollover.py** - запуск торговой стратегии на склейке данных из файла с историческими данными и последней загруженной истории с брокера
+* **07 - Get Asset Balance.py** - получение баланса тикера напрямую через API Binance
+* **08 - Timeframes.py** - торговая стратегия для одного тикера по разным таймфреймам
+* **Strategy.py** - Пример торговой стратегии, которая только выводит данные по тикеру/тикерам OHLCV
+
+В папке **StrategyExamplesBinance_ru** находится код примеров стратегий.  
+
+* **01 - Live Trade.py** - Пример торговой стратегии в live режиме для двух тикеров BTC и ETH на базовом тикере USDT. 
+  * В стратегии показано как применять индикаторы (SMA, RSI) к нескольким тикерам одновременно. 
+  * Пример выставления заявок на биржу Binance и их снятие.
+    * Пожалуйста, имейте в виду! Это live режим - если на рынке произойдет значительное изменение цены в сторону понижения более чем на 5% - ордер может быть выполнен.... 
+    * **Не забудьте после теста снять с биржи выставленные заявки!**
+* **02 - Live Trade MultiPortfolio.py** - Пример торговой стратегии в live режиме для множества тикеров, которые можно передавать в стратегию списком (BTC, ETH, BNB) на базовом тикере USDT. 
+  * В стратегии показано как применять индикаторы (SMA, RSI) к нескольким тикерам одновременно. 
+  * Пример выставления заявок на биржу Binance и их снятие.
+    * Пожалуйста, имейте в виду! Это live режим - если на рынке произойдет значительное изменение цены в сторону понижения более чем на 5% - ордер может быть выполнен....
+    * **Не забудьте после теста снять с биржи выставленные заявки!**
+* **03 - Live Trade ETH.py** - Пример торговой стратегии в live режиме для двух тикеров BNB и XMR на базовом тикере ETH. 
+  * В стратегии показано как применять индикаторы (SMA, RSI) к нескольким тикерам одновременно. 
+  * Пример выставления заявок на биржу Binance и их снятие.
+    * Пожалуйста, имейте в виду! Это live режим - если на рынке произойдет значительное изменение цены в сторону понижения более чем на 5% - ордер может быть выполнен....
+    * **Не забудьте после теста снять с биржи выставленные заявки!**
+* **04 - Offline Backtest.py** - Пример торговой стратегии для теста на истории - не live режим - для двух тикеров BTC и ETH на базовом тикере USDT. 
+  * В стратегии показано как применять индикаторы (SMA, RSI) к нескольким тикерам одновременно.
+    * Не live режим - для тестирования стратегий без отправки заявок на биржу!
+* **05 - Offline Backtest MultiPortfolio.py** - Пример торговой стратегии для теста на истории - не live режим - для множества тикеров, которые можно передавать в стратегию списком (BTC, ETH, BNB) на базовом тикере USDT. 
+  * В стратегии показано как применять индикаторы (SMA, RSI) к нескольким тикерам одновременно.
+    * Не live режим - для тестирования стратегий без отправки заявок на биржу!
+* **06 - Live Trade Just Buy and Close by Market.py** - Пример торговой стратегии в live для тикера ETH на базовом тикере USDT.
+  * Стратегия показывает, как покупать по цене закрытия и продавать по рыночной небольшое количество ETH через 3 бара.
+  * Пример размещения ордеров на бирже Binance.
+    * **Не забудьте отменить выставленные ордера с биржи после тестирования!**
+* **07 - Offline Backtest Indicators.py** - Пример торговой стратегии для теста на истории с использованием индикаторов SMA и RSI - не live режим - для двух тикеров BTC и ETH на базовом тикере USDT. 
+  * В стратегии показано как применять индикаторы (SMA, RSI) к нескольким тикерам одновременно.
+    * генерит 177% дохода на момент записи видео )) 
+    * Не live режим - для тестирования стратегий без отправки заявок на биржу!
+* **08 - Timeframes.py** - торговая стратегия работает на разных таймфреймах.
+* **09 - Get Asset Info.py* - получение информации об активе: баланс, размер лота, минимальный шаг цены, минимальная стоимость покупки и т.д.
+* **09 - Get Asset Info - no Decimal.py** - получение информации об активе: баланс, размер лота, минимальный шаг цены, минимальная стоимость покупки и т.д.
+* **09 - Get Asset Info - through client.py** - получение информации об активе: баланс, размер лота, минимальный шаг цены, минимальная стоимость покупки и т.д.
+* **10 - Get Historical Data.py** - получение исторических данных через клиент binance для актива.
+
+## Спасибо
+- backtrader: очень простая и классная библиотека!
+- [python-binance](https://github.com/sammchardy/python-binance ): Для создания оболочки Binance API, сокращающей большую часть работы.
+- lindomar-oliveira за некоторый код
+
+## Важно
+Исправление ошибок, доработка и развитие библиотеки осуществляется автором и сообществом!
+
+**Пушьте ваши коммиты!** 
+
+# Условия использования
+Библиотека backtrader_binance позволяющая делать интеграцию Backtrader и Binance API - это **Программа** созданная исключительно для удобства работы.
+При использовании **Программы** Пользователь обязан соблюдать положения действующего законодательства Российской Федерации или своей страны.
+Использование **Программы** предлагается по принципу «Как есть» («AS IS»). Никаких гарантий, как устных, так и письменных не прилагается и не предусматривается.
+Автор и сообщество не дает гарантии, что все ошибки **Программы** были устранены, соответственно автор и сообщество не несет никакой ответственности за
+последствия использования **Программы**, включая, но, не ограничиваясь любым ущербом оборудованию, компьютерам, мобильным устройствам, 
+программному обеспечению Пользователя вызванным или связанным с использованием **Программы**, а также за любые финансовые потери,
+понесенные Пользователем в результате использования **Программы**.
+Никто не ответственен за потерю данных, убытки, ущерб, включаю случайный или косвенный, упущенную выгоду, потерю доходов или любые другие потери,
+связанные с использованием **Программы**.
+
+**Программа** распространяется на условиях лицензии [MIT](https://choosealicense.com/licenses/mit).
```

### Comparing `backtrader_binance-1.0.4/setup.py` & `backtrader_binance-1.0.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 here = os.path.abspath(os.path.dirname(__file__))
 
 # Get the long description from the relevant file
 with codecs.open(os.path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='backtrader_binance',
-      version='1.0.4',
+      version='1.0.5',
       author='wiseplat',
       author_email='oshpagin@gmail.com',
       license='MIT License',
       description='Binance API integration with Backtrader',
       long_description=long_description,
       long_description_content_type='text/markdown',
       url='https://github.com/WISEPLAT/backtrader_binance',
```

