# Comparing `tmp/gb2seq-0.2.4.tar.gz` & `tmp/gb2seq-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gb2seq-0.2.4.tar", last modified: Mon Jan 16 13:34:26 2023, max compression
+gzip compressed data, was "gb2seq-0.2.5.tar", last modified: Sun May 21 12:43:18 2023, max compression
```

## Comparing `gb2seq-0.2.4.tar` & `gb2seq-0.2.5.tar`

### file list

```diff
@@ -1,38 +1,46 @@
-drwxrwxr-x   0 terry      (501) staff       (20)        0 2023-01-16 13:34:26.600740 gb2seq-0.2.4/
--rw-rw-r--   0 terry      (501) staff       (20)       82 2022-08-03 22:54:17.000000 gb2seq-0.2.4/AUTHORS
--rw-rw-r--   0 terry      (501) staff       (20)      955 2023-01-16 13:34:26.599973 gb2seq-0.2.4/PKG-INFO
--rw-rw-r--   0 terry      (501) staff       (20)    23553 2023-01-16 13:33:54.000000 gb2seq-0.2.4/README.md
-drwxrwxr-x   0 terry      (501) staff       (20)        0 2023-01-16 13:34:26.586880 gb2seq-0.2.4/bin/
--rwxrwxr-x   0 terry      (501) staff       (20)     1933 2022-08-04 07:08:53.000000 gb2seq-0.2.4/bin/annotate-genome.py
--rwxrwxr-x   0 terry      (501) staff       (20)     7015 2023-01-16 13:33:54.000000 gb2seq-0.2.4/bin/describe-feature.py
--rwxrwxr-x   0 terry      (501) staff       (20)    15354 2022-09-12 20:04:04.000000 gb2seq-0.2.4/bin/describe-genome.py
--rwxrwxr-x   0 terry      (501) staff       (20)     5766 2023-01-16 13:33:54.000000 gb2seq-0.2.4/bin/describe-site.py
-drwxrwxr-x   0 terry      (501) staff       (20)        0 2023-01-16 13:34:26.590371 gb2seq-0.2.4/gb2seq/
--rw-rw-r--   0 terry      (501) staff       (20)      169 2023-01-16 13:33:54.000000 gb2seq-0.2.4/gb2seq/__init__.py
--rw-rw-r--   0 terry      (501) staff       (20)    41604 2023-01-16 13:33:54.000000 gb2seq-0.2.4/gb2seq/alignment.py
--rw-rw-r--   0 terry      (501) staff       (20)     7745 2022-11-27 10:10:32.000000 gb2seq-0.2.4/gb2seq/annotate.py
--rw-rw-r--   0 terry      (501) staff       (20)     1701 2022-08-03 22:54:17.000000 gb2seq-0.2.4/gb2seq/change.py
--rw-rw-r--   0 terry      (501) staff       (20)     1961 2022-08-03 22:54:17.000000 gb2seq-0.2.4/gb2seq/checker.py
--rw-rw-r--   0 terry      (501) staff       (20)    27103 2023-01-16 13:33:54.000000 gb2seq-0.2.4/gb2seq/features.py
--rw-rw-r--   0 terry      (501) staff       (20)      558 2022-08-03 22:54:17.000000 gb2seq-0.2.4/gb2seq/genome.py
--rw-rw-r--   0 terry      (501) staff       (20)     2457 2022-11-27 10:14:28.000000 gb2seq-0.2.4/gb2seq/sars2.py
--rw-rw-r--   0 terry      (501) staff       (20)    20495 2023-01-16 13:33:54.000000 gb2seq-0.2.4/gb2seq/translate.py
--rw-rw-r--   0 terry      (501) staff       (20)     2049 2022-08-03 22:56:02.000000 gb2seq-0.2.4/gb2seq/variants.py
-drwxrwxr-x   0 terry      (501) staff       (20)        0 2023-01-16 13:34:26.591911 gb2seq-0.2.4/gb2seq.egg-info/
--rw-rw-r--   0 terry      (501) staff       (20)      955 2023-01-16 13:34:25.000000 gb2seq-0.2.4/gb2seq.egg-info/PKG-INFO
--rw-rw-r--   0 terry      (501) staff       (20)      636 2023-01-16 13:34:26.000000 gb2seq-0.2.4/gb2seq.egg-info/SOURCES.txt
--rw-rw-r--   0 terry      (501) staff       (20)        1 2023-01-16 13:34:26.000000 gb2seq-0.2.4/gb2seq.egg-info/dependency_links.txt
--rw-rw-r--   0 terry      (501) staff       (20)       20 2023-01-16 13:34:26.000000 gb2seq-0.2.4/gb2seq.egg-info/requires.txt
--rw-rw-r--   0 terry      (501) staff       (20)        7 2023-01-16 13:34:26.000000 gb2seq-0.2.4/gb2seq.egg-info/top_level.txt
--rw-rw-r--   0 terry      (501) staff       (20)       30 2022-08-03 22:54:17.000000 gb2seq-0.2.4/pyproject.toml
--rw-rw-r--   0 terry      (501) staff       (20)       38 2023-01-16 13:34:26.601057 gb2seq-0.2.4/setup.cfg
--rw-rw-r--   0 terry      (501) staff       (20)     1793 2022-09-12 20:46:46.000000 gb2seq-0.2.4/setup.py
-drwxrwxr-x   0 terry      (501) staff       (20)        0 2023-01-16 13:34:26.598531 gb2seq-0.2.4/test/
--rw-rw-r--   0 terry      (501) staff       (20)    64269 2023-01-16 13:33:54.000000 gb2seq-0.2.4/test/test_alignment.py
--rw-rw-r--   0 terry      (501) staff       (20)     1903 2022-08-03 23:06:40.000000 gb2seq-0.2.4/test/test_change.py
--rw-rw-r--   0 terry      (501) staff       (20)     5155 2022-08-04 09:52:00.000000 gb2seq-0.2.4/test/test_checker.py
--rw-rw-r--   0 terry      (501) staff       (20)    12860 2023-01-16 13:33:54.000000 gb2seq-0.2.4/test/test_features.py
--rw-rw-r--   0 terry      (501) staff       (20)    17184 2022-09-12 21:20:27.000000 gb2seq-0.2.4/test/test_genomes.py
--rw-rw-r--   0 terry      (501) staff       (20)      414 2022-08-03 23:08:39.000000 gb2seq-0.2.4/test/test_sars2.py
--rw-rw-r--   0 terry      (501) staff       (20)    21036 2022-09-12 21:30:21.000000 gb2seq-0.2.4/test/test_translate.py
--rw-rw-r--   0 terry      (501) staff       (20)     1141 2022-08-04 09:51:21.000000 gb2seq-0.2.4/test/test_variants.py
+drwxrwxr-x   0 terry      (501) staff       (20)        0 2023-05-21 12:43:18.053129 gb2seq-0.2.5/
+-rw-rw-r--   0 terry      (501) staff       (20)       82 2022-08-03 22:54:17.000000 gb2seq-0.2.5/AUTHORS
+-rw-rw-r--   0 terry      (501) staff       (20)       39 2023-05-20 21:53:46.000000 gb2seq-0.2.5/MANIFEST.in
+-rw-rw-r--   0 terry      (501) staff       (20)     1124 2023-05-21 12:43:18.052664 gb2seq-0.2.5/PKG-INFO
+-rw-rw-r--   0 terry      (501) staff       (20)    26579 2023-05-21 12:40:12.000000 gb2seq-0.2.5/README.md
+drwxrwxr-x   0 terry      (501) staff       (20)        0 2023-05-21 12:43:18.039235 gb2seq-0.2.5/bin/
+-rwxrwxr-x   0 terry      (501) staff       (20)     1933 2022-08-04 07:08:53.000000 gb2seq-0.2.5/bin/annotate-genome.py
+-rwxrwxr-x   0 terry      (501) staff       (20)     7257 2023-05-21 10:01:54.000000 gb2seq-0.2.5/bin/describe-feature.py
+-rwxrwxr-x   0 terry      (501) staff       (20)    15353 2023-05-20 07:09:01.000000 gb2seq-0.2.5/bin/describe-genome.py
+-rwxrwxr-x   0 terry      (501) staff       (20)     6171 2023-05-21 10:32:17.000000 gb2seq-0.2.5/bin/describe-site.py
+drwxrwxr-x   0 terry      (501) staff       (20)        0 2023-05-21 12:43:18.041384 gb2seq-0.2.5/data/
+-rw-rw-r--   0 terry      (501) staff       (20)    29907 2022-08-03 22:52:44.000000 gb2seq-0.2.5/data/BavPat2.fasta
+-rw-rw-r--   0 terry      (501) staff       (20)    29944 2022-08-03 22:52:44.000000 gb2seq-0.2.5/data/EPI_ISL_402125.fasta
+-rw-rw-r--   0 terry      (501) staff       (20)    29814 2022-08-03 22:52:44.000000 gb2seq-0.2.5/data/EPI_ISL_601443.fasta
+-rw-rw-r--   0 terry      (501) staff       (20)    29927 2022-08-03 22:52:44.000000 gb2seq-0.2.5/data/EPI_ISL_678597.fasta
+-rw-rw-r--   0 terry      (501) staff       (20)    30001 2022-08-03 22:52:44.000000 gb2seq-0.2.5/data/NC_045512.2.fasta
+-rw-rw-r--   0 terry      (501) staff       (20)    78471 2022-08-03 22:52:44.000000 gb2seq-0.2.5/data/NC_045512.2.gb
+drwxrwxr-x   0 terry      (501) staff       (20)        0 2023-05-21 12:43:18.045944 gb2seq-0.2.5/gb2seq/
+-rw-rw-r--   0 terry      (501) staff       (20)      170 2023-05-20 12:23:13.000000 gb2seq-0.2.5/gb2seq/__init__.py
+-rw-rw-r--   0 terry      (501) staff       (20)    41849 2023-05-21 12:40:54.000000 gb2seq-0.2.5/gb2seq/alignment.py
+-rw-rw-r--   0 terry      (501) staff       (20)     7745 2023-03-24 11:55:34.000000 gb2seq-0.2.5/gb2seq/annotate.py
+-rw-rw-r--   0 terry      (501) staff       (20)     1701 2022-08-03 22:54:17.000000 gb2seq-0.2.5/gb2seq/change.py
+-rw-rw-r--   0 terry      (501) staff       (20)     1961 2022-08-03 22:54:17.000000 gb2seq-0.2.5/gb2seq/checker.py
+-rw-rw-r--   0 terry      (501) staff       (20)    27096 2023-05-21 12:37:42.000000 gb2seq-0.2.5/gb2seq/features.py
+-rw-rw-r--   0 terry      (501) staff       (20)      558 2022-08-03 22:54:17.000000 gb2seq-0.2.5/gb2seq/genome.py
+-rw-rw-r--   0 terry      (501) staff       (20)     2457 2023-03-24 11:55:34.000000 gb2seq-0.2.5/gb2seq/sars2.py
+-rw-rw-r--   0 terry      (501) staff       (20)    20485 2023-05-21 07:41:44.000000 gb2seq-0.2.5/gb2seq/translate.py
+-rw-rw-r--   0 terry      (501) staff       (20)     2049 2022-08-03 22:56:02.000000 gb2seq-0.2.5/gb2seq/variants.py
+drwxrwxr-x   0 terry      (501) staff       (20)        0 2023-05-21 12:43:18.048165 gb2seq-0.2.5/gb2seq.egg-info/
+-rw-rw-r--   0 terry      (501) staff       (20)     1124 2023-05-21 12:43:17.000000 gb2seq-0.2.5/gb2seq.egg-info/PKG-INFO
+-rw-rw-r--   0 terry      (501) staff       (20)      788 2023-05-21 12:43:17.000000 gb2seq-0.2.5/gb2seq.egg-info/SOURCES.txt
+-rw-rw-r--   0 terry      (501) staff       (20)        1 2023-05-21 12:43:17.000000 gb2seq-0.2.5/gb2seq.egg-info/dependency_links.txt
+-rw-rw-r--   0 terry      (501) staff       (20)       20 2023-05-21 12:43:17.000000 gb2seq-0.2.5/gb2seq.egg-info/requires.txt
+-rw-rw-r--   0 terry      (501) staff       (20)        7 2023-05-21 12:43:17.000000 gb2seq-0.2.5/gb2seq.egg-info/top_level.txt
+-rw-rw-r--   0 terry      (501) staff       (20)      539 2023-05-20 13:31:27.000000 gb2seq-0.2.5/pyproject.toml
+-rw-rw-r--   0 terry      (501) staff       (20)       38 2023-05-21 12:43:18.053253 gb2seq-0.2.5/setup.cfg
+-rw-rw-r--   0 terry      (501) staff       (20)     2065 2023-05-21 10:43:53.000000 gb2seq-0.2.5/setup.py
+drwxrwxr-x   0 terry      (501) staff       (20)        0 2023-05-21 12:43:18.052090 gb2seq-0.2.5/test/
+-rw-rw-r--   0 terry      (501) staff       (20)    66769 2023-05-20 14:35:53.000000 gb2seq-0.2.5/test/test_alignment.py
+-rw-rw-r--   0 terry      (501) staff       (20)     1903 2022-08-03 23:06:40.000000 gb2seq-0.2.5/test/test_change.py
+-rw-rw-r--   0 terry      (501) staff       (20)     5155 2022-08-04 09:52:00.000000 gb2seq-0.2.5/test/test_checker.py
+-rw-rw-r--   0 terry      (501) staff       (20)    12860 2023-03-24 11:55:34.000000 gb2seq-0.2.5/test/test_features.py
+-rw-rw-r--   0 terry      (501) staff       (20)    17184 2022-09-12 21:20:27.000000 gb2seq-0.2.5/test/test_genomes.py
+-rw-rw-r--   0 terry      (501) staff       (20)      414 2022-08-03 23:08:39.000000 gb2seq-0.2.5/test/test_sars2.py
+-rw-rw-r--   0 terry      (501) staff       (20)    21028 2023-05-21 12:34:49.000000 gb2seq-0.2.5/test/test_translate.py
+-rw-rw-r--   0 terry      (501) staff       (20)     1141 2022-08-04 09:51:21.000000 gb2seq-0.2.5/test/test_variants.py
```

### Comparing `gb2seq-0.2.4/PKG-INFO` & `gb2seq-0.2.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: gb2seq
-Version: 0.2.4
-Summary: Python library and scripts for working with SARS-CoV-2 sequences.
+Version: 0.2.5
+Summary: Python library and scripts for working with unannotated sequences based on an annotated reference genome provided by a GenBank file.
 Home-page: https://github.com/virologycharite/gb2seq
 Download-URL: https://github.com/virologycharite/gb2seq
 Author: Terry C. Jones
 Author-email: terence.jones@charite.de
+Maintainer: Terry C. Jones
+Maintainer-email: terence.jones@charite.de
 License: MIT
 Keywords: GenBank,genetic sequences
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 License-File: AUTHORS
 
 See https://github.com/virologycharite/gb2seq for details.
-
```

### Comparing `gb2seq-0.2.4/README.md` & `gb2seq-0.2.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,1473 +1,1662 @@
 00000000: 2320 4120 5079 7468 6f6e 206c 6962 7261  # A Python libra
 00000010: 7279 2061 6e64 2063 6f6d 6d61 6e64 2d6c  ry and command-l
 00000020: 696e 6520 7363 7269 7074 7320 666f 7220  ine scripts for 
 00000030: 776f 726b 696e 6720 7769 7468 2047 656e  working with Gen
 00000040: 4261 6e6b 2067 656e 6f6d 6520 7365 7175  Bank genome sequ
 00000050: 656e 6365 7320 616e 6420 616e 6e6f 7461  ences and annota
 00000060: 7469 6f6e 730a 0a60 6762 3273 6571 6020  tions..`gb2seq` 
-00000070: 7072 6f76 6964 6573 2075 7469 6c69 7479  provides utility
-00000080: 2073 6372 6970 7473 2066 6f72 2065 7861   scripts for exa
-00000090: 6d69 6e69 6e67 2047 656e 4261 6e6b 2067  mining GenBank g
-000000a0: 656e 6f6d 6520 7365 7175 656e 6365 730a  enome sequences.
-000000b0: 616e 6420 7468 6569 7220 616e 6e6f 7461  and their annota
-000000c0: 7469 6f6e 732c 2061 6e64 2061 2050 7974  tions, and a Pyt
-000000d0: 686f 6e20 6c69 6272 6172 7920 4150 4920  hon library API 
-000000e0: 666f 7220 776f 726b 696e 6720 7769 7468  for working with
-000000f0: 2062 6f74 682e 0a0a 5468 6520 6c69 6272   both...The libr
-00000100: 6172 7920 636f 6465 206b 6e6f 7773 2068  ary code knows h
-00000110: 6f77 2074 6f20 6578 7472 6163 7420 6765  ow to extract ge
-00000120: 6e65 7320 6174 2074 6865 206e 7563 6c65  nes at the nucle
-00000130: 6f74 6964 6520 6f72 2061 6d69 6e6f 2061  otide or amino a
-00000140: 6369 640a 6c65 7665 6c2c 2068 6f77 2074  cid.level, how t
-00000150: 6f20 6964 656e 7469 6679 206f 7220 6368  o identify or ch
-00000160: 6563 6b20 666f 7220 6578 7065 6374 6564  eck for expected
-00000170: 2067 656e 6f6d 6520 6368 616e 6765 732c   genome changes,
-00000180: 2068 6f77 2074 6f0a 7472 616e 736c 6174   how to.translat
-00000190: 6520 6265 7477 6565 6e20 6161 2061 6e64  e between aa and
-000001a0: 206e 7420 6f66 6673 6574 732c 2061 6e64   nt offsets, and
-000001b0: 2061 626f 7574 2061 6c6c 2067 656e 6f6d   about all genom
-000001c0: 6520 6665 6174 7572 6573 2e0a 0a23 2320  e features...## 
-000001d0: 436f 6e76 656e 7469 6f6e 730a 0a23 2323  Conventions..###
-000001e0: 2053 4152 532d 436f 562d 3220 6765 6e6f   SARS-CoV-2 geno
-000001f0: 6d65 730a 0a54 6869 7320 636f 6465 2077  mes..This code w
-00000200: 6173 2077 7269 7474 656e 2069 6e20 6c61  as written in la
-00000210: 7465 2032 3032 3020 666f 7220 7072 6f63  te 2020 for proc
-00000220: 6573 7369 6e67 2053 4152 532d 436f 562d  essing SARS-CoV-
-00000230: 3220 6765 6e6f 6d65 732e 2049 740a 6861  2 genomes. It.ha
-00000240: 7320 7369 6e63 6520 6265 656e 2067 656e  s since been gen
-00000250: 6572 616c 697a 6564 2074 6f20 6465 616c  eralized to deal
-00000260: 2077 6974 6820 616e 7920 4765 6e42 616e   with any GenBan
-00000270: 6b20 6669 6c65 2e20 5468 6520 636f 6d6d  k file. The comm
-00000280: 616e 642d 6c69 6e65 0a73 6372 6970 7473  and-line.scripts
-00000290: 2063 616e 2062 6520 6769 7665 6e20 6120   can be given a 
-000002a0: 602d 2d73 6172 7332 6020 746f 2068 6176  `--sars2` to hav
-000002b0: 6520 7468 656d 2075 7365 2074 6865 2057  e them use the W
-000002c0: 7568 616e 2072 6566 6572 656e 6365 2c20  uhan reference, 
-000002d0: 696e 0a77 6869 6368 2063 6173 6520 7468  in.which case th
-000002e0: 6572 6520 6973 206e 6f20 6e65 6564 2074  ere is no need t
-000002f0: 6f20 7072 6f76 6964 6520 6120 4765 6e42  o provide a GenB
-00000300: 616e 6b20 6669 6c65 2e20 5369 6d69 6c61  ank file. Simila
-00000310: 726c 792c 2074 6865 0a50 7974 686f 6e20  rly, the.Python 
-00000320: 636c 6173 7365 7320 6361 6e20 7461 6b65  classes can take
-00000330: 2061 2060 7361 7273 3260 2061 7267 756d   a `sars2` argum
-00000340: 656e 7420 7769 7468 2074 6865 2073 616d  ent with the sam
-00000350: 6520 6566 6665 6374 2077 6865 6e20 6974  e effect when it
-00000360: 2069 730a 7365 7420 746f 2060 5472 7565   is.set to `True
-00000370: 602e 2049 6620 796f 7527 7265 206e 6f74  `. If you're not
-00000380: 2077 6f72 6b69 6e67 2077 6974 6820 5341   working with SA
-00000390: 5253 2d43 6f56 2d32 2067 656e 6f6d 6573  RS-CoV-2 genomes
-000003a0: 2c20 6a75 7374 2070 6173 7320 7468 650a  , just pass the.
-000003b0: 4765 6e42 616e 6b20 6669 6c65 2066 6f72  GenBank file for
-000003c0: 2079 6f75 7220 6765 6e6f 6d65 2074 6f20   your genome to 
-000003d0: 7468 6520 636f 6d6d 616e 642d 6c69 6e65  the command-line
-000003e0: 2073 6372 6970 7473 2077 6974 6820 602d   scripts with `-
-000003f0: 2d72 6566 6572 656e 6365 600a 6f72 2074  -reference`.or t
-00000400: 6f20 7468 6520 5079 7468 6f6e 2066 756e  o the Python fun
-00000410: 6374 696f 6e73 2e20 4966 2079 6f75 2061  ctions. If you a
-00000420: 7265 2077 6f72 6b69 6e67 2077 6974 6820  re working with 
-00000430: 5341 5253 2d43 6f56 2d32 2c20 616e 6420  SARS-CoV-2, and 
-00000440: 796f 750a 7761 6e74 2074 6f20 7573 6520  you.want to use 
-00000450: 7468 6520 5775 6861 6e20 7265 6665 7265  the Wuhan refere
-00000460: 6e63 652c 2079 6f75 2063 616e 2075 7365  nce, you can use
-00000470: 2074 6865 2073 686f 7274 6375 7420 6a75   the shortcut ju
-00000480: 7374 2064 6573 6372 6962 6564 2e0a 0a23  st described...#
-00000490: 2323 204c 6f63 6174 696f 6e73 2076 7320  ## Locations vs 
-000004a0: 6f66 6673 6574 730a 0a57 6865 6e20 6769  offsets..When gi
-000004b0: 7669 6e67 206c 6f63 6174 696f 6e73 2077  ving locations w
-000004c0: 6974 6869 6e20 6120 6765 6e6f 6d65 206f  ithin a genome o
-000004d0: 7220 6120 6765 6e6f 6d65 2066 6561 7475  r a genome featu
-000004e0: 7265 2028 652e 672e 2c20 610a 7061 7274  re (e.g., a.part
-000004f0: 6963 756c 6172 2070 726f 7465 696e 292c  icular protein),
-00000500: 2061 2022 7369 7465 2220 7265 6665 7273   a "site" refers
-00000510: 2074 6f20 6120 312d 6261 7365 6420 6c6f   to a 1-based lo
-00000520: 6361 7469 6f6e 2c20 6173 2077 6f75 6c64  cation, as would
-00000530: 0a6e 6f72 6d61 6c6c 7920 6265 2075 7365  .normally be use
-00000540: 6420 6279 2061 2072 6567 756c 6172 2070  d by a regular p
-00000550: 6572 736f 6e2c 2077 6865 7265 6173 2061  erson, whereas a
-00000560: 6e20 226f 6666 7365 7422 2072 6566 6572  n "offset" refer
-00000570: 7320 746f 2061 0a30 2d62 6173 6564 206c  s to a.0-based l
-00000580: 6f63 6174 696f 6e2c 2061 7320 776f 756c  ocation, as woul
-00000590: 6420 6265 2075 7365 6420 6279 2061 2050  d be used by a P
-000005a0: 7974 686f 6e20 7072 6f67 7261 6d6d 6572  ython programmer
-000005b0: 2e20 2054 6865 2075 7469 6c69 7479 0a73  .  The utility.s
-000005c0: 6372 6970 7473 2c20 7275 6e20 6672 6f6d  cripts, run from
-000005d0: 2074 6865 2063 6f6d 6d61 6e64 206c 696e   the command lin
-000005e0: 652c 2065 7870 6563 7420 7468 6520 666f  e, expect the fo
-000005f0: 726d 6572 2c20 7768 6572 6561 7320 6c69  rmer, whereas li
-00000600: 6272 6172 7920 636f 6465 0a63 616c 6c65  brary code.calle
-00000610: 6420 6279 2061 2070 726f 6772 616d 6d65  d by a programme
-00000620: 7220 6578 7065 6374 7320 7468 6520 6c61  r expects the la
-00000630: 7474 6572 2e20 5468 6973 2074 6572 6d69  tter. This termi
-00000640: 6e6f 6c6f 6779 2069 7320 7573 6564 0a74  nology is used.t
-00000650: 6872 6f75 6768 6f75 7420 7468 6520 636f  hroughout the co
-00000660: 6465 2061 7320 7765 6c6c 2e0a 0a23 2323  de as well...###
-00000670: 2041 7267 756d 656e 7420 616e 6420 7265   Argument and re
-00000680: 7475 726e 2076 616c 7565 206f 7264 6572  turn value order
-00000690: 696e 670a 0a49 6e20 6675 6e63 7469 6f6e  ing..In function
-000006a0: 7320 7468 6174 2064 6561 6c20 7769 7468  s that deal with
-000006b0: 2062 6f74 6820 6120 7265 6665 7265 6e63   both a referenc
-000006c0: 6520 616e 6420 6120 6765 6e6f 6d65 2073  e and a genome s
-000006d0: 6571 7565 6e63 652c 2074 6865 0a72 6566  equence, the.ref
-000006e0: 6572 656e 6365 2069 7320 616c 7761 7973  erence is always
-000006f0: 2067 6976 656e 206f 7220 7265 7475 726e   given or return
-00000700: 6564 2066 6972 7374 2e0a 0a23 2320 416c  ed first...## Al
-00000710: 6967 6e6d 656e 740a 0a60 6762 3273 6571  ignment..`gb2seq
-00000720: 6020 6d61 6b65 7320 616e 2061 6c69 676e  ` makes an align
-00000730: 6d65 6e74 2062 6574 7765 656e 2065 6163  ment between eac
-00000740: 6820 6765 6e6f 6d65 2079 6f75 2067 6976  h genome you giv
-00000750: 6520 6974 2061 6e64 2061 0a72 6566 6572  e it and a.refer
-00000760: 656e 6365 2073 6571 7565 6e63 652e 0a0a  ence sequence...
-00000770: 5468 6520 6465 6661 756c 7420 616c 6967  The default alig
-00000780: 6e6d 656e 7420 616c 676f 7269 7468 6d20  nment algorithm 
-00000790: 6973 0a5b 4d41 4646 545d 2868 7474 7073  is.[MAFFT](https
-000007a0: 3a2f 2f6d 6166 6674 2e63 6272 632e 6a70  ://mafft.cbrc.jp
-000007b0: 2f61 6c69 676e 6d65 6e74 2f73 6f66 7477  /alignment/softw
-000007c0: 6172 652f 292c 2077 6869 6368 2063 616e  are/), which can
-000007d0: 2062 6520 736c 6f77 2062 7574 0a69 7320   be slow but.is 
-000007e0: 7265 6c69 6162 6c65 2e20 596f 7520 6361  reliable. You ca
-000007f0: 6e20 616c 736f 2072 756e 2073 6372 6970  n also run scrip
-00000800: 7473 2077 6974 6820 602d 2d61 6c69 676e  ts with `--align
-00000810: 6572 2065 646c 6962 6020 286f 7220 7061  er edlib` (or pa
-00000820: 7373 0a60 616c 6967 6e65 723d 2765 646c  ss.`aligner='edl
-00000830: 6962 2760 2074 6f20 6c69 6272 6172 7920  ib'` to library 
-00000840: 6675 6e63 7469 6f6e 7329 2074 6f20 7573  functions) to us
-00000850: 6520 5b74 6865 2050 7974 686f 6e0a 7772  e [the Python.wr
-00000860: 6170 7065 725d 2868 7474 7073 3a2f 2f70  apper](https://p
-00000870: 7970 692e 6f72 672f 7072 6f6a 6563 742f  ypi.org/project/
-00000880: 6564 6c69 622f 2920 666f 7220 7468 6520  edlib/) for the 
-00000890: 6578 7472 656d 656c 7920 6661 7374 0a5b  extremely fast.[
-000008a0: 6564 6c69 625d 2868 7474 7073 3a2f 2f67  edlib](https://g
-000008b0: 6974 6875 622e 636f 6d2f 4d61 7274 696e  ithub.com/Martin
-000008c0: 736f 732f 6564 6c69 6229 206c 6962 7261  sos/edlib) libra
-000008d0: 7279 2e0a 0a23 2055 7469 6c69 7479 2073  ry...# Utility s
-000008e0: 6372 6970 7473 0a0a 5468 6520 7363 7269  cripts..The scri
-000008f0: 7074 7320 6465 7363 7269 6265 6420 6265  pts described be
-00000900: 6c6f 7720 616c 6c20 6163 6365 7074 2061  low all accept a
-00000910: 2060 2d2d 6865 6c70 6020 6f70 7469 6f6e   `--help` option
-00000920: 2e20 4265 6c6f 7720 6973 0a73 6f6d 6520  . Below is.some 
-00000930: 7265 7072 6573 656e 7461 7469 7665 2075  representative u
-00000940: 7361 6765 2e0a 0a23 2320 6465 7363 7269  sage...## descri
-00000950: 6265 2d66 6561 7475 7265 2e70 790a 0a54  be-feature.py..T
-00000960: 6865 2073 696d 706c 6573 7420 7363 7269  he simplest scri
-00000970: 7074 2069 7320 6064 6573 6372 6962 652d  pt is `describe-
-00000980: 6665 6174 7572 652e 7079 602c 2077 6869  feature.py`, whi
-00000990: 6368 2063 616e 2062 6520 7573 6564 2074  ch can be used t
-000009a0: 6f20 6765 740a 696e 666f 726d 6174 696f  o get.informatio
-000009b0: 6e20 6162 6f75 7420 6665 6174 7572 6573  n about features
-000009c0: 2069 6e20 6120 7265 6665 7265 6e63 6520   in a reference 
-000009d0: 6765 6e6f 6d65 2073 7065 6369 6669 6564  genome specified
-000009e0: 2062 7920 7061 7373 696e 6720 7468 650a   by passing the.
-000009f0: 6e61 6d65 206f 6620 6120 4765 6e42 616e  name of a GenBan
-00000a00: 6b20 6669 6c65 2077 6974 6820 602d 2d67  k file with `--g
-00000a10: 6246 696c 6560 2028 6f72 206a 7573 7420  bFile` (or just 
-00000a20: 7573 6520 602d 2d73 6172 7332 6020 746f  use `--sars2` to
-00000a30: 2069 6620 796f 750a 7761 6e74 2074 6865   if you.want the
-00000a40: 2057 7568 616e 2072 6566 6572 656e 6365   Wuhan reference
-00000a50: 0a5b 4e43 5f30 3435 3531 325d 2868 7474  .[NC_045512](htt
-00000a60: 7073 3a2f 2f77 7777 2e6e 6362 692e 6e6c  ps://www.ncbi.nl
-00000a70: 6d2e 6e69 682e 676f 762f 6e75 6363 6f72  m.nih.gov/nuccor
-00000a80: 652f 4e43 5f30 3435 3531 3229 292e 0a0a  e/NC_045512))...
-00000a90: 4966 2079 6f75 2072 756e 2060 6465 7363  If you run `desc
-00000aa0: 7269 6265 2d66 6561 7475 7265 2e70 7960  ribe-feature.py`
-00000ab0: 2077 6974 6820 6e6f 2061 7267 756d 656e   with no argumen
-00000ac0: 7473 2c20 6974 2077 696c 6c20 7072 696e  ts, it will prin
-00000ad0: 7420 7375 6d6d 6172 790a 6465 7461 696c  t summary.detail
-00000ae0: 7320 6f66 2061 6c6c 2066 6561 7475 7265  s of all feature
-00000af0: 732c 2077 6974 6820 7468 6569 7220 2830  s, with their (0
-00000b00: 2d62 6173 6564 2920 6e75 636c 656f 7469  -based) nucleoti
-00000b10: 6465 206f 6666 7365 7473 2e20 452e 672e  de offsets. E.g.
-00000b20: 2c0a 0a60 6060 7368 0a24 2064 6573 6372  ,..```sh.$ descr
-00000b30: 6962 652d 6665 6174 7572 652e 7079 202d  ibe-feature.py -
-00000b40: 2d73 6172 7332 0a46 6561 7475 7265 7320  -sars2.Features 
-00000b50: 666f 7220 4e43 5f30 3435 3531 322e 323a  for NC_045512.2:
-00000b60: 0a32 272d 4f2d 7269 626f 7365 206d 6574  .2'-O-ribose met
-00000b70: 6879 6c74 7261 6e73 6665 7261 7365 3a0a  hyltransferase:.
-00000b80: 2020 7374 6172 743a 2032 3036 3538 0a20    start: 20658. 
-00000b90: 2073 746f 703a 2032 3135 3532 0a20 206c   stop: 21552.  l
-00000ba0: 656e 6774 683a 2038 3934 0a20 2070 726f  ength: 894.  pro
-00000bb0: 6475 6374 3a20 3227 2d4f 2d72 6962 6f73  duct: 2'-O-ribos
-00000bc0: 6520 6d65 7468 796c 7472 616e 7366 6572  e methyltransfer
-00000bd0: 6173 650a 2020 7365 7175 656e 6365 2020  ase.  sequence  
-00000be0: 2020 286c 656e 2020 2038 3934 206e 7429    (len   894 nt)
-00000bf0: 3a20 5443 5441 4754 4341 4147 4347 5447  : TCTAGTCAAGCGTG
-00000c00: 4743 4141 4343 4747 4754 4754 5447 4354  GCAACCGGGTGTTGCT
-00000c10: 4154 4743 4354 4141 5443 5454 5441 4341  ATGCCTAATCTTTACA
-00000c20: 4141 412e 2e2e 0a33 272d 746f 2d35 2720  AAA....3'-to-5' 
-00000c30: 6578 6f6e 7563 6c65 6173 653a 0a20 2073  exonuclease:.  s
-00000c40: 7461 7274 3a20 3138 3033 390a 2020 7374  tart: 18039.  st
-00000c50: 6f70 3a20 3139 3632 300a 2020 6c65 6e67  op: 19620.  leng
-00000c60: 7468 3a20 3135 3831 0a20 2070 726f 6475  th: 1581.  produ
-00000c70: 6374 3a20 3327 2d74 6f2d 3527 2065 786f  ct: 3'-to-5' exo
-00000c80: 6e75 636c 6561 7365 0a20 2073 6571 7565  nuclease.  seque
-00000c90: 6e63 6520 2020 2028 6c65 6e20 2031 3538  nce    (len  158
-00000ca0: 3120 6e74 293a 2047 4354 4741 4141 4154  1 nt): GCTGAAAAT
-00000cb0: 4754 4141 4341 4747 4143 5443 5454 5441  GTAACAGGACTCTTTA
-00000cc0: 4141 4741 5454 4754 4147 5441 4147 4754  AAGATTGTAGTAAGGT
-00000cd0: 4141 5443 4143 5447 2e2e 2e0a 3327 5554  AATCACTG....3'UT
-00000ce0: 523a 0a20 2073 7461 7274 3a20 3239 3637  R:.  start: 2967
-00000cf0: 340a 2020 7374 6f70 3a20 3239 3930 330a  4.  stop: 29903.
-00000d00: 2020 6c65 6e67 7468 3a20 3232 390a 2020    length: 229.  
-00000d10: 7365 7175 656e 6365 2020 2020 286c 656e  sequence    (len
-00000d20: 2020 2032 3239 206e 7429 3a20 4341 4154     229 nt): CAAT
-00000d30: 4354 5454 4141 5443 4147 5447 5447 5441  CTTTAATCAGTGTGTA
-00000d40: 4143 4154 5441 4747 4741 4747 4143 5454  ACATTAGGGAGGACTT
-00000d50: 4741 4141 4741 4743 4341 4343 412e 2e2e  GAAAGAGCCACCA...
-00000d60: 0a23 205b 4d61 6e79 2061 6464 6974 696f  .# [Many additio
-00000d70: 6e61 6c20 6f75 7470 7574 206c 696e 6573  nal output lines
-00000d80: 206f 6d69 7474 6564 2068 6572 652e 5d0a   omitted here.].
-00000d90: 6060 600a 0a59 6f75 2063 616e 2061 6c73  ```..You can als
-00000da0: 6f20 7061 7373 2069 7420 6120 6665 6174  o pass it a feat
-00000db0: 7572 6520 6e61 6d65 2028 6f72 206d 756c  ure name (or mul
-00000dc0: 7469 706c 6520 6665 6174 7572 6520 6e61  tiple feature na
-00000dd0: 6d65 7329 3a0a 0a60 6060 7368 0a24 2064  mes):..```sh.$ d
-00000de0: 6573 6372 6962 652d 6665 6174 7572 652e  escribe-feature.
-00000df0: 7079 202d 2d73 6172 7332 202d 2d6e 616d  py --sars2 --nam
-00000e00: 6520 7370 696b 650a 7375 7266 6163 6520  e spike.surface 
-00000e10: 676c 7963 6f70 726f 7465 696e 3a0a 2020  glycoprotein:.  
-00000e20: 7374 6172 743a 2032 3135 3632 0a20 2073  start: 21562.  s
-00000e30: 746f 703a 2032 3533 3834 0a20 206c 656e  top: 25384.  len
-00000e40: 6774 683a 2033 3832 320a 2020 7072 6f64  gth: 3822.  prod
-00000e50: 7563 743a 2073 7572 6661 6365 2067 6c79  uct: surface gly
-00000e60: 636f 7072 6f74 6569 6e0a 2020 7365 7175  coprotein.  sequ
-00000e70: 656e 6365 2020 2020 286c 656e 2020 3338  ence    (len  38
-00000e80: 3232 206e 7429 3a20 4154 4754 5454 4754  22 nt): ATGTTTGT
-00000e90: 5454 5454 4354 5447 5454 5454 4154 5447  TTTTCTTGTTTTATTG
-00000ea0: 4343 4143 5441 4754 4354 4354 4147 5443  CCACTAGTCTCTAGTC
-00000eb0: 4147 5447 5447 5454 412e 2e2e 0a20 2074  AGTGTGTTA....  t
-00000ec0: 7261 6e73 6c61 7469 6f6e 2028 6c65 6e20  ranslation (len 
-00000ed0: 2031 3237 3420 6161 293a 204d 4656 464c   1274 aa): MFVFL
-00000ee0: 564c 4c50 4c56 5353 5143 564e 4c54 5452  VLLPLVSSQCVNLTTR
-00000ef0: 5451 4c50 5041 5954 4e53 4654 5247 5659  TQLPPAYTNSFTRGVY
-00000f00: 5950 444b 5646 5253 5356 4c48 2e2e 2e0a  YPDKVFRSSVLH....
-00000f10: 6060 600a 0a41 6e64 2079 6f75 2063 616e  ```..And you can
-00000f20: 2070 6173 7320 696e 2061 2067 656e 6f6d   pass in a genom
-00000f30: 6520 746f 2067 6574 2069 6e66 6f72 6d61  e to get informa
-00000f40: 7469 6f6e 206f 6e20 7468 6520 6665 6174  tion on the feat
-00000f50: 7572 6520 696e 2062 6f74 6820 7468 650a  ure in both the.
-00000f60: 7265 6665 7265 6e63 6520 616e 6420 7468  reference and th
-00000f70: 6520 7061 7373 6564 2067 656e 6f6d 6520  e passed genome 
-00000f80: 2877 6869 6368 2077 696c 6c20 6265 2061  (which will be a
-00000f90: 6c69 676e 6564 2074 6f20 7468 650a 7265  ligned to the.re
-00000fa0: 6665 7265 6e63 6529 2e20 5468 6520 6f66  ference). The of
-00000fb0: 6673 6574 2061 6e64 206c 656e 6774 6820  fset and length 
-00000fc0: 6f66 2074 6865 2066 6561 7475 7265 2069  of the feature i
-00000fd0: 6e20 7468 6520 6765 6e6f 6d65 206d 6179  n the genome may
-00000fe0: 206f 660a 636f 7572 7365 2064 6966 6665   of.course diffe
-00000ff0: 7220 6672 6f6d 2074 6865 2072 6566 6572  r from the refer
-00001000: 656e 6365 3a0a 0a60 6060 7368 0a24 2064  ence:..```sh.$ d
-00001010: 6573 6372 6962 652d 6665 6174 7572 652e  escribe-feature.
-00001020: 7079 202d 2d6e 616d 6520 7320 2d2d 7361  py --name s --sa
-00001030: 7273 3220 2d2d 6765 6e6f 6d65 2043 5370  rs2 --genome CSp
-00001040: 6563 5669 7239 3239 302e 6661 7374 610a  ecVir9290.fasta.
-00001050: 5265 6665 7265 6e63 653a 0a20 2073 7572  Reference:.  sur
-00001060: 6661 6365 2067 6c79 636f 7072 6f74 6569  face glycoprotei
-00001070: 6e3a 0a20 2020 2073 7461 7274 3a20 3231  n:.    start: 21
-00001080: 3536 320a 2020 2020 7374 6f70 3a20 3235  562.    stop: 25
-00001090: 3338 340a 2020 2020 6c65 6e67 7468 2028  384.    length (
-000010a0: 6e74 293a 2033 3832 320a 2020 2020 7072  nt): 3822.    pr
-000010b0: 6f64 7563 743a 2073 7572 6661 6365 2067  oduct: surface g
-000010c0: 6c79 636f 7072 6f74 6569 6e0a 2020 2020  lycoprotein.    
-000010d0: 6e6f 7465 3a20 7374 7275 6374 7572 616c  note: structural
-000010e0: 2070 726f 7465 696e 3b20 7370 696b 6520   protein; spike 
-000010f0: 7072 6f74 6569 6e0a 2020 2020 6665 6174  protein.    feat
-00001100: 7572 6520 6973 2074 7261 6e73 6c61 7465  ure is translate
-00001110: 6420 6c65 6674 2d74 6f2d 7269 6768 742e  d left-to-right.
-00001120: 0a20 2020 2073 6571 7565 6e63 653a 2041  .    sequence: A
-00001130: 5447 5454 5447 5454 5454 5443 5454 4754  TGTTTGTTTTTCTTGT
-00001140: 5454 5441 5454 4743 4341 4354 4147 5443  TTTATTGCCACTAGTC
-00001150: 5443 5441 4754 4341 4754 4754 4754 5441  TCTAGTCAGTGTGTTA
-00001160: 4154 4354 5441 4341 4143 4341 4741 4143  ATCTTACAACCAGAAC
-00001170: 5443 4141 5454 4143 4343 4343 5447 432e  TCAATTACCCCCTGC.
-00001180: 2e2e 0a20 2020 206c 656e 6774 6820 2861  ...    length (a
-00001190: 6129 3a20 3132 3734 0a20 2020 2074 7261  a): 1274.    tra
-000011a0: 6e73 6c61 7469 6f6e 3a20 4d46 5646 4c56  nslation: MFVFLV
-000011b0: 4c4c 504c 5653 5351 4356 4e4c 5454 5254  LLPLVSSQCVNLTTRT
-000011c0: 514c 5050 4159 544e 5346 5452 4756 5959  QLPPAYTNSFTRGVYY
-000011d0: 5044 4b56 4652 5353 564c 4853 5451 444c  PDKVFRSSVLHSTQDL
-000011e0: 464c 5046 4653 4e56 5457 4648 4149 4856  FLPFFSNVTWFHAIHV
-000011f0: 5347 544e 4754 4b52 4644 2e2e 2e0a 2020  SGTNGTKRFD....  
-00001200: 4765 6e6f 6d65 2042 6574 6143 6f56 2f52  Genome BetaCoV/R
-00001210: 656e 6473 6275 7267 2d45 636b 6572 6e66  endsburg-Eckernf
-00001220: 6f65 7264 652f 4368 5669 7239 3239 302f  oerde/ChVir9290/
-00001230: 3230 3230 3a0a 2020 2020 7374 6172 743a  2020:.    start:
-00001240: 2032 3135 3530 0a20 2020 2073 746f 703a   21550.    stop:
-00001250: 2032 3533 3636 0a20 2020 206c 656e 6774   25366.    lengt
-00001260: 6820 286e 7429 3a20 3338 3232 0a20 2020  h (nt): 3822.   
-00001270: 2073 6571 7565 6e63 653a 2041 5447 5454   sequence: ATGTT
-00001280: 5447 5454 5454 5443 5454 4754 5454 5441  TGTTTTTCTTGTTTTA
-00001290: 5454 4743 4341 4354 4147 5443 5443 5441  TTGCCACTAGTCTCTA
-000012a0: 4754 4341 4754 4754 4754 5441 4154 4354  GTCAGTGTGTTAATCT
-000012b0: 5441 4341 4143 4341 4741 4143 5443 4141  TACAACCAGAACTCAA
-000012c0: 5454 4143 4343 4343 5447 432e 2e2e 0a20  TTACCCCCTGC.... 
-000012d0: 2020 2074 7261 6e73 6c61 7469 6f6e 3a20     translation: 
-000012e0: 4d46 5646 4c56 4c4c 504c 5653 5351 4356  MFVFLVLLPLVSSQCV
-000012f0: 4e4c 5454 5254 514c 5050 4159 544e 5346  NLTTRTQLPPAYTNSF
-00001300: 5452 4756 5959 5044 4b56 4652 5353 564c  TRGVYYPDKVFRSSVL
-00001310: 4853 5451 444c 464c 5046 4653 4e56 5457  HSTQDLFLPFFSNVTW
-00001320: 4648 4149 5347 544e 4754 4b52 4644 4e50  FHAISGTNGTKRFDNP
-00001330: 2e2e 2e0a 6060 600a 0a4f 7220 6173 6b20  ....```..Or ask 
-00001340: 746f 2073 6565 2061 6c6c 206b 6e6f 776e  to see all known
-00001350: 2066 6561 7475 7265 206e 616d 6573 2028   feature names (
-00001360: 7573 696e 6720 602d 2d6e 616d 6573 6029  using `--names`)
-00001370: 2e20 4966 2079 6f75 2070 6173 730a 602d  . If you pass.`-
-00001380: 2d73 6172 7332 602c 2065 6163 6820 6e61  -sars2`, each na
-00001390: 6d65 2069 7320 7072 696e 7465 6420 666f  me is printed fo
-000013a0: 6c6c 6f77 6564 2062 7920 6120 636f 6c6f  llowed by a colo
-000013b0: 6e20 616e 6420 6120 2870 6f73 7369 626c  n and a (possibl
-000013c0: 7920 656d 7074 7929 0a6c 6973 7420 6f66  y empty).list of
-000013d0: 2061 6c69 6173 6573 3a0a 0a60 6060 7368   aliases:..```sh
-000013e0: 0a24 2064 6573 6372 6962 652d 6665 6174  .$ describe-feat
-000013f0: 7572 652e 7079 202d 2d73 6172 7332 202d  ure.py --sars2 -
-00001400: 2d6e 616d 6573 0a32 272d 4f2d 7269 626f  -names.2'-O-ribo
-00001410: 7365 206d 6574 6879 6c74 7261 6e73 6665  se methyltransfe
-00001420: 7261 7365 3a20 320a 3327 2d74 6f2d 3527  rase: 2.3'-to-5'
-00001430: 2065 786f 6e75 636c 6561 7365 3a20 6578   exonuclease: ex
-00001440: 6f6e 2c20 6578 6f6e 7563 6c65 6173 652c  on, exonuclease,
-00001450: 206e 7370 3134 0a33 2755 5452 3a20 3375   nsp14.3'UTR: 3u
-00001460: 7472 0a33 432d 6c69 6b65 2070 726f 7465  tr.3C-like prote
-00001470: 696e 6173 653a 2033 636c 7072 6f2c 206d  inase: 3clpro, m
-00001480: 7072 6f2c 206e 7370 350a 3527 5554 523a  pro, nsp5.5'UTR:
-00001490: 2035 7574 720a 656e 646f 524e 4173 653a   5utr.endoRNAse:
-000014a0: 2065 6e64 6f72 6e61 7365 2c20 6e73 7031   endornase, nsp1
-000014b0: 350a 656e 7665 6c6f 7065 2070 726f 7465  5.envelope prote
-000014c0: 696e 3a20 652c 2065 6e76 656c 6f70 652c  in: e, envelope,
-000014d0: 206f 7266 340a 6865 6c69 6361 7365 3a20   orf4.helicase: 
-000014e0: 6e73 7031 330a 6c65 6164 6572 2070 726f  nsp13.leader pro
-000014f0: 7465 696e 3a20 6c65 6164 6572 2c20 6e73  tein: leader, ns
-00001500: 7031 0a6d 656d 6272 616e 6520 676c 7963  p1.membrane glyc
-00001510: 6f70 726f 7465 696e 3a20 6d2c 206d 656d  oprotein: m, mem
-00001520: 6272 616e 652c 206f 7266 350a 6e73 7032  brane, orf5.nsp2
-00001530: 3a0a 6e73 7033 3a0a 6e73 7034 3a0a 6e73  :.nsp3:.nsp4:.ns
-00001540: 7036 3a0a 6e73 7037 3a0a 6e73 7038 3a0a  p6:.nsp7:.nsp8:.
-00001550: 6e73 7039 3a0a 6e73 7031 303a 0a6e 7370  nsp9:.nsp10:.nsp
-00001560: 3131 3a0a 6e75 636c 656f 6361 7073 6964  11:.nucleocapsid
-00001570: 2070 686f 7370 686f 7072 6f74 6569 6e3a   phosphoprotein:
-00001580: 206e 2c20 6f72 6639 0a4f 5246 3161 6220   n, orf9.ORF1ab 
-00001590: 706f 6c79 7072 6f74 6569 6e3a 206f 7266  polyprotein: orf
-000015a0: 3161 620a 4f52 4631 6120 706f 6c79 7072  1ab.ORF1a polypr
-000015b0: 6f74 6569 6e3a 206f 7266 3161 0a4f 5246  otein: orf1a.ORF
-000015c0: 3361 2070 726f 7465 696e 3a20 6f72 6633  3a protein: orf3
-000015d0: 610a 4f52 4636 2070 726f 7465 696e 3a20  a.ORF6 protein: 
-000015e0: 6f72 6636 0a4f 5246 3761 2070 726f 7465  orf6.ORF7a prote
-000015f0: 696e 3a20 6f72 6637 610a 4f52 4637 623a  in: orf7a.ORF7b:
-00001600: 206f 7266 3762 0a4f 5246 3820 7072 6f74   orf7b.ORF8 prot
-00001610: 6569 6e3a 206f 7266 380a 4f52 4631 3020  ein: orf8.ORF10 
-00001620: 7072 6f74 6569 6e3a 206f 7266 3130 0a52  protein: orf10.R
-00001630: 4e41 2d64 6570 656e 6465 6e74 2052 4e41  NA-dependent RNA
-00001640: 2070 6f6c 796d 6572 6173 653a 206e 7370   polymerase: nsp
-00001650: 3132 2c20 7264 7270 0a73 7465 6d20 6c6f  12, rdrp.stem lo
-00001660: 6f70 2031 3a20 736c 310a 7374 656d 206c  op 1: sl1.stem l
-00001670: 6f6f 7020 323a 2073 6c32 0a73 7465 6d20  oop 2: sl2.stem 
-00001680: 6c6f 6f70 2033 3a20 736c 330a 7374 656d  loop 3: sl3.stem
-00001690: 206c 6f6f 7020 343a 2073 6c34 0a73 7465   loop 4: sl4.ste
-000016a0: 6d20 6c6f 6f70 2035 3a20 736c 350a 7375  m loop 5: sl5.su
-000016b0: 7266 6163 6520 676c 7963 6f70 726f 7465  rface glycoprote
-000016c0: 696e 3a20 732c 2073 7069 6b65 0a60 6060  in: s, spike.```
-000016d0: 0a0a 5468 6572 6520 6973 2061 6c73 6f20  ..There is also 
-000016e0: 6120 602d 2d73 6f72 7442 7960 206f 7074  a `--sortBy` opt
-000016f0: 696f 6e20 666f 7220 736f 7274 696e 6720  ion for sorting 
-00001700: 7468 6520 6f72 6465 7220 6f66 2074 6865  the order of the
-00001710: 2072 6570 6f72 7465 640a 6665 6174 7572   reported.featur
-00001720: 6573 2e20 5468 6520 6465 6661 756c 7420  es. The default 
-00001730: 6973 2074 6865 206f 7264 6572 2074 6865  is the order the
-00001740: 7920 6172 6520 6769 7665 6e20 6f6e 2074  y are given on t
-00001750: 6865 2063 6f6d 6d61 6e64 0a6c 696e 652e  he command.line.
-00001760: 204f 7468 6572 206f 7074 696f 6e73 2061   Other options a
-00001770: 7265 2060 2d2d 736f 7274 4279 206e 616d  re `--sortBy nam
-00001780: 6560 2061 6e64 2060 2d2d 736f 7274 4279  e` and `--sortBy
-00001790: 2073 6974 6560 2028 692e 652e 2c20 6765   site` (i.e., ge
-000017a0: 6e6f 6d65 0a6f 6666 7365 7429 2e0a 0a23  nome.offset)...#
-000017b0: 2320 6465 7363 7269 6265 2d67 656e 6f6d  # describe-genom
-000017c0: 652e 7079 0a0a 6064 6573 6372 6962 652d  e.py..`describe-
-000017d0: 6765 6e6f 6d65 2e70 7960 2068 6173 206d  genome.py` has m
-000017e0: 616e 7920 7573 6573 2e20 4974 2063 616e  any uses. It can
-000017f0: 2065 7874 7261 6374 206d 756c 7469 706c   extract multipl
-00001800: 6520 6665 6174 7572 6573 2066 726f 6d0a  e features from.
-00001810: 6d75 6c74 6970 6c65 2067 6976 656e 2067  multiple given g
-00001820: 656e 6f6d 6573 2c20 6173 2061 6d69 6e6f  enomes, as amino
-00001830: 2061 6369 6473 206f 7220 6e75 636c 656f   acids or nucleo
-00001840: 7469 6465 7320 286f 7220 626f 7468 292e  tides (or both).
-00001850: 2049 7420 7769 6c6c 0a70 7269 6e74 2074   It will.print t
-00001860: 6f20 7374 616e 6461 7264 206f 7574 7075  o standard outpu
-00001870: 7420 6279 2064 6566 6175 6c74 2c20 6275  t by default, bu
-00001880: 7420 6966 2079 6f75 2075 7365 2074 6865  t if you use the
-00001890: 2060 2d2d 6f75 7444 6972 6020 6f70 7469   `--outDir` opti
-000018a0: 6f6e 0a74 6f20 7072 6f76 6964 6520 6120  on.to provide a 
-000018b0: 6469 7265 6374 6f72 792c 2069 6e64 6976  directory, indiv
-000018c0: 6964 7561 6c20 6f75 7470 7574 2066 696c  idual output fil
-000018d0: 6573 2077 6974 6820 2868 6f70 6566 756c  es with (hopeful
-000018e0: 6c79 290a 7365 6c66 2d65 7870 6c61 6e61  ly).self-explana
-000018f0: 746f 7279 206e 616d 6573 2077 696c 6c20  tory names will 
-00001900: 6265 2063 7265 6174 6564 2069 6e20 7468  be created in th
-00001910: 6174 2064 6972 6563 746f 7279 2e20 5468  at directory. Th
-00001920: 6520 6469 7265 6374 6f72 790a 7769 6c6c  e directory.will
-00001930: 2062 6520 6372 6561 7465 6420 666f 7220   be created for 
-00001940: 796f 7520 6966 2069 7420 646f 6573 6e27  you if it doesn'
-00001950: 7420 6578 6973 742e 0a0a 4120 736d 616c  t exist...A smal
-00001960: 6c20 6578 616d 706c 6520 6973 2070 6572  l example is per
-00001970: 6861 7073 2062 6573 742e 2048 6572 6520  haps best. Here 
-00001980: 7765 2070 756c 6c20 6f75 7420 7468 6520  we pull out the 
-00001990: 7370 696b 6520 6e75 636c 656f 7469 6465  spike nucleotide
-000019a0: 2061 6e64 0a61 6d69 6e6f 2061 6369 6420   and.amino acid 
-000019b0: 7365 7175 656e 6365 2066 726f 6d20 422e  sequence from B.
-000019c0: 312e 312e 3720 616e 6420 616c 736f 2061  1.1.7 and also a
-000019d0: 736b 2066 6f72 2061 2073 756d 6d61 7279  sk for a summary
-000019e0: 206f 6620 7468 6520 616d 696e 6f0a 6163   of the amino.ac
-000019f0: 6964 2064 6966 6665 7265 6e63 6573 3a0a  id differences:.
-00001a00: 0a60 6060 7368 0a24 2064 6573 6372 6962  .```sh.$ describ
-00001a10: 652d 6765 6e6f 6d65 2e70 7920 2d2d 6765  e-genome.py --ge
-00001a20: 6e6f 6d65 2064 6174 612f 4550 495f 4953  nome data/EPI_IS
-00001a30: 4c5f 3630 3134 3433 2e66 6173 7461 202d  L_601443.fasta -
-00001a40: 2d6f 7574 4469 7220 2f74 6d70 2f6f 7574  -outDir /tmp/out
-00001a50: 205c 0a20 2020 202d 2d66 6561 7475 7265   \.    --feature
-00001a60: 2073 7069 6b65 202d 2d70 7269 6e74 4e74   spike --printNt
-00001a70: 5365 7175 656e 6365 202d 2d70 7269 6e74  Sequence --print
-00001a80: 4161 5365 7175 656e 6365 202d 2d70 7269  AaSequence --pri
-00001a90: 6e74 4161 4d61 7463 680a 4578 616d 696e  ntAaMatch.Examin
-00001aa0: 6564 2031 2067 656e 6f6d 652e 0a0a 2420  ed 1 genome...$ 
-00001ab0: 6c73 202d 6c20 2f74 6d70 2f6f 7574 0a74  ls -l /tmp/out.t
-00001ac0: 6f74 616c 2032 340a 2d72 772d 7277 2d72  otal 24.-rw-rw-r
-00001ad0: 2d2d 2020 3120 7465 7272 7920 2077 6865  --  1 terry  whe
-00001ae0: 656c 2020 2037 3438 2041 7072 2031 3120  el   748 Apr 11 
-00001af0: 3135 3a32 3520 4550 495f 4953 4c5f 3630  15:25 EPI_ISL_60
-00001b00: 3134 3433 2d73 7069 6b65 2d61 612d 6d61  1443-spike-aa-ma
-00001b10: 7463 682e 7478 740a 2d72 772d 7277 2d72  tch.txt.-rw-rw-r
-00001b20: 2d2d 2020 3120 7465 7272 7920 2077 6865  --  1 terry  whe
-00001b30: 656c 2020 3133 3434 2041 7072 2031 3120  el  1344 Apr 11 
-00001b40: 3135 3a32 3520 4550 495f 4953 4c5f 3630  15:25 EPI_ISL_60
-00001b50: 3134 3433 2d73 7069 6b65 2d61 612d 7365  1443-spike-aa-se
-00001b60: 7175 656e 6365 2e66 6173 7461 0a2d 7277  quence.fasta.-rw
-00001b70: 2d72 772d 722d 2d20 2031 2074 6572 7279  -rw-r--  1 terry
-00001b80: 2020 7768 6565 6c20 2033 3838 3620 4170    wheel  3886 Ap
-00001b90: 7220 3131 2031 353a 3235 2045 5049 5f49  r 11 15:25 EPI_I
-00001ba0: 534c 5f36 3031 3434 332d 7370 696b 652d  SL_601443-spike-
-00001bb0: 6e74 2d73 6571 7565 6e63 652e 6661 7374  nt-sequence.fast
-00001bc0: 610a 6060 600a 0a49 6620 7468 6520 6669  a.```..If the fi
-00001bd0: 6c65 2067 6976 656e 2062 7920 602d 2d67  le given by `--g
-00001be0: 656e 6f6d 6560 2068 6164 2063 6f6e 7461  enome` had conta
-00001bf0: 696e 6564 206d 6f72 6520 7468 616e 206f  ined more than o
-00001c00: 6e65 2053 4152 532d 436f 562d 320a 6765  ne SARS-CoV-2.ge
-00001c10: 6e6f 6d65 2c20 7468 6520 7370 696b 6520  nome, the spike 
-00001c20: 776f 756c 6420 6861 7665 2062 6565 6e20  would have been 
-00001c30: 6578 7472 6163 7465 6420 666f 7220 616c  extracted for al
-00001c40: 6c20 6f66 2074 6865 6d2e 2053 696d 696c  l of them. Simil
-00001c50: 6172 6c79 2c20 6966 0a60 2d2d 6665 6174  arly, if.`--feat
-00001c60: 7572 6560 2068 6164 2062 6565 6e20 7265  ure` had been re
-00001c70: 7065 6174 6564 2c20 6d75 6c74 6970 6c65  peated, multiple
-00001c80: 2066 6561 7475 7265 7320 776f 756c 6420   features would 
-00001c90: 6861 7665 2062 6565 6e20 6578 7472 6163  have been extrac
-00001ca0: 7465 640a 616e 6420 636f 6d70 6172 6564  ted.and compared
-00001cb0: 2e20 4966 206e 6f20 602d 2d66 6561 7475  . If no `--featu
-00001cc0: 7265 6020 6973 2067 6976 656e 2c20 796f  re` is given, yo
-00001cd0: 7527 6c6c 2067 6574 2074 6865 6d20 616c  u'll get them al
-00001ce0: 6c2e 0a0a 6060 6073 680a 2420 6361 7420  l...```sh.$ cat 
-00001cf0: 2f74 6d70 2f6f 7574 2f45 5049 5f49 534c  /tmp/out/EPI_ISL
-00001d00: 5f36 3031 3434 332d 7370 696b 652d 6161  _601443-spike-aa
-00001d10: 2d6d 6174 6368 2e74 7874 0a46 6561 7475  -match.txt.Featu
-00001d20: 7265 3a20 7370 696b 6520 616d 696e 6f20  re: spike amino 
-00001d30: 6163 6964 206d 6174 6368 0a20 204d 6174  acid match.  Mat
-00001d40: 6368 6573 3a20 3132 3634 2f31 3237 3420  ches: 1264/1274 
-00001d50: 2839 392e 3232 2529 0a20 204d 6973 6d61  (99.22%).  Misma
-00001d60: 7463 6865 733a 2031 302f 3132 3734 2028  tches: 10/1274 (
-00001d70: 302e 3738 2529 0a20 2020 204e 6f74 2069  0.78%).    Not i
-00001d80: 6e76 6f6c 7669 6e67 2067 6170 7320 2869  nvolving gaps (i
-00001d90: 2e65 2e2c 2063 6f6e 666c 6963 7473 293a  .e., conflicts):
-00001da0: 2037 2f31 3237 3420 2830 2e35 3525 290a   7/1274 (0.55%).
-00001db0: 2020 2020 496e 766f 6c76 696e 6720 6120      Involving a 
-00001dc0: 6761 7020 696e 206f 6e65 2073 6571 7565  gap in one seque
-00001dd0: 6e63 653a 2033 2f31 3237 3420 2830 2e32  nce: 3/1274 (0.2
-00001de0: 3425 290a 2020 2020 496e 766f 6c76 696e  4%).    Involvin
-00001df0: 6720 6120 6761 7020 696e 2062 6f74 6820  g a gap in both 
-00001e00: 7365 7175 656e 6365 733a 2030 0a20 2020  sequences: 0.   
-00001e10: 2049 643a 204e 435f 3034 3535 3132 2e32   Id: NC_045512.2
-00001e20: 2028 7375 7266 6163 6520 676c 7963 6f70   (surface glycop
-00001e30: 726f 7465 696e 290a 2020 2020 2020 4c65  rotein).      Le
-00001e40: 6e67 7468 3a20 3132 3734 0a20 2020 2020  ngth: 1274.     
-00001e50: 2047 6170 733a 2030 0a20 2020 2049 643a   Gaps: 0.    Id:
-00001e60: 2045 5049 5f49 534c 5f36 3031 3434 3320   EPI_ISL_601443 
-00001e70: 6843 6f56 2d31 392f 456e 676c 616e 642f  hCoV-19/England/
-00001e80: 4d49 4c4b 2d39 4530 3542 332f 3230 3230  MILK-9E05B3/2020
-00001e90: 2028 7375 7266 6163 6520 676c 7963 6f70   (surface glycop
-00001ea0: 726f 7465 696e 290a 2020 2020 2020 4c65  rotein).      Le
-00001eb0: 6e67 7468 3a20 3132 3734 0a20 2020 2020  ngth: 1274.     
-00001ec0: 2047 6170 733a 2033 2f31 3237 3420 2830   Gaps: 3/1274 (0
-00001ed0: 2e32 3425 290a 2020 2020 2020 4761 7020  .24%).      Gap 
-00001ee0: 6c6f 6361 7469 6f6e 7320 2831 2d62 6173  locations (1-bas
-00001ef0: 6564 293a 2036 392c 2037 302c 2031 3434  ed): 69, 70, 144
-00001f00: 0a20 2020 2044 6966 6665 7265 6e63 6573  .    Differences
-00001f10: 3a20 7369 7465 2c20 6161 312c 2061 6132  : site, aa1, aa2
-00001f20: 2c20 7265 6620 6e74 2063 6f64 6f6e 2073  , ref nt codon s
-00001f30: 7461 7274 0a20 2020 2020 2020 2036 3920  tart.        69 
-00001f40: 4820 2d20 3231 3736 370a 2020 2020 2020  H - 21767.      
-00001f50: 2020 3730 2056 202d 2032 3137 3730 0a20    70 V - 21770. 
-00001f60: 2020 2020 2020 3134 3420 5920 2d20 3231        144 Y - 21
-00001f70: 3939 320a 2020 2020 2020 2035 3031 204e  992.       501 N
-00001f80: 2059 2032 3330 3633 0a20 2020 2020 2020   Y 23063.       
-00001f90: 3537 3020 4120 4420 3233 3237 300a 2020  570 A D 23270.  
-00001fa0: 2020 2020 2036 3134 2044 2047 2032 3334       614 D G 234
-00001fb0: 3032 0a20 2020 2020 2020 3638 3120 5020  02.       681 P 
-00001fc0: 4820 3233 3630 330a 2020 2020 2020 2037  H 23603.       7
-00001fd0: 3136 2054 2049 2032 3337 3038 0a20 2020  16 T I 23708.   
-00001fe0: 2020 2020 3938 3220 5320 4120 3234 3530      982 S A 2450
-00001ff0: 360a 2020 2020 2020 3131 3138 2044 2048  6.      1118 D H
-00002000: 2032 3439 3134 0a60 6060 0a0a 596f 7520   24914.```..You 
-00002010: 6361 6e20 616c 736f 2061 736b 2066 6f72  can also ask for
-00002020: 2074 6865 2063 6861 6e67 6573 2069 6e20   the changes in 
-00002030: 6120 7661 7269 616e 7420 746f 2062 6520  a variant to be 
-00002040: 6368 6563 6b65 642e 0a20 2020 2020 200a  checked..      .
-00002050: 6060 6073 680a 2420 6465 7363 7269 6265  ```sh.$ describe
-00002060: 2d67 656e 6f6d 652e 7079 202d 2d73 6172  -genome.py --sar
-00002070: 7332 202d 2d67 656e 6f6d 6520 6461 7461  s2 --genome data
-00002080: 2f45 5049 5f49 534c 5f36 3031 3434 332e  /EPI_ISL_601443.
-00002090: 6661 7374 6120 2d2d 6368 6563 6b56 6172  fasta --checkVar
-000020a0: 6961 6e74 2056 4f43 5f32 3032 3031 3230  iant VOC_2020120
-000020b0: 315f 554b 0a45 5049 5f49 534c 5f36 3031  1_UK.EPI_ISL_601
-000020c0: 3434 3320 6843 6f56 2d31 392f 456e 676c  443 hCoV-19/Engl
-000020d0: 616e 642f 4d49 4c4b 2d39 4530 3542 332f  and/MILK-9E05B3/
-000020e0: 3230 3230 0a56 6172 6961 6e74 2073 756d  2020.Variant sum
-000020f0: 6d61 7279 3a0a 2020 554b 2076 6172 6961  mary:.  UK varia
-00002100: 6e74 206f 6620 636f 6e63 6572 6e20 2856  nt of concern (V
-00002110: 4f43 2920 3230 3230 3132 2f30 313a 0a20  OC) 202012/01:. 
-00002120: 2032 3020 6368 6563 6b73 2c20 3230 2070   20 checks, 20 p
-00002130: 6173 7365 642e 0a20 2020 206f 7266 3161  assed..    orf1a
-00002140: 6220 6161 3a20 5041 5353 3a20 3130 3031  b aa: PASS: 1001
-00002150: 492c 2031 3730 3844 2c20 3232 3330 542c  I, 1708D, 2230T,
-00002160: 2033 3637 352d 2c20 3336 3736 2d2c 2033   3675-, 3676-, 3
-00002170: 3637 372d 0a20 2020 2073 7069 6b65 2061  677-.    spike a
-00002180: 613a 2050 4153 533a 2031 3131 3848 2c20  a: PASS: 1118H, 
-00002190: 3134 342d 2c20 3530 3159 2c20 3537 3044  144-, 501Y, 570D
-000021a0: 2c20 3638 3148 2c20 3639 2d2c 2037 302d  , 681H, 69-, 70-
-000021b0: 2c20 3731 3649 2c20 3938 3241 0a20 2020  , 716I, 982A.   
-000021c0: 206f 7266 3820 6161 3a20 5041 5353 3a20   orf8 aa: PASS: 
-000021d0: 3532 492c 2037 3343 2c20 5132 372a 0a20  52I, 73C, Q27*. 
-000021e0: 2020 206e 2061 613a 2050 4153 533a 2032     n aa: PASS: 2
-000021f0: 3335 462c 2033 4c0a 6060 600a 0a54 6865  35F, 3L.```..The
-00002200: 7265 2061 7265 2073 6f6d 6520 6b6e 6f77  re are some know
-00002210: 6e20 7661 7269 616e 7473 2c20 616e 6420  n variants, and 
-00002220: 796f 7520 6361 6e20 616c 736f 2070 726f  you can also pro
-00002230: 7669 6465 2079 6f75 7220 6f77 6e20 7669  vide your own vi
-00002240: 6120 6120 4a53 4f4e 0a66 696c 6520 616e  a a JSON.file an
-00002250: 6420 7468 6520 602d 2d76 6172 6961 6e74  d the `--variant
-00002260: 4669 6c65 6020 6f70 7469 6f6e 2e20 452e  File` option. E.
-00002270: 672e 2c3a 0a0a 6060 600a 5641 5249 414e  g.,:..```.VARIAN
-00002280: 5453 203d 207b 0a20 2020 2027 564f 435f  TS = {.    'VOC_
-00002290: 3230 3230 3132 3031 5f55 4b27 3a20 7b0a  20201201_UK': {.
-000022a0: 2020 2020 2020 2020 2764 6573 6372 6970          'descrip
-000022b0: 7469 6f6e 273a 2027 554b 2076 6172 6961  tion': 'UK varia
-000022c0: 6e74 206f 6620 636f 6e63 6572 6e20 2856  nt of concern (V
-000022d0: 4f43 2920 3230 3230 3132 2f30 3127 2c0a  OC) 202012/01',.
-000022e0: 2020 2020 2020 2020 2763 6f6d 6d65 6e74          'comment
-000022f0: 273a 2028 2746 726f 6d20 5461 626c 6520  ': ('From Table 
-00002300: 3120 6f66 2068 7474 7073 3a2f 2f77 7777  1 of https://www
-00002310: 2e67 6f76 2e75 6b2f 676f 7665 726e 6d65  .gov.uk/governme
-00002320: 6e74 2f27 0a20 2020 2020 2020 2020 2020  nt/'.           
-00002330: 2020 2020 2020 2020 2027 7075 626c 6963           'public
-00002340: 6174 696f 6e73 2f69 6e76 6573 7469 6761  ations/investiga
-00002350: 7469 6f6e 2d6f 662d 6e6f 7665 6c2d 7361  tion-of-novel-sa
-00002360: 7273 2d63 6f76 2d32 270a 2020 2020 2020  rs-cov-2'.      
-00002370: 2020 2020 2020 2020 2020 2020 2020 272d                '-
-00002380: 7661 7269 616e 742d 7661 7269 616e 742d  variant-variant-
-00002390: 6f66 2d63 6f6e 6365 726e 2d32 3032 3031  of-concern-20201
-000023a0: 3230 3127 292c 0a20 2020 2020 2020 2027  201'),.        '
-000023b0: 6368 616e 6765 7327 3a20 7b0a 2020 2020  changes': {.    
-000023c0: 2020 2020 2020 2020 276f 7266 3161 6227          'orf1ab'
-000023d0: 3a20 7b0a 2020 2020 2020 2020 2020 2020  : {.            
-000023e0: 2020 2020 2761 6127 3a20 2731 3030 3149      'aa': '1001I
-000023f0: 2031 3730 3844 2032 3233 3054 2033 3637   1708D 2230T 367
-00002400: 352d 2033 3637 362d 2033 3637 372d 272c  5- 3676- 3677-',
-00002410: 0a20 2020 2020 2020 2020 2020 207d 2c0a  .            },.
-00002420: 2020 2020 2020 2020 2020 2020 2773 7069              'spi
-00002430: 6b65 273a 207b 0a20 2020 2020 2020 2020  ke': {.         
-00002440: 2020 2020 2020 2027 6161 273a 2027 3639         'aa': '69
-00002450: 2d20 3730 2d20 3134 342d 2035 3031 5920  - 70- 144- 501Y 
-00002460: 3537 3044 2036 3831 4820 3731 3649 2039  570D 681H 716I 9
-00002470: 3832 4120 3131 3138 4827 2c0a 2020 2020  82A 1118H',.    
-00002480: 2020 2020 2020 2020 7d2c 0a20 2020 2020          },.     
-00002490: 2020 2020 2020 2027 6f72 6638 273a 207b         'orf8': {
-000024a0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-000024b0: 2027 6161 273a 2027 5132 372a 2035 3249   'aa': 'Q27* 52I
-000024c0: 2037 3343 272c 0a20 2020 2020 2020 2020   73C',.         
-000024d0: 2020 207d 2c0a 2020 2020 2020 2020 2020     },.          
-000024e0: 2020 276e 273a 207b 0a20 2020 2020 2020    'n': {.       
-000024f0: 2020 2020 2020 2020 2027 6161 273a 2027           'aa': '
-00002500: 334c 2032 3335 4627 2c0a 2020 2020 2020  3L 235F',.      
-00002510: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
-00002520: 7d0a 2020 2020 7d0a 7d0a 6060 600a 0a23  }.    }.}.```..#
-00002530: 2320 6465 7363 7269 6265 2d73 6974 652e  # describe-site.
-00002540: 7079 0a0a 5769 6c6c 2070 7269 6e74 2069  py..Will print i
-00002550: 6e66 6f72 6d61 7469 6f6e 2061 626f 7574  nformation about
-00002560: 2061 2067 6976 656e 206c 6f63 6174 696f   a given locatio
-00002570: 6e20 2861 2022 7369 7465 2229 2069 6e20  n (a "site") in 
-00002580: 7468 6520 6765 6e6f 6d65 2c0a 7368 6f77  the genome,.show
-00002590: 696e 6720 796f 7520 7768 6174 2773 2069  ing you what's i
-000025a0: 6e20 7468 6520 7265 6665 7265 6e63 6520  n the reference 
-000025b0: 616e 6420 696e 2074 6865 2067 656e 6f6d  and in the genom
-000025c0: 6520 796f 7520 286f 7074 696f 6e61 6c6c  e you (optionall
-000025d0: 7929 0a70 6173 732e 0a0a 496e 2074 6865  y).pass...In the
-000025e0: 2073 696d 706c 6573 7420 6361 7365 2c20   simplest case, 
-000025f0: 6a75 7374 2067 6976 6520 6120 312d 6261  just give a 1-ba
-00002600: 7365 6420 7369 7465 2061 6e64 2079 6f75  sed site and you
-00002610: 276c 6c20 7365 6520 7768 6174 2773 2069  'll see what's i
-00002620: 6e20 7468 650a 7265 6665 7265 6e63 6520  n the.reference 
-00002630: 2877 6974 6820 302d 6261 7365 6420 5079  (with 0-based Py
-00002640: 7468 6f6e 206f 6666 7365 7473 293a 0a0a  thon offsets):..
-00002650: 6060 6073 680a 2420 6465 7363 7269 6265  ```sh.$ describe
-00002660: 2d73 6974 652e 7079 202d 2d73 6172 7332  -site.py --sars2
-00002670: 202d 2d73 6974 6520 3236 3030 300a 7b0a   --site 26000.{.
-00002680: 2020 2020 2261 6c69 676e 6d65 6e74 4f66      "alignmentOf
-00002690: 6673 6574 223a 2032 3539 3939 2c0a 2020  fset": 25999,.  
-000026a0: 2020 2266 6561 7475 7265 4e61 6d65 223a    "featureName":
-000026b0: 2022 4f52 4633 6120 7072 6f74 6569 6e22   "ORF3a protein"
-000026c0: 2c0a 2020 2020 2266 6561 7475 7265 4e61  ,.    "featureNa
-000026d0: 6d65 7322 3a20 5b0a 2020 2020 2020 2020  mes": [.        
-000026e0: 224f 5246 3361 2070 726f 7465 696e 220a  "ORF3a protein".
-000026f0: 2020 2020 5d2c 0a20 2020 2022 7265 6665      ],.    "refe
-00002700: 7265 6e63 6522 3a20 7b0a 2020 2020 2020  rence": {.      
-00002710: 2020 2261 6122 3a20 224c 222c 0a20 2020    "aa": "L",.   
-00002720: 2020 2020 2022 6161 4f66 6673 6574 223a       "aaOffset":
-00002730: 2032 3032 2c0a 2020 2020 2020 2020 2263   202,.        "c
-00002740: 6f64 6f6e 223a 2022 5454 4122 2c0a 2020  odon": "TTA",.  
-00002750: 2020 2020 2020 2266 7261 6d65 223a 2031        "frame": 1
-00002760: 2c0a 2020 2020 2020 2020 2269 6422 3a20  ,.        "id": 
-00002770: 224e 435f 3034 3535 3132 2e32 222c 0a20  "NC_045512.2",. 
-00002780: 2020 2020 2020 2022 6e74 4f66 6673 6574         "ntOffset
-00002790: 223a 2032 3539 3939 0a20 2020 207d 0a7d  ": 25999.    }.}
-000027a0: 0a60 6060 0a0a 4174 2074 6865 206d 6f6d  .```..At the mom
-000027b0: 656e 742c 2074 6865 2064 6566 6175 6c74  ent, the default
-000027c0: 206f 7574 7075 7420 6973 2061 204a 534f   output is a JSO
-000027d0: 4e20 6f62 6a65 6374 2c20 7468 6f75 6768  N object, though
-000027e0: 2074 6869 7320 6d61 7920 736f 6d65 6461   this may someda
-000027f0: 790a 6368 616e 6765 2074 6f20 6120 6d6f  y.change to a mo
-00002800: 7265 2076 6572 626f 7365 2f72 6561 6461  re verbose/reada
-00002810: 626c 6520 666f 726d 2e20 5573 6520 602d  ble form. Use `-
-00002820: 2d6a 736f 6e60 2074 6f20 6d61 6b65 2073  -json` to make s
-00002830: 7572 6520 796f 750a 616c 7761 7973 2067  ure you.always g
-00002840: 6574 204a 534f 4e2e 0a0a 596f 7520 6361  et JSON...You ca
-00002850: 6e20 616c 736f 2073 7065 6369 6679 2074  n also specify t
-00002860: 6865 2073 6974 6520 7265 6c61 7469 7665  he site relative
-00002870: 2074 6f20 6120 6665 6174 7572 653a 0a0a   to a feature:..
-00002880: 6060 6073 680a 2420 6465 7363 7269 6265  ```sh.$ describe
-00002890: 2d73 6974 652e 7079 202d 2d73 6172 7332  -site.py --sars2
-000028a0: 202d 2d73 6974 6520 3135 3031 202d 2d66   --site 1501 --f
-000028b0: 6561 7475 7265 2073 7069 6b65 202d 2d72  eature spike --r
-000028c0: 656c 6174 6976 650a 7b0a 2020 2020 2261  elative.{.    "a
-000028d0: 6c69 676e 6d65 6e74 4f66 6673 6574 223a  lignmentOffset":
-000028e0: 2032 3330 3632 2c0a 2020 2020 2266 6561   23062,.    "fea
-000028f0: 7475 7265 4e61 6d65 223a 2022 7375 7266  tureName": "surf
-00002900: 6163 6520 676c 7963 6f70 726f 7465 696e  ace glycoprotein
-00002910: 222c 0a20 2020 2022 6665 6174 7572 654e  ",.    "featureN
-00002920: 616d 6573 223a 205b 0a20 2020 2020 2020  ames": [.       
-00002930: 2022 7375 7266 6163 6520 676c 7963 6f70   "surface glycop
-00002940: 726f 7465 696e 220a 2020 2020 5d2c 0a20  rotein".    ],. 
-00002950: 2020 2022 7265 6665 7265 6e63 6522 3a20     "reference": 
-00002960: 7b0a 2020 2020 2020 2020 2261 6122 3a20  {.        "aa": 
-00002970: 224e 222c 0a20 2020 2020 2020 2022 6161  "N",.        "aa
-00002980: 4f66 6673 6574 223a 2035 3030 2c0a 2020  Offset": 500,.  
-00002990: 2020 2020 2020 2263 6f64 6f6e 223a 2022        "codon": "
-000029a0: 4141 5422 2c0a 2020 2020 2020 2020 2266  AAT",.        "f
-000029b0: 7261 6d65 223a 2030 2c0a 2020 2020 2020  rame": 0,.      
-000029c0: 2020 2269 6422 3a20 224e 435f 3034 3535    "id": "NC_0455
-000029d0: 3132 2e32 222c 0a20 2020 2020 2020 2022  12.2",.        "
-000029e0: 6e74 4f66 6673 6574 223a 2032 3330 3632  ntOffset": 23062
-000029f0: 0a20 2020 207d 0a7d 0a60 6060 0a0a 4f72  .    }.}.```..Or
-00002a00: 2070 6173 7320 616e 2061 6d69 6e6f 2061   pass an amino a
-00002a10: 6369 6420 7369 7465 206e 756d 6265 7220  cid site number 
-00002a20: 2876 6961 2060 2d2d 6161 6029 3a0a 0a60  (via `--aa`):..`
-00002a30: 6060 7368 0a24 2064 6573 6372 6962 652d  ``sh.$ describe-
-00002a40: 7369 7465 2e70 7920 2d2d 7361 7273 3220  site.py --sars2 
-00002a50: 2d2d 7369 7465 2035 3031 202d 2d66 6561  --site 501 --fea
-00002a60: 7475 7265 2073 7069 6b65 202d 2d72 656c  ture spike --rel
-00002a70: 6174 6976 6520 2d2d 6161 0a7b 0a20 2020  ative --aa.{.   
-00002a80: 2022 616c 6967 6e6d 656e 744f 6666 7365   "alignmentOffse
-00002a90: 7422 3a20 3233 3036 322c 0a20 2020 2022  t": 23062,.    "
-00002aa0: 6665 6174 7572 654e 616d 6522 3a20 2273  featureName": "s
-00002ab0: 7572 6661 6365 2067 6c79 636f 7072 6f74  urface glycoprot
-00002ac0: 6569 6e22 2c0a 2020 2020 2266 6561 7475  ein",.    "featu
-00002ad0: 7265 4e61 6d65 7322 3a20 5b0a 2020 2020  reNames": [.    
-00002ae0: 2020 2020 2273 7572 6661 6365 2067 6c79      "surface gly
-00002af0: 636f 7072 6f74 6569 6e22 0a20 2020 205d  coprotein".    ]
-00002b00: 2c0a 2020 2020 2272 6566 6572 656e 6365  ,.    "reference
-00002b10: 223a 207b 0a20 2020 2020 2020 2022 6161  ": {.        "aa
-00002b20: 223a 2022 4e22 2c0a 2020 2020 2020 2020  ": "N",.        
-00002b30: 2261 614f 6666 7365 7422 3a20 3530 302c  "aaOffset": 500,
-00002b40: 0a20 2020 2020 2020 2022 636f 646f 6e22  .        "codon"
-00002b50: 3a20 2241 4154 222c 0a20 2020 2020 2020  : "AAT",.       
-00002b60: 2022 6672 616d 6522 3a20 302c 0a20 2020   "frame": 0,.   
-00002b70: 2020 2020 2022 6964 223a 2022 4e43 5f30       "id": "NC_0
-00002b80: 3435 3531 322e 3222 2c0a 2020 2020 2020  45512.2",.      
-00002b90: 2020 226e 744f 6666 7365 7422 3a20 3233    "ntOffset": 23
-00002ba0: 3036 320a 2020 2020 7d0a 7d0a 6060 600a  062.    }.}.```.
-00002bb0: 0a4f 6620 636f 7572 7365 2069 7427 7320  .Of course it's 
-00002bc0: 6d6f 7265 2066 756e 2069 6620 796f 7520  more fun if you 
-00002bd0: 616c 736f 2070 726f 7669 6465 2061 2067  also provide a g
-00002be0: 656e 6f6d 6520 746f 2063 6f6d 7061 7265  enome to compare
-00002bf0: 2074 6865 2072 6566 6572 656e 6365 2074   the reference t
-00002c00: 6f2e 0a48 6572 6527 7320 7468 6520 604e  o..Here's the `N
-00002c10: 3530 3159 6020 6368 616e 6765 2069 6e20  501Y` change in 
-00002c20: 422e 312e 312e 3720 2841 6c70 6861 293a  B.1.1.7 (Alpha):
-00002c30: 0a0a 6060 6073 680a 2420 6465 7363 7269  ..```sh.$ descri
-00002c40: 6265 2d73 6974 652e 7079 202d 2d73 6172  be-site.py --sar
-00002c50: 7332 202d 2d73 6974 6520 3530 3120 2d2d  s2 --site 501 --
-00002c60: 7265 6c61 7469 7665 202d 2d67 656e 6f6d  relative --genom
-00002c70: 6520 4550 495f 4953 4c5f 3630 3134 3433  e EPI_ISL_601443
-00002c80: 2e66 6173 7461 202d 2d66 6561 7475 7265  .fasta --feature
-00002c90: 2073 7069 6b65 202d 2d61 610a 7b0a 2020   spike --aa.{.  
-00002ca0: 2020 2261 6c69 676e 6d65 6e74 4f66 6673    "alignmentOffs
-00002cb0: 6574 223a 2032 3330 3632 2c0a 2020 2020  et": 23062,.    
-00002cc0: 2266 6561 7475 7265 4e61 6d65 223a 2022  "featureName": "
-00002cd0: 7375 7266 6163 6520 676c 7963 6f70 726f  surface glycopro
-00002ce0: 7465 696e 222c 0a20 2020 2022 6665 6174  tein",.    "feat
-00002cf0: 7572 654e 616d 6573 223a 205b 0a20 2020  ureNames": [.   
-00002d00: 2020 2020 2022 7375 7266 6163 6520 676c       "surface gl
-00002d10: 7963 6f70 726f 7465 696e 220a 2020 2020  ycoprotein".    
-00002d20: 5d2c 0a20 2020 2022 6765 6e6f 6d65 223a  ],.    "genome":
-00002d30: 207b 0a20 2020 2020 2020 2022 6161 223a   {.        "aa":
-00002d40: 2022 5922 2c0a 2020 2020 2020 2020 2261   "Y",.        "a
-00002d50: 614f 6666 7365 7422 3a20 3439 372c 0a20  aOffset": 497,. 
-00002d60: 2020 2020 2020 2022 636f 646f 6e22 3a20         "codon": 
-00002d70: 2254 4154 222c 0a20 2020 2020 2020 2022  "TAT",.        "
-00002d80: 6672 616d 6522 3a20 302c 0a20 2020 2020  frame": 0,.     
-00002d90: 2020 2022 6964 223a 2022 4550 495f 4953     "id": "EPI_IS
-00002da0: 4c5f 3630 3134 3433 2068 436f 562d 3139  L_601443 hCoV-19
-00002db0: 2f45 6e67 6c61 6e64 2f4d 494c 4b2d 3945  /England/MILK-9E
-00002dc0: 3035 4233 2f32 3032 3022 2c0a 2020 2020  05B3/2020",.    
-00002dd0: 2020 2020 226e 744f 6666 7365 7422 3a20      "ntOffset": 
-00002de0: 3232 3939 300a 2020 2020 7d2c 0a20 2020  22990.    },.   
-00002df0: 2022 7265 6665 7265 6e63 6522 3a20 7b0a   "reference": {.
-00002e00: 2020 2020 2020 2020 2261 6122 3a20 224e          "aa": "N
-00002e10: 222c 0a20 2020 2020 2020 2022 6161 4f66  ",.        "aaOf
-00002e20: 6673 6574 223a 2035 3030 2c0a 2020 2020  fset": 500,.    
-00002e30: 2020 2020 2263 6f64 6f6e 223a 2022 4141      "codon": "AA
-00002e40: 5422 2c0a 2020 2020 2020 2020 2266 7261  T",.        "fra
-00002e50: 6d65 223a 2030 2c0a 2020 2020 2020 2020  me": 0,.        
-00002e60: 2269 6422 3a20 224e 435f 3034 3535 3132  "id": "NC_045512
-00002e70: 2e32 222c 0a20 2020 2020 2020 2022 6e74  .2",.        "nt
-00002e80: 4f66 6673 6574 223a 2032 3330 3632 0a20  Offset": 23062. 
-00002e90: 2020 207d 0a7d 0a60 6060 0a0a 4f74 6865     }.}.```..Othe
-00002ea0: 7220 6f70 7469 6f6e 7320 696e 636c 7564  r options includ
-00002eb0: 6520 602d 2d67 656e 6f6d 6541 614f 6e6c  e `--genomeAaOnl
-00002ec0: 7960 2074 6f20 6a75 7374 2070 7269 6e74  y` to just print
-00002ed0: 2074 6865 2061 6d69 6e6f 2061 6369 6420   the amino acid 
-00002ee0: 6174 2061 0a6c 6f63 6174 696f 6e20 696e  at a.location in
-00002ef0: 2074 6865 2067 656e 6f6d 652c 2060 2d2d   the genome, `--
-00002f00: 696e 636c 7564 6546 6561 7475 7265 6020  includeFeature` 
-00002f10: 746f 2061 6c73 6f20 7265 6365 6976 6520  to also receive 
-00002f20: 696e 666f 726d 6174 696f 6e0a 6162 6f75  information.abou
-00002f30: 7420 7468 6520 6665 6174 7572 6520 6174  t the feature at
-00002f40: 2074 6865 2073 6974 652c 2061 6e64 2060   the site, and `
-00002f50: 2d2d 6d69 6e52 6566 6572 656e 6365 436f  --minReferenceCo
-00002f60: 7665 7261 6765 6020 746f 2065 7863 6c75  verage` to exclu
-00002f70: 6465 0a6c 6f77 2d63 6f76 6572 6167 6520  de.low-coverage 
-00002f80: 6765 6e6f 6d65 7320 6f72 2066 6561 7475  genomes or featu
-00002f90: 7265 7320 6672 6f6d 2074 6865 2072 6573  res from the res
-00002fa0: 756c 7473 2e0a 0a23 2320 616e 6e6f 7461  ults...## annota
-00002fb0: 7465 2d67 656e 6f6d 652e 7079 0a0a 5072  te-genome.py..Pr
-00002fc0: 6f64 7563 6573 204a 534f 4e20 6f75 7470  oduces JSON outp
-00002fd0: 7574 2077 6974 6820 616e 6e6f 7461 7469  ut with annotati
-00002fe0: 6f6e 2069 6e66 6f72 6d61 7469 6f6e 2066  on information f
-00002ff0: 6f72 2061 2067 656e 6f6d 652e 2048 6572  or a genome. Her
-00003000: 6527 7320 616e 0a65 7861 6d70 6c65 206f  e's an.example o
-00003010: 6620 7468 6520 7374 6172 7420 6f66 206f  f the start of o
-00003020: 7574 7075 7420 666f 7220 6120 4d6f 6e6b  utput for a Monk
-00003030: 6579 706f 7820 6765 6e6f 6d65 2028 6e6f  eypox genome (no
-00003040: 7465 2074 6861 7420 7468 650a 6e75 636c  te that the.nucl
-00003050: 656f 7469 6465 2073 6571 7565 6e63 6573  eotide sequences
-00003060: 2068 6176 6520 6265 656e 2074 7275 6e63   have been trunc
-00003070: 6174 6564 2074 6f20 7265 6475 6365 206f  ated to reduce o
-00003080: 7574 7075 7420 7769 6474 6829 3a0a 0a60  utput width):..`
-00003090: 6060 7368 0a24 2061 6e6e 6f74 6174 652d  ``sh.$ annotate-
-000030a0: 6765 6e6f 6d65 2e70 7920 2d2d 616c 6967  genome.py --alig
-000030b0: 6e65 7220 6564 6c69 6220 2d2d 7265 6665  ner edlib --refe
-000030c0: 7265 6e63 6520 4f4e 3637 3637 3038 2e31  rence ON676708.1
-000030d0: 2e67 6220 2d2d 6765 6e6f 6d65 2043 6856  .gb --genome ChV
-000030e0: 6972 3238 3338 392e 6661 7374 610a 7b0a  ir28389.fasta.{.
-000030f0: 2020 2020 2266 6561 7475 7265 7322 3a20      "features": 
-00003100: 7b0a 2020 2020 2020 2020 2241 3135 2e35  {.        "A15.5
-00003110: 4c22 3a20 7b0a 2020 2020 2020 2020 2020  L": {.          
-00003120: 2020 2267 656e 6f6d 6522 3a20 7b0a 2020    "genome": {.  
-00003130: 2020 2020 2020 2020 2020 2020 2020 2273                "s
-00003140: 6571 7565 6e63 6522 3a20 2241 5447 4154  equence": "ATGAT
-00003150: 4141 4754 4141 5454 4143 4741 4743 4347  AAGTAATTACGAGCCG
-00003160: 5454 4743 5447 4354 4754 5441 4754 5441  TTGCTGCTGTTAGTTA
-00003170: 5441 4143 2e2e 2e22 2c0a 2020 2020 2020  TAAC...",.      
-00003180: 2020 2020 2020 2020 2020 2273 7461 7274            "start
-00003190: 223a 2031 3231 3832 332c 0a20 2020 2020  ": 121823,.     
-000031a0: 2020 2020 2020 2020 2020 2022 7374 6f70             "stop
-000031b0: 223a 2031 3231 3938 352c 0a20 2020 2020  ": 121985,.     
-000031c0: 2020 2020 2020 2020 2020 2022 7472 616e             "tran
-000031d0: 736c 6174 696f 6e22 3a20 224d 4953 4e59  slation": "MISNY
-000031e0: 4550 4c4c 4c4c 5649 5443 4356 4c4c 464e  EPLLLLVITCCVLLFN
-000031f0: 4654 4953 534b 544b 4944 4949 4641 5651  FTISSKTKIDIIFAVQ
-00003200: 5449 5646 4957 4649 4648 4656 5953 4149  TIVFIWFIFHFVYSAI
-00003210: 2a22 0a20 2020 2020 2020 2020 2020 207d  *".            }
-00003220: 2c0a 2020 2020 2020 2020 2020 2020 2272  ,.            "r
-00003230: 6566 6572 656e 6365 223a 207b 0a20 2020  eference": {.   
-00003240: 2020 2020 2020 2020 2020 2020 2022 666f               "fo
-00003250: 7277 6172 6422 3a20 6661 6c73 652c 0a20  rward": false,. 
-00003260: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00003270: 6e61 6d65 223a 2022 4131 352e 354c 222c  name": "A15.5L",
-00003280: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003290: 2022 6e6f 7465 223a 2022 4e6f 6e2d 6573   "note": "Non-es
-000032a0: 7365 6e74 6961 6c20 494d 5620 6d65 6d62  sential IMV memb
-000032b0: 7261 6e65 2070 726f 7465 696e 2028 436f  rane protein (Co
-000032c0: 702d 4131 342e 354c 2922 2c0a 2020 2020  p-A14.5L)",.    
-000032d0: 2020 2020 2020 2020 2020 2020 2270 726f              "pro
-000032e0: 6475 6374 223a 2022 4131 352e 354c 222c  duct": "A15.5L",
-000032f0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003300: 2022 7365 7175 656e 6365 223a 2022 5454   "sequence": "TT
-00003310: 4141 4154 4347 4343 4741 4154 4141 4143  AAATCGCCGAATAAAC
-00003320: 4141 4147 5447 4741 4154 4154 4141 4143  AAAGTGGAATATAAAC
-00003330: 4341 5441 5441 412e 2e2e 222c 0a20 2020  CATATAA...",.   
-00003340: 2020 2020 2020 2020 2020 2020 2022 7374               "st
-00003350: 6172 7422 3a20 3132 3137 3539 2c0a 2020  art": 121759,.  
-00003360: 2020 2020 2020 2020 2020 2020 2020 2273                "s
-00003370: 746f 7022 3a20 3132 3139 3231 2c0a 2020  top": 121921,.  
-00003380: 2020 2020 2020 2020 2020 2020 2020 2274                "t
-00003390: 7261 6e73 6c61 7469 6f6e 223a 2022 4d49  ranslation": "MI
-000033a0: 534e 5945 504c 4c4c 4c56 4954 4343 564c  SNYEPLLLLVITCCVL
-000033b0: 4c46 4e46 5449 5353 4b54 4b49 4449 4946  LFNFTISSKTKIDIIF
-000033c0: 4156 5154 4956 4649 5746 4946 4846 5659  AVQTIVFIWFIFHFVY
-000033d0: 5341 492a 220a 2020 2020 2020 2020 2020  SAI*".          
-000033e0: 2020 7d0a 2020 2020 2020 2020 7d2c 0a20    }.        },. 
-000033f0: 2020 2020 2020 2022 4133 322e 354c 223a         "A32.5L":
-00003400: 207b 0a20 2020 2020 2020 2020 2020 2022   {.            "
-00003410: 6765 6e6f 6d65 223a 207b 0a20 2020 2020  genome": {.     
-00003420: 2020 2020 2020 2020 2020 2022 7365 7175             "sequ
-00003430: 656e 6365 223a 2022 4154 4754 5441 4141  ence": "ATGTTAAA
-00003440: 4141 5447 5443 4147 4354 4743 4347 4143  AATGTCAGCTGCCGAC
-00003450: 5454 5454 5447 4741 4143 4754 5454 4741  TTTTTGGAACGTTTGA
-00003460: 542e 2e2e 222c 0a20 2020 2020 2020 2020  T...",.         
-00003470: 2020 2020 2020 2022 7374 6172 7422 3a20         "start": 
-00003480: 3133 3936 3936 2c0a 2020 2020 2020 2020  139696,.        
-00003490: 2020 2020 2020 2020 2273 746f 7022 3a20          "stop": 
-000034a0: 3133 3938 3235 2c0a 2020 2020 2020 2020  139825,.        
-000034b0: 2020 2020 2020 2020 2274 7261 6e73 6c61          "transla
-000034c0: 7469 6f6e 223a 2022 4d4c 4b4d 5341 4144  tion": "MLKMSAAD
-000034d0: 464c 4552 4c49 4b41 4749 5949 5956 4c52  FLERLIKAGIYIYVLR
-000034e0: 544b 5956 4954 414c 4c56 4b4e 5950 494b  TKYVITALLVKNYPIK
-000034f0: 4445 2a22 0a20 2020 2020 2020 2020 2020  DE*".           
-00003500: 207d 2c0a 2020 2020 2020 2020 2020 2020   },.            
-00003510: 2272 6566 6572 656e 6365 223a 207b 0a20  "reference": {. 
-00003520: 2020 2020 2020 2020 2020 2020 2020 2022                 "
-00003530: 666f 7277 6172 6422 3a20 6661 6c73 652c  forward": false,
-00003540: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00003550: 2022 6e61 6d65 223a 2022 4133 322e 354c   "name": "A32.5L
-00003560: 222c 0a20 2020 2020 2020 2020 2020 2020  ",.             
-00003570: 2020 2022 6e6f 7465 223a 2022 5669 7261     "note": "Vira
-00003580: 6c20 6d65 6d62 7261 6e65 2061 7373 656d  l membrane assem
-00003590: 626c 7920 7072 6f74 6569 6e73 2028 564d  bly proteins (VM
-000035a0: 4150 2920 2843 6f70 2d41 2033 302e 354c  AP) (Cop-A 30.5L
-000035b0: 2922 2c0a 2020 2020 2020 2020 2020 2020  )",.            
-000035c0: 2020 2020 2270 726f 6475 6374 223a 2022      "product": "
-000035d0: 4133 322e 354c 222c 0a20 2020 2020 2020  A32.5L",.       
-000035e0: 2020 2020 2020 2020 2022 7365 7175 656e           "sequen
-000035f0: 6365 223a 2022 5454 4154 5443 4754 4354  ce": "TTATTCGTCT
-00003600: 5454 5441 5447 4747 4154 4147 5454 5454  TTTATGGGATAGTTTT
-00003610: 5441 4143 5441 4754 4141 4147 4354 4754  TAACTAGTAAAGCTGT
-00003620: 4141 2e2e 2e22 2c0a 2020 2020 2020 2020  AA...",.        
-00003630: 2020 2020 2020 2020 2273 7461 7274 223a          "start":
-00003640: 2031 3339 3633 352c 0a20 2020 2020 2020   139635,.       
-00003650: 2020 2020 2020 2020 2022 7374 6f70 223a           "stop":
-00003660: 2031 3339 3736 342c 0a20 2020 2020 2020   139764,.       
-00003670: 2020 2020 2020 2020 2022 7472 616e 736c           "transl
-00003680: 6174 696f 6e22 3a20 224d 4c4b 4d53 4141  ation": "MLKMSAA
-00003690: 4446 4c45 524c 494b 4147 4959 4959 564c  DFLERLIKAGIYIYVL
-000036a0: 5254 4b59 5649 5441 4c4c 564b 4e59 5049  RTKYVITALLVKNYPI
-000036b0: 4b44 452a 220a 2020 2020 2020 2020 2020  KDE*".          
-000036c0: 2020 7d0a 2020 2020 2020 2020 7d2c 0a7d    }.        },.}
-000036d0: 0a60 6060 0a0a 2320 5079 7468 6f6e 2041  .```..# Python A
-000036e0: 5049 0a0a 5468 6572 6520 6172 6520 7477  PI..There are tw
-000036f0: 6f20 6d61 696e 2050 7974 686f 6e20 636c  o main Python cl
-00003700: 6173 7365 7320 7072 6f76 6964 6564 2062  asses provided b
-00003710: 7920 6067 6232 7365 7160 3a20 6046 6561  y `gb2seq`: `Fea
-00003720: 7475 7265 7360 2061 6e64 0a60 4762 3241  tures` and.`Gb2A
-00003730: 6c69 676e 6d65 6e74 602e 0a0a 2323 2046  lignment`...## F
-00003740: 6561 7475 7265 730a 0a54 6865 2060 4665  eatures..The `Fe
-00003750: 6174 7572 6573 6020 636c 6173 7320 7072  atures` class pr
-00003760: 6f76 6964 6573 206d 6574 686f 6473 2066  ovides methods f
-00003770: 6f72 2061 6363 6573 7369 6e67 2069 6e66  or accessing inf
-00003780: 6f72 6d61 7469 6f6e 2061 626f 7574 0a67  ormation about.g
-00003790: 656e 6f6d 6520 6665 6174 7572 6573 206f  enome features o
-000037a0: 6274 6169 6e65 6420 6672 6f6d 0a5b 6120  btained from.[a 
-000037b0: 4765 6e42 616e 6b20 666c 6174 2066 696c  GenBank flat fil
-000037c0: 655d 2868 7474 7073 3a2f 2f77 7777 2e6e  e](https://www.n
-000037d0: 6362 692e 6e6c 6d2e 6e69 682e 676f 762f  cbi.nlm.nih.gov/
-000037e0: 5369 7465 6d61 702f 7361 6d70 6c65 7265  Sitemap/samplere
-000037f0: 636f 7264 2e68 746d 6c29 2e0a 0a59 6f75  cord.html)...You
-00003800: 2776 6520 6c69 6b65 6c79 2072 756e 2061  've likely run a
-00003810: 6372 6f73 7320 7468 6573 6520 7265 636f  cross these reco
-00003820: 7264 7320 6265 666f 7265 2e20 452e 672e  rds before. E.g.
-00003830: 2c20 6865 7265 2773 2074 6865 2053 4152  , here's the SAR
-00003840: 532d 436f 562d 320a 5775 6861 6e20 7265  S-CoV-2.Wuhan re
-00003850: 6665 7265 6e63 652c 0a5b 4e43 5f30 3435  ference,.[NC_045
-00003860: 3531 325d 2868 7474 7073 3a2f 2f77 7777  512](https://www
-00003870: 2e6e 6362 692e 6e6c 6d2e 6e69 682e 676f  .ncbi.nlm.nih.go
-00003880: 762f 6e75 6363 6f72 652f 4e43 5f30 3435  v/nuccore/NC_045
-00003890: 3531 3229 2e20 546f 2064 6f77 6e6c 6f61  512). To downloa
-000038a0: 640a 7468 6520 4765 6e42 616e 6b20 6669  d.the GenBank fi
-000038b0: 6c65 2066 6f72 2074 6861 7420 7265 6665  le for that refe
-000038c0: 7265 6e63 652c 2063 6c69 636b 206f 6e20  rence, click on 
-000038d0: 2253 656e 6420 746f 2220 616e 6420 7365  "Send to" and se
-000038e0: 6c65 6374 0a22 436f 6d70 6c65 7465 2052  lect."Complete R
-000038f0: 6563 6f72 6422 2c20 2246 696c 6522 2c20  ecord", "File", 
-00003900: 616e 6420 2247 656e 4261 6e6b 2220 666f  and "GenBank" fo
-00003910: 726d 6174 2e20 5468 656e 2063 6c69 636b  rmat. Then click
-00003920: 2022 4372 6561 7465 2046 696c 6522 2e0a   "Create File"..
-00003930: 0a59 6f75 2063 616e 2070 6173 7320 7468  .You can pass th
-00003940: 6520 7061 7468 2074 6f20 6120 4765 6e42  e path to a GenB
-00003950: 616e 6b20 6669 6c65 2074 6f20 7468 6520  ank file to the 
-00003960: 6046 6561 7475 7265 7360 2063 6c61 7373  `Features` class
-00003970: 2e20 596f 7520 6361 6e0a 616c 736f 206a  . You can.also j
-00003980: 7573 7420 7061 7373 2061 6e20 6163 6365  ust pass an acce
-00003990: 7373 696f 6e20 6e75 6d62 6572 2c20 616e  ssion number, an
-000039a0: 6420 7468 6520 6669 6c65 2077 696c 6c20  d the file will 
-000039b0: 6265 2064 6f77 6e6c 6f61 6465 6420 666f  be downloaded fo
-000039c0: 720a 796f 752e 2049 6620 796f 7520 7061  r.you. If you pa
-000039d0: 7373 2060 7265 6665 7265 6e63 6553 7065  ss `referenceSpe
-000039e0: 6369 6669 6361 7469 6f6e 6020 6173 2060  cification` as `
-000039f0: 4e6f 6e65 6020 616e 6420 6073 6172 7332  None` and `sars2
-00003a00: 6020 6173 2060 5472 7565 602c 0a74 6865  ` as `True`,.the
-00003a10: 2057 7568 616e 2072 6566 6572 656e 6365   Wuhan reference
-00003a20: 2028 7665 7273 696f 6e0a 5b4e 435f 3034   (version.[NC_04
-00003a30: 3535 3132 2e32 5d28 6874 7470 733a 2f2f  5512.2](https://
-00003a40: 7777 772e 6e63 6269 2e6e 6c6d 2e6e 6968  www.ncbi.nlm.nih
-00003a50: 2e67 6f76 2f6e 7563 636f 7265 2f4e 435f  .gov/nuccore/NC_
-00003a60: 3034 3535 3132 2e32 2929 2077 696c 6c20  045512.2)) will 
-00003a70: 6265 0a75 7365 642e 0a0a 596f 7520 6361  be.used...You ca
-00003a80: 6e20 7573 6520 6120 6046 6561 7475 7265  n use a `Feature
-00003a90: 7360 2069 6e73 7461 6e63 6520 6c69 6b65  s` instance like
-00003aa0: 2061 2064 6963 7469 6f6e 6172 793a 0a0a   a dictionary:..
-00003ab0: 6060 6070 790a 6672 6f6d 2070 7072 696e  ```py.from pprin
-00003ac0: 7420 696d 706f 7274 2070 7072 696e 7420  t import pprint 
-00003ad0: 6173 2070 700a 6672 6f6d 2067 6232 7365  as pp.from gb2se
-00003ae0: 712e 6665 6174 7572 6573 2069 6d70 6f72  q.features impor
-00003af0: 7420 4665 6174 7572 6573 0a0a 3e3e 3e20  t Features..>>> 
-00003b00: 6620 3d20 4665 6174 7572 6573 2822 4e43  f = Features("NC
-00003b10: 5f30 3435 3531 322e 322e 6762 2229 0a3e  _045512.2.gb").>
-00003b20: 3e3e 2070 7028 665b 2765 275d 290a 7b27  >> pp(f['e']).{'
-00003b30: 6e61 6d65 273a 2027 656e 7665 6c6f 7065  name': 'envelope
-00003b40: 2070 726f 7465 696e 272c 0a20 276e 6f74   protein',. 'not
-00003b50: 6527 3a20 274f 5246 343b 2073 7472 7563  e': 'ORF4; struc
-00003b60: 7475 7261 6c20 7072 6f74 6569 6e3b 2045  tural protein; E
-00003b70: 2070 726f 7465 696e 272c 0a20 2770 726f   protein',. 'pro
-00003b80: 6475 6374 273a 2027 656e 7665 6c6f 7065  duct': 'envelope
-00003b90: 2070 726f 7465 696e 272c 0a20 2773 6571   protein',. 'seq
-00003ba0: 7565 6e63 6527 3a20 2741 5447 5441 4354  uence': 'ATGTACT
-00003bb0: 4341 5454 4347 5454 5443 4747 4141 4741  CATTCGTTTCGGAAGA
-00003bc0: 4741 4341 4747 5441 4347 5454 4141 5441  GACAGGTACGTTAATA
-00003bd0: 4754 5441 4154 4147 4347 5441 4354 5443  GTTAATAGCGTACTTC
-00003be0: 5454 5454 5443 5454 4743 5454 5443 4754  TTTTTCTTGCTTTCGT
-00003bf0: 4747 5441 5454 2e2e 2e27 2c0a 2027 7374  GGTATT...',. 'st
-00003c00: 6172 7427 3a20 3236 3234 342c 0a20 2773  art': 26244,. 's
-00003c10: 746f 7027 3a20 3236 3437 322c 0a20 2774  top': 26472,. 't
-00003c20: 7261 6e73 6c61 7469 6f6e 273a 2027 4d59  ranslation': 'MY
-00003c30: 5346 5653 4545 5447 544c 4956 4e53 564c  SFVSEETGTLIVNSVL
-00003c40: 4c46 4c41 4656 5646 4c4c 5654 4c41 494c  LFLAFVVFLLVTLAIL
-00003c50: 5441 4c52 4c43 4159 4343 4e49 564e 5653  TALRLCAYCCNIVNVS
-00003c60: 4c56 4b50 5346 5956 5953 5256 4b4e 4c4e  LVKPSFYVYSRVKNLN
-00003c70: 5353 5256 5044 4c4c 562a 277d 0a0a 2320  SSRVPDLLV*'}..# 
-00003c80: 596f 7520 6361 6e20 7573 6520 6162 6272  You can use abbr
-00003c90: 6576 6961 7465 6420 6e61 6d65 732c 2061  eviated names, a
-00003ca0: 6e64 2067 6574 2074 6865 2063 616e 6f6e  nd get the canon
-00003cb0: 6963 616c 206e 616d 6573 3a0a 3e3e 3e20  ical names:.>>> 
-00003cc0: 662e 6361 6e6f 6e69 6361 6c4e 616d 6528  f.canonicalName(
-00003cd0: 2773 2729 0a27 7375 7266 6163 6520 676c  's').'surface gl
-00003ce0: 7963 6f70 726f 7465 696e 270a 0a23 2047  ycoprotein'..# G
-00003cf0: 6574 2074 6865 206c 6973 7420 6f66 2061  et the list of a
-00003d00: 6c69 6173 6573 2066 6f72 2061 206e 616d  liases for a nam
-00003d10: 653a 0a3e 3e3e 2066 2e61 6c69 6173 6573  e:.>>> f.aliases
-00003d20: 2827 7327 290a 7b27 7370 696b 6527 2c20  ('s').{'spike', 
-00003d30: 2773 7572 6661 6365 2067 6c79 636f 7072  'surface glycopr
-00003d40: 6f74 6569 6e27 2c20 2773 277d 0a0a 2320  otein', 's'}..# 
-00003d50: 4769 7665 6e20 616e 206f 6666 7365 7420  Given an offset 
-00003d60: 7265 6c61 7469 7665 2074 6f20 6120 6665  relative to a fe
-00003d70: 6174 7572 652c 2067 6574 2074 6865 206f  ature, get the o
-00003d80: 6666 7365 7420 696e 2074 6865 2067 656e  ffset in the gen
-00003d90: 6f6d 653a 0a3e 3e3e 2066 2e72 6566 6572  ome:.>>> f.refer
-00003da0: 656e 6365 4f66 6673 6574 2827 7370 696b  enceOffset('spik
-00003db0: 6527 2c20 3135 3033 290a 3233 3036 350a  e', 1503).23065.
-00003dc0: 0a23 2053 616d 6520 7468 696e 672c 2062  .# Same thing, b
-00003dd0: 7574 2077 6974 6820 616e 2061 6d69 6e6f  ut with an amino
-00003de0: 2061 6369 6420 6f66 6673 6574 2e0a 3e3e   acid offset..>>
-00003df0: 3e20 662e 7265 6665 7265 6e63 654f 6666  > f.referenceOff
-00003e00: 7365 7428 2773 7069 6b65 272c 2035 3031  set('spike', 501
-00003e10: 2c20 6161 3d54 7275 6529 0a32 3330 3635  , aa=True).23065
-00003e20: 0a0a 2320 5768 6174 2066 6561 7475 7265  ..# What feature
-00003e30: 7320 6172 6520 7072 6573 656e 7420 6174  s are present at
-00003e40: 2061 6e20 6f66 6673 6574 3f0a 3e3e 3e20   an offset?.>>> 
-00003e50: 662e 6765 7446 6561 7475 7265 4e61 6d65  f.getFeatureName
-00003e60: 7328 3133 3435 3029 0a7b 274f 5246 3161  s(13450).{'ORF1a
-00003e70: 6220 706f 6c79 7072 6f74 6569 6e27 2c20  b polyprotein', 
-00003e80: 276e 7370 3131 272c 2027 4f52 4631 6120  'nsp11', 'ORF1a 
-00003e90: 706f 6c79 7072 6f74 6569 6e27 2c20 2752  polyprotein', 'R
-00003ea0: 4e41 2d64 6570 656e 6465 6e74 2052 4e41  NA-dependent RNA
-00003eb0: 2070 6f6c 796d 6572 6173 6527 7d0a 0a23   polymerase'}..#
-00003ec0: 2057 6861 7420 6665 6174 7572 6573 2061   What features a
-00003ed0: 7265 2070 7265 7365 6e74 2061 7420 616e  re present at an
-00003ee0: 206f 6666 7365 742c 2069 6e63 6c75 6469   offset, includi
-00003ef0: 6e67 2074 686f 7365 2074 6861 7420 6172  ng those that ar
-00003f00: 6520 6e6f 7420 7472 616e 736c 6174 6564  e not translated
-00003f10: 3f0a 3e3e 3e20 662e 6765 7446 6561 7475  ?.>>> f.getFeatu
-00003f20: 7265 4e61 6d65 7328 3231 3030 302c 2069  reNames(21000, i
-00003f30: 6e63 6c75 6465 556e 7472 616e 736c 6174  ncludeUntranslat
-00003f40: 6564 3d54 7275 6529 0a7b 274f 5246 3161  ed=True).{'ORF1a
-00003f50: 6220 706f 6c79 7072 6f74 6569 6e27 2c20  b polyprotein', 
-00003f60: 2232 272d 4f2d 7269 626f 7365 206d 6574  "2'-O-ribose met
-00003f70: 6879 6c74 7261 6e73 6665 7261 7365 227d  hyltransferase"}
-00003f80: 0a60 6060 0a0a 2323 2047 6232 416c 6967  .```..## Gb2Alig
-00003f90: 6e6d 656e 740a 0a54 6865 2060 4762 3241  nment..The `Gb2A
-00003fa0: 6c69 676e 6d65 6e74 6020 636c 6173 7320  lignment` class 
-00003fb0: 6361 6e20 6265 2075 7365 6420 746f 2065  can be used to e
-00003fc0: 7874 7261 6374 2061 6e64 2063 6f6d 7061  xtract and compa
-00003fd0: 7265 2066 6561 7475 7265 7320 6672 6f6d  re features from
-00003fe0: 0a74 6865 2072 6566 6572 656e 6365 2061  .the reference a
-00003ff0: 6e64 2074 6865 2067 6976 656e 2067 656e  nd the given gen
-00004000: 6f6d 6520 7365 7175 656e 6365 2e0a 0a59  ome sequence...Y
-00004010: 6f75 2070 6173 7320 6974 2061 2060 5265  ou pass it a `Re
-00004020: 6164 6020 696e 7374 616e 6365 2066 726f  ad` instance fro
-00004030: 6d20 7468 650a 5b64 6172 6b2d 6d61 7474  m the.[dark-matt
-00004040: 6572 5d28 6874 7470 733a 2f2f 6769 7468  er](https://gith
-00004050: 7562 2e63 6f6d 2f61 636f 7267 2f64 6172  ub.com/acorg/dar
-00004060: 6b2d 6d61 7474 6572 2920 6d6f 6475 6c65  k-matter) module
-00004070: 2028 7768 6963 6820 6973 0a69 6e73 7461   (which is.insta
-00004080: 6c6c 6564 2066 6f72 2079 6f75 2077 6865  lled for you whe
-00004090: 6e20 796f 7520 696e 7374 616c 6c20 6067  n you install `g
-000040a0: 6232 7365 7160 292e 0a0a 6060 6070 790a  b2seq`)...```py.
-000040b0: 6672 6f6d 2067 6232 7365 712e 616c 6967  from gb2seq.alig
-000040c0: 6e6d 656e 7420 696d 706f 7274 2047 6232  nment import Gb2
-000040d0: 416c 6967 6e6d 656e 740a 6672 6f6d 2064  Alignment.from d
-000040e0: 6172 6b2e 7265 6164 7320 696d 706f 7274  ark.reads import
-000040f0: 2052 6561 640a 0a61 6c69 676e 6d65 6e74   Read..alignment
-00004100: 203d 2047 6232 416c 6967 6e6d 656e 7428   = Gb2Alignment(
-00004110: 5265 6164 2827 6964 272c 2027 4147 4354  Read('id', 'AGCT
-00004120: 2e2e 2e27 2929 0a60 6060 0a0a 5468 6573  ...')).```..Thes
-00004130: 6520 6361 6e20 616c 736f 2062 6520 7265  e can also be re
-00004140: 6164 2066 726f 6d20 6120 4641 5354 4120  ad from a FASTA 
-00004150: 6669 6c65 3a0a 0a60 6060 7079 0a66 726f  file:..```py.fro
-00004160: 6d20 6762 3273 6571 2e61 6c69 676e 6d65  m gb2seq.alignme
-00004170: 6e74 2069 6d70 6f72 7420 4762 3241 6c69  nt import Gb2Ali
-00004180: 676e 6d65 6e74 0a66 726f 6d20 6461 726b  gnment.from dark
-00004190: 2e66 6173 7461 2069 6d70 6f72 7420 4661  .fasta import Fa
-000041a0: 7374 6152 6561 6473 0a0a 666f 7220 7265  staReads..for re
-000041b0: 6164 2069 6e20 4661 7374 6152 6561 6473  ad in FastaReads
-000041c0: 2827 7365 7175 656e 6365 732e 6661 7374  ('sequences.fast
-000041d0: 6127 293a 0a20 2020 2061 6c69 676e 6d65  a'):.    alignme
-000041e0: 6e74 203d 2047 6232 416c 6967 6e6d 656e  nt = Gb2Alignmen
-000041f0: 7428 7265 6164 290a 6060 600a 0a4f 6e63  t(read).```..Onc
-00004200: 6520 796f 7520 6861 7665 2061 2060 4762  e you have a `Gb
-00004210: 3241 6c69 676e 6d65 6e74 6020 696e 7374  2Alignment` inst
-00004220: 616e 6365 2c20 796f 7520 6361 6e20 6173  ance, you can as
-00004230: 6b20 6974 2066 6f72 2074 6865 2061 6c69  k it for the ali
-00004240: 676e 6564 0a73 6571 7565 6e63 6573 206f  gned.sequences o
-00004250: 7220 6665 6174 7572 6573 2e0a 0a42 656c  r features...Bel
-00004260: 6f77 2049 276c 6c20 7573 6520 7468 6520  ow I'll use the 
-00004270: 4749 5341 4944 2060 4550 495f 4953 4c5f  GISAID `EPI_ISL_
-00004280: 3630 3134 3433 6020 2842 2e31 2e31 2e37  601443` (B.1.1.7
-00004290: 2c20 6f72 2041 6c70 6861 2c20 7661 7269  , or Alpha, vari
-000042a0: 616e 7429 0a73 6571 7565 6e63 652c 2077  ant).sequence, w
-000042b0: 6869 6368 2079 6f75 2063 616e 2066 696e  hich you can fin
-000042c0: 6420 696e 0a5b 6461 7461 2f45 5049 5f49  d in.[data/EPI_I
-000042d0: 534c 5f36 3031 3434 332e 6661 7374 615d  SL_601443.fasta]
-000042e0: 2864 6174 612f 4550 495f 4953 4c5f 3630  (data/EPI_ISL_60
-000042f0: 3134 3433 2e66 6173 7461 2920 696e 2074  1443.fasta) in t
-00004300: 6869 7320 7265 706f 3a0a 0a60 6060 7079  his repo:..```py
-00004310: 0a3e 3e3e 2066 726f 6d20 7061 7468 6c69  .>>> from pathli
-00004320: 6220 696d 706f 7274 2050 6174 680a 3e3e  b import Path.>>
-00004330: 3e20 6672 6f6d 2070 7072 696e 7420 696d  > from pprint im
-00004340: 706f 7274 2070 7072 696e 7420 6173 2070  port pprint as p
-00004350: 700a 3e3e 3e20 6672 6f6d 2067 6232 7365  p.>>> from gb2se
-00004360: 712e 616c 6967 6e6d 656e 7420 696d 706f  q.alignment impo
-00004370: 7274 2047 6232 416c 6967 6e6d 656e 740a  rt Gb2Alignment.
-00004380: 3e3e 3e20 6672 6f6d 2064 6172 6b2e 6661  >>> from dark.fa
-00004390: 7374 6120 696d 706f 7274 2046 6173 7461  sta import Fasta
-000043a0: 5265 6164 730a 0a3e 3e3e 2061 6c70 6861  Reads..>>> alpha
-000043b0: 203d 206c 6973 7428 4661 7374 6152 6561   = list(FastaRea
-000043c0: 6473 2850 6174 6828 2764 6174 612f 4550  ds(Path('data/EP
-000043d0: 495f 4953 4c5f 3630 3134 3433 2e66 6173  I_ISL_601443.fas
-000043e0: 7461 2729 2929 5b30 5d0a 3e3e 3e20 6c65  ta')))[0].>>> le
-000043f0: 6e28 616c 7068 6129 0a32 3937 3634 0a3e  n(alpha).29764.>
-00004400: 3e3e 2061 6c70 6861 2e69 640a 2745 5049  >> alpha.id.'EPI
-00004410: 5f49 534c 5f36 3031 3434 3320 6843 6f56  _ISL_601443 hCoV
-00004420: 2d31 392f 456e 676c 616e 642f 4d49 4c4b  -19/England/MILK
-00004430: 2d39 4530 3542 332f 3230 3230 270a 3e3e  -9E05B3/2020'.>>
-00004440: 3e20 616c 7068 612e 7365 7175 656e 6365  > alpha.sequence
-00004450: 5b3a 3530 5d0a 2741 4741 5443 5447 5454  [:50].'AGATCTGTT
-00004460: 4354 4354 4141 4143 4741 4143 5454 5441  CTCTAAACGAACTTTA
-00004470: 4141 4154 4354 4754 4754 4747 4354 4754  AAATCTGTGTGGCTGT
-00004480: 4341 4354 4347 4743 5427 0a0a 3e3e 3e20  CACTCGGCT'..>>> 
-00004490: 616c 6967 6e6d 656e 7420 3d20 4762 3241  alignment = Gb2A
-000044a0: 6c69 676e 6d65 6e74 2861 6c70 6861 290a  lignment(alpha).
-000044b0: 6060 600a 0a59 6f75 276c 6c20 6669 6e64  ```..You'll find
-000044c0: 2074 6865 2061 6c69 676e 6564 2072 6566   the aligned ref
-000044d0: 6572 656e 6365 2061 6e64 2067 656e 6f6d  erence and genom
-000044e0: 6520 696e 2060 616c 6967 6e6d 656e 742e  e in `alignment.
-000044f0: 7265 6665 7265 6e63 6541 6c69 676e 6564  referenceAligned
-00004500: 600a 616e 6420 6061 6c69 676e 6d65 6e74  `.and `alignment
-00004510: 2e67 656e 6f6d 6541 6c69 676e 6564 602c  .genomeAligned`,
-00004520: 2062 6f74 6820 6f66 2077 6869 6368 2061   both of which a
-00004530: 7265 2020 6052 6561 6460 2069 6e73 7461  re  `Read` insta
-00004540: 6e63 6573 3a0a 0a60 6060 7079 0a3e 3e3e  nces:..```py.>>>
-00004550: 206c 656e 2861 6c69 676e 6d65 6e74 2e72   len(alignment.r
-00004560: 6566 6572 656e 6365 416c 6967 6e65 6429  eferenceAligned)
-00004570: 0a32 3939 3033 0a3e 3e3e 206c 656e 2861  .29903.>>> len(a
-00004580: 6c69 676e 6d65 6e74 2e67 656e 6f6d 6541  lignment.genomeA
-00004590: 6c69 676e 6564 290a 3239 3930 330a 0a23  ligned).29903..#
-000045a0: 2047 6574 2074 6865 206e 7563 6c65 6f74   Get the nucleot
-000045b0: 6964 6520 7365 7175 656e 6365 2066 6f72  ide sequence for
-000045c0: 2074 6865 2073 7069 6b65 2070 726f 7465   the spike prote
-000045d0: 696e 2066 6f72 2074 6865 2072 6566 6572  in for the refer
-000045e0: 656e 6365 2061 6e64 2067 656e 6f6d 652e  ence and genome.
-000045f0: 0a3e 3e3e 2072 6566 6572 656e 6365 5370  .>>> referenceSp
-00004600: 696b 654e 742c 2067 656e 6f6d 6553 7069  ikeNt, genomeSpi
-00004610: 6b65 4e74 203d 2061 6c69 676e 6d65 6e74  keNt = alignment
-00004620: 2e6e 7453 6571 7565 6e63 6573 2827 7370  .ntSequences('sp
-00004630: 696b 6527 290a 3e3e 3e20 6c65 6e28 7265  ike').>>> len(re
-00004640: 6665 7265 6e63 6553 7069 6b65 4e74 290a  ferenceSpikeNt).
-00004650: 3338 3232 0a0a 2320 4765 7420 7468 6520  3822..# Get the 
-00004660: 616d 696e 6f20 6163 6964 2073 6571 7565  amino acid seque
-00004670: 6e63 6520 666f 7220 7468 6520 7370 696b  nce for the spik
-00004680: 6520 7072 6f74 6569 6e20 666f 7220 7468  e protein for th
-00004690: 6520 7265 6665 7265 6e63 6520 616e 6420  e reference and 
-000046a0: 6765 6e6f 6d65 2e0a 3e3e 3e20 7265 6665  genome..>>> refe
-000046b0: 7265 6e63 6553 7069 6b65 4161 2c20 6765  renceSpikeAa, ge
-000046c0: 6e6f 6d65 5370 696b 6541 6120 3d20 616c  nomeSpikeAa = al
-000046d0: 6967 6e6d 656e 742e 6161 5365 7175 656e  ignment.aaSequen
-000046e0: 6365 7328 2773 7069 6b65 2729 0a3e 3e3e  ces('spike').>>>
-000046f0: 206c 656e 2872 6566 6572 656e 6365 5370   len(referenceSp
-00004700: 696b 6541 6129 0a31 3237 340a 0a23 2054  ikeAa).1274..# T
-00004710: 6865 7265 2077 6572 6520 7468 7265 6520  here were three 
-00004720: 6465 6c65 7469 6f6e 7320 696e 2074 6865  deletions in the
-00004730: 2061 6c70 6861 2073 7069 6b65 2c20 736f   alpha spike, so
-00004740: 2069 7420 6f6e 6c79 2063 6f76 6572 7320   it only covers 
-00004750: 3338 3133 206f 6620 7468 650a 2320 3338  3813 of the.# 38
-00004760: 3232 2062 6173 6573 2069 6e20 7468 6520  22 bases in the 
-00004770: 7265 6665 7265 6e63 6520 7370 696b 652e  reference spike.
-00004780: 0a3e 3e3e 2061 6c69 676e 6d65 6e74 2e63  .>>> alignment.c
-00004790: 6f76 6572 6167 6528 2773 2729 0a28 3338  overage('s').(38
-000047a0: 3133 2c20 3338 3232 290a 0a23 2047 6574  13, 3822)..# Get
-000047b0: 2069 6e66 6f72 6d61 7469 6f6e 2061 626f   information abo
-000047c0: 7574 2077 6861 7427 7320 6174 2061 6e20  ut what's at an 
-000047d0: 6f66 6673 6574 2028 302d 6261 7365 6429  offset (0-based)
-000047e0: 2e20 5468 6973 2069 7320 7768 6174 2074  . This is what t
-000047f0: 6865 2064 6573 6372 6962 652d 7369 7465  he describe-site
-00004800: 2e70 790a 2320 7574 696c 6974 7920 646f  .py.# utility do
-00004810: 6573 2028 7468 6f75 6768 2069 7420 7461  es (though it ta
-00004820: 6b65 7320 6120 312d 6261 7365 6420 7369  kes a 1-based si
-00004830: 7465 292e 0a23 0a23 2048 6572 6520 6973  te)..#.# Here is
-00004840: 2074 6865 2041 6c70 6861 204e 3530 3159   the Alpha N501Y
-00004850: 2063 6861 6e67 653a 0a3e 3e3e 2070 7028   change:.>>> pp(
-00004860: 616c 6967 6e6d 656e 742e 6f66 6673 6574  alignment.offset
-00004870: 496e 666f 2835 3030 2c20 7265 6c61 7469  Info(500, relati
-00004880: 7665 546f 4665 6174 7572 653d 5472 7565  veToFeature=True
-00004890: 2c20 6161 3d54 7275 652c 2066 6561 7475  , aa=True, featu
-000048a0: 7265 4e61 6d65 3d27 7327 2929 0a7b 2766  reName='s')).{'f
-000048b0: 6561 7475 7265 4e61 6d65 273a 2027 7375  eatureName': 'su
-000048c0: 7266 6163 6520 676c 7963 6f70 726f 7465  rface glycoprote
-000048d0: 696e 272c 0a20 2766 6561 7475 7265 4e61  in',. 'featureNa
-000048e0: 6d65 7327 3a20 7b27 7375 7266 6163 6520  mes': {'surface 
-000048f0: 676c 7963 6f70 726f 7465 696e 277d 2c0a  glycoprotein'},.
-00004900: 2027 616c 6967 6e6d 656e 744f 6666 7365   'alignmentOffse
-00004910: 7427 3a20 3233 3036 322c 0a20 2772 6566  t': 23062,. 'ref
-00004920: 6572 656e 6365 273a 207b 2761 6127 3a20  erence': {'aa': 
-00004930: 274e 272c 0a20 2027 636f 646f 6e27 3a20  'N',.  'codon': 
-00004940: 2741 4154 272c 0a20 2027 6672 616d 6527  'AAT',.  'frame'
-00004950: 3a20 302c 0a20 2027 6964 273a 2027 4e43  : 0,.  'id': 'NC
-00004960: 5f30 3435 3531 322e 3227 2c0a 2020 2761  _045512.2',.  'a
-00004970: 614f 6666 7365 7427 3a20 3530 302c 0a20  aOffset': 500,. 
-00004980: 2027 6e74 4f66 6673 6574 273a 2032 3330   'ntOffset': 230
-00004990: 3632 7d2c 0a20 2767 656e 6f6d 6527 3a20  62},. 'genome': 
-000049a0: 7b27 6161 273a 2027 5927 2c0a 2020 2763  {'aa': 'Y',.  'c
-000049b0: 6f64 6f6e 273a 2027 5441 5427 2c0a 2020  odon': 'TAT',.  
-000049c0: 2766 7261 6d65 273a 2030 2c0a 2020 2769  'frame': 0,.  'i
-000049d0: 6427 3a20 2745 5049 5f49 534c 5f36 3031  d': 'EPI_ISL_601
-000049e0: 3434 3320 6843 6f56 2d31 392f 456e 676c  443 hCoV-19/Engl
-000049f0: 616e 642f 4d49 4c4b 2d39 4530 3542 332f  and/MILK-9E05B3/
-00004a00: 3230 3230 272c 0a20 2027 6161 4f66 6673  2020',.  'aaOffs
-00004a10: 6574 273a 2034 3937 2c0a 2020 276e 744f  et': 497,.  'ntO
-00004a20: 6666 7365 7427 3a20 3232 3939 307d 7d0a  ffset': 22990}}.
-00004a30: 6060 600a 0a59 6f75 2063 616e 2063 6865  ```..You can che
-00004a40: 636b 2061 2066 6561 7475 7265 2066 6f72  ck a feature for
-00004a50: 2061 6e20 6578 7065 6374 6564 2063 6861   an expected cha
-00004a60: 6e67 653a 0a0a 6060 6020 7079 0a3e 3e3e  nge:..``` py.>>>
-00004a70: 2061 6c69 676e 6d65 6e74 2e63 6865 636b   alignment.check
-00004a80: 4665 6174 7572 6528 2773 7069 6b65 272c  Feature('spike',
-00004a90: 2027 4e35 3031 5927 2c20 6161 3d54 7275   'N501Y', aa=Tru
-00004aa0: 6529 0a28 312c 2030 2c20 7b27 4e35 3031  e).(1, 0, {'N501
-00004ab0: 5927 3a20 2854 7275 652c 2027 4e27 2c20  Y': (True, 'N', 
-00004ac0: 5472 7565 2c20 2759 2729 7d29 0a60 6060  True, 'Y')}).```
-00004ad0: 0a0a 5468 6520 7265 7475 726e 2076 616c  ..The return val
-00004ae0: 7565 2067 6976 6573 2074 6865 206e 756d  ue gives the num
-00004af0: 6265 7220 6f66 2074 6573 7473 2064 6f6e  ber of tests don
-00004b00: 6520 2831 292c 2074 6865 206e 756d 6265  e (1), the numbe
-00004b10: 7220 7468 6174 2066 6169 6c65 640a 2830  r that failed.(0
-00004b20: 292c 2061 6e64 2061 2060 6469 6374 6020  ), and a `dict` 
-00004b30: 7769 7468 2069 6e66 6f72 6d61 7469 6f6e  with information
-00004b40: 2061 626f 7574 2065 6163 6820 7465 7374   about each test
-00004b50: 2e20 5468 6520 6064 6963 7460 2076 616c  . The `dict` val
-00004b60: 7565 7320 6172 650a 342d 7475 706c 6573  ues are.4-tuples
-00004b70: 2c20 696e 6469 6361 7469 6e67 2077 6865  , indicating whe
-00004b80: 7468 6572 2077 6861 7420 7761 7320 696e  ther what was in
-00004b90: 2074 6865 2072 6566 6572 656e 6365 2077   the reference w
-00004ba0: 6173 2061 7320 6578 7065 6374 6564 0a28  as as expected.(
-00004bb0: 6054 7275 6560 292c 2074 6865 2076 616c  `True`), the val
-00004bc0: 7565 2069 6e20 7468 6520 7265 6665 7265  ue in the refere
-00004bd0: 6e63 6520 2860 4e60 292c 2077 6865 7468  nce (`N`), wheth
-00004be0: 6572 2077 6861 7420 7761 7320 696e 2074  er what was in t
-00004bf0: 6865 2067 656e 6f6d 6520 7761 730a 6173  he genome was.as
-00004c00: 2065 7870 6563 7465 6420 2860 5472 7565   expected (`True
-00004c10: 6029 2c20 7468 6520 7661 6c75 6520 696e  `), the value in
-00004c20: 2074 6865 2067 656e 6f6d 6520 2860 5960   the genome (`Y`
-00004c30: 292e 0a0a 596f 7520 6361 6e20 7465 7374  )...You can test
-00004c40: 206d 756c 7469 706c 6520 7468 696e 6773   multiple things
-00004c50: 3a0a 0a60 6060 2070 790a 2320 4e6f 7465  :..``` py.# Note
-00004c60: 2074 6861 7420 7765 2075 7365 2035 3031   that we use 501
-00004c70: 5920 696e 2074 6865 2066 6f6c 6c6f 7769  Y in the followi
-00004c80: 6e67 2c20 6e6f 7420 4e35 3031 592c 2073  ng, not N501Y, s
-00004c90: 696e 6365 2077 6520 6d69 6768 7420 6a75  ince we might ju
-00004ca0: 7374 0a23 2077 616e 7420 746f 2063 6865  st.# want to che
-00004cb0: 636b 2074 6861 7420 736f 6d65 7468 696e  ck that somethin
-00004cc0: 6720 6973 2069 6e20 7468 6520 6765 6e6f  g is in the geno
-00004cd0: 6d65 2077 6974 686f 7574 206b 6e6f 7769  me without knowi
-00004ce0: 6e67 206f 7220 6361 7269 6e67 0a23 2061  ng or caring.# a
-00004cf0: 626f 7574 2077 6861 7427 7320 696e 2074  bout what's in t
-00004d00: 6865 2072 6566 6572 656e 6365 2e0a 3e3e  he reference..>>
-00004d10: 3e20 7070 2861 6c69 676e 6d65 6e74 2e63  > pp(alignment.c
-00004d20: 6865 636b 4665 6174 7572 6528 2773 7069  heckFeature('spi
-00004d30: 6b65 272c 2027 3530 3159 2036 392d 2037  ke', '501Y 69- 7
-00004d40: 302d 272c 2061 613d 5472 7565 2929 0a28  0-', aa=True)).(
-00004d50: 332c 0a20 302c 0a20 7b27 3530 3159 273a  3,. 0,. {'501Y':
-00004d60: 2028 5472 7565 2c20 274e 272c 2054 7275   (True, 'N', Tru
-00004d70: 652c 2027 5927 292c 0a20 2027 3639 2d27  e, 'Y'),.  '69-'
-00004d80: 3a20 2854 7275 652c 2027 4827 2c20 5472  : (True, 'H', Tr
-00004d90: 7565 2c20 272d 2729 2c0a 2020 2737 302d  ue, '-'),.  '70-
-00004da0: 273a 2028 5472 7565 2c20 2756 272c 2054  ': (True, 'V', T
-00004db0: 7275 652c 2027 2d27 297d 290a 6060 600a  rue, '-')}).```.
-00004dc0: 0a0a 5468 6572 6520 6973 2061 6c73 6f20  ..There is also 
-00004dd0: 6120 636f 6e76 656e 6965 6e63 6520 6043  a convenience `C
-00004de0: 6865 636b 6572 6020 636c 6173 7320 7468  hecker` class th
-00004df0: 6174 2063 616e 2063 6865 636b 2077 6865  at can check whe
-00004e00: 7468 6572 206c 6f67 6963 616c 0a63 6f6d  ther logical.com
-00004e10: 6269 6e61 7469 6f6e 7320 6f66 2061 6d69  binations of ami
-00004e20: 6e6f 2061 6369 6420 616e 6420 6e75 636c  no acid and nucl
-00004e30: 656f 7469 6465 2063 6861 6e67 6573 2061  eotide changes a
-00004e40: 7265 2073 6174 6973 6669 6564 2066 6f72  re satisfied for
-00004e50: 2061 2067 656e 6f6d 652e 0a43 6f6e 7469   a genome..Conti
-00004e60: 6e75 696e 6720 6672 6f6d 2074 6865 2061  nuing from the a
-00004e70: 626f 7665 3a0a 0a60 6060 2070 790a 3e3e  bove:..``` py.>>
-00004e80: 3e20 6672 6f6d 2067 6232 7365 712e 6368  > from gb2seq.ch
-00004e90: 6563 6b65 7220 696d 706f 7274 2041 4143  ecker import AAC
-00004ea0: 6865 636b 6572 2c20 4e54 4368 6563 6b65  hecker, NTChecke
-00004eb0: 720a 0a23 204d 616b 6520 6120 426f 6f6c  r..# Make a Bool
-00004ec0: 6561 6e20 6368 6563 6b65 7220 6675 6e63  ean checker func
-00004ed0: 7469 6f6e 2074 6f20 7465 7374 2077 6865  tion to test whe
-00004ee0: 7468 6572 2061 2067 656e 6f6d 6520 6861  ther a genome ha
-00004ef0: 7320 7468 6520 4e35 3031 590a 2320 616e  s the N501Y.# an
-00004f00: 6420 4135 3730 4420 7370 696b 6520 6368  d A570D spike ch
-00004f10: 616e 6765 7320 7365 656e 2069 6e20 416c  anges seen in Al
-00004f20: 7068 612e 0a3e 3e3e 2063 6865 636b 6572  pha..>>> checker
-00004f30: 203d 2041 4143 6865 636b 6572 2827 7370   = AAChecker('sp
-00004f40: 696b 6527 2c20 274e 3530 3159 2729 2026  ike', 'N501Y') &
-00004f50: 2041 4143 6865 636b 6572 2827 7370 696b   AAChecker('spik
-00004f60: 6527 2c20 2741 3537 3044 2729 0a3e 3e3e  e', 'A570D').>>>
-00004f70: 2063 6865 636b 6572 2861 6c69 676e 6d65   checker(alignme
-00004f80: 6e74 290a 5472 7565 0a0a 2320 4368 6563  nt).True..# Chec
-00004f90: 6b20 666f 7220 736f 6d65 206e 7563 6c65  k for some nucle
-00004fa0: 6f74 6964 6520 6368 616e 6765 7320 696e  otide changes in
-00004fb0: 2074 6865 206e 7563 6c65 6f63 6170 7369   the nucleocapsi
-00004fc0: 6420 616e 6420 736f 6d65 2061 6d69 6e6f  d and some amino
-00004fd0: 0a23 2061 6369 6420 6368 616e 6765 7320  .# acid changes 
-00004fe0: 696e 2074 6865 2073 7069 6b65 2e0a 6368  in the spike..ch
-00004ff0: 6563 6b65 7220 3d20 284e 5443 6865 636b  ecker = (NTCheck
-00005000: 6572 2827 4e27 2c20 2747 3743 2041 3854  er('N', 'G7C A8T
-00005010: 2054 3941 2047 3630 3841 2047 3630 3941   T9A G608A G609A
-00005020: 2047 3631 3043 2043 3730 3454 2729 2026   G610C C704T') &
-00005030: 0a20 2020 2020 2020 2020 2020 4141 4368  .           AACh
-00005040: 6563 6b65 7228 2753 272c 2027 4e35 3031  ecker('S', 'N501
-00005050: 5920 4836 392d 2056 3730 2d20 5931 3434  Y H69- V70- Y144
-00005060: 2d27 2929 0a0a 2320 596f 7520 6361 6e20  -'))..# You can 
-00005070: 616c 736f 2075 7365 2060 7c60 2074 6f20  also use `|` to 
-00005080: 6368 6563 6b20 616e 204f 5220 636f 6e64  check an OR cond
-00005090: 6974 696f 6e2e 0a3e 3e3e 2063 6865 636b  ition..>>> check
-000050a0: 6572 203d 2041 4143 6865 636b 6572 2827  er = AAChecker('
-000050b0: 7370 696b 6527 2c20 2745 3438 344b 2729  spike', 'E484K')
-000050c0: 207c 2041 4143 6865 636b 6572 2827 7370   | AAChecker('sp
-000050d0: 696b 6527 2c20 2745 3438 3451 2729 0a3e  ike', 'E484Q').>
-000050e0: 3e3e 2063 6865 636b 6572 2861 6c69 676e  >> checker(align
-000050f0: 6d65 6e74 290a 4661 6c73 650a 6060 600a  ment).False.```.
-00005100: 0a4e 6f74 6520 7468 6174 2062 6563 6175  .Note that becau
-00005110: 7365 2074 6865 2060 4368 6563 6b65 7260  se the `Checker`
-00005120: 2063 6c61 7373 2074 616b 6573 2061 2073   class takes a s
-00005130: 7472 696e 6720 6172 6775 6d65 6e74 2074  tring argument t
-00005140: 6861 7420 6c69 6b65 6c79 0a6f 7269 6769  hat likely.origi
-00005150: 6e61 7465 7320 6672 6f6d 2061 2068 756d  nates from a hum
-00005160: 616e 2d72 6561 6461 626c 6520 736f 7572  an-readable sour
-00005170: 6365 2c20 652e 672e 2c20 224e 3530 3159  ce, e.g., "N501Y
-00005180: 222c 2074 6865 2063 6861 6e67 6573 0a73  ", the changes.s
-00005190: 7065 6369 6669 6564 2066 6f72 2074 6865  pecified for the
-000051a0: 2063 6865 636b 6572 2061 7265 2069 6e20   checker are in 
-000051b0: 7465 726d 7320 6f66 2031 2d62 6173 6564  terms of 1-based
-000051c0: 2073 6974 6573 2e0a 0a53 696d 696c 6961   sites...Similia
-000051d0: 7220 746f 2074 6865 2060 2d2d 6368 6563  r to the `--chec
-000051e0: 6b56 6172 6961 6e74 6020 6172 6775 6d65  kVariant` argume
-000051f0: 6e74 2074 6f20 6064 6573 6372 6962 652d  nt to `describe-
-00005200: 6765 6e6f 6d65 2e70 7960 2028 6162 6f76  genome.py` (abov
-00005210: 6529 2c0a 796f 7520 6361 6e20 616c 736f  e),.you can also
-00005220: 2063 6865 636b 2061 2070 7265 2d64 6566   check a pre-def
-00005230: 696e 6564 2076 6172 6961 6e74 3a0a 0a60  ined variant:..`
-00005240: 6060 7079 0a3e 3e3e 2070 7028 616c 6967  ``py.>>> pp(alig
-00005250: 6e6d 656e 742e 6368 6563 6b56 6172 6961  nment.checkVaria
-00005260: 6e74 2827 564f 435f 3230 3230 3132 3031  nt('VOC_20201201
-00005270: 5f55 4b27 2929 0a28 3230 2c0a 2030 2c0a  _UK')).(20,. 0,.
-00005280: 207b 276e 273a 207b 2761 6127 3a20 7b27   {'n': {'aa': {'
-00005290: 3233 3546 273a 2028 5472 7565 2c20 2753  235F': (True, 'S
-000052a0: 272c 2054 7275 652c 2027 4627 292c 2027  ', True, 'F'), '
-000052b0: 334c 273a 2028 5472 7565 2c20 2744 272c  3L': (True, 'D',
-000052c0: 2054 7275 652c 2027 4c27 297d 7d2c 0a20   True, 'L')}},. 
-000052d0: 2027 6f72 6631 6162 273a 207b 2761 6127   'orf1ab': {'aa'
-000052e0: 3a20 7b27 3130 3031 4927 3a20 2854 7275  : {'1001I': (Tru
-000052f0: 652c 2027 5427 2c20 5472 7565 2c20 2749  e, 'T', True, 'I
-00005300: 2729 2c0a 2020 2020 2020 2020 2020 2020  '),.            
-00005310: 2020 2020 2020 2020 2731 3730 3844 273a          '1708D':
-00005320: 2028 5472 7565 2c20 2741 272c 2054 7275   (True, 'A', Tru
-00005330: 652c 2027 4427 292c 0a20 2020 2020 2020  e, 'D'),.       
-00005340: 2020 2020 2020 2020 2020 2020 2027 3232               '22
-00005350: 3330 5427 3a20 2854 7275 652c 2027 4927  30T': (True, 'I'
-00005360: 2c20 5472 7565 2c20 2754 2729 2c0a 2020  , True, 'T'),.  
-00005370: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005380: 2020 2733 3637 352d 273a 2028 5472 7565    '3675-': (True
-00005390: 2c20 2753 272c 2054 7275 652c 2027 2d27  , 'S', True, '-'
-000053a0: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
-000053b0: 2020 2020 2020 2027 3336 3736 2d27 3a20         '3676-': 
-000053c0: 2854 7275 652c 2027 4727 2c20 5472 7565  (True, 'G', True
-000053d0: 2c20 272d 2729 2c0a 2020 2020 2020 2020  , '-'),.        
-000053e0: 2020 2020 2020 2020 2020 2020 2733 3637              '367
-000053f0: 372d 273a 2028 5472 7565 2c20 2746 272c  7-': (True, 'F',
-00005400: 2054 7275 652c 2027 2d27 297d 7d2c 0a20   True, '-')}},. 
-00005410: 2027 6f72 6638 273a 207b 2761 6127 3a20   'orf8': {'aa': 
-00005420: 7b27 3532 4927 3a20 2854 7275 652c 2027  {'52I': (True, '
-00005430: 5227 2c20 5472 7565 2c20 2749 2729 2c0a  R', True, 'I'),.
-00005440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005450: 2020 2737 3343 273a 2028 5472 7565 2c20    '73C': (True, 
-00005460: 2759 272c 2054 7275 652c 2027 4327 292c  'Y', True, 'C'),
-00005470: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
-00005480: 2020 2027 5132 372a 273a 2028 5472 7565     'Q27*': (True
-00005490: 2c20 2751 272c 2054 7275 652c 2027 2a27  , 'Q', True, '*'
-000054a0: 297d 7d2c 0a20 2027 7370 696b 6527 3a20  )}},.  'spike': 
-000054b0: 7b27 6161 273a 207b 2731 3131 3848 273a  {'aa': {'1118H':
-000054c0: 2028 5472 7565 2c20 2744 272c 2054 7275   (True, 'D', Tru
-000054d0: 652c 2027 4827 292c 0a20 2020 2020 2020  e, 'H'),.       
-000054e0: 2020 2020 2020 2020 2020 2020 2731 3434              '144
-000054f0: 2d27 3a20 2854 7275 652c 2027 5927 2c20  -': (True, 'Y', 
-00005500: 5472 7565 2c20 272d 2729 2c0a 2020 2020  True, '-'),.    
-00005510: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00005520: 3530 3159 273a 2028 5472 7565 2c20 274e  501Y': (True, 'N
-00005530: 272c 2054 7275 652c 2027 5927 292c 0a20  ', True, 'Y'),. 
-00005540: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00005550: 2020 2735 3730 4427 3a20 2854 7275 652c    '570D': (True,
-00005560: 2027 4127 2c20 5472 7565 2c20 2744 2729   'A', True, 'D')
-00005570: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
-00005580: 2020 2020 2027 3638 3148 273a 2028 5472       '681H': (Tr
-00005590: 7565 2c20 2750 272c 2054 7275 652c 2027  ue, 'P', True, '
-000055a0: 4827 292c 0a20 2020 2020 2020 2020 2020  H'),.           
-000055b0: 2020 2020 2020 2020 2736 392d 273a 2028          '69-': (
-000055c0: 5472 7565 2c20 2748 272c 2054 7275 652c  True, 'H', True,
-000055d0: 2027 2d27 292c 0a20 2020 2020 2020 2020   '-'),.         
-000055e0: 2020 2020 2020 2020 2020 2737 302d 273a            '70-':
-000055f0: 2028 5472 7565 2c20 2756 272c 2054 7275   (True, 'V', Tru
-00005600: 652c 2027 2d27 292c 0a20 2020 2020 2020  e, '-'),.       
-00005610: 2020 2020 2020 2020 2020 2020 2737 3136              '716
-00005620: 4927 3a20 2854 7275 652c 2027 5427 2c20  I': (True, 'T', 
-00005630: 5472 7565 2c20 2749 2729 2c0a 2020 2020  True, 'I'),.    
-00005640: 2020 2020 2020 2020 2020 2020 2020 2027                 '
-00005650: 3938 3241 273a 2028 5472 7565 2c20 2753  982A': (True, 'S
-00005660: 272c 2054 7275 652c 2027 4127 297d 7d7d  ', True, 'A')}}}
-00005670: 290a 6060 600a 0a77 6974 6820 7468 6520  ).```..with the 
-00005680: 7265 7375 6c74 7320 7375 6d6d 6172 697a  results summariz
-00005690: 696e 6720 7468 6520 6e75 6d62 6572 206f  ing the number o
-000056a0: 6620 7465 7374 7320 646f 6e65 2c20 7468  f tests done, th
-000056b0: 6520 6e75 6d62 6572 2074 6861 740a 6661  e number that.fa
-000056c0: 696c 6564 2c20 616e 6420 7468 656e 2074  iled, and then t
-000056d0: 6865 2066 6561 7475 7265 7320 6368 6563  he features chec
-000056e0: 6b65 642c 2077 6974 6820 6061 6160 2061  ked, with `aa` a
-000056f0: 6e64 2060 6e74 6020 6469 6374 696f 6e61  nd `nt` dictiona
-00005700: 7269 6573 2066 6f72 0a74 6865 2061 6d69  ries for.the ami
-00005710: 6e6f 2061 6369 6420 616e 6420 6e75 636c  no acid and nucl
-00005720: 656f 7469 6465 2063 6865 636b 732e 0a0a  eotide checks...
-00005730: 596f 7520 6361 6e20 7061 7373 2079 6f75  You can pass you
-00005740: 7220 6f77 6e20 7661 7269 616e 7420 6469  r own variant di
-00005750: 6374 696f 6e61 7279 2073 7065 6369 6679  ctionary specify
-00005760: 696e 6720 7768 6174 2079 6f75 2077 616e  ing what you wan
-00005770: 7420 6368 6563 6b65 642e 0a0a 2323 2054  t checked...## T
-00005780: 6f20 6c65 6172 6e20 6d6f 7265 0a0a 5365  o learn more..Se
-00005790: 6520 7468 6520 6046 6561 7475 7265 7360  e the `Features`
-000057a0: 2061 6e64 2060 4762 3241 6c69 676e 6d65   and `Gb2Alignme
-000057b0: 6e74 6020 636c 6173 7365 7320 696e 0a5b  nt` classes in.[
-000057c0: 6762 3273 6571 2f66 6561 7475 7265 2e70  gb2seq/feature.p
-000057d0: 795d 2867 6232 7365 712f 6665 6174 7572  y](gb2seq/featur
-000057e0: 652e 7079 2920 616e 640a 5b67 6232 7365  e.py) and.[gb2se
-000057f0: 712f 616c 6967 6e6d 656e 742e 7079 5d28  q/alignment.py](
-00005800: 6762 3273 6571 2f61 6c69 676e 6d65 6e74  gb2seq/alignment
-00005810: 2e70 7929 2e20 416c 736f 2c20 7468 6520  .py). Also, the 
-00005820: 7465 7374 7320 2865 2e67 2e2c 2069 6e0a  tests (e.g., in.
-00005830: 5b74 6573 742f 7465 7374 5f66 6561 7475  [test/test_featu
-00005840: 7265 2e70 795d 2874 6573 742f 7465 7374  re.py](test/test
-00005850: 5f66 6561 7475 7265 2e70 7929 2c0a 5b74  _feature.py),.[t
-00005860: 6573 742f 7465 7374 5f61 6c69 676e 6d65  est/test_alignme
-00005870: 6e74 2e70 795d 2874 6573 742f 7465 7374  nt.py](test/test
-00005880: 5f61 6c69 676e 6d65 6e74 2e70 7929 2c0a  _alignment.py),.
-00005890: 5b74 6573 742f 7465 7374 5f63 6865 636b  [test/test_check
-000058a0: 6572 2e70 795d 2874 6573 742f 7465 7374  er.py](test/test
-000058b0: 5f63 6865 636b 6572 2e70 7929 0a5b 7465  _checker.py).[te
-000058c0: 7374 2f74 6573 745f 7661 7269 616e 7473  st/test_variants
-000058d0: 2e70 795d 2874 6573 742f 7465 7374 5f76  .py](test/test_v
-000058e0: 6172 6961 6e74 732e 7079 2929 2073 686f  ariants.py)) sho
-000058f0: 7720 796f 7520 6578 616d 706c 6520 7573  w you example us
-00005900: 6573 206f 660a 7468 6573 6520 636c 6173  es of.these clas
-00005910: 7365 7320 616e 6420 7468 6569 7220 6d65  ses and their me
-00005920: 7468 6f64 732e 2020 596f 7520 6361 6e20  thods.  You can 
-00005930: 616c 736f 206c 6f6f 6b20 746f 2073 6565  also look to see
-00005940: 2068 6f77 2074 6865 2074 6872 6565 0a75   how the three.u
-00005950: 7469 6c69 7479 2073 6372 6970 7473 2064  tility scripts d
-00005960: 6573 6372 6962 6564 2061 626f 7665 2028  escribed above (
-00005970: 7768 6963 6820 6361 6e20 616c 6c20 6265  which can all be
-00005980: 2066 6f75 6e64 2069 6e20 7468 6520 5b62   found in the [b
-00005990: 696e 0a64 6972 6563 746f 7279 5d28 6269  in.directory](bi
-000059a0: 6e29 2920 6361 6c6c 2074 6865 206c 6962  n)) call the lib
-000059b0: 7261 7279 2066 756e 6374 696f 6e73 2061  rary functions a
-000059c0: 6e64 2075 7365 2074 6865 2072 6573 756c  nd use the resul
-000059d0: 7473 2e0a 0a23 2044 6576 656c 6f70 696e  ts...# Developin
-000059e0: 670a 0a52 756e 2074 6865 2074 6573 7473  g..Run the tests
-000059f0: 2076 6961 200a 0a60 6060 7368 0a24 2070   via ..```sh.$ p
-00005a00: 7974 6573 740a 6060 600a 0a23 2320 4e6f  ytest.```..## No
-00005a10: 7465 730a 0a2a 2054 6865 2074 6573 7473  tes..* The tests
-00005a20: 2077 696c 6c20 7275 6e20 604d 4146 4654   will run `MAFFT
-00005a30: 602c 2073 6f20 796f 7520 6e65 6564 2074  `, so you need t
-00005a40: 6861 7420 696e 7374 616c 6c65 6420 616e  hat installed an
-00005a50: 6420 696e 0a20 2020 2079 6f75 7220 7368  d in.    your sh
-00005a60: 656c 6c27 7320 7061 7468 2e0a 2a20 5468  ell's path..* Th
-00005a70: 6520 7465 7374 7320 646f 206e 6f74 2061  e tests do not a
-00005a80: 6c6c 2070 6173 7320 6966 2079 6f75 2073  ll pass if you s
-00005a90: 6574 2060 4445 4641 554c 545f 414c 4947  et `DEFAULT_ALIG
-00005aa0: 4e45 5260 2074 6f20 6265 2022 6564 6c69  NER` to be "edli
-00005ab0: 6222 2069 6e0a 2020 2020 6067 6232 7365  b" in.    `gb2se
-00005ac0: 712f 616c 6967 6e6d 656e 742e 7079 602e  q/alignment.py`.
-00005ad0: 2054 6869 7320 6973 2062 6563 6175 7365   This is because
-00005ae0: 2060 4d41 4646 5460 2061 6e64 2060 6564   `MAFFT` and `ed
-00005af0: 6c69 6260 2070 726f 6475 6365 0a20 2020  lib` produce.   
-00005b00: 2073 6c69 6768 746c 7920 6469 6666 6572   slightly differ
-00005b10: 656e 7420 7265 7375 6c74 7320 616e 6420  ent results and 
-00005b20: 736f 6d65 2074 6573 7473 206f 6620 7468  some tests of th
-00005b30: 6520 5341 5253 2d43 6f56 2d32 2073 7069  e SARS-CoV-2 spi
-00005b40: 6b65 0a20 2020 2074 7261 6e73 6c61 7469  ke.    translati
-00005b50: 6f6e 2074 6573 7473 2066 6169 6c20 6173  on tests fail as
-00005b60: 2061 2072 6573 756c 742e 2049 2077 6f75   a result. I wou
-00005b70: 6c64 206c 696b 6520 746f 2070 6f73 742d  ld like to post-
-00005b80: 7072 6f63 6573 7320 7468 650a 2020 2020  process the.    
-00005b90: 6065 646c 6962 6020 6f75 7470 7574 2074  `edlib` output t
-00005ba0: 6f20 6d61 7463 6820 7468 6174 206f 6620  o match that of 
-00005bb0: 604d 4146 4654 6020 2874 6869 7320 6973  `MAFFT` (this is
-00005bc0: 2069 6e20 6361 7365 7320 7768 6572 6520   in cases where 
-00005bd0: 7468 6572 650a 2020 2020 6172 6520 6d75  there.    are mu
-00005be0: 6c74 6970 6c65 2065 7175 616c 6c79 2d67  ltiple equally-g
-00005bf0: 6f6f 6420 616c 6967 6e6d 656e 7473 292e  ood alignments).
-00005c00: 0a                                       .
+00000070: 7072 6f76 6964 6573 2061 2050 7974 686f  provides a Pytho
+00000080: 6e20 6c69 6272 6172 7920 616e 6420 636f  n library and co
+00000090: 6d6d 616e 642d 6c69 6e65 2073 6372 6970  mmand-line scrip
+000000a0: 7473 2074 6861 7420 6465 7269 7665 0a69  ts that derive.i
+000000b0: 6e66 6f72 6d61 7469 6f6e 2072 6567 6172  nformation regar
+000000c0: 6469 6e67 2075 6e61 6e6e 6f74 6174 6564  ding unannotated
+000000d0: 2061 6e20 7669 7261 6c20 6765 6e6f 6d65   an viral genome
+000000e0: 2066 726f 6d20 616e 6e6f 7461 7469 6f6e   from annotation
+000000f0: 7320 696e 2061 0a47 656e 4261 6e6b 2072  s in a.GenBank r
+00000100: 6566 6572 656e 6365 2e20 4120 7479 7069  eference. A typi
+00000110: 6361 6c20 7573 6520 6361 7365 2069 7320  cal use case is 
+00000120: 746f 2069 6e76 6573 7469 6761 7465 2074  to investigate t
+00000130: 6865 2070 726f 7065 7274 6965 7320 6f66  he properties of
+00000140: 0a61 6e20 756e 616e 6e6f 7461 7465 6420  .an unannotated 
+00000150: 6765 6e6f 6d65 2063 616c 6c65 6420 6672  genome called fr
+00000160: 6f6d 2061 205b 5341 4d2f 4241 4d0a 6669  om a [SAM/BAM.fi
+00000170: 6c65 5d28 6874 7470 733a 2f2f 656e 2e77  le](https://en.w
+00000180: 696b 6970 6564 6961 2e6f 7267 2f77 696b  ikipedia.org/wik
+00000190: 692f 5341 4d5f 2866 696c 655f 666f 726d  i/SAM_(file_form
+000001a0: 6174 2929 2066 6f6c 6c6f 7769 6e67 2061  at)) following a
+000001b0: 6c69 676e 6d65 6e74 0a6f 6620 6869 6768  lignment.of high
+000001c0: 2d74 6872 6f75 6768 7075 7420 7365 7175  -throughput sequ
+000001d0: 656e 6369 6e67 2072 6561 6473 2028 652e  encing reads (e.
+000001e0: 672e 2c20 7769 7468 0a5b 6277 615d 2868  g., with.[bwa](h
+000001f0: 7474 7073 3a2f 2f62 696f 2d62 7761 2e73  ttps://bio-bwa.s
+00000200: 6f75 7263 6566 6f72 6765 2e6e 6574 2f29  ourceforge.net/)
+00000210: 206f 720a 5b62 6f77 7469 6532 5d28 6874   or.[bowtie2](ht
+00000220: 7470 733a 2f2f 626f 7774 6965 2d62 696f  tps://bowtie-bio
+00000230: 2e73 6f75 7263 6566 6f72 6765 2e6e 6574  .sourceforge.net
+00000240: 2f62 6f77 7469 6532 2f6d 616e 7561 6c2e  /bowtie2/manual.
+00000250: 7368 746d 6c29 2920 746f 2061 0a72 6566  shtml)) to a.ref
+00000260: 6572 656e 6365 2e0a 0a23 2320 5079 7468  erence...## Pyth
+00000270: 6f6e 206c 6962 7261 7279 0a0a 5468 6520  on library..The 
+00000280: 5079 7468 6f6e 206c 6962 7261 7279 2028  Python library (
+00000290: 3c61 2068 7265 663d 2223 6170 6922 3e41  <a href="#api">A
+000002a0: 5049 2064 6573 6372 6962 6564 2062 656c  PI described bel
+000002b0: 6f77 3c2f 613e 2920 7072 6f76 6964 6573  ow</a>) provides
+000002c0: 2066 6f72 3a0a 0a2a 2045 7874 7261 6374   for:..* Extract
+000002d0: 696f 6e20 6f66 2061 6c69 676e 6564 2066  ion of aligned f
+000002e0: 6561 7475 7265 7320 6173 206e 7563 6c65  eatures as nucle
+000002f0: 6f74 6964 6520 6f72 2061 6d69 6e6f 2061  otide or amino a
+00000300: 6369 6420 7365 7175 656e 6365 732e 0a2a  cid sequences..*
+00000310: 2052 6574 7269 6576 696e 6720 696e 666f   Retrieving info
+00000320: 726d 6174 696f 6e20 6162 6f75 7420 7768  rmation about wh
+00000330: 6174 2069 7320 6174 2061 2073 6974 6520  at is at a site 
+00000340: 2861 6e6e 6f74 6174 6564 2066 6561 7475  (annotated featu
+00000350: 7265 732c 0a20 2020 206e 7563 6c65 6f74  res,.    nucleot
+00000360: 6964 652c 2061 6d69 6e6f 2061 6369 642c  ide, amino acid,
+00000370: 2063 6f64 6f6e 2c20 6672 616d 652c 2065   codon, frame, e
+00000380: 7463 292e 0a2a 2054 7261 6e73 6c61 7469  tc)..* Translati
+00000390: 6f6e 206f 6620 6f66 6673 6574 7320 6265  on of offsets be
+000003a0: 7477 6565 6e20 7468 6520 7265 6665 7265  tween the refere
+000003b0: 6e63 6520 616e 6420 7468 6520 756e 616e  nce and the unan
+000003c0: 6e6f 7461 7465 6420 6765 6e6f 6d65 0a20  notated genome. 
+000003d0: 2020 2077 6974 6820 6f66 6673 6574 7320     with offsets 
+000003e0: 7468 6174 2061 7265 2061 6273 6f6c 7574  that are absolut
+000003f0: 6520 6f72 2072 656c 6174 6976 6520 746f  e or relative to
+00000400: 2061 2066 6561 7475 7265 2e0a 2a20 4465   a feature..* De
+00000410: 7461 696c 6564 2061 6c69 676e 6d65 6e74  tailed alignment
+00000420: 2069 6e66 6f72 6d61 7469 6f6e 2066 6f72   information for
+00000430: 2066 6561 7475 7265 732e 0a2a 204a 534f   features..* JSO
+00000440: 4e20 616e 6e6f 7461 7469 6f6e 7320 6f66  N annotations of
+00000450: 2074 6865 2066 6561 7475 7265 7320 6f66   the features of
+00000460: 2074 6865 2075 6e61 6e6e 6f74 6174 6564   the unannotated
+00000470: 2067 656e 6f6d 652e 0a2a 2043 6f6e 7665   genome..* Conve
+00000480: 6e69 656e 6365 206d 6574 686f 6473 2066  nience methods f
+00000490: 6f72 2063 6865 636b 696e 6720 6765 6e6f  or checking geno
+000004a0: 6d65 7320 666f 7220 7365 7473 206f 6620  mes for sets of 
+000004b0: 6578 7065 6374 6564 206e 7563 6c65 6f74  expected nucleot
+000004c0: 6964 650a 2020 2020 6f72 2061 6d69 6e6f  ide.    or amino
+000004d0: 2061 6369 6420 7661 6c75 6573 2e0a 0a23   acid values...#
+000004e0: 2320 5363 7269 7074 730a 0a54 6865 2063  # Scripts..The c
+000004f0: 6f6d 6d61 6e64 2d6c 696e 6520 7363 7269  ommand-line scri
+00000500: 7074 7320 283c 6120 6872 6566 3d22 2373  pts (<a href="#s
+00000510: 6372 6970 7473 223e 6465 7363 7269 6265  cripts">describe
+00000520: 6420 6265 6c6f 773c 2f61 3e29 0a70 726f  d below</a>).pro
+00000530: 7669 6465 2061 2063 6f6e 7665 6e69 656e  vide a convenien
+00000540: 7420 696e 7465 7266 6163 6520 746f 2074  t interface to t
+00000550: 6865 206c 6962 7261 7279 2066 756e 6374  he library funct
+00000560: 696f 6e73 2e20 5468 6572 6520 6172 6520  ions. There are 
+00000570: 7468 650a 666f 6c6c 6f77 696e 6720 7363  the.following sc
+00000580: 7269 7074 733a 0a0a 2a20 6061 6e6e 6f74  ripts:..* `annot
+00000590: 6174 652d 6765 6e6f 6d65 2e70 7960 202d  ate-genome.py` -
+000005a0: 2070 7269 6e74 7320 6120 4a53 4f4e 206f   prints a JSON o
+000005b0: 626a 6563 7420 636f 6e74 6169 6e69 6e67  bject containing
+000005c0: 2064 6574 6169 6c73 206f 6620 616c 6c0a   details of all.
+000005d0: 2020 2020 6665 6174 7572 6573 206f 6620      features of 
+000005e0: 616e 2075 6e61 6e6e 6f74 6174 6564 2067  an unannotated g
+000005f0: 656e 6f6d 6520 2866 6f75 6e64 2076 6961  enome (found via
+00000600: 2061 6c69 676e 6d65 6e74 2077 6974 6820   alignment with 
+00000610: 6120 7265 6665 7265 6e63 650a 2020 2020  a reference.    
+00000620: 6765 6e6f 6d65 292e 0a2a 2060 6465 7363  genome)..* `desc
+00000630: 7269 6265 2d66 6561 7475 7265 2e70 7960  ribe-feature.py`
+00000640: 202d 2070 7269 6e74 2069 6e66 6f72 6d61   - print informa
+00000650: 7469 6f6e 2061 626f 7574 2061 2067 6976  tion about a giv
+00000660: 656e 2066 6561 7475 7265 206f 720a 2020  en feature or.  
+00000670: 2020 6665 6174 7572 6573 2e0a 2a20 6064    features..* `d
+00000680: 6573 6372 6962 652d 6765 6e6f 6d65 2e70  escribe-genome.p
+00000690: 7960 202d 2065 7874 7261 6374 206e 7563  y` - extract nuc
+000006a0: 6c65 6f74 6964 6520 616e 642f 6f72 2061  leotide and/or a
+000006b0: 6d69 6e6f 2061 6369 6420 7365 7175 656e  mino acid sequen
+000006c0: 6365 7320 666f 720a 2020 2020 6665 6174  ces for.    feat
+000006d0: 7572 6573 2061 6e64 2073 756d 6d61 7269  ures and summari
+000006e0: 7a65 2074 6865 6972 2073 696d 696c 6172  ze their similar
+000006f0: 6974 792e 0a2a 2060 6465 7363 7269 6265  ity..* `describe
+00000700: 2d73 6974 652e 7079 6020 2d20 7072 696e  -site.py` - prin
+00000710: 7420 696e 666f 726d 6174 696f 6e20 6162  t information ab
+00000720: 6f75 7420 7061 7274 6963 756c 6172 2067  out particular g
+00000730: 656e 6f6d 6520 6c6f 6361 7469 6f6e 732e  enome locations.
+00000740: 0a0a 5468 6520 7661 7269 6f75 7320 6064  ..The various `d
+00000750: 6573 6372 6962 652d 2a2e 7079 6020 7363  escribe-*.py` sc
+00000760: 7269 7074 7320 7769 6c6c 2065 7874 7261  ripts will extra
+00000770: 6374 2069 6e66 6f72 6d61 7469 6f6e 2061  ct information a
+00000780: 626f 7574 206a 7573 7420 7468 650a 7265  bout just the.re
+00000790: 6665 7265 6e63 6520 7365 7175 656e 6365  ference sequence
+000007a0: 2069 6620 6e6f 2075 6e61 6e6e 6f74 6174   if no unannotat
+000007b0: 6564 2067 656e 6f6d 6520 6973 2067 6976  ed genome is giv
+000007c0: 656e 2e20 5468 6973 2063 616e 2062 6520  en. This can be 
+000007d0: 7573 6564 2c20 666f 720a 6578 616d 706c  used, for.exampl
+000007e0: 652c 2074 6f20 6f62 7461 696e 2061 6e20  e, to obtain an 
+000007f0: 6162 736f 6c75 7465 206e 7563 6c65 6f74  absolute nucleot
+00000800: 6964 6520 6f66 6673 6574 2069 6e20 6120  ide offset in a 
+00000810: 7265 6665 7265 6e63 6520 6769 7665 6e20  reference given 
+00000820: 610a 7265 6c61 7469 7665 2061 6d69 6e6f  a.relative amino
+00000830: 2061 6369 6420 6f66 6673 6574 2066 6f72   acid offset for
+00000840: 2061 2070 6172 7469 6375 6c61 7220 6765   a particular ge
+00000850: 6e65 2028 7365 6520 6578 616d 706c 6573  ne (see examples
+00000860: 2062 656c 6f77 292e 0a0a 2323 2054 6572   below)...## Ter
+00000870: 6d69 6e6f 6c6f 6779 2c20 636f 6e76 656e  minology, conven
+00000880: 7469 6f6e 732c 2061 6e64 2053 4152 532d  tions, and SARS-
+00000890: 436f 562d 3220 6675 6e63 7469 6f6e 616c  CoV-2 functional
+000008a0: 6974 790a 0a23 2323 2047 656e 6f6d 6520  ity..### Genome 
+000008b0: 6c6f 6361 7469 6f6e 733a 2073 6974 6573  locations: sites
+000008c0: 2076 7320 6f66 6673 6574 730a 0a57 6865   vs offsets..Whe
+000008d0: 6e20 7265 6665 7272 696e 6720 746f 206c  n referring to l
+000008e0: 6f63 6174 696f 6e73 2077 6974 6869 6e20  ocations within 
+000008f0: 6120 6765 6e6f 6d65 206f 7220 6120 6765  a genome or a ge
+00000900: 6e6f 6d65 2066 6561 7475 7265 2028 652e  nome feature (e.
+00000910: 672e 2c20 610a 7061 7274 6963 756c 6172  g., a.particular
+00000920: 2070 726f 7465 696e 292c 2022 7369 7465   protein), "site
+00000930: 2220 6973 2075 7365 6420 746f 2064 6573  " is used to des
+00000940: 6372 6962 6520 312d 6261 7365 6420 6c6f  cribe 1-based lo
+00000950: 6361 7469 6f6e 732c 2061 7320 776f 756c  cations, as woul
+00000960: 640a 6e6f 726d 616c 6c79 2062 6520 7573  d.normally be us
+00000970: 6564 2062 7920 6120 7265 6775 6c61 7220  ed by a regular 
+00000980: 7065 7273 6f6e 2e20 2054 6865 7265 666f  person.  Therefo
+00000990: 7265 2c20 7468 6520 696e 7075 7420 616e  re, the input an
+000009a0: 6420 6f75 7470 7574 206f 660a 636f 6d6d  d output of.comm
+000009b0: 616e 642d 6c69 6e65 2073 6372 6970 7473  and-line scripts
+000009c0: 2075 7365 2031 2d62 6173 6564 206e 756d   use 1-based num
+000009d0: 6265 7269 6e67 2062 7920 6465 6661 756c  bering by defaul
+000009e0: 742e 0a0a 486f 7765 7665 722c 2074 6865  t...However, the
+000009f0: 206c 6962 7261 7279 2041 5049 2c20 6173   library API, as
+00000a00: 2075 7365 6420 6279 2050 7974 686f 6e20   used by Python 
+00000a10: 7072 6f67 7261 6d6d 6572 732c 2065 7870  programmers, exp
+00000a20: 6563 7473 2061 6e64 0a72 6574 7572 6e73  ects and.returns
+00000a30: 2030 2d62 6173 6564 206f 6666 7365 7473   0-based offsets
+00000a40: 2e0a 0a54 6865 2022 7369 7465 2220 616e  ...The "site" an
+00000a50: 6420 226f 6666 7365 7422 2074 6572 6d69  d "offset" termi
+00000a60: 6e6f 6c6f 6779 2069 7320 7573 6564 2063  nology is used c
+00000a70: 6f6e 7369 7374 656e 746c 7920 7468 726f  onsistently thro
+00000a80: 7567 686f 7574 2074 6865 0a63 6f64 652e  ughout the.code.
+00000a90: 0a0a 2323 2320 4665 6174 7572 6573 0a0a  ..### Features..
+00000aa0: 4765 6e42 616e 6b20 616e 6e6f 7461 7469  GenBank annotati
+00000ab0: 6f6e 2066 696c 6573 2069 6e64 6963 6174  on files indicat
+00000ac0: 6520 7468 6520 6765 6e6f 6d65 206c 6f63  e the genome loc
+00000ad0: 6174 696f 6e73 206f 6620 2266 6561 7475  ations of "featu
+00000ae0: 7265 7322 2e20 5468 6573 650a 6172 6520  res". These.are 
+00000af0: 6a75 7374 2067 656e 6f6d 6520 7265 6769  just genome regi
+00000b00: 6f6e 732e 2041 6c74 686f 7567 6820 616e  ons. Although an
+00000b10: 6e6f 7461 7465 6420 6665 6174 7572 6573  notated features
+00000b20: 206f 6620 696e 7465 7265 7374 2061 7265   of interest are
+00000b30: 206f 6674 656e 0a4f 5246 7320 6f72 2067   often.ORFs or g
+00000b40: 656e 6573 2c20 7468 6579 2061 6c73 6f20  enes, they also 
+00000b50: 696e 636c 7564 6520 756e 7472 616e 736c  include untransl
+00000b60: 6174 6564 2072 6567 696f 6e73 2061 6e64  ated regions and
+00000b70: 205b 6d61 6e79 0a6f 7468 6572 5d28 6874   [many.other](ht
+00000b80: 7470 733a 2f2f 656d 756e 6978 2e65 6d69  tps://emunix.emi
+00000b90: 6368 2e65 6475 2f7e 6d65 7665 7474 2f42  ch.edu/~mevett/B
+00000ba0: 696f 696e 666f 726d 6174 6963 7354 6f6f  ioinformaticsToo
+00000bb0: 6c73 2f47 656e 4261 6e6b 5f66 6561 7475  ls/GenBank_featu
+00000bc0: 7265 732e 6874 6d29 2e0a 5468 6520 6067  res.htm)..The `g
+00000bd0: 6232 7365 7160 2063 6f64 6520 7468 6174  b2seq` code that
+00000be0: 2072 6561 6473 2047 656e 4261 6e6b 2066   reads GenBank f
+00000bf0: 696c 6573 2075 7365 7320 7468 6973 2067  iles uses this g
+00000c00: 656e 6572 616c 2074 6572 6d20 746f 6f2c  eneral term too,
+00000c10: 2061 730a 796f 7520 7769 6c6c 2073 6565   as.you will see
+00000c20: 2069 6e20 7468 6520 6578 616d 706c 6573   in the examples
+00000c30: 2062 656c 6f77 2e0a 0a23 2323 2046 756e   below...### Fun
+00000c40: 6374 696f 6e20 6172 6775 6d65 6e74 2061  ction argument a
+00000c50: 6e64 2072 6574 7572 6e20 7661 6c75 6520  nd return value 
+00000c60: 6f72 6465 720a 0a49 6e20 616c 6c20 5079  order..In all Py
+00000c70: 7468 6f6e 2066 756e 6374 696f 6e73 2074  thon functions t
+00000c80: 6861 7420 6465 616c 2077 6974 6820 626f  hat deal with bo
+00000c90: 7468 2061 2072 6566 6572 656e 6365 2061  th a reference a
+00000ca0: 6e64 2061 6e20 756e 616e 6e6f 7461 7465  nd an unannotate
+00000cb0: 640a 6765 6e6f 6d65 2073 6571 7565 6e63  d.genome sequenc
+00000cc0: 652c 2074 6865 2072 6566 6572 656e 6365  e, the reference
+00000cd0: 2069 7320 616c 7761 7973 2070 6173 7365   is always passe
+00000ce0: 6420 616e 642f 6f72 2072 6574 7572 6e65  d and/or returne
+00000cf0: 6420 6669 7273 742e 0a0a 2323 2320 4869  d first...### Hi
+00000d00: 7374 6f72 6963 616c 206e 6f74 6520 6f6e  storical note on
+00000d10: 2077 6f72 6b69 6e67 2077 6974 6820 5341   working with SA
+00000d20: 5253 2d43 6f56 2d32 2067 656e 6f6d 6573  RS-CoV-2 genomes
+00000d30: 0a0a 5468 6973 2063 6f64 6520 7761 7320  ..This code was 
+00000d40: 7772 6974 7465 6e20 696e 206c 6174 6520  written in late 
+00000d50: 3230 3230 2066 6f72 2070 726f 6365 7373  2020 for process
+00000d60: 696e 6720 5341 5253 2d43 6f56 2d32 2067  ing SARS-CoV-2 g
+00000d70: 656e 6f6d 6573 2e20 4974 0a68 6173 2073  enomes. It.has s
+00000d80: 696e 6365 2062 6565 6e20 6765 6e65 7261  ince been genera
+00000d90: 6c69 7a65 6420 746f 2061 6c6c 6f77 2061  lized to allow a
+00000da0: 6e79 2047 656e 4261 6e6b 2066 696c 6520  ny GenBank file 
+00000db0: 6173 2061 2072 6566 6572 656e 6365 2e0a  as a reference..
+00000dc0: 0a54 6865 2063 6f6d 6d61 6e64 2d6c 696e  .The command-lin
+00000dd0: 6520 7363 7269 7074 7320 6361 6e20 6265  e scripts can be
+00000de0: 2067 6976 656e 2061 2060 2d2d 7361 7273   given a `--sars
+00000df0: 3260 2074 6f20 6861 7665 2074 6865 6d20  2` to have them 
+00000e00: 7573 6520 7468 650a 5775 6861 6e20 7265  use the.Wuhan re
+00000e10: 6665 7265 6e63 650a 285b 4e43 5f30 3435  ference.([NC_045
+00000e20: 3531 325d 2868 7474 7073 3a2f 2f77 7777  512](https://www
+00000e30: 2e6e 6362 692e 6e6c 6d2e 6e69 682e 676f  .ncbi.nlm.nih.go
+00000e40: 762f 6e75 6363 6f72 652f 4e43 5f30 3435  v/nuccore/NC_045
+00000e50: 3531 3229 292c 2069 6e20 7768 6963 680a  512)), in which.
+00000e60: 6361 7365 2074 6865 7265 2069 7320 6e6f  case there is no
+00000e70: 206e 6565 6420 746f 2070 726f 7669 6465   need to provide
+00000e80: 2061 2047 656e 4261 6e6b 2072 6566 6572   a GenBank refer
+00000e90: 656e 6365 2066 696c 652e 2020 5369 6d69  ence file.  Simi
+00000ea0: 6c61 726c 792c 2074 6865 0a50 7974 686f  larly, the.Pytho
+00000eb0: 6e20 636c 6173 7365 7320 6361 6e20 7461  n classes can ta
+00000ec0: 6b65 2061 2060 7361 7273 3260 2061 7267  ke a `sars2` arg
+00000ed0: 756d 656e 7420 7769 7468 2074 6865 2073  ument with the s
+00000ee0: 616d 6520 6566 6665 6374 2e0a 0a49 6620  ame effect...If 
+00000ef0: 796f 7520 6172 6520 6e6f 7420 776f 726b  you are not work
+00000f00: 696e 6720 7769 7468 2053 4152 532d 436f  ing with SARS-Co
+00000f10: 562d 3220 6765 6e6f 6d65 732c 206a 7573  V-2 genomes, jus
+00000f20: 7420 7061 7373 2061 2047 656e 4261 6e6b  t pass a GenBank
+00000f30: 2066 696c 650a 666f 7220 796f 7572 2072   file.for your r
+00000f40: 6566 6572 656e 6365 2067 656e 6f6d 6520  eference genome 
+00000f50: 746f 2074 6865 2063 6f6d 6d61 6e64 2d6c  to the command-l
+00000f60: 696e 6520 7363 7269 7074 7320 2876 6961  ine scripts (via
+00000f70: 2060 2d2d 7265 6665 7265 6e63 6560 290a   `--reference`).
+00000f80: 6f72 2074 6f20 5079 7468 6f6e 206c 6962  or to Python lib
+00000f90: 7261 7279 2066 756e 6374 696f 6e73 2e0a  rary functions..
+00000fa0: 0a23 2320 416c 6967 6e6d 656e 7420 616c  .## Alignment al
+00000fb0: 676f 7269 7468 6d73 2061 6e64 2073 7065  gorithms and spe
+00000fc0: 6564 0a0a 6067 6232 7365 7160 206d 616b  ed..`gb2seq` mak
+00000fd0: 6573 2061 6e20 616c 6967 6e6d 656e 7420  es an alignment 
+00000fe0: 6265 7477 6565 6e20 7468 6520 7265 6665  between the refe
+00000ff0: 7265 6e63 6520 7365 7175 656e 6365 2061  rence sequence a
+00001000: 6e64 2074 6f20 616e 790a 756e 616e 6e6f  nd to any.unanno
+00001010: 7461 7465 6420 6765 6e6f 6d65 2873 2920  tated genome(s) 
+00001020: 796f 7520 6769 7665 2069 742e 0a0a 5468  you give it...Th
+00001030: 6520 6465 6661 756c 7420 616c 6967 6e6d  e default alignm
+00001040: 656e 7420 616c 676f 7269 7468 6d20 6973  ent algorithm is
+00001050: 0a5b 4d41 4646 545d 2868 7474 7073 3a2f  .[MAFFT](https:/
+00001060: 2f6d 6166 6674 2e63 6272 632e 6a70 2f61  /mafft.cbrc.jp/a
+00001070: 6c69 676e 6d65 6e74 2f73 6f66 7477 6172  lignment/softwar
+00001080: 652f 292c 2077 6869 6368 2079 6f75 2077  e/), which you w
+00001090: 696c 6c20 6e65 6564 2074 6f0a 6861 7665  ill need to.have
+000010a0: 2069 6e73 7461 6c6c 6564 2069 6e20 6120   installed in a 
+000010b0: 6469 7265 6374 6f72 7920 696e 2079 6f75  directory in you
+000010c0: 7220 7368 656c 6c27 7320 6050 4154 4860  r shell's `PATH`
+000010d0: 2e0a 0a4d 4146 4654 2063 616e 2063 616e  ...MAFFT can can
+000010e0: 2062 6520 736c 6f77 2075 6e64 6572 2073   be slow under s
+000010f0: 6f6d 6520 6369 7263 756d 7374 616e 6365  ome circumstance
+00001100: 732e 2053 6f20 796f 7520 6361 6e20 616c  s. So you can al
+00001110: 736f 2072 756e 2073 6372 6970 7473 0a77  so run scripts.w
+00001120: 6974 6820 602d 2d61 6c69 676e 6572 2065  ith `--aligner e
+00001130: 646c 6962 6020 286f 7220 7061 7373 2060  dlib` (or pass `
+00001140: 616c 6967 6e65 723d 2765 646c 6962 2760  aligner='edlib'`
+00001150: 2074 6f20 6c69 6272 6172 7920 6675 6e63   to library func
+00001160: 7469 6f6e 7329 2074 6f0a 7573 6520 5b74  tions) to.use [t
+00001170: 6865 2050 7974 686f 6e20 7772 6170 7065  he Python wrappe
+00001180: 725d 2868 7474 7073 3a2f 2f70 7970 692e  r](https://pypi.
+00001190: 6f72 672f 7072 6f6a 6563 742f 6564 6c69  org/project/edli
+000011a0: 622f 2920 666f 7220 7468 6520 6661 7374  b/) for the fast
+000011b0: 0a5b 6564 6c69 625d 2868 7474 7073 3a2f  .[edlib](https:/
+000011c0: 2f67 6974 6875 622e 636f 6d2f 4d61 7274  /github.com/Mart
+000011d0: 696e 736f 732f 6564 6c69 6229 206c 6962  insos/edlib) lib
+000011e0: 7261 7279 2e20 6065 646c 6962 6020 7368  rary. `edlib` sh
+000011f0: 6f75 6c64 0a70 726f 6261 626c 7920 6265  ould.probably be
+00001200: 2074 6865 2064 6566 6175 6c74 2e0a 0a3c   the default...<
+00001210: 6120 6964 3d22 2373 6372 6970 7473 223e  a id="#scripts">
+00001220: 3c2f 613e 0a23 2055 7469 6c69 7479 2073  </a>.# Utility s
+00001230: 6372 6970 7473 0a0a 5468 6520 7363 7269  cripts..The scri
+00001240: 7074 7320 6465 7363 7269 6265 6420 6265  pts described be
+00001250: 6c6f 7720 616c 6c20 6163 6365 7074 2061  low all accept a
+00001260: 2060 2d2d 6865 6c70 6020 6f70 7469 6f6e   `--help` option
+00001270: 2e20 4265 6c6f 7720 6973 0a73 6f6d 6520  . Below is.some 
+00001280: 7265 7072 6573 656e 7461 7469 7665 2075  representative u
+00001290: 7361 6765 2e0a 0a23 2320 6465 7363 7269  sage...## descri
+000012a0: 6265 2d66 6561 7475 7265 2e70 790a 0a54  be-feature.py..T
+000012b0: 6865 2073 696d 706c 6573 7420 7363 7269  he simplest scri
+000012c0: 7074 2069 7320 6064 6573 6372 6962 652d  pt is `describe-
+000012d0: 6665 6174 7572 652e 7079 602c 2077 6869  feature.py`, whi
+000012e0: 6368 2063 616e 2062 6520 7573 6564 2074  ch can be used t
+000012f0: 6f20 6765 740a 696e 666f 726d 6174 696f  o get.informatio
+00001300: 6e20 6162 6f75 7420 6765 6e6f 6d65 2066  n about genome f
+00001310: 6561 7475 7265 732e 0a0a 4966 2079 6f75  eatures...If you
+00001320: 2067 6976 6520 6e6f 2061 7267 756d 656e   give no argumen
+00001330: 7473 2028 6f74 6865 7220 7468 616e 2069  ts (other than i
+00001340: 6e64 6963 6174 696e 6720 7468 6520 7265  ndicating the re
+00001350: 6665 7265 6e63 6520 6765 6e6f 6d65 292c  ference genome),
+00001360: 2069 740a 7769 6c6c 2070 7269 6e74 2073   it.will print s
+00001370: 756d 6d61 7279 2064 6574 6169 6c73 206f  ummary details o
+00001380: 6620 616c 6c20 6665 6174 7572 6573 2c20  f all features, 
+00001390: 7769 7468 2074 6865 6972 2028 312d 6261  with their (1-ba
+000013a0: 7365 6429 206e 7563 6c65 6f74 6964 650a  sed) nucleotide.
+000013b0: 7369 7465 732e 2049 6620 796f 7520 7761  sites. If you wa
+000013c0: 6e74 207a 6572 6f2d 6261 7365 6420 6f66  nt zero-based of
+000013d0: 6673 6574 732c 2075 7365 2060 2d2d 7a65  fsets, use `--ze
+000013e0: 726f 4261 7365 6460 2e0a 0a60 6060 7368  roBased`...```sh
+000013f0: 0a24 2064 6573 6372 6962 652d 6665 6174  .$ describe-feat
+00001400: 7572 652e 7079 202d 2d73 6172 7332 0a46  ure.py --sars2.F
+00001410: 6561 7475 7265 7320 666f 7220 4e43 5f30  eatures for NC_0
+00001420: 3435 3531 322e 323a 0a32 272d 4f2d 7269  45512.2:.2'-O-ri
+00001430: 626f 7365 206d 6574 6879 6c74 7261 6e73  bose methyltrans
+00001440: 6665 7261 7365 3a0a 2020 7374 6172 743a  ferase:.  start:
+00001450: 2032 3036 3538 0a20 2073 746f 703a 2032   20658.  stop: 2
+00001460: 3135 3532 0a20 206c 656e 6774 683a 2038  1552.  length: 8
+00001470: 3934 0a20 2070 726f 6475 6374 3a20 3227  94.  product: 2'
+00001480: 2d4f 2d72 6962 6f73 6520 6d65 7468 796c  -O-ribose methyl
+00001490: 7472 616e 7366 6572 6173 650a 2020 7365  transferase.  se
+000014a0: 7175 656e 6365 2020 2020 286c 656e 2020  quence    (len  
+000014b0: 2038 3934 206e 7429 3a20 5443 5441 4754   894 nt): TCTAGT
+000014c0: 4341 4147 4347 5447 4743 4141 4343 4747  CAAGCGTGGCAACCGG
+000014d0: 4754 4754 5447 4354 4154 4743 4354 4141  GTGTTGCTATGCCTAA
+000014e0: 5443 5454 5441 4341 4141 412e 2e2e 0a33  TCTTTACAAAA....3
+000014f0: 272d 746f 2d35 2720 6578 6f6e 7563 6c65  '-to-5' exonucle
+00001500: 6173 653a 0a20 2073 7461 7274 3a20 3138  ase:.  start: 18
+00001510: 3034 300a 2020 7374 6f70 3a20 3139 3632  040.  stop: 1962
+00001520: 300a 2020 6c65 6e67 7468 3a20 3135 3831  0.  length: 1581
+00001530: 0a20 2070 726f 6475 6374 3a20 3327 2d74  .  product: 3'-t
+00001540: 6f2d 3527 2065 786f 6e75 636c 6561 7365  o-5' exonuclease
+00001550: 0a20 2073 6571 7565 6e63 6520 2020 2028  .  sequence    (
+00001560: 6c65 6e20 2031 3538 3120 6e74 293a 2047  len  1581 nt): G
+00001570: 4354 4741 4141 4154 4754 4141 4341 4747  CTGAAAATGTAACAGG
+00001580: 4143 5443 5454 5441 4141 4741 5454 4754  ACTCTTTAAAGATTGT
+00001590: 4147 5441 4147 4754 4141 5443 4143 5447  AGTAAGGTAATCACTG
+000015a0: 2e2e 2e0a 3327 5554 523a 0a20 2073 7461  ....3'UTR:.  sta
+000015b0: 7274 3a20 3239 3637 350a 2020 7374 6f70  rt: 29675.  stop
+000015c0: 3a20 3239 3930 330a 2020 6c65 6e67 7468  : 29903.  length
+000015d0: 3a20 3232 390a 2020 7365 7175 656e 6365  : 229.  sequence
+000015e0: 2020 2020 286c 656e 2020 2032 3239 206e      (len   229 n
+000015f0: 7429 3a20 4341 4154 4354 5454 4141 5443  t): CAATCTTTAATC
+00001600: 4147 5447 5447 5441 4143 4154 5441 4747  AGTGTGTAACATTAGG
+00001610: 4741 4747 4143 5454 4741 4141 4741 4743  GAGGACTTGAAAGAGC
+00001620: 4341 4343 412e 2e2e 0a23 205b 4d61 6e79  CACCA....# [Many
+00001630: 2061 6464 6974 696f 6e61 6c20 6f75 7470   additional outp
+00001640: 7574 206c 696e 6573 206f 6d69 7474 6564  ut lines omitted
+00001650: 2068 6572 652e 5d0a 6060 600a 0a59 6f75   here.].```..You
+00001660: 2063 616e 2073 7065 6369 6679 2061 2066   can specify a f
+00001670: 6561 7475 7265 206e 616d 6520 286f 7220  eature name (or 
+00001680: 6e61 6d65 7329 3a0a 0a60 6060 7368 0a24  names):..```sh.$
+00001690: 2064 6573 6372 6962 652d 6665 6174 7572   describe-featur
+000016a0: 652e 7079 202d 2d73 6172 7332 202d 2d6e  e.py --sars2 --n
+000016b0: 616d 6520 7370 696b 650a 7375 7266 6163  ame spike.surfac
+000016c0: 6520 676c 7963 6f70 726f 7465 696e 3a0a  e glycoprotein:.
+000016d0: 2020 7374 6172 743a 2032 3135 3633 0a20    start: 21563. 
+000016e0: 2073 746f 703a 2032 3533 3834 0a20 206c   stop: 25384.  l
+000016f0: 656e 6774 683a 2033 3832 320a 2020 7072  ength: 3822.  pr
+00001700: 6f64 7563 743a 2073 7572 6661 6365 2067  oduct: surface g
+00001710: 6c79 636f 7072 6f74 6569 6e0a 2020 7365  lycoprotein.  se
+00001720: 7175 656e 6365 2020 2020 286c 656e 2020  quence    (len  
+00001730: 3338 3232 206e 7429 3a20 4154 4754 5454  3822 nt): ATGTTT
+00001740: 4754 5454 5454 4354 5447 5454 5454 4154  GTTTTTCTTGTTTTAT
+00001750: 5447 4343 4143 5441 4754 4354 4354 4147  TGCCACTAGTCTCTAG
+00001760: 5443 4147 5447 5447 5454 412e 2e2e 0a20  TCAGTGTGTTA.... 
+00001770: 2074 7261 6e73 6c61 7469 6f6e 2028 6c65   translation (le
+00001780: 6e20 2031 3237 3420 6161 293a 204d 4656  n  1274 aa): MFV
+00001790: 464c 564c 4c50 4c56 5353 5143 564e 4c54  FLVLLPLVSSQCVNLT
+000017a0: 5452 5451 4c50 5041 5954 4e53 4654 5247  TRTQLPPAYTNSFTRG
+000017b0: 5659 5950 444b 5646 5253 5356 4c48 2e2e  VYYPDKVFRSSVLH..
+000017c0: 2e0a 6060 600a 0a41 6e64 2079 6f75 2063  ..```..And you c
+000017d0: 616e 2070 6173 7320 616e 2075 6e61 6e6e  an pass an unann
+000017e0: 6f74 6174 6564 2067 656e 6f6d 6520 746f  otated genome to
+000017f0: 2067 6574 2069 6e66 6f72 6d61 7469 6f6e   get information
+00001800: 206f 6e20 7468 6520 6665 6174 7572 6520   on the feature 
+00001810: 696e 0a74 6865 2072 6566 6572 656e 6365  in.the reference
+00001820: 2061 6e64 2074 6865 2067 656e 6f6d 6520   and the genome 
+00001830: 2877 6869 6368 2077 696c 6c20 6265 2061  (which will be a
+00001840: 6c69 676e 6564 2074 6f20 7468 6520 7265  ligned to the re
+00001850: 6665 7265 6e63 6529 2e20 5468 650a 706f  ference). The.po
+00001860: 7369 7469 6f6e 2061 6e64 206c 656e 6774  sition and lengt
+00001870: 6820 6f66 2074 6865 2066 6561 7475 7265  h of the feature
+00001880: 2069 6e20 7468 6520 756e 616e 6e6f 7461   in the unannota
+00001890: 7465 6420 6765 6e6f 6d65 206d 6179 206f  ted genome may o
+000018a0: 6620 636f 7572 7365 0a64 6966 6665 7220  f course.differ 
+000018b0: 6672 6f6d 2074 6865 2072 6566 6572 656e  from the referen
+000018c0: 6365 3a0a 0a60 6060 7368 0a24 2064 6573  ce:..```sh.$ des
+000018d0: 6372 6962 652d 6665 6174 7572 652e 7079  cribe-feature.py
+000018e0: 202d 2d6e 616d 6520 7370 696b 6520 2d2d   --name spike --
+000018f0: 7361 7273 3220 2d2d 6765 6e6f 6d65 2043  sars2 --genome C
+00001900: 6856 6972 3932 3930 2e66 6173 7461 0a52  hVir9290.fasta.R
+00001910: 6566 6572 656e 6365 3a0a 2020 7375 7266  eference:.  surf
+00001920: 6163 6520 676c 7963 6f70 726f 7465 696e  ace glycoprotein
+00001930: 3a0a 2020 2020 7374 6172 743a 2032 3135  :.    start: 215
+00001940: 3633 0a20 2020 2073 746f 703a 2032 3533  63.    stop: 253
+00001950: 3834 0a20 2020 206c 656e 6774 6820 286e  84.    length (n
+00001960: 7429 3a20 3338 3232 0a20 2020 2070 726f  t): 3822.    pro
+00001970: 6475 6374 3a20 7375 7266 6163 6520 676c  duct: surface gl
+00001980: 7963 6f70 726f 7465 696e 0a20 2020 206e  ycoprotein.    n
+00001990: 6f74 653a 2073 7472 7563 7475 7261 6c20  ote: structural 
+000019a0: 7072 6f74 6569 6e3b 2073 7069 6b65 2070  protein; spike p
+000019b0: 726f 7465 696e 0a20 2020 2066 6561 7475  rotein.    featu
+000019c0: 7265 2069 7320 7472 616e 736c 6174 6564  re is translated
+000019d0: 206c 6566 742d 746f 2d72 6967 6874 2e0a   left-to-right..
+000019e0: 2020 2020 7365 7175 656e 6365 3a20 4154      sequence: AT
+000019f0: 4754 5454 4754 5454 5454 4354 5447 5454  GTTTGTTTTTCTTGTT
+00001a00: 5454 4154 5447 4343 4143 5441 4754 4354  TTATTGCCACTAGTCT
+00001a10: 4354 4147 5443 4147 5447 5447 5454 4141  CTAGTCAGTGTGTTAA
+00001a20: 5443 5454 4143 4141 4343 4147 4141 4354  TCTTACAACCAGAACT
+00001a30: 4341 4154 5441 4343 4343 4354 4743 2e2e  CAATTACCCCCTGC..
+00001a40: 2e0a 2020 2020 6c65 6e67 7468 2028 6161  ..    length (aa
+00001a50: 293a 2031 3237 340a 2020 2020 7472 616e  ): 1274.    tran
+00001a60: 736c 6174 696f 6e3a 204d 4656 464c 564c  slation: MFVFLVL
+00001a70: 4c50 4c56 5353 5143 564e 4c54 5452 5451  LPLVSSQCVNLTTRTQ
+00001a80: 4c50 5041 5954 4e53 4654 5247 5659 5950  LPPAYTNSFTRGVYYP
+00001a90: 444b 5646 5253 5356 4c48 5354 5144 4c46  DKVFRSSVLHSTQDLF
+00001aa0: 4c50 4646 534e 5654 5746 4841 4948 5653  LPFFSNVTWFHAIHVS
+00001ab0: 4754 4e47 544b 5246 442e 2e2e 0a20 2047  GTNGTKRFD....  G
+00001ac0: 656e 6f6d 6520 4265 7461 436f 562f 5265  enome BetaCoV/Re
+00001ad0: 6e64 7362 7572 672d 4563 6b65 726e 666f  ndsburg-Eckernfo
+00001ae0: 6572 6465 2f43 6856 6972 3932 3930 2f32  erde/ChVir9290/2
+00001af0: 3032 303a 0a20 2020 2073 7461 7274 3a20  020:.    start: 
+00001b00: 3231 3535 300a 2020 2020 7374 6f70 3a20  21550.    stop: 
+00001b10: 3235 3336 360a 2020 2020 6c65 6e67 7468  25366.    length
+00001b20: 2028 6e74 293a 2033 3832 320a 2020 2020   (nt): 3822.    
+00001b30: 7365 7175 656e 6365 3a20 4154 4754 5454  sequence: ATGTTT
+00001b40: 4754 5454 5454 4354 5447 5454 5454 4154  GTTTTTCTTGTTTTAT
+00001b50: 5447 4343 4143 5441 4754 4354 4354 4147  TGCCACTAGTCTCTAG
+00001b60: 5443 4147 5447 5447 5454 4141 5443 5454  TCAGTGTGTTAATCTT
+00001b70: 4143 4141 4343 4147 4141 4354 4341 4154  ACAACCAGAACTCAAT
+00001b80: 5441 4343 4343 4354 4743 2e2e 2e0a 2020  TACCCCCTGC....  
+00001b90: 2020 7472 616e 736c 6174 696f 6e3a 204d    translation: M
+00001ba0: 4656 464c 564c 4c50 4c56 5353 5143 564e  FVFLVLLPLVSSQCVN
+00001bb0: 4c54 5452 5451 4c50 5041 5954 4e53 4654  LTTRTQLPPAYTNSFT
+00001bc0: 5247 5659 5950 444b 5646 5253 5356 4c48  RGVYYPDKVFRSSVLH
+00001bd0: 5354 5144 4c46 4c50 4646 534e 5654 5746  STQDLFLPFFSNVTWF
+00001be0: 4841 4953 4754 4e47 544b 5246 444e 502e  HAISGTNGTKRFDNP.
+00001bf0: 2e2e 0a60 6060 0a0a 4f72 2079 6f75 2063  ...```..Or you c
+00001c00: 616e 2075 7365 2060 2d2d 6e61 6d65 7360  an use `--names`
+00001c10: 2074 6f20 6765 7420 6120 6c69 7374 206f   to get a list o
+00001c20: 6620 616c 6c20 6665 6174 7572 6520 6e61  f all feature na
+00001c30: 6d65 732e 2020 4966 2060 2d2d 7361 7273  mes.  If `--sars
+00001c40: 3260 0a69 7320 7573 6564 2c20 6e61 6d65  2`.is used, name
+00001c50: 7320 6172 6520 7072 696e 7465 6420 666f  s are printed fo
+00001c60: 6c6c 6f77 6564 2062 7920 6120 636f 6c6f  llowed by a colo
+00001c70: 6e20 616e 6420 6120 2870 6f73 7369 626c  n and a (possibl
+00001c80: 7920 656d 7074 7929 206c 6973 740a 6f66  y empty) list.of
+00001c90: 2061 6c69 6173 6573 3a0a 0a60 6060 7368   aliases:..```sh
+00001ca0: 0a24 2064 6573 6372 6962 652d 6665 6174  .$ describe-feat
+00001cb0: 7572 652e 7079 202d 2d73 6172 7332 202d  ure.py --sars2 -
+00001cc0: 2d6e 616d 6573 0a32 272d 4f2d 7269 626f  -names.2'-O-ribo
+00001cd0: 7365 206d 6574 6879 6c74 7261 6e73 6665  se methyltransfe
+00001ce0: 7261 7365 3a20 320a 3327 2d74 6f2d 3527  rase: 2.3'-to-5'
+00001cf0: 2065 786f 6e75 636c 6561 7365 3a20 6578   exonuclease: ex
+00001d00: 6f6e 2c20 6578 6f6e 7563 6c65 6173 652c  on, exonuclease,
+00001d10: 206e 7370 3134 0a33 2755 5452 3a20 3375   nsp14.3'UTR: 3u
+00001d20: 7472 0a33 432d 6c69 6b65 2070 726f 7465  tr.3C-like prote
+00001d30: 696e 6173 653a 2033 636c 7072 6f2c 206d  inase: 3clpro, m
+00001d40: 7072 6f2c 206e 7370 350a 3527 5554 523a  pro, nsp5.5'UTR:
+00001d50: 2035 7574 720a 656e 646f 524e 4173 653a   5utr.endoRNAse:
+00001d60: 2065 6e64 6f72 6e61 7365 2c20 6e73 7031   endornase, nsp1
+00001d70: 350a 656e 7665 6c6f 7065 2070 726f 7465  5.envelope prote
+00001d80: 696e 3a20 652c 2065 6e76 656c 6f70 652c  in: e, envelope,
+00001d90: 206f 7266 340a 6865 6c69 6361 7365 3a20   orf4.helicase: 
+00001da0: 6e73 7031 330a 6c65 6164 6572 2070 726f  nsp13.leader pro
+00001db0: 7465 696e 3a20 6c65 6164 6572 2c20 6e73  tein: leader, ns
+00001dc0: 7031 0a6d 656d 6272 616e 6520 676c 7963  p1.membrane glyc
+00001dd0: 6f70 726f 7465 696e 3a20 6d2c 206d 656d  oprotein: m, mem
+00001de0: 6272 616e 652c 206f 7266 350a 6e73 7032  brane, orf5.nsp2
+00001df0: 3a0a 6e73 7033 3a0a 6e73 7034 3a0a 6e73  :.nsp3:.nsp4:.ns
+00001e00: 7036 3a0a 6e73 7037 3a0a 6e73 7038 3a0a  p6:.nsp7:.nsp8:.
+00001e10: 6e73 7039 3a0a 6e73 7031 303a 0a6e 7370  nsp9:.nsp10:.nsp
+00001e20: 3131 3a0a 6e75 636c 656f 6361 7073 6964  11:.nucleocapsid
+00001e30: 2070 686f 7370 686f 7072 6f74 6569 6e3a   phosphoprotein:
+00001e40: 206e 2c20 6f72 6639 0a4f 5246 3161 6220   n, orf9.ORF1ab 
+00001e50: 706f 6c79 7072 6f74 6569 6e3a 206f 7266  polyprotein: orf
+00001e60: 3161 620a 4f52 4631 6120 706f 6c79 7072  1ab.ORF1a polypr
+00001e70: 6f74 6569 6e3a 206f 7266 3161 0a4f 5246  otein: orf1a.ORF
+00001e80: 3361 2070 726f 7465 696e 3a20 6f72 6633  3a protein: orf3
+00001e90: 610a 4f52 4636 2070 726f 7465 696e 3a20  a.ORF6 protein: 
+00001ea0: 6f72 6636 0a4f 5246 3761 2070 726f 7465  orf6.ORF7a prote
+00001eb0: 696e 3a20 6f72 6637 610a 4f52 4637 623a  in: orf7a.ORF7b:
+00001ec0: 206f 7266 3762 0a4f 5246 3820 7072 6f74   orf7b.ORF8 prot
+00001ed0: 6569 6e3a 206f 7266 380a 4f52 4631 3020  ein: orf8.ORF10 
+00001ee0: 7072 6f74 6569 6e3a 206f 7266 3130 0a52  protein: orf10.R
+00001ef0: 4e41 2d64 6570 656e 6465 6e74 2052 4e41  NA-dependent RNA
+00001f00: 2070 6f6c 796d 6572 6173 653a 206e 7370   polymerase: nsp
+00001f10: 3132 2c20 7264 7270 0a73 7465 6d20 6c6f  12, rdrp.stem lo
+00001f20: 6f70 2031 3a20 736c 310a 7374 656d 206c  op 1: sl1.stem l
+00001f30: 6f6f 7020 323a 2073 6c32 0a73 7465 6d20  oop 2: sl2.stem 
+00001f40: 6c6f 6f70 2033 3a20 736c 330a 7374 656d  loop 3: sl3.stem
+00001f50: 206c 6f6f 7020 343a 2073 6c34 0a73 7465   loop 4: sl4.ste
+00001f60: 6d20 6c6f 6f70 2035 3a20 736c 350a 7375  m loop 5: sl5.su
+00001f70: 7266 6163 6520 676c 7963 6f70 726f 7465  rface glycoprote
+00001f80: 696e 3a20 732c 2073 7069 6b65 0a60 6060  in: s, spike.```
+00001f90: 0a0a 5468 6572 6520 6973 2061 2060 2d2d  ..There is a `--
+00001fa0: 736f 7274 4279 6020 6f70 7469 6f6e 2066  sortBy` option f
+00001fb0: 6f72 2073 6f72 7469 6e67 2074 6865 206f  or sorting the o
+00001fc0: 7264 6572 206f 6620 7468 6520 7265 706f  rder of the repo
+00001fd0: 7274 6564 0a66 6561 7475 7265 732e 2054  rted.features. T
+00001fe0: 6865 2064 6566 6175 6c74 2069 7320 7468  he default is th
+00001ff0: 6520 6f72 6465 7220 7468 6579 2061 7265  e order they are
+00002000: 2067 6976 656e 206f 6e20 7468 6520 636f   given on the co
+00002010: 6d6d 616e 6420 6c69 6e65 2e0a 4f74 6865  mmand line..Othe
+00002020: 7220 6f70 7469 6f6e 7320 6172 6520 602d  r options are `-
+00002030: 2d73 6f72 7442 7920 6e61 6d65 6020 616e  -sortBy name` an
+00002040: 6420 602d 2d73 6f72 7442 7920 7369 7465  d `--sortBy site
+00002050: 6020 2869 2e65 2e2c 2069 6e63 7265 6173  ` (i.e., increas
+00002060: 696e 670a 6765 6e6f 6d65 2073 7461 7274  ing.genome start
+00002070: 2070 6f73 6974 696f 6e29 2e0a 0a23 2320   position)...## 
+00002080: 6465 7363 7269 6265 2d73 6974 652e 7079  describe-site.py
+00002090: 0a0a 5072 696e 7473 2069 6e66 6f72 6d61  ..Prints informa
+000020a0: 7469 6f6e 2061 626f 7574 2061 2067 6976  tion about a giv
+000020b0: 656e 206c 6f63 6174 696f 6e20 696e 2074  en location in t
+000020c0: 6865 2067 656e 6f6d 652c 2073 686f 7769  he genome, showi
+000020d0: 6e67 2079 6f75 2077 6861 7427 730a 696e  ng you what's.in
+000020e0: 2074 6865 2072 6566 6572 656e 6365 2061   the reference a
+000020f0: 6e64 2074 6865 2075 6e61 6e6e 6f74 6174  nd the unannotat
+00002100: 6564 2067 656e 6f6d 6520 796f 7520 286f  ed genome you (o
+00002110: 7074 696f 6e61 6c6c 7929 2070 6173 732e  ptionally) pass.
+00002120: 0a0a 496e 2074 6865 2073 696d 706c 6573  ..In the simples
+00002130: 7420 6361 7365 2c20 6769 7665 2061 2028  t case, give a (
+00002140: 312d 6261 7365 6429 2073 6974 6520 6e75  1-based) site nu
+00002150: 6d62 6572 2061 6e64 2079 6f75 276c 6c20  mber and you'll 
+00002160: 7365 6520 7768 6174 2773 2061 740a 7468  see what's at.th
+00002170: 6174 206c 6f63 6174 696f 6e20 696e 2074  at location in t
+00002180: 6865 2072 6566 6572 656e 6365 2e20 5468  he reference. Th
+00002190: 6520 6f75 7470 7574 2073 686f 7773 2031  e output shows 1
+000021a0: 2d62 6173 6564 2073 6974 6573 2e20 5573  -based sites. Us
+000021b0: 650a 602d 2d7a 6572 6f42 6173 6564 6020  e.`--zeroBased` 
+000021c0: 746f 2067 6574 2030 2d62 6173 6564 206f  to get 0-based o
+000021d0: 6666 7365 7473 2e0a 0a60 6060 7368 0a24  ffsets...```sh.$
+000021e0: 2064 6573 6372 6962 652d 7369 7465 2e70   describe-site.p
+000021f0: 7920 2d2d 7361 7273 3220 2d2d 7369 7465  y --sars2 --site
+00002200: 2032 3630 3030 0a7b 0a20 2020 2022 616c   26000.{.    "al
+00002210: 6967 6e6d 656e 744f 6666 7365 7422 3a20  ignmentOffset": 
+00002220: 3236 3030 302c 0a20 2020 2022 6665 6174  26000,.    "feat
+00002230: 7572 654e 616d 6522 3a20 224f 5246 3361  ureName": "ORF3a
+00002240: 2070 726f 7465 696e 222c 0a20 2020 2022   protein",.    "
+00002250: 6665 6174 7572 654e 616d 6573 223a 205b  featureNames": [
+00002260: 0a20 2020 2020 2020 2022 4f52 4633 6120  .        "ORF3a 
+00002270: 7072 6f74 6569 6e22 0a20 2020 205d 2c0a  protein".    ],.
+00002280: 2020 2020 2272 6566 6572 656e 6365 223a      "reference":
+00002290: 207b 0a20 2020 2020 2020 2022 6161 223a   {.        "aa":
+000022a0: 2022 4c22 2c0a 2020 2020 2020 2020 2261   "L",.        "a
+000022b0: 614f 6666 7365 7422 3a20 3230 322c 0a20  aOffset": 202,. 
+000022c0: 2020 2020 2020 2022 636f 646f 6e22 3a20         "codon": 
+000022d0: 2254 5441 222c 0a20 2020 2020 2020 2022  "TTA",.        "
+000022e0: 6672 616d 6522 3a20 312c 0a20 2020 2020  frame": 1,.     
+000022f0: 2020 2022 6964 223a 2022 4e43 5f30 3435     "id": "NC_045
+00002300: 3531 322e 3222 2c0a 2020 2020 2020 2020  512.2",.        
+00002310: 226e 744f 6666 7365 7422 3a20 3236 3030  "ntOffset": 2600
+00002320: 300a 2020 2020 7d0a 7d0a 6060 600a 0a41  0.    }.}.```..A
+00002330: 7420 7468 6520 6d6f 6d65 6e74 2c20 7468  t the moment, th
+00002340: 6520 6f75 7470 7574 2069 7320 6120 4a53  e output is a JS
+00002350: 4f4e 206f 626a 6563 742c 2074 686f 7567  ON object, thoug
+00002360: 6820 7468 6973 206d 6179 2073 6f6d 6564  h this may somed
+00002370: 6179 2063 6861 6e67 650a 746f 2061 206d  ay change.to a m
+00002380: 6f72 6520 7665 7262 6f73 652f 7265 6164  ore verbose/read
+00002390: 6162 6c65 2066 6f72 6d2e 2055 7365 2060  able form. Use `
+000023a0: 2d2d 6a73 6f6e 6020 746f 206d 616b 6520  --json` to make 
+000023b0: 7375 7265 2079 6f75 2061 6c77 6179 7320  sure you always 
+000023c0: 6765 740a 4a53 4f4e 2e0a 0a59 6f75 2063  get.JSON...You c
+000023d0: 616e 2061 6c73 6f20 7370 6563 6966 7920  an also specify 
+000023e0: 7468 6520 7369 7465 206e 756d 6265 7220  the site number 
+000023f0: 7265 6c61 7469 7665 2074 6f20 6120 6665  relative to a fe
+00002400: 6174 7572 653a 0a0a 6060 6073 680a 2420  ature:..```sh.$ 
+00002410: 6465 7363 7269 6265 2d73 6974 652e 7079  describe-site.py
+00002420: 202d 2d73 6172 7332 202d 2d73 6974 6520   --sars2 --site 
+00002430: 3135 3031 202d 2d66 6561 7475 7265 2073  1501 --feature s
+00002440: 7069 6b65 202d 2d72 656c 6174 6976 650a  pike --relative.
+00002450: 7b0a 2020 2020 2261 6c69 676e 6d65 6e74  {.    "alignment
+00002460: 4f66 6673 6574 223a 2032 3330 3633 2c0a  Offset": 23063,.
+00002470: 2020 2020 2266 6561 7475 7265 4e61 6d65      "featureName
+00002480: 223a 2022 7375 7266 6163 6520 676c 7963  ": "surface glyc
+00002490: 6f70 726f 7465 696e 222c 0a20 2020 2022  oprotein",.    "
+000024a0: 6665 6174 7572 654e 616d 6573 223a 205b  featureNames": [
+000024b0: 0a20 2020 2020 2020 2022 7375 7266 6163  .        "surfac
+000024c0: 6520 676c 7963 6f70 726f 7465 696e 220a  e glycoprotein".
+000024d0: 2020 2020 5d2c 0a20 2020 2022 7265 6665      ],.    "refe
+000024e0: 7265 6e63 6522 3a20 7b0a 2020 2020 2020  rence": {.      
+000024f0: 2020 2261 6122 3a20 224e 222c 0a20 2020    "aa": "N",.   
+00002500: 2020 2020 2022 6161 4f66 6673 6574 223a       "aaOffset":
+00002510: 2035 3030 2c0a 2020 2020 2020 2020 2263   500,.        "c
+00002520: 6f64 6f6e 223a 2022 4141 5422 2c0a 2020  odon": "AAT",.  
+00002530: 2020 2020 2020 2266 7261 6d65 223a 2030        "frame": 0
+00002540: 2c0a 2020 2020 2020 2020 2269 6422 3a20  ,.        "id": 
+00002550: 224e 435f 3034 3535 3132 2e32 222c 0a20  "NC_045512.2",. 
+00002560: 2020 2020 2020 2022 6e74 4f66 6673 6574         "ntOffset
+00002570: 223a 2032 3330 3633 0a20 2020 207d 0a7d  ": 23063.    }.}
+00002580: 0a60 6060 0a0a 4f72 2070 6173 7320 616e  .```..Or pass an
+00002590: 2061 6d69 6e6f 2061 6369 6420 7369 7465   amino acid site
+000025a0: 206e 756d 6265 7220 2876 6961 2060 2d2d   number (via `--
+000025b0: 6161 6029 3a0a 0a60 6060 7368 0a24 2064  aa`):..```sh.$ d
+000025c0: 6573 6372 6962 652d 7369 7465 2e70 7920  escribe-site.py 
+000025d0: 2d2d 7361 7273 3220 2d2d 7369 7465 2035  --sars2 --site 5
+000025e0: 3031 202d 2d66 6561 7475 7265 2073 7069  01 --feature spi
+000025f0: 6b65 202d 2d72 656c 6174 6976 6520 2d2d  ke --relative --
+00002600: 6161 0a7b 0a20 2020 2022 616c 6967 6e6d  aa.{.    "alignm
+00002610: 656e 744f 6666 7365 7422 3a20 3233 3036  entOffset": 2306
+00002620: 332c 0a20 2020 2022 6665 6174 7572 654e  3,.    "featureN
+00002630: 616d 6522 3a20 2273 7572 6661 6365 2067  ame": "surface g
+00002640: 6c79 636f 7072 6f74 6569 6e22 2c0a 2020  lycoprotein",.  
+00002650: 2020 2266 6561 7475 7265 4e61 6d65 7322    "featureNames"
+00002660: 3a20 5b0a 2020 2020 2020 2020 2273 7572  : [.        "sur
+00002670: 6661 6365 2067 6c79 636f 7072 6f74 6569  face glycoprotei
+00002680: 6e22 0a20 2020 205d 2c0a 2020 2020 2272  n".    ],.    "r
+00002690: 6566 6572 656e 6365 223a 207b 0a20 2020  eference": {.   
+000026a0: 2020 2020 2022 6161 223a 2022 4e22 2c0a       "aa": "N",.
+000026b0: 2020 2020 2020 2020 2261 614f 6666 7365          "aaOffse
+000026c0: 7422 3a20 3530 302c 0a20 2020 2020 2020  t": 500,.       
+000026d0: 2022 636f 646f 6e22 3a20 2241 4154 222c   "codon": "AAT",
+000026e0: 0a20 2020 2020 2020 2022 6672 616d 6522  .        "frame"
+000026f0: 3a20 302c 0a20 2020 2020 2020 2022 6964  : 0,.        "id
+00002700: 223a 2022 4e43 5f30 3435 3531 322e 3222  ": "NC_045512.2"
+00002710: 2c0a 2020 2020 2020 2020 226e 744f 6666  ,.        "ntOff
+00002720: 7365 7422 3a20 3233 3036 330a 2020 2020  set": 23063.    
+00002730: 7d0a 7d0a 6060 600a 0a4f 6620 636f 7572  }.}.```..Of cour
+00002740: 7365 2069 7427 7320 6d6f 7265 2066 756e  se it's more fun
+00002750: 2069 6620 796f 7520 616c 736f 2070 726f   if you also pro
+00002760: 7669 6465 2061 6e20 756e 616e 6e6f 7461  vide an unannota
+00002770: 7465 6420 6765 6e6f 6d65 2074 6f0a 636f  ted genome to.co
+00002780: 6d70 6172 6520 7468 6520 7265 6665 7265  mpare the refere
+00002790: 6e63 6520 746f 2e20 2048 6572 6527 7320  nce to.  Here's 
+000027a0: 7468 6520 604e 3530 3159 6020 6368 616e  the `N501Y` chan
+000027b0: 6765 2069 6e20 6120 5341 5253 2d43 6f56  ge in a SARS-CoV
+000027c0: 2d32 0a42 2e31 2e31 2e37 2028 416c 7068  -2.B.1.1.7 (Alph
+000027d0: 6120 7661 7269 616e 7429 2073 6571 7565  a variant) seque
+000027e0: 6e63 653a 0a0a 6060 6073 680a 2420 6465  nce:..```sh.$ de
+000027f0: 7363 7269 6265 2d73 6974 652e 7079 202d  scribe-site.py -
+00002800: 2d73 6172 7332 202d 2d73 6974 6520 3530  -sars2 --site 50
+00002810: 3120 2d2d 7265 6c61 7469 7665 202d 2d67  1 --relative --g
+00002820: 656e 6f6d 6520 6461 7461 2f45 5049 5f49  enome data/EPI_I
+00002830: 534c 5f36 3031 3434 332e 6661 7374 6120  SL_601443.fasta 
+00002840: 5c0a 2020 2020 2d2d 6665 6174 7572 6520  \.    --feature 
+00002850: 7370 696b 6520 2d2d 6161 0a7b 0a20 2020  spike --aa.{.   
+00002860: 2022 616c 6967 6e6d 656e 744f 6666 7365   "alignmentOffse
+00002870: 7422 3a20 3233 3036 332c 0a20 2020 2022  t": 23063,.    "
+00002880: 6665 6174 7572 654e 616d 6522 3a20 2273  featureName": "s
+00002890: 7572 6661 6365 2067 6c79 636f 7072 6f74  urface glycoprot
+000028a0: 6569 6e22 2c0a 2020 2020 2266 6561 7475  ein",.    "featu
+000028b0: 7265 4e61 6d65 7322 3a20 5b0a 2020 2020  reNames": [.    
+000028c0: 2020 2020 2273 7572 6661 6365 2067 6c79      "surface gly
+000028d0: 636f 7072 6f74 6569 6e22 0a20 2020 205d  coprotein".    ]
+000028e0: 2c0a 2020 2020 2267 656e 6f6d 6522 3a20  ,.    "genome": 
+000028f0: 7b0a 2020 2020 2020 2020 2261 6122 3a20  {.        "aa": 
+00002900: 2259 222c 0a20 2020 2020 2020 2022 6161  "Y",.        "aa
+00002910: 4f66 6673 6574 223a 2034 3937 2c0a 2020  Offset": 497,.  
+00002920: 2020 2020 2020 2263 6f64 6f6e 223a 2022        "codon": "
+00002930: 5441 5422 2c0a 2020 2020 2020 2020 2266  TAT",.        "f
+00002940: 7261 6d65 223a 2030 2c0a 2020 2020 2020  rame": 0,.      
+00002950: 2020 2269 6422 3a20 2245 5049 5f49 534c    "id": "EPI_ISL
+00002960: 5f36 3031 3434 3320 6843 6f56 2d31 392f  _601443 hCoV-19/
+00002970: 456e 676c 616e 642f 4d49 4c4b 2d39 4530  England/MILK-9E0
+00002980: 3542 332f 3230 3230 222c 0a20 2020 2020  5B3/2020",.     
+00002990: 2020 2022 6e74 4f66 6673 6574 223a 2032     "ntOffset": 2
+000029a0: 3239 3931 0a20 2020 207d 2c0a 2020 2020  2991.    },.    
+000029b0: 2272 6566 6572 656e 6365 223a 207b 0a20  "reference": {. 
+000029c0: 2020 2020 2020 2022 6161 223a 2022 4e22         "aa": "N"
+000029d0: 2c0a 2020 2020 2020 2020 2261 614f 6666  ,.        "aaOff
+000029e0: 7365 7422 3a20 3530 302c 0a20 2020 2020  set": 500,.     
+000029f0: 2020 2022 636f 646f 6e22 3a20 2241 4154     "codon": "AAT
+00002a00: 222c 0a20 2020 2020 2020 2022 6672 616d  ",.        "fram
+00002a10: 6522 3a20 302c 0a20 2020 2020 2020 2022  e": 0,.        "
+00002a20: 6964 223a 2022 4e43 5f30 3435 3531 322e  id": "NC_045512.
+00002a30: 3222 2c0a 2020 2020 2020 2020 226e 744f  2",.        "ntO
+00002a40: 6666 7365 7422 3a20 3233 3036 330a 2020  ffset": 23063.  
+00002a50: 2020 7d0a 7d0a 6060 600a 0a4f 7468 6572    }.}.```..Other
+00002a60: 206f 7074 696f 6e73 2069 6e63 6c75 6465   options include
+00002a70: 2060 2d2d 6765 6e6f 6d65 4161 4f6e 6c79   `--genomeAaOnly
+00002a80: 6020 746f 206a 7573 7420 7072 696e 7420  ` to just print 
+00002a90: 7468 6520 616d 696e 6f20 6163 6964 2061  the amino acid a
+00002aa0: 7420 610a 6c6f 6361 7469 6f6e 2069 6e20  t a.location in 
+00002ab0: 7468 6520 6765 6e6f 6d65 2c20 602d 2d69  the genome, `--i
+00002ac0: 6e63 6c75 6465 4665 6174 7572 6560 2074  ncludeFeature` t
+00002ad0: 6f20 616c 736f 2072 6563 6569 7665 2069  o also receive i
+00002ae0: 6e66 6f72 6d61 7469 6f6e 0a61 626f 7574  nformation.about
+00002af0: 2074 6865 2066 6561 7475 7265 2061 7420   the feature at 
+00002b00: 7468 6520 7369 7465 2c20 616e 6420 602d  the site, and `-
+00002b10: 2d6d 696e 5265 6665 7265 6e63 6543 6f76  -minReferenceCov
+00002b20: 6572 6167 6560 2074 6f20 6578 636c 7564  erage` to exclud
+00002b30: 650a 6c6f 772d 636f 7665 7261 6765 2067  e.low-coverage g
+00002b40: 656e 6f6d 6573 206f 7220 6665 6174 7572  enomes or featur
+00002b50: 6573 2066 726f 6d20 7468 6520 7265 7375  es from the resu
+00002b60: 6c74 732e 0a0a 2323 2064 6573 6372 6962  lts...## describ
+00002b70: 652d 6765 6e6f 6d65 2e70 790a 0a60 6465  e-genome.py..`de
+00002b80: 7363 7269 6265 2d67 656e 6f6d 652e 7079  scribe-genome.py
+00002b90: 6020 6861 7320 6d61 6e79 2075 7365 732e  ` has many uses.
+00002ba0: 2049 7420 6361 6e20 6578 7472 6163 7420   It can extract 
+00002bb0: 6d75 6c74 6970 6c65 2066 6561 7475 7265  multiple feature
+00002bc0: 7320 6672 6f6d 0a6d 756c 7469 706c 6520  s from.multiple 
+00002bd0: 6769 7665 6e20 6765 6e6f 6d65 732c 2061  given genomes, a
+00002be0: 7320 616d 696e 6f20 6163 6964 7320 6f72  s amino acids or
+00002bf0: 206e 7563 6c65 6f74 6964 6573 206f 7220   nucleotides or 
+00002c00: 626f 7468 2e20 4974 2077 696c 6c0a 7072  both. It will.pr
+00002c10: 696e 7420 746f 2073 7461 6e64 6172 6420  int to standard 
+00002c20: 6f75 7470 7574 2062 7920 6465 6661 756c  output by defaul
+00002c30: 742c 2062 7574 2069 6620 796f 7520 7573  t, but if you us
+00002c40: 6520 7468 6520 602d 2d6f 7574 4469 7260  e the `--outDir`
+00002c50: 206f 7074 696f 6e0a 746f 2070 726f 7669   option.to provi
+00002c60: 6465 2061 2064 6972 6563 746f 7279 2c20  de a directory, 
+00002c70: 696e 6469 7669 6475 616c 206f 7574 7075  individual outpu
+00002c80: 7420 6669 6c65 7320 7769 7468 2028 686f  t files with (ho
+00002c90: 7065 6675 6c6c 7929 0a73 656c 662d 6578  pefully).self-ex
+00002ca0: 706c 616e 6174 6f72 7920 6e61 6d65 7320  planatory names 
+00002cb0: 7769 6c6c 2062 6520 6372 6561 7465 6420  will be created 
+00002cc0: 696e 2074 6861 7420 6469 7265 6374 6f72  in that director
+00002cd0: 792e 2054 6865 2064 6972 6563 746f 7279  y. The directory
+00002ce0: 0a77 696c 6c20 6265 2063 7265 6174 6564  .will be created
+00002cf0: 2066 6f72 2079 6f75 2069 6620 6974 2064   for you if it d
+00002d00: 6f65 736e 2774 2065 7869 7374 2e0a 0a41  oesn't exist...A
+00002d10: 2073 6d61 6c6c 2065 7861 6d70 6c65 2069   small example i
+00002d20: 7320 7065 7268 6170 7320 6265 7374 2e20  s perhaps best. 
+00002d30: 4865 7265 2077 6520 6578 7472 6163 7420  Here we extract 
+00002d40: 7468 6520 7370 696b 6520 6e75 636c 656f  the spike nucleo
+00002d50: 7469 6465 2061 6e64 0a61 6d69 6e6f 2061  tide and.amino a
+00002d60: 6369 6420 7365 7175 656e 6365 2066 726f  cid sequence fro
+00002d70: 6d20 422e 312e 312e 3720 616e 6420 616c  m B.1.1.7 and al
+00002d80: 736f 2061 736b 2066 6f72 2061 2073 756d  so ask for a sum
+00002d90: 6d61 7279 206f 6620 7468 6520 616d 696e  mary of the amin
+00002da0: 6f0a 6163 6964 2064 6966 6665 7265 6e63  o.acid differenc
+00002db0: 6573 3a0a 0a60 6060 7368 0a24 2064 6573  es:..```sh.$ des
+00002dc0: 6372 6962 652d 6765 6e6f 6d65 2e70 7920  cribe-genome.py 
+00002dd0: 2d2d 6765 6e6f 6d65 2064 6174 612f 4550  --genome data/EP
+00002de0: 495f 4953 4c5f 3630 3134 3433 2e66 6173  I_ISL_601443.fas
+00002df0: 7461 202d 2d6f 7574 4469 7220 2f74 6d70  ta --outDir /tmp
+00002e00: 2f6f 7574 205c 0a20 2020 202d 2d66 6561  /out \.    --fea
+00002e10: 7475 7265 2073 7069 6b65 202d 2d70 7269  ture spike --pri
+00002e20: 6e74 4e74 5365 7175 656e 6365 202d 2d70  ntNtSequence --p
+00002e30: 7269 6e74 4161 5365 7175 656e 6365 202d  rintAaSequence -
+00002e40: 2d70 7269 6e74 4161 4d61 7463 680a 4578  -printAaMatch.Ex
+00002e50: 616d 696e 6564 2031 2067 656e 6f6d 652e  amined 1 genome.
+00002e60: 0a0a 2420 6c73 202d 6c20 2f74 6d70 2f6f  ..$ ls -l /tmp/o
+00002e70: 7574 0a74 6f74 616c 2032 340a 2d72 772d  ut.total 24.-rw-
+00002e80: 7277 2d72 2d2d 2020 3120 7465 7272 7920  rw-r--  1 terry 
+00002e90: 2077 6865 656c 2020 2037 3438 2041 7072   wheel   748 Apr
+00002ea0: 2031 3120 3135 3a32 3520 4550 495f 4953   11 15:25 EPI_IS
+00002eb0: 4c5f 3630 3134 3433 2d73 7069 6b65 2d61  L_601443-spike-a
+00002ec0: 612d 6d61 7463 682e 7478 740a 2d72 772d  a-match.txt.-rw-
+00002ed0: 7277 2d72 2d2d 2020 3120 7465 7272 7920  rw-r--  1 terry 
+00002ee0: 2077 6865 656c 2020 3133 3434 2041 7072   wheel  1344 Apr
+00002ef0: 2031 3120 3135 3a32 3520 4550 495f 4953   11 15:25 EPI_IS
+00002f00: 4c5f 3630 3134 3433 2d73 7069 6b65 2d61  L_601443-spike-a
+00002f10: 612d 7365 7175 656e 6365 2e66 6173 7461  a-sequence.fasta
+00002f20: 0a2d 7277 2d72 772d 722d 2d20 2031 2074  .-rw-rw-r--  1 t
+00002f30: 6572 7279 2020 7768 6565 6c20 2033 3838  erry  wheel  388
+00002f40: 3620 4170 7220 3131 2031 353a 3235 2045  6 Apr 11 15:25 E
+00002f50: 5049 5f49 534c 5f36 3031 3434 332d 7370  PI_ISL_601443-sp
+00002f60: 696b 652d 6e74 2d73 6571 7565 6e63 652e  ike-nt-sequence.
+00002f70: 6661 7374 610a 6060 600a 0a49 6620 7468  fasta.```..If th
+00002f80: 6520 6669 6c65 2067 6976 656e 2062 7920  e file given by 
+00002f90: 602d 2d67 656e 6f6d 6560 2068 6164 2063  `--genome` had c
+00002fa0: 6f6e 7461 696e 6564 206d 6f72 6520 7468  ontained more th
+00002fb0: 616e 206f 6e65 2053 4152 532d 436f 562d  an one SARS-CoV-
+00002fc0: 320a 6765 6e6f 6d65 2c20 7468 6520 7370  2.genome, the sp
+00002fd0: 696b 6520 776f 756c 6420 6861 7665 2062  ike would have b
+00002fe0: 6565 6e20 6578 7472 6163 7465 6420 666f  een extracted fo
+00002ff0: 7220 616c 6c20 6f66 2074 6865 6d2e 2053  r all of them. S
+00003000: 696d 696c 6172 6c79 2c20 6966 0a60 2d2d  imilarly, if.`--
+00003010: 6665 6174 7572 6560 2068 6164 2062 6565  feature` had bee
+00003020: 6e20 7265 7065 6174 6564 2c20 6d75 6c74  n repeated, mult
+00003030: 6970 6c65 2066 6561 7475 7265 7320 776f  iple features wo
+00003040: 756c 6420 6861 7665 2062 6565 6e20 6578  uld have been ex
+00003050: 7472 6163 7465 640a 616e 6420 636f 6d70  tracted.and comp
+00003060: 6172 6564 2e20 4966 206e 6f20 602d 2d66  ared. If no `--f
+00003070: 6561 7475 7265 6020 6973 2067 6976 656e  eature` is given
+00003080: 2c20 796f 7527 6c6c 2067 6574 2074 6865  , you'll get the
+00003090: 6d20 616c 6c2e 0a0a 6060 6073 680a 2420  m all...```sh.$ 
+000030a0: 6361 7420 2f74 6d70 2f6f 7574 2f45 5049  cat /tmp/out/EPI
+000030b0: 5f49 534c 5f36 3031 3434 332d 7370 696b  _ISL_601443-spik
+000030c0: 652d 6161 2d6d 6174 6368 2e74 7874 0a46  e-aa-match.txt.F
+000030d0: 6561 7475 7265 3a20 7370 696b 6520 616d  eature: spike am
+000030e0: 696e 6f20 6163 6964 206d 6174 6368 0a20  ino acid match. 
+000030f0: 204d 6174 6368 6573 3a20 3132 3634 2f31   Matches: 1264/1
+00003100: 3237 3420 2839 392e 3232 2529 0a20 204d  274 (99.22%).  M
+00003110: 6973 6d61 7463 6865 733a 2031 302f 3132  ismatches: 10/12
+00003120: 3734 2028 302e 3738 2529 0a20 2020 204e  74 (0.78%).    N
+00003130: 6f74 2069 6e76 6f6c 7669 6e67 2067 6170  ot involving gap
+00003140: 7320 2869 2e65 2e2c 2063 6f6e 666c 6963  s (i.e., conflic
+00003150: 7473 293a 2037 2f31 3237 3420 2830 2e35  ts): 7/1274 (0.5
+00003160: 3525 290a 2020 2020 496e 766f 6c76 696e  5%).    Involvin
+00003170: 6720 6120 6761 7020 696e 206f 6e65 2073  g a gap in one s
+00003180: 6571 7565 6e63 653a 2033 2f31 3237 3420  equence: 3/1274 
+00003190: 2830 2e32 3425 290a 2020 2020 496e 766f  (0.24%).    Invo
+000031a0: 6c76 696e 6720 6120 6761 7020 696e 2062  lving a gap in b
+000031b0: 6f74 6820 7365 7175 656e 6365 733a 2030  oth sequences: 0
+000031c0: 0a20 2020 2049 643a 204e 435f 3034 3535  .    Id: NC_0455
+000031d0: 3132 2e32 2028 7375 7266 6163 6520 676c  12.2 (surface gl
+000031e0: 7963 6f70 726f 7465 696e 290a 2020 2020  ycoprotein).    
+000031f0: 2020 4c65 6e67 7468 3a20 3132 3734 0a20    Length: 1274. 
+00003200: 2020 2020 2047 6170 733a 2030 0a20 2020       Gaps: 0.   
+00003210: 2049 643a 2045 5049 5f49 534c 5f36 3031   Id: EPI_ISL_601
+00003220: 3434 3320 6843 6f56 2d31 392f 456e 676c  443 hCoV-19/Engl
+00003230: 616e 642f 4d49 4c4b 2d39 4530 3542 332f  and/MILK-9E05B3/
+00003240: 3230 3230 2028 7375 7266 6163 6520 676c  2020 (surface gl
+00003250: 7963 6f70 726f 7465 696e 290a 2020 2020  ycoprotein).    
+00003260: 2020 4c65 6e67 7468 3a20 3132 3734 0a20    Length: 1274. 
+00003270: 2020 2020 2047 6170 733a 2033 2f31 3237       Gaps: 3/127
+00003280: 3420 2830 2e32 3425 290a 2020 2020 2020  4 (0.24%).      
+00003290: 4761 7020 6c6f 6361 7469 6f6e 7320 2831  Gap locations (1
+000032a0: 2d62 6173 6564 293a 2036 392c 2037 302c  -based): 69, 70,
+000032b0: 2031 3434 0a20 2020 2044 6966 6665 7265   144.    Differe
+000032c0: 6e63 6573 3a20 7369 7465 2c20 6161 312c  nces: site, aa1,
+000032d0: 2061 6132 2c20 7265 6620 6e74 2063 6f64   aa2, ref nt cod
+000032e0: 6f6e 2073 7461 7274 0a20 2020 2020 2020  on start.       
+000032f0: 2036 3920 4820 2d20 3231 3736 370a 2020   69 H - 21767.  
+00003300: 2020 2020 2020 3730 2056 202d 2032 3137        70 V - 217
+00003310: 3730 0a20 2020 2020 2020 3134 3420 5920  70.       144 Y 
+00003320: 2d20 3231 3939 320a 2020 2020 2020 2035  - 21992.       5
+00003330: 3031 204e 2059 2032 3330 3633 0a20 2020  01 N Y 23063.   
+00003340: 2020 2020 3537 3020 4120 4420 3233 3237      570 A D 2327
+00003350: 300a 2020 2020 2020 2036 3134 2044 2047  0.       614 D G
+00003360: 2032 3334 3032 0a20 2020 2020 2020 3638   23402.       68
+00003370: 3120 5020 4820 3233 3630 330a 2020 2020  1 P H 23603.    
+00003380: 2020 2037 3136 2054 2049 2032 3337 3038     716 T I 23708
+00003390: 0a20 2020 2020 2020 3938 3220 5320 4120  .       982 S A 
+000033a0: 3234 3530 360a 2020 2020 2020 3131 3138  24506.      1118
+000033b0: 2044 2048 2032 3439 3134 0a60 6060 0a0a   D H 24914.```..
+000033c0: 596f 7520 6361 6e20 616c 736f 2061 736b  You can also ask
+000033d0: 2066 6f72 2074 6865 2063 6861 6e67 6573   for the changes
+000033e0: 2069 6e20 6120 7661 7269 616e 7420 746f   in a variant to
+000033f0: 2062 6520 6368 6563 6b65 642e 0a20 2020   be checked..   
+00003400: 2020 200a 6060 6073 680a 2420 6465 7363     .```sh.$ desc
+00003410: 7269 6265 2d67 656e 6f6d 652e 7079 202d  ribe-genome.py -
+00003420: 2d73 6172 7332 202d 2d67 656e 6f6d 6520  -sars2 --genome 
+00003430: 6461 7461 2f45 5049 5f49 534c 5f36 3031  data/EPI_ISL_601
+00003440: 3434 332e 6661 7374 6120 2d2d 6368 6563  443.fasta --chec
+00003450: 6b56 6172 6961 6e74 2056 4f43 5f32 3032  kVariant VOC_202
+00003460: 3031 3230 315f 554b 0a45 5049 5f49 534c  01201_UK.EPI_ISL
+00003470: 5f36 3031 3434 3320 6843 6f56 2d31 392f  _601443 hCoV-19/
+00003480: 456e 676c 616e 642f 4d49 4c4b 2d39 4530  England/MILK-9E0
+00003490: 3542 332f 3230 3230 0a56 6172 6961 6e74  5B3/2020.Variant
+000034a0: 2073 756d 6d61 7279 3a0a 2020 554b 2076   summary:.  UK v
+000034b0: 6172 6961 6e74 206f 6620 636f 6e63 6572  ariant of concer
+000034c0: 6e20 2856 4f43 2920 3230 3230 3132 2f30  n (VOC) 202012/0
+000034d0: 313a 0a20 2032 3020 6368 6563 6b73 2c20  1:.  20 checks, 
+000034e0: 3230 2070 6173 7365 642e 0a20 2020 206f  20 passed..    o
+000034f0: 7266 3161 6220 6161 3a20 5041 5353 3a20  rf1ab aa: PASS: 
+00003500: 3130 3031 492c 2031 3730 3844 2c20 3232  1001I, 1708D, 22
+00003510: 3330 542c 2033 3637 352d 2c20 3336 3736  30T, 3675-, 3676
+00003520: 2d2c 2033 3637 372d 0a20 2020 2073 7069  -, 3677-.    spi
+00003530: 6b65 2061 613a 2050 4153 533a 2031 3131  ke aa: PASS: 111
+00003540: 3848 2c20 3134 342d 2c20 3530 3159 2c20  8H, 144-, 501Y, 
+00003550: 3537 3044 2c20 3638 3148 2c20 3639 2d2c  570D, 681H, 69-,
+00003560: 2037 302d 2c20 3731 3649 2c20 3938 3241   70-, 716I, 982A
+00003570: 0a20 2020 206f 7266 3820 6161 3a20 5041  .    orf8 aa: PA
+00003580: 5353 3a20 3532 492c 2037 3343 2c20 5132  SS: 52I, 73C, Q2
+00003590: 372a 0a20 2020 206e 2061 613a 2050 4153  7*.    n aa: PAS
+000035a0: 533a 2032 3335 462c 2033 4c0a 6060 600a  S: 235F, 3L.```.
+000035b0: 0a54 6865 7265 2061 7265 2073 6f6d 6520  .There are some 
+000035c0: 6b6e 6f77 6e20 7661 7269 616e 7473 2c20  known variants, 
+000035d0: 616e 6420 796f 7520 6361 6e20 616c 736f  and you can also
+000035e0: 2070 726f 7669 6465 2079 6f75 7220 6f77   provide your ow
+000035f0: 6e20 7669 6120 6120 4a53 4f4e 0a66 696c  n via a JSON.fil
+00003600: 6520 616e 6420 7468 6520 602d 2d76 6172  e and the `--var
+00003610: 6961 6e74 4669 6c65 6020 6f70 7469 6f6e  iantFile` option
+00003620: 2e20 596f 7572 204a 534f 4e20 7368 6f75  . Your JSON shou
+00003630: 6c64 2068 6176 6520 7468 6520 666f 726d  ld have the form
+00003640: 6174 0a79 6f75 276c 6c20 7365 6520 696e  at.you'll see in
+00003650: 0a5b 7661 7269 616e 7473 2e70 795d 2868  .[variants.py](h
+00003660: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00003670: 6d2f 5669 726f 6c6f 6779 4368 6172 6974  m/VirologyCharit
+00003680: 652f 6762 3273 6571 2f62 6c6f 622f 6d61  e/gb2seq/blob/ma
+00003690: 7374 6572 2f67 6232 7365 712f 7661 7269  ster/gb2seq/vari
+000036a0: 616e 7473 2e70 7929 2e20 452e 672e 2c3a  ants.py). E.g.,:
+000036b0: 0a0a 6060 600a 5641 5249 414e 5453 203d  ..```.VARIANTS =
+000036c0: 207b 0a20 2020 2027 564f 435f 3230 3230   {.    'VOC_2020
+000036d0: 3132 3031 5f55 4b27 3a20 7b0a 2020 2020  1201_UK': {.    
+000036e0: 2020 2020 2764 6573 6372 6970 7469 6f6e      'description
+000036f0: 273a 2027 554b 2076 6172 6961 6e74 206f  ': 'UK variant o
+00003700: 6620 636f 6e63 6572 6e20 2856 4f43 2920  f concern (VOC) 
+00003710: 3230 3230 3132 2f30 3127 2c0a 2020 2020  202012/01',.    
+00003720: 2020 2020 2763 6f6d 6d65 6e74 273a 2028      'comment': (
+00003730: 2746 726f 6d20 5461 626c 6520 3120 6f66  'From Table 1 of
+00003740: 2068 7474 7073 3a2f 2f77 7777 2e67 6f76   https://www.gov
+00003750: 2e75 6b2f 676f 7665 726e 6d65 6e74 2f27  .uk/government/'
+00003760: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003770: 2020 2020 2027 7075 626c 6963 6174 696f       'publicatio
+00003780: 6e73 2f69 6e76 6573 7469 6761 7469 6f6e  ns/investigation
+00003790: 2d6f 662d 6e6f 7665 6c2d 7361 7273 2d63  -of-novel-sars-c
+000037a0: 6f76 2d32 270a 2020 2020 2020 2020 2020  ov-2'.          
+000037b0: 2020 2020 2020 2020 2020 272d 7661 7269            '-vari
+000037c0: 616e 742d 7661 7269 616e 742d 6f66 2d63  ant-variant-of-c
+000037d0: 6f6e 6365 726e 2d32 3032 3031 3230 3127  oncern-20201201'
+000037e0: 292c 0a20 2020 2020 2020 2027 6368 616e  ),.        'chan
+000037f0: 6765 7327 3a20 7b0a 2020 2020 2020 2020  ges': {.        
+00003800: 2020 2020 276f 7266 3161 6227 3a20 7b0a      'orf1ab': {.
+00003810: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003820: 2761 6127 3a20 2731 3030 3149 2031 3730  'aa': '1001I 170
+00003830: 3844 2032 3233 3054 2033 3637 352d 2033  8D 2230T 3675- 3
+00003840: 3637 362d 2033 3637 372d 272c 0a20 2020  676- 3677-',.   
+00003850: 2020 2020 2020 2020 207d 2c0a 2020 2020           },.    
+00003860: 2020 2020 2020 2020 2773 7069 6b65 273a          'spike':
+00003870: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+00003880: 2020 2027 6161 273a 2027 3639 2d20 3730     'aa': '69- 70
+00003890: 2d20 3134 342d 2035 3031 5920 3537 3044  - 144- 501Y 570D
+000038a0: 2036 3831 4820 3731 3649 2039 3832 4120   681H 716I 982A 
+000038b0: 3131 3138 4827 2c0a 2020 2020 2020 2020  1118H',.        
+000038c0: 2020 2020 7d2c 0a20 2020 2020 2020 2020      },.         
+000038d0: 2020 2027 6f72 6638 273a 207b 0a20 2020     'orf8': {.   
+000038e0: 2020 2020 2020 2020 2020 2020 2027 6161               'aa
+000038f0: 273a 2027 5132 372a 2035 3249 2037 3343  ': 'Q27* 52I 73C
+00003900: 272c 0a20 2020 2020 2020 2020 2020 207d  ',.            }
+00003910: 2c0a 2020 2020 2020 2020 2020 2020 276e  ,.            'n
+00003920: 273a 207b 0a20 2020 2020 2020 2020 2020  ': {.           
+00003930: 2020 2020 2027 6161 273a 2027 334c 2032       'aa': '3L 2
+00003940: 3335 4627 2c0a 2020 2020 2020 2020 2020  35F',.          
+00003950: 2020 7d0a 2020 2020 2020 2020 7d0a 2020    }.        }.  
+00003960: 2020 7d0a 7d0a 6060 600a 0a23 2320 616e    }.}.```..## an
+00003970: 6e6f 7461 7465 2d67 656e 6f6d 652e 7079  notate-genome.py
+00003980: 0a0a 5072 6f64 7563 6573 204a 534f 4e20  ..Produces JSON 
+00003990: 6f75 7470 7574 2077 6974 6820 616e 6e6f  output with anno
+000039a0: 7461 7469 6f6e 2069 6e66 6f72 6d61 7469  tation informati
+000039b0: 6f6e 2066 6f72 2061 2067 656e 6f6d 652e  on for a genome.
+000039c0: 2048 6572 6527 7320 616e 0a65 7861 6d70   Here's an.examp
+000039d0: 6c65 206f 6620 7468 6520 7374 6172 7420  le of the start 
+000039e0: 6f66 206f 7574 7075 7420 666f 7220 6120  of output for a 
+000039f0: 4d6f 6e6b 6579 706f 7820 6765 6e6f 6d65  Monkeypox genome
+00003a00: 2028 6e6f 7465 2074 6861 7420 7468 650a   (note that the.
+00003a10: 6e75 636c 656f 7469 6465 2073 6571 7565  nucleotide seque
+00003a20: 6e63 6573 2068 6176 6520 6265 656e 2074  nces have been t
+00003a30: 7275 6e63 6174 6564 2074 6f20 7265 6475  runcated to redu
+00003a40: 6365 206f 7574 7075 7420 7769 6474 6829  ce output width)
+00003a50: 3a0a 0a60 6060 7368 0a24 2061 6e6e 6f74  :..```sh.$ annot
+00003a60: 6174 652d 6765 6e6f 6d65 2e70 7920 2d2d  ate-genome.py --
+00003a70: 616c 6967 6e65 7220 6564 6c69 6220 2d2d  aligner edlib --
+00003a80: 7265 6665 7265 6e63 6520 4f4e 3637 3637  reference ON6767
+00003a90: 3038 2e31 2e67 6220 2d2d 6765 6e6f 6d65  08.1.gb --genome
+00003aa0: 2043 6856 6972 3238 3338 392e 6661 7374   ChVir28389.fast
+00003ab0: 610a 7b0a 2020 2020 2266 6561 7475 7265  a.{.    "feature
+00003ac0: 7322 3a20 7b0a 2020 2020 2020 2020 2241  s": {.        "A
+00003ad0: 3135 2e35 4c22 3a20 7b0a 2020 2020 2020  15.5L": {.      
+00003ae0: 2020 2020 2020 2267 656e 6f6d 6522 3a20        "genome": 
+00003af0: 7b0a 2020 2020 2020 2020 2020 2020 2020  {.              
+00003b00: 2020 2273 6571 7565 6e63 6522 3a20 2241    "sequence": "A
+00003b10: 5447 4154 4141 4754 4141 5454 4143 4741  TGATAAGTAATTACGA
+00003b20: 4743 4347 5454 4743 5447 4354 4754 5441  GCCGTTGCTGCTGTTA
+00003b30: 4754 5441 5441 4143 2e2e 2e22 2c0a 2020  GTTATAAC...",.  
+00003b40: 2020 2020 2020 2020 2020 2020 2020 2273                "s
+00003b50: 7461 7274 223a 2031 3231 3832 332c 0a20  tart": 121823,. 
+00003b60: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00003b70: 7374 6f70 223a 2031 3231 3938 352c 0a20  stop": 121985,. 
+00003b80: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00003b90: 7472 616e 736c 6174 696f 6e22 3a20 224d  translation": "M
+00003ba0: 4953 4e59 4550 4c4c 4c4c 5649 5443 4356  ISNYEPLLLLVITCCV
+00003bb0: 4c4c 464e 4654 4953 534b 544b 4944 4949  LLFNFTISSKTKIDII
+00003bc0: 4641 5651 5449 5646 4957 4649 4648 4656  FAVQTIVFIWFIFHFV
+00003bd0: 5953 4149 2a22 0a20 2020 2020 2020 2020  YSAI*".         
+00003be0: 2020 207d 2c0a 2020 2020 2020 2020 2020     },.          
+00003bf0: 2020 2272 6566 6572 656e 6365 223a 207b    "reference": {
+00003c00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003c10: 2022 666f 7277 6172 6422 3a20 6661 6c73   "forward": fals
+00003c20: 652c 0a20 2020 2020 2020 2020 2020 2020  e,.             
+00003c30: 2020 2022 6e61 6d65 223a 2022 4131 352e     "name": "A15.
+00003c40: 354c 222c 0a20 2020 2020 2020 2020 2020  5L",.           
+00003c50: 2020 2020 2022 6e6f 7465 223a 2022 4e6f       "note": "No
+00003c60: 6e2d 6573 7365 6e74 6961 6c20 494d 5620  n-essential IMV 
+00003c70: 6d65 6d62 7261 6e65 2070 726f 7465 696e  membrane protein
+00003c80: 2028 436f 702d 4131 342e 354c 2922 2c0a   (Cop-A14.5L)",.
+00003c90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00003ca0: 2270 726f 6475 6374 223a 2022 4131 352e  "product": "A15.
+00003cb0: 354c 222c 0a20 2020 2020 2020 2020 2020  5L",.           
+00003cc0: 2020 2020 2022 7365 7175 656e 6365 223a       "sequence":
+00003cd0: 2022 5454 4141 4154 4347 4343 4741 4154   "TTAAATCGCCGAAT
+00003ce0: 4141 4143 4141 4147 5447 4741 4154 4154  AAACAAAGTGGAATAT
+00003cf0: 4141 4143 4341 5441 5441 412e 2e2e 222c  AAACCATATAA...",
+00003d00: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00003d10: 2022 7374 6172 7422 3a20 3132 3137 3539   "start": 121759
+00003d20: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00003d30: 2020 2273 746f 7022 3a20 3132 3139 3231    "stop": 121921
+00003d40: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+00003d50: 2020 2274 7261 6e73 6c61 7469 6f6e 223a    "translation":
+00003d60: 2022 4d49 534e 5945 504c 4c4c 4c56 4954   "MISNYEPLLLLVIT
+00003d70: 4343 564c 4c46 4e46 5449 5353 4b54 4b49  CCVLLFNFTISSKTKI
+00003d80: 4449 4946 4156 5154 4956 4649 5746 4946  DIIFAVQTIVFIWFIF
+00003d90: 4846 5659 5341 492a 220a 2020 2020 2020  HFVYSAI*".      
+00003da0: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+00003db0: 7d2c 0a20 2020 2020 2020 2022 4133 322e  },.        "A32.
+00003dc0: 354c 223a 207b 0a20 2020 2020 2020 2020  5L": {.         
+00003dd0: 2020 2022 6765 6e6f 6d65 223a 207b 0a20     "genome": {. 
+00003de0: 2020 2020 2020 2020 2020 2020 2020 2022                 "
+00003df0: 7365 7175 656e 6365 223a 2022 4154 4754  sequence": "ATGT
+00003e00: 5441 4141 4141 5447 5443 4147 4354 4743  TAAAAATGTCAGCTGC
+00003e10: 4347 4143 5454 5454 5447 4741 4143 4754  CGACTTTTTGGAACGT
+00003e20: 5454 4741 542e 2e2e 222c 0a20 2020 2020  TTGAT...",.     
+00003e30: 2020 2020 2020 2020 2020 2022 7374 6172             "star
+00003e40: 7422 3a20 3133 3936 3936 2c0a 2020 2020  t": 139696,.    
+00003e50: 2020 2020 2020 2020 2020 2020 2273 746f              "sto
+00003e60: 7022 3a20 3133 3938 3235 2c0a 2020 2020  p": 139825,.    
+00003e70: 2020 2020 2020 2020 2020 2020 2274 7261              "tra
+00003e80: 6e73 6c61 7469 6f6e 223a 2022 4d4c 4b4d  nslation": "MLKM
+00003e90: 5341 4144 464c 4552 4c49 4b41 4749 5949  SAADFLERLIKAGIYI
+00003ea0: 5956 4c52 544b 5956 4954 414c 4c56 4b4e  YVLRTKYVITALLVKN
+00003eb0: 5950 494b 4445 2a22 0a20 2020 2020 2020  YPIKDE*".       
+00003ec0: 2020 2020 207d 2c0a 2020 2020 2020 2020       },.        
+00003ed0: 2020 2020 2272 6566 6572 656e 6365 223a      "reference":
+00003ee0: 207b 0a20 2020 2020 2020 2020 2020 2020   {.             
+00003ef0: 2020 2022 666f 7277 6172 6422 3a20 6661     "forward": fa
+00003f00: 6c73 652c 0a20 2020 2020 2020 2020 2020  lse,.           
+00003f10: 2020 2020 2022 6e61 6d65 223a 2022 4133       "name": "A3
+00003f20: 322e 354c 222c 0a20 2020 2020 2020 2020  2.5L",.         
+00003f30: 2020 2020 2020 2022 6e6f 7465 223a 2022         "note": "
+00003f40: 5669 7261 6c20 6d65 6d62 7261 6e65 2061  Viral membrane a
+00003f50: 7373 656d 626c 7920 7072 6f74 6569 6e73  ssembly proteins
+00003f60: 2028 564d 4150 2920 2843 6f70 2d41 2033   (VMAP) (Cop-A 3
+00003f70: 302e 354c 2922 2c0a 2020 2020 2020 2020  0.5L)",.        
+00003f80: 2020 2020 2020 2020 2270 726f 6475 6374          "product
+00003f90: 223a 2022 4133 322e 354c 222c 0a20 2020  ": "A32.5L",.   
+00003fa0: 2020 2020 2020 2020 2020 2020 2022 7365               "se
+00003fb0: 7175 656e 6365 223a 2022 5454 4154 5443  quence": "TTATTC
+00003fc0: 4754 4354 5454 5441 5447 4747 4154 4147  GTCTTTTATGGGATAG
+00003fd0: 5454 5454 5441 4143 5441 4754 4141 4147  TTTTTAACTAGTAAAG
+00003fe0: 4354 4754 4141 2e2e 2e22 2c0a 2020 2020  CTGTAA...",.    
+00003ff0: 2020 2020 2020 2020 2020 2020 2273 7461              "sta
+00004000: 7274 223a 2031 3339 3633 352c 0a20 2020  rt": 139635,.   
+00004010: 2020 2020 2020 2020 2020 2020 2022 7374               "st
+00004020: 6f70 223a 2031 3339 3736 342c 0a20 2020  op": 139764,.   
+00004030: 2020 2020 2020 2020 2020 2020 2022 7472               "tr
+00004040: 616e 736c 6174 696f 6e22 3a20 224d 4c4b  anslation": "MLK
+00004050: 4d53 4141 4446 4c45 524c 494b 4147 4959  MSAADFLERLIKAGIY
+00004060: 4959 564c 5254 4b59 5649 5441 4c4c 564b  IYVLRTKYVITALLVK
+00004070: 4e59 5049 4b44 452a 220a 2020 2020 2020  NYPIKDE*".      
+00004080: 2020 2020 2020 7d0a 2020 2020 2020 2020        }.        
+00004090: 7d2c 0a7d 0a60 6060 0a0a 5468 6520 6f75  },.}.```..The ou
+000040a0: 7470 7574 204a 534f 4e20 6973 206e 6f74  tput JSON is not
+000040b0: 2072 6561 6c6c 7920 696e 7465 6e64 6564   really intended
+000040c0: 2066 6f72 2068 756d 616e 2063 6f6e 7375   for human consu
+000040d0: 6d70 7469 6f6e 2061 6e64 2c20 666f 7220  mption and, for 
+000040e0: 6e6f 772c 0a61 6c77 6179 7320 636f 6e74  now,.always cont
+000040f0: 6169 6e73 2030 2d62 6173 6564 2067 656e  ains 0-based gen
+00004100: 6f6d 6520 6f66 6673 6574 732e 0a0a 3c61  ome offsets...<a
+00004110: 2069 643d 2223 6170 6922 3e3c 2f61 3e0a   id="#api"></a>.
+00004120: 2320 5079 7468 6f6e 2041 5049 0a0a 5468  # Python API..Th
+00004130: 6572 6520 6172 6520 7477 6f20 6d61 696e  ere are two main
+00004140: 2050 7974 686f 6e20 636c 6173 7365 7320   Python classes 
+00004150: 7072 6f76 6964 6564 2062 7920 6067 6232  provided by `gb2
+00004160: 7365 7160 3a20 6046 6561 7475 7265 7360  seq`: `Features`
+00004170: 2061 6e64 0a60 4762 3241 6c69 676e 6d65   and.`Gb2Alignme
+00004180: 6e74 602e 0a0a 2323 2046 6561 7475 7265  nt`...## Feature
+00004190: 730a 0a54 6865 2060 4665 6174 7572 6573  s..The `Features
+000041a0: 6020 636c 6173 7320 7072 6f76 6964 6573  ` class provides
+000041b0: 206d 6574 686f 6473 2066 6f72 2061 6363   methods for acc
+000041c0: 6573 7369 6e67 2069 6e66 6f72 6d61 7469  essing informati
+000041d0: 6f6e 2061 626f 7574 0a67 656e 6f6d 6520  on about.genome 
+000041e0: 6665 6174 7572 6573 206f 6274 6169 6e65  features obtaine
+000041f0: 6420 6672 6f6d 0a5b 6120 4765 6e42 616e  d from.[a GenBan
+00004200: 6b20 666c 6174 2066 696c 655d 2868 7474  k flat file](htt
+00004210: 7073 3a2f 2f77 7777 2e6e 6362 692e 6e6c  ps://www.ncbi.nl
+00004220: 6d2e 6e69 682e 676f 762f 5369 7465 6d61  m.nih.gov/Sitema
+00004230: 702f 7361 6d70 6c65 7265 636f 7264 2e68  p/samplerecord.h
+00004240: 746d 6c29 2e0a 0a59 6f75 2776 6520 6c69  tml)...You've li
+00004250: 6b65 6c79 2072 756e 2061 6372 6f73 7320  kely run across 
+00004260: 7468 6573 6520 7265 636f 7264 7320 6265  these records be
+00004270: 666f 7265 2e20 452e 672e 2c20 6865 7265  fore. E.g., here
+00004280: 2773 2074 6865 2053 4152 532d 436f 562d  's the SARS-CoV-
+00004290: 320a 5775 6861 6e20 7265 6665 7265 6e63  2.Wuhan referenc
+000042a0: 652c 0a5b 4e43 5f30 3435 3531 325d 2868  e,.[NC_045512](h
+000042b0: 7474 7073 3a2f 2f77 7777 2e6e 6362 692e  ttps://www.ncbi.
+000042c0: 6e6c 6d2e 6e69 682e 676f 762f 6e75 6363  nlm.nih.gov/nucc
+000042d0: 6f72 652f 4e43 5f30 3435 3531 3229 2e20  ore/NC_045512). 
+000042e0: 546f 2064 6f77 6e6c 6f61 640a 7468 6520  To download.the 
+000042f0: 4765 6e42 616e 6b20 6669 6c65 2066 6f72  GenBank file for
+00004300: 2074 6861 7420 7265 6665 7265 6e63 6520   that reference 
+00004310: 6672 6f6d 2074 6865 204e 4342 4920 7369  from the NCBI si
+00004320: 7465 2c20 636c 6963 6b20 6f6e 2022 5365  te, click on "Se
+00004330: 6e64 2074 6f22 0a61 6e64 2073 656c 6563  nd to".and selec
+00004340: 7420 2243 6f6d 706c 6574 6520 5265 636f  t "Complete Reco
+00004350: 7264 222c 2022 4669 6c65 222c 2061 6e64  rd", "File", and
+00004360: 2022 4765 6e42 616e 6b22 2066 6f72 6d61   "GenBank" forma
+00004370: 742e 2054 6865 6e20 636c 6963 6b0a 2243  t. Then click."C
+00004380: 7265 6174 6520 4669 6c65 222e 0a0a 596f  reate File"...Yo
+00004390: 7520 6361 6e20 7061 7373 2074 6865 2070  u can pass the p
+000043a0: 6174 6820 746f 2061 2047 656e 4261 6e6b  ath to a GenBank
+000043b0: 2066 696c 6520 746f 2074 6865 2060 4665   file to the `Fe
+000043c0: 6174 7572 6573 6020 636c 6173 732e 2059  atures` class. Y
+000043d0: 6f75 2063 616e 0a61 6c73 6f20 6a75 7374  ou can.also just
+000043e0: 2070 6173 7320 616e 2061 6363 6573 7369   pass an accessi
+000043f0: 6f6e 206e 756d 6265 722c 2061 6e64 2074  on number, and t
+00004400: 6865 2066 696c 6520 7769 6c6c 2062 6520  he file will be 
+00004410: 646f 776e 6c6f 6164 6564 2066 6f72 0a79  downloaded for.y
+00004420: 6f75 2e20 4966 2079 6f75 2070 6173 7320  ou. If you pass 
+00004430: 6072 6566 6572 656e 6365 5370 6563 6966  `referenceSpecif
+00004440: 6963 6174 696f 6e60 2061 7320 604e 6f6e  ication` as `Non
+00004450: 6560 2061 6e64 2060 7361 7273 3260 2061  e` and `sars2` a
+00004460: 7320 6054 7275 6560 2c0a 7468 6520 5775  s `True`,.the Wu
+00004470: 6861 6e20 7265 6665 7265 6e63 6520 2876  han reference (v
+00004480: 6572 7369 6f6e 0a5b 4e43 5f30 3435 3531  ersion.[NC_04551
+00004490: 322e 325d 2868 7474 7073 3a2f 2f77 7777  2.2](https://www
+000044a0: 2e6e 6362 692e 6e6c 6d2e 6e69 682e 676f  .ncbi.nlm.nih.go
+000044b0: 762f 6e75 6363 6f72 652f 4e43 5f30 3435  v/nuccore/NC_045
+000044c0: 3531 322e 3229 2920 7769 6c6c 2062 650a  512.2)) will be.
+000044d0: 7573 6564 2e0a 0a59 6f75 2063 616e 2075  used...You can u
+000044e0: 7365 2061 2060 4665 6174 7572 6573 6020  se a `Features` 
+000044f0: 696e 7374 616e 6365 206c 696b 6520 6120  instance like a 
+00004500: 6469 6374 696f 6e61 7279 3a0a 0a60 6060  dictionary:..```
+00004510: 7079 0a66 726f 6d20 7070 7269 6e74 2069  py.from pprint i
+00004520: 6d70 6f72 7420 7070 7269 6e74 2061 7320  mport pprint as 
+00004530: 7070 0a66 726f 6d20 6762 3273 6571 2e66  pp.from gb2seq.f
+00004540: 6561 7475 7265 7320 696d 706f 7274 2046  eatures import F
+00004550: 6561 7475 7265 730a 0a3e 3e3e 2066 203d  eatures..>>> f =
+00004560: 2046 6561 7475 7265 7328 224e 435f 3034   Features("NC_04
+00004570: 3535 3132 2e32 2e67 6222 290a 3e3e 3e20  5512.2.gb").>>> 
+00004580: 7070 2866 5b27 6527 5d29 0a7b 276e 616d  pp(f['e']).{'nam
+00004590: 6527 3a20 2765 6e76 656c 6f70 6520 7072  e': 'envelope pr
+000045a0: 6f74 6569 6e27 2c0a 2027 6e6f 7465 273a  otein',. 'note':
+000045b0: 2027 4f52 4634 3b20 7374 7275 6374 7572   'ORF4; structur
+000045c0: 616c 2070 726f 7465 696e 3b20 4520 7072  al protein; E pr
+000045d0: 6f74 6569 6e27 2c0a 2027 7072 6f64 7563  otein',. 'produc
+000045e0: 7427 3a20 2765 6e76 656c 6f70 6520 7072  t': 'envelope pr
+000045f0: 6f74 6569 6e27 2c0a 2027 7365 7175 656e  otein',. 'sequen
+00004600: 6365 273a 2027 4154 4754 4143 5443 4154  ce': 'ATGTACTCAT
+00004610: 5443 4754 5454 4347 4741 4147 4147 4143  TCGTTTCGGAAGAGAC
+00004620: 4147 4754 4143 4754 5441 4154 4147 5454  AGGTACGTTAATAGTT
+00004630: 4141 5441 4743 4754 4143 5454 4354 5454  AATAGCGTACTTCTTT
+00004640: 5454 4354 5447 4354 5454 4347 5447 4754  TTCTTGCTTTCGTGGT
+00004650: 4154 542e 2e2e 272c 0a20 2773 7461 7274  ATT...',. 'start
+00004660: 273a 2032 3632 3434 2c0a 2027 7374 6f70  ': 26244,. 'stop
+00004670: 273a 2032 3634 3732 2c0a 2027 7472 616e  ': 26472,. 'tran
+00004680: 736c 6174 696f 6e27 3a20 274d 5953 4656  slation': 'MYSFV
+00004690: 5345 4554 4754 4c49 564e 5356 4c4c 464c  SEETGTLIVNSVLLFL
+000046a0: 4146 5656 464c 4c56 544c 4149 4c54 414c  AFVVFLLVTLAILTAL
+000046b0: 524c 4341 5943 434e 4956 4e56 534c 564b  RLCAYCCNIVNVSLVK
+000046c0: 5053 4659 5659 5352 564b 4e4c 4e53 5352  PSFYVYSRVKNLNSSR
+000046d0: 5650 444c 4c56 2a27 7d0a 0a23 2059 6f75  VPDLLV*'}..# You
+000046e0: 2063 616e 2075 7365 2061 6262 7265 7669   can use abbrevi
+000046f0: 6174 6564 206e 616d 6573 2c20 616e 6420  ated names, and 
+00004700: 6765 7420 7468 6520 6361 6e6f 6e69 6361  get the canonica
+00004710: 6c20 6e61 6d65 733a 0a3e 3e3e 2066 2e63  l names:.>>> f.c
+00004720: 616e 6f6e 6963 616c 4e61 6d65 2827 7327  anonicalName('s'
+00004730: 290a 2773 7572 6661 6365 2067 6c79 636f  ).'surface glyco
+00004740: 7072 6f74 6569 6e27 0a0a 2320 4765 7420  protein'..# Get 
+00004750: 7468 6520 6c69 7374 206f 6620 616c 6961  the list of alia
+00004760: 7365 7320 666f 7220 6120 6e61 6d65 3a0a  ses for a name:.
+00004770: 3e3e 3e20 662e 616c 6961 7365 7328 2773  >>> f.aliases('s
+00004780: 2729 0a7b 2773 7069 6b65 272c 2027 7375  ').{'spike', 'su
+00004790: 7266 6163 6520 676c 7963 6f70 726f 7465  rface glycoprote
+000047a0: 696e 272c 2027 7327 7d0a 0a23 2047 6976  in', 's'}..# Giv
+000047b0: 656e 2061 6e20 6f66 6673 6574 2072 656c  en an offset rel
+000047c0: 6174 6976 6520 746f 2061 2066 6561 7475  ative to a featu
+000047d0: 7265 2c20 6765 7420 7468 6520 6f66 6673  re, get the offs
+000047e0: 6574 2069 6e20 7468 6520 6765 6e6f 6d65  et in the genome
+000047f0: 3a0a 3e3e 3e20 662e 7265 6665 7265 6e63  :.>>> f.referenc
+00004800: 654f 6666 7365 7428 2773 7069 6b65 272c  eOffset('spike',
+00004810: 2031 3530 3329 0a32 3330 3635 0a0a 2320   1503).23065..# 
+00004820: 5361 6d65 2074 6869 6e67 2c20 6275 7420  Same thing, but 
+00004830: 7769 7468 2061 6e20 616d 696e 6f20 6163  with an amino ac
+00004840: 6964 206f 6666 7365 742e 0a3e 3e3e 2066  id offset..>>> f
+00004850: 2e72 6566 6572 656e 6365 4f66 6673 6574  .referenceOffset
+00004860: 2827 7370 696b 6527 2c20 3530 312c 2061  ('spike', 501, a
+00004870: 613d 5472 7565 290a 3233 3036 350a 0a23  a=True).23065..#
+00004880: 2057 6861 7420 6665 6174 7572 6573 2061   What features a
+00004890: 7265 2070 7265 7365 6e74 2061 7420 616e  re present at an
+000048a0: 206f 6666 7365 743f 0a3e 3e3e 2066 2e67   offset?.>>> f.g
+000048b0: 6574 4665 6174 7572 654e 616d 6573 2831  etFeatureNames(1
+000048c0: 3334 3530 290a 7b27 4f52 4631 6162 2070  3450).{'ORF1ab p
+000048d0: 6f6c 7970 726f 7465 696e 272c 2027 6e73  olyprotein', 'ns
+000048e0: 7031 3127 2c20 274f 5246 3161 2070 6f6c  p11', 'ORF1a pol
+000048f0: 7970 726f 7465 696e 272c 2027 524e 412d  yprotein', 'RNA-
+00004900: 6465 7065 6e64 656e 7420 524e 4120 706f  dependent RNA po
+00004910: 6c79 6d65 7261 7365 277d 0a0a 2320 5768  lymerase'}..# Wh
+00004920: 6174 2066 6561 7475 7265 7320 6172 6520  at features are 
+00004930: 7072 6573 656e 7420 6174 2061 6e20 6f66  present at an of
+00004940: 6673 6574 2c20 696e 636c 7564 696e 6720  fset, including 
+00004950: 7468 6f73 6520 7468 6174 2061 7265 206e  those that are n
+00004960: 6f74 2074 7261 6e73 6c61 7465 643f 0a3e  ot translated?.>
+00004970: 3e3e 2066 2e67 6574 4665 6174 7572 654e  >> f.getFeatureN
+00004980: 616d 6573 2832 3130 3030 2c20 696e 636c  ames(21000, incl
+00004990: 7564 6555 6e74 7261 6e73 6c61 7465 643d  udeUntranslated=
+000049a0: 5472 7565 290a 7b27 4f52 4631 6162 2070  True).{'ORF1ab p
+000049b0: 6f6c 7970 726f 7465 696e 272c 2022 3227  olyprotein', "2'
+000049c0: 2d4f 2d72 6962 6f73 6520 6d65 7468 796c  -O-ribose methyl
+000049d0: 7472 616e 7366 6572 6173 6522 7d0a 6060  transferase"}.``
+000049e0: 600a 0a23 2320 4762 3241 6c69 676e 6d65  `..## Gb2Alignme
+000049f0: 6e74 0a0a 5468 6520 6047 6232 416c 6967  nt..The `Gb2Alig
+00004a00: 6e6d 656e 7460 2063 6c61 7373 2063 616e  nment` class can
+00004a10: 2062 6520 7573 6564 2074 6f20 6578 7472   be used to extr
+00004a20: 6163 7420 616e 6420 636f 6d70 6172 6520  act and compare 
+00004a30: 6665 6174 7572 6573 2066 726f 6d0a 7468  features from.th
+00004a40: 6520 7265 6665 7265 6e63 6520 616e 6420  e reference and 
+00004a50: 7468 6520 6769 7665 6e20 6765 6e6f 6d65  the given genome
+00004a60: 2073 6571 7565 6e63 652e 0a0a 596f 7520   sequence...You 
+00004a70: 7061 7373 2069 7420 6120 6052 6561 6460  pass it a `Read`
+00004a80: 2069 6e73 7461 6e63 6520 6672 6f6d 2074   instance from t
+00004a90: 6865 0a5b 6461 726b 2d6d 6174 7465 725d  he.[dark-matter]
+00004aa0: 2868 7474 7073 3a2f 2f67 6974 6875 622e  (https://github.
+00004ab0: 636f 6d2f 6163 6f72 672f 6461 726b 2d6d  com/acorg/dark-m
+00004ac0: 6174 7465 7229 206d 6f64 756c 6520 2877  atter) module (w
+00004ad0: 6869 6368 2069 730a 696e 7374 616c 6c65  hich is.installe
+00004ae0: 6420 666f 7220 796f 7520 7768 656e 2079  d for you when y
+00004af0: 6f75 2069 6e73 7461 6c6c 2060 6762 3273  ou install `gb2s
+00004b00: 6571 6029 2e0a 0a60 6060 7079 0a66 726f  eq`)...```py.fro
+00004b10: 6d20 6762 3273 6571 2e61 6c69 676e 6d65  m gb2seq.alignme
+00004b20: 6e74 2069 6d70 6f72 7420 4762 3241 6c69  nt import Gb2Ali
+00004b30: 676e 6d65 6e74 0a66 726f 6d20 6762 3273  gnment.from gb2s
+00004b40: 6571 2e66 6561 7475 7265 7320 696d 706f  eq.features impo
+00004b50: 7274 2046 6561 7475 7265 730a 6672 6f6d  rt Features.from
+00004b60: 2064 6172 6b2e 7265 6164 7320 696d 706f   dark.reads impo
+00004b70: 7274 2052 6561 640a 0a66 6561 7475 7265  rt Read..feature
+00004b80: 7320 3d20 4665 6174 7572 6573 2822 4e43  s = Features("NC
+00004b90: 5f30 3435 3531 322e 322e 6762 2229 0a61  _045512.2.gb").a
+00004ba0: 6c69 676e 6d65 6e74 203d 2047 6232 416c  lignment = Gb2Al
+00004bb0: 6967 6e6d 656e 7428 5265 6164 2827 6964  ignment(Read('id
+00004bc0: 272c 2027 4147 4354 2e2e 2e27 292c 2066  ', 'AGCT...'), f
+00004bd0: 6561 7475 7265 7329 0a60 6060 0a0a 5468  eatures).```..Th
+00004be0: 6573 6520 6361 6e20 616c 736f 2062 6520  ese can also be 
+00004bf0: 7265 6164 2066 726f 6d20 6120 4641 5354  read from a FAST
+00004c00: 4120 6669 6c65 3a0a 0a60 6060 7079 0a66  A file:..```py.f
+00004c10: 726f 6d20 6762 3273 6571 2e61 6c69 676e  rom gb2seq.align
+00004c20: 6d65 6e74 2069 6d70 6f72 7420 4762 3241  ment import Gb2A
+00004c30: 6c69 676e 6d65 6e74 0a66 726f 6d20 6762  lignment.from gb
+00004c40: 3273 6571 2e66 6561 7475 7265 7320 696d  2seq.features im
+00004c50: 706f 7274 2046 6561 7475 7265 730a 6672  port Features.fr
+00004c60: 6f6d 2064 6172 6b2e 6661 7374 6120 696d  om dark.fasta im
+00004c70: 706f 7274 2046 6173 7461 5265 6164 730a  port FastaReads.
+00004c80: 0a66 6561 7475 7265 7320 3d20 4665 6174  .features = Feat
+00004c90: 7572 6573 2822 4e43 5f30 3435 3531 322e  ures("NC_045512.
+00004ca0: 322e 6762 2229 0a66 6f72 2072 6561 6420  2.gb").for read 
+00004cb0: 696e 2046 6173 7461 5265 6164 7328 2773  in FastaReads('s
+00004cc0: 6571 7565 6e63 6573 2e66 6173 7461 2729  equences.fasta')
+00004cd0: 3a0a 2020 2020 616c 6967 6e6d 656e 7420  :.    alignment 
+00004ce0: 3d20 4762 3241 6c69 676e 6d65 6e74 2872  = Gb2Alignment(r
+00004cf0: 6561 642c 2066 6561 7475 7265 7329 0a60  ead, features).`
+00004d00: 6060 0a0a 4f6e 6365 2079 6f75 2068 6176  ``..Once you hav
+00004d10: 6520 6120 6047 6232 416c 6967 6e6d 656e  e a `Gb2Alignmen
+00004d20: 7460 2069 6e73 7461 6e63 652c 2079 6f75  t` instance, you
+00004d30: 2063 616e 2061 736b 2069 7420 666f 7220   can ask it for 
+00004d40: 616c 6967 6e65 640a 7365 7175 656e 6365  aligned.sequence
+00004d50: 7320 6f72 2066 6561 7475 7265 732e 0a0a  s or features...
+00004d60: 4265 6c6f 7720 4927 6c6c 2075 7365 2074  Below I'll use t
+00004d70: 6865 2047 4953 4149 4420 6045 5049 5f49  he GISAID `EPI_I
+00004d80: 534c 5f36 3031 3434 3360 2028 422e 312e  SL_601443` (B.1.
+00004d90: 312e 372c 206f 7220 416c 7068 612c 2076  1.7, or Alpha, v
+00004da0: 6172 6961 6e74 290a 7365 7175 656e 6365  ariant).sequence
+00004db0: 2c20 7768 6963 6820 796f 7520 6361 6e20  , which you can 
+00004dc0: 6669 6e64 2069 6e0a 5b64 6174 612f 4550  find in.[data/EP
+00004dd0: 495f 4953 4c5f 3630 3134 3433 2e66 6173  I_ISL_601443.fas
+00004de0: 7461 5d28 6461 7461 2f45 5049 5f49 534c  ta](data/EPI_ISL
+00004df0: 5f36 3031 3434 332e 6661 7374 6129 2069  _601443.fasta) i
+00004e00: 6e20 7468 6973 2072 6570 6f3a 0a0a 6060  n this repo:..``
+00004e10: 6070 790a 3e3e 3e20 6672 6f6d 2070 6174  `py.>>> from pat
+00004e20: 686c 6962 2069 6d70 6f72 7420 5061 7468  hlib import Path
+00004e30: 0a3e 3e3e 2066 726f 6d20 7070 7269 6e74  .>>> from pprint
+00004e40: 2069 6d70 6f72 7420 7070 7269 6e74 2061   import pprint a
+00004e50: 7320 7070 0a3e 3e3e 2066 726f 6d20 6762  s pp.>>> from gb
+00004e60: 3273 6571 2e61 6c69 676e 6d65 6e74 2069  2seq.alignment i
+00004e70: 6d70 6f72 7420 4762 3241 6c69 676e 6d65  mport Gb2Alignme
+00004e80: 6e74 0a3e 3e3e 2066 726f 6d20 6762 3273  nt.>>> from gb2s
+00004e90: 6571 2e66 6561 7475 7265 7320 696d 706f  eq.features impo
+00004ea0: 7274 2046 6561 7475 7265 730a 3e3e 3e20  rt Features.>>> 
+00004eb0: 6672 6f6d 2064 6172 6b2e 6661 7374 6120  from dark.fasta 
+00004ec0: 696d 706f 7274 2046 6173 7461 5265 6164  import FastaRead
+00004ed0: 730a 0a3e 3e3e 2061 6c70 6861 203d 206c  s..>>> alpha = l
+00004ee0: 6973 7428 4661 7374 6152 6561 6473 2850  ist(FastaReads(P
+00004ef0: 6174 6828 2764 6174 612f 4550 495f 4953  ath('data/EPI_IS
+00004f00: 4c5f 3630 3134 3433 2e66 6173 7461 2729  L_601443.fasta')
+00004f10: 2929 5b30 5d0a 3e3e 3e20 6c65 6e28 616c  ))[0].>>> len(al
+00004f20: 7068 6129 0a32 3937 3634 0a3e 3e3e 2061  pha).29764.>>> a
+00004f30: 6c70 6861 2e69 640a 2745 5049 5f49 534c  lpha.id.'EPI_ISL
+00004f40: 5f36 3031 3434 3320 6843 6f56 2d31 392f  _601443 hCoV-19/
+00004f50: 456e 676c 616e 642f 4d49 4c4b 2d39 4530  England/MILK-9E0
+00004f60: 3542 332f 3230 3230 270a 3e3e 3e20 616c  5B3/2020'.>>> al
+00004f70: 7068 612e 7365 7175 656e 6365 5b3a 3530  pha.sequence[:50
+00004f80: 5d0a 2741 4741 5443 5447 5454 4354 4354  ].'AGATCTGTTCTCT
+00004f90: 4141 4143 4741 4143 5454 5441 4141 4154  AAACGAACTTTAAAAT
+00004fa0: 4354 4754 4754 4747 4354 4754 4341 4354  CTGTGTGGCTGTCACT
+00004fb0: 4347 4743 5427 0a0a 3e3e 3e20 6665 6174  CGGCT'..>>> feat
+00004fc0: 7572 6573 203d 2046 6561 7475 7265 7328  ures = Features(
+00004fd0: 7361 7273 323d 5472 7565 290a 3e3e 3e20  sars2=True).>>> 
+00004fe0: 616c 6967 6e6d 656e 7420 3d20 4762 3241  alignment = Gb2A
+00004ff0: 6c69 676e 6d65 6e74 2861 6c70 6861 290a  lignment(alpha).
+00005000: 6060 600a 0a59 6f75 276c 6c20 6669 6e64  ```..You'll find
+00005010: 2074 6865 2061 6c69 676e 6564 2072 6566   the aligned ref
+00005020: 6572 656e 6365 2061 6e64 2067 656e 6f6d  erence and genom
+00005030: 6520 696e 2060 616c 6967 6e6d 656e 742e  e in `alignment.
+00005040: 7265 6665 7265 6e63 6541 6c69 676e 6564  referenceAligned
+00005050: 600a 616e 6420 6061 6c69 676e 6d65 6e74  `.and `alignment
+00005060: 2e67 656e 6f6d 6541 6c69 676e 6564 602c  .genomeAligned`,
+00005070: 2062 6f74 6820 6f66 2077 6869 6368 2061   both of which a
+00005080: 7265 2020 6052 6561 6460 2069 6e73 7461  re  `Read` insta
+00005090: 6e63 6573 3a0a 0a60 6060 7079 0a3e 3e3e  nces:..```py.>>>
+000050a0: 206c 656e 2861 6c69 676e 6d65 6e74 2e72   len(alignment.r
+000050b0: 6566 6572 656e 6365 416c 6967 6e65 6429  eferenceAligned)
+000050c0: 0a32 3939 3033 0a3e 3e3e 206c 656e 2861  .29903.>>> len(a
+000050d0: 6c69 676e 6d65 6e74 2e67 656e 6f6d 6541  lignment.genomeA
+000050e0: 6c69 676e 6564 290a 3239 3930 330a 0a23  ligned).29903..#
+000050f0: 2047 6574 2074 6865 206e 7563 6c65 6f74   Get the nucleot
+00005100: 6964 6520 7365 7175 656e 6365 2066 6f72  ide sequence for
+00005110: 2074 6865 2073 7069 6b65 2070 726f 7465   the spike prote
+00005120: 696e 2066 6f72 2074 6865 2072 6566 6572  in for the refer
+00005130: 656e 6365 2061 6e64 2067 656e 6f6d 652e  ence and genome.
+00005140: 0a3e 3e3e 2072 6566 6572 656e 6365 5370  .>>> referenceSp
+00005150: 696b 654e 742c 2067 656e 6f6d 6553 7069  ikeNt, genomeSpi
+00005160: 6b65 4e74 203d 2061 6c69 676e 6d65 6e74  keNt = alignment
+00005170: 2e6e 7453 6571 7565 6e63 6573 2827 7370  .ntSequences('sp
+00005180: 696b 6527 290a 3e3e 3e20 6c65 6e28 7265  ike').>>> len(re
+00005190: 6665 7265 6e63 6553 7069 6b65 4e74 290a  ferenceSpikeNt).
+000051a0: 3338 3232 0a0a 2320 4765 7420 7468 6520  3822..# Get the 
+000051b0: 616d 696e 6f20 6163 6964 2073 6571 7565  amino acid seque
+000051c0: 6e63 6520 666f 7220 7468 6520 7370 696b  nce for the spik
+000051d0: 6520 7072 6f74 6569 6e20 666f 7220 7468  e protein for th
+000051e0: 6520 7265 6665 7265 6e63 6520 616e 6420  e reference and 
+000051f0: 6765 6e6f 6d65 2e0a 3e3e 3e20 7265 6665  genome..>>> refe
+00005200: 7265 6e63 6553 7069 6b65 4161 2c20 6765  renceSpikeAa, ge
+00005210: 6e6f 6d65 5370 696b 6541 6120 3d20 616c  nomeSpikeAa = al
+00005220: 6967 6e6d 656e 742e 6161 5365 7175 656e  ignment.aaSequen
+00005230: 6365 7328 2773 7069 6b65 2729 0a3e 3e3e  ces('spike').>>>
+00005240: 206c 656e 2872 6566 6572 656e 6365 5370   len(referenceSp
+00005250: 696b 6541 6129 0a31 3237 340a 0a23 2054  ikeAa).1274..# T
+00005260: 6865 7265 2077 6572 6520 7468 7265 6520  here were three 
+00005270: 6465 6c65 7469 6f6e 7320 696e 2074 6865  deletions in the
+00005280: 2061 6c70 6861 2073 7069 6b65 2c20 736f   alpha spike, so
+00005290: 2069 7420 6f6e 6c79 2063 6f76 6572 7320   it only covers 
+000052a0: 3338 3133 206f 6620 7468 650a 2320 3338  3813 of the.# 38
+000052b0: 3232 2062 6173 6573 2069 6e20 7468 6520  22 bases in the 
+000052c0: 7265 6665 7265 6e63 6520 7370 696b 652e  reference spike.
+000052d0: 0a3e 3e3e 2061 6c69 676e 6d65 6e74 2e63  .>>> alignment.c
+000052e0: 6f76 6572 6167 6528 2773 2729 0a28 3338  overage('s').(38
+000052f0: 3133 2c20 3338 3232 290a 0a23 2047 6574  13, 3822)..# Get
+00005300: 2069 6e66 6f72 6d61 7469 6f6e 2061 626f   information abo
+00005310: 7574 2077 6861 7427 7320 6174 2061 6e20  ut what's at an 
+00005320: 6f66 6673 6574 2028 302d 6261 7365 6429  offset (0-based)
+00005330: 2e20 5468 6973 2069 7320 7768 6174 2074  . This is what t
+00005340: 6865 2064 6573 6372 6962 652d 7369 7465  he describe-site
+00005350: 2e70 790a 2320 7574 696c 6974 7920 646f  .py.# utility do
+00005360: 6573 2028 7468 6f75 6768 2069 7420 7461  es (though it ta
+00005370: 6b65 7320 6120 312d 6261 7365 6420 7369  kes a 1-based si
+00005380: 7465 292e 0a23 0a23 2048 6572 6520 6973  te)..#.# Here is
+00005390: 2074 6865 2041 6c70 6861 204e 3530 3159   the Alpha N501Y
+000053a0: 2063 6861 6e67 653a 0a3e 3e3e 2070 7028   change:.>>> pp(
+000053b0: 616c 6967 6e6d 656e 742e 6f66 6673 6574  alignment.offset
+000053c0: 496e 666f 2835 3030 2c20 7265 6c61 7469  Info(500, relati
+000053d0: 7665 546f 4665 6174 7572 653d 5472 7565  veToFeature=True
+000053e0: 2c20 6161 3d54 7275 652c 2066 6561 7475  , aa=True, featu
+000053f0: 7265 4e61 6d65 3d27 7327 2929 0a7b 2766  reName='s')).{'f
+00005400: 6561 7475 7265 4e61 6d65 273a 2027 7375  eatureName': 'su
+00005410: 7266 6163 6520 676c 7963 6f70 726f 7465  rface glycoprote
+00005420: 696e 272c 0a20 2766 6561 7475 7265 4e61  in',. 'featureNa
+00005430: 6d65 7327 3a20 7b27 7375 7266 6163 6520  mes': {'surface 
+00005440: 676c 7963 6f70 726f 7465 696e 277d 2c0a  glycoprotein'},.
+00005450: 2027 616c 6967 6e6d 656e 744f 6666 7365   'alignmentOffse
+00005460: 7427 3a20 3233 3036 322c 0a20 2772 6566  t': 23062,. 'ref
+00005470: 6572 656e 6365 273a 207b 2761 6127 3a20  erence': {'aa': 
+00005480: 274e 272c 0a20 2027 636f 646f 6e27 3a20  'N',.  'codon': 
+00005490: 2741 4154 272c 0a20 2027 6672 616d 6527  'AAT',.  'frame'
+000054a0: 3a20 302c 0a20 2027 6964 273a 2027 4e43  : 0,.  'id': 'NC
+000054b0: 5f30 3435 3531 322e 3227 2c0a 2020 2761  _045512.2',.  'a
+000054c0: 614f 6666 7365 7427 3a20 3530 302c 0a20  aOffset': 500,. 
+000054d0: 2027 6e74 4f66 6673 6574 273a 2032 3330   'ntOffset': 230
+000054e0: 3632 7d2c 0a20 2767 656e 6f6d 6527 3a20  62},. 'genome': 
+000054f0: 7b27 6161 273a 2027 5927 2c0a 2020 2763  {'aa': 'Y',.  'c
+00005500: 6f64 6f6e 273a 2027 5441 5427 2c0a 2020  odon': 'TAT',.  
+00005510: 2766 7261 6d65 273a 2030 2c0a 2020 2769  'frame': 0,.  'i
+00005520: 6427 3a20 2745 5049 5f49 534c 5f36 3031  d': 'EPI_ISL_601
+00005530: 3434 3320 6843 6f56 2d31 392f 456e 676c  443 hCoV-19/Engl
+00005540: 616e 642f 4d49 4c4b 2d39 4530 3542 332f  and/MILK-9E05B3/
+00005550: 3230 3230 272c 0a20 2027 6161 4f66 6673  2020',.  'aaOffs
+00005560: 6574 273a 2034 3937 2c0a 2020 276e 744f  et': 497,.  'ntO
+00005570: 6666 7365 7427 3a20 3232 3939 307d 7d0a  ffset': 22990}}.
+00005580: 6060 600a 0a59 6f75 2063 616e 2063 6865  ```..You can che
+00005590: 636b 2061 2066 6561 7475 7265 2066 6f72  ck a feature for
+000055a0: 2061 6e20 6578 7065 6374 6564 2063 6861   an expected cha
+000055b0: 6e67 653a 0a0a 6060 6020 7079 0a3e 3e3e  nge:..``` py.>>>
+000055c0: 2061 6c69 676e 6d65 6e74 2e63 6865 636b   alignment.check
+000055d0: 4665 6174 7572 6528 2773 7069 6b65 272c  Feature('spike',
+000055e0: 2027 4e35 3031 5927 2c20 6161 3d54 7275   'N501Y', aa=Tru
+000055f0: 6529 0a28 312c 2030 2c20 7b27 4e35 3031  e).(1, 0, {'N501
+00005600: 5927 3a20 2854 7275 652c 2027 4e27 2c20  Y': (True, 'N', 
+00005610: 5472 7565 2c20 2759 2729 7d29 0a60 6060  True, 'Y')}).```
+00005620: 0a0a 5468 6520 7265 7475 726e 2076 616c  ..The return val
+00005630: 7565 2067 6976 6573 2074 6865 206e 756d  ue gives the num
+00005640: 6265 7220 6f66 2074 6573 7473 2064 6f6e  ber of tests don
+00005650: 6520 2831 292c 2074 6865 206e 756d 6265  e (1), the numbe
+00005660: 7220 7468 6174 2066 6169 6c65 640a 2830  r that failed.(0
+00005670: 292c 2061 6e64 2061 2060 6469 6374 6020  ), and a `dict` 
+00005680: 7769 7468 2069 6e66 6f72 6d61 7469 6f6e  with information
+00005690: 2061 626f 7574 2065 6163 6820 7465 7374   about each test
+000056a0: 2e20 5468 6520 6064 6963 7460 2076 616c  . The `dict` val
+000056b0: 7565 7320 6172 650a 342d 7475 706c 6573  ues are.4-tuples
+000056c0: 2c20 696e 6469 6361 7469 6e67 2077 6865  , indicating whe
+000056d0: 7468 6572 2077 6861 7420 7761 7320 696e  ther what was in
+000056e0: 2074 6865 2072 6566 6572 656e 6365 2077   the reference w
+000056f0: 6173 2061 7320 6578 7065 6374 6564 0a28  as as expected.(
+00005700: 6054 7275 6560 292c 2074 6865 2076 616c  `True`), the val
+00005710: 7565 2069 6e20 7468 6520 7265 6665 7265  ue in the refere
+00005720: 6e63 6520 2860 4e60 292c 2077 6865 7468  nce (`N`), wheth
+00005730: 6572 2077 6861 7420 7761 7320 696e 2074  er what was in t
+00005740: 6865 2067 656e 6f6d 6520 7761 730a 6173  he genome was.as
+00005750: 2065 7870 6563 7465 6420 2860 5472 7565   expected (`True
+00005760: 6029 2c20 7468 6520 7661 6c75 6520 696e  `), the value in
+00005770: 2074 6865 2067 656e 6f6d 6520 2860 5960   the genome (`Y`
+00005780: 292e 0a0a 596f 7520 6361 6e20 7465 7374  )...You can test
+00005790: 206d 756c 7469 706c 6520 7468 696e 6773   multiple things
+000057a0: 3a0a 0a60 6060 2070 790a 2320 4e6f 7465  :..``` py.# Note
+000057b0: 2074 6861 7420 7765 2075 7365 2035 3031   that we use 501
+000057c0: 5920 696e 2074 6865 2066 6f6c 6c6f 7769  Y in the followi
+000057d0: 6e67 2c20 6e6f 7420 4e35 3031 592c 2073  ng, not N501Y, s
+000057e0: 696e 6365 2077 6520 6d69 6768 7420 6a75  ince we might ju
+000057f0: 7374 0a23 2077 616e 7420 746f 2063 6865  st.# want to che
+00005800: 636b 2074 6861 7420 736f 6d65 7468 696e  ck that somethin
+00005810: 6720 6973 2069 6e20 7468 6520 6765 6e6f  g is in the geno
+00005820: 6d65 2077 6974 686f 7574 206b 6e6f 7769  me without knowi
+00005830: 6e67 206f 7220 6361 7269 6e67 0a23 2061  ng or caring.# a
+00005840: 626f 7574 2077 6861 7427 7320 696e 2074  bout what's in t
+00005850: 6865 2072 6566 6572 656e 6365 2e0a 3e3e  he reference..>>
+00005860: 3e20 7070 2861 6c69 676e 6d65 6e74 2e63  > pp(alignment.c
+00005870: 6865 636b 4665 6174 7572 6528 2773 7069  heckFeature('spi
+00005880: 6b65 272c 2027 3530 3159 2036 392d 2037  ke', '501Y 69- 7
+00005890: 302d 272c 2061 613d 5472 7565 2929 0a28  0-', aa=True)).(
+000058a0: 332c 0a20 302c 0a20 7b27 3530 3159 273a  3,. 0,. {'501Y':
+000058b0: 2028 5472 7565 2c20 274e 272c 2054 7275   (True, 'N', Tru
+000058c0: 652c 2027 5927 292c 0a20 2027 3639 2d27  e, 'Y'),.  '69-'
+000058d0: 3a20 2854 7275 652c 2027 4827 2c20 5472  : (True, 'H', Tr
+000058e0: 7565 2c20 272d 2729 2c0a 2020 2737 302d  ue, '-'),.  '70-
+000058f0: 273a 2028 5472 7565 2c20 2756 272c 2054  ': (True, 'V', T
+00005900: 7275 652c 2027 2d27 297d 290a 6060 600a  rue, '-')}).```.
+00005910: 0a0a 5468 6572 6520 6973 2061 6c73 6f20  ..There is also 
+00005920: 6120 636f 6e76 656e 6965 6e63 6520 6043  a convenience `C
+00005930: 6865 636b 6572 6020 636c 6173 7320 7468  hecker` class th
+00005940: 6174 2063 616e 2063 6865 636b 2077 6865  at can check whe
+00005950: 7468 6572 206c 6f67 6963 616c 0a63 6f6d  ther logical.com
+00005960: 6269 6e61 7469 6f6e 7320 6f66 2061 6d69  binations of ami
+00005970: 6e6f 2061 6369 6420 616e 6420 6e75 636c  no acid and nucl
+00005980: 656f 7469 6465 2063 6861 6e67 6573 2061  eotide changes a
+00005990: 7265 2073 6174 6973 6669 6564 2066 6f72  re satisfied for
+000059a0: 2061 2067 656e 6f6d 652e 0a43 6f6e 7469   a genome..Conti
+000059b0: 6e75 696e 6720 6672 6f6d 2074 6865 2061  nuing from the a
+000059c0: 626f 7665 3a0a 0a60 6060 2070 790a 3e3e  bove:..``` py.>>
+000059d0: 3e20 6672 6f6d 2067 6232 7365 712e 6368  > from gb2seq.ch
+000059e0: 6563 6b65 7220 696d 706f 7274 2041 4143  ecker import AAC
+000059f0: 6865 636b 6572 2c20 4e54 4368 6563 6b65  hecker, NTChecke
+00005a00: 720a 0a23 204d 616b 6520 6120 426f 6f6c  r..# Make a Bool
+00005a10: 6561 6e20 6368 6563 6b65 7220 6675 6e63  ean checker func
+00005a20: 7469 6f6e 2074 6f20 7465 7374 2077 6865  tion to test whe
+00005a30: 7468 6572 2061 2067 656e 6f6d 6520 6861  ther a genome ha
+00005a40: 7320 7468 6520 4e35 3031 590a 2320 616e  s the N501Y.# an
+00005a50: 6420 4135 3730 4420 7370 696b 6520 6368  d A570D spike ch
+00005a60: 616e 6765 7320 7365 656e 2069 6e20 416c  anges seen in Al
+00005a70: 7068 612e 0a3e 3e3e 2063 6865 636b 6572  pha..>>> checker
+00005a80: 203d 2041 4143 6865 636b 6572 2827 7370   = AAChecker('sp
+00005a90: 696b 6527 2c20 274e 3530 3159 2729 2026  ike', 'N501Y') &
+00005aa0: 2041 4143 6865 636b 6572 2827 7370 696b   AAChecker('spik
+00005ab0: 6527 2c20 2741 3537 3044 2729 0a3e 3e3e  e', 'A570D').>>>
+00005ac0: 2063 6865 636b 6572 2861 6c69 676e 6d65   checker(alignme
+00005ad0: 6e74 290a 5472 7565 0a0a 2320 4368 6563  nt).True..# Chec
+00005ae0: 6b20 666f 7220 736f 6d65 206e 7563 6c65  k for some nucle
+00005af0: 6f74 6964 6520 6368 616e 6765 7320 696e  otide changes in
+00005b00: 2074 6865 206e 7563 6c65 6f63 6170 7369   the nucleocapsi
+00005b10: 6420 616e 6420 736f 6d65 2061 6d69 6e6f  d and some amino
+00005b20: 0a23 2061 6369 6420 6368 616e 6765 7320  .# acid changes 
+00005b30: 696e 2074 6865 2073 7069 6b65 2e0a 6368  in the spike..ch
+00005b40: 6563 6b65 7220 3d20 284e 5443 6865 636b  ecker = (NTCheck
+00005b50: 6572 2827 4e27 2c20 2747 3743 2041 3854  er('N', 'G7C A8T
+00005b60: 2054 3941 2047 3630 3841 2047 3630 3941   T9A G608A G609A
+00005b70: 2047 3631 3043 2043 3730 3454 2729 2026   G610C C704T') &
+00005b80: 0a20 2020 2020 2020 2020 2020 4141 4368  .           AACh
+00005b90: 6563 6b65 7228 2753 272c 2027 4e35 3031  ecker('S', 'N501
+00005ba0: 5920 4836 392d 2056 3730 2d20 5931 3434  Y H69- V70- Y144
+00005bb0: 2d27 2929 0a0a 2320 596f 7520 6361 6e20  -'))..# You can 
+00005bc0: 616c 736f 2075 7365 2060 7c60 2074 6f20  also use `|` to 
+00005bd0: 6368 6563 6b20 616e 204f 5220 636f 6e64  check an OR cond
+00005be0: 6974 696f 6e2e 0a3e 3e3e 2063 6865 636b  ition..>>> check
+00005bf0: 6572 203d 2041 4143 6865 636b 6572 2827  er = AAChecker('
+00005c00: 7370 696b 6527 2c20 2745 3438 344b 2729  spike', 'E484K')
+00005c10: 207c 2041 4143 6865 636b 6572 2827 7370   | AAChecker('sp
+00005c20: 696b 6527 2c20 2745 3438 3451 2729 0a3e  ike', 'E484Q').>
+00005c30: 3e3e 2063 6865 636b 6572 2861 6c69 676e  >> checker(align
+00005c40: 6d65 6e74 290a 4661 6c73 650a 6060 600a  ment).False.```.
+00005c50: 0a4e 6f74 6520 7468 6174 2062 6563 6175  .Note that becau
+00005c60: 7365 2074 6865 2060 4368 6563 6b65 7260  se the `Checker`
+00005c70: 2063 6c61 7373 2074 616b 6573 2061 2073   class takes a s
+00005c80: 7472 696e 6720 6172 6775 6d65 6e74 2074  tring argument t
+00005c90: 6861 7420 6c69 6b65 6c79 0a6f 7269 6769  hat likely.origi
+00005ca0: 6e61 7465 7320 6672 6f6d 2061 2068 756d  nates from a hum
+00005cb0: 616e 2d72 6561 6461 626c 6520 736f 7572  an-readable sour
+00005cc0: 6365 2c20 652e 672e 2c20 224e 3530 3159  ce, e.g., "N501Y
+00005cd0: 222c 2074 6865 2063 6861 6e67 6573 0a73  ", the changes.s
+00005ce0: 7065 6369 6669 6564 2066 6f72 2074 6865  pecified for the
+00005cf0: 2063 6865 636b 6572 2061 7265 2069 6e20   checker are in 
+00005d00: 7465 726d 7320 6f66 2031 2d62 6173 6564  terms of 1-based
+00005d10: 2073 6974 6573 2e0a 0a53 696d 696c 6961   sites...Similia
+00005d20: 7220 746f 2074 6865 2060 2d2d 6368 6563  r to the `--chec
+00005d30: 6b56 6172 6961 6e74 6020 6172 6775 6d65  kVariant` argume
+00005d40: 6e74 2074 6f20 6064 6573 6372 6962 652d  nt to `describe-
+00005d50: 6765 6e6f 6d65 2e70 7960 2028 6162 6f76  genome.py` (abov
+00005d60: 6529 2c0a 796f 7520 6361 6e20 616c 736f  e),.you can also
+00005d70: 2063 6865 636b 2061 2070 7265 2d64 6566   check a pre-def
+00005d80: 696e 6564 2076 6172 6961 6e74 3a0a 0a60  ined variant:..`
+00005d90: 6060 7079 0a3e 3e3e 2070 7028 616c 6967  ``py.>>> pp(alig
+00005da0: 6e6d 656e 742e 6368 6563 6b56 6172 6961  nment.checkVaria
+00005db0: 6e74 2827 564f 435f 3230 3230 3132 3031  nt('VOC_20201201
+00005dc0: 5f55 4b27 2929 0a28 3230 2c0a 2030 2c0a  _UK')).(20,. 0,.
+00005dd0: 207b 276e 273a 207b 2761 6127 3a20 7b27   {'n': {'aa': {'
+00005de0: 3233 3546 273a 2028 5472 7565 2c20 2753  235F': (True, 'S
+00005df0: 272c 2054 7275 652c 2027 4627 292c 2027  ', True, 'F'), '
+00005e00: 334c 273a 2028 5472 7565 2c20 2744 272c  3L': (True, 'D',
+00005e10: 2054 7275 652c 2027 4c27 297d 7d2c 0a20   True, 'L')}},. 
+00005e20: 2027 6f72 6631 6162 273a 207b 2761 6127   'orf1ab': {'aa'
+00005e30: 3a20 7b27 3130 3031 4927 3a20 2854 7275  : {'1001I': (Tru
+00005e40: 652c 2027 5427 2c20 5472 7565 2c20 2749  e, 'T', True, 'I
+00005e50: 2729 2c0a 2020 2020 2020 2020 2020 2020  '),.            
+00005e60: 2020 2020 2020 2020 2731 3730 3844 273a          '1708D':
+00005e70: 2028 5472 7565 2c20 2741 272c 2054 7275   (True, 'A', Tru
+00005e80: 652c 2027 4427 292c 0a20 2020 2020 2020  e, 'D'),.       
+00005e90: 2020 2020 2020 2020 2020 2020 2027 3232               '22
+00005ea0: 3330 5427 3a20 2854 7275 652c 2027 4927  30T': (True, 'I'
+00005eb0: 2c20 5472 7565 2c20 2754 2729 2c0a 2020  , True, 'T'),.  
+00005ec0: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005ed0: 2020 2733 3637 352d 273a 2028 5472 7565    '3675-': (True
+00005ee0: 2c20 2753 272c 2054 7275 652c 2027 2d27  , 'S', True, '-'
+00005ef0: 292c 0a20 2020 2020 2020 2020 2020 2020  ),.             
+00005f00: 2020 2020 2020 2027 3336 3736 2d27 3a20         '3676-': 
+00005f10: 2854 7275 652c 2027 4727 2c20 5472 7565  (True, 'G', True
+00005f20: 2c20 272d 2729 2c0a 2020 2020 2020 2020  , '-'),.        
+00005f30: 2020 2020 2020 2020 2020 2020 2733 3637              '367
+00005f40: 372d 273a 2028 5472 7565 2c20 2746 272c  7-': (True, 'F',
+00005f50: 2054 7275 652c 2027 2d27 297d 7d2c 0a20   True, '-')}},. 
+00005f60: 2027 6f72 6638 273a 207b 2761 6127 3a20   'orf8': {'aa': 
+00005f70: 7b27 3532 4927 3a20 2854 7275 652c 2027  {'52I': (True, '
+00005f80: 5227 2c20 5472 7565 2c20 2749 2729 2c0a  R', True, 'I'),.
+00005f90: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00005fa0: 2020 2737 3343 273a 2028 5472 7565 2c20    '73C': (True, 
+00005fb0: 2759 272c 2054 7275 652c 2027 4327 292c  'Y', True, 'C'),
+00005fc0: 0a20 2020 2020 2020 2020 2020 2020 2020  .               
+00005fd0: 2020 2027 5132 372a 273a 2028 5472 7565     'Q27*': (True
+00005fe0: 2c20 2751 272c 2054 7275 652c 2027 2a27  , 'Q', True, '*'
+00005ff0: 297d 7d2c 0a20 2027 7370 696b 6527 3a20  )}},.  'spike': 
+00006000: 7b27 6161 273a 207b 2731 3131 3848 273a  {'aa': {'1118H':
+00006010: 2028 5472 7565 2c20 2744 272c 2054 7275   (True, 'D', Tru
+00006020: 652c 2027 4827 292c 0a20 2020 2020 2020  e, 'H'),.       
+00006030: 2020 2020 2020 2020 2020 2020 2731 3434              '144
+00006040: 2d27 3a20 2854 7275 652c 2027 5927 2c20  -': (True, 'Y', 
+00006050: 5472 7565 2c20 272d 2729 2c0a 2020 2020  True, '-'),.    
+00006060: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+00006070: 3530 3159 273a 2028 5472 7565 2c20 274e  501Y': (True, 'N
+00006080: 272c 2054 7275 652c 2027 5927 292c 0a20  ', True, 'Y'),. 
+00006090: 2020 2020 2020 2020 2020 2020 2020 2020                  
+000060a0: 2020 2735 3730 4427 3a20 2854 7275 652c    '570D': (True,
+000060b0: 2027 4127 2c20 5472 7565 2c20 2744 2729   'A', True, 'D')
+000060c0: 2c0a 2020 2020 2020 2020 2020 2020 2020  ,.              
+000060d0: 2020 2020 2027 3638 3148 273a 2028 5472       '681H': (Tr
+000060e0: 7565 2c20 2750 272c 2054 7275 652c 2027  ue, 'P', True, '
+000060f0: 4827 292c 0a20 2020 2020 2020 2020 2020  H'),.           
+00006100: 2020 2020 2020 2020 2736 392d 273a 2028          '69-': (
+00006110: 5472 7565 2c20 2748 272c 2054 7275 652c  True, 'H', True,
+00006120: 2027 2d27 292c 0a20 2020 2020 2020 2020   '-'),.         
+00006130: 2020 2020 2020 2020 2020 2737 302d 273a            '70-':
+00006140: 2028 5472 7565 2c20 2756 272c 2054 7275   (True, 'V', Tru
+00006150: 652c 2027 2d27 292c 0a20 2020 2020 2020  e, '-'),.       
+00006160: 2020 2020 2020 2020 2020 2020 2737 3136              '716
+00006170: 4927 3a20 2854 7275 652c 2027 5427 2c20  I': (True, 'T', 
+00006180: 5472 7565 2c20 2749 2729 2c0a 2020 2020  True, 'I'),.    
+00006190: 2020 2020 2020 2020 2020 2020 2020 2027                 '
+000061a0: 3938 3241 273a 2028 5472 7565 2c20 2753  982A': (True, 'S
+000061b0: 272c 2054 7275 652c 2027 4127 297d 7d7d  ', True, 'A')}}}
+000061c0: 290a 6060 600a 0a77 6974 6820 7468 6520  ).```..with the 
+000061d0: 7265 7375 6c74 7320 7375 6d6d 6172 697a  results summariz
+000061e0: 696e 6720 7468 6520 6e75 6d62 6572 206f  ing the number o
+000061f0: 6620 7465 7374 7320 646f 6e65 2c20 7468  f tests done, th
+00006200: 6520 6e75 6d62 6572 2074 6861 740a 6661  e number that.fa
+00006210: 696c 6564 2c20 616e 6420 7468 656e 2074  iled, and then t
+00006220: 6865 2066 6561 7475 7265 7320 6368 6563  he features chec
+00006230: 6b65 642c 2077 6974 6820 6061 6160 2061  ked, with `aa` a
+00006240: 6e64 2060 6e74 6020 6469 6374 696f 6e61  nd `nt` dictiona
+00006250: 7269 6573 2066 6f72 0a74 6865 2061 6d69  ries for.the ami
+00006260: 6e6f 2061 6369 6420 616e 6420 6e75 636c  no acid and nucl
+00006270: 656f 7469 6465 2063 6865 636b 732e 0a0a  eotide checks...
+00006280: 596f 7520 6361 6e20 7061 7373 2079 6f75  You can pass you
+00006290: 7220 6f77 6e20 7661 7269 616e 7420 6469  r own variant di
+000062a0: 6374 696f 6e61 7279 2073 7065 6369 6679  ctionary specify
+000062b0: 696e 6720 7768 6174 2079 6f75 2077 616e  ing what you wan
+000062c0: 7420 6368 6563 6b65 642e 0a0a 2323 2054  t checked...## T
+000062d0: 6f20 6c65 6172 6e20 6d6f 7265 0a0a 5365  o learn more..Se
+000062e0: 6520 7468 6520 6046 6561 7475 7265 7360  e the `Features`
+000062f0: 2061 6e64 2060 4762 3241 6c69 676e 6d65   and `Gb2Alignme
+00006300: 6e74 6020 636c 6173 7365 7320 696e 0a5b  nt` classes in.[
+00006310: 6762 3273 6571 2f66 6561 7475 7265 2e70  gb2seq/feature.p
+00006320: 795d 2867 6232 7365 712f 6665 6174 7572  y](gb2seq/featur
+00006330: 652e 7079 2920 616e 640a 5b67 6232 7365  e.py) and.[gb2se
+00006340: 712f 616c 6967 6e6d 656e 742e 7079 5d28  q/alignment.py](
+00006350: 6762 3273 6571 2f61 6c69 676e 6d65 6e74  gb2seq/alignment
+00006360: 2e70 7929 2e20 416c 736f 2c20 7468 6520  .py). Also, the 
+00006370: 7465 7374 7320 2865 2e67 2e2c 2069 6e0a  tests (e.g., in.
+00006380: 5b74 6573 742f 7465 7374 5f66 6561 7475  [test/test_featu
+00006390: 7265 2e70 795d 2874 6573 742f 7465 7374  re.py](test/test
+000063a0: 5f66 6561 7475 7265 2e70 7929 2c0a 5b74  _feature.py),.[t
+000063b0: 6573 742f 7465 7374 5f61 6c69 676e 6d65  est/test_alignme
+000063c0: 6e74 2e70 795d 2874 6573 742f 7465 7374  nt.py](test/test
+000063d0: 5f61 6c69 676e 6d65 6e74 2e70 7929 2c0a  _alignment.py),.
+000063e0: 5b74 6573 742f 7465 7374 5f63 6865 636b  [test/test_check
+000063f0: 6572 2e70 795d 2874 6573 742f 7465 7374  er.py](test/test
+00006400: 5f63 6865 636b 6572 2e70 7929 0a5b 7465  _checker.py).[te
+00006410: 7374 2f74 6573 745f 7661 7269 616e 7473  st/test_variants
+00006420: 2e70 795d 2874 6573 742f 7465 7374 5f76  .py](test/test_v
+00006430: 6172 6961 6e74 732e 7079 2929 2073 686f  ariants.py)) sho
+00006440: 7720 796f 7520 6578 616d 706c 6520 7573  w you example us
+00006450: 6573 206f 660a 7468 6573 6520 636c 6173  es of.these clas
+00006460: 7365 7320 616e 6420 7468 6569 7220 6d65  ses and their me
+00006470: 7468 6f64 732e 2020 596f 7520 6361 6e20  thods.  You can 
+00006480: 616c 736f 206c 6f6f 6b20 746f 2073 6565  also look to see
+00006490: 2068 6f77 2074 6865 2074 6872 6565 0a75   how the three.u
+000064a0: 7469 6c69 7479 2073 6372 6970 7473 2064  tility scripts d
+000064b0: 6573 6372 6962 6564 2061 626f 7665 2028  escribed above (
+000064c0: 7768 6963 6820 6361 6e20 616c 6c20 6265  which can all be
+000064d0: 2066 6f75 6e64 2069 6e20 7468 6520 5b62   found in the [b
+000064e0: 696e 0a64 6972 6563 746f 7279 5d28 6269  in.directory](bi
+000064f0: 6e29 2920 6361 6c6c 2074 6865 206c 6962  n)) call the lib
+00006500: 7261 7279 2066 756e 6374 696f 6e73 2061  rary functions a
+00006510: 6e64 2075 7365 2074 6865 2072 6573 756c  nd use the resul
+00006520: 7473 2e0a 0a23 2044 6576 656c 6f70 696e  ts...# Developin
+00006530: 670a 0a52 756e 2074 6865 2074 6573 7473  g..Run the tests
+00006540: 2076 6961 200a 0a60 6060 7368 0a24 2070   via ..```sh.$ p
+00006550: 7974 6573 740a 6060 600a 0a0a 2323 204e  ytest.```...## N
+00006560: 6f74 6573 0a0a 2a20 5468 6520 7465 7374  otes..* The test
+00006570: 7320 7769 6c6c 2072 756e 205b 4d41 4646  s will run [MAFF
+00006580: 545d 2868 7474 7073 3a2f 2f6d 6166 6674  T](https://mafft
+00006590: 2e63 6272 632e 6a70 2f61 6c69 676e 6d65  .cbrc.jp/alignme
+000065a0: 6e74 2f73 6f66 7477 6172 652f 292c 2073  nt/software/), s
+000065b0: 6f0a 2020 2020 796f 7520 6e65 6564 2074  o.    you need t
+000065c0: 6861 7420 696e 7374 616c 6c65 6420 616e  hat installed an
+000065d0: 6420 696e 2079 6f75 7220 7368 656c 6c27  d in your shell'
+000065e0: 7320 6050 4154 4860 2e0a 2a20 5468 6520  s `PATH`..* The 
+000065f0: 7465 7374 7320 7275 6e20 736c 6f77 6c79  tests run slowly
+00006600: 2028 3138 2073 6563 6f6e 6473 206f 6e20   (18 seconds on 
+00006610: 6d79 206c 6170 746f 7029 2064 7565 2074  my laptop) due t
+00006620: 6f20 7468 6520 6465 6661 756c 7420 7573  o the default us
+00006630: 6520 6f66 0a20 204d 4146 4654 2e0a 2a20  e of.  MAFFT..* 
+00006640: 5468 6520 7465 7374 7320 646f 206e 6f74  The tests do not
+00006650: 2061 6c6c 2070 6173 7320 6966 2079 6f75   all pass if you
+00006660: 2073 6574 2060 4445 4641 554c 545f 414c   set `DEFAULT_AL
+00006670: 4947 4e45 5260 2074 6f20 6265 2022 6564  IGNER` to be "ed
+00006680: 6c69 6222 2069 6e0a 2020 2020 6067 6232  lib" in.    `gb2
+00006690: 7365 712f 616c 6967 6e6d 656e 742e 7079  seq/alignment.py
+000066a0: 602e 2054 6869 7320 6973 2062 6563 6175  `. This is becau
+000066b0: 7365 2060 4d41 4646 5460 2061 6e64 2060  se `MAFFT` and `
+000066c0: 6564 6c69 6260 2070 726f 6475 6365 0a20  edlib` produce. 
+000066d0: 2020 2073 6c69 6768 746c 7920 6469 6666     slightly diff
+000066e0: 6572 656e 7420 7265 7375 6c74 7320 616e  erent results an
+000066f0: 6420 736f 6d65 2074 6573 7473 206f 6620  d some tests of 
+00006700: 7468 6520 5341 5253 2d43 6f56 2d32 2073  the SARS-CoV-2 s
+00006710: 7069 6b65 0a20 2020 2074 7261 6e73 6c61  pike.    transla
+00006720: 7469 6f6e 2074 6573 7473 2066 6169 6c20  tion tests fail 
+00006730: 6173 2061 2072 6573 756c 742e 2049 2077  as a result. I w
+00006740: 6f75 6c64 206c 696b 6520 746f 2070 6f73  ould like to pos
+00006750: 742d 7072 6f63 6573 7320 7468 650a 2020  t-process the.  
+00006760: 2020 6065 646c 6962 6020 6f75 7470 7574    `edlib` output
+00006770: 2074 6f20 6d61 7463 6820 7468 6174 206f   to match that o
+00006780: 6620 604d 4146 4654 6020 2874 6869 7320  f `MAFFT` (this 
+00006790: 6973 2069 6e20 6361 7365 7320 7768 6572  is in cases wher
+000067a0: 6520 7468 6572 650a 2020 2020 6172 6520  e there.    are 
+000067b0: 6d75 6c74 6970 6c65 2065 7175 616c 6c79  multiple equally
+000067c0: 2d67 6f6f 6420 616c 6967 6e6d 656e 7473  -good alignments
+000067d0: 292e 0a                                  )..
```

### Comparing `gb2seq-0.2.4/bin/annotate-genome.py` & `gb2seq-0.2.5/bin/annotate-genome.py`

 * *Files identical despite different names*

### Comparing `gb2seq-0.2.4/bin/describe-feature.py` & `gb2seq-0.2.5/bin/describe-feature.py`

 * *Files 4% similar despite different names*

```diff
@@ -55,47 +55,46 @@
                 akas = ""
 
             print(f"{featureName}:{akas}")
     else:
         print("\n".join(featureNames))
 
 
-def reportGenomeFeature(features, name, alignment, maxSequenceLength):
+def reportGenomeFeature(features, name, alignment, maxSequenceLength, oneBased):
     """
     Print details of a feature in a passed genome.
 
     @param features: A C{Features} instance.
     @param name: A C{str} feature name.
     @param alignment: A C{Gb2seq} instance with the aligned genome whose feature
         should be reported.
     @param maxSequenceLength: The maximum sequence length to print. Longer sequences
-        will "be truncated. Use 0 or C{None} to skip printing sequences.
+        will be truncated. Use 0 or C{None} to skip printing sequences.
+    @param oneBased: If true, print one-based sites instead of zero-based offsets.
 
     """
     print(f"  Genome {alignment.genome.id}:")
     feature = features[name]
-    alignedStart = alignment.gappedOffsets[feature["start"]]
     try:
+        alignedStart = alignment.gappedOffsets[feature["start"]]
         alignedStop = alignment.gappedOffsets[feature["stop"]]
     except KeyError:
         print(
-            f"Offset {feature['stop']} not found in gappedOffsets (len {len(alignment.gappedOffsets)})."
+            f"Offset {feature['stop']} not found in gappedOffsets "
+            f"(len {len(alignment.gappedOffsets)})."
         )
         sys.exit(1)
-    sequence = alignment.genomeAligned.sequence[alignedStart:alignedStop].replace(
-        "-", ""
-    )
-    absoluteStart = len(
-        alignment.genomeAligned.sequence[:alignedStart].replace("-", "")
-    )
-    absoluteStop = len(alignment.genomeAligned.sequence[:alignedStop].replace("-", ""))
 
+    gappedSequence = alignment.genomeAligned.sequence
+    sequence = gappedSequence[alignedStart:alignedStop].replace("-", "")
+    absoluteStart = len(gappedSequence[:alignedStart].replace("-", ""))
+    absoluteStop = len(gappedSequence[:alignedStop].replace("-", ""))
     _, genomeNt = alignment.ntSequences(name, raiseOnReferenceGaps=False)
 
-    print(f"    start: {absoluteStart}")
+    print(f"    start: {absoluteStart + bool(oneBased)}")
     print(f"    stop: {absoluteStop}")
     print(f"    length (nt): {len(genomeNt.sequence)}")
 
     if maxSequenceLength:
         print(
             "    sequence: " + (genomeNt.sequence[:maxSequenceLength] + "...")
             if maxSequenceLength > 0 and len(sequence) > maxSequenceLength
@@ -159,15 +158,16 @@
         if args.genome:
             fp.close()
     else:
         alignments = []
 
     if args.sortBy == "name":
         wantedNames.sort()
-    elif args.sortBy == "site":
+    else:
+        assert args.sortBy == "site"
 
         def key(name):
             return features[name]["start"]
 
         wantedNames.sort(key=key)
 
     for name in wantedNames:
@@ -178,27 +178,29 @@
                 maxSequenceLength=args.maxLen,
                 oneBased=args.oneBased,
                 prefix="  ",
             )
         )
 
         for alignment in alignments:
-            reportGenomeFeature(features, name, alignment, args.maxLen)
+            reportGenomeFeature(features, name, alignment, args.maxLen, args.oneBased)
 
 
 if __name__ == "__main__":
-
     parser = argparse.ArgumentParser(
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
-        description="Describe a reference genome feature.",
+        description=(
+            "Describe a genome feature in the reference and "
+            "(optionally) an unannotated genome."
+        ),
     )
 
     parser.add_argument(
         "--genome",
-        metavar="file.fasta",
+        metavar="genome.fasta",
         help="The FASTA file containing the genome to examine for features.",
     )
 
     parser.add_argument(
         "--name",
         metavar="NAME",
         action="append",
@@ -223,21 +225,22 @@
         action="store_true",
         help="Only print feature names and aliases (if any).",
     )
 
     parser.add_argument(
         "--zeroBased",
         dest="oneBased",
-        action="store_true",
+        action="store_false",
         help="Print zero-based offsets instead of one-based sites.",
     )
 
     parser.add_argument(
         "--sortBy",
         choices=("name", "site"),
+        default="name",
         help=(
             "The order in which to print features (default is the order given "
             "on the command line)."
         ),
     )
 
     addAlignerOption(parser)
```

### Comparing `gb2seq-0.2.4/bin/describe-genome.py` & `gb2seq-0.2.5/bin/describe-genome.py`

 * *Files 1% similar despite different names*

```diff
@@ -322,15 +322,14 @@
     if args.minReferenceCoverage is not None:
         print(f"Ignored {ignoredDueToCoverageCount} genomes due to low " f"coverage.")
 
     return 0
 
 
 if __name__ == "__main__":
-
     parser = argparse.ArgumentParser(
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
         description="Describe a genome (or genomes).",
     )
 
     parser.add_argument(
         "--genome",
```

### Comparing `gb2seq-0.2.4/bin/describe-site.py` & `gb2seq-0.2.5/bin/describe-site.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,15 +40,22 @@
         what = args.featureName or "genome"
         print(f"Insufficient {what} coverage", file=sys.stderr)
         return
 
     if args.genomeAaOnly:
         print(offsetInfo["genome"]["aa"])
     else:
-        if not includeGenome:
+        offsetInc = int(bool(args.oneBased))
+
+        offsetInfo["alignmentOffset"] += offsetInc
+        offsetInfo["reference"]["ntOffset"] += offsetInc
+
+        if includeGenome:
+            offsetInfo["genome"]["ntOffset"] += offsetInc
+        else:
             del offsetInfo["genome"]
 
         if args.includeFeature:
             featureName = offsetInfo["featureName"]
             if featureName:
                 assert "feature" not in offsetInfo
                 offsetInfo["feature"] = genome.features[featureName]
@@ -74,20 +81,20 @@
     @return: An C{int} exit status.
     """
     features = Features(
         args.reference,
         sars2=args.sars2,
         addUnannotatedRegions=args.addUnannotatedRegions,
     )
-    count = 0
 
     if args.genome is None and os.isatty(0):
         alignment = Gb2Alignment(features.reference, features, aligner=args.aligner)
         report(alignment, args, False)
     else:
+        count = 0
         fp = open(args.genome) if args.genome else sys.stdin
         for count, read in enumerate(FastaReads(fp), start=1):
             alignment = Gb2Alignment(read, features, aligner=args.aligner)
             report(alignment, args)
 
         if args.verbose:
             print(f"Examined {count} genomes.", file=sys.stderr)
@@ -95,15 +102,14 @@
         if args.genome:
             fp.close()
 
     return 0
 
 
 if __name__ == "__main__":
-
     parser = argparse.ArgumentParser(
         formatter_class=argparse.ArgumentDefaultsHelpFormatter,
         description="Describe a site of a genome(s).",
     )
 
     parser.add_argument(
         "--genome",
@@ -181,13 +187,20 @@
             "the denominator used to compute the coverage fraction is the "
             "length of the reference. I.e., coverage is computed as number "
             "of non-N bases in the genome divided by the length of the "
             "reference."
         ),
     )
 
+    parser.add_argument(
+        "--zeroBased",
+        dest="oneBased",
+        action="store_false",
+        help="Print zero-based offsets instead of one-based sites.",
+    )
+
     addFeatureOptions(parser)
     addAlignerOption(parser)
 
     args = parser.parse_args()
 
     sys.exit(main(args))
```

### Comparing `gb2seq-0.2.4/gb2seq/alignment.py` & `gb2seq-0.2.5/gb2seq/alignment.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,20 +53,20 @@
     """
     Make a dictionary mapping offsets in a sequence with no gaps to the
     equivalent offset in a gapped sequence.
 
     In more detail, we are given C{s}, which is an aligned sequence
     (potentially) with gaps in it and we want a mapping that will allow us to
     go from an offset in the original string C{s} (i.e., before it was aligned)
-    to the equivalent offset in the aligned (with gaps) string. This function
-    returns such a mapping (a C{dict})
+    to the equivalent offset in the aligned (with gaps) string that we have been
+    passed. This function returns such a mapping (a C{dict})
 
     @param s: A C{str} sequence, possibly with gap ('-') characters.
-    @return: A C{dict} mapping C{int} offsets (in the sequence without its
-        gaps) to equivalent C{int} offsets in C{s}, when gaps are ignored.
+    @return: A C{dict} mapping C{int} offsets in the sequence without its
+        gaps to equivalent C{int} offsets in C{s}, when gaps are ignored.
 
     """
     result = {}
     gapCount = index = 0
 
     # To build the mapping, we walk through s. If we see a gap we just
     # count it. Non-gap offsets go into the map with their offset plus the
@@ -447,15 +447,14 @@
                 # "aligned" genome that is all gaps. This matches what
                 # ntSequences will return.
                 referenceAaAligned = referenceAa
                 genomeAaAligned = AARead(
                     self.features.reference.id + idSuffix, "-" * len(referenceAaAligned)
                 )
             else:
-
                 genomeAa = AARead(
                     self.genome.id + idSuffix,
                     translate(
                         genomeNtNoGaps.sequence,
                         name,
                         sars2=self.features.sars2,
                         untranslatable=self._untranslatable,
@@ -624,17 +623,15 @@
                     referenceBase, offset, genomeBase = splitChange(change)
                     yield change, referenceBase, offset, genomeBase
             else:
                 for change in changes:
                     referenceBase, offset, genomeBase = change
                     yield change, referenceBase, offset, genomeBase
 
-        result: Dict[
-            Union[str, Tuple[Optional[str], int, Optional[str]]],
-        ] = {}
+        result: Dict[Union[str, Tuple[Optional[str], int, Optional[str]]],] = {}
         testCount = errorCount = 0
 
         try:
             reference, genome = (
                 self.aaSequences(featureName, raiseOnReferenceGaps=raiseOnReferenceGaps)
                 if aa
                 else self.ntSequences(featureName)
@@ -819,14 +816,20 @@
             if aa:
                 raise ValueError(
                     "You cannot pass aa=True unless the offset "
                     "you pass is relative to the feature."
                 )
             referenceOffset = offset
 
+        if referenceOffset >= len(self.features.reference):
+            raise IndexError(
+                f"Request for offset {referenceOffset} in a reference "
+                f"genome of length {len(self.features.reference)}."
+            )
+
         feature, features = self.features.getFeature(
             referenceOffset, featureName, includeUntranslated, allowAmbiguous
         )
 
         # The 'None' values in the following are filled in below. They're set
         # up-front here to explicitly show what's in the returned dictionary.
         #
```

### Comparing `gb2seq-0.2.4/gb2seq/annotate.py` & `gb2seq-0.2.5/gb2seq/annotate.py`

 * *Files identical despite different names*

### Comparing `gb2seq-0.2.4/gb2seq/change.py` & `gb2seq-0.2.5/gb2seq/change.py`

 * *Files identical despite different names*

### Comparing `gb2seq-0.2.4/gb2seq/checker.py` & `gb2seq-0.2.5/gb2seq/checker.py`

 * *Files identical despite different names*

### Comparing `gb2seq-0.2.4/gb2seq/features.py` & `gb2seq-0.2.5/gb2seq/features.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,15 +78,16 @@
                 self.WUHAN_REF
                 if referenceSpecification is None
                 else referenceSpecification
             )
         else:
             if referenceSpecification is None:
                 raise ValueError(
-                    "A reference specification must be provided for non-SARS-CoV-2 features."
+                    "A reference specification must be provided for non-SARS-CoV-2 "
+                    "features."
                 )
 
         if isinstance(referenceSpecification, SeqRecord):
             record = referenceSpecification
             self._initializeFromGenBankRecord(record)
         elif isinstance(referenceSpecification, str):
             if reference is not None:
@@ -114,16 +115,16 @@
                         except Exception as e:
                             seqError = e
                         else:
                             self._initializeFromGenBankRecord(record)
 
                 if jsonError and seqError:
                     print(
-                        f"Could not read {referenceSpecification!r} as a JSON or GenBank file. "
-                        f"Here are the parsing errors.\nJSON: "
+                        f"Could not read {referenceSpecification!r} as a JSON or "
+                        f"GenBank file. Here are the parsing errors.\nJSON: "
                         f"{jsonError}\nGenBank: {seqError}",
                         file=sys.stderr,
                     )
                     sys.exit(1)
             else:
                 print(
                     f"Fetching GenBank record for {referenceSpecification!r}.",
@@ -519,35 +520,35 @@
         @param featureName: A C{str} feature name. Used for disambiguation when
             multiple features are present at the offset. If C{None}, a feature
             will be returned if there is only one at the given offset.
         @param includeUntranslated: If C{True}, also consider features that are
             not translated.
         @allowAmbiguous: If C{True}, do not raise an error if multiple features
             are found for the offset and no feature name is given to
-            disambiguate. Instead, use the first feature name returned by
-            C{getFeatureNames}.
+            disambiguate. Instead, use the alphabetically first feature name
+            returned by C{getFeatureNames}.
         @raise MissingFeatureError: if the requested feature does not overlap
             the given C{offset} or if there are no features at the offset.
         @raise AmbiguousFeatureError: if there are multiple features at the
             offset and a feature name is not given.
         @return: A 2-tuple, containing 1) a features C{dict} (as returned by
             __getitem__), if the requested feature is among those present at
             the offset, and 2) the set of all C{str} feature names present at
             the offset.
         """
         features = self.getFeatureNames(offset, includeUntranslated)
 
         if featureName is None:
             if features:
-                # There are some features here, but we weren't told which one
-                # to use. Only proceed if there's just one or if we've been
-                # told to allow ambiguity (in which case we use the first
-                # feature name).
+                # There are some features here, but we weren't told which
+                # one to use. Only proceed if there's just one or if we've
+                # been told to allow ambiguity (in which case we use the
+                # alphabetically first feature name).
                 if len(features) == 1 or allowAmbiguous:
-                    featureName = list(features)[0]
+                    featureName = list(sorted(features))[0]
                     feature = self[featureName]
                 else:
                     present = ", ".join(
                         f"{f!r} ({self[f]['start'] + 1} - {self[f]['stop']})"
                         for f in sorted(features)
                     )
                     raise AmbiguousFeatureError(
@@ -601,79 +602,82 @@
             1-based instead of 0-based.
         @param prefix: A C{str} to put at the start of each line.
         @return: A C{str}.
         """
         canonicalName = self.canonicalName(name)
         feature = self[canonicalName]
         sequence = feature["sequence"]
+        start = feature["start"]
+        stop = feature["stop"]
         result = [
-            f"{prefix}{name}:",
-            f"{prefix}  start: {feature['start'] + bool(oneBased)}",
-            f"{prefix}  stop: {feature['stop']}",
-            f"{prefix}  length (nt): {feature['stop'] - feature['start']}",
+            f"{name}:",
+            f"  start: {start + bool(oneBased)}",
+            f"  stop: {feature['stop']}",
+            f"  length (nt): {stop - start}",
         ]
 
         for name in "product", "note", "function":
             try:
-                result.append(f"{prefix}  {name}: {feature[name]}")
+                result.append(f"  {name}: {feature[name]}")
             except KeyError:
                 pass
 
         if "translation" in feature:
             if "forward" in feature:
                 if feature["forward"]:
-                    result.append(f"{prefix}  feature is translated left-to-right.")
+                    result.append("  feature is translated left-to-right.")
                 else:
                     result.append(
-                        f"{prefix}  feature is translated right-to-left from the "
-                        f"reverse complement."
+                        "  feature is translated right-to-left from the "
+                        "reverse complement."
                     )
                     rc = DNARead("id", sequence).reverseComplement().sequence
                     result.append(
-                        f"{prefix}  reverse complement: "
+                        "  reverse complement: "
                         + (
                             (rc[:maxSequenceLength] + "...")
                             if maxSequenceLength > 0 and len(rc) > maxSequenceLength
                             else rc
                         )
                     )
 
         if maxSequenceLength:
             result.append(
-                f"{prefix}  sequence: "
+                "  sequence: "
                 + (
                     (sequence[:maxSequenceLength] + "...")
                     if maxSequenceLength > 0 and len(sequence) > maxSequenceLength
                     else sequence
                 )
             )
 
             try:
                 translation = feature["translation"]
 
                 result.extend(
                     [
-                        f"{prefix}  length (aa): {len(translation)}",
-                        f"{prefix}  translation: "
+                        f"  length (aa): {len(translation)}",
+                        "  translation: "
                         + (
                             (translation[:maxSequenceLength] + "...")
                             if maxSequenceLength > 0
                             and len(translation) > maxSequenceLength
                             else translation
                         ),
                     ]
                 )
             except KeyError:
-                result.append(f"{prefix}  region is not translated.")
+                result.append("  region is not translated.")
 
-        return "\n".join(result)
+        return "\n".join(prefix + s for s in result)
 
 
-def addFeatureOptions(parser: argparse.ArgumentParser,
-                      referenceHelpInfo: str = "") -> None:
+def addFeatureOptions(
+    parser: argparse.ArgumentParser, referenceHelpInfo: str = ""
+) -> None:
     """
     Add standard command-line options that can then be passed to the Feature
     constructor.
 
     @param parser: An argparse parser to add options to.
     @param referenceHelpInfo: A C{str} to append to the usage information for the
         --reference option. Note that you need to put a space at the start, if
```

### Comparing `gb2seq-0.2.4/gb2seq/genome.py` & `gb2seq-0.2.5/gb2seq/genome.py`

 * *Files identical despite different names*

### Comparing `gb2seq-0.2.4/gb2seq/sars2.py` & `gb2seq-0.2.5/gb2seq/sars2.py`

 * *Files identical despite different names*

### Comparing `gb2seq-0.2.4/gb2seq/translate.py` & `gb2seq-0.2.5/gb2seq/translate.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,22 +87,22 @@
         offset = seq.find(SLIPPERY_SEQUENCE, 13000)
         stop = seq.find("TAA", offset + _SLIPPERY_LEN)
         if offset == -1:
             raise NoSlipperySequenceError("No slippery sequence found.")
         if stop == -1:
             raise NoStopCodonError(
                 f"Could not find a stop codon downstream from the start of "
-                f"the slippery sequence at location {offset + 1}."
+                f"the slippery sequence at site {offset + 1}."
             )
         if stop - offset > _MAX_DISTANCE_TO_STOP:
             raise StopCodonTooDistantError(
                 f"The stop codon was too far ({stop - offset} nucleotides) "
                 f"downstream (max allowed distance is "
                 f"{_MAX_DISTANCE_TO_STOP}) from the start of the slippery "
-                f"sequence at location {offset + 1}."
+                f"sequence at site {offset + 1}."
             )
 
         seq = seq[: offset + _SLIPPERY_LEN] + seq[offset + _SLIPPERY_LEN - 1 :]
 
     # Pad with 'N' to avoid a 'BiopythonWarning: Partial codon' warning.
     remainder = len(seq) % 3
     seq += "N" * (3 - remainder if remainder else 0)
@@ -462,15 +462,15 @@
     """
     seq = genomeAa.sequence
     seqLen = len(seq)
     if seqLen == 1274:
         # There are no insertions.
         return seq
     elif seqLen > 1274:
-        for (target, findStart, findStop, sliceStart, sliceStop) in KNOWN_INSERTIONS:
+        for target, findStart, findStop, sliceStart, sliceStop in KNOWN_INSERTIONS:
             if seq.find(target, findStart, findStop) > -1:
                 return seq[:sliceStart] + seq[sliceStop:]
         if seqLen < 1290:
             substitutions = getSubstitutionsString(referenceAa, genomeAa)
             raise TranslatedSequenceLengthError(
                 f"Sequence with accession {accession} is too long "
                 f"(length: {seqLen}) and does not have a known insertion. "
```

### Comparing `gb2seq-0.2.4/gb2seq/variants.py` & `gb2seq-0.2.5/gb2seq/variants.py`

 * *Files identical despite different names*

### Comparing `gb2seq-0.2.4/gb2seq.egg-info/PKG-INFO` & `gb2seq-0.2.5/gb2seq.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: gb2seq
-Version: 0.2.4
-Summary: Python library and scripts for working with SARS-CoV-2 sequences.
+Version: 0.2.5
+Summary: Python library and scripts for working with unannotated sequences based on an annotated reference genome provided by a GenBank file.
 Home-page: https://github.com/virologycharite/gb2seq
 Download-URL: https://github.com/virologycharite/gb2seq
 Author: Terry C. Jones
 Author-email: terence.jones@charite.de
+Maintainer: Terry C. Jones
+Maintainer-email: terence.jones@charite.de
 License: MIT
 Keywords: GenBank,genetic sequences
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 License-File: AUTHORS
 
 See https://github.com/virologycharite/gb2seq for details.
-
```

### Comparing `gb2seq-0.2.4/setup.py` & `gb2seq-0.2.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,55 +1,60 @@
 #!/usr/bin/env python
 
 from setuptools import setup
 from pathlib import Path
+import re
 
 
 # Modified from http://stackoverflow.com/questions/2058802/
 # how-can-i-get-the-version-defined-in-setup-py-setuptools-in-my-package
 def version():
-    import re
-
     init = Path("gb2seq") / "__init__.py"
     with open(init) as fp:
-        initData = fp.read()
-    match = re.search(r"^__version__ = ['\"]([^'\"]+)['\"]", initData, re.M)
+        data = fp.read()
+    match = re.search(r"^__version__ = ['\"]([^'\"]+)['\"]", data, re.M)
     if match:
         return match.group(1)
-    else:
-        raise RuntimeError(f"Unable to find version string in {init!r}.")
+
+    raise RuntimeError(f"Unable to find version string in {init!r}.")
 
 
 setup(
     name="gb2seq",
     version=version(),
     packages=["gb2seq"],
     url="https://github.com/virologycharite/gb2seq",
     download_url="https://github.com/virologycharite/gb2seq",
     author="Terry C. Jones",
     author_email="terence.jones@charite.de",
+    maintainer="Terry C. Jones",
+    maintainer_email="terence.jones@charite.de",
     keywords=["GenBank", "genetic sequences"],
     scripts=[
         "bin/annotate-genome.py",
         "bin/describe-feature.py",
         "bin/describe-genome.py",
         "bin/describe-site.py",
     ],
+    include_package_data=True,
+    package_data={"gb2seq": ["data/*.fasta", "data/*.gb"]},
     classifiers=[
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Topic :: Software Development :: Libraries :: Python Modules",
     ],
     description=(
-        "Python library and scripts for working with SARS-CoV-2 " "sequences."
+        "Python library and scripts for working with unannotated sequences "
+        "based on an annotated reference genome provided by a GenBank file."
     ),
     long_description=("See https://github.com/virologycharite/gb2seq for details."),
     license="MIT",
-    install_requires=["dark-matter>=4.0.21"],
+    install_requires=["dark-matter>=4.0.55"],
 )
```

### Comparing `gb2seq-0.2.4/test/test_alignment.py` & `gb2seq-0.2.5/test/test_alignment.py`

 * *Files 2% similar despite different names*

```diff
@@ -609,29 +609,60 @@
             error,
             alignment.offsetInfo,
             0,
             featureName="surface glycoprotein",
             aa=True,
         )
 
+    def testOffsetTooBig(self):
+        """
+        If the requested offset is beyond the end of the reference genome, an
+        IndexError must be raised.
+        """
+        features = Features(
+            {
+                "nsp10": {
+                    "name": "nsp10",
+                    "start": 10,
+                    "stop": 16,
+                },
+                "nsp11": {
+                    "name": "nsp11",
+                    "start": 10,
+                    "stop": 16,
+                },
+            },
+            DNARead("refId", "AA"),
+            sars2=True,
+        )
+        alignment = Gb2Alignment(DNARead("genId", "AA"), features=features)
+        error = r"^Request for offset 12 in a reference genome of length 2\.$"
+
+        self.assertRaisesRegex(
+            IndexError,
+            error,
+            alignment.offsetInfo,
+            12,
+        )
+
     def testNoFeaturesAtOffset(self):
         """
         If there are no features at the given offset, a MissingFeatureError
         must be raised. This must be true regardless of the passed value of
         relativeToFeature.
         """
         features = Features(
             {
                 "surface glycoprotein": {
                     "name": "surface glycoprotein",
                     "start": 0,
                     "stop": 6,
                 },
             },
-            DNARead("refId", "AA"),
+            DNARead("refId", "A" * 200),
             sars2=True,
         )
         alignment = Gb2Alignment(DNARead("genId", "AA"), features=features)
         error = (
             r"^Feature 'surface glycoprotein' \(located at sites 1-6\) "
             r"does not overlap site 101\. There are no features at "
             r"that site\.$"
@@ -662,15 +693,15 @@
                 },
                 "nsp10": {
                     "name": "nsp10",
                     "start": 10,
                     "stop": 16,
                 },
             },
-            DNARead("refId", "AA"),
+            DNARead("refId", "A" * 25),
             sars2=True,
         )
         alignment = Gb2Alignment(DNARead("genId", "AA"), features=features)
         error = (
             r"^Requested feature 'surface glycoprotein' \(located at "
             r"sites 1-6\) does not overlap site 11. The feature\(s\) "
             r"at that site are: 'nsp10' \(11 - 16\)\.$"
@@ -706,15 +737,15 @@
                 },
                 "nsp11": {
                     "name": "nsp11",
                     "start": 10,
                     "stop": 16,
                 },
             },
-            DNARead("refId", "AA"),
+            DNARead("refId", "A" * 25),
             sars2=True,
         )
         alignment = Gb2Alignment(DNARead("genId", "AA"), features=features)
         error = (
             r"^Requested feature 'surface glycoprotein' \(located at "
             r"sites 1-6\) does not overlap site 11. The feature\(s\) "
             r"at that site are: 'nsp10' \(11 - 16\), 'nsp11' \(11 - 16\)\.$"
@@ -725,42 +756,93 @@
                 error,
                 alignment.offsetInfo,
                 10,
                 featureName="surface glycoprotein",
                 relativeToFeature=relativeToFeature,
             )
 
-    def testMultipleFeaturesAtOffsetButNoFeatureRequested(self):
+    def testMultipleFeaturesAtOffsetButNoFeatureRequestedNoAmbiguous(self):
         """
         If multiple features are found at an offset but no feature name is
-        passed, an AmbiguousFeatureError must be raised.
+        passed and allowAmbiguous is False, an AmbiguousFeatureError must be
+        raised.
         """
         features = Features(
             {
                 "nsp10": {
                     "name": "nsp10",
                     "start": 10,
                     "stop": 16,
                 },
                 "nsp11": {
                     "name": "nsp11",
                     "start": 10,
                     "stop": 16,
                 },
             },
-            DNARead("refId", "AA"),
+            DNARead("refId", "AAAAAAAAAAAAAA"),
             sars2=True,
         )
         alignment = Gb2Alignment(DNARead("genId", "AA"), features=features)
         error = (
             r"^There are multiple features at site 13: 'nsp10' \(11 - 16\), 'nsp11' "
             r"\(11 - 16\). Pass a feature name to specify which one you want\.$"
         )
 
-        self.assertRaisesRegex(AmbiguousFeatureError, error, alignment.offsetInfo, 12)
+        self.assertRaisesRegex(
+            AmbiguousFeatureError, error, alignment.offsetInfo, 12, allowAmbiguous=False
+        )
+
+    def testMultipleFeaturesAtOffsetButNoFeatureRequestedAllowAmbiguous(self):
+        """
+        If multiple features are found at an offset but no feature name is
+        passed and allowAmbiguous is true,...
+        """
+        features = Features(
+            {
+                "nsp10": {
+                    "name": "nsp10",
+                    "start": 10,
+                    "stop": 16,
+                },
+                "nsp11": {
+                    "name": "nsp11",
+                    "start": 10,
+                    "stop": 16,
+                },
+            },
+            DNARead("refId", "AAAAAAAAAAAAAA"),
+            sars2=True,
+        )
+        alignment = Gb2Alignment(DNARead("genId", "AA"), features=features)
+
+        self.assertEqual(
+            {
+                "alignmentOffset": 11,
+                "featureName": "nsp10",
+                "featureNames": {"nsp10", "nsp11"},
+                "reference": {
+                    "aa": "K",
+                    "codon": "AAA",
+                    "frame": 1,
+                    "id": "refId",
+                    "aaOffset": 0,
+                    "ntOffset": 11,
+                },
+                "genome": {
+                    "aa": "-",
+                    "codon": "AA-",
+                    "frame": 0,
+                    "id": "genId",
+                    "aaOffset": 0,
+                    "ntOffset": 0,
+                },
+            },
+            alignment.offsetInfo(11, allowAmbiguous=True),
+        )
 
     def testNoFeaturesAtOffsetZero(self):
         """
         If there are no features at offset zero, the return information
         should indicate that, but a codon and amino acid are still returned.
         """
         features = Features(
```

### Comparing `gb2seq-0.2.4/test/test_change.py` & `gb2seq-0.2.5/test/test_change.py`

 * *Files identical despite different names*

### Comparing `gb2seq-0.2.4/test/test_checker.py` & `gb2seq-0.2.5/test/test_checker.py`

 * *Files identical despite different names*

### Comparing `gb2seq-0.2.4/test/test_features.py` & `gb2seq-0.2.5/test/test_features.py`

 * *Files identical despite different names*

### Comparing `gb2seq-0.2.4/test/test_genomes.py` & `gb2seq-0.2.5/test/test_genomes.py`

 * *Files identical despite different names*

### Comparing `gb2seq-0.2.4/test/test_translate.py` & `gb2seq-0.2.5/test/test_translate.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,30 +33,30 @@
     def testNoStopCodonFollowingTheSlipperySequence(self):
         """
         An ORF1ab polyprotein sequence must have a stop codon after the
         slippery sequence.
         """
         error = (
             r"^Could not find a stop codon downstream from the start of "
-            r"the slippery sequence at location 13001\.$"
+            r"the slippery sequence at site 13001\.$"
         )
         sequence = "A" * 13000 + SLIPPERY_SEQUENCE
         self.assertRaisesRegex(
             NoStopCodonError, error, translate, sequence, "ORF1ab polyprotein"
         )
 
     def testDistantStopCodonFollowingTheSlipperySequence(self):
         """
         An ORF1ab polyprotein sequence must have a stop codon not too far
         downstream of the slippery sequence.
         """
         error = (
             r"The stop codon was too far \(107 nucleotides\) downstream "
             r"\(max allowed distance is 20\) from the start of the "
-            r"slippery sequence at location 13001\.$"
+            r"slippery sequence at site 13001\.$"
         )
         sequence = "A" * 13000 + SLIPPERY_SEQUENCE + "A" * 100 + "TAA"
         self.assertRaisesRegex(
             StopCodonTooDistantError, error, translate, sequence, "ORF1ab polyprotein"
         )
 
     def testEmpty(self):
```

### Comparing `gb2seq-0.2.4/test/test_variants.py` & `gb2seq-0.2.5/test/test_variants.py`

 * *Files identical despite different names*

