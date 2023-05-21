# Comparing `tmp/nef_pipelines-0.1.40.tar.gz` & `tmp/nef_pipelines-0.1.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nef_pipelines-0.1.40.tar", last modified: Wed May 17 06:37:07 2023, max compression
+gzip compressed data, was "nef_pipelines-0.1.41.tar", last modified: Sun May 21 14:33:58 2023, max compression
```

## Comparing `nef_pipelines-0.1.40.tar` & `nef_pipelines-0.1.41.tar`

### file list

```diff
@@ -1,368 +1,384 @@
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:07.125676 nef_pipelines-0.1.40/
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:05.409539 nef_pipelines-0.1.40/.github/
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:05.523433 nef_pipelines-0.1.40/.github/workflows/
--rw-r--r--   0 garythompson   (501) staff       (20)     4094 2023-02-01 22:03:42.000000 nef_pipelines-0.1.40/.github/workflows/ci.yml
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:05.549041 nef_pipelines-0.1.40/.idea/
--rw-r--r--   0 garythompson   (501) staff       (20)      176 2022-11-25 17:14:12.000000 nef_pipelines-0.1.40/.idea/.gitignore
--rw-r--r--   0 garythompson   (501) staff       (20)       14 2022-11-26 23:48:55.000000 nef_pipelines-0.1.40/.idea/.name
--rw-r--r--   0 garythompson   (501) staff       (20)      299 2023-01-11 23:02:58.000000 nef_pipelines-0.1.40/.idea/NFC.iml
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:05.552897 nef_pipelines-0.1.40/.idea/inspectionProfiles/
--rw-r--r--   0 garythompson   (501) staff       (20)     1184 2023-01-11 23:02:58.000000 nef_pipelines-0.1.40/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 garythompson   (501) staff       (20)      175 2023-01-11 23:02:58.000000 nef_pipelines-0.1.40/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 garythompson   (501) staff       (20)      287 2023-01-11 23:02:58.000000 nef_pipelines-0.1.40/.idea/modules.xml
--rw-r--r--   0 garythompson   (501) staff       (20)      325 2023-04-26 19:24:39.000000 nef_pipelines-0.1.40/.idea/vcs.xml
--rw-r--r--   0 garythompson   (501) staff       (20)     1331 2022-11-26 14:34:37.000000 nef_pipelines-0.1.40/.pre-commit-config.yaml
--rw-r--r--   0 garythompson   (501) staff       (20)      490 2022-11-26 14:33:30.000000 nef_pipelines-0.1.40/.readthedocs.yml
--rw-r--r--   0 garythompson   (501) staff       (20)      372 2023-02-07 22:36:51.000000 nef_pipelines-0.1.40/AUTHORS.md
--rw-r--r--   0 garythompson   (501) staff       (20)     3605 2023-05-17 06:31:52.000000 nef_pipelines-0.1.40/CHANGELOG.md
--rw-r--r--   0 garythompson   (501) staff       (20)    12299 2022-11-27 14:11:11.000000 nef_pipelines-0.1.40/CONTRIBUTING.md
--rw-r--r--   0 garythompson   (501) staff       (20)    24410 2022-11-27 14:11:12.000000 nef_pipelines-0.1.40/LICENSE.txt
--rw-r--r--   0 garythompson   (501) staff       (20)     8765 2023-05-17 06:37:07.126244 nef_pipelines-0.1.40/PKG-INFO
--rw-r--r--   0 garythompson   (501) staff       (20)     8212 2023-02-07 22:28:55.000000 nef_pipelines-0.1.40/README.md
--rw-r--r--   0 garythompson   (501) staff       (20)      826 2023-02-05 15:31:16.000000 nef_pipelines-0.1.40/TODO.md
--rw-r--r--   0 garythompson   (501) staff       (20)      346 2023-01-31 22:56:36.000000 nef_pipelines-0.1.40/pyproject.toml
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:05.565181 nef_pipelines-0.1.40/references/
--rw-r--r--   0 garythompson   (501) staff       (20)    22346 2023-04-16 16:41:23.000000 nef_pipelines-0.1.40/references/Nmr Experiment Nomenclature v2.docx
--rw-r--r--   0 garythompson   (501) staff       (20)   282399 2023-04-16 14:33:43.000000 nef_pipelines-0.1.40/references/fogh.vrankenj.bio.nmr.2006.36.147.pdf
--rw-r--r--   0 garythompson   (501) staff       (20)     1229 2023-04-17 21:03:23.000000 nef_pipelines-0.1.40/release_to_pypi.sh
--rw-r--r--   0 garythompson   (501) staff       (20)      354 2023-04-17 20:13:08.000000 nef_pipelines-0.1.40/requirements.txt
--rw-r--r--   0 garythompson   (501) staff       (20)     1630 2023-05-17 06:37:07.129749 nef_pipelines-0.1.40/setup.cfg
--rw-r--r--   0 garythompson   (501) staff       (20)      710 2022-11-26 14:33:30.000000 nef_pipelines-0.1.40/setup.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:05.413156 nef_pipelines-0.1.40/src/
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:05.605759 nef_pipelines-0.1.40/src/nef_pipelines/
--rw-r--r--   0 garythompson   (501) staff       (20)        6 2023-03-23 08:31:34.000000 nef_pipelines-0.1.40/src/nef_pipelines/VERSION
--rw-r--r--   0 garythompson   (501) staff       (20)      577 2022-11-27 18:49:20.000000 nef_pipelines-0.1.40/src/nef_pipelines/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)       62 2022-11-27 18:48:20.000000 nef_pipelines-0.1.40/src/nef_pipelines/__main__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:05.657222 nef_pipelines-0.1.40/src/nef_pipelines/data/
--rw-r--r--   0 garythompson   (501) staff       (20)  1486198 2023-05-06 14:31:14.000000 nef_pipelines-0.1.40/src/nef_pipelines/data/mmcif_nef_v1_1.dic
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:05.780848 nef_pipelines-0.1.40/src/nef_pipelines/lib/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.40/src/nef_pipelines/lib/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)      124 2023-02-07 22:55:44.000000 nef_pipelines-0.1.40/src/nef_pipelines/lib/constants.py
--rw-r--r--   0 garythompson   (501) staff       (20)     1297 2022-11-27 19:40:25.000000 nef_pipelines-0.1.40/src/nef_pipelines/lib/header_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)      945 2023-03-19 15:38:08.000000 nef_pipelines-0.1.40/src/nef_pipelines/lib/isotope_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2812 2023-04-26 21:04:53.000000 nef_pipelines-0.1.40/src/nef_pipelines/lib/nef_frames_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)    18119 2023-05-07 11:12:00.000000 nef_pipelines-0.1.40/src/nef_pipelines/lib/nef_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)    15051 2023-05-16 20:25:17.000000 nef_pipelines-0.1.40/src/nef_pipelines/lib/peak_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)    21187 2023-04-30 15:31:02.000000 nef_pipelines-0.1.40/src/nef_pipelines/lib/sequence_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)     6348 2023-02-07 21:12:56.000000 nef_pipelines-0.1.40/src/nef_pipelines/lib/shift_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)     6548 2023-04-17 20:48:44.000000 nef_pipelines-0.1.40/src/nef_pipelines/lib/spectra_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)     4109 2023-05-16 09:41:48.000000 nef_pipelines-0.1.40/src/nef_pipelines/lib/structures.py
--rw-r--r--   0 garythompson   (501) staff       (20)    10234 2023-04-26 19:21:33.000000 nef_pipelines-0.1.40/src/nef_pipelines/lib/test_lib.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:05.784179 nef_pipelines-0.1.40/src/nef_pipelines/lib/translation/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.40/src/nef_pipelines/lib/translation/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2160 2023-05-07 09:41:01.000000 nef_pipelines-0.1.40/src/nef_pipelines/lib/translation_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)      292 2022-11-27 18:48:20.000000 nef_pipelines-0.1.40/src/nef_pipelines/lib/typer_utils.py
--rw-r--r--   0 garythompson   (501) staff       (20)    23686 2023-05-16 09:41:30.000000 nef_pipelines-0.1.40/src/nef_pipelines/lib/util.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     5288 2023-05-06 20:58:23.000000 nef_pipelines-0.1.40/src/nef_pipelines/main.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:05.786846 nef_pipelines-0.1.40/src/nef_pipelines/nef_app/
--rw-r--r--   0 garythompson   (501) staff       (20)       49 2022-11-27 18:48:20.000000 nef_pipelines-0.1.40/src/nef_pipelines/nef_app/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:05.808999 nef_pipelines-0.1.40/src/nef_pipelines/tests/
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:05.828754 nef_pipelines-0.1.40/src/nef_pipelines/tests/chains/
--rwxr--r--   0 garythompson   (501) staff       (20)        0 2022-11-25 17:14:10.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/chains/__init__.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     5259 2023-03-18 23:31:39.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/chains/test_clone.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:05.854333 nef_pipelines-0.1.40/src/nef_pipelines/tests/chains/test_data/
--rwxr--r--   0 garythompson   (501) staff       (20)      581 2022-11-25 17:14:10.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/chains/test_data/3aa.nef
--rwxr-xr-x   0 garythompson   (501) staff       (20)      837 2023-03-18 23:31:39.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/chains/test_data/3aa_x3.nef
--rwxr--r--   0 garythompson   (501) staff       (20)     2172 2022-12-16 20:37:04.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/chains/test_data/multi_chain_shifts.nef
--rwxr--r--   0 garythompson   (501) staff       (20)      491 2022-12-16 20:38:38.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/chains/test_list.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)    10032 2023-03-18 23:31:39.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/chains/test_rename.py
--rwxr--r--   0 garythompson   (501) staff       (20)     9304 2023-01-30 23:11:50.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/chains/test_renumber.py
--rw-r--r--   0 garythompson   (501) staff       (20)      709 2023-01-12 09:57:27.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/conftest.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:05.862945 nef_pipelines-0.1.40/src/nef_pipelines/tests/csv/
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:05.874772 nef_pipelines-0.1.40/src/nef_pipelines/tests/csv/test_data/
--rw-r--r--   0 garythompson   (501) staff       (20)       45 2023-01-31 08:50:56.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/csv/test_data/short.csv
--rw-r--r--   0 garythompson   (501) staff       (20)      218 2023-01-31 08:49:14.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/csv/test_data/short_complete.csv
--rw-r--r--   0 garythompson   (501) staff       (20)     5079 2023-01-31 22:17:03.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/csv/test_import_rdcs.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:05.881255 nef_pipelines-0.1.40/src/nef_pipelines/tests/echidna/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-05-04 20:35:04.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/echidna/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:05.891361 nef_pipelines-0.1.40/src/nef_pipelines/tests/echidna/test_data/
--rw-r--r--   0 garythompson   (501) staff       (20)      695 2023-05-06 14:02:40.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/echidna/test_data/echidna_peaks.txt
--rw-r--r--   0 garythompson   (501) staff       (20)     1775 2023-05-06 14:16:20.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/echidna/test_data/echidna_sequence.nef
--rw-r--r--   0 garythompson   (501) staff       (20)     3610 2023-05-06 20:59:13.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/echidna/test_import_peaks.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:05.897012 nef_pipelines-0.1.40/src/nef_pipelines/tests/fasta/
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:05.906922 nef_pipelines-0.1.40/src/nef_pipelines/tests/fasta/test_data/
--rwxr--r--   0 garythompson   (501) staff       (20)       11 2022-12-06 19:49:15.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/fasta/test_data/3aa.fasta
--rwxr-xr-x   0 garythompson   (501) staff       (20)       24 2023-03-18 23:31:39.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/fasta/test_data/3aa_x2.fasta
--rwxr-xr-x   0 garythompson   (501) staff       (20)     3178 2023-03-18 23:31:39.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/fasta/test_sequence.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:05.937317 nef_pipelines-0.1.40/src/nef_pipelines/tests/frames/
--rwxr--r--   0 garythompson   (501) staff       (20)        0 2022-12-06 20:53:09.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/frames/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:05.957059 nef_pipelines-0.1.40/src/nef_pipelines/tests/frames/test_data/
--rwxr-xr-x   0 garythompson   (501) staff       (20)     1470 2023-03-18 23:31:39.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/frames/test_data/frames.nef
--rwxr--r--   0 garythompson   (501) staff       (20)     1626 2022-12-16 21:06:02.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/frames/test_data/pales_test_1.nef
--rwxr--r--   0 garythompson   (501) staff       (20)     2690 2022-12-16 21:06:48.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/frames/test_delete.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     1884 2023-05-16 09:49:59.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/frames/test_list.py
--rwxr--r--   0 garythompson   (501) staff       (20)    10090 2023-04-15 16:15:29.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/frames/test_rename.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     1312 2023-03-18 23:31:39.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/frames/test_tabulate.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:05.969559 nef_pipelines-0.1.40/src/nef_pipelines/tests/mars/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-05 13:08:51.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/mars/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:05.981704 nef_pipelines-0.1.40/src/nef_pipelines/tests/mars/test_data/
--rw-r--r--   0 garythompson   (501) staff       (20)     9631 2023-02-01 22:03:42.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/mars/test_data/sec5_short.neff
--rw-r--r--   0 garythompson   (501) staff       (20)      311 2023-02-05 15:30:43.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/mars/test_data/sec5_short.txt
--rw-r--r--   0 garythompson   (501) staff       (20)      838 2023-02-01 22:29:59.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/mars/test_export_shifts.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2537 2023-02-05 15:30:44.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/mars/test_import_shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:06.007147 nef_pipelines-0.1.40/src/nef_pipelines/tests/nmrpipe/
--rwxr--r--   0 garythompson   (501) staff       (20)        0 2022-12-10 21:27:09.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/nmrpipe/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:06.087216 nef_pipelines-0.1.40/src/nef_pipelines/tests/nmrpipe/test_data/
--rwxr-xr-x   0 garythompson   (501) staff       (20)       12 2023-03-18 23:31:39.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/nmrpipe/test_data/3aa.seq
--rwxr--r--   0 garythompson   (501) staff       (20)       18 2022-12-16 20:31:09.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/nmrpipe/test_data/3aa.tab
--rwxr-xr-x   0 garythompson   (501) staff       (20)       15 2023-03-18 23:31:39.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/nmrpipe/test_data/3aa10.seq
--rwxr--r--   0 garythompson   (501) staff       (20)       16 2022-12-16 20:31:09.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/nmrpipe/test_data/4peaks.seq
--rw-------   0 garythompson   (501) staff       (20)      455 2023-01-10 13:25:00.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/nmrpipe/test_data/P3a_l273R_nmrpipe_shifts_short.tab
--rwxr--r--   0 garythompson   (501) staff       (20)    10961 2022-12-16 20:31:08.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/nmrpipe/test_data/gb3.tab
--rwxr--r--   0 garythompson   (501) staff       (20)    11038 2022-12-16 20:31:08.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned.tab
--rwxr-xr-x   0 garythompson   (501) staff       (20)      943 2023-03-18 23:31:39.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc.tab
--rwxr-xr-x   0 garythompson   (501) staff       (20)     1878 2023-03-18 23:31:39.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc_expected.tab
--rwxr--r--   0 garythompson   (501) staff       (20)    26327 2022-12-16 20:31:09.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/nmrpipe/test_data/ns3_S135A_BMRB1.txt
--rwxr--r--   0 garythompson   (501) staff       (20)      247 2022-12-16 20:31:09.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/nmrpipe/test_data/ns3_S135A_BMRB1_short.txt
--rwxr-xr-x   0 garythompson   (501) staff       (20)      800 2023-03-18 23:31:39.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/nmrpipe/test_data/test_header_entry.txt
--rwxr-xr-x   0 garythompson   (501) staff       (20)    14392 2023-04-24 21:03:24.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/nmrpipe/test_gdb.py
--rwxr--r--   0 garythompson   (501) staff       (20)      840 2022-12-16 20:35:58.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/nmrpipe/test_peaks.py
--rwxr--r--   0 garythompson   (501) staff       (20)      486 2022-12-16 20:35:58.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/nmrpipe/test_pipe_lib.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     4158 2023-03-18 23:31:39.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/nmrpipe/test_sequence.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     4454 2023-01-18 07:36:14.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/nmrpipe/test_shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:06.120987 nef_pipelines-0.1.40/src/nef_pipelines/tests/nmrview/
--rwxr--r--   0 garythompson   (501) staff       (20)        0 2022-12-11 15:04:32.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/nmrview/__init__.py
--rwxr--r--   0 garythompson   (501) staff       (20)    10752 2022-12-17 11:29:00.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/nmrview/tcl_diag.html
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:06.204990 nef_pipelines-0.1.40/src/nef_pipelines/tests/nmrview/test_data/
--rwxr--r--   0 garythompson   (501) staff       (20)       12 2022-12-11 15:04:32.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/nmrview/test_data/3aa.seq
--rwxr--r--   0 garythompson   (501) staff       (20)       15 2022-12-11 15:04:32.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/nmrview/test_data/3aa10.seq
--rwxr--r--   0 garythompson   (501) staff       (20)       16 2022-12-17 11:29:00.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/nmrview/test_data/4peaks.seq
--rwxr-xr-x   0 garythompson   (501) staff       (20)      980 2023-03-18 23:31:39.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/nmrview/test_data/4peaks.xpk
--rwxr--r--   0 garythompson   (501) staff       (20)      880 2022-12-11 15:04:32.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/nmrview/test_data/expected_nmr_view.xpk
--rwxr-xr-x   0 garythompson   (501) staff       (20)     2178 2023-03-18 23:31:39.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/nmrview/test_data/expected_sequence_and_peaks_nmrview.txt
--rwxr--r--   0 garythompson   (501) staff       (20)      319 2022-12-11 15:04:32.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/nmrview/test_data/joe_clic.xpk
--rwxr--r--   0 garythompson   (501) staff       (20)     2172 2022-12-11 15:04:32.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/nmrview/test_data/nmrview_expected_4aa.txt
--rwxr--r--   0 garythompson   (501) staff       (20)    29631 2022-12-11 15:04:32.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/nmrview/test_data/ppm.out
--rwxr--r--   0 garythompson   (501) staff       (20)      540 2022-12-11 15:04:32.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/nmrview/test_data/ppm_out.seq
--rwxr--r--   0 garythompson   (501) staff       (20)       12 2022-12-11 15:04:32.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/nmrview/test_data/ppm_out_short.seq
--rwxr--r--   0 garythompson   (501) staff       (20)      126 2022-12-11 15:04:32.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/nmrview/test_data/ppm_short.out
--rwxr--r--   0 garythompson   (501) staff       (20)      522 2022-12-17 11:29:00.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/nmrview/test_data/ppm_short_seq.nef
--rwxr--r--   0 garythompson   (501) staff       (20)      800 2022-12-11 15:05:20.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/nmrview/test_data/test_header_entry.txt
--rwxr-xr-x   0 garythompson   (501) staff       (20)     2646 2023-03-18 23:31:39.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/nmrview/test_export_peaks.py
--rwxr--r--   0 garythompson   (501) staff       (20)     3343 2023-01-14 17:44:39.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/nmrview/test_export_sequences.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     3872 2023-02-15 22:22:17.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/nmrview/test_import_peaks.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     3915 2023-02-07 23:04:20.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/nmrview/test_import_sequence.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     4734 2023-01-18 07:36:14.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/nmrview/test_import_shifts.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     2166 2023-03-18 23:31:39.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/nmrview/test_tcl.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:06.225538 nef_pipelines-0.1.40/src/nef_pipelines/tests/pales/
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:06.242899 nef_pipelines-0.1.40/src/nef_pipelines/tests/pales/test_data/
--rwxr--r--   0 garythompson   (501) staff       (20)     1626 2022-12-17 16:34:00.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/pales/test_data/pales_test_1.nef
--rwxr--r--   0 garythompson   (501) staff       (20)     1627 2022-12-17 16:34:00.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/pales/test_data/pales_test_2.nef
--rwxr--r--   0 garythompson   (501) staff       (20)     1647 2023-01-27 21:30:12.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/pales/test_data/pales_test_segids.nef
--rwxr-xr-x   0 garythompson   (501) staff       (20)     2773 2023-01-30 23:21:17.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/pales/test_rdcs.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     2043 2023-03-18 23:31:39.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/pales/test_template.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:06.249128 nef_pipelines-0.1.40/src/nef_pipelines/tests/pdbx/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-01-31 19:44:59.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/pdbx/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:06.285930 nef_pipelines-0.1.40/src/nef_pipelines/tests/pdbx/test_data/
--rwxr-xr-x   0 garythompson   (501) staff       (20)     4795 2023-03-18 23:31:39.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/pdbx/test_data/3a_ab.pdb
--rwxr--r--   0 garythompson   (501) staff       (20)     4795 2022-12-17 16:52:18.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/pdbx/test_data/3a_cccc_dddd.pdb
--rwxr--r--   0 garythompson   (501) staff       (20)     4195 2022-12-17 16:52:18.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/pdbx/test_data/3a_no_chain_no_segid.pdb
--rwxr--r--   0 garythompson   (501) staff       (20)     2395 2022-12-17 16:52:18.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/pdbx/test_data/3aa.pdb
--rwxr--r--   0 garythompson   (501) staff       (20)     2254 2022-12-17 16:52:18.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/pdbx/test_data/3aa11_13.pdb
--rwxr--r--   0 garythompson   (501) staff       (20)      800 2022-12-10 20:00:10.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/pdbx/test_data/test_header_entry.txt
--rwxr-xr-x   0 garythompson   (501) staff       (20)     4248 2023-01-15 11:02:28.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/pdbx/test_sequence.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:06.294735 nef_pipelines-0.1.40/src/nef_pipelines/tests/shifts/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-04-16 09:07:56.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/shifts/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     8438 2023-04-17 20:44:38.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/shifts/test_make_peaks.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:06.299725 nef_pipelines-0.1.40/src/nef_pipelines/tests/shifty/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-09 08:07:44.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/shifty/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)      773 2023-02-09 08:08:24.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/shifty/test_export_shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:06.330963 nef_pipelines-0.1.40/src/nef_pipelines/tests/sparky/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-04-26 18:29:03.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/sparky/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:06.418330 nef_pipelines-0.1.40/src/nef_pipelines/tests/sparky/test_data/
--rw-r--r--   0 garythompson   (501) staff       (20)     1393 2023-01-31 21:17:52.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/sparky/test_data/P3a_L273R_sequence_short.neff
--rw-r--r--   0 garythompson   (501) staff       (20)     2342 2023-03-19 00:02:41.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/sparky/test_data/peaks_short_with_assignments.neff
--rw-r--r--   0 garythompson   (501) staff       (20)       40 2023-04-26 18:38:57.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/sparky/test_data/sparky_basic_sequence_dna.txt
--rw-r--r--   0 garythompson   (501) staff       (20)        9 2023-04-26 18:38:57.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/sparky/test_data/sparky_basic_sequence_protein.txt
--rw-r--r--   0 garythompson   (501) staff       (20)      241 2023-04-26 21:06:34.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/sparky/test_data/sparky_manual_basic.peaks
--rw-r--r--   0 garythompson   (501) staff       (20)     1187 2023-04-26 18:24:37.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/sparky/test_data/sparky_manual_basic_sequence.nef
--rw-r--r--   0 garythompson   (501) staff       (20)      359 2023-04-26 19:32:49.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/sparky/test_data/sparky_manual_full.peaks
--rw-r--r--   0 garythompson   (501) staff       (20)      422 2023-04-26 20:35:49.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/sparky/test_data/sparky_manual_full_comment.peaks
--rw-r--r--   0 garythompson   (501) staff       (20)      354 2023-05-04 18:45:19.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/sparky/test_data/sparky_manual_full_no_sequence.peaks
--rw-r--r--   0 garythompson   (501) staff       (20)     1718 2023-01-17 09:55:08.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/sparky/test_data/test_shifts_P3a_L273R_shifts_short.txt
--rw-r--r--   0 garythompson   (501) staff       (20)     2342 2023-03-19 00:02:41.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short.neff
--rw-r--r--   0 garythompson   (501) staff       (20)     2157 2023-03-19 00:02:41.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_chains.neff
--rw-r--r--   0 garythompson   (501) staff       (20)     2156 2023-03-19 00:02:41.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_different_residues.neff
--rw-r--r--   0 garythompson   (501) staff       (20)     2803 2023-03-19 00:02:41.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_i_minus_one.neff
--rw-r--r--   0 garythompson   (501) staff       (20)     2326 2023-03-19 00:02:41.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_overlapping_chains.neff
--rw-r--r--   0 garythompson   (501) staff       (20)    12427 2023-03-24 20:06:24.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/sparky/test_export_peaks.py
--rw-r--r--   0 garythompson   (501) staff       (20)     4153 2023-05-04 20:25:28.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/sparky/test_import_peaks.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2475 2023-04-26 18:38:58.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/sparky/test_import_sequence.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2661 2023-01-17 17:17:45.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/sparky/test_import_shifts.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2322 2023-05-16 09:41:29.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/sparky/test_sparky_lib.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:06.497843 nef_pipelines-0.1.40/src/nef_pipelines/tests/test_data/
--rw-r--r--   0 garythompson   (501) staff       (20)      658 2023-01-11 15:13:08.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/test_data/3a_ab.neff
--rw-r--r--   0 garythompson   (501) staff       (20)       11 2023-04-15 14:38:14.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/test_data/empty.nef
--rw-r--r--   0 garythompson   (501) staff       (20)      837 2022-12-15 21:03:33.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/test_data/header.nef
--rwxr-xr-x   0 garythompson   (501) staff       (20)      908 2023-03-18 23:31:39.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/test_data/multi_chain.nef
--rwxr-xr-x   0 garythompson   (501) staff       (20)     2979 2023-03-18 23:31:39.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/test_data/nef_3_peaks.nef
--rwxr--r--   0 garythompson   (501) staff       (20)      979 2023-01-18 17:43:15.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/test_data/tailin_seq_short.nef
--rw-r--r--   0 garythompson   (501) staff       (20)     2958 2023-02-07 21:50:52.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/test_data/test_agv.neff
--rwxr-xr-x   0 garythompson   (501) staff       (20)    64721 2023-04-16 09:21:50.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/test_data/ubiquitin_short.nef
--rw-r--r--   0 garythompson   (501) staff       (20)     1884 2023-02-07 23:05:23.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/test_header.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     9456 2023-03-18 23:11:48.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/test_nef_lib.py
--rwxr-xr-x   0 garythompson   (501) staff       (20)     7641 2023-04-24 20:39:10.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/test_sequence_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2750 2022-12-14 20:48:12.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/test_test.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:06.511084 nef_pipelines-0.1.40/src/nef_pipelines/tests/xcamshift/
--rw-r--r--   0 garythompson   (501) staff       (20)     1860 2023-02-07 22:05:04.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/xcamshift/test_export_shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:06.567916 nef_pipelines-0.1.40/src/nef_pipelines/tests/xplor/
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:06.653986 nef_pipelines-0.1.40/src/nef_pipelines/tests/xplor/test_data/
--rw-r--r--   0 garythompson   (501) staff       (20)    10948 2022-12-22 19:24:27.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/xplor/test_data/3a_ab.psf
--rw-r--r--   0 garythompson   (501) staff       (20)     2700 2023-01-31 09:42:10.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/xplor/test_data/3a_ab_rdcs.neff
--rw-r--r--   0 garythompson   (501) staff       (20)      417 2022-12-22 19:24:27.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/xplor/test_data/bad_field_count.psf
--rw-r--r--   0 garythompson   (501) staff       (20)        7 2022-12-22 19:24:28.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/xplor/test_data/bad_header.psf
--rw-r--r--   0 garythompson   (501) staff       (20)      434 2022-12-22 19:24:27.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/xplor/test_data/bad_natom.psf
--rw-r--r--   0 garythompson   (501) staff       (20)      429 2022-12-22 19:24:27.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/xplor/test_data/bad_residue_number.psf
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-12-21 15:10:23.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/xplor/test_data/empty.psf
--rw-r--r--   0 garythompson   (501) staff       (20)      216 2022-12-22 19:24:28.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/xplor/test_data/no_residues_found.psf
--rw-r--r--   0 garythompson   (501) staff       (20)      623 2023-01-04 12:41:40.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals.tbl
--rw-r--r--   0 garythompson   (501) staff       (20)      580 2023-01-11 14:25:21.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals_bad.tbl
--rw-r--r--   0 garythompson   (501) staff       (20)      503 2023-01-11 14:57:02.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals_no_segids.tbl
--rw-r--r--   0 garythompson   (501) staff       (20)      197 2023-01-11 22:37:32.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/xplor/test_data/test_2_distances.tbl
--rw-r--r--   0 garythompson   (501) staff       (20)      159 2023-01-11 22:37:32.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/xplor/test_data/test_2_distances_bad.tbl
--rw-r--r--   0 garythompson   (501) staff       (20)      137 2023-01-11 22:37:32.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/xplor/test_data/test_2_distances_no_segids.tbl
--rw-r--r--   0 garythompson   (501) staff       (20)      186 2023-01-04 11:17:43.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/xplor/test_data/test_2_noes.tbl
--rw-r--r--   0 garythompson   (501) staff       (20)     8093 2023-01-15 11:02:28.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/xplor/test_dihedrals.py
--rw-r--r--   0 garythompson   (501) staff       (20)     6535 2023-01-15 10:58:38.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/xplor/test_distances.py
--rw-r--r--   0 garythompson   (501) staff       (20)     1974 2023-01-31 09:53:27.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/xplor/test_export_rdcs.py
--rw-r--r--   0 garythompson   (501) staff       (20)     1487 2023-01-04 12:32:55.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/xplor/test_import_sequence.py
--rw-r--r--   0 garythompson   (501) staff       (20)     3413 2022-12-22 19:24:29.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/xplor/test_psf_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)    11065 2023-01-11 21:19:43.000000 nef_pipelines-0.1.40/src/nef_pipelines/tests/xplor/test_xplor_lib.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:06.684049 nef_pipelines-0.1.40/src/nef_pipelines/tools/
--rw-r--r--   0 garythompson   (501) staff       (20)     2268 2023-04-02 20:29:58.000000 nef_pipelines-0.1.40/src/nef_pipelines/tools/about.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:06.706188 nef_pipelines-0.1.40/src/nef_pipelines/tools/chains/
--rw-r--r--   0 garythompson   (501) staff       (20)      527 2023-01-02 20:41:38.000000 nef_pipelines-0.1.40/src/nef_pipelines/tools/chains/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2593 2023-04-23 18:00:54.000000 nef_pipelines-0.1.40/src/nef_pipelines/tools/chains/clone.py
--rw-r--r--   0 garythompson   (501) staff       (20)     1417 2023-03-21 20:24:03.000000 nef_pipelines-0.1.40/src/nef_pipelines/tools/chains/list.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2670 2023-03-18 23:07:53.000000 nef_pipelines-0.1.40/src/nef_pipelines/tools/chains/rename.py
--rw-r--r--   0 garythompson   (501) staff       (20)     9203 2023-01-10 10:15:33.000000 nef_pipelines-0.1.40/src/nef_pipelines/tools/chains/renumber.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:06.714227 nef_pipelines-0.1.40/src/nef_pipelines/tools/entry/
--rw-r--r--   0 garythompson   (501) staff       (20)      376 2022-11-29 12:15:24.000000 nef_pipelines-0.1.40/src/nef_pipelines/tools/entry/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)      692 2023-02-07 13:11:22.000000 nef_pipelines-0.1.40/src/nef_pipelines/tools/entry/rename.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:06.763037 nef_pipelines-0.1.40/src/nef_pipelines/tools/frames/
--rw-r--r--   0 garythompson   (501) staff       (20)      639 2023-04-15 16:14:41.000000 nef_pipelines-0.1.40/src/nef_pipelines/tools/frames/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2556 2023-03-19 00:07:20.000000 nef_pipelines-0.1.40/src/nef_pipelines/tools/frames/delete.py
--rw-r--r--   0 garythompson   (501) staff       (20)     4111 2023-03-21 19:38:23.000000 nef_pipelines-0.1.40/src/nef_pipelines/tools/frames/insert.py
--rw-r--r--   0 garythompson   (501) staff       (20)     7414 2023-05-16 09:49:59.000000 nef_pipelines-0.1.40/src/nef_pipelines/tools/frames/list.py
--rw-r--r--   0 garythompson   (501) staff       (20)     6711 2023-04-17 20:20:20.000000 nef_pipelines-0.1.40/src/nef_pipelines/tools/frames/rename.py
--rw-r--r--   0 garythompson   (501) staff       (20)     8952 2023-03-21 20:29:06.000000 nef_pipelines-0.1.40/src/nef_pipelines/tools/frames/tabulate.py
--rw-r--r--   0 garythompson   (501) staff       (20)      871 2023-02-07 23:05:12.000000 nef_pipelines-0.1.40/src/nef_pipelines/tools/header.py
--rw-r--r--   0 garythompson   (501) staff       (20)     5132 2022-11-27 18:48:20.000000 nef_pipelines-0.1.40/src/nef_pipelines/tools/offset_shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:06.767720 nef_pipelines-0.1.40/src/nef_pipelines/tools/peaks/
--rw-r--r--   0 garythompson   (501) staff       (20)    10891 2023-03-23 08:18:29.000000 nef_pipelines-0.1.40/src/nef_pipelines/tools/peaks/match.py
--rw-r--r--   0 garythompson   (501) staff       (20)    10539 2022-12-22 18:47:15.000000 nef_pipelines-0.1.40/src/nef_pipelines/tools/res_assign.py_unused
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:06.776624 nef_pipelines-0.1.40/src/nef_pipelines/tools/shifts/
--rw-r--r--   0 garythompson   (501) staff       (20)      372 2023-03-20 08:59:26.000000 nef_pipelines-0.1.40/src/nef_pipelines/tools/shifts/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     7145 2023-05-16 20:28:28.000000 nef_pipelines-0.1.40/src/nef_pipelines/tools/shifts/make_peaks.py
--rw-r--r--   0 garythompson   (501) staff       (20)      200 2022-11-28 23:58:46.000000 nef_pipelines-0.1.40/src/nef_pipelines/tools/sink.py
--rw-r--r--   0 garythompson   (501) staff       (20)      445 2022-11-28 21:57:18.000000 nef_pipelines-0.1.40/src/nef_pipelines/tools/stream.py
--rw-r--r--   0 garythompson   (501) staff       (20)     3753 2023-04-17 20:08:48.000000 nef_pipelines-0.1.40/src/nef_pipelines/tools/test.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:06.778773 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:06.780756 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/csv/
--rw-r--r--   0 garythompson   (501) staff       (20)      409 2023-03-19 00:07:20.000000 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/csv/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:06.790912 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/csv/importers/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-01-18 16:41:09.000000 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/csv/importers/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)    14955 2023-01-31 09:30:29.000000 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/csv/importers/rdcs.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:06.795483 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/echidna/
--rw-r--r--   0 garythompson   (501) staff       (20)      465 2023-05-04 20:35:04.000000 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/echidna/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:06.802917 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/echidna/importers/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-05-04 20:35:04.000000 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/echidna/importers/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)    15316 2023-05-07 11:13:51.000000 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/echidna/importers/peaks.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:06.808573 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/fasta/
--rw-r--r--   0 garythompson   (501) staff       (20)      646 2022-11-27 19:51:40.000000 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/fasta/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:06.812697 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/fasta/exporters/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/fasta/exporters/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     3952 2023-03-22 17:47:24.000000 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/fasta/exporters/sequence.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:06.817176 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/fasta/importers/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/fasta/importers/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     5532 2023-04-24 20:34:49.000000 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/fasta/importers/sequence.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:06.828151 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/mars/
--rw-r--r--   0 garythompson   (501) staff       (20)      946 2023-02-15 11:20:25.000000 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/mars/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:06.849029 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/mars/exporters/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/mars/exporters/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     6571 2023-02-15 21:49:23.000000 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/mars/exporters/fragments.py
--rw-r--r--   0 garythompson   (501) staff       (20)     4299 2023-02-15 22:21:34.000000 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/mars/exporters/input.py
--rw-r--r--   0 garythompson   (501) staff       (20)      780 2022-11-28 23:56:55.000000 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/mars/exporters/sequence.py
--rw-r--r--   0 garythompson   (501) staff       (20)     6001 2023-03-11 19:52:09.000000 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/mars/exporters/shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:06.855979 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/mars/importers/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-05 10:22:38.000000 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/mars/importers/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)    11657 2023-04-24 20:38:57.000000 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/mars/importers/shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:06.923958 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/nmrpipe/
--rw-r--r--   0 garythompson   (501) staff       (20)      679 2022-11-27 19:52:05.000000 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/nmrpipe/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:06.938130 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/nmrpipe/importers/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/nmrpipe/importers/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2414 2022-12-13 19:17:42.000000 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/nmrpipe/importers/peaks.py
--rw-r--r--   0 garythompson   (501) staff       (20)     3498 2023-04-24 20:38:57.000000 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/nmrpipe/importers/sequence.py
--rw-r--r--   0 garythompson   (501) staff       (20)     3151 2023-04-24 20:36:47.000000 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/nmrpipe/importers/shifts.py
--rw-r--r--   0 garythompson   (501) staff       (20)    20224 2023-04-24 21:17:19.000000 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/nmrpipe/nmrpipe_lib.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:06.946724 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/nmrview/
--rw-r--r--   0 garythompson   (501) staff       (20)     1056 2023-01-16 22:48:48.000000 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/nmrview/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:06.968415 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/nmrview/exporters/
--rw-r--r--   0 garythompson   (501) staff       (20)    13841 2023-02-07 13:14:10.000000 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/nmrview/exporters/peaks.py
--rw-r--r--   0 garythompson   (501) staff       (20)     7053 2023-01-30 07:39:27.000000 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/nmrview/exporters/sequences.py
--rw-r--r--   0 garythompson   (501) staff       (20)     9136 2023-01-16 22:47:55.000000 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/nmrview/exporters/shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:06.984707 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/nmrview/importers/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/nmrview/importers/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)    17212 2022-12-22 18:41:48.000000 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/nmrview/importers/peaks.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2330 2023-04-24 20:38:58.000000 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/nmrview/importers/sequence.py
--rw-r--r--   0 garythompson   (501) staff       (20)     5787 2023-04-24 20:38:58.000000 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/nmrview/importers/shifts.py
--rw-r--r--   0 garythompson   (501) staff       (20)     8866 2023-01-16 22:43:21.000000 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/nmrview/nmrview_lib.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:06.987764 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/pales/
--rw-r--r--   0 garythompson   (501) staff       (20)      660 2022-11-27 19:52:13.000000 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/pales/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:06.994628 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/pales/exporters/
--rw-r--r--   0 garythompson   (501) staff       (20)    10943 2023-05-07 09:41:03.000000 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/pales/exporters/rdcs.py
--rw-r--r--   0 garythompson   (501) staff       (20)     4817 2023-03-06 22:17:20.000000 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/pales/exporters/template.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:06.997769 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/pdbx/
--rw-r--r--   0 garythompson   (501) staff       (20)      454 2022-12-17 16:50:37.000000 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/pdbx/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:07.001005 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/pdbx/importers/
--rw-r--r--   0 garythompson   (501) staff       (20)     4655 2022-12-17 16:51:05.000000 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/pdbx/importers/sequence.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:07.006703 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/rpf/
--rw-r--r--   0 garythompson   (501) staff       (20)      608 2023-03-23 08:19:19.000000 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/rpf/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:07.021111 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/rpf/exporters/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-03-22 21:34:49.000000 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/rpf/exporters/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)    11873 2023-03-22 22:37:50.000000 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/rpf/exporters/shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:07.026145 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/shifty/
--rw-r--r--   0 garythompson   (501) staff       (20)      523 2023-02-08 16:38:07.000000 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/shifty/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:07.030978 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/shifty/exporters/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-05 22:19:02.000000 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/shifty/exporters/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     6339 2023-04-24 20:32:00.000000 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/shifty/exporters/shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:07.038830 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/sparky/
--rw-r--r--   0 garythompson   (501) staff       (20)      804 2023-04-26 18:38:57.000000 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/sparky/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:07.044873 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/sparky/exporters/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-03-18 23:36:58.000000 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/sparky/exporters/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)    15804 2023-05-04 07:46:41.000000 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/sparky/exporters/peaks.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:07.072119 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/sparky/importers/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-01-16 13:30:23.000000 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/sparky/importers/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)    16125 2023-05-07 09:39:01.000000 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/sparky/importers/peaks.py
--rw-r--r--   0 garythompson   (501) staff       (20)     6463 2023-04-26 18:39:25.000000 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/sparky/importers/sequence.py
--rw-r--r--   0 garythompson   (501) staff       (20)     8953 2023-03-19 00:07:20.000000 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/sparky/importers/shifts.py
--rw-r--r--   0 garythompson   (501) staff       (20)     8328 2023-05-15 12:35:13.000000 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/sparky/sparky_lib.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:07.077150 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/xcamshift/
--rw-r--r--   0 garythompson   (501) staff       (20)      554 2023-02-07 22:05:04.000000 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/xcamshift/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:07.080896 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/xcamshift/exporters/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-05 22:19:02.000000 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/xcamshift/exporters/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     3787 2023-02-07 22:05:13.000000 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/xcamshift/exporters/shifts.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:07.085243 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/xeasy/
--rw-r--r--   0 garythompson   (501) staff       (20)    18357 2023-05-16 09:57:46.000000 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/xeasy/xeasy_lib.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:07.096649 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/xplor/
--rw-r--r--   0 garythompson   (501) staff       (20)      933 2023-02-05 22:57:14.000000 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/xplor/__init__.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:07.110625 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/xplor/exporters/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-01-20 20:08:15.000000 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/xplor/exporters/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     7167 2023-01-31 09:54:44.000000 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/xplor/exporters/rdcs.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:07.122662 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/xplor/importers/
--rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-12-17 17:33:41.000000 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/xplor/importers/__init__.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2834 2023-03-24 21:54:07.000000 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/xplor/importers/dihedrals.py
--rw-r--r--   0 garythompson   (501) staff       (20)     2888 2023-01-11 22:37:57.000000 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/xplor/importers/distances.py
--rw-r--r--   0 garythompson   (501) staff       (20)     3298 2023-01-04 12:32:55.000000 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/xplor/importers/sequence.py
--rw-r--r--   0 garythompson   (501) staff       (20)     3663 2022-12-22 19:24:58.000000 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/xplor/psf_lib.py
--rw-r--r--   0 garythompson   (501) staff       (20)    38877 2023-01-11 22:37:34.000000 nef_pipelines-0.1.40/src/nef_pipelines/transcoders/xplor/xplor_lib.py
-drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-17 06:37:05.626089 nef_pipelines-0.1.40/src/nef_pipelines.egg-info/
--rw-r--r--   0 garythompson   (501) staff       (20)     8765 2023-05-17 06:37:05.000000 nef_pipelines-0.1.40/src/nef_pipelines.egg-info/PKG-INFO
--rw-r--r--   0 garythompson   (501) staff       (20)    13977 2023-05-17 06:37:05.000000 nef_pipelines-0.1.40/src/nef_pipelines.egg-info/SOURCES.txt
--rw-r--r--   0 garythompson   (501) staff       (20)        1 2023-05-17 06:37:05.000000 nef_pipelines-0.1.40/src/nef_pipelines.egg-info/dependency_links.txt
--rw-r--r--   0 garythompson   (501) staff       (20)       48 2023-05-17 06:37:05.000000 nef_pipelines-0.1.40/src/nef_pipelines.egg-info/entry_points.txt
--rw-r--r--   0 garythompson   (501) staff       (20)        1 2022-11-27 19:48:54.000000 nef_pipelines-0.1.40/src/nef_pipelines.egg-info/not-zip-safe
--rw-r--r--   0 garythompson   (501) staff       (20)      363 2023-05-17 06:37:05.000000 nef_pipelines-0.1.40/src/nef_pipelines.egg-info/requires.txt
--rw-r--r--   0 garythompson   (501) staff       (20)       14 2023-05-17 06:37:05.000000 nef_pipelines-0.1.40/src/nef_pipelines.egg-info/top_level.txt
--rw-r--r--   0 garythompson   (501) staff       (20)     3032 2023-02-01 22:03:42.000000 nef_pipelines-0.1.40/tox.ini
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.517225 nef_pipelines-0.1.41/
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:57.194884 nef_pipelines-0.1.41/.github/
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:57.346278 nef_pipelines-0.1.41/.github/workflows/
+-rw-r--r--   0 garythompson   (501) staff       (20)     4094 2023-02-01 22:03:42.000000 nef_pipelines-0.1.41/.github/workflows/ci.yml
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:57.371524 nef_pipelines-0.1.41/.idea/
+-rw-r--r--   0 garythompson   (501) staff       (20)      176 2022-11-25 17:14:12.000000 nef_pipelines-0.1.41/.idea/.gitignore
+-rw-r--r--   0 garythompson   (501) staff       (20)       14 2022-11-26 23:48:55.000000 nef_pipelines-0.1.41/.idea/.name
+-rw-r--r--   0 garythompson   (501) staff       (20)      299 2023-01-11 23:02:58.000000 nef_pipelines-0.1.41/.idea/NFC.iml
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:57.378198 nef_pipelines-0.1.41/.idea/inspectionProfiles/
+-rw-r--r--   0 garythompson   (501) staff       (20)     1184 2023-01-11 23:02:58.000000 nef_pipelines-0.1.41/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 garythompson   (501) staff       (20)      175 2023-01-11 23:02:58.000000 nef_pipelines-0.1.41/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 garythompson   (501) staff       (20)      287 2023-01-11 23:02:58.000000 nef_pipelines-0.1.41/.idea/modules.xml
+-rw-r--r--   0 garythompson   (501) staff       (20)      325 2023-04-26 19:24:39.000000 nef_pipelines-0.1.41/.idea/vcs.xml
+-rw-r--r--   0 garythompson   (501) staff       (20)     1331 2022-11-26 14:34:37.000000 nef_pipelines-0.1.41/.pre-commit-config.yaml
+-rw-r--r--   0 garythompson   (501) staff       (20)      490 2022-11-26 14:33:30.000000 nef_pipelines-0.1.41/.readthedocs.yml
+-rw-r--r--   0 garythompson   (501) staff       (20)      372 2023-02-07 22:36:51.000000 nef_pipelines-0.1.41/AUTHORS.md
+-rw-r--r--   0 garythompson   (501) staff       (20)     3747 2023-05-21 14:33:32.000000 nef_pipelines-0.1.41/CHANGELOG.md
+-rw-r--r--   0 garythompson   (501) staff       (20)    12299 2022-11-27 14:11:11.000000 nef_pipelines-0.1.41/CONTRIBUTING.md
+-rw-r--r--   0 garythompson   (501) staff       (20)    24410 2022-11-27 14:11:12.000000 nef_pipelines-0.1.41/LICENSE.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)     8765 2023-05-21 14:33:58.517928 nef_pipelines-0.1.41/PKG-INFO
+-rw-r--r--   0 garythompson   (501) staff       (20)     8212 2023-02-07 22:28:55.000000 nef_pipelines-0.1.41/README.md
+-rw-r--r--   0 garythompson   (501) staff       (20)      826 2023-02-05 15:31:16.000000 nef_pipelines-0.1.41/TODO.md
+-rw-r--r--   0 garythompson   (501) staff       (20)      346 2023-05-21 12:25:21.000000 nef_pipelines-0.1.41/pyproject.toml
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:57.420488 nef_pipelines-0.1.41/references/
+-rw-r--r--   0 garythompson   (501) staff       (20)    22346 2023-04-16 16:41:23.000000 nef_pipelines-0.1.41/references/Nmr Experiment Nomenclature v2.docx
+-rw-r--r--   0 garythompson   (501) staff       (20)   282399 2023-04-16 14:33:43.000000 nef_pipelines-0.1.41/references/fogh.vrankenj.bio.nmr.2006.36.147.pdf
+-rw-r--r--   0 garythompson   (501) staff       (20)     1229 2023-04-17 21:03:23.000000 nef_pipelines-0.1.41/release_to_pypi.sh
+-rw-r--r--   0 garythompson   (501) staff       (20)      354 2023-04-17 20:13:08.000000 nef_pipelines-0.1.41/requirements.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)     1630 2023-05-21 14:33:58.520813 nef_pipelines-0.1.41/setup.cfg
+-rw-r--r--   0 garythompson   (501) staff       (20)      710 2022-11-26 14:33:30.000000 nef_pipelines-0.1.41/setup.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:57.196515 nef_pipelines-0.1.41/src/
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:57.437581 nef_pipelines-0.1.41/src/nef_pipelines/
+-rw-r--r--   0 garythompson   (501) staff       (20)        6 2023-03-23 08:31:34.000000 nef_pipelines-0.1.41/src/nef_pipelines/VERSION
+-rw-r--r--   0 garythompson   (501) staff       (20)      577 2022-11-27 18:49:20.000000 nef_pipelines-0.1.41/src/nef_pipelines/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)       62 2022-11-27 18:48:20.000000 nef_pipelines-0.1.41/src/nef_pipelines/__main__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:57.483392 nef_pipelines-0.1.41/src/nef_pipelines/data/
+-rw-r--r--   0 garythompson   (501) staff       (20)  1486198 2023-05-06 14:31:14.000000 nef_pipelines-0.1.41/src/nef_pipelines/data/mmcif_nef_v1_1.dic
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:57.522436 nef_pipelines-0.1.41/src/nef_pipelines/lib/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.41/src/nef_pipelines/lib/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      124 2023-02-07 22:55:44.000000 nef_pipelines-0.1.41/src/nef_pipelines/lib/constants.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     1297 2022-11-27 19:40:25.000000 nef_pipelines-0.1.41/src/nef_pipelines/lib/header_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      945 2023-03-19 15:38:08.000000 nef_pipelines-0.1.41/src/nef_pipelines/lib/isotope_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2812 2023-04-26 21:04:53.000000 nef_pipelines-0.1.41/src/nef_pipelines/lib/nef_frames_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    18119 2023-05-07 11:12:00.000000 nef_pipelines-0.1.41/src/nef_pipelines/lib/nef_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    15083 2023-05-21 10:50:19.000000 nef_pipelines-0.1.41/src/nef_pipelines/lib/peak_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    21187 2023-04-30 15:31:02.000000 nef_pipelines-0.1.41/src/nef_pipelines/lib/sequence_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     6348 2023-02-07 21:12:56.000000 nef_pipelines-0.1.41/src/nef_pipelines/lib/shift_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     6548 2023-04-17 20:48:44.000000 nef_pipelines-0.1.41/src/nef_pipelines/lib/spectra_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     4191 2023-05-21 10:59:57.000000 nef_pipelines-0.1.41/src/nef_pipelines/lib/structures.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    10234 2023-04-26 19:21:33.000000 nef_pipelines-0.1.41/src/nef_pipelines/lib/test_lib.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:57.526259 nef_pipelines-0.1.41/src/nef_pipelines/lib/translation/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.41/src/nef_pipelines/lib/translation/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2160 2023-05-07 09:41:01.000000 nef_pipelines-0.1.41/src/nef_pipelines/lib/translation_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      292 2022-11-27 18:48:20.000000 nef_pipelines-0.1.41/src/nef_pipelines/lib/typer_utils.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    23798 2023-05-20 12:39:44.000000 nef_pipelines-0.1.41/src/nef_pipelines/lib/util.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     5335 2023-05-20 12:46:21.000000 nef_pipelines-0.1.41/src/nef_pipelines/main.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:57.526744 nef_pipelines-0.1.41/src/nef_pipelines/nef_app/
+-rw-r--r--   0 garythompson   (501) staff       (20)       49 2022-11-27 18:48:20.000000 nef_pipelines-0.1.41/src/nef_pipelines/nef_app/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:57.541052 nef_pipelines-0.1.41/src/nef_pipelines/tests/
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:57.551539 nef_pipelines-0.1.41/src/nef_pipelines/tests/chains/
+-rwxr--r--   0 garythompson   (501) staff       (20)        0 2022-11-25 17:14:10.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/chains/__init__.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     5259 2023-03-18 23:31:39.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/chains/test_clone.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:57.560572 nef_pipelines-0.1.41/src/nef_pipelines/tests/chains/test_data/
+-rwxr--r--   0 garythompson   (501) staff       (20)      581 2022-11-25 17:14:10.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/chains/test_data/3aa.nef
+-rwxr-xr-x   0 garythompson   (501) staff       (20)      837 2023-03-18 23:31:39.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/chains/test_data/3aa_x3.nef
+-rwxr--r--   0 garythompson   (501) staff       (20)     2172 2022-12-16 20:37:04.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/chains/test_data/multi_chain_shifts.nef
+-rwxr--r--   0 garythompson   (501) staff       (20)      491 2022-12-16 20:38:38.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/chains/test_list.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)    10032 2023-03-18 23:31:39.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/chains/test_rename.py
+-rwxr--r--   0 garythompson   (501) staff       (20)     9304 2023-01-30 23:11:50.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/chains/test_renumber.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      709 2023-01-12 09:57:27.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/conftest.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:57.561663 nef_pipelines-0.1.41/src/nef_pipelines/tests/csv/
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:57.565697 nef_pipelines-0.1.41/src/nef_pipelines/tests/csv/test_data/
+-rw-r--r--   0 garythompson   (501) staff       (20)       45 2023-01-31 08:50:56.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/csv/test_data/short.csv
+-rw-r--r--   0 garythompson   (501) staff       (20)      218 2023-01-31 08:49:14.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/csv/test_data/short_complete.csv
+-rw-r--r--   0 garythompson   (501) staff       (20)     5079 2023-01-31 22:17:03.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/csv/test_import_rdcs.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:57.567189 nef_pipelines-0.1.41/src/nef_pipelines/tests/echidna/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-05-04 20:35:04.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/echidna/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:57.569703 nef_pipelines-0.1.41/src/nef_pipelines/tests/echidna/test_data/
+-rw-r--r--   0 garythompson   (501) staff       (20)      695 2023-05-06 14:02:40.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/echidna/test_data/echidna_peaks.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)     1775 2023-05-06 14:16:20.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/echidna/test_data/echidna_sequence.nef
+-rw-r--r--   0 garythompson   (501) staff       (20)     3610 2023-05-06 20:59:13.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/echidna/test_import_peaks.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:57.570775 nef_pipelines-0.1.41/src/nef_pipelines/tests/fasta/
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:57.587194 nef_pipelines-0.1.41/src/nef_pipelines/tests/fasta/test_data/
+-rwxr--r--   0 garythompson   (501) staff       (20)       11 2022-12-06 19:49:15.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/fasta/test_data/3aa.fasta
+-rwxr-xr-x   0 garythompson   (501) staff       (20)       24 2023-03-18 23:31:39.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/fasta/test_data/3aa_x2.fasta
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     3178 2023-03-18 23:31:39.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/fasta/test_sequence.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:57.599153 nef_pipelines-0.1.41/src/nef_pipelines/tests/frames/
+-rwxr--r--   0 garythompson   (501) staff       (20)        0 2022-12-06 20:53:09.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/frames/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:57.601611 nef_pipelines-0.1.41/src/nef_pipelines/tests/frames/test_data/
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     1470 2023-03-18 23:31:39.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/frames/test_data/frames.nef
+-rwxr--r--   0 garythompson   (501) staff       (20)     1626 2022-12-16 21:06:02.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/frames/test_data/pales_test_1.nef
+-rwxr--r--   0 garythompson   (501) staff       (20)     2690 2022-12-16 21:06:48.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/frames/test_delete.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     1884 2023-05-16 09:49:59.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/frames/test_list.py
+-rwxr--r--   0 garythompson   (501) staff       (20)    10090 2023-04-15 16:15:29.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/frames/test_rename.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     1312 2023-03-18 23:31:39.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/frames/test_tabulate.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:57.619120 nef_pipelines-0.1.41/src/nef_pipelines/tests/mars/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-05 13:08:51.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/mars/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:57.622078 nef_pipelines-0.1.41/src/nef_pipelines/tests/mars/test_data/
+-rw-r--r--   0 garythompson   (501) staff       (20)     9631 2023-02-01 22:03:42.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/mars/test_data/sec5_short.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)      311 2023-02-05 15:30:43.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/mars/test_data/sec5_short.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)      838 2023-02-01 22:29:59.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/mars/test_export_shifts.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2537 2023-02-05 15:30:44.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/mars/test_import_shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:57.633915 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrpipe/
+-rwxr--r--   0 garythompson   (501) staff       (20)        0 2022-12-10 21:27:09.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrpipe/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:57.721788 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrpipe/test_data/
+-rwxr-xr-x   0 garythompson   (501) staff       (20)       12 2023-03-18 23:31:39.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrpipe/test_data/3aa.seq
+-rwxr--r--   0 garythompson   (501) staff       (20)       18 2022-12-16 20:31:09.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrpipe/test_data/3aa.tab
+-rwxr-xr-x   0 garythompson   (501) staff       (20)       15 2023-03-18 23:31:39.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrpipe/test_data/3aa10.seq
+-rwxr--r--   0 garythompson   (501) staff       (20)       16 2022-12-16 20:31:09.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrpipe/test_data/4peaks.seq
+-rw-------   0 garythompson   (501) staff       (20)      455 2023-01-10 13:25:00.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrpipe/test_data/P3a_l273R_nmrpipe_shifts_short.tab
+-rwxr--r--   0 garythompson   (501) staff       (20)    10961 2022-12-16 20:31:08.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrpipe/test_data/gb3.tab
+-rwxr--r--   0 garythompson   (501) staff       (20)    11038 2022-12-16 20:31:08.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned.tab
+-rwxr-xr-x   0 garythompson   (501) staff       (20)      943 2023-03-18 23:31:39.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc.tab
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     1878 2023-03-18 23:31:39.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc_expected.tab
+-rwxr--r--   0 garythompson   (501) staff       (20)    26327 2022-12-16 20:31:09.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrpipe/test_data/ns3_S135A_BMRB1.txt
+-rwxr--r--   0 garythompson   (501) staff       (20)      247 2022-12-16 20:31:09.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrpipe/test_data/ns3_S135A_BMRB1_short.txt
+-rwxr-xr-x   0 garythompson   (501) staff       (20)      800 2023-03-18 23:31:39.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrpipe/test_data/test_header_entry.txt
+-rwxr-xr-x   0 garythompson   (501) staff       (20)    14392 2023-04-24 21:03:24.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrpipe/test_gdb.py
+-rwxr--r--   0 garythompson   (501) staff       (20)      840 2022-12-16 20:35:58.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrpipe/test_peaks.py
+-rwxr--r--   0 garythompson   (501) staff       (20)      486 2022-12-16 20:35:58.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrpipe/test_pipe_lib.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     4158 2023-03-18 23:31:39.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrpipe/test_sequence.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     4454 2023-01-18 07:36:14.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrpipe/test_shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:57.750362 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrview/
+-rwxr--r--   0 garythompson   (501) staff       (20)        0 2022-12-11 15:04:32.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrview/__init__.py
+-rwxr--r--   0 garythompson   (501) staff       (20)    10752 2022-12-17 11:29:00.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrview/tcl_diag.html
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:57.801095 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrview/test_data/
+-rwxr--r--   0 garythompson   (501) staff       (20)       12 2022-12-11 15:04:32.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrview/test_data/3aa.seq
+-rwxr--r--   0 garythompson   (501) staff       (20)       15 2022-12-11 15:04:32.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrview/test_data/3aa10.seq
+-rwxr--r--   0 garythompson   (501) staff       (20)       16 2022-12-17 11:29:00.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrview/test_data/4peaks.seq
+-rwxr-xr-x   0 garythompson   (501) staff       (20)      980 2023-03-18 23:31:39.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrview/test_data/4peaks.xpk
+-rwxr--r--   0 garythompson   (501) staff       (20)      880 2022-12-11 15:04:32.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrview/test_data/expected_nmr_view.xpk
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     2178 2023-03-18 23:31:39.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrview/test_data/expected_sequence_and_peaks_nmrview.txt
+-rwxr--r--   0 garythompson   (501) staff       (20)      319 2022-12-11 15:04:32.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrview/test_data/joe_clic.xpk
+-rwxr--r--   0 garythompson   (501) staff       (20)     2172 2022-12-11 15:04:32.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrview/test_data/nmrview_expected_4aa.txt
+-rwxr--r--   0 garythompson   (501) staff       (20)    29631 2022-12-11 15:04:32.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrview/test_data/ppm.out
+-rwxr--r--   0 garythompson   (501) staff       (20)      540 2022-12-11 15:04:32.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrview/test_data/ppm_out.seq
+-rwxr--r--   0 garythompson   (501) staff       (20)       12 2022-12-11 15:04:32.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrview/test_data/ppm_out_short.seq
+-rwxr--r--   0 garythompson   (501) staff       (20)      126 2022-12-11 15:04:32.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrview/test_data/ppm_short.out
+-rwxr--r--   0 garythompson   (501) staff       (20)      522 2022-12-17 11:29:00.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrview/test_data/ppm_short_seq.nef
+-rwxr--r--   0 garythompson   (501) staff       (20)      800 2022-12-11 15:05:20.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrview/test_data/test_header_entry.txt
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     2646 2023-03-18 23:31:39.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrview/test_export_peaks.py
+-rwxr--r--   0 garythompson   (501) staff       (20)     3343 2023-01-14 17:44:39.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrview/test_export_sequences.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     3872 2023-02-15 22:22:17.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrview/test_import_peaks.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     3915 2023-02-07 23:04:20.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrview/test_import_sequence.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     4734 2023-01-18 07:36:14.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrview/test_import_shifts.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     2166 2023-03-18 23:31:39.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrview/test_tcl.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:57.804024 nef_pipelines-0.1.41/src/nef_pipelines/tests/pales/
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:57.837308 nef_pipelines-0.1.41/src/nef_pipelines/tests/pales/test_data/
+-rwxr--r--   0 garythompson   (501) staff       (20)     1626 2022-12-17 16:34:00.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/pales/test_data/pales_test_1.nef
+-rwxr--r--   0 garythompson   (501) staff       (20)     1627 2022-12-17 16:34:00.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/pales/test_data/pales_test_2.nef
+-rwxr--r--   0 garythompson   (501) staff       (20)     1647 2023-01-27 21:30:12.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/pales/test_data/pales_test_segids.nef
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     2773 2023-01-30 23:21:17.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/pales/test_rdcs.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     2043 2023-03-18 23:31:39.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/pales/test_template.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:57.839184 nef_pipelines-0.1.41/src/nef_pipelines/tests/pdbx/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-01-31 19:44:59.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/pdbx/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:57.855641 nef_pipelines-0.1.41/src/nef_pipelines/tests/pdbx/test_data/
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     4795 2023-03-18 23:31:39.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/pdbx/test_data/3a_ab.pdb
+-rwxr--r--   0 garythompson   (501) staff       (20)     4795 2022-12-17 16:52:18.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/pdbx/test_data/3a_cccc_dddd.pdb
+-rwxr--r--   0 garythompson   (501) staff       (20)     4195 2022-12-17 16:52:18.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/pdbx/test_data/3a_no_chain_no_segid.pdb
+-rwxr--r--   0 garythompson   (501) staff       (20)     2395 2022-12-17 16:52:18.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/pdbx/test_data/3aa.pdb
+-rwxr--r--   0 garythompson   (501) staff       (20)     2254 2022-12-17 16:52:18.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/pdbx/test_data/3aa11_13.pdb
+-rwxr--r--   0 garythompson   (501) staff       (20)      800 2022-12-10 20:00:10.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/pdbx/test_data/test_header_entry.txt
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     4248 2023-01-15 11:02:28.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/pdbx/test_sequence.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:57.857177 nef_pipelines-0.1.41/src/nef_pipelines/tests/shifts/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-04-16 09:07:56.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/shifts/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     8438 2023-04-17 20:44:38.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/shifts/test_make_peaks.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:57.862181 nef_pipelines-0.1.41/src/nef_pipelines/tests/shifty/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-09 08:07:44.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/shifty/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      773 2023-02-09 08:08:24.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/shifty/test_export_shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:57.912707 nef_pipelines-0.1.41/src/nef_pipelines/tests/sparky/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-04-26 18:29:03.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/sparky/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:57.945053 nef_pipelines-0.1.41/src/nef_pipelines/tests/sparky/test_data/
+-rw-r--r--   0 garythompson   (501) staff       (20)     1393 2023-01-31 21:17:52.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/sparky/test_data/P3a_L273R_sequence_short.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)     2342 2023-03-19 00:02:41.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/sparky/test_data/peaks_short_with_assignments.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)       40 2023-04-26 18:38:57.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/sparky/test_data/sparky_basic_sequence_dna.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)        9 2023-04-26 18:38:57.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/sparky/test_data/sparky_basic_sequence_protein.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)      241 2023-04-26 21:06:34.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/sparky/test_data/sparky_manual_basic.peaks
+-rw-r--r--   0 garythompson   (501) staff       (20)     1187 2023-04-26 18:24:37.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/sparky/test_data/sparky_manual_basic_sequence.nef
+-rw-r--r--   0 garythompson   (501) staff       (20)      359 2023-04-26 19:32:49.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/sparky/test_data/sparky_manual_full.peaks
+-rw-r--r--   0 garythompson   (501) staff       (20)      422 2023-04-26 20:35:49.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/sparky/test_data/sparky_manual_full_comment.peaks
+-rw-r--r--   0 garythompson   (501) staff       (20)      354 2023-05-04 18:45:19.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/sparky/test_data/sparky_manual_full_no_sequence.peaks
+-rw-r--r--   0 garythompson   (501) staff       (20)     1718 2023-01-17 09:55:08.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/sparky/test_data/test_shifts_P3a_L273R_shifts_short.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)     2342 2023-03-19 00:02:41.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)     2157 2023-03-19 00:02:41.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_chains.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)     2156 2023-03-19 00:02:41.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_different_residues.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)     2803 2023-03-19 00:02:41.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_i_minus_one.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)     2326 2023-03-19 00:02:41.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_overlapping_chains.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)    12427 2023-03-24 20:06:24.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/sparky/test_export_peaks.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     4311 2023-05-21 12:09:19.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/sparky/test_import_peaks.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2475 2023-04-26 18:38:58.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/sparky/test_import_sequence.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2661 2023-01-17 17:17:45.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/sparky/test_import_shifts.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2322 2023-05-16 09:41:29.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/sparky/test_sparky_lib.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:57.980425 nef_pipelines-0.1.41/src/nef_pipelines/tests/test_data/
+-rw-r--r--   0 garythompson   (501) staff       (20)      658 2023-01-11 15:13:08.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/test_data/3a_ab.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)       11 2023-04-15 14:38:14.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/test_data/empty.nef
+-rw-r--r--   0 garythompson   (501) staff       (20)      837 2022-12-15 21:03:33.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/test_data/header.nef
+-rwxr-xr-x   0 garythompson   (501) staff       (20)      908 2023-03-18 23:31:39.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/test_data/multi_chain.nef
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     2979 2023-03-18 23:31:39.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/test_data/nef_3_peaks.nef
+-rwxr--r--   0 garythompson   (501) staff       (20)      979 2023-01-18 17:43:15.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/test_data/tailin_seq_short.nef
+-rw-r--r--   0 garythompson   (501) staff       (20)     2958 2023-02-07 21:50:52.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/test_data/test_agv.neff
+-rwxr-xr-x   0 garythompson   (501) staff       (20)    64721 2023-04-16 09:21:50.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/test_data/ubiquitin_short.nef
+-rw-r--r--   0 garythompson   (501) staff       (20)     1884 2023-02-07 23:05:23.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/test_header.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     9456 2023-03-18 23:11:48.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/test_nef_lib.py
+-rwxr-xr-x   0 garythompson   (501) staff       (20)     7641 2023-04-24 20:39:10.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/test_sequence_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2750 2022-12-14 20:48:12.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/test_test.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      708 2023-05-18 21:37:12.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/test_util.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:57.982508 nef_pipelines-0.1.41/src/nef_pipelines/tests/xcamshift/
+-rw-r--r--   0 garythompson   (501) staff       (20)     1860 2023-02-07 22:05:04.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/xcamshift/test_export_shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.023205 nef_pipelines-0.1.41/src/nef_pipelines/tests/xeasy/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-04-26 18:29:03.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/xeasy/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.028630 nef_pipelines-0.1.41/src/nef_pipelines/tests/xeasy/test_data/
+-rw-r--r--   0 garythompson   (501) staff       (20)      516 2023-05-18 21:29:57.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/xeasy/test_data/basic.peaks
+-rw-r--r--   0 garythompson   (501) staff       (20)       99 2023-05-20 13:22:50.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/xeasy/test_data/basic.seq
+-rw-r--r--   0 garythompson   (501) staff       (20)      747 2023-05-21 10:34:57.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/xeasy/test_data/basic_sequence.nef
+-rw-r--r--   0 garythompson   (501) staff       (20)     3392 2023-05-21 11:56:45.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/xeasy/test_import_peaks.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     1124 2023-05-20 13:24:53.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/xeasy/test_import_sequence.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     1551 2023-05-21 14:27:41.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/xeasy/test_import_shifts.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     8984 2023-05-21 14:27:42.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/xeasy/test_xeasy_lib.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.043376 nef_pipelines-0.1.41/src/nef_pipelines/tests/xplor/
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.114938 nef_pipelines-0.1.41/src/nef_pipelines/tests/xplor/test_data/
+-rw-r--r--   0 garythompson   (501) staff       (20)    10948 2022-12-22 19:24:27.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/xplor/test_data/3a_ab.psf
+-rw-r--r--   0 garythompson   (501) staff       (20)     2700 2023-01-31 09:42:10.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/xplor/test_data/3a_ab_rdcs.neff
+-rw-r--r--   0 garythompson   (501) staff       (20)      417 2022-12-22 19:24:27.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/xplor/test_data/bad_field_count.psf
+-rw-r--r--   0 garythompson   (501) staff       (20)        7 2022-12-22 19:24:28.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/xplor/test_data/bad_header.psf
+-rw-r--r--   0 garythompson   (501) staff       (20)      434 2022-12-22 19:24:27.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/xplor/test_data/bad_natom.psf
+-rw-r--r--   0 garythompson   (501) staff       (20)      429 2022-12-22 19:24:27.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/xplor/test_data/bad_residue_number.psf
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-12-21 15:10:23.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/xplor/test_data/empty.psf
+-rw-r--r--   0 garythompson   (501) staff       (20)      216 2022-12-22 19:24:28.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/xplor/test_data/no_residues_found.psf
+-rw-r--r--   0 garythompson   (501) staff       (20)      623 2023-01-04 12:41:40.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals.tbl
+-rw-r--r--   0 garythompson   (501) staff       (20)      580 2023-01-11 14:25:21.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals_bad.tbl
+-rw-r--r--   0 garythompson   (501) staff       (20)      503 2023-01-11 14:57:02.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals_no_segids.tbl
+-rw-r--r--   0 garythompson   (501) staff       (20)      197 2023-01-11 22:37:32.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/xplor/test_data/test_2_distances.tbl
+-rw-r--r--   0 garythompson   (501) staff       (20)      159 2023-01-11 22:37:32.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/xplor/test_data/test_2_distances_bad.tbl
+-rw-r--r--   0 garythompson   (501) staff       (20)      137 2023-01-11 22:37:32.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/xplor/test_data/test_2_distances_no_segids.tbl
+-rw-r--r--   0 garythompson   (501) staff       (20)      186 2023-01-04 11:17:43.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/xplor/test_data/test_2_noes.tbl
+-rw-r--r--   0 garythompson   (501) staff       (20)     8093 2023-01-15 11:02:28.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/xplor/test_dihedrals.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     6535 2023-01-15 10:58:38.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/xplor/test_distances.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     1974 2023-01-31 09:53:27.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/xplor/test_export_rdcs.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     1487 2023-01-04 12:32:55.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/xplor/test_import_sequence.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     3413 2022-12-22 19:24:29.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/xplor/test_psf_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    11065 2023-01-11 21:19:43.000000 nef_pipelines-0.1.41/src/nef_pipelines/tests/xplor/test_xplor_lib.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.130156 nef_pipelines-0.1.41/src/nef_pipelines/tools/
+-rw-r--r--   0 garythompson   (501) staff       (20)     2268 2023-04-02 20:29:58.000000 nef_pipelines-0.1.41/src/nef_pipelines/tools/about.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.164161 nef_pipelines-0.1.41/src/nef_pipelines/tools/chains/
+-rw-r--r--   0 garythompson   (501) staff       (20)      527 2023-01-02 20:41:38.000000 nef_pipelines-0.1.41/src/nef_pipelines/tools/chains/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2593 2023-04-23 18:00:54.000000 nef_pipelines-0.1.41/src/nef_pipelines/tools/chains/clone.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     1417 2023-03-21 20:24:03.000000 nef_pipelines-0.1.41/src/nef_pipelines/tools/chains/list.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2670 2023-03-18 23:07:53.000000 nef_pipelines-0.1.41/src/nef_pipelines/tools/chains/rename.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     9203 2023-01-10 10:15:33.000000 nef_pipelines-0.1.41/src/nef_pipelines/tools/chains/renumber.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.169319 nef_pipelines-0.1.41/src/nef_pipelines/tools/entry/
+-rw-r--r--   0 garythompson   (501) staff       (20)      376 2022-11-29 12:15:24.000000 nef_pipelines-0.1.41/src/nef_pipelines/tools/entry/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      692 2023-02-07 13:11:22.000000 nef_pipelines-0.1.41/src/nef_pipelines/tools/entry/rename.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.184455 nef_pipelines-0.1.41/src/nef_pipelines/tools/frames/
+-rw-r--r--   0 garythompson   (501) staff       (20)      639 2023-04-15 16:14:41.000000 nef_pipelines-0.1.41/src/nef_pipelines/tools/frames/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2556 2023-03-19 00:07:20.000000 nef_pipelines-0.1.41/src/nef_pipelines/tools/frames/delete.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     4111 2023-03-21 19:38:23.000000 nef_pipelines-0.1.41/src/nef_pipelines/tools/frames/insert.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     7414 2023-05-16 09:49:59.000000 nef_pipelines-0.1.41/src/nef_pipelines/tools/frames/list.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     6711 2023-04-17 20:20:20.000000 nef_pipelines-0.1.41/src/nef_pipelines/tools/frames/rename.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     8952 2023-03-21 20:29:06.000000 nef_pipelines-0.1.41/src/nef_pipelines/tools/frames/tabulate.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      871 2023-02-07 23:05:12.000000 nef_pipelines-0.1.41/src/nef_pipelines/tools/header.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     5132 2022-11-27 18:48:20.000000 nef_pipelines-0.1.41/src/nef_pipelines/tools/offset_shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.186767 nef_pipelines-0.1.41/src/nef_pipelines/tools/peaks/
+-rw-r--r--   0 garythompson   (501) staff       (20)    10891 2023-03-23 08:18:29.000000 nef_pipelines-0.1.41/src/nef_pipelines/tools/peaks/match.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    10539 2022-12-22 18:47:15.000000 nef_pipelines-0.1.41/src/nef_pipelines/tools/res_assign.py_unused
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.207948 nef_pipelines-0.1.41/src/nef_pipelines/tools/shifts/
+-rw-r--r--   0 garythompson   (501) staff       (20)      372 2023-03-20 08:59:26.000000 nef_pipelines-0.1.41/src/nef_pipelines/tools/shifts/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     7145 2023-05-16 20:28:28.000000 nef_pipelines-0.1.41/src/nef_pipelines/tools/shifts/make_peaks.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      200 2022-11-28 23:58:46.000000 nef_pipelines-0.1.41/src/nef_pipelines/tools/sink.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      445 2022-11-28 21:57:18.000000 nef_pipelines-0.1.41/src/nef_pipelines/tools/stream.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     3753 2023-04-17 20:08:48.000000 nef_pipelines-0.1.41/src/nef_pipelines/tools/test.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.210415 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.211088 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/csv/
+-rw-r--r--   0 garythompson   (501) staff       (20)      409 2023-03-19 00:07:20.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/csv/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.213451 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/csv/importers/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-01-18 16:41:09.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/csv/importers/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    14955 2023-01-31 09:30:29.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/csv/importers/rdcs.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.217845 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/echidna/
+-rw-r--r--   0 garythompson   (501) staff       (20)      465 2023-05-04 20:35:04.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/echidna/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.219645 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/echidna/importers/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-05-04 20:35:04.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/echidna/importers/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    15433 2023-05-21 12:09:20.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/echidna/importers/peaks.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.221960 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/fasta/
+-rw-r--r--   0 garythompson   (501) staff       (20)      646 2022-11-27 19:51:40.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/fasta/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.244582 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/fasta/exporters/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/fasta/exporters/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     3952 2023-03-22 17:47:24.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/fasta/exporters/sequence.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.249655 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/fasta/importers/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/fasta/importers/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     5532 2023-04-24 20:34:49.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/fasta/importers/sequence.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.252169 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/mars/
+-rw-r--r--   0 garythompson   (501) staff       (20)      892 2023-05-21 10:50:14.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/mars/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.264103 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/mars/exporters/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/mars/exporters/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     6571 2023-02-15 21:49:23.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/mars/exporters/fragments.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     4299 2023-02-15 22:21:34.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/mars/exporters/input.py
+-rw-r--r--   0 garythompson   (501) staff       (20)      780 2022-11-28 23:56:55.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/mars/exporters/sequence.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     6001 2023-03-11 19:52:09.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/mars/exporters/shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.267115 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/mars/importers/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-05 10:22:38.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/mars/importers/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    11657 2023-04-24 20:38:57.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/mars/importers/shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.300090 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/nmrpipe/
+-rw-r--r--   0 garythompson   (501) staff       (20)      679 2022-11-27 19:52:05.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/nmrpipe/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.308412 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/nmrpipe/importers/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/nmrpipe/importers/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2414 2022-12-13 19:17:42.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/nmrpipe/importers/peaks.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     3498 2023-04-24 20:38:57.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/nmrpipe/importers/sequence.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     3151 2023-04-24 20:36:47.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/nmrpipe/importers/shifts.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    20224 2023-04-24 21:17:19.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/nmrpipe/nmrpipe_lib.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.315992 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/nmrview/
+-rw-r--r--   0 garythompson   (501) staff       (20)     1056 2023-01-16 22:48:48.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/nmrview/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.351483 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/nmrview/exporters/
+-rw-r--r--   0 garythompson   (501) staff       (20)    13841 2023-02-07 13:14:10.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/nmrview/exporters/peaks.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     7053 2023-01-30 07:39:27.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/nmrview/exporters/sequences.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     9136 2023-01-16 22:47:55.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/nmrview/exporters/shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.361872 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/nmrview/importers/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-11-27 18:48:20.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/nmrview/importers/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    17212 2022-12-22 18:41:48.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/nmrview/importers/peaks.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2330 2023-04-24 20:38:58.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/nmrview/importers/sequence.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     5787 2023-04-24 20:38:58.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/nmrview/importers/shifts.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     8866 2023-01-16 22:43:21.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/nmrview/nmrview_lib.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.365683 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/pales/
+-rw-r--r--   0 garythompson   (501) staff       (20)      660 2022-11-27 19:52:13.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/pales/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.369587 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/pales/exporters/
+-rw-r--r--   0 garythompson   (501) staff       (20)    10943 2023-05-07 09:41:03.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/pales/exporters/rdcs.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     4817 2023-03-06 22:17:20.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/pales/exporters/template.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.371699 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/pdbx/
+-rw-r--r--   0 garythompson   (501) staff       (20)      454 2022-12-17 16:50:37.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/pdbx/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.391469 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/pdbx/importers/
+-rw-r--r--   0 garythompson   (501) staff       (20)     4655 2022-12-17 16:51:05.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/pdbx/importers/sequence.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.395773 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/rpf/
+-rw-r--r--   0 garythompson   (501) staff       (20)      608 2023-03-23 08:19:19.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/rpf/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.399364 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/rpf/exporters/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-03-22 21:34:49.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/rpf/exporters/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    11873 2023-03-22 22:37:50.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/rpf/exporters/shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.401394 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/shifty/
+-rw-r--r--   0 garythompson   (501) staff       (20)      523 2023-02-08 16:38:07.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/shifty/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.403816 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/shifty/exporters/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-05 22:19:02.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/shifty/exporters/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     6339 2023-04-24 20:32:00.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/shifty/exporters/shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.408395 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/sparky/
+-rw-r--r--   0 garythompson   (501) staff       (20)      804 2023-04-26 18:38:57.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/sparky/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.437163 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/sparky/exporters/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-03-18 23:36:58.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/sparky/exporters/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    15804 2023-05-04 07:46:41.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/sparky/exporters/peaks.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.446559 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/sparky/importers/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-01-16 13:30:23.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/sparky/importers/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    16181 2023-05-21 12:09:20.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/sparky/importers/peaks.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     6463 2023-05-20 13:08:43.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/sparky/importers/sequence.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     8953 2023-03-19 00:07:20.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/sparky/importers/shifts.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     8328 2023-05-15 12:35:13.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/sparky/sparky_lib.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.449738 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/xcamshift/
+-rw-r--r--   0 garythompson   (501) staff       (20)      554 2023-02-07 22:05:04.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/xcamshift/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.451599 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/xcamshift/exporters/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-02-05 22:19:02.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/xcamshift/exporters/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     3787 2023-02-07 22:05:13.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/xcamshift/exporters/shifts.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.454990 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/xeasy/
+-rw-r--r--   0 garythompson   (501) staff       (20)      666 2023-05-21 14:27:41.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/xeasy/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.478916 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/xeasy/importers/
+-rw-r--r--   0 garythompson   (501) staff       (20)     2925 2023-05-21 12:09:19.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/xeasy/importers/peaks.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2852 2023-05-21 11:00:00.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/xeasy/importers/sequence.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     1899 2023-05-21 14:30:07.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/xeasy/importers/shifts.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    22539 2023-05-21 14:29:12.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/xeasy/xeasy_lib.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.485417 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/xplor/
+-rw-r--r--   0 garythompson   (501) staff       (20)      933 2023-02-05 22:57:14.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/xplor/__init__.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.489902 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/xplor/exporters/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2023-01-20 20:08:15.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/xplor/exporters/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     7167 2023-01-31 09:54:44.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/xplor/exporters/rdcs.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:58.515026 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/xplor/importers/
+-rw-r--r--   0 garythompson   (501) staff       (20)        0 2022-12-17 17:33:41.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/xplor/importers/__init__.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2834 2023-03-24 21:54:07.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/xplor/importers/dihedrals.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     2888 2023-01-11 22:37:57.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/xplor/importers/distances.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     3298 2023-01-04 12:32:55.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/xplor/importers/sequence.py
+-rw-r--r--   0 garythompson   (501) staff       (20)     3663 2022-12-22 19:24:58.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/xplor/psf_lib.py
+-rw-r--r--   0 garythompson   (501) staff       (20)    38877 2023-01-11 22:37:34.000000 nef_pipelines-0.1.41/src/nef_pipelines/transcoders/xplor/xplor_lib.py
+drwxr-xr-x   0 garythompson   (501) staff       (20)        0 2023-05-21 14:33:57.455047 nef_pipelines-0.1.41/src/nef_pipelines.egg-info/
+-rw-r--r--   0 garythompson   (501) staff       (20)     8765 2023-05-21 14:33:57.000000 nef_pipelines-0.1.41/src/nef_pipelines.egg-info/PKG-INFO
+-rw-r--r--   0 garythompson   (501) staff       (20)    14639 2023-05-21 14:33:57.000000 nef_pipelines-0.1.41/src/nef_pipelines.egg-info/SOURCES.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)        1 2023-05-21 14:33:57.000000 nef_pipelines-0.1.41/src/nef_pipelines.egg-info/dependency_links.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)       48 2023-05-21 14:33:57.000000 nef_pipelines-0.1.41/src/nef_pipelines.egg-info/entry_points.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)        1 2022-11-27 19:48:54.000000 nef_pipelines-0.1.41/src/nef_pipelines.egg-info/not-zip-safe
+-rw-r--r--   0 garythompson   (501) staff       (20)      363 2023-05-21 14:33:57.000000 nef_pipelines-0.1.41/src/nef_pipelines.egg-info/requires.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)       14 2023-05-21 14:33:57.000000 nef_pipelines-0.1.41/src/nef_pipelines.egg-info/top_level.txt
+-rw-r--r--   0 garythompson   (501) staff       (20)     3032 2023-02-01 22:03:42.000000 nef_pipelines-0.1.41/tox.ini
```

### Comparing `nef_pipelines-0.1.40/.github/workflows/ci.yml` & `nef_pipelines-0.1.41/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/.idea/inspectionProfiles/Project_Default.xml` & `nef_pipelines-0.1.41/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/.pre-commit-config.yaml` & `nef_pipelines-0.1.41/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/CHANGELOG.md` & `nef_pipelines-0.1.41/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -148,7 +148,12 @@
 ## version 0.1.39
 
 fixed a bug in frames list (verbose option was ignored)
 
 ## version 0.1.40
 
 fix a bug: make peaks faaled on generating empty peak lists
+
+## version 0.1.41
+
+add importers for xeasy [flya dialect] sequences, peaks and shifts
+a  number of gug fixes in the sparky and exhdnia tools
```

### Comparing `nef_pipelines-0.1.40/CONTRIBUTING.md` & `nef_pipelines-0.1.41/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/LICENSE.txt` & `nef_pipelines-0.1.41/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/PKG-INFO` & `nef_pipelines-0.1.41/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nef_pipelines
-Version: 0.1.40
+Version: 0.1.41
 Summary: Tools for Manipulating NEF [NMR Exchange Format] Files and Foreign File Access
 Home-page: https://github.com/varioustoxins/NEF-Pipelines
 Author: varioustoxins
 Author-email: g.s.thompson@kent.ac.uk
 License: LGPL-2.1
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `nef_pipelines-0.1.40/README.md` & `nef_pipelines-0.1.41/README.md`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/TODO.md` & `nef_pipelines-0.1.41/TODO.md`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/references/Nmr Experiment Nomenclature v2.docx` & `nef_pipelines-0.1.41/references/Nmr Experiment Nomenclature v2.docx`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/references/fogh.vrankenj.bio.nmr.2006.36.147.pdf` & `nef_pipelines-0.1.41/references/fogh.vrankenj.bio.nmr.2006.36.147.pdf`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/release_to_pypi.sh` & `nef_pipelines-0.1.41/release_to_pypi.sh`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/setup.cfg` & `nef_pipelines-0.1.41/setup.cfg`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/setup.py` & `nef_pipelines-0.1.41/setup.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/__init__.py` & `nef_pipelines-0.1.41/src/nef_pipelines/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/data/mmcif_nef_v1_1.dic` & `nef_pipelines-0.1.41/src/nef_pipelines/data/mmcif_nef_v1_1.dic`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/lib/header_lib.py` & `nef_pipelines-0.1.41/src/nef_pipelines/lib/header_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/lib/isotope_lib.py` & `nef_pipelines-0.1.41/src/nef_pipelines/lib/isotope_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/lib/nef_frames_lib.py` & `nef_pipelines-0.1.41/src/nef_pipelines/lib/nef_frames_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/lib/nef_lib.py` & `nef_pipelines-0.1.41/src/nef_pipelines/lib/nef_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/lib/peak_lib.py` & `nef_pipelines-0.1.41/src/nef_pipelines/lib/peak_lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -320,15 +320,15 @@
         peak_loop_tags.append(CCPN_COMMENT)
 
     peak_loop.add_tag(peak_loop_tags)
 
     for index, peak in enumerate(peaks):
         peak_data = {
             INDEX: index,
-            PEAK_ID: index,
+            PEAK_ID: index if peak.id is None else peak.id,
             HEIGHT: peak.height,
             HEIGHT_UNCERTAINTY: peak.height_uncertainty,
             VOLUME: peak.volume,
             VOLUME_UNCERTAINTY: peak.volume_uncertainty,
         }
 
         for dim_index, shift in enumerate(peak.shifts, start=1):
```

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/lib/sequence_lib.py` & `nef_pipelines-0.1.41/src/nef_pipelines/lib/sequence_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/lib/shift_lib.py` & `nef_pipelines-0.1.41/src/nef_pipelines/lib/shift_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/lib/spectra_lib.py` & `nef_pipelines-0.1.41/src/nef_pipelines/lib/spectra_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/lib/structures.py` & `nef_pipelines-0.1.41/src/nef_pipelines/lib/structures.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,15 +166,17 @@
     LORENTZIAN = auto()
     SPLINE = auto()
 
 
 @dataclass(frozen=True, order=True)
 class NewPeak:
 
-    shifts: List[ShiftData]
+    shifts: List[
+        ShiftData
+    ]  # shifts we support this by maving mutiples peaks with the same id
 
     id: Optional[int] = None
     height: Optional[float] = None
     height_uncertainty: Optional[float] = None
     volume: Optional[float] = None
     volume_uncertainty: Optional[float] = None
     peak_fit_method: Optional[Union[str, PeakFitMethod]] = None
```

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/lib/test_lib.py` & `nef_pipelines-0.1.41/src/nef_pipelines/lib/test_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/lib/translation_lib.py` & `nef_pipelines-0.1.41/src/nef_pipelines/lib/translation_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/lib/util.py` & `nef_pipelines-0.1.41/src/nef_pipelines/lib/util.py`

 * *Files 1% similar despite different names*

```diff
@@ -856,15 +856,16 @@
     :param target: the string to strip
     :param letters:  the letters to be stripper
     :return: a tuple of the form (<stripped-string>, <stripped-letters>)
     """
 
     remaining = target.lstrip(letters)
 
-    stripped = target[: len(target) - len(remaining)]
+    num_stripped = len(target) - len(remaining)
+    stripped = target[:num_stripped] if num_stripped > 0 else ""
 
     return stripped, remaining
 
 
 def strip_characters_right(target: str, letters: str) -> Tuple[str, str]:
     """
     strip the characters from letters from the right of the target and return a tuple containing
@@ -873,18 +874,18 @@
 
     :param target: the string to strip
     :param letters:  the letters to be stripper
     :return: a tuple of the form (<stripped-string>, <stripped-letters>)
     """
 
     remaining = target.rstrip(letters)
+    num_stripped = len(target) - len(remaining)
+    stripped = target[-num_stripped:] if num_stripped > 0 else ""
 
-    stripped = target[(len(target) - len(remaining)) - 1 :]
-
-    return stripped, remaining
+    return remaining, stripped
 
 
 def strip_line_comment(line: str, comment_character: str = "#") -> Tuple[str, str]:
     comment = None
     if comment_character in line:
         index = line.index(comment_character)
         comment = line[index + 1 :]
```

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/main.py` & `nef_pipelines-0.1.41/src/nef_pipelines/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -93,14 +93,15 @@
             "nef_pipelines.transcoders.nmrview",
             "nef_pipelines.transcoders.pales",
             "nef_pipelines.transcoders.pdbx",
             "nef_pipelines.transcoders.rpf",
             "nef_pipelines.transcoders.shifty",
             "nef_pipelines.transcoders.sparky",
             "nef_pipelines.transcoders.xcamshift",
+            "nef_pipelines.transcoders.xeasy",
             "nef_pipelines.transcoders.xplor",
         ]
         for module_name in modules:
             try:
                 import_module(module_name)
             except Exception:
                 msg = f"plugin {module_name}\n{format_exc()}"
```

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/chains/test_clone.py` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/chains/test_clone.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/chains/test_data/3aa.nef` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/chains/test_data/3aa.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/chains/test_data/3aa_x3.nef` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/chains/test_data/3aa_x3.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/chains/test_data/multi_chain_shifts.nef` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/chains/test_data/multi_chain_shifts.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/chains/test_rename.py` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/chains/test_rename.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/chains/test_renumber.py` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/chains/test_renumber.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/conftest.py` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/csv/test_import_rdcs.py` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/csv/test_import_rdcs.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/echidna/test_data/echidna_peaks.txt` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/echidna/test_data/echidna_peaks.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/echidna/test_data/echidna_sequence.nef` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/echidna/test_data/echidna_sequence.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/echidna/test_import_peaks.py` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/echidna/test_import_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/fasta/test_sequence.py` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/fasta/test_sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/frames/test_data/frames.nef` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/frames/test_data/frames.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/frames/test_data/pales_test_1.nef` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/frames/test_data/pales_test_1.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/frames/test_delete.py` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/frames/test_delete.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/frames/test_list.py` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/frames/test_list.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/frames/test_rename.py` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/frames/test_rename.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/frames/test_tabulate.py` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/frames/test_tabulate.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/mars/test_data/sec5_short.neff` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/mars/test_data/sec5_short.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/mars/test_export_shifts.py` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/mars/test_export_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/mars/test_import_shifts.py` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/mars/test_import_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/nmrpipe/test_data/gb3.tab` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrpipe/test_data/gb3.tab`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned.tab` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned.tab`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc.tab` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc.tab`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc_expected.tab` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrpipe/test_data/gb3_assigned_trunc_expected.tab`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/nmrpipe/test_data/ns3_S135A_BMRB1.txt` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrpipe/test_data/ns3_S135A_BMRB1.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/nmrpipe/test_data/test_header_entry.txt` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrpipe/test_data/test_header_entry.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/nmrpipe/test_gdb.py` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrpipe/test_gdb.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/nmrpipe/test_peaks.py` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrpipe/test_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/nmrpipe/test_sequence.py` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrpipe/test_sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/nmrpipe/test_shifts.py` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrpipe/test_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/nmrview/tcl_diag.html` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrview/tcl_diag.html`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/nmrview/test_data/4peaks.xpk` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrview/test_data/4peaks.xpk`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/nmrview/test_data/expected_nmr_view.xpk` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrview/test_data/expected_nmr_view.xpk`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/nmrview/test_data/expected_sequence_and_peaks_nmrview.txt` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrview/test_data/expected_sequence_and_peaks_nmrview.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/nmrview/test_data/nmrview_expected_4aa.txt` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrview/test_data/nmrview_expected_4aa.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/nmrview/test_data/ppm.out` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrview/test_data/ppm.out`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/nmrview/test_data/ppm_out.seq` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrview/test_data/ppm_out.seq`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/nmrview/test_data/ppm_short_seq.nef` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrview/test_data/ppm_short_seq.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/nmrview/test_data/test_header_entry.txt` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrview/test_data/test_header_entry.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/nmrview/test_export_peaks.py` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrview/test_export_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/nmrview/test_export_sequences.py` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrview/test_export_sequences.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/nmrview/test_import_peaks.py` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrview/test_import_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/nmrview/test_import_sequence.py` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrview/test_import_sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/nmrview/test_import_shifts.py` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrview/test_import_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/nmrview/test_tcl.py` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/nmrview/test_tcl.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/pales/test_data/pales_test_1.nef` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/pales/test_data/pales_test_1.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/pales/test_data/pales_test_2.nef` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/pales/test_data/pales_test_2.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/pales/test_data/pales_test_segids.nef` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/pales/test_data/pales_test_segids.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/pales/test_rdcs.py` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/pales/test_rdcs.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/pales/test_template.py` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/pales/test_template.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/pdbx/test_data/3a_ab.pdb` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/pdbx/test_data/3a_ab.pdb`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/pdbx/test_data/3a_cccc_dddd.pdb` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/pdbx/test_data/3a_cccc_dddd.pdb`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/pdbx/test_data/3a_no_chain_no_segid.pdb` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/pdbx/test_data/3a_no_chain_no_segid.pdb`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/pdbx/test_data/3aa.pdb` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/pdbx/test_data/3aa.pdb`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/pdbx/test_data/3aa11_13.pdb` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/pdbx/test_data/3aa11_13.pdb`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/pdbx/test_data/test_header_entry.txt` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/pdbx/test_data/test_header_entry.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/pdbx/test_sequence.py` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/pdbx/test_sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/shifts/test_make_peaks.py` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/shifts/test_make_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/shifty/test_export_shifts.py` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/shifty/test_export_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/sparky/test_data/P3a_L273R_sequence_short.neff` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/sparky/test_data/P3a_L273R_sequence_short.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/sparky/test_data/peaks_short_with_assignments.neff` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/sparky/test_data/peaks_short_with_assignments.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/sparky/test_data/sparky_manual_basic_sequence.nef` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/sparky/test_data/sparky_manual_basic_sequence.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/sparky/test_data/test_shifts_P3a_L273R_shifts_short.txt` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/sparky/test_data/test_shifts_P3a_L273R_shifts_short.txt`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short.neff` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_chains.neff` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_chains.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_different_residues.neff` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_different_residues.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_i_minus_one.neff` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_i_minus_one.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_overlapping_chains.neff` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/sparky/test_data/ubi_peaks_short_overlapping_chains.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/sparky/test_export_peaks.py` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/sparky/test_export_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/sparky/test_import_peaks.py` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/sparky/test_import_peaks.py`

 * *Files 4% similar despite different names*

```diff
@@ -51,26 +51,30 @@
 
     data_sequence = open(
         path_in_test_data(__file__, "sparky_manual_basic_sequence.nef")
     ).read()
 
     result = run_and_report(app, ["--molecule-type", "dna", path], input=data_sequence)
 
-    loop = isolate_loop(result.stdout, "sparky_sparky_manual_basic", "nef_peak")
+    loop = isolate_loop(
+        result.stdout, "nef_nmr_spectrum_sparky_sparky_manual_basic", "nef_peak"
+    )
 
     assert_lines_match(EXPECTED, str(loop))
 
 
 def test_basic_no_sequence():
 
     path = path_in_test_data(__file__, "sparky_manual_basic.peaks")
 
     result = run_and_report(app, ["--molecule-type", "dna", path])
 
-    loop = isolate_loop(result.stdout, "sparky_sparky_manual_basic", "nef_peak")
+    loop = isolate_loop(
+        result.stdout, "nef_nmr_spectrum_sparky_sparky_manual_basic", "nef_peak"
+    )
 
     assert_lines_match(EXPECTED, str(loop))
 
 
 def test_basic_no_sequence_requires_sequence():
 
     path = path_in_test_data(__file__, "sparky_manual_full_no_sequence.peaks")
@@ -78,27 +82,31 @@
     sequence = open(
         path_in_test_data(__file__, "sparky_manual_basic_sequence.nef")
     ).read()
 
     result = run_and_report(app, [path], input=sequence)
 
     loop = isolate_loop(
-        result.stdout, "sparky_sparky_manual_full_no_sequence", "nef_peak"
+        result.stdout,
+        "nef_nmr_spectrum_sparky_sparky_manual_full_no_sequence",
+        "nef_peak",
     )
 
     assert_lines_match(EXPECTED, str(loop))
 
 
 def test_full():
 
     path = path_in_test_data(__file__, "sparky_manual_full.peaks")
 
     result = run_and_report(app, ["--molecule-type", "dna", path])
 
-    loop = isolate_loop(result.stdout, "sparky_sparky_manual_full", "nef_peak")
+    loop = isolate_loop(
+        result.stdout, "nef_nmr_spectrum_sparky_sparky_manual_full", "nef_peak"
+    )
 
     assert_lines_match(EXPECTED, str(loop))
 
 
 EXPECTED_FULL_COMMENT = """ # noqa: E501
 loop_
   _nef_peak.index
@@ -133,10 +141,12 @@
 
 def test_full_comment():
 
     path = path_in_test_data(__file__, "sparky_manual_full_comment.peaks")
 
     result = run_and_report(app, ["--molecule-type", "dna", path])
 
-    loop = isolate_loop(result.stdout, "sparky_sparky_manual_full_comment", "nef_peak")
+    loop = isolate_loop(
+        result.stdout, "nef_nmr_spectrum_sparky_sparky_manual_full_comment", "nef_peak"
+    )
 
     assert_lines_match(EXPECTED_FULL_COMMENT, str(loop))
```

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/sparky/test_import_sequence.py` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/sparky/test_import_sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/sparky/test_import_shifts.py` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/sparky/test_import_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/sparky/test_sparky_lib.py` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/sparky/test_sparky_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/test_data/3a_ab.neff` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/test_data/3a_ab.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/test_data/header.nef` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/test_data/header.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/test_data/multi_chain.nef` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/test_data/multi_chain.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/test_data/nef_3_peaks.nef` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/test_data/nef_3_peaks.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/test_data/tailin_seq_short.nef` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/test_data/tailin_seq_short.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/test_data/test_agv.neff` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/test_data/test_agv.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/test_data/ubiquitin_short.nef` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/test_data/ubiquitin_short.nef`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/test_header.py` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/test_header.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/test_nef_lib.py` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/test_nef_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/test_sequence_lib.py` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/test_sequence_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/test_test.py` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/test_test.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/xcamshift/test_export_shifts.py` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/xcamshift/test_export_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/xplor/test_data/3a_ab.psf` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/xplor/test_data/3a_ab.psf`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/xplor/test_data/3a_ab_rdcs.neff` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/xplor/test_data/3a_ab_rdcs.neff`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals.tbl` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals.tbl`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals_bad.tbl` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/xplor/test_data/test_2_dihedrals_bad.tbl`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/xplor/test_dihedrals.py` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/xplor/test_dihedrals.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/xplor/test_distances.py` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/xplor/test_distances.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/xplor/test_export_rdcs.py` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/xplor/test_export_rdcs.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/xplor/test_import_sequence.py` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/xplor/test_import_sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/xplor/test_psf_lib.py` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/xplor/test_psf_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tests/xplor/test_xplor_lib.py` & `nef_pipelines-0.1.41/src/nef_pipelines/tests/xplor/test_xplor_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tools/about.py` & `nef_pipelines-0.1.41/src/nef_pipelines/tools/about.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tools/chains/__init__.py` & `nef_pipelines-0.1.41/src/nef_pipelines/tools/chains/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tools/chains/clone.py` & `nef_pipelines-0.1.41/src/nef_pipelines/tools/chains/clone.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tools/chains/list.py` & `nef_pipelines-0.1.41/src/nef_pipelines/tools/chains/list.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tools/chains/rename.py` & `nef_pipelines-0.1.41/src/nef_pipelines/tools/chains/rename.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tools/chains/renumber.py` & `nef_pipelines-0.1.41/src/nef_pipelines/tools/chains/renumber.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tools/entry/rename.py` & `nef_pipelines-0.1.41/src/nef_pipelines/tools/entry/rename.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tools/frames/__init__.py` & `nef_pipelines-0.1.41/src/nef_pipelines/tools/frames/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tools/frames/delete.py` & `nef_pipelines-0.1.41/src/nef_pipelines/tools/frames/delete.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tools/frames/insert.py` & `nef_pipelines-0.1.41/src/nef_pipelines/tools/frames/insert.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tools/frames/list.py` & `nef_pipelines-0.1.41/src/nef_pipelines/tools/frames/list.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tools/frames/rename.py` & `nef_pipelines-0.1.41/src/nef_pipelines/tools/frames/rename.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tools/frames/tabulate.py` & `nef_pipelines-0.1.41/src/nef_pipelines/tools/frames/tabulate.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tools/header.py` & `nef_pipelines-0.1.41/src/nef_pipelines/tools/header.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tools/offset_shifts.py` & `nef_pipelines-0.1.41/src/nef_pipelines/tools/offset_shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tools/peaks/match.py` & `nef_pipelines-0.1.41/src/nef_pipelines/tools/peaks/match.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tools/res_assign.py_unused` & `nef_pipelines-0.1.41/src/nef_pipelines/tools/res_assign.py_unused`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tools/shifts/make_peaks.py` & `nef_pipelines-0.1.41/src/nef_pipelines/tools/shifts/make_peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/tools/test.py` & `nef_pipelines-0.1.41/src/nef_pipelines/tools/test.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/transcoders/csv/importers/rdcs.py` & `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/csv/importers/rdcs.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/transcoders/echidna/importers/peaks.py` & `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/echidna/importers/peaks.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from pathlib import Path
 from typing import Iterator, List
 
 import typer
 from fyeah import f
 from pynmrstar import Saveframe
 
+from nef_pipelines.lib.nef_frames_lib import SPECTRUM_FRAME_CATEGORY
 from nef_pipelines.lib.nef_lib import (
     UNUSED,
     extract_column,
     read_or_create_entry_exit_error_on_bad_file,
     set_column,
     set_column_to_value,
 )
@@ -294,15 +295,15 @@
     function to calculate a merit value from an echidna error value, the error value is provided as the parameter x
 """
 
 
 @import_app.command(no_args_is_help=True)
 def peaks(
     frame_name: str = typer.Option(
-        "nef_nmr_spectrum_{file_name}",
+        "{file_name}",
         "-f",
         "--frame-name",
         help="a templated name for the frame {file_name} will be replaced by input filename without its extension",
     ),
     input: Path = typer.Option(
         STDIN,
         "-i",
@@ -397,15 +398,18 @@
             sequence,
             input_dimensions,
             spectrometer_frequency,
             molecule_type=molecule_type,
         )
 
         file_name = file_name.stem  # used by f()
-        frame = entry.get_saveframe_by_name(f(frame_name_template))
+
+        frame_code = f"{SPECTRUM_FRAME_CATEGORY}_{f(frame_name_template)}"
+
+        frame = entry.get_saveframe_by_name(frame_code)
 
         frame_name = file_name
 
         loop = frame.get_loop(NEF_PEAK)
         loop.add_tag(CCPN_MERIT, update_data=True)
 
         comment_values = _remove_and_store_comments(loop)
```

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/transcoders/fasta/__init__.py` & `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/fasta/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/transcoders/fasta/exporters/sequence.py` & `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/fasta/exporters/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/transcoders/fasta/importers/sequence.py` & `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/fasta/importers/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/transcoders/mars/__init__.py` & `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/nmrpipe/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,21 @@
 import typer
 
+import nef_pipelines
 from nef_pipelines import nef_app
 
 app = typer.Typer()
-export_app = typer.Typer()
 import_app = typer.Typer()
 
 if nef_app.app:
-
-    nef_app.app.add_typer(app, name="mars", help="- export mars [shifts and sequences]")
+    nef_app.app.add_typer(
+        app, name="nmrpipe", help="-  read nmrpipe [peaks shifts & sequencess]"
+    )
 
     app.add_typer(
-        export_app, name="export", help="- export mars [shifts and sequences]"
+        import_app, name="import", help="-  import nmrpipe [peaks, shifts & sequences]"
     )
 
-    nef_app.app.add_typer(app, name="mars", help="- import mars [shifts]")
-
-    app.add_typer(import_app, name="import", help="- import mars [shifts]")
-
     # import of specific importers must be after app creation to avoid circular imports
-    import nef_pipelines.transcoders.mars.exporters.fragments  # noqa: F401
-    import nef_pipelines.transcoders.mars.exporters.input  # noqa: F401
-    import nef_pipelines.transcoders.mars.exporters.sequence  # noqa: F401
-    import nef_pipelines.transcoders.mars.exporters.shifts  # noqa: F401
-    import nef_pipelines.transcoders.mars.importers.shifts  # noqa: F401
+    import nef_pipelines.transcoders.nmrpipe.importers.peaks  # noqa: F401
+    import nef_pipelines.transcoders.nmrpipe.importers.sequence  # noqa: F401
+    import nef_pipelines.transcoders.nmrpipe.importers.shifts  # noqa: F401
```

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/transcoders/mars/exporters/fragments.py` & `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/mars/exporters/fragments.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/transcoders/mars/exporters/input.py` & `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/mars/exporters/input.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/transcoders/mars/exporters/sequence.py` & `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/mars/exporters/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/transcoders/mars/exporters/shifts.py` & `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/mars/exporters/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/transcoders/mars/importers/shifts.py` & `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/mars/importers/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/transcoders/nmrpipe/__init__.py` & `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/rpf/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 import typer
 
-import nef_pipelines
 from nef_pipelines import nef_app
 
 app = typer.Typer()
-import_app = typer.Typer()
+# import_app = typer.Typer()
+export_app = typer.Typer()
 
 if nef_app.app:
-    nef_app.app.add_typer(
-        app, name="nmrpipe", help="-  read nmrpipe [peaks shifts & sequencess]"
-    )
-
-    app.add_typer(
-        import_app, name="import", help="-  import nmrpipe [peaks, shifts & sequences]"
-    )
+
+    nef_app.app.add_typer(app, name="rpf", help="-  write rpf shifts")
+
+    # app.add_typer(import_app, name="import", help="- import fasta sequences")
+    app.add_typer(export_app, name="export", help="- export rpf shifts")
 
     # import of specific importers must be after app creation to avoid circular imports
-    import nef_pipelines.transcoders.nmrpipe.importers.peaks  # noqa: F401
-    import nef_pipelines.transcoders.nmrpipe.importers.sequence  # noqa: F401
-    import nef_pipelines.transcoders.nmrpipe.importers.shifts  # noqa: F401
+    import nef_pipelines.transcoders.rpf.exporters.shifts  # noqa: F401
+
+    # import nef_pipelines.transcoders.fasta.importers.sequence  # noqa: F401
```

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/transcoders/nmrpipe/importers/peaks.py` & `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/nmrpipe/importers/peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/transcoders/nmrpipe/importers/sequence.py` & `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/nmrpipe/importers/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/transcoders/nmrpipe/importers/shifts.py` & `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/nmrpipe/importers/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/transcoders/nmrpipe/nmrpipe_lib.py` & `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/nmrpipe/nmrpipe_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/transcoders/nmrview/__init__.py` & `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/nmrview/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/transcoders/nmrview/exporters/peaks.py` & `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/nmrview/exporters/peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/transcoders/nmrview/exporters/sequences.py` & `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/nmrview/exporters/sequences.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/transcoders/nmrview/exporters/shifts.py` & `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/nmrview/exporters/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/transcoders/nmrview/importers/peaks.py` & `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/nmrview/importers/peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/transcoders/nmrview/importers/sequence.py` & `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/nmrview/importers/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/transcoders/nmrview/importers/shifts.py` & `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/nmrview/importers/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/transcoders/nmrview/nmrview_lib.py` & `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/nmrview/nmrview_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/transcoders/pales/__init__.py` & `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/pales/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/transcoders/pales/exporters/rdcs.py` & `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/pales/exporters/rdcs.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/transcoders/pales/exporters/template.py` & `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/pales/exporters/template.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/transcoders/pdbx/importers/sequence.py` & `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/pdbx/importers/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/transcoders/rpf/__init__.py` & `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/xeasy/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,23 @@
 import typer
 
 from nef_pipelines import nef_app
 
 app = typer.Typer()
-# import_app = typer.Typer()
-export_app = typer.Typer()
+import_app = typer.Typer()
+# export_app = typer.Typer()
+
 
 if nef_app.app:
 
-    nef_app.app.add_typer(app, name="rpf", help="-  write rpf shifts")
+    nef_app.app.add_typer(
+        app,
+        name="xeasy",
+        help="-  read xeasy files [flya dialect: sequence]",
+    )
 
-    # app.add_typer(import_app, name="import", help="- import fasta sequences")
-    app.add_typer(export_app, name="export", help="- export rpf shifts")
+    app.add_typer(import_app, name="import", help="-  import xeasy [sequence]")
 
     # import of specific importers must be after app creation to avoid circular imports
-    import nef_pipelines.transcoders.rpf.exporters.shifts  # noqa: F401
-
-    # import nef_pipelines.transcoders.fasta.importers.sequence  # noqa: F401
+    import nef_pipelines.transcoders.xeasy.importers.peaks  # noqa: F401
+    import nef_pipelines.transcoders.xeasy.importers.sequence  # noqa: F401
+    import nef_pipelines.transcoders.xeasy.importers.shifts  # noqa: F401
```

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/transcoders/rpf/exporters/shifts.py` & `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/rpf/exporters/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/transcoders/shifty/__init__.py` & `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/shifty/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/transcoders/shifty/exporters/shifts.py` & `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/shifty/exporters/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/transcoders/sparky/__init__.py` & `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/sparky/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/transcoders/sparky/exporters/peaks.py` & `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/sparky/exporters/peaks.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/transcoders/sparky/importers/peaks.py` & `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/sparky/importers/peaks.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,21 +82,21 @@
         help="default chain code to use if none is provided in the file",
     ),
     molecule_type: MoleculeTypes = typer.Option(
         MoleculeTypes.PROTEIN, help="the type of molecule"
     ),
     no_validate: bool = typer.Option(
         False,
-        help="if set don't validate the peaks agains the inpuy sequence if provided",
+        help="if set don't validate the peaks against the input sequence if provided",
     ),
     spectrometer_frequency: float = typer.Option(
         600.123456789, help="spectrometer frequency in MHz"
     ),
 ):
-    """convert sparky peaks file <SPARKY-PEAKS>.txt to NEF [alpha]"""
+    """convert sparky peaks file <SPARKY-PEAKS>.txt to NEF"""
 
     chain_codes = parse_comma_separated_options(chain_codes)
 
     if not chain_codes:
         chain_codes = ["A"]
 
     # make this a library function
@@ -141,15 +141,15 @@
     )
 
     print(entry)
 
 
 def pipe(
     entry,
-    frame_name,
+    frame_code_template,
     file_names_and_lines,
     chain_code,
     sequence,
     input_dimensions,
     spectrometer_frequency,
     molecule_type=MoleculeTypes.PROTEIN,
 ):
@@ -170,19 +170,21 @@
 
         dimensions = _guess_dimensions_if_not_defined_or_throw(
             sparky_peaks, input_dimensions
         )
 
         dimensions = [{"axis_code": dimension} for dimension in dimensions]
 
-        frame = peaks_to_frame(sparky_peaks, dimensions, spectrometer_frequency)
-
         file_name = Path(file_name).stem  # used in f method...
 
-        frame.name = f(frame_name)
+        frame_code = f(frame_code_template)
+
+        frame = peaks_to_frame(
+            sparky_peaks, dimensions, spectrometer_frequency, frame_code=frame_code
+        )
 
         sparky_frames.append(frame)
 
     return add_frames_to_entry(entry, sparky_frames)
 
 
 def parse_header_to_columns(header_line: str, file_name) -> Dict[str, int]:
```

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/transcoders/sparky/importers/sequence.py` & `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/sparky/importers/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/transcoders/sparky/importers/shifts.py` & `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/sparky/importers/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/transcoders/sparky/sparky_lib.py` & `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/sparky/sparky_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/transcoders/xcamshift/__init__.py` & `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/xcamshift/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/transcoders/xcamshift/exporters/shifts.py` & `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/xcamshift/exporters/shifts.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/transcoders/xeasy/xeasy_lib.py` & `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/xeasy/xeasy_lib.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,71 +1,68 @@
 import string
 from collections import OrderedDict
 from typing import Dict, Iterator, List, Tuple, Union
 
 from nef_pipelines.lib.isotope_lib import ATOM_TO_ISOTOPE
 from nef_pipelines.lib.nef_lib import UNUSED
-from nef_pipelines.lib.sequence_lib import (
-    get_residue_name_from_lookup,
-    sequence_to_residue_type_lookup,
-)
+from nef_pipelines.lib.sequence_lib import get_residue_name_from_lookup
 from nef_pipelines.lib.structures import (
     AtomLabel,
     DimensionInfo,
     LineInfo,
     NewPeak,
+    Residue,
     SequenceResidue,
     ShiftData,
 )
 from nef_pipelines.lib.util import (
     exit_error,
     is_float,
     is_int,
     strip_characters_right,
     strip_line_comment,
 )
 
 XEASY_PEAK_MAGIC = "FORMAT xeasy3D"
 
-test = """
-HIS     A1
-MET     A2
-ARG     A3
-GLN     A4
-PRO     A5
-PRO     A6
-LEU     A7
-VAL     A8
-THR     A9
-"""
-
 
 def line_info_iter(lines: Iterator[str], source="unknown") -> Iterator[LineInfo]:
     for line_no, line in enumerate(lines, start=1):
         line = line.strip()
 
         if len(line) == 0:
             continue
 
         yield LineInfo(source, line_no, line)
 
 
-def parse_xeasy_sequence(
-    lines: Iterator[str], source="unknown"
-) -> List[SequenceResidue]:
+def parse_sequence(lines: Iterator[str], source="unknown") -> List[SequenceResidue]:
     result = []
     for line_info in line_info_iter(lines, source):
 
+        if line_info.line_no == 1 and line_info.line.startswith("#"):
+            continue
+
         fields = line_info.line.split()
 
         exit_if_wrong_field_count_sequence(fields, line_info)
 
         residue_name, chain_seq_code = fields
 
-        sequence_code, chain_code = strip_characters_right(
+        if residue_name == "SS":
+            msg = f"""
+                Original xeasy sequences are not supported only those used by flya
+                at line {line_info.line_no} in file {line_info.file_name} if found a residue type SS
+                where as it must be a standard 3 letter amino acid code, the whole line was
+
+                {line_info.line}
+            """
+            exit_error(msg)
+
+        chain_code, sequence_code = strip_characters_right(
             chain_seq_code, string.digits
         )
 
         sequence_residue = SequenceResidue(chain_code, sequence_code, residue_name)
 
         result.append(sequence_residue)
 
@@ -163,15 +160,15 @@
 
             {line_info.line}
 
         """
         exit_error(msg)
     else:
         atom_name, chain_residue = fields
-        sequence_code, chain_code = strip_characters_right(chain_residue, string.digits)
+        chain_code, sequence_code = strip_characters_right(chain_residue, string.digits)
 
         residue_name = get_residue_name_from_lookup(
             chain_code, sequence_code, residue_lookup
         )
         _exit_if_no_residue_name_in_sequence(
             residue_name, chain_code, sequence_code, line_info
         )
@@ -196,27 +193,25 @@
                 {line_info.line}
             """
         exit_error(msg)
 
 
 def parse_peaks(
     lines: Iterator[str], source: str, residue_name_lookup: Dict[Union[str, int], str]
-) -> List[NewPeak]:
+) -> Tuple[str, List[DimensionInfo], List[NewPeak]]:
     have_magic = False
     number_dimensions = None
     experiment_type = None
     dimensions = OrderedDict()
 
     peaks = []
 
     for line_info in line_info_iter(lines, source):
 
-        shifts = []
-        assignments = []
-
+        shifts: list[float] = []
         if line_info.line.startswith("#"):
 
             stripped_line = line_info.line.lstrip("#").lstrip()
 
             if stripped_line.startswith(XEASY_PEAK_MAGIC):
                 have_magic = True
                 continue
@@ -248,16 +243,14 @@
                 if len(fields) > 1:
                     experiment_type = fields[1]
 
         else:
             _exit_if_no_magic_before_data(have_magic, line_info)
             line, comment = strip_line_comment(line_info.line)
 
-            current_column = 1
-            # print(f'{line}-{comment}')
             fields = line.split()
 
             serial = fields[0]
             _check_serial_is_integer_or_exit(serial, line_info)
             serial = int(serial)
             current_column = 1
 
@@ -281,46 +274,167 @@
             volume_error = float(volume_error)
             volume_error = volume * volume_error / 100.0
             current_column += 1
 
             # ignore the peak integration method
             current_column += 2
 
+            assignments = []
+
             for assignment_column_number in dimensions:
                 target_column = current_column + assignment_column_number
                 assignment = _parse_xeasy_assignment(
                     fields[target_column], residue_name_lookup, line_info
                 )
                 assignments.append(assignment)
 
-            shift_data = []
-            for assignment, shift in zip(assignments, shifts):
-                shift_data.append(ShiftData(assignment, shift))
-
+            shift_data = [
+                ShiftData(assignment, shift)
+                for assignment, shift in zip(assignments, shifts)
+            ]
             peak = NewPeak(
                 shifts=shift_data,
                 id=serial,
                 volume=volume,
                 volume_uncertainty=volume_error,
                 comment=comment,
             )
+
             peaks.append(peak)
 
     dimension_names = [
         dimensions[dimension_index] for dimension_index in sorted(dimensions)
     ]
     axis_codes = [
         ATOM_TO_ISOTOPE[dimension_name[0]] for dimension_name in dimension_names
     ]
     dimension_info = [
         DimensionInfo(axis_code, dimension_name)
         for axis_code, dimension_name in zip(axis_codes, dimension_names)
     ]
 
-    return experiment_type, dimension_info, tuple(axis_codes), peaks
+    return experiment_type, dimension_info, peaks
+
+
+# 3.4.2 Atom List
+#
+# The atom list contains the names and frequencies of resonances. They define the possible assignments for
+# each dimension of a peak.
+#
+# Table 3.4.2.A - Atom Fields
+#
+# Fields              Description
+#
+# atom number         unique number identifying the atom
+# shift               mean chemical shift in ppm
+# shift error         deviation of the assigned peaks from the mean value
+# name                atom name
+# fragment number     number of the fragment to which the atom belongs
+# lineshapes          data structure containing the reference lineshapes
+#
+#
+# The fields listed in Table 3.4.2.A constitute an atom entry. They can be modified in the peak editing
+# window. The atom numbers, used to reference the atoms, must be unique but not necessarily continuous.
+# The number -9999 is reserved to denote invalid entries. The average chemical shift and the shift error can
+# be calculated from the assigned peaks. The command is "Average chem. shift [ac]".
+#
+# If the chemical shift is not defined it is set to the value 999.000.
+#
+# A new atom list is generated each time when a fragment list is loaded. For each fragment the
+# corresponding atoms are looked up in the fragment library file and added to the list. New atom entries are
+# added to the atom list if a non existing atom is used with the "Assign peak [ap]" command, if the fragment
+# type is changed in the peak editing window, or with the "Add new fragment [af]" command.
+#
+# The atom list file has the extension ".prot" originating from the old EASY format. The following line is
+# taken from such a file:
+#
+# 32   4.370  0.004   HA  2
+#
+# The first number is the atom number, followed by its mean chemical shift and the deviation from the
+# mean value. The atom name and the fragment number follow. The commands to read or write an atom list
+# are "Load atoms (chem. shift) [lc]" and "Write atoms (chem. shift) [wc]".
+
+
+def parse_shifts(
+    lines: Iterator[str], source: str, residue_lookup: Dict[Union[str, int], str]
+):
+    shifts = []
+    for line_no, line in enumerate(lines, start=1):
+
+        line_info = LineInfo(source, line_no, line.strip())
+
+        if len(line_info.line) == 0:
+            continue
+
+        fields = line_info.line.split()
+
+        _check_number_fields_correct_or_exit(fields, line_info)
+
+        column = 1
+        serial = fields[column - 1]
+        _check_serial_is_integer_or_exit(serial, line_info)
+
+        column += 1
+        shift = fields[column - 1]
+        _check_fields_is_float_or_exit(shift, column, line_info)
+
+        column += 1
+        shift_error = fields[column - 1]
+        _check_fields_is_float_or_exit(shift_error, column, line_info)
+
+        column += 1
+        atom_name = fields[column - 1]
+
+        column += 1
+        chain_residue = fields[column - 1]
+        chain_code, sequence_code = strip_characters_right(chain_residue, string.digits)
+
+        residue_name = get_residue_name_from_lookup(
+            chain_code, sequence_code, residue_lookup
+        )
+        _exit_if_no_residue_name_in_sequence(
+            residue_name, chain_code, sequence_code, line_info
+        )
+
+        residue = Residue(chain_code, sequence_code, residue_name)
+        atom = AtomLabel(residue, atom_name)
+
+        shift = ShiftData(atom=atom, value=shift, value_uncertainty=shift_error)
+
+        shifts.append(shift)
+
+    return shifts
+
+
+def _check_fields_is_float_or_exit(value, column, line_info):
+    if not is_float(value):
+        msg = f"""
+                column {column} of {line_info.file_name} at line {line_info.line_no} should be a floating point
+                 number I got {value}, the line was
+
+                {line_info.line}
+            """
+        exit_error(msg)
+
+
+def _check_number_fields_correct_or_exit(fields, line_info):
+
+    num_fields = len(fields)
+    if num_fields != 5:
+        msg = f"""
+                in the file {line_info.file_name} at line {line_info.line_no} I expected 5 fields but got {num_fields}
+                the line was
+
+                {line_info}
+
+                i expected something like
+
+                32 4.370 0.004 HA A2
+            """
+        exit_error(msg)
 
 
 def _exit_if_no_magic_before_data(have_magic, line_info):
     if not have_magic:
         msg = f"""
                     Xeasy files should have the line #{XEASY_PEAK_MAGIC} before any data is read
                     at line {line_info.line_no} in file {line_info.file_name} i appear to have data
@@ -335,18 +449,18 @@
     msg = None
     if not is_float(volume_error):
         msg = f"""
             the volume error column (column {column_number}) should be a floating point number
             i got {volume_error} in the file {line_info.file_name} at line {line_info.line_no} the value of the
             line was
 
-            {line_info_iter.line}
+            {line_info.line}
         """
     volume_error = float(volume_error)
-    if not (volume_error <= 100.0 and volume_error >= 0.0):
+    if not (100.0 >= volume_error >= 0.0):
         msg = f"""
             the volume error column (column {column_number}) should be a nunber between 0.0 and 100.0 i got
             {volume_error} in the file {line_info.file_name} at line {line_info.line_no} the value of the line was
 
             {line_info.line}
         """
 
@@ -356,34 +470,34 @@
 
 def _check_volume_is_float_or_exit(volume, column_number, line_info):
     if not is_float(volume):
         msg = f"""
             the volume column (column {column_number}) should be a floating point number i got {volume}
             in the file {line_info.file_name} at line {line_info.line_no} the value of the line was
 
-            {line_info_iter.line}
+            {line_info.line}
         """
         exit_error(msg)
 
 
 def _check_shift_is_float_or_exit(shift, column_number, line_info):
     if not is_float(shift):
         msg = f"""
                 chemical shift fields should be floating point numbers i got {shift} at column number {column_number}
                 in the file {line_info.file_name} at line {line_info.line_no} the value of the line was
 
-                {line_info_iter.line}
+                {line_info.line}
                     """
         exit_error(msg)
 
 
 def _check_serial_is_integer_or_exit(serial, line_info):
     if not is_int(serial):
         msg = f"""
-            the first field of a xeasy peak list should be an integer serial number i got: {serial}
+            the first field of a xeasy peak or shift  list should be an integer serial number i got: {serial}
             in file {line_info.file_name} at line {line_info.line_no}, the line was:
 
             {line_info.line}
         """
         exit_error(msg)
 
 
@@ -419,15 +533,15 @@
                         I got {number_dimensions} at line {line_info.line_no} the value for the line was
                         {line_info.line}
                     """
         exit_error(msg)
 
 
 def _check_for_peaks_magic_or_exit(line_info):
-    if not line_info.line == (XEASY_PEAK_MAGIC):
+    if line_info.line != XEASY_PEAK_MAGIC:
         msg = f"""
                     an xeasy peak files should start with {XEASY_PEAK_MAGIC} but i got:
 
                     {line_info.line}
 
                     at line {line_info.line_no} in {line_info.file_name}
                 """
@@ -452,17 +566,7 @@
                 in file {line_info.file_name} at line {line_info.line_no} there should be 2 columns i got {len(fields)}
                 the line should be of the form 'HIS A1' [<RESIDUE-NAME> <CHAIN-RESIDUE-NUMBER>] but was
 
                 {line_info.line}
             """
 
         exit_error(msg)
-
-
-if __name__ == "__main__":
-    sequence = parse_xeasy_sequence(test.split("\n"))
-
-    residue_name_lookup = sequence_to_residue_type_lookup(sequence)
-
-    peaks = parse_peaks(test_peaks.split("\n"), "wibble", residue_name_lookup)
-
-    print(peaks)
```

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/transcoders/xplor/__init__.py` & `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/xplor/__init__.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/transcoders/xplor/exporters/rdcs.py` & `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/xplor/exporters/rdcs.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/transcoders/xplor/importers/dihedrals.py` & `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/xplor/importers/dihedrals.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/transcoders/xplor/importers/distances.py` & `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/xplor/importers/distances.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/transcoders/xplor/importers/sequence.py` & `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/xplor/importers/sequence.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/transcoders/xplor/psf_lib.py` & `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/xplor/psf_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines/transcoders/xplor/xplor_lib.py` & `nef_pipelines-0.1.41/src/nef_pipelines/transcoders/xplor/xplor_lib.py`

 * *Files identical despite different names*

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines.egg-info/PKG-INFO` & `nef_pipelines-0.1.41/src/nef_pipelines.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nef-pipelines
-Version: 0.1.40
+Version: 0.1.41
 Summary: Tools for Manipulating NEF [NMR Exchange Format] Files and Foreign File Access
 Home-page: https://github.com/varioustoxins/NEF-Pipelines
 Author: varioustoxins
 Author-email: g.s.thompson@kent.ac.uk
 License: LGPL-2.1
 Project-URL: Documentation, https://pyscaffold.org/
 Platform: any
```

### Comparing `nef_pipelines-0.1.40/src/nef_pipelines.egg-info/SOURCES.txt` & `nef_pipelines-0.1.41/src/nef_pipelines.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -52,14 +52,15 @@
 src/nef_pipelines/lib/translation/__init__.py
 src/nef_pipelines/nef_app/__init__.py
 src/nef_pipelines/tests/conftest.py
 src/nef_pipelines/tests/test_header.py
 src/nef_pipelines/tests/test_nef_lib.py
 src/nef_pipelines/tests/test_sequence_lib.py
 src/nef_pipelines/tests/test_test.py
+src/nef_pipelines/tests/test_util.py
 src/nef_pipelines/tests/chains/__init__.py
 src/nef_pipelines/tests/chains/test_clone.py
 src/nef_pipelines/tests/chains/test_list.py
 src/nef_pipelines/tests/chains/test_rename.py
 src/nef_pipelines/tests/chains/test_renumber.py
 src/nef_pipelines/tests/chains/test_data/3aa.nef
 src/nef_pipelines/tests/chains/test_data/3aa_x3.nef
@@ -169,14 +170,22 @@
 src/nef_pipelines/tests/test_data/header.nef
 src/nef_pipelines/tests/test_data/multi_chain.nef
 src/nef_pipelines/tests/test_data/nef_3_peaks.nef
 src/nef_pipelines/tests/test_data/tailin_seq_short.nef
 src/nef_pipelines/tests/test_data/test_agv.neff
 src/nef_pipelines/tests/test_data/ubiquitin_short.nef
 src/nef_pipelines/tests/xcamshift/test_export_shifts.py
+src/nef_pipelines/tests/xeasy/__init__.py
+src/nef_pipelines/tests/xeasy/test_import_peaks.py
+src/nef_pipelines/tests/xeasy/test_import_sequence.py
+src/nef_pipelines/tests/xeasy/test_import_shifts.py
+src/nef_pipelines/tests/xeasy/test_xeasy_lib.py
+src/nef_pipelines/tests/xeasy/test_data/basic.peaks
+src/nef_pipelines/tests/xeasy/test_data/basic.seq
+src/nef_pipelines/tests/xeasy/test_data/basic_sequence.nef
 src/nef_pipelines/tests/xplor/test_dihedrals.py
 src/nef_pipelines/tests/xplor/test_distances.py
 src/nef_pipelines/tests/xplor/test_export_rdcs.py
 src/nef_pipelines/tests/xplor/test_import_sequence.py
 src/nef_pipelines/tests/xplor/test_psf_lib.py
 src/nef_pipelines/tests/xplor/test_xplor_lib.py
 src/nef_pipelines/tests/xplor/test_data/3a_ab.psf
@@ -270,15 +279,19 @@
 src/nef_pipelines/transcoders/sparky/importers/__init__.py
 src/nef_pipelines/transcoders/sparky/importers/peaks.py
 src/nef_pipelines/transcoders/sparky/importers/sequence.py
 src/nef_pipelines/transcoders/sparky/importers/shifts.py
 src/nef_pipelines/transcoders/xcamshift/__init__.py
 src/nef_pipelines/transcoders/xcamshift/exporters/__init__.py
 src/nef_pipelines/transcoders/xcamshift/exporters/shifts.py
+src/nef_pipelines/transcoders/xeasy/__init__.py
 src/nef_pipelines/transcoders/xeasy/xeasy_lib.py
+src/nef_pipelines/transcoders/xeasy/importers/peaks.py
+src/nef_pipelines/transcoders/xeasy/importers/sequence.py
+src/nef_pipelines/transcoders/xeasy/importers/shifts.py
 src/nef_pipelines/transcoders/xplor/__init__.py
 src/nef_pipelines/transcoders/xplor/psf_lib.py
 src/nef_pipelines/transcoders/xplor/xplor_lib.py
 src/nef_pipelines/transcoders/xplor/exporters/__init__.py
 src/nef_pipelines/transcoders/xplor/exporters/rdcs.py
 src/nef_pipelines/transcoders/xplor/importers/__init__.py
 src/nef_pipelines/transcoders/xplor/importers/dihedrals.py
```

### Comparing `nef_pipelines-0.1.40/tox.ini` & `nef_pipelines-0.1.41/tox.ini`

 * *Files identical despite different names*

