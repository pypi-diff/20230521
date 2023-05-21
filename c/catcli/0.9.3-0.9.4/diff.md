# Comparing `tmp/catcli-0.9.3.tar.gz` & `tmp/catcli-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "catcli-0.9.3.tar", last modified: Mon Apr  3 21:10:48 2023, max compression
+gzip compressed data, was "catcli-0.9.4.tar", last modified: Sun May 21 19:02:16 2023, max compression
```

## Comparing `catcli-0.9.3.tar` & `catcli-0.9.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 21:10:48.148366 catcli-0.9.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-04-03 21:10:20.000000 catcli-0.9.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-03 21:10:20.000000 catcli-0.9.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    17646 2023-04-03 21:10:48.148366 catcli-0.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    13267 2023-04-03 21:10:20.000000 catcli-0.9.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 21:10:48.144366 catcli-0.9.3/catcli/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-04-03 21:10:20.000000 catcli-0.9.3/catcli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-04-03 21:10:20.000000 catcli-0.9.3/catcli/catalog.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12258 2023-04-03 21:10:20.000000 catcli-0.9.3/catcli/catcli.py
--rw-r--r--   0 runner    (1001) docker     (123)      853 2023-04-03 21:10:20.000000 catcli-0.9.3/catcli/colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-04-03 21:10:20.000000 catcli-0.9.3/catcli/decomp.py
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-03 21:10:20.000000 catcli-0.9.3/catcli/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-04-03 21:10:20.000000 catcli-0.9.3/catcli/fuser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-04-03 21:10:20.000000 catcli-0.9.3/catcli/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-04-03 21:10:20.000000 catcli-0.9.3/catcli/nodeprinter.py
--rw-r--r--   0 runner    (1001) docker     (123)    29841 2023-04-03 21:10:20.000000 catcli-0.9.3/catcli/noder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5377 2023-04-03 21:10:20.000000 catcli-0.9.3/catcli/nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-04-03 21:10:20.000000 catcli-0.9.3/catcli/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-03 21:10:20.000000 catcli-0.9.3/catcli/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-04-03 21:10:20.000000 catcli-0.9.3/catcli/walker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 21:10:48.148366 catcli-0.9.3/catcli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17646 2023-04-03 21:10:48.000000 catcli-0.9.3/catcli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-04-03 21:10:48.000000 catcli-0.9.3/catcli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 21:10:48.000000 catcli-0.9.3/catcli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-03 21:10:48.000000 catcli-0.9.3/catcli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-03 21:10:48.000000 catcli-0.9.3/catcli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-03 21:10:48.000000 catcli-0.9.3/catcli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-04-03 21:10:20.000000 catcli-0.9.3/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 21:10:48.148366 catcli-0.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-04-03 21:10:20.000000 catcli-0.9.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:02:16.424508 catcli-0.9.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35141 2023-05-21 19:01:54.000000 catcli-0.9.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-21 19:01:54.000000 catcli-0.9.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    17670 2023-05-21 19:02:16.424508 catcli-0.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    13291 2023-05-21 19:01:54.000000 catcli-0.9.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:02:16.424508 catcli-0.9.4/catcli/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-21 19:01:54.000000 catcli-0.9.4/catcli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3355 2023-05-21 19:01:54.000000 catcli-0.9.4/catcli/catalog.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12386 2023-05-21 19:01:54.000000 catcli-0.9.4/catcli/catcli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      853 2023-05-21 19:01:54.000000 catcli-0.9.4/catcli/colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-05-21 19:01:54.000000 catcli-0.9.4/catcli/decomp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-21 19:01:54.000000 catcli-0.9.4/catcli/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4060 2023-05-21 19:01:54.000000 catcli-0.9.4/catcli/fuser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-05-21 19:01:54.000000 catcli-0.9.4/catcli/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2384 2023-05-21 19:01:54.000000 catcli-0.9.4/catcli/nodeprinter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29990 2023-05-21 19:01:54.000000 catcli-0.9.4/catcli/noder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-05-21 19:01:54.000000 catcli-0.9.4/catcli/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3023 2023-05-21 19:01:54.000000 catcli-0.9.4/catcli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-21 19:01:54.000000 catcli-0.9.4/catcli/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6670 2023-05-21 19:01:54.000000 catcli-0.9.4/catcli/walker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:02:16.424508 catcli-0.9.4/catcli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17670 2023-05-21 19:02:16.000000 catcli-0.9.4/catcli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-21 19:02:16.000000 catcli-0.9.4/catcli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 19:02:16.000000 catcli-0.9.4/catcli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-21 19:02:16.000000 catcli-0.9.4/catcli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-21 19:02:16.000000 catcli-0.9.4/catcli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-21 19:02:16.000000 catcli-0.9.4/catcli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-21 19:01:54.000000 catcli-0.9.4/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 19:02:16.424508 catcli-0.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-05-21 19:01:54.000000 catcli-0.9.4/setup.py
```

### Comparing `catcli-0.9.3/LICENSE` & `catcli-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `catcli-0.9.3/PKG-INFO` & `catcli-0.9.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: catcli
-Version: 0.9.3
+Version: 0.9.4
 Summary: The command line catalog tool for your offline data
 Home-page: https://github.com/deadc0de6/catcli
 Author: deadc0de6
 Author-email: deadc0de6@foo.bar
 License: GPLv3
-Download-URL: https://github.com/deadc0de6/catcli/archive/v0.9.3.tar.gz
+Download-URL: https://github.com/deadc0de6/catcli/archive/v0.9.4.tar.gz
 Description: # CATCLI
         
-        [![Build Status](https://travis-ci.org/deadc0de6/catcli.svg?branch=master)](https://travis-ci.org/deadc0de6/catcli)
+        [![Tests Status](https://github.com/deadc0de6/catcli/workflows/tests/badge.svg?branch=master)](https://github.com/deadc0de6/catcli/actions)
         [![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](http://www.gnu.org/licenses/gpl-3.0)
         [![Coveralls](https://img.shields.io/coveralls/github/deadc0de6/catcli)](https://coveralls.io/github/deadc0de6/catcli?branch=master)
         
         [![PyPI version](https://badge.fury.io/py/catcli.svg)](https://badge.fury.io/py/catcli)
         [![AUR](https://img.shields.io/aur/version/catcli-git.svg)](https://aur.archlinux.org/packages/catcli-git)
         [![Python](https://img.shields.io/pypi/pyversions/catcli.svg)](https://pypi.python.org/pypi/catcli)
```

#### html2text {}

```diff
@@ -1,150 +1,150 @@
-Metadata-Version: 2.1 Name: catcli Version: 0.9.3 Summary: The command line
+Metadata-Version: 2.1 Name: catcli Version: 0.9.4 Summary: The command line
 catalog tool for your offline data Home-page: https://github.com/deadc0de6/
 catcli Author: deadc0de6 Author-email: deadc0de6@foo.bar License: GPLv3
-Download-URL: https://github.com/deadc0de6/catcli/archive/v0.9.3.tar.gz
-Description: # CATCLI [![Build Status](https://travis-ci.org/deadc0de6/
-catcli.svg?branch=master)](https://travis-ci.org/deadc0de6/catcli) [![License:
-GPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](http://
-www.gnu.org/licenses/gpl-3.0) [![Coveralls](https://img.shields.io/coveralls/
-github/deadc0de6/catcli)](https://coveralls.io/github/deadc0de6/
-catcli?branch=master) [![PyPI version](https://badge.fury.io/py/catcli.svg)]
-(https://badge.fury.io/py/catcli) [![AUR](https://img.shields.io/aur/version/
-catcli-git.svg)](https://aur.archlinux.org/packages/catcli-git) [![Python]
-(https://img.shields.io/pypi/pyversions/catcli.svg)](https://pypi.python.org/
-pypi/catcli) [![Donate](https://img.shields.io/badge/donate-KoFi-blue.svg)]
-(https://ko-fi.com/deadc0de6) *The command line catalog tool for your offline
-data* Did you ever wanted to find back that specific file that should be on one
-of your backup DVDs or one of your external hard drives? You usually go through
-all of them hoping to find the right one on the first try? [Catcli](https://
-github.com/deadc0de6/catcli) indexes external media in a catalog file and
-allows to quickly find specific files or even navigate in the catalog of
-indexed files while these are not connected to your host. Features: * Index any
-directories in a catalog * Ability to search for files by name in the catalog *
-Ability to navigate through indexed data Ã  la `ls` * Support for fuse to mount
-the indexed data as a virtual filesystem * Handle archive files (zip, tar, ...)
-and index their content * Save catalog to json for easy versioning with git *
-Command line interface FTW * Store files and directories sizes * Store md5 hash
-of files * Ability to update the catalog * Support for `fzf` for finding files
-* Tag your different storages with additional information * Export catalog to
-CSV [https://asciinema.org/a/hRE22qbVtBGxOM1yxw2y4fBy8.png] Quick start:
-```bash # install catcli with pip pip3 install catcli --user # index a
-directory in the catalog catcli index --meta='some description' log /var/log #
-display the content catcli ls -r # navigate catcli ls log # find files/
-directories named '*log*' catcli find log ``` see [usage](#usage) for specific
-info ## Why catcli? [Catcli](https://github.com/deadc0de6/catcli) gives the
-ability to navigate, explore and find your files that are stored on external
-media (DVDs, hard drives, USB sticks, etc) when those are not connected. Catcli
-can just as easily index any arbitrary directories. See the [examples]
-(#examples) for an overview of the available features. --- **Table of
-Contents** * [Installation](#installation) * [Usage](#usage) * [Index data]
-(#index-data) * [Index archive files](#index-archive-files) * [Walk indexed
-files with ls](#walk-indexed-files-with-ls) * [Find files](#find-files) *
-[Mount catalog](#mount-catalog) * [Display entire hierarchy](#display-entire-
-hierarchy) * [Catalog graph](#catalog-graph) * [Edit storage](#edit-storage) *
-[Update catalog](#update-catalog) * [CSV format](#csv-format) * [Examples]
-(#examples) * [Contribution](#contribution) * [Thank you](#thank-you) #
-Installation Install from Pypi ```bash $ pip3 install catcli --user ``` Or from
-github directly ```bash $ cd /tmp; git clone https://github.com/deadc0de6/
-catcli && cd catcli $ sudo python3 setup.py install $ catcli --help ``` To work
-with catcli without installing it, you can do the following ```bash $ cd /tmp;
-git clone https://github.com/deadc0de6/catcli && cd catcli $ pip3 install -
-r requirements.txt --user $ python3 -m catcli.catcli --help ``` or install it
-in a virtualenv ```bash $ cd /tmp; git clone https://github.com/deadc0de6/
-catcli && cd catcli $ virtualenv -p python3 env $ source env/bin/activate $
-python setup.py install $ catcli --help ``` Catcli is also available on aur:
-https://aur.archlinux.org/packages/catcli-git/ # Usage Each indexed directory
-is stored in the catalog. Multiple directories can be indexed and they are all
-available through the command line interface of catcli. Five different types of
-entry are present in a catalog: * **top node**: this is the root of the
-hierarchy * **storage node**: this represents an indexed storage (a DVD, an
-external hard drive, an USB drive, some arbitrary directory, etc). * **dir
-node**: this is a directory * **file node**: this is a file * **archive node**:
-this is a file contained in an archive (tar, zip, etc) ## Index data Let's say
-the DVD or external hard drive that needs to be indexed is mounted on `/media/
-mnt`. The following command will index the entire directory `/media/mnt` and
-store that in your catalog under the name ``. ```bash $ catcli index --meta=  /
-media/mnt ``` If not specified otherwise (with the switch `--catalog`), the
-catalog is saved in the current directory under `catcli.catalog`. The `--meta`
-switch allows to add any additional information to store along in the catalog
-like for example `the blue disk in my office`. Catcli will calculate and store
-the total size of each node (directories, storages, etc) unless the `-n --no-
-subsize` switch is used. Using the `-a --archive` switch allows to also index
-archive files as explained [below](#index-archive-files). ## Index archive
-files Catcli is able to index and explore the content of archive files.
-Following archive formats are supported: *tar*, *tar.gz*, *tar.xz*, *lzma*,
-*tar.bz2*, *zip*. Catcli is also able to find files within indexed archive
-files. See the [archive example](#archive-example) for more. ## Walk indexed
-files with ls A catalog can be walked using the command `ls` as if the media is
-mounted (File/directories separator is `/`). ```bash $ catcli ls tmp/a/b/c ```
-Resulting files can be sorted by size using `-S --sortsize`. See the [examples]
-(#examples) for more. ## Find files Files and directories can be found based on
-their names using the `find` command. `Find` support two formats that allow to
-use `fzf` for searching: * `--format=fzf-native`: display the result in native
-format * `--format=fzf-csv`: display the result in csv See the [examples]
-(#examples) for more. ## Mount catalog The catalog can be mounted with [fuse]
-(https://www.kernel.org/doc/html/next/filesystems/fuse.html) and navigate like
-any filesystem. ```bash $ mkdir /tmp/mnt $ catcli index -c github .github $
-catcli mount /tmp/mnt $ ls -laR /tmp/mnt drwxrwxrwx - user 8 Mar 22:08 github
-mnt/github: .rwxrwxrwx 17 user 19 Oct 2022 FUNDING.yml drwxrwxrwx - user 2 Mar
-10:15 workflows mnt/github/workflows: .rwxrwxrwx 691 user 19 Oct 2022 pypi-
-release.yml .rwxrwxrwx 635 user 8 Mar 21:08 testing.yml ``` ## Display entire
-hierarchy The entire catalog can be shown using the `ls -r` command. Resulting
-files can be sorted by size using the `-S --sortsize` switch. See the
-[examples](#examples) for more. ## Catalog graph The catalog can be exported in
-a dot file that can be used to generate a graph of the indexed files. ```bash $
-catcli graph dot file created under "/tmp/catcli.dot" create graph with "dot /
-tmp/catcli.dot -T png -o /tmp/tree.png" (you need graphviz) $ dot /tmp/
-catcli.dot -T png -o /tmp/tree.png ``` ## Edit storage Storage entry can be
-edited with following catcli commands: * `rename` - rename the storage * `edit`
-- edit storage metadata ## Update catalog The catalog can be updated with the
-`update` command. Updates are based on the access time of each of the files and
-on the hash checksum if present (catalog was indexed with `-c --hash` and
-`update` is called with the switch `-c --hash`). ## CSV format Results can be
-printed to CSV using `--format=csv`. Fields are separated by a comma (`,`) and
-are quoted with double quotes (`"`). Each line contains the following fields: *
-**name**: the entry name * **type**: the entry type (file, directory, storage,
-etc) * **path**: the entry path * **size**: the entry size * **indexed_at**:
-when this entry was indexed * **maccess**: the entry modification date/time *
-**md5**: the entry checksum (if any) * **nbfiles**: the number of children
-(empty for nodes that are not storage or directory) * **free_space**: free
-space (empty for not storage nodes) * **total_space**: total space (empty for
-not storage nodes) * **meta**: meta information (empty for not storage nodes) #
-Examples ## Simple example Let's first create some files and directories:
-```bash $ mkdir -p /tmp/test/{a,b,c} $ echo 'something in files in a' > /tmp/
-test/a/{1,2,3} $ echo 'something else in files in b' > /tmp/test/b/{4,5,6} $
-echo 'some bytes' > /tmp/test/c/{7,8,9} $ tree /tmp/test /tmp/test âââ a
-âÂ Â  âââ 1 âÂ Â  âââ 2 âÂ Â  âââ 3 âââ b âÂ Â 
-âââ 4 âÂ Â  âââ 5 âÂ Â  âââ 6 âââ c âââ 7
-âââ 8 âââ 9 3 directories, 9 files ``` First this directory is
-indexed with `catcli` as if it was some kind of external storage: ```bash $
-catcli index --meta='my test directory' tmptest /tmp/test ``` Catcli creates
-its catalog file in the current directory as `catcli.catalog`. Printing the
-entire catalog as a tree is done with the command `ls -r` ``` $ catcli ls -
-r top âââ storage: tmptest (my test directory) (nbfiles:3, free:3.7G/
-3.7G, date:2019-01-26 19:59:47) âââ a [nbfiles:3, totsize:72] â
-âââ 1 [size:24] â âââ 2 [size:24] â âââ 3 [size:24]
-âââ b [nbfiles:3, totsize:87] â âââ 4 [size:29] â âââ 5
-[size:29] â âââ 6 [size:29] âââ c [nbfiles:3, totsize:33]
-âââ 7 [size:11] âââ 8 [size:11] âââ 9 [size:11] ``` The
-catalog can be walked with `ls` as if it was a normal directory ``` $ catcli ls
-top - storage: tmptest (my test directory) (nbfiles:3, free:3.7G/3.7G, date:
-2019-01-26 19:59:47) $ catcli ls tmptest storage: tmptest (my test directory)
-(nbfiles:3, free:3.7G/3.7G, date:2019-01-26 19:59:47) - a [nbfiles:3, totsize:
-72] - b [nbfiles:3, totsize:87] - c [nbfiles:3, totsize:33] $ catcli ls
-tmptest/b b [nbfiles:3, totsize:87] - 4 [size:29] - 5 [size:29] - 6 [size:29]
-``` And files can be found using the command `find` ```bash $ catcli find 9 c/
-9 [size:11, storage:tmptest] ``` When using the `-b --script` switch, a one-
-liner is generated that allows to handle the found file(s) ``` $ catcli find 9
---script c/9 [size:11, storage:tmptest] op=file; source=/media/mnt; $op $
-{source}/c/9 ``` ## Archive example Let's consider a directory containing
-archive files: ```bash $ ls -1 /tmp/catcli catcli-0.3.1 v0.3.1.tar.gz
-v0.3.1.zip ``` To enable the indexing of archive contents use the `-a --
-archive` switch ```bash $ catcli index -au some-name /tmp/catcli ``` Then any
-command can be used to explore the catalog as for normal files but, by
+Download-URL: https://github.com/deadc0de6/catcli/archive/v0.9.4.tar.gz
+Description: # CATCLI [![Tests Status](https://github.com/deadc0de6/catcli/
+workflows/tests/badge.svg?branch=master)](https://github.com/deadc0de6/catcli/
+actions) [![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-
+blue.svg)](http://www.gnu.org/licenses/gpl-3.0) [![Coveralls](https://
+img.shields.io/coveralls/github/deadc0de6/catcli)](https://coveralls.io/github/
+deadc0de6/catcli?branch=master) [![PyPI version](https://badge.fury.io/py/
+catcli.svg)](https://badge.fury.io/py/catcli) [![AUR](https://img.shields.io/
+aur/version/catcli-git.svg)](https://aur.archlinux.org/packages/catcli-git) [!
+[Python](https://img.shields.io/pypi/pyversions/catcli.svg)](https://
+pypi.python.org/pypi/catcli) [![Donate](https://img.shields.io/badge/donate-
+KoFi-blue.svg)](https://ko-fi.com/deadc0de6) *The command line catalog tool for
+your offline data* Did you ever wanted to find back that specific file that
+should be on one of your backup DVDs or one of your external hard drives? You
+usually go through all of them hoping to find the right one on the first try?
+[Catcli](https://github.com/deadc0de6/catcli) indexes external media in a
+catalog file and allows to quickly find specific files or even navigate in the
+catalog of indexed files while these are not connected to your host. Features:
+* Index any directories in a catalog * Ability to search for files by name in
+the catalog * Ability to navigate through indexed data Ã  la `ls` * Support for
+fuse to mount the indexed data as a virtual filesystem * Handle archive files
+(zip, tar, ...) and index their content * Save catalog to json for easy
+versioning with git * Command line interface FTW * Store files and directories
+sizes * Store md5 hash of files * Ability to update the catalog * Support for
+`fzf` for finding files * Tag your different storages with additional
+information * Export catalog to CSV [https://asciinema.org/a/
+hRE22qbVtBGxOM1yxw2y4fBy8.png] Quick start: ```bash # install catcli with pip
+pip3 install catcli --user # index a directory in the catalog catcli index --
+meta='some description' log /var/log # display the content catcli ls -r #
+navigate catcli ls log # find files/directories named '*log*' catcli find log
+``` see [usage](#usage) for specific info ## Why catcli? [Catcli](https://
+github.com/deadc0de6/catcli) gives the ability to navigate, explore and find
+your files that are stored on external media (DVDs, hard drives, USB sticks,
+etc) when those are not connected. Catcli can just as easily index any
+arbitrary directories. See the [examples](#examples) for an overview of the
+available features. --- **Table of Contents** * [Installation](#installation) *
+[Usage](#usage) * [Index data](#index-data) * [Index archive files](#index-
+archive-files) * [Walk indexed files with ls](#walk-indexed-files-with-ls) *
+[Find files](#find-files) * [Mount catalog](#mount-catalog) * [Display entire
+hierarchy](#display-entire-hierarchy) * [Catalog graph](#catalog-graph) * [Edit
+storage](#edit-storage) * [Update catalog](#update-catalog) * [CSV format]
+(#csv-format) * [Examples](#examples) * [Contribution](#contribution) * [Thank
+you](#thank-you) # Installation Install from Pypi ```bash $ pip3 install catcli
+--user ``` Or from github directly ```bash $ cd /tmp; git clone https://
+github.com/deadc0de6/catcli && cd catcli $ sudo python3 setup.py install $
+catcli --help ``` To work with catcli without installing it, you can do the
+following ```bash $ cd /tmp; git clone https://github.com/deadc0de6/catcli &&
+cd catcli $ pip3 install -r requirements.txt --user $ python3 -m catcli.catcli
+--help ``` or install it in a virtualenv ```bash $ cd /tmp; git clone https://
+github.com/deadc0de6/catcli && cd catcli $ virtualenv -p python3 env $ source
+env/bin/activate $ python setup.py install $ catcli --help ``` Catcli is also
+available on aur: https://aur.archlinux.org/packages/catcli-git/ # Usage Each
+indexed directory is stored in the catalog. Multiple directories can be indexed
+and they are all available through the command line interface of catcli. Five
+different types of entry are present in a catalog: * **top node**: this is the
+root of the hierarchy * **storage node**: this represents an indexed storage (a
+DVD, an external hard drive, an USB drive, some arbitrary directory, etc). *
+**dir node**: this is a directory * **file node**: this is a file * **archive
+node**: this is a file contained in an archive (tar, zip, etc) ## Index data
+Let's say the DVD or external hard drive that needs to be indexed is mounted on
+`/media/mnt`. The following command will index the entire directory `/media/
+mnt` and store that in your catalog under the name ``. ```bash $ catcli index -
+-meta=  /media/mnt ``` If not specified otherwise (with the switch `--
+catalog`), the catalog is saved in the current directory under
+`catcli.catalog`. The `--meta` switch allows to add any additional information
+to store along in the catalog like for example `the blue disk in my office`.
+Catcli will calculate and store the total size of each node (directories,
+storages, etc) unless the `-n --no-subsize` switch is used. Using the `-a --
+archive` switch allows to also index archive files as explained [below](#index-
+archive-files). ## Index archive files Catcli is able to index and explore the
+content of archive files. Following archive formats are supported: *tar*,
+*tar.gz*, *tar.xz*, *lzma*, *tar.bz2*, *zip*. Catcli is also able to find files
+within indexed archive files. See the [archive example](#archive-example) for
+more. ## Walk indexed files with ls A catalog can be walked using the command
+`ls` as if the media is mounted (File/directories separator is `/`). ```bash $
+catcli ls tmp/a/b/c ``` Resulting files can be sorted by size using `-S --
+sortsize`. See the [examples](#examples) for more. ## Find files Files and
+directories can be found based on their names using the `find` command. `Find`
+support two formats that allow to use `fzf` for searching: * `--format=fzf-
+native`: display the result in native format * `--format=fzf-csv`: display the
+result in csv See the [examples](#examples) for more. ## Mount catalog The
+catalog can be mounted with [fuse](https://www.kernel.org/doc/html/next/
+filesystems/fuse.html) and navigate like any filesystem. ```bash $ mkdir /tmp/
+mnt $ catcli index -c github .github $ catcli mount /tmp/mnt $ ls -laR /tmp/mnt
+drwxrwxrwx - user 8 Mar 22:08 github mnt/github: .rwxrwxrwx 17 user 19 Oct 2022
+FUNDING.yml drwxrwxrwx - user 2 Mar 10:15 workflows mnt/github/workflows:
+.rwxrwxrwx 691 user 19 Oct 2022 pypi-release.yml .rwxrwxrwx 635 user 8 Mar 21:
+08 testing.yml ``` ## Display entire hierarchy The entire catalog can be shown
+using the `ls -r` command. Resulting files can be sorted by size using the `-
+S --sortsize` switch. See the [examples](#examples) for more. ## Catalog graph
+The catalog can be exported in a dot file that can be used to generate a graph
+of the indexed files. ```bash $ catcli graph dot file created under "/tmp/
+catcli.dot" create graph with "dot /tmp/catcli.dot -T png -o /tmp/tree.png"
+(you need graphviz) $ dot /tmp/catcli.dot -T png -o /tmp/tree.png ``` ## Edit
+storage Storage entry can be edited with following catcli commands: * `rename`
+- rename the storage * `edit` - edit storage metadata ## Update catalog The
+catalog can be updated with the `update` command. Updates are based on the
+access time of each of the files and on the hash checksum if present (catalog
+was indexed with `-c --hash` and `update` is called with the switch `-c --
+hash`). ## CSV format Results can be printed to CSV using `--format=csv`.
+Fields are separated by a comma (`,`) and are quoted with double quotes (`"`).
+Each line contains the following fields: * **name**: the entry name * **type**:
+the entry type (file, directory, storage, etc) * **path**: the entry path *
+**size**: the entry size * **indexed_at**: when this entry was indexed *
+**maccess**: the entry modification date/time * **md5**: the entry checksum (if
+any) * **nbfiles**: the number of children (empty for nodes that are not
+storage or directory) * **free_space**: free space (empty for not storage
+nodes) * **total_space**: total space (empty for not storage nodes) * **meta**:
+meta information (empty for not storage nodes) # Examples ## Simple example
+Let's first create some files and directories: ```bash $ mkdir -p /tmp/test/
+{a,b,c} $ echo 'something in files in a' > /tmp/test/a/{1,2,3} $ echo
+'something else in files in b' > /tmp/test/b/{4,5,6} $ echo 'some bytes' > /
+tmp/test/c/{7,8,9} $ tree /tmp/test /tmp/test âââ a âÂ Â  âââ 1
+âÂ Â  âââ 2 âÂ Â  âââ 3 âââ b âÂ Â  âââ 4 âÂ Â 
+âââ 5 âÂ Â  âââ 6 âââ c âââ 7 âââ 8 âââ 9
+3 directories, 9 files ``` First this directory is indexed with `catcli` as if
+it was some kind of external storage: ```bash $ catcli index --meta='my test
+directory' tmptest /tmp/test ``` Catcli creates its catalog file in the current
+directory as `catcli.catalog`. Printing the entire catalog as a tree is done
+with the command `ls -r` ``` $ catcli ls -r top âââ storage: tmptest (my
+test directory) (nbfiles:3, free:3.7G/3.7G, date:2019-01-26 19:59:47) âââ
+a [nbfiles:3, totsize:72] â âââ 1 [size:24] â âââ 2 [size:24]
+â âââ 3 [size:24] âââ b [nbfiles:3, totsize:87] â âââ 4
+[size:29] â âââ 5 [size:29] â âââ 6 [size:29] âââ c
+[nbfiles:3, totsize:33] âââ 7 [size:11] âââ 8 [size:11] âââ 9
+[size:11] ``` The catalog can be walked with `ls` as if it was a normal
+directory ``` $ catcli ls top - storage: tmptest (my test directory) (nbfiles:
+3, free:3.7G/3.7G, date:2019-01-26 19:59:47) $ catcli ls tmptest storage:
+tmptest (my test directory) (nbfiles:3, free:3.7G/3.7G, date:2019-01-26 19:59:
+47) - a [nbfiles:3, totsize:72] - b [nbfiles:3, totsize:87] - c [nbfiles:3,
+totsize:33] $ catcli ls tmptest/b b [nbfiles:3, totsize:87] - 4 [size:29] - 5
+[size:29] - 6 [size:29] ``` And files can be found using the command `find`
+```bash $ catcli find 9 c/9 [size:11, storage:tmptest] ``` When using the `-b -
+-script` switch, a one-liner is generated that allows to handle the found file
+(s) ``` $ catcli find 9 --script c/9 [size:11, storage:tmptest] op=file;
+source=/media/mnt; $op ${source}/c/9 ``` ## Archive example Let's consider a
+directory containing archive files: ```bash $ ls -1 /tmp/catcli catcli-0.3.1
+v0.3.1.tar.gz v0.3.1.zip ``` To enable the indexing of archive contents use the
+`-a --archive` switch ```bash $ catcli index -au some-name /tmp/catcli ``` Then
+any command can be used to explore the catalog as for normal files but, by
 providing the `-a --archive` switch, archive content are displayed. ```bash $
 catcli ls some-name storage: some-name (free:800G, total:1T) - catcli-0.3.1
 [nbfiles:11, totsize:80.5K] - v0.3.1.tar.gz [size:24.2K] - v0.3.1.zip [size:
 31.2K] $ catcli ls -r some-name/v0.3.1.zip v0.3.1.zip [size:31.2K] $ catcli ls
 -ar some-name/v0.3.1.zip v0.3.1.zip [size:31.2K] âââ catcli-0.3.1
 [archive:v0.3.1.zip] â âââ catcli [archive:v0.3.1.zip] â â
 âââ __init__.py [archive:v0.3.1.zip] â â âââ catalog.py
```

### Comparing `catcli-0.9.3/README.md` & `catcli-0.9.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # CATCLI
 
-[![Build Status](https://travis-ci.org/deadc0de6/catcli.svg?branch=master)](https://travis-ci.org/deadc0de6/catcli)
+[![Tests Status](https://github.com/deadc0de6/catcli/workflows/tests/badge.svg?branch=master)](https://github.com/deadc0de6/catcli/actions)
 [![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](http://www.gnu.org/licenses/gpl-3.0)
 [![Coveralls](https://img.shields.io/coveralls/github/deadc0de6/catcli)](https://coveralls.io/github/deadc0de6/catcli?branch=master)
 
 [![PyPI version](https://badge.fury.io/py/catcli.svg)](https://badge.fury.io/py/catcli)
 [![AUR](https://img.shields.io/aur/version/catcli-git.svg)](https://aur.archlinux.org/packages/catcli-git)
 [![Python](https://img.shields.io/pypi/pyversions/catcli.svg)](https://pypi.python.org/pypi/catcli)
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-# CATCLI [![Build Status](https://travis-ci.org/deadc0de6/
-catcli.svg?branch=master)](https://travis-ci.org/deadc0de6/catcli) [![License:
-GPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](http://
-www.gnu.org/licenses/gpl-3.0) [![Coveralls](https://img.shields.io/coveralls/
-github/deadc0de6/catcli)](https://coveralls.io/github/deadc0de6/
+# CATCLI [![Tests Status](https://github.com/deadc0de6/catcli/workflows/tests/
+badge.svg?branch=master)](https://github.com/deadc0de6/catcli/actions) [!
+[License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)]
+(http://www.gnu.org/licenses/gpl-3.0) [![Coveralls](https://img.shields.io/
+coveralls/github/deadc0de6/catcli)](https://coveralls.io/github/deadc0de6/
 catcli?branch=master) [![PyPI version](https://badge.fury.io/py/catcli.svg)]
 (https://badge.fury.io/py/catcli) [![AUR](https://img.shields.io/aur/version/
 catcli-git.svg)](https://aur.archlinux.org/packages/catcli-git) [![Python]
 (https://img.shields.io/pypi/pyversions/catcli.svg)](https://pypi.python.org/
 pypi/catcli) [![Donate](https://img.shields.io/badge/donate-KoFi-blue.svg)]
 (https://ko-fi.com/deadc0de6) *The command line catalog tool for your offline
 data* Did you ever wanted to find back that specific file that should be on one
```

### Comparing `catcli-0.9.3/catcli/catalog.py` & `catcli-0.9.4/catcli/catalog.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,15 +90,15 @@
             exp.write(top, file)
         self._debug(f'Catalog saved to json \"{self.path}\"')
         return True
 
     def _restore_json(self, string: str) -> Optional[NodeTop]:
         """restore the tree from json"""
         imp = JsonImporter()
-        self._debug(f'import from string: {string}')
+        self._debug('import from string...')
         root = imp.import_(string)
         self._debug(f'Catalog imported from json \"{self.path}\"')
         self._debug(f'root imported: {root}')
         if root.type != nodes.TYPE_TOP:
             return None
         top = NodeTop(root.name, children=root.children)
         self._debug(f'top imported: {top}')
```

### Comparing `catcli-0.9.3/catcli/catcli.py` & `catcli-0.9.4/catcli/catcli.py`

 * *Files 2% similar despite different names*

```diff
@@ -206,20 +206,23 @@
     fromtree = args['--parent']
     directory = args['--directory']
     startpath = args['--path']
     fmt = args['--format']
     raw = args['--raw-size']
     script = args['--script']
     search_for = args['<term>']
+    if args['--verbose']:
+        Logger.debug(f'search for \"{search_for}\" under \"{top.name}\"')
     found = noder.find_name(top, search_for,
                             script=script,
                             startnode=startpath,
                             only_dir=directory,
                             parentfromtree=fromtree,
-                            fmt=fmt, raw=raw)
+                            fmt=fmt,
+                            raw=raw)
     return found
 
 
 def cmd_graph(args: Dict[str, Any],
               noder: Noder,
               top: NodeTop) -> None:
     """graph action"""
```

### Comparing `catcli-0.9.3/catcli/colors.py` & `catcli-0.9.4/catcli/colors.py`

 * *Files identical despite different names*

### Comparing `catcli-0.9.3/catcli/decomp.py` & `catcli-0.9.4/catcli/decomp.py`

 * *Files identical despite different names*

### Comparing `catcli-0.9.3/catcli/fuser.py` & `catcli-0.9.4/catcli/fuser.py`

 * *Files identical despite different names*

### Comparing `catcli-0.9.3/catcli/logger.py` & `catcli-0.9.4/catcli/logger.py`

 * *Files identical despite different names*

### Comparing `catcli-0.9.3/catcli/nodeprinter.py` & `catcli-0.9.4/catcli/nodeprinter.py`

 * *Files identical despite different names*

### Comparing `catcli-0.9.3/catcli/noder.py` & `catcli-0.9.4/catcli/noder.py`

 * *Files 0% similar despite different names*

```diff
@@ -578,27 +578,30 @@
 
         # search for nodes based on path
         start: Optional[NodeAny] = top
         if startnode:
             start = self.get_node(top, startnode)
         filterfunc = self._callback_find_name(key, only_dir)
         found = anytree.findall(start, filter_=filterfunc)
-        nbfound = len(found)
-        self._debug(f'found {nbfound} node(s)')
+        self._debug(f'found {len(found)} node(s)')
 
         # compile found nodes
         paths = {}
         for item in found:
             item.name = fix_badchars(item.name)
             if hasattr(item, 'relpath'):
                 item.relpath = fix_badchars(item.relpath)
+            storage = self._get_storage(item)
             if parentfromtree:
-                paths[self._get_parents(item)] = item
+                parent = self._get_parents(item)
+                key = f'{storage}/{parent}/{item.relpath}'
+                paths[parent] = item
             else:
-                paths[item.relpath] = item
+                key = f'{storage}/{item.path}'
+                paths[key] = item
 
         # handle fzf mode
         if fmt.startswith('fzf'):
             selected = self._fzf_prompt(paths.keys())
             newpaths = {}
             subfmt = fmt.replace('fzf-', '')
             for item in selected:
```

### Comparing `catcli-0.9.3/catcli/nodes.py` & `catcli-0.9.4/catcli/nodes.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
             self.children = children
 
     def _to_str(self) -> str:
         ret = str(self.__class__) + ": " + str(self.__dict__)
         if self.children:
             ret += '\n'
         for child in self.children:
-            ret += '  child => ' + str(child)
+            ret += f'  child => {child}\n'
         return ret
 
     def __str__(self) -> str:
         return self._to_str()
 
     def flagged(self) -> bool:
         """is flagged"""
```

### Comparing `catcli-0.9.3/catcli/utils.py` & `catcli-0.9.4/catcli/utils.py`

 * *Files identical despite different names*

### Comparing `catcli-0.9.3/catcli/walker.py` & `catcli-0.9.4/catcli/walker.py`

 * *Files identical despite different names*

### Comparing `catcli-0.9.3/catcli.egg-info/PKG-INFO` & `catcli-0.9.4/catcli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: catcli
-Version: 0.9.3
+Version: 0.9.4
 Summary: The command line catalog tool for your offline data
 Home-page: https://github.com/deadc0de6/catcli
 Author: deadc0de6
 Author-email: deadc0de6@foo.bar
 License: GPLv3
-Download-URL: https://github.com/deadc0de6/catcli/archive/v0.9.3.tar.gz
+Download-URL: https://github.com/deadc0de6/catcli/archive/v0.9.4.tar.gz
 Description: # CATCLI
         
-        [![Build Status](https://travis-ci.org/deadc0de6/catcli.svg?branch=master)](https://travis-ci.org/deadc0de6/catcli)
+        [![Tests Status](https://github.com/deadc0de6/catcli/workflows/tests/badge.svg?branch=master)](https://github.com/deadc0de6/catcli/actions)
         [![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](http://www.gnu.org/licenses/gpl-3.0)
         [![Coveralls](https://img.shields.io/coveralls/github/deadc0de6/catcli)](https://coveralls.io/github/deadc0de6/catcli?branch=master)
         
         [![PyPI version](https://badge.fury.io/py/catcli.svg)](https://badge.fury.io/py/catcli)
         [![AUR](https://img.shields.io/aur/version/catcli-git.svg)](https://aur.archlinux.org/packages/catcli-git)
         [![Python](https://img.shields.io/pypi/pyversions/catcli.svg)](https://pypi.python.org/pypi/catcli)
```

#### html2text {}

```diff
@@ -1,150 +1,150 @@
-Metadata-Version: 2.1 Name: catcli Version: 0.9.3 Summary: The command line
+Metadata-Version: 2.1 Name: catcli Version: 0.9.4 Summary: The command line
 catalog tool for your offline data Home-page: https://github.com/deadc0de6/
 catcli Author: deadc0de6 Author-email: deadc0de6@foo.bar License: GPLv3
-Download-URL: https://github.com/deadc0de6/catcli/archive/v0.9.3.tar.gz
-Description: # CATCLI [![Build Status](https://travis-ci.org/deadc0de6/
-catcli.svg?branch=master)](https://travis-ci.org/deadc0de6/catcli) [![License:
-GPL v3](https://img.shields.io/badge/License-GPL%20v3-blue.svg)](http://
-www.gnu.org/licenses/gpl-3.0) [![Coveralls](https://img.shields.io/coveralls/
-github/deadc0de6/catcli)](https://coveralls.io/github/deadc0de6/
-catcli?branch=master) [![PyPI version](https://badge.fury.io/py/catcli.svg)]
-(https://badge.fury.io/py/catcli) [![AUR](https://img.shields.io/aur/version/
-catcli-git.svg)](https://aur.archlinux.org/packages/catcli-git) [![Python]
-(https://img.shields.io/pypi/pyversions/catcli.svg)](https://pypi.python.org/
-pypi/catcli) [![Donate](https://img.shields.io/badge/donate-KoFi-blue.svg)]
-(https://ko-fi.com/deadc0de6) *The command line catalog tool for your offline
-data* Did you ever wanted to find back that specific file that should be on one
-of your backup DVDs or one of your external hard drives? You usually go through
-all of them hoping to find the right one on the first try? [Catcli](https://
-github.com/deadc0de6/catcli) indexes external media in a catalog file and
-allows to quickly find specific files or even navigate in the catalog of
-indexed files while these are not connected to your host. Features: * Index any
-directories in a catalog * Ability to search for files by name in the catalog *
-Ability to navigate through indexed data Ã  la `ls` * Support for fuse to mount
-the indexed data as a virtual filesystem * Handle archive files (zip, tar, ...)
-and index their content * Save catalog to json for easy versioning with git *
-Command line interface FTW * Store files and directories sizes * Store md5 hash
-of files * Ability to update the catalog * Support for `fzf` for finding files
-* Tag your different storages with additional information * Export catalog to
-CSV [https://asciinema.org/a/hRE22qbVtBGxOM1yxw2y4fBy8.png] Quick start:
-```bash # install catcli with pip pip3 install catcli --user # index a
-directory in the catalog catcli index --meta='some description' log /var/log #
-display the content catcli ls -r # navigate catcli ls log # find files/
-directories named '*log*' catcli find log ``` see [usage](#usage) for specific
-info ## Why catcli? [Catcli](https://github.com/deadc0de6/catcli) gives the
-ability to navigate, explore and find your files that are stored on external
-media (DVDs, hard drives, USB sticks, etc) when those are not connected. Catcli
-can just as easily index any arbitrary directories. See the [examples]
-(#examples) for an overview of the available features. --- **Table of
-Contents** * [Installation](#installation) * [Usage](#usage) * [Index data]
-(#index-data) * [Index archive files](#index-archive-files) * [Walk indexed
-files with ls](#walk-indexed-files-with-ls) * [Find files](#find-files) *
-[Mount catalog](#mount-catalog) * [Display entire hierarchy](#display-entire-
-hierarchy) * [Catalog graph](#catalog-graph) * [Edit storage](#edit-storage) *
-[Update catalog](#update-catalog) * [CSV format](#csv-format) * [Examples]
-(#examples) * [Contribution](#contribution) * [Thank you](#thank-you) #
-Installation Install from Pypi ```bash $ pip3 install catcli --user ``` Or from
-github directly ```bash $ cd /tmp; git clone https://github.com/deadc0de6/
-catcli && cd catcli $ sudo python3 setup.py install $ catcli --help ``` To work
-with catcli without installing it, you can do the following ```bash $ cd /tmp;
-git clone https://github.com/deadc0de6/catcli && cd catcli $ pip3 install -
-r requirements.txt --user $ python3 -m catcli.catcli --help ``` or install it
-in a virtualenv ```bash $ cd /tmp; git clone https://github.com/deadc0de6/
-catcli && cd catcli $ virtualenv -p python3 env $ source env/bin/activate $
-python setup.py install $ catcli --help ``` Catcli is also available on aur:
-https://aur.archlinux.org/packages/catcli-git/ # Usage Each indexed directory
-is stored in the catalog. Multiple directories can be indexed and they are all
-available through the command line interface of catcli. Five different types of
-entry are present in a catalog: * **top node**: this is the root of the
-hierarchy * **storage node**: this represents an indexed storage (a DVD, an
-external hard drive, an USB drive, some arbitrary directory, etc). * **dir
-node**: this is a directory * **file node**: this is a file * **archive node**:
-this is a file contained in an archive (tar, zip, etc) ## Index data Let's say
-the DVD or external hard drive that needs to be indexed is mounted on `/media/
-mnt`. The following command will index the entire directory `/media/mnt` and
-store that in your catalog under the name ``. ```bash $ catcli index --meta=  /
-media/mnt ``` If not specified otherwise (with the switch `--catalog`), the
-catalog is saved in the current directory under `catcli.catalog`. The `--meta`
-switch allows to add any additional information to store along in the catalog
-like for example `the blue disk in my office`. Catcli will calculate and store
-the total size of each node (directories, storages, etc) unless the `-n --no-
-subsize` switch is used. Using the `-a --archive` switch allows to also index
-archive files as explained [below](#index-archive-files). ## Index archive
-files Catcli is able to index and explore the content of archive files.
-Following archive formats are supported: *tar*, *tar.gz*, *tar.xz*, *lzma*,
-*tar.bz2*, *zip*. Catcli is also able to find files within indexed archive
-files. See the [archive example](#archive-example) for more. ## Walk indexed
-files with ls A catalog can be walked using the command `ls` as if the media is
-mounted (File/directories separator is `/`). ```bash $ catcli ls tmp/a/b/c ```
-Resulting files can be sorted by size using `-S --sortsize`. See the [examples]
-(#examples) for more. ## Find files Files and directories can be found based on
-their names using the `find` command. `Find` support two formats that allow to
-use `fzf` for searching: * `--format=fzf-native`: display the result in native
-format * `--format=fzf-csv`: display the result in csv See the [examples]
-(#examples) for more. ## Mount catalog The catalog can be mounted with [fuse]
-(https://www.kernel.org/doc/html/next/filesystems/fuse.html) and navigate like
-any filesystem. ```bash $ mkdir /tmp/mnt $ catcli index -c github .github $
-catcli mount /tmp/mnt $ ls -laR /tmp/mnt drwxrwxrwx - user 8 Mar 22:08 github
-mnt/github: .rwxrwxrwx 17 user 19 Oct 2022 FUNDING.yml drwxrwxrwx - user 2 Mar
-10:15 workflows mnt/github/workflows: .rwxrwxrwx 691 user 19 Oct 2022 pypi-
-release.yml .rwxrwxrwx 635 user 8 Mar 21:08 testing.yml ``` ## Display entire
-hierarchy The entire catalog can be shown using the `ls -r` command. Resulting
-files can be sorted by size using the `-S --sortsize` switch. See the
-[examples](#examples) for more. ## Catalog graph The catalog can be exported in
-a dot file that can be used to generate a graph of the indexed files. ```bash $
-catcli graph dot file created under "/tmp/catcli.dot" create graph with "dot /
-tmp/catcli.dot -T png -o /tmp/tree.png" (you need graphviz) $ dot /tmp/
-catcli.dot -T png -o /tmp/tree.png ``` ## Edit storage Storage entry can be
-edited with following catcli commands: * `rename` - rename the storage * `edit`
-- edit storage metadata ## Update catalog The catalog can be updated with the
-`update` command. Updates are based on the access time of each of the files and
-on the hash checksum if present (catalog was indexed with `-c --hash` and
-`update` is called with the switch `-c --hash`). ## CSV format Results can be
-printed to CSV using `--format=csv`. Fields are separated by a comma (`,`) and
-are quoted with double quotes (`"`). Each line contains the following fields: *
-**name**: the entry name * **type**: the entry type (file, directory, storage,
-etc) * **path**: the entry path * **size**: the entry size * **indexed_at**:
-when this entry was indexed * **maccess**: the entry modification date/time *
-**md5**: the entry checksum (if any) * **nbfiles**: the number of children
-(empty for nodes that are not storage or directory) * **free_space**: free
-space (empty for not storage nodes) * **total_space**: total space (empty for
-not storage nodes) * **meta**: meta information (empty for not storage nodes) #
-Examples ## Simple example Let's first create some files and directories:
-```bash $ mkdir -p /tmp/test/{a,b,c} $ echo 'something in files in a' > /tmp/
-test/a/{1,2,3} $ echo 'something else in files in b' > /tmp/test/b/{4,5,6} $
-echo 'some bytes' > /tmp/test/c/{7,8,9} $ tree /tmp/test /tmp/test âââ a
-âÂ Â  âââ 1 âÂ Â  âââ 2 âÂ Â  âââ 3 âââ b âÂ Â 
-âââ 4 âÂ Â  âââ 5 âÂ Â  âââ 6 âââ c âââ 7
-âââ 8 âââ 9 3 directories, 9 files ``` First this directory is
-indexed with `catcli` as if it was some kind of external storage: ```bash $
-catcli index --meta='my test directory' tmptest /tmp/test ``` Catcli creates
-its catalog file in the current directory as `catcli.catalog`. Printing the
-entire catalog as a tree is done with the command `ls -r` ``` $ catcli ls -
-r top âââ storage: tmptest (my test directory) (nbfiles:3, free:3.7G/
-3.7G, date:2019-01-26 19:59:47) âââ a [nbfiles:3, totsize:72] â
-âââ 1 [size:24] â âââ 2 [size:24] â âââ 3 [size:24]
-âââ b [nbfiles:3, totsize:87] â âââ 4 [size:29] â âââ 5
-[size:29] â âââ 6 [size:29] âââ c [nbfiles:3, totsize:33]
-âââ 7 [size:11] âââ 8 [size:11] âââ 9 [size:11] ``` The
-catalog can be walked with `ls` as if it was a normal directory ``` $ catcli ls
-top - storage: tmptest (my test directory) (nbfiles:3, free:3.7G/3.7G, date:
-2019-01-26 19:59:47) $ catcli ls tmptest storage: tmptest (my test directory)
-(nbfiles:3, free:3.7G/3.7G, date:2019-01-26 19:59:47) - a [nbfiles:3, totsize:
-72] - b [nbfiles:3, totsize:87] - c [nbfiles:3, totsize:33] $ catcli ls
-tmptest/b b [nbfiles:3, totsize:87] - 4 [size:29] - 5 [size:29] - 6 [size:29]
-``` And files can be found using the command `find` ```bash $ catcli find 9 c/
-9 [size:11, storage:tmptest] ``` When using the `-b --script` switch, a one-
-liner is generated that allows to handle the found file(s) ``` $ catcli find 9
---script c/9 [size:11, storage:tmptest] op=file; source=/media/mnt; $op $
-{source}/c/9 ``` ## Archive example Let's consider a directory containing
-archive files: ```bash $ ls -1 /tmp/catcli catcli-0.3.1 v0.3.1.tar.gz
-v0.3.1.zip ``` To enable the indexing of archive contents use the `-a --
-archive` switch ```bash $ catcli index -au some-name /tmp/catcli ``` Then any
-command can be used to explore the catalog as for normal files but, by
+Download-URL: https://github.com/deadc0de6/catcli/archive/v0.9.4.tar.gz
+Description: # CATCLI [![Tests Status](https://github.com/deadc0de6/catcli/
+workflows/tests/badge.svg?branch=master)](https://github.com/deadc0de6/catcli/
+actions) [![License: GPL v3](https://img.shields.io/badge/License-GPL%20v3-
+blue.svg)](http://www.gnu.org/licenses/gpl-3.0) [![Coveralls](https://
+img.shields.io/coveralls/github/deadc0de6/catcli)](https://coveralls.io/github/
+deadc0de6/catcli?branch=master) [![PyPI version](https://badge.fury.io/py/
+catcli.svg)](https://badge.fury.io/py/catcli) [![AUR](https://img.shields.io/
+aur/version/catcli-git.svg)](https://aur.archlinux.org/packages/catcli-git) [!
+[Python](https://img.shields.io/pypi/pyversions/catcli.svg)](https://
+pypi.python.org/pypi/catcli) [![Donate](https://img.shields.io/badge/donate-
+KoFi-blue.svg)](https://ko-fi.com/deadc0de6) *The command line catalog tool for
+your offline data* Did you ever wanted to find back that specific file that
+should be on one of your backup DVDs or one of your external hard drives? You
+usually go through all of them hoping to find the right one on the first try?
+[Catcli](https://github.com/deadc0de6/catcli) indexes external media in a
+catalog file and allows to quickly find specific files or even navigate in the
+catalog of indexed files while these are not connected to your host. Features:
+* Index any directories in a catalog * Ability to search for files by name in
+the catalog * Ability to navigate through indexed data Ã  la `ls` * Support for
+fuse to mount the indexed data as a virtual filesystem * Handle archive files
+(zip, tar, ...) and index their content * Save catalog to json for easy
+versioning with git * Command line interface FTW * Store files and directories
+sizes * Store md5 hash of files * Ability to update the catalog * Support for
+`fzf` for finding files * Tag your different storages with additional
+information * Export catalog to CSV [https://asciinema.org/a/
+hRE22qbVtBGxOM1yxw2y4fBy8.png] Quick start: ```bash # install catcli with pip
+pip3 install catcli --user # index a directory in the catalog catcli index --
+meta='some description' log /var/log # display the content catcli ls -r #
+navigate catcli ls log # find files/directories named '*log*' catcli find log
+``` see [usage](#usage) for specific info ## Why catcli? [Catcli](https://
+github.com/deadc0de6/catcli) gives the ability to navigate, explore and find
+your files that are stored on external media (DVDs, hard drives, USB sticks,
+etc) when those are not connected. Catcli can just as easily index any
+arbitrary directories. See the [examples](#examples) for an overview of the
+available features. --- **Table of Contents** * [Installation](#installation) *
+[Usage](#usage) * [Index data](#index-data) * [Index archive files](#index-
+archive-files) * [Walk indexed files with ls](#walk-indexed-files-with-ls) *
+[Find files](#find-files) * [Mount catalog](#mount-catalog) * [Display entire
+hierarchy](#display-entire-hierarchy) * [Catalog graph](#catalog-graph) * [Edit
+storage](#edit-storage) * [Update catalog](#update-catalog) * [CSV format]
+(#csv-format) * [Examples](#examples) * [Contribution](#contribution) * [Thank
+you](#thank-you) # Installation Install from Pypi ```bash $ pip3 install catcli
+--user ``` Or from github directly ```bash $ cd /tmp; git clone https://
+github.com/deadc0de6/catcli && cd catcli $ sudo python3 setup.py install $
+catcli --help ``` To work with catcli without installing it, you can do the
+following ```bash $ cd /tmp; git clone https://github.com/deadc0de6/catcli &&
+cd catcli $ pip3 install -r requirements.txt --user $ python3 -m catcli.catcli
+--help ``` or install it in a virtualenv ```bash $ cd /tmp; git clone https://
+github.com/deadc0de6/catcli && cd catcli $ virtualenv -p python3 env $ source
+env/bin/activate $ python setup.py install $ catcli --help ``` Catcli is also
+available on aur: https://aur.archlinux.org/packages/catcli-git/ # Usage Each
+indexed directory is stored in the catalog. Multiple directories can be indexed
+and they are all available through the command line interface of catcli. Five
+different types of entry are present in a catalog: * **top node**: this is the
+root of the hierarchy * **storage node**: this represents an indexed storage (a
+DVD, an external hard drive, an USB drive, some arbitrary directory, etc). *
+**dir node**: this is a directory * **file node**: this is a file * **archive
+node**: this is a file contained in an archive (tar, zip, etc) ## Index data
+Let's say the DVD or external hard drive that needs to be indexed is mounted on
+`/media/mnt`. The following command will index the entire directory `/media/
+mnt` and store that in your catalog under the name ``. ```bash $ catcli index -
+-meta=  /media/mnt ``` If not specified otherwise (with the switch `--
+catalog`), the catalog is saved in the current directory under
+`catcli.catalog`. The `--meta` switch allows to add any additional information
+to store along in the catalog like for example `the blue disk in my office`.
+Catcli will calculate and store the total size of each node (directories,
+storages, etc) unless the `-n --no-subsize` switch is used. Using the `-a --
+archive` switch allows to also index archive files as explained [below](#index-
+archive-files). ## Index archive files Catcli is able to index and explore the
+content of archive files. Following archive formats are supported: *tar*,
+*tar.gz*, *tar.xz*, *lzma*, *tar.bz2*, *zip*. Catcli is also able to find files
+within indexed archive files. See the [archive example](#archive-example) for
+more. ## Walk indexed files with ls A catalog can be walked using the command
+`ls` as if the media is mounted (File/directories separator is `/`). ```bash $
+catcli ls tmp/a/b/c ``` Resulting files can be sorted by size using `-S --
+sortsize`. See the [examples](#examples) for more. ## Find files Files and
+directories can be found based on their names using the `find` command. `Find`
+support two formats that allow to use `fzf` for searching: * `--format=fzf-
+native`: display the result in native format * `--format=fzf-csv`: display the
+result in csv See the [examples](#examples) for more. ## Mount catalog The
+catalog can be mounted with [fuse](https://www.kernel.org/doc/html/next/
+filesystems/fuse.html) and navigate like any filesystem. ```bash $ mkdir /tmp/
+mnt $ catcli index -c github .github $ catcli mount /tmp/mnt $ ls -laR /tmp/mnt
+drwxrwxrwx - user 8 Mar 22:08 github mnt/github: .rwxrwxrwx 17 user 19 Oct 2022
+FUNDING.yml drwxrwxrwx - user 2 Mar 10:15 workflows mnt/github/workflows:
+.rwxrwxrwx 691 user 19 Oct 2022 pypi-release.yml .rwxrwxrwx 635 user 8 Mar 21:
+08 testing.yml ``` ## Display entire hierarchy The entire catalog can be shown
+using the `ls -r` command. Resulting files can be sorted by size using the `-
+S --sortsize` switch. See the [examples](#examples) for more. ## Catalog graph
+The catalog can be exported in a dot file that can be used to generate a graph
+of the indexed files. ```bash $ catcli graph dot file created under "/tmp/
+catcli.dot" create graph with "dot /tmp/catcli.dot -T png -o /tmp/tree.png"
+(you need graphviz) $ dot /tmp/catcli.dot -T png -o /tmp/tree.png ``` ## Edit
+storage Storage entry can be edited with following catcli commands: * `rename`
+- rename the storage * `edit` - edit storage metadata ## Update catalog The
+catalog can be updated with the `update` command. Updates are based on the
+access time of each of the files and on the hash checksum if present (catalog
+was indexed with `-c --hash` and `update` is called with the switch `-c --
+hash`). ## CSV format Results can be printed to CSV using `--format=csv`.
+Fields are separated by a comma (`,`) and are quoted with double quotes (`"`).
+Each line contains the following fields: * **name**: the entry name * **type**:
+the entry type (file, directory, storage, etc) * **path**: the entry path *
+**size**: the entry size * **indexed_at**: when this entry was indexed *
+**maccess**: the entry modification date/time * **md5**: the entry checksum (if
+any) * **nbfiles**: the number of children (empty for nodes that are not
+storage or directory) * **free_space**: free space (empty for not storage
+nodes) * **total_space**: total space (empty for not storage nodes) * **meta**:
+meta information (empty for not storage nodes) # Examples ## Simple example
+Let's first create some files and directories: ```bash $ mkdir -p /tmp/test/
+{a,b,c} $ echo 'something in files in a' > /tmp/test/a/{1,2,3} $ echo
+'something else in files in b' > /tmp/test/b/{4,5,6} $ echo 'some bytes' > /
+tmp/test/c/{7,8,9} $ tree /tmp/test /tmp/test âââ a âÂ Â  âââ 1
+âÂ Â  âââ 2 âÂ Â  âââ 3 âââ b âÂ Â  âââ 4 âÂ Â 
+âââ 5 âÂ Â  âââ 6 âââ c âââ 7 âââ 8 âââ 9
+3 directories, 9 files ``` First this directory is indexed with `catcli` as if
+it was some kind of external storage: ```bash $ catcli index --meta='my test
+directory' tmptest /tmp/test ``` Catcli creates its catalog file in the current
+directory as `catcli.catalog`. Printing the entire catalog as a tree is done
+with the command `ls -r` ``` $ catcli ls -r top âââ storage: tmptest (my
+test directory) (nbfiles:3, free:3.7G/3.7G, date:2019-01-26 19:59:47) âââ
+a [nbfiles:3, totsize:72] â âââ 1 [size:24] â âââ 2 [size:24]
+â âââ 3 [size:24] âââ b [nbfiles:3, totsize:87] â âââ 4
+[size:29] â âââ 5 [size:29] â âââ 6 [size:29] âââ c
+[nbfiles:3, totsize:33] âââ 7 [size:11] âââ 8 [size:11] âââ 9
+[size:11] ``` The catalog can be walked with `ls` as if it was a normal
+directory ``` $ catcli ls top - storage: tmptest (my test directory) (nbfiles:
+3, free:3.7G/3.7G, date:2019-01-26 19:59:47) $ catcli ls tmptest storage:
+tmptest (my test directory) (nbfiles:3, free:3.7G/3.7G, date:2019-01-26 19:59:
+47) - a [nbfiles:3, totsize:72] - b [nbfiles:3, totsize:87] - c [nbfiles:3,
+totsize:33] $ catcli ls tmptest/b b [nbfiles:3, totsize:87] - 4 [size:29] - 5
+[size:29] - 6 [size:29] ``` And files can be found using the command `find`
+```bash $ catcli find 9 c/9 [size:11, storage:tmptest] ``` When using the `-b -
+-script` switch, a one-liner is generated that allows to handle the found file
+(s) ``` $ catcli find 9 --script c/9 [size:11, storage:tmptest] op=file;
+source=/media/mnt; $op ${source}/c/9 ``` ## Archive example Let's consider a
+directory containing archive files: ```bash $ ls -1 /tmp/catcli catcli-0.3.1
+v0.3.1.tar.gz v0.3.1.zip ``` To enable the indexing of archive contents use the
+`-a --archive` switch ```bash $ catcli index -au some-name /tmp/catcli ``` Then
+any command can be used to explore the catalog as for normal files but, by
 providing the `-a --archive` switch, archive content are displayed. ```bash $
 catcli ls some-name storage: some-name (free:800G, total:1T) - catcli-0.3.1
 [nbfiles:11, totsize:80.5K] - v0.3.1.tar.gz [size:24.2K] - v0.3.1.zip [size:
 31.2K] $ catcli ls -r some-name/v0.3.1.zip v0.3.1.zip [size:31.2K] $ catcli ls
 -ar some-name/v0.3.1.zip v0.3.1.zip [size:31.2K] âââ catcli-0.3.1
 [archive:v0.3.1.zip] â âââ catcli [archive:v0.3.1.zip] â â
 âââ __init__.py [archive:v0.3.1.zip] â â âââ catalog.py
```

### Comparing `catcli-0.9.3/setup.py` & `catcli-0.9.4/setup.py`

 * *Files identical despite different names*

