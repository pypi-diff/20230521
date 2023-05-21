# Comparing `tmp/timeblok_py-0.4.5.tar.gz` & `tmp/timeblok_py-0.5.0.tar.gz`

## Comparing `timeblok_py-0.4.5.tar` & `timeblok_py-0.5.0.tar`

### file list

```diff
@@ -1,41 +1,43 @@
--rw-r--r--   0        0        0     1142 1970-01-01 00:00:00.000000 timeblok_py-0.4.5/local_dependencies/timeblok/Cargo.toml
--rw-r--r--   0      501       20     2108 2023-05-02 12:02:14.000000 timeblok_py-0.4.5/local_dependencies/timeblok/src/blok.pest
--rw-r--r--   0      501       20     5915 2023-05-04 05:39:53.000000 timeblok_py-0.4.5/local_dependencies/timeblok/src/converter.rs
--rw-r--r--   0      501       20     5122 2023-03-29 01:03:59.000000 timeblok_py-0.4.5/local_dependencies/timeblok/src/environment.rs
--rw-r--r--   0      501       20     4621 2023-05-04 05:33:49.000000 timeblok_py-0.4.5/local_dependencies/timeblok/src/importer.rs
--rw-r--r--   0      501       20     1595 2023-05-02 12:02:14.000000 timeblok_py-0.4.5/local_dependencies/timeblok/src/ir/command.rs
--rw-r--r--   0      501       20      864 2023-04-29 02:18:21.000000 timeblok_py-0.4.5/local_dependencies/timeblok/src/ir/displays.rs
--rw-r--r--   0      501       20     7292 2023-03-29 01:03:59.000000 timeblok_py-0.4.5/local_dependencies/timeblok/src/ir/filter.rs
--rw-r--r--   0      501       20     1517 2023-03-29 01:03:59.000000 timeblok_py-0.4.5/local_dependencies/timeblok/src/ir/ident.rs
--rw-r--r--   0      501       20     9886 2023-05-04 05:51:06.000000 timeblok_py-0.4.5/local_dependencies/timeblok/src/ir/mod.rs
--rw-r--r--   0      501       20     1861 2023-05-04 00:31:24.000000 timeblok_py-0.4.5/local_dependencies/timeblok/src/lib.rs
--rw-r--r--   0      501       20       96 2023-03-29 01:03:59.000000 timeblok_py-0.4.5/local_dependencies/timeblok/src/output.rs
--rw-r--r--   0      501       20    12746 2023-05-02 12:02:14.000000 timeblok_py-0.4.5/local_dependencies/timeblok/src/parser.rs
--rw-r--r--   0      501       20     9510 2023-05-04 02:18:03.000000 timeblok_py-0.4.5/local_dependencies/timeblok/src/preset/mod.rs
--rw-r--r--   0      501       20     2717 2023-03-29 01:03:59.000000 timeblok_py-0.4.5/local_dependencies/timeblok/src/preset/workalendar.rs
--rw-r--r--   0      501       20     9753 2023-05-02 12:31:21.000000 timeblok_py-0.4.5/local_dependencies/timeblok/src/resolver.rs
--rw-r--r--   0      501       20       63 2023-05-03 23:54:33.000000 timeblok_py-0.4.5/local_dependencies/timeblok/src/tests/bloks/filter_dow.tb
--rw-r--r--   0      501       20       49 2023-05-03 23:55:01.000000 timeblok_py-0.4.5/local_dependencies/timeblok/src/tests/bloks/filter_workday.tb
--rw-r--r--   0      501       20       55 2023-05-03 23:54:36.000000 timeblok_py-0.4.5/local_dependencies/timeblok/src/tests/bloks/sanity.tb
--rw-r--r--   0      501       20      107 2023-05-04 00:03:45.000000 timeblok_py-0.4.5/local_dependencies/timeblok/src/tests/bloks/semester.tb
--rw-r--r--   0      501       20       37 2023-05-04 00:03:01.000000 timeblok_py-0.4.5/local_dependencies/timeblok/src/tests/bloks/todos.tb
--rw-r--r--   0      501       20       10 2023-05-03 15:04:27.000000 timeblok_py-0.4.5/local_dependencies/timeblok/src/tests/mod.rs
--rw-r--r--   0      501       20    32469 2023-05-03 15:30:02.000000 timeblok_py-0.4.5/local_dependencies/timeblok/src/tests/snapshots/timeblok__tests__tests__filters.snap
--rw-r--r--   0      501       20    32451 2023-05-04 01:47:21.000000 timeblok_py-0.4.5/local_dependencies/timeblok/src/tests/snapshots/timeblok__tests__tests__run_tests@filter_dow.tb.snap
--rw-r--r--   0      501       20    56475 2023-05-04 01:47:20.000000 timeblok_py-0.4.5/local_dependencies/timeblok/src/tests/snapshots/timeblok__tests__tests__run_tests@filter_workday.tb.snap
--rw-r--r--   0      501       20      640 2023-05-04 01:47:21.000000 timeblok_py-0.4.5/local_dependencies/timeblok/src/tests/snapshots/timeblok__tests__tests__run_tests@sanity.tb.snap
--rw-r--r--   0      501       20     3103 2023-05-04 01:47:20.000000 timeblok_py-0.4.5/local_dependencies/timeblok/src/tests/snapshots/timeblok__tests__tests__run_tests@semester.tb.snap
--rw-r--r--   0      501       20      504 2023-05-04 01:47:20.000000 timeblok_py-0.4.5/local_dependencies/timeblok/src/tests/snapshots/timeblok__tests__tests__run_tests@todos.tb.snap
--rw-r--r--   0      501       20      652 2023-05-03 15:30:02.000000 timeblok_py-0.4.5/local_dependencies/timeblok/src/tests/snapshots/timeblok__tests__tests__sanity.snap
--rw-r--r--   0      501       20      803 2023-05-04 04:53:32.000000 timeblok_py-0.4.5/local_dependencies/timeblok/src/tests/tests.rs
--rw-r--r--   0      501       20       63 2023-05-04 04:51:47.000000 timeblok_py-0.4.5/local_dependencies/timeblok/src/tests/wsm-bloks/filter_dow.tb
--rw-r--r--   0      501       20       49 2023-05-04 04:51:47.000000 timeblok_py-0.4.5/local_dependencies/timeblok/src/tests/wsm-bloks/filter_workday.tb
--rw-r--r--   0      501       20       55 2023-05-04 04:51:47.000000 timeblok_py-0.4.5/local_dependencies/timeblok/src/tests/wsm-bloks/sanity.tb
--rw-r--r--   0      501       20      107 2023-05-04 04:51:47.000000 timeblok_py-0.4.5/local_dependencies/timeblok/src/tests/wsm-bloks/semester.tb
--rw-r--r--   0      501       20       37 2023-05-04 04:51:47.000000 timeblok_py-0.4.5/local_dependencies/timeblok/src/tests/wsm-bloks/todos.tb
--rw-r--r--   0      501       20     3467 2023-05-04 01:49:58.000000 timeblok_py-0.4.5/local_dependencies/timeblok/src/utils/mod.rs
--rw-r--r--   0        0        0      657 1970-01-01 00:00:00.000000 timeblok_py-0.4.5/Cargo.toml
--rw-r--r--   0      501       20      235 2023-05-11 07:30:42.000000 timeblok_py-0.4.5/pyproject.toml
--rw-r--r--   0      501       20      533 2023-05-11 07:53:18.000000 timeblok_py-0.4.5/src/lib.rs
--rw-r--r--   0      501       20    57498 2023-05-11 07:37:45.000000 timeblok_py-0.4.5/Cargo.lock
--rw-r--r--   0        0        0      143 1970-01-01 00:00:00.000000 timeblok_py-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0     1142 1970-01-01 00:00:00.000000 timeblok_py-0.5.0/local_dependencies/timeblok/Cargo.toml
+-rw-r--r--   0      501       20     2210 2023-05-21 15:03:04.000000 timeblok_py-0.5.0/local_dependencies/timeblok/src/blok.pest
+-rw-r--r--   0      501       20     6085 2023-05-21 14:28:49.000000 timeblok_py-0.5.0/local_dependencies/timeblok/src/converter.rs
+-rw-r--r--   0      501       20     5122 2023-03-29 01:03:59.000000 timeblok_py-0.5.0/local_dependencies/timeblok/src/environment.rs
+-rw-r--r--   0      501       20     4860 2023-05-21 14:32:23.000000 timeblok_py-0.5.0/local_dependencies/timeblok/src/importer.rs
+-rw-r--r--   0      501       20     1595 2023-05-02 12:02:14.000000 timeblok_py-0.5.0/local_dependencies/timeblok/src/ir/command.rs
+-rw-r--r--   0      501       20      864 2023-04-29 02:18:21.000000 timeblok_py-0.5.0/local_dependencies/timeblok/src/ir/displays.rs
+-rw-r--r--   0      501       20     7292 2023-03-29 01:03:59.000000 timeblok_py-0.5.0/local_dependencies/timeblok/src/ir/filter.rs
+-rw-r--r--   0      501       20     1517 2023-03-29 01:03:59.000000 timeblok_py-0.5.0/local_dependencies/timeblok/src/ir/ident.rs
+-rw-r--r--   0      501       20    10303 2023-05-21 14:18:29.000000 timeblok_py-0.5.0/local_dependencies/timeblok/src/ir/mod.rs
+-rw-r--r--   0      501       20     1861 2023-05-04 00:31:24.000000 timeblok_py-0.5.0/local_dependencies/timeblok/src/lib.rs
+-rw-r--r--   0      501       20       96 2023-03-29 01:03:59.000000 timeblok_py-0.5.0/local_dependencies/timeblok/src/output.rs
+-rw-r--r--   0      501       20    13546 2023-05-21 14:41:42.000000 timeblok_py-0.5.0/local_dependencies/timeblok/src/parser.rs
+-rw-r--r--   0      501       20     9510 2023-05-04 02:18:03.000000 timeblok_py-0.5.0/local_dependencies/timeblok/src/preset/mod.rs
+-rw-r--r--   0      501       20     2717 2023-03-29 01:03:59.000000 timeblok_py-0.5.0/local_dependencies/timeblok/src/preset/workalendar.rs
+-rw-r--r--   0      501       20    10804 2023-05-21 14:53:53.000000 timeblok_py-0.5.0/local_dependencies/timeblok/src/resolver.rs
+-rw-r--r--   0      501       20       63 2023-05-03 23:54:33.000000 timeblok_py-0.5.0/local_dependencies/timeblok/src/tests/bloks/filter_dow.tb
+-rw-r--r--   0      501       20       49 2023-05-03 23:55:01.000000 timeblok_py-0.5.0/local_dependencies/timeblok/src/tests/bloks/filter_workday.tb
+-rw-r--r--   0      501       20      169 2023-05-21 14:54:43.000000 timeblok_py-0.5.0/local_dependencies/timeblok/src/tests/bloks/notes.tb
+-rw-r--r--   0      501       20       55 2023-05-03 23:54:36.000000 timeblok_py-0.5.0/local_dependencies/timeblok/src/tests/bloks/sanity.tb
+-rw-r--r--   0      501       20      107 2023-05-04 00:03:45.000000 timeblok_py-0.5.0/local_dependencies/timeblok/src/tests/bloks/semester.tb
+-rw-r--r--   0      501       20       37 2023-05-04 00:03:01.000000 timeblok_py-0.5.0/local_dependencies/timeblok/src/tests/bloks/todos.tb
+-rw-r--r--   0      501       20       10 2023-05-03 15:04:27.000000 timeblok_py-0.5.0/local_dependencies/timeblok/src/tests/mod.rs
+-rw-r--r--   0      501       20    32469 2023-05-03 15:30:02.000000 timeblok_py-0.5.0/local_dependencies/timeblok/src/tests/snapshots/timeblok__tests__tests__filters.snap
+-rw-r--r--   0      501       20    32451 2023-05-04 01:47:21.000000 timeblok_py-0.5.0/local_dependencies/timeblok/src/tests/snapshots/timeblok__tests__tests__run_tests@filter_dow.tb.snap
+-rw-r--r--   0      501       20    56475 2023-05-04 01:47:20.000000 timeblok_py-0.5.0/local_dependencies/timeblok/src/tests/snapshots/timeblok__tests__tests__run_tests@filter_workday.tb.snap
+-rw-r--r--   0      501       20      776 2023-05-21 15:05:07.000000 timeblok_py-0.5.0/local_dependencies/timeblok/src/tests/snapshots/timeblok__tests__tests__run_tests@notes.tb.snap
+-rw-r--r--   0      501       20      640 2023-05-04 01:47:21.000000 timeblok_py-0.5.0/local_dependencies/timeblok/src/tests/snapshots/timeblok__tests__tests__run_tests@sanity.tb.snap
+-rw-r--r--   0      501       20     3103 2023-05-04 01:47:20.000000 timeblok_py-0.5.0/local_dependencies/timeblok/src/tests/snapshots/timeblok__tests__tests__run_tests@semester.tb.snap
+-rw-r--r--   0      501       20      504 2023-05-04 01:47:20.000000 timeblok_py-0.5.0/local_dependencies/timeblok/src/tests/snapshots/timeblok__tests__tests__run_tests@todos.tb.snap
+-rw-r--r--   0      501       20      652 2023-05-03 15:30:02.000000 timeblok_py-0.5.0/local_dependencies/timeblok/src/tests/snapshots/timeblok__tests__tests__sanity.snap
+-rw-r--r--   0      501       20      803 2023-05-04 04:53:32.000000 timeblok_py-0.5.0/local_dependencies/timeblok/src/tests/tests.rs
+-rw-r--r--   0      501       20       63 2023-05-04 04:51:47.000000 timeblok_py-0.5.0/local_dependencies/timeblok/src/tests/wsm-bloks/filter_dow.tb
+-rw-r--r--   0      501       20       49 2023-05-04 04:51:47.000000 timeblok_py-0.5.0/local_dependencies/timeblok/src/tests/wsm-bloks/filter_workday.tb
+-rw-r--r--   0      501       20       55 2023-05-04 04:51:47.000000 timeblok_py-0.5.0/local_dependencies/timeblok/src/tests/wsm-bloks/sanity.tb
+-rw-r--r--   0      501       20      107 2023-05-04 04:51:47.000000 timeblok_py-0.5.0/local_dependencies/timeblok/src/tests/wsm-bloks/semester.tb
+-rw-r--r--   0      501       20       37 2023-05-04 04:51:47.000000 timeblok_py-0.5.0/local_dependencies/timeblok/src/tests/wsm-bloks/todos.tb
+-rw-r--r--   0      501       20     3467 2023-05-04 01:49:58.000000 timeblok_py-0.5.0/local_dependencies/timeblok/src/utils/mod.rs
+-rw-r--r--   0        0        0      657 1970-01-01 00:00:00.000000 timeblok_py-0.5.0/Cargo.toml
+-rw-r--r--   0      501       20      235 2023-05-11 07:30:42.000000 timeblok_py-0.5.0/pyproject.toml
+-rw-r--r--   0      501       20      533 2023-05-11 07:53:18.000000 timeblok_py-0.5.0/src/lib.rs
+-rw-r--r--   0      501       20    57498 2023-05-21 15:07:38.000000 timeblok_py-0.5.0/Cargo.lock
+-rw-r--r--   0        0        0      143 1970-01-01 00:00:00.000000 timeblok_py-0.5.0/PKG-INFO
```

### Comparing `timeblok_py-0.4.5/local_dependencies/timeblok/Cargo.toml` & `timeblok_py-0.5.0/local_dependencies/timeblok/Cargo.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [package]
 name = "timeblok"
 description = "A language for event scheduling in plain text"
 
 edition="2021"
 license= "MIT/Apache-2.0"
 repository= "https://github.com/JettChenT/timeblok"
-version= "0.4.5"
+version= "0.5.0"
 authors= ["contact@jettchen.me"]
 homepage= "https://github.com/JettChenT/timeblok"
 
 [dependencies]
 pest = "2.5.2"
 pest_derive = "2.5.2"
 anyhow = {version = "1.0", features = ["backtrace"]}
```

### Comparing `timeblok_py-0.4.5/local_dependencies/timeblok/src/blok.pest` & `timeblok_py-0.5.0/local_dependencies/timeblok/src/blok.pest`

 * *Files 11% similar despite different names*

```diff
@@ -79,54 +79,61 @@
 000004e0: 585f 4441 5445 5449 4d45 207c 2046 4c45  X_DATETIME | FLE
 000004f0: 585f 4441 5445 207c 2054 494d 4520 7c20  X_DATE | TIME | 
 00000500: 4441 5445 5f46 494c 5445 527d 202f 2f20  DATE_FILTER} // 
 00000510: 446f 6e27 7420 7365 6520 6d75 6368 2076  Don't see much v
 00000520: 616c 7565 2069 6e20 6272 696e 6769 6e67  alue in bringing
 00000530: 2066 6c65 7820 746f 2074 696d 6520 696e   flex to time in
 00000540: 2064 6179 2e0a 5354 5249 4e47 203d 207b   day..STRING = {
-00000550: 225c 2222 207e 2028 2122 5c22 2220 7e20  "\"" ~ (!"\"" ~ 
-00000560: 4153 4349 4929 2a20 7e20 225c 2222 7d0a  ASCII)* ~ "\""}.
-00000570: 4341 5247 203d 207b 2821 284e 4557 4c49  CARG = {(!(NEWLI
-00000580: 4e45 7c57 4849 5445 5350 4143 4529 7e41  NE|WHITESPACE)~A
-00000590: 4e59 292b 7d0a 0a41 5247 5720 3d20 5f7b  NY)+}..ARGW = _{
-000005a0: 2028 4441 5445 5f46 494c 5445 5220 7c20   (DATE_FILTER | 
-000005b0: 4649 4c54 4552 207c 204e 554d 5f46 4945  FILTER | NUM_FIE
-000005c0: 4c44 7c20 4944 454e 5420 7c20 5354 5249  LD| IDENT | STRI
-000005d0: 4e47 207c 2043 4152 4729 207e 2057 4849  NG | CARG) ~ WHI
-000005e0: 5445 5350 4143 452a 7d0a 4152 4745 203d  TESPACE*}.ARGE =
-000005f0: 205f 7b20 2844 4154 455f 4649 4c54 4552   _{ (DATE_FILTER
-00000600: 207c 2046 494c 5445 5220 7c20 4e55 4d5f   | FILTER | NUM_
-00000610: 4649 454c 447c 2049 4445 4e54 207c 2053  FIELD| IDENT | S
-00000620: 5452 494e 4720 7c20 4341 5247 2920 7e20  TRING | CARG) ~ 
-00000630: 5748 4954 4553 5041 4345 2a20 7e20 284e  WHITESPACE* ~ (N
-00000640: 4557 4c49 4e45 7c45 4f49 297d 0a41 5247  EWLINE|EOI)}.ARG
-00000650: 5320 3d20 7b28 2141 5247 457e 4152 4757  S = {(!ARGE~ARGW
-00000660: 292a 7e41 5247 457d 0a43 4f4d 4d41 4e44  )*~ARGE}.COMMAND
-00000670: 203d 2024 7b22 2f22 207e 2028 4944 454e   = ${"/" ~ (IDEN
-00000680: 547e 5748 4954 4553 5041 4345 2920 7e20  T~WHITESPACE) ~ 
-00000690: 4152 4753 7d0a 0a52 414e 4745 203d 207b  ARGS}..RANGE = {
-000006a0: 4f43 4341 5349 4f4e 207e 2053 5020 7e20  OCCASION ~ SP ~ 
-000006b0: 227e 2220 7e20 5350 207e 204f 4343 4153  "~" ~ SP ~ OCCAS
-000006c0: 494f 4e7d 0a45 5645 4e54 5f48 4541 4445  ION}.EVENT_HEADE
-000006d0: 5220 3d20 7b28 5241 4e47 4520 7c20 4f43  R = {(RANGE | OC
-000006e0: 4341 5349 4f4e 2920 7e20 5350 207e 204e  CASION) ~ SP ~ N
-000006f0: 4f54 455f 4c49 4e45 7d0a 4e4f 5445 203d  OTE_LINE}.NOTE =
-00000700: 207b 2821 4e45 574c 494e 457e 414e 5929   {(!NEWLINE~ANY)
-00000710: 2b7d 0a4e 4f54 455f 4c49 4e45 203d 205f  +}.NOTE_LINE = _
-00000720: 7b4e 4f54 4520 7e20 4e45 574c 494e 453f  {NOTE ~ NEWLINE?
-00000730: 7d0a 4556 454e 5420 3d20 7b0a 2020 2020  }.EVENT = {.    
-00000740: 4556 454e 545f 4845 4144 4552 207e 204e  EVENT_HEADER ~ N
-00000750: 4557 4c49 4e45 2a20 7e0a 2020 2020 2821  EWLINE* ~.    (!
-00000760: 2845 5645 4e54 5f48 4541 4445 5220 7c20  (EVENT_HEADER | 
-00000770: 4f43 4341 5349 4f4e 207c 2046 4c45 585f  OCCASION | FLEX_
-00000780: 4f43 4341 5349 4f4e 2920 7e20 4e4f 5445  OCCASION) ~ NOTE
-00000790: 5f4c 494e 4529 2a0a 7d0a 464c 4558 5f45  _LINE)*.}.FLEX_E
-000007a0: 5645 4e54 5320 3d20 7b0a 0946 4c45 585f  VENTS = {..FLEX_
-000007b0: 4f43 4341 5349 4f4e 207e 204e 4557 4c49  OCCASION ~ NEWLI
-000007c0: 4e45 2a20 7e20 4556 454e 542a 0a7d 0a52  NE* ~ EVENT*.}.R
-000007d0: 4543 4f52 4420 3d20 7b45 5645 4e54 207c  ECORD = {EVENT |
-000007e0: 204f 4343 4153 494f 4e20 7c20 434f 4d4d   OCCASION | COMM
-000007f0: 414e 4420 7c20 464c 4558 5f45 5645 4e54  AND | FLEX_EVENT
-00000800: 5320 7c20 4e4f 5445 5f4c 494e 457d 0a46  S | NOTE_LINE}.F
-00000810: 494c 4520 3d20 7b0a 2020 2020 534f 4920  ILE = {.    SOI 
-00000820: 7e0a 2020 2020 2852 4543 4f52 4420 7e20  ~.    (RECORD ~ 
-00000830: 4e45 574c 494e 452a 292a 0a7d            NEWLINE*)*.}
+00000550: 2821 225c 2222 207e 2041 5343 4949 292a  (!"\"" ~ ASCII)*
+00000560: 7d0a 5354 5249 4e47 5f57 5241 5020 3d20  }.STRING_WRAP = 
+00000570: 5f7b 225c 2222 207e 2053 5452 494e 4720  _{"\"" ~ STRING 
+00000580: 7e20 225c 2222 7d0a 4341 5247 203d 207b  ~ "\""}.CARG = {
+00000590: 2821 284e 4557 4c49 4e45 7c57 4849 5445  (!(NEWLINE|WHITE
+000005a0: 5350 4143 4529 7e41 4e59 292b 7d0a 0a41  SPACE)~ANY)+}..A
+000005b0: 5247 5720 3d20 5f7b 2028 4441 5445 5f46  RGW = _{ (DATE_F
+000005c0: 494c 5445 5220 7c20 4649 4c54 4552 207c  ILTER | FILTER |
+000005d0: 204e 554d 5f46 4945 4c44 7c20 4944 454e   NUM_FIELD| IDEN
+000005e0: 5420 7c20 5354 5249 4e47 5f57 5241 5020  T | STRING_WRAP 
+000005f0: 7c20 4341 5247 2920 7e20 5748 4954 4553  | CARG) ~ WHITES
+00000600: 5041 4345 2a7d 0a41 5247 4520 3d20 5f7b  PACE*}.ARGE = _{
+00000610: 2028 4441 5445 5f46 494c 5445 5220 7c20   (DATE_FILTER | 
+00000620: 4649 4c54 4552 207c 204e 554d 5f46 4945  FILTER | NUM_FIE
+00000630: 4c44 7c20 4944 454e 5420 7c20 5354 5249  LD| IDENT | STRI
+00000640: 4e47 5f57 5241 5020 7c20 4341 5247 2920  NG_WRAP | CARG) 
+00000650: 7e20 5748 4954 4553 5041 4345 2a20 7e20  ~ WHITESPACE* ~ 
+00000660: 284e 4557 4c49 4e45 7c45 4f49 297d 0a41  (NEWLINE|EOI)}.A
+00000670: 5247 5320 3d20 7b28 2141 5247 457e 4152  RGS = {(!ARGE~AR
+00000680: 4757 292a 7e41 5247 457d 0a43 4f4d 4d41  GW)*~ARGE}.COMMA
+00000690: 4e44 203d 2024 7b22 2f22 207e 2028 4944  ND = ${"/" ~ (ID
+000006a0: 454e 547e 5748 4954 4553 5041 4345 2920  ENT~WHITESPACE) 
+000006b0: 7e20 4152 4753 7d0a 5052 4f50 4552 5459  ~ ARGS}.PROPERTY
+000006c0: 203d 2024 7b22 4022 207e 2028 4944 454e   = ${"@" ~ (IDEN
+000006d0: 547e 5748 4954 4553 5041 4345 2920 7e20  T~WHITESPACE) ~ 
+000006e0: 4152 4745 7d0a 0a52 414e 4745 203d 207b  ARGE}..RANGE = {
+000006f0: 4f43 4341 5349 4f4e 207e 2053 5020 7e20  OCCASION ~ SP ~ 
+00000700: 227e 2220 7e20 5350 207e 204f 4343 4153  "~" ~ SP ~ OCCAS
+00000710: 494f 4e7d 0a45 5645 4e54 5f48 4541 4445  ION}.EVENT_HEADE
+00000720: 5220 3d20 7b28 5241 4e47 4520 7c20 4f43  R = {(RANGE | OC
+00000730: 4341 5349 4f4e 2920 7e20 5350 207e 204e  CASION) ~ SP ~ N
+00000740: 4f54 455f 4c49 4e45 7d0a 4e4f 5445 203d  OTE_LINE}.NOTE =
+00000750: 207b 2821 4e45 574c 494e 457e 414e 5929   {(!NEWLINE~ANY)
+00000760: 2b7d 0a4e 4f54 455f 4c49 4e45 203d 205f  +}.NOTE_LINE = _
+00000770: 7b4e 4f54 4520 7e20 4e45 574c 494e 453f  {NOTE ~ NEWLINE?
+00000780: 7d0a 4556 454e 5420 3d20 7b0a 2020 2020  }.EVENT = {.    
+00000790: 4556 454e 545f 4845 4144 4552 207e 204e  EVENT_HEADER ~ N
+000007a0: 4557 4c49 4e45 2a20 7e0a 2020 2020 2821  EWLINE* ~.    (!
+000007b0: 2845 5645 4e54 5f48 4541 4445 5220 7c20  (EVENT_HEADER | 
+000007c0: 4f43 4341 5349 4f4e 207c 2046 4c45 585f  OCCASION | FLEX_
+000007d0: 4f43 4341 5349 4f4e 207c 2043 4f4d 4d41  OCCASION | COMMA
+000007e0: 4e44 2920 7e20 2850 524f 5045 5254 5920  ND) ~ (PROPERTY 
+000007f0: 7c4e 4f54 455f 4c49 4e45 2929 2a0a 7d0a  |NOTE_LINE))*.}.
+00000800: 464c 4558 5f45 5645 4e54 5320 3d20 7b0a  FLEX_EVENTS = {.
+00000810: 0946 4c45 585f 4f43 4341 5349 4f4e 207e  .FLEX_OCCASION ~
+00000820: 204e 4557 4c49 4e45 2a20 7e20 4556 454e   NEWLINE* ~ EVEN
+00000830: 542a 0a7d 0a52 4543 4f52 4420 3d20 7b45  T*.}.RECORD = {E
+00000840: 5645 4e54 207c 204f 4343 4153 494f 4e20  VENT | OCCASION 
+00000850: 7c20 434f 4d4d 414e 4420 7c20 464c 4558  | COMMAND | FLEX
+00000860: 5f45 5645 4e54 5320 7c20 4e4f 5445 5f4c  _EVENTS | NOTE_L
+00000870: 494e 457d 0a46 494c 4520 3d20 7b0a 2020  INE}.FILE = {.  
+00000880: 2020 534f 4920 7e0a 2020 2020 2852 4543    SOI ~.    (REC
+00000890: 4f52 4420 7e20 4e45 574c 494e 452a 292a  ORD ~ NEWLINE*)*
+000008a0: 0a7d                                     .}
```

### Comparing `timeblok_py-0.4.5/local_dependencies/timeblok/src/converter.rs` & `timeblok_py-0.5.0/local_dependencies/timeblok/src/converter.rs`

 * *Files 2% similar despite different names*

```diff
@@ -89,15 +89,18 @@
 }
 
 impl ExactEvent {
     fn to_icalevent(&self, key: Option<String>, tsmp: Option<chrono::DateTime<Utc>>) -> Result<ical::Event> {
         let mut calevent = ical::Event::new();
         calevent.summary(self.name.as_str());
         if let Some(notes) = self.notes.as_ref() {
-            calevent.description(notes.as_str());
+            calevent.description(notes.description.as_str());
+            for prop in notes.properties.iter() {
+                calevent.add_property(prop.name.to_uppercase().as_str(), prop.data.as_str());
+            }
         }
         if let Some(s) = key {
             calevent.uid(Uuid::new_v3(&Uuid::NAMESPACE_URL, s.as_bytes()).to_string().as_str());
         }
         if let Some(tsmp)=tsmp{
             calevent.timestamp(tsmp);
         }
```

### Comparing `timeblok_py-0.4.5/local_dependencies/timeblok/src/environment.rs` & `timeblok_py-0.5.0/local_dependencies/timeblok/src/environment.rs`

 * *Files identical despite different names*

### Comparing `timeblok_py-0.4.5/local_dependencies/timeblok/src/importer.rs` & `timeblok_py-0.5.0/local_dependencies/timeblok/src/importer.rs`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 use crate::{
     environment::Environment,
     ir::{filter::Filter, Date, ExactDate},
     resolver::resolve_date,
 };
 use chrono::NaiveDate;
 use icalendar::{Calendar, Component};
-use crate::ir::{ExactDateTime, ExactEvent, ExactRange, ExactRecord, ExactTime, ExactTimeRange, Todo};
+use crate::ir::{ExactDateTime, ExactEvent, ExactRange, ExactRecord, ExactTime, ExactTimeRange, Todo, ExactNotes};
 use anyhow::{Result, anyhow};
 use crate::utils::get_dir;
 #[cfg(not(target_family = "wasm"))]
 use crate::utils::download_file;
 
 #[derive(Debug, Clone)]
 pub struct SetFilter {
@@ -116,15 +116,21 @@
                     ExactRange::AllDay(end)
                 }
                 (_, _) => {continue;}
             };
             records.push(ExactRecord::Event(ExactEvent{
                 range,
                 name: event.get_summary().unwrap_or("").to_string(),
-                notes: event.get_description().map(|s| s.to_string())
+                notes: match event.get_description(){
+                    Some(s) => Some(ExactNotes{
+                        description: s.to_string(),
+                        properties: vec![], // TODO: add properties
+                    }),
+                    None => None
+                }
             }))
         }
         if let Some(td) = c.as_todo(){
             records.push(ExactRecord::Todo(Todo{
                 name: td.get_summary().unwrap_or("").to_string(),
                 due: None,
                 status: td.get_status().unwrap_or(icalendar::TodoStatus::NeedsAction),
```

### Comparing `timeblok_py-0.4.5/local_dependencies/timeblok/src/ir/command.rs` & `timeblok_py-0.5.0/local_dependencies/timeblok/src/ir/command.rs`

 * *Files identical despite different names*

### Comparing `timeblok_py-0.4.5/local_dependencies/timeblok/src/ir/displays.rs` & `timeblok_py-0.5.0/local_dependencies/timeblok/src/ir/displays.rs`

 * *Files identical despite different names*

### Comparing `timeblok_py-0.4.5/local_dependencies/timeblok/src/ir/filter.rs` & `timeblok_py-0.5.0/local_dependencies/timeblok/src/ir/filter.rs`

 * *Files identical despite different names*

### Comparing `timeblok_py-0.4.5/local_dependencies/timeblok/src/ir/ident.rs` & `timeblok_py-0.5.0/local_dependencies/timeblok/src/ir/ident.rs`

 * *Files identical despite different names*

### Comparing `timeblok_py-0.4.5/local_dependencies/timeblok/src/ir/mod.rs` & `timeblok_py-0.5.0/local_dependencies/timeblok/src/ir/mod.rs`

 * *Files 6% similar despite different names*

```diff
@@ -130,22 +130,46 @@
 }
 
 // PERFORMANCE: Figure out how to use &str instead of String
 #[derive(Debug)]
 pub struct Event {
     pub range: Range,
     pub name: String,
-    pub notes: Option<String>,
+    pub notes: Option<Notes>,
 }
 
 #[derive(Debug)]
 pub struct ExactEvent {
     pub range: ExactRange,
     pub name: String,
-    pub notes: Option<String>,
+    pub notes: Option<ExactNotes>,
+}
+
+#[derive(Debug, Clone)]
+pub struct Property{
+    pub name: String,
+    pub data: Value
+}
+
+#[derive(Debug, Clone)]
+pub struct ExactProperty{
+    pub name: String,
+    pub data: String
+}
+
+#[derive(Debug, Clone)]
+pub struct Notes{
+    pub description: String,
+    pub properties: Vec<Property> 
+}
+
+#[derive(Debug, Clone)]
+pub struct ExactNotes{
+    pub description: String,
+    pub properties: Vec<ExactProperty> 
 }
 
 #[derive(Debug)]
 pub enum Record {
     Event(Event),
     Occasion(DateTime),
     Note(String),
```

### Comparing `timeblok_py-0.4.5/local_dependencies/timeblok/src/lib.rs` & `timeblok_py-0.5.0/local_dependencies/timeblok/src/lib.rs`

 * *Files identical despite different names*

### Comparing `timeblok_py-0.4.5/local_dependencies/timeblok/src/parser.rs` & `timeblok_py-0.5.0/local_dependencies/timeblok/src/parser.rs`

 * *Files 2% similar despite different names*

```diff
@@ -103,36 +103,54 @@
     let mut pairs = pair.into_inner();
     let command = get_next!(pairs);
     let mut argpairs = get_next!(pairs).into_inner();
     let s = argpairs.as_str();
     let mut args = vec![];
     while argpairs.peek().is_some() {
         let nxt = get_next!(argpairs);
-        let res = match nxt.as_rule() {
-            Rule::FILTER => Value::NumFilter(parse_num_filter(nxt)?),
-            Rule::DATE_FILTER => Value::DateFilter(parse_date_filter(nxt)?),
-            Rule::IDENT => Value::Ident(parse_ident(nxt)?),
-            Rule::NUM_FIELD => Value::Num(parse_numval(nxt)?),
+        match nxt.as_rule() {
             Rule::EOI => {break;}
-            Rule::CARG => Value::String(nxt.as_str().to_string()),
-            Rule::STRING => Value::String(nxt.as_str().to_string()),
-            r => {
-                eprintln!("unexpected rule: {:?}", r);
-                unreachable!()
-            },
-        };
-        args.push(res);
+            _ => {
+                let res = parse_value(nxt)?;
+                args.push(res);
+            }
+        }
     }
     Ok(CommandCall {
         command: command.as_str().to_string(),
         args,
         plain: s.to_string(),
     })
 }
 
+fn parse_property(pair: Pair<Rule>) -> Result<Property> {
+    let mut pairs = pair.into_inner();
+    let name = get_next!(pairs);
+    let value = get_next!(pairs);
+    let data = parse_value(value)?;
+    Ok(Property {
+        name: name.as_str().to_string(),
+        data
+    })
+}
+
+fn parse_value(pair: Pair<Rule>) -> Result<Value> {
+    match pair.as_rule() {
+        Rule::FILTER => Ok(Value::NumFilter(parse_num_filter(pair)?)),
+        Rule::DATE_FILTER => Ok(Value::DateFilter(parse_date_filter(pair)?)),
+        Rule::IDENT => Ok(Value::Ident(parse_ident(pair)?)),
+        Rule::NUM_FIELD => Ok(Value::Num(parse_numval(pair)?)),
+        Rule::CARG | Rule::STRING => Ok(Value::String(pair.as_str().to_string())),
+        r => {
+            eprintln!("unexpected rule: {:?}", r);
+            unreachable!()
+        },
+    }
+}
+
 fn parse_occasion(pair: Pair<Rule>) -> Result<DateTime> {
     let mut pairs = pair.clone().into_inner();
     let pair = get_next!(pairs);
     match pair.as_rule() {
         Rule::DATETIME => {
             let date: Date = parse_date(pair)?;
             let time: Time = get_match!(parse_time, pairs)?;
@@ -209,31 +227,46 @@
     let mut pairs = pair.into_inner();
     let mut event: Event = {
         let raw = get_next!(pairs);
         parse_event_header(raw)?
     };
     if pairs.peek().is_some() {
         // Assuming that all stuff are notes for now...
-        let notes = parse_notes(&mut pairs);
-        let descriptions = notes.join("\n");
-        event.notes = Some(descriptions);
+        let notes = parse_notes(&mut pairs)?;
+        event.notes = Some(notes);
     }
     Ok(event)
 }
 
 fn parse_note(pair: Pair<Rule>) -> &str {
     pair.as_str()
 }
 
-fn parse_notes(pairs: &mut Pairs<Rule>) -> Vec<String> {
-    let mut notes = vec![];
+fn parse_notes(pairs: &mut Pairs<Rule>) -> Result<Notes> {
+    let mut description = String::new();
+    let mut properties = vec![];
     for note in pairs {
-        notes.push(parse_note(note).to_string());
+        match note.as_rule() {
+            Rule::PROPERTY => {
+                properties.push(parse_property(note).unwrap());
+            }
+            Rule::NOTE => {
+                description.push_str(parse_note(note));
+                description.push('\n');
+            }
+            _ => {
+                eprintln!("unexpected rule: {:?}", note.as_rule());
+                unreachable!()
+            }
+        }
     }
-    notes
+    Ok(Notes{
+        description,
+        properties,
+    })
 }
 
 fn parse_event_header(pair: Pair<Rule>) -> Result<Event> {
     let mut pairs = pair.into_inner();
     let timerange = get_match!(parse_timerange, pairs)?;
     let name = get_match!(parse_note, pairs).to_string();
```

### Comparing `timeblok_py-0.4.5/local_dependencies/timeblok/src/preset/mod.rs` & `timeblok_py-0.5.0/local_dependencies/timeblok/src/preset/mod.rs`

 * *Files identical despite different names*

### Comparing `timeblok_py-0.4.5/local_dependencies/timeblok/src/preset/workalendar.rs` & `timeblok_py-0.5.0/local_dependencies/timeblok/src/preset/workalendar.rs`

 * *Files identical despite different names*

### Comparing `timeblok_py-0.4.5/local_dependencies/timeblok/src/resolver.rs` & `timeblok_py-0.5.0/local_dependencies/timeblok/src/resolver.rs`

 * *Files 10% similar despite different names*

```diff
@@ -224,15 +224,47 @@
     Ok(res)
 }
 
 pub fn resolve_event(event: &Event, base: &Environment) -> Result<ExactEvent> {
     Ok(ExactEvent {
         range: resolve_range(&event.range, base)?,
         name: event.name.clone(),
-        notes: event.notes.clone(),
+        notes: match &event.notes{
+            Some(n) => Some(resolve_notes(n, base)?),
+            None => None
+        }
+    })
+}
+
+pub fn resolve_notes(notes: &Notes, base: &Environment) -> Result<ExactNotes> {
+    let mut properties:Vec<ExactProperty> = vec![];
+    for prop in &notes.properties {
+        properties.push(resolve_property(prop, base)?);
+    }
+    Ok(ExactNotes {
+        description: notes.description.clone(),
+        properties
+    })
+}
+
+pub fn resolve_property(property: &Property, base: &Environment) -> Result<ExactProperty> {
+    let data: String = match &property.data {
+        Value::Date(date) => {
+            let date = resolve_date(&date, base)?;
+            // format date into YYYYMMDD
+            format!("{}{:02}{:02}", date.year, date.month, date.day)
+        },
+        Value::Num(Number(n)) => n.to_string(),
+        Value::String(s) => s.to_owned(),
+        Value::Ident(ident) => ident.name.clone(),
+        _ => return Err(anyhow!("Invalid property data type")),
+    };
+    Ok(ExactProperty {
+        name: property.name.clone(),
+        data
     })
 }
 
 pub fn resolve_range(range: &Range, base: &Environment) -> Result<ExactRange> {
     Ok(match range {
         Range::AllDay(date) => {
             let date = resolve_date(date, base)?;
```

### Comparing `timeblok_py-0.4.5/local_dependencies/timeblok/src/tests/snapshots/timeblok__tests__tests__filters.snap` & `timeblok_py-0.5.0/local_dependencies/timeblok/src/tests/snapshots/timeblok__tests__tests__filters.snap`

 * *Files identical despite different names*

### Comparing `timeblok_py-0.4.5/local_dependencies/timeblok/src/tests/snapshots/timeblok__tests__tests__run_tests@filter_dow.tb.snap` & `timeblok_py-0.5.0/local_dependencies/timeblok/src/tests/snapshots/timeblok__tests__tests__run_tests@filter_dow.tb.snap`

 * *Files identical despite different names*

### Comparing `timeblok_py-0.4.5/local_dependencies/timeblok/src/tests/snapshots/timeblok__tests__tests__run_tests@filter_workday.tb.snap` & `timeblok_py-0.5.0/local_dependencies/timeblok/src/tests/snapshots/timeblok__tests__tests__run_tests@filter_workday.tb.snap`

 * *Files identical despite different names*

### Comparing `timeblok_py-0.4.5/local_dependencies/timeblok/src/tests/snapshots/timeblok__tests__tests__run_tests@sanity.tb.snap` & `timeblok_py-0.5.0/local_dependencies/timeblok/src/tests/snapshots/timeblok__tests__tests__run_tests@sanity.tb.snap`

 * *Files identical despite different names*

### Comparing `timeblok_py-0.4.5/local_dependencies/timeblok/src/tests/snapshots/timeblok__tests__tests__run_tests@semester.tb.snap` & `timeblok_py-0.5.0/local_dependencies/timeblok/src/tests/snapshots/timeblok__tests__tests__run_tests@semester.tb.snap`

 * *Files identical despite different names*

### Comparing `timeblok_py-0.4.5/local_dependencies/timeblok/src/tests/snapshots/timeblok__tests__tests__sanity.snap` & `timeblok_py-0.5.0/local_dependencies/timeblok/src/tests/snapshots/timeblok__tests__tests__sanity.snap`

 * *Files identical despite different names*

### Comparing `timeblok_py-0.4.5/local_dependencies/timeblok/src/tests/tests.rs` & `timeblok_py-0.5.0/local_dependencies/timeblok/src/tests/tests.rs`

 * *Files identical despite different names*

### Comparing `timeblok_py-0.4.5/local_dependencies/timeblok/src/utils/mod.rs` & `timeblok_py-0.5.0/local_dependencies/timeblok/src/utils/mod.rs`

 * *Files identical despite different names*

### Comparing `timeblok_py-0.4.5/Cargo.toml` & `timeblok_py-0.5.0/Cargo.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [package]
 name = "timeblok-py"
 publish = false
 
 edition="2021"
 license= "MIT/Apache-2.0"
 repository= "https://github.com/JettChenT/timeblok"
-version= "0.4.5"
+version= "0.5.0"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [lib]
 name = "timeblok_py"
 # "cdylib" is necessary to produce a shared library for Python to import from.
 crate-type = ["cdylib"]
 
 [dependencies]
-timeblok = {path= "local_dependencies/timeblok", package="timeblok", version= "0.4.5" }
+timeblok = {path= "local_dependencies/timeblok", package="timeblok", version= "0.5.0" }
 
 [dependencies.pyo3]
 version = "0.18.0"
 # "abi3-py37" tells pyo3 (and maturin) to build using the stable ABI with minimum Python version 3.7
 features = ["abi3-py37"]
```

### Comparing `timeblok_py-0.4.5/src/lib.rs` & `timeblok_py-0.5.0/src/lib.rs`

 * *Files identical despite different names*

### Comparing `timeblok_py-0.4.5/Cargo.lock` & `timeblok_py-0.5.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1774,15 +1774,15 @@
  "libc",
  "wasi 0.10.0+wasi-snapshot-preview1",
  "winapi",
 ]
 
 [[package]]
 name = "timeblok"
-version = "0.4.5"
+version = "0.5.0"
 dependencies = [
  "anyhow",
  "chrono",
  "chrono-tz",
  "csv",
  "dateparser",
  "directories 4.0.1",
@@ -1802,39 +1802,39 @@
  "wasm-bindgen",
  "wasm-bindgen-futures",
  "web-sys",
 ]
 
 [[package]]
 name = "timeblok-cli"
-version = "0.4.5"
+version = "0.5.0"
 dependencies = [
  "anyhow",
  "chrono",
  "clap",
  "directories 5.0.0",
  "edit",
  "open",
  "timeblok",
 ]
 
 [[package]]
 name = "timeblok-js"
-version = "0.4.5"
+version = "0.5.0"
 dependencies = [
  "console_error_panic_hook",
  "timeblok",
  "wasm-bindgen",
  "wasm-bindgen-test",
  "web-sys",
 ]
 
 [[package]]
 name = "timeblok-py"
-version = "0.4.5"
+version = "0.5.0"
 dependencies = [
  "pyo3",
  "timeblok",
 ]
 
 [[package]]
 name = "tinyvec"
```

