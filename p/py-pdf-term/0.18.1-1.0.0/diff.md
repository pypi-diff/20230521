# Comparing `tmp/py-pdf-term-0.18.1.tar.gz` & `tmp/py_pdf_term-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-pdf-term-0.18.1.tar", max compression
+gzip compressed data, was "py_pdf_term-1.0.0.tar", max compression
```

## Comparing `py-pdf-term-0.18.1.tar` & `py_pdf_term-1.0.0.tar`

### file list

```diff
@@ -1,186 +1,188 @@
--rw-r--r--   0        0        0     1065 2021-08-01 13:41:41.018921 py-pdf-term-0.18.1/LICENSE
--rw-r--r--   0        0        0      558 2021-12-23 09:14:20.699259 py-pdf-term-0.18.1/README.md
--rw-r--r--   0        0        0      198 2022-03-09 08:58:21.283602 py-pdf-term-0.18.1/py_pdf_term/__init__.py
--rw-r--r--   0        0        0        0 2021-07-17 01:56:39.528684 py-pdf-term-0.18.1/py_pdf_term/_common/__init__.py
--rw-r--r--   0        0        0     2415 2021-12-23 08:48:45.044349 py-pdf-term-0.18.1/py_pdf_term/_common/consts.py
--rw-r--r--   0        0        0     1927 2022-01-28 14:27:59.214216 py-pdf-term-0.18.1/py_pdf_term/_common/data.py
--rw-r--r--   0        0        0      756 2021-07-17 01:56:39.530258 py-pdf-term-0.18.1/py_pdf_term/_common/extended_math.py
--rw-r--r--   0        0        0       72 2021-10-27 15:05:43.326137 py-pdf-term-0.18.1/py_pdf_term/analysis/__init__.py
--rw-r--r--   0        0        0      442 2022-01-28 14:27:59.215385 py-pdf-term-0.18.1/py_pdf_term/analysis/_analysis/__init__.py
--rw-r--r--   0        0        0      168 2021-10-27 15:17:22.072592 py-pdf-term-0.18.1/py_pdf_term/analysis/_analysis/concats/__init__.py
--rw-r--r--   0        0        0     3286 2022-03-09 08:26:28.188562 py-pdf-term-0.18.1/py_pdf_term/analysis/_analysis/concats/lr.py
--rw-r--r--   0        0        0      151 2021-10-27 15:17:22.073536 py-pdf-term-0.18.1/py_pdf_term/analysis/_analysis/cooccurrences/__init__.py
--rw-r--r--   0        0        0     2485 2021-10-27 15:17:22.074088 py-pdf-term-0.18.1/py_pdf_term/analysis/_analysis/cooccurrences/container.py
--rw-r--r--   0        0        0      146 2022-01-28 14:27:59.216328 py-pdf-term-0.18.1/py_pdf_term/analysis/_analysis/occurrences/__init__.py
--rw-r--r--   0        0        0     2753 2021-10-27 14:58:53.697234 py-pdf-term-0.18.1/py_pdf_term/analysis/_analysis/occurrences/term.py
--rw-r--r--   0        0        0     2212 2021-10-27 15:17:22.075089 py-pdf-term-0.18.1/py_pdf_term/analysis/_analysis/runner.py
--rw-r--r--   0        0        0       76 2021-10-27 15:05:43.333785 py-pdf-term-0.18.1/py_pdf_term/candidates/__init__.py
--rw-r--r--   0        0        0      287 2021-10-27 15:17:22.075460 py-pdf-term-0.18.1/py_pdf_term/candidates/_candidates/__init__.py
--rw-r--r--   0        0        0      315 2022-03-09 08:26:28.189353 py-pdf-term-0.18.1/py_pdf_term/candidates/_candidates/augmenters/__init__.py
--rw-r--r--   0        0        0      338 2021-10-27 14:58:53.699304 py-pdf-term-0.18.1/py_pdf_term/candidates/_candidates/augmenters/base.py
--rw-r--r--   0        0        0      795 2022-03-09 08:26:28.190217 py-pdf-term-0.18.1/py_pdf_term/candidates/_candidates/augmenters/combiner.py
--rw-r--r--   0        0        0     1875 2022-03-09 08:26:28.191267 py-pdf-term-0.18.1/py_pdf_term/candidates/_candidates/augmenters/separation.py
--rw-r--r--   0        0        0      315 2022-03-09 08:26:28.191751 py-pdf-term-0.18.1/py_pdf_term/candidates/_candidates/classifiers/__init__.py
--rw-r--r--   0        0        0     1118 2022-03-09 08:26:28.192170 py-pdf-term-0.18.1/py_pdf_term/candidates/_candidates/classifiers/base.py
--rw-r--r--   0        0        0      533 2022-03-09 08:26:28.192676 py-pdf-term-0.18.1/py_pdf_term/candidates/_candidates/classifiers/english.py
--rw-r--r--   0        0        0      569 2022-03-09 08:26:28.193499 py-pdf-term-0.18.1/py_pdf_term/candidates/_candidates/classifiers/japanese.py
--rw-r--r--   0        0        0      871 2022-03-09 08:26:28.193989 py-pdf-term-0.18.1/py_pdf_term/candidates/_candidates/classifiers/marker.py
--rw-r--r--   0        0        0     3821 2021-10-27 15:17:22.078647 py-pdf-term-0.18.1/py_pdf_term/candidates/_candidates/data.py
--rw-r--r--   0        0        0     6005 2022-03-09 08:26:28.194680 py-pdf-term-0.18.1/py_pdf_term/candidates/_candidates/extractor.py
--rw-r--r--   0        0        0      835 2021-10-27 15:17:22.079350 py-pdf-term-0.18.1/py_pdf_term/candidates/_candidates/filters/__init__.py
--rw-r--r--   0        0        0     2081 2021-10-27 15:17:22.079682 py-pdf-term-0.18.1/py_pdf_term/candidates/_candidates/filters/combiner.py
--rw-r--r--   0        0        0      657 2021-10-27 15:17:22.080030 py-pdf-term-0.18.1/py_pdf_term/candidates/_candidates/filters/term/__init__.py
--rw-r--r--   0        0        0     1096 2021-10-27 14:58:53.704568 py-pdf-term-0.18.1/py_pdf_term/candidates/_candidates/filters/term/base.py
--rw-r--r--   0        0        0      192 2021-10-27 15:17:22.080367 py-pdf-term-0.18.1/py_pdf_term/candidates/_candidates/filters/term/concatenation/__init__.py
--rw-r--r--   0        0        0     3664 2022-03-09 08:26:28.195381 py-pdf-term-0.18.1/py_pdf_term/candidates/_candidates/filters/term/concatenation/english.py
--rw-r--r--   0        0        0     5360 2022-03-09 08:26:28.196046 py-pdf-term-0.18.1/py_pdf_term/candidates/_candidates/filters/term/concatenation/japanese.py
--rw-r--r--   0        0        0      168 2021-10-27 15:17:22.082765 py-pdf-term-0.18.1/py_pdf_term/candidates/_candidates/filters/term/numeric/__init__.py
--rw-r--r--   0        0        0      717 2022-03-09 08:26:28.196717 py-pdf-term-0.18.1/py_pdf_term/candidates/_candidates/filters/term/numeric/english.py
--rw-r--r--   0        0        0     1095 2022-03-09 08:26:28.197369 py-pdf-term-0.18.1/py_pdf_term/candidates/_candidates/filters/term/numeric/japanese.py
--rw-r--r--   0        0        0      180 2021-10-27 15:17:22.084044 py-pdf-term-0.18.1/py_pdf_term/candidates/_candidates/filters/term/propernoun/__init__.py
--rw-r--r--   0        0        0      279 2021-10-27 14:58:53.708617 py-pdf-term-0.18.1/py_pdf_term/candidates/_candidates/filters/term/propernoun/english.py
--rw-r--r--   0        0        0     1009 2022-03-09 08:26:28.197845 py-pdf-term-0.18.1/py_pdf_term/candidates/_candidates/filters/term/propernoun/japanese.py
--rw-r--r--   0        0        0      180 2021-10-27 15:17:22.089092 py-pdf-term-0.18.1/py_pdf_term/candidates/_candidates/filters/term/symbollike/__init__.py
--rw-r--r--   0        0        0     2213 2022-03-09 08:26:28.198202 py-pdf-term-0.18.1/py_pdf_term/candidates/_candidates/filters/term/symbollike/english.py
--rw-r--r--   0        0        0     2315 2022-03-09 08:26:28.198536 py-pdf-term-0.18.1/py_pdf_term/candidates/_candidates/filters/term/symbollike/japanese.py
--rw-r--r--   0        0        0      231 2021-10-27 15:17:22.091318 py-pdf-term-0.18.1/py_pdf_term/candidates/_candidates/filters/token/__init__.py
--rw-r--r--   0        0        0      524 2022-03-09 03:25:01.666413 py-pdf-term-0.18.1/py_pdf_term/candidates/_candidates/filters/token/base.py
--rw-r--r--   0        0        0     1705 2022-03-09 03:35:47.856735 py-pdf-term-0.18.1/py_pdf_term/candidates/_candidates/filters/token/english.py
--rw-r--r--   0        0        0     2839 2022-03-09 08:26:28.199158 py-pdf-term-0.18.1/py_pdf_term/candidates/_candidates/filters/token/japanese.py
--rw-r--r--   0        0        0      254 2021-10-27 15:17:22.094118 py-pdf-term-0.18.1/py_pdf_term/candidates/_candidates/splitters/__init__.py
--rw-r--r--   0        0        0      699 2022-03-09 08:26:28.200008 py-pdf-term-0.18.1/py_pdf_term/candidates/_candidates/splitters/base.py
--rw-r--r--   0        0        0      687 2021-10-27 14:58:53.713658 py-pdf-term-0.18.1/py_pdf_term/candidates/_candidates/splitters/combiner.py
--rw-r--r--   0        0        0     2570 2022-03-09 08:26:28.200813 py-pdf-term-0.18.1/py_pdf_term/candidates/_candidates/splitters/repeat.py
--rw-r--r--   0        0        0     1020 2022-03-09 08:26:28.201590 py-pdf-term-0.18.1/py_pdf_term/candidates/_candidates/splitters/symname.py
--rw-r--r--   0        0        0     1579 2021-07-17 01:56:39.543825 py-pdf-term-0.18.1/py_pdf_term/candidates/_candidates/utils.py
--rw-r--r--   0        0        0       98 2021-10-27 15:05:43.345770 py-pdf-term-0.18.1/py_pdf_term/candidates/augmenters.py
--rw-r--r--   0        0        0      100 2022-03-09 08:26:28.202274 py-pdf-term-0.18.1/py_pdf_term/candidates/classifiers.py
--rw-r--r--   0        0        0       92 2021-10-27 15:05:43.346505 py-pdf-term-0.18.1/py_pdf_term/candidates/filters.py
--rw-r--r--   0        0        0       96 2021-10-27 15:05:43.346958 py-pdf-term-0.18.1/py_pdf_term/candidates/splitters.py
--rw-r--r--   0        0        0      336 2022-03-09 08:11:28.633222 py-pdf-term-0.18.1/py_pdf_term/configs.py
--rw-r--r--   0        0        0       72 2021-10-27 15:05:43.347969 py-pdf-term-0.18.1/py_pdf_term/endtoend/__init__.py
--rw-r--r--   0        0        0      226 2022-03-09 08:11:28.633599 py-pdf-term-0.18.1/py_pdf_term/endtoend/_endtoend/__init__.py
--rw-r--r--   0        0        0     1024 2021-10-27 15:17:22.101742 py-pdf-term-0.18.1/py_pdf_term/endtoend/_endtoend/caches/__init__.py
--rw-r--r--   0        0        0      254 2021-10-27 15:17:22.103054 py-pdf-term-0.18.1/py_pdf_term/endtoend/_endtoend/caches/candidate/__init__.py
--rw-r--r--   0        0        0      857 2021-10-27 14:58:53.723764 py-pdf-term-0.18.1/py_pdf_term/endtoend/_endtoend/caches/candidate/base.py
--rw-r--r--   0        0        0     2213 2021-10-27 14:58:53.725799 py-pdf-term-0.18.1/py_pdf_term/endtoend/_endtoend/caches/candidate/file.py
--rw-r--r--   0        0        0      626 2021-10-27 14:58:53.726309 py-pdf-term-0.18.1/py_pdf_term/endtoend/_endtoend/caches/candidate/nocache.py
--rw-r--r--   0        0        0      184 2021-07-17 01:56:39.546898 py-pdf-term-0.18.1/py_pdf_term/endtoend/_endtoend/caches/consts.py
--rw-r--r--   0        0        0      448 2021-10-27 15:17:22.104558 py-pdf-term-0.18.1/py_pdf_term/endtoend/_endtoend/caches/method/__init__.py
--rw-r--r--   0        0        0     1844 2022-03-09 08:11:28.637867 py-pdf-term-0.18.1/py_pdf_term/endtoend/_endtoend/caches/method/base.py
--rw-r--r--   0        0        0     4397 2022-03-09 08:11:28.638692 py-pdf-term-0.18.1/py_pdf_term/endtoend/_endtoend/caches/method/file.py
--rw-r--r--   0        0        0     1397 2022-03-09 08:11:28.640200 py-pdf-term-0.18.1/py_pdf_term/endtoend/_endtoend/caches/method/nocache.py
--rw-r--r--   0        0        0      227 2021-10-27 15:17:22.104951 py-pdf-term-0.18.1/py_pdf_term/endtoend/_endtoend/caches/styling/__init__.py
--rw-r--r--   0        0        0      846 2021-10-27 14:58:53.732304 py-pdf-term-0.18.1/py_pdf_term/endtoend/_endtoend/caches/styling/base.py
--rw-r--r--   0        0        0     2205 2021-10-27 14:58:53.732680 py-pdf-term-0.18.1/py_pdf_term/endtoend/_endtoend/caches/styling/file.py
--rw-r--r--   0        0        0      611 2021-10-27 14:58:53.733094 py-pdf-term-0.18.1/py_pdf_term/endtoend/_endtoend/caches/styling/nocache.py
--rw-r--r--   0        0        0      702 2021-07-17 01:56:39.549058 py-pdf-term-0.18.1/py_pdf_term/endtoend/_endtoend/caches/util.py
--rw-r--r--   0        0        0      203 2021-10-27 15:17:22.105345 py-pdf-term-0.18.1/py_pdf_term/endtoend/_endtoend/caches/xml/__init__.py
--rw-r--r--   0        0        0      790 2021-10-27 14:58:53.733724 py-pdf-term-0.18.1/py_pdf_term/endtoend/_endtoend/caches/xml/base.py
--rw-r--r--   0        0        0     2173 2021-10-27 14:58:53.734051 py-pdf-term-0.18.1/py_pdf_term/endtoend/_endtoend/caches/xml/file.py
--rw-r--r--   0        0        0      547 2021-10-27 14:58:53.734349 py-pdf-term-0.18.1/py_pdf_term/endtoend/_endtoend/caches/xml/nocache.py
--rw-r--r--   0        0        0      427 2022-03-09 08:11:28.641166 py-pdf-term-0.18.1/py_pdf_term/endtoend/_endtoend/configs/__init__.py
--rw-r--r--   0        0        0      670 2021-10-27 14:58:53.734925 py-pdf-term-0.18.1/py_pdf_term/endtoend/_endtoend/configs/base.py
--rw-r--r--   0        0        0     1650 2022-03-09 08:26:28.203169 py-pdf-term-0.18.1/py_pdf_term/endtoend/_endtoend/configs/candidate.py
--rw-r--r--   0        0        0      442 2022-03-09 08:11:28.641870 py-pdf-term-0.18.1/py_pdf_term/endtoend/_endtoend/configs/method.py
--rw-r--r--   0        0        0      390 2021-07-17 01:56:39.550790 py-pdf-term-0.18.1/py_pdf_term/endtoend/_endtoend/configs/styling.py
--rw-r--r--   0        0        0      206 2021-07-17 01:56:39.550976 py-pdf-term-0.18.1/py_pdf_term/endtoend/_endtoend/configs/techterm.py
--rw-r--r--   0        0        0      355 2021-08-02 12:51:58.472973 py-pdf-term-0.18.1/py_pdf_term/endtoend/_endtoend/configs/xml.py
--rw-r--r--   0        0        0      146 2021-07-17 01:56:39.551370 py-pdf-term-0.18.1/py_pdf_term/endtoend/_endtoend/data.py
--rw-r--r--   0        0        0    11177 2022-03-09 08:57:41.611961 py-pdf-term-0.18.1/py_pdf_term/endtoend/_endtoend/extractor.py
--rw-r--r--   0        0        0      310 2022-03-09 08:11:28.643261 py-pdf-term-0.18.1/py_pdf_term/endtoend/_endtoend/layers/__init__.py
--rw-r--r--   0        0        0     3975 2022-03-09 08:26:28.205768 py-pdf-term-0.18.1/py_pdf_term/endtoend/_endtoend/layers/candidate.py
--rw-r--r--   0        0        0     6637 2022-03-09 08:26:28.206619 py-pdf-term-0.18.1/py_pdf_term/endtoend/_endtoend/layers/method.py
--rw-r--r--   0        0        0     1785 2021-10-27 14:58:53.737811 py-pdf-term-0.18.1/py_pdf_term/endtoend/_endtoend/layers/styling.py
--rw-r--r--   0        0        0     1636 2022-03-09 08:11:28.645248 py-pdf-term-0.18.1/py_pdf_term/endtoend/_endtoend/layers/techterm.py
--rw-r--r--   0        0        0     1666 2021-10-27 14:58:53.738508 py-pdf-term-0.18.1/py_pdf_term/endtoend/_endtoend/layers/xml.py
--rw-r--r--   0        0        0     1032 2022-03-09 08:26:28.207464 py-pdf-term-0.18.1/py_pdf_term/endtoend/_endtoend/mappers/__init__.py
--rw-r--r--   0        0        0     1079 2021-10-27 14:58:53.739143 py-pdf-term-0.18.1/py_pdf_term/endtoend/_endtoend/mappers/base.py
--rw-r--r--   0        0        0      407 2021-10-27 15:17:22.107924 py-pdf-term-0.18.1/py_pdf_term/endtoend/_endtoend/mappers/caches/__init__.py
--rw-r--r--   0        0        0      609 2021-10-27 14:58:53.740059 py-pdf-term-0.18.1/py_pdf_term/endtoend/_endtoend/mappers/caches/candidate.py
--rw-r--r--   0        0        0     1248 2021-10-27 14:58:53.740458 py-pdf-term-0.18.1/py_pdf_term/endtoend/_endtoend/mappers/caches/method.py
--rw-r--r--   0        0        0      576 2021-10-27 14:58:53.741192 py-pdf-term-0.18.1/py_pdf_term/endtoend/_endtoend/mappers/caches/styling.py
--rw-r--r--   0        0        0      544 2021-10-27 14:58:53.743375 py-pdf-term-0.18.1/py_pdf_term/endtoend/_endtoend/mappers/caches/xml.py
--rw-r--r--   0        0        0      448 2022-03-09 08:26:28.208387 py-pdf-term-0.18.1/py_pdf_term/endtoend/_endtoend/mappers/candidates/__init__.py
--rw-r--r--   0        0        0      709 2022-03-09 08:26:28.209192 py-pdf-term-0.18.1/py_pdf_term/endtoend/_endtoend/mappers/candidates/augmenter.py
--rw-r--r--   0        0        0      713 2022-03-09 08:26:28.209640 py-pdf-term-0.18.1/py_pdf_term/endtoend/_endtoend/mappers/candidates/classifier.py
--rw-r--r--   0        0        0     1590 2022-03-09 08:26:28.209912 py-pdf-term-0.18.1/py_pdf_term/endtoend/_endtoend/mappers/candidates/filter.py
--rw-r--r--   0        0        0      667 2022-03-09 08:26:28.210448 py-pdf-term-0.18.1/py_pdf_term/endtoend/_endtoend/mappers/candidates/lang.py
--rw-r--r--   0        0        0      580 2021-10-27 14:58:53.745600 py-pdf-term-0.18.1/py_pdf_term/endtoend/_endtoend/mappers/candidates/splitter.py
--rw-r--r--   0        0        0       29 2021-07-17 01:56:39.555562 py-pdf-term-0.18.1/py_pdf_term/endtoend/_endtoend/mappers/consts.py
--rw-r--r--   0        0        0      204 2021-10-27 15:17:22.110541 py-pdf-term-0.18.1/py_pdf_term/endtoend/_endtoend/mappers/methods/__init__.py
--rw-r--r--   0        0        0      608 2022-01-28 14:27:59.217641 py-pdf-term-0.18.1/py_pdf_term/endtoend/_endtoend/mappers/methods/multi.py
--rw-r--r--   0        0        0      691 2021-10-27 14:58:53.746570 py-pdf-term-0.18.1/py_pdf_term/endtoend/_endtoend/mappers/methods/single.py
--rw-r--r--   0        0        0       95 2021-10-27 15:17:22.110948 py-pdf-term-0.18.1/py_pdf_term/endtoend/_endtoend/mappers/pdftoxml/__init__.py
--rw-r--r--   0        0        0      335 2021-10-27 14:58:53.747258 py-pdf-term-0.18.1/py_pdf_term/endtoend/_endtoend/mappers/pdftoxml/openbin.py
--rw-r--r--   0        0        0       93 2021-10-27 15:17:22.111481 py-pdf-term-0.18.1/py_pdf_term/endtoend/_endtoend/mappers/stylings/__init__.py
--rw-r--r--   0        0        0      611 2021-10-27 14:58:53.748314 py-pdf-term-0.18.1/py_pdf_term/endtoend/_endtoend/mappers/stylings/score.py
--rw-r--r--   0        0        0       86 2021-10-27 15:05:43.358189 py-pdf-term-0.18.1/py_pdf_term/endtoend/caches.py
--rw-r--r--   0        0        0      978 2022-03-09 08:57:41.612962 py-pdf-term-0.18.1/py_pdf_term/mappers.py
--rw-r--r--   0        0        0       70 2021-10-27 15:05:43.359648 py-pdf-term-0.18.1/py_pdf_term/methods/__init__.py
--rw-r--r--   0        0        0      536 2022-01-28 14:27:59.218346 py-pdf-term-0.18.1/py_pdf_term/methods/_methods/__init__.py
--rw-r--r--   0        0        0     3290 2021-10-27 14:58:53.750273 py-pdf-term-0.18.1/py_pdf_term/methods/_methods/base.py
--rw-r--r--   0        0        0      567 2022-01-28 14:27:59.219068 py-pdf-term-0.18.1/py_pdf_term/methods/_methods/collectors/__init__.py
--rw-r--r--   0        0        0      468 2022-03-09 05:47:54.439135 py-pdf-term-0.18.1/py_pdf_term/methods/_methods/collectors/base.py
--rw-r--r--   0        0        0      881 2022-03-09 05:47:54.439737 py-pdf-term-0.18.1/py_pdf_term/methods/_methods/collectors/flr.py
--rw-r--r--   0        0        0      886 2022-03-09 05:47:54.440311 py-pdf-term-0.18.1/py_pdf_term/methods/_methods/collectors/flrh.py
--rw-r--r--   0        0        0      886 2022-03-09 05:47:54.440785 py-pdf-term-0.18.1/py_pdf_term/methods/_methods/collectors/hits.py
--rw-r--r--   0        0        0      886 2022-03-09 05:47:54.443668 py-pdf-term-0.18.1/py_pdf_term/methods/_methods/collectors/mcvalue.py
--rw-r--r--   0        0        0      621 2022-03-09 05:47:54.444910 py-pdf-term-0.18.1/py_pdf_term/methods/_methods/collectors/mdp.py
--rw-r--r--   0        0        0      771 2022-03-09 05:47:54.446225 py-pdf-term-0.18.1/py_pdf_term/methods/_methods/collectors/tfidf.py
--rw-r--r--   0        0        0      733 2021-10-27 14:58:53.753549 py-pdf-term-0.18.1/py_pdf_term/methods/_methods/data.py
--rw-r--r--   0        0        0      545 2022-03-09 05:47:54.446762 py-pdf-term-0.18.1/py_pdf_term/methods/_methods/flr.py
--rw-r--r--   0        0        0      639 2022-03-09 05:47:54.447162 py-pdf-term-0.18.1/py_pdf_term/methods/_methods/flrh.py
--rw-r--r--   0        0        0      639 2022-03-09 05:47:54.448219 py-pdf-term-0.18.1/py_pdf_term/methods/_methods/hits.py
--rw-r--r--   0        0        0      581 2022-03-09 05:47:54.448644 py-pdf-term-0.18.1/py_pdf_term/methods/_methods/mcvalue.py
--rw-r--r--   0        0        0      664 2022-03-09 05:47:54.449159 py-pdf-term-0.18.1/py_pdf_term/methods/_methods/mdp.py
--rw-r--r--   0        0        0      447 2022-01-28 14:27:59.219920 py-pdf-term-0.18.1/py_pdf_term/methods/_methods/rankers/__init__.py
--rw-r--r--   0        0        0      954 2022-03-09 05:47:54.450073 py-pdf-term-0.18.1/py_pdf_term/methods/_methods/rankers/base.py
--rw-r--r--   0        0        0     1947 2022-03-09 08:26:28.211226 py-pdf-term-0.18.1/py_pdf_term/methods/_methods/rankers/flr.py
--rw-r--r--   0        0        0     2384 2022-03-09 05:47:54.451087 py-pdf-term-0.18.1/py_pdf_term/methods/_methods/rankers/flrh.py
--rw-r--r--   0        0        0     5438 2022-03-09 08:26:28.212210 py-pdf-term-0.18.1/py_pdf_term/methods/_methods/rankers/hits.py
--rw-r--r--   0        0        0     1881 2022-03-09 05:47:54.453950 py-pdf-term-0.18.1/py_pdf_term/methods/_methods/rankers/mcvalue.py
--rw-r--r--   0        0        0     3081 2022-03-09 05:47:54.455185 py-pdf-term-0.18.1/py_pdf_term/methods/_methods/rankers/mdp.py
--rw-r--r--   0        0        0     3689 2022-03-09 05:47:54.455913 py-pdf-term-0.18.1/py_pdf_term/methods/_methods/rankers/tfidf.py
--rw-r--r--   0        0        0      473 2022-01-28 14:27:59.220746 py-pdf-term-0.18.1/py_pdf_term/methods/_methods/rankingdata/__init__.py
--rw-r--r--   0        0        0      412 2021-10-27 14:58:53.759986 py-pdf-term-0.18.1/py_pdf_term/methods/_methods/rankingdata/base.py
--rw-r--r--   0        0        0      726 2021-10-27 15:17:22.115474 py-pdf-term-0.18.1/py_pdf_term/methods/_methods/rankingdata/flr.py
--rw-r--r--   0        0        0      727 2021-10-27 15:17:22.115816 py-pdf-term-0.18.1/py_pdf_term/methods/_methods/rankingdata/flrh.py
--rw-r--r--   0        0        0      727 2021-10-27 15:17:22.116178 py-pdf-term-0.18.1/py_pdf_term/methods/_methods/rankingdata/hits.py
--rw-r--r--   0        0        0     1213 2021-10-27 14:58:53.760645 py-pdf-term-0.18.1/py_pdf_term/methods/_methods/rankingdata/mcvalue.py
--rw-r--r--   0        0        0      698 2021-07-17 01:56:39.564342 py-pdf-term-0.18.1/py_pdf_term/methods/_methods/rankingdata/mdp.py
--rw-r--r--   0        0        0      623 2021-07-17 01:56:39.564527 py-pdf-term-0.18.1/py_pdf_term/methods/_methods/rankingdata/tfidf.py
--rw-r--r--   0        0        0      638 2022-03-09 05:47:54.456953 py-pdf-term-0.18.1/py_pdf_term/methods/_methods/tfidf.py
--rw-r--r--   0        0        0       92 2021-10-27 15:05:43.364451 py-pdf-term-0.18.1/py_pdf_term/methods/collectors.py
--rw-r--r--   0        0        0       86 2021-10-27 15:05:43.365208 py-pdf-term-0.18.1/py_pdf_term/methods/rankers.py
--rw-r--r--   0        0        0       94 2021-10-27 15:05:43.365852 py-pdf-term-0.18.1/py_pdf_term/methods/rankingdata.py
--rw-r--r--   0        0        0       72 2021-10-27 15:05:43.366579 py-pdf-term-0.18.1/py_pdf_term/pdftoxml/__init__.py
--rw-r--r--   0        0        0      174 2021-12-23 08:24:39.299487 py-pdf-term-0.18.1/py_pdf_term/pdftoxml/_pdftoxml/__init__.py
--rw-r--r--   0        0        0     2346 2021-10-27 14:58:53.761881 py-pdf-term-0.18.1/py_pdf_term/pdftoxml/_pdftoxml/converter.py
--rw-r--r--   0        0        0      819 2021-11-02 11:49:54.509685 py-pdf-term-0.18.1/py_pdf_term/pdftoxml/_pdftoxml/data.py
--rw-r--r--   0        0        0     5417 2021-12-23 08:48:45.045128 py-pdf-term-0.18.1/py_pdf_term/pdftoxml/_pdftoxml/textful.py
--rw-r--r--   0        0        0      871 2021-12-23 08:24:58.272396 py-pdf-term-0.18.1/py_pdf_term/pdftoxml/_pdftoxml/utils.py
--rw-r--r--   0        0        0       72 2021-10-27 15:05:43.369229 py-pdf-term-0.18.1/py_pdf_term/stylings/__init__.py
--rw-r--r--   0        0        0      260 2021-10-27 15:17:22.117153 py-pdf-term-0.18.1/py_pdf_term/stylings/_stylings/__init__.py
--rw-r--r--   0        0        0     1805 2021-10-27 14:58:53.764535 py-pdf-term-0.18.1/py_pdf_term/stylings/_stylings/data.py
--rw-r--r--   0        0        0     2296 2021-10-27 14:58:53.765139 py-pdf-term-0.18.1/py_pdf_term/stylings/_stylings/scorer.py
--rw-r--r--   0        0        0      185 2021-10-27 15:17:22.117554 py-pdf-term-0.18.1/py_pdf_term/stylings/_stylings/scores/__init__.py
--rw-r--r--   0        0        0      430 2021-10-27 14:58:53.765997 py-pdf-term-0.18.1/py_pdf_term/stylings/_stylings/scores/base.py
--rw-r--r--   0        0        0      969 2021-10-27 14:58:53.766332 py-pdf-term-0.18.1/py_pdf_term/stylings/_stylings/scores/color.py
--rw-r--r--   0        0        0     1194 2021-10-27 14:58:53.766792 py-pdf-term-0.18.1/py_pdf_term/stylings/_stylings/scores/fontsize.py
--rw-r--r--   0        0        0       86 2021-10-27 15:05:43.371069 py-pdf-term-0.18.1/py_pdf_term/stylings/scores.py
--rw-r--r--   0        0        0       74 2021-10-27 15:05:43.372705 py-pdf-term-0.18.1/py_pdf_term/techterms/__init__.py
--rw-r--r--   0        0        0      287 2021-10-27 15:17:22.120150 py-pdf-term-0.18.1/py_pdf_term/techterms/_techterms/__init__.py
--rw-r--r--   0        0        0     1760 2021-10-27 14:58:53.767755 py-pdf-term-0.18.1/py_pdf_term/techterms/_techterms/data.py
--rw-r--r--   0        0        0     3936 2021-10-27 14:58:53.768144 py-pdf-term-0.18.1/py_pdf_term/techterms/_techterms/extractor.py
--rw-r--r--   0        0        0      394 2021-10-27 14:58:53.768485 py-pdf-term-0.18.1/py_pdf_term/techterms/_techterms/utils.py
--rw-r--r--   0        0        0       74 2021-10-27 15:05:43.379375 py-pdf-term-0.18.1/py_pdf_term/tokenizer/__init__.py
--rw-r--r--   0        0        0      319 2022-03-09 08:26:28.213241 py-pdf-term-0.18.1/py_pdf_term/tokenizer/_tokenizer/__init__.py
--rw-r--r--   0        0        0      421 2022-03-09 08:26:28.213876 py-pdf-term-0.18.1/py_pdf_term/tokenizer/_tokenizer/base.py
--rw-r--r--   0        0        0      510 2022-03-09 08:26:28.214614 py-pdf-term-0.18.1/py_pdf_term/tokenizer/_tokenizer/data.py
--rw-r--r--   0        0        0     1246 2022-03-09 08:26:28.215036 py-pdf-term-0.18.1/py_pdf_term/tokenizer/_tokenizer/english.py
--rw-r--r--   0        0        0     2623 2022-03-09 08:26:28.215506 py-pdf-term-0.18.1/py_pdf_term/tokenizer/_tokenizer/japanese.py
--rw-r--r--   0        0        0      712 2022-03-09 08:26:28.216196 py-pdf-term-0.18.1/py_pdf_term/tokenizer/_tokenizer/tokenizer.py
--rw-r--r--   0        0        0     1144 2022-03-09 08:58:21.142776 py-pdf-term-0.18.1/pyproject.toml
--rw-r--r--   0        0        0     3296 2022-03-09 09:02:45.397374 py-pdf-term-0.18.1/setup.py
--rw-r--r--   0        0        0     1307 2022-03-09 09:02:45.397718 py-pdf-term-0.18.1/PKG-INFO
+-rw-r--r--   0        0        0     1065 2021-08-01 13:41:41.018921 py_pdf_term-1.0.0/LICENSE
+-rw-r--r--   0        0        0      558 2023-04-22 03:34:12.853470 py_pdf_term-1.0.0/README.md
+-rw-r--r--   0        0        0      325 2023-05-21 11:41:58.441154 py_pdf_term-1.0.0/py_pdf_term/__init__.py
+-rw-r--r--   0        0        0        0 2021-07-17 01:56:39.528684 py_pdf_term-1.0.0/py_pdf_term/_common/__init__.py
+-rw-r--r--   0        0        0     2445 2023-04-30 07:57:40.302941 py_pdf_term-1.0.0/py_pdf_term/_common/consts.py
+-rw-r--r--   0        0        0      377 2023-05-07 09:38:40.927900 py_pdf_term-1.0.0/py_pdf_term/_common/data.py
+-rw-r--r--   0        0        0      279 2023-05-07 09:38:40.928433 py_pdf_term-1.0.0/py_pdf_term/_common/utils.py
+-rw-r--r--   0        0        0       89 2023-04-23 12:35:30.854867 py_pdf_term-1.0.0/py_pdf_term/analysis/__init__.py
+-rw-r--r--   0        0        0      442 2023-05-21 10:48:35.970334 py_pdf_term-1.0.0/py_pdf_term/analysis/_analysis/__init__.py
+-rw-r--r--   0        0        0      168 2023-05-21 10:48:35.871081 py_pdf_term-1.0.0/py_pdf_term/analysis/_analysis/concats/__init__.py
+-rw-r--r--   0        0        0     4037 2023-05-07 09:38:40.929139 py_pdf_term-1.0.0/py_pdf_term/analysis/_analysis/concats/lr.py
+-rw-r--r--   0        0        0      151 2023-05-21 10:48:35.871055 py_pdf_term-1.0.0/py_pdf_term/analysis/_analysis/cooccurrences/__init__.py
+-rw-r--r--   0        0        0     3188 2023-05-07 09:38:40.930038 py_pdf_term-1.0.0/py_pdf_term/analysis/_analysis/cooccurrences/container.py
+-rw-r--r--   0        0        0      146 2023-05-21 10:48:35.888277 py_pdf_term-1.0.0/py_pdf_term/analysis/_analysis/occurrences/__init__.py
+-rw-r--r--   0        0        0     3682 2023-05-07 09:38:40.930653 py_pdf_term-1.0.0/py_pdf_term/analysis/_analysis/occurrences/term.py
+-rw-r--r--   0        0        0     2210 2023-05-07 09:38:40.931460 py_pdf_term-1.0.0/py_pdf_term/analysis/_analysis/runner.py
+-rw-r--r--   0        0        0       92 2023-04-23 12:35:30.855657 py_pdf_term-1.0.0/py_pdf_term/candidates/__init__.py
+-rw-r--r--   0        0        0      287 2023-05-21 10:48:35.963075 py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/__init__.py
+-rw-r--r--   0        0        0      315 2023-05-21 10:48:35.923659 py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/augmenters/__init__.py
+-rw-r--r--   0        0        0      993 2023-05-07 09:38:40.932281 py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/augmenters/base.py
+-rw-r--r--   0        0        0     1451 2023-05-07 09:38:40.933258 py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/augmenters/combiner.py
+-rw-r--r--   0        0        0     3499 2023-05-07 09:38:40.934024 py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/augmenters/separation.py
+-rw-r--r--   0        0        0      315 2023-05-21 10:48:35.928200 py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/classifiers/__init__.py
+-rw-r--r--   0        0        0     3446 2023-05-01 10:52:18.632436 py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/classifiers/base.py
+-rw-r--r--   0        0        0      585 2023-05-01 10:52:18.633202 py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/classifiers/english.py
+-rw-r--r--   0        0        0      622 2023-05-01 10:52:18.633951 py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/classifiers/japanese.py
+-rw-r--r--   0        0        0     1418 2023-05-07 09:38:40.934955 py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/classifiers/marker.py
+-rw-r--r--   0        0        0     4479 2023-05-07 09:38:40.936309 py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/data.py
+-rw-r--r--   0        0        0     8826 2023-05-07 09:38:40.936924 py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/extractor.py
+-rw-r--r--   0        0        0      985 2023-05-21 10:48:35.957866 py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/filters/__init__.py
+-rw-r--r--   0        0        0     3422 2023-05-07 09:38:40.938498 py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/filters/combiner.py
+-rw-r--r--   0        0        0      816 2023-05-21 10:48:35.959032 py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/filters/term/__init__.py
+-rw-r--r--   0        0        0     1844 2023-05-07 09:38:40.940803 py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/filters/term/base.py
+-rw-r--r--   0        0        0      192 2023-05-21 10:48:36.026802 py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/filters/term/concatenation/__init__.py
+-rw-r--r--   0        0        0     3749 2023-05-07 09:38:40.941707 py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/filters/term/concatenation/english.py
+-rw-r--r--   0        0        0     5446 2023-05-07 09:38:40.942264 py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/filters/term/concatenation/japanese.py
+-rw-r--r--   0        0        0      168 2023-05-21 10:48:35.977851 py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/filters/term/numeric/__init__.py
+-rw-r--r--   0        0        0      763 2023-05-07 09:38:40.943040 py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/filters/term/numeric/english.py
+-rw-r--r--   0        0        0     1142 2023-05-07 09:38:40.943767 py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/filters/term/numeric/japanese.py
+-rw-r--r--   0        0        0      180 2023-05-21 10:48:35.985218 py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/filters/term/propernoun/__init__.py
+-rw-r--r--   0        0        0      355 2023-05-07 09:38:40.944518 py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/filters/term/propernoun/english.py
+-rw-r--r--   0        0        0     1053 2023-05-07 09:38:40.945146 py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/filters/term/propernoun/japanese.py
+-rw-r--r--   0        0        0      180 2023-05-21 10:48:35.994920 py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/filters/term/symbollike/__init__.py
+-rw-r--r--   0        0        0     2254 2023-05-07 09:38:40.945849 py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/filters/term/symbollike/english.py
+-rw-r--r--   0        0        0     2357 2023-05-07 09:38:40.946502 py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/filters/term/symbollike/japanese.py
+-rw-r--r--   0        0        0      231 2023-05-21 10:48:36.028806 py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/filters/token/__init__.py
+-rw-r--r--   0        0        0     1250 2023-05-01 10:52:18.644721 py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/filters/token/base.py
+-rw-r--r--   0        0        0     1821 2023-05-01 10:52:18.645564 py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/filters/token/english.py
+-rw-r--r--   0        0        0     2956 2023-05-01 10:52:18.646465 py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/filters/token/japanese.py
+-rw-r--r--   0        0        0      254 2023-05-21 10:48:36.025521 py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/splitters/__init__.py
+-rw-r--r--   0        0        0     1793 2023-05-07 09:38:40.947207 py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/splitters/base.py
+-rw-r--r--   0        0        0     1235 2023-05-07 09:38:40.947993 py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/splitters/combiner.py
+-rw-r--r--   0        0        0     3013 2023-05-07 09:38:40.949139 py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/splitters/repeat.py
+-rw-r--r--   0        0        0     1474 2023-05-07 09:38:40.950192 py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/splitters/symname.py
+-rw-r--r--   0        0        0     1579 2023-05-01 09:56:20.542921 py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/utils.py
+-rw-r--r--   0        0        0      115 2023-04-23 12:35:30.856299 py_pdf_term-1.0.0/py_pdf_term/candidates/augmenters.py
+-rw-r--r--   0        0        0      117 2023-04-23 12:35:30.857009 py_pdf_term-1.0.0/py_pdf_term/candidates/classifiers.py
+-rw-r--r--   0        0        0      109 2023-04-23 12:35:30.858941 py_pdf_term-1.0.0/py_pdf_term/candidates/filters.py
+-rw-r--r--   0        0        0      113 2023-04-23 12:35:30.859936 py_pdf_term-1.0.0/py_pdf_term/candidates/splitters.py
+-rw-r--r--   0        0        0      430 2023-05-21 10:48:36.041965 py_pdf_term-1.0.0/py_pdf_term/configs.py
+-rw-r--r--   0        0        0       88 2023-04-23 12:35:30.860623 py_pdf_term-1.0.0/py_pdf_term/endtoend/__init__.py
+-rw-r--r--   0        0        0      333 2023-05-21 10:48:36.055901 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/__init__.py
+-rw-r--r--   0        0        0     1024 2023-05-21 10:48:36.093130 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/caches/__init__.py
+-rw-r--r--   0        0        0      254 2023-05-21 10:48:36.054361 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/caches/candidate/__init__.py
+-rw-r--r--   0        0        0     2245 2023-05-01 10:52:18.650657 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/caches/candidate/base.py
+-rw-r--r--   0        0        0     2388 2023-05-07 09:38:40.950934 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/caches/candidate/file.py
+-rw-r--r--   0        0        0      788 2023-05-01 10:52:18.652062 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/caches/candidate/nocache.py
+-rw-r--r--   0        0        0      184 2023-04-30 03:53:53.377462 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/caches/consts.py
+-rw-r--r--   0        0        0      448 2023-05-21 10:48:36.076321 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/caches/method/__init__.py
+-rw-r--r--   0        0        0     6005 2023-05-01 10:52:18.652631 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/caches/method/base.py
+-rw-r--r--   0        0        0     4896 2023-05-07 09:38:40.951642 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/caches/method/file.py
+-rw-r--r--   0        0        0     1777 2023-05-01 10:52:18.653880 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/caches/method/nocache.py
+-rw-r--r--   0        0        0      227 2023-05-21 10:48:36.069449 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/caches/styling/__init__.py
+-rw-r--r--   0        0        0     2222 2023-05-01 10:52:18.654501 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/caches/styling/base.py
+-rw-r--r--   0        0        0     2377 2023-05-07 09:38:40.952425 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/caches/styling/file.py
+-rw-r--r--   0        0        0      770 2023-05-01 10:52:18.655623 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/caches/styling/nocache.py
+-rw-r--r--   0        0        0      702 2021-07-17 01:56:39.549058 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/caches/util.py
+-rw-r--r--   0        0        0      203 2023-05-21 10:48:36.064385 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/caches/xml/__init__.py
+-rw-r--r--   0        0        0     2122 2023-05-01 10:52:18.656159 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/caches/xml/base.py
+-rw-r--r--   0        0        0     2348 2023-05-03 08:07:06.640739 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/caches/xml/file.py
+-rw-r--r--   0        0        0      701 2023-05-01 10:52:18.657277 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/caches/xml/nocache.py
+-rw-r--r--   0        0        0      586 2023-05-21 10:48:36.206572 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/configs/__init__.py
+-rw-r--r--   0        0        0      707 2023-05-01 10:52:18.658128 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/configs/base.py
+-rw-r--r--   0        0        0     3264 2023-05-01 10:52:18.659057 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/configs/candidate.py
+-rw-r--r--   0        0        0     1821 2023-05-01 10:52:18.659640 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/configs/method.py
+-rw-r--r--   0        0        0      743 2023-05-01 10:52:18.660263 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/configs/styling.py
+-rw-r--r--   0        0        0      752 2023-05-01 10:52:18.660806 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/configs/techterm.py
+-rw-r--r--   0        0        0     1005 2023-05-01 10:52:18.662558 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/configs/xml.py
+-rw-r--r--   0        0        0      635 2023-05-21 09:40:45.033904 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/data.py
+-rw-r--r--   0        0        0    18045 2023-05-21 09:40:45.035210 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/extractor.py
+-rw-r--r--   0        0        0      480 2023-05-21 10:48:36.091002 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/layers/__init__.py
+-rw-r--r--   0        0        0     6156 2023-05-21 09:44:19.458264 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/layers/candidate.py
+-rw-r--r--   0        0        0     9788 2023-05-21 09:44:19.459767 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/layers/method.py
+-rw-r--r--   0        0        0     2832 2023-05-21 09:44:19.461295 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/layers/styling.py
+-rw-r--r--   0        0        0     5405 2023-05-01 10:52:18.667346 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/layers/techterm.py
+-rw-r--r--   0        0        0     2700 2023-05-21 09:44:19.462264 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/layers/xml.py
+-rw-r--r--   0        0        0     1077 2023-05-21 10:48:36.178877 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/mappers/__init__.py
+-rw-r--r--   0        0        0     2925 2023-05-21 09:44:19.463517 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/mappers/base.py
+-rw-r--r--   0        0        0      407 2023-05-21 10:48:36.215373 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/mappers/caches/__init__.py
+-rw-r--r--   0        0        0      687 2023-05-21 09:44:19.464771 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/mappers/caches/candidate.py
+-rw-r--r--   0        0        0     1392 2023-05-21 09:44:19.466267 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/mappers/caches/method.py
+-rw-r--r--   0        0        0      652 2023-05-21 09:44:19.467168 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/mappers/caches/styling.py
+-rw-r--r--   0        0        0      616 2023-05-21 09:44:19.468834 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/mappers/caches/xml.py
+-rw-r--r--   0        0        0      446 2023-05-21 10:48:36.239199 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/mappers/candidates/__init__.py
+-rw-r--r--   0        0        0      774 2023-05-21 09:44:19.469622 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/mappers/candidates/augmenter.py
+-rw-r--r--   0        0        0      783 2023-05-21 09:44:19.470490 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/mappers/candidates/classifier.py
+-rw-r--r--   0        0        0     1727 2023-05-21 09:44:19.471360 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/mappers/candidates/filter.py
+-rw-r--r--   0        0        0      742 2023-05-21 09:44:19.472913 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/mappers/candidates/lang.py
+-rw-r--r--   0        0        0      644 2023-05-21 09:44:19.473977 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/mappers/candidates/splitter.py
+-rw-r--r--   0        0        0      204 2023-05-21 10:48:36.187774 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/mappers/methods/__init__.py
+-rw-r--r--   0        0        0      691 2023-05-21 09:44:19.476084 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/mappers/methods/multi.py
+-rw-r--r--   0        0        0      775 2023-05-21 09:44:19.478488 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/mappers/methods/single.py
+-rw-r--r--   0        0        0       97 2023-05-21 10:48:36.192351 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/mappers/pdftoxml/__init__.py
+-rw-r--r--   0        0        0      654 2023-05-21 09:44:19.479440 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/mappers/pdftoxml/binopener.py
+-rw-r--r--   0        0        0       93 2023-05-21 10:48:36.200466 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/mappers/stylings/__init__.py
+-rw-r--r--   0        0        0      680 2023-05-21 09:44:19.481386 py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/mappers/stylings/score.py
+-rw-r--r--   0        0        0      102 2023-04-23 12:35:30.862807 py_pdf_term-1.0.0/py_pdf_term/endtoend/caches.py
+-rw-r--r--   0        0        0      976 2023-05-21 10:48:36.271106 py_pdf_term-1.0.0/py_pdf_term/mappers.py
+-rw-r--r--   0        0        0       88 2023-04-23 12:35:30.863506 py_pdf_term-1.0.0/py_pdf_term/methods/__init__.py
+-rw-r--r--   0        0        0      536 2023-05-21 10:48:36.254137 py_pdf_term-1.0.0/py_pdf_term/methods/_methods/__init__.py
+-rw-r--r--   0        0        0     8534 2023-05-01 10:52:18.677653 py_pdf_term-1.0.0/py_pdf_term/methods/_methods/base.py
+-rw-r--r--   0        0        0      567 2023-05-21 10:48:36.245483 py_pdf_term-1.0.0/py_pdf_term/methods/_methods/collectors/__init__.py
+-rw-r--r--   0        0        0      983 2023-05-01 10:52:18.678289 py_pdf_term-1.0.0/py_pdf_term/methods/_methods/collectors/base.py
+-rw-r--r--   0        0        0     1000 2023-05-01 10:52:18.678854 py_pdf_term-1.0.0/py_pdf_term/methods/_methods/collectors/flr.py
+-rw-r--r--   0        0        0     1006 2023-05-01 10:52:18.679428 py_pdf_term-1.0.0/py_pdf_term/methods/_methods/collectors/flrh.py
+-rw-r--r--   0        0        0     1006 2023-05-01 10:52:18.679998 py_pdf_term-1.0.0/py_pdf_term/methods/_methods/collectors/hits.py
+-rw-r--r--   0        0        0     1010 2023-05-01 10:52:18.680523 py_pdf_term-1.0.0/py_pdf_term/methods/_methods/collectors/mcvalue.py
+-rw-r--r--   0        0        0      740 2023-05-01 10:52:18.681051 py_pdf_term-1.0.0/py_pdf_term/methods/_methods/collectors/mdp.py
+-rw-r--r--   0        0        0      893 2023-05-01 10:52:18.681650 py_pdf_term-1.0.0/py_pdf_term/methods/_methods/collectors/tfidf.py
+-rw-r--r--   0        0        0      936 2023-05-02 07:56:39.552792 py_pdf_term-1.0.0/py_pdf_term/methods/_methods/data.py
+-rw-r--r--   0        0        0      591 2023-05-01 10:52:18.682880 py_pdf_term-1.0.0/py_pdf_term/methods/_methods/flr.py
+-rw-r--r--   0        0        0      951 2023-05-01 10:52:18.683430 py_pdf_term-1.0.0/py_pdf_term/methods/_methods/flrh.py
+-rw-r--r--   0        0        0     1186 2023-05-21 07:39:18.389207 py_pdf_term-1.0.0/py_pdf_term/methods/_methods/hits.py
+-rw-r--r--   0        0        0      632 2023-05-01 10:52:18.684461 py_pdf_term-1.0.0/py_pdf_term/methods/_methods/mcvalue.py
+-rw-r--r--   0        0        0      589 2023-05-21 10:54:59.338573 py_pdf_term-1.0.0/py_pdf_term/methods/_methods/mdp.py
+-rw-r--r--   0        0        0      447 2023-05-21 10:48:36.254929 py_pdf_term-1.0.0/py_pdf_term/methods/_methods/rankers/__init__.py
+-rw-r--r--   0        0        0     2101 2023-05-01 10:52:18.685791 py_pdf_term-1.0.0/py_pdf_term/methods/_methods/rankers/base.py
+-rw-r--r--   0        0        0     2029 2023-05-07 09:38:40.961943 py_pdf_term-1.0.0/py_pdf_term/methods/_methods/rankers/flr.py
+-rw-r--r--   0        0        0     2853 2023-05-07 09:38:40.962849 py_pdf_term-1.0.0/py_pdf_term/methods/_methods/rankers/flrh.py
+-rw-r--r--   0        0        0     6342 2023-05-21 09:40:45.036164 py_pdf_term-1.0.0/py_pdf_term/methods/_methods/rankers/hits.py
+-rw-r--r--   0        0        0     1968 2023-05-07 09:38:40.967316 py_pdf_term-1.0.0/py_pdf_term/methods/_methods/rankers/mcvalue.py
+-rw-r--r--   0        0        0     3171 2023-05-21 10:54:59.339804 py_pdf_term-1.0.0/py_pdf_term/methods/_methods/rankers/mdp.py
+-rw-r--r--   0        0        0     2009 2023-05-21 10:54:59.340978 py_pdf_term-1.0.0/py_pdf_term/methods/_methods/rankers/tfidf.py
+-rw-r--r--   0        0        0      473 2023-05-21 10:48:36.275731 py_pdf_term-1.0.0/py_pdf_term/methods/_methods/rankingdata/__init__.py
+-rw-r--r--   0        0        0      561 2023-05-01 10:52:18.689999 py_pdf_term-1.0.0/py_pdf_term/methods/_methods/rankingdata/base.py
+-rw-r--r--   0        0        0      970 2023-05-01 10:52:18.690868 py_pdf_term-1.0.0/py_pdf_term/methods/_methods/rankingdata/flr.py
+-rw-r--r--   0        0        0      972 2023-05-01 10:52:18.691383 py_pdf_term-1.0.0/py_pdf_term/methods/_methods/rankingdata/flrh.py
+-rw-r--r--   0        0        0      972 2023-05-01 10:52:18.691953 py_pdf_term-1.0.0/py_pdf_term/methods/_methods/rankingdata/hits.py
+-rw-r--r--   0        0        0     1440 2023-05-01 10:52:18.692557 py_pdf_term-1.0.0/py_pdf_term/methods/_methods/rankingdata/mcvalue.py
+-rw-r--r--   0        0        0     1189 2023-05-21 09:40:45.038339 py_pdf_term-1.0.0/py_pdf_term/methods/_methods/rankingdata/mdp.py
+-rw-r--r--   0        0        0      860 2023-05-01 10:52:18.693606 py_pdf_term-1.0.0/py_pdf_term/methods/_methods/rankingdata/tfidf.py
+-rw-r--r--   0        0        0      610 2023-05-21 10:54:59.341988 py_pdf_term-1.0.0/py_pdf_term/methods/_methods/tfidf.py
+-rw-r--r--   0        0        0      110 2023-04-23 12:35:30.865641 py_pdf_term-1.0.0/py_pdf_term/methods/collectors.py
+-rw-r--r--   0        0        0      104 2023-04-23 12:35:30.866294 py_pdf_term-1.0.0/py_pdf_term/methods/rankers.py
+-rw-r--r--   0        0        0      112 2023-04-23 12:35:30.866995 py_pdf_term-1.0.0/py_pdf_term/methods/rankingdata.py
+-rw-r--r--   0        0        0       88 2023-04-23 12:35:30.867710 py_pdf_term-1.0.0/py_pdf_term/pdftoxml/__init__.py
+-rw-r--r--   0        0        0      174 2023-05-21 10:48:36.260616 py_pdf_term-1.0.0/py_pdf_term/pdftoxml/_pdftoxml/__init__.py
+-rw-r--r--   0        0        0      155 2023-05-21 10:48:36.285807 py_pdf_term-1.0.0/py_pdf_term/pdftoxml/_pdftoxml/binopeners/__init__.py
+-rw-r--r--   0        0        0      577 2023-05-01 10:52:18.694863 py_pdf_term-1.0.0/py_pdf_term/pdftoxml/_pdftoxml/binopeners/base.py
+-rw-r--r--   0        0        0      369 2023-05-01 10:52:18.695436 py_pdf_term-1.0.0/py_pdf_term/pdftoxml/_pdftoxml/binopeners/standard.py
+-rw-r--r--   0        0        0     4111 2023-05-01 10:52:18.695967 py_pdf_term-1.0.0/py_pdf_term/pdftoxml/_pdftoxml/converter.py
+-rw-r--r--   0        0        0     1421 2023-05-07 09:38:40.970029 py_pdf_term-1.0.0/py_pdf_term/pdftoxml/_pdftoxml/data.py
+-rw-r--r--   0        0        0     6064 2023-05-01 10:52:18.697047 py_pdf_term-1.0.0/py_pdf_term/pdftoxml/_pdftoxml/textful.py
+-rw-r--r--   0        0        0      871 2021-12-23 08:24:58.272396 py_pdf_term-1.0.0/py_pdf_term/pdftoxml/_pdftoxml/utils.py
+-rw-r--r--   0        0        0      111 2023-04-30 07:57:40.332098 py_pdf_term-1.0.0/py_pdf_term/pdftoxml/binopeners.py
+-rw-r--r--   0        0        0       88 2023-04-23 12:35:30.870578 py_pdf_term-1.0.0/py_pdf_term/stylings/__init__.py
+-rw-r--r--   0        0        0      260 2023-05-21 10:48:36.286348 py_pdf_term-1.0.0/py_pdf_term/stylings/_stylings/__init__.py
+-rw-r--r--   0        0        0     2487 2023-05-02 07:56:40.346196 py_pdf_term-1.0.0/py_pdf_term/stylings/_stylings/data.py
+-rw-r--r--   0        0        0     3474 2023-05-02 07:56:40.422973 py_pdf_term-1.0.0/py_pdf_term/stylings/_stylings/scorer.py
+-rw-r--r--   0        0        0      185 2023-05-21 10:48:36.278288 py_pdf_term-1.0.0/py_pdf_term/stylings/_stylings/scores/__init__.py
+-rw-r--r--   0        0        0     1215 2023-05-07 09:38:40.970711 py_pdf_term-1.0.0/py_pdf_term/stylings/_stylings/scores/base.py
+-rw-r--r--   0        0        0     1212 2023-05-07 09:38:40.971530 py_pdf_term-1.0.0/py_pdf_term/stylings/_stylings/scores/color.py
+-rw-r--r--   0        0        0     1512 2023-05-07 09:38:40.972047 py_pdf_term-1.0.0/py_pdf_term/stylings/_stylings/scores/fontsize.py
+-rw-r--r--   0        0        0      102 2023-04-23 12:35:30.871198 py_pdf_term-1.0.0/py_pdf_term/stylings/scores.py
+-rw-r--r--   0        0        0       91 2023-04-23 12:35:30.872290 py_pdf_term-1.0.0/py_pdf_term/techterms/__init__.py
+-rw-r--r--   0        0        0      287 2023-05-21 10:48:36.292986 py_pdf_term-1.0.0/py_pdf_term/techterms/_techterms/__init__.py
+-rw-r--r--   0        0        0     2415 2023-05-02 07:56:40.104927 py_pdf_term-1.0.0/py_pdf_term/techterms/_techterms/data.py
+-rw-r--r--   0        0        0     6115 2023-05-21 09:40:45.039682 py_pdf_term-1.0.0/py_pdf_term/techterms/_techterms/extractor.py
+-rw-r--r--   0        0        0      494 2023-05-21 09:40:45.040935 py_pdf_term-1.0.0/py_pdf_term/techterms/_techterms/utils.py
+-rw-r--r--   0        0        0       92 2023-04-30 07:57:40.332522 py_pdf_term-1.0.0/py_pdf_term/tokenizers/__init__.py
+-rw-r--r--   0        0        0      337 2023-05-21 10:48:36.294274 py_pdf_term-1.0.0/py_pdf_term/tokenizers/_tokenizers/__init__.py
+-rw-r--r--   0        0        0     1512 2023-05-07 09:38:40.975403 py_pdf_term-1.0.0/py_pdf_term/tokenizers/_tokenizers/base.py
+-rw-r--r--   0        0        0     2560 2023-05-07 09:38:40.976423 py_pdf_term-1.0.0/py_pdf_term/tokenizers/_tokenizers/data.py
+-rw-r--r--   0        0        0     1425 2023-05-07 09:38:40.977066 py_pdf_term-1.0.0/py_pdf_term/tokenizers/_tokenizers/english.py
+-rw-r--r--   0        0        0     2854 2023-05-07 09:38:40.977733 py_pdf_term-1.0.0/py_pdf_term/tokenizers/_tokenizers/japanese.py
+-rw-r--r--   0        0        0     1396 2023-05-01 10:52:18.703945 py_pdf_term-1.0.0/py_pdf_term/tokenizers/_tokenizers/tokenizer.py
+-rw-r--r--   0        0        0     1185 2023-05-21 11:41:58.442912 py_pdf_term-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1259 1970-01-01 00:00:00.000000 py_pdf_term-1.0.0/PKG-INFO
```

### Comparing `py-pdf-term-0.18.1/LICENSE` & `py_pdf_term-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py-pdf-term-0.18.1/README.md` & `py_pdf_term-1.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,14 @@
 ```
 pip install py-pdf-term
 ```
 
 You also need to install spaCy models `ja_core_news_sm` and `en_core_web_sm`, which this module depends on.
 
 ```
-pip install https://github.com/explosion/spacy-models/releases/download/ja_core_news_sm-3.2.0/ja_core_news_sm-3.2.0.tar.gz
-pip install https://github.com/explosion/spacy-models/releases/download/en_core_web_sm-3.2.0/en_core_web_sm-3.2.0.tar.gz
+pip install https://github.com/explosion/spacy-models/releases/download/ja_core_news_sm-3.5.0/ja_core_news_sm-3.5.0.tar.gz
+pip install https://github.com/explosion/spacy-models/releases/download/en_core_web_sm-3.5.0/en_core_web_sm-3.5.0.tar.gz
 ```
 
 ## Documentation
 
 https://kumachan-mis.github.io/py-pdf-term
```

### Comparing `py-pdf-term-0.18.1/py_pdf_term/_common/consts.py` & `py_pdf_term-1.0.0/py_pdf_term/_common/consts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,151 +1,153 @@
-00000000: 2320 6874 7470 3a2f 2f77 7777 2e75 6e69  # http://www.uni
-00000010: 636f 6465 2e6f 7267 2f63 6861 7274 732f  code.org/charts/
-00000020: 0a0a 2320 416c 7068 6162 6574 0a41 4c50  ..# Alphabet.ALP
-00000030: 4841 4245 545f 5245 4745 5820 3d20 7222  HABET_REGEX = r"
-00000040: 5b41 2d5a 612d 7a5d 220a 0a23 204e 756d  [A-Za-z]"..# Num
-00000050: 6265 720a 4e55 4d42 4552 5f52 4547 4558  ber.NUMBER_REGEX
-00000060: 203d 2072 225b 302d 395d 220a 0a23 2048   = r"[0-9]"..# H
-00000070: 6972 6167 616e 610a 4849 5241 4741 4e41  iragana.HIRAGANA
-00000080: 5f52 4547 4558 203d 2072 225b 5c75 3330  _REGEX = r"[\u30
-00000090: 3430 2d5c 7533 3039 465d 220a 0a23 204b  40-\u309F]"..# K
-000000a0: 6174 616b 616e 610a 4b41 5441 4b41 4e41  atakana.KATAKANA
-000000b0: 5f52 4547 4558 203d 2072 225b 5c75 3330  _REGEX = r"[\u30
-000000c0: 4130 2d5c 7533 3046 465d 220a 0a23 204b  A0-\u30FF]"..# K
-000000d0: 616e 6a69 0a4b 414e 4a49 5f52 4547 4558  anji.KANJI_REGEX
-000000e0: 203d 2028 0a20 2020 2022 5b22 0a20 2020   = (.    "[".   
-000000f0: 202b 2022 222e 6a6f 696e 280a 2020 2020   + "".join(.    
-00000100: 2020 2020 5b0a 2020 2020 2020 2020 2020      [.          
-00000110: 2020 2320 434a 4b20 5261 6469 6361 6c73    # CJK Radicals
-00000120: 2053 7570 706c 656d 656e 740a 2020 2020   Supplement.    
-00000130: 2020 2020 2020 2020 225c 7532 4538 302d          "\u2E80-
-00000140: 5c75 3245 4646 222c 0a20 2020 2020 2020  \u2EFF",.       
-00000150: 2020 2020 2023 204b 616e 6778 6920 5261       # Kangxi Ra
-00000160: 6469 6361 6c73 0a20 2020 2020 2020 2020  dicals.         
-00000170: 2020 2022 5c75 3246 3030 2d5c 7532 4644     "\u2F00-\u2FD
-00000180: 4622 2c0a 2020 2020 2020 2020 2020 2020  F",.            
-00000190: 2320 434a 4b20 556e 6966 6965 6420 4964  # CJK Unified Id
-000001a0: 656f 6772 6170 6873 2045 7874 656e 7369  eographs Extensi
-000001b0: 6f6e 2041 0a20 2020 2020 2020 2020 2020  on A.           
-000001c0: 2022 5c75 3334 3030 2d5c 7534 4442 4622   "\u3400-\u4DBF"
-000001d0: 2c0a 2020 2020 2020 2020 2020 2020 2320  ,.            # 
-000001e0: 434a 4b20 556e 6966 6965 6420 4964 656f  CJK Unified Ideo
-000001f0: 6772 6170 6873 0a20 2020 2020 2020 2020  graphs.         
-00000200: 2020 2022 5c75 3445 3030 2d5c 7539 4646     "\u4E00-\u9FF
-00000210: 4622 2c0a 2020 2020 2020 2020 2020 2020  F",.            
-00000220: 2320 434a 4b20 436f 6d70 6174 6962 696c  # CJK Compatibil
-00000230: 6974 7920 4964 656f 6772 6170 6873 0a20  ity Ideographs. 
-00000240: 2020 2020 2020 2020 2020 2022 5c75 4639             "\uF9
-00000250: 3030 2d5c 7546 4146 4622 2c0a 2020 2020  00-\uFAFF",.    
-00000260: 2020 2020 5d0a 2020 2020 290a 2020 2020      ].    ).    
-00000270: 2b20 225d 220a 290a 0a23 2053 796d 626f  + "]".)..# Symbo
-00000280: 6c0a 5359 4d42 4f4c 5f52 4547 4558 203d  l.SYMBOL_REGEX =
-00000290: 2028 0a20 2020 2022 5b22 0a20 2020 202b   (.    "[".    +
-000002a0: 2022 222e 6a6f 696e 280a 2020 2020 2020   "".join(.      
-000002b0: 2020 5b0a 2020 2020 2020 2020 2020 2020    [.            
-000002c0: 2320 4261 7369 6320 4c61 7469 6e20 5379  # Basic Latin Sy
-000002d0: 6d62 6f6c 0a20 2020 2020 2020 2020 2020  mbol.           
-000002e0: 2022 5c75 3030 3231 2d5c 7530 3032 4622   "\u0021-\u002F"
-000002f0: 2c0a 2020 2020 2020 2020 2020 2020 225c  ,.            "\
-00000300: 7530 3033 412d 5c75 3030 3430 222c 0a20  u003A-\u0040",. 
-00000310: 2020 2020 2020 2020 2020 2022 5c75 3030             "\u00
-00000320: 3542 2d5c 7530 3036 3022 2c0a 2020 2020  5B-\u0060",.    
-00000330: 2020 2020 2020 2020 225c 7530 3037 422d          "\u007B-
-00000340: 5c75 3030 3746 222c 0a20 2020 2020 2020  \u007F",.       
-00000350: 2020 2020 2023 204c 6174 696e 2d31 2053       # Latin-1 S
-00000360: 7570 706c 656d 656e 7420 5379 6d62 6f6c  upplement Symbol
-00000370: 0a20 2020 2020 2020 2020 2020 2022 5c75  .            "\u
-00000380: 3030 4131 2d5c 7530 3042 465c 7530 3044  00A1-\u00BF\u00D
-00000390: 375c 7530 3046 3722 2c0a 2020 2020 2020  7\u00F7",.      
-000003a0: 2020 2020 2020 2320 5370 6163 696e 6720        # Spacing 
-000003b0: 4d6f 6469 6669 6572 204c 6574 7465 7273  Modifier Letters
-000003c0: 202d 2043 6f6d 6269 6e69 6e67 2044 6961   - Combining Dia
-000003d0: 6372 6974 6963 616c 204d 6172 6b73 0a20  critical Marks. 
-000003e0: 2020 2020 2020 2020 2020 2022 5c75 3032             "\u02
-000003f0: 4230 2d5c 7530 3336 4622 2c0a 2020 2020  B0-\u036F",.    
-00000400: 2020 2020 2020 2020 2320 5068 6f6e 6574          # Phonet
-00000410: 6963 2045 7874 656e 7369 6f6e 7320 2d20  ic Extensions - 
-00000420: 436f 6d62 696e 696e 6720 4469 6163 7269  Combining Diacri
-00000430: 7469 6361 6c20 4d61 726b 7320 5375 7070  tical Marks Supp
-00000440: 6c65 6d65 6e74 0a20 2020 2020 2020 2020  lement.         
-00000450: 2020 2022 5c75 3144 3030 2d5c 7531 4446     "\u1D00-\u1DF
-00000460: 4622 2c0a 2020 2020 2020 2020 2020 2020  F",.            
-00000470: 2320 4765 6e65 7261 6c20 5075 6e63 7475  # General Punctu
-00000480: 6174 696f 6e20 2d20 4d69 7363 656c 6c61  ation - Miscella
-00000490: 6e65 6f75 7320 5379 6d62 6f6c 7320 616e  neous Symbols an
-000004a0: 6420 4172 726f 7773 0a20 2020 2020 2020  d Arrows.       
-000004b0: 2020 2020 2022 5c75 3230 3130 2d5c 7532       "\u2010-\u2
-000004c0: 4246 4622 2c0a 2020 2020 2020 2020 2020  BFF",.          
-000004d0: 2020 2320 5375 7070 6c65 6d65 6e74 616c    # Supplemental
-000004e0: 2050 756e 6374 7561 7469 6f6e 0a20 2020   Punctuation.   
-000004f0: 2020 2020 2020 2020 2022 5c75 3245 3030           "\u2E00
-00000500: 2d5c 7532 4537 4622 2c0a 2020 2020 2020  -\u2E7F",.      
-00000510: 2020 2020 2020 2320 4964 656f 6772 6170        # Ideograp
-00000520: 6869 6320 4465 7363 7269 7074 696f 6e20  hic Description 
-00000530: 4368 6172 6163 7465 7273 202d 2043 4a4b  Characters - CJK
-00000540: 2053 796d 626f 6c73 2061 6e64 2050 756e   Symbols and Pun
-00000550: 6374 7561 7469 6f6e 0a20 2020 2020 2020  ctuation.       
-00000560: 2020 2020 2022 5c75 3246 4630 2d5c 7533       "\u2FF0-\u3
-00000570: 3033 4622 0a20 2020 2020 2020 2020 2020  03F".           
-00000580: 2023 2042 6f70 6f6d 6f66 6f20 2d20 434a   # Bopomofo - CJ
-00000590: 4b20 5374 726f 6b65 730a 2020 2020 2020  K Strokes.      
-000005a0: 2020 2020 2020 225c 7533 3130 302d 5c75        "\u3100-\u
-000005b0: 3331 4546 222c 0a20 2020 2020 2020 2020  31EF",.         
-000005c0: 2020 2023 2045 6e63 6c6f 7365 6420 434a     # Enclosed CJ
-000005d0: 4b20 4c65 7474 6572 7320 616e 6420 4d6f  K Letters and Mo
-000005e0: 6e74 6873 202d 2043 4a4b 2043 6f6d 7061  nths - CJK Compa
-000005f0: 7469 6269 6c69 7479 0a20 2020 2020 2020  tibility.       
-00000600: 2020 2020 2022 5c75 3332 3030 2d5c 7533       "\u3200-\u3
-00000610: 3346 4622 2c0a 2020 2020 2020 2020 2020  3FF",.          
-00000620: 2020 2320 5969 6a69 6e67 2048 6578 6167    # Yijing Hexag
-00000630: 7261 6d20 5379 6d62 6f6c 730a 2020 2020  ram Symbols.    
-00000640: 2020 2020 2020 2020 225c 7534 4443 302d          "\u4DC0-
-00000650: 5c75 3444 4646 222c 0a20 2020 2020 2020  \u4DFF",.       
-00000660: 2020 2020 2023 204d 6f64 6966 6965 7220       # Modifier 
-00000670: 546f 6e65 204c 6574 7465 7273 0a20 2020  Tone Letters.   
-00000680: 2020 2020 2020 2020 2022 5c75 4137 3030           "\uA700
-00000690: 2d5c 7541 3731 4622 2c0a 2020 2020 2020  -\uA71F",.      
-000006a0: 2020 2020 2020 2320 4869 6768 2053 7572        # High Sur
-000006b0: 726f 6761 7465 7320 2d20 5072 6976 6174  rogates - Privat
-000006c0: 6520 5573 6520 4172 6561 0a20 2020 2020  e Use Area.     
-000006d0: 2020 2020 2020 2022 5c75 4438 3030 2d5c         "\uD800-\
-000006e0: 7546 3846 4622 2c0a 2020 2020 2020 2020  uF8FF",.        
-000006f0: 2020 2020 2320 5661 7269 6174 696f 6e20      # Variation 
-00000700: 5365 6c65 6374 6f72 7320 2d20 536d 616c  Selectors - Smal
-00000710: 6c20 466f 726d 2056 6172 6961 6e74 730a  l Form Variants.
-00000720: 2020 2020 2020 2020 2020 2020 225c 7546              "\uF
-00000730: 4530 302d 5c75 4645 3646 222c 0a20 2020  E00-\uFE6F",.   
-00000740: 2020 2020 2020 2020 2023 2053 7065 6369           # Speci
-00000750: 616c 730a 2020 2020 2020 2020 2020 2020  als.            
-00000760: 225c 7546 4646 302d 5c75 4646 4646 222c  "\uFFF0-\uFFFF",
-00000770: 0a20 2020 2020 2020 205d 0a20 2020 2029  .        ].    )
-00000780: 0a20 2020 202b 2022 5d22 0a29 0a0a 2320  .    + "]".)..# 
-00000790: 4861 6c66 7769 6474 6820 616e 6420 4675  Halfwidth and Fu
-000007a0: 6c6c 7769 6474 680a 4841 4c46 5749 4454  llwidth.HALFWIDT
-000007b0: 485f 4153 4349 495f 4348 4152 5320 3d20  H_ASCII_CHARS = 
-000007c0: 2222 2e6a 6f69 6e28 5b63 6872 2863 6f64  "".join([chr(cod
-000007d0: 6529 2066 6f72 2063 6f64 6520 696e 2072  e) for code in r
-000007e0: 616e 6765 2830 7830 3032 312c 2030 7830  ange(0x0021, 0x0
-000007f0: 3037 4520 2b20 3129 5d29 0a46 554c 4c57  07E + 1)]).FULLW
-00000800: 4944 5448 5f41 5343 4949 5f43 4841 5253  IDTH_ASCII_CHARS
-00000810: 203d 2022 222e 6a6f 696e 285b 6368 7228   = "".join([chr(
-00000820: 636f 6465 2920 666f 7220 636f 6465 2069  code) for code i
-00000830: 6e20 7261 6e67 6528 3078 4646 3031 2c20  n range(0xFF01, 
-00000840: 3078 4646 3545 202b 2031 295d 290a 0a23  0xFF5E + 1)])..#
-00000850: 204c 616e 6775 6167 6573 0a4a 4150 414e   Languages.JAPAN
-00000860: 4553 455f 5245 4745 5820 3d20 7266 2228  ESE_REGEX = rf"(
-00000870: 3f3a 7b48 4952 4147 414e 415f 5245 4745  ?:{HIRAGANA_REGE
-00000880: 587d 7c7b 4b41 5441 4b41 4e41 5f52 4547  X}|{KATAKANA_REG
-00000890: 4558 7d7c 7b4b 414e 4a49 5f52 4547 4558  EX}|{KANJI_REGEX
-000008a0: 7d29 220a 454e 474c 4953 485f 5245 4745  })".ENGLISH_REGE
-000008b0: 5820 3d20 7266 2228 3f3a 7b41 4c50 4841  X = rf"(?:{ALPHA
-000008c0: 4245 545f 5245 4745 587d 2922 0a0a 2320  BET_REGEX})"..# 
-000008d0: 4368 6172 6163 7465 7220 7265 7175 6972  Character requir
-000008e0: 696e 6720 6e6f 6e2d 7370 6163 6520 6265  ing non-space be
-000008f0: 7477 6565 6e0a 4e4f 5350 4143 455f 5245  tween.NOSPACE_RE
-00000900: 4745 5820 3d20 280a 2020 2020 2228 3f3a  GEX = (.    "(?:
-00000910: 220a 2020 2020 2b20 227c 222e 6a6f 696e  ".    + "|".join
-00000920: 285b 4849 5241 4741 4e41 5f52 4547 4558  ([HIRAGANA_REGEX
-00000930: 2c20 4b41 5441 4b41 4e41 5f52 4547 4558  , KATAKANA_REGEX
-00000940: 2c20 4b41 4e4a 495f 5245 4745 582c 204e  , KANJI_REGEX, N
-00000950: 554d 4245 525f 5245 4745 582c 2022 2d22  UMBER_REGEX, "-"
-00000960: 5d29 0a20 2020 202b 2022 2922 0a29 0a    ]).    + ")".).
+00000000: 5041 434b 4147 455f 4e41 4d45 203d 2022  PACKAGE_NAME = "
+00000010: 7079 5f70 6466 5f74 6572 6d22 0a0a 2320  py_pdf_term"..# 
+00000020: 6874 7470 3a2f 2f77 7777 2e75 6e69 636f  http://www.unico
+00000030: 6465 2e6f 7267 2f63 6861 7274 732f 0a0a  de.org/charts/..
+00000040: 2320 416c 7068 6162 6574 0a41 4c50 4841  # Alphabet.ALPHA
+00000050: 4245 545f 5245 4745 5820 3d20 7222 5b41  BET_REGEX = r"[A
+00000060: 2d5a 612d 7a5d 220a 0a23 204e 756d 6265  -Za-z]"..# Numbe
+00000070: 720a 4e55 4d42 4552 5f52 4547 4558 203d  r.NUMBER_REGEX =
+00000080: 2072 225b 302d 395d 220a 0a23 2048 6972   r"[0-9]"..# Hir
+00000090: 6167 616e 610a 4849 5241 4741 4e41 5f52  agana.HIRAGANA_R
+000000a0: 4547 4558 203d 2072 225b 5c75 3330 3430  EGEX = r"[\u3040
+000000b0: 2d5c 7533 3039 465d 220a 0a23 204b 6174  -\u309F]"..# Kat
+000000c0: 616b 616e 610a 4b41 5441 4b41 4e41 5f52  akana.KATAKANA_R
+000000d0: 4547 4558 203d 2072 225b 5c75 3330 4130  EGEX = r"[\u30A0
+000000e0: 2d5c 7533 3046 465d 220a 0a23 204b 616e  -\u30FF]"..# Kan
+000000f0: 6a69 0a4b 414e 4a49 5f52 4547 4558 203d  ji.KANJI_REGEX =
+00000100: 2028 0a20 2020 2022 5b22 0a20 2020 202b   (.    "[".    +
+00000110: 2022 222e 6a6f 696e 280a 2020 2020 2020   "".join(.      
+00000120: 2020 5b0a 2020 2020 2020 2020 2020 2020    [.            
+00000130: 2320 434a 4b20 5261 6469 6361 6c73 2053  # CJK Radicals S
+00000140: 7570 706c 656d 656e 740a 2020 2020 2020  upplement.      
+00000150: 2020 2020 2020 225c 7532 4538 302d 5c75        "\u2E80-\u
+00000160: 3245 4646 222c 0a20 2020 2020 2020 2020  2EFF",.         
+00000170: 2020 2023 204b 616e 6778 6920 5261 6469     # Kangxi Radi
+00000180: 6361 6c73 0a20 2020 2020 2020 2020 2020  cals.           
+00000190: 2022 5c75 3246 3030 2d5c 7532 4644 4622   "\u2F00-\u2FDF"
+000001a0: 2c0a 2020 2020 2020 2020 2020 2020 2320  ,.            # 
+000001b0: 434a 4b20 556e 6966 6965 6420 4964 656f  CJK Unified Ideo
+000001c0: 6772 6170 6873 2045 7874 656e 7369 6f6e  graphs Extension
+000001d0: 2041 0a20 2020 2020 2020 2020 2020 2022   A.            "
+000001e0: 5c75 3334 3030 2d5c 7534 4442 4622 2c0a  \u3400-\u4DBF",.
+000001f0: 2020 2020 2020 2020 2020 2020 2320 434a              # CJ
+00000200: 4b20 556e 6966 6965 6420 4964 656f 6772  K Unified Ideogr
+00000210: 6170 6873 0a20 2020 2020 2020 2020 2020  aphs.           
+00000220: 2022 5c75 3445 3030 2d5c 7539 4646 4622   "\u4E00-\u9FFF"
+00000230: 2c0a 2020 2020 2020 2020 2020 2020 2320  ,.            # 
+00000240: 434a 4b20 436f 6d70 6174 6962 696c 6974  CJK Compatibilit
+00000250: 7920 4964 656f 6772 6170 6873 0a20 2020  y Ideographs.   
+00000260: 2020 2020 2020 2020 2022 5c75 4639 3030           "\uF900
+00000270: 2d5c 7546 4146 4622 2c0a 2020 2020 2020  -\uFAFF",.      
+00000280: 2020 5d0a 2020 2020 290a 2020 2020 2b20    ].    ).    + 
+00000290: 225d 220a 290a 0a23 2053 796d 626f 6c0a  "]".)..# Symbol.
+000002a0: 5359 4d42 4f4c 5f52 4547 4558 203d 2028  SYMBOL_REGEX = (
+000002b0: 0a20 2020 2022 5b22 0a20 2020 202b 2022  .    "[".    + "
+000002c0: 222e 6a6f 696e 280a 2020 2020 2020 2020  ".join(.        
+000002d0: 5b0a 2020 2020 2020 2020 2020 2020 2320  [.            # 
+000002e0: 4261 7369 6320 4c61 7469 6e20 5379 6d62  Basic Latin Symb
+000002f0: 6f6c 0a20 2020 2020 2020 2020 2020 2022  ol.            "
+00000300: 5c75 3030 3231 2d5c 7530 3032 4622 2c0a  \u0021-\u002F",.
+00000310: 2020 2020 2020 2020 2020 2020 225c 7530              "\u0
+00000320: 3033 412d 5c75 3030 3430 222c 0a20 2020  03A-\u0040",.   
+00000330: 2020 2020 2020 2020 2022 5c75 3030 3542           "\u005B
+00000340: 2d5c 7530 3036 3022 2c0a 2020 2020 2020  -\u0060",.      
+00000350: 2020 2020 2020 225c 7530 3037 422d 5c75        "\u007B-\u
+00000360: 3030 3746 222c 0a20 2020 2020 2020 2020  007F",.         
+00000370: 2020 2023 204c 6174 696e 2d31 2053 7570     # Latin-1 Sup
+00000380: 706c 656d 656e 7420 5379 6d62 6f6c 0a20  plement Symbol. 
+00000390: 2020 2020 2020 2020 2020 2022 5c75 3030             "\u00
+000003a0: 4131 2d5c 7530 3042 465c 7530 3044 375c  A1-\u00BF\u00D7\
+000003b0: 7530 3046 3722 2c0a 2020 2020 2020 2020  u00F7",.        
+000003c0: 2020 2020 2320 5370 6163 696e 6720 4d6f      # Spacing Mo
+000003d0: 6469 6669 6572 204c 6574 7465 7273 202d  difier Letters -
+000003e0: 2043 6f6d 6269 6e69 6e67 2044 6961 6372   Combining Diacr
+000003f0: 6974 6963 616c 204d 6172 6b73 0a20 2020  itical Marks.   
+00000400: 2020 2020 2020 2020 2022 5c75 3032 4230           "\u02B0
+00000410: 2d5c 7530 3336 4622 2c0a 2020 2020 2020  -\u036F",.      
+00000420: 2020 2020 2020 2320 5068 6f6e 6574 6963        # Phonetic
+00000430: 2045 7874 656e 7369 6f6e 7320 2d20 436f   Extensions - Co
+00000440: 6d62 696e 696e 6720 4469 6163 7269 7469  mbining Diacriti
+00000450: 6361 6c20 4d61 726b 7320 5375 7070 6c65  cal Marks Supple
+00000460: 6d65 6e74 0a20 2020 2020 2020 2020 2020  ment.           
+00000470: 2022 5c75 3144 3030 2d5c 7531 4446 4622   "\u1D00-\u1DFF"
+00000480: 2c0a 2020 2020 2020 2020 2020 2020 2320  ,.            # 
+00000490: 4765 6e65 7261 6c20 5075 6e63 7475 6174  General Punctuat
+000004a0: 696f 6e20 2d20 4d69 7363 656c 6c61 6e65  ion - Miscellane
+000004b0: 6f75 7320 5379 6d62 6f6c 7320 616e 6420  ous Symbols and 
+000004c0: 4172 726f 7773 0a20 2020 2020 2020 2020  Arrows.         
+000004d0: 2020 2022 5c75 3230 3130 2d5c 7532 4246     "\u2010-\u2BF
+000004e0: 4622 2c0a 2020 2020 2020 2020 2020 2020  F",.            
+000004f0: 2320 5375 7070 6c65 6d65 6e74 616c 2050  # Supplemental P
+00000500: 756e 6374 7561 7469 6f6e 0a20 2020 2020  unctuation.     
+00000510: 2020 2020 2020 2022 5c75 3245 3030 2d5c         "\u2E00-\
+00000520: 7532 4537 4622 2c0a 2020 2020 2020 2020  u2E7F",.        
+00000530: 2020 2020 2320 4964 656f 6772 6170 6869      # Ideographi
+00000540: 6320 4465 7363 7269 7074 696f 6e20 4368  c Description Ch
+00000550: 6172 6163 7465 7273 202d 2043 4a4b 2053  aracters - CJK S
+00000560: 796d 626f 6c73 2061 6e64 2050 756e 6374  ymbols and Punct
+00000570: 7561 7469 6f6e 0a20 2020 2020 2020 2020  uation.         
+00000580: 2020 2022 5c75 3246 4630 2d5c 7533 3033     "\u2FF0-\u303
+00000590: 4622 0a20 2020 2020 2020 2020 2020 2023  F".            #
+000005a0: 2042 6f70 6f6d 6f66 6f20 2d20 434a 4b20   Bopomofo - CJK 
+000005b0: 5374 726f 6b65 730a 2020 2020 2020 2020  Strokes.        
+000005c0: 2020 2020 225c 7533 3130 302d 5c75 3331      "\u3100-\u31
+000005d0: 4546 222c 0a20 2020 2020 2020 2020 2020  EF",.           
+000005e0: 2023 2045 6e63 6c6f 7365 6420 434a 4b20   # Enclosed CJK 
+000005f0: 4c65 7474 6572 7320 616e 6420 4d6f 6e74  Letters and Mont
+00000600: 6873 202d 2043 4a4b 2043 6f6d 7061 7469  hs - CJK Compati
+00000610: 6269 6c69 7479 0a20 2020 2020 2020 2020  bility.         
+00000620: 2020 2022 5c75 3332 3030 2d5c 7533 3346     "\u3200-\u33F
+00000630: 4622 2c0a 2020 2020 2020 2020 2020 2020  F",.            
+00000640: 2320 5969 6a69 6e67 2048 6578 6167 7261  # Yijing Hexagra
+00000650: 6d20 5379 6d62 6f6c 730a 2020 2020 2020  m Symbols.      
+00000660: 2020 2020 2020 225c 7534 4443 302d 5c75        "\u4DC0-\u
+00000670: 3444 4646 222c 0a20 2020 2020 2020 2020  4DFF",.         
+00000680: 2020 2023 204d 6f64 6966 6965 7220 546f     # Modifier To
+00000690: 6e65 204c 6574 7465 7273 0a20 2020 2020  ne Letters.     
+000006a0: 2020 2020 2020 2022 5c75 4137 3030 2d5c         "\uA700-\
+000006b0: 7541 3731 4622 2c0a 2020 2020 2020 2020  uA71F",.        
+000006c0: 2020 2020 2320 4869 6768 2053 7572 726f      # High Surro
+000006d0: 6761 7465 7320 2d20 5072 6976 6174 6520  gates - Private 
+000006e0: 5573 6520 4172 6561 0a20 2020 2020 2020  Use Area.       
+000006f0: 2020 2020 2022 5c75 4438 3030 2d5c 7546       "\uD800-\uF
+00000700: 3846 4622 2c0a 2020 2020 2020 2020 2020  8FF",.          
+00000710: 2020 2320 5661 7269 6174 696f 6e20 5365    # Variation Se
+00000720: 6c65 6374 6f72 7320 2d20 536d 616c 6c20  lectors - Small 
+00000730: 466f 726d 2056 6172 6961 6e74 730a 2020  Form Variants.  
+00000740: 2020 2020 2020 2020 2020 225c 7546 4530            "\uFE0
+00000750: 302d 5c75 4645 3646 222c 0a20 2020 2020  0-\uFE6F",.     
+00000760: 2020 2020 2020 2023 2053 7065 6369 616c         # Special
+00000770: 730a 2020 2020 2020 2020 2020 2020 225c  s.            "\
+00000780: 7546 4646 302d 5c75 4646 4646 222c 0a20  uFFF0-\uFFFF",. 
+00000790: 2020 2020 2020 205d 0a20 2020 2029 0a20         ].    ). 
+000007a0: 2020 202b 2022 5d22 0a29 0a0a 2320 4861     + "]".)..# Ha
+000007b0: 6c66 7769 6474 6820 616e 6420 4675 6c6c  lfwidth and Full
+000007c0: 7769 6474 680a 4841 4c46 5749 4454 485f  width.HALFWIDTH_
+000007d0: 4153 4349 495f 4348 4152 5320 3d20 2222  ASCII_CHARS = ""
+000007e0: 2e6a 6f69 6e28 5b63 6872 2863 6f64 6529  .join([chr(code)
+000007f0: 2066 6f72 2063 6f64 6520 696e 2072 616e   for code in ran
+00000800: 6765 2830 7830 3032 312c 2030 7830 3037  ge(0x0021, 0x007
+00000810: 4520 2b20 3129 5d29 0a46 554c 4c57 4944  E + 1)]).FULLWID
+00000820: 5448 5f41 5343 4949 5f43 4841 5253 203d  TH_ASCII_CHARS =
+00000830: 2022 222e 6a6f 696e 285b 6368 7228 636f   "".join([chr(co
+00000840: 6465 2920 666f 7220 636f 6465 2069 6e20  de) for code in 
+00000850: 7261 6e67 6528 3078 4646 3031 2c20 3078  range(0xFF01, 0x
+00000860: 4646 3545 202b 2031 295d 290a 0a23 204c  FF5E + 1)])..# L
+00000870: 616e 6775 6167 6573 0a4a 4150 414e 4553  anguages.JAPANES
+00000880: 455f 5245 4745 5820 3d20 7266 2228 3f3a  E_REGEX = rf"(?:
+00000890: 7b48 4952 4147 414e 415f 5245 4745 587d  {HIRAGANA_REGEX}
+000008a0: 7c7b 4b41 5441 4b41 4e41 5f52 4547 4558  |{KATAKANA_REGEX
+000008b0: 7d7c 7b4b 414e 4a49 5f52 4547 4558 7d29  }|{KANJI_REGEX})
+000008c0: 220a 454e 474c 4953 485f 5245 4745 5820  ".ENGLISH_REGEX 
+000008d0: 3d20 7266 2228 3f3a 7b41 4c50 4841 4245  = rf"(?:{ALPHABE
+000008e0: 545f 5245 4745 587d 2922 0a0a 2320 4368  T_REGEX})"..# Ch
+000008f0: 6172 6163 7465 7220 7265 7175 6972 696e  aracter requirin
+00000900: 6720 6e6f 6e2d 7370 6163 6520 6265 7477  g non-space betw
+00000910: 6565 6e0a 4e4f 5350 4143 455f 5245 4745  een.NOSPACE_REGE
+00000920: 5820 3d20 280a 2020 2020 2228 3f3a 220a  X = (.    "(?:".
+00000930: 2020 2020 2b20 227c 222e 6a6f 696e 285b      + "|".join([
+00000940: 4849 5241 4741 4e41 5f52 4547 4558 2c20  HIRAGANA_REGEX, 
+00000950: 4b41 5441 4b41 4e41 5f52 4547 4558 2c20  KATAKANA_REGEX, 
+00000960: 4b41 4e4a 495f 5245 4745 582c 204e 554d  KANJI_REGEX, NUM
+00000970: 4245 525f 5245 4745 582c 2022 2d22 5d29  BER_REGEX, "-"])
+00000980: 0a20 2020 202b 2022 2922 0a29 0a         .    + ")".).
```

### Comparing `py-pdf-term-0.18.1/py_pdf_term/analysis/_analysis/concats/lr.py` & `py_pdf_term-1.0.0/py_pdf_term/analysis/_analysis/concats/lr.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,37 +1,66 @@
 from dataclasses import dataclass
 from typing import Dict
 
-from py_pdf_term._common.data import Term
 from py_pdf_term.candidates import DomainCandidateTermList
-
+from py_pdf_term.tokenizers import Term
 
 from ..runner import AnalysisRunner
 
 
 @dataclass(frozen=True)
 class DomainLeftRightFrequency:
+    """Domain name and left/right frequency of the domain.
+
+    Args
+    ----
+        domain:
+            Domain name. (e.g., "natural language processing")
+        left_freq:
+            Number of occurrences of lemmatized (left, token) in the domain.
+            If token or left is meaningless, this is fixed at zero.
+        right_freq:
+            Number of occurrences of lemmatized (token, right) in the domain.
+            If token or right is meaningless, this is fixed at zero.
+    """
+
     domain: str
-    # unique domain name
     left_freq: Dict[str, Dict[str, int]]
-    # number of occurrences of lemmatized (left, token) in the domain
-    # if token or left is meaningless, this is fixed at zero
     right_freq: Dict[str, Dict[str, int]]
-    # number of occurrences of lemmatized (token, right) in the domain
-    # if token or right is meaningless, this is fixed at zero
 
 
 class TermLeftRightFrequencyAnalyzer:
+    """Analyze left/right frequency of terms in a domain.
+
+    Args
+    ----
+        ignore_augmented:
+            If True, ignore augmented terms. The default is True.
+    """
+
     def __init__(self, ignore_augmented: bool = True) -> None:
         self._ignore_augmented = ignore_augmented
         self._runner = AnalysisRunner(ignore_augmented=ignore_augmented)
 
     def analyze(
         self, domain_candidates: DomainCandidateTermList
     ) -> DomainLeftRightFrequency:
+        """Analyze left/right frequency of terms in a domain.
+
+        Args
+        ----
+            domain_candidates:
+                List of candidate terms in a domain. The target of analysis.
+
+        Returns
+        -------
+            DomainLeftRightFrequency:
+                Domain name and left/right frequency of candidate terms in the domain.
+        """
+
         def update(
             lrfreq: DomainLeftRightFrequency,
             pdf_id: int,
             page_num: int,
             candidate: Term,
         ) -> None:
             num_tokens = len(candidate.tokens)
```

### Comparing `py-pdf-term-0.18.1/py_pdf_term/analysis/_analysis/cooccurrences/container.py` & `py_pdf_term-1.0.0/py_pdf_term/analysis/_analysis/cooccurrences/container.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,33 +1,62 @@
 from dataclasses import dataclass
 from typing import Dict, Set
 
-from py_pdf_term._common.data import Term
 from py_pdf_term.candidates import DomainCandidateTermList
+from py_pdf_term.tokenizers import Term
 
 from ..runner import AnalysisRunner
 
 
 @dataclass(frozen=True)
 class DomainContainerTerms:
+    """Domain name and container terms of the domain.
+
+    Args
+    ----
+        domain:
+            Domain name. (e.g., "natural language processing")
+        container_terms:
+            Set of lemmatized containers of the lemmatized term in the domain.
+            (term, container) is valid if and only if the container contains the term as
+            a proper subsequence.
+    """
+
     domain: str
-    # unique domain name
     container_terms: Dict[str, Set[str]]
-    # set of lemmatized containers of the lemmatized term in the domain
-    # (term, container) is valid iff the container contains the term
-    # as a proper subsequence
 
 
 class ContainerTermsAnalyzer:
+    """Analyze container terms of the domain.
+
+    Args
+    ----
+        ignore_augmented:
+            If True, ignore augmented terms. The default is True.
+    """
+
     def __init__(self, ignore_augmented: bool = True) -> None:
         self._runner = AnalysisRunner(ignore_augmented=ignore_augmented)
 
     def analyze(
         self, domain_candidates: DomainCandidateTermList
     ) -> DomainContainerTerms:
+        """Analyze container terms of the domain.
+
+        Args
+        ----
+            domain_candidates:
+                List of candidate terms in a domain. The target of analysis.
+
+        Returns
+        -------
+            DomainContainerTerms:
+                Domain name and container terms of candidate terms in the domain.
+        """
+
         domain_candidates_set = domain_candidates.to_candidates_str_set(
             lambda candidate: candidate.lemma()
         )
 
         def update(
             container_terms: DomainContainerTerms,
             pdf_id: int,
```

### Comparing `py-pdf-term-0.18.1/py_pdf_term/analysis/_analysis/runner.py` & `py_pdf_term-1.0.0/py_pdf_term/analysis/_analysis/runner.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Callable, TypeVar
 
-from py_pdf_term._common.data import Term
 from py_pdf_term.candidates import DomainCandidateTermList
+from py_pdf_term.tokenizers import Term
 
 AnalysisResult = TypeVar("AnalysisResult")
 
 
 class AnalysisRunner:
     def __init__(self, ignore_augmented: bool = True) -> None:
         self._ignore_augmented = ignore_augmented
```

### Comparing `py-pdf-term-0.18.1/py_pdf_term/candidates/_candidates/classifiers/english.py` & `py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/classifiers/english.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,15 @@
-from py_pdf_term.tokenizer import Token
+from py_pdf_term.tokenizers import Token
+
 from .base import BaseTokenClassifier
 
 
 class EnglishTokenClassifier(BaseTokenClassifier):
+    """A token classifier for English tokens."""
+
     def inscope(self, token: Token) -> bool:
         return token.lang == "en"
 
     def is_symbol(self, token: Token) -> bool:
         return token.pos in {"SYM"}
 
     def is_connector_symbol(self, token: Token) -> bool:
```

### Comparing `py-pdf-term-0.18.1/py_pdf_term/candidates/_candidates/classifiers/japanese.py` & `py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/classifiers/japanese.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,12 +1,15 @@
-from py_pdf_term.tokenizer import Token
+from py_pdf_term.tokenizers import Token
+
 from .base import BaseTokenClassifier
 
 
 class JapaneseTokenClassifier(BaseTokenClassifier):
+    """A token classifier for Japanese tokens."""
+
     def inscope(self, token: Token) -> bool:
         return token.lang == "ja"
 
     def is_symbol(self, token: Token) -> bool:
         return token.pos in {"補助記号"}
 
     def is_connector_symbol(self, token: Token) -> bool:
```

### Comparing `py-pdf-term-0.18.1/py_pdf_term/candidates/_candidates/filters/__init__.py` & `py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/filters/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from .combiner import FilterCombiner
 from .term import (
     BaseCandidateTermFilter,
+    BaseEnglishCandidateTermFilter,
+    BaseJapaneseCandidateTermFilter,
     EnglishConcatenationFilter,
     EnglishNumericFilter,
     EnglishProperNounFilter,
     EnglishSymbolLikeFilter,
     JapaneseConcatenationFilter,
     JapaneseNumericFilter,
     JapaneseProperNounFilter,
@@ -12,14 +14,16 @@
 )
 from .token import BaseCandidateTokenFilter, EnglishTokenFilter, JapaneseTokenFilter
 
 # isort: unique-list
 __all__ = [
     "BaseCandidateTermFilter",
     "BaseCandidateTokenFilter",
+    "BaseEnglishCandidateTermFilter",
+    "BaseJapaneseCandidateTermFilter",
     "EnglishConcatenationFilter",
     "EnglishNumericFilter",
     "EnglishProperNounFilter",
     "EnglishSymbolLikeFilter",
     "EnglishTokenFilter",
     "FilterCombiner",
     "JapaneseConcatenationFilter",
```

### Comparing `py-pdf-term-0.18.1/py_pdf_term/candidates/_candidates/filters/combiner.py` & `py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/mappers/candidates/filter.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,67 +1,56 @@
-from typing import List, Optional
+from typing import Type
 
-from py_pdf_term._common.data import Term
-from py_pdf_term.tokenizer import Token
-
-from .term import (
+from py_pdf_term._common.consts import PACKAGE_NAME
+from py_pdf_term.candidates.filters import (
     BaseCandidateTermFilter,
+    BaseCandidateTokenFilter,
     EnglishConcatenationFilter,
     EnglishNumericFilter,
     EnglishProperNounFilter,
     EnglishSymbolLikeFilter,
+    EnglishTokenFilter,
     JapaneseConcatenationFilter,
     JapaneseNumericFilter,
     JapaneseProperNounFilter,
     JapaneseSymbolLikeFilter,
+    JapaneseTokenFilter,
 )
-from .token import BaseCandidateTokenFilter, EnglishTokenFilter, JapaneseTokenFilter
 
+from ..base import BaseMapper
+
+
+class CandidateTokenFilterMapper(BaseMapper[Type[BaseCandidateTokenFilter]]):
+    """A mapper to find candidate token filter classes."""
+
+    @classmethod
+    def default_mapper(cls) -> "CandidateTokenFilterMapper":
+        default_mapper = cls()
+
+        token_filter_clses = [JapaneseTokenFilter, EnglishTokenFilter]
+        for filter_cls in token_filter_clses:
+            default_mapper.add(f"{PACKAGE_NAME}.{filter_cls.__name__}", filter_cls)
+
+        return default_mapper
+
+
+class CandidateTermFilterMapper(BaseMapper[Type[BaseCandidateTermFilter]]):
+    """A mapper to find candidate term filter classes."""
+
+    @classmethod
+    def default_mapper(cls) -> "CandidateTermFilterMapper":
+        default_mapper = cls()
+
+        term_filter_clses = [
+            JapaneseConcatenationFilter,
+            EnglishConcatenationFilter,
+            JapaneseSymbolLikeFilter,
+            EnglishSymbolLikeFilter,
+            JapaneseProperNounFilter,
+            EnglishProperNounFilter,
+            JapaneseNumericFilter,
+            EnglishNumericFilter,
+        ]
+        for filter_cls in term_filter_clses:
+            default_mapper.add(f"{PACKAGE_NAME}.{filter_cls.__name__}", filter_cls)
 
-class FilterCombiner:
-    def __init__(
-        self,
-        token_filters: Optional[List[BaseCandidateTokenFilter]] = None,
-        term_filters: Optional[List[BaseCandidateTermFilter]] = None,
-    ) -> None:
-        if token_filters is None:
-            token_filters = [
-                JapaneseTokenFilter(),
-                EnglishTokenFilter(),
-            ]
-        if term_filters is None:
-            term_filters = [
-                JapaneseConcatenationFilter(),
-                EnglishConcatenationFilter(),
-                JapaneseSymbolLikeFilter(),
-                EnglishSymbolLikeFilter(),
-                JapaneseProperNounFilter(),
-                EnglishProperNounFilter(),
-                JapaneseNumericFilter(),
-                EnglishNumericFilter(),
-            ]
-
-        self._token_filters = token_filters
-        self._term_filters = term_filters
-
-    def is_partof_candidate(self, tokens: List[Token], idx: int) -> bool:
-        token = tokens[idx]
-        if all(map(lambda mf: not mf.inscope(token), self._token_filters)):
-            return False
-
-        return all(
-            map(
-                lambda mf: not mf.inscope(token) or mf.is_partof_candidate(tokens, idx),
-                self._token_filters,
-            )
-        )
-
-    def is_candidate(self, term: Term) -> bool:
-        if all(map(lambda tf: not tf.inscope(term), self._term_filters)):
-            return False
-
-        return all(
-            map(
-                lambda tf: not tf.inscope(term) or tf.is_candidate(term),
-                self._term_filters,
-            )
-        )
+        return default_mapper
```

### Comparing `py-pdf-term-0.18.1/py_pdf_term/candidates/_candidates/filters/term/__init__.py` & `py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/filters/term/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,22 @@
-from .base import BaseCandidateTermFilter
+from .base import (
+    BaseCandidateTermFilter,
+    BaseEnglishCandidateTermFilter,
+    BaseJapaneseCandidateTermFilter,
+)
 from .concatenation import EnglishConcatenationFilter, JapaneseConcatenationFilter
 from .numeric import EnglishNumericFilter, JapaneseNumericFilter
 from .propernoun import EnglishProperNounFilter, JapaneseProperNounFilter
 from .symbollike import EnglishSymbolLikeFilter, JapaneseSymbolLikeFilter
 
 # isort: unique-list
 __all__ = [
     "BaseCandidateTermFilter",
+    "BaseEnglishCandidateTermFilter",
+    "BaseJapaneseCandidateTermFilter",
     "EnglishConcatenationFilter",
     "EnglishNumericFilter",
     "EnglishProperNounFilter",
     "EnglishSymbolLikeFilter",
     "JapaneseConcatenationFilter",
     "JapaneseNumericFilter",
     "JapaneseProperNounFilter",
```

### Comparing `py-pdf-term-0.18.1/py_pdf_term/candidates/_candidates/filters/term/base.py` & `py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/filters/term/propernoun/japanese.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,28 @@
-import re
-from abc import ABCMeta, abstractmethod
+from py_pdf_term.tokenizers import Term, Token
 
-from py_pdf_term._common.consts import ENGLISH_REGEX, JAPANESE_REGEX, NUMBER_REGEX
-from py_pdf_term._common.data import Term
+from ....classifiers import JapaneseTokenClassifier
+from ..base import BaseJapaneseCandidateTermFilter
 
 
-class BaseCandidateTermFilter(metaclass=ABCMeta):
-    def __init__(self) -> None:
-        pass
+class JapaneseProperNounFilter(BaseJapaneseCandidateTermFilter):
+    """A term filter to remove Japanese proper nouns from candidate terms."""
 
-    @abstractmethod
-    def inscope(self, term: Term) -> bool:
-        raise NotImplementedError(f"{self.__class__.__name__}.inscope()")
+    def __init__(self) -> None:
+        self._classifier = JapaneseTokenClassifier()
 
-    @abstractmethod
     def is_candidate(self, scoped_term: Term) -> bool:
-        raise NotImplementedError(f"{self.__class__.__name__}.is_candidate()")
-
-
-class BaseJapaneseCandidateTermFilter(BaseCandidateTermFilter):
-    def inscope(self, term: Term) -> bool:
-        regex = re.compile(rf"({ENGLISH_REGEX}|{JAPANESE_REGEX}|{NUMBER_REGEX}|\s|\-)+")
-        return term.lang == "ja" and regex.fullmatch(str(term)) is not None
+        return not self._is_region_or_person(scoped_term)
 
+    def _is_region_or_person(self, scoped_term: Term) -> bool:
+        def is_region_or_person_token(token: Token) -> bool:
+            return (
+                (
+                    token.pos == "名詞"
+                    and token.category == "固有名詞"
+                    and token.subcategory in {"人名", "地名"}
+                )
+                or self._classifier.is_connector_term(token)
+                or self._classifier.is_connector_symbol(token)
+            )
 
-class BaseEnglishCandidateTermFilter(BaseCandidateTermFilter):
-    def inscope(self, term: Term) -> bool:
-        regex = re.compile(rf"({ENGLISH_REGEX}|{NUMBER_REGEX}|\s|\-)+")
-        return term.lang == "en" and regex.fullmatch(str(term)) is not None
+        return all(map(is_region_or_person_token, scoped_term.tokens))
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `py-pdf-term-0.18.1/py_pdf_term/candidates/_candidates/filters/term/concatenation/english.py` & `py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/filters/term/concatenation/english.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import re
 
 from py_pdf_term._common.consts import ALPHABET_REGEX
-from py_pdf_term._common.data import Term
-from ....classifiers import EnglishTokenClassifier
+from py_pdf_term.tokenizers import Term
 
+from ....classifiers import EnglishTokenClassifier
 from ..base import BaseEnglishCandidateTermFilter
 
 PHONETIC_REGEX = ALPHABET_REGEX
 
 
 class EnglishConcatenationFilter(BaseEnglishCandidateTermFilter):
+    """A candidate term filter to filter out invalidly concatenated English terms."""
+
     def __init__(self) -> None:
         self._classifier = EnglishTokenClassifier()
 
     def is_candidate(self, scoped_term: Term) -> bool:
         return (
             self._is_norn_phrase(scoped_term)
             and not self._has_invalid_connector_symbol(scoped_term)
```

### Comparing `py-pdf-term-0.18.1/py_pdf_term/candidates/_candidates/filters/term/concatenation/japanese.py` & `py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/filters/term/concatenation/japanese.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 import re
 
 from py_pdf_term._common.consts import ALPHABET_REGEX, HIRAGANA_REGEX, KATAKANA_REGEX
-from py_pdf_term._common.data import Term
-from ....classifiers import JapaneseTokenClassifier
+from py_pdf_term.tokenizers import Term
 
+from ....classifiers import JapaneseTokenClassifier
 from ..base import BaseJapaneseCandidateTermFilter
 
 PHONETIC_REGEX = rf"{HIRAGANA_REGEX}|{KATAKANA_REGEX}|{ALPHABET_REGEX}"
 
 
 class JapaneseConcatenationFilter(BaseJapaneseCandidateTermFilter):
+    """A candidate term filter to filter out invalidly concatenated Japanese terms."""
+
     def __init__(self) -> None:
         self._classifier = JapaneseTokenClassifier()
 
     def is_candidate(self, scoped_term: Term) -> bool:
         return (
             self._is_norn_phrase(scoped_term)
             and not self._has_invalid_connector_symbol(scoped_term)
```

### Comparing `py-pdf-term-0.18.1/py_pdf_term/candidates/_candidates/filters/term/numeric/english.py` & `py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/mappers/candidates/classifier.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,29 @@
-from py_pdf_term._common.data import Term
-from py_pdf_term.tokenizer import Token
-from ....classifiers import EnglishTokenClassifier
+from typing import Type
 
-from ..base import BaseEnglishCandidateTermFilter
+from py_pdf_term._common.consts import PACKAGE_NAME
+from py_pdf_term.candidates.classifiers import (
+    BaseTokenClassifier,
+    EnglishTokenClassifier,
+    JapaneseTokenClassifier,
+)
+
+from ..base import BaseMapper
+
+
+class TokenClassifierMapper(BaseMapper[Type[BaseTokenClassifier]]):
+    """A mapper to find token classifier classes."""
+
+    @classmethod
+    def default_mapper(cls) -> "TokenClassifierMapper":
+        default_mapper = cls()
+
+        classifier_clses = [
+            JapaneseTokenClassifier,
+            EnglishTokenClassifier,
+        ]
+        for classifier_cls in classifier_clses:
+            default_mapper.add(
+                f"{PACKAGE_NAME}.{classifier_cls.__name__}", classifier_cls
+            )
 
-
-class EnglishNumericFilter(BaseEnglishCandidateTermFilter):
-    def __init__(self) -> None:
-        self._classifier = EnglishTokenClassifier()
-
-    def is_candidate(self, scoped_term: Term) -> bool:
-        return not self._is_numeric_phrase(scoped_term)
-
-    def _is_numeric_phrase(self, scoped_term: Term) -> bool:
-        def is_numeric_or_meaningless(token: Token) -> bool:
-            return token.pos == "NUM" or self._classifier.is_meaningless(token)
-
-        return all(map(is_numeric_or_meaningless, scoped_term.tokens))
+        return default_mapper
```

### Comparing `py-pdf-term-0.18.1/py_pdf_term/candidates/_candidates/filters/term/numeric/japanese.py` & `py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/filters/term/numeric/japanese.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-from py_pdf_term._common.data import Term
-from py_pdf_term.tokenizer import Token
-from ....classifiers import JapaneseTokenClassifier
+from py_pdf_term.tokenizers import Term, Token
 
+from ....classifiers import JapaneseTokenClassifier
 from ..base import BaseJapaneseCandidateTermFilter
 
 
 class JapaneseNumericFilter(BaseJapaneseCandidateTermFilter):
+    """A term filter to remove Japanese numeric phrases from candidate terms."""
+
     def __init__(self) -> None:
         self._classifier = JapaneseTokenClassifier()
 
     def is_candidate(self, scoped_term: Term) -> bool:
         return not self._is_numeric_phrase(scoped_term)
 
     def _is_numeric_phrase(self, scoped_term: Term) -> bool:
```

### Comparing `py-pdf-term-0.18.1/py_pdf_term/candidates/_candidates/filters/term/symbollike/english.py` & `py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/filters/term/symbollike/english.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 import re
 
 from py_pdf_term._common.consts import ALPHABET_REGEX, NUMBER_REGEX
-from py_pdf_term._common.data import Term
-from py_pdf_term.tokenizer import Token
-from ....classifiers import EnglishTokenClassifier
+from py_pdf_term.tokenizers import Term, Token
 
+from ....classifiers import EnglishTokenClassifier
 from ..base import BaseEnglishCandidateTermFilter
 
 PHONETIC_REGEX = ALPHABET_REGEX
 
 
 class EnglishSymbolLikeFilter(BaseEnglishCandidateTermFilter):
+    """A candidate term filter to filter out symbol-like English terms."""
+
     def __init__(self) -> None:
         self._classifier = EnglishTokenClassifier()
         self._phonetic_regex = re.compile(PHONETIC_REGEX)
         self._indexed_phonetic_regex = re.compile(
             rf"({PHONETIC_REGEX}{NUMBER_REGEX}+)+{PHONETIC_REGEX}?"
             + "|"
             + rf"({NUMBER_REGEX}+{PHONETIC_REGEX})+({NUMBER_REGEX}+)?"
```

### Comparing `py-pdf-term-0.18.1/py_pdf_term/candidates/_candidates/filters/term/symbollike/japanese.py` & `py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/filters/term/symbollike/japanese.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,24 +2,25 @@
 
 from py_pdf_term._common.consts import (
     ALPHABET_REGEX,
     HIRAGANA_REGEX,
     KATAKANA_REGEX,
     NUMBER_REGEX,
 )
-from py_pdf_term._common.data import Term
-from py_pdf_term.tokenizer import Token
-from ....classifiers import JapaneseTokenClassifier
+from py_pdf_term.tokenizers import Term, Token
 
+from ....classifiers import JapaneseTokenClassifier
 from ..base import BaseJapaneseCandidateTermFilter
 
 PHONETIC_REGEX = rf"(?:{HIRAGANA_REGEX}|{KATAKANA_REGEX}|{ALPHABET_REGEX})"
 
 
 class JapaneseSymbolLikeFilter(BaseJapaneseCandidateTermFilter):
+    """A candidate term filter to filter out symbol-like Japanese terms."""
+
     def __init__(self) -> None:
         self._classifier = JapaneseTokenClassifier()
         self._phonetic_regex = re.compile(PHONETIC_REGEX)
         self._indexed_phonetic_regex = re.compile(
             rf"({PHONETIC_REGEX}{NUMBER_REGEX}+)+{PHONETIC_REGEX}?"
             + "|"
             + rf"({NUMBER_REGEX}+{PHONETIC_REGEX})+({NUMBER_REGEX}+)?"
```

### Comparing `py-pdf-term-0.18.1/py_pdf_term/candidates/_candidates/filters/token/english.py` & `py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/filters/token/english.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 import re
 from typing import List
 
 from py_pdf_term._common.consts import ENGLISH_REGEX, NUMBER_REGEX
-from py_pdf_term.tokenizer import Token
+from py_pdf_term.tokenizers import Token
 
 from .base import BaseCandidateTokenFilter
 
 
 class EnglishTokenFilter(BaseCandidateTokenFilter):
+    """A candidate token filter to filter out English tokens which cannot be part of
+    candidate terms.
+    """
+
     def __init__(self) -> None:
         self._regex = re.compile(rf"({ENGLISH_REGEX}|{NUMBER_REGEX})+")
 
     def inscope(self, token: Token) -> bool:
         token_str = str(token)
         return token.lang == "en" and (
             self._regex.fullmatch(token_str) is not None or token_str == "-"
```

### Comparing `py-pdf-term-0.18.1/py_pdf_term/candidates/_candidates/filters/token/japanese.py` & `py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/filters/token/japanese.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 import re
 from typing import List
 
 from py_pdf_term._common.consts import ENGLISH_REGEX, JAPANESE_REGEX, NUMBER_REGEX
-from py_pdf_term.tokenizer import Token
+from py_pdf_term.tokenizers import Token
 
 from .base import BaseCandidateTokenFilter
 
 
 class JapaneseTokenFilter(BaseCandidateTokenFilter):
+    """A candidate token filter to filter out Japanese tokens which cannot be part of
+    candidate terms.
+    """
+
     def __init__(self) -> None:
         self._regex = re.compile(rf"({JAPANESE_REGEX}|{ENGLISH_REGEX}|{NUMBER_REGEX})+")
 
     def inscope(self, token: Token) -> bool:
         token_str = str(token)
         return token.lang == "ja" and (
             self._regex.fullmatch(token_str) is not None or token_str == "-"
```

### Comparing `py-pdf-term-0.18.1/py_pdf_term/candidates/_candidates/splitters/base.py` & `py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/filters/term/numeric/english.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,20 @@
-from abc import ABCMeta, abstractmethod
-from typing import List, Optional
+from py_pdf_term.tokenizers import Term, Token
 
-from py_pdf_term._common.data import Term
-from ..classifiers import (
-    BaseTokenClassifier,
-    EnglishTokenClassifier,
-    JapaneseTokenClassifier,
-)
-
-
-class BaseSplitter(metaclass=ABCMeta):
-    def __init__(self, classifiers: Optional[List[BaseTokenClassifier]] = None) -> None:
-        if classifiers is None:
-            classifiers = [
-                JapaneseTokenClassifier(),
-                EnglishTokenClassifier(),
-            ]
-
-        self._classifiers = classifiers
-
-    @abstractmethod
-    def split(self, term: Term) -> List[Term]:
-        raise NotImplementedError(f"{self.__class__.__name__}.split()")
+from ....classifiers import EnglishTokenClassifier
+from ..base import BaseEnglishCandidateTermFilter
+
+
+class EnglishNumericFilter(BaseEnglishCandidateTermFilter):
+    """A term filter to remove English numeric phrases from candidate terms."""
+
+    def __init__(self) -> None:
+        self._classifier = EnglishTokenClassifier()
+
+    def is_candidate(self, scoped_term: Term) -> bool:
+        return not self._is_numeric_phrase(scoped_term)
+
+    def _is_numeric_phrase(self, scoped_term: Term) -> bool:
+        def is_numeric_or_meaningless(token: Token) -> bool:
+            return token.pos == "NUM" or self._classifier.is_meaningless(token)
+
+        return all(map(is_numeric_or_meaningless, scoped_term.tokens))
```

### Comparing `py-pdf-term-0.18.1/py_pdf_term/candidates/_candidates/splitters/repeat.py` & `py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/splitters/repeat.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,27 @@
-from typing import List, Tuple, Optional
+from typing import List, Optional, Tuple
 
-from py_pdf_term._common.data import Term
+from py_pdf_term.tokenizers import Term
 
-from .base import BaseSplitter
 from ..classifiers import BaseTokenClassifier
+from .base import BaseSplitter
 
 
 class RepeatSplitter(BaseSplitter):
+    """A splitter to split a term by repeated tokens. For example, "quick sort merge
+    sort heap sort" is split into "quick sort", "merge sort", and "heap sort".
+
+    Args
+    ----
+        classifiers:
+            A list of token classifiers to classify tokens into specific categories.
+            If None, the default classifiers are used. The default classifiers are
+            JapaneseTokenClassifier and EnglishTokenClassifier.
+    """
+
     def __init__(self, classifiers: Optional[List[BaseTokenClassifier]] = None) -> None:
         super().__init__(classifiers=classifiers)
 
     def split(self, term: Term) -> List[Term]:
         if self._contains_connector_token(term):
             return [term]
```

### Comparing `py-pdf-term-0.18.1/py_pdf_term/candidates/_candidates/utils.py` & `py_pdf_term-1.0.0/py_pdf_term/candidates/_candidates/utils.py`

 * *Files identical despite different names*

### Comparing `py-pdf-term-0.18.1/py_pdf_term/endtoend/_endtoend/caches/__init__.py` & `py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/caches/__init__.py`

 * *Files identical despite different names*

### Comparing `py-pdf-term-0.18.1/py_pdf_term/endtoend/_endtoend/caches/candidate/file.py` & `py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/caches/candidate/file.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,22 @@
 
 from ...configs import CandidateLayerConfig
 from ..util import create_dir_name_from_config, create_file_name_from_path
 from .base import BaseCandidateLayerCache
 
 
 class CandidateLayerFileCache(BaseCandidateLayerCache):
+    """A candidate layer cache that stores and loads candidate terms to/from a file.
+
+    Args
+    ----
+        cache_dir:
+            The directory path to store cache files.
+    """
+
     def __init__(self, cache_dir: str) -> None:
         super().__init__(cache_dir)
         self._cache_dir = cache_dir
 
     def load(
         self, pdf_path: str, config: CandidateLayerConfig
     ) -> Union[PDFCandidateTermList, None]:
@@ -40,15 +48,15 @@
         dir_name = create_dir_name_from_config(config)
         file_name = create_file_name_from_path(candidates.pdf_path, "json")
         cache_file_path = os.path.join(self._cache_dir, dir_name, file_name)
 
         os.makedirs(os.path.dirname(cache_file_path), exist_ok=True)
 
         with open(cache_file_path, "w") as json_file:
-            json.dump(candidates.to_dict(), json_file, ensure_ascii=False, indent=2)
+            json.dump(candidates.to_dict(), json_file, ensure_ascii=False)
 
     def remove(self, pdf_path: str, config: CandidateLayerConfig) -> None:
         dir_name = create_dir_name_from_config(config)
         file_name = create_file_name_from_path(pdf_path, "json")
         cache_dir_path = os.path.join(self._cache_dir, dir_name)
         cache_file_path = os.path.join(cache_dir_path, file_name)
```

### Comparing `py-pdf-term-0.18.1/py_pdf_term/endtoend/_endtoend/caches/method/file.py` & `py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/caches/method/file.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,28 +3,36 @@
 from glob import glob
 from shutil import rmtree
 from typing import Any, Callable, Dict, List, Union
 
 from py_pdf_term.methods import MethodTermRanking
 from py_pdf_term.methods._methods.rankingdata import RankingData
 
-from ...configs import MethodLayerConfig
+from ...configs import BaseMethodLayerConfig
 from ..util import create_dir_name_from_config, create_file_name_from_paths
 from .base import BaseMethodLayerDataCache, BaseMethodLayerRankingCache
 
 
 class MethodLayerRankingFileCache(BaseMethodLayerRankingCache):
+    """A method layer ranking cache that stores and loads term rankings to/from a file.
+
+    Args
+    ----
+        cache_dir:
+            The directory path to store cache files.
+    """
+
     def __init__(self, cache_dir: str) -> None:
         super().__init__(cache_dir)
         self._cache_dir = cache_dir
 
     def load(
         self,
         pdf_paths: List[str],
-        config: MethodLayerConfig,
+        config: BaseMethodLayerConfig,
     ) -> Union[MethodTermRanking, None]:
         dir_name = create_dir_name_from_config(config, prefix="rank")
         file_name = create_file_name_from_paths(pdf_paths, "json")
         cache_file_path = os.path.join(self._cache_dir, dir_name, file_name)
 
         if not os.path.isfile(cache_file_path):
             return None
@@ -37,26 +45,26 @@
 
         return MethodTermRanking.from_dict(obj)
 
     def store(
         self,
         pdf_paths: List[str],
         term_ranking: MethodTermRanking,
-        config: MethodLayerConfig,
+        config: BaseMethodLayerConfig,
     ) -> None:
         dir_name = create_dir_name_from_config(config, prefix="rank")
         file_name = create_file_name_from_paths(pdf_paths, "json")
         cache_file_path = os.path.join(self._cache_dir, dir_name, file_name)
 
         os.makedirs(os.path.dirname(cache_file_path), exist_ok=True)
 
         with open(cache_file_path, "w") as json_file:
-            json.dump(term_ranking.to_dict(), json_file, ensure_ascii=False, indent=2)
+            json.dump(term_ranking.to_dict(), json_file, ensure_ascii=False)
 
-    def remove(self, pdf_paths: List[str], config: MethodLayerConfig) -> None:
+    def remove(self, pdf_paths: List[str], config: BaseMethodLayerConfig) -> None:
         dir_name = create_dir_name_from_config(config, prefix="rank")
         file_name = create_file_name_from_paths(pdf_paths, "json")
         cache_dir_path = os.path.join(self._cache_dir, dir_name)
         cache_file_path = os.path.join(cache_dir_path, file_name)
 
         if not os.path.isfile(cache_file_path):
             return
@@ -65,52 +73,64 @@
 
         cache_file_paths = glob(os.path.join(cache_dir_path, "*.json"))
         if not cache_file_paths:
             rmtree(cache_dir_path)
 
 
 class MethodLayerDataFileCache(BaseMethodLayerDataCache[RankingData]):
+    """A method layer data cache that stores and loads metadata to to generate term
+    rankings to/from a file.
+
+    Args
+    ----
+        cache_dir:
+            The directory path to store cache files.
+    """
+
     def __init__(self, cache_dir: str) -> None:
         super().__init__(cache_dir)
         self._cache_dir = cache_dir
 
     def load(
         self,
         pdf_paths: List[str],
-        config: MethodLayerConfig,
+        config: BaseMethodLayerConfig,
         from_dict: Callable[[Dict[str, Any]], RankingData],
     ) -> Union[RankingData, None]:
         dir_name = create_dir_name_from_config(config, prefix="data")
         file_name = create_file_name_from_paths(pdf_paths, "json")
         cache_file_path = os.path.join(self._cache_dir, dir_name, file_name)
 
         if not os.path.isfile(cache_file_path):
             return None
 
         with open(cache_file_path, "r") as json_file:
-            obj = json.load(json_file)
+            try:
+                obj = json.load(json_file)
+            except json.JSONDecodeError:
+                return None
 
         return from_dict(obj)
 
     def store(
         self,
         pdf_paths: List[str],
         ranking_data: RankingData,
-        config: MethodLayerConfig,
+        config: BaseMethodLayerConfig,
     ) -> None:
         dir_name = create_dir_name_from_config(config, prefix="data")
         file_name = create_file_name_from_paths(pdf_paths, "json")
         cache_file_path = os.path.join(self._cache_dir, dir_name, file_name)
 
         os.makedirs(os.path.dirname(cache_file_path), exist_ok=True)
 
         with open(cache_file_path, "w") as json_file:
-            json.dump(ranking_data.to_dict(), json_file, ensure_ascii=False, indent=2)
+            json.dump(ranking_data.to_dict(), json_file, ensure_ascii=False)
 
-    def remove(self, pdf_paths: List[str], config: MethodLayerConfig) -> None:
+    def remove(self, pdf_paths: List[str], config: BaseMethodLayerConfig) -> None:
         dir_name = create_dir_name_from_config(config, prefix="data")
         file_name = create_file_name_from_paths(pdf_paths, "json")
         cache_dir_path = os.path.join(self._cache_dir, dir_name)
         cache_file_path = os.path.join(cache_dir_path, file_name)
 
         if not os.path.isfile(cache_file_path):
             return
```

### Comparing `py-pdf-term-0.18.1/py_pdf_term/endtoend/_endtoend/caches/styling/base.py` & `py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/caches/styling/nocache.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,32 @@
-from abc import ABCMeta, abstractmethod
 from typing import Union
 
 from py_pdf_term.stylings import PDFStylingScoreList
 
 from ...configs import StylingLayerConfig
+from .base import BaseStylingLayerCache
 
 
-class BaseStylingLayerCache(metaclass=ABCMeta):
+class StylingLayerNoCache(BaseStylingLayerCache):
+    """A styling layer cache that does not store and load styling scores.
+
+    Args
+    ----
+        cache_dir:
+            This argument is ignored.
+    """
+
     def __init__(self, cache_dir: str) -> None:
         pass
 
-    @abstractmethod
     def load(
         self, pdf_path: str, config: StylingLayerConfig
     ) -> Union[PDFStylingScoreList, None]:
-        raise NotImplementedError(f"{self.__class__.__name__}.load()")
+        pass
 
-    @abstractmethod
     def store(
         self, styling_scores: PDFStylingScoreList, config: StylingLayerConfig
     ) -> None:
-        raise NotImplementedError(f"{self.__class__.__name__}.store()")
+        pass
 
-    @abstractmethod
     def remove(self, pdf_path: str, config: StylingLayerConfig) -> None:
-        raise NotImplementedError(f"{self.__class__.__name__}.remove()")
+        pass
```

### Comparing `py-pdf-term-0.18.1/py_pdf_term/endtoend/_endtoend/caches/styling/file.py` & `py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/caches/xml/file.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,62 +1,68 @@
-import json
 import os
 from glob import glob
 from shutil import rmtree
 from typing import Union
+from xml.etree.ElementTree import ParseError, fromstring, tostring
 
-from py_pdf_term.stylings import PDFStylingScoreList
+from py_pdf_term.pdftoxml import PDFnXMLElement
 
-from ...configs import StylingLayerConfig
+from ...configs import XMLLayerConfig
 from ..util import create_dir_name_from_config, create_file_name_from_path
-from .base import BaseStylingLayerCache
+from .base import BaseXMLLayerCache
 
 
-class StylingLayerFileCache(BaseStylingLayerCache):
+class XMLLayerFileCache(BaseXMLLayerCache):
+    """A XML layer cache that stores and loads XML elements to/from a file.
+
+    Args
+    ----
+        cache_dir:
+            The directory path to store cache files.
+    """
+
     def __init__(self, cache_dir: str) -> None:
-        super().__init__(cache_dir)
         self._cache_dir = cache_dir
 
     def load(
-        self, pdf_path: str, config: StylingLayerConfig
-    ) -> Union[PDFStylingScoreList, None]:
+        self, pdf_path: str, config: XMLLayerConfig
+    ) -> Union[PDFnXMLElement, None]:
         dir_name = create_dir_name_from_config(config)
-        file_name = create_file_name_from_path(pdf_path, "json")
+        file_name = create_file_name_from_path(pdf_path, "xml")
         cache_file_path = os.path.join(self._cache_dir, dir_name, file_name)
 
         if not os.path.isfile(cache_file_path):
             return None
 
-        with open(cache_file_path, "r") as json_file:
+        with open(cache_file_path, "r") as xml_file:
             try:
-                obj = json.load(json_file)
-            except json.JSONDecodeError:
+                xml_root = fromstring(xml_file.read())
+            except ParseError:
                 return None
 
-        return PDFStylingScoreList.from_dict(obj)
+        return PDFnXMLElement(pdf_path, xml_root)
 
-    def store(
-        self, styling_scores: PDFStylingScoreList, config: StylingLayerConfig
-    ) -> None:
+    def store(self, pdfnxml: PDFnXMLElement, config: XMLLayerConfig) -> None:
         dir_name = create_dir_name_from_config(config)
-        file_name = create_file_name_from_path(styling_scores.pdf_path, "json")
+        file_name = create_file_name_from_path(pdfnxml.pdf_path, "xml")
         cache_file_path = os.path.join(self._cache_dir, dir_name, file_name)
 
         os.makedirs(os.path.dirname(cache_file_path), exist_ok=True)
 
-        with open(cache_file_path, "w") as json_file:
-            json.dump(styling_scores.to_dict(), json_file, ensure_ascii=False, indent=2)
+        with open(cache_file_path, "wb") as xml_file:
+            xml_content = tostring(pdfnxml.xml_root, encoding="utf-8")
+            xml_file.write(xml_content)
 
-    def remove(self, pdf_path: str, config: StylingLayerConfig) -> None:
+    def remove(self, pdf_path: str, config: XMLLayerConfig) -> None:
         dir_name = create_dir_name_from_config(config)
-        file_name = create_file_name_from_path(pdf_path, "json")
+        file_name = create_file_name_from_path(pdf_path, "xml")
         cache_dir_path = os.path.join(self._cache_dir, dir_name)
         cache_file_path = os.path.join(cache_dir_path, file_name)
 
         if not os.path.isfile(cache_file_path):
             return
 
         os.remove(cache_file_path)
 
-        cache_file_paths = glob(os.path.join(cache_dir_path, "*.json"))
+        cache_file_paths = glob(os.path.join(cache_dir_path, "*.xml"))
         if not cache_file_paths:
             rmtree(cache_dir_path)
```

### Comparing `py-pdf-term-0.18.1/py_pdf_term/endtoend/_endtoend/caches/util.py` & `py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/caches/util.py`

 * *Files identical despite different names*

### Comparing `py-pdf-term-0.18.1/py_pdf_term/endtoend/_endtoend/caches/xml/file.py` & `py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/caches/styling/file.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,61 +1,70 @@
+import json
 import os
 from glob import glob
 from shutil import rmtree
 from typing import Union
-from xml.etree.ElementTree import ParseError, fromstring, tostring
 
-from py_pdf_term.pdftoxml import PDFnXMLElement
+from py_pdf_term.stylings import PDFStylingScoreList
 
-from ...configs import XMLLayerConfig
+from ...configs import StylingLayerConfig
 from ..util import create_dir_name_from_config, create_file_name_from_path
-from .base import BaseXMLLayerCache
+from .base import BaseStylingLayerCache
 
 
-class XMLLayerFileCache(BaseXMLLayerCache):
-    def __init__(self, cache_dir: str) -> None:
+class StylingLayerFileCache(BaseStylingLayerCache):
+    """A styling layer cache that stores and loads styling scores to/from a file.
+
+    Args
+    ----
+        cache_dir:
+            The directory path to store cache files.
+    """
 
+    def __init__(self, cache_dir: str) -> None:
+        super().__init__(cache_dir)
         self._cache_dir = cache_dir
 
     def load(
-        self, pdf_path: str, config: XMLLayerConfig
-    ) -> Union[PDFnXMLElement, None]:
+        self, pdf_path: str, config: StylingLayerConfig
+    ) -> Union[PDFStylingScoreList, None]:
         dir_name = create_dir_name_from_config(config)
-        file_name = create_file_name_from_path(pdf_path, "xml")
+        file_name = create_file_name_from_path(pdf_path, "json")
         cache_file_path = os.path.join(self._cache_dir, dir_name, file_name)
 
         if not os.path.isfile(cache_file_path):
             return None
 
-        with open(cache_file_path, "r") as xml_file:
+        with open(cache_file_path, "r") as json_file:
             try:
-                xml_root = fromstring(xml_file.read())
-            except ParseError:
+                obj = json.load(json_file)
+            except json.JSONDecodeError:
                 return None
 
-        return PDFnXMLElement(pdf_path, xml_root)
+        return PDFStylingScoreList.from_dict(obj)
 
-    def store(self, pdfnxml: PDFnXMLElement, config: XMLLayerConfig) -> None:
+    def store(
+        self, styling_scores: PDFStylingScoreList, config: StylingLayerConfig
+    ) -> None:
         dir_name = create_dir_name_from_config(config)
-        file_name = create_file_name_from_path(pdfnxml.pdf_path, "xml")
+        file_name = create_file_name_from_path(styling_scores.pdf_path, "json")
         cache_file_path = os.path.join(self._cache_dir, dir_name, file_name)
 
         os.makedirs(os.path.dirname(cache_file_path), exist_ok=True)
 
-        with open(cache_file_path, "wb") as xml_file:
-            xml_content = tostring(pdfnxml.xml_root, encoding="utf-8")
-            xml_file.write(xml_content)
+        with open(cache_file_path, "w") as json_file:
+            json.dump(styling_scores.to_dict(), json_file, ensure_ascii=False)
 
-    def remove(self, pdf_path: str, config: XMLLayerConfig) -> None:
+    def remove(self, pdf_path: str, config: StylingLayerConfig) -> None:
         dir_name = create_dir_name_from_config(config)
-        file_name = create_file_name_from_path(pdf_path, "xml")
+        file_name = create_file_name_from_path(pdf_path, "json")
         cache_dir_path = os.path.join(self._cache_dir, dir_name)
         cache_file_path = os.path.join(cache_dir_path, file_name)
 
         if not os.path.isfile(cache_file_path):
             return
 
         os.remove(cache_file_path)
 
-        cache_file_paths = glob(os.path.join(cache_dir_path, "*.xml"))
+        cache_file_paths = glob(os.path.join(cache_dir_path, "*.json"))
         if not cache_file_paths:
             rmtree(cache_dir_path)
```

### Comparing `py-pdf-term-0.18.1/py_pdf_term/endtoend/_endtoend/caches/xml/nocache.py` & `py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/caches/xml/nocache.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,14 +3,22 @@
 from py_pdf_term.pdftoxml import PDFnXMLElement
 
 from ...configs import XMLLayerConfig
 from .base import BaseXMLLayerCache
 
 
 class XMLLayerNoCache(BaseXMLLayerCache):
+    """An XML layer cache that does not store and load XML elements.
+
+    Args
+    ----
+        cache_dir:
+            This argument is ignored.
+    """
+
     def __init__(self, cache_dir: str) -> None:
         pass
 
     def load(
         self, pdf_path: str, config: XMLLayerConfig
     ) -> Union[PDFnXMLElement, None]:
         pass
```

### Comparing `py-pdf-term-0.18.1/py_pdf_term/endtoend/_endtoend/configs/base.py` & `py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/configs/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Any, Dict, Type, TypeVar
 
 CACHE_CONFIGS = ["cache", "data_cache", "ranking_cache"]
 
 
 @dataclass(frozen=True)
 class BaseLayerConfig:
-    pass
+    """Base class for layer configuration."""
 
     def to_dict(self) -> Dict[str, Any]:
         return asdict(self)
 
     def to_dict_without_cache(self) -> Dict[str, Any]:
         config_dict = asdict(self)
         for cache_config in CACHE_CONFIGS:
```

### Comparing `py-pdf-term-0.18.1/py_pdf_term/endtoend/_endtoend/extractor.py` & `py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/extractor.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 from typing import List, Optional
 
 from py_pdf_term.techterms import PDFTechnicalTermList
 
 from .caches import DEFAULT_CACHE_DIR
 from .configs import (
     CandidateLayerConfig,
-    MethodLayerConfig,
+    MultiDomainMethodLayerConfig,
+    SingleDomainMethodLayerConfig,
     StylingLayerConfig,
     TechnicalTermLayerConfig,
     XMLLayerConfig,
 )
 from .data import DomainPDFList
 from .layers import (
     CandidateLayer,
-    MethodLayer,
+    MultiDomainMethodLayer,
+    MultiDomainTechnicalTermLayer,
+    SingleDomainMethodLayer,
+    SingleDomainTechnicalTermLayer,
     StylingLayer,
-    TechnicalTermLayer,
     XMLLayer,
 )
 from .mappers import (
     AugmenterMapper,
     BinaryOpenerMapper,
     CandidateLayerCacheMapper,
     CandidateTermFilterMapper,
@@ -28,23 +31,25 @@
     MethodLayerDataCacheMapper,
     MethodLayerRankingCacheMapper,
     MultiDomainRankingMethodMapper,
     SingleDomainRankingMethodMapper,
     SplitterMapper,
     StylingLayerCacheMapper,
     StylingScoreMapper,
-    TokenClassifilerMapper,
+    TokenClassifierMapper,
     XMLLayerCacheMapper,
 )
 
 
-class PyPDFTermExtractor:
-    """Top level class of py-pdf-term. E2E class to extract terminologies from PDF file.
+class PyPDFTermSingleDomainExtractor:
+    """Top level class of py-pdf-term. This class extracts technical terms from a PDF
+    file withoout cross-domain information.
 
-    Args:
+    Args
+    ----
         xml_config:
             Config of XML Layer.
 
         candidate_config:
             Config of Candidate Term Layer.
 
         method_config:
@@ -78,54 +83,222 @@
         term_filter_mapper:
             Mapper from an element in `candidate_config.term_filters` to a class to
             filter terms which are likely to be candidates. This is used in Candidate
             Term Layer.
 
         splitter_mapper:
             Mapper from an element in `candidate_config.splitters` to a class to split
-            too long terms or wrongly concatenated terms. When XML Layer extracts a text
-            from a table, figure or something in a PDF file, texts in them are often
-            wrongly concatenated so that the text looks like one too long candidate
-            term. This is used in Candidate Term Layer.
-            e.g. If a PDF have a table to compare sort algorithms and the header text
-            wanna mean "Selection Sort" | "Quick Sort" | "Merge Sort", the text is
-            recognized as a word like "Selection Sort Quick Sort Merge Sort". This
-            wrongly concatenated word must be split down into three algorithm names.
+            too long terms or wrongly concatenated terms. This is used in Candidate Term
+            Layer.
 
         augmenter_mapper:
             Mapper from an element in `candidate_config.augmenters` to a class to
-            augment candidates. The augumentation means that if a long candidate term is
-            found, sub-terms of the original term could also be candidates. This is used
-            in Candidate Term Layer.
-            e.g. Original long term: "Structure of Layered Architecture". Augmented sub-
-            terms: "Structure" and "Layered Architecture".
+            augment candidates. The augumentation means that if a long candidate is
+            found, sub-terms of it could also be candidates. This is used in Candidate
+            Term Layer.
 
-        single_method_mapper:
+        method_mapper:
             Mapper from `method_config.method` to a class to calculate method scores of
-            candidate terms when `method_config.method_type` equals to "single".
-            A single-domain ranking method is an ranking algorithm which can calculate
-            method scores without cross-domain information.
-            e.g. Term-Frequency algorithm uses only frequency of occurcences of terms.
-            Therefore, TF is a single-domain ranking method.
+            candidate terms. This is used in Method Layer.
+
+        styling_score_mapper:
+            Mapper from an element in `styling_config.styling_scores` to a class to
+            calculate scores of candidate terms based on their styling such as color,
+            fontsize and so on. This is used in Styling Layer.
+
+        xml_cache_mapper:
+            Mapper from `xml_config.cache` to a class to provide XML Layer with the
+            cache  mechanism. The xml cache manages XML files converted from input PDF
+            files.
+
+        candidate_cache_mapper:
+            Mapper from `candidate_config.cache` to a class to provide Candidate Term
+            Layer with the cache mechanism. The candidate cache manages lists of
+            candidate terms.
+
+        method_ranking_cache_mapper:
+            Mapper from `method_config.ranking_cache` to a class to provide Method Layer
+            with the cache mechanism. The method ranking cache manages candidate terms
+            ordered by the method scores.
+
+        method_data_cache_mapper:
+            Mapper from `method_config.data_cache` to a class to provide Method Layer
+            with the cache mechanism. The method data cache manages analysis data of the
+            candidate terms such as frequency or likelihood.
+
+        styling_cache_mapper:
+            Mapper from `styling_config.cache` to a class to provide Styling Layer with
+            the cache mechanism. The styling cache manages candidate terms ordered by
+            the styling scores.
+
+        cache_dir:
+            Path like string where cache files to be stored. For example, path to a
+            local directory, a url or a bucket name of a cloud storage service.
+    """
+
+    def __init__(
+        self,
+        xml_config: Optional[XMLLayerConfig] = None,
+        candidate_config: Optional[CandidateLayerConfig] = None,
+        method_config: Optional[SingleDomainMethodLayerConfig] = None,
+        styling_config: Optional[StylingLayerConfig] = None,
+        techterm_config: Optional[TechnicalTermLayerConfig] = None,
+        bin_opener_mapper: Optional[BinaryOpenerMapper] = None,
+        lang_tokenizer_mapper: Optional[LanguageTokenizerMapper] = None,
+        token_classifier_mapper: Optional[TokenClassifierMapper] = None,
+        token_filter_mapper: Optional[CandidateTokenFilterMapper] = None,
+        term_filter_mapper: Optional[CandidateTermFilterMapper] = None,
+        splitter_mapper: Optional[SplitterMapper] = None,
+        augmenter_mapper: Optional[AugmenterMapper] = None,
+        method_mapper: Optional[SingleDomainRankingMethodMapper] = None,
+        styling_score_mapper: Optional[StylingScoreMapper] = None,
+        xml_cache_mapper: Optional[XMLLayerCacheMapper] = None,
+        candidate_cache_mapper: Optional[CandidateLayerCacheMapper] = None,
+        method_ranking_cache_mapper: Optional[MethodLayerRankingCacheMapper] = None,
+        method_data_cache_mapper: Optional[MethodLayerDataCacheMapper] = None,
+        styling_cache_mapper: Optional[StylingLayerCacheMapper] = None,
+        cache_dir: str = DEFAULT_CACHE_DIR,
+    ) -> None:
+        xml_layer = XMLLayer(
+            config=xml_config,
+            bin_opener_mapper=bin_opener_mapper,
+            cache_mapper=xml_cache_mapper,
+            cache_dir=cache_dir,
+        )
+        candidate_layer = CandidateLayer(
+            xml_layer=xml_layer,
+            config=candidate_config,
+            lang_tokenizer_mapper=lang_tokenizer_mapper,
+            token_classifier_mapper=token_classifier_mapper,
+            token_filter_mapper=token_filter_mapper,
+            term_filter_mapper=term_filter_mapper,
+            splitter_mapper=splitter_mapper,
+            augmenter_mapper=augmenter_mapper,
+            cache_mapper=candidate_cache_mapper,
+            cache_dir=cache_dir,
+        )
+        method_layer = SingleDomainMethodLayer(
+            candidate_layer=candidate_layer,
+            config=method_config,
+            method_mapper=method_mapper,
+            ranking_cache_mapper=method_ranking_cache_mapper,
+            data_cache_mapper=method_data_cache_mapper,
+            cache_dir=cache_dir,
+        )
+        styling_layer = StylingLayer(
+            candidate_layer=candidate_layer,
+            config=styling_config,
+            styling_score_mapper=styling_score_mapper,
+            cache_mapper=styling_cache_mapper,
+            cache_dir=cache_dir,
+        )
+        techterm_layer = SingleDomainTechnicalTermLayer(
+            candidate_layer=candidate_layer,
+            method_layer=method_layer,
+            styling_layer=styling_layer,
+            config=techterm_config,
+        )
+
+        self._techterm_layer = techterm_layer
+
+    def extract(
+        self, pdf_path: str, domain_pdfs: DomainPDFList
+    ) -> PDFTechnicalTermList:
+        """Extract technical terms from a PDF file.
+
+        Args
+        ----
+            pdf_path:
+                Path like string to the input PDF file which terminologies to be
+                extracted. The file MUST belong to `domain`.
+
+            domain_pdfs:
+                List of path like strings to the PDF files which belong to a specific
+                domain.
+
+        Returns:
+            PDFTechnicalTermList:
+                Terminology list per page from the input PDF file.
+        """
+        self._validate(pdf_path, domain_pdfs)
+
+        pdf_techterms = self._techterm_layer.create_pdf_techterms(pdf_path, domain_pdfs)
+        return pdf_techterms
+
+    def _validate(self, pdf_path: str, domain_pdfs: DomainPDFList) -> None:
+        DomainPDFList.validate(domain_pdfs)
+
+        if pdf_path not in domain_pdfs.pdf_paths:
+            raise ValueError(f"{pdf_path} must be included in domain_pdfs")
+
+
+class PyPDFTermMultiDomainExtractor:
+    """Top level class of py-pdf-term. This class extracts technical terms from a PDF
+    file with cross-domain information.
+
+    Args
+    ----
+        xml_config:
+            Config of XML Layer.
+
+        candidate_config:
+            Config of Candidate Term Layer.
+
+        method_config:
+            Config of Method Layer.
+
+        styling_config:
+            Config of Styling Layer.
+
+        techterm_config:
+            Config of Technial Term Layer.
 
-        multi_method_mapper:
+        bin_opener_mapper:
+            Mapper from `xml_config.open_bin` to a function to open a input PDF file in
+            the binary mode. This is used in XML Layer.
+
+        lang_tokenizer_mapper:
+            Mapper from an element in `candidate_config.lang_tokenizers` to a class to
+            tokenize texts in a specific language with spaCy. This is used in Candidate
+            Term Layer.
+
+        token_classifier_mapper:
+            Mapper from an element in `candidate_config.token_classifiers` to a class to
+            classify tokens into True/False by several functions. This is used in
+            Candidate Term Layer.
+
+        token_filter_mapper:
+            Mapper from an element in `candidate_config.token_filters` to a class to
+            filter tokens which are likely to be parts of candidates. This is used in
+            Candidate Term Layer.
+
+        term_filter_mapper:
+            Mapper from an element in `candidate_config.term_filters` to a class to
+            filter terms which are likely to be candidates. This is used in Candidate
+            Term Layer.
+
+        splitter_mapper:
+            Mapper from an element in `candidate_config.splitters` to a class to split
+            too long terms or wrongly concatenated terms. This is used in Candidate Term
+            Layer.
+
+        augmenter_mapper:
+            Mapper from an element in `candidate_config.augmenters` to a class to
+            augment candidates. The augumentation means that if a long candidate is
+            found, sub-terms of it could also be candidates. This is used in Candidate
+            Term Layer.
+
+        method_mapper:
             Mapper from `method_config.method` to a class to calculate method scores of
-            candidate terms when `method_config.method_type` equals to "multi".
-            A multi-domain ranking method is an ranking algorithm which calculate method
-            scores with cross-domain information.
-            e.g. TF-IDF algorithm uses Inverse Document Frequency, which goes to high
-            then a term appears frequently in a target domain but not in the other
-            domains. To find IDF score, cross-domain data are required. Therefore,
-            TF-IDF is a multi-domain ranking method.
+            candidate terms. This is used in Method Layer.
 
         styling_score_mapper:
             Mapper from an element in `styling_config.styling_scores` to a class to
-            calculate styling scores of candidate terms. Each scoring class is expected
-            to focus one specific styling feature. Then different types of scores are
-            combined later.
+            calculate scores of candidate terms based on their styling such as color,
+            fontsize and so on. This is used in Styling Layer.
 
         xml_cache_mapper:
             Mapper from `xml_config.cache` to a class to provide XML Layer with the
             cache  mechanism. The xml cache manages XML files converted from input PDF
             files.
 
         candidate_cache_mapper:
@@ -146,33 +319,32 @@
         styling_cache_mapper:
             Mapper from `styling_config.cache` to a class to provide Styling Layer with
             the cache mechanism. The styling cache manages candidate terms ordered by
             the styling scores.
 
         cache_dir:
             Path like string where cache files to be stored. For example, path to a
-            local dirctory, a url or a bucket name of a cloud storage service.
+            local directory, a url or a bucket name of a cloud storage service.
     """
 
     def __init__(
         self,
         xml_config: Optional[XMLLayerConfig] = None,
         candidate_config: Optional[CandidateLayerConfig] = None,
-        method_config: Optional[MethodLayerConfig] = None,
+        method_config: Optional[MultiDomainMethodLayerConfig] = None,
         styling_config: Optional[StylingLayerConfig] = None,
         techterm_config: Optional[TechnicalTermLayerConfig] = None,
         bin_opener_mapper: Optional[BinaryOpenerMapper] = None,
         lang_tokenizer_mapper: Optional[LanguageTokenizerMapper] = None,
-        token_classifier_mapper: Optional[TokenClassifilerMapper] = None,
+        token_classifier_mapper: Optional[TokenClassifierMapper] = None,
         token_filter_mapper: Optional[CandidateTokenFilterMapper] = None,
         term_filter_mapper: Optional[CandidateTermFilterMapper] = None,
         splitter_mapper: Optional[SplitterMapper] = None,
         augmenter_mapper: Optional[AugmenterMapper] = None,
-        single_method_mapper: Optional[SingleDomainRankingMethodMapper] = None,
-        multi_method_mapper: Optional[MultiDomainRankingMethodMapper] = None,
+        method_mapper: Optional[MultiDomainRankingMethodMapper] = None,
         styling_score_mapper: Optional[StylingScoreMapper] = None,
         xml_cache_mapper: Optional[XMLLayerCacheMapper] = None,
         candidate_cache_mapper: Optional[CandidateLayerCacheMapper] = None,
         method_ranking_cache_mapper: Optional[MethodLayerRankingCacheMapper] = None,
         method_data_cache_mapper: Optional[MethodLayerDataCacheMapper] = None,
         styling_cache_mapper: Optional[StylingLayerCacheMapper] = None,
         cache_dir: str = DEFAULT_CACHE_DIR,
@@ -191,69 +363,86 @@
             token_filter_mapper=token_filter_mapper,
             term_filter_mapper=term_filter_mapper,
             splitter_mapper=splitter_mapper,
             augmenter_mapper=augmenter_mapper,
             cache_mapper=candidate_cache_mapper,
             cache_dir=cache_dir,
         )
-        method_layer = MethodLayer(
+        method_layer = MultiDomainMethodLayer(
             candidate_layer=candidate_layer,
             config=method_config,
-            single_method_mapper=single_method_mapper,
-            multi_method_mapper=multi_method_mapper,
+            method_mapper=method_mapper,
             ranking_cache_mapper=method_ranking_cache_mapper,
             data_cache_mapper=method_data_cache_mapper,
             cache_dir=cache_dir,
         )
         styling_layer = StylingLayer(
             candidate_layer=candidate_layer,
             config=styling_config,
             styling_score_mapper=styling_score_mapper,
             cache_mapper=styling_cache_mapper,
             cache_dir=cache_dir,
         )
-        techterm_layer = TechnicalTermLayer(
+        techterm_layer = MultiDomainTechnicalTermLayer(
             candidate_layer=candidate_layer,
             method_layer=method_layer,
             styling_layer=styling_layer,
             config=techterm_config,
         )
 
         self._techterm_layer = techterm_layer
 
     def extract(
-        self,
-        domain: str,
-        pdf_path: str,
-        single_domain_pdfs: Optional[DomainPDFList] = None,
-        multi_domain_pdfs: Optional[List[DomainPDFList]] = None,
+        self, domain: str, pdf_path: str, multi_domain_pdfs: List[DomainPDFList]
     ) -> PDFTechnicalTermList:
-        """Function to extract terminologies from PDF file.
+        """Extract technical terms from a PDF file.
 
-        Args:
+        Args
+        ----
             domain:
                 Domain name which the input PDF file belongs to. This may be the name of
                 a course, the name of a technical field or something.
 
             pdf_path:
                 Path like string to the input PDF file which terminologies to be
                 extracted. The file MUST belong to `domain`.
 
-            single_domain_pdfs:
-                List of path like strings to the PDF files which belong to `domain`.
-                `single_domain_pdfs.domain` MUST equals to `domain`. This argument is
-                required when a single-domain ranking method is to be used.
-
             multi_domain_pdfs:
                 List of path like strings to the PDF files which classified by domain.
                 There MUST be an element in `multi_domain_pdfs` whose domain equals to
-                `domain`. This argument is required when a multi-domain ranking method
-                is to be used.
+                `domain`.
 
         Returns:
             PDFTechnicalTermList:
                 Terminology list per page from the input PDF file.
         """
+        self._validate(domain, pdf_path, multi_domain_pdfs)
+
         pdf_techterms = self._techterm_layer.create_pdf_techterms(
-            domain, pdf_path, single_domain_pdfs, multi_domain_pdfs
+            domain, pdf_path, multi_domain_pdfs
         )
         return pdf_techterms
+
+    def _validate(
+        self, domain: str, pdf_path: str, multi_domain_pdfs: List[DomainPDFList]
+    ) -> None:
+        if domain == "":
+            raise ValueError("domain name must not be empty")
+
+        if len(multi_domain_pdfs) < 2:
+            raise ValueError("multi_domain_pdfs must have at least two elements")
+
+        for domain_pdfs in multi_domain_pdfs:
+            DomainPDFList.validate(domain_pdfs)
+
+        domain_set = set(map(lambda pdfs: pdfs.domain, multi_domain_pdfs))
+        if len(domain_set) != len(multi_domain_pdfs):
+            raise ValueError("multi_domain_pdfs must have unique domain names")
+
+        if domain not in domain_set:
+            raise ValueError(f"{domain} must be included in multi_domain_pdfs")
+
+        domain_pdfs = next(
+            filter(lambda pdfs: pdfs.domain == domain, multi_domain_pdfs)
+        )
+        if pdf_path not in domain_pdfs.pdf_paths:
+            raise ValueError(f"{pdf_path} must be included in {domain}")
```

### Comparing `py-pdf-term-0.18.1/py_pdf_term/endtoend/_endtoend/layers/candidate.py` & `py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/layers/candidate.py`

 * *Files 22% similar despite different names*

```diff
@@ -12,39 +12,73 @@
 from ..mappers import (
     AugmenterMapper,
     CandidateLayerCacheMapper,
     CandidateTermFilterMapper,
     CandidateTokenFilterMapper,
     LanguageTokenizerMapper,
     SplitterMapper,
-    TokenClassifilerMapper,
+    TokenClassifierMapper,
 )
 from .xml import XMLLayer
 
 
 class CandidateLayer:
+    """A layer to extract candidate terms using XMLLayer.
+
+    Args
+    ----
+        xml_layer:
+            a layer to create textful XML elements from a PDF file.
+        config:
+            a configuration for this layer. If None, the default configuration is used.
+        lang_tokenizer_mapper:
+            a mapper to find language tokenizer classes from configuration. If None, the
+            default mapper is used.
+        token_classifier_mapper:
+            a mapper to find token classifier classes from configuration. If None, the
+            default mapper is used.
+        token_filter_mapper:
+            a mapper to find token filter classes from configuration. If None, the
+            default mapper is used.
+        term_filter_mapper:
+            a mapper to find term filter classes from configuration. If None, the
+            default mapper is used.
+        splitter_mapper:
+            a mapper to find splitter classes from configuration. If None, the default
+            mapper is used.
+        augmenter_mapper:
+            a mapper to find augmenter classes from configuration. If None, the default
+            mapper is used.
+        cache_mapper:
+            a mapper to find cache class from configuration. If None, the default mapper
+            is used.
+        cache_dir:
+            a directory path to store cache files. If None, the default directory is
+            used.
+    """
+
     def __init__(
         self,
         xml_layer: XMLLayer,
         config: Optional[CandidateLayerConfig] = None,
         lang_tokenizer_mapper: Optional[LanguageTokenizerMapper] = None,
-        token_classifier_mapper: Optional[TokenClassifilerMapper] = None,
+        token_classifier_mapper: Optional[TokenClassifierMapper] = None,
         token_filter_mapper: Optional[CandidateTokenFilterMapper] = None,
         term_filter_mapper: Optional[CandidateTermFilterMapper] = None,
         splitter_mapper: Optional[SplitterMapper] = None,
         augmenter_mapper: Optional[AugmenterMapper] = None,
         cache_mapper: Optional[CandidateLayerCacheMapper] = None,
         cache_dir: str = DEFAULT_CACHE_DIR,
     ) -> None:
         if config is None:
             config = CandidateLayerConfig()
         if lang_tokenizer_mapper is None:
             lang_tokenizer_mapper = LanguageTokenizerMapper.default_mapper()
         if token_classifier_mapper is None:
-            token_classifier_mapper = TokenClassifilerMapper.default_mapper()
+            token_classifier_mapper = TokenClassifierMapper.default_mapper()
         if token_filter_mapper is None:
             token_filter_mapper = CandidateTokenFilterMapper.default_mapper()
         if term_filter_mapper is None:
             term_filter_mapper = CandidateTermFilterMapper.default_mapper()
         if splitter_mapper is None:
             splitter_mapper = SplitterMapper.default_mapper()
         if augmenter_mapper is None:
@@ -69,30 +103,64 @@
             augmenter_clses=augmenter_clses,
         )
         self._cache = cache_cls(cache_dir=cache_dir)
         self._config = config
 
         self._xml_layer = xml_layer
 
-    def create_domain_candiates(
+    def create_domain_candidates(
         self, domain_pdfs: DomainPDFList
     ) -> DomainCandidateTermList:
+        """Create candidate term list from a list of PDF files in a domain.
+
+        Args
+        ----
+            domain_pdfs:
+                a list of PDF files in a domain.
+
+        Returns
+        -------
+            DomainCandidateTermList:
+                a list of candidate terms in a domain.
+        """
+
         pdf_candidates_list: List[PDFCandidateTermList] = []
         for pdf_path in domain_pdfs.pdf_paths:
             pdf_candidates = self.create_pdf_candidates(pdf_path)
             pdf_candidates_list.append(pdf_candidates)
 
         return DomainCandidateTermList(domain_pdfs.domain, pdf_candidates_list)
 
     def create_pdf_candidates(self, pdf_path: str) -> PDFCandidateTermList:
+        """Create candidate term list from a PDF file.
+
+        Args
+        ----
+            pdf_path:
+                a path to a PDF file.
+
+        Returns
+        -------
+            PDFCandidateTermList:
+                a list of candidate terms in a PDF file.
+        """
+
         pdf_candidates = self._cache.load(pdf_path, self._config)
 
         if pdf_candidates is None:
             pdfnxml = self._xml_layer.create_pdfnxml(pdf_path)
             pdf_candidates = self._extractor.extract_from_xml_element(pdfnxml)
 
         self._cache.store(pdf_candidates, self._config)
 
         return pdf_candidates
 
     def remove_cache(self, pdf_path: str) -> None:
+        """Remove a cache file for a PDF file.
+
+        Args
+        ----
+            pdf_path:
+                a path to a PDF file to remove a cache file.
+        """
+
         self._cache.remove(pdf_path, self._config)
```

### Comparing `py-pdf-term-0.18.1/py_pdf_term/endtoend/_endtoend/layers/styling.py` & `py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/layers/styling.py`

 * *Files 20% similar despite different names*

```diff
@@ -5,14 +5,31 @@
 from ..caches import DEFAULT_CACHE_DIR
 from ..configs import StylingLayerConfig
 from ..mappers import StylingLayerCacheMapper, StylingScoreMapper
 from .candidate import CandidateLayer
 
 
 class StylingLayer:
+    """A layer to calclate styling scores from a PDF file using candidate layer.
+
+    Args
+    ----
+        candidate_layer:
+            a layer to extract candidate terms.
+        config:
+            a configuration for this layer. If None, the default configuration is used.
+        styling_score_mapper:
+            a mapper to find styling score classes from configuration. If None, the
+            default mapper is used.
+        cache_mapper:
+            a mapper to find cache class from configuration. If None, the default mapper
+            is used.
+
+    """
+
     def __init__(
         self,
         candidate_layer: CandidateLayer,
         config: Optional[StylingLayerConfig] = None,
         styling_score_mapper: Optional[StylingScoreMapper] = None,
         cache_mapper: Optional[StylingLayerCacheMapper] = None,
         cache_dir: str = DEFAULT_CACHE_DIR,
@@ -30,19 +47,40 @@
         self._scorer = StylingScorer(styling_score_clses=styling_score_clses)
         self._cache = cache_cls(cache_dir=cache_dir)
         self._config = config
 
         self._candidate_layer = candidate_layer
 
     def create_pdf_styling_scores(self, pdf_path: str) -> PDFStylingScoreList:
+        """Create style score list from a PDF file.
+
+        Args
+        ----
+            pdf_path:
+                a PDF file path to calculate styling scores.
+
+        Returns
+        -------
+            PDFStylingScoreList:
+                a list of styling scores for each page in the PDF file.
+        """
+
         styling_scores = self._cache.load(pdf_path, self._config)
 
         if styling_scores is None:
             pdf_candidates = self._candidate_layer.create_pdf_candidates(pdf_path)
             styling_scores = self._scorer.score_pdf_candidates(pdf_candidates)
 
         self._cache.store(styling_scores, self._config)
 
         return styling_scores
 
     def remove_cache(self, pdf_path: str) -> None:
+        """Remove a cache file for a PDF file.
+
+        Args
+        ----
+            pdf_path:
+                a PDF file path to remove a cache file.
+        """
+
         self._cache.remove(pdf_path, self._config)
```

### Comparing `py-pdf-term-0.18.1/py_pdf_term/endtoend/_endtoend/mappers/__init__.py` & `py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/mappers/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,37 +1,39 @@
+from .base import BaseMapper
 from .caches import (
     CandidateLayerCacheMapper,
     MethodLayerDataCacheMapper,
     MethodLayerRankingCacheMapper,
     StylingLayerCacheMapper,
     XMLLayerCacheMapper,
 )
 from .candidates import (
     AugmenterMapper,
     CandidateTermFilterMapper,
     CandidateTokenFilterMapper,
     LanguageTokenizerMapper,
     SplitterMapper,
-    TokenClassifilerMapper,
+    TokenClassifierMapper,
 )
 from .methods import MultiDomainRankingMethodMapper, SingleDomainRankingMethodMapper
 from .pdftoxml import BinaryOpenerMapper
 from .stylings import StylingScoreMapper
 
 # isort: unique-list
 __all__ = [
     "AugmenterMapper",
+    "BaseMapper",
     "BinaryOpenerMapper",
     "CandidateLayerCacheMapper",
     "CandidateTermFilterMapper",
     "CandidateTokenFilterMapper",
     "LanguageTokenizerMapper",
     "MethodLayerDataCacheMapper",
     "MethodLayerRankingCacheMapper",
     "MultiDomainRankingMethodMapper",
     "SingleDomainRankingMethodMapper",
     "SplitterMapper",
     "StylingLayerCacheMapper",
     "StylingScoreMapper",
-    "TokenClassifilerMapper",
+    "TokenClassifierMapper",
     "XMLLayerCacheMapper",
 ]
```

### Comparing `py-pdf-term-0.18.1/py_pdf_term/endtoend/_endtoend/mappers/caches/candidate.py` & `py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/mappers/caches/styling.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 from typing import Type
 
-from ...caches import (
-    BaseCandidateLayerCache,
-    CandidateLayerFileCache,
-    CandidateLayerNoCache,
-)
+from py_pdf_term._common.consts import PACKAGE_NAME
+
+from ...caches import BaseStylingLayerCache, StylingLayerFileCache, StylingLayerNoCache
 from ..base import BaseMapper
-from ..consts import PACKAGE_NAME
 
 
-class CandidateLayerCacheMapper(BaseMapper[Type[BaseCandidateLayerCache]]):
+class StylingLayerCacheMapper(BaseMapper[Type[BaseStylingLayerCache]]):
+    """A mapper to find styling layer cache classes."""
+
     @classmethod
-    def default_mapper(cls) -> "CandidateLayerCacheMapper":
+    def default_mapper(cls) -> "StylingLayerCacheMapper":
         default_mapper = cls()
 
-        cache_clses = [CandidateLayerNoCache, CandidateLayerFileCache]
+        cache_clses = [StylingLayerNoCache, StylingLayerFileCache]
         for cache_cls in cache_clses:
             default_mapper.add(f"{PACKAGE_NAME}.{cache_cls.__name__}", cache_cls)
 
         return default_mapper
```

### Comparing `py-pdf-term-0.18.1/py_pdf_term/endtoend/_endtoend/mappers/caches/method.py` & `py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/mappers/caches/method.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,39 @@
 from typing import Any, Type
 
+from py_pdf_term._common.consts import PACKAGE_NAME
+
 from ...caches import (
     BaseMethodLayerDataCache,
     BaseMethodLayerRankingCache,
     MethodLayerDataFileCache,
     MethodLayerDataNoCache,
     MethodLayerRankingFileCache,
     MethodLayerRankingNoCache,
 )
 from ..base import BaseMapper
-from ..consts import PACKAGE_NAME
 
 
 class MethodLayerRankingCacheMapper(BaseMapper[Type[BaseMethodLayerRankingCache]]):
+    """A mapper to find method layer ranking cache classes."""
+
     @classmethod
     def default_mapper(cls) -> "MethodLayerRankingCacheMapper":
         default_mapper = cls()
 
         cache_clses = [MethodLayerRankingNoCache, MethodLayerRankingFileCache]
         for cache_cls in cache_clses:
             default_mapper.add(f"{PACKAGE_NAME}.{cache_cls.__name__}", cache_cls)
 
         return default_mapper
 
 
 class MethodLayerDataCacheMapper(BaseMapper[Type[BaseMethodLayerDataCache[Any]]]):
+    """A mapper to find method layer data cache classes."""
+
     @classmethod
     def default_mapper(cls) -> "MethodLayerDataCacheMapper":
         default_mapper = cls()
 
         cache_clses = [
             ("MethodLayerDataNoCache", MethodLayerDataNoCache[Any]),
             ("MethodLayerDataFileCache", MethodLayerDataFileCache[Any]),
```

### Comparing `py-pdf-term-0.18.1/py_pdf_term/endtoend/_endtoend/mappers/caches/xml.py` & `py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/mappers/caches/xml.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 from typing import Type
 
+from py_pdf_term._common.consts import PACKAGE_NAME
+
 from ...caches import BaseXMLLayerCache, XMLLayerFileCache, XMLLayerNoCache
 from ..base import BaseMapper
-from ..consts import PACKAGE_NAME
 
 
 class XMLLayerCacheMapper(BaseMapper[Type[BaseXMLLayerCache]]):
+    """A mapper to find XML layer cache classes."""
+
     @classmethod
     def default_mapper(cls) -> "XMLLayerCacheMapper":
         default_mapper = cls()
 
         cache_clses = [XMLLayerNoCache, XMLLayerFileCache]
         for cache_cls in cache_clses:
             default_mapper.add(f"{PACKAGE_NAME}.{cache_cls.__name__}", cache_cls)
```

### Comparing `py-pdf-term-0.18.1/py_pdf_term/endtoend/_endtoend/mappers/candidates/augmenter.py` & `py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/mappers/candidates/augmenter.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from typing import Type
 
+from py_pdf_term._common.consts import PACKAGE_NAME
 from py_pdf_term.candidates.augmenters import (
     BaseAugmenter,
     EnglishConnectorTermAugmenter,
     JapaneseConnectorTermAugmenter,
 )
 
 from ..base import BaseMapper
-from ..consts import PACKAGE_NAME
 
 
 class AugmenterMapper(BaseMapper[Type[BaseAugmenter]]):
+    """A mapper to find augmenter classes."""
+
     @classmethod
     def default_mapper(cls) -> "AugmenterMapper":
         default_mapper = cls()
 
         augmenter_clses = [
             JapaneseConnectorTermAugmenter,
             EnglishConnectorTermAugmenter,
```

### Comparing `py-pdf-term-0.18.1/py_pdf_term/endtoend/_endtoend/mappers/candidates/lang.py` & `py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/mappers/candidates/lang.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from typing import Type
 
-from py_pdf_term.tokenizer import (
+from py_pdf_term._common.consts import PACKAGE_NAME
+from py_pdf_term.tokenizers import (
     BaseLanguageTokenizer,
     EnglishTokenizer,
     JapaneseTokenizer,
 )
 
 from ..base import BaseMapper
-from ..consts import PACKAGE_NAME
 
 
 class LanguageTokenizerMapper(BaseMapper[Type[BaseLanguageTokenizer]]):
+    """A mapper to find language tokenizer classes."""
+
     @classmethod
     def default_mapper(cls) -> "LanguageTokenizerMapper":
         default_mapper = cls()
 
         lang_tokenizer_clses = [JapaneseTokenizer, EnglishTokenizer]
         for lang_tokenizer_cls in lang_tokenizer_clses:
             default_mapper.add(
```

### Comparing `py-pdf-term-0.18.1/py_pdf_term/endtoend/_endtoend/mappers/candidates/splitter.py` & `py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/mappers/candidates/splitter.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from typing import Type
 
+from py_pdf_term._common.consts import PACKAGE_NAME
 from py_pdf_term.candidates.splitters import (
     BaseSplitter,
     RepeatSplitter,
     SymbolNameSplitter,
 )
 
 from ..base import BaseMapper
-from ..consts import PACKAGE_NAME
 
 
 class SplitterMapper(BaseMapper[Type[BaseSplitter]]):
+    """A mapper to find splitter classes."""
+
     @classmethod
     def default_mapper(cls) -> "SplitterMapper":
         default_mapper = cls()
 
         splitter_clses = [SymbolNameSplitter, RepeatSplitter]
         for splitter_cls in splitter_clses:
             default_mapper.add(f"{PACKAGE_NAME}.{splitter_cls.__name__}", splitter_cls)
```

### Comparing `py-pdf-term-0.18.1/py_pdf_term/endtoend/_endtoend/mappers/methods/multi.py` & `py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/mappers/methods/multi.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from typing import Any, Type
 
+from py_pdf_term._common.consts import PACKAGE_NAME
 from py_pdf_term.methods import BaseMultiDomainRankingMethod, MDPMethod, TFIDFMethod
 
 from ..base import BaseMapper
-from ..consts import PACKAGE_NAME
 
 
 class MultiDomainRankingMethodMapper(
     BaseMapper[Type[BaseMultiDomainRankingMethod[Any]]]
 ):
+    """A mapper to find multi-domain ranking method classes."""
+
     @classmethod
     def default_mapper(cls) -> "MultiDomainRankingMethodMapper":
         default_mapper = cls()
 
         multi_domain_clses = [TFIDFMethod, MDPMethod]
         for method_cls in multi_domain_clses:
             default_mapper.add(f"{PACKAGE_NAME}.{method_cls.__name__}", method_cls)
```

### Comparing `py-pdf-term-0.18.1/py_pdf_term/endtoend/_endtoend/mappers/methods/single.py` & `py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/mappers/methods/single.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 from typing import Any, Type
 
+from py_pdf_term._common.consts import PACKAGE_NAME
 from py_pdf_term.methods import (
     BaseSingleDomainRankingMethod,
     FLRHMethod,
     FLRMethod,
     HITSMethod,
     MCValueMethod,
 )
 
 from ..base import BaseMapper
-from ..consts import PACKAGE_NAME
 
 
 class SingleDomainRankingMethodMapper(
     BaseMapper[Type[BaseSingleDomainRankingMethod[Any]]]
 ):
+    """A mapper to find single-domain ranking method classes."""
+
     @classmethod
     def default_mapper(cls) -> "SingleDomainRankingMethodMapper":
         default_mapper = cls()
 
         single_domain_clses = [MCValueMethod, FLRMethod, HITSMethod, FLRHMethod]
         for method_cls in single_domain_clses:
             default_mapper.add(f"{PACKAGE_NAME}.{method_cls.__name__}", method_cls)
```

### Comparing `py-pdf-term-0.18.1/py_pdf_term/endtoend/_endtoend/mappers/stylings/score.py` & `py_pdf_term-1.0.0/py_pdf_term/endtoend/_endtoend/mappers/stylings/score.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from typing import Type
 
+from py_pdf_term._common.consts import PACKAGE_NAME
 from py_pdf_term.stylings.scores import BaseStylingScore, ColorScore, FontsizeScore
 
 from ..base import BaseMapper
-from ..consts import PACKAGE_NAME
 
 
 class StylingScoreMapper(BaseMapper[Type[BaseStylingScore]]):
+    """A mapper to find styling score classes."""
+
     @classmethod
     def default_mapper(cls) -> "StylingScoreMapper":
         default_mapper = cls()
 
         styling_score_clses = [FontsizeScore, ColorScore]
         for styling_score_cls in styling_score_clses:
             default_mapper.add(
```

### Comparing `py-pdf-term-0.18.1/py_pdf_term/mappers.py` & `py_pdf_term-1.0.0/py_pdf_term/mappers.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from .endtoend._endtoend.mappers import (
     AugmenterMapper,
     BinaryOpenerMapper,
     CandidateLayerCacheMapper,
     CandidateTermFilterMapper,
     CandidateTokenFilterMapper,
-    TokenClassifilerMapper,
     LanguageTokenizerMapper,
     MethodLayerDataCacheMapper,
     MethodLayerRankingCacheMapper,
     MultiDomainRankingMethodMapper,
     SingleDomainRankingMethodMapper,
     SplitterMapper,
     StylingLayerCacheMapper,
     StylingScoreMapper,
+    TokenClassifierMapper,
     XMLLayerCacheMapper,
 )
 
 # isort: unique-list
 __all__ = [
     "AugmenterMapper",
     "BinaryOpenerMapper",
@@ -27,10 +27,10 @@
     "MethodLayerDataCacheMapper",
     "MethodLayerRankingCacheMapper",
     "MultiDomainRankingMethodMapper",
     "SingleDomainRankingMethodMapper",
     "SplitterMapper",
     "StylingLayerCacheMapper",
     "StylingScoreMapper",
+    "TokenClassifierMapper",
     "XMLLayerCacheMapper",
-    "TokenClassifilerMapper",
 ]
```

### Comparing `py-pdf-term-0.18.1/py_pdf_term/methods/_methods/__init__.py` & `py_pdf_term-1.0.0/py_pdf_term/methods/_methods/__init__.py`

 * *Files identical despite different names*

### Comparing `py-pdf-term-0.18.1/py_pdf_term/methods/_methods/base.py` & `py_pdf_term-1.0.0/py_pdf_term/methods/_methods/rankers/flrh.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,89 +1,74 @@
-from abc import ABCMeta, abstractmethod
-from typing import Any, Dict, Generic, Iterator, List, Optional
-
+from py_pdf_term._common.data import ScoredTerm
 from py_pdf_term.candidates import DomainCandidateTermList
+from py_pdf_term.tokenizers import Term
 
-from .collectors import BaseRankingDataCollector
-from .data import MethodTermRanking
-from .rankers import BaseMultiDomainRanker, BaseSingleDomainRanker
-from .rankingdata.base import RankingData
-
-
-class BaseSingleDomainRankingMethod(Generic[RankingData], metaclass=ABCMeta):
-    def __init__(
-        self,
-        data_collector: BaseRankingDataCollector[RankingData],
-        ranker: BaseSingleDomainRanker[RankingData],
-    ) -> None:
-        self._data_collector = data_collector
-        self._ranker = ranker
-
-    def rank_terms(
-        self,
-        domain_candidates: DomainCandidateTermList,
-        ranking_data: Optional[RankingData] = None,
-    ) -> MethodTermRanking:
-        if ranking_data is None:
-            ranking_data = self._data_collector.collect(domain_candidates)
-        term_ranking = self._ranker.rank_terms(domain_candidates, ranking_data)
-        return term_ranking
-
-    def collect_data(self, domain_candidates: DomainCandidateTermList) -> RankingData:
-        ranking_data = self._data_collector.collect(domain_candidates)
-        return ranking_data
-
-    @classmethod
-    @abstractmethod
-    def collect_data_from_dict(cls, obj: Dict[str, Any]) -> RankingData:
-        raise NotImplementedError(f"{cls.__name__}.collect_data_from_dict()")
-
-
-class BaseMultiDomainRankingMethod(Generic[RankingData], metaclass=ABCMeta):
-    def __init__(
-        self,
-        data_collector: BaseRankingDataCollector[RankingData],
-        ranker: BaseMultiDomainRanker[RankingData],
-    ) -> None:
-        self._data_collector = data_collector
-        self._ranker = ranker
+from ..data import MethodTermRanking
+from ..rankingdata import FLRHRankingData, FLRRankingData, HITSRankingData
+from .base import BaseSingleDomainRanker
+from .flr import FLRRanker
+from .hits import HITSAuthHubData, HITSRanker
+
+
+class FLRHRanker(BaseSingleDomainRanker[FLRHRankingData]):
+    """A term ranker by FLRH algorithm. This algorithm is a combination of FLR and HITS.
+
+    Args
+    ----
+        threshold:
+            A threshold value for HITS algorithm. The default is 1e-8.
+        max_loop:
+            A maximum number of loops for HITS algorithm. The default is 1000.
+    """
+
+    def __init__(self, threshold: float = 1e-8, max_loop: int = 1000) -> None:
+        self._flr_ranker = FLRRanker()
+        self._hits_ranker = HITSRanker(threshold=threshold, max_loop=max_loop)
 
     def rank_terms(
-        self,
-        domain_candidates_list: List[DomainCandidateTermList],
-        ranking_data_list: Optional[List[RankingData]] = None,
-    ) -> Iterator[MethodTermRanking]:
-        if ranking_data_list is None:
-            ranking_data_list = list(
-                map(self._data_collector.collect, domain_candidates_list)
-            )
-
-        for domain_candidates in domain_candidates_list:
-            term_ranking = self._ranker.rank_terms(domain_candidates, ranking_data_list)
-            yield term_ranking
-
-    def rank_domain_terms(
-        self,
-        domain: str,
-        domain_candidates_list: List[DomainCandidateTermList],
-        ranking_data_list: Optional[List[RankingData]] = None,
+        self, domain_candidates: DomainCandidateTermList, ranking_data: FLRHRankingData
     ) -> MethodTermRanking:
-        domain_candidates = next(
-            filter(lambda item: item.domain == domain, domain_candidates_list)
+        flr_ranking_data = FLRRankingData(
+            ranking_data.domain,
+            ranking_data.term_freq,
+            ranking_data.left_freq,
+            ranking_data.right_freq,
+        )
+        hits_ranking_data = HITSRankingData(
+            ranking_data.domain,
+            ranking_data.term_freq,
+            ranking_data.left_freq,
+            ranking_data.right_freq,
         )
 
-        if ranking_data_list is None:
-            ranking_data_list = list(
-                map(self._data_collector.collect, domain_candidates_list)
+        auth_hub_data = self._hits_ranker._create_auth_hub_data(  # pyright: ignore[reportPrivateUsage] # noqa: E501
+            hits_ranking_data
+        )
+        domain_candidates_dict = domain_candidates.to_nostyle_candidates_dict(
+            to_str=lambda candidate: candidate.lemma()
+        )
+        ranking = list(
+            map(
+                lambda candidate: self._calculate_score(
+                    candidate, flr_ranking_data, hits_ranking_data, auth_hub_data
+                ),
+                domain_candidates_dict.values(),
             )
+        )
+        ranking.sort(key=lambda scored_term: scored_term.score, reverse=True)
+        return MethodTermRanking(domain_candidates.domain, ranking)
 
-        term_ranking = self._ranker.rank_terms(domain_candidates, ranking_data_list)
-        return term_ranking
-
-    def collect_data(self, domain_candidates: DomainCandidateTermList) -> RankingData:
-        ranking_data = self._data_collector.collect(domain_candidates)
-        return ranking_data
-
-    @classmethod
-    @abstractmethod
-    def collect_data_from_dict(cls, obj: Dict[str, Any]) -> RankingData:
-        raise NotImplementedError(f"{cls.__name__}.collect_data_from_dict()")
+    def _calculate_score(
+        self,
+        candidate: Term,
+        flr_ranking_data: FLRRankingData,
+        hits_ranking_data: HITSRankingData,
+        auth_hub_data: HITSAuthHubData,
+    ) -> ScoredTerm:
+        candidate_lemma = candidate.lemma()
+        flr_score = self._flr_ranker._calculate_score(  # pyright: ignore[reportPrivateUsage] # noqa: E501
+            candidate, flr_ranking_data
+        ).score
+        hits_score = self._hits_ranker._calculate_score(  # pyright: ignore[reportPrivateUsage] # noqa: E501
+            candidate, hits_ranking_data, auth_hub_data
+        ).score
+        return ScoredTerm(candidate_lemma, flr_score + hits_score)
```

### Comparing `py-pdf-term-0.18.1/py_pdf_term/methods/_methods/collectors/__init__.py` & `py_pdf_term-1.0.0/py_pdf_term/methods/_methods/collectors/__init__.py`

 * *Files identical despite different names*

### Comparing `py-pdf-term-0.18.1/py_pdf_term/methods/_methods/collectors/flr.py` & `py_pdf_term-1.0.0/py_pdf_term/methods/_methods/collectors/flrh.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 from py_pdf_term.analysis import TermLeftRightFrequencyAnalyzer, TermOccurrenceAnalyzer
 from py_pdf_term.candidates import DomainCandidateTermList
 
-from ..rankingdata import FLRRankingData
+from ..rankingdata import FLRHRankingData
 from .base import BaseRankingDataCollector
 
 
-class FLRRankingDataCollector(BaseRankingDataCollector[FLRRankingData]):
+class FLRHRankingDataCollector(BaseRankingDataCollector[FLRHRankingData]):
+    """A collector of metadata to rank candidate terms in domain-specific PDF documents
+    by FLRH algorithm.
+    """
+
     def __init__(self) -> None:
         super().__init__()
         self._termocc_analyzer = TermOccurrenceAnalyzer()
         self._lrfreq_analyzer = TermLeftRightFrequencyAnalyzer()
 
-    def collect(self, domain_candidates: DomainCandidateTermList) -> FLRRankingData:
+    def collect(self, domain_candidates: DomainCandidateTermList) -> FLRHRankingData:
         termocc = self._termocc_analyzer.analyze(domain_candidates)
         lrfreq = self._lrfreq_analyzer.analyze(domain_candidates)
 
-        return FLRRankingData(
+        return FLRHRankingData(
             domain_candidates.domain,
             termocc.term_freq,
             lrfreq.left_freq,
             lrfreq.right_freq,
         )
```

### Comparing `py-pdf-term-0.18.1/py_pdf_term/methods/_methods/collectors/flrh.py` & `py_pdf_term-1.0.0/py_pdf_term/methods/_methods/collectors/hits.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 from py_pdf_term.analysis import TermLeftRightFrequencyAnalyzer, TermOccurrenceAnalyzer
 from py_pdf_term.candidates import DomainCandidateTermList
 
-from ..rankingdata import FLRHRankingData
+from ..rankingdata import HITSRankingData
 from .base import BaseRankingDataCollector
 
 
-class FLRHRankingDataCollector(BaseRankingDataCollector[FLRHRankingData]):
+class HITSRankingDataCollector(BaseRankingDataCollector[HITSRankingData]):
+    """A collector of metadata to rank candidate terms in domain-specific PDF documents
+    by HITS algorithm.
+    """
+
     def __init__(self) -> None:
         super().__init__()
         self._termocc_analyzer = TermOccurrenceAnalyzer()
         self._lrfreq_analyzer = TermLeftRightFrequencyAnalyzer()
 
-    def collect(self, domain_candidates: DomainCandidateTermList) -> FLRHRankingData:
+    def collect(self, domain_candidates: DomainCandidateTermList) -> HITSRankingData:
         termocc = self._termocc_analyzer.analyze(domain_candidates)
         lrfreq = self._lrfreq_analyzer.analyze(domain_candidates)
 
-        return FLRHRankingData(
+        return HITSRankingData(
             domain_candidates.domain,
             termocc.term_freq,
             lrfreq.left_freq,
             lrfreq.right_freq,
         )
```

### Comparing `py-pdf-term-0.18.1/py_pdf_term/methods/_methods/collectors/hits.py` & `py_pdf_term-1.0.0/py_pdf_term/methods/_methods/collectors/flr.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,27 @@
 from py_pdf_term.analysis import TermLeftRightFrequencyAnalyzer, TermOccurrenceAnalyzer
 from py_pdf_term.candidates import DomainCandidateTermList
 
-from ..rankingdata import HITSRankingData
+from ..rankingdata import FLRRankingData
 from .base import BaseRankingDataCollector
 
 
-class HITSRankingDataCollector(BaseRankingDataCollector[HITSRankingData]):
+class FLRRankingDataCollector(BaseRankingDataCollector[FLRRankingData]):
+    """A collector of metadata to rank candidate terms in domain-specific PDF documents
+    by FLR algorithm.
+    """
+
     def __init__(self) -> None:
         super().__init__()
         self._termocc_analyzer = TermOccurrenceAnalyzer()
         self._lrfreq_analyzer = TermLeftRightFrequencyAnalyzer()
 
-    def collect(self, domain_candidates: DomainCandidateTermList) -> HITSRankingData:
+    def collect(self, domain_candidates: DomainCandidateTermList) -> FLRRankingData:
         termocc = self._termocc_analyzer.analyze(domain_candidates)
         lrfreq = self._lrfreq_analyzer.analyze(domain_candidates)
 
-        return HITSRankingData(
+        return FLRRankingData(
             domain_candidates.domain,
             termocc.term_freq,
             lrfreq.left_freq,
             lrfreq.right_freq,
         )
```

### Comparing `py-pdf-term-0.18.1/py_pdf_term/methods/_methods/collectors/mcvalue.py` & `py_pdf_term-1.0.0/py_pdf_term/methods/_methods/collectors/tfidf.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,22 +1,26 @@
-from py_pdf_term.analysis import ContainerTermsAnalyzer, TermOccurrenceAnalyzer
+from py_pdf_term.analysis import TermOccurrenceAnalyzer
 from py_pdf_term.candidates import DomainCandidateTermList
 
-from ..rankingdata import MCValueRankingData
+from ..rankingdata import TFIDFRankingData
 from .base import BaseRankingDataCollector
 
 
-class MCValueRankingDataCollector(BaseRankingDataCollector[MCValueRankingData]):
+class TFIDFRankingDataCollector(BaseRankingDataCollector[TFIDFRankingData]):
+    """A collector of metadata to rank candidate terms in domain-specific PDF documents
+    by TF-IDF algorithm.
+    """
+
     def __init__(self) -> None:
         super().__init__()
         self._termocc_analyzer = TermOccurrenceAnalyzer()
-        self._containers_analyzer = ContainerTermsAnalyzer()
 
-    def collect(self, domain_candidates: DomainCandidateTermList) -> MCValueRankingData:
+    def collect(self, domain_candidates: DomainCandidateTermList) -> TFIDFRankingData:
         termocc = self._termocc_analyzer.analyze(domain_candidates)
-        container_terms = self._containers_analyzer.analyze(domain_candidates)
+        num_docs = len(domain_candidates.pdfs)
 
-        return MCValueRankingData(
+        return TFIDFRankingData(
             domain_candidates.domain,
             termocc.term_freq,
-            container_terms.container_terms,
+            termocc.doc_term_freq,
+            num_docs,
         )
```

### Comparing `py-pdf-term-0.18.1/py_pdf_term/methods/_methods/collectors/mdp.py` & `py_pdf_term-1.0.0/py_pdf_term/methods/_methods/collectors/mdp.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 from py_pdf_term.candidates import DomainCandidateTermList
 
 from ..rankingdata import MDPRankingData
 from .base import BaseRankingDataCollector
 
 
 class MDPRankingDataCollector(BaseRankingDataCollector[MDPRankingData]):
+    """A collector of metadata to rank candidate terms in domain-specific PDF documents
+    by MDP algorithm.
+    """
+
     def __init__(self) -> None:
         super().__init__()
         self._termocc_analyzer = TermOccurrenceAnalyzer()
 
     def collect(self, domain_candidates: DomainCandidateTermList) -> MDPRankingData:
         termocc = self._termocc_analyzer.analyze(domain_candidates)
         return MDPRankingData(domain_candidates.domain, termocc.term_freq)
```

### Comparing `py-pdf-term-0.18.1/py_pdf_term/methods/_methods/data.py` & `py_pdf_term-1.0.0/py_pdf_term/methods/_methods/data.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,18 +2,27 @@
 from typing import Any, Dict, List
 
 from py_pdf_term._common.data import ScoredTerm
 
 
 @dataclass(frozen=True)
 class MethodTermRanking:
+    """Domain name and ranking of technical terms of the domain.
+
+    Args
+    ----
+        domain:
+            Domain name. (e.g., "natural language processing")
+        ranking:
+            List of pairs of lemmatized term and method score.
+            The list is sorted by the score in descending order.
+    """
+
     domain: str
     ranking: List[ScoredTerm]
-    # list of pairs of lemmatized term and method score
-    # the list is sorted by the score in descending order
 
     def to_dict(self) -> Dict[str, Any]:
         return {
             "domain": self.domain,
             "ranking": list(map(lambda term: term.to_dict(), self.ranking)),
         }
```

### Comparing `py-pdf-term-0.18.1/py_pdf_term/methods/_methods/flr.py` & `py_pdf_term-1.0.0/py_pdf_term/methods/_methods/flr.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 from .base import BaseSingleDomainRankingMethod
 from .collectors import FLRRankingDataCollector
 from .rankers import FLRRanker
 from .rankingdata import FLRRankingData
 
 
 class FLRMethod(BaseSingleDomainRankingMethod[FLRRankingData]):
+    """A ranking method by FLR algorithm."""
+
     def __init__(self) -> None:
         collector = FLRRankingDataCollector()
         ranker = FLRRanker()
         super().__init__(collector, ranker)
 
     @classmethod
     def collect_data_from_dict(cls, obj: Dict[str, Any]) -> FLRRankingData:
```

### Comparing `py-pdf-term-0.18.1/py_pdf_term/methods/_methods/flrh.py` & `py_pdf_term-1.0.0/py_pdf_term/methods/_methods/flrh.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,14 +3,26 @@
 from .base import BaseSingleDomainRankingMethod
 from .collectors import FLRHRankingDataCollector
 from .rankers import FLRHRanker
 from .rankingdata import FLRHRankingData
 
 
 class FLRHMethod(BaseSingleDomainRankingMethod[FLRHRankingData]):
+    """A ranking method by FLRH algorithm. This algorithm is a combination of FLR and
+    HITS.
+
+    Args
+    ----
+        threshold:
+            A threshold of the FLRH algorithm. The default is 1e-8.
+
+        max_loop:
+            A maximum number of loops of the FLRH algorithm. The default is 1000.
+    """
+
     def __init__(self, threshold: float = 1e-8, max_loop: int = 1000) -> None:
         collector = FLRHRankingDataCollector()
         ranker = FLRHRanker(threshold=threshold, max_loop=max_loop)
         super().__init__(collector, ranker)
 
     @classmethod
     def collect_data_from_dict(cls, obj: Dict[str, Any]) -> FLRHRankingData:
```

### Comparing `py-pdf-term-0.18.1/py_pdf_term/methods/_methods/hits.py` & `py_pdf_term-1.0.0/py_pdf_term/methods/_methods/hits.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,14 +3,28 @@
 from .base import BaseSingleDomainRankingMethod
 from .collectors import HITSRankingDataCollector
 from .rankers import HITSRanker
 from .rankingdata import HITSRankingData
 
 
 class HITSMethod(BaseSingleDomainRankingMethod[HITSRankingData]):
+    """A ranking method by HITS algorithm.
+
+    Args
+    ----
+        threshold:
+            The threshold to determine convergence. If the difference between
+            original auth/hub values and new auth/hub values is less than this
+            threshold, the algorithm is considered to be converged. The default is 1e-8.
+        max_loop:
+            The maximum number of loops to run the algorithm. If the algorithm
+            does not converge within this number of loops, it is forced to stop. The
+            default is 1000.
+    """
+
     def __init__(self, threshold: float = 1e-8, max_loop: int = 1000) -> None:
         collector = HITSRankingDataCollector()
         ranker = HITSRanker(threshold=threshold, max_loop=max_loop)
         super().__init__(collector, ranker)
 
     @classmethod
     def collect_data_from_dict(cls, obj: Dict[str, Any]) -> HITSRankingData:
```

### Comparing `py-pdf-term-0.18.1/py_pdf_term/methods/_methods/mcvalue.py` & `py_pdf_term-1.0.0/py_pdf_term/methods/_methods/mcvalue.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 from .base import BaseSingleDomainRankingMethod
 from .collectors import MCValueRankingDataCollector
 from .rankers import MCValueRanker
 from .rankingdata import MCValueRankingData
 
 
 class MCValueMethod(BaseSingleDomainRankingMethod[MCValueRankingData]):
+    """A ranking method by MC-Value algorithm."""
+
     def __init__(self) -> None:
         collector = MCValueRankingDataCollector()
         ranker = MCValueRanker()
         super().__init__(collector, ranker)
 
     @classmethod
     def collect_data_from_dict(cls, obj: Dict[str, Any]) -> MCValueRankingData:
```

### Comparing `py-pdf-term-0.18.1/py_pdf_term/methods/_methods/mdp.py` & `py_pdf_term-1.0.0/py_pdf_term/methods/_methods/tfidf.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from typing import Any, Callable, Dict, Iterable
+from typing import Any, Dict
 
 from .base import BaseMultiDomainRankingMethod
-from .collectors import MDPRankingDataCollector
-from .rankers import MDPRanker
-from .rankingdata import MDPRankingData
+from .collectors import TFIDFRankingDataCollector
+from .rankers import TFIDFRanker
+from .rankingdata import TFIDFRankingData
 
 
-class MDPMethod(BaseMultiDomainRankingMethod[MDPRankingData]):
-    def __init__(
-        self, compile_scores: Callable[[Iterable[float]], float] = min
-    ) -> None:
-        collector = MDPRankingDataCollector()
-        ranker = MDPRanker(compile_scores=compile_scores)
+class TFIDFMethod(BaseMultiDomainRankingMethod[TFIDFRankingData]):
+    """A ranking method by TF-IDF algorithm."""
+
+    def __init__(self) -> None:
+        collector = TFIDFRankingDataCollector()
+        ranker = TFIDFRanker()
         super().__init__(collector, ranker)
 
     @classmethod
-    def collect_data_from_dict(cls, obj: Dict[str, Any]) -> MDPRankingData:
-        return MDPRankingData(**obj)
+    def collect_data_from_dict(cls, obj: Dict[str, Any]) -> TFIDFRankingData:
+        return TFIDFRankingData(**obj)
```

### Comparing `py-pdf-term-0.18.1/py_pdf_term/methods/_methods/rankers/flr.py` & `py_pdf_term-1.0.0/py_pdf_term/methods/_methods/rankers/flr.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,20 @@
-from py_pdf_term._common.data import ScoredTerm, Term
-from py_pdf_term._common.extended_math import extended_log10
+from py_pdf_term._common.data import ScoredTerm
+from py_pdf_term._common.utils import extended_log10
 from py_pdf_term.candidates import DomainCandidateTermList
+from py_pdf_term.tokenizers import Term
 
 from ..data import MethodTermRanking
 from ..rankingdata import FLRRankingData
 from .base import BaseSingleDomainRanker
 
 
 class FLRRanker(BaseSingleDomainRanker[FLRRankingData]):
+    """A term ranker by FLR algorithm."""
+
     def __init__(self) -> None:
         pass
 
     def rank_terms(
         self, domain_candidates: DomainCandidateTermList, ranking_data: FLRRankingData
     ) -> MethodTermRanking:
         domain_candidates_dict = domain_candidates.to_nostyle_candidates_dict(
@@ -19,15 +22,15 @@
         )
         ranking = list(
             map(
                 lambda candidate: self._calculate_score(candidate, ranking_data),
                 domain_candidates_dict.values(),
             )
         )
-        ranking.sort(key=lambda term: -term.score)
+        ranking.sort(key=lambda term: term.score, reverse=True)
         return MethodTermRanking(domain_candidates.domain, ranking)
 
     def _calculate_score(
         self, candidate: Term, ranking_data: FLRRankingData
     ) -> ScoredTerm:
         candidate_lemma = candidate.lemma()
         num_tokens = len(candidate.tokens)
```

### Comparing `py-pdf-term-0.18.1/py_pdf_term/methods/_methods/rankers/hits.py` & `py_pdf_term-1.0.0/py_pdf_term/methods/_methods/rankers/hits.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,60 @@
 from dataclasses import dataclass
 from math import sqrt
 from typing import Dict
 
-from py_pdf_term._common.data import ScoredTerm, Term
-from py_pdf_term._common.extended_math import extended_log10
+from py_pdf_term._common.data import ScoredTerm
+from py_pdf_term._common.utils import extended_log10
 from py_pdf_term.candidates import DomainCandidateTermList
+from py_pdf_term.tokenizers import Term
 
 from ..data import MethodTermRanking
 from ..rankingdata import HITSRankingData
 from .base import BaseSingleDomainRanker
 
 
 @dataclass(frozen=True)
 class HITSAuthHubData:
+    """Auth and hub values of tokens for HITS algorithm.
+
+    Args
+    ----
+        token_auth:
+            Auth value of the token. The more tokens links to, the larger the auth value
+            becomes. The initial auth value is 1.0.
+        token_hub:
+            Hub value of the term. The more tokens is linked from, the larger the hub
+            value becomes. The initial hub value is 1.0.
+    """
+
     token_auth: Dict[str, float]
-    # auth value of the token
-    # the more tokens links to, the larger the auth value becomes
-    # initial auth value is 1.0
     token_hub: Dict[str, float]
-    # hub value of the term
-    # the more tokens is linked from, the larger the hub value becomes
-    # initial hub value is 1.0
 
 
 class HITSRanker(BaseSingleDomainRanker[HITSRankingData]):
+    """A term ranker by HITS algorithm.
+
+    Args
+    ----
+        threshold:
+            The threshold to determine convergence. If the difference between
+            original auth/hub values and new auth/hub values is less than this
+            threshold, the algorithm is considered to be converged. The default is 1e-8.
+        max_loop:
+            The maximum number of loops to run the algorithm. If the algorithm
+            does not converge within this number of loops, it is forced to stop. The
+            default is 1000.
+    """
+
     def __init__(self, threshold: float = 1e-8, max_loop: int = 1000) -> None:
+        if threshold <= 0:
+            raise ValueError("threshold must be positive")
+        if max_loop <= 0:
+            raise ValueError("max_loop must be positive")
+
         self._threshold = threshold
         self._max_loop = max_loop
 
     def rank_terms(
         self, domain_candidates: DomainCandidateTermList, ranking_data: HITSRankingData
     ) -> MethodTermRanking:
         auth_hub_data = self._create_auth_hub_data(ranking_data)
@@ -39,15 +65,15 @@
             map(
                 lambda candidate: self._calculate_score(
                     candidate, ranking_data, auth_hub_data
                 ),
                 domain_candidates_dict.values(),
             )
         )
-        ranking.sort(key=lambda term: -term.score)
+        ranking.sort(key=lambda term: term.score, reverse=True)
         return MethodTermRanking(domain_candidates.domain, ranking)
 
     def _create_auth_hub_data(self, ranking_data: HITSRankingData) -> HITSAuthHubData:
         token_auth: Dict[str, float] = {
             token_lemma: 1.0 for token_lemma in ranking_data.left_freq
         }
         token_hub: Dict[str, float] = {
```

### Comparing `py-pdf-term-0.18.1/py_pdf_term/methods/_methods/rankers/mcvalue.py` & `py_pdf_term-1.0.0/py_pdf_term/methods/_methods/rankers/tfidf.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,53 +1,61 @@
-from py_pdf_term._common.data import ScoredTerm, Term
-from py_pdf_term._common.extended_math import extended_log10
+from math import log10
+from typing import List
+
+from py_pdf_term._common.data import ScoredTerm
+from py_pdf_term._common.utils import extended_log10
 from py_pdf_term.candidates import DomainCandidateTermList
+from py_pdf_term.tokenizers import Term
 
 from ..data import MethodTermRanking
-from ..rankingdata import MCValueRankingData
-from .base import BaseSingleDomainRanker
+from ..rankingdata import TFIDFRankingData
+from .base import BaseMultiDomainRanker
+
 
+class TFIDFRanker(BaseMultiDomainRanker[TFIDFRankingData]):
+    """A term ranker by TF-IDF algorithm."""
 
-class MCValueRanker(BaseSingleDomainRanker[MCValueRankingData]):
     def __init__(self) -> None:
         pass
 
     def rank_terms(
         self,
         domain_candidates: DomainCandidateTermList,
-        ranking_data: MCValueRankingData,
+        ranking_data_list: List[TFIDFRankingData],
     ) -> MethodTermRanking:
-        domain_candidates_dict = domain_candidates.to_nostyle_candidates_dict(
-            to_str=lambda candidate: candidate.lemma()
+        domain_candidates_dict = domain_candidates.to_nostyle_candidates_dict()
+        ranking_data = next(
+            filter(
+                lambda item: item.domain == domain_candidates.domain,
+                ranking_data_list,
+            )
         )
         ranking = list(
             map(
-                lambda candidate: self._calculate_score(candidate, ranking_data),
+                lambda candidate: self._calculate_score(
+                    candidate, ranking_data, ranking_data_list
+                ),
                 domain_candidates_dict.values(),
             )
         )
-        ranking.sort(key=lambda term: -term.score)
+        ranking.sort(key=lambda term: term.score, reverse=True)
         return MethodTermRanking(domain_candidates.domain, ranking)
 
     def _calculate_score(
-        self, candidate: Term, ranking_data: MCValueRankingData
+        self,
+        candidate: Term,
+        ranking_data: TFIDFRankingData,
+        ranking_data_list: List[TFIDFRankingData],
     ) -> ScoredTerm:
         candidate_lemma = candidate.lemma()
 
-        term_freq = ranking_data.term_freq.get(candidate_lemma, 0)
-        container_terms = ranking_data.container_terms.get(candidate_lemma, set())
-        num_containers = len(container_terms)
-        container_freq = sum(
-            map(
-                lambda container: ranking_data.term_freq.get(container, 0),
-                container_terms,
-            )
-        )
+        tf = ranking_data.term_freq.get(candidate_lemma, 0)
+        log_tf = log10(tf) if tf > 0 else 0.0
 
-        term_len_score = extended_log10(len(candidate.tokens))
-        freq_score = extended_log10(
-            term_freq - container_freq / num_containers
-            if num_containers > 0
-            else term_freq
+        num_docs = sum(map(lambda data: data.num_docs, ranking_data_list))
+        df = sum(
+            map(lambda data: data.doc_freq.get(candidate_lemma, 0), ranking_data_list)
         )
-        score = term_len_score + freq_score
+        log_idf = log10(num_docs / df) if df > 0 else 0.0
+
+        score = extended_log10(log_tf * log_idf)
         return ScoredTerm(candidate_lemma, score)
```

### Comparing `py-pdf-term-0.18.1/py_pdf_term/methods/_methods/rankers/mdp.py` & `py_pdf_term-1.0.0/py_pdf_term/methods/_methods/rankers/mdp.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,23 +1,25 @@
-from typing import Callable, Iterable, List
+from sys import float_info
+from typing import List
 
-from py_pdf_term._common.data import ScoredTerm, Term
-from py_pdf_term._common.extended_math import extended_log10
+from py_pdf_term._common.data import ScoredTerm
+from py_pdf_term._common.utils import extended_log10
 from py_pdf_term.candidates import DomainCandidateTermList
+from py_pdf_term.tokenizers import Term
 
 from ..data import MethodTermRanking
 from ..rankingdata import MDPRankingData
 from .base import BaseMultiDomainRanker
 
 
 class MDPRanker(BaseMultiDomainRanker[MDPRankingData]):
-    def __init__(
-        self, compile_scores: Callable[[Iterable[float]], float] = min
-    ) -> None:
-        self._compile_scores = compile_scores
+    """A term ranker by MDP algorithm."""
+
+    def __init__(self) -> None:
+        pass
 
     def rank_terms(
         self,
         domain_candidates: DomainCandidateTermList,
         ranking_data_list: List[MDPRankingData],
     ) -> MethodTermRanking:
         domain_candidates_dict = domain_candidates.to_nostyle_candidates_dict(
@@ -39,25 +41,25 @@
             map(
                 lambda candidate: self._calculate_score(
                     candidate, ranking_data, other_ranking_data_list
                 ),
                 domain_candidates_dict.values(),
             )
         )
-        ranking.sort(key=lambda term: -term.score)
+        ranking.sort(key=lambda term: term.score, reverse=True)
         return MethodTermRanking(domain_candidates.domain, ranking)
 
     def _calculate_score(
         self,
         candidate: Term,
         ranking_data: MDPRankingData,
         other_ranking_data_list: List[MDPRankingData],
     ) -> ScoredTerm:
         candidate_lemma = candidate.lemma()
-        score = self._compile_scores(
+        score = min(
             map(
                 lambda other_ranking_data: self._calculate_zvalue(
                     candidate, ranking_data, other_ranking_data
                 ),
                 other_ranking_data_list,
             )
         )
@@ -68,24 +70,27 @@
         self,
         candidate: Term,
         our_ranking_data: MDPRankingData,
         their_ranking_data: MDPRankingData,
     ) -> float:
         candidate_lemma = candidate.lemma()
 
+        num_terms = our_ranking_data.num_terms + their_ranking_data.num_terms
+
         our_term_freq = our_ranking_data.term_freq.get(candidate_lemma, 0)
         their_term_freq = their_ranking_data.term_freq.get(candidate_lemma, 0)
+        term_freq = our_term_freq + their_term_freq
+
+        if term_freq == 0 or term_freq == num_terms:
+            return -float_info.max
 
         our_inum_terms = 1 / our_ranking_data.num_terms
         their_inum_terms = 1 / their_ranking_data.num_terms
 
         our_term_prob = our_term_freq / our_ranking_data.num_terms
         their_term_prob = their_term_freq / their_ranking_data.num_terms
-
-        term_prob = (our_term_freq + their_term_freq) / (
-            our_ranking_data.num_terms + their_ranking_data.num_terms
-        )
+        term_prob = term_freq / num_terms
 
         return extended_log10(
             (our_term_prob - their_term_prob)
             / (term_prob * (1.0 - term_prob) * (our_inum_terms + their_inum_terms))
         )
```

### Comparing `py-pdf-term-0.18.1/py_pdf_term/methods/_methods/rankingdata/flr.py` & `py_pdf_term-1.0.0/py_pdf_term/methods/_methods/rankingdata/tfidf.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,19 +1,28 @@
 from dataclasses import dataclass
 from typing import Dict
 
 from .base import BaseRankingData
 
 
 @dataclass(frozen=True)
-class FLRRankingData(BaseRankingData):
+class TFIDFRankingData(BaseRankingData):
+    """Data of technical terms of a domain for TF-IDF algorithm.
+
+    Args
+    ----
+        domain:
+            Domain name. (e.g., "natural language processing")
+        term_freq:
+            Brute force counting of lemmatized term occurrences in the domain.
+            Count even if the lemmatized term occurs as a part of a lemmatized phrase.
+        doc_freq:
+            Number of documents in the domain that contain the lemmatized term.
+            Count even if the lemmatized term occurs as a part of a lemmatized phrase.
+        num_docs:
+            Number of documents in the domain.
+    """
+
     domain: str
-    # unique domain name
     term_freq: Dict[str, int]
-    # brute force counting of lemmatized term occurrences in the domain
-    # count even if the lemmatized term occurs as a part of a lemmatized phrase
-    left_freq: Dict[str, Dict[str, int]]
-    # number of occurrences of lemmatized (left, token) in the domain
-    # if token or left is meaningless this is fixed at zero
-    right_freq: Dict[str, Dict[str, int]]
-    # number of occurrences of lemmatized (token, right) in the domain
-    # if token or right is meaningless this is fixed at zero
+    doc_freq: Dict[str, int]
+    num_docs: int
```

### Comparing `py-pdf-term-0.18.1/py_pdf_term/methods/_methods/rankingdata/mcvalue.py` & `py_pdf_term-1.0.0/py_pdf_term/methods/_methods/rankingdata/mcvalue.py`

 * *Files 17% similar despite different names*

```diff
@@ -2,23 +2,32 @@
 from typing import Any, Dict, Set
 
 from .base import BaseRankingData
 
 
 @dataclass(frozen=True)
 class MCValueRankingData(BaseRankingData):
+    """Data of technical terms of a domain for MC-Value algorithm.
+
+    Args
+    ----
+        domain:
+            Domain name. (e.g., "natural language processing")
+        term_freq:
+            Brute force counting of lemmatized term occurrences in the domain.
+            Count even if the lemmatized term occurs as a part of a lemmatized phrase.
+        container_terms:
+            Set of containers of the lemmatized term in the domain.
+            (term, container) is valid iff the container contains the term as a proper
+            subsequence.
+    """
+
     domain: str
-    # unique domain name
     term_freq: Dict[str, int]
-    # brute force counting of lemmatized term occurrences in the domain
-    # count even if the lemmatized term occurs as a part of a lemmatized phrase
     container_terms: Dict[str, Set[str]]
-    # set of containers of the lemmatized term in the domain
-    # (term, container) is valid iff the container contains the term
-    # as a proper subsequence
 
     def to_dict(self) -> Dict[str, Any]:
         container_terms = {
             term: list(containers) for term, containers in self.container_terms.items()
         }
         return {
             "domain": self.domain,
```

### Comparing `py-pdf-term-0.18.1/py_pdf_term/pdftoxml/_pdftoxml/textful.py` & `py_pdf_term-1.0.0/py_pdf_term/pdftoxml/_pdftoxml/textful.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,90 +1,117 @@
-# pyright:reportGeneralTypeIssues=false
-# pyright:reportUnknownMemberType=false
-# pyright:reportUnknownParameterType=false
-# pyright:reportUnknownArgumentType=false
-# pyright:reportMissingParameterType=false
-# pyright:reportMissingTypeArgument=false
-# pyright:reportIncompatibleMethodOverride=false
-
 from dataclasses import dataclass
-from typing import Any, BinaryIO, Optional, Union
+from typing import Any, BinaryIO, Optional, Sequence, Tuple, Union
 
-from pdfminer.converter import PDFConverter
+from pdfminer.converter import (
+    Matrix,
+    PathSegment,
+    PDFConverter,
+    PDFGraphicState,
+    PDFStream,
+    Rect,
+)
 from pdfminer.layout import (
     LAParams,
     LTAnno,
     LTChar,
     LTPage,
     LTText,
     LTTextBox,
     LTTextLine,
 )
 from pdfminer.pdfinterp import PDFResourceManager
 from pdfminer.utils import bbox2str, enc
 
 from .utils import clean_content_text
 
+NColor = Union[float, Tuple[float, float, float], Tuple[float, float, float, float]]
+
 
 @dataclass
 class TextboxState:
     within_section: bool
     size: float
-    ncolor: str
+    ncolor: Optional[NColor]
     bbox: str
     text: str
 
 
-class TextfulXMLConverter(PDFConverter):
+class TextfulXMLConverter(PDFConverter[BinaryIO]):
+    """A PDFConverter subclass that outputs textful XML format.
+
+    Args
+    ----
+        rsrcmgr:
+            A PDFResourceManager object from pdfminer.
+        outfp:
+            A file-like object to output XML.
+        codec:
+            A codec name to encode XML.
+        pageno:
+            A page number to start.
+        laparams:
+            A LAParams object from pdfminer.
+        nfc_norm:
+            If True, normalize text to NFC, otherwise keep original.
+        include_pattern:
+            A regular expression pattern of text to include in the output.
+        exclude_pattern:
+            A regular expression pattern of text to exclude from the output (overrides
+            include_pattern).
+    """
+
     def __init__(
         self,
         rsrcmgr: PDFResourceManager,
         outfp: BinaryIO,
         codec: str = "utf-8",
         pageno: int = 1,
         laparams: Optional[LAParams] = None,
         nfc_norm: bool = True,
         include_pattern: Optional[str] = None,
         exclude_pattern: Optional[str] = None,
     ) -> None:
-        PDFConverter.__init__(self, rsrcmgr, outfp, codec, pageno, laparams)
+        super().__init__(rsrcmgr, outfp, codec, pageno, laparams)
 
         def _clean_content_text(text: str) -> str:
             return clean_content_text(text, nfc_norm, include_pattern, exclude_pattern)
 
         self._clean_content_text = _clean_content_text
 
     def write_header(self) -> None:
-        if self.codec:
-            self._write('<?xml version="1.0" encoding="%s" ?>\n' % self.codec)
-        else:
-            self._write('<?xml version="1.0" ?>\n')
-
+        self._write('<?xml version="1.0" encoding="%s" ?>\n' % self.codec)
         self._write("<pages>\n")
 
     def receive_layout(self, ltpage: LTPage) -> None:
         self._render(ltpage)
 
     def write_footer(self) -> None:
         self._write("</pages>\n")
 
     # override to ignore LTFigure
-    def begin_figure(self, name, bbox, matrix) -> None:
+    def begin_figure(self, name: str, bbox: Rect, matrix: Matrix) -> None:
         pass
 
     # override to ignore LTFigure
-    def end_figure(self, name) -> None:
+    def end_figure(self, _: str) -> None:
         pass
 
     # override to ignore LTImage
-    def render_image(self, name, stream) -> None:
+    def render_image(self, name: str, stream: PDFStream) -> None:
         pass
 
     # override to ignore LTLine, LTRect and LTCurve
-    def paint_path(self, graphicstate, stroke, fill, evenodd, path) -> None:
+    def paint_path(
+        self,
+        gstate: PDFGraphicState,
+        stroke: bool,
+        fill: bool,
+        evenodd: bool,
+        path: Sequence[PathSegment],
+    ) -> None:
         pass
 
     def _render(self, item: Any) -> None:
         if isinstance(item, LTPage):
             self._render_page(item)
         elif isinstance(item, LTTextBox):
             self._render_textbox(item)
@@ -94,15 +121,15 @@
     def _render_page(self, ltpage: LTPage) -> None:
         self._write('<page id="%s">\n' % ltpage.pageid)
         for child in ltpage:
             self._render(child)
         self._write("</page>\n")
 
     def _render_textbox(self, lttextbox: LTTextBox) -> None:
-        state = TextboxState(False, 0.0, "", "", "")
+        state = TextboxState(False, 0.0, None, "", "")
 
         def render_textbox_child(child: Any) -> None:
             if isinstance(child, LTTextLine):
                 for grandchild in child:
                     render_textbox_child(grandchild)
             elif isinstance(child, LTChar):
                 if not state.within_section:
@@ -118,15 +145,15 @@
                 if not state.within_section:
                     pass
                 elif text_section_continues(child):
                     state.text += child.get_text()
                 else:
                     exit_text_section()
 
-        def enter_text_section(item: Union[LTChar, LTAnno]) -> None:
+        def enter_text_section(item: LTChar) -> None:
             state.within_section = True
             state.size = item.size
             state.ncolor = item.graphicstate.ncolor
             state.bbox = bbox2str(item.bbox)
             state.text = ""
 
         def text_section_continues(item: Union[LTChar, LTAnno]) -> bool:
@@ -148,15 +175,15 @@
                     % (state.size, state.ncolor, state.bbox)
                 )
                 self._write(enc(text))
                 self._write("</text>\n")
 
             state.within_section = False
             state.size = 0.0
-            state.ncolor = ""
+            state.ncolor = None
             state.bbox = ""
             state.text = ""
 
         for child in lttextbox:
             render_textbox_child(child)
 
         exit_text_section()
@@ -165,10 +192,9 @@
         text = self._clean_content_text(lttext.get_text())
         if text:
             self._write("<text>")
             self._write(enc(text))
             self._write("</text>\n")
 
     def _write(self, text: str) -> None:
-        if self.codec:
-            text = text.encode(self.codec)
-        self.outfp.write(text)
+        text_bytes = text.encode(self.codec)
+        self.outfp.write(text_bytes)
```

### Comparing `py-pdf-term-0.18.1/py_pdf_term/pdftoxml/_pdftoxml/utils.py` & `py_pdf_term-1.0.0/py_pdf_term/pdftoxml/_pdftoxml/utils.py`

 * *Files identical despite different names*

### Comparing `py-pdf-term-0.18.1/py_pdf_term/stylings/_stylings/scorer.py` & `py_pdf_term-1.0.0/py_pdf_term/stylings/_stylings/scorer.py`

 * *Files 17% similar despite different names*

```diff
@@ -8,33 +8,71 @@
 )
 
 from .data import DomainStylingScoreList, PageStylingScoreList, PDFStylingScoreList
 from .scores import BaseStylingScore, ColorScore, FontsizeScore
 
 
 class StylingScorer:
+    """A scorer for styling scores. The styling scores are combined by multiplication of
+    each score.
+
+    Args
+    ----
+        styling_score_clses:
+            styling scorers to be combined. If None, the default scorers are used.
+            The default scorers are FontsizeScore and ColorScore.
+    """
+
     def __init__(
         self, styling_score_clses: Optional[List[Type[BaseStylingScore]]] = None
     ) -> None:
         if styling_score_clses is None:
             styling_score_clses = [FontsizeScore, ColorScore]
 
         self._styling_score_clses = styling_score_clses
 
     def score_domain_candidates(
         self, domain_candidates: DomainCandidateTermList
     ) -> DomainStylingScoreList:
+        """Calculate styling scores for each candidate term in a domain.
+
+        Args
+        ----
+            domain_candidates:
+                List of candidate terms in a domain. The target of analysis.
+
+        Returns
+        -------
+            DomainStylingScoreList:
+                A list of styling scores for each candidate term in a domain. The
+                scores are sorted in descending order.
+        """
+
         return DomainStylingScoreList(
             domain_candidates.domain,
             list(map(self.score_pdf_candidates, domain_candidates.pdfs)),
         )
 
     def score_pdf_candidates(
         self, pdf_candidates: PDFCandidateTermList
     ) -> PDFStylingScoreList:
+        """Calculate styling scores for each candidate term in a PDF file.
+
+        Args
+        ----
+            pdf_candidates:
+                List of candidate terms in a PDF file. The target of analysis.
+
+        Returns
+        -------
+            PDFStylingScoreList:
+                A list of styling scores for each candidate term in a PDF file. The
+                scores are sorted in descending order.
+        """
+
         return PDFStylingScoreList(
             pdf_candidates.pdf_path,
             list(map(self._score_page_candidates, pdf_candidates.pages)),
         )
 
     def _score_page_candidates(
         self, page_candidates: PageCandidateTermList
@@ -53,9 +91,9 @@
                 if candidate_lemma not in scores or score > scores[candidate_lemma]:
                     scores[candidate_lemma] = score
 
             for candidate_lemma in styling_scores:
                 styling_scores[candidate_lemma] *= scores[candidate_lemma]
 
         ranking = list(map(lambda item: ScoredTerm(*item), styling_scores.items()))
-        ranking.sort(key=lambda scored_term: -scored_term.score)
+        ranking.sort(key=lambda scored_term: scored_term.score, reverse=True)
         return PageStylingScoreList(page_candidates.page_num, ranking)
```

### Comparing `py-pdf-term-0.18.1/py_pdf_term/stylings/_stylings/scores/color.py` & `py_pdf_term-1.0.0/py_pdf_term/stylings/_stylings/scores/color.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,26 @@
 from typing import Dict
 
-from py_pdf_term._common.data import Term
-from py_pdf_term._common.extended_math import extended_log10
+from py_pdf_term._common.utils import extended_log10
 from py_pdf_term.candidates import PageCandidateTermList
+from py_pdf_term.tokenizers import Term
 
 from .base import BaseStylingScore
 
 
 class ColorScore(BaseStylingScore):
+    """A styling score for font color. The more rarely the color appears in the page,
+    the higher the score is.
+
+    Args
+    ----
+        page_candidates:
+            List of candidate terms in a page of a PDF file. The target of analysis.
+    """
+
     def __init__(self, page_candidates: PageCandidateTermList) -> None:
         super().__init__(page_candidates)
 
         self._num_candidates = len(page_candidates.candidates)
 
         self._color_freq: Dict[str, int] = dict()
         for candidate in page_candidates.candidates:
```

### Comparing `py-pdf-term-0.18.1/py_pdf_term/techterms/_techterms/data.py` & `py_pdf_term-1.0.0/py_pdf_term/techterms/_techterms/data.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,14 +2,24 @@
 from typing import Any, Dict, List
 
 from py_pdf_term._common.data import ScoredTerm
 
 
 @dataclass(frozen=True)
 class PageTechnicalTermList:
+    """Page number and technical terms of the page.
+
+    Args
+    ----
+        page_num:
+            Page number of a PDF file.
+        terms:
+            Technical terms of the page.
+    """
+
     page_num: int
     terms: List[ScoredTerm]
 
     def to_dict(self) -> Dict[str, Any]:
         return {
             "page_num": self.page_num,
             "terms": list(map(lambda term: term.to_dict(), self.terms)),
@@ -19,14 +29,24 @@
     def from_dict(cls, obj: Dict[str, Any]) -> "PageTechnicalTermList":
         page_num, terms = obj["page_num"], obj["terms"]
         return cls(page_num, list(map(lambda item: ScoredTerm.from_dict(item), terms)))
 
 
 @dataclass(frozen=True)
 class PDFTechnicalTermList:
+    """Path of a PDF file and technical terms of the PDF file.
+
+    Args
+    ----
+        pdf_path:
+            Path of a PDF file.
+        pages:
+            Technical terms of each page of the PDF file.
+    """
+
     pdf_path: str
     pages: List[PageTechnicalTermList]
 
     def to_dict(self) -> Dict[str, Any]:
         return {
             "pdf_path": self.pdf_path,
             "pages": list(map(lambda page: page.to_dict(), self.pages)),
@@ -39,14 +59,24 @@
             pdf_path,
             list(map(lambda item: PageTechnicalTermList.from_dict(item), pages)),
         )
 
 
 @dataclass(frozen=True)
 class DomainTechnicalTermList:
+    """Domain name of PDF files and technical terms of the domain.
+
+    Args
+    ----
+        domain:
+            Domain name. (e.g., "natural language processing")
+        pdfs:
+            Technical terms of each PDF file of the domain.
+    """
+
     domain: str
     pdfs: List[PDFTechnicalTermList]
 
     def to_dict(self) -> Dict[str, Any]:
         return {
             "domain": self.domain,
             "pdfs": list(map(lambda pdf: pdf.to_dict(), self.pdfs)),
```

### Comparing `py-pdf-term-0.18.1/py_pdf_term/tokenizer/_tokenizer/english.py` & `py_pdf_term-1.0.0/py_pdf_term/tokenizers/_tokenizers/english.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,38 +1,41 @@
-# pyright:reportUnknownMemberType=false
-# pyright:reportUnknownArgumentType=false
-# pyright:reportUnknownLambdaType=false
-
 import re
 from typing import Any, List
 
 import en_core_web_sm
 
 from py_pdf_term._common.consts import ALPHABET_REGEX, SYMBOL_REGEX
 
-from .data import Token
 from .base import BaseLanguageTokenizer
+from .data import Token
 
 
 class EnglishTokenizer(BaseLanguageTokenizer):
-    def __init__(self) -> None:
-        enable_pipes = ["tok2vec", "tagger", "attribute_ruler", "lemmatizer"]
-        self._model = en_core_web_sm.load()
-        self._model.select_pipes(enable=enable_pipes)
-
-        self._en_regex = re.compile(ALPHABET_REGEX)
-        self._symbol_regex = re.compile(rf"({SYMBOL_REGEX})")
+    """A tokenizer for English. This tokenizer uses SpaCy's en_core_web_sm model."""
 
     def inscope(self, text: str) -> bool:
-        return self._en_regex.search(text) is not None
+        return EnglishTokenizer._regex.search(text) is not None
 
-    def tokenize(self, text: str) -> List[Token]:
-        text = self._symbol_regex.sub(r" \1 ", text)
-        return list(map(self._create_token, self._model(text)))
+    def tokenize(self, scoped_text: str) -> List[Token]:
+        scoped_text = EnglishTokenizer._symbol_regex.sub(r" \1 ", scoped_text)
+        return list(map(self._create_token, EnglishTokenizer._model(scoped_text)))
 
     def _create_token(self, token: Any) -> Token:
-        if self._symbol_regex.fullmatch(token.text):
+        if EnglishTokenizer._symbol_regex.fullmatch(token.text):
             return Token("en", token.text, "SYM", "*", "*", token.text)
 
         return Token(
             "en", token.text, token.pos_, token.tag_, "*", token.lemma_.lower()
         )
+
+    @classmethod
+    def class_init(cls) -> None:
+        model = en_core_web_sm.load()  # pyright: ignore[reportUnknownMemberType]
+        enable_pipes = ["tok2vec", "tagger", "attribute_ruler", "lemmatizer"]
+        model.select_pipes(enable=enable_pipes)
+        EnglishTokenizer._model = model
+
+        EnglishTokenizer._regex = re.compile(ALPHABET_REGEX)
+        EnglishTokenizer._symbol_regex = re.compile(rf"({SYMBOL_REGEX})")
+
+
+EnglishTokenizer.class_init()
```

### Comparing `py-pdf-term-0.18.1/py_pdf_term/tokenizer/_tokenizer/japanese.py` & `py_pdf_term-1.0.0/py_pdf_term/tokenizers/_tokenizers/japanese.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,49 +1,39 @@
-# pyright:reportUnknownMemberType=false
-# pyright:reportUnknownArgumentType=false
-# pyright:reportUnknownLambdaType=false
-
 import re
 from itertools import accumulate
 from typing import Any, List
 
 import ja_core_news_sm
 
 from py_pdf_term._common.consts import JAPANESE_REGEX, NOSPACE_REGEX, SYMBOL_REGEX
 
-from .data import Token
 from .base import BaseLanguageTokenizer
+from .data import Token
 
 SPACES = re.compile(r"\s+")
 DELIM_SPACE = re.compile(rf"(?<={NOSPACE_REGEX}) (?={NOSPACE_REGEX})")
 
 
 class JapaneseTokenizer(BaseLanguageTokenizer):
-    def __init__(self) -> None:
-        enable_pipes = []
-        self._model = ja_core_news_sm.load()
-        self._model.select_pipes(enable=enable_pipes)
-
-        self._ja_regex = re.compile(JAPANESE_REGEX)
-        self._symbol_regex = re.compile(rf"({SYMBOL_REGEX})")
+    """A tokenizer for Japanese. This tokenizer uses SpaCy's ja_core_news_sm model."""
 
     def inscope(self, text: str) -> bool:
-        return self._ja_regex.search(text) is not None
+        return JapaneseTokenizer._regex.search(text) is not None
 
-    def tokenize(self, text: str) -> List[Token]:
-        text = SPACES.sub(" ", text).strip()
+    def tokenize(self, scoped_text: str) -> List[Token]:
+        scoped_text = SPACES.sub(" ", scoped_text).strip()
         orginal_space_pos = {
             match.start() - offset
-            for offset, match in enumerate(re.finditer(r" ", text))
-            if DELIM_SPACE.match(text, match.start()) is not None
+            for offset, match in enumerate(re.finditer(r" ", scoped_text))
+            if DELIM_SPACE.match(scoped_text, match.start()) is not None
         }
 
-        text = DELIM_SPACE.sub("", text)
-        text = self._symbol_regex.sub(r" \1 ", text)
-        tokens = list(map(self._create_token, self._model(text)))
+        scoped_text = DELIM_SPACE.sub("", scoped_text)
+        scoped_text = JapaneseTokenizer._symbol_regex.sub(r" \1 ", scoped_text)
+        tokens = list(map(self._create_token, JapaneseTokenizer._model(scoped_text)))
 
         if not orginal_space_pos:
             return tokens
 
         tokenized_space_pos = set(
             accumulate(map(lambda token: len(str(token)), tokens))
         )
@@ -61,18 +51,31 @@
             else:
                 pos += len(str(tokens[i]))
                 i += 1
 
         return tokens
 
     def _create_token(self, token: Any) -> Token:
-        if self._symbol_regex.fullmatch(token.text):
+        if JapaneseTokenizer._symbol_regex.fullmatch(token.text):
             return Token("ja", token.text, "補助記号", "一般", "*", token.text)
 
         pos_with_categories = token.tag_.split("-")
         num_categories = len(pos_with_categories) - 1
 
         pos = pos_with_categories[0]
         category = pos_with_categories[1] if num_categories >= 1 else "*"
         subcategory = pos_with_categories[2] if num_categories >= 2 else "*"
 
         return Token("ja", token.text, pos, category, subcategory, token.lemma_.lower())
+
+    @classmethod
+    def class_init(cls) -> None:
+        model = ja_core_news_sm.load()  # pyright: ignore[reportUnknownMemberType]
+        enable_pipes = []
+        model.select_pipes(enable=enable_pipes)
+        JapaneseTokenizer._model = model
+
+        JapaneseTokenizer._regex = re.compile(JAPANESE_REGEX)
+        JapaneseTokenizer._symbol_regex = re.compile(rf"({SYMBOL_REGEX})")
+
+
+JapaneseTokenizer.class_init()
```

### Comparing `py-pdf-term-0.18.1/pyproject.toml` & `py_pdf_term-1.0.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,38 @@
 [tool.poetry]
 name = "py-pdf-term"
-version = "0.18.1"
+version = "1.0.0"
 description = "A fully-configurable terminology extraction module written in Python"
 authors = ["Yuya Suwa"]
 license = "MIT License"
 readme = "README.md"
 homepage = "https://github.com/kumachan-mis/py-pdf-term"
 repository = "https://github.com/kumachan-mis/py-pdf-term"
 keywords = ["terminology extraction", "technical term", "pdf"]
 
 [tool.poetry.dependencies]
-python = ">=3.7,<4.0"
-"pdfminer.six" = "^20211012"
-spacy = "^3.2.3"
+python = ">=3.10,<4.0"
+"pdfminer.six" = "^20221105"
+spacy = "^3.5.3"
 
-[tool.poetry.dev-dependencies]
-black = "^22.1.0"
-flake8 = "^4.0.1"
-flake8-quotes = "^3.3.1"
-ghp-import = "^2.0.1"
-isort = "^5.10.1"
-pep8-naming = "^0.12.1"
-pre-commit = "^2.17.0"
-pytest = "^7.0.1"
-pytest-cov = "^3.0.0"
-Sphinx = "^4.3.2"
+[tool.poetry.group.dev.dependencies]
+black = "^23.3.0"
+flake8 = "^6.0.0"
+flake8-quotes = "^3.3.2"
+ghp-import = "^2.1.0"
+isort = "^5.12.0"
+pep8-naming = "^0.13.3"
+pre-commit = "^3.3.2"
+pytest-mock = "^3.10.0"
+pytest = "^7.3.1"
+pytest-cov = "^4.0.0"
+Sphinx = "^7.0.1"
 
-[tool.poetry.dev-dependencies.en_core_web_sm]
-url = "https://github.com/explosion/spacy-models/releases/download/en_core_web_sm-3.2.0/en_core_web_sm-3.2.0.tar.gz"
+[tool.poetry.group.dev.dependencies.en_core_web_sm]
+url = "https://github.com/explosion/spacy-models/releases/download/en_core_web_sm-3.5.0/en_core_web_sm-3.5.0.tar.gz"
 
-[tool.poetry.dev-dependencies.ja_core_news_sm]
-url = "https://github.com/explosion/spacy-models/releases/download/ja_core_news_sm-3.2.0/ja_core_news_sm-3.2.0.tar.gz"
+[tool.poetry.group.dev.dependencies.ja_core_news_sm]
+url = "https://github.com/explosion/spacy-models/releases/download/ja_core_news_sm-3.5.0/ja_core_news_sm-3.5.0.tar.gz"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `py-pdf-term-0.18.1/PKG-INFO` & `py_pdf_term-1.0.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: py-pdf-term
-Version: 0.18.1
+Version: 1.0.0
 Summary: A fully-configurable terminology extraction module written in Python
 Home-page: https://github.com/kumachan-mis/py-pdf-term
 License: MIT
 Keywords: terminology extraction,technical term,pdf
 Author: Yuya Suwa
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Dist: pdfminer.six (>=20211012,<20211013)
-Requires-Dist: spacy (>=3.2.3,<4.0.0)
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: pdfminer.six (>=20221105,<20221106)
+Requires-Dist: spacy (>=3.5.3,<4.0.0)
 Project-URL: Repository, https://github.com/kumachan-mis/py-pdf-term
 Description-Content-Type: text/markdown
 
 # py-pdf-term
 
 A fully-configurable terminology extraction module written in Python
 
@@ -26,15 +25,15 @@
 ```
 pip install py-pdf-term
 ```
 
 You also need to install spaCy models `ja_core_news_sm` and `en_core_web_sm`, which this module depends on.
 
 ```
-pip install https://github.com/explosion/spacy-models/releases/download/ja_core_news_sm-3.2.0/ja_core_news_sm-3.2.0.tar.gz
-pip install https://github.com/explosion/spacy-models/releases/download/en_core_web_sm-3.2.0/en_core_web_sm-3.2.0.tar.gz
+pip install https://github.com/explosion/spacy-models/releases/download/ja_core_news_sm-3.5.0/ja_core_news_sm-3.5.0.tar.gz
+pip install https://github.com/explosion/spacy-models/releases/download/en_core_web_sm-3.5.0/en_core_web_sm-3.5.0.tar.gz
 ```
 
 ## Documentation
 
 https://kumachan-mis.github.io/py-pdf-term
```

