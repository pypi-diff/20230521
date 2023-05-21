# Comparing `tmp/dramkit-0.5.41.tar.gz` & `tmp/dramkit-0.5.42.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dramkit-0.5.41.tar", last modified: Mon May 15 11:05:13 2023, max compression
+gzip compressed data, was "dramkit-0.5.42.tar", last modified: Sun May 21 02:55:36 2023, max compression
```

## Comparing `dramkit-0.5.41.tar` & `dramkit-0.5.42.tar`

### file list

```diff
@@ -1,188 +1,188 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 11:05:13.149780 dramkit-0.5.41/
--rw-rw-rw-   0        0        0     1072 2023-02-25 10:45:19.000000 dramkit-0.5.41/LICENSE
--rw-rw-rw-   0        0        0     1095 2023-05-15 11:05:13.148782 dramkit-0.5.41/PKG-INFO
--rw-rw-rw-   0        0        0      795 2022-05-06 14:18:52.000000 dramkit-0.5.41/README.md
-drwxrwxrwx   0        0        0        0 2023-05-15 11:05:12.587781 dramkit-0.5.41/dramkit/
--rw-rw-rw-   0        0        0      999 2023-04-24 03:43:26.000000 dramkit-0.5.41/dramkit/__init__.py
--rw-rw-rw-   0        0        0      662 2023-05-15 11:04:30.000000 dramkit-0.5.41/dramkit/_pkg_info.py
-drwxrwxrwx   0        0        0        0 2023-05-15 11:05:12.760785 dramkit-0.5.41/dramkit/_tmp/
--rw-rw-rw-   0        0        0     6600 2021-12-24 09:25:22.000000 dramkit-0.5.41/dramkit/_tmp/CRR.py
--rw-rw-rw-   0        0        0     1844 2022-08-02 09:50:33.000000 dramkit-0.5.41/dramkit/_tmp/CtrlPreTS.py
--rw-rw-rw-   0        0        0      515 2022-01-09 09:11:34.000000 dramkit-0.5.41/dramkit/_tmp/NPairSum.py
--rw-rw-rw-   0        0        0     3672 2021-12-24 09:25:22.000000 dramkit-0.5.41/dramkit/_tmp/PIDtest.py
--rw-rw-rw-   0        0        0     2316 2021-12-24 09:25:22.000000 dramkit-0.5.41/dramkit/_tmp/PIDtest2.py
--rw-rw-rw-   0        0        0     6152 2021-12-24 09:25:22.000000 dramkit-0.5.41/dramkit/_tmp/VMD.py
--rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.41/dramkit/_tmp/__init__.py
--rw-rw-rw-   0        0        0     2182 2021-12-24 09:25:22.000000 dramkit-0.5.41/dramkit/_tmp/cca_test.py
--rw-rw-rw-   0        0        0     1768 2021-12-24 09:25:22.000000 dramkit-0.5.41/dramkit/_tmp/dtw_test.py
--rw-rw-rw-   0        0        0    10656 2021-12-24 09:25:22.000000 dramkit-0.5.41/dramkit/_tmp/explore.py
--rw-rw-rw-   0        0        0     2857 2021-12-24 09:25:22.000000 dramkit-0.5.41/dramkit/_tmp/gini.py
--rw-rw-rw-   0        0        0      899 2021-12-24 09:25:22.000000 dramkit-0.5.41/dramkit/_tmp/merge_sort.py
--rw-rw-rw-   0        0        0      910 2021-12-24 09:25:22.000000 dramkit-0.5.41/dramkit/_tmp/mouse_move.py
--rw-rw-rw-   0        0        0     1600 2021-12-24 09:25:22.000000 dramkit-0.5.41/dramkit/_tmp/mpc_test1.py
--rw-rw-rw-   0        0        0     7521 2021-12-24 09:25:22.000000 dramkit-0.5.41/dramkit/_tmp/options_Implied_volatility.py
--rw-rw-rw-   0        0        0      501 2021-12-24 09:25:22.000000 dramkit-0.5.41/dramkit/_tmp/pf_test.py
--rw-rw-rw-   0        0        0     4142 2021-12-24 09:25:22.000000 dramkit-0.5.41/dramkit/_tmp/plot_test.py
--rw-rw-rw-   0        0        0     1567 2022-05-06 11:02:39.000000 dramkit-0.5.41/dramkit/_tmp/plot_test2.py
--rw-rw-rw-   0        0        0     2618 2022-07-06 06:24:15.000000 dramkit-0.5.41/dramkit/_tmp/simple_smooth.py
--rw-rw-rw-   0        0        0     1057 2023-03-17 03:20:46.000000 dramkit-0.5.41/dramkit/_tmp/test_async_washs.py
--rw-rw-rw-   0        0        0     1720 2023-04-03 01:16:22.000000 dramkit-0.5.41/dramkit/_tmp/test_await_timeout.py
--rw-rw-rw-   0        0        0      747 2021-12-24 09:25:22.000000 dramkit-0.5.41/dramkit/_tmp/test_backtrader.py
--rw-rw-rw-   0        0        0     1917 2023-02-16 09:04:46.000000 dramkit-0.5.41/dramkit/_tmp/test_chatgpt_v1.py
--rw-rw-rw-   0        0        0      657 2021-12-24 09:25:22.000000 dramkit-0.5.41/dramkit/_tmp/test_code.py
--rw-rw-rw-   0        0        0     3629 2022-04-13 14:32:40.000000 dramkit-0.5.41/dramkit/_tmp/test_find_peaks.py
--rw-rw-rw-   0        0        0      585 2023-01-29 09:46:43.000000 dramkit-0.5.41/dramkit/_tmp/test_get_var_name.py
--rw-rw-rw-   0        0        0     1263 2022-06-22 06:15:28.000000 dramkit-0.5.41/dramkit/_tmp/test_grading.py
--rw-rw-rw-   0        0        0     2193 2021-12-24 09:25:22.000000 dramkit-0.5.41/dramkit/_tmp/test_lr.py
--rw-rw-rw-   0        0        0     1154 2023-01-13 09:20:58.000000 dramkit-0.5.41/dramkit/_tmp/test_maxsort.py
--rw-rw-rw-   0        0        0      466 2023-04-06 07:48:43.000000 dramkit-0.5.41/dramkit/_tmp/test_multiprocessing.py
--rw-rw-rw-   0        0        0      318 2022-01-26 13:43:15.000000 dramkit-0.5.41/dramkit/_tmp/test_ocr.py
--rw-rw-rw-   0        0        0     1791 2022-04-22 14:45:04.000000 dramkit-0.5.41/dramkit/_tmp/test_pywechat.py
--rw-rw-rw-   0        0        0     3046 2022-09-12 10:04:35.000000 dramkit-0.5.41/dramkit/_tmp/test_tree.py
--rw-rw-rw-   0        0        0     1154 2023-03-08 08:28:22.000000 dramkit-0.5.41/dramkit/_tmp/test_tree2.py
--rw-rw-rw-   0        0        0     1590 2022-09-06 13:36:18.000000 dramkit-0.5.41/dramkit/_tmp/test_wechat_work.py
--rw-rw-rw-   0        0        0     4876 2021-12-24 09:25:22.000000 dramkit-0.5.41/dramkit/_tmp/tfDNNCls_test.py
--rw-rw-rw-   0        0        0     2832 2021-12-24 09:25:22.000000 dramkit-0.5.41/dramkit/_tmp/tmp.py
--rw-rw-rw-   0        0        0     1323 2023-03-28 09:21:10.000000 dramkit-0.5.41/dramkit/_tmp/tmp_args.py
--rw-rw-rw-   0        0        0     5409 2021-12-24 09:25:22.000000 dramkit-0.5.41/dramkit/_tmp/transformer_pytorch.py
--rw-rw-rw-   0        0        0     4675 2022-07-06 06:13:38.000000 dramkit-0.5.41/dramkit/_tmp/utils_SignalDec.py
--rw-rw-rw-   0        0        0    10430 2022-05-06 10:45:29.000000 dramkit-0.5.41/dramkit/_tmp/utils_TimeSeries.py
--rw-rw-rw-   0        0        0     3190 2022-05-06 10:38:49.000000 dramkit-0.5.41/dramkit/_tmp/utils_lottery.py
--rw-rw-rw-   0        0        0     3295 2021-12-24 09:25:22.000000 dramkit-0.5.41/dramkit/_tmp/utils_rl.py
--rw-rw-rw-   0        0        0     2178 2021-12-24 09:25:22.000000 dramkit-0.5.41/dramkit/_tmp/utils_rl2.py
--rw-rw-rw-   0        0        0     4310 2021-12-24 09:25:22.000000 dramkit-0.5.41/dramkit/_tmp/utils_rl3.py
--rw-rw-rw-   0        0        0     4703 2021-12-24 09:25:22.000000 dramkit-0.5.41/dramkit/_tmp/utils_rl4.py
--rw-rw-rw-   0        0        0    10517 2021-12-24 09:25:22.000000 dramkit-0.5.41/dramkit/_tmp/utils_rl5.py
--rw-rw-rw-   0        0        0    10095 2021-12-24 09:25:22.000000 dramkit-0.5.41/dramkit/_tmp/utils_rl6.py
--rw-rw-rw-   0        0        0     5426 2021-12-24 09:25:22.000000 dramkit-0.5.41/dramkit/_tmp/utils_rl7.py
--rw-rw-rw-   0        0        0     2959 2021-12-24 09:25:22.000000 dramkit-0.5.41/dramkit/_tmp/utils_sem.py
-drwxrwxrwx   0        0        0        0 2023-05-15 11:05:12.771781 dramkit-0.5.41/dramkit/backpacks/
--rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.41/dramkit/backpacks/__init__.py
--rw-rw-rw-   0        0        0     7101 2022-05-01 13:07:37.000000 dramkit-0.5.41/dramkit/backpacks/backpack01_float_dy.py
--rw-rw-rw-   0        0        0     6771 2022-05-01 13:50:22.000000 dramkit-0.5.41/dramkit/backpacks/backpack01_int_dy.py
-drwxrwxrwx   0        0        0        0 2023-05-15 11:05:12.819779 dramkit-0.5.41/dramkit/chncal/
--rw-rw-rw-   0        0        0      730 2023-05-12 02:03:24.000000 dramkit-0.5.41/dramkit/chncal/__init__.py
--rw-rw-rw-   0        0        0    21004 2023-05-12 02:03:24.000000 dramkit-0.5.41/dramkit/chncal/apis.py
--rw-rw-rw-   0        0        0    69806 2023-05-12 02:03:24.000000 dramkit-0.5.41/dramkit/chncal/constants.py
--rw-rw-rw-   0        0        0     8480 2023-05-12 02:03:24.000000 dramkit-0.5.41/dramkit/chncal/constants_fate.py
--rw-rw-rw-   0        0        0  9509384 2023-05-12 02:03:24.000000 dramkit-0.5.41/dramkit/chncal/constants_hko.py
--rw-rw-rw-   0        0        0  3958798 2023-05-12 02:03:24.000000 dramkit-0.5.41/dramkit/chncal/constants_trade_dates.py
--rw-rw-rw-   0        0        0     2501 2023-05-12 02:03:24.000000 dramkit-0.5.41/dramkit/chncal/constants_wuxing.py
--rw-rw-rw-   0        0        0     8342 2023-05-12 02:03:24.000000 dramkit-0.5.41/dramkit/chncal/constants_zodiac_marry.py
--rw-rw-rw-   0        0        0     4570 2023-05-12 02:03:24.000000 dramkit-0.5.41/dramkit/chncal/solar_terms.py
--rw-rw-rw-   0        0        0     6723 2023-04-24 06:40:29.000000 dramkit-0.5.41/dramkit/cryptotools.py
--rw-rw-rw-   0        0        0    34313 2023-05-11 01:22:24.000000 dramkit-0.5.41/dramkit/datetimetools.py
-drwxrwxrwx   0        0        0        0 2023-05-15 11:05:12.881781 dramkit-0.5.41/dramkit/datsci/
--rw-rw-rw-   0        0        0       65 2022-05-06 02:08:55.000000 dramkit-0.5.41/dramkit/datsci/__init__.py
--rw-rw-rw-   0        0        0     2865 2023-03-22 07:56:05.000000 dramkit-0.5.41/dramkit/datsci/_utils_ann.py
--rw-rw-rw-   0        0        0     2090 2022-05-05 14:04:35.000000 dramkit-0.5.41/dramkit/datsci/activate_funcs.py
--rw-rw-rw-   0        0        0    19078 2023-03-22 07:56:56.000000 dramkit-0.5.41/dramkit/datsci/ahp.py
--rw-rw-rw-   0        0        0     2992 2023-03-22 07:58:04.000000 dramkit-0.5.41/dramkit/datsci/ahp_sim_ri.py
--rw-rw-rw-   0        0        0    10071 2022-05-19 06:37:13.000000 dramkit-0.5.41/dramkit/datsci/apriori.py
--rw-rw-rw-   0        0        0     4362 2022-05-06 06:17:24.000000 dramkit-0.5.41/dramkit/datsci/curvature.py
--rw-rw-rw-   0        0        0     6966 2023-03-22 07:59:58.000000 dramkit-0.5.41/dramkit/datsci/elm_cls.py
--rw-rw-rw-   0        0        0     8216 2023-03-22 08:00:46.000000 dramkit-0.5.41/dramkit/datsci/elm_reg.py
--rw-rw-rw-   0        0        0     3697 2022-06-25 18:21:15.000000 dramkit-0.5.41/dramkit/datsci/entropy_weight.py
--rw-rw-rw-   0        0        0    50084 2023-05-10 02:47:36.000000 dramkit-0.5.41/dramkit/datsci/find_maxmin.py
--rw-rw-rw-   0        0        0     7229 2023-03-22 08:06:26.000000 dramkit-0.5.41/dramkit/datsci/freq_item_set.py
--rw-rw-rw-   0        0        0     6219 2023-03-22 07:59:12.000000 dramkit-0.5.41/dramkit/datsci/lr.py
--rw-rw-rw-   0        0        0    19374 2023-04-25 08:42:22.000000 dramkit-0.5.41/dramkit/datsci/preprocess.py
--rw-rw-rw-   0        0        0    41389 2023-03-23 13:45:46.000000 dramkit-0.5.41/dramkit/datsci/stats.py
--rw-rw-rw-   0        0        0    36092 2023-03-22 08:04:05.000000 dramkit-0.5.41/dramkit/datsci/time_series.py
--rw-rw-rw-   0        0        0     3451 2022-06-25 18:24:48.000000 dramkit-0.5.41/dramkit/datsci/topsis.py
--rw-rw-rw-   0        0        0    23324 2022-10-17 06:00:47.000000 dramkit-0.5.41/dramkit/datsci/utils_lgb.py
--rw-rw-rw-   0        0        0     6843 2022-09-09 05:44:56.000000 dramkit-0.5.41/dramkit/datsci/utils_ml.py
--rw-rw-rw-   0        0        0    21037 2023-05-11 01:05:22.000000 dramkit-0.5.41/dramkit/datsci/zigzag.py
-drwxrwxrwx   0        0        0        0 2023-05-15 11:05:12.906781 dramkit-0.5.41/dramkit/find_addends/
--rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.41/dramkit/find_addends/__init__.py
--rw-rw-rw-   0        0        0     3433 2023-03-22 08:18:35.000000 dramkit-0.5.41/dramkit/find_addends/find_addends_backpack01float.py
--rw-rw-rw-   0        0        0     2149 2022-05-01 08:15:22.000000 dramkit-0.5.41/dramkit/find_addends/find_addends_backpack01int.py
--rw-rw-rw-   0        0        0    12658 2023-03-22 08:17:39.000000 dramkit-0.5.41/dramkit/find_addends/find_addends_bigfirst.py
--rw-rw-rw-   0        0        0     4500 2023-03-22 08:17:06.000000 dramkit-0.5.41/dramkit/find_addends/find_addends_recu.py
--rw-rw-rw-   0        0        0     9576 2023-03-22 08:16:00.000000 dramkit-0.5.41/dramkit/find_addends/find_addends_smlfirst.py
--rw-rw-rw-   0        0        0     3988 2022-04-30 16:29:18.000000 dramkit-0.5.41/dramkit/find_addends/find_addends_utils.py
--rw-rw-rw-   0        0        0   119309 2023-05-10 06:51:27.000000 dramkit-0.5.41/dramkit/gentools.py
--rw-rw-rw-   0        0        0      735 2022-08-04 06:40:11.000000 dramkit-0.5.41/dramkit/install_check.py
--rw-rw-rw-   0        0        0    67244 2023-05-15 09:46:05.000000 dramkit-0.5.41/dramkit/iotools.py
-drwxrwxrwx   0        0        0        0 2023-05-15 11:05:12.924781 dramkit-0.5.41/dramkit/logtools/
--rw-rw-rw-   0        0        0      139 2023-05-01 07:34:20.000000 dramkit-0.5.41/dramkit/logtools/__init__.py
--rw-rw-rw-   0        0        0     2566 2023-02-08 04:11:46.000000 dramkit-0.5.41/dramkit/logtools/logger_general.py
--rw-rw-rw-   0        0        0     3597 2023-02-07 03:04:57.000000 dramkit-0.5.41/dramkit/logtools/logger_rotating.py
--rw-rw-rw-   0        0        0     2880 2023-02-07 03:04:39.000000 dramkit-0.5.41/dramkit/logtools/logger_timedrotating.py
--rw-rw-rw-   0        0        0     4214 2023-02-28 10:31:30.000000 dramkit-0.5.41/dramkit/logtools/utils_logger.py
-drwxrwxrwx   0        0        0        0 2023-05-15 11:05:12.938780 dramkit-0.5.41/dramkit/openai/
--rw-rw-rw-   0        0        0      203 2023-04-24 02:54:37.000000 dramkit-0.5.41/dramkit/openai/__init__.py
--rw-rw-rw-   0        0        0     5656 2023-04-25 16:34:10.000000 dramkit-0.5.41/dramkit/openai/aiedu_chat.py
--rw-rw-rw-   0        0        0    16999 2023-05-08 02:26:05.000000 dramkit-0.5.41/dramkit/openai/openai_chat.py
--rw-rw-rw-   0        0        0     4461 2023-04-25 02:00:24.000000 dramkit-0.5.41/dramkit/openai/openai_chat_hs.py
-drwxrwxrwx   0        0        0        0 2023-05-15 11:05:12.982781 dramkit-0.5.41/dramkit/optimizer/
--rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.41/dramkit/optimizer/__init__.py
--rw-rw-rw-   0        0        0     9712 2023-03-22 08:26:32.000000 dramkit-0.5.41/dramkit/optimizer/alo.py
--rw-rw-rw-   0        0        0     3141 2022-05-02 02:31:44.000000 dramkit-0.5.41/dramkit/optimizer/base_funcs.py
--rw-rw-rw-   0        0        0     7428 2023-03-22 08:35:00.000000 dramkit-0.5.41/dramkit/optimizer/boa.py
--rw-rw-rw-   0        0        0     8863 2023-03-22 08:34:30.000000 dramkit-0.5.41/dramkit/optimizer/cs.py
--rw-rw-rw-   0        0        0    13415 2023-03-22 08:33:50.000000 dramkit-0.5.41/dramkit/optimizer/ga.py
--rw-rw-rw-   0        0        0     8701 2023-03-22 08:33:17.000000 dramkit-0.5.41/dramkit/optimizer/gwo.py
--rw-rw-rw-   0        0        0     9311 2023-03-22 08:32:10.000000 dramkit-0.5.41/dramkit/optimizer/hcpsoboa.py
--rw-rw-rw-   0        0        0     9929 2023-03-22 08:31:27.000000 dramkit-0.5.41/dramkit/optimizer/hho.py
--rw-rw-rw-   0        0        0     8817 2023-03-22 08:30:38.000000 dramkit-0.5.41/dramkit/optimizer/hpsoboa.py
--rw-rw-rw-   0        0        0     8889 2023-03-22 08:29:43.000000 dramkit-0.5.41/dramkit/optimizer/pso.py
--rw-rw-rw-   0        0        0     5222 2022-05-02 02:18:28.000000 dramkit-0.5.41/dramkit/optimizer/utils_heuristic.py
--rw-rw-rw-   0        0        0     7334 2023-03-22 08:27:35.000000 dramkit-0.5.41/dramkit/optimizer/woa.py
-drwxrwxrwx   0        0        0        0 2023-05-15 11:05:13.011799 dramkit-0.5.41/dramkit/other/
--rw-rw-rw-   0        0        0     3856 2023-04-30 10:22:45.000000 dramkit-0.5.41/dramkit/other/_Linux_notes.py
--rw-rw-rw-   0        0        0     2871 2023-04-19 03:27:58.000000 dramkit-0.5.41/dramkit/other/_Python_notes.py
--rw-rw-rw-   0        0        0     4777 2023-04-24 08:14:04.000000 dramkit-0.5.41/dramkit/other/_Vim_notes.py
--rw-rw-rw-   0        0        0      164 2022-08-25 01:46:27.000000 dramkit-0.5.41/dramkit/other/__init__.py
--rw-rw-rw-   0        0        0     7988 2022-10-27 06:38:44.000000 dramkit-0.5.41/dramkit/other/langconv.py
--rw-rw-rw-   0        0        0     8353 2022-12-10 15:26:10.000000 dramkit-0.5.41/dramkit/other/othertools.py
--rw-rw-rw-   0        0        0     1804 2023-03-22 08:36:51.000000 dramkit-0.5.41/dramkit/other/replace_endblank.py
--rw-rw-rw-   0        0        0   143066 2022-08-25 01:37:20.000000 dramkit-0.5.41/dramkit/other/zh_wiki.py
-drwxrwxrwx   0        0        0        0 2023-05-15 11:05:13.035776 dramkit-0.5.41/dramkit/plottools/
--rw-rw-rw-   0        0        0      112 2022-05-04 14:50:04.000000 dramkit-0.5.41/dramkit/plottools/__init__.py
--rw-rw-rw-   0        0        0     4400 2022-01-09 07:36:22.000000 dramkit-0.5.41/dramkit/plottools/plot_barline.py
--rw-rw-rw-   0        0        0    48559 2023-04-22 13:09:27.000000 dramkit-0.5.41/dramkit/plottools/plot_common.py
--rw-rw-rw-   0        0        0     9033 2022-06-25 18:36:48.000000 dramkit-0.5.41/dramkit/plottools/plot_histdist.py
--rw-rw-rw-   0        0        0     2145 2023-03-04 13:10:35.000000 dramkit-0.5.41/dramkit/plottools/plot_scatter.py
--rw-rw-rw-   0        0        0     5120 2023-03-21 14:27:12.000000 dramkit-0.5.41/dramkit/plottools/utils_plot.py
-drwxrwxrwx   0        0        0        0 2023-05-15 11:05:13.045776 dramkit-0.5.41/dramkit/pystyles/
--rw-rw-rw-   0        0        0       25 2021-12-25 16:04:07.000000 dramkit-0.5.41/dramkit/pystyles/__init__.py
--rw-rw-rw-   0        0        0     8021 2022-04-30 13:24:37.000000 dramkit-0.5.41/dramkit/pystyles/dramkit_style.py
-drwxrwxrwx   0        0        0        0 2023-05-15 11:05:13.068781 dramkit-0.5.41/dramkit/sorts/
--rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.41/dramkit/sorts/__init__.py
--rw-rw-rw-   0        0        0     1302 2022-01-09 08:45:28.000000 dramkit-0.5.41/dramkit/sorts/bubble_sort.py
--rw-rw-rw-   0        0        0     1426 2022-01-09 08:51:55.000000 dramkit-0.5.41/dramkit/sorts/bucket_sort.py
--rw-rw-rw-   0        0        0     4742 2022-01-09 08:10:56.000000 dramkit-0.5.41/dramkit/sorts/insert_sort.py
--rw-rw-rw-   0        0        0     4833 2022-01-09 09:23:30.000000 dramkit-0.5.41/dramkit/sorts/insert_sort_bin.py
--rw-rw-rw-   0        0        0     1339 2022-01-09 08:55:14.000000 dramkit-0.5.41/dramkit/sorts/quick_sort.py
-drwxrwxrwx   0        0        0        0 2023-05-15 11:05:13.090781 dramkit-0.5.41/dramkit/speedup/
--rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.41/dramkit/speedup/__init__.py
--rw-rw-rw-   0        0        0     1231 2023-04-14 13:02:46.000000 dramkit-0.5.41/dramkit/speedup/_mp_test1.py
--rw-rw-rw-   0        0        0      886 2023-04-14 13:17:44.000000 dramkit-0.5.41/dramkit/speedup/_mp_test2.py
--rw-rw-rw-   0        0        0      684 2023-04-14 13:14:44.000000 dramkit-0.5.41/dramkit/speedup/_mp_test3.py
--rw-rw-rw-   0        0        0     3384 2023-04-14 13:25:51.000000 dramkit-0.5.41/dramkit/speedup/iotools_tmp.py
--rw-rw-rw-   0        0        0     3754 2023-04-12 08:17:22.000000 dramkit-0.5.41/dramkit/speedup/multi_process_concurrent.py
--rw-rw-rw-   0        0        0     7888 2023-04-07 08:59:34.000000 dramkit-0.5.41/dramkit/speedup/multi_thread.py
-drwxrwxrwx   0        0        0        0 2023-05-15 11:05:13.121780 dramkit-0.5.41/dramkit/sqltools/
--rw-rw-rw-   0        0        0     2495 2023-02-23 05:15:08.000000 dramkit-0.5.41/dramkit/sqltools/_Hive_notes.py
--rw-rw-rw-   0        0        0    30416 2023-04-11 01:33:28.000000 dramkit-0.5.41/dramkit/sqltools/_MySQL_notes.py
--rw-rw-rw-   0        0        0     6849 2023-03-07 09:26:53.000000 dramkit-0.5.41/dramkit/sqltools/_Oracle_notes.py
--rw-rw-rw-   0        0        0      160 2023-05-01 12:57:19.000000 dramkit-0.5.41/dramkit/sqltools/__init__.py
--rw-rw-rw-   0        0        0    20285 2023-05-06 13:49:07.000000 dramkit-0.5.41/dramkit/sqltools/cxoracle.py
--rw-rw-rw-   0        0        0    25908 2023-02-24 11:31:13.000000 dramkit-0.5.41/dramkit/sqltools/py_hive.py
--rw-rw-rw-   0        0        0    50966 2023-05-06 13:23:21.000000 dramkit-0.5.41/dramkit/sqltools/py_mysql.py
--rw-rw-rw-   0        0        0    18391 2023-03-22 02:56:24.000000 dramkit-0.5.41/dramkit/sqltools/sql_alchemy.py
-drwxrwxrwx   0        0        0        0 2023-05-15 11:05:13.131781 dramkit-0.5.41/dramkit/webtools/
--rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.41/dramkit/webtools/__init__.py
--rw-rw-rw-   0        0        0     5337 2022-06-25 18:37:55.000000 dramkit-0.5.41/dramkit/webtools/utils_html.py
-drwxrwxrwx   0        0        0        0 2023-05-15 11:05:13.145778 dramkit-0.5.41/dramkit/wechat/
--rw-rw-rw-   0        0        0       58 2022-09-06 14:04:57.000000 dramkit-0.5.41/dramkit/wechat/__init__.py
--rw-rw-rw-   0        0        0     7473 2022-10-28 03:03:37.000000 dramkit-0.5.41/dramkit/wechat/qywechat.py
-drwxrwxrwx   0        0        0        0 2023-05-15 11:05:12.603779 dramkit-0.5.41/dramkit.egg-info/
--rw-rw-rw-   0        0        0     1095 2023-05-15 11:05:08.000000 dramkit-0.5.41/dramkit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4877 2023-05-15 11:05:11.000000 dramkit-0.5.41/dramkit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 11:05:08.000000 dramkit-0.5.41/dramkit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       66 2023-05-15 11:05:08.000000 dramkit-0.5.41/dramkit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-15 11:05:08.000000 dramkit-0.5.41/dramkit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-15 11:05:13.149780 dramkit-0.5.41/setup.cfg
--rw-rw-rw-   0        0        0     1944 2023-05-01 12:58:33.000000 dramkit-0.5.41/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-21 02:55:36.663125 dramkit-0.5.42/
+-rw-rw-rw-   0        0        0     1072 2023-02-25 10:45:19.000000 dramkit-0.5.42/LICENSE
+-rw-rw-rw-   0        0        0     1095 2023-05-21 02:55:36.663125 dramkit-0.5.42/PKG-INFO
+-rw-rw-rw-   0        0        0      795 2022-05-06 14:18:52.000000 dramkit-0.5.42/README.md
+drwxrwxrwx   0        0        0        0 2023-05-21 02:55:36.505541 dramkit-0.5.42/dramkit/
+-rw-rw-rw-   0        0        0      999 2023-04-24 03:43:26.000000 dramkit-0.5.42/dramkit/__init__.py
+-rw-rw-rw-   0        0        0      662 2023-05-16 01:56:43.000000 dramkit-0.5.42/dramkit/_pkg_info.py
+drwxrwxrwx   0        0        0        0 2023-05-21 02:55:36.552417 dramkit-0.5.42/dramkit/_tmp/
+-rw-rw-rw-   0        0        0     6600 2021-12-24 09:25:22.000000 dramkit-0.5.42/dramkit/_tmp/CRR.py
+-rw-rw-rw-   0        0        0     1844 2022-08-02 09:50:33.000000 dramkit-0.5.42/dramkit/_tmp/CtrlPreTS.py
+-rw-rw-rw-   0        0        0      515 2022-01-09 09:11:34.000000 dramkit-0.5.42/dramkit/_tmp/NPairSum.py
+-rw-rw-rw-   0        0        0     3672 2021-12-24 09:25:22.000000 dramkit-0.5.42/dramkit/_tmp/PIDtest.py
+-rw-rw-rw-   0        0        0     2316 2021-12-24 09:25:22.000000 dramkit-0.5.42/dramkit/_tmp/PIDtest2.py
+-rw-rw-rw-   0        0        0     6152 2021-12-24 09:25:22.000000 dramkit-0.5.42/dramkit/_tmp/VMD.py
+-rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.42/dramkit/_tmp/__init__.py
+-rw-rw-rw-   0        0        0     2182 2021-12-24 09:25:22.000000 dramkit-0.5.42/dramkit/_tmp/cca_test.py
+-rw-rw-rw-   0        0        0     1768 2021-12-24 09:25:22.000000 dramkit-0.5.42/dramkit/_tmp/dtw_test.py
+-rw-rw-rw-   0        0        0    10656 2021-12-24 09:25:22.000000 dramkit-0.5.42/dramkit/_tmp/explore.py
+-rw-rw-rw-   0        0        0     2857 2021-12-24 09:25:22.000000 dramkit-0.5.42/dramkit/_tmp/gini.py
+-rw-rw-rw-   0        0        0      899 2021-12-24 09:25:22.000000 dramkit-0.5.42/dramkit/_tmp/merge_sort.py
+-rw-rw-rw-   0        0        0      910 2021-12-24 09:25:22.000000 dramkit-0.5.42/dramkit/_tmp/mouse_move.py
+-rw-rw-rw-   0        0        0     1600 2021-12-24 09:25:22.000000 dramkit-0.5.42/dramkit/_tmp/mpc_test1.py
+-rw-rw-rw-   0        0        0     7521 2021-12-24 09:25:22.000000 dramkit-0.5.42/dramkit/_tmp/options_Implied_volatility.py
+-rw-rw-rw-   0        0        0      501 2021-12-24 09:25:22.000000 dramkit-0.5.42/dramkit/_tmp/pf_test.py
+-rw-rw-rw-   0        0        0     4142 2021-12-24 09:25:22.000000 dramkit-0.5.42/dramkit/_tmp/plot_test.py
+-rw-rw-rw-   0        0        0     1567 2022-05-06 11:02:39.000000 dramkit-0.5.42/dramkit/_tmp/plot_test2.py
+-rw-rw-rw-   0        0        0     2618 2022-07-06 06:24:15.000000 dramkit-0.5.42/dramkit/_tmp/simple_smooth.py
+-rw-rw-rw-   0        0        0     1057 2023-03-17 03:20:46.000000 dramkit-0.5.42/dramkit/_tmp/test_async_washs.py
+-rw-rw-rw-   0        0        0     1720 2023-04-03 01:16:22.000000 dramkit-0.5.42/dramkit/_tmp/test_await_timeout.py
+-rw-rw-rw-   0        0        0      747 2021-12-24 09:25:22.000000 dramkit-0.5.42/dramkit/_tmp/test_backtrader.py
+-rw-rw-rw-   0        0        0     1917 2023-02-16 09:04:46.000000 dramkit-0.5.42/dramkit/_tmp/test_chatgpt_v1.py
+-rw-rw-rw-   0        0        0      657 2021-12-24 09:25:22.000000 dramkit-0.5.42/dramkit/_tmp/test_code.py
+-rw-rw-rw-   0        0        0     3629 2022-04-13 14:32:40.000000 dramkit-0.5.42/dramkit/_tmp/test_find_peaks.py
+-rw-rw-rw-   0        0        0      585 2023-01-29 09:46:43.000000 dramkit-0.5.42/dramkit/_tmp/test_get_var_name.py
+-rw-rw-rw-   0        0        0     1263 2022-06-22 06:15:28.000000 dramkit-0.5.42/dramkit/_tmp/test_grading.py
+-rw-rw-rw-   0        0        0     2193 2021-12-24 09:25:22.000000 dramkit-0.5.42/dramkit/_tmp/test_lr.py
+-rw-rw-rw-   0        0        0     1154 2023-01-13 09:20:58.000000 dramkit-0.5.42/dramkit/_tmp/test_maxsort.py
+-rw-rw-rw-   0        0        0      466 2023-04-06 07:48:43.000000 dramkit-0.5.42/dramkit/_tmp/test_multiprocessing.py
+-rw-rw-rw-   0        0        0      318 2022-01-26 13:43:15.000000 dramkit-0.5.42/dramkit/_tmp/test_ocr.py
+-rw-rw-rw-   0        0        0     1791 2022-04-22 14:45:04.000000 dramkit-0.5.42/dramkit/_tmp/test_pywechat.py
+-rw-rw-rw-   0        0        0     3046 2022-09-12 10:04:35.000000 dramkit-0.5.42/dramkit/_tmp/test_tree.py
+-rw-rw-rw-   0        0        0     1154 2023-03-08 08:28:22.000000 dramkit-0.5.42/dramkit/_tmp/test_tree2.py
+-rw-rw-rw-   0        0        0     1590 2022-09-06 13:36:18.000000 dramkit-0.5.42/dramkit/_tmp/test_wechat_work.py
+-rw-rw-rw-   0        0        0     4876 2021-12-24 09:25:22.000000 dramkit-0.5.42/dramkit/_tmp/tfDNNCls_test.py
+-rw-rw-rw-   0        0        0     2832 2021-12-24 09:25:22.000000 dramkit-0.5.42/dramkit/_tmp/tmp.py
+-rw-rw-rw-   0        0        0     1323 2023-03-28 09:21:10.000000 dramkit-0.5.42/dramkit/_tmp/tmp_args.py
+-rw-rw-rw-   0        0        0     5409 2021-12-24 09:25:22.000000 dramkit-0.5.42/dramkit/_tmp/transformer_pytorch.py
+-rw-rw-rw-   0        0        0     4675 2022-07-06 06:13:38.000000 dramkit-0.5.42/dramkit/_tmp/utils_SignalDec.py
+-rw-rw-rw-   0        0        0    10430 2022-05-06 10:45:29.000000 dramkit-0.5.42/dramkit/_tmp/utils_TimeSeries.py
+-rw-rw-rw-   0        0        0     3190 2022-05-06 10:38:49.000000 dramkit-0.5.42/dramkit/_tmp/utils_lottery.py
+-rw-rw-rw-   0        0        0     3295 2021-12-24 09:25:22.000000 dramkit-0.5.42/dramkit/_tmp/utils_rl.py
+-rw-rw-rw-   0        0        0     2178 2021-12-24 09:25:22.000000 dramkit-0.5.42/dramkit/_tmp/utils_rl2.py
+-rw-rw-rw-   0        0        0     4310 2021-12-24 09:25:22.000000 dramkit-0.5.42/dramkit/_tmp/utils_rl3.py
+-rw-rw-rw-   0        0        0     4703 2021-12-24 09:25:22.000000 dramkit-0.5.42/dramkit/_tmp/utils_rl4.py
+-rw-rw-rw-   0        0        0    10517 2021-12-24 09:25:22.000000 dramkit-0.5.42/dramkit/_tmp/utils_rl5.py
+-rw-rw-rw-   0        0        0    10095 2021-12-24 09:25:22.000000 dramkit-0.5.42/dramkit/_tmp/utils_rl6.py
+-rw-rw-rw-   0        0        0     5426 2021-12-24 09:25:22.000000 dramkit-0.5.42/dramkit/_tmp/utils_rl7.py
+-rw-rw-rw-   0        0        0     2959 2021-12-24 09:25:22.000000 dramkit-0.5.42/dramkit/_tmp/utils_sem.py
+drwxrwxrwx   0        0        0        0 2023-05-21 02:55:36.555408 dramkit-0.5.42/dramkit/backpacks/
+-rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.42/dramkit/backpacks/__init__.py
+-rw-rw-rw-   0        0        0     7101 2022-05-01 13:07:37.000000 dramkit-0.5.42/dramkit/backpacks/backpack01_float_dy.py
+-rw-rw-rw-   0        0        0     6771 2022-05-01 13:50:22.000000 dramkit-0.5.42/dramkit/backpacks/backpack01_int_dy.py
+drwxrwxrwx   0        0        0        0 2023-05-21 02:55:36.581339 dramkit-0.5.42/dramkit/chncal/
+-rw-rw-rw-   0        0        0      730 2023-05-19 13:42:53.000000 dramkit-0.5.42/dramkit/chncal/__init__.py
+-rw-rw-rw-   0        0        0    21188 2023-05-19 13:42:53.000000 dramkit-0.5.42/dramkit/chncal/apis.py
+-rw-rw-rw-   0        0        0    69806 2023-05-19 13:42:53.000000 dramkit-0.5.42/dramkit/chncal/constants.py
+-rw-rw-rw-   0        0        0     8480 2023-05-19 13:42:53.000000 dramkit-0.5.42/dramkit/chncal/constants_fate.py
+-rw-rw-rw-   0        0        0  9509384 2023-05-19 13:42:53.000000 dramkit-0.5.42/dramkit/chncal/constants_hko.py
+-rw-rw-rw-   0        0        0  3961724 2023-05-19 13:42:53.000000 dramkit-0.5.42/dramkit/chncal/constants_trade_dates.py
+-rw-rw-rw-   0        0        0     2501 2023-05-19 13:42:53.000000 dramkit-0.5.42/dramkit/chncal/constants_wuxing.py
+-rw-rw-rw-   0        0        0     8342 2023-05-19 13:42:53.000000 dramkit-0.5.42/dramkit/chncal/constants_zodiac_marry.py
+-rw-rw-rw-   0        0        0     4570 2023-05-19 13:42:53.000000 dramkit-0.5.42/dramkit/chncal/solar_terms.py
+-rw-rw-rw-   0        0        0     6723 2023-04-24 06:40:29.000000 dramkit-0.5.42/dramkit/cryptotools.py
+-rw-rw-rw-   0        0        0    34826 2023-05-20 15:37:28.000000 dramkit-0.5.42/dramkit/datetimetools.py
+drwxrwxrwx   0        0        0        0 2023-05-21 02:55:36.601290 dramkit-0.5.42/dramkit/datsci/
+-rw-rw-rw-   0        0        0       65 2022-05-06 02:08:55.000000 dramkit-0.5.42/dramkit/datsci/__init__.py
+-rw-rw-rw-   0        0        0     2865 2023-03-22 07:56:05.000000 dramkit-0.5.42/dramkit/datsci/_utils_ann.py
+-rw-rw-rw-   0        0        0     2090 2022-05-05 14:04:35.000000 dramkit-0.5.42/dramkit/datsci/activate_funcs.py
+-rw-rw-rw-   0        0        0    19078 2023-03-22 07:56:56.000000 dramkit-0.5.42/dramkit/datsci/ahp.py
+-rw-rw-rw-   0        0        0     2992 2023-03-22 07:58:04.000000 dramkit-0.5.42/dramkit/datsci/ahp_sim_ri.py
+-rw-rw-rw-   0        0        0    10071 2022-05-19 06:37:13.000000 dramkit-0.5.42/dramkit/datsci/apriori.py
+-rw-rw-rw-   0        0        0     4362 2022-05-06 06:17:24.000000 dramkit-0.5.42/dramkit/datsci/curvature.py
+-rw-rw-rw-   0        0        0     6966 2023-03-22 07:59:58.000000 dramkit-0.5.42/dramkit/datsci/elm_cls.py
+-rw-rw-rw-   0        0        0     8216 2023-03-22 08:00:46.000000 dramkit-0.5.42/dramkit/datsci/elm_reg.py
+-rw-rw-rw-   0        0        0     3697 2022-06-25 18:21:15.000000 dramkit-0.5.42/dramkit/datsci/entropy_weight.py
+-rw-rw-rw-   0        0        0    50084 2023-05-10 02:47:36.000000 dramkit-0.5.42/dramkit/datsci/find_maxmin.py
+-rw-rw-rw-   0        0        0     7229 2023-03-22 08:06:26.000000 dramkit-0.5.42/dramkit/datsci/freq_item_set.py
+-rw-rw-rw-   0        0        0     6219 2023-03-22 07:59:12.000000 dramkit-0.5.42/dramkit/datsci/lr.py
+-rw-rw-rw-   0        0        0    20288 2023-05-19 06:29:01.000000 dramkit-0.5.42/dramkit/datsci/preprocess.py
+-rw-rw-rw-   0        0        0    41389 2023-03-23 13:45:46.000000 dramkit-0.5.42/dramkit/datsci/stats.py
+-rw-rw-rw-   0        0        0    36092 2023-03-22 08:04:05.000000 dramkit-0.5.42/dramkit/datsci/time_series.py
+-rw-rw-rw-   0        0        0     3451 2022-06-25 18:24:48.000000 dramkit-0.5.42/dramkit/datsci/topsis.py
+-rw-rw-rw-   0        0        0    23324 2022-10-17 06:00:47.000000 dramkit-0.5.42/dramkit/datsci/utils_lgb.py
+-rw-rw-rw-   0        0        0     6843 2022-09-09 05:44:56.000000 dramkit-0.5.42/dramkit/datsci/utils_ml.py
+-rw-rw-rw-   0        0        0    21037 2023-05-11 01:05:22.000000 dramkit-0.5.42/dramkit/datsci/zigzag.py
+drwxrwxrwx   0        0        0        0 2023-05-21 02:55:36.609269 dramkit-0.5.42/dramkit/find_addends/
+-rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.42/dramkit/find_addends/__init__.py
+-rw-rw-rw-   0        0        0     3433 2023-03-22 08:18:35.000000 dramkit-0.5.42/dramkit/find_addends/find_addends_backpack01float.py
+-rw-rw-rw-   0        0        0     2149 2022-05-01 08:15:22.000000 dramkit-0.5.42/dramkit/find_addends/find_addends_backpack01int.py
+-rw-rw-rw-   0        0        0    12658 2023-03-22 08:17:39.000000 dramkit-0.5.42/dramkit/find_addends/find_addends_bigfirst.py
+-rw-rw-rw-   0        0        0     4500 2023-03-22 08:17:06.000000 dramkit-0.5.42/dramkit/find_addends/find_addends_recu.py
+-rw-rw-rw-   0        0        0     9576 2023-03-22 08:16:00.000000 dramkit-0.5.42/dramkit/find_addends/find_addends_smlfirst.py
+-rw-rw-rw-   0        0        0     3988 2022-04-30 16:29:18.000000 dramkit-0.5.42/dramkit/find_addends/find_addends_utils.py
+-rw-rw-rw-   0        0        0   125549 2023-05-20 16:49:14.000000 dramkit-0.5.42/dramkit/gentools.py
+-rw-rw-rw-   0        0        0      735 2022-08-04 06:40:11.000000 dramkit-0.5.42/dramkit/install_check.py
+-rw-rw-rw-   0        0        0    67350 2023-05-19 01:46:24.000000 dramkit-0.5.42/dramkit/iotools.py
+drwxrwxrwx   0        0        0        0 2023-05-21 02:55:36.612261 dramkit-0.5.42/dramkit/logtools/
+-rw-rw-rw-   0        0        0      139 2023-05-01 07:34:20.000000 dramkit-0.5.42/dramkit/logtools/__init__.py
+-rw-rw-rw-   0        0        0     2566 2023-02-08 04:11:46.000000 dramkit-0.5.42/dramkit/logtools/logger_general.py
+-rw-rw-rw-   0        0        0     3597 2023-02-07 03:04:57.000000 dramkit-0.5.42/dramkit/logtools/logger_rotating.py
+-rw-rw-rw-   0        0        0     2880 2023-02-07 03:04:39.000000 dramkit-0.5.42/dramkit/logtools/logger_timedrotating.py
+-rw-rw-rw-   0        0        0     4214 2023-02-28 10:31:30.000000 dramkit-0.5.42/dramkit/logtools/utils_logger.py
+drwxrwxrwx   0        0        0        0 2023-05-21 02:55:36.615253 dramkit-0.5.42/dramkit/openai/
+-rw-rw-rw-   0        0        0      203 2023-04-24 02:54:37.000000 dramkit-0.5.42/dramkit/openai/__init__.py
+-rw-rw-rw-   0        0        0     5656 2023-04-25 16:34:10.000000 dramkit-0.5.42/dramkit/openai/aiedu_chat.py
+-rw-rw-rw-   0        0        0    16999 2023-05-08 02:26:05.000000 dramkit-0.5.42/dramkit/openai/openai_chat.py
+-rw-rw-rw-   0        0        0     4461 2023-04-25 02:00:24.000000 dramkit-0.5.42/dramkit/openai/openai_chat_hs.py
+drwxrwxrwx   0        0        0        0 2023-05-21 02:55:36.627221 dramkit-0.5.42/dramkit/optimizer/
+-rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.42/dramkit/optimizer/__init__.py
+-rw-rw-rw-   0        0        0     9712 2023-03-22 08:26:32.000000 dramkit-0.5.42/dramkit/optimizer/alo.py
+-rw-rw-rw-   0        0        0     3141 2022-05-02 02:31:44.000000 dramkit-0.5.42/dramkit/optimizer/base_funcs.py
+-rw-rw-rw-   0        0        0     7428 2023-03-22 08:35:00.000000 dramkit-0.5.42/dramkit/optimizer/boa.py
+-rw-rw-rw-   0        0        0     8863 2023-03-22 08:34:30.000000 dramkit-0.5.42/dramkit/optimizer/cs.py
+-rw-rw-rw-   0        0        0    13415 2023-03-22 08:33:50.000000 dramkit-0.5.42/dramkit/optimizer/ga.py
+-rw-rw-rw-   0        0        0     8701 2023-03-22 08:33:17.000000 dramkit-0.5.42/dramkit/optimizer/gwo.py
+-rw-rw-rw-   0        0        0     9311 2023-03-22 08:32:10.000000 dramkit-0.5.42/dramkit/optimizer/hcpsoboa.py
+-rw-rw-rw-   0        0        0     9929 2023-03-22 08:31:27.000000 dramkit-0.5.42/dramkit/optimizer/hho.py
+-rw-rw-rw-   0        0        0     8817 2023-03-22 08:30:38.000000 dramkit-0.5.42/dramkit/optimizer/hpsoboa.py
+-rw-rw-rw-   0        0        0     8889 2023-03-22 08:29:43.000000 dramkit-0.5.42/dramkit/optimizer/pso.py
+-rw-rw-rw-   0        0        0     5222 2022-05-02 02:18:28.000000 dramkit-0.5.42/dramkit/optimizer/utils_heuristic.py
+-rw-rw-rw-   0        0        0     7334 2023-03-22 08:27:35.000000 dramkit-0.5.42/dramkit/optimizer/woa.py
+drwxrwxrwx   0        0        0        0 2023-05-21 02:55:36.634202 dramkit-0.5.42/dramkit/other/
+-rw-rw-rw-   0        0        0     3856 2023-04-30 10:22:45.000000 dramkit-0.5.42/dramkit/other/_Linux_notes.py
+-rw-rw-rw-   0        0        0     2947 2023-05-17 06:10:10.000000 dramkit-0.5.42/dramkit/other/_Python_notes.py
+-rw-rw-rw-   0        0        0     4777 2023-04-24 08:14:04.000000 dramkit-0.5.42/dramkit/other/_Vim_notes.py
+-rw-rw-rw-   0        0        0      164 2022-08-25 01:46:27.000000 dramkit-0.5.42/dramkit/other/__init__.py
+-rw-rw-rw-   0        0        0     7988 2022-10-27 06:38:44.000000 dramkit-0.5.42/dramkit/other/langconv.py
+-rw-rw-rw-   0        0        0     8353 2022-12-10 15:26:10.000000 dramkit-0.5.42/dramkit/other/othertools.py
+-rw-rw-rw-   0        0        0     1804 2023-03-22 08:36:51.000000 dramkit-0.5.42/dramkit/other/replace_endblank.py
+-rw-rw-rw-   0        0        0   143066 2022-08-25 01:37:20.000000 dramkit-0.5.42/dramkit/other/zh_wiki.py
+drwxrwxrwx   0        0        0        0 2023-05-21 02:55:36.640186 dramkit-0.5.42/dramkit/plottools/
+-rw-rw-rw-   0        0        0      112 2022-05-04 14:50:04.000000 dramkit-0.5.42/dramkit/plottools/__init__.py
+-rw-rw-rw-   0        0        0     4400 2022-01-09 07:36:22.000000 dramkit-0.5.42/dramkit/plottools/plot_barline.py
+-rw-rw-rw-   0        0        0    48559 2023-04-22 13:09:27.000000 dramkit-0.5.42/dramkit/plottools/plot_common.py
+-rw-rw-rw-   0        0        0     9033 2022-06-25 18:36:48.000000 dramkit-0.5.42/dramkit/plottools/plot_histdist.py
+-rw-rw-rw-   0        0        0     2145 2023-03-04 13:10:35.000000 dramkit-0.5.42/dramkit/plottools/plot_scatter.py
+-rw-rw-rw-   0        0        0     5120 2023-03-21 14:27:12.000000 dramkit-0.5.42/dramkit/plottools/utils_plot.py
+drwxrwxrwx   0        0        0        0 2023-05-21 02:55:36.641183 dramkit-0.5.42/dramkit/pystyles/
+-rw-rw-rw-   0        0        0       25 2021-12-25 16:04:07.000000 dramkit-0.5.42/dramkit/pystyles/__init__.py
+-rw-rw-rw-   0        0        0     8021 2022-04-30 13:24:37.000000 dramkit-0.5.42/dramkit/pystyles/dramkit_style.py
+drwxrwxrwx   0        0        0        0 2023-05-21 02:55:36.645169 dramkit-0.5.42/dramkit/sorts/
+-rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.42/dramkit/sorts/__init__.py
+-rw-rw-rw-   0        0        0     1302 2022-01-09 08:45:28.000000 dramkit-0.5.42/dramkit/sorts/bubble_sort.py
+-rw-rw-rw-   0        0        0     1426 2022-01-09 08:51:55.000000 dramkit-0.5.42/dramkit/sorts/bucket_sort.py
+-rw-rw-rw-   0        0        0     4742 2022-01-09 08:10:56.000000 dramkit-0.5.42/dramkit/sorts/insert_sort.py
+-rw-rw-rw-   0        0        0     4833 2022-01-09 09:23:30.000000 dramkit-0.5.42/dramkit/sorts/insert_sort_bin.py
+-rw-rw-rw-   0        0        0     1339 2022-01-09 08:55:14.000000 dramkit-0.5.42/dramkit/sorts/quick_sort.py
+drwxrwxrwx   0        0        0        0 2023-05-21 02:55:36.652150 dramkit-0.5.42/dramkit/speedup/
+-rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.42/dramkit/speedup/__init__.py
+-rw-rw-rw-   0        0        0     1231 2023-04-14 13:02:46.000000 dramkit-0.5.42/dramkit/speedup/_mp_test1.py
+-rw-rw-rw-   0        0        0      886 2023-04-14 13:17:44.000000 dramkit-0.5.42/dramkit/speedup/_mp_test2.py
+-rw-rw-rw-   0        0        0      684 2023-04-14 13:14:44.000000 dramkit-0.5.42/dramkit/speedup/_mp_test3.py
+-rw-rw-rw-   0        0        0     3384 2023-04-14 13:25:51.000000 dramkit-0.5.42/dramkit/speedup/iotools_tmp.py
+-rw-rw-rw-   0        0        0     3754 2023-04-12 08:17:22.000000 dramkit-0.5.42/dramkit/speedup/multi_process_concurrent.py
+-rw-rw-rw-   0        0        0     7888 2023-04-07 08:59:34.000000 dramkit-0.5.42/dramkit/speedup/multi_thread.py
+drwxrwxrwx   0        0        0        0 2023-05-21 02:55:36.659136 dramkit-0.5.42/dramkit/sqltools/
+-rw-rw-rw-   0        0        0     2495 2023-02-23 05:15:08.000000 dramkit-0.5.42/dramkit/sqltools/_Hive_notes.py
+-rw-rw-rw-   0        0        0    30416 2023-04-11 01:33:28.000000 dramkit-0.5.42/dramkit/sqltools/_MySQL_notes.py
+-rw-rw-rw-   0        0        0     6849 2023-03-07 09:26:53.000000 dramkit-0.5.42/dramkit/sqltools/_Oracle_notes.py
+-rw-rw-rw-   0        0        0      160 2023-05-01 12:57:19.000000 dramkit-0.5.42/dramkit/sqltools/__init__.py
+-rw-rw-rw-   0        0        0    20285 2023-05-06 13:49:07.000000 dramkit-0.5.42/dramkit/sqltools/cxoracle.py
+-rw-rw-rw-   0        0        0    25908 2023-02-24 11:31:13.000000 dramkit-0.5.42/dramkit/sqltools/py_hive.py
+-rw-rw-rw-   0        0        0    50966 2023-05-06 13:23:21.000000 dramkit-0.5.42/dramkit/sqltools/py_mysql.py
+-rw-rw-rw-   0        0        0    18391 2023-03-22 02:56:24.000000 dramkit-0.5.42/dramkit/sqltools/sql_alchemy.py
+drwxrwxrwx   0        0        0        0 2023-05-21 02:55:36.660132 dramkit-0.5.42/dramkit/webtools/
+-rw-rw-rw-   0        0        0       25 2021-12-24 09:25:22.000000 dramkit-0.5.42/dramkit/webtools/__init__.py
+-rw-rw-rw-   0        0        0     5337 2022-06-25 18:37:55.000000 dramkit-0.5.42/dramkit/webtools/utils_html.py
+drwxrwxrwx   0        0        0        0 2023-05-21 02:55:36.662123 dramkit-0.5.42/dramkit/wechat/
+-rw-rw-rw-   0        0        0       58 2022-09-06 14:04:57.000000 dramkit-0.5.42/dramkit/wechat/__init__.py
+-rw-rw-rw-   0        0        0     7473 2022-10-28 03:03:37.000000 dramkit-0.5.42/dramkit/wechat/qywechat.py
+drwxrwxrwx   0        0        0        0 2023-05-21 02:55:36.510533 dramkit-0.5.42/dramkit.egg-info/
+-rw-rw-rw-   0        0        0     1095 2023-05-21 02:55:36.000000 dramkit-0.5.42/dramkit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4877 2023-05-21 02:55:36.000000 dramkit-0.5.42/dramkit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-21 02:55:36.000000 dramkit-0.5.42/dramkit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2023-05-21 02:55:36.000000 dramkit-0.5.42/dramkit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-21 02:55:36.000000 dramkit-0.5.42/dramkit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-21 02:55:36.663125 dramkit-0.5.42/setup.cfg
+-rw-rw-rw-   0        0        0     1944 2023-05-01 12:58:33.000000 dramkit-0.5.42/setup.py
```

### Comparing `dramkit-0.5.41/LICENSE` & `dramkit-0.5.42/LICENSE`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/PKG-INFO` & `dramkit-0.5.42/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dramkit
-Version: 0.5.41
+Version: 0.5.42
 Summary: DramKit is a toolbox.
 Home-page: https://github.com/Genlovy-Hoo/dramkit/
 Author: Genlovy Hoo, YueYong Hu
 Author-email: genlovhyy@163.com
 License: MIT
 Platform: any
 Description-Content-Type: text/markdown
```

### Comparing `dramkit-0.5.41/README.md` & `dramkit-0.5.42/README.md`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/__init__.py` & `dramkit-0.5.42/dramkit/__init__.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/_pkg_info.py` & `dramkit-0.5.42/dramkit/_pkg_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 pkg_info = {
     '__pkgname__': 'dramkit',
-    '__version__': '0.5.41',
+    '__version__': '0.5.42',
     '__license__': 'MIT',
     '__url__': 'https://github.com/Genlovy-Hoo/dramkit/',
     '__urls__':
         {'pypi': 'https://pypi.org/project/dramkit/',
          'github': 'https://github.com/Genlovy-Hoo/dramkit/',
 		 'document': 'http://www.glhyy.cn/dramkit/doc/html/index.html'
         },
```

### Comparing `dramkit-0.5.41/dramkit/_tmp/CRR.py` & `dramkit-0.5.42/dramkit/_tmp/CRR.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/_tmp/CtrlPreTS.py` & `dramkit-0.5.42/dramkit/_tmp/CtrlPreTS.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/_tmp/NPairSum.py` & `dramkit-0.5.42/dramkit/_tmp/NPairSum.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/_tmp/PIDtest.py` & `dramkit-0.5.42/dramkit/_tmp/PIDtest.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/_tmp/PIDtest2.py` & `dramkit-0.5.42/dramkit/_tmp/PIDtest2.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/_tmp/VMD.py` & `dramkit-0.5.42/dramkit/_tmp/VMD.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/_tmp/cca_test.py` & `dramkit-0.5.42/dramkit/_tmp/cca_test.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/_tmp/dtw_test.py` & `dramkit-0.5.42/dramkit/_tmp/dtw_test.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/_tmp/explore.py` & `dramkit-0.5.42/dramkit/_tmp/explore.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/_tmp/gini.py` & `dramkit-0.5.42/dramkit/_tmp/gini.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/_tmp/merge_sort.py` & `dramkit-0.5.42/dramkit/_tmp/merge_sort.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/_tmp/mouse_move.py` & `dramkit-0.5.42/dramkit/_tmp/mouse_move.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/_tmp/mpc_test1.py` & `dramkit-0.5.42/dramkit/_tmp/mpc_test1.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/_tmp/options_Implied_volatility.py` & `dramkit-0.5.42/dramkit/_tmp/options_Implied_volatility.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/_tmp/plot_test.py` & `dramkit-0.5.42/dramkit/_tmp/plot_test.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/_tmp/plot_test2.py` & `dramkit-0.5.42/dramkit/_tmp/plot_test2.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/_tmp/simple_smooth.py` & `dramkit-0.5.42/dramkit/_tmp/simple_smooth.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/_tmp/test_async_washs.py` & `dramkit-0.5.42/dramkit/_tmp/test_async_washs.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/_tmp/test_await_timeout.py` & `dramkit-0.5.42/dramkit/_tmp/test_await_timeout.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/_tmp/test_backtrader.py` & `dramkit-0.5.42/dramkit/_tmp/test_backtrader.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/_tmp/test_chatgpt_v1.py` & `dramkit-0.5.42/dramkit/_tmp/test_chatgpt_v1.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/_tmp/test_code.py` & `dramkit-0.5.42/dramkit/_tmp/test_code.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/_tmp/test_find_peaks.py` & `dramkit-0.5.42/dramkit/_tmp/test_find_peaks.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/_tmp/test_get_var_name.py` & `dramkit-0.5.42/dramkit/_tmp/test_get_var_name.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/_tmp/test_grading.py` & `dramkit-0.5.42/dramkit/_tmp/test_grading.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/_tmp/test_lr.py` & `dramkit-0.5.42/dramkit/_tmp/test_lr.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/_tmp/test_maxsort.py` & `dramkit-0.5.42/dramkit/_tmp/test_maxsort.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/_tmp/test_pywechat.py` & `dramkit-0.5.42/dramkit/_tmp/test_pywechat.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/_tmp/test_tree.py` & `dramkit-0.5.42/dramkit/_tmp/test_tree.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/_tmp/test_tree2.py` & `dramkit-0.5.42/dramkit/_tmp/test_tree2.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/_tmp/test_wechat_work.py` & `dramkit-0.5.42/dramkit/_tmp/test_wechat_work.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/_tmp/tfDNNCls_test.py` & `dramkit-0.5.42/dramkit/_tmp/tfDNNCls_test.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/_tmp/tmp.py` & `dramkit-0.5.42/dramkit/_tmp/tmp.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/_tmp/tmp_args.py` & `dramkit-0.5.42/dramkit/_tmp/tmp_args.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/_tmp/transformer_pytorch.py` & `dramkit-0.5.42/dramkit/_tmp/transformer_pytorch.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/_tmp/utils_SignalDec.py` & `dramkit-0.5.42/dramkit/_tmp/utils_SignalDec.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/_tmp/utils_TimeSeries.py` & `dramkit-0.5.42/dramkit/_tmp/utils_TimeSeries.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/_tmp/utils_lottery.py` & `dramkit-0.5.42/dramkit/_tmp/utils_lottery.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/_tmp/utils_rl.py` & `dramkit-0.5.42/dramkit/_tmp/utils_rl.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/_tmp/utils_rl2.py` & `dramkit-0.5.42/dramkit/_tmp/utils_rl2.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/_tmp/utils_rl3.py` & `dramkit-0.5.42/dramkit/_tmp/utils_rl3.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/_tmp/utils_rl4.py` & `dramkit-0.5.42/dramkit/_tmp/utils_rl4.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/_tmp/utils_rl5.py` & `dramkit-0.5.42/dramkit/_tmp/utils_rl5.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/_tmp/utils_rl6.py` & `dramkit-0.5.42/dramkit/_tmp/utils_rl6.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/_tmp/utils_rl7.py` & `dramkit-0.5.42/dramkit/_tmp/utils_rl7.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/_tmp/utils_sem.py` & `dramkit-0.5.42/dramkit/_tmp/utils_sem.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/backpacks/backpack01_float_dy.py` & `dramkit-0.5.42/dramkit/backpacks/backpack01_float_dy.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/backpacks/backpack01_int_dy.py` & `dramkit-0.5.42/dramkit/backpacks/backpack01_int_dy.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/chncal/__init__.py` & `dramkit-0.5.42/dramkit/chncal/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 
 # from __future__ import absolute_import, unicode_literals
 
-__version__ = '2.2.1'
+__version__ = '2.2.3'
 
 from .apis import (
     find_workday,
     get_dates,
     get_holiday_detail,
     get_holidays,
     get_solar_terms,
```

### Comparing `dramkit-0.5.41/dramkit/chncal/apis.py` & `dramkit-0.5.42/dramkit/chncal/apis.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from __future__ import absolute_import, unicode_literals
 
 import time
 import datetime
 import pandas as pd
 
-# '''
+'''
 from .constants import (holidays,
                         in_lieu_days,
                         workdays)
 from .solar_terms import (SolarTerms,
                           SOLAR_TERMS_C_NUMS,
                           SOLAR_TERMS_MONTH,
                           SOLAR_TERMS_DELTA)
@@ -24,15 +24,15 @@
 from .constants_trade_dates import trade_dates
 from .constants_hko import gen_lun, lun_gen, gen_gz
 from .constants_fate import w_year, w_month, w_date, w_hour, song
 from .constants_zodiac_marry import zodiac_match
 from .constants_wuxing import tgwx, dzwx, tgdznywx
 # '''
 
-'''
+# '''
 from chncal.constants import (holidays,
                               in_lieu_days,
                               workdays)
 from chncal.solar_terms import (SolarTerms,
                                 SOLAR_TERMS_C_NUMS,
                                 SOLAR_TERMS_MONTH,
                                 SOLAR_TERMS_DELTA)
@@ -596,28 +596,33 @@
     date = _trans_date(date)
     tdelta = datetime.timedelta(1)
     if dirt == 'post':
         while not is_tradeday(date, market=market):
             date = date + tdelta
     elif dirt == 'pre':
         while not is_tradeday(date, market=market):
+            if date.date() < MARKETS[market]:
+                date = MARKETS[market]
+                break
             date = date - tdelta
     return _wrap_date(date)
 
 
 def get_next_nth_tradeday(date=None, n=1, market='SSE'):
     '''
     | 给定日期date，返回其后第n个交易日日期，n可为负数（返回结果在date之前）
     | 若n为0，直接返回date
     '''
     date = _trans_date(date)
     n_add = -1 if n < 0 else 1
     n = abs(n)
     tmp = 0
     while tmp < n:
+        if n_add == -1 and date.date() <= MARKETS[market]:
+            break
         date = date + datetime.timedelta(n_add)
         if is_tradeday(date, market=market):
             tmp += 1
     return _wrap_date(date)
 
 
 def get_trade_dates(start_date, end_date=None, market='SSE'):
```

### Comparing `dramkit-0.5.41/dramkit/chncal/constants.py` & `dramkit-0.5.42/dramkit/chncal/constants.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/chncal/constants_fate.py` & `dramkit-0.5.42/dramkit/chncal/constants_fate.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/chncal/constants_hko.py` & `dramkit-0.5.42/dramkit/chncal/constants_hko.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/chncal/constants_trade_dates.py` & `dramkit-0.5.42/dramkit/chncal/constants_trade_dates.py`

 * *Files 0% similar despite different names*

```diff
@@ -6094,14 +6094,21 @@
     ("CFFEX", datetime.date(year=2023, month=5, day=6)): 0,
     ("CFFEX", datetime.date(year=2023, month=5, day=7)): 0,
     ("CFFEX", datetime.date(year=2023, month=5, day=8)): 1,
     ("CFFEX", datetime.date(year=2023, month=5, day=9)): 1,
     ("CFFEX", datetime.date(year=2023, month=5, day=10)): 1,
     ("CFFEX", datetime.date(year=2023, month=5, day=11)): 1,
     ("CFFEX", datetime.date(year=2023, month=5, day=12)): 1,
+    ("CFFEX", datetime.date(year=2023, month=5, day=13)): 0,
+    ("CFFEX", datetime.date(year=2023, month=5, day=14)): 0,
+    ("CFFEX", datetime.date(year=2023, month=5, day=15)): 1,
+    ("CFFEX", datetime.date(year=2023, month=5, day=16)): 1,
+    ("CFFEX", datetime.date(year=2023, month=5, day=17)): 1,
+    ("CFFEX", datetime.date(year=2023, month=5, day=18)): 1,
+    ("CFFEX", datetime.date(year=2023, month=5, day=19)): 1,
     ("CZCE", datetime.date(year=1990, month=10, day=12)): 1,
     ("CZCE", datetime.date(year=1990, month=10, day=13)): 0,
     ("CZCE", datetime.date(year=1990, month=10, day=14)): 0,
     ("CZCE", datetime.date(year=1990, month=10, day=15)): 1,
     ("CZCE", datetime.date(year=1990, month=10, day=16)): 1,
     ("CZCE", datetime.date(year=1990, month=10, day=17)): 1,
     ("CZCE", datetime.date(year=1990, month=10, day=18)): 1,
@@ -17994,14 +18001,21 @@
     ("CZCE", datetime.date(year=2023, month=5, day=6)): 0,
     ("CZCE", datetime.date(year=2023, month=5, day=7)): 0,
     ("CZCE", datetime.date(year=2023, month=5, day=8)): 1,
     ("CZCE", datetime.date(year=2023, month=5, day=9)): 1,
     ("CZCE", datetime.date(year=2023, month=5, day=10)): 1,
     ("CZCE", datetime.date(year=2023, month=5, day=11)): 1,
     ("CZCE", datetime.date(year=2023, month=5, day=12)): 1,
+    ("CZCE", datetime.date(year=2023, month=5, day=13)): 0,
+    ("CZCE", datetime.date(year=2023, month=5, day=14)): 0,
+    ("CZCE", datetime.date(year=2023, month=5, day=15)): 1,
+    ("CZCE", datetime.date(year=2023, month=5, day=16)): 1,
+    ("CZCE", datetime.date(year=2023, month=5, day=17)): 1,
+    ("CZCE", datetime.date(year=2023, month=5, day=18)): 1,
+    ("CZCE", datetime.date(year=2023, month=5, day=19)): 1,
     ("DCE", datetime.date(year=1993, month=3, day=1)): 1,
     ("DCE", datetime.date(year=1993, month=3, day=2)): 1,
     ("DCE", datetime.date(year=1993, month=3, day=3)): 1,
     ("DCE", datetime.date(year=1993, month=3, day=4)): 1,
     ("DCE", datetime.date(year=1993, month=3, day=5)): 1,
     ("DCE", datetime.date(year=1993, month=3, day=6)): 0,
     ("DCE", datetime.date(year=1993, month=3, day=7)): 0,
@@ -29023,14 +29037,21 @@
     ("DCE", datetime.date(year=2023, month=5, day=6)): 0,
     ("DCE", datetime.date(year=2023, month=5, day=7)): 0,
     ("DCE", datetime.date(year=2023, month=5, day=8)): 1,
     ("DCE", datetime.date(year=2023, month=5, day=9)): 1,
     ("DCE", datetime.date(year=2023, month=5, day=10)): 1,
     ("DCE", datetime.date(year=2023, month=5, day=11)): 1,
     ("DCE", datetime.date(year=2023, month=5, day=12)): 1,
+    ("DCE", datetime.date(year=2023, month=5, day=13)): 0,
+    ("DCE", datetime.date(year=2023, month=5, day=14)): 0,
+    ("DCE", datetime.date(year=2023, month=5, day=15)): 1,
+    ("DCE", datetime.date(year=2023, month=5, day=16)): 1,
+    ("DCE", datetime.date(year=2023, month=5, day=17)): 1,
+    ("DCE", datetime.date(year=2023, month=5, day=18)): 1,
+    ("DCE", datetime.date(year=2023, month=5, day=19)): 1,
     ("INE", datetime.date(year=2017, month=5, day=23)): 1,
     ("INE", datetime.date(year=2017, month=5, day=24)): 1,
     ("INE", datetime.date(year=2017, month=5, day=25)): 1,
     ("INE", datetime.date(year=2017, month=5, day=26)): 1,
     ("INE", datetime.date(year=2017, month=5, day=27)): 0,
     ("INE", datetime.date(year=2017, month=5, day=28)): 0,
     ("INE", datetime.date(year=2017, month=5, day=29)): 0,
@@ -31203,14 +31224,21 @@
     ("INE", datetime.date(year=2023, month=5, day=6)): 0,
     ("INE", datetime.date(year=2023, month=5, day=7)): 0,
     ("INE", datetime.date(year=2023, month=5, day=8)): 1,
     ("INE", datetime.date(year=2023, month=5, day=9)): 1,
     ("INE", datetime.date(year=2023, month=5, day=10)): 1,
     ("INE", datetime.date(year=2023, month=5, day=11)): 1,
     ("INE", datetime.date(year=2023, month=5, day=12)): 1,
+    ("INE", datetime.date(year=2023, month=5, day=13)): 0,
+    ("INE", datetime.date(year=2023, month=5, day=14)): 0,
+    ("INE", datetime.date(year=2023, month=5, day=15)): 1,
+    ("INE", datetime.date(year=2023, month=5, day=16)): 1,
+    ("INE", datetime.date(year=2023, month=5, day=17)): 1,
+    ("INE", datetime.date(year=2023, month=5, day=18)): 1,
+    ("INE", datetime.date(year=2023, month=5, day=19)): 1,
     ("SHFE", datetime.date(year=1991, month=5, day=28)): 1,
     ("SHFE", datetime.date(year=1991, month=5, day=29)): 1,
     ("SHFE", datetime.date(year=1991, month=5, day=30)): 1,
     ("SHFE", datetime.date(year=1991, month=5, day=31)): 1,
     ("SHFE", datetime.date(year=1991, month=6, day=1)): 0,
     ("SHFE", datetime.date(year=1991, month=6, day=2)): 0,
     ("SHFE", datetime.date(year=1991, month=6, day=3)): 1,
@@ -42875,14 +42903,21 @@
     ("SHFE", datetime.date(year=2023, month=5, day=6)): 0,
     ("SHFE", datetime.date(year=2023, month=5, day=7)): 0,
     ("SHFE", datetime.date(year=2023, month=5, day=8)): 1,
     ("SHFE", datetime.date(year=2023, month=5, day=9)): 1,
     ("SHFE", datetime.date(year=2023, month=5, day=10)): 1,
     ("SHFE", datetime.date(year=2023, month=5, day=11)): 1,
     ("SHFE", datetime.date(year=2023, month=5, day=12)): 1,
+    ("SHFE", datetime.date(year=2023, month=5, day=13)): 0,
+    ("SHFE", datetime.date(year=2023, month=5, day=14)): 0,
+    ("SHFE", datetime.date(year=2023, month=5, day=15)): 1,
+    ("SHFE", datetime.date(year=2023, month=5, day=16)): 1,
+    ("SHFE", datetime.date(year=2023, month=5, day=17)): 1,
+    ("SHFE", datetime.date(year=2023, month=5, day=18)): 1,
+    ("SHFE", datetime.date(year=2023, month=5, day=19)): 1,
     ("SSE", datetime.date(year=1990, month=12, day=19)): 1,
     ("SSE", datetime.date(year=1990, month=12, day=20)): 1,
     ("SSE", datetime.date(year=1990, month=12, day=21)): 1,
     ("SSE", datetime.date(year=1990, month=12, day=22)): 0,
     ("SSE", datetime.date(year=1990, month=12, day=23)): 0,
     ("SSE", datetime.date(year=1990, month=12, day=24)): 1,
     ("SSE", datetime.date(year=1990, month=12, day=25)): 1,
@@ -54708,14 +54743,21 @@
     ("SSE", datetime.date(year=2023, month=5, day=6)): 0,
     ("SSE", datetime.date(year=2023, month=5, day=7)): 0,
     ("SSE", datetime.date(year=2023, month=5, day=8)): 1,
     ("SSE", datetime.date(year=2023, month=5, day=9)): 1,
     ("SSE", datetime.date(year=2023, month=5, day=10)): 1,
     ("SSE", datetime.date(year=2023, month=5, day=11)): 1,
     ("SSE", datetime.date(year=2023, month=5, day=12)): 1,
+    ("SSE", datetime.date(year=2023, month=5, day=13)): 0,
+    ("SSE", datetime.date(year=2023, month=5, day=14)): 0,
+    ("SSE", datetime.date(year=2023, month=5, day=15)): 1,
+    ("SSE", datetime.date(year=2023, month=5, day=16)): 1,
+    ("SSE", datetime.date(year=2023, month=5, day=17)): 1,
+    ("SSE", datetime.date(year=2023, month=5, day=18)): 1,
+    ("SSE", datetime.date(year=2023, month=5, day=19)): 1,
     ("SZSE", datetime.date(year=1991, month=7, day=3)): 1,
     ("SZSE", datetime.date(year=1991, month=7, day=4)): 1,
     ("SZSE", datetime.date(year=1991, month=7, day=5)): 1,
     ("SZSE", datetime.date(year=1991, month=7, day=6)): 0,
     ("SZSE", datetime.date(year=1991, month=7, day=7)): 0,
     ("SZSE", datetime.date(year=1991, month=7, day=8)): 1,
     ("SZSE", datetime.date(year=1991, month=7, day=9)): 1,
@@ -66345,8 +66387,15 @@
     ("SZSE", datetime.date(year=2023, month=5, day=6)): 0,
     ("SZSE", datetime.date(year=2023, month=5, day=7)): 0,
     ("SZSE", datetime.date(year=2023, month=5, day=8)): 1,
     ("SZSE", datetime.date(year=2023, month=5, day=9)): 1,
     ("SZSE", datetime.date(year=2023, month=5, day=10)): 1,
     ("SZSE", datetime.date(year=2023, month=5, day=11)): 1,
     ("SZSE", datetime.date(year=2023, month=5, day=12)): 1,
+    ("SZSE", datetime.date(year=2023, month=5, day=13)): 0,
+    ("SZSE", datetime.date(year=2023, month=5, day=14)): 0,
+    ("SZSE", datetime.date(year=2023, month=5, day=15)): 1,
+    ("SZSE", datetime.date(year=2023, month=5, day=16)): 1,
+    ("SZSE", datetime.date(year=2023, month=5, day=17)): 1,
+    ("SZSE", datetime.date(year=2023, month=5, day=18)): 1,
+    ("SZSE", datetime.date(year=2023, month=5, day=19)): 1,
 }
```

### Comparing `dramkit-0.5.41/dramkit/chncal/constants_wuxing.py` & `dramkit-0.5.42/dramkit/chncal/constants_wuxing.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/chncal/constants_zodiac_marry.py` & `dramkit-0.5.42/dramkit/chncal/constants_zodiac_marry.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/chncal/solar_terms.py` & `dramkit-0.5.42/dramkit/chncal/solar_terms.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/cryptotools.py` & `dramkit-0.5.42/dramkit/cryptotools.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/datetimetools.py` & `dramkit-0.5.42/dramkit/datetimetools.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,14 +29,17 @@
 
 
 # pandas模块和datetime以及time模块的时间戳有差别（pd多8小时(28800秒)，后两者是一致的）
 TSDIF_PD_DTTM = pd.to_datetime('19700102 08:00:00').timestamp() - \
                 datetime.datetime(1970, 1, 2, 8, 0, 0).timestamp()
 TS_BIAS_DT = (datetime.datetime.fromtimestamp(0) - \
               datetime.datetime.utcfromtimestamp(0)).seconds
+    
+MONTH_DAYS = {1: 31, 2: 28, 3:31, 4: 30, 5:31, 6:30, 7: 31,
+              8: 31, 9: 30, 10: 31, 11:30, 12: 31}
 
 
 def _show_time_infos():
     t, t_ns = time.time(), time.time_ns()
     print('原始时间戳:                ', t)
     print('秒级(second, 10位):       ', int(t))
     print('毫秒级(millisecond, 13位):', int(round(t*1000)))
@@ -541,19 +544,25 @@
     # 到毫秒
     # return dt.isoformat(sep=' ', timespec='milliseconds')
     # return dt.strftime('%Y-%m-%d %H:%M:%S.%f')[:-3]
 
 
 def today_month(joiner='-'):
     '''获取今日所在年月，格式由连接符joiner确定'''
+    if joiner.lower() == 'int':
+        return int(datetime.date.today().strftime('%Y%m'))
     return datetime.date.today().strftime('%Y{}%m'.format(joiner))
 
 
 def today_date(joiner='-'):
     '''获取今日日期，格式由连接符joiner确定'''
+    if joiner.lower() == 'int':
+        return int(datetime.date.today().strftime('%Y%m%d'))
+    if joiner.lower() in ['dt', 'datetime']:
+        return pd.to_datetime(datetime.date.today())
     return datetime.date.today().strftime(joiner.join(['%Y', '%m', '%d']))
 
 
 def get_quarter(dt=None, joiner='Q'):
     '''获取日期所在季度'''
     if pd.isnull(dt):
         dt = datetime.datetime.now()
@@ -668,16 +677,20 @@
 
 
 def get_month_end(date=None):
     '''获取date所在月的月末日期'''
     if pd.isnull(date):
         date = today_date()
     day = x2datetime(date)
-    next_month = day.replace(day=28) + datetime.timedelta(days=4)
-    month_end = next_month - datetime.timedelta(days=next_month.day)
+    m = day.month
+    if m != 2:
+        month_end = day.replace(day=MONTH_DAYS[m])
+    else:
+        next_month = day.replace(day=28) + datetime.timedelta(days=4)
+        month_end = next_month - datetime.timedelta(days=next_month.day)
     return copy_format(month_end, date)
 
 
 def get_next_nmonth_start_end(date=None, n=1):
     if pd.isnull(date):
         date = today_date()
     day = x2datetime(date)
```

### Comparing `dramkit-0.5.41/dramkit/datsci/_utils_ann.py` & `dramkit-0.5.42/dramkit/datsci/_utils_ann.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/datsci/activate_funcs.py` & `dramkit-0.5.42/dramkit/datsci/activate_funcs.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/datsci/ahp.py` & `dramkit-0.5.42/dramkit/datsci/ahp.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/datsci/ahp_sim_ri.py` & `dramkit-0.5.42/dramkit/datsci/ahp_sim_ri.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/datsci/apriori.py` & `dramkit-0.5.42/dramkit/datsci/apriori.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/datsci/curvature.py` & `dramkit-0.5.42/dramkit/datsci/curvature.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/datsci/elm_cls.py` & `dramkit-0.5.42/dramkit/datsci/elm_cls.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/datsci/elm_reg.py` & `dramkit-0.5.42/dramkit/datsci/elm_reg.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/datsci/entropy_weight.py` & `dramkit-0.5.42/dramkit/datsci/entropy_weight.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/datsci/find_maxmin.py` & `dramkit-0.5.42/dramkit/datsci/find_maxmin.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/datsci/freq_item_set.py` & `dramkit-0.5.42/dramkit/datsci/freq_item_set.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/datsci/lr.py` & `dramkit-0.5.42/dramkit/datsci/lr.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/datsci/preprocess.py` & `dramkit-0.5.42/dramkit/datsci/preprocess.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,64 @@
 # -*- coding: utf-8 -*-
 
 import numpy as np
 import pandas as pd
+from collections.abc import Callable
 
 from sklearn.decomposition import PCA
 from sklearn.preprocessing import StandardScaler, MinMaxScaler
 
 from dramkit.gentools import con_count, isnull
 
 
-def mad(series, n=3, up_cut_val=None, low_cut_val=None):
-    '''MAD计算值处理方法'''
+def cut_mad(series, n=3,
+            up_cut_val=None,
+            low_cut_val=None,
+            func_filter=None):
+    '''
+    | MAD极端值处理方法
+    | func_filter为对计算中位数和偏差之前对数据进行筛的函数，返回值为True的才参与计算
+    '''
+    isinstance(func_filter, (Callable, type(None)))
     values = np.array(series)
-    median = np.nanmedian(values, axis=0)
-    abs_med_dif = np.abs(values - median)
+    if isnull(func_filter):
+        values_ = values.copy()
+    else:
+        values_ = values[func_filter(values)]
+    median = np.nanmedian(values_, axis=0)
+    abs_med_dif = np.abs(values_ - median)
     med = np.nanmedian(abs_med_dif) * 1.483
     upper = median + n * med
     lower = median - n * med
     if isnull(up_cut_val):
         up_cut_val = upper
     if isnull(low_cut_val):
         low_cut_val = lower
     values[values > upper] = up_cut_val
     values[values < lower] = low_cut_val
     try:
         return pd.Series(values, index=series.index)
     except:
         return values
+    
+    
+def cut_nstd(series, n=3, up_cut_val=None, low_cut_val=None):
+    '''标准差倍数截断方法，极端值处理'''
+    df = pd.DataFrame({'s': series})
+    mean = df['s'].mean()
+    std = df['s'].std()
+    upper = mean + n * std
+    lower = mean - n * std
+    if isnull(up_cut_val):
+        up_cut_val = upper
+    if isnull(low_cut_val):
+        low_cut_val = lower
+    df.loc[df['s'] > upper, 's'] = up_cut_val
+    df.loc[df['s'] < lower, 's'] = low_cut_val
+    return df['s']
 
 
 class ExternalStd(object):
     '''极端值处理，标准差倍数法'''
 
     def __init__(self, nstd=3, cols=None):
         raise NotImplementedError
```

### Comparing `dramkit-0.5.41/dramkit/datsci/stats.py` & `dramkit-0.5.42/dramkit/datsci/stats.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/datsci/time_series.py` & `dramkit-0.5.42/dramkit/datsci/time_series.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/datsci/topsis.py` & `dramkit-0.5.42/dramkit/datsci/topsis.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/datsci/utils_lgb.py` & `dramkit-0.5.42/dramkit/datsci/utils_lgb.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/datsci/utils_ml.py` & `dramkit-0.5.42/dramkit/datsci/utils_ml.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/datsci/zigzag.py` & `dramkit-0.5.42/dramkit/datsci/zigzag.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/find_addends/find_addends_backpack01float.py` & `dramkit-0.5.42/dramkit/find_addends/find_addends_backpack01float.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/find_addends/find_addends_backpack01int.py` & `dramkit-0.5.42/dramkit/find_addends/find_addends_backpack01int.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/find_addends/find_addends_bigfirst.py` & `dramkit-0.5.42/dramkit/find_addends/find_addends_bigfirst.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/find_addends/find_addends_recu.py` & `dramkit-0.5.42/dramkit/find_addends/find_addends_recu.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/find_addends/find_addends_smlfirst.py` & `dramkit-0.5.42/dramkit/find_addends/find_addends_smlfirst.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/find_addends/find_addends_utils.py` & `dramkit-0.5.42/dramkit/find_addends/find_addends_utils.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/gentools.py` & `dramkit-0.5.42/dramkit/gentools.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,21 +15,25 @@
 import datetime
 import traceback
 import numpy as np
 import pandas as pd
 import urllib.parse
 from tqdm import tqdm
 from io import StringIO
+from itertools import product
 from collections import Counter
 from functools import reduce, wraps
 from random import randint, random, uniform
+from collections.abc import Iterable, Callable
+from typing import Union, NewType, Literal, Any
 from dramkit.logtools.utils_logger import logger_show
 from dramkit.speedup.multi_thread import SingleThread
 
 from beartype import beartype as checkin
+from beartype.typing import List
 
 
 PYTHON_VERSION = float(sys.version[:3])
 
 
 class TimeRecoder(object):
     '''
@@ -2109,20 +2113,34 @@
 
 
 def copy_df_structure(df):
     '''复制df的结构到一个空的dataframe'''
     return df.drop(df.index)
 
 
+def get_tmp_new(exists, tmp_new, ext='_'):
+    '''以tmp_new为基础生成一个不在exists的值'''
+    assert isinstance(exists, Iterable)
+    assert isinstance(ext, (str, Callable))
+    if isinstance(ext, str) and isinstance(tmp_new, str):
+        while tmp_new in exists:
+            tmp_new += ext
+        return tmp_new
+    while tmp_new in exists:
+        tmp_new = ext(tmp_new)
+    return tmp_new
+    
+
 def get_tmp_col(df, tmp_col_name):
     '''以tmp_col_name为基础生成一个不在df的列名中的列'''
     assert isinstance(tmp_col_name, str)
-    while tmp_col_name in df.columns:
-        tmp_col_name += '_'
-    return tmp_col_name
+    return get_tmp_new(df.columns, tmp_col_name, ext='_')
+    # while tmp_col_name in df.columns:
+    #     tmp_col_name += '_'
+    # return tmp_col_name
 
 
 def merge_df(df_left, df_right, same_keep='left', **kwargs):
     '''
     在 ``pd.merge`` 上改进，相同列名时自动去除重复的
 
     Parameters
@@ -2747,55 +2765,170 @@
     df = df.stack(dropna=dropna)
     df = pd.DataFrame(df, columns=[col_val_name])
     df.index.names = idx_cols + [col_name]
     df = df.reset_index()
     return df
 
 
-def df_freq_low2high(df, tcol, idcols, vcols=None,
-                     tmin=None, tmax=None, keepna=True):
+FullMethodType = NewType('FullMethodType',
+                         Literal['product', 'pivot'])
+FillMethodType = NewType('FillMethodType',
+                         Literal['ffill', 'bfill',
+                                 'ffillbfill', 'bfillffill'])
+
+@checkin
+def get_full_df(df: pd.DataFrame,
+                full_col : str,
+                fulls: Iterable,
+                idcols: Union[str, List[str], None] = None,
+                vcols: Union[str, List[str], None] = None,
+                val_nan: Any = None,
+                fill: Union[FillMethodType, None] = 'ffill',
+                final_dropna: bool = True,
+                only_fulls: bool = True,
+                method: FullMethodType = 'pivot'):
     '''
-    数据填充为日频
+    df中full_col列的值扩充到fulls
     
-    TODO
-    ----
-    - idcols唯一性检查
-    - 填充时选择交易日或工作日参数设置
-    - idx_cols中有nan时检查和处理
-    - 其他参数/变量规范重写
-    - 日期格式不写死，根据tcol列转化
-    - 日期生成函数自定义，比如可以日频、月频、小时频率等
-    '''
-    vcols = check_list_arg(vcols, allow_none=True)
-    idcols = check_list_arg(idcols)
-    if isnull(vcols):
-        vcols = [x for x in df.columns if not x in idcols+[tcol]]
+    Example
+    -------
+    >>> df = pd.DataFrame({'t': [2, 3, 5, 7, 9],
+    ...                    'a': ['x1', 'x1', 'x3', 'x4', 'x4'],
+    ...                    'b': ['y1', 'y2', 'y3', 'y4', 'y4'],
+    ...                    'c': ['z1', 'z1', 'z5', 'z7', 'z9']})
+    >>> get_full_df(df, 't', range(1, 11))
+    >>> get_full_df(df, 't', range(1, 11), idcols='c', method='product')
+    >>> get_full_df(df, 't', range(1, 11), idcols=['a', 'b'], method='product')
+    >>> get_full_df(df, 't', range(1, 11), idcols=['a', 'b'])
+    >>> df['c'] = ['z1', 'z1', np.nan, np.nan, 'z9']
+    >>> get_full_df(df, 't', range(1, 11), idcols=['a', 'b'], val_nan='npnan')
+    >>> get_full_df(df, 't', [2, 5, 9, 10], idcols=['a', 'b'], val_nan='npnan', final_dropna=False)
+    >>> get_full_df(df, 't', [2, 5, 9, 10], idcols=['a', 'b'], val_nan='npnan', final_dropna=True, method='product')
+    '''
     if df.shape[0] == 0:
-        return pd.DataFrame(columns=[tcol]+idcols+vcols)
-    if isnull(tmin):
-        tmin = df[tcol].min()
-    if isnull(tmax):
-        # tmax = datetime.datetime.today().strftime('%Y%m%d')
-        tmax = df[tcol].max()
-    if tmin == tmax:
-        return df[[tcol]+idcols+vcols]
-    dates = pd.date_range(tmin, tmax)
-    dates = [x.strftime('%Y%m%d') for x in dates]
-    if keepna:
-        df = df.fillna('__tmp_None_tmp__')
-    df = df.pivot_table(values=vcols, index=tcol, columns=idcols,
-                        aggfunc=lambda x: x)
-    index_all = list(set(dates + list(df.index)))
-    index_all.sort()
-    df = df.reindex(index=index_all)
-    df = df.fillna(method='ffill')#.fillna(method='bfill')
-    df = df.stack(level=idcols).reset_index()
-    df = df.replace({'__tmp_None_tmp__': np.nan})
-    df = df.sort_values(idcols+[tcol])
-    return df
+        return df
+    idcols = check_list_arg(idcols, allow_none=True)
+    if isnull(idcols):
+        vcols = check_list_arg(vcols, allow_none=True)
+        if isnull(vcols):
+            vcols = [x for x in df.columns if not x != full_col]
+        res = pd.DataFrame({full_col: fulls})
+        res = pd.merge(res, df, how='left', on=full_col)
+        res = res.sort_values(full_col)
+        if fill in ['ffill', 'bfill']:
+            res = res.fillna(method=fill)
+        elif fill == 'ffillbfill':
+            res = res.fillna(method='ffill').fillna(method='bfill')
+        elif fill == 'bfillffill':
+            res = res.fillna(method='bfill').fillna(method='ffill')
+        if final_dropna:
+            res = res.dropna()
+    else:
+        # 受影响的列
+        vcols = check_list_arg(vcols, allow_none=True)
+        if isnull(vcols):
+            vcols = [x for x in df.columns if not x in idcols+[full_col]]
+        res = df[[full_col]+idcols+vcols].copy()
+        if not isnull(val_nan):
+            for c in vcols:
+                res[c] = res[c].fillna(val_nan)
+        oncols = [full_col]+idcols
+        assert res[oncols].isna().sum().sum() == 0
+        if method == 'product':
+            full = pd.DataFrame(
+                   product(fulls, *(res[c].unique() for c in idcols)),
+                   columns=oncols)
+            res = pd.merge(full, res, how='left', on=oncols)
+            res = res.sort_values(oncols)
+            if fill in ['ffill', 'bfill']:
+                res = res.groupby(idcols, as_index=False, group_keys=False).apply(
+                      lambda x: x.fillna(method=fill))
+            elif fill == 'ffillbfill':
+                res = res.groupby(idcols, as_index=False, group_keys=False).apply(
+                      lambda x: x.fillna(method='ffill').fillna(method='bfill'))
+            elif fill == 'bfillffill':
+                res = res.groupby(idcols, as_index=False, group_keys=False).apply(
+                      lambda x: x.fillna(method='bfill').fillna(method='ffill'))
+            if final_dropna:
+                res = res.dropna(subset=vcols, how='all')
+        elif method == 'pivot':
+            res = res.pivot_table(values=vcols, index=full_col,
+                                  columns=idcols, aggfunc=lambda x: x)
+            index_all = list(set(list(fulls) + list(res.index)))
+            index_all.sort()
+            res = res.reindex(index=index_all)
+            if fill in ['ffill', 'bfill']:
+                res = res.fillna(method=fill)
+            elif fill == 'ffillbfill':
+                res = res.fillna(method='ffill').fillna(method='bfill')
+            elif fill == 'bfillffill':
+                res = res.fillna(method='bfill').fillna(method='ffill')
+            res = res.stack(level=idcols, dropna=final_dropna).reset_index()
+    if only_fulls:
+        res = res[res[full_col].isin(list(fulls))]
+    res = res.reset_index(drop=True)
+    return res
+
+
+DateTimeType = NewType('DateTimeType',
+                       Union[str,
+                             datetime.datetime,
+                             datetime.date]
+                       )
+
+
+# @checkin
+def get_full_components_df(df: pd.DataFrame,
+                           parent_col: str,
+                           child_col: str,
+                           tincol: str,
+                           toutcol: str,
+                           tfulls: Iterable,
+                           toutnan: DateTimeType,
+                           tcol_res: str = 'time',
+                           keep_inout: bool = False
+                           ):
+    '''
+    | 根据纳入、退出日期获取在给定时间内的所有成分
+    
+    Example
+    -------
+    >>> df = pd.DataFrame(
+    ...      {'idxname': ['a', 'a', 'b', 'b', 'a', 'c', 'c'],
+    ...       'stock': ['a1', 'a2', 'b1', 'b2', 'a3', 'c1', 'c2'],
+    ...       'indate': ['20210101', '20210515', '20210405', '20210206',
+    ...                  '20220307', '20220910', '20230409'],
+    ...       'outdate': ['20220305', np.nan, np.nan, '20230209',
+    ...                   np.nan, np.nan, '20230518']})
+    >>> parent_col, child_col, tincol, toutcol = 'idxname', 'stock', 'indate', 'outdate'
+    >>> from finfactory.fintools.utils_chn import get_dates_conds
+    >>> tfulls = get_dates_conds('quarter_end', '20210101')
+    >>> tfulls = [x.strftime('%Y%m%d') for x in tfulls]
+    >>> toutnan = '20991231'
+    >>> df1 = get_full_components_df(
+    ...       df, parent_col, child_col, tincol, toutcol,
+    ...       tfulls, toutnan, tcol_res='time')
+    '''
+    df = df[[parent_col, child_col, tincol, toutcol]].copy()
+    df[toutcol] = df[toutcol].fillna(toutnan)
+    tmp = df.to_dict(orient='split')['data']
+    tmp = [tuple(x) for x in tmp]
+    df = pd.DataFrame(np.ones((len(tfulls), len(tmp))), index=tfulls)
+    df.index.name = tcol_res
+    df.columns = tmp
+    df = df.reset_index()
+    df = df_cols2rows(df, tmp, 'tmp', 'IsIn')
+    df[[parent_col, child_col, tincol, toutcol]] = df['tmp'].apply(pd.Series)
+    df = df[(df[tincol] <= df[tcol_res]) & (df[toutcol]>= df[tcol_res])]
+    if keep_inout:
+        df = df[[parent_col, child_col, tcol_res, tincol, toutcol]]
+    else:
+        df = df[[parent_col, child_col, tcol_res]]
+    df = df.sort_values([parent_col, tcol_res, child_col])
+    return df.reset_index(drop=True)
 
 
 def get_first_appear(series, func_cond,
                      reverse=False,
                      return_iloc=False):
     '''
     | 获取满足func_cond(x)为True的值在series中第一次出现时的索引
```

### Comparing `dramkit-0.5.41/dramkit/install_check.py` & `dramkit-0.5.42/dramkit/install_check.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/iotools.py` & `dramkit-0.5.42/dramkit/iotools.py`

 * *Files 1% similar despite different names*

```diff
@@ -1940,15 +1940,18 @@
 def get_file_ext_type(fpath):
     '''提取文件扩展名'''
     return os.path.splitext(fpath)[-1]
 
 
 def get_parent_path(path, n=1):
     '''获取路径path的n级父路径'''
-    f = Path(os.path.abspath(path))
+    if (not os.path.isabs(path)) and (not path.startswith('./')):
+        f = Path(os.path.abspath(path))
+    else:
+        f = Path(path)
     res = eval('f'+'.parent'*n)
     res = str(res).replace('\\', '/') + '/'
     # TODO: path以'./'开头时，得到的res不是以'./'开头，原因待查
     if path.startswith('./') and not res.startswith('./'):
         res = './' + res
     return res
```

### Comparing `dramkit-0.5.41/dramkit/logtools/logger_general.py` & `dramkit-0.5.42/dramkit/logtools/logger_general.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/logtools/logger_rotating.py` & `dramkit-0.5.42/dramkit/logtools/logger_rotating.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/logtools/logger_timedrotating.py` & `dramkit-0.5.42/dramkit/logtools/logger_timedrotating.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/logtools/utils_logger.py` & `dramkit-0.5.42/dramkit/logtools/utils_logger.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/openai/aiedu_chat.py` & `dramkit-0.5.42/dramkit/openai/aiedu_chat.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/openai/openai_chat.py` & `dramkit-0.5.42/dramkit/openai/openai_chat.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/openai/openai_chat_hs.py` & `dramkit-0.5.42/dramkit/openai/openai_chat_hs.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/optimizer/alo.py` & `dramkit-0.5.42/dramkit/optimizer/alo.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/optimizer/base_funcs.py` & `dramkit-0.5.42/dramkit/optimizer/base_funcs.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/optimizer/boa.py` & `dramkit-0.5.42/dramkit/optimizer/boa.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/optimizer/cs.py` & `dramkit-0.5.42/dramkit/optimizer/cs.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/optimizer/ga.py` & `dramkit-0.5.42/dramkit/optimizer/ga.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/optimizer/gwo.py` & `dramkit-0.5.42/dramkit/optimizer/gwo.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/optimizer/hcpsoboa.py` & `dramkit-0.5.42/dramkit/optimizer/hcpsoboa.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/optimizer/hho.py` & `dramkit-0.5.42/dramkit/optimizer/hho.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/optimizer/hpsoboa.py` & `dramkit-0.5.42/dramkit/optimizer/hpsoboa.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/optimizer/pso.py` & `dramkit-0.5.42/dramkit/optimizer/pso.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/optimizer/utils_heuristic.py` & `dramkit-0.5.42/dramkit/optimizer/utils_heuristic.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/optimizer/woa.py` & `dramkit-0.5.42/dramkit/optimizer/woa.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/other/_Linux_notes.py` & `dramkit-0.5.42/dramkit/other/_Linux_notes.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/other/_Python_notes.py` & `dramkit-0.5.42/dramkit/other/_Python_notes.py`

 * *Files 18% similar despite different names*

```diff
@@ -84,8 +84,11 @@
 
 # pip安装忽略依赖
 --no-dependencies
  
 # pip强制重新安装所有软件包，即使它们已经是最新的
 --force-reinstall
 
+# pip批量安装文件夹下所有的whl包
+pip install /dirpath/*.whl
+
 # '''
```

### Comparing `dramkit-0.5.41/dramkit/other/_Vim_notes.py` & `dramkit-0.5.42/dramkit/other/_Vim_notes.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/other/langconv.py` & `dramkit-0.5.42/dramkit/other/langconv.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/other/othertools.py` & `dramkit-0.5.42/dramkit/other/othertools.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/other/replace_endblank.py` & `dramkit-0.5.42/dramkit/other/replace_endblank.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/other/zh_wiki.py` & `dramkit-0.5.42/dramkit/other/zh_wiki.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/plottools/plot_barline.py` & `dramkit-0.5.42/dramkit/plottools/plot_barline.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/plottools/plot_common.py` & `dramkit-0.5.42/dramkit/plottools/plot_common.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/plottools/plot_histdist.py` & `dramkit-0.5.42/dramkit/plottools/plot_histdist.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/plottools/plot_scatter.py` & `dramkit-0.5.42/dramkit/plottools/plot_scatter.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/plottools/utils_plot.py` & `dramkit-0.5.42/dramkit/plottools/utils_plot.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/pystyles/dramkit_style.py` & `dramkit-0.5.42/dramkit/pystyles/dramkit_style.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/sorts/bubble_sort.py` & `dramkit-0.5.42/dramkit/sorts/bubble_sort.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/sorts/bucket_sort.py` & `dramkit-0.5.42/dramkit/sorts/bucket_sort.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/sorts/insert_sort.py` & `dramkit-0.5.42/dramkit/sorts/insert_sort.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/sorts/insert_sort_bin.py` & `dramkit-0.5.42/dramkit/sorts/insert_sort_bin.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/sorts/quick_sort.py` & `dramkit-0.5.42/dramkit/sorts/quick_sort.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/speedup/_mp_test1.py` & `dramkit-0.5.42/dramkit/speedup/_mp_test1.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/speedup/_mp_test2.py` & `dramkit-0.5.42/dramkit/speedup/_mp_test2.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/speedup/_mp_test3.py` & `dramkit-0.5.42/dramkit/speedup/_mp_test3.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/speedup/iotools_tmp.py` & `dramkit-0.5.42/dramkit/speedup/iotools_tmp.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/speedup/multi_process_concurrent.py` & `dramkit-0.5.42/dramkit/speedup/multi_process_concurrent.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/speedup/multi_thread.py` & `dramkit-0.5.42/dramkit/speedup/multi_thread.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/sqltools/_Hive_notes.py` & `dramkit-0.5.42/dramkit/sqltools/_Hive_notes.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/sqltools/_MySQL_notes.py` & `dramkit-0.5.42/dramkit/sqltools/_MySQL_notes.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/sqltools/_Oracle_notes.py` & `dramkit-0.5.42/dramkit/sqltools/_Oracle_notes.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/sqltools/cxoracle.py` & `dramkit-0.5.42/dramkit/sqltools/cxoracle.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/sqltools/py_hive.py` & `dramkit-0.5.42/dramkit/sqltools/py_hive.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/sqltools/py_mysql.py` & `dramkit-0.5.42/dramkit/sqltools/py_mysql.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/sqltools/sql_alchemy.py` & `dramkit-0.5.42/dramkit/sqltools/sql_alchemy.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/webtools/utils_html.py` & `dramkit-0.5.42/dramkit/webtools/utils_html.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit/wechat/qywechat.py` & `dramkit-0.5.42/dramkit/wechat/qywechat.py`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/dramkit.egg-info/PKG-INFO` & `dramkit-0.5.42/dramkit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dramkit
-Version: 0.5.41
+Version: 0.5.42
 Summary: DramKit is a toolbox.
 Home-page: https://github.com/Genlovy-Hoo/dramkit/
 Author: Genlovy Hoo, YueYong Hu
 Author-email: genlovhyy@163.com
 License: MIT
 Platform: any
 Description-Content-Type: text/markdown
```

### Comparing `dramkit-0.5.41/dramkit.egg-info/SOURCES.txt` & `dramkit-0.5.42/dramkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dramkit-0.5.41/setup.py` & `dramkit-0.5.42/setup.py`

 * *Files identical despite different names*

