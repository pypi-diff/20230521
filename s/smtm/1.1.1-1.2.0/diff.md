# Comparing `tmp/smtm-1.1.1.tar.gz` & `tmp/smtm-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\smtm-1.1.1.tar", last modified: Sat Apr  1 07:28:36 2023, max compression
+gzip compressed data, was "dist\smtm-1.2.0.tar", last modified: Sun May 21 10:37:05 2023, max compression
```

## Comparing `smtm-1.1.1.tar` & `smtm-1.2.0.tar`

### file list

```diff
@@ -1,120 +1,122 @@
-drwxrwxrwx   0        0        0        0 2023-04-01 07:28:36.000000 smtm-1.1.1/
--rw-rw-rw-   0        0        0    18982 2022-04-24 14:40:18.000000 smtm-1.1.1/.pylintrc
--rwxrwxrwx   0        0        0       61 2022-04-24 14:40:18.000000 smtm-1.1.1/clear_notebook.bat
-drwxrwxrwx   0        0        0        0 2023-04-01 07:28:35.000000 smtm-1.1.1/example_data/
--rw-rw-rw-   0        0        0    12554 2022-04-24 14:40:18.000000 smtm-1.1.1/example_data/generated_config.json
--rw-rw-rw-   0        0        0    12558 2022-04-24 14:40:18.000000 smtm-1.1.1/example_data/generated_config_mix.json
--rw-rw-rw-   0        0        0      432 2022-04-24 14:40:18.000000 smtm-1.1.1/example_data/sma0_simulation.json
-drwxrwxrwx   0        0        0        0 2023-04-01 07:28:36.000000 smtm-1.1.1/integration_tests/
--rw-rw-rw-   0        0        0    10432 2022-04-24 14:40:18.000000 smtm-1.1.1/integration_tests/analyzer_ITG_test.py
--rw-rw-rw-   0        0        0      819 2022-04-24 14:40:18.000000 smtm-1.1.1/integration_tests/bithumb_data_provider_ITG_test.py
-drwxrwxrwx   0        0        0        0 2023-04-01 07:28:36.000000 smtm-1.1.1/integration_tests/data/
--rw-rw-rw-   0        0        0    17392 2022-04-24 14:40:18.000000 smtm-1.1.1/integration_tests/data/analyzer_data.py
--rw-rw-rw-   0        0        0      427 2023-03-30 14:36:30.000000 smtm-1.1.1/integration_tests/data/mass_simulation_config.json
--rw-rw-rw-   0        0        0     7919 2022-04-24 14:40:18.000000 smtm-1.1.1/integration_tests/data/simulation_data.py
--rw-rw-rw-   0        0        0   109759 2022-04-24 14:40:18.000000 smtm-1.1.1/integration_tests/data/test_report.jpg
--rw-rw-rw-   0        0        0     4809 2022-04-24 14:40:18.000000 smtm-1.1.1/integration_tests/data/test_report.txt
--rw-rw-rw-   0        0        0     5628 2023-04-01 07:06:13.000000 smtm-1.1.1/integration_tests/data_repository_ITG_test.py
--rw-rw-rw-   0        0        0      426 2022-04-24 14:40:18.000000 smtm-1.1.1/integration_tests/mass_simulator_ITG_test.py
--rw-rw-rw-   0        0        0     2342 2023-02-21 14:04:55.000000 smtm-1.1.1/integration_tests/operator_ITG_test.py
--rw-rw-rw-   0        0        0     3355 2022-04-24 14:40:18.000000 smtm-1.1.1/integration_tests/simulation_operator_ITG_test.py
--rw-rw-rw-   0        0        0     5433 2022-04-24 14:40:18.000000 smtm-1.1.1/integration_tests/simulation_trader_ITG_test.py
--rw-rw-rw-   0        0        0     1974 2023-03-30 14:37:30.000000 smtm-1.1.1/integration_tests/simulator_ITG_test.py
--rw-rw-rw-   0        0        0    11182 2022-04-24 14:40:18.000000 smtm-1.1.1/integration_tests/strategy_bnh_ITG_test.py
--rw-rw-rw-   0        0        0     3099 2022-05-15 04:12:08.000000 smtm-1.1.1/integration_tests/upbit_data_provider_ITG_test.py
--rw-rw-rw-   0        0        0      730 2023-04-01 07:10:03.000000 smtm-1.1.1/integration_tests/__init__.py
--rw-rw-rw-   0        0        0      481 2022-04-24 14:40:18.000000 smtm-1.1.1/jupyter_notebook.md
--rw-rw-rw-   0        0        0     1086 2021-12-11 06:03:04.000000 smtm-1.1.1/LICENSE
--rw-rw-rw-   0        0        0      302 2023-04-01 07:09:39.000000 smtm-1.1.1/MANIFEST.in
-drwxrwxrwx   0        0        0        0 2023-04-01 07:28:36.000000 smtm-1.1.1/notebook/
--rw-rw-rw-   0        0        0    21154 2022-04-24 14:40:18.000000 smtm-1.1.1/notebook/analyzer_exercise.ipynb
--rw-rw-rw-   0        0        0     6816 2022-04-24 14:40:18.000000 smtm-1.1.1/notebook/analyzer_test.ipynb
--rw-rw-rw-   0        0        0     1849 2022-04-24 14:40:18.000000 smtm-1.1.1/notebook/bithumb_data_provider_test.ipynb
--rw-rw-rw-   0        0        0    11784 2022-04-24 14:40:18.000000 smtm-1.1.1/notebook/bithumb_exercise.ipynb
--rw-rw-rw-   0        0        0     2990 2022-04-24 14:40:18.000000 smtm-1.1.1/notebook/bithumb_trader_test.ipynb
--rw-rw-rw-   0        0        0     2163 2022-04-24 14:40:18.000000 smtm-1.1.1/notebook/controller_test.ipynb
--rw-rw-rw-   0        0        0     4025 2023-03-31 13:38:18.000000 smtm-1.1.1/notebook/database_test.ipynb
--rw-rw-rw-   0        0        0     3578 2022-04-24 14:40:18.000000 smtm-1.1.1/notebook/data_repository_test.ipynb
--rw-rw-rw-   0        0        0     5583 2022-04-24 14:40:18.000000 smtm-1.1.1/notebook/jpt_controller.ipynb
--rw-rw-rw-   0        0        0     2880 2022-04-24 14:40:18.000000 smtm-1.1.1/notebook/logging_exercise.ipynb
--rw-rw-rw-   0        0        0     2882 2022-04-24 14:40:18.000000 smtm-1.1.1/notebook/simulation_data_provider_test.ipynb
--rw-rw-rw-   0        0        0     5676 2022-04-24 14:40:18.000000 smtm-1.1.1/notebook/simulation_operator_test.ipynb
--rw-rw-rw-   0        0        0     3206 2022-04-24 14:40:18.000000 smtm-1.1.1/notebook/simulation_trader_test.ipynb
--rw-rw-rw-   0        0        0     5163 2022-04-24 14:40:18.000000 smtm-1.1.1/notebook/strategy_bnh_test.ipynb
--rw-rw-rw-   0        0        0     1846 2022-04-24 14:40:18.000000 smtm-1.1.1/notebook/upbit_data_provider_test.ipynb
--rw-rw-rw-   0        0        0    13493 2022-04-24 14:40:18.000000 smtm-1.1.1/notebook/upbit_exercise.ipynb
--rw-rw-rw-   0        0        0     3445 2022-04-24 14:40:18.000000 smtm-1.1.1/notebook/upbit_trader_test.ipynb
--rw-rw-rw-   0        0        0     6716 2023-04-01 07:28:36.000000 smtm-1.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     6086 2023-03-19 04:31:29.000000 smtm-1.1.1/README-en_us.md
--rw-rw-rw-   0        0        0     9088 2023-03-19 04:26:38.000000 smtm-1.1.1/README.md
--rw-rw-rw-   0        0        0     2350 2023-03-19 05:57:17.000000 smtm-1.1.1/RELEASE_NOTES.md
--rw-rw-rw-   0        0        0      194 2022-04-24 14:40:18.000000 smtm-1.1.1/requirements-dev.txt
--rw-rw-rw-   0        0        0      178 2022-04-24 14:40:18.000000 smtm-1.1.1/requirements.txt
--rwxrwxrwx   0        0        0       36 2023-04-01 07:09:34.000000 smtm-1.1.1/run_integration_test.bat
--rwxrwxrwx   0        0        0       47 2022-04-24 14:40:18.000000 smtm-1.1.1/run_unittest.bat
--rw-rw-rw-   0        0        0      901 2023-04-01 07:28:36.000000 smtm-1.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1353 2023-04-01 07:19:47.000000 smtm-1.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-01 07:28:36.000000 smtm-1.1.1/smtm/
--rw-rw-rw-   0        0        0    30804 2023-03-18 05:03:53.000000 smtm-1.1.1/smtm/analyzer.py
--rw-rw-rw-   0        0        0     3424 2022-04-24 14:40:18.000000 smtm-1.1.1/smtm/bithumb_data_provider.py
--rw-rw-rw-   0        0        0    19358 2022-04-24 14:40:18.000000 smtm-1.1.1/smtm/bithumb_trader.py
--rw-rw-rw-   0        0        0     6070 2023-03-30 14:20:07.000000 smtm-1.1.1/smtm/controller.py
--rw-rw-rw-   0        0        0     3471 2022-04-24 14:40:18.000000 smtm-1.1.1/smtm/database.py
--rw-rw-rw-   0        0        0      960 2022-04-24 14:40:18.000000 smtm-1.1.1/smtm/data_provider.py
--rw-rw-rw-   0        0        0     9684 2022-04-24 14:40:18.000000 smtm-1.1.1/smtm/data_repository.py
--rw-rw-rw-   0        0        0     3687 2022-04-24 14:40:18.000000 smtm-1.1.1/smtm/date_converter.py
--rw-rw-rw-   0        0        0     7488 2023-03-15 15:28:14.000000 smtm-1.1.1/smtm/demo_trader.py
--rw-rw-rw-   0        0        0     4517 2023-03-30 13:40:53.000000 smtm-1.1.1/smtm/jpt_controller.py
--rw-rw-rw-   0        0        0     2618 2023-03-26 11:48:56.000000 smtm-1.1.1/smtm/log_manager.py
--rw-rw-rw-   0        0        0    16888 2023-03-31 13:05:21.000000 smtm-1.1.1/smtm/mass_simulator.py
--rw-rw-rw-   0        0        0    10045 2023-02-21 14:04:55.000000 smtm-1.1.1/smtm/operator.py
--rw-rw-rw-   0        0        0     2119 2022-05-15 04:12:08.000000 smtm-1.1.1/smtm/simulation_data_provider.py
--rw-rw-rw-   0        0        0     5572 2022-05-15 04:12:32.000000 smtm-1.1.1/smtm/simulation_operator.py
--rw-rw-rw-   0        0        0     3838 2022-05-15 04:12:08.000000 smtm-1.1.1/smtm/simulation_trader.py
--rw-rw-rw-   0        0        0    10344 2023-03-30 14:52:44.000000 smtm-1.1.1/smtm/simulator.py
--rw-rw-rw-   0        0        0     2389 2023-03-30 14:19:57.000000 smtm-1.1.1/smtm/strategy.py
--rw-rw-rw-   0        0        0     7332 2023-03-31 12:39:37.000000 smtm-1.1.1/smtm/strategy_bnh.py
--rw-rw-rw-   0        0        0      907 2023-03-30 14:04:18.000000 smtm-1.1.1/smtm/strategy_factory.py
--rw-rw-rw-   0        0        0    12575 2023-03-31 12:39:41.000000 smtm-1.1.1/smtm/strategy_rsi.py
--rw-rw-rw-   0        0        0    13422 2023-03-29 14:48:19.000000 smtm-1.1.1/smtm/strategy_sma_0.py
--rw-rw-rw-   0        0        0    20845 2023-03-31 12:39:23.000000 smtm-1.1.1/smtm/telegram_controller.py
--rw-rw-rw-   0        0        0     2244 2022-04-24 14:40:18.000000 smtm-1.1.1/smtm/trader.py
--rw-rw-rw-   0        0        0     3137 2022-05-15 04:12:08.000000 smtm-1.1.1/smtm/upbit_data_provider.py
--rw-rw-rw-   0        0        0    22159 2023-03-15 15:36:19.000000 smtm-1.1.1/smtm/upbit_trader.py
--rw-rw-rw-   0        0        0     8816 2022-04-24 14:40:18.000000 smtm-1.1.1/smtm/virtual_market.py
--rw-rw-rw-   0        0        0     2836 2023-02-21 14:04:55.000000 smtm-1.1.1/smtm/worker.py
--rw-rw-rw-   0        0        0     1692 2023-04-01 07:20:00.000000 smtm-1.1.1/smtm/__init__.py
--rw-rw-rw-   0        0        0     5451 2023-03-31 12:55:07.000000 smtm-1.1.1/smtm/__main__.py
-drwxrwxrwx   0        0        0        0 2023-04-01 07:28:36.000000 smtm-1.1.1/smtm.egg-info/
--rw-rw-rw-   0        0        0        1 2023-04-01 07:28:35.000000 smtm-1.1.1/smtm.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-01 07:28:35.000000 smtm-1.1.1/smtm.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0     6716 2023-04-01 07:28:35.000000 smtm-1.1.1/smtm.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0       95 2023-04-01 07:28:35.000000 smtm-1.1.1/smtm.egg-info/requires.txt
--rw-rw-rw-   0        0        0     3135 2023-04-01 07:28:35.000000 smtm-1.1.1/smtm.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        5 2023-04-01 07:28:35.000000 smtm-1.1.1/smtm.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-01 07:28:36.000000 smtm-1.1.1/tests/
--rw-rw-rw-   0        0        0    60979 2023-03-29 14:31:28.000000 smtm-1.1.1/tests/analyzer_test.py
--rw-rw-rw-   0        0        0     2741 2022-04-24 14:40:18.000000 smtm-1.1.1/tests/bithumb_data_provider_test.py
--rw-rw-rw-   0        0        0    26065 2023-03-29 14:31:40.000000 smtm-1.1.1/tests/bithumb_trader_test.py
--rw-rw-rw-   0        0        0     5128 2022-04-24 14:40:18.000000 smtm-1.1.1/tests/controller_test.py
--rw-rw-rw-   0        0        0     4685 2023-03-29 14:32:09.000000 smtm-1.1.1/tests/database_test.py
--rw-rw-rw-   0        0        0    23792 2023-03-29 14:32:01.000000 smtm-1.1.1/tests/data_repository_test.py
--rw-rw-rw-   0        0        0    10700 2022-04-24 14:40:18.000000 smtm-1.1.1/tests/date_converter_test.py
--rw-rw-rw-   0        0        0     4687 2023-03-15 15:28:37.000000 smtm-1.1.1/tests/demo_trader_test.py
--rw-rw-rw-   0        0        0     5110 2023-03-30 14:15:13.000000 smtm-1.1.1/tests/jpt_controller_test.py
--rw-rw-rw-   0        0        0     2025 2023-03-26 11:48:27.000000 smtm-1.1.1/tests/log_manager_test.py
--rw-rw-rw-   0        0        0    16228 2023-03-31 13:02:02.000000 smtm-1.1.1/tests/mass_simulator_test.py
--rw-rw-rw-   0        0        0    15823 2023-03-29 14:32:46.000000 smtm-1.1.1/tests/operator_test.py
--rw-rw-rw-   0        0        0     1504 2023-03-29 14:32:53.000000 smtm-1.1.1/tests/simulation_data_provider_test.py
--rw-rw-rw-   0        0        0     7921 2023-03-29 14:32:58.000000 smtm-1.1.1/tests/simulation_operator_test.py
--rw-rw-rw-   0        0        0     3556 2023-03-29 14:33:04.000000 smtm-1.1.1/tests/simulation_trader_test.py
--rw-rw-rw-   0        0        0     8240 2023-03-31 13:01:58.000000 smtm-1.1.1/tests/simulator_test.py
--rw-rw-rw-   0        0        0    11192 2022-04-24 14:40:18.000000 smtm-1.1.1/tests/strategy_bnh_test.py
--rw-rw-rw-   0        0        0     1842 2023-03-30 14:04:13.000000 smtm-1.1.1/tests/strategy_factory_test.py
--rw-rw-rw-   0        0        0     7763 2023-02-21 14:04:55.000000 smtm-1.1.1/tests/strategy_rsi_test.py
--rw-rw-rw-   0        0        0    18247 2022-05-15 04:12:08.000000 smtm-1.1.1/tests/strategy_sma_0_test.py
--rw-rw-rw-   0        0        0    24099 2023-03-30 14:13:22.000000 smtm-1.1.1/tests/telegram_controller_test.py
--rw-rw-rw-   0        0        0     3146 2022-04-24 14:40:18.000000 smtm-1.1.1/tests/upbit_data_provider_test.py
--rw-rw-rw-   0        0        0    43207 2023-03-29 14:33:26.000000 smtm-1.1.1/tests/upbit_trader_test.py
--rw-rw-rw-   0        0        0    24905 2023-03-29 14:33:40.000000 smtm-1.1.1/tests/virtual_market_test.py
--rw-rw-rw-   0        0        0     2039 2023-03-29 14:33:49.000000 smtm-1.1.1/tests/worker_test.py
+drwxrwxrwx   0        0        0        0 2023-05-21 10:37:05.000000 smtm-1.2.0/
+-rw-rw-rw-   0        0        0    18982 2022-04-24 14:40:18.000000 smtm-1.2.0/.pylintrc
+-rwxrwxrwx   0        0        0       61 2022-04-24 14:40:18.000000 smtm-1.2.0/clear_notebook.bat
+drwxrwxrwx   0        0        0        0 2023-05-21 10:37:04.000000 smtm-1.2.0/example_data/
+-rw-rw-rw-   0        0        0    12554 2022-04-24 14:40:18.000000 smtm-1.2.0/example_data/generated_config.json
+-rw-rw-rw-   0        0        0    12558 2022-04-24 14:40:18.000000 smtm-1.2.0/example_data/generated_config_mix.json
+-rw-rw-rw-   0        0        0      432 2022-04-24 14:40:18.000000 smtm-1.2.0/example_data/sma0_simulation.json
+drwxrwxrwx   0        0        0        0 2023-05-21 10:37:04.000000 smtm-1.2.0/integration_tests/
+-rw-rw-rw-   0        0        0    10432 2022-04-24 14:40:18.000000 smtm-1.2.0/integration_tests/analyzer_ITG_test.py
+-rw-rw-rw-   0        0        0      819 2022-04-24 14:40:18.000000 smtm-1.2.0/integration_tests/bithumb_data_provider_ITG_test.py
+drwxrwxrwx   0        0        0        0 2023-05-21 10:37:04.000000 smtm-1.2.0/integration_tests/data/
+-rw-rw-rw-   0        0        0    17392 2022-04-24 14:40:18.000000 smtm-1.2.0/integration_tests/data/analyzer_data.py
+-rw-rw-rw-   0        0        0      427 2023-03-30 14:36:30.000000 smtm-1.2.0/integration_tests/data/mass_simulation_config.json
+-rw-rw-rw-   0        0        0     7919 2022-04-24 14:40:18.000000 smtm-1.2.0/integration_tests/data/simulation_data.py
+-rw-rw-rw-   0        0        0   109759 2022-04-24 14:40:18.000000 smtm-1.2.0/integration_tests/data/test_report.jpg
+-rw-rw-rw-   0        0        0     4809 2022-04-24 14:40:18.000000 smtm-1.2.0/integration_tests/data/test_report.txt
+-rw-rw-rw-   0        0        0     5628 2023-04-01 07:06:13.000000 smtm-1.2.0/integration_tests/data_repository_ITG_test.py
+-rw-rw-rw-   0        0        0      426 2022-04-24 14:40:18.000000 smtm-1.2.0/integration_tests/mass_simulator_ITG_test.py
+-rw-rw-rw-   0        0        0     2342 2023-02-21 14:04:55.000000 smtm-1.2.0/integration_tests/operator_ITG_test.py
+-rw-rw-rw-   0        0        0     8477 2023-04-12 12:18:59.000000 smtm-1.2.0/integration_tests/simulation_operator_ITG_test.py
+-rw-rw-rw-   0        0        0     5433 2022-04-24 14:40:18.000000 smtm-1.2.0/integration_tests/simulation_trader_ITG_test.py
+-rw-rw-rw-   0        0        0     1974 2023-03-30 14:37:30.000000 smtm-1.2.0/integration_tests/simulator_ITG_test.py
+-rw-rw-rw-   0        0        0    11182 2022-04-24 14:40:18.000000 smtm-1.2.0/integration_tests/strategy_bnh_ITG_test.py
+-rw-rw-rw-   0        0        0     3099 2022-05-15 04:12:08.000000 smtm-1.2.0/integration_tests/upbit_data_provider_ITG_test.py
+-rw-rw-rw-   0        0        0      727 2023-04-12 12:18:59.000000 smtm-1.2.0/integration_tests/__init__.py
+-rw-rw-rw-   0        0        0      481 2022-04-24 14:40:18.000000 smtm-1.2.0/jupyter_notebook.md
+-rw-rw-rw-   0        0        0     1086 2021-12-11 06:03:04.000000 smtm-1.2.0/LICENSE
+-rw-rw-rw-   0        0        0      302 2023-04-01 07:09:39.000000 smtm-1.2.0/MANIFEST.in
+drwxrwxrwx   0        0        0        0 2023-05-21 10:37:05.000000 smtm-1.2.0/notebook/
+-rw-rw-rw-   0        0        0    21154 2022-04-24 14:40:18.000000 smtm-1.2.0/notebook/analyzer_exercise.ipynb
+-rw-rw-rw-   0        0        0     6816 2022-04-24 14:40:18.000000 smtm-1.2.0/notebook/analyzer_test.ipynb
+-rw-rw-rw-   0        0        0     1849 2022-04-24 14:40:18.000000 smtm-1.2.0/notebook/bithumb_data_provider_test.ipynb
+-rw-rw-rw-   0        0        0    11784 2022-04-24 14:40:18.000000 smtm-1.2.0/notebook/bithumb_exercise.ipynb
+-rw-rw-rw-   0        0        0     2990 2022-04-24 14:40:18.000000 smtm-1.2.0/notebook/bithumb_trader_test.ipynb
+-rw-rw-rw-   0        0        0     2163 2022-04-24 14:40:18.000000 smtm-1.2.0/notebook/controller_test.ipynb
+-rw-rw-rw-   0        0        0     4025 2023-03-31 13:38:18.000000 smtm-1.2.0/notebook/database_test.ipynb
+-rw-rw-rw-   0        0        0     3578 2022-04-24 14:40:18.000000 smtm-1.2.0/notebook/data_repository_test.ipynb
+-rw-rw-rw-   0        0        0     5583 2022-04-24 14:40:18.000000 smtm-1.2.0/notebook/jpt_controller.ipynb
+-rw-rw-rw-   0        0        0     2880 2022-04-24 14:40:18.000000 smtm-1.2.0/notebook/logging_exercise.ipynb
+-rw-rw-rw-   0        0        0     2882 2022-04-24 14:40:18.000000 smtm-1.2.0/notebook/simulation_data_provider_test.ipynb
+-rw-rw-rw-   0        0        0     5676 2022-04-24 14:40:18.000000 smtm-1.2.0/notebook/simulation_operator_test.ipynb
+-rw-rw-rw-   0        0        0     3206 2022-04-24 14:40:18.000000 smtm-1.2.0/notebook/simulation_trader_test.ipynb
+-rw-rw-rw-   0        0        0     5163 2022-04-24 14:40:18.000000 smtm-1.2.0/notebook/strategy_bnh_test.ipynb
+-rw-rw-rw-   0        0        0     1846 2022-04-24 14:40:18.000000 smtm-1.2.0/notebook/upbit_data_provider_test.ipynb
+-rw-rw-rw-   0        0        0    13493 2022-04-24 14:40:18.000000 smtm-1.2.0/notebook/upbit_exercise.ipynb
+-rw-rw-rw-   0        0        0     3445 2022-04-24 14:40:18.000000 smtm-1.2.0/notebook/upbit_trader_test.ipynb
+-rw-rw-rw-   0        0        0     6734 2023-05-21 10:37:05.000000 smtm-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     6104 2023-04-09 15:09:51.000000 smtm-1.2.0/README-en_us.md
+-rw-rw-rw-   0        0        0     9106 2023-04-09 15:09:41.000000 smtm-1.2.0/README.md
+-rw-rw-rw-   0        0        0     4861 2023-05-21 10:32:16.000000 smtm-1.2.0/RELEASE_NOTES.md
+-rw-rw-rw-   0        0        0      226 2023-04-12 12:18:59.000000 smtm-1.2.0/requirements-dev.txt
+-rw-rw-rw-   0        0        0      206 2023-04-12 12:18:59.000000 smtm-1.2.0/requirements.txt
+-rwxrwxrwx   0        0        0       36 2023-04-01 07:09:34.000000 smtm-1.2.0/run_integration_test.bat
+-rwxrwxrwx   0        0        0       47 2022-04-24 14:40:18.000000 smtm-1.2.0/run_unittest.bat
+-rw-rw-rw-   0        0        0      916 2023-05-21 10:37:05.000000 smtm-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1359 2023-05-21 10:35:03.000000 smtm-1.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-21 10:37:05.000000 smtm-1.2.0/smtm/
+-rw-rw-rw-   0        0        0    30804 2023-03-18 05:03:53.000000 smtm-1.2.0/smtm/analyzer.py
+-rw-rw-rw-   0        0        0     3424 2022-04-24 14:40:18.000000 smtm-1.2.0/smtm/bithumb_data_provider.py
+-rw-rw-rw-   0        0        0    19358 2022-04-24 14:40:18.000000 smtm-1.2.0/smtm/bithumb_trader.py
+-rw-rw-rw-   0        0        0     6070 2023-03-30 14:20:07.000000 smtm-1.2.0/smtm/controller.py
+-rw-rw-rw-   0        0        0     3471 2022-04-24 14:40:18.000000 smtm-1.2.0/smtm/database.py
+-rw-rw-rw-   0        0        0      960 2022-04-24 14:40:18.000000 smtm-1.2.0/smtm/data_provider.py
+-rw-rw-rw-   0        0        0     9684 2022-04-24 14:40:18.000000 smtm-1.2.0/smtm/data_repository.py
+-rw-rw-rw-   0        0        0     3687 2022-04-24 14:40:18.000000 smtm-1.2.0/smtm/date_converter.py
+-rw-rw-rw-   0        0        0     7488 2023-03-15 15:28:14.000000 smtm-1.2.0/smtm/demo_trader.py
+-rw-rw-rw-   0        0        0     4517 2023-03-30 13:40:53.000000 smtm-1.2.0/smtm/jpt_controller.py
+-rw-rw-rw-   0        0        0     2618 2023-04-09 12:39:35.000000 smtm-1.2.0/smtm/log_manager.py
+-rw-rw-rw-   0        0        0    16998 2023-04-18 14:14:43.000000 smtm-1.2.0/smtm/mass_simulator.py
+-rw-rw-rw-   0        0        0    10201 2023-04-18 14:15:27.000000 smtm-1.2.0/smtm/operator.py
+-rw-rw-rw-   0        0        0     2119 2022-05-15 04:12:08.000000 smtm-1.2.0/smtm/simulation_data_provider.py
+-rw-rw-rw-   0        0        0     5572 2022-05-15 04:12:32.000000 smtm-1.2.0/smtm/simulation_operator.py
+-rw-rw-rw-   0        0        0     3838 2022-05-15 04:12:08.000000 smtm-1.2.0/smtm/simulation_trader.py
+-rw-rw-rw-   0        0        0    10344 2023-04-10 15:10:25.000000 smtm-1.2.0/smtm/simulator.py
+-rw-rw-rw-   0        0        0     2389 2023-03-30 14:19:57.000000 smtm-1.2.0/smtm/strategy.py
+-rw-rw-rw-   0        0        0     7332 2023-03-31 12:39:37.000000 smtm-1.2.0/smtm/strategy_bnh.py
+-rw-rw-rw-   0        0        0      937 2023-04-12 12:18:59.000000 smtm-1.2.0/smtm/strategy_factory.py
+-rw-rw-rw-   0        0        0    12575 2023-03-31 12:39:41.000000 smtm-1.2.0/smtm/strategy_rsi.py
+-rw-rw-rw-   0        0        0    13422 2023-03-29 14:48:19.000000 smtm-1.2.0/smtm/strategy_sma_0.py
+-rw-rw-rw-   0        0        0    14331 2023-04-12 12:18:59.000000 smtm-1.2.0/smtm/strategy_sma_ml.py
+-rw-rw-rw-   0        0        0    20861 2023-04-09 07:00:15.000000 smtm-1.2.0/smtm/telegram_controller.py
+-rw-rw-rw-   0        0        0     2244 2022-04-24 14:40:18.000000 smtm-1.2.0/smtm/trader.py
+-rw-rw-rw-   0        0        0     3137 2022-05-15 04:12:08.000000 smtm-1.2.0/smtm/upbit_data_provider.py
+-rw-rw-rw-   0        0        0    22159 2023-03-15 15:36:19.000000 smtm-1.2.0/smtm/upbit_trader.py
+-rw-rw-rw-   0        0        0     8816 2022-04-24 14:40:18.000000 smtm-1.2.0/smtm/virtual_market.py
+-rw-rw-rw-   0        0        0     2836 2023-02-21 14:04:55.000000 smtm-1.2.0/smtm/worker.py
+-rw-rw-rw-   0        0        0     1758 2023-05-21 10:35:13.000000 smtm-1.2.0/smtm/__init__.py
+-rw-rw-rw-   0        0        0     5451 2023-03-31 12:55:07.000000 smtm-1.2.0/smtm/__main__.py
+drwxrwxrwx   0        0        0        0 2023-05-21 10:37:05.000000 smtm-1.2.0/smtm.egg-info/
+-rw-rw-rw-   0        0        0        1 2023-05-21 10:37:04.000000 smtm-1.2.0/smtm.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-01 07:28:35.000000 smtm-1.2.0/smtm.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0     6734 2023-05-21 10:37:04.000000 smtm-1.2.0/smtm.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      108 2023-05-21 10:37:04.000000 smtm-1.2.0/smtm.egg-info/requires.txt
+-rw-rw-rw-   0        0        0     3189 2023-05-21 10:37:04.000000 smtm-1.2.0/smtm.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        5 2023-05-21 10:37:04.000000 smtm-1.2.0/smtm.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-21 10:37:05.000000 smtm-1.2.0/tests/
+-rw-rw-rw-   0        0        0    60979 2023-03-29 14:31:28.000000 smtm-1.2.0/tests/analyzer_test.py
+-rw-rw-rw-   0        0        0     2741 2022-04-24 14:40:18.000000 smtm-1.2.0/tests/bithumb_data_provider_test.py
+-rw-rw-rw-   0        0        0    26065 2023-03-29 14:31:40.000000 smtm-1.2.0/tests/bithumb_trader_test.py
+-rw-rw-rw-   0        0        0     5128 2022-04-24 14:40:18.000000 smtm-1.2.0/tests/controller_test.py
+-rw-rw-rw-   0        0        0     4685 2023-03-29 14:32:09.000000 smtm-1.2.0/tests/database_test.py
+-rw-rw-rw-   0        0        0    23792 2023-03-29 14:32:01.000000 smtm-1.2.0/tests/data_repository_test.py
+-rw-rw-rw-   0        0        0    10700 2022-04-24 14:40:18.000000 smtm-1.2.0/tests/date_converter_test.py
+-rw-rw-rw-   0        0        0     4687 2023-03-15 15:28:37.000000 smtm-1.2.0/tests/demo_trader_test.py
+-rw-rw-rw-   0        0        0     5110 2023-03-30 14:15:13.000000 smtm-1.2.0/tests/jpt_controller_test.py
+-rw-rw-rw-   0        0        0     2025 2023-04-09 11:19:05.000000 smtm-1.2.0/tests/log_manager_test.py
+-rw-rw-rw-   0        0        0    16228 2023-03-31 13:02:02.000000 smtm-1.2.0/tests/mass_simulator_test.py
+-rw-rw-rw-   0        0        0    15813 2023-04-10 15:18:11.000000 smtm-1.2.0/tests/operator_test.py
+-rw-rw-rw-   0        0        0     1504 2023-03-29 14:32:53.000000 smtm-1.2.0/tests/simulation_data_provider_test.py
+-rw-rw-rw-   0        0        0     7901 2023-04-10 15:16:33.000000 smtm-1.2.0/tests/simulation_operator_test.py
+-rw-rw-rw-   0        0        0     3556 2023-03-29 14:33:04.000000 smtm-1.2.0/tests/simulation_trader_test.py
+-rw-rw-rw-   0        0        0     8240 2023-03-31 13:01:58.000000 smtm-1.2.0/tests/simulator_test.py
+-rw-rw-rw-   0        0        0    11192 2022-04-24 14:40:18.000000 smtm-1.2.0/tests/strategy_bnh_test.py
+-rw-rw-rw-   0        0        0     2197 2023-04-12 12:18:59.000000 smtm-1.2.0/tests/strategy_factory_test.py
+-rw-rw-rw-   0        0        0     7763 2023-02-21 14:04:55.000000 smtm-1.2.0/tests/strategy_rsi_test.py
+-rw-rw-rw-   0        0        0    18247 2022-05-15 04:12:08.000000 smtm-1.2.0/tests/strategy_sma_0_test.py
+-rw-rw-rw-   0        0        0     5349 2023-04-12 12:18:59.000000 smtm-1.2.0/tests/strategy_sma_ml_test.py
+-rw-rw-rw-   0        0        0    24091 2023-04-09 13:45:15.000000 smtm-1.2.0/tests/telegram_controller_test.py
+-rw-rw-rw-   0        0        0     3146 2022-04-24 14:40:18.000000 smtm-1.2.0/tests/upbit_data_provider_test.py
+-rw-rw-rw-   0        0        0    43207 2023-03-29 14:33:26.000000 smtm-1.2.0/tests/upbit_trader_test.py
+-rw-rw-rw-   0        0        0    24905 2023-03-29 14:33:40.000000 smtm-1.2.0/tests/virtual_market_test.py
+-rw-rw-rw-   0        0        0     2039 2023-03-29 14:33:49.000000 smtm-1.2.0/tests/worker_test.py
```

### Comparing `smtm-1.1.1/.pylintrc` & `smtm-1.2.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `smtm-1.1.1/example_data/generated_config.json` & `smtm-1.2.0/example_data/generated_config.json`

 * *Files identical despite different names*

### Comparing `smtm-1.1.1/example_data/generated_config_mix.json` & `smtm-1.2.0/example_data/generated_config_mix.json`

 * *Files identical despite different names*

### Comparing `smtm-1.1.1/integration_tests/analyzer_ITG_test.py` & `smtm-1.2.0/integration_tests/analyzer_ITG_test.py`

 * *Files identical despite different names*

### Comparing `smtm-1.1.1/integration_tests/bithumb_data_provider_ITG_test.py` & `smtm-1.2.0/integration_tests/bithumb_data_provider_ITG_test.py`

 * *Files identical despite different names*

### Comparing `smtm-1.1.1/integration_tests/data/analyzer_data.py` & `smtm-1.2.0/integration_tests/data/analyzer_data.py`

 * *Files identical despite different names*

### Comparing `smtm-1.1.1/integration_tests/data/simulation_data.py` & `smtm-1.2.0/integration_tests/data/simulation_data.py`

 * *Files identical despite different names*

### Comparing `smtm-1.1.1/integration_tests/data/test_report.jpg` & `smtm-1.2.0/integration_tests/data/test_report.jpg`

 * *Files identical despite different names*

### Comparing `smtm-1.1.1/integration_tests/data/test_report.txt` & `smtm-1.2.0/integration_tests/data/test_report.txt`

 * *Files identical despite different names*

### Comparing `smtm-1.1.1/integration_tests/data_repository_ITG_test.py` & `smtm-1.2.0/integration_tests/data_repository_ITG_test.py`

 * *Files identical despite different names*

### Comparing `smtm-1.1.1/integration_tests/operator_ITG_test.py` & `smtm-1.2.0/integration_tests/operator_ITG_test.py`

 * *Files identical despite different names*

### Comparing `smtm-1.1.1/integration_tests/simulation_trader_ITG_test.py` & `smtm-1.2.0/integration_tests/simulation_trader_ITG_test.py`

 * *Files identical despite different names*

### Comparing `smtm-1.1.1/integration_tests/simulator_ITG_test.py` & `smtm-1.2.0/integration_tests/simulator_ITG_test.py`

 * *Files identical despite different names*

### Comparing `smtm-1.1.1/integration_tests/strategy_bnh_ITG_test.py` & `smtm-1.2.0/integration_tests/strategy_bnh_ITG_test.py`

 * *Files identical despite different names*

### Comparing `smtm-1.1.1/integration_tests/upbit_data_provider_ITG_test.py` & `smtm-1.2.0/integration_tests/upbit_data_provider_ITG_test.py`

 * *Files identical despite different names*

### Comparing `smtm-1.1.1/integration_tests/__init__.py` & `smtm-1.2.0/integration_tests/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
 Description for Package
 """
 from .analyzer_ITG_test import AnalyzerIntegrationTests
 from .bithumb_data_provider_ITG_test import BithumbDataProviderIntegrationTests
 from .operator_ITG_test import OperatorIntegrationTests
-from .simulation_operator_ITG_test import SimulationOperatorIntegrationBnhTests
+from .simulation_operator_ITG_test import SimulationOperatorIntegrationTests
 from .simulation_trader_ITG_test import SimulationTraderIntegrationTests
 from .strategy_bnh_ITG_test import StrategyBuyAndHoldIntegrationTests
 from .upbit_data_provider_ITG_test import UpbitDataProviderIntegrationTests
 from .simulator_ITG_test import SimulatorIntegrationTests
 from .data_repository_ITG_test import DataRepositoryIntegrationTests
 from .mass_simulator_ITG_test import MassSimulatorIntegrationTests
```

### Comparing `smtm-1.1.1/LICENSE` & `smtm-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `smtm-1.1.1/notebook/analyzer_exercise.ipynb` & `smtm-1.2.0/notebook/analyzer_exercise.ipynb`

 * *Files identical despite different names*

### Comparing `smtm-1.1.1/notebook/analyzer_test.ipynb` & `smtm-1.2.0/notebook/analyzer_test.ipynb`

 * *Files identical despite different names*

### Comparing `smtm-1.1.1/notebook/bithumb_data_provider_test.ipynb` & `smtm-1.2.0/notebook/bithumb_data_provider_test.ipynb`

 * *Files identical despite different names*

### Comparing `smtm-1.1.1/notebook/bithumb_exercise.ipynb` & `smtm-1.2.0/notebook/bithumb_exercise.ipynb`

 * *Files identical despite different names*

### Comparing `smtm-1.1.1/notebook/bithumb_trader_test.ipynb` & `smtm-1.2.0/notebook/bithumb_trader_test.ipynb`

 * *Files identical despite different names*

### Comparing `smtm-1.1.1/notebook/controller_test.ipynb` & `smtm-1.2.0/notebook/controller_test.ipynb`

 * *Files identical despite different names*

### Comparing `smtm-1.1.1/notebook/database_test.ipynb` & `smtm-1.2.0/notebook/database_test.ipynb`

 * *Files identical despite different names*

### Comparing `smtm-1.1.1/notebook/data_repository_test.ipynb` & `smtm-1.2.0/notebook/data_repository_test.ipynb`

 * *Files identical despite different names*

### Comparing `smtm-1.1.1/notebook/jpt_controller.ipynb` & `smtm-1.2.0/notebook/jpt_controller.ipynb`

 * *Files identical despite different names*

### Comparing `smtm-1.1.1/notebook/logging_exercise.ipynb` & `smtm-1.2.0/notebook/logging_exercise.ipynb`

 * *Files identical despite different names*

### Comparing `smtm-1.1.1/notebook/simulation_data_provider_test.ipynb` & `smtm-1.2.0/notebook/simulation_data_provider_test.ipynb`

 * *Files identical despite different names*

### Comparing `smtm-1.1.1/notebook/simulation_operator_test.ipynb` & `smtm-1.2.0/notebook/simulation_operator_test.ipynb`

 * *Files identical despite different names*

### Comparing `smtm-1.1.1/notebook/simulation_trader_test.ipynb` & `smtm-1.2.0/notebook/simulation_trader_test.ipynb`

 * *Files identical despite different names*

### Comparing `smtm-1.1.1/notebook/strategy_bnh_test.ipynb` & `smtm-1.2.0/notebook/strategy_bnh_test.ipynb`

 * *Files identical despite different names*

### Comparing `smtm-1.1.1/notebook/upbit_data_provider_test.ipynb` & `smtm-1.2.0/notebook/upbit_data_provider_test.ipynb`

 * *Files identical despite different names*

### Comparing `smtm-1.1.1/notebook/upbit_exercise.ipynb` & `smtm-1.2.0/notebook/upbit_exercise.ipynb`

 * *Files identical despite different names*

### Comparing `smtm-1.1.1/notebook/upbit_trader_test.ipynb` & `smtm-1.2.0/notebook/upbit_trader_test.ipynb`

 * *Files identical despite different names*

### Comparing `smtm-1.1.1/PKG-INFO` & `smtm-1.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smtm
-Version: 1.1.1
+Version: 1.2.0
 Summary: A algorithm crypto trading system.
 Home-page: https://github.com/msaltnet/smtm
 Author: msalt
 Author-email: salt.jeong@gmail.com
 License: MIT
 Project-URL: Documentation, https://smtm.msalt.net/
 Project-URL: Source Code, https://github.com/msaltnet/smtm
@@ -14,15 +14,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # smtm
-[![Travis](https://travis-ci.com/msaltnet/smtm.svg?branch=master&style=flat-square&colorB=green)](https://app.travis-ci.com/github/msaltnet/smtm)
+[![build status](https://github.com/msaltnet/smtm/actions/workflows/python-test.yml/badge.svg)](https://github.com/msaltnet/smtm/actions/workflows/python-test.yml)
 [![license](https://img.shields.io/github/license/msaltnet/smtm.svg?style=flat-square)](https://github.com/msaltnet/smtm/blob/master/LICENSE)
 ![language](https://img.shields.io/github/languages/top/msaltnet/smtm.svg?style=flat-square&colorB=green)
 [![codecov](https://codecov.io/gh/msaltnet/smtm/branch/master/graph/badge.svg?token=USXTX7MG70)](https://codecov.io/gh/msaltnet/smtm)
 
 > It's a game to get money. 
 
 An algorithm-based cryptocurrency automatic trading system made in Python. https://smtm.msalt.net
```

### Comparing `smtm-1.1.1/README-en_us.md` & `smtm-1.2.0/README-en_us.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # smtm
-[![Travis](https://travis-ci.com/msaltnet/smtm.svg?branch=master&style=flat-square&colorB=green)](https://app.travis-ci.com/github/msaltnet/smtm)
+[![build status](https://github.com/msaltnet/smtm/actions/workflows/python-test.yml/badge.svg)](https://github.com/msaltnet/smtm/actions/workflows/python-test.yml)
 [![license](https://img.shields.io/github/license/msaltnet/smtm.svg?style=flat-square)](https://github.com/msaltnet/smtm/blob/master/LICENSE)
 ![language](https://img.shields.io/github/languages/top/msaltnet/smtm.svg?style=flat-square&colorB=green)
 [![codecov](https://codecov.io/gh/msaltnet/smtm/branch/master/graph/badge.svg?token=USXTX7MG70)](https://codecov.io/gh/msaltnet/smtm)
 
 > It's a game to get money. 
 
 An algorithm-based cryptocurrency automatic trading system made in Python. https://smtm.msalt.net
```

### Comparing `smtm-1.1.1/README.md` & `smtm-1.2.0/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # smtm
-[![Travis](https://travis-ci.com/msaltnet/smtm.svg?branch=master&style=flat-square&colorB=green)](https://app.travis-ci.com/github/msaltnet/smtm)
+[![build status](https://github.com/msaltnet/smtm/actions/workflows/python-test.yml/badge.svg)](https://github.com/msaltnet/smtm/actions/workflows/python-test.yml)
 [![license](https://img.shields.io/github/license/msaltnet/smtm.svg?style=flat-square)](https://github.com/msaltnet/smtm/blob/master/LICENSE)
 ![language](https://img.shields.io/github/languages/top/msaltnet/smtm.svg?style=flat-square&colorB=green)
 [![codecov](https://codecov.io/gh/msaltnet/smtm/branch/master/graph/badge.svg?token=USXTX7MG70)](https://codecov.io/gh/msaltnet/smtm)
 
 > It's a game to get money. 
 
 파이썬 알고리즘기반 암호화폐 자동매매 프로그램. https://smtm.msalt.net
```

### Comparing `smtm-1.1.1/setup.cfg` & `smtm-1.2.0/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -47,11 +47,12 @@
 000002e0: 7265 7175 6972 6573 203d 200d 0a09 7265  requires = ...re
 000002f0: 7175 6573 7473 0d0a 0970 616e 6461 730d  quests...pandas.
 00000300: 0a09 6e75 6d70 790d 0a09 6d70 6c66 696e  ..numpy...mplfin
 00000310: 616e 6365 0d0a 096d 6174 706c 6f74 6c69  ance...matplotli
 00000320: 620d 0a09 7079 6a77 740d 0a09 7079 7468  b...pyjwt...pyth
 00000330: 6f6e 2d64 6f74 656e 760d 0a09 6a75 7079  on-dotenv...jupy
 00000340: 7465 720d 0a09 7073 7574 696c 0d0a 0963  ter...psutil...c
-00000350: 6f76 6572 6167 650d 0a0d 0a5b 6567 675f  overage....[egg_
-00000360: 696e 666f 5d0d 0a74 6167 5f62 7569 6c64  info]..tag_build
-00000370: 203d 200d 0a74 6167 5f64 6174 6520 3d20   = ..tag_date = 
-00000380: 300d 0a0d 0a                             0....
+00000350: 6f76 6572 6167 650d 0a09 7363 696b 6974  overage...scikit
+00000360: 2d6c 6561 726e 0d0a 0d0a 5b65 6767 5f69  -learn....[egg_i
+00000370: 6e66 6f5d 0d0a 7461 675f 6275 696c 6420  nfo]..tag_build 
+00000380: 3d20 0d0a 7461 675f 6461 7465 203d 2030  = ..tag_date = 0
+00000390: 0d0a 0d0a                                ....
```

### Comparing `smtm-1.1.1/setup.py` & `smtm-1.2.0/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 import io
 import unittest
-from setuptools import find_packages, setup
+from setuptools import setup
 
 # Package meta-data.
 NAME = "smtm"
 DESCRIPTION = "A algorithm crypto trading system."
 URL = "https://github.com/msaltnet/smtm"
 EMAIL = "salt.jeong@gmail.com"
 AUTHOR = "msalt"
-VERSION = "1.1.1"
+VERSION = "1.2.0"
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     "requests",
     "pandas",
     "numpy",
     "matplotlib",
     "mplfinance",
     "pyjwt",
     "python-dotenv",
     "jupyter",
     "psutil",
+    "scikit-learn",
 ]
 
 
 def long_description():
     with io.open("README-en_us.md", "r", encoding="utf-8") as f:
         readme = f.read()
     return readme
```

### Comparing `smtm-1.1.1/smtm/analyzer.py` & `smtm-1.2.0/smtm/analyzer.py`

 * *Files identical despite different names*

### Comparing `smtm-1.1.1/smtm/bithumb_data_provider.py` & `smtm-1.2.0/smtm/bithumb_data_provider.py`

 * *Files identical despite different names*

### Comparing `smtm-1.1.1/smtm/bithumb_trader.py` & `smtm-1.2.0/smtm/bithumb_trader.py`

 * *Files identical despite different names*

### Comparing `smtm-1.1.1/smtm/controller.py` & `smtm-1.2.0/smtm/controller.py`

 * *Files identical despite different names*

### Comparing `smtm-1.1.1/smtm/database.py` & `smtm-1.2.0/smtm/database.py`

 * *Files identical despite different names*

### Comparing `smtm-1.1.1/smtm/data_provider.py` & `smtm-1.2.0/smtm/data_provider.py`

 * *Files identical despite different names*

### Comparing `smtm-1.1.1/smtm/data_repository.py` & `smtm-1.2.0/smtm/data_repository.py`

 * *Files identical despite different names*

### Comparing `smtm-1.1.1/smtm/date_converter.py` & `smtm-1.2.0/smtm/date_converter.py`

 * *Files identical despite different names*

### Comparing `smtm-1.1.1/smtm/demo_trader.py` & `smtm-1.2.0/smtm/demo_trader.py`

 * *Files identical despite different names*

### Comparing `smtm-1.1.1/smtm/jpt_controller.py` & `smtm-1.2.0/smtm/jpt_controller.py`

 * *Files identical despite different names*

### Comparing `smtm-1.1.1/smtm/log_manager.py` & `smtm-1.2.0/smtm/log_manager.py`

 * *Files identical despite different names*

### Comparing `smtm-1.1.1/smtm/mass_simulator.py` & `smtm-1.2.0/smtm/mass_simulator.py`

 * *Files 1% similar despite different names*

```diff
@@ -202,16 +202,18 @@
                         is_running = False
                     except TimeoutError:
                         self.print_state()
 
                 for result in result_list:
                     self._update_result(result)
             except KeyboardInterrupt:
-                print("Terminating......")
-                sys.exit(0)
+                print("Terminating...")
+
+        if is_running is True:
+            sys.exit(0)
 
     def _update_result(self, partial_result):
         for result in partial_result:
             idx = result["idx"]
             self.result[idx] = result["result"]
 
     @staticmethod
@@ -219,31 +221,32 @@
         LogManager.set_stream_level(30)
         LogManager.change_log_file(f"mass-simulation-{config['partial_idx']}.log")
         period_list = config["partial_period_list"]
         result_list = []
         MassSimulator.memory_usage()
         print(f"partial simulation start @{current_process().name}")
         for period in period_list:
-            tag = f"MASS-{config['title']}-{period['idx']}"
-            operator = MassSimulator.get_initialized_operator(
-                config["budget"],
-                config["strategy"],
-                config["interval"],
-                config["currency"],
-                period["period"]["start"],
-                period["period"]["end"],
-                tag,
-            )
             try:
+                tag = f"MASS-{config['title']}-{period['idx']}"
+                operator = MassSimulator.get_initialized_operator(
+                    config["budget"],
+                    config["strategy"],
+                    config["interval"],
+                    config["currency"],
+                    period["period"]["start"],
+                    period["period"]["end"],
+                    tag,
+                )
                 report = MassSimulator.run_single(operator)
                 result_list.append({"idx": period["idx"], "result": report})
                 print(f"     #{period['idx']} return: {report[2]}")
             except KeyboardInterrupt:
-                print(f"Terminating......@{current_process().name}")
-                operator.stop()
+                print(f"Terminating...@{current_process().name}")
+                if operator is not None:
+                    operator.stop()
 
         return result_list
 
     @staticmethod
     def _round(num):
         return round(num, 3)
```

### Comparing `smtm-1.1.1/smtm/operator.py` & `smtm-1.2.0/smtm/operator.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
         self.trader = trader
         self.analyzer = analyzer
         self.state = "ready"
         self.strategy.initialize(budget, add_spot_callback=add_spot_callback)
         self.analyzer.initialize(trader.get_account_info)
         self.tag = datetime.now().strftime("%Y%m%d-%H%M%S")
         try:
-            self.tag += "-" + self.trader.NAME + "-" + self.strategy.NAME
+            self.tag += "-" + self.trader.NAME + "-" + self.strategy.CODE
         except AttributeError as err:
             self.logger.warning(f"can't get additional info form strategy and trader: {err}")
 
     def set_interval(self, interval):
         """자동 거래 시간 간격을 설정한다.
 
         interval : 거래 프로세스가 수행되는 간격
@@ -105,14 +105,20 @@
         if self.is_timer_running or self.state != "running":
             return
 
         def on_timer_expired():
             self.timer_expired_time = datetime.now()
             self.worker.post_task({"runnable": self._execute_trading})
 
+        if self.interval < 1:
+            # call the handler directly to enhance performance. Timer create new thread always.
+            self.is_timer_running = True
+            on_timer_expired()
+            return
+
         adjusted_interval = self.interval
         if self.interval > 1 and self.timer_expired_time is not None:
             time_delta = datetime.now() - self.timer_expired_time
             adjusted_interval = self.interval - round(time_delta.total_seconds(), 1)
 
         self.timer = threading.Timer(adjusted_interval, on_timer_expired)
         self.timer.start()
@@ -162,19 +168,17 @@
     def stop(self):
         """거래를 중단한다
         analyzer.create_report을 실행하고 반환값을 반환한다.
         """
         if self.state != "running":
             return None
 
-        try:
-            self.logger.info("cancel timer first")
+        self.logger.info("cancel timer first")
+        if self.timer is not None:
             self.timer.cancel()
-        except AttributeError:
-            self.logger.error("stop operation fail")
         self.is_timer_running = False
 
         self.trader.cancel_all_requests()
         trading_info = self.data_provider.get_info()
         self.analyzer.put_trading_info(trading_info)
         self.last_report = self.analyzer.create_report(tag=self.tag)
         self.logger.info("===== Stop operating =====")
```

### Comparing `smtm-1.1.1/smtm/simulation_data_provider.py` & `smtm-1.2.0/smtm/simulation_data_provider.py`

 * *Files identical despite different names*

### Comparing `smtm-1.1.1/smtm/simulation_operator.py` & `smtm-1.2.0/smtm/simulation_operator.py`

 * *Files identical despite different names*

### Comparing `smtm-1.1.1/smtm/simulation_trader.py` & `smtm-1.2.0/smtm/simulation_trader.py`

 * *Files identical despite different names*

### Comparing `smtm-1.1.1/smtm/simulator.py` & `smtm-1.2.0/smtm/simulator.py`

 * *Files 1% similar despite different names*

```diff
@@ -163,21 +163,21 @@
         self.operator.initialize(
             data_provider,
             strategy,
             trader,
             analyzer,
             budget=self.budget,
         )
-        self.operator.tag = self._make_tag(self.start_str, self.end_str, strategy.NAME)
+        self.operator.tag = self._make_tag(self.start_str, self.end_str, strategy.CODE)
         self.operator.set_interval(self.interval)
         self.need_init = False
 
     @staticmethod
-    def _make_tag(start_str, end_str, strategy_name):
-        return "SIM-" + strategy_name + "-" + start_str + "-" + end_str
+    def _make_tag(start_str, end_str, strategy_code):
+        return "SIM-" + strategy_code + "-" + start_str + "-" + end_str
 
     def start(self):
         """시뮬레이션 시작, 재시작"""
         if self.operator is None or self.need_init:
             self._print("초기화가 필요합니다")
             return
```

### Comparing `smtm-1.1.1/smtm/strategy.py` & `smtm-1.2.0/smtm/strategy.py`

 * *Files identical despite different names*

### Comparing `smtm-1.1.1/smtm/strategy_bnh.py` & `smtm-1.2.0/smtm/strategy_bnh.py`

 * *Files identical despite different names*

### Comparing `smtm-1.1.1/smtm/strategy_factory.py` & `smtm-1.2.0/smtm/strategy_factory.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Strategy 정보 조회 및 생성을 담당하는 Factory 클래스"""
 
-from . import StrategyBuyAndHold, StrategySma0, StrategyRsi
+from . import StrategyBuyAndHold, StrategySma0, StrategyRsi, StrategySmaMl
 
 
 class StrategyFactory:
     """Strategy 정보 조회 및 생성을 담당하는 Factory 클래스"""
 
-    STRATEGY_LIST = [StrategyBuyAndHold, StrategySma0, StrategyRsi]
+    STRATEGY_LIST = [StrategyBuyAndHold, StrategySma0, StrategyRsi, StrategySmaMl]
 
     @staticmethod
     def create(code):
         for strategy in StrategyFactory.STRATEGY_LIST:
             if strategy.CODE == code:
                 return strategy()
```

### Comparing `smtm-1.1.1/smtm/strategy_rsi.py` & `smtm-1.2.0/smtm/strategy_rsi.py`

 * *Files identical despite different names*

### Comparing `smtm-1.1.1/smtm/strategy_sma_0.py` & `smtm-1.2.0/smtm/strategy_sma_0.py`

 * *Files identical despite different names*

### Comparing `smtm-1.1.1/smtm/telegram_controller.py` & `smtm-1.2.0/smtm/telegram_controller.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,17 +71,17 @@
     def _update_strategy(self):
         self.STRATEGY = []
         for idx, strategy in enumerate(StrategyFactory.get_all_strategy_info()):
             self.STRATEGY.append(
                 {
                     "name": f"{idx}. {strategy['name']}",
                     "selector": [
-                        f"{idx}. {strategy['name']}",
+                        f"{idx}. {strategy['name']}".upper(),
                         f"{idx}",
-                        f"{strategy['name']}",
+                        f"{strategy['name']}".upper(),
                         f"{strategy['code']}",
                     ],
                     "builder": strategy["class"],
                 }
             )
 
     def _create_command(self):
```

### Comparing `smtm-1.1.1/smtm/trader.py` & `smtm-1.2.0/smtm/trader.py`

 * *Files identical despite different names*

### Comparing `smtm-1.1.1/smtm/upbit_data_provider.py` & `smtm-1.2.0/smtm/upbit_data_provider.py`

 * *Files identical despite different names*

### Comparing `smtm-1.1.1/smtm/upbit_trader.py` & `smtm-1.2.0/smtm/upbit_trader.py`

 * *Files identical despite different names*

### Comparing `smtm-1.1.1/smtm/virtual_market.py` & `smtm-1.2.0/smtm/virtual_market.py`

 * *Files identical despite different names*

### Comparing `smtm-1.1.1/smtm/worker.py` & `smtm-1.2.0/smtm/worker.py`

 * *Files identical despite different names*

### Comparing `smtm-1.1.1/smtm/__init__.py` & `smtm-1.2.0/smtm/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from .log_manager import LogManager
 from .analyzer import Analyzer
 from .simulation_trader import SimulationTrader
 from .simulation_data_provider import SimulationDataProvider
 from .simulation_operator import SimulationOperator
 from .strategy_bnh import StrategyBuyAndHold
 from .strategy_sma_0 import StrategySma0
+from .strategy_sma_ml import StrategySmaMl
 from .strategy_rsi import StrategyRsi
 from .strategy_factory import StrategyFactory
 from .virtual_market import VirtualMarket
 from .worker import Worker
 from .simulator import Simulator
 from .demo_trader import DemoTrader
 from .upbit_trader import UpbitTrader
@@ -33,14 +34,15 @@
     "LogManager",
     "Analyzer",
     "SimulationTrader",
     "SimulationDataProvider",
     "SimulationOperator",
     "StrategyBuyAndHold",
     "StrategySma0",
+    "StrategySmaMl",
     "StrategyRsi",
     "StrategyFactory",
     "VirtualMarket",
     "Worker",
     "Simulator",
     "UpbitTrader",
     "BithumbTrader",
@@ -50,8 +52,8 @@
     "MassSimulator",
     "Controller",
     "JptController",
     "TelegramController",
     "DataRepository",
     "Database",
 ]
-__version__ = "1.1.1"
+__version__ = "1.2.0"
```

### Comparing `smtm-1.1.1/smtm/__main__.py` & `smtm-1.2.0/smtm/__main__.py`

 * *Files identical despite different names*

### Comparing `smtm-1.1.1/smtm.egg-info/PKG-INFO` & `smtm-1.2.0/smtm.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smtm
-Version: 1.1.1
+Version: 1.2.0
 Summary: A algorithm crypto trading system.
 Home-page: https://github.com/msaltnet/smtm
 Author: msalt
 Author-email: salt.jeong@gmail.com
 License: MIT
 Project-URL: Documentation, https://smtm.msalt.net/
 Project-URL: Source Code, https://github.com/msaltnet/smtm
@@ -14,15 +14,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.6
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # smtm
-[![Travis](https://travis-ci.com/msaltnet/smtm.svg?branch=master&style=flat-square&colorB=green)](https://app.travis-ci.com/github/msaltnet/smtm)
+[![build status](https://github.com/msaltnet/smtm/actions/workflows/python-test.yml/badge.svg)](https://github.com/msaltnet/smtm/actions/workflows/python-test.yml)
 [![license](https://img.shields.io/github/license/msaltnet/smtm.svg?style=flat-square)](https://github.com/msaltnet/smtm/blob/master/LICENSE)
 ![language](https://img.shields.io/github/languages/top/msaltnet/smtm.svg?style=flat-square&colorB=green)
 [![codecov](https://codecov.io/gh/msaltnet/smtm/branch/master/graph/badge.svg?token=USXTX7MG70)](https://codecov.io/gh/msaltnet/smtm)
 
 > It's a game to get money. 
 
 An algorithm-based cryptocurrency automatic trading system made in Python. https://smtm.msalt.net
```

### Comparing `smtm-1.1.1/smtm.egg-info/SOURCES.txt` & `smtm-1.2.0/smtm.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -68,14 +68,15 @@
 smtm/simulation_trader.py
 smtm/simulator.py
 smtm/strategy.py
 smtm/strategy_bnh.py
 smtm/strategy_factory.py
 smtm/strategy_rsi.py
 smtm/strategy_sma_0.py
+smtm/strategy_sma_ml.py
 smtm/telegram_controller.py
 smtm/trader.py
 smtm/upbit_data_provider.py
 smtm/upbit_trader.py
 smtm/virtual_market.py
 smtm/worker.py
 smtm.egg-info/PKG-INFO
@@ -100,12 +101,13 @@
 tests/simulation_operator_test.py
 tests/simulation_trader_test.py
 tests/simulator_test.py
 tests/strategy_bnh_test.py
 tests/strategy_factory_test.py
 tests/strategy_rsi_test.py
 tests/strategy_sma_0_test.py
+tests/strategy_sma_ml_test.py
 tests/telegram_controller_test.py
 tests/upbit_data_provider_test.py
 tests/upbit_trader_test.py
 tests/virtual_market_test.py
 tests/worker_test.py
```

### Comparing `smtm-1.1.1/tests/analyzer_test.py` & `smtm-1.2.0/tests/analyzer_test.py`

 * *Files identical despite different names*

### Comparing `smtm-1.1.1/tests/bithumb_data_provider_test.py` & `smtm-1.2.0/tests/bithumb_data_provider_test.py`

 * *Files identical despite different names*

### Comparing `smtm-1.1.1/tests/bithumb_trader_test.py` & `smtm-1.2.0/tests/bithumb_trader_test.py`

 * *Files identical despite different names*

### Comparing `smtm-1.1.1/tests/controller_test.py` & `smtm-1.2.0/tests/controller_test.py`

 * *Files identical despite different names*

### Comparing `smtm-1.1.1/tests/database_test.py` & `smtm-1.2.0/tests/database_test.py`

 * *Files identical despite different names*

### Comparing `smtm-1.1.1/tests/data_repository_test.py` & `smtm-1.2.0/tests/data_repository_test.py`

 * *Files identical despite different names*

### Comparing `smtm-1.1.1/tests/date_converter_test.py` & `smtm-1.2.0/tests/date_converter_test.py`

 * *Files identical despite different names*

### Comparing `smtm-1.1.1/tests/demo_trader_test.py` & `smtm-1.2.0/tests/demo_trader_test.py`

 * *Files identical despite different names*

### Comparing `smtm-1.1.1/tests/jpt_controller_test.py` & `smtm-1.2.0/tests/jpt_controller_test.py`

 * *Files identical despite different names*

### Comparing `smtm-1.1.1/tests/log_manager_test.py` & `smtm-1.2.0/tests/log_manager_test.py`

 * *Files identical despite different names*

### Comparing `smtm-1.1.1/tests/mass_simulator_test.py` & `smtm-1.2.0/tests/mass_simulator_test.py`

 * *Files identical despite different names*

### Comparing `smtm-1.1.1/tests/operator_test.py` & `smtm-1.2.0/tests/operator_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,16 +47,16 @@
         self.assertEqual(self.operator.data_provider, None)
         self.assertEqual(self.operator.strategy, None)
         self.assertEqual(self.operator.trader, None)
         self.assertEqual(self.operator.analyzer, None)
 
     def test_initialize_should_update_tag_correctly(self):
         self.trader_mock.NAME = "mango_tr"
-        self.strategy_mock.NAME = "super_st"
-        expected_tag = "-mango_tr-super_st"
+        self.strategy_mock.CODE = "SPR"
+        expected_tag = "-mango_tr-SPR"
         self.operator.initialize(
             "mango", self.strategy_mock, self.trader_mock, self.analyzer_mock, "banana"
         )
 
         self.assertEqual(self.operator.tag[-len(expected_tag) :], expected_tag)
 
     def test_setup_set_interval_correctly(self):
```

### Comparing `smtm-1.1.1/tests/simulation_data_provider_test.py` & `smtm-1.2.0/tests/simulation_data_provider_test.py`

 * *Files identical despite different names*

### Comparing `smtm-1.1.1/tests/simulation_operator_test.py` & `smtm-1.2.0/tests/simulation_operator_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         analyzer_mock.put_trading_info = MagicMock()
         dp_mock = Mock()
         dp_mock.initialize = MagicMock(return_value="")
         dp_mock.get_info = MagicMock(return_value="mango")
 
         dummy_request = {"id": "mango", "type": "orange", "price": 500, "amount": 10}
         strategy_mock = Mock()
-        strategy_mock.NAME = "mango_st"
+        strategy_mock.CODE = "MAG"
         strategy_mock.update_trading_info = MagicMock(return_value="orange")
         strategy_mock.get_request = MagicMock(return_value=dummy_request)
         trader_mock = Mock()
         trader_mock.NAME = "orange_tr"
         trader_mock.send_request = MagicMock()
         operator.initialize(dp_mock, strategy_mock, trader_mock, analyzer_mock)
         operator.set_interval(27)
@@ -45,15 +45,15 @@
         analyzer_mock.put_result = MagicMock()
         dp_mock = Mock()
         dp_mock.initialize = MagicMock(return_value="")
         dp_mock.get_info = MagicMock(return_value="mango")
 
         dummy_request = {"id": "mango", "type": "orange", "price": 500, "amount": 10}
         strategy_mock = Mock()
-        strategy_mock.NAME = "mango_st"
+        strategy_mock.CODE = "MAG"
         strategy_mock.update_trading_info = MagicMock(return_value="orange")
         strategy_mock.update_result = MagicMock()
         strategy_mock.get_request = MagicMock(return_value=dummy_request)
         trader_mock = Mock()
         trader_mock.NAME = "orange_tr"
         trader_mock.send_request = MagicMock()
         operator.initialize(dp_mock, strategy_mock, trader_mock, analyzer_mock)
@@ -76,15 +76,15 @@
         analyzer_mock.create_report = MagicMock()
         dp_mock = Mock()
         dp_mock.initialize = MagicMock(return_value="")
         dp_mock.get_info = MagicMock(return_value="mango")
 
         dummy_request = {"id": "mango", "type": "orange", "price": 500, "amount": 10}
         strategy_mock = Mock()
-        strategy_mock.NAME = "mango_st"
+        strategy_mock.CODE = "MAG"
         strategy_mock.update_trading_info = MagicMock(return_value="orange")
         strategy_mock.update_result = MagicMock()
         strategy_mock.get_request = MagicMock(return_value=dummy_request)
         trader_mock = Mock()
         trader_mock.NAME = "orange_tr"
         trader_mock.send_request = MagicMock()
         operator.initialize(dp_mock, strategy_mock, trader_mock, analyzer_mock)
@@ -104,15 +104,15 @@
     def test_execute_trading_should_NOT_call_trader_send_request_when_request_is_None(self):
         operator = SimulationOperator()
         analyzer_mock = Mock()
         dp_mock = Mock()
         dp_mock.initialize = MagicMock(return_value="")
         dp_mock.get_info = MagicMock(return_value="mango")
         strategy_mock = Mock()
-        strategy_mock.NAME = "mango_st"
+        strategy_mock.CODE = "MAG"
         strategy_mock.update_trading_info = MagicMock(return_value="orange")
         strategy_mock.get_request = MagicMock(return_value=None)
         trader_mock = Mock()
         trader_mock.NAME = "orange_tr"
         trader_mock.send_request = MagicMock()
         operator.initialize(dp_mock, strategy_mock, trader_mock, analyzer_mock)
         operator.set_interval(27)
```

### Comparing `smtm-1.1.1/tests/simulation_trader_test.py` & `smtm-1.2.0/tests/simulation_trader_test.py`

 * *Files identical despite different names*

### Comparing `smtm-1.1.1/tests/simulator_test.py` & `smtm-1.2.0/tests/simulator_test.py`

 * *Files identical despite different names*

### Comparing `smtm-1.1.1/tests/strategy_bnh_test.py` & `smtm-1.2.0/tests/strategy_bnh_test.py`

 * *Files identical despite different names*

### Comparing `smtm-1.1.1/tests/strategy_factory_test.py` & `smtm-1.2.0/tests/strategy_factory_test.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import unittest
-from smtm import StrategyFactory, StrategyBuyAndHold, StrategySma0, StrategyRsi
+from smtm import StrategyFactory, StrategyBuyAndHold, StrategySma0, StrategyRsi, StrategySmaMl
 from unittest.mock import *
 
 
 class StrategyFactoryTests(unittest.TestCase):
     def setUp(self):
         pass
 
@@ -14,28 +14,33 @@
         strategy = StrategyFactory.create("")
         self.assertEqual(strategy, None)
 
     def test_create_return_correct_strategy(self):
         self.assertTrue(isinstance(StrategyFactory.create("BNH"), StrategyBuyAndHold))
         self.assertTrue(isinstance(StrategyFactory.create("SMA"), StrategySma0))
         self.assertTrue(isinstance(StrategyFactory.create("RSI"), StrategyRsi))
+        self.assertTrue(isinstance(StrategyFactory.create("SML"), StrategySmaMl))
 
     def test_get_name_return_None_when_called_with_invalid_code(self):
         strategy = StrategyFactory.get_name("")
         self.assertEqual(strategy, None)
 
     def test_get_name_return_correct_strategy(self):
         self.assertTrue(StrategyFactory.get_name("BNH"), StrategyBuyAndHold.NAME)
         self.assertTrue(StrategyFactory.get_name("SMA"), StrategySma0.NAME)
         self.assertTrue(StrategyFactory.get_name("RSI"), StrategyRsi.NAME)
+        self.assertTrue(StrategyFactory.get_name("SML"), StrategySmaMl.NAME)
 
     def test_get_all_strategy_info_return_correct_info(self):
         all = StrategyFactory.get_all_strategy_info()
         self.assertTrue(all[0]["name"], StrategyBuyAndHold.NAME)
         self.assertTrue(all[0]["code"], StrategyBuyAndHold.CODE)
         self.assertTrue(all[0]["class"], StrategyBuyAndHold)
         self.assertTrue(all[1]["name"], StrategySma0.NAME)
         self.assertTrue(all[1]["code"], StrategySma0.CODE)
         self.assertTrue(all[1]["class"], StrategySma0)
         self.assertTrue(all[2]["name"], StrategyRsi.NAME)
         self.assertTrue(all[2]["code"], StrategyRsi.CODE)
         self.assertTrue(all[2]["class"], StrategyRsi)
+        self.assertTrue(all[3]["name"], StrategySmaMl.NAME)
+        self.assertTrue(all[3]["code"], StrategySmaMl.CODE)
+        self.assertTrue(all[3]["class"], StrategySmaMl)
```

### Comparing `smtm-1.1.1/tests/strategy_rsi_test.py` & `smtm-1.2.0/tests/strategy_rsi_test.py`

 * *Files identical despite different names*

### Comparing `smtm-1.1.1/tests/strategy_sma_0_test.py` & `smtm-1.2.0/tests/strategy_sma_0_test.py`

 * *Files identical despite different names*

### Comparing `smtm-1.1.1/tests/telegram_controller_test.py` & `smtm-1.2.0/tests/telegram_controller_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,36 +165,36 @@
 
     def test__send_text_message_shoul_call_sendMessage_api_correctly(self):
         tcb = TelegramController()
         tcb.post_worker = MagicMock()
         tcb.TOKEN = "banana"
         tcb.CHAT_ID = "to_banana"
         tcb._send_http = MagicMock()
-        tcb._send_text_message("hello~ banana")
+        tcb._send_text_message("hello banana")
         tcb.post_worker.post_task.assert_called_once_with(ANY)
         task = tcb.post_worker.post_task.call_args[0][0]
         tcb.post_worker.post_task.call_args[0][0]["runnable"](task)
 
         tcb._send_http.assert_called_once_with(
-            "https://api.telegram.org/banana/sendMessage?chat_id=to_banana&text=hello%7E%20banana"
+            "https://api.telegram.org/banana/sendMessage?chat_id=to_banana&text=hello%20banana"
         )
 
     def test__send_text_message_shoul_call_sendMessage_api_correctly_with_keyboard(self):
         tcb = TelegramController()
         tcb.post_worker = MagicMock()
         tcb.TOKEN = "banana"
         tcb.CHAT_ID = "to_banana"
         tcb._send_http = MagicMock()
-        tcb._send_text_message("hello~ banana", "banana_keyboard_markup")
+        tcb._send_text_message("hello banana", "banana_keyboard_markup")
         tcb.post_worker.post_task.assert_called_once_with(ANY)
         task = tcb.post_worker.post_task.call_args[0][0]
         tcb.post_worker.post_task.call_args[0][0]["runnable"](task)
 
         tcb._send_http.assert_called_once_with(
-            "https://api.telegram.org/banana/sendMessage?chat_id=to_banana&text=hello%7E%20banana&reply_markup=banana_keyboard_markup"
+            "https://api.telegram.org/banana/sendMessage?chat_id=to_banana&text=hello%20banana&reply_markup=banana_keyboard_markup"
         )
 
     def test__get_updates_call_getUpdates_api_correctly(self):
         tcb = TelegramController()
         tcb.TOKEN = "banana"
         expected_response = "banana_result"
         tcb._send_http = MagicMock(return_value=expected_response)
```

### Comparing `smtm-1.1.1/tests/upbit_data_provider_test.py` & `smtm-1.2.0/tests/upbit_data_provider_test.py`

 * *Files identical despite different names*

### Comparing `smtm-1.1.1/tests/upbit_trader_test.py` & `smtm-1.2.0/tests/upbit_trader_test.py`

 * *Files identical despite different names*

### Comparing `smtm-1.1.1/tests/virtual_market_test.py` & `smtm-1.2.0/tests/virtual_market_test.py`

 * *Files identical despite different names*

### Comparing `smtm-1.1.1/tests/worker_test.py` & `smtm-1.2.0/tests/worker_test.py`

 * *Files identical despite different names*

