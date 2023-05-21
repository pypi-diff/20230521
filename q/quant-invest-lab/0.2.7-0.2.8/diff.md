# Comparing `tmp/quant_invest_lab-0.2.7.tar.gz` & `tmp/quant_invest_lab-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quant_invest_lab-0.2.7.tar", max compression
+gzip compressed data, was "quant_invest_lab-0.2.8.tar", max compression
```

## Comparing `quant_invest_lab-0.2.7.tar` & `quant_invest_lab-0.2.8.tar`

### file list

```diff
@@ -1,12 +1,15 @@
--rw-r--r--   0        0        0     5020 2023-05-18 21:52:51.578303 quant_invest_lab-0.2.7/README.md
--rw-r--r--   0        0        0     1543 2023-05-18 21:52:51.582303 quant_invest_lab-0.2.7/pyproject.toml
--rw-r--r--   0        0        0    28604 2023-05-18 21:52:51.582303 quant_invest_lab-0.2.7/quant_invest_lab/backtest.py
--rw-r--r--   0        0        0    17212 2023-05-18 21:52:51.582303 quant_invest_lab-0.2.7/quant_invest_lab/data_provider.py
--rw-r--r--   0        0        0    26301 2023-05-18 21:52:51.582303 quant_invest_lab-0.2.7/quant_invest_lab/indicators.py
--rw-r--r--   0        0        0    11102 2023-05-18 21:52:51.582303 quant_invest_lab-0.2.7/quant_invest_lab/metrics.py
--rw-r--r--   0        0        0     7659 2023-05-18 21:52:51.582303 quant_invest_lab-0.2.7/quant_invest_lab/optimization.py
--rw-r--r--   0        0        0    18363 2023-05-18 21:52:51.582303 quant_invest_lab-0.2.7/quant_invest_lab/portfolio.py
--rw-r--r--   0        0        0     3577 2023-05-18 21:52:51.582303 quant_invest_lab-0.2.7/quant_invest_lab/screener.py
--rw-r--r--   0        0        0     8477 2023-05-18 21:52:51.582303 quant_invest_lab-0.2.7/quant_invest_lab/simulation.py
--rw-r--r--   0        0        0     3758 2023-05-18 21:52:51.582303 quant_invest_lab-0.2.7/quant_invest_lab/utils.py
--rw-r--r--   0        0        0     6939 1970-01-01 00:00:00.000000 quant_invest_lab-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0     5020 2023-05-21 20:12:27.924557 quant_invest_lab-0.2.8/README.md
+-rw-r--r--   0        0        0     1727 2023-05-21 20:12:27.928557 quant_invest_lab-0.2.8/pyproject.toml
+-rw-r--r--   0        0        0    29186 2023-05-21 20:12:27.928557 quant_invest_lab-0.2.8/quant_invest_lab/backtest.py
+-rw-r--r--   0        0        0     1007 2023-05-21 20:12:27.928557 quant_invest_lab-0.2.8/quant_invest_lab/constants.py
+-rw-r--r--   0        0        0    16533 2023-05-21 20:12:27.928557 quant_invest_lab-0.2.8/quant_invest_lab/data_provider.py
+-rw-r--r--   0        0        0    26301 2023-05-21 20:12:27.928557 quant_invest_lab-0.2.8/quant_invest_lab/indicators.py
+-rw-r--r--   0        0        0    11102 2023-05-21 20:12:27.928557 quant_invest_lab-0.2.8/quant_invest_lab/metrics.py
+-rw-r--r--   0        0        0     7659 2023-05-21 20:12:27.928557 quant_invest_lab-0.2.8/quant_invest_lab/optimization.py
+-rw-r--r--   0        0        0    18363 2023-05-21 20:12:27.928557 quant_invest_lab-0.2.8/quant_invest_lab/portfolio.py
+-rw-r--r--   0        0        0     3577 2023-05-21 20:12:27.928557 quant_invest_lab-0.2.8/quant_invest_lab/screener.py
+-rw-r--r--   0        0        0     7329 2023-05-21 20:12:27.928557 quant_invest_lab-0.2.8/quant_invest_lab/signal_processing.py
+-rw-r--r--   0        0        0     7848 2023-05-21 20:12:27.928557 quant_invest_lab-0.2.8/quant_invest_lab/simulation.py
+-rw-r--r--   0        0        0      178 2023-05-21 20:12:27.928557 quant_invest_lab-0.2.8/quant_invest_lab/types.py
+-rw-r--r--   0        0        0     3403 2023-05-21 20:12:27.928557 quant_invest_lab-0.2.8/quant_invest_lab/utils.py
+-rw-r--r--   0        0        0     7025 1970-01-01 00:00:00.000000 quant_invest_lab-0.2.8/PKG-INFO
```

### Comparing `quant_invest_lab-0.2.7/README.md` & `quant_invest_lab-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `quant_invest_lab-0.2.7/pyproject.toml` & `quant_invest_lab-0.2.8/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "quant-invest-lab"
-version = "0.2.7"
+version = "0.2.8"
 description = "Quant Invest Lab is a python package to help you to do some quantitative experiments, while trying to learn or build quantitative investment solutions. This project was initially my own set of functionnalities but I decided to build a package for that and sharing it as open source project."
 authors = ["BaptisteZloch <bzloch@hotmail.fr>"]
 maintainers = ["BaptisteZloch <bzloch@hotmail.fr>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/BaptisteZloch/Quant-Invest-Lab"
 classifiers = [
@@ -31,15 +31,22 @@
 nbformat = "^5.8.0"
 matplotlib = "^3.7.1"
 seaborn = "^0.12.2"
 tqdm = "^4.64.1"
 beautifulsoup4 = "^4.12.2"
 fitter = "^1.5.2"
 scikit-learn = "^1.2.2"
+emd-signal = "^1.4.0"
+pywavelets = "^1.4.1"
 
 [tool.poetry.group.dev.dependencies]
 ipykernel = "^6.23.0"
 black = "^23.3.0"
+mkdocs = "^1.4.3"
+mkdocs-material = "^9.1.14"
+mkdocs-material-extensions = "^1.1.1"
+mkdocstrings = "^0.21.2"
+mkdocstrings-python = "^1.0.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `quant_invest_lab-0.2.7/quant_invest_lab/backtest.py` & `quant_invest_lab-0.2.8/quant_invest_lab/backtest.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,33 +17,23 @@
     sortino_ratio,
     max_drawdown,
     drawdown,
     kelly_criterion,
     value_at_risk,
     conditional_value_at_risk,
 )
-from quant_invest_lab.utils import timeframe_annualized
+from quant_invest_lab.constants import TIMEFRAME_ANNUALIZED, TIMEFRAMES
+from quant_invest_lab.types import Timeframe
 
 
 def print_ohlc_backtest_report(
     returns_df: pd.DataFrame,
     trades_df: pd.DataFrame,
     ohlcv_df: pd.DataFrame,
-    timeframe: Literal[
-        "1min",
-        "2min",
-        "5min",
-        "15min",
-        "30min",
-        "1hour",
-        "2hour",
-        "4hour",
-        "12hour",
-        "1day",
-    ],
+    timeframe: Timeframe,
     initial_equity: Union[int, float] = 1000,
 ) -> None:
     good_trades = trades_df.loc[trades_df["trade_return"] > 0]
     bad_trades = trades_df.loc[trades_df["trade_return"] < 0]
     total_trades = len(trades_df)
     print(f"\n{'  Strategy performances  ':-^50}")
 
@@ -60,21 +50,21 @@
     print(
         f"Strategy expectancy: {100*expectancy(len(good_trades) / total_trades,good_trades['trade_return'].mean(),bad_trades['trade_return'].mean()):.2f} %"
     )
 
     print(f"\n{'  Returns statistical information  ':-^50}")
 
     print(
-        f"Expected return : {100*returns_df['Returns'].mean():.2f} %, annuzalized: {100*returns_df['Returns'].mean()*timeframe_annualized[timeframe]:.2f} %"
+        f"Expected return : {100*returns_df['Returns'].mean():.2f} %, annuzalized: {100*returns_df['Returns'].mean()*TIMEFRAME_ANNUALIZED[timeframe]:.2f} %"
     )
     print(
-        f"Median return : {100*returns_df['Returns'].median():.2f} %, annuzalized: {100*returns_df['Returns'].median()*timeframe_annualized[timeframe]:.2f} %"
+        f"Median return : {100*returns_df['Returns'].median():.2f} %, annuzalized: {100*returns_df['Returns'].median()*TIMEFRAME_ANNUALIZED[timeframe]:.2f} %"
     )
     print(
-        f'Expected volatility: {100*returns_df["Returns"].std():.2f} %, annualized: {100*returns_df["Returns"].std()*(timeframe_annualized[timeframe]**0.5):.2f} %'
+        f'Expected volatility: {100*returns_df["Returns"].std():.2f} %, annualized: {100*returns_df["Returns"].std()*(TIMEFRAME_ANNUALIZED[timeframe]**0.5):.2f} %'
     )
     print(
         f"Skewness: {skew(returns_df.Returns.values):.2f} vs {skew(ohlcv_df.Returns.values):.2f} (buy and hold), <0 = left tail, >0 = right tail -> the higher the better"
     )
     print(
         f"Kurtosis: {kurtosis(returns_df.Returns.values):.2f} vs {kurtosis(ohlcv_df.Returns.values):.2f} (buy and hold)",
         ", >3 = fat tails, <3 = thin tails -> the lower the better",
@@ -90,21 +80,21 @@
     print(
         f"Max drawdown: {100*max_drawdown(returns_df.Returns):.2f} % vs {100*max_drawdown(ohlcv_df.Returns):.2f} % (buy and hold)"
     )
     print(
         f"Kelly criterion: {100*kelly_criterion(returns_df.Returns):.2f} % vs {100*kelly_criterion(ohlcv_df.Returns):.2f} % (buy and hold)"
     )
     print(
-        f"Sharpe ratio (annualized): {sharpe_ratio(returns_df['Returns'], timeframe_annualized[timeframe],risk_free_rate=timeframe_annualized[timeframe]*ohlcv_df.Returns.mean()):.2f} (risk free rate = buy and hold)"
+        f"Sharpe ratio (annualized): {sharpe_ratio(returns_df['Returns'], TIMEFRAME_ANNUALIZED[timeframe],risk_free_rate=TIMEFRAME_ANNUALIZED[timeframe]*ohlcv_df.Returns.mean()):.2f} (risk free rate = buy and hold)"
     )
     print(
-        f"Sortino ratio (annualized): {sortino_ratio(returns_df['Returns'], timeframe_annualized[timeframe],risk_free_rate=timeframe_annualized[timeframe]*ohlcv_df.Returns.mean()):.2f} (risk free rate = buy and hold)"
+        f"Sortino ratio (annualized): {sortino_ratio(returns_df['Returns'], TIMEFRAME_ANNUALIZED[timeframe],risk_free_rate=TIMEFRAME_ANNUALIZED[timeframe]*ohlcv_df.Returns.mean()):.2f} (risk free rate = buy and hold)"
     )
     print(
-        f"Calmar ratio (annualized): {calmar_ratio(returns_df['Returns'], timeframe_annualized[timeframe]):.2f} (risk free rate = buy and hold)"
+        f"Calmar ratio (annualized): {calmar_ratio(returns_df['Returns'], TIMEFRAME_ANNUALIZED[timeframe]):.2f} (risk free rate = buy and hold)"
     )
 
     print(f"\n{'  Trades informations  ':-^50}")
     print(f"Mean trade return : {100*trades_df['trade_return'].mean():.2f} %")
     print(f"Median trade return : {100*trades_df['trade_return'].median():.2f} %")
     print(f'Mean trade volatility: {100*trades_df["trade_return"].std():.2f} %')
     print(
@@ -176,15 +166,15 @@
 
     Returns:
     -----
         tuple[pd.DataFrame, pd.DataFrame]: It returns 2 dataframes, the first is the trades_df : trade summary dataframe and the second is the returns dataframe : returns_df.
     """
     assert position_type in ["long", "short"], "position_type must be long or short"
 
-    returns_signs = {"long": 1, "short": -1}
+    RETURNS_SIGNS = {"long": 1, "short": -1}
     previous_row = ohlcv_df.iloc[0]
     position_opened = False
     timeframe_count = 0
     current_trade: dict[str, float | datetime | int | str | pd.Timestamp] = {}
 
     trades_df = pd.DataFrame(
         columns=[
@@ -196,53 +186,53 @@
             "exit_reason",
             "trade_return",
         ]
     )
 
     returns_df = pd.DataFrame(columns=["Returns"])
 
-    for index, row in tqdm(
-        ohlcv_df[1:].iterrows(),
+    for row in tqdm(
+        ohlcv_df[1:-1].itertuples(index=True),
         desc="Backtesting...",
         total=ohlcv_df.shape[0] - 1,
         leave=False,
     ):
         if position_opened is False and entry_function(row, previous_row) is True:
             position_opened = True
-            current_trade["entry_date"] = index
+            current_trade["entry_date"] = row.Index
             current_trade["entry_price"] = row.Close
             current_trade["entry_reason"] = "Entry position triggered"
             timeframe_count = 1
             entry_price = row.Close
         elif (
             position_type == "long"
             and position_opened is True
             and current_trade["entry_price"] * (1 + take_profit) <= row.High
         ) or (
             position_type == "short"
             and position_opened is True
             and current_trade["entry_price"] * (1 + stop_loss) <= row.High
         ):
             position_opened = False
-            current_trade["exit_date"] = index
+            current_trade["exit_date"] = row.Index
 
             current_trade["exit_price"] = (
                 current_trade["entry_price"] * (1 + take_profit)
                 if position_type == "long"
                 else current_trade["entry_price"] * (1 + stop_loss)
             )
 
             current_trade["exit_reason"] = (
                 "Long take profit triggered"
                 if position_type == "long"
                 else "Short stop loss triggered"
             )
 
             rets = (
-                returns_signs[position_type]
+                RETURNS_SIGNS[position_type]
                 * ohlcv_df.loc[
                     current_trade["entry_date"] : current_trade["exit_date"]
                 ].Returns
             )
             if isinstance(taker_fees, float) and taker_fees > 0:
                 rets.iloc[0] = rets.iloc[0] - taker_fees
                 rets.iloc[-1] = rets.iloc[-1] - taker_fees
@@ -265,29 +255,29 @@
             and current_trade["entry_price"] * (1 - stop_loss) >= row.Low
         ) or (
             position_type == "short"
             and position_opened is True
             and current_trade["entry_price"] * (1 - take_profit) >= row.Low
         ):
             position_opened = False
-            current_trade["exit_date"] = index
+            current_trade["exit_date"] = row.Index
 
             current_trade["exit_price"] = (
                 current_trade["entry_price"] * (1 - stop_loss)
                 if position_type == "long"
                 else current_trade["entry_price"] * (1 - take_profit)
             )
             current_trade["exit_reason"] = (
                 "Long stop loss triggered"
                 if position_type == "long"
                 else "Short take profit triggered"
             )
 
             rets = (
-                returns_signs[position_type]
+                RETURNS_SIGNS[position_type]
                 * ohlcv_df.loc[
                     current_trade["entry_date"] : current_trade["exit_date"]
                 ].Returns
             )
             if isinstance(taker_fees, float) and taker_fees > 0:
                 rets.iloc[0] = rets.iloc[0] - taker_fees
                 rets.iloc[-1] = rets.iloc[-1] - taker_fees
@@ -302,21 +292,25 @@
             )
             timeframe_count = 0
             current_trade = {}
         elif (
             position_opened is True
             and exit_function(row, previous_row, timeframe_count) is True
         ):
+            next_row_index = (
+                ohlcv_df.index.get_loc(row.Index) + 1
+            )  # To close on next open.
+
             position_opened = False
-            current_trade["exit_date"] = index
-            current_trade["exit_price"] = row.Close
+            current_trade["exit_date"] = ohlcv_df.iloc[next_row_index].name
+            current_trade["exit_price"] = ohlcv_df.iloc[next_row_index].Open
             current_trade["exit_reason"] = "Exit position triggered"
 
             rets = (
-                returns_signs[position_type]
+                RETURNS_SIGNS[position_type]
                 * ohlcv_df.loc[
                     current_trade["entry_date"] : current_trade["exit_date"]
                 ].Returns
             )
 
             if isinstance(taker_fees, float) and taker_fees > 0:
                 rets.iloc[0] = rets.iloc[0] - taker_fees
@@ -332,34 +326,52 @@
                 ignore_index=False,
             )
             timeframe_count = 0
             current_trade = {}
         else:
             timeframe_count += 1
         previous_row = row
+    # Close last trade
+    if position_opened is True:
+        # print("Closing trade at end of backtest")
+        position_opened = False
+        current_trade["exit_date"] = ohlcv_df.index[-1]
+        current_trade["exit_price"] = ohlcv_df.iloc[-1].Close
+        current_trade["exit_reason"] = "Exit position triggered"
+
+        rets = (
+            RETURNS_SIGNS[position_type]
+            * ohlcv_df.loc[
+                current_trade["entry_date"] : current_trade["exit_date"]
+            ].Returns
+        )
+
+        if isinstance(taker_fees, float) and taker_fees > 0:
+            rets.iloc[0] = rets.iloc[0] - taker_fees
+            rets.iloc[-1] = rets.iloc[-1] - taker_fees
 
+        current_trade["trade_return"] = ((rets + 1).cumprod().iloc[-1]) - 1  # ret
+
+        trades_df = pd.concat(
+            [trades_df, pd.DataFrame([current_trade])], ignore_index=True
+        )
+        returns_df = pd.concat(
+            [returns_df, pd.DataFrame({"Returns": rets.values}, index=rets.index)],
+            ignore_index=False,
+        )
+        timeframe_count = 0
+        current_trade = {}
     return trades_df, returns_df
 
 
 def ohlc_long_only_backtester(
     df: pd.DataFrame,
     long_entry_function: Callable[[pd.Series, pd.Series], bool],
     long_exit_function: Callable[[pd.Series, pd.Series, int], bool],
-    timeframe: Literal[
-        "1min",
-        "2min",
-        "5min",
-        "15min",
-        "30min",
-        "1hour",
-        "2hour",
-        "4hour",
-        "12hour",
-        "1day",
-    ],
+    timeframe: Timeframe,
     take_profit: float = np.inf,
     stop_loss: float = np.inf,
     initial_equity: int = 1000,
     maker_fees: Optional[float] = 0.001,
     taker_fees: Optional[float] = 0.001,
     get_trade_df: bool = False,
     get_returns_df: bool = False,
@@ -372,15 +384,15 @@
     ----
         df (pd.DataFrame): The dataframe containing the OHLC data.
 
         long_entry_function (Callable[[pd.Series, pd.Series], bool]): The long entry function, it should take 2 arguments, the current row and the previous row and return True or False depending on your strategy.
 
         long_exit_function (Callable[[pd.Series, pd.Series, int], bool]): The long exit function, it should take 3 arguments, the current row, the previous row and the number of timeframe count since the last entry order, and return True or False depending on your strategy.
 
-        timeframe (Literal[ &quot;1min&quot;, &quot;2min&quot;, &quot;5min&quot;, &quot;15min&quot;, &quot;30min&quot;, &quot;1hour&quot;, &quot;2hour&quot;, &quot;4hour&quot;, &quot;12hour&quot;, &quot;1day&quot;, ]): The timeframe granularity of the dataframe.
+        timeframe (Timeframe): The timeframe granularity of the dataframe.
 
         take_profit (float, optional): The percent of the buy price to add to create a stop order and take the profit associated. Defaults to np.inf.
 
         stop_loss (float, optional): The percent of the buy price to cut to create a stop order and stop the loss associated. Defaults to np.inf.
 
         initial_equity (int, optional): The initial capital. Defaults to 1000.
 
@@ -396,26 +408,17 @@
 
         plot_result (bool, optional): Plot equity, price, drawdown, distribution of the strategy. Defaults to True.
 
     Returns:
     -----
         Union[None, Union[float, Union[pd.DataFrame, Tuple[pd.DataFrame, pd.DataFrame]]]]: Nothing or the strategy total return or the trade_df or the return_df or the trade_df and the return_df.
     """
-    assert timeframe in [
-        "1min",
-        "2min",
-        "5min",
-        "15min",
-        "30min",
-        "1hour",
-        "2hour",
-        "4hour",
-        "12hour",
-        "1day",
-    ], "timeframe must be one of the following: 1min, 2min, 5min, 15min, 30min, 1hour, 2hour, 4hour, 12hour, 1day"
+    assert (
+        timeframe in TIMEFRAMES
+    ), f"timeframe must be one of the following: {','.join(TIMEFRAMES)}"
     assert df.shape[0] > 1, "Dataframe must have at least 2 rows"
     assert set({"Open", "High", "Low", "Close", "Returns"}).issubset(
         df.columns
     ), "Dataframe must have columns Open, High, Low, Close, Returns"
 
     ohlcv_df = df.copy()
     trades_df, returns_df = __ohlc_backtest_one_position_type(
@@ -448,14 +451,19 @@
     print(f"Intial balance: {initial_equity:.2f} $")
     if taker_fees is not None and maker_fees is not None:
         print(
             f"Taker fees: {taker_fees*100:.2f} %, Maker fees: {maker_fees*100:.2f} %, All the metrics will be calculated considering these fees"
         )
     else:
         print("No fees considered here.")
+    if take_profit != np.inf:
+        print(f"Take profit is set to {take_profit*100:.2f} % of the buy price")
+    if stop_loss != np.inf:
+        print(f"Stop loss is set to {stop_loss*100:.2f} % of the buy price")
+    print("Long only position")
 
     print_ohlc_backtest_report(
         returns_df=returns_df,
         trades_df=trades_df,
         ohlcv_df=ohlcv_df,
         timeframe=timeframe,
         initial_equity=initial_equity,
@@ -471,26 +479,15 @@
         return returns_df
 
 
 def ohlc_short_only_backtester(
     df: pd.DataFrame,
     short_entry_function: Callable[[pd.Series, pd.Series], bool],
     short_exit_function: Callable[[pd.Series, pd.Series, int], bool],
-    timeframe: Literal[
-        "1min",
-        "2min",
-        "5min",
-        "15min",
-        "30min",
-        "1hour",
-        "2hour",
-        "4hour",
-        "12hour",
-        "1day",
-    ],
+    timeframe: Timeframe,
     take_profit: float = np.inf,
     stop_loss: float = np.inf,
     initial_equity: int = 1000,
     maker_fees: Optional[float] = 0.001,
     taker_fees: Optional[float] = 0.001,
     get_trade_df: bool = False,
     get_returns_df: bool = False,
@@ -503,15 +500,15 @@
     ----
         df (pd.DataFrame): The dataframe containing the OHLC data.
 
         short_entry_function (Callable[[pd.Series, pd.Series], bool]): The short entry function, it should take 2 arguments, the current row and the previous row and return True or False depending on your strategy.
 
         short_exit_function (Callable[[pd.Series, pd.Series, int], bool]): The short exit function, it should take 3 arguments, the current row, the previous row and the number of timeframe count since the last entry order, and return True or False depending on your strategy.
 
-        timeframe (Literal[ &quot;1min&quot;, &quot;2min&quot;, &quot;5min&quot;, &quot;15min&quot;, &quot;30min&quot;, &quot;1hour&quot;, &quot;2hour&quot;, &quot;4hour&quot;, &quot;12hour&quot;, &quot;1day&quot;, ]): The timeframe granularity of the dataframe.
+        timeframe (Timeframe): The timeframe granularity of the dataframe.
 
         take_profit (float, optional): The percent of the buy price to add to create a stop order and take the profit associated. Defaults to np.inf.
 
         stop_loss (float, optional): The percent of the buy price to cut to create a stop order and stop the loss associated. Defaults to np.inf.
 
         initial_equity (int, optional): The initial capital. Defaults to 1000.
 
@@ -527,26 +524,17 @@
 
         plot_result (bool, optional): Plot equity, price, drawdown, distribution of the strategy. Defaults to True.
 
     Returns:
     -----
         Union[None, Union[float, Union[pd.DataFrame, Tuple[pd.DataFrame, pd.DataFrame]]]]: Nothing or the strategy total return or the trade_df or the return_df or the trade_df and the return_df.
     """
-    assert timeframe in [
-        "1min",
-        "2min",
-        "5min",
-        "15min",
-        "30min",
-        "1hour",
-        "2hour",
-        "4hour",
-        "12hour",
-        "1day",
-    ], "timeframe must be one of the following: 1min, 2min, 5min, 15min, 30min, 1hour, 2hour, 4hour, 12hour, 1day"
+    assert (
+        timeframe in TIMEFRAMES
+    ), f"timeframe must be one of the following: {','.join(TIMEFRAMES)}"
     assert df.shape[0] > 1, "Dataframe must have at least 2 rows"
     assert set({"Open", "High", "Low", "Close", "Returns"}).issubset(
         df.columns
     ), "Dataframe must have columns Open, High, Low, Close, Returns"
 
     ohlcv_df = df.copy()
     trades_df, returns_df = __ohlc_backtest_one_position_type(
@@ -579,14 +567,19 @@
     print(f"Intial balance: {initial_equity:.2f} $")
     if taker_fees is not None and maker_fees is not None:
         print(
             f"Taker fees: {taker_fees*100:.2f} %, Maker fees: {maker_fees*100:.2f} %, All the metrics will be calculated considering these fees"
         )
     else:
         print("No fees considered here.")
+    if take_profit != np.inf:
+        print(f"Take profit is set to {take_profit*100:.2f} % of the buy price")
+    if stop_loss != np.inf:
+        print(f"Stop loss is set to {stop_loss*100:.2f} % of the buy price")
+    print("Short only positions")
     print_ohlc_backtest_report(
         returns_df=returns_df,
         trades_df=trades_df,
         ohlcv_df=ohlcv_df,
         timeframe=timeframe,
         initial_equity=initial_equity,
     )
```

### Comparing `quant_invest_lab-0.2.7/quant_invest_lab/data_provider.py` & `quant_invest_lab-0.2.8/quant_invest_lab/data_provider.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,44 +6,36 @@
 import json
 import time
 from random import randint
 from kucoin.client import Market
 from concurrent.futures import ThreadPoolExecutor, as_completed
 from tqdm import tqdm
 
+from quant_invest_lab.constants import TIMEFRAME_IN_S, TIMEFRAMES
+from quant_invest_lab.types import Timeframe
+
 
 @lru_cache(maxsize=32, typed=True)
 def build_multi_crypto_dataframe(
     symbols: set,
     drop_na: bool = False,
     column_to_keep: str = "Close",
-    timeframe: Literal[
-        "1min",
-        "2min",
-        "5min",
-        "15min",
-        "30min",
-        "1hour",
-        "2hour",
-        "4hour",
-        "12hour",
-        "1day",
-    ] = "1day",
+    timeframe: Timeframe = "1day",
 ) -> pd.DataFrame:
     """Build a multi cryptocurrencies dataframe from a set of symbols. This dataframe will contain the closing price of each symbol or any other column specified in `column_to_keep`. This function is useful to build a dataframe for a multi cryptocurrencies portfolio.
 
     Args:
     -----
         symbols (set): The name of the symbols to download.
 
         drop_na (bool, optional): Whether or not to drop NaNs. Defaults to False.
 
         column_to_keep (str, optional): The name of the column to keep. Defaults to "Close".
 
-        timeframe (Literal[ &quot;1min&quot;, &quot;2min&quot;, &quot;5min&quot;, &quot;15min&quot;, &quot;30min&quot;, &quot;1hour&quot;, &quot;2hour&quot;, &quot;4hour&quot;, &quot;12hour&quot;, &quot;1day&quot;, ], optional): The data granularity. Defaults to "1day".
+        timeframe (Timeframe, optional): The data granularity. Defaults to "1day".
 
     Returns:
     -----
         pd.DataFrame: The multi cryptocurrencies dataframe.
     """
     df = pd.DataFrame()
     for symbol in tqdm(symbols, desc="Fetching symbols..."):
@@ -68,105 +60,82 @@
         )
     return df if not drop_na else df.dropna()
 
 
 @lru_cache(maxsize=32, typed=True)
 def download_crypto_historical_data(
     symbol: str,
-    timeframe: str = "1hour",
+    timeframe: Timeframe = "1hour",
     compute_return: bool = True,
     refresh_list_of_symbol: bool = True,
+    keep_timestamps_col: bool = False,
 ) -> pd.DataFrame:
     """Fetch a cryptocurrency historical data from Kucoin for a given symbol and timeframe.
 
     Args:
     ----
         symbol (str): The symbol to download.
 
-        timeframe (str, optional): The timeframe of the data to download. Defaults to "1hour".
+        timeframe (Timeframe, optional): The timeframe of the data to download. Defaults to "1hour".
 
         compute_return (bool, optional): Whether or not to compute the return on close T and T-1. Defaults to True.
 
         refresh_list_of_symbol (bool, optional): Refresh the list of symbols/ticker from kucoin, it must be true for the first execution of the code. Defaults to True.
 
+        keep_timestamps_col (bool, optional): Whether or not to keep the timestamps. Defaults to False.
+
     Returns:
     ----
         pd.DataFrame: The historical data of the symbol with date index
     """
     service = CryptoService()
     if refresh_list_of_symbol is True:
         service.refresh_list_of_symbols()  # Uncomment for the first usage
     df = service.get_history_of_symbol(f"{symbol}", timeframe)
     df["Date"] = df["Timestamp"].apply(datetime.fromtimestamp)
     df = df.set_index("Date")
     df = df.loc[~df.index.duplicated(), :]
     df = df.sort_index()
 
-    timeframe_to_freq = {
-        "1min": "1T",
-        "2min": "2T",
-        "5min": "5T",
-        "15min": "15T",
-        "30min": "30T",
-        "1hour": "1H",
-        "2hour": "2H",
-        "4hour": "4H",
-        "12hour": "12H",
-        "1day": "1D",
-    }
     if compute_return is True:
         df["Returns"] = df["Close"].pct_change()
+    if keep_timestamps_col is False:
+        df = df.drop(columns=["Timestamp"])
+
     df = df.fillna(0.0)
-    return df  # .asfreq(timeframe_to_freq[timeframe])#.ffill()
+    return df  # .asfreq(TIMEFRAME_TO_FREQ[timeframe])#.ffill()
 
 
 class CryptoService:
     class KucoinDataFetcher:
         __client = Market(url="https://api.kucoin.com")
-        __timeframes_in_s: dict[str, int] = {
-            "1min": 60,
-            "2min": 120,
-            "5min": 300,
-            "15min": 900,
-            "30min": 1800,
-            "1hour": 3600,
-            "2hour": 7200,
-            "4hour": 14400,
-            "12hour": 43200,
-            "1day": 86400,
-        }
-        timeframes: tuple[str] = tuple(__timeframes_in_s.keys())
 
         def __construct_timestamp_list(
             self,
             start_timestamp: int,
             end_timestamp: int,
-            timeframe: str,
+            timeframe: Timeframe,
             exchange_limit: int = 1500,
         ) -> list[int]:
             """Private function that generates a list of timestamps spaced of `exchange_limit` times `timeframe`.
             Args:
                 start_timestamp (str): The initial timestamp.
                 end_timestamp (str): The final timestamp.
-                timeframe (str): The desired timeframe, sould be 1min, 2min, 5min, 15min, 1hour, 4hour, 1day...
+                timeframe (Timeframe): The desired timeframe, sould be 1min, 2min, 5min, 15min, 1hour, 4hour, 1day...
                 exchange_limit (int, optional): The exchange limit : 1500 for Kucoin here.. Defaults to 1500.
             Returns:
                 list[int]: The list of timestamps.
             """
-            remaining = (end_timestamp - start_timestamp) // self.__timeframes_in_s[
-                timeframe
-            ]
+            remaining = (end_timestamp - start_timestamp) // TIMEFRAME_IN_S[timeframe]
 
             timestamp_i = end_timestamp
             timestamps = [timestamp_i]
 
             while remaining > exchange_limit:
-                timestamp_i = (
-                    timestamp_i - self.__timeframes_in_s[timeframe] * exchange_limit
-                )
+                timestamp_i = timestamp_i - TIMEFRAME_IN_S[timeframe] * exchange_limit
                 remaining = remaining - exchange_limit
                 timestamps.append(timestamp_i)
 
             timestamps.append(start_timestamp)
 
             return sorted(timestamps, reverse=True)
 
@@ -188,22 +157,26 @@
                         time.sleep(randint(10, 100) / 100)
                         pass
 
             return wrapper
 
         @__handle_429_error
         def __get_data(
-            self, symbol: str, start_at: int, end_at: int, timeframe: str = "15min"
+            self,
+            symbol: str,
+            start_at: int,
+            end_at: int,
+            timeframe: Timeframe = "15min",
         ) -> pd.DataFrame:
             """Private function that uses Kucoin API to get the data for a specific symbol and timeframe.
             Args:
                 symbol (str): The symbol for the data we want to extract. Defaults to "BTC-USDT".
                 start_at (int): The starting timestamp and. Note that this function could only outputs 1500 records. If the timeframe and the timestamps don't satisfy it, it will return a dataframe with 1500 records from the starting timestamp.
                 end_at (int): The ending timestamp.
-                timeframe (str, optional): The timeframe, it must be 1min, 2min, 5min, 15min, 1hour, 4hour, 1day... Defaults to '15min'.
+                timeframe (Timeframe, optional): The timeframe, it must be 1min, 2min, 5min, 15min, 1hour, 4hour, 1day... Defaults to '15min'.
             Returns:
                 Optional[pd.DataFrame]: The dataframe containing historical records.
             """
             klines = self.__client.get_kline(
                 f"{symbol}", timeframe, startAt=start_at, endAt=end_at
             )
             df = pd.DataFrame(
@@ -230,21 +203,21 @@
             """
             tickers = self.__client.get_all_tickers()
             if tickers is not None:
                 return [tik["symbol"] for tik in tickers["ticker"]]
             raise ValueError("Error, no symbols found.")
 
         def download_history(
-            self, symbol: str, since: str, timeframe: str, jobs: int = -1
+            self, symbol: str, since: str, timeframe: Timeframe, jobs: int = -1
         ) -> pd.DataFrame:
             """Download a set of historical data and save it.
             Args:
                 symbol (str): The symbol for the data we want to extract. Defaults to "BTC-USDT".
                 since (str): The initial date in format : dd-mm-yyyy.
-                timeframe (str): The timeframe, it must be 1min, 2min, 5min, 15min, 1hour, 4hour, 1day... Defaults to '15min'.
+                timeframe (Timeframe): The timeframe, it must be 1min, 2min, 5min, 15min, 1hour, 4hour, 1day... Defaults to '15min'.
                 jobs (int, optional): The number of thread to parallelize the code. Defaults to -1.
             Raises:
                 ValueError: Error in using parallelism.
             Returns:
                 pd.DataFrame: The dataframe containing historical records.
             """
             try:
@@ -351,60 +324,60 @@
                     lambda symbol: symbol.split("-")[0] == base_currency.upper()
                     and symbol.split("-")[-1] == quote_currency.upper(),
                     symbols,
                 )
             )
         raise ValueError("Error, wrong parameters.")
 
-    def get_history_of_symbol(self, symbol: str, timeframe: str) -> pd.DataFrame:
+    def get_history_of_symbol(self, symbol: str, timeframe: Timeframe) -> pd.DataFrame:
         """Function that get the history of a symbol.
         Args:
             symbol (str): The crypto symbol file.
-            timeframe (str): The history's timeframe.
+            timeframe (Timeframe): The history's timeframe.
         Returns:
             pd.DataFrame: Records corresponding to the history.
         """
         assert (
-            timeframe in self.__kucoin_fetcher.timeframes
-        ), f"Error, timeframe must be in {self.__kucoin_fetcher.timeframes}"
+            timeframe in TIMEFRAMES
+        ), f"Error, timeframe must be in {','.join(TIMEFRAMES)}"
 
         assert (
             symbol in self.get_list_of_symbols()
         ), "Error, wrong symbol, provide something like 'BTC-USDT'."
         return self.__refresh_or_download(symbol, timeframe)
 
     def refresh_list_of_symbols(self) -> None:
         """Function that refreshes the database's crypto listing."""
         self.__init_directories()
         with open(f"{self.__base_dir}list_available/crypto_available.json", "w") as f:
             json.dump({"listing": self.__kucoin_fetcher.get_symbols()}, f)
 
-    def check_file_exists(self, symbol: str, timeframe: str) -> bool:
+    def check_file_exists(self, symbol: str, timeframe: Timeframe) -> bool:
         """Verify if the history has already been fetched
         Args:
             symbol (str): The crypto symbol file.
-            timeframe (str): The history's timeframe.
+            timeframe (Timeframe): The history's timeframe.
         Returns:
             bool: Whether or not the history is present.
         """
         return os.path.exists(f"{self.__base_dir}{timeframe}/{symbol}.csv")
 
     def __open_symbols_list(self) -> list[str]:
         """Private function that opens, reads and returns the list of symbols from the database's file.
         Returns:
             list[str]: The list of symbols.
         """
         with open(f"{self.__base_dir}list_available/crypto_available.json", "r") as f:
             return json.load(f)["listing"]
 
-    def __refresh_or_download(self, symbol: str, timeframe: str) -> pd.DataFrame:
+    def __refresh_or_download(self, symbol: str, timeframe: Timeframe) -> pd.DataFrame:
         """Private function used to refresh or download the history of a symbol.
         Args:
             symbol (str): The crypto symbol file.
-            timeframe (str): The history's timeframe.
+            timeframe (Timeframe): The history's timeframe.
         Returns:
             pd.DataFrame: The complete history refreshed or not.
         """
         if self.check_file_exists(symbol, timeframe):
             # print("History present -> Checking for refresh...")
             data = pd.read_csv(
                 f"{self.__base_dir}{timeframe}/{symbol}.csv",
@@ -438,10 +411,10 @@
                 f"{self.__base_dir}{timeframe}/{symbol}.csv", sep=",", index=False
             )
             # print("Finished")
             return data
 
     def __init_directories(self) -> None:
         """Private function that init all directories."""
-        for tf in self.__kucoin_fetcher.timeframes:
+        for tf in TIMEFRAMES:
             os.makedirs(f"{self.__base_dir}{tf}", exist_ok=True)
         os.makedirs(f"{self.__base_dir}list_available", exist_ok=True)
```

### Comparing `quant_invest_lab-0.2.7/quant_invest_lab/indicators.py` & `quant_invest_lab-0.2.8/quant_invest_lab/indicators.py`

 * *Files identical despite different names*

### Comparing `quant_invest_lab-0.2.7/quant_invest_lab/metrics.py` & `quant_invest_lab-0.2.8/quant_invest_lab/metrics.py`

 * *Files identical despite different names*

### Comparing `quant_invest_lab-0.2.7/quant_invest_lab/optimization.py` & `quant_invest_lab-0.2.8/quant_invest_lab/optimization.py`

 * *Files identical despite different names*

### Comparing `quant_invest_lab-0.2.7/quant_invest_lab/portfolio.py` & `quant_invest_lab-0.2.8/quant_invest_lab/portfolio.py`

 * *Files identical despite different names*

### Comparing `quant_invest_lab-0.2.7/quant_invest_lab/screener.py` & `quant_invest_lab-0.2.8/quant_invest_lab/screener.py`

 * *Files identical despite different names*

### Comparing `quant_invest_lab-0.2.7/quant_invest_lab/simulation.py` & `quant_invest_lab-0.2.8/quant_invest_lab/simulation.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,14 +4,21 @@
 import numpy.typing as npt
 from typing import Literal
 import matplotlib.pyplot as plt
 from tqdm import tqdm
 from fitter import Fitter
 from psutil import cpu_count
 
+from quant_invest_lab.constants import (
+    TIMEFRAME_ANNUALIZED,
+    TIMEFRAME_TO_FREQ,
+    TIMEFRAMES,
+)
+from quant_invest_lab.types import Timeframe
+
 
 def generate_brownian_paths(
     n_paths: int,
     n_steps: int,
     T: float | int,
     mu: float | int,
     sigma: float | int,
@@ -19,16 +26,22 @@
     brownian_type: Literal["ABM", "GBM"] = "ABM",
     get_time: bool = True,
 ) -> npt.NDArray[np.float64] | tuple[npt.NDArray[np.float64], npt.NDArray[np.float64]]:
     dt = T / n_steps
     paths = np.zeros((n_paths, n_steps + 1))
     paths[:, 0] = np.log(s0)
 
-    for i in tqdm(range(0, n_paths)):
-        for j in range(n_steps):
+    for i in tqdm(
+        range(0, n_paths), desc="Simulating Brownian Motion paths...", leave=False
+    ):
+        for j in tqdm(
+            range(n_steps),
+            desc="Simulating Brownian Motion path's steps...",
+            leave=False,
+        ):
             paths[i, j + 1] = (
                 paths[i, j]
                 + (mu * 0.5 * sigma**2) * dt
                 + sigma * np.random.normal(0, np.sqrt(dt))
             )
 
     if brownian_type == "GBM":
@@ -82,15 +95,15 @@
 def generate_open(
     open_divided_by_close: pd.Series, generated_close: npt.NDArray[np.float64]
 ) -> npt.NDArray[np.float64]:
     f = Fitter(
         open_divided_by_close.values,
         distributions=["laplace"],
     )
-    f.fit(max_workers=cpu_count(), n_jobs=cpu_count())
+    f.fit(max_workers=cpu_count(), n_jobs=cpu_count(), progress=False)
     return (
         np.random.laplace(
             f.fitted_param["laplace"][0],
             f.fitted_param["laplace"][-1],
             generated_close.shape[0],
         )
     ) * generated_close
@@ -99,96 +112,65 @@
 def generate_high_coef(
     high_from_body: pd.Series, n: int = 1000
 ) -> npt.NDArray[np.float64]:
     f = Fitter(
         high_from_body.values,
         distributions=["expon"],
     )
-    f.fit(max_workers=cpu_count(), n_jobs=cpu_count())
+    f.fit(max_workers=cpu_count(), n_jobs=cpu_count(), progress=False)
 
     return 1 + np.random.exponential(f.fitted_param["expon"][-1], n)
 
 
 def generate_low_coef(
     low_from_body: pd.Series, n: int = 1000
 ) -> npt.NDArray[np.float64]:
     f = Fitter(
         low_from_body.values,
         distributions=["expon"],
     )
-    f.fit(max_workers=cpu_count(), n_jobs=cpu_count())
+    f.fit(max_workers=cpu_count(), n_jobs=cpu_count(), progress=False)
     return np.random.exponential(f.fitted_param["expon"][-1], n)
 
 
 def generate_brownian_candle_from_dataframe(
     dataframe: pd.DataFrame,
-    timeframe: Literal[
-        "1min",
-        "2min",
-        "5min",
-        "15min",
-        "30min",
-        "1hour",
-        "2hour",
-        "4hour",
-        "12hour",
-        "1day",
-    ] = "1day",
+    timeframe: Timeframe = "1day",
     generated_dataframe_length: int = 5000,
     date_index: bool = True,
+    compute_return: bool = True,
 ) -> pd.DataFrame:
     """Generate a new dataframe with the same structure (global continuous distribution) as the initial dataframe but with generated data using a geometric brownian motion.
 
     Args:
     ----
         dataframe (pd.DataFrame): The initial dataframe, it should be a real dataframe containing OHLC data. I must contains OHLC columns. This dataframe will to extract the mean return, the std return, the initial price and the distribution of the open, high and low prices.
 
-        timeframe (Literal[ &quot;1min&quot;, &quot;2min&quot;, &quot;5min&quot;, &quot;15min&quot;, &quot;30min&quot;, &quot;1hour&quot;, &quot;2hour&quot;, &quot;4hour&quot;, &quot;12hour&quot;, &quot;1day&quot;, ], optional): The timeframe or data interval frequency, it's used to compute the period parameter. Defaults to "1day".
+        timeframe (Timeframe, optional): The timeframe or data interval frequency, it's used to compute the period parameter. Defaults to "1day".
 
         generated_dataframe_length (int, optional): The number of record to generate in the new dataframe. Defaults to 5000.
 
         date_index (bool, optional): Create as of today date index. Defaults to True.
 
+        compute_return (bool, optional): Compute the returns of the generated dataframe. Defaults to True.
     Returns:
     ----
         pd.DataFrame: The generated dataframe and it's candle stick.
     """
-    assert timeframe in [
-        "1min",
-        "2min",
-        "5min",
-        "15min",
-        "30min",
-        "1hour",
-        "2hour",
-        "4hour",
-        "12hour",
-        "1day",
-    ], "timeframe must be one of the following: 1min, 2min, 5min, 15min, 30min, 1hour, 2hour, 4hour, 12hour, 1day"
+    assert (
+        timeframe in TIMEFRAMES
+    ), f"timeframe must be one of the following: {','.join(TIMEFRAMES)}"
     assert isinstance(dataframe, pd.DataFrame), "dataframe must be a pandas DataFrame"
     assert set(dataframe.columns).issuperset(
         ["Open", "High", "Low", "Close"]
     ), "dataframe must contains Open, High, Low, Close columns"
     assert (
         generated_dataframe_length >= 10
     ), "generated_dataframe_length must be greater than 10"
 
-    timeframe_annualized = {
-        "1min": int(365 * 24 / 1 * 60),
-        "2min": int(365 * 24 / 1 * 30),
-        "5min": int(365 * 24 / 1 * 12),
-        "15min": int(365 * 24 / 1 * 4),
-        "30min": int(365 * 24 / 1 * 2),
-        "1hour": int(365 * 24 / 1),
-        "2hour": int(365 * 24 / 2),
-        "4hour": int(365 * 24 / 4),
-        "12hour": int(365 * 24 / 12),
-        "1day": 365,
-    }
-
     if not "Returns" in dataframe.columns:
         dataframe["Returns"] = dataframe.Close.pct_change().fillna(0)
 
     dataframe["High_from_body"] = dataframe.apply(
         lambda row: row["High"] / row["Close"]
         if row["Open"] <= row["Close"]
         else row["High"] / row["Open"],
@@ -203,17 +185,17 @@
     )
 
     dataframe["Open_by_close"] = dataframe["Open"] / dataframe["Close"]
 
     time, sim = generate_brownian_paths(
         1,
         generated_dataframe_length - 1,
-        generated_dataframe_length / timeframe_annualized.get(timeframe, 365),
-        dataframe.Returns.mean() * timeframe_annualized.get(timeframe, 365),
-        dataframe.Returns.std() * timeframe_annualized.get(timeframe, 365) ** 0.5,
+        generated_dataframe_length / TIMEFRAME_ANNUALIZED.get(timeframe, 365),
+        dataframe.Returns.mean() * TIMEFRAME_ANNUALIZED.get(timeframe, 365),
+        dataframe.Returns.std() * TIMEFRAME_ANNUALIZED.get(timeframe, 365) ** 0.5,
         dataframe.Close.iloc[0],
         "GBM",
     )
 
     generated_close = sim[-1, :]
     generated_open = generate_open(dataframe["Open_by_close"], generated_close)
 
@@ -243,31 +225,20 @@
     generated_ohlc["Low"] = generated_ohlc.apply(
         lambda row: (1 - row["Low_from_body"]) * row["Close"]
         if row["Open"] >= row["Close"]
         else (1 - row["Low_from_body"]) * row["Open"],
         axis=1,
     )
     if date_index:
-        timeframe_to_freq = {
-            "1min": "1T",
-            "2min": "2T",
-            "5min": "5T",
-            "15min": "15T",
-            "30min": "30T",
-            "1hour": "1H",
-            "2hour": "2H",
-            "4hour": "4H",
-            "12hour": "12H",
-            "1day": "1D",
-        }
-
         generated_ohlc.set_index(
             pd.date_range(
                 end=datetime.now(),
                 periods=generated_dataframe_length,
-                freq=timeframe_to_freq[timeframe],
+                freq=TIMEFRAME_TO_FREQ[timeframe],
                 normalize=True,
                 name="Date",
             ),
             inplace=True,
         )
+    if compute_return:
+        generated_ohlc["Returns"] = generated_ohlc.Close.pct_change().fillna(0.0)
     return generated_ohlc.drop(columns=["High_from_body", "Low_from_body"])
```

### Comparing `quant_invest_lab-0.2.7/quant_invest_lab/utils.py` & `quant_invest_lab-0.2.8/quant_invest_lab/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -93,20 +93,7 @@
                 )
             return pca.transform(X)
         case "tsne":
             raise NotImplementedError("TSNE is not implemented yet")
         case _:
             raise ValueError("mode must be either pca or tsne")
 
-
-timeframe_annualized = {
-    "1min": int(365 * 24 / 1 * 60),
-    "2min": int(365 * 24 / 1 * 30),
-    "5min": int(365 * 24 / 1 * 12),
-    "15min": int(365 * 24 / 1 * 4),
-    "30min": int(365 * 24 / 1 * 2),
-    "1hour": int(365 * 24 / 1),
-    "2hour": int(365 * 24 / 2),
-    "4hour": int(365 * 24 / 4),
-    "12hour": int(365 * 24 / 12),
-    "1day": 365,
-}
```

### Comparing `quant_invest_lab-0.2.7/PKG-INFO` & `quant_invest_lab-0.2.8/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quant-invest-lab
-Version: 0.2.7
+Version: 0.2.8
 Summary: Quant Invest Lab is a python package to help you to do some quantitative experiments, while trying to learn or build quantitative investment solutions. This project was initially my own set of functionnalities but I decided to build a package for that and sharing it as open source project.
 Home-page: https://github.com/BaptisteZloch/Quant-Invest-Lab
 License: MIT
 Keywords: trading,backtest,investments,portfolio,quantitative
 Author: BaptisteZloch
 Author-email: bzloch@hotmail.fr
 Maintainer: BaptisteZloch
@@ -16,21 +16,23 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Office/Business :: Financial :: Investment
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0)
+Requires-Dist: emd-signal (>=1.4.0,<2.0.0)
 Requires-Dist: fitter (>=1.5.2,<2.0.0)
 Requires-Dist: kucoin-python (>=1.0.11,<2.0.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: nbformat (>=5.8.0,<6.0.0)
 Requires-Dist: numpy (>=1.23.5,<2.0.0)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: plotly (>=5.14.1,<6.0.0)
+Requires-Dist: pywavelets (>=1.4.1,<2.0.0)
 Requires-Dist: scikit-learn (>=1.2.2,<2.0.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Requires-Dist: seaborn (>=0.12.2,<0.13.0)
 Requires-Dist: statsmodels (>=0.14.0,<0.15.0)
 Requires-Dist: ta (>=0.10.2,<0.11.0)
 Requires-Dist: tqdm (>=4.64.1,<5.0.0)
 Project-URL: Bug Tracker, https://github.com/BaptisteZloch/Quant-Invest-Lab/issues
```

#### html2text {}

```diff
@@ -1,28 +1,29 @@
-Metadata-Version: 2.1 Name: quant-invest-lab Version: 0.2.7 Summary: Quant
+Metadata-Version: 2.1 Name: quant-invest-lab Version: 0.2.8 Summary: Quant
 Invest Lab is a python package to help you to do some quantitative experiments,
 while trying to learn or build quantitative investment solutions. This project
 was initially my own set of functionnalities but I decided to build a package
 for that and sharing it as open source project. Home-page: https://github.com/
 BaptisteZloch/Quant-Invest-Lab License: MIT Keywords:
 trading,backtest,investments,portfolio,quantitative Author: BaptisteZloch
 Author-email: bzloch@hotmail.fr Maintainer: BaptisteZloch Maintainer-email:
 bzloch@hotmail.fr Requires-Python: >=3.8,<3.12 Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Topic :: Office/
 Business :: Financial :: Investment Classifier: Topic :: Software Development
 :: Build Tools Classifier: Topic :: Software Development :: Libraries :: Python
-Modules Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0) Requires-Dist: fitter
-(>=1.5.2,<2.0.0) Requires-Dist: kucoin-python (>=1.0.11,<2.0.0) Requires-Dist:
-matplotlib (>=3.7.1,<4.0.0) Requires-Dist: nbformat (>=5.8.0,<6.0.0) Requires-
-Dist: numpy (>=1.23.5,<2.0.0) Requires-Dist: pandas (>=1.5.3,<2.0.0) Requires-
-Dist: plotly (>=5.14.1,<6.0.0) Requires-Dist: scikit-learn (>=1.2.2,<2.0.0)
-Requires-Dist: scipy (>=1.10.1,<2.0.0) Requires-Dist: seaborn
+Modules Requires-Dist: beautifulsoup4 (>=4.12.2,<5.0.0) Requires-Dist: emd-
+signal (>=1.4.0,<2.0.0) Requires-Dist: fitter (>=1.5.2,<2.0.0) Requires-Dist:
+kucoin-python (>=1.0.11,<2.0.0) Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
+Requires-Dist: nbformat (>=5.8.0,<6.0.0) Requires-Dist: numpy (>=1.23.5,<2.0.0)
+Requires-Dist: pandas (>=1.5.3,<2.0.0) Requires-Dist: plotly (>=5.14.1,<6.0.0)
+Requires-Dist: pywavelets (>=1.4.1,<2.0.0) Requires-Dist: scikit-learn
+(>=1.2.2,<2.0.0) Requires-Dist: scipy (>=1.10.1,<2.0.0) Requires-Dist: seaborn
 (>=0.12.2,<0.13.0) Requires-Dist: statsmodels (>=0.14.0,<0.15.0) Requires-Dist:
 ta (>=0.10.2,<0.11.0) Requires-Dist: tqdm (>=4.64.1,<5.0.0) Project-URL: Bug
 Tracker, https://github.com/BaptisteZloch/Quant-Invest-Lab/issues Project-URL:
 Repository, https://github.com/BaptisteZloch/Quant-Invest-Lab Description-
 Content-Type: text/markdown # Quant Invest Lab
 [PyPI] [commit update] [Code_style:_black] [Code_Climate] [GitHub_Actions_CI]
 [![contributions welcome](https://img.shields.io/badge/contributions-welcome-
```

