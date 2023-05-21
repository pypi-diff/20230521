# Comparing `tmp/gb2seq-0.2.5.tar.gz` & `tmp/gb2seq-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gb2seq-0.2.5.tar", last modified: Sun May 21 12:43:18 2023, max compression
+gzip compressed data, was "gb2seq-0.2.6.tar", last modified: Sun May 21 14:18:29 2023, max compression
```

## Comparing `gb2seq-0.2.5.tar` & `gb2seq-0.2.6.tar`

### file list

```diff
@@ -1,46 +1,39 @@
-drwxrwxr-x   0 terry      (501) staff       (20)        0 2023-05-21 12:43:18.053129 gb2seq-0.2.5/
--rw-rw-r--   0 terry      (501) staff       (20)       82 2022-08-03 22:54:17.000000 gb2seq-0.2.5/AUTHORS
--rw-rw-r--   0 terry      (501) staff       (20)       39 2023-05-20 21:53:46.000000 gb2seq-0.2.5/MANIFEST.in
--rw-rw-r--   0 terry      (501) staff       (20)     1124 2023-05-21 12:43:18.052664 gb2seq-0.2.5/PKG-INFO
--rw-rw-r--   0 terry      (501) staff       (20)    26579 2023-05-21 12:40:12.000000 gb2seq-0.2.5/README.md
-drwxrwxr-x   0 terry      (501) staff       (20)        0 2023-05-21 12:43:18.039235 gb2seq-0.2.5/bin/
--rwxrwxr-x   0 terry      (501) staff       (20)     1933 2022-08-04 07:08:53.000000 gb2seq-0.2.5/bin/annotate-genome.py
--rwxrwxr-x   0 terry      (501) staff       (20)     7257 2023-05-21 10:01:54.000000 gb2seq-0.2.5/bin/describe-feature.py
--rwxrwxr-x   0 terry      (501) staff       (20)    15353 2023-05-20 07:09:01.000000 gb2seq-0.2.5/bin/describe-genome.py
--rwxrwxr-x   0 terry      (501) staff       (20)     6171 2023-05-21 10:32:17.000000 gb2seq-0.2.5/bin/describe-site.py
-drwxrwxr-x   0 terry      (501) staff       (20)        0 2023-05-21 12:43:18.041384 gb2seq-0.2.5/data/
--rw-rw-r--   0 terry      (501) staff       (20)    29907 2022-08-03 22:52:44.000000 gb2seq-0.2.5/data/BavPat2.fasta
--rw-rw-r--   0 terry      (501) staff       (20)    29944 2022-08-03 22:52:44.000000 gb2seq-0.2.5/data/EPI_ISL_402125.fasta
--rw-rw-r--   0 terry      (501) staff       (20)    29814 2022-08-03 22:52:44.000000 gb2seq-0.2.5/data/EPI_ISL_601443.fasta
--rw-rw-r--   0 terry      (501) staff       (20)    29927 2022-08-03 22:52:44.000000 gb2seq-0.2.5/data/EPI_ISL_678597.fasta
--rw-rw-r--   0 terry      (501) staff       (20)    30001 2022-08-03 22:52:44.000000 gb2seq-0.2.5/data/NC_045512.2.fasta
--rw-rw-r--   0 terry      (501) staff       (20)    78471 2022-08-03 22:52:44.000000 gb2seq-0.2.5/data/NC_045512.2.gb
-drwxrwxr-x   0 terry      (501) staff       (20)        0 2023-05-21 12:43:18.045944 gb2seq-0.2.5/gb2seq/
--rw-rw-r--   0 terry      (501) staff       (20)      170 2023-05-20 12:23:13.000000 gb2seq-0.2.5/gb2seq/__init__.py
--rw-rw-r--   0 terry      (501) staff       (20)    41849 2023-05-21 12:40:54.000000 gb2seq-0.2.5/gb2seq/alignment.py
--rw-rw-r--   0 terry      (501) staff       (20)     7745 2023-03-24 11:55:34.000000 gb2seq-0.2.5/gb2seq/annotate.py
--rw-rw-r--   0 terry      (501) staff       (20)     1701 2022-08-03 22:54:17.000000 gb2seq-0.2.5/gb2seq/change.py
--rw-rw-r--   0 terry      (501) staff       (20)     1961 2022-08-03 22:54:17.000000 gb2seq-0.2.5/gb2seq/checker.py
--rw-rw-r--   0 terry      (501) staff       (20)    27096 2023-05-21 12:37:42.000000 gb2seq-0.2.5/gb2seq/features.py
--rw-rw-r--   0 terry      (501) staff       (20)      558 2022-08-03 22:54:17.000000 gb2seq-0.2.5/gb2seq/genome.py
--rw-rw-r--   0 terry      (501) staff       (20)     2457 2023-03-24 11:55:34.000000 gb2seq-0.2.5/gb2seq/sars2.py
--rw-rw-r--   0 terry      (501) staff       (20)    20485 2023-05-21 07:41:44.000000 gb2seq-0.2.5/gb2seq/translate.py
--rw-rw-r--   0 terry      (501) staff       (20)     2049 2022-08-03 22:56:02.000000 gb2seq-0.2.5/gb2seq/variants.py
-drwxrwxr-x   0 terry      (501) staff       (20)        0 2023-05-21 12:43:18.048165 gb2seq-0.2.5/gb2seq.egg-info/
--rw-rw-r--   0 terry      (501) staff       (20)     1124 2023-05-21 12:43:17.000000 gb2seq-0.2.5/gb2seq.egg-info/PKG-INFO
--rw-rw-r--   0 terry      (501) staff       (20)      788 2023-05-21 12:43:17.000000 gb2seq-0.2.5/gb2seq.egg-info/SOURCES.txt
--rw-rw-r--   0 terry      (501) staff       (20)        1 2023-05-21 12:43:17.000000 gb2seq-0.2.5/gb2seq.egg-info/dependency_links.txt
--rw-rw-r--   0 terry      (501) staff       (20)       20 2023-05-21 12:43:17.000000 gb2seq-0.2.5/gb2seq.egg-info/requires.txt
--rw-rw-r--   0 terry      (501) staff       (20)        7 2023-05-21 12:43:17.000000 gb2seq-0.2.5/gb2seq.egg-info/top_level.txt
--rw-rw-r--   0 terry      (501) staff       (20)      539 2023-05-20 13:31:27.000000 gb2seq-0.2.5/pyproject.toml
--rw-rw-r--   0 terry      (501) staff       (20)       38 2023-05-21 12:43:18.053253 gb2seq-0.2.5/setup.cfg
--rw-rw-r--   0 terry      (501) staff       (20)     2065 2023-05-21 10:43:53.000000 gb2seq-0.2.5/setup.py
-drwxrwxr-x   0 terry      (501) staff       (20)        0 2023-05-21 12:43:18.052090 gb2seq-0.2.5/test/
--rw-rw-r--   0 terry      (501) staff       (20)    66769 2023-05-20 14:35:53.000000 gb2seq-0.2.5/test/test_alignment.py
--rw-rw-r--   0 terry      (501) staff       (20)     1903 2022-08-03 23:06:40.000000 gb2seq-0.2.5/test/test_change.py
--rw-rw-r--   0 terry      (501) staff       (20)     5155 2022-08-04 09:52:00.000000 gb2seq-0.2.5/test/test_checker.py
--rw-rw-r--   0 terry      (501) staff       (20)    12860 2023-03-24 11:55:34.000000 gb2seq-0.2.5/test/test_features.py
--rw-rw-r--   0 terry      (501) staff       (20)    17184 2022-09-12 21:20:27.000000 gb2seq-0.2.5/test/test_genomes.py
--rw-rw-r--   0 terry      (501) staff       (20)      414 2022-08-03 23:08:39.000000 gb2seq-0.2.5/test/test_sars2.py
--rw-rw-r--   0 terry      (501) staff       (20)    21028 2023-05-21 12:34:49.000000 gb2seq-0.2.5/test/test_translate.py
--rw-rw-r--   0 terry      (501) staff       (20)     1141 2022-08-04 09:51:21.000000 gb2seq-0.2.5/test/test_variants.py
+drwxrwxr-x   0 terry      (501) staff       (20)        0 2023-05-21 14:18:29.961735 gb2seq-0.2.6/
+-rw-rw-r--   0 terry      (501) staff       (20)       82 2022-08-03 22:54:17.000000 gb2seq-0.2.6/AUTHORS
+-rw-rw-r--   0 terry      (501) staff       (20)       39 2023-05-20 21:53:46.000000 gb2seq-0.2.6/MANIFEST.in
+-rw-rw-r--   0 terry      (501) staff       (20)     1124 2023-05-21 14:18:29.961277 gb2seq-0.2.6/PKG-INFO
+-rw-rw-r--   0 terry      (501) staff       (20)    26621 2023-05-21 12:53:46.000000 gb2seq-0.2.6/README.md
+drwxrwxr-x   0 terry      (501) staff       (20)        0 2023-05-21 14:18:29.947806 gb2seq-0.2.6/bin/
+-rwxrwxr-x   0 terry      (501) staff       (20)     1933 2022-08-04 07:08:53.000000 gb2seq-0.2.6/bin/annotate-genome.py
+-rwxrwxr-x   0 terry      (501) staff       (20)     7257 2023-05-21 10:01:54.000000 gb2seq-0.2.6/bin/describe-feature.py
+-rwxrwxr-x   0 terry      (501) staff       (20)    15353 2023-05-20 07:09:01.000000 gb2seq-0.2.6/bin/describe-genome.py
+-rwxrwxr-x   0 terry      (501) staff       (20)     6171 2023-05-21 10:32:17.000000 gb2seq-0.2.6/bin/describe-site.py
+drwxrwxr-x   0 terry      (501) staff       (20)        0 2023-05-21 14:18:29.952612 gb2seq-0.2.6/gb2seq/
+-rw-rw-r--   0 terry      (501) staff       (20)       93 2023-05-21 13:47:53.000000 gb2seq-0.2.6/gb2seq/__init__.py
+-rw-rw-r--   0 terry      (501) staff       (20)    41849 2023-05-21 12:40:54.000000 gb2seq-0.2.6/gb2seq/alignment.py
+-rw-rw-r--   0 terry      (501) staff       (20)     7745 2023-03-24 11:55:34.000000 gb2seq-0.2.6/gb2seq/annotate.py
+-rw-rw-r--   0 terry      (501) staff       (20)     1701 2022-08-03 22:54:17.000000 gb2seq-0.2.6/gb2seq/change.py
+-rw-rw-r--   0 terry      (501) staff       (20)     1961 2022-08-03 22:54:17.000000 gb2seq-0.2.6/gb2seq/checker.py
+-rw-rw-r--   0 terry      (501) staff       (20)    27532 2023-05-21 14:02:33.000000 gb2seq-0.2.6/gb2seq/features.py
+-rw-rw-r--   0 terry      (501) staff       (20)      558 2022-08-03 22:54:17.000000 gb2seq-0.2.6/gb2seq/genome.py
+-rw-rw-r--   0 terry      (501) staff       (20)     2457 2023-03-24 11:55:34.000000 gb2seq-0.2.6/gb2seq/sars2.py
+-rw-rw-r--   0 terry      (501) staff       (20)    20485 2023-05-21 07:41:44.000000 gb2seq-0.2.6/gb2seq/translate.py
+-rw-rw-r--   0 terry      (501) staff       (20)     2049 2022-08-03 22:56:02.000000 gb2seq-0.2.6/gb2seq/variants.py
+drwxrwxr-x   0 terry      (501) staff       (20)        0 2023-05-21 14:18:29.954893 gb2seq-0.2.6/gb2seq.egg-info/
+-rw-rw-r--   0 terry      (501) staff       (20)     1124 2023-05-21 14:18:29.000000 gb2seq-0.2.6/gb2seq.egg-info/PKG-INFO
+-rw-rw-r--   0 terry      (501) staff       (20)      648 2023-05-21 14:18:29.000000 gb2seq-0.2.6/gb2seq.egg-info/SOURCES.txt
+-rw-rw-r--   0 terry      (501) staff       (20)        1 2023-05-21 14:18:29.000000 gb2seq-0.2.6/gb2seq.egg-info/dependency_links.txt
+-rw-rw-r--   0 terry      (501) staff       (20)       20 2023-05-21 14:18:29.000000 gb2seq-0.2.6/gb2seq.egg-info/requires.txt
+-rw-rw-r--   0 terry      (501) staff       (20)        7 2023-05-21 14:18:29.000000 gb2seq-0.2.6/gb2seq.egg-info/top_level.txt
+-rw-rw-r--   0 terry      (501) staff       (20)      539 2023-05-20 13:31:27.000000 gb2seq-0.2.6/pyproject.toml
+-rw-rw-r--   0 terry      (501) staff       (20)       38 2023-05-21 14:18:29.961870 gb2seq-0.2.6/setup.cfg
+-rw-rw-r--   0 terry      (501) staff       (20)     2079 2023-05-21 13:34:44.000000 gb2seq-0.2.6/setup.py
+drwxrwxr-x   0 terry      (501) staff       (20)        0 2023-05-21 14:18:29.960564 gb2seq-0.2.6/test/
+-rw-rw-r--   0 terry      (501) staff       (20)    66686 2023-05-21 13:39:01.000000 gb2seq-0.2.6/test/test_alignment.py
+-rw-rw-r--   0 terry      (501) staff       (20)     1903 2022-08-03 23:06:40.000000 gb2seq-0.2.6/test/test_change.py
+-rw-rw-r--   0 terry      (501) staff       (20)     5116 2023-05-21 13:39:38.000000 gb2seq-0.2.6/test/test_checker.py
+-rw-rw-r--   0 terry      (501) staff       (20)    12860 2023-03-24 11:55:34.000000 gb2seq-0.2.6/test/test_features.py
+-rw-rw-r--   0 terry      (501) staff       (20)    17090 2023-05-21 13:40:07.000000 gb2seq-0.2.6/test/test_genomes.py
+-rw-rw-r--   0 terry      (501) staff       (20)      414 2022-08-03 23:08:39.000000 gb2seq-0.2.6/test/test_sars2.py
+-rw-rw-r--   0 terry      (501) staff       (20)    21028 2023-05-21 12:34:49.000000 gb2seq-0.2.6/test/test_translate.py
+-rw-rw-r--   0 terry      (501) staff       (20)     1075 2023-05-21 13:47:12.000000 gb2seq-0.2.6/test/test_variants.py
```

### Comparing `gb2seq-0.2.5/PKG-INFO` & `gb2seq-0.2.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gb2seq
-Version: 0.2.5
+Version: 0.2.6
 Summary: Python library and scripts for working with unannotated sequences based on an annotated reference genome provided by a GenBank file.
 Home-page: https://github.com/virologycharite/gb2seq
 Download-URL: https://github.com/virologycharite/gb2seq
 Author: Terry C. Jones
 Author-email: terence.jones@charite.de
 Maintainer: Terry C. Jones
 Maintainer-email: terence.jones@charite.de
```

### Comparing `gb2seq-0.2.5/README.md` & `gb2seq-0.2.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -303,15 +303,15 @@
 ```
 
 Of course it's more fun if you also provide an unannotated genome to
 compare the reference to.  Here's the `N501Y` change in a SARS-CoV-2
 B.1.1.7 (Alpha variant) sequence:
 
 ```sh
-$ describe-site.py --sars2 --site 501 --relative --genome data/EPI_ISL_601443.fasta \
+$ describe-site.py --sars2 --site 501 --relative --genome gb2seq/data/EPI_ISL_601443.fasta \
     --feature spike --aa
 {
     "alignmentOffset": 23063,
     "featureName": "surface glycoprotein",
     "featureNames": [
         "surface glycoprotein"
     ],
@@ -349,15 +349,15 @@
 will be created for you if it doesn't exist.
 
 A small example is perhaps best. Here we extract the spike nucleotide and
 amino acid sequence from B.1.1.7 and also ask for a summary of the amino
 acid differences:
 
 ```sh
-$ describe-genome.py --genome data/EPI_ISL_601443.fasta --outDir /tmp/out \
+$ describe-genome.py --genome gb2seq/data/EPI_ISL_601443.fasta --outDir /tmp/out \
     --feature spike --printNtSequence --printAaSequence --printAaMatch
 Examined 1 genome.
 
 $ ls -l /tmp/out
 total 24
 -rw-rw-r--  1 terry  wheel   748 Apr 11 15:25 EPI_ISL_601443-spike-aa-match.txt
 -rw-rw-r--  1 terry  wheel  1344 Apr 11 15:25 EPI_ISL_601443-spike-aa-sequence.fasta
@@ -396,15 +396,15 @@
        982 S A 24506
       1118 D H 24914
 ```
 
 You can also ask for the changes in a variant to be checked.
       
 ```sh
-$ describe-genome.py --sars2 --genome data/EPI_ISL_601443.fasta --checkVariant VOC_20201201_UK
+$ describe-genome.py --sars2 --genome gb2seq/data/EPI_ISL_601443.fasta --checkVariant VOC_20201201_UK
 EPI_ISL_601443 hCoV-19/England/MILK-9E05B3/2020
 Variant summary:
   UK variant of concern (VOC) 202012/01:
   20 checks, 20 passed.
     orf1ab aa: PASS: 1001I, 1708D, 2230T, 3675-, 3676-, 3677-
     spike aa: PASS: 1118H, 144-, 501Y, 570D, 681H, 69-, 70-, 716I, 982A
     orf8 aa: PASS: 52I, 73C, Q27*
@@ -591,24 +591,24 @@
 ```
 
 Once you have a `Gb2Alignment` instance, you can ask it for aligned
 sequences or features.
 
 Below I'll use the GISAID `EPI_ISL_601443` (B.1.1.7, or Alpha, variant)
 sequence, which you can find in
-[data/EPI_ISL_601443.fasta](data/EPI_ISL_601443.fasta) in this repo:
+[gb2seq/data/EPI_ISL_601443.fasta](gb2seq/data/EPI_ISL_601443.fasta) in this repo:
 
 ```py
 >>> from pathlib import Path
 >>> from pprint import pprint as pp
 >>> from gb2seq.alignment import Gb2Alignment
 >>> from gb2seq.features import Features
 >>> from dark.fasta import FastaReads
 
->>> alpha = list(FastaReads(Path('data/EPI_ISL_601443.fasta')))[0]
+>>> alpha = list(FastaReads(Path('gb2seq/data/EPI_ISL_601443.fasta')))[0]
 >>> len(alpha)
 29764
 >>> alpha.id
 'EPI_ISL_601443 hCoV-19/England/MILK-9E05B3/2020'
 >>> alpha.sequence[:50]
 'AGATCTGTTCTCTAAACGAACTTTAAAATCTGTGTGGCTGTCACTCGGCT'
```

#### html2text {}

```diff
@@ -124,16 +124,16 @@
 acid site number (via `--aa`): ```sh $ describe-site.py --sars2 --site 501 --
 feature spike --relative --aa { "alignmentOffset": 23063, "featureName":
 "surface glycoprotein", "featureNames": [ "surface glycoprotein" ],
 "reference": { "aa": "N", "aaOffset": 500, "codon": "AAT", "frame": 0, "id":
 "NC_045512.2", "ntOffset": 23063 } } ``` Of course it's more fun if you also
 provide an unannotated genome to compare the reference to. Here's the `N501Y`
 change in a SARS-CoV-2 B.1.1.7 (Alpha variant) sequence: ```sh $ describe-
-site.py --sars2 --site 501 --relative --genome data/EPI_ISL_601443.fasta \ --
-feature spike --aa { "alignmentOffset": 23063, "featureName": "surface
+site.py --sars2 --site 501 --relative --genome gb2seq/data/EPI_ISL_601443.fasta
+\ --feature spike --aa { "alignmentOffset": 23063, "featureName": "surface
 glycoprotein", "featureNames": [ "surface glycoprotein" ], "genome": { "aa":
 "Y", "aaOffset": 497, "codon": "TAT", "frame": 0, "id": "EPI_ISL_601443 hCoV-
 19/England/MILK-9E05B3/2020", "ntOffset": 22991 }, "reference": { "aa": "N",
 "aaOffset": 500, "codon": "AAT", "frame": 0, "id": "NC_045512.2", "ntOffset":
 23063 } } ``` Other options include `--genomeAaOnly` to just print the amino
 acid at a location in the genome, `--includeFeature` to also receive
 information about the feature at the site, and `--minReferenceCoverage` to
@@ -141,15 +141,15 @@
 genome.py `describe-genome.py` has many uses. It can extract multiple features
 from multiple given genomes, as amino acids or nucleotides or both. It will
 print to standard output by default, but if you use the `--outDir` option to
 provide a directory, individual output files with (hopefully) self-explanatory
 names will be created in that directory. The directory will be created for you
 if it doesn't exist. A small example is perhaps best. Here we extract the spike
 nucleotide and amino acid sequence from B.1.1.7 and also ask for a summary of
-the amino acid differences: ```sh $ describe-genome.py --genome data/
+the amino acid differences: ```sh $ describe-genome.py --genome gb2seq/data/
 EPI_ISL_601443.fasta --outDir /tmp/out \ --feature spike --printNtSequence --
 printAaSequence --printAaMatch Examined 1 genome. $ ls -l /tmp/out total 24 -
 rw-rw-r-- 1 terry wheel 748 Apr 11 15:25 EPI_ISL_601443-spike-aa-match.txt -rw-
 rw-r-- 1 terry wheel 1344 Apr 11 15:25 EPI_ISL_601443-spike-aa-sequence.fasta -
 rw-rw-r-- 1 terry wheel 3886 Apr 11 15:25 EPI_ISL_601443-spike-nt-
 sequence.fasta ``` If the file given by `--genome` had contained more than one
 SARS-CoV-2 genome, the spike would have been extracted for all of them.
@@ -161,38 +161,38 @@
 (0.24%) Involving a gap in both sequences: 0 Id: NC_045512.2 (surface
 glycoprotein) Length: 1274 Gaps: 0 Id: EPI_ISL_601443 hCoV-19/England/MILK-
 9E05B3/2020 (surface glycoprotein) Length: 1274 Gaps: 3/1274 (0.24%) Gap
 locations (1-based): 69, 70, 144 Differences: site, aa1, aa2, ref nt codon
 start 69 H - 21767 70 V - 21770 144 Y - 21992 501 N Y 23063 570 A D 23270 614 D
 G 23402 681 P H 23603 716 T I 23708 982 S A 24506 1118 D H 24914 ``` You can
 also ask for the changes in a variant to be checked. ```sh $ describe-genome.py
---sars2 --genome data/EPI_ISL_601443.fasta --checkVariant VOC_20201201_UK
-EPI_ISL_601443 hCoV-19/England/MILK-9E05B3/2020 Variant summary: UK variant of
-concern (VOC) 202012/01: 20 checks, 20 passed. orf1ab aa: PASS: 1001I, 1708D,
-2230T, 3675-, 3676-, 3677- spike aa: PASS: 1118H, 144-, 501Y, 570D, 681H, 69-,
-70-, 716I, 982A orf8 aa: PASS: 52I, 73C, Q27* n aa: PASS: 235F, 3L ``` There
-are some known variants, and you can also provide your own via a JSON file and
-the `--variantFile` option. Your JSON should have the format you'll see in
-[variants.py](https://github.com/VirologyCharite/gb2seq/blob/master/gb2seq/
-variants.py). E.g.,: ``` VARIANTS = { 'VOC_20201201_UK': { 'description': 'UK
-variant of concern (VOC) 202012/01', 'comment': ('From Table 1 of https://
-www.gov.uk/government/' 'publications/investigation-of-novel-sars-cov-2' '-
-variant-variant-of-concern-20201201'), 'changes': { 'orf1ab': { 'aa': '1001I
-1708D 2230T 3675- 3676- 3677-', }, 'spike': { 'aa': '69- 70- 144- 501Y 570D
-681H 716I 982A 1118H', }, 'orf8': { 'aa': 'Q27* 52I 73C', }, 'n': { 'aa': '3L
-235F', } } } } ``` ## annotate-genome.py Produces JSON output with annotation
-information for a genome. Here's an example of the start of output for a
-Monkeypox genome (note that the nucleotide sequences have been truncated to
-reduce output width): ```sh $ annotate-genome.py --aligner edlib --reference
-ON676708.1.gb --genome ChVir28389.fasta { "features": { "A15.5L": { "genome":
-{ "sequence": "ATGATAAGTAATTACGAGCCGTTGCTGCTGTTAGTTATAAC...", "start": 121823,
-"stop": 121985, "translation":
-"MISNYEPLLLLVITCCVLLFNFTISSKTKIDIIFAVQTIVFIWFIFHFVYSAI*" }, "reference":
-{ "forward": false, "name": "A15.5L", "note": "Non-essential IMV membrane
-protein (Cop-A14.5L)", "product": "A15.5L", "sequence":
+--sars2 --genome gb2seq/data/EPI_ISL_601443.fasta --checkVariant
+VOC_20201201_UK EPI_ISL_601443 hCoV-19/England/MILK-9E05B3/2020 Variant
+summary: UK variant of concern (VOC) 202012/01: 20 checks, 20 passed. orf1ab
+aa: PASS: 1001I, 1708D, 2230T, 3675-, 3676-, 3677- spike aa: PASS: 1118H, 144-,
+501Y, 570D, 681H, 69-, 70-, 716I, 982A orf8 aa: PASS: 52I, 73C, Q27* n aa:
+PASS: 235F, 3L ``` There are some known variants, and you can also provide your
+own via a JSON file and the `--variantFile` option. Your JSON should have the
+format you'll see in [variants.py](https://github.com/VirologyCharite/gb2seq/
+blob/master/gb2seq/variants.py). E.g.,: ``` VARIANTS = { 'VOC_20201201_UK':
+{ 'description': 'UK variant of concern (VOC) 202012/01', 'comment': ('From
+Table 1 of https://www.gov.uk/government/' 'publications/investigation-of-
+novel-sars-cov-2' '-variant-variant-of-concern-20201201'), 'changes':
+{ 'orf1ab': { 'aa': '1001I 1708D 2230T 3675- 3676- 3677-', }, 'spike': { 'aa':
+'69- 70- 144- 501Y 570D 681H 716I 982A 1118H', }, 'orf8': { 'aa': 'Q27* 52I
+73C', }, 'n': { 'aa': '3L 235F', } } } } ``` ## annotate-genome.py Produces
+JSON output with annotation information for a genome. Here's an example of the
+start of output for a Monkeypox genome (note that the nucleotide sequences have
+been truncated to reduce output width): ```sh $ annotate-genome.py --aligner
+edlib --reference ON676708.1.gb --genome ChVir28389.fasta { "features":
+{ "A15.5L": { "genome": { "sequence":
+"ATGATAAGTAATTACGAGCCGTTGCTGCTGTTAGTTATAAC...", "start": 121823, "stop":
+121985, "translation": "MISNYEPLLLLVITCCVLLFNFTISSKTKIDIIFAVQTIVFIWFIFHFVYSAI*"
+}, "reference": { "forward": false, "name": "A15.5L", "note": "Non-essential
+IMV membrane protein (Cop-A14.5L)", "product": "A15.5L", "sequence":
 "TTAAATCGCCGAATAAACAAAGTGGAATATAAACCATATAA...", "start": 121759, "stop":
 121921, "translation": "MISNYEPLLLLVITCCVLLFNFTISSKTKIDIIFAVQTIVFIWFIFHFVYSAI*"
 } }, "A32.5L": { "genome": { "sequence":
 "ATGTTAAAAATGTCAGCTGCCGACTTTTTGGAACGTTTGAT...", "start": 139696, "stop":
 139825, "translation": "MLKMSAADFLERLIKAGIYIYVLRTKYVITALLVKNYPIKDE*" },
 "reference": { "forward": false, "name": "A32.5L", "note": "Viral membrane
 assembly proteins (VMAP) (Cop-A 30.5L)", "product": "A32.5L", "sequence":
@@ -238,27 +238,27 @@
 ("NC_045512.2.gb") alignment = Gb2Alignment(Read('id', 'AGCT...'), features)
 ``` These can also be read from a FASTA file: ```py from gb2seq.alignment
 import Gb2Alignment from gb2seq.features import Features from dark.fasta import
 FastaReads features = Features("NC_045512.2.gb") for read in FastaReads
 ('sequences.fasta'): alignment = Gb2Alignment(read, features) ``` Once you have
 a `Gb2Alignment` instance, you can ask it for aligned sequences or features.
 Below I'll use the GISAID `EPI_ISL_601443` (B.1.1.7, or Alpha, variant)
-sequence, which you can find in [data/EPI_ISL_601443.fasta](data/
+sequence, which you can find in [gb2seq/data/EPI_ISL_601443.fasta](gb2seq/data/
 EPI_ISL_601443.fasta) in this repo: ```py >>> from pathlib import Path >>> from
 pprint import pprint as pp >>> from gb2seq.alignment import Gb2Alignment >>>
 from gb2seq.features import Features >>> from dark.fasta import FastaReads >>>
-alpha = list(FastaReads(Path('data/EPI_ISL_601443.fasta')))[0] >>> len(alpha)
-29764 >>> alpha.id 'EPI_ISL_601443 hCoV-19/England/MILK-9E05B3/2020' >>>
-alpha.sequence[:50] 'AGATCTGTTCTCTAAACGAACTTTAAAATCTGTGTGGCTGTCACTCGGCT' >>>
-features = Features(sars2=True) >>> alignment = Gb2Alignment(alpha) ``` You'll
-find the aligned reference and genome in `alignment.referenceAligned` and
-`alignment.genomeAligned`, both of which are `Read` instances: ```py >>> len
-(alignment.referenceAligned) 29903 >>> len(alignment.genomeAligned) 29903 # Get
-the nucleotide sequence for the spike protein for the reference and genome. >>>
-referenceSpikeNt, genomeSpikeNt = alignment.ntSequences('spike') >>> len
+alpha = list(FastaReads(Path('gb2seq/data/EPI_ISL_601443.fasta')))[0] >>> len
+(alpha) 29764 >>> alpha.id 'EPI_ISL_601443 hCoV-19/England/MILK-9E05B3/2020'
+>>> alpha.sequence[:50] 'AGATCTGTTCTCTAAACGAACTTTAAAATCTGTGTGGCTGTCACTCGGCT'
+>>> features = Features(sars2=True) >>> alignment = Gb2Alignment(alpha) ```
+You'll find the aligned reference and genome in `alignment.referenceAligned`
+and `alignment.genomeAligned`, both of which are `Read` instances: ```py >>>
+len(alignment.referenceAligned) 29903 >>> len(alignment.genomeAligned) 29903 #
+Get the nucleotide sequence for the spike protein for the reference and genome.
+>>> referenceSpikeNt, genomeSpikeNt = alignment.ntSequences('spike') >>> len
 (referenceSpikeNt) 3822 # Get the amino acid sequence for the spike protein for
 the reference and genome. >>> referenceSpikeAa, genomeSpikeAa =
 alignment.aaSequences('spike') >>> len(referenceSpikeAa) 1274 # There were
 three deletions in the alpha spike, so it only covers 3813 of the # 3822 bases
 in the reference spike. >>> alignment.coverage('s') (3813, 3822) # Get
 information about what's at an offset (0-based). This is what the describe-
 site.py # utility does (though it takes a 1-based site). # # Here is the Alpha
```

### Comparing `gb2seq-0.2.5/bin/annotate-genome.py` & `gb2seq-0.2.6/bin/annotate-genome.py`

 * *Files identical despite different names*

### Comparing `gb2seq-0.2.5/bin/describe-feature.py` & `gb2seq-0.2.6/bin/describe-feature.py`

 * *Files identical despite different names*

### Comparing `gb2seq-0.2.5/bin/describe-genome.py` & `gb2seq-0.2.6/bin/describe-genome.py`

 * *Files identical despite different names*

### Comparing `gb2seq-0.2.5/bin/describe-site.py` & `gb2seq-0.2.6/bin/describe-site.py`

 * *Files identical despite different names*

### Comparing `gb2seq-0.2.5/gb2seq/alignment.py` & `gb2seq-0.2.6/gb2seq/alignment.py`

 * *Files identical despite different names*

### Comparing `gb2seq-0.2.5/gb2seq/annotate.py` & `gb2seq-0.2.6/gb2seq/annotate.py`

 * *Files identical despite different names*

### Comparing `gb2seq-0.2.5/gb2seq/change.py` & `gb2seq-0.2.6/gb2seq/change.py`

 * *Files identical despite different names*

### Comparing `gb2seq-0.2.5/gb2seq/checker.py` & `gb2seq-0.2.6/gb2seq/checker.py`

 * *Files identical despite different names*

### Comparing `gb2seq-0.2.5/gb2seq/features.py` & `gb2seq-0.2.6/gb2seq/features.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 import sys
 from os import environ
 import itertools
 from collections import UserDict
 from pathlib import Path
 from typing import Dict, Optional, Set, Union
 
+try:
+    from importlib.resources import open_text
+except ImportError:
+    from importlib_resources import open_text
+
+
 # from warnings import warn
 import json
 import argparse
 
 from Bio import Entrez, SeqIO
 from Bio.SeqRecord import SeqRecord
 
 from dark.aa import STOP_CODONS
 from dark.genbank import GenomeRanges
 from dark.reads import DNARead
 
-from gb2seq import Gb2SeqError, DATA_DIR
+from gb2seq import Gb2SeqError
 from gb2seq.sars2 import SARS_COV_2_ALIASES, SARS_COV_2_TRANSLATED
 
 # Set ENTREZ_EMAIL in your environment to have your requests to NCBI Entez
 # be accompanied by your address. If you don't do this you'll see warning
 # messages and be limited to a lower rate of querying.
 Entrez.email = environ.get("ENTREZ_EMAIL")
 
@@ -54,43 +60,47 @@
         features (in which case some defaults can be set).
     @raise ValueError: If a reference is passed with a string or Path
         specification.
     @raise ReferenceWithGapError: If the reference or one of its features has a
         gap in its nucleotide sequence.
     """
 
-    WUHAN_REF = DATA_DIR / "NC_045512.2.gb"
-
     def __init__(
         self,
         referenceSpecification: Union[str, Dict, Path] = None,
         reference: Optional[DNARead] = None,
         sars2: bool = False,
         translated: Optional[Set[str]] = None,
         aliases: Optional[Dict[str, str]] = None,
         addUnannotatedRegions: bool = False,
     ) -> None:
         super().__init__()
         self.sars2 = sars2
         self.translatedNames: Set[str] = set()
 
-        if sars2:
-            referenceSpecification = (
-                self.WUHAN_REF
-                if referenceSpecification is None
-                else referenceSpecification
-            )
-        else:
-            if referenceSpecification is None:
+        if referenceSpecification is None:
+            if sars2:
+                with open_text("gb2seq.data", "NC_045512.2.gb") as fp:
+                    try:
+                        record = SeqIO.read(fp, "genbank")
+                    except Exception as e:
+                        print(
+                            "Could not parse default SARS-CoV-2 GenBank record",
+                            e,
+                            file=sys.stderr,
+                        )
+                        sys.exit(1)
+                    else:
+                        self._initializeFromGenBankRecord(record)
+            else:
                 raise ValueError(
                     "A reference specification must be provided for non-SARS-CoV-2 "
                     "features."
                 )
-
-        if isinstance(referenceSpecification, SeqRecord):
+        elif isinstance(referenceSpecification, SeqRecord):
             record = referenceSpecification
             self._initializeFromGenBankRecord(record)
         elif isinstance(referenceSpecification, str):
             if reference is not None:
                 raise ValueError(
                     "A reference cannot be passed with a string specification."
                 )
@@ -134,15 +144,15 @@
                     client = Entrez.efetch(
                         db="nucleotide",
                         rettype="gb",
                         retmode="text",
                         id=referenceSpecification,
                     )
                     try:
-                        record = SeqIO.read(client, "gb")
+                        record = SeqIO.read(client, "genbank")
                     except Exception as e:
                         print(
                             "Could not parse fetched GenBank record:",
                             e,
                             file=sys.stderr,
                         )
                         sys.exit(1)
```

### Comparing `gb2seq-0.2.5/gb2seq/genome.py` & `gb2seq-0.2.6/gb2seq/genome.py`

 * *Files identical despite different names*

### Comparing `gb2seq-0.2.5/gb2seq/sars2.py` & `gb2seq-0.2.6/gb2seq/sars2.py`

 * *Files identical despite different names*

### Comparing `gb2seq-0.2.5/gb2seq/translate.py` & `gb2seq-0.2.6/gb2seq/translate.py`

 * *Files identical despite different names*

### Comparing `gb2seq-0.2.5/gb2seq/variants.py` & `gb2seq-0.2.6/gb2seq/variants.py`

 * *Files identical despite different names*

### Comparing `gb2seq-0.2.5/gb2seq.egg-info/PKG-INFO` & `gb2seq-0.2.6/gb2seq.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gb2seq
-Version: 0.2.5
+Version: 0.2.6
 Summary: Python library and scripts for working with unannotated sequences based on an annotated reference genome provided by a GenBank file.
 Home-page: https://github.com/virologycharite/gb2seq
 Download-URL: https://github.com/virologycharite/gb2seq
 Author: Terry C. Jones
 Author-email: terence.jones@charite.de
 Maintainer: Terry C. Jones
 Maintainer-email: terence.jones@charite.de
```

### Comparing `gb2seq-0.2.5/pyproject.toml` & `gb2seq-0.2.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gb2seq-0.2.5/setup.py` & `gb2seq-0.2.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     scripts=[
         "bin/annotate-genome.py",
         "bin/describe-feature.py",
         "bin/describe-genome.py",
         "bin/describe-site.py",
     ],
     include_package_data=True,
-    package_data={"gb2seq": ["data/*.fasta", "data/*.gb"]},
+    package_data={"gb2seq": ["gb2seq/data/*.fasta", "gb2seq/data/*.gb"]},
     classifiers=[
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
```

### Comparing `gb2seq-0.2.5/test/test_alignment.py` & `gb2seq-0.2.6/test/test_alignment.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 """
 
 from unittest import TestCase
 from io import StringIO
 
 from dark.reads import DNARead
 
-from gb2seq import DATA_DIR
 from gb2seq.alignment import (
     Gb2Alignment,
     getGappedOffsets,
     alignmentEnd,
     offsetInfoMultipleGenomes,
     AlignmentError,
 )
@@ -1449,15 +1448,15 @@
             )
 
     def testAlphaN501YByNucleotideOffsetRelativeToFeatureAllFrames(self):
         """
         We must be able to see the N501Y change in the spike of Alpha
         relative to the feature when using any frame and a nucleotide offset.
         """
-        genomeRead = getSequence(DATA_DIR / "EPI_ISL_601443.fasta")
+        genomeRead = getSequence("EPI_ISL_601443.fasta")
         alignment = Gb2Alignment(genomeRead, features=Features(sars2=True))
         start = alignment.features["surface glycoprotein"]["start"]
         for frame in range(3):
             # The 500 comes from the N501Y.
             offset = 500 * 3 + frame
 
             # The offset in the genome should be 22990 + frame (this is based
@@ -1506,15 +1505,15 @@
             )
 
     def testAlphaN501YWithNucleotideOffset(self):
         """
         We must be able to see the N501Y change in the spike of Alpha when
         the offset is given in nucleotides in any frame.
         """
-        genomeRead = getSequence(DATA_DIR / "EPI_ISL_601443.fasta")
+        genomeRead = getSequence("EPI_ISL_601443.fasta")
         alignment = Gb2Alignment(genomeRead, features=Features(sars2=True))
         start = alignment.features["surface glycoprotein"]["start"]
         for frame in range(3):
             offset = start + 1500 + frame
 
             # See comment in test above re the 22990 test below.
             expectedGenomeOffset = offset - alignment.genomeAligned.sequence[
@@ -1549,15 +1548,15 @@
             )
 
     def testAlphaN501YWithAaOffset(self):
         """
         We must be able to see the N501Y change in the spike of Alpha
         using an amino acid offset.
         """
-        genomeRead = getSequence(DATA_DIR / "EPI_ISL_601443.fasta")
+        genomeRead = getSequence("EPI_ISL_601443.fasta")
         alignment = Gb2Alignment(genomeRead, features=Features(sars2=True))
         start = alignment.features["surface glycoprotein"]["start"]
         offset = 500
 
         # See comment in test above re the 22990 test below.
         expectedGenomeOffset = (
             start
@@ -1597,30 +1596,30 @@
             ),
         )
 
     def testAlphaSpikeSubstitutions(self):
         """
         We must be able to see all the substitutions in the spike of Alpha.
         """
-        genomeRead = getSequence(DATA_DIR / "EPI_ISL_601443.fasta")
+        genomeRead = getSequence("EPI_ISL_601443.fasta")
         alignment = Gb2Alignment(genomeRead, features=Features(sars2=True))
 
         for change in "N501Y A570D D614G P681H T716I S982A D1118H".split():
             referenceAa, offset, genomeAa = splitChange(change)
             offsetInfo = alignment.offsetInfo(
                 offset, aa=True, relativeToFeature=True, featureName="spike"
             )
             self.assertEqual(offsetInfo["reference"]["aa"], referenceAa)
             self.assertEqual(offsetInfo["genome"]["aa"], genomeAa)
 
     def testAlphaSpikeDeletions(self):
         """
         We must be able to see all the deletions in the spike of Alpha.
         """
-        genomeRead = getSequence(DATA_DIR / "EPI_ISL_601443.fasta")
+        genomeRead = getSequence("EPI_ISL_601443.fasta")
         alignment = Gb2Alignment(genomeRead, features=Features(sars2=True))
 
         for change in "H69- V70- Y144-".split():
             referenceAa, offset, genomeAa = splitChange(change)
             offsetInfo = alignment.offsetInfo(
                 offset, aa=True, relativeToFeature=True, featureName="spike"
             )
```

### Comparing `gb2seq-0.2.5/test/test_change.py` & `gb2seq-0.2.6/test/test_change.py`

 * *Files identical despite different names*

### Comparing `gb2seq-0.2.5/test/test_checker.py` & `gb2seq-0.2.6/test/test_checker.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 from unittest import TestCase
 
 from .fasta import getSequence
 
-from gb2seq import DATA_DIR
 from gb2seq.alignment import Gb2Alignment
 from gb2seq.checker import Checker, AAChecker, NTChecker
 from gb2seq.features import Features
 
 FEATURES = Features(sars2=True)
 
 
 class Test_EPI_ISL_601443(TestCase):
     """
     Test the EPI_ISL_601433 sequence. This is the variant of concern
     (VOC 202012/01) referred to in https://www.gov.uk/government/publications/
     investigation-of-novel-sars-cov-2-variant-variant-of-concern-20201201
     """
 
-    genomeRead = getSequence(DATA_DIR / "EPI_ISL_601443.fasta")
+    genomeRead = getSequence("EPI_ISL_601443.fasta")
     alignment = Gb2Alignment(genomeRead, FEATURES)
 
     def testIndexError(self):
         """
         If an check on a non-existent index is attempted, an IndexError must
         be raised.
         """
```

### Comparing `gb2seq-0.2.5/test/test_features.py` & `gb2seq-0.2.6/test/test_features.py`

 * *Files identical despite different names*

### Comparing `gb2seq-0.2.5/test/test_genomes.py` & `gb2seq-0.2.6/test/test_genomes.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 See test_alignment.py for tests of more basic Gb2Alignment functionality.
 """
 
 from unittest import TestCase
 
 from .fasta import getSequence
 
-from gb2seq import DATA_DIR
 from gb2seq.alignment import Gb2Alignment
 from gb2seq.features import Features
 from gb2seq.variants import VARIANTS
 
 FEATURES = Features(sars2=True)
 
 
@@ -54,27 +53,27 @@
 
     def testIdentical(self):
         """
         The EPI_ISL_402125 sequence from GISAID should be the same as the
         NC_045512.2 reference sequence from NCBI.
         """
         self.assertEqual(
-            getSequence(DATA_DIR / "EPI_ISL_402125.fasta").sequence,
-            getSequence(DATA_DIR / "NC_045512.2.fasta").sequence,
+            getSequence("EPI_ISL_402125.fasta").sequence,
+            getSequence("NC_045512.2.fasta").sequence,
         )
 
 
 class Test_EPI_ISL_601443(TestCase, _Mixin):
     """
     Test the EPI_ISL_601433 sequence. This is the variant of concern
     (VOC 202012/01) referred to in https://www.gov.uk/government/publications/
     investigation-of-novel-sars-cov-2-variant-variant-of-concern-20201201
     """
 
-    genomeRead = getSequence(DATA_DIR / "EPI_ISL_601443.fasta")
+    genomeRead = getSequence("EPI_ISL_601443.fasta")
     alignment = Gb2Alignment(genomeRead, FEATURES)
 
     def testSpikeDeletionsAa(self):
         """
         The spike protein should have the three deletions.
         """
         self.check("spike", "H69- V70- Y144-", True)
@@ -237,15 +236,15 @@
 
 
 class Test_BavPat2(TestCase, _Mixin):
     """
     Test the BavPat2 sequence. This is Bavarian patient #2.
     """
 
-    genomeRead = getSequence(DATA_DIR / "BavPat2.fasta")
+    genomeRead = getSequence("BavPat2.fasta")
     alignment = Gb2Alignment(genomeRead, FEATURES)
 
     def testSpikeMutationsNt(self):
         """
         The spike genome should have the expected change.
         """
         self.check("spike", "A1841G", False)
@@ -358,15 +357,15 @@
 
 class Test_NC_045512(TestCase, _Mixin):
     """
     Test the NC_045512.2 sequence, which should test as equal seeing as it is
     the default feature reference.
     """
 
-    genomeRead = getSequence(DATA_DIR / "NC_045512.2.fasta")
+    genomeRead = getSequence("NC_045512.2.fasta")
     alignment = Gb2Alignment(genomeRead, FEATURES)
 
     def testSpikeIdenticalNt(self):
         """
         The spike nucleotides should be identical.
         """
         genomeNt, referenceNt = self.alignment.ntSequences("S")
@@ -428,15 +427,15 @@
 
 class Test_EPI_ISL_678597(TestCase, _Mixin):
     """
     Test the EPI_ISL_678597 sequence. This is the South African variant of
     concern.
     """
 
-    genomeRead = getSequence(DATA_DIR / "EPI_ISL_678597.fasta")
+    genomeRead = getSequence("EPI_ISL_678597.fasta")
     alignment = Gb2Alignment(genomeRead, FEATURES)
 
     def testSpikeDeletionsAa(self):
         """
         The spike protein should have the three deletions.
         """
         self.check("spike", "L241- L242- A243-", True)
```

### Comparing `gb2seq-0.2.5/test/test_translate.py` & `gb2seq-0.2.6/test/test_translate.py`

 * *Files identical despite different names*

