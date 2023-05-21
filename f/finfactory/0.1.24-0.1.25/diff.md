# Comparing `tmp/finfactory-0.1.24.tar.gz` & `tmp/finfactory-0.1.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "finfactory-0.1.24.tar", last modified: Sat Feb 25 10:24:31 2023, max compression
+gzip compressed data, was "finfactory-0.1.25.tar", last modified: Sun May 21 02:58:21 2023, max compression
```

## Comparing `finfactory-0.1.24.tar` & `finfactory-0.1.25.tar`

### file list

```diff
@@ -1,101 +1,102 @@
-drwxrwxrwx   0        0        0        0 2023-02-25 10:24:31.882564 finfactory-0.1.24/
--rw-rw-rw-   0        0        0      975 2023-02-25 10:24:31.882564 finfactory-0.1.24/PKG-INFO
--rw-rw-rw-   0        0        0      675 2022-06-26 13:47:05.000000 finfactory-0.1.24/README.md
-drwxrwxrwx   0        0        0        0 2023-02-25 10:24:31.649617 finfactory-0.1.24/finfactory/
--rw-rw-rw-   0        0        0      183 2022-12-28 10:37:31.000000 finfactory-0.1.24/finfactory/__init__.py
--rw-rw-rw-   0        0        0      740 2023-02-25 10:24:17.000000 finfactory-0.1.24/finfactory/_pkg_info.py
--rw-rw-rw-   0        0        0     5096 2023-01-08 14:22:27.000000 finfactory-0.1.24/finfactory/config.py
-drwxrwxrwx   0        0        0        0 2023-02-25 10:24:31.667185 finfactory-0.1.24/finfactory/findata/
--rw-rw-rw-   0        0        0       61 2022-09-19 08:32:04.000000 finfactory-0.1.24/finfactory/findata/__init__.py
--rw-rw-rw-   0        0        0     1583 2023-02-25 08:48:40.000000 finfactory-0.1.24/finfactory/findata/api.py
-drwxrwxrwx   0        0        0        0 2023-02-25 10:24:31.678630 finfactory-0.1.24/finfactory/finplot/
--rw-rw-rw-   0        0        0       65 2022-08-24 07:43:17.000000 finfactory-0.1.24/finfactory/finplot/__init__.py
--rw-rw-rw-   0        0        0    28195 2022-01-09 07:11:47.000000 finfactory-0.1.24/finfactory/finplot/_mpfold.py
--rw-rw-rw-   0        0        0     5998 2022-11-03 09:21:01.000000 finfactory-0.1.24/finfactory/finplot/_plot_candle_deprecated.py
--rw-rw-rw-   0        0        0     2760 2022-07-06 06:29:25.000000 finfactory-0.1.24/finfactory/finplot/finplot.py
--rw-rw-rw-   0        0        0    21854 2022-11-22 11:06:58.000000 finfactory-0.1.24/finfactory/finplot/plot_candle.py
-drwxrwxrwx   0        0        0        0 2023-02-25 10:24:31.707158 finfactory-0.1.24/finfactory/fintools/
--rw-rw-rw-   0        0        0     1039 2022-07-15 05:32:54.000000 finfactory-0.1.24/finfactory/fintools/__init__.py
--rw-rw-rw-   0        0        0      321 2023-02-16 08:50:17.000000 finfactory-0.1.24/finfactory/fintools/backtest_timselection.py
--rw-rw-rw-   0        0        0    83122 2022-11-26 11:28:33.000000 finfactory-0.1.24/finfactory/fintools/cal_sig_gains.py
--rw-rw-rw-   0        0        0    76415 2022-10-03 08:59:44.000000 finfactory-0.1.24/finfactory/fintools/cal_sig_gains_bk.py
--rw-rw-rw-   0        0        0    17120 2022-10-03 02:12:54.000000 finfactory-0.1.24/finfactory/fintools/copy_line.py
--rw-rw-rw-   0        0        0    42382 2022-09-02 09:58:31.000000 finfactory-0.1.24/finfactory/fintools/fintools.py
--rw-rw-rw-   0        0        0     9258 2022-10-11 01:33:43.000000 finfactory-0.1.24/finfactory/fintools/fundnet.py
--rw-rw-rw-   0        0        0    27973 2022-05-08 13:44:56.000000 finfactory-0.1.24/finfactory/fintools/options.py
--rw-rw-rw-   0        0        0    27650 2023-02-08 07:44:41.000000 finfactory-0.1.24/finfactory/fintools/utils_chn.py
--rw-rw-rw-   0        0        0   155757 2022-11-30 13:13:24.000000 finfactory-0.1.24/finfactory/fintools/utils_gains.py
--rw-rw-rw-   0        0        0     7633 2022-07-06 06:35:50.000000 finfactory-0.1.24/finfactory/fintools/zigzag.py
-drwxrwxrwx   0        0        0        0 2023-02-25 10:24:31.876915 finfactory-0.1.24/finfactory/get_data/
--rw-rw-rw-   0        0        0       25 2023-01-01 05:35:26.000000 finfactory-0.1.24/finfactory/get_data/__init__.py
--rw-rw-rw-   0        0        0     1168 2023-01-01 05:35:26.000000 finfactory-0.1.24/finfactory/get_data/_ccxt.py
--rw-rw-rw-   0        0        0     3518 2023-02-08 04:13:20.000000 finfactory-0.1.24/finfactory/get_data/_get_data.py
--rw-rw-rw-   0        0        0     2694 2023-01-01 05:35:26.000000 finfactory-0.1.24/finfactory/get_data/_jq_opts_minute_check.py
--rw-rw-rw-   0        0        0     3067 2023-01-08 03:26:29.000000 finfactory-0.1.24/finfactory/get_data/_split_data.py
--rw-rw-rw-   0        0        0     1381 2023-01-01 05:35:27.000000 finfactory-0.1.24/finfactory/get_data/_stocks_cut.py
--rw-rw-rw-   0        0        0     2946 2023-01-08 03:39:54.000000 finfactory-0.1.24/finfactory/get_data/_stocks_merge.py
--rw-rw-rw-   0        0        0     6075 2023-01-01 05:35:27.000000 finfactory-0.1.24/finfactory/get_data/ccxt_1d.py
--rw-rw-rw-   0        0        0     8731 2023-02-20 01:43:45.000000 finfactory-0.1.24/finfactory/get_data/ccxt_minute.py
--rw-rw-rw-   0        0        0     7507 2023-01-01 05:35:27.000000 finfactory-0.1.24/finfactory/get_data/cffex_futures_lhb.py
--rw-rw-rw-   0        0        0     9976 2023-01-01 05:35:27.000000 finfactory-0.1.24/finfactory/get_data/chn_local_bond_rates.py
--rw-rw-rw-   0        0        0     9903 2023-01-01 05:35:27.000000 finfactory-0.1.24/finfactory/get_data/chn_national_bond_rates.py
--rw-rw-rw-   0        0        0     2138 2023-01-01 05:35:28.000000 finfactory-0.1.24/finfactory/get_data/eastmoney.py
--rw-rw-rw-   0        0        0     5458 2023-01-01 05:35:28.000000 finfactory-0.1.24/finfactory/get_data/eastmoney_tonorth_netbuy_daily.py
--rw-rw-rw-   0        0        0     5466 2023-01-01 05:35:28.000000 finfactory-0.1.24/finfactory/get_data/eastmoney_tonorth_netin_daily.py
--rw-rw-rw-   0        0        0     5491 2023-01-01 05:35:28.000000 finfactory-0.1.24/finfactory/get_data/eastmoney_tosouth_netbuy_daily.py
--rw-rw-rw-   0        0        0     5490 2023-01-01 05:35:28.000000 finfactory-0.1.24/finfactory/get_data/eastmoney_tosouth_netin_daily.py
--rw-rw-rw-   0        0        0     1501 2023-01-01 05:35:28.000000 finfactory-0.1.24/finfactory/get_data/ef.py
--rw-rw-rw-   0        0        0     5251 2023-02-09 14:35:32.000000 finfactory-0.1.24/finfactory/get_data/eniu_index_pe.py
--rw-rw-rw-   0        0        0     7445 2023-01-01 05:35:28.000000 finfactory-0.1.24/finfactory/get_data/fundex_index_dpe.py
--rw-rw-rw-   0        0        0     6141 2023-01-01 05:35:28.000000 finfactory-0.1.24/finfactory/get_data/hexun_gold_daily.py
--rw-rw-rw-   0        0        0     6181 2023-01-01 05:35:28.000000 finfactory-0.1.24/finfactory/get_data/hexun_silver_daily.py
--rw-rw-rw-   0        0        0    12793 2023-02-07 05:40:03.000000 finfactory-0.1.24/finfactory/get_data/sw_daily_info.py
--rw-rw-rw-   0        0        0    11647 2023-01-01 05:35:29.000000 finfactory-0.1.24/finfactory/get_data/sw_daily_info_old.py
--rw-rw-rw-   0        0        0     4770 2023-01-01 05:35:29.000000 finfactory-0.1.24/finfactory/get_data/tushare_astocks_list.py
--rw-rw-rw-   0        0        0     8319 2023-01-01 05:35:29.000000 finfactory-0.1.24/finfactory/get_data/tushare_block_trades.py
--rw-rw-rw-   0        0        0     5737 2023-01-01 05:35:29.000000 finfactory-0.1.24/finfactory/get_data/tushare_cctv_news.py
--rw-rw-rw-   0        0        0     6136 2023-01-01 05:35:29.000000 finfactory-0.1.24/finfactory/get_data/tushare_chn_cpi.py
--rw-rw-rw-   0        0        0     5995 2023-01-01 05:35:29.000000 finfactory-0.1.24/finfactory/get_data/tushare_chn_gdp.py
--rw-rw-rw-   0        0        0     5917 2023-01-01 05:35:29.000000 finfactory-0.1.24/finfactory/get_data/tushare_chn_money.py
--rw-rw-rw-   0        0        0     6674 2023-01-01 05:35:29.000000 finfactory-0.1.24/finfactory/get_data/tushare_chn_ppi.py
--rw-rw-rw-   0        0        0     7341 2023-01-01 05:35:29.000000 finfactory-0.1.24/finfactory/get_data/tushare_fund_adj.py
--rw-rw-rw-   0        0        0     8076 2023-01-01 05:35:29.000000 finfactory-0.1.24/finfactory/get_data/tushare_fund_daily.py
--rw-rw-rw-   0        0        0     2364 2023-01-01 05:35:29.000000 finfactory-0.1.24/finfactory/get_data/tushare_fund_fq.py
--rw-rw-rw-   0        0        0     4706 2023-01-01 05:35:29.000000 finfactory-0.1.24/finfactory/get_data/tushare_fund_list.py
--rw-rw-rw-   0        0        0     8237 2023-01-01 05:35:30.000000 finfactory-0.1.24/finfactory/get_data/tushare_futures_daily.py
--rw-rw-rw-   0        0        0     9814 2023-01-01 05:35:30.000000 finfactory-0.1.24/finfactory/get_data/tushare_futures_daily_ex.py
--rw-rw-rw-   0        0        0     5162 2023-01-01 05:35:30.000000 finfactory-0.1.24/finfactory/get_data/tushare_futures_info.py
--rw-rw-rw-   0        0        0     8290 2023-01-01 05:35:30.000000 finfactory-0.1.24/finfactory/get_data/tushare_futures_mapping.py
--rw-rw-rw-   0        0        0     7949 2023-01-01 05:35:30.000000 finfactory-0.1.24/finfactory/get_data/tushare_index_daily.py
--rw-rw-rw-   0        0        0     8452 2023-01-01 05:35:30.000000 finfactory-0.1.24/finfactory/get_data/tushare_index_daily_basic.py
--rw-rw-rw-   0        0        0     4794 2023-01-01 05:35:30.000000 finfactory-0.1.24/finfactory/get_data/tushare_index_info.py
--rw-rw-rw-   0        0        0     6135 2023-01-01 05:35:30.000000 finfactory-0.1.24/finfactory/get_data/tushare_lpr.py
--rw-rw-rw-   0        0        0     9564 2023-01-01 05:35:30.000000 finfactory-0.1.24/finfactory/get_data/tushare_options_daily.py
--rw-rw-rw-   0        0        0     7238 2023-01-01 05:35:30.000000 finfactory-0.1.24/finfactory/get_data/tushare_options_info.py
--rw-rw-rw-   0        0        0     7846 2023-01-01 05:35:31.000000 finfactory-0.1.24/finfactory/get_data/tushare_rzrq_daily.py
--rw-rw-rw-   0        0        0     6344 2023-01-01 05:35:31.000000 finfactory-0.1.24/finfactory/get_data/tushare_shibor.py
--rw-rw-rw-   0        0        0     9988 2023-01-01 05:35:31.000000 finfactory-0.1.24/finfactory/get_data/tushare_stock_daily.py
--rw-rw-rw-   0        0        0    10237 2023-01-01 05:35:31.000000 finfactory-0.1.24/finfactory/get_data/tushare_stock_daily_basic.py
--rw-rw-rw-   0        0        0    10205 2023-01-01 05:35:31.000000 finfactory-0.1.24/finfactory/get_data/tushare_stock_daily_stk.py
--rw-rw-rw-   0        0        0     9673 2023-01-01 05:35:31.000000 finfactory-0.1.24/finfactory/get_data/tushare_stock_top10holders.py
--rw-rw-rw-   0        0        0    10096 2023-01-01 05:35:31.000000 finfactory-0.1.24/finfactory/get_data/tushare_stock_top10holders_free.py
--rw-rw-rw-   0        0        0     9425 2023-01-01 05:35:31.000000 finfactory-0.1.24/finfactory/get_data/tushare_stock_zjc.py
--rw-rw-rw-   0        0        0    12098 2023-01-01 05:35:31.000000 finfactory-0.1.24/finfactory/get_data/tushare_stocks_daily.py
--rw-rw-rw-   0        0        0    11396 2023-01-01 05:35:31.000000 finfactory-0.1.24/finfactory/get_data/tushare_stocks_daily_basic.py
--rw-rw-rw-   0        0        0    11369 2023-01-01 05:35:31.000000 finfactory-0.1.24/finfactory/get_data/tushare_stocks_daily_stk.py
--rw-rw-rw-   0        0        0     7975 2023-02-08 04:11:06.000000 finfactory-0.1.24/finfactory/get_data/tushare_trade_dates.py
--rw-rw-rw-   0        0        0     6669 2023-01-01 05:35:31.000000 finfactory-0.1.24/finfactory/get_data/tushare_usa_bond_rates.py
--rw-rw-rw-   0        0        0     6609 2023-01-01 05:35:32.000000 finfactory-0.1.24/finfactory/get_data/tushare_usa_bond_rates_act.py
--rw-rw-rw-   0        0        0      952 2022-08-04 06:39:56.000000 finfactory-0.1.24/finfactory/install_check.py
--rw-rw-rw-   0        0        0    27804 2022-11-22 11:14:04.000000 finfactory-0.1.24/finfactory/load_his_data.py
-drwxrwxrwx   0        0        0        0 2023-02-25 10:24:31.880602 finfactory-0.1.24/finfactory/utils/
--rw-rw-rw-   0        0        0       25 2022-06-08 01:24:02.000000 finfactory-0.1.24/finfactory/utils/__init__.py
--rw-rw-rw-   0        0        0    10456 2022-12-11 13:20:01.000000 finfactory-0.1.24/finfactory/utils/utils.py
--rw-rw-rw-   0        0        0     5912 2022-11-23 04:58:52.000000 finfactory-0.1.24/finfactory/utils/utils_crypto.py
-drwxrwxrwx   0        0        0        0 2023-02-25 10:24:31.664709 finfactory-0.1.24/finfactory.egg-info/
--rw-rw-rw-   0        0        0      975 2023-02-25 10:24:30.000000 finfactory-0.1.24/finfactory.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3464 2023-02-25 10:24:31.000000 finfactory-0.1.24/finfactory.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-25 10:24:30.000000 finfactory-0.1.24/finfactory.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-02-25 10:24:30.000000 finfactory-0.1.24/finfactory.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-02-25 10:24:31.882564 finfactory-0.1.24/setup.cfg
--rw-rw-rw-   0        0        0     1234 2022-10-23 14:13:58.000000 finfactory-0.1.24/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-21 02:58:21.300853 finfactory-0.1.25/
+-rw-rw-rw-   0        0        0     1072 2023-02-25 10:44:38.000000 finfactory-0.1.25/LICENSE
+-rw-rw-rw-   0        0        0      994 2023-05-21 02:58:21.299857 finfactory-0.1.25/PKG-INFO
+-rw-rw-rw-   0        0        0      675 2022-06-26 13:47:05.000000 finfactory-0.1.25/README.md
+drwxrwxrwx   0        0        0        0 2023-05-21 02:58:21.230042 finfactory-0.1.25/finfactory/
+-rw-rw-rw-   0        0        0      378 2023-03-28 13:15:39.000000 finfactory-0.1.25/finfactory/__init__.py
+-rw-rw-rw-   0        0        0      740 2023-05-16 02:02:47.000000 finfactory-0.1.25/finfactory/_pkg_info.py
+-rw-rw-rw-   0        0        0     5078 2023-03-23 09:16:05.000000 finfactory-0.1.25/finfactory/config.py
+drwxrwxrwx   0        0        0        0 2023-05-21 02:58:21.235029 finfactory-0.1.25/finfactory/findata/
+-rw-rw-rw-   0        0        0       61 2022-09-19 08:32:04.000000 finfactory-0.1.25/finfactory/findata/__init__.py
+-rw-rw-rw-   0        0        0     1583 2023-02-25 08:48:40.000000 finfactory-0.1.25/finfactory/findata/api.py
+drwxrwxrwx   0        0        0        0 2023-05-21 02:58:21.239018 finfactory-0.1.25/finfactory/finplot/
+-rw-rw-rw-   0        0        0       65 2022-08-24 07:43:17.000000 finfactory-0.1.25/finfactory/finplot/__init__.py
+-rw-rw-rw-   0        0        0    28195 2022-01-09 07:11:47.000000 finfactory-0.1.25/finfactory/finplot/_mpfold.py
+-rw-rw-rw-   0        0        0     5998 2022-11-03 09:21:01.000000 finfactory-0.1.25/finfactory/finplot/_plot_candle_deprecated.py
+-rw-rw-rw-   0        0        0     2760 2022-07-06 06:29:25.000000 finfactory-0.1.25/finfactory/finplot/finplot.py
+-rw-rw-rw-   0        0        0    21794 2023-03-22 08:52:36.000000 finfactory-0.1.25/finfactory/finplot/plot_candle.py
+drwxrwxrwx   0        0        0        0 2023-05-21 02:58:21.248993 finfactory-0.1.25/finfactory/fintools/
+-rw-rw-rw-   0        0        0     1039 2022-07-15 05:32:54.000000 finfactory-0.1.25/finfactory/fintools/__init__.py
+-rw-rw-rw-   0        0        0     1746 2023-03-23 09:16:23.000000 finfactory-0.1.25/finfactory/fintools/backtest_timselection.py
+-rw-rw-rw-   0        0        0    83122 2022-11-26 11:28:33.000000 finfactory-0.1.25/finfactory/fintools/cal_sig_gains.py
+-rw-rw-rw-   0        0        0    76415 2022-10-03 08:59:44.000000 finfactory-0.1.25/finfactory/fintools/cal_sig_gains_bk.py
+-rw-rw-rw-   0        0        0    17120 2022-10-03 02:12:54.000000 finfactory-0.1.25/finfactory/fintools/copy_line.py
+-rw-rw-rw-   0        0        0    42326 2023-03-22 08:46:52.000000 finfactory-0.1.25/finfactory/fintools/fintools.py
+-rw-rw-rw-   0        0        0     9258 2022-10-11 01:33:43.000000 finfactory-0.1.25/finfactory/fintools/fundnet.py
+-rw-rw-rw-   0        0        0    27973 2022-05-08 13:44:56.000000 finfactory-0.1.25/finfactory/fintools/options.py
+-rw-rw-rw-   0        0        0    35115 2023-05-21 02:50:09.000000 finfactory-0.1.25/finfactory/fintools/utils_chn.py
+-rw-rw-rw-   0        0        0   155723 2023-05-12 02:44:37.000000 finfactory-0.1.25/finfactory/fintools/utils_gains.py
+drwxrwxrwx   0        0        0        0 2023-05-21 02:58:21.296865 finfactory-0.1.25/finfactory/get_data/
+-rw-rw-rw-   0        0        0       25 2023-01-01 05:35:26.000000 finfactory-0.1.25/finfactory/get_data/__init__.py
+-rw-rw-rw-   0        0        0     1168 2023-01-01 05:35:26.000000 finfactory-0.1.25/finfactory/get_data/_ccxt.py
+-rw-rw-rw-   0        0        0     3620 2023-04-27 13:34:25.000000 finfactory-0.1.25/finfactory/get_data/_get_data.py
+-rw-rw-rw-   0        0        0     2694 2023-01-01 05:35:26.000000 finfactory-0.1.25/finfactory/get_data/_jq_opts_minute_check.py
+-rw-rw-rw-   0        0        0    20530 2023-05-18 07:48:56.000000 finfactory-0.1.25/finfactory/get_data/_jy_downloader.py
+-rw-rw-rw-   0        0        0     3067 2023-01-08 03:26:29.000000 finfactory-0.1.25/finfactory/get_data/_split_data.py
+-rw-rw-rw-   0        0        0     1368 2023-03-22 08:44:56.000000 finfactory-0.1.25/finfactory/get_data/_stocks_cut.py
+-rw-rw-rw-   0        0        0     2925 2023-03-22 08:45:28.000000 finfactory-0.1.25/finfactory/get_data/_stocks_merge.py
+-rw-rw-rw-   0        0        0     6075 2023-01-01 05:35:27.000000 finfactory-0.1.25/finfactory/get_data/ccxt_1d.py
+-rw-rw-rw-   0        0        0     8731 2023-02-20 01:43:45.000000 finfactory-0.1.25/finfactory/get_data/ccxt_minute.py
+-rw-rw-rw-   0        0        0     7507 2023-01-01 05:35:27.000000 finfactory-0.1.25/finfactory/get_data/cffex_futures_lhb.py
+-rw-rw-rw-   0        0        0     9976 2023-01-01 05:35:27.000000 finfactory-0.1.25/finfactory/get_data/chn_local_bond_rates.py
+-rw-rw-rw-   0        0        0     9903 2023-01-01 05:35:27.000000 finfactory-0.1.25/finfactory/get_data/chn_national_bond_rates.py
+-rw-rw-rw-   0        0        0     2138 2023-01-01 05:35:28.000000 finfactory-0.1.25/finfactory/get_data/eastmoney.py
+-rw-rw-rw-   0        0        0     5458 2023-01-01 05:35:28.000000 finfactory-0.1.25/finfactory/get_data/eastmoney_tonorth_netbuy_daily.py
+-rw-rw-rw-   0        0        0     5466 2023-01-01 05:35:28.000000 finfactory-0.1.25/finfactory/get_data/eastmoney_tonorth_netin_daily.py
+-rw-rw-rw-   0        0        0     5491 2023-01-01 05:35:28.000000 finfactory-0.1.25/finfactory/get_data/eastmoney_tosouth_netbuy_daily.py
+-rw-rw-rw-   0        0        0     5490 2023-01-01 05:35:28.000000 finfactory-0.1.25/finfactory/get_data/eastmoney_tosouth_netin_daily.py
+-rw-rw-rw-   0        0        0     1501 2023-01-01 05:35:28.000000 finfactory-0.1.25/finfactory/get_data/ef.py
+-rw-rw-rw-   0        0        0     5251 2023-02-09 14:35:32.000000 finfactory-0.1.25/finfactory/get_data/eniu_index_pe.py
+-rw-rw-rw-   0        0        0     7445 2023-01-01 05:35:28.000000 finfactory-0.1.25/finfactory/get_data/fundex_index_dpe.py
+-rw-rw-rw-   0        0        0     6141 2023-01-01 05:35:28.000000 finfactory-0.1.25/finfactory/get_data/hexun_gold_daily.py
+-rw-rw-rw-   0        0        0     6181 2023-01-01 05:35:28.000000 finfactory-0.1.25/finfactory/get_data/hexun_silver_daily.py
+-rw-rw-rw-   0        0        0    12793 2023-02-07 05:40:03.000000 finfactory-0.1.25/finfactory/get_data/sw_daily_info.py
+-rw-rw-rw-   0        0        0    11647 2023-01-01 05:35:29.000000 finfactory-0.1.25/finfactory/get_data/sw_daily_info_old.py
+-rw-rw-rw-   0        0        0     4770 2023-01-01 05:35:29.000000 finfactory-0.1.25/finfactory/get_data/tushare_astocks_list.py
+-rw-rw-rw-   0        0        0     8319 2023-01-01 05:35:29.000000 finfactory-0.1.25/finfactory/get_data/tushare_block_trades.py
+-rw-rw-rw-   0        0        0     5737 2023-01-01 05:35:29.000000 finfactory-0.1.25/finfactory/get_data/tushare_cctv_news.py
+-rw-rw-rw-   0        0        0     6136 2023-01-01 05:35:29.000000 finfactory-0.1.25/finfactory/get_data/tushare_chn_cpi.py
+-rw-rw-rw-   0        0        0     5995 2023-01-01 05:35:29.000000 finfactory-0.1.25/finfactory/get_data/tushare_chn_gdp.py
+-rw-rw-rw-   0        0        0     5917 2023-01-01 05:35:29.000000 finfactory-0.1.25/finfactory/get_data/tushare_chn_money.py
+-rw-rw-rw-   0        0        0     6674 2023-01-01 05:35:29.000000 finfactory-0.1.25/finfactory/get_data/tushare_chn_ppi.py
+-rw-rw-rw-   0        0        0     7341 2023-01-01 05:35:29.000000 finfactory-0.1.25/finfactory/get_data/tushare_fund_adj.py
+-rw-rw-rw-   0        0        0     8076 2023-01-01 05:35:29.000000 finfactory-0.1.25/finfactory/get_data/tushare_fund_daily.py
+-rw-rw-rw-   0        0        0     2364 2023-01-01 05:35:29.000000 finfactory-0.1.25/finfactory/get_data/tushare_fund_fq.py
+-rw-rw-rw-   0        0        0     4706 2023-01-01 05:35:29.000000 finfactory-0.1.25/finfactory/get_data/tushare_fund_list.py
+-rw-rw-rw-   0        0        0     8237 2023-01-01 05:35:30.000000 finfactory-0.1.25/finfactory/get_data/tushare_futures_daily.py
+-rw-rw-rw-   0        0        0     9814 2023-01-01 05:35:30.000000 finfactory-0.1.25/finfactory/get_data/tushare_futures_daily_ex.py
+-rw-rw-rw-   0        0        0     5162 2023-01-01 05:35:30.000000 finfactory-0.1.25/finfactory/get_data/tushare_futures_info.py
+-rw-rw-rw-   0        0        0     8290 2023-01-01 05:35:30.000000 finfactory-0.1.25/finfactory/get_data/tushare_futures_mapping.py
+-rw-rw-rw-   0        0        0     7949 2023-01-01 05:35:30.000000 finfactory-0.1.25/finfactory/get_data/tushare_index_daily.py
+-rw-rw-rw-   0        0        0     8452 2023-01-01 05:35:30.000000 finfactory-0.1.25/finfactory/get_data/tushare_index_daily_basic.py
+-rw-rw-rw-   0        0        0     4794 2023-01-01 05:35:30.000000 finfactory-0.1.25/finfactory/get_data/tushare_index_info.py
+-rw-rw-rw-   0        0        0     6135 2023-01-01 05:35:30.000000 finfactory-0.1.25/finfactory/get_data/tushare_lpr.py
+-rw-rw-rw-   0        0        0     9564 2023-01-01 05:35:30.000000 finfactory-0.1.25/finfactory/get_data/tushare_options_daily.py
+-rw-rw-rw-   0        0        0     7238 2023-01-01 05:35:30.000000 finfactory-0.1.25/finfactory/get_data/tushare_options_info.py
+-rw-rw-rw-   0        0        0     7846 2023-01-01 05:35:31.000000 finfactory-0.1.25/finfactory/get_data/tushare_rzrq_daily.py
+-rw-rw-rw-   0        0        0     6344 2023-01-01 05:35:31.000000 finfactory-0.1.25/finfactory/get_data/tushare_shibor.py
+-rw-rw-rw-   0        0        0     9988 2023-01-01 05:35:31.000000 finfactory-0.1.25/finfactory/get_data/tushare_stock_daily.py
+-rw-rw-rw-   0        0        0    10237 2023-01-01 05:35:31.000000 finfactory-0.1.25/finfactory/get_data/tushare_stock_daily_basic.py
+-rw-rw-rw-   0        0        0    10205 2023-01-01 05:35:31.000000 finfactory-0.1.25/finfactory/get_data/tushare_stock_daily_stk.py
+-rw-rw-rw-   0        0        0     9673 2023-01-01 05:35:31.000000 finfactory-0.1.25/finfactory/get_data/tushare_stock_top10holders.py
+-rw-rw-rw-   0        0        0    10096 2023-01-01 05:35:31.000000 finfactory-0.1.25/finfactory/get_data/tushare_stock_top10holders_free.py
+-rw-rw-rw-   0        0        0     9425 2023-01-01 05:35:31.000000 finfactory-0.1.25/finfactory/get_data/tushare_stock_zjc.py
+-rw-rw-rw-   0        0        0    12098 2023-01-01 05:35:31.000000 finfactory-0.1.25/finfactory/get_data/tushare_stocks_daily.py
+-rw-rw-rw-   0        0        0    11396 2023-01-01 05:35:31.000000 finfactory-0.1.25/finfactory/get_data/tushare_stocks_daily_basic.py
+-rw-rw-rw-   0        0        0    11369 2023-01-01 05:35:31.000000 finfactory-0.1.25/finfactory/get_data/tushare_stocks_daily_stk.py
+-rw-rw-rw-   0        0        0     7975 2023-02-08 04:11:06.000000 finfactory-0.1.25/finfactory/get_data/tushare_trade_dates.py
+-rw-rw-rw-   0        0        0     6669 2023-01-01 05:35:31.000000 finfactory-0.1.25/finfactory/get_data/tushare_usa_bond_rates.py
+-rw-rw-rw-   0        0        0     6609 2023-01-01 05:35:32.000000 finfactory-0.1.25/finfactory/get_data/tushare_usa_bond_rates_act.py
+-rw-rw-rw-   0        0        0      952 2022-08-04 06:39:56.000000 finfactory-0.1.25/finfactory/install_check.py
+-rw-rw-rw-   0        0        0    28000 2023-04-01 10:51:40.000000 finfactory-0.1.25/finfactory/load_his_data.py
+drwxrwxrwx   0        0        0        0 2023-05-21 02:58:21.298860 finfactory-0.1.25/finfactory/utils/
+-rw-rw-rw-   0        0        0       25 2022-06-08 01:24:02.000000 finfactory-0.1.25/finfactory/utils/__init__.py
+-rw-rw-rw-   0        0        0    10456 2022-12-11 13:20:01.000000 finfactory-0.1.25/finfactory/utils/utils.py
+-rw-rw-rw-   0        0        0     5914 2023-03-24 14:16:56.000000 finfactory-0.1.25/finfactory/utils/utils_crypto.py
+drwxrwxrwx   0        0        0        0 2023-05-21 02:58:21.234032 finfactory-0.1.25/finfactory.egg-info/
+-rw-rw-rw-   0        0        0      994 2023-05-21 02:58:21.000000 finfactory-0.1.25/finfactory.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3480 2023-05-21 02:58:21.000000 finfactory-0.1.25/finfactory.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-21 02:58:21.000000 finfactory-0.1.25/finfactory.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-21 02:58:21.000000 finfactory-0.1.25/finfactory.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-21 02:58:21.300853 finfactory-0.1.25/setup.cfg
+-rw-rw-rw-   0        0        0     1234 2022-10-23 14:13:58.000000 finfactory-0.1.25/setup.py
```

### Comparing `finfactory-0.1.24/PKG-INFO` & `finfactory-0.1.25/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: finfactory
-Version: 0.1.24
+Version: 0.1.25
 Summary: FinFactory is a financial toolbox.
 Home-page: https://github.com/Genlovy-Hoo/finfactory/
 Author: Genlovy Hoo, YueYong Hu
 Author-email: genlovhyy@163.com
 License: MIT
 Platform: any
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 ## 欢迎使用FinFactory
 
 FinFactory是一个金融研究工具箱，其目标是使金融研究更便捷和高效。
 
 FfnFactory的主要工具（将）包括：金融数据下载、清洗整理、因子开发及计算、常用金融模型计算工具、量化策略工具。
 
@@ -33,9 +34,7 @@
 
 Pypi
 
 [finfactory](https://pypi.org/project/finfactory/)
 
 感谢使用和支持！
 
-
-
```

### Comparing `finfactory-0.1.24/README.md` & `finfactory-0.1.25/README.md`

 * *Files identical despite different names*

### Comparing `finfactory-0.1.24/finfactory/_pkg_info.py` & `finfactory-0.1.25/finfactory/_pkg_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 pkg_info = {
     '__pkgname__': 'finfactory',
-    '__version__': '0.1.24',
+    '__version__': '0.1.25',
     '__license__': 'MIT',
     '__url__': 'https://github.com/Genlovy-Hoo/finfactory/',
     '__urls__':
         {'pypi': 'https://pypi.org/project/finfactory/',
          'github': 'https://github.com/Genlovy-Hoo/finfactory/',
 		 'document': 'http://www.glhyy.cn/finfactory/doc/html/index.html'
         },
```

### Comparing `finfactory-0.1.24/finfactory/config.py` & `finfactory-0.1.25/finfactory/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 import os
 from pathlib import Path
 from dramkit import isnull
-from dramkit import StructureObject
+from dramkit import GenObject
 from dramkit.iotools import load_yml
 
 
 FILE_PATH = Path(os.path.realpath(__file__))
 
 
 # 默认配置文件路径查找顺序，根据需要修改
@@ -28,17 +28,17 @@
 for fpath in config_paths:
     if os.path.exists(fpath):
         cfg_path = fpath
         break
 
 if not isnull(cfg_path):
     cfg_yml = load_yml(cfg_path, encoding='utf-8')
-    cfg = StructureObject(**cfg_yml)
+    cfg = GenObject(**cfg_yml)
 else:    
-    cfg = StructureObject()
+    cfg = GenObject()
 
 # 根据需要修改下面的参数
 cfg.set_from_dict(
     {
     # 默认数据存档根目录
     'archive_roots': [
         'D:/FinFactory/data/archives/',
```

### Comparing `finfactory-0.1.24/finfactory/findata/api.py` & `finfactory-0.1.25/finfactory/findata/api.py`

 * *Files identical despite different names*

### Comparing `finfactory-0.1.24/finfactory/finplot/_mpfold.py` & `finfactory-0.1.25/finfactory/finplot/_mpfold.py`

 * *Files identical despite different names*

### Comparing `finfactory-0.1.24/finfactory/finplot/_plot_candle_deprecated.py` & `finfactory-0.1.25/finfactory/finplot/_plot_candle_deprecated.py`

 * *Files identical despite different names*

### Comparing `finfactory-0.1.24/finfactory/finplot/finplot.py` & `finfactory-0.1.25/finfactory/finplot/finplot.py`

 * *Files identical despite different names*

### Comparing `finfactory-0.1.24/finfactory/finplot/plot_candle.py` & `finfactory-0.1.25/finfactory/finplot/plot_candle.py`

 * *Files 1% similar despite different names*

```diff
@@ -465,17 +465,16 @@
     if fig_save_path:
         plt.savefig(fig_save_path)
 
     plt.show()
 
 
 if __name__ == '__main__':
-    import time
-    from dramkit import load_csv
-    strt_tm = time.time()
+    from dramkit import load_csv, TimeRecoder
+    tr = TimeRecoder()
 
     daily_50etf_pre_fq_path = '../_test/510050.SH_daily_qfq.csv'
     data = load_csv(daily_50etf_pre_fq_path)
     data['time'] = data['date'].copy()
     data.set_index('time', drop=False, inplace=True)
     tcol = 'time'
     data = data.reindex(columns=['time', 'open', 'low', 'high', 'close',
@@ -496,15 +495,15 @@
         data.loc[data.index[k], 'sig_low'] = -1
     data['sig_avg'] = 0
     for k in range(9, data.shape[0]-5, 11):
         data.loc[data.index[k], 'sig_avg'] = 1
     for k in range(13, data.shape[0]-5, 17):
         data.loc[data.index[k], 'sig_avg'] = -1
 
-    data = data.iloc[-500:, :].copy()
+    data = data.iloc[-800:, :].copy()
 
     args_ma = None
     # args_ma = [5, 10, 20, 30, 50]
     # args_boll = None
     args_boll = [15, 2]
     # cols_other_upleft = {}
     cols_other_upleft = {'Pavg1': ('m-', None)}
@@ -564,8 +563,8 @@
                 ylabels=ylabels, xlabels=xlabels, yscales=yscales,
                 figsize=figsize, fig_save_path=fig_save_path, title=title,
                 fontsize_label=fontsize_label, fontsize_legend=fontsize_legend,
                 width=width, alpha=alpha,
                 grid=grid, markersize=markersize, n_xticks=n_xticks)
 
 
-    print('used time: {}s.'.format(round(time.time()-strt_tm, 6)))
+    tr.used()
```

### Comparing `finfactory-0.1.24/finfactory/fintools/__init__.py` & `finfactory-0.1.25/finfactory/fintools/__init__.py`

 * *Files identical despite different names*

### Comparing `finfactory-0.1.24/finfactory/fintools/cal_sig_gains.py` & `finfactory-0.1.25/finfactory/fintools/cal_sig_gains.py`

 * *Files identical despite different names*

### Comparing `finfactory-0.1.24/finfactory/fintools/cal_sig_gains_bk.py` & `finfactory-0.1.25/finfactory/fintools/cal_sig_gains_bk.py`

 * *Files identical despite different names*

### Comparing `finfactory-0.1.24/finfactory/fintools/copy_line.py` & `finfactory-0.1.25/finfactory/fintools/copy_line.py`

 * *Files identical despite different names*

### Comparing `finfactory-0.1.24/finfactory/fintools/fintools.py` & `finfactory-0.1.25/finfactory/fintools/fintools.py`

 * *Files 1% similar despite different names*

```diff
@@ -973,22 +973,21 @@
     df['signal'] = cross2_plot(df, 'rmax2now', thr_rmax2now, 'rmin2now',
                                thr_rmin2now, buy_sig=buy_sig, sel_sig=sel_sig,
                                col_price=col_price, plot=plot, **kwargs_plot)
     return df['signal']
 
 #%%
 if __name__ == '__main__':
-    import time
-    from dramkit import load_csv
-    from dramkit.gentools import get_preval_func_cond
-    from dramkit.gentools import replace_repeat_iter
+    from dramkit import load_csv, TimeRecoder
+    from dramkit.gentools import (get_preval_func_cond,
+                                  replace_repeat_iter)
     from finfactory.finplot.plot_candle import plot_candle
     from finfactory.fintools.utils_gains import get_yield_curve
 
-    strt_tm = time.time()
+    tr = TimeRecoder()
 
     #%%
     # 50ETF日线行情
     fpath = '../_test/510050.SH_daily_qfq.csv'
     df = load_csv(fpath)
     df.set_index('date', drop=False, inplace=True)
     # df = df.reindex(columns=['high', 'low', 'close'])
@@ -1127,8 +1126,8 @@
     # VRI
     df['vri'] = vri(df, n=5)
     plot_series(df.iloc[-1000:, :], {'close': '.-k'},
                 cols_styl_up_right={'vri': '.-b'},
                 xparls_info={'vri': [(0, 'b', '-', 1.0)]})
 
     #%%
-    print('used time: {}s.'.format(round(time.time()-strt_tm, 6)))
+    tr.used()
```

### Comparing `finfactory-0.1.24/finfactory/fintools/fundnet.py` & `finfactory-0.1.25/finfactory/fintools/fundnet.py`

 * *Files identical despite different names*

### Comparing `finfactory-0.1.24/finfactory/fintools/options.py` & `finfactory-0.1.25/finfactory/fintools/options.py`

 * *Files identical despite different names*

### Comparing `finfactory-0.1.24/finfactory/fintools/utils_chn.py` & `finfactory-0.1.25/finfactory/fintools/utils_chn.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,20 +1,26 @@
 # -*- coding: utf-8 -*-
 
 import calendar
+import datetime
 import numpy as np
 import pandas as pd
 from itertools import product
-import datetime
+from typing import Union
 from dateutil.relativedelta import relativedelta
 import chncal
 from chncal import is_tradeday
 from dramkit.gentools import (isnull,
                               sort_dict,
-                              print_used_time)
+                              print_used_time,
+                              get_preval_func_cond,
+                              check_list_arg,
+                              get_full_df,
+                              get_full_components_df,
+                              DateTimeType)
 from dramkit import datetimetools as dttools
 
 
 # 上市公司公告披露日期：https://zhuanlan.zhihu.com/p/29007967
 # http://www.csrc.gov.cn/pub/zjhpublic/zjh/202103/t20210319_394491.htm
 # https://xueqiu.com/5749132507/142221762
 # https://zhuanlan.zhihu.com/p/127156379
@@ -162,18 +168,21 @@
     assert edge in ['start', 'end']
     if isnull(date):
         date = datetime.date.today()
     if not is_tradeday(date, market=market):
         return False
     date = dttools.x2datetime(date)
     n = 1 if edge == 'end' else -1
-    next_ = pd.to_datetime(chncal.get_next_nth_tradeday(date, n=n))
+    next_ = pd.to_datetime(chncal.get_next_nth_tradeday(date, n=n, market=market))
     if eval('next_.%s != date.%s'%(period, period)):
         return True
-    return False
+    else:
+        if n == -1 and date == next_:
+            return True
+        return False
 
 
 def is_weekend_tradeday(date=None, market='SSE'):
     '''判断是否为一周的最后一个交易日'''
     return is_period_edge_tradeday('week', 'end', date=date, market=market)
 
 
@@ -208,14 +217,250 @@
 
 
 def is_yearstart_tradeday(date=None, market='SSE'):
     '''判断是否为年度的第一个交易日'''
     return is_period_edge_tradeday('year', 'start', date=date, market=market)
 
 
+def is_periods_edge_tradeday(periods, edge, date=None, market='SSE'):
+    '''
+    | 判断是否为指定周期的最后一个交易日或第一个交易日
+    | periods: 'week'周, 'month'月, 'quarter'季度, 'year'年度 的列表
+    | edge: 'start'首个交易日, 'end'最后一个交易日
+    '''
+    assert all([p in ['week', 'month', 'quarter', 'year'] for p in periods])
+    assert edge in ['start', 'end']
+    if isnull(date):
+        date = datetime.date.today()
+    if not is_tradeday(date, market=market):
+        return [0]*len(periods)
+    date = dttools.x2datetime(date)
+    n = 1 if edge == 'end' else -1
+    next_ = pd.to_datetime(chncal.get_next_nth_tradeday(date, n=n, market=market))
+    res = []
+    for period in periods:
+        if eval('next_.%s != date.%s'%(period, period)):
+            res.append(1)
+        else:
+            if n == -1 and date == next_:
+                res.append(1)
+            else:
+                res.append(0)
+    return res
+
+
+def get_all_trade_dates(markets='SSE', **kwargs):
+    markets = check_list_arg(markets, allow_none=True)
+    from chncal.constants_trade_dates import trade_dates
+    df = pd.Series(trade_dates)
+    df = df.reset_index()
+    df.columns = ['market', 'date', 'if_trade']
+    if not isnull(markets):
+        df = df[df['market'].isin(markets)]
+    df['date'] = pd.to_datetime(df['date'])
+    dtmax = dttools.time_add(df['date'].max(), days=1)
+    if dtmax.date() <= datetime.date.today():
+        df1 = []
+        for market in df['market'].unique().tolist():
+            dates = get_trade_dates(dtmax, market=market)
+            dates_ = pd.date_range(dtmax, datetime.date.today()).tolist()
+            tmp = [[market, x, 1 if x in dates else 0] for x in dates_]
+            df1 += tmp
+        df1 = pd.DataFrame(df1, columns=df.columns)
+        df = pd.concat((df, df1), axis=0)
+    df = df.sort_values(['market', 'date'])
+    df = df.drop_duplicates(subset=['market', 'date'])
+    return df.reset_index(drop=True)
+
+
+# @print_used_time
+def add_trade_dates_end(df):
+    freqs = ['week', 'month', 'quarter', 'year']
+    ends = df[['market', 'date']].apply(lambda x:
+                 is_periods_edge_tradeday(
+                     freqs, 'end',
+                     x['date'], x['market']), axis=1)
+    ends = ends.apply(lambda x: x[k] for k in range(4))
+    ends.columns = ['%s_end'%x for x in freqs]
+    df[list(ends.columns)] = ends
+    return df
+
+
+# @print_used_time
+def add_trade_dates_start(df):
+    freqs = ['week', 'month', 'quarter', 'year']
+    starts = df[['market', 'date']].apply(lambda x:
+                 is_periods_edge_tradeday(
+                     freqs, 'start',
+                     x['date'], x['market']), axis=1)
+    starts = starts.apply(lambda x: x[k] for k in range(4))
+    starts.columns = ['%s_start'%x for x in freqs]
+    df[list(starts.columns)] = starts
+    return df
+
+
+def add_trade_dates_pre(df, freq, edge):
+    '''
+    | df = get_all_trade_dates()
+    | freq in ['week', 'month', 'quarter', 'year']
+    | edge in ['start', 'end']
+    '''
+    def _tmp(df):
+        df['pre_%s_%s'%(freq, edge)] = get_preval_func_cond(
+            df, 'date', '%s_%s'%(freq, edge), lambda x: x == 1)
+        return df
+    return df.groupby('market', as_index=False).apply(_tmp)
+
+
+def add_trade_dates_next(df, freq, edge):
+    '''
+    | df = get_all_trade_dates()
+    | freq in ['week', 'month', 'quarter', 'year']
+    | edge in ['start', 'end']
+    '''
+    def _tmp(df):
+        df = df[::-1].copy()
+        df['next_%s_%s'%(freq, edge)] = get_preval_func_cond(
+            df, 'date', '%s_%s'%(freq, edge), lambda x: x == 1)
+        return df[::-1]
+    return df.groupby('market', as_index=False).apply(_tmp)
+
+
+def get_dates_cond(cond, date_min, date_max=None, market='SSE'):
+    assert cond in [
+        'nature',
+        'week1', 'week2', 'week3', 'week4', 'week5', 'week6', 'week7',
+        'month_end', 'quarter_end', 'year_end',
+        'month_start', 'quarter_start', 'year_start',
+        'finreport',
+        'trade',
+        'trade_week_end', 'trade_month_end', 'trade_quarter_end', 'trade_year_end',
+        'trade_week_start', 'trade_month_start', 'trade_quarter_start', 'trade_year_start']
+    if isnull(date_max):
+        date_max = dttools.today_date()
+    date_min = dttools.x2datetime(date_min)
+    date_max = dttools.x2datetime(date_max)
+    if cond == 'nature' or cond.startswith('week'):
+        dates = dttools.get_dates_between(date_min, date_max, keep1=True)
+        if cond.startswith('week'):
+            n = int(cond[-1])
+            dates = [x for x in dates if x.weekday() == n-1]
+    elif cond in ['month_end', 'quarter_end', 'year_end',
+                  'month_start', 'quarter_start', 'year_start']:
+        freq = cond.split('_')[0]
+        edge = cond.split('_')[-1]
+        dates = dttools.get_dates_between(date_min, date_max, keep1=True)
+        dates = [x for x in dates if eval('x.is_%s_%s'%(freq, edge))]
+    elif cond == 'finreport':
+        dates = get_finreport_dates(date_min, date_max,
+                                    end_dirt='post')
+    else:
+        dft = get_all_trade_dates(market=market)
+        dft = dft[(dft['date'] >= date_min) & (dft['date'] <= date_max)]
+        if cond == 'trade':
+            dates = dft[dft['if_trade'] == 1]['date'].tolist()
+        elif cond.startswith('trade') and cond.endswith('_end'):
+            dft = add_trade_dates_end(dft)
+            freq = cond.split('_')[1]
+            dates = dft[dft['%s_end'%freq] == 1]['date'].tolist()
+        elif cond.startswith('trade') and cond.endswith('_start'):
+            dft = add_trade_dates_start(dft)
+            freq = cond.split('_')[1]
+            dates = dft[dft['%s_start'%freq] == 1]['date'].tolist()
+    return dates
+
+
+def df_freq_low2high(df, tcol, idcols, vcols=None,
+                     tmin=None, tmax=None, tall='trade',
+                     **kwargs):
+    '''
+    数据低频填充为高频
+    
+    Examples
+    --------
+    >>> df = pd.DataFrame(
+    ...         {'end_date': ['20220101', '20220605', '20220910', '20221010',
+    ...                       '20220205', '20220708', '20221005', '20221010'],
+    ...          'code': ['000001.SH']*4+['000002.SZ']*4,
+    ...          'cate': ['a', 'b', 'a', 'b', 'c', 'd', 'c', 'd'],
+    ...          'value1': [1, 2, np.nan, 3, 3, np.nan, 4, 5],
+    ...          'value2': [None, 3, np.nan, 4, 6, 5, np.nan, 7]})
+    >>> vcols = None # 'value1'
+    >>> tcol = 'end_date'
+    >>> idcols1 = 'code'
+    >>> df1 = df_freq_low2high(df, tcol, idcols1, vcols=vcols)
+    >>> idcols2 = ['code', 'cate']
+    >>> df2 = df_freq_low2high(df, tcol, idcols2, vcols=vcols)
+    '''
+    frmt_tm = df[tcol].iloc[0]    
+    df = df.copy()
+    df[tcol] = pd.to_datetime(df[tcol])
+    if isnull(tmin):
+        tmin = df[tcol].min()
+    if isnull(tmax):
+        tmax = df[tcol].max()
+    times = get_dates_cond(tall, tmin, tmax)
+    df = get_full_df(df, tcol, times,
+                     idcols=idcols,
+                     vcols=vcols,
+                     **kwargs)
+    df[tcol] = dttools.copy_format(df[tcol], frmt_tm)    
+    return df
+
+
+def get_full_components(df: pd.DataFrame,
+                        parent_col: str,
+                        child_col: str,
+                        tincol: str,
+                        toutcol: str,
+                        tfulls: str,
+                        tstart: Union[DateTimeType, None] = None,
+                        tend: Union[DateTimeType, None] = None,
+                        toutnan: Union[DateTimeType, None] = None,
+                        tcol_res: str = 'time',
+                        keep_inout: bool = False
+                        ):
+    '''
+    | 根据纳入、退出日期获取在给定时间内的所有成分
+    
+    Example
+    -------
+    >>> df = pd.DataFrame(
+    ...      {'index': ['a', 'a', 'b', 'b', 'a', 'c', 'c'],
+    ...       'stock': ['a1', 'a2', 'b1', 'b2', 'a3', 'c1', 'c2'],
+    ...       'indate': ['20210101', '20210515', '20210405', '20210206',
+    ...                  '20220307', '20220910', '20230409'],
+    ...       'outdate': ['20220305', np.nan, np.nan, '20230409',
+    ...                   np.nan, np.nan, '20230518']})
+    >>> parent_col, child_col, tincol, toutcol = 'index', 'stock', 'indate', 'outdate'
+    >>> tfulls = 'trade_month_end'
+    >>> df['indate'] = pd.to_datetime(df['indate'])
+    >>> df['outdate'] = pd.to_datetime(df['outdate'])
+    >>> df1 = get_full_components(
+    ...       df, parent_col, child_col, tincol, toutcol, tfulls)
+    '''
+    df = df[[parent_col, child_col, tincol, toutcol]].copy()
+    frmt_tm = df[tincol].iloc[0]
+    df[tincol] = pd.to_datetime(df[tincol])
+    df[toutcol] = pd.to_datetime(df[toutcol])
+    if isnull(tstart):
+        tstart = df[tincol].min()
+    if isnull(tend):
+        tend = pd.to_datetime(datetime.date.today())
+    if isnull(toutnan):
+        toutnan = pd.to_datetime(datetime.date.today())
+    times = get_dates_cond(tfulls, tstart, tend)
+    res = get_full_components_df(
+            df, parent_col, child_col, tincol, toutcol,
+            times, toutnan, tcol_res=tcol_res, keep_inout=keep_inout)
+    fmtcols = [tincol, toutcol, tcol_res] if keep_inout else [tcol_res]
+    for c in fmtcols:
+        res[c] = dttools.copy_format(res[c], frmt_tm)
+    return res
+    
 
 
 
 # @print_used_time
 def merge_minute_candle(data, new_freq=30, cols_sum=None,
                         tstart=False, time_trans=False):
     '''
@@ -633,83 +878,14 @@
 
 
 def check_fill_trade_dates(df, date_col='date',
                            fill_func={}):
     '''检查并填充交易日'''
     raise NotImplementedError
 
-
-def check_list_str_arg(arg, allow_none=False):
-    if allow_none:
-        assert isinstance(arg, (type(None), str, list, tuple))
-    else:
-        assert isinstance(arg, (str, list, tuple))
-    if isinstance(arg, str):
-        arg = [arg]
-    return arg
-
-
-def df_freq_low2high(df, tcol, id_cols, vcols=None,
-                     tmin=None, tmax=None, tall='trade',
-                     keepna=False, fill_1st2last=False):
-    '''
-    低频数据填充为高频
-    
-    TODO
-    ----
-    函数待完善
-    
-    Examples
-    --------
-    >>> df = pd.DataFrame(
-    ...         {'end_date': ['20220101', '20220605', '20220910', '20221010',
-    ...                       '20220205', '20220708', '20221005', '20221010'],
-    ...          'code': ['000001.SH']*4+['000002.SZ']*4,
-    ...          'cate': ['a', 'b', 'a', 'b', 'c', 'd', 'c', 'd'],
-    ...          'value1': [1, 2, np.nan, 3, 3, np.nan, 4, 5],
-    ...          'value2': [None, 3, np.nan, 4, 6, 5, np.nan, 7]})
-    >>> vcols = None # 'value1'
-    >>> tcol = 'end_date'
-    >>> id_cols1 = 'code'
-    >>> df1 = df_freq_low2high(df, tcol, id_cols1, vcols=vcols)
-    >>> id_cols2 = ['code', 'cate']
-    >>> df2 = df_freq_low2high(df, tcol, id_cols2, vcols=vcols)
-    '''
-    vcols = check_list_str_arg(vcols, allow_none=True)
-    id_cols = check_list_str_arg(id_cols)
-    assert tall in ['nature', 'trade', 'finreport']
-    if isnull(tmin):
-        tmin = df[tcol].min()
-    _, joiner = dttools.get_date_format(tmin)
-    if isnull(tmax):
-        # tmax = df[tcol].max()
-        tmax = dttools.today_date('')
-    if tall == 'nature':
-        dates = dttools.get_dates_between(tmin, tmax,
-                                          keep1=True, joiner=1)
-    elif tall == 'trade':
-        dates = get_trade_dates(tmin, tmax, joiner=1)
-    elif tall == 'finreport':
-        dates = get_finreport_dates(tmin, tmax, joiner=joiner)
-    if keepna:
-        df = df.fillna('__tmp_None_tmp__')
-    df = df.pivot_table(values=vcols, index=tcol, columns=id_cols,
-                        aggfunc=lambda x: x)
-    index_all = dates + list(df.index)
-    index_all.sort()
-    df = df.reindex(index=index_all)
-    df = df.fillna(method='ffill')
-    df = df.stack(level=id_cols).reset_index()
-    df = df.replace({'__tmp_None_tmp__': np.nan})
-    df = df.sort_values(id_cols+[tcol])
-    return df
-    
-    
-    
-
```

### Comparing `finfactory-0.1.24/finfactory/fintools/utils_gains.py` & `finfactory-0.1.25/finfactory/fintools/utils_gains.py`

 * *Files 0% similar despite different names*

```diff
@@ -2741,15 +2741,16 @@
     '''根据每期收益和成本/资金占用计算收益曲线'''
 
     assert net_type in ['fundnet', 'prod', 'sum', 'maxused_act', 'maxused_final']
 
     # 价格列检查
     if isnull(col_price) and \
                 (show_mkt or (ext_type is not False and not isnull(ext_type))):
-        logger_show('未识别价格列，收益曲线无法与市场基准比较！', logger, 'warn')
+        if show_mkt:
+            logger_show('未识别价格列，收益曲线无法与市场基准比较！', logger, 'warn')
     if isnull(col_price):
         show_mkt = False
         df = data.reindex(columns=[col_gain, col_cost])
     else:
         df = data.reindex(columns=[col_gain, col_cost, col_price])
 
     df[col_gain] = df[col_gain].fillna(0)
@@ -3001,19 +3002,18 @@
             print('夏普比率：{}'.format(round(gain_info['夏普'], 4)))
             print('最大回撤区间长度: {}'.format(round(gain_info['最大回撤区间长度'], 4)))
 
     return gain_info, df
 
 #%%
 if __name__ == '__main__':
-    import time
     from pprint import pprint
-    from dramkit import load_csv
+    from dramkit import load_csv, TimeRecoder
 
-    strt_tm = time.time()
+    tr = TimeRecoder()
 
     #%%
     # 最大回撤测试
     values = [1.0, 1.01, 1.05, 1.1, 1.11, 1.07, 1.03, 1.03, 1.01, 1.02, 1.04,
               1.05, 1.07, 1.06, 1.05, 1.06, 1.07, 1.09, 1.12, 1.18, 1.15,
               1.15, 1.18, 1.16, 1.19, 1.17, 1.17, 1.18, 1.19, 1.23, 1.24,
               1.25, 1.24, 1.25, 1.24, 1.25, 1.24, 1.25, 1.24, 1.27, 1.23,
@@ -3248,8 +3248,8 @@
         {'gain': [10, 20 , 5, -5, -10, 1, 3, 20, 30, -15],
          'cost': [100, 110, 100, 120, 100, 100, 100, 90, 80, 100]}
         )
     gain_info, df = get_yield_curve2(data, 'gain', 'cost',
                                      net_type='sum')
 
     #%%
-    print('used time: {}s.'.format(round(time.time()-strt_tm, 6)))
+    tr.used()
```

### Comparing `finfactory-0.1.24/finfactory/get_data/_ccxt.py` & `finfactory-0.1.25/finfactory/get_data/_ccxt.py`

 * *Files identical despite different names*

### Comparing `finfactory-0.1.24/finfactory/get_data/_get_data.py` & `finfactory-0.1.25/finfactory/get_data/_get_data.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 # -*- coding: utf-8 -*-
 
 if __name__ == '__main__':
 
     import traceback
-    from dramkit import simple_logger
-    from dramkit import logger_show
-    try:
+    from dramkit import (simple_logger,
+                         logger_show,
+                         TimeRecoder)
+    tr = TimeRecoder()
+    
+    try:        
         import sys
         import time
         from dramkit import TimeRecoder
         from dramkit import close_log_file
         from dramkit.iotools import cmd_run_pys
         from dramkit.iotools import cmd_run_pys_multi_process
         from finfactory.utils.utils import gen_py_logger
@@ -62,15 +65,15 @@
             'eastmoney_tonorth_netbuy_daily.py',
             'eastmoney_tonorth_netin_daily.py',
             'eastmoney_tosouth_netbuy_daily.py',
             'eastmoney_tosouth_netin_daily.py',
             
             'sw_daily_info.py',
             
-            'fundex_index_dpe.py',
+            # 'fundex_index_dpe.py',
             
             'tushare_stocks_daily.py',
             'tushare_stocks_daily_basic.py',
             'tushare_stocks_daily_stk.py',
             # 'tushare_stock_daily.py',
             # 'tushare_stock_daily_basic.py',
             # 'tushare_stock_daily_stk.py',
@@ -95,14 +98,15 @@
         cmd_run_pys_multi_process(files, logger,
                                   multi_line=5,
                                   keep_order=True)
         
         
         tr.used(logger)
         close_log_file(logger)
-    
     except:
         logger = simple_logger('../../log/_get_data.log', 'a')
         logger_show(traceback.format_exc(), logger, 'error')
         logger_show('运行出错！', logger, 'error')
         close_log_file(logger)
+        
+    tr.used()
```

### Comparing `finfactory-0.1.24/finfactory/get_data/_jq_opts_minute_check.py` & `finfactory-0.1.25/finfactory/get_data/_jq_opts_minute_check.py`

 * *Files identical despite different names*

### Comparing `finfactory-0.1.24/finfactory/get_data/_split_data.py` & `finfactory-0.1.25/finfactory/get_data/_split_data.py`

 * *Files identical despite different names*

### Comparing `finfactory-0.1.24/finfactory/get_data/_stocks_cut.py` & `finfactory-0.1.25/finfactory/get_data/_stocks_cut.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,15 +20,16 @@
         if df.shape[0] > 0:
             df.to_csv(fpath, encoding='gbk', index=None)
         else:
             tqdm.write('{}无数据'.format(c))
 
 
 if __name__ == '__main__':
-    strt_tm = time.time()
+    from dramkit import TimeRecoder
+    tr = TimeRecoder()
     
     
     # 单只股票数据存放路径
     fdir = find_target_dir('stocks/tushare/')
     codes = [x for x in os.listdir(fdir) if x not in \
                  ['stocks_daily', 'stocks_holders']]
     dirs = {x: fdir+x for x in codes if os.path.isdir(fdir+x)}
@@ -39,9 +40,9 @@
     # # top10holders_free
     # df_top10holders_free = cut_holder(dirs, 'top10holders_free')
     
     # # zjc
     # df_zjc = cut_holder(dirs, 'zjc')
     
     
-    print(f'\nused time: {round(time.time()-strt_tm, 6)}s.')
+    tr.used()
```

### Comparing `finfactory-0.1.24/finfactory/get_data/_stocks_merge.py` & `finfactory-0.1.25/finfactory/get_data/_stocks_merge.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,17 +48,18 @@
     data.reset_index(drop=True, inplace=True)
     data.to_csv('{}stocks_holders/astocks_{}.csv'.format(fdir, ext),
                 index=None)
     return data
 
 
 if __name__ == '__main__':
+    from dramkit import TimeRecoder
     from finfactory.load_his_data import find_target_dir
     
-    strt_tm = time.time()
+    tr = TimeRecoder()
     
     
     # 单只股票数据存放路径
     fdir = find_target_dir('stocks/tushare/')
     codes = [x for x in os.listdir(fdir) if x not in \
                  ['stocks_daily', 'stocks_holders']]
     dirs = {x: fdir+x for x in codes if os.path.isdir(fdir+x)}
@@ -83,9 +84,9 @@
     #                         ['code', '报告期', 'holder_name'])
     
     # # zjc
     # df_zjc = merge_holder(dirs, 'zjc',
     #                       ['code', '公告日期', 'holder_name'])
     
     
-    print('\nused time: {}s.'.format(round(time.time()-strt_tm, 6)))
+    tr.used()
```

### Comparing `finfactory-0.1.24/finfactory/get_data/ccxt_1d.py` & `finfactory-0.1.25/finfactory/get_data/ccxt_1d.py`

 * *Files identical despite different names*

### Comparing `finfactory-0.1.24/finfactory/get_data/ccxt_minute.py` & `finfactory-0.1.25/finfactory/get_data/ccxt_minute.py`

 * *Files identical despite different names*

### Comparing `finfactory-0.1.24/finfactory/get_data/cffex_futures_lhb.py` & `finfactory-0.1.25/finfactory/get_data/cffex_futures_lhb.py`

 * *Files identical despite different names*

### Comparing `finfactory-0.1.24/finfactory/get_data/chn_local_bond_rates.py` & `finfactory-0.1.25/finfactory/get_data/chn_local_bond_rates.py`

 * *Files identical despite different names*

### Comparing `finfactory-0.1.24/finfactory/get_data/chn_national_bond_rates.py` & `finfactory-0.1.25/finfactory/get_data/chn_national_bond_rates.py`

 * *Files identical despite different names*

### Comparing `finfactory-0.1.24/finfactory/get_data/eastmoney.py` & `finfactory-0.1.25/finfactory/get_data/eastmoney.py`

 * *Files identical despite different names*

### Comparing `finfactory-0.1.24/finfactory/get_data/eastmoney_tonorth_netbuy_daily.py` & `finfactory-0.1.25/finfactory/get_data/eastmoney_tonorth_netbuy_daily.py`

 * *Files identical despite different names*

### Comparing `finfactory-0.1.24/finfactory/get_data/eastmoney_tonorth_netin_daily.py` & `finfactory-0.1.25/finfactory/get_data/eastmoney_tonorth_netin_daily.py`

 * *Files identical despite different names*

### Comparing `finfactory-0.1.24/finfactory/get_data/eastmoney_tosouth_netbuy_daily.py` & `finfactory-0.1.25/finfactory/get_data/eastmoney_tosouth_netbuy_daily.py`

 * *Files identical despite different names*

### Comparing `finfactory-0.1.24/finfactory/get_data/eastmoney_tosouth_netin_daily.py` & `finfactory-0.1.25/finfactory/get_data/eastmoney_tosouth_netin_daily.py`

 * *Files identical despite different names*

### Comparing `finfactory-0.1.24/finfactory/get_data/ef.py` & `finfactory-0.1.25/finfactory/get_data/ef.py`

 * *Files identical despite different names*

### Comparing `finfactory-0.1.24/finfactory/get_data/eniu_index_pe.py` & `finfactory-0.1.25/finfactory/get_data/eniu_index_pe.py`

 * *Files identical despite different names*

### Comparing `finfactory-0.1.24/finfactory/get_data/fundex_index_dpe.py` & `finfactory-0.1.25/finfactory/get_data/fundex_index_dpe.py`

 * *Files identical despite different names*

### Comparing `finfactory-0.1.24/finfactory/get_data/hexun_gold_daily.py` & `finfactory-0.1.25/finfactory/get_data/hexun_gold_daily.py`

 * *Files identical despite different names*

### Comparing `finfactory-0.1.24/finfactory/get_data/hexun_silver_daily.py` & `finfactory-0.1.25/finfactory/get_data/hexun_silver_daily.py`

 * *Files identical despite different names*

### Comparing `finfactory-0.1.24/finfactory/get_data/sw_daily_info.py` & `finfactory-0.1.25/finfactory/get_data/sw_daily_info.py`

 * *Files identical despite different names*

### Comparing `finfactory-0.1.24/finfactory/get_data/sw_daily_info_old.py` & `finfactory-0.1.25/finfactory/get_data/sw_daily_info_old.py`

 * *Files identical despite different names*

### Comparing `finfactory-0.1.24/finfactory/get_data/tushare_astocks_list.py` & `finfactory-0.1.25/finfactory/get_data/tushare_astocks_list.py`

 * *Files identical despite different names*

### Comparing `finfactory-0.1.24/finfactory/get_data/tushare_block_trades.py` & `finfactory-0.1.25/finfactory/get_data/tushare_block_trades.py`

 * *Files identical despite different names*

### Comparing `finfactory-0.1.24/finfactory/get_data/tushare_cctv_news.py` & `finfactory-0.1.25/finfactory/get_data/tushare_cctv_news.py`

 * *Files identical despite different names*

### Comparing `finfactory-0.1.24/finfactory/get_data/tushare_chn_cpi.py` & `finfactory-0.1.25/finfactory/get_data/tushare_chn_cpi.py`

 * *Files identical despite different names*

### Comparing `finfactory-0.1.24/finfactory/get_data/tushare_chn_gdp.py` & `finfactory-0.1.25/finfactory/get_data/tushare_chn_gdp.py`

 * *Files identical despite different names*

### Comparing `finfactory-0.1.24/finfactory/get_data/tushare_chn_money.py` & `finfactory-0.1.25/finfactory/get_data/tushare_chn_money.py`

 * *Files identical despite different names*

### Comparing `finfactory-0.1.24/finfactory/get_data/tushare_chn_ppi.py` & `finfactory-0.1.25/finfactory/get_data/tushare_chn_ppi.py`

 * *Files identical despite different names*

### Comparing `finfactory-0.1.24/finfactory/get_data/tushare_fund_adj.py` & `finfactory-0.1.25/finfactory/get_data/tushare_fund_adj.py`

 * *Files identical despite different names*

### Comparing `finfactory-0.1.24/finfactory/get_data/tushare_fund_daily.py` & `finfactory-0.1.25/finfactory/get_data/tushare_fund_daily.py`

 * *Files identical despite different names*

### Comparing `finfactory-0.1.24/finfactory/get_data/tushare_fund_fq.py` & `finfactory-0.1.25/finfactory/get_data/tushare_fund_fq.py`

 * *Files identical despite different names*

### Comparing `finfactory-0.1.24/finfactory/get_data/tushare_fund_list.py` & `finfactory-0.1.25/finfactory/get_data/tushare_fund_list.py`

 * *Files identical despite different names*

### Comparing `finfactory-0.1.24/finfactory/get_data/tushare_futures_daily.py` & `finfactory-0.1.25/finfactory/get_data/tushare_futures_daily.py`

 * *Files identical despite different names*

### Comparing `finfactory-0.1.24/finfactory/get_data/tushare_futures_daily_ex.py` & `finfactory-0.1.25/finfactory/get_data/tushare_futures_daily_ex.py`

 * *Files identical despite different names*

### Comparing `finfactory-0.1.24/finfactory/get_data/tushare_futures_info.py` & `finfactory-0.1.25/finfactory/get_data/tushare_futures_info.py`

 * *Files identical despite different names*

### Comparing `finfactory-0.1.24/finfactory/get_data/tushare_futures_mapping.py` & `finfactory-0.1.25/finfactory/get_data/tushare_futures_mapping.py`

 * *Files identical despite different names*

### Comparing `finfactory-0.1.24/finfactory/get_data/tushare_index_daily.py` & `finfactory-0.1.25/finfactory/get_data/tushare_index_daily.py`

 * *Files identical despite different names*

### Comparing `finfactory-0.1.24/finfactory/get_data/tushare_index_daily_basic.py` & `finfactory-0.1.25/finfactory/get_data/tushare_index_daily_basic.py`

 * *Files identical despite different names*

### Comparing `finfactory-0.1.24/finfactory/get_data/tushare_index_info.py` & `finfactory-0.1.25/finfactory/get_data/tushare_index_info.py`

 * *Files identical despite different names*

### Comparing `finfactory-0.1.24/finfactory/get_data/tushare_lpr.py` & `finfactory-0.1.25/finfactory/get_data/tushare_lpr.py`

 * *Files identical despite different names*

### Comparing `finfactory-0.1.24/finfactory/get_data/tushare_options_daily.py` & `finfactory-0.1.25/finfactory/get_data/tushare_options_daily.py`

 * *Files identical despite different names*

### Comparing `finfactory-0.1.24/finfactory/get_data/tushare_options_info.py` & `finfactory-0.1.25/finfactory/get_data/tushare_options_info.py`

 * *Files identical despite different names*

### Comparing `finfactory-0.1.24/finfactory/get_data/tushare_rzrq_daily.py` & `finfactory-0.1.25/finfactory/get_data/tushare_rzrq_daily.py`

 * *Files identical despite different names*

### Comparing `finfactory-0.1.24/finfactory/get_data/tushare_shibor.py` & `finfactory-0.1.25/finfactory/get_data/tushare_shibor.py`

 * *Files identical despite different names*

### Comparing `finfactory-0.1.24/finfactory/get_data/tushare_stock_daily.py` & `finfactory-0.1.25/finfactory/get_data/tushare_stock_daily.py`

 * *Files identical despite different names*

### Comparing `finfactory-0.1.24/finfactory/get_data/tushare_stock_daily_basic.py` & `finfactory-0.1.25/finfactory/get_data/tushare_stock_daily_basic.py`

 * *Files identical despite different names*

### Comparing `finfactory-0.1.24/finfactory/get_data/tushare_stock_daily_stk.py` & `finfactory-0.1.25/finfactory/get_data/tushare_stock_daily_stk.py`

 * *Files identical despite different names*

### Comparing `finfactory-0.1.24/finfactory/get_data/tushare_stock_top10holders.py` & `finfactory-0.1.25/finfactory/get_data/tushare_stock_top10holders.py`

 * *Files identical despite different names*

### Comparing `finfactory-0.1.24/finfactory/get_data/tushare_stock_top10holders_free.py` & `finfactory-0.1.25/finfactory/get_data/tushare_stock_top10holders_free.py`

 * *Files identical despite different names*

### Comparing `finfactory-0.1.24/finfactory/get_data/tushare_stock_zjc.py` & `finfactory-0.1.25/finfactory/get_data/tushare_stock_zjc.py`

 * *Files identical despite different names*

### Comparing `finfactory-0.1.24/finfactory/get_data/tushare_stocks_daily.py` & `finfactory-0.1.25/finfactory/get_data/tushare_stocks_daily.py`

 * *Files identical despite different names*

### Comparing `finfactory-0.1.24/finfactory/get_data/tushare_stocks_daily_basic.py` & `finfactory-0.1.25/finfactory/get_data/tushare_stocks_daily_basic.py`

 * *Files identical despite different names*

### Comparing `finfactory-0.1.24/finfactory/get_data/tushare_stocks_daily_stk.py` & `finfactory-0.1.25/finfactory/get_data/tushare_stocks_daily_stk.py`

 * *Files identical despite different names*

### Comparing `finfactory-0.1.24/finfactory/get_data/tushare_trade_dates.py` & `finfactory-0.1.25/finfactory/get_data/tushare_trade_dates.py`

 * *Files identical despite different names*

### Comparing `finfactory-0.1.24/finfactory/get_data/tushare_usa_bond_rates.py` & `finfactory-0.1.25/finfactory/get_data/tushare_usa_bond_rates.py`

 * *Files identical despite different names*

### Comparing `finfactory-0.1.24/finfactory/get_data/tushare_usa_bond_rates_act.py` & `finfactory-0.1.25/finfactory/get_data/tushare_usa_bond_rates_act.py`

 * *Files identical despite different names*

### Comparing `finfactory-0.1.24/finfactory/install_check.py` & `finfactory-0.1.25/finfactory/install_check.py`

 * *Files identical despite different names*

### Comparing `finfactory-0.1.24/finfactory/load_his_data.py` & `finfactory-0.1.25/finfactory/load_his_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 
 import os
 import numpy as np
 import pandas as pd
 from pathlib import Path
 from dramkit import isnull, load_csv, logger_show
-from dramkit.iotools import make_dir,load_csvs
+from dramkit.iotools import make_dir, load_csvs
 from dramkit.gentools import merge_df
 from dramkit.datetimetools import date_reformat
 from dramkit.other.othertools import load_text_multi
 from finfactory.fintools.utils_chn import get_code_ext
 from finfactory.utils.utils import check_date_loss
 
 #%%
@@ -67,15 +67,19 @@
             raise ValueError('未找到文件夹`{}{}`路径，请检查！'.format(
                              root_dir, dir_name))
     else:
         return dir_path
     
     
 def find_paths_year(fpath):
-    '''根据fpath查找与其相关的带年份后缀的所有路径'''
+    '''
+    根据fpath查找与其相关的带年份后缀的所有路径
+    
+    TODO: 后缀补位年份时处理（比如后缀为_nan）
+    '''
     file = os.path.basename(fpath)
     fdir = str(Path(fpath).parent)
     fdir = fdir.replace('\\', '/')
     tmp = os.listdir(fdir)
     files = []
     for x in tmp:
         x_, type_ = os.path.splitext(x)
@@ -147,24 +151,27 @@
     df['time'] = df['time'].apply(lambda x: x.strftime('%Y-%m-%d'))
     df['date'] = df['time']
     df.sort_values('date', ascending=True, inplace=True)
     df.set_index('date', inplace=True)
     return df
 
 
-def load_daily_crypto_usdt(name1, name2, mkt='binance',
+def load_daily_crypto_usdt(name1, name2=None, mkt='binance',
                            root_dir=None, logger=None):
     '''
     读取BTC和ETH对USDT日行情数据
     
     Examples
     --------
     >>> df_eth = load_daily_crypto_usdt('eth', 'eth_usdt')
     >>> df_btc = load_daily_crypto_usdt('btc', 'btc_usdt')
     '''
+    if isnull(name2):
+        name2 = name1 + '_usdt'
+    name1, name2 = name1.lower(), name2.lower()
     assert name1 in ['btc', 'eth'], '`name1`只能是`btc`或`eth`！'
     df0 = load_ccxt_daily(name1, name2, mkt, root_dir)
     df0['data_source'] = 'binance'
     df0['idx'] = range(0, df0.shape[0])
     df1 = load_daily_btc126(name1, root_dir)
     df1['data_source'] = 'btc126'
     df1['idx'] = range(df0.shape[0], df0.shape[0]+df1.shape[0])
@@ -728,14 +735,15 @@
     Examples
     --------
     >>> df = load_future_mindgo('IF9999')
     >>> df = load_future_mindgo('IF9999', '1min')
     '''
     fpath = get_path_future_mindgo(code, freq=freq, root_dir=root_dir)
     df = load_csv(fpath)
+    df.insert(0, 'code', code)
     return df
     
 #%%
 def get_path_options_info_tushare(exchange, root_dir=None):
     fdir = find_target_dir('options/tushare/options_info/',
                            root_dir=root_dir)
     fpath = fdir + exchange + '.csv'
@@ -804,13 +812,18 @@
     '''
     fpath = get_path_fund_daily_tushare(code, fq=fq, root_dir=root_dir)
     df = load_csv(fpath)
     return df
 
 #%%
 if __name__ == '__main__':
-    import time
+    from dramkit import TimeRecoder
+    tr = TimeRecoder()
+    
+    tr.used()
+
+
+
+
+
 
-    strt_tm = time.time()
 
-    #%%
-    print('used time: {}s.'.format(round(time.time()-strt_tm, 6)))
```

### Comparing `finfactory-0.1.24/finfactory/utils/utils.py` & `finfactory-0.1.25/finfactory/utils/utils.py`

 * *Files identical despite different names*

### Comparing `finfactory-0.1.24/finfactory/utils/utils_crypto.py` & `finfactory-0.1.25/finfactory/utils/utils_crypto.py`

 * *Files 0% similar despite different names*

```diff
@@ -133,13 +133,13 @@
     sums = []
     for col in cols_sum:
         df_ = df_new.groupby('time')[col].apply(lambda x: x.sum())
         sums.append(df_)
     df_new = pd.concat([df_open, df_close, df_high, df_low]+sums, axis=1)
     df_new.reset_index(inplace=True)
     df_new.sort_values('time', ascending=True, inplace=True)
-    df_new.dropna(subset=['close'], inplace=True)
+    # df_new.dropna(subset=['close'], inplace=True)
     return df_new
```

### Comparing `finfactory-0.1.24/finfactory.egg-info/PKG-INFO` & `finfactory-0.1.25/finfactory.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: finfactory
-Version: 0.1.24
+Version: 0.1.25
 Summary: FinFactory is a financial toolbox.
 Home-page: https://github.com/Genlovy-Hoo/finfactory/
 Author: Genlovy Hoo, YueYong Hu
 Author-email: genlovhyy@163.com
 License: MIT
 Platform: any
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 ## 欢迎使用FinFactory
 
 FinFactory是一个金融研究工具箱，其目标是使金融研究更便捷和高效。
 
 FfnFactory的主要工具（将）包括：金融数据下载、清洗整理、因子开发及计算、常用金融模型计算工具、量化策略工具。
 
@@ -33,9 +34,7 @@
 
 Pypi
 
 [finfactory](https://pypi.org/project/finfactory/)
 
 感谢使用和支持！
 
-
-
```

### Comparing `finfactory-0.1.24/finfactory.egg-info/SOURCES.txt` & `finfactory-0.1.25/finfactory.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 finfactory/__init__.py
 finfactory/_pkg_info.py
 finfactory/config.py
 finfactory/install_check.py
 finfactory/load_his_data.py
@@ -22,19 +23,19 @@
 finfactory/fintools/cal_sig_gains_bk.py
 finfactory/fintools/copy_line.py
 finfactory/fintools/fintools.py
 finfactory/fintools/fundnet.py
 finfactory/fintools/options.py
 finfactory/fintools/utils_chn.py
 finfactory/fintools/utils_gains.py
-finfactory/fintools/zigzag.py
 finfactory/get_data/__init__.py
 finfactory/get_data/_ccxt.py
 finfactory/get_data/_get_data.py
 finfactory/get_data/_jq_opts_minute_check.py
+finfactory/get_data/_jy_downloader.py
 finfactory/get_data/_split_data.py
 finfactory/get_data/_stocks_cut.py
 finfactory/get_data/_stocks_merge.py
 finfactory/get_data/ccxt_1d.py
 finfactory/get_data/ccxt_minute.py
 finfactory/get_data/cffex_futures_lhb.py
 finfactory/get_data/chn_local_bond_rates.py
```

### Comparing `finfactory-0.1.24/setup.py` & `finfactory-0.1.25/setup.py`

 * *Files identical despite different names*

