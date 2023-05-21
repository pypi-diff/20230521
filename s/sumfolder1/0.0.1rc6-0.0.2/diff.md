# Comparing `tmp/sumfolder1-0.0.1rc6.tar.gz` & `tmp/sumfolder1-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sumfolder1-0.0.1rc6.tar", last modified: Mon Jan 16 13:02:55 2023, max compression
+gzip compressed data, was "sumfolder1-0.0.2.tar", last modified: Sun May 21 10:37:07 2023, max compression
```

## Comparing `sumfolder1-0.0.1rc6.tar` & `sumfolder1-0.0.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 ross-spencer  (1000) ross-spencer  (1000)        0 2023-01-16 13:02:55.477026 sumfolder1-0.0.1rc6/
--rw-rw-r--   0 ross-spencer  (1000) ross-spencer  (1000)    35149 2023-01-04 22:32:34.000000 sumfolder1-0.0.1rc6/LICENSE
--rw-rw-r--   0 ross-spencer  (1000) ross-spencer  (1000)    11522 2023-01-16 13:02:55.477026 sumfolder1-0.0.1rc6/PKG-INFO
--rw-rw-r--   0 ross-spencer  (1000) ross-spencer  (1000)    10601 2023-01-16 13:01:48.000000 sumfolder1-0.0.1rc6/README.md
--rw-rw-r--   0 ross-spencer  (1000) ross-spencer  (1000)       98 2023-01-16 12:55:55.000000 sumfolder1-0.0.1rc6/pyproject.toml
--rw-rw-r--   0 ross-spencer  (1000) ross-spencer  (1000)       74 2023-01-16 13:02:55.477026 sumfolder1-0.0.1rc6/setup.cfg
--rw-rw-r--   0 ross-spencer  (1000) ross-spencer  (1000)     1555 2023-01-16 12:55:55.000000 sumfolder1-0.0.1rc6/setup.py
-drwxrwxr-x   0 ross-spencer  (1000) ross-spencer  (1000)        0 2023-01-16 13:02:55.473026 sumfolder1-0.0.1rc6/src/
-drwxrwxr-x   0 ross-spencer  (1000) ross-spencer  (1000)        0 2023-01-16 13:02:55.473026 sumfolder1-0.0.1rc6/src/sumfolder1/
--rw-rw-r--   0 ross-spencer  (1000) ross-spencer  (1000)        0 2023-01-16 12:55:55.000000 sumfolder1-0.0.1rc6/src/sumfolder1/__init__.py
--rw-rw-r--   0 ross-spencer  (1000) ross-spencer  (1000)     3037 2023-01-16 12:55:55.000000 sumfolder1-0.0.1rc6/src/sumfolder1/droidcsvhandler.py
--rw-rw-r--   0 ross-spencer  (1000) ross-spencer  (1000)     6113 2023-01-16 12:55:55.000000 sumfolder1-0.0.1rc6/src/sumfolder1/referenceset.py
--rw-rw-r--   0 ross-spencer  (1000) ross-spencer  (1000)     2477 2023-01-16 12:55:55.000000 sumfolder1-0.0.1rc6/src/sumfolder1/results.py
--rw-rw-r--   0 ross-spencer  (1000) ross-spencer  (1000)     3741 2023-01-16 12:55:55.000000 sumfolder1-0.0.1rc6/src/sumfolder1/storageobjects.py
--rw-rw-r--   0 ross-spencer  (1000) ross-spencer  (1000)     4552 2023-01-16 12:55:55.000000 sumfolder1-0.0.1rc6/src/sumfolder1/sumfolder1.py
--rw-rw-r--   0 ross-spencer  (1000) ross-spencer  (1000)    20466 2023-01-16 12:55:55.000000 sumfolder1-0.0.1rc6/src/sumfolder1/sumfolders.py
--rw-rw-r--   0 ross-spencer  (1000) ross-spencer  (1000)      584 2023-01-16 12:55:55.000000 sumfolder1-0.0.1rc6/src/sumfolder1/utilities.py
--rw-rw-r--   0 ross-spencer  (1000) ross-spencer  (1000)      129 2023-01-16 13:01:48.000000 sumfolder1-0.0.1rc6/src/sumfolder1/version.py
-drwxrwxr-x   0 ross-spencer  (1000) ross-spencer  (1000)        0 2023-01-16 13:02:55.477026 sumfolder1-0.0.1rc6/src/sumfolder1.egg-info/
--rw-rw-r--   0 ross-spencer  (1000) ross-spencer  (1000)    11522 2023-01-16 13:02:55.000000 sumfolder1-0.0.1rc6/src/sumfolder1.egg-info/PKG-INFO
--rw-rw-r--   0 ross-spencer  (1000) ross-spencer  (1000)      544 2023-01-16 13:02:55.000000 sumfolder1-0.0.1rc6/src/sumfolder1.egg-info/SOURCES.txt
--rw-rw-r--   0 ross-spencer  (1000) ross-spencer  (1000)        1 2023-01-16 13:02:55.000000 sumfolder1-0.0.1rc6/src/sumfolder1.egg-info/dependency_links.txt
--rw-rw-r--   0 ross-spencer  (1000) ross-spencer  (1000)       59 2023-01-16 13:02:55.000000 sumfolder1-0.0.1rc6/src/sumfolder1.egg-info/entry_points.txt
--rw-rw-r--   0 ross-spencer  (1000) ross-spencer  (1000)       16 2023-01-16 13:02:55.000000 sumfolder1-0.0.1rc6/src/sumfolder1.egg-info/requires.txt
--rw-rw-r--   0 ross-spencer  (1000) ross-spencer  (1000)       11 2023-01-16 13:02:55.000000 sumfolder1-0.0.1rc6/src/sumfolder1.egg-info/top_level.txt
+drwxrwxr-x   0 ross-spencer  (1000) ross-spencer  (1000)        0 2023-05-21 10:37:07.181141 sumfolder1-0.0.2/
+-rw-rw-r--   0 ross-spencer  (1000) ross-spencer  (1000)    35149 2023-01-04 22:32:34.000000 sumfolder1-0.0.2/LICENSE
+-rw-rw-r--   0 ross-spencer  (1000) ross-spencer  (1000)    11618 2023-05-21 10:37:07.181141 sumfolder1-0.0.2/PKG-INFO
+-rw-rw-r--   0 ross-spencer  (1000) ross-spencer  (1000)    10700 2023-05-21 10:35:33.000000 sumfolder1-0.0.2/README.md
+-rw-rw-r--   0 ross-spencer  (1000) ross-spencer  (1000)       98 2023-01-16 12:55:55.000000 sumfolder1-0.0.2/pyproject.toml
+-rw-rw-r--   0 ross-spencer  (1000) ross-spencer  (1000)       74 2023-05-21 10:37:07.181141 sumfolder1-0.0.2/setup.cfg
+-rw-rw-r--   0 ross-spencer  (1000) ross-spencer  (1000)     1555 2023-01-16 12:55:55.000000 sumfolder1-0.0.2/setup.py
+drwxrwxr-x   0 ross-spencer  (1000) ross-spencer  (1000)        0 2023-05-21 10:37:07.177141 sumfolder1-0.0.2/src/
+drwxrwxr-x   0 ross-spencer  (1000) ross-spencer  (1000)        0 2023-05-21 10:37:07.181141 sumfolder1-0.0.2/src/sumfolder1/
+-rw-rw-r--   0 ross-spencer  (1000) ross-spencer  (1000)        0 2023-01-16 12:55:55.000000 sumfolder1-0.0.2/src/sumfolder1/__init__.py
+-rw-rw-r--   0 ross-spencer  (1000) ross-spencer  (1000)     3037 2023-01-16 12:55:55.000000 sumfolder1-0.0.2/src/sumfolder1/droidcsvhandler.py
+-rw-rw-r--   0 ross-spencer  (1000) ross-spencer  (1000)     6113 2023-01-16 12:55:55.000000 sumfolder1-0.0.2/src/sumfolder1/referenceset.py
+-rw-rw-r--   0 ross-spencer  (1000) ross-spencer  (1000)     2477 2023-01-16 12:55:55.000000 sumfolder1-0.0.2/src/sumfolder1/results.py
+-rw-rw-r--   0 ross-spencer  (1000) ross-spencer  (1000)     3743 2023-05-21 10:35:33.000000 sumfolder1-0.0.2/src/sumfolder1/storageobjects.py
+-rw-rw-r--   0 ross-spencer  (1000) ross-spencer  (1000)     4552 2023-01-16 12:55:55.000000 sumfolder1-0.0.2/src/sumfolder1/sumfolder1.py
+-rw-rw-r--   0 ross-spencer  (1000) ross-spencer  (1000)    20335 2023-05-21 10:35:33.000000 sumfolder1-0.0.2/src/sumfolder1/sumfolders.py
+-rw-rw-r--   0 ross-spencer  (1000) ross-spencer  (1000)      584 2023-05-18 10:16:30.000000 sumfolder1-0.0.2/src/sumfolder1/utilities.py
+-rw-rw-r--   0 ross-spencer  (1000) ross-spencer  (1000)      125 2023-05-21 10:35:33.000000 sumfolder1-0.0.2/src/sumfolder1/version.py
+drwxrwxr-x   0 ross-spencer  (1000) ross-spencer  (1000)        0 2023-05-21 10:37:07.181141 sumfolder1-0.0.2/src/sumfolder1.egg-info/
+-rw-rw-r--   0 ross-spencer  (1000) ross-spencer  (1000)    11618 2023-05-21 10:37:07.000000 sumfolder1-0.0.2/src/sumfolder1.egg-info/PKG-INFO
+-rw-rw-r--   0 ross-spencer  (1000) ross-spencer  (1000)      544 2023-05-21 10:37:07.000000 sumfolder1-0.0.2/src/sumfolder1.egg-info/SOURCES.txt
+-rw-rw-r--   0 ross-spencer  (1000) ross-spencer  (1000)        1 2023-05-21 10:37:07.000000 sumfolder1-0.0.2/src/sumfolder1.egg-info/dependency_links.txt
+-rw-rw-r--   0 ross-spencer  (1000) ross-spencer  (1000)       59 2023-05-21 10:37:07.000000 sumfolder1-0.0.2/src/sumfolder1.egg-info/entry_points.txt
+-rw-rw-r--   0 ross-spencer  (1000) ross-spencer  (1000)       16 2023-05-21 10:37:07.000000 sumfolder1-0.0.2/src/sumfolder1.egg-info/requires.txt
+-rw-rw-r--   0 ross-spencer  (1000) ross-spencer  (1000)       11 2023-05-21 10:37:07.000000 sumfolder1-0.0.2/src/sumfolder1.egg-info/top_level.txt
```

### Comparing `sumfolder1-0.0.1rc6/LICENSE` & `sumfolder1-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sumfolder1-0.0.1rc6/PKG-INFO` & `sumfolder1-0.0.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sumfolder1
-Version: 0.0.1rc6
+Version: 0.0.2
 Summary: Checksums for folders.
 Home-page: https://github.com/ross-spencer/sumfolder1
 Author: Ross Spencer
 Author-email: all.along.the.watchtower2001+github@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/ross-spencer/sumfolder1/issues
 Project-URL: Source, https://github.com/ross-spencer/sumfolder1
@@ -22,46 +22,47 @@
 License-File: LICENSE
 
 <p align="center">
   <img
    width="786"
    height="204"
    alt="Logo for sumfolder1"
-   src="https://github.com/ross-spencer/sumfolder1/blob/7bca71d8f944ffd55424307523f84b962bc74a89/logo/sumfolder1.png">
+   src="https://raw.githubusercontent.com/ross-spencer/sumfolder1/main/logo/sumfolder1.png">
 </p>
 
 sumfolder1 is a utility for use within the archival and digital preservation
-community to generate checksums for file directories, and to generate
+community to generate checksums for file system directories, and to generate
 an overall "collection" checksum for a given set of files.
 
-- [Why?](#why-)
+* [Why?](#why)
   * [Archival questions](#archival-questions)
   * [Structural questions](#structural-questions)
   * [Forensics questions](#forensics-questions)
-- [How?](#how-)
+* [How?](#how)
   * [Reference set](#reference-set)
   * [Reference implementation](#reference-implementation)
   * [Merkle trees](#merkle-trees)
   * [Terminology](#terminology)
   * [New folder attributes](#new-folder-attributes)
   * [Sensitivity](#sensitivity)
-- [DROID](#droid)
+* [DROID](#droid)
   * [DROID in Siegfried](#droid-in-siegfried)
   * [DROID as an inspiration](#droid-as-an-inspiration)
-- [Installation](#installation)
-- [Usage](#usage)
+  * [Writing about sumfolder1](#writing-about-sumfolder1)
+* [Installation](#installation)
+* [Usage](#usage)
   * [Demo output](#demo-output)
   * [Use with a DROID csv](#use-with-a-droid-csv)
   * [Outputting the reference CSV](#outputting-the-reference-csv)
-- [License](#license)
+* [License](#license)
 
 ## Why?
 
-Conventionally, checksums exist for files, they do not exist for directories. They have
-no payload that can be summed together to calculate a digest/checksum.
+Conventionally, checksums exist for files, they do not exist for directories.
+They have no payload that can be summed together to calculate a digest/checksum.
 
 If it were possible to create checksums for folders or a global checksum for a
 collection of objects, it would become possible to ask the following:
 
 ### Archival questions
 
 * What is the collection checksum for a given set of files and folders?
@@ -106,15 +107,15 @@
 
 We can iterate through the directory tree to create sets of directory checksums
 and a collection checksum: `52b94608dc70813aa88dae01176dc73b`.
 
 The reference set then looks as follows:
 
 ```text
-📁 collection 52b94608dc70813aa88dae01176dc73b
+📁 collection 93778c524035d5d3e429a2fe43b7700a
    📄 file_0001 14118ff9ad0344decb37960809b2f17a
    📄 file_0000 8cfda2609b880a553759cd6200823f3b
    📄 file_0002 a4501ee1a5c711ea9db78a800a24e830
    📁 sub_dir_1 82301616d7e24f474dbe21de93af0a34
       📄 file_empty d41d8cd98f00b204e9800998ecf8427e
       📄 file_0003 dc7f828c5fe622925181d06edada350f
       📄 file_0004 e3d90a4bf14a9b355f0e69ba08df522d
@@ -130,35 +131,32 @@
       📄 file_0008 fdffe4dd2d39c7d9986dbf5c6ec5ad39
    📁 sub_dir_5 d818d29b75f89a9b5d8d1c5a4c70dbbb
       📁 sub_5_dir_1 82f9e9a4305714fffdd7932783980cbc
          📄 file_0009 7c1f9f9a4d0ce9a72ee63f37a1b7f694
          📄 file_0010 aececec0bc3f515039aec9e60c413cd3
    📁 sub_dir_6 74be16979710d4c4e7c6647856088456
       📄 file_empty d41d8cd98f00b204e9800998ecf8427e
+
 ```
 
 ### Reference implementation
 
-The reference implementation for sumfolder1 does the followsing:
-
-1. Order the set alphabetically by file path.
-1. Give each folder in order an increasing value: sort order.
-1. Order the set in reverse sort order.
+The reference implementation for sumfolder1 does the following:
 
 From the lowest sub-directory in the tree:
 
-1. Check for sub-directories and add these to a hash digest (in reverse sort
-order).
-1. For files in the directory add these to a hash digest in alphabetical order
+1. Check for sub-directories and add the checksums for these to a hash digest in
+alphabetical order by checksum.
+1. For files in the directory add these to the hash digest in alphabetical order
 by checksum.
 1. Create a digest for the list of checksums.
 
 Repeat, processing each folder backwards up to the top level.
 
-> NB. If the folder is completely empty it is assigned a constant value
+> NB. If a folder is completely empty it is assigned a constant value
 chosen in the code: `2600_EMPTY_DIRECTORY`. This evaluates to an MD5 value of
 `1ccb49edc4e873f1a8affd4bad5e9b90`.
 
 ### Merkle trees
 
 The concept I have used here is based on Merkle trees and a loose understanding
 of techniques used in the block-chain and in the source control system GitHub.
@@ -170,17 +168,18 @@
 And a Python tutorial I found useful in starting this work:
 
 * [Dan Nolan on Merkle Trees][merkle-2]
 
 The technique required for a directory tree is a little more convoluted than
 that of a Merkle tree which uses binary nodes and evaluates checksums from left
 to right. I believe the implementation used for sumfolder1 is more closely
-aligned to that of a "Radix Tree" or "Patricia Tree", however, this is to be explored more.
+aligned to that of a "Radix Tree" or "Patricia Tree", however, this is to be
+explored more.
 
-> NB. A merkle tree is partially used for performance, however, sumfolder1 does
+> NB. A merkle tree can be used in its context for performance; sumfolder1 does
 not yet have a performance use-case.
 
 ### Terminology
 
 The reference implementation introduces some terminology that helps with
 understanding the approach:
 
@@ -194,34 +193,35 @@
 
 ### New folder attributes
 
 Folder objects need to be given additional attributes to enable the algorithm
 to work.
 
 * Folder-depth, so directories can be grouped and distinguished from
-one-another.
-* Sort_order, so they can be consistently recalculated.
+one-another by level in the hierarchy.
 * Hash, the goal of this tool is to enable a hash to be calculated for
 an entire collection.
 
 ### Sensitivity
 
-The code is sensitive to small changes. If checksums are calculated in different orders the results will be different. To elaborate on the algorithm above, this
-is controlled by:
-
-1. Creating a sort order for directories. This needs only be contiguous
-from the root node (Rn): so Rn == 0, folder1 = 1, folder2 = 3, and so
-on. Sub directory checksums are then calculated by ordering the folders
-in the sub-directory in reverse sort order, and then adding the hashes
-together.
-
-2. Files already have checksums. These checksums need to be ordered
-alphanumerically in order, 0, 1, 2, 3, a, b, c, etc.
+I am trying to make this code as portable as possible, i.e. while it works with
+DROID-style reports today, it might also work with other checksum-based outputs
+tomorrow. Additionally, to be able to compare folder structures, this utility
+may also work with DROID-style reports later on in a transfer workflow; at which
+point, folders and files may have been renamed, but their content remains
+consistent.
+
+To calculate a single folder checksum we currently do the following:
+
+* If there are folders in the directory, order their hashes alphabetically
+and add to a list.
+* File checksums are then ordered alphabetically and added to the end of the
+list.
+* The checksums are then summed together to create a new folder-level checksum.
 
-Then, no-matter the shape of the file-format identification report used, the tool should work to enable verification of the files in a given set.
 ## DROID
 
 sumfolder1 uses the DROID format identification report to generate folder level
 checksums.
 
 DROID can be found at The National Archives UK website:
 
@@ -235,27 +235,36 @@
 ```bash
 sf --hash=md5 --droid <collection_folder>
 ```
 
 ### DROID as an inspiration
 
 File format reports provide a means of statically analyzing collections of
-digital objects. A DROID report satisfies the pre-conditions required to create reliable folder- and collection-level checksums for digital collections:
+digital objects. A DROID report satisfies the pre-conditions required to create
+reliable folder- and collection-level checksums for digital collections:
 
 * A collection is static, i.e. unlikely to change.
 * Digital objects within the collection have checksums.
 
 > NB: A collection need not be static to be analyzed but it is not the primary
 use-case of this utility.
 
 More information about the different uses for a file-format identification
 report can be found in my paper in the Code4Lib journal.
 
 * [Fractal in detail: What information is in a file format identification report?][code4lib-1]
 
+### Writing about sumfolder1
+
+I wrote a blog describing the utility on the OPF website.
+
+* [What is the checksum of a directory?][opf-1]
+
+[opf-1]: https://openpreservation.org/blogs/what-is-the-checksum-of-a-directory/?q=1
+
 ## Installation
 
 sumfolder1 is available on pypi and can be installed as follows:
 
 ```bash
 pip install -U sumfolder1
 ```
@@ -263,15 +272,16 @@
 ## Usage
 
 sumfolder1 has the following usage instructions:
 
 ```text
 usage: sumfolder1.py [-h] [--csv CSV] [--demo] [--ref] [-v]
 
-Calculate checksums for folders in a collection of objects using a DROID format identification report
+Calculate checksums for folders in a collection of objects using a DROID format
+identification report
 
 options:
   -h, --help          show this help message and exit
   --csv CSV           Single DROID CSV to read.
   --demo              Run demo queries and output a tree to demo.txt
   --ref, --reference  Write reference set to stdout.
   -v, --version       Return version information.
@@ -297,15 +307,16 @@
 
 ```bash
 python sumfolder1 --csv <droid_csv_file>
 ```
 
 ### Outputting the reference CSV
 
-A reference CSV can be output to `stdout`. Ideally it is piped to some other  file using a command such as follows:
+A reference CSV can be output to `stdout`. Ideally it is piped to some other
+file using a command such as follows:
 
 ```bash
 python sumfolder1 --ref > <output_file>
 ```
 
 ## License
```

### Comparing `sumfolder1-0.0.1rc6/README.md` & `sumfolder1-0.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 <p align="center">
   <img
    width="786"
    height="204"
    alt="Logo for sumfolder1"
-   src="https://github.com/ross-spencer/sumfolder1/blob/7bca71d8f944ffd55424307523f84b962bc74a89/logo/sumfolder1.png">
+   src="https://raw.githubusercontent.com/ross-spencer/sumfolder1/main/logo/sumfolder1.png">
 </p>
 
 sumfolder1 is a utility for use within the archival and digital preservation
-community to generate checksums for file directories, and to generate
+community to generate checksums for file system directories, and to generate
 an overall "collection" checksum for a given set of files.
 
-- [Why?](#why-)
+* [Why?](#why)
   * [Archival questions](#archival-questions)
   * [Structural questions](#structural-questions)
   * [Forensics questions](#forensics-questions)
-- [How?](#how-)
+* [How?](#how)
   * [Reference set](#reference-set)
   * [Reference implementation](#reference-implementation)
   * [Merkle trees](#merkle-trees)
   * [Terminology](#terminology)
   * [New folder attributes](#new-folder-attributes)
   * [Sensitivity](#sensitivity)
-- [DROID](#droid)
+* [DROID](#droid)
   * [DROID in Siegfried](#droid-in-siegfried)
   * [DROID as an inspiration](#droid-as-an-inspiration)
-- [Installation](#installation)
-- [Usage](#usage)
+  * [Writing about sumfolder1](#writing-about-sumfolder1)
+* [Installation](#installation)
+* [Usage](#usage)
   * [Demo output](#demo-output)
   * [Use with a DROID csv](#use-with-a-droid-csv)
   * [Outputting the reference CSV](#outputting-the-reference-csv)
-- [License](#license)
+* [License](#license)
 
 ## Why?
 
-Conventionally, checksums exist for files, they do not exist for directories. They have
-no payload that can be summed together to calculate a digest/checksum.
+Conventionally, checksums exist for files, they do not exist for directories.
+They have no payload that can be summed together to calculate a digest/checksum.
 
 If it were possible to create checksums for folders or a global checksum for a
 collection of objects, it would become possible to ask the following:
 
 ### Archival questions
 
 * What is the collection checksum for a given set of files and folders?
@@ -83,15 +84,15 @@
 
 We can iterate through the directory tree to create sets of directory checksums
 and a collection checksum: `52b94608dc70813aa88dae01176dc73b`.
 
 The reference set then looks as follows:
 
 ```text
-📁 collection 52b94608dc70813aa88dae01176dc73b
+📁 collection 93778c524035d5d3e429a2fe43b7700a
    📄 file_0001 14118ff9ad0344decb37960809b2f17a
    📄 file_0000 8cfda2609b880a553759cd6200823f3b
    📄 file_0002 a4501ee1a5c711ea9db78a800a24e830
    📁 sub_dir_1 82301616d7e24f474dbe21de93af0a34
       📄 file_empty d41d8cd98f00b204e9800998ecf8427e
       📄 file_0003 dc7f828c5fe622925181d06edada350f
       📄 file_0004 e3d90a4bf14a9b355f0e69ba08df522d
@@ -107,35 +108,32 @@
       📄 file_0008 fdffe4dd2d39c7d9986dbf5c6ec5ad39
    📁 sub_dir_5 d818d29b75f89a9b5d8d1c5a4c70dbbb
       📁 sub_5_dir_1 82f9e9a4305714fffdd7932783980cbc
          📄 file_0009 7c1f9f9a4d0ce9a72ee63f37a1b7f694
          📄 file_0010 aececec0bc3f515039aec9e60c413cd3
    📁 sub_dir_6 74be16979710d4c4e7c6647856088456
       📄 file_empty d41d8cd98f00b204e9800998ecf8427e
+
 ```
 
 ### Reference implementation
 
-The reference implementation for sumfolder1 does the followsing:
-
-1. Order the set alphabetically by file path.
-1. Give each folder in order an increasing value: sort order.
-1. Order the set in reverse sort order.
+The reference implementation for sumfolder1 does the following:
 
 From the lowest sub-directory in the tree:
 
-1. Check for sub-directories and add these to a hash digest (in reverse sort
-order).
-1. For files in the directory add these to a hash digest in alphabetical order
+1. Check for sub-directories and add the checksums for these to a hash digest in
+alphabetical order by checksum.
+1. For files in the directory add these to the hash digest in alphabetical order
 by checksum.
 1. Create a digest for the list of checksums.
 
 Repeat, processing each folder backwards up to the top level.
 
-> NB. If the folder is completely empty it is assigned a constant value
+> NB. If a folder is completely empty it is assigned a constant value
 chosen in the code: `2600_EMPTY_DIRECTORY`. This evaluates to an MD5 value of
 `1ccb49edc4e873f1a8affd4bad5e9b90`.
 
 ### Merkle trees
 
 The concept I have used here is based on Merkle trees and a loose understanding
 of techniques used in the block-chain and in the source control system GitHub.
@@ -147,17 +145,18 @@
 And a Python tutorial I found useful in starting this work:
 
 * [Dan Nolan on Merkle Trees][merkle-2]
 
 The technique required for a directory tree is a little more convoluted than
 that of a Merkle tree which uses binary nodes and evaluates checksums from left
 to right. I believe the implementation used for sumfolder1 is more closely
-aligned to that of a "Radix Tree" or "Patricia Tree", however, this is to be explored more.
+aligned to that of a "Radix Tree" or "Patricia Tree", however, this is to be
+explored more.
 
-> NB. A merkle tree is partially used for performance, however, sumfolder1 does
+> NB. A merkle tree can be used in its context for performance; sumfolder1 does
 not yet have a performance use-case.
 
 ### Terminology
 
 The reference implementation introduces some terminology that helps with
 understanding the approach:
 
@@ -171,34 +170,35 @@
 
 ### New folder attributes
 
 Folder objects need to be given additional attributes to enable the algorithm
 to work.
 
 * Folder-depth, so directories can be grouped and distinguished from
-one-another.
-* Sort_order, so they can be consistently recalculated.
+one-another by level in the hierarchy.
 * Hash, the goal of this tool is to enable a hash to be calculated for
 an entire collection.
 
 ### Sensitivity
 
-The code is sensitive to small changes. If checksums are calculated in different orders the results will be different. To elaborate on the algorithm above, this
-is controlled by:
-
-1. Creating a sort order for directories. This needs only be contiguous
-from the root node (Rn): so Rn == 0, folder1 = 1, folder2 = 3, and so
-on. Sub directory checksums are then calculated by ordering the folders
-in the sub-directory in reverse sort order, and then adding the hashes
-together.
-
-2. Files already have checksums. These checksums need to be ordered
-alphanumerically in order, 0, 1, 2, 3, a, b, c, etc.
+I am trying to make this code as portable as possible, i.e. while it works with
+DROID-style reports today, it might also work with other checksum-based outputs
+tomorrow. Additionally, to be able to compare folder structures, this utility
+may also work with DROID-style reports later on in a transfer workflow; at which
+point, folders and files may have been renamed, but their content remains
+consistent.
+
+To calculate a single folder checksum we currently do the following:
+
+* If there are folders in the directory, order their hashes alphabetically
+and add to a list.
+* File checksums are then ordered alphabetically and added to the end of the
+list.
+* The checksums are then summed together to create a new folder-level checksum.
 
-Then, no-matter the shape of the file-format identification report used, the tool should work to enable verification of the files in a given set.
 ## DROID
 
 sumfolder1 uses the DROID format identification report to generate folder level
 checksums.
 
 DROID can be found at The National Archives UK website:
 
@@ -212,27 +212,36 @@
 ```bash
 sf --hash=md5 --droid <collection_folder>
 ```
 
 ### DROID as an inspiration
 
 File format reports provide a means of statically analyzing collections of
-digital objects. A DROID report satisfies the pre-conditions required to create reliable folder- and collection-level checksums for digital collections:
+digital objects. A DROID report satisfies the pre-conditions required to create
+reliable folder- and collection-level checksums for digital collections:
 
 * A collection is static, i.e. unlikely to change.
 * Digital objects within the collection have checksums.
 
 > NB: A collection need not be static to be analyzed but it is not the primary
 use-case of this utility.
 
 More information about the different uses for a file-format identification
 report can be found in my paper in the Code4Lib journal.
 
 * [Fractal in detail: What information is in a file format identification report?][code4lib-1]
 
+### Writing about sumfolder1
+
+I wrote a blog describing the utility on the OPF website.
+
+* [What is the checksum of a directory?][opf-1]
+
+[opf-1]: https://openpreservation.org/blogs/what-is-the-checksum-of-a-directory/?q=1
+
 ## Installation
 
 sumfolder1 is available on pypi and can be installed as follows:
 
 ```bash
 pip install -U sumfolder1
 ```
@@ -240,15 +249,16 @@
 ## Usage
 
 sumfolder1 has the following usage instructions:
 
 ```text
 usage: sumfolder1.py [-h] [--csv CSV] [--demo] [--ref] [-v]
 
-Calculate checksums for folders in a collection of objects using a DROID format identification report
+Calculate checksums for folders in a collection of objects using a DROID format
+identification report
 
 options:
   -h, --help          show this help message and exit
   --csv CSV           Single DROID CSV to read.
   --demo              Run demo queries and output a tree to demo.txt
   --ref, --reference  Write reference set to stdout.
   -v, --version       Return version information.
@@ -274,15 +284,16 @@
 
 ```bash
 python sumfolder1 --csv <droid_csv_file>
 ```
 
 ### Outputting the reference CSV
 
-A reference CSV can be output to `stdout`. Ideally it is piped to some other  file using a command such as follows:
+A reference CSV can be output to `stdout`. Ideally it is piped to some other
+file using a command such as follows:
 
 ```bash
 python sumfolder1 --ref > <output_file>
 ```
 
 ## License
```

### Comparing `sumfolder1-0.0.1rc6/setup.py` & `sumfolder1-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `sumfolder1-0.0.1rc6/src/sumfolder1/droidcsvhandler.py` & `sumfolder1-0.0.2/src/sumfolder1/droidcsvhandler.py`

 * *Files identical despite different names*

### Comparing `sumfolder1-0.0.1rc6/src/sumfolder1/referenceset.py` & `sumfolder1-0.0.2/src/sumfolder1/referenceset.py`

 * *Files identical despite different names*

### Comparing `sumfolder1-0.0.1rc6/src/sumfolder1/results.py` & `sumfolder1-0.0.2/src/sumfolder1/results.py`

 * *Files identical despite different names*

### Comparing `sumfolder1-0.0.1rc6/src/sumfolder1/storageobjects.py` & `sumfolder1-0.0.2/src/sumfolder1/storageobjects.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,17 +16,14 @@
     is_root: bool = False
     depth: int = None
     sub_dirs: list = field(default_factory=list)
     files: list = field(default_factory=list)
     hash_of_files: str = None
     hash_: str = None
 
-    # Order for sorting directories across the tree.
-    sort_order: int = None
-
     # Non-functional, tree-view helper.
     displayed: bool = False
 
     EMPTY_DIR: Final[str] = b"2600_EMPTY_DIRECTORY"  # pylint: disable=C0103
 
     def __repr__(self):
         """Create a string representation of this object."""
@@ -49,22 +46,23 @@
     def _hash_empty_directory(self, digest):
         """Return a hash for a completely empty directory."""
         digest.update(self.EMPTY_DIR)
         self.hash_ = digest.hexdigest()
 
     @staticmethod
     def _sort_directories(folders):
-        """Sort directories by their `sort_order` attribute in reverse
-        order.
+        """Sort directories by their hash values providing they have
+        been calculated.
 
-        While reverse sort-order, to this author, better mimics a
-        virtual vertical view of the tree, this could be the opposite
-        of reverse order too. (I believe.)
+        NB. Hashes are a natural value to sort here. Previously a
+        mechanic existed to generate a sort order, but this makes the
+        heuristic less portable. Sorting by hash values (once
+        calculated) makes this utility truly content based.
         """
-        return _sort_obj_list(folders, "sort_order", True)
+        return _sort_obj_list(folders, "hash_", False)
 
     def hash_folders(self, hash_func) -> str:
         """Generate a single hash for folders."""
         digest = None
         digest = _get_hash_obj(hash_func)
         if not self.sub_dirs and not self.files:
             # There are no sub directories and no files. We have a
```

### Comparing `sumfolder1-0.0.1rc6/src/sumfolder1/sumfolder1.py` & `sumfolder1-0.0.2/src/sumfolder1/sumfolder1.py`

 * *Files identical despite different names*

### Comparing `sumfolder1-0.0.1rc6/src/sumfolder1/sumfolders.py` & `sumfolder1-0.0.2/src/sumfolder1/sumfolders.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """Identify contents of folders and sub-folders and output hashes for
 what we discover.
 """
 
 import logging
 import os
-from operator import itemgetter
 from pathlib import PureWindowsPath
 from typing import Final, Union
 
 from colorama import Fore, Style
 from colorama import init as colorama_init
 
 from .droidcsvhandler import DROIDCSVHandler
@@ -101,34 +100,28 @@
     @staticmethod
     def _create_root(min_depth: int) -> Folder:
         """Create a root folder for this collection."""
         root = Folder()
         root.depth = min_depth - 1
         root.is_root = True
         root.path = PureWindowsPath("/merkle_collection_root")
-        root.sort_order = 0
         return root
 
     def generate_lists(
         self, droid_list: list[dict], csv_hash: str, make_root_node: bool = False
     ) -> Union[list[Folder], list[File]]:
         """Extract information about our folders and files and some of
         their relationships.
         """
         folders = []
         files = []
         min_depth = 1000
         override_root = False
 
-        # Paths need to be sorted to be consistent across DROID and
-        # Siegfried. Both output their results slightly differently
-        # from one another.
-        sorted_paths = sorted(droid_list, key=itemgetter("FILE_PATH"))
-
-        for idx, row in enumerate(sorted_paths, 1):
+        for idx, row in enumerate(droid_list, 1):
             path = PureWindowsPath(row["FILE_PATH"])
             type_ = row["TYPE"]
             hash_ = row[csv_hash]
             root = False
             # A root node (Rn) that sits above all other folders and
             # files needs to exist to provide a collection hash. This
             # ideally comes from the report and is identified currently
@@ -145,18 +138,14 @@
                     self.given_root = True
             if type_ == "Folder":
                 folder = Folder()
                 folder.path = path
                 folder.is_root = root
                 folder.depth = len(path.parts)
                 min_depth = min(folder.depth, min_depth)
-                # Add sort order...
-                folder.sort_order = idx
-                if root:
-                    folder.sort_order = 0
                 folders.append(folder)
             elif type_ in ("File", "Container"):
                 file = File()
                 file.path = path
                 file.name = path.name
                 file.hash_ = hash_
                 try:
@@ -415,20 +404,23 @@
             folder_depths = []
             for folder in folders:
                 if folder.depth == root_group:
                     continue
                 folder_depths.append(folder.depth)
             require = min(folder_depths)
             logging.info("Rn+1 depth: %s (out of: %s)", require, folder_depths)
-            # Sort the folders for eventual hashing using sort_order.
-            folders = _sort_obj_list(folders, "sort_order", True)
             # Root node hashes minus 1 (H1).
             rn_m1_hashes = [
                 folder.hash_ for folder in folders if folder.depth == require
             ]
+            # Sort checksums alphabetically so that they are consistently
+            # added together, i.e. this ensures that they are added by content
+            # and no additional data needs adding to the objects, e.g. such
+            # as sort order in a previous version of this code.
+            rn_m1_hashes.sort()
             # Active-tree (H2).
             active_tree_folders = self.get_active_tree(match, folders)
             active_tree_hashes = [folder.hash_ for folder in active_tree_folders]
             logging.info("Rn+1 hashes: %s", rn_m1_hashes)
             logging.info("Identified active-tree: %s", active_tree_hashes)
             if search_hash in root_files:
                 digest = _get_hash_obj(self.hash_func)
@@ -462,15 +454,17 @@
             # match the previously calculated Rn.
             all_hashes = rn_m1_hashes + root_files
             logging.info("Recalculating with all hashes %s", all_hashes)
             final_compute = _get_hash_obj(self.hash_func)
             for hashes in all_hashes:
                 final_compute.update(hashes.encode())
             final_computed = final_compute.hexdigest()
-            assert final_computed == self.root_folder_hash
+            assert (
+                final_computed == self.root_folder_hash
+            ), f"final_computed: ({final_computed}) doesn't equal expected: ({self.root_folder_hash})"
             assert self.root_folder_hash in active_tree_hashes
             try:
                 active_tree_hashes.remove(search_hash)
             except ValueError:
                 pass
             for hashes in active_tree_hashes:
                 hash_result.containing_dirs.append(hashes)
```

### Comparing `sumfolder1-0.0.1rc6/src/sumfolder1/utilities.py` & `sumfolder1-0.0.2/src/sumfolder1/utilities.py`

 * *Files identical despite different names*

### Comparing `sumfolder1-0.0.1rc6/src/sumfolder1.egg-info/PKG-INFO` & `sumfolder1-0.0.2/src/sumfolder1.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sumfolder1
-Version: 0.0.1rc6
+Version: 0.0.2
 Summary: Checksums for folders.
 Home-page: https://github.com/ross-spencer/sumfolder1
 Author: Ross Spencer
 Author-email: all.along.the.watchtower2001+github@gmail.com
 License: UNKNOWN
 Project-URL: Bug Reports, https://github.com/ross-spencer/sumfolder1/issues
 Project-URL: Source, https://github.com/ross-spencer/sumfolder1
@@ -22,46 +22,47 @@
 License-File: LICENSE
 
 <p align="center">
   <img
    width="786"
    height="204"
    alt="Logo for sumfolder1"
-   src="https://github.com/ross-spencer/sumfolder1/blob/7bca71d8f944ffd55424307523f84b962bc74a89/logo/sumfolder1.png">
+   src="https://raw.githubusercontent.com/ross-spencer/sumfolder1/main/logo/sumfolder1.png">
 </p>
 
 sumfolder1 is a utility for use within the archival and digital preservation
-community to generate checksums for file directories, and to generate
+community to generate checksums for file system directories, and to generate
 an overall "collection" checksum for a given set of files.
 
-- [Why?](#why-)
+* [Why?](#why)
   * [Archival questions](#archival-questions)
   * [Structural questions](#structural-questions)
   * [Forensics questions](#forensics-questions)
-- [How?](#how-)
+* [How?](#how)
   * [Reference set](#reference-set)
   * [Reference implementation](#reference-implementation)
   * [Merkle trees](#merkle-trees)
   * [Terminology](#terminology)
   * [New folder attributes](#new-folder-attributes)
   * [Sensitivity](#sensitivity)
-- [DROID](#droid)
+* [DROID](#droid)
   * [DROID in Siegfried](#droid-in-siegfried)
   * [DROID as an inspiration](#droid-as-an-inspiration)
-- [Installation](#installation)
-- [Usage](#usage)
+  * [Writing about sumfolder1](#writing-about-sumfolder1)
+* [Installation](#installation)
+* [Usage](#usage)
   * [Demo output](#demo-output)
   * [Use with a DROID csv](#use-with-a-droid-csv)
   * [Outputting the reference CSV](#outputting-the-reference-csv)
-- [License](#license)
+* [License](#license)
 
 ## Why?
 
-Conventionally, checksums exist for files, they do not exist for directories. They have
-no payload that can be summed together to calculate a digest/checksum.
+Conventionally, checksums exist for files, they do not exist for directories.
+They have no payload that can be summed together to calculate a digest/checksum.
 
 If it were possible to create checksums for folders or a global checksum for a
 collection of objects, it would become possible to ask the following:
 
 ### Archival questions
 
 * What is the collection checksum for a given set of files and folders?
@@ -106,15 +107,15 @@
 
 We can iterate through the directory tree to create sets of directory checksums
 and a collection checksum: `52b94608dc70813aa88dae01176dc73b`.
 
 The reference set then looks as follows:
 
 ```text
-📁 collection 52b94608dc70813aa88dae01176dc73b
+📁 collection 93778c524035d5d3e429a2fe43b7700a
    📄 file_0001 14118ff9ad0344decb37960809b2f17a
    📄 file_0000 8cfda2609b880a553759cd6200823f3b
    📄 file_0002 a4501ee1a5c711ea9db78a800a24e830
    📁 sub_dir_1 82301616d7e24f474dbe21de93af0a34
       📄 file_empty d41d8cd98f00b204e9800998ecf8427e
       📄 file_0003 dc7f828c5fe622925181d06edada350f
       📄 file_0004 e3d90a4bf14a9b355f0e69ba08df522d
@@ -130,35 +131,32 @@
       📄 file_0008 fdffe4dd2d39c7d9986dbf5c6ec5ad39
    📁 sub_dir_5 d818d29b75f89a9b5d8d1c5a4c70dbbb
       📁 sub_5_dir_1 82f9e9a4305714fffdd7932783980cbc
          📄 file_0009 7c1f9f9a4d0ce9a72ee63f37a1b7f694
          📄 file_0010 aececec0bc3f515039aec9e60c413cd3
    📁 sub_dir_6 74be16979710d4c4e7c6647856088456
       📄 file_empty d41d8cd98f00b204e9800998ecf8427e
+
 ```
 
 ### Reference implementation
 
-The reference implementation for sumfolder1 does the followsing:
-
-1. Order the set alphabetically by file path.
-1. Give each folder in order an increasing value: sort order.
-1. Order the set in reverse sort order.
+The reference implementation for sumfolder1 does the following:
 
 From the lowest sub-directory in the tree:
 
-1. Check for sub-directories and add these to a hash digest (in reverse sort
-order).
-1. For files in the directory add these to a hash digest in alphabetical order
+1. Check for sub-directories and add the checksums for these to a hash digest in
+alphabetical order by checksum.
+1. For files in the directory add these to the hash digest in alphabetical order
 by checksum.
 1. Create a digest for the list of checksums.
 
 Repeat, processing each folder backwards up to the top level.
 
-> NB. If the folder is completely empty it is assigned a constant value
+> NB. If a folder is completely empty it is assigned a constant value
 chosen in the code: `2600_EMPTY_DIRECTORY`. This evaluates to an MD5 value of
 `1ccb49edc4e873f1a8affd4bad5e9b90`.
 
 ### Merkle trees
 
 The concept I have used here is based on Merkle trees and a loose understanding
 of techniques used in the block-chain and in the source control system GitHub.
@@ -170,17 +168,18 @@
 And a Python tutorial I found useful in starting this work:
 
 * [Dan Nolan on Merkle Trees][merkle-2]
 
 The technique required for a directory tree is a little more convoluted than
 that of a Merkle tree which uses binary nodes and evaluates checksums from left
 to right. I believe the implementation used for sumfolder1 is more closely
-aligned to that of a "Radix Tree" or "Patricia Tree", however, this is to be explored more.
+aligned to that of a "Radix Tree" or "Patricia Tree", however, this is to be
+explored more.
 
-> NB. A merkle tree is partially used for performance, however, sumfolder1 does
+> NB. A merkle tree can be used in its context for performance; sumfolder1 does
 not yet have a performance use-case.
 
 ### Terminology
 
 The reference implementation introduces some terminology that helps with
 understanding the approach:
 
@@ -194,34 +193,35 @@
 
 ### New folder attributes
 
 Folder objects need to be given additional attributes to enable the algorithm
 to work.
 
 * Folder-depth, so directories can be grouped and distinguished from
-one-another.
-* Sort_order, so they can be consistently recalculated.
+one-another by level in the hierarchy.
 * Hash, the goal of this tool is to enable a hash to be calculated for
 an entire collection.
 
 ### Sensitivity
 
-The code is sensitive to small changes. If checksums are calculated in different orders the results will be different. To elaborate on the algorithm above, this
-is controlled by:
-
-1. Creating a sort order for directories. This needs only be contiguous
-from the root node (Rn): so Rn == 0, folder1 = 1, folder2 = 3, and so
-on. Sub directory checksums are then calculated by ordering the folders
-in the sub-directory in reverse sort order, and then adding the hashes
-together.
-
-2. Files already have checksums. These checksums need to be ordered
-alphanumerically in order, 0, 1, 2, 3, a, b, c, etc.
+I am trying to make this code as portable as possible, i.e. while it works with
+DROID-style reports today, it might also work with other checksum-based outputs
+tomorrow. Additionally, to be able to compare folder structures, this utility
+may also work with DROID-style reports later on in a transfer workflow; at which
+point, folders and files may have been renamed, but their content remains
+consistent.
+
+To calculate a single folder checksum we currently do the following:
+
+* If there are folders in the directory, order their hashes alphabetically
+and add to a list.
+* File checksums are then ordered alphabetically and added to the end of the
+list.
+* The checksums are then summed together to create a new folder-level checksum.
 
-Then, no-matter the shape of the file-format identification report used, the tool should work to enable verification of the files in a given set.
 ## DROID
 
 sumfolder1 uses the DROID format identification report to generate folder level
 checksums.
 
 DROID can be found at The National Archives UK website:
 
@@ -235,27 +235,36 @@
 ```bash
 sf --hash=md5 --droid <collection_folder>
 ```
 
 ### DROID as an inspiration
 
 File format reports provide a means of statically analyzing collections of
-digital objects. A DROID report satisfies the pre-conditions required to create reliable folder- and collection-level checksums for digital collections:
+digital objects. A DROID report satisfies the pre-conditions required to create
+reliable folder- and collection-level checksums for digital collections:
 
 * A collection is static, i.e. unlikely to change.
 * Digital objects within the collection have checksums.
 
 > NB: A collection need not be static to be analyzed but it is not the primary
 use-case of this utility.
 
 More information about the different uses for a file-format identification
 report can be found in my paper in the Code4Lib journal.
 
 * [Fractal in detail: What information is in a file format identification report?][code4lib-1]
 
+### Writing about sumfolder1
+
+I wrote a blog describing the utility on the OPF website.
+
+* [What is the checksum of a directory?][opf-1]
+
+[opf-1]: https://openpreservation.org/blogs/what-is-the-checksum-of-a-directory/?q=1
+
 ## Installation
 
 sumfolder1 is available on pypi and can be installed as follows:
 
 ```bash
 pip install -U sumfolder1
 ```
@@ -263,15 +272,16 @@
 ## Usage
 
 sumfolder1 has the following usage instructions:
 
 ```text
 usage: sumfolder1.py [-h] [--csv CSV] [--demo] [--ref] [-v]
 
-Calculate checksums for folders in a collection of objects using a DROID format identification report
+Calculate checksums for folders in a collection of objects using a DROID format
+identification report
 
 options:
   -h, --help          show this help message and exit
   --csv CSV           Single DROID CSV to read.
   --demo              Run demo queries and output a tree to demo.txt
   --ref, --reference  Write reference set to stdout.
   -v, --version       Return version information.
@@ -297,15 +307,16 @@
 
 ```bash
 python sumfolder1 --csv <droid_csv_file>
 ```
 
 ### Outputting the reference CSV
 
-A reference CSV can be output to `stdout`. Ideally it is piped to some other  file using a command such as follows:
+A reference CSV can be output to `stdout`. Ideally it is piped to some other
+file using a command such as follows:
 
 ```bash
 python sumfolder1 --ref > <output_file>
 ```
 
 ## License
```

### Comparing `sumfolder1-0.0.1rc6/src/sumfolder1.egg-info/SOURCES.txt` & `sumfolder1-0.0.2/src/sumfolder1.egg-info/SOURCES.txt`

 * *Files identical despite different names*

