# Comparing `tmp/sequana_denovo-0.8.5.tar.gz` & `tmp/sequana_denovo-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/sequana_denovo-0.8.5.tar", last modified: Wed Nov 25 22:17:08 2020, max compression
+gzip compressed data, was "sequana_denovo-0.9.0.tar", last modified: Sun May 21 19:55:41 2023, max compression
```

## Comparing `sequana_denovo-0.8.5.tar` & `sequana_denovo-0.9.0.tar`

### file list

```diff
@@ -1,29 +1,28 @@
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2020-11-25 22:17:08.000000 sequana_denovo-0.8.5/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      128 2020-11-25 22:15:06.000000 sequana_denovo-0.8.5/MANIFEST.in
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     6129 2020-11-25 22:17:08.000000 sequana_denovo-0.8.5/PKG-INFO
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4052 2020-11-25 22:15:56.000000 sequana_denovo-0.8.5/README.rst
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       40 2020-11-25 22:15:16.000000 sequana_denovo-0.8.5/requirements.txt
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2020-11-25 22:17:08.000000 sequana_denovo-0.8.5/sequana_denovo.egg-info/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     6129 2020-11-25 22:17:08.000000 sequana_denovo-0.8.5/sequana_denovo.egg-info/PKG-INFO
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      695 2020-11-25 22:17:08.000000 sequana_denovo-0.8.5/sequana_denovo.egg-info/SOURCES.txt
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        1 2020-11-25 22:17:08.000000 sequana_denovo-0.8.5/sequana_denovo.egg-info/dependency_links.txt
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      133 2020-11-25 22:17:08.000000 sequana_denovo-0.8.5/sequana_denovo.egg-info/entry_points.txt
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        1 2020-11-25 22:16:22.000000 sequana_denovo-0.8.5/sequana_denovo.egg-info/not-zip-safe
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       40 2020-11-25 22:17:08.000000 sequana_denovo-0.8.5/sequana_denovo.egg-info/requires.txt
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       18 2020-11-25 22:17:08.000000 sequana_denovo-0.8.5/sequana_denovo.egg-info/top_level.txt
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2020-11-25 22:17:08.000000 sequana_denovo-0.8.5/sequana_pipelines/
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2020-11-25 22:17:08.000000 sequana_denovo-0.8.5/sequana_pipelines/denovo/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      124 2020-06-02 19:53:50.000000 sequana_denovo-0.8.5/sequana_pipelines/denovo/__init__.py
--rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)      326 2020-06-02 19:53:50.000000 sequana_denovo-0.8.5/sequana_pipelines/denovo/cluster_config.json
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     6407 2020-11-25 22:14:50.000000 sequana_denovo-0.8.5/sequana_pipelines/denovo/config.yaml
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    91750 2020-06-02 19:53:50.000000 sequana_denovo-0.8.5/sequana_pipelines/denovo/dag.png
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2020-11-25 22:17:08.000000 sequana_denovo-0.8.5/sequana_pipelines/denovo/data/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        0 2020-06-02 19:53:50.000000 sequana_denovo-0.8.5/sequana_pipelines/denovo/data/__init__.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    11663 2020-11-25 22:05:21.000000 sequana_denovo-0.8.5/sequana_pipelines/denovo/denovo.rules
--rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)     4847 2020-11-25 22:15:06.000000 sequana_denovo-0.8.5/sequana_pipelines/denovo/main.py
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4625 2020-11-25 22:12:02.000000 sequana_denovo-0.8.5/sequana_pipelines/denovo/multiqc_config.yaml
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       81 2020-06-02 19:53:50.000000 sequana_denovo-0.8.5/sequana_pipelines/denovo/requirements.txt
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      252 2020-11-25 22:17:08.000000 sequana_denovo-0.8.5/setup.cfg
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     3285 2020-11-25 22:16:37.000000 sequana_denovo-0.8.5/setup.py
-drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2020-11-25 22:17:08.000000 sequana_denovo-0.8.5/test/
--rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1302 2020-06-02 19:53:50.000000 sequana_denovo-0.8.5/test/test_main.py
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-05-21 19:55:41.222870 sequana_denovo-0.9.0/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1530 2022-11-18 10:29:50.000000 sequana_denovo-0.9.0/LICENSE
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      157 2022-11-18 10:29:50.000000 sequana_denovo-0.9.0/MANIFEST.in
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     6445 2023-05-21 19:55:41.222870 sequana_denovo-0.9.0/PKG-INFO
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     5173 2023-05-21 19:55:29.000000 sequana_denovo-0.9.0/README.rst
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       41 2022-11-18 10:29:50.000000 sequana_denovo-0.9.0/requirements.txt
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-05-21 19:55:41.221871 sequana_denovo-0.9.0/sequana_denovo.egg-info/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     6445 2023-05-21 19:55:41.000000 sequana_denovo-0.9.0/sequana_denovo.egg-info/PKG-INFO
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      651 2023-05-21 19:55:41.000000 sequana_denovo-0.9.0/sequana_denovo.egg-info/SOURCES.txt
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        1 2023-05-21 19:55:41.000000 sequana_denovo-0.9.0/sequana_denovo.egg-info/dependency_links.txt
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       70 2023-05-21 19:55:41.000000 sequana_denovo-0.9.0/sequana_denovo.egg-info/entry_points.txt
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)        1 2023-02-01 21:02:33.000000 sequana_denovo-0.9.0/sequana_denovo.egg-info/not-zip-safe
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      134 2023-05-21 19:55:41.000000 sequana_denovo-0.9.0/sequana_denovo.egg-info/requires.txt
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)       18 2023-05-21 19:55:41.000000 sequana_denovo-0.9.0/sequana_denovo.egg-info/top_level.txt
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-05-21 19:55:41.220870 sequana_denovo-0.9.0/sequana_pipelines/
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-05-21 19:55:41.222870 sequana_denovo-0.9.0/sequana_pipelines/denovo/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      124 2022-11-18 10:29:50.000000 sequana_denovo-0.9.0/sequana_pipelines/denovo/__init__.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     8746 2023-05-17 21:33:03.000000 sequana_denovo-0.9.0/sequana_pipelines/denovo/config.yaml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    91750 2022-11-18 10:29:50.000000 sequana_denovo-0.9.0/sequana_pipelines/denovo/dag.png
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)    18715 2023-05-17 21:33:03.000000 sequana_denovo-0.9.0/sequana_pipelines/denovo/denovo.smk
+-rwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)     5726 2023-05-17 21:33:03.000000 sequana_denovo-0.9.0/sequana_pipelines/denovo/main.py
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     4625 2022-11-18 10:29:50.000000 sequana_denovo-0.9.0/sequana_pipelines/denovo/multiqc_config.yaml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      106 2023-02-01 20:46:18.000000 sequana_denovo-0.9.0/sequana_pipelines/denovo/requirements.txt
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     5669 2023-05-17 21:03:55.000000 sequana_denovo-0.9.0/sequana_pipelines/denovo/schema.yaml
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)      252 2023-05-21 19:55:41.222870 sequana_denovo-0.9.0/setup.cfg
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     2993 2023-05-17 21:33:03.000000 sequana_denovo-0.9.0/setup.py
+drwxrwxr-x   0 cokelaer  (1000) cokelaer  (1000)        0 2023-05-21 19:55:41.222870 sequana_denovo-0.9.0/test/
+-rw-rw-r--   0 cokelaer  (1000) cokelaer  (1000)     1227 2022-11-18 10:29:50.000000 sequana_denovo-0.9.0/test/test_main.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `sequana_denovo-0.8.5/PKG-INFO` & `sequana_denovo-0.9.0/README.rst`

 * *Files 20% similar despite different names*

```diff
@@ -1,141 +1,133 @@
-Metadata-Version: 1.2
-Name: sequana_denovo
-Version: 0.8.5
-Summary: Denovo Assembly from FASTQ files
-Home-page: https://github.com/sequana/
-Author: thomas cokelaer
-Author-email: thomas.cokelaer@pasteur.fr
-Maintainer: thomas cokelaer
-Maintainer-email: thomas.cokelaer@pasteur.fr
-License: new BSD
-Description: This is is the **denovo** pipeline from the `Sequana <https://sequana.readthedocs.org>`_ projet
-        
-        :Overview: a de-novo assembly pipeline for short-read sequencing data
-        :Input: A set of FastQ files
-        :Output: Fasta, VCF, HTML report
-        :Status: production
-        :Citation: Cokelaer et al, (2017), ‘Sequana’: a Set of Snakemake NGS pipelines, Journal of Open Source Software, 2(16), 352, JOSS DOI doi:10.21105/joss.00352
-        
-        
-        Installation
-        ~~~~~~~~~~~~
-        
-        You must install Sequana first::
-        
-            pip install sequana
-        
-        Then, just install this package::
-        
-            pip install sequana_denovo
-        
-        
-        Usage
-        ~~~~~
-        
-        ::
-        
-            sequana_pipelines_denovo --help
-            sequana_pipelines_denovo --input-directory DATAPATH 
-        
-        This creates a directory with the pipeline and configuration file. You will then need 
-        to execute the pipeline::
-        
-            cd denovo
-            sh denovo.sh  # for a local run
-        
-        This launch a snakemake pipeline. If you are familiar with snakemake, you can 
-        retrieve the pipeline itself and its configuration files and then execute the pipeline yourself with specific parameters::
-        
-            snakemake -s denovo.rules -c config.yaml --cores 4 --stats stats.txt
-        
-        Or use `sequanix <https://sequana.readthedocs.io/en/master/sequanix.html>`_ interface.
-        
-        Requirements
-        ~~~~~~~~~~~~
-        
-        This pipelines requires the following executable(s):
-        
-        - spades
-        - busco
-        - bwa
-        - khmer : there is not executable called kmher but a set of executables (.e.g .normalize-by-median.py)
-        - freebayes
-        - picard
-        - prokka
-        - quast
-        - spades
-        - sambamba
-        - samtools
-        
-        
-        
-        .. image:: https://raw.githubusercontent.com/sequana/sequana_denovo/master/sequana_pipelines/denovo/dag.png
-        
-        
-        Details
-        ~~~~~~~~~
-        
-        
-        Snakemake *de-novo* assembly pipeline dedicates to small genome like bacteria.
-        It is based on `SPAdes <http://cab.spbu.ru/software/spades/>`_.
-        The assembler corrects reads and then assemble them using different size of kmer.
-        If the correct option is set, SPAdes corrects mismatches and short INDELs in
-        the contigs using BWA.
-        
-        The sequencing depth can be normalised with `khmer <https://github.com/dib-lab/khmer>`_.
-        Digital normalisation converts the existing high coverage regions into a Gaussian
-        distributions centered around a lower sequencing depth. To put it another way,
-        genome regions covered at 200x will be covered at 20x after normalisation. Thus,
-        some reads from high coverage regions are discarded to reduce the quantity of data.
-        Although the coverage is drastically reduce, the assembly will be as good or better
-        than assembling the unnormalised data. Furthermore, SPAdes with normalised data
-        is notably speeder and cost less memory than without digital normalisation.
-        Above all, khmer does this in fixed, low memory and without any reference
-        sequence needed.
-        
-        The pipeline assess the assembly with several tools and approach. The first one
-        is `Quast <http://quast.sourceforge.net/>`_, a tools for genome assemblies
-        evaluation and comparison. It provides a HTML report with useful metrics like
-        N50, number of mismatch and so on. Furthermore, it creates a viewer of contigs
-        called `Icarus <http://quast.sourceforge.net/icarus.html>`_.
-        
-        The second approach is to characterise coverage with sequana coverage and
-        to detect mismatchs and short INDELs with
-        `Freebayes <https://github.com/ekg/freebayes>`_.
-        
-        The last approach but not the least is `BUSCO <http://busco.ezlab.org/>`_, that
-        provides quantitative measures for the assessment of genome assembly based on
-        expectations of gene content from near-universal single-copy orthologs selected
-        from `OrthoDB <http://www.orthodb.org/>`_.
-        
-        
-        ========= ====================================================================
-        Version   Description
-        ========= ====================================================================
-        0.8.5     * add multiqc and use newest version of sequana
-        0.8.4     * update pipeline to use new pipetools features
-        0.8.3     * fix requirements (spades -> spades.py)
-        0.8.2     * fix readtag, update config to account for new coverage setup
-        0.8.1     
-        0.8.0     **First release.**
-        ========= ====================================================================
-        
-Keywords: snakemake, ngs, denovo, assembly, short read
-Platform: Linux
-Platform: Unix
-Platform: MacOsX
-Platform: Windows
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Education
-Classifier: Intended Audience :: End Users/Desktop
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: BSD License
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Classifier: Topic :: Scientific/Engineering :: Information Analysis
-Classifier: Topic :: Scientific/Engineering :: Mathematics
-Classifier: Topic :: Scientific/Engineering :: Physics
+
+.. image:: https://badge.fury.io/py/sequana-denovo.svg
+     :target: https://pypi.python.org/pypi/sequana_denovo
+
+.. image:: https://github.com/sequana/denovo/actions/workflows/main.yml/badge.svg
+   :target: https://github.com/sequana/denovo/actions/workflows/main.yml
+
+.. image:: https://coveralls.io/repos/github/sequana/denovo/badge.svg?branch=main
+    :target: https://coveralls.io/github/sequana/denovo?branch=main
+
+.. image:: https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C3.10-blue.svg
+    :target: https://pypi.python.org/pypi/sequana
+    :alt: Python 3.8 | 3.9 | 3.10
+
+.. image:: http://joss.theoj.org/papers/10.21105/joss.00352/status.svg
+   :target: http://joss.theoj.org/papers/10.21105/joss.00352
+   :alt: JOSS (journal of open source software) DOI
+
+This is is the **denovo** pipeline from the `Sequana <https://sequana.readthedocs.org>`_ projet
+
+
+:Overview: a de-novo assembly pipeline for short-read sequencing data
+:Input: A set of FastQ files
+:Output: Fasta, VCF, HTML report
+:Status: production
+:Citation: Cokelaer et al, (2017), ‘Sequana’: a Set of Snakemake NGS pipelines, Journal of Open Source Software, 2(16), 352, JOSS DOI doi:10.21105/joss.00352
+
+
+Installation
+~~~~~~~~~~~~
+
+**sequana_denovo** is based on Python3, just install the package as follows::
+
+    pip install sequana --upgrade
+
+You will need third-party software such as fastqc. Please see below for details.
+
+Usage
+~~~~~
+
+The following command will scan all files ending in .fastq.gz found in the local
+directory, create a directory called denovo/ where a snakemake pipeline is
+stored. Depending on the number of files and their sizes, the
+process may be long::
+
+::
+
+    sequana_denovo --help
+    sequana_denovo --input-directory DATAPATH 
+
+This creates a directory with the pipeline and configuration file. You will then need 
+to execute the pipeline::
+
+    cd denovo
+    sh denovo.sh  # for a local run
+
+This launch a snakemake pipeline. If you are familiar with snakemake, you can 
+retrieve the pipeline itself and its configuration files and then execute the pipeline yourself with specific parameters::
+
+    snakemake -s denovo.smk -c config.yaml --cores 4 --stats stats.txt
+
+Or use `sequanix <https://sequana.readthedocs.io/en/main/sequanix.html>`_ interface.
+
+Requirements
+~~~~~~~~~~~~
+
+This pipelines requires the following executable(s):
+
+- spades
+- busco
+- bwa
+- khmer : there is not executable called kmher but a set of executables (.e.g .normalize-by-median.py)
+- freebayes
+- picard
+- prokka
+- quast
+- spades
+- sambamba
+- samtools
+
+
+
+.. image:: https://raw.githubusercontent.com/sequana/sequana_denovo/main/sequana_pipelines/denovo/dag.png
+
+
+Details
+~~~~~~~~~
+
+
+Snakemake *de-novo* assembly pipeline dedicates to small genome like bacteria.
+It is based on `SPAdes <http://cab.spbu.ru/software/spades/>`_.
+The assembler corrects reads and then assemble them using different size of kmer.
+If the correct option is set, SPAdes corrects mismatches and short INDELs in
+the contigs using BWA.
+
+The sequencing depth can be normalised with `khmer <https://github.com/dib-lab/khmer>`_.
+Digital normalisation converts the existing high coverage regions into a Gaussian
+distributions centered around a lower sequencing depth. To put it another way,
+genome regions covered at 200x will be covered at 20x after normalisation. Thus,
+some reads from high coverage regions are discarded to reduce the quantity of data.
+Although the coverage is drastically reduce, the assembly will be as good or better
+than assembling the unnormalised data. Furthermore, SPAdes with normalised data
+is notably speeder and cost less memory than without digital normalisation.
+Above all, khmer does this in fixed, low memory and without any reference
+sequence needed.
+
+The pipeline assess the assembly with several tools and approach. The first one
+is `Quast <http://quast.sourceforge.net/>`_, a tools for genome assemblies
+evaluation and comparison. It provides a HTML report with useful metrics like
+N50, number of mismatch and so on. Furthermore, it creates a viewer of contigs
+called `Icarus <http://quast.sourceforge.net/icarus.html>`_.
+
+The second approach is to characterise coverage with sequana coverage and
+to detect mismatchs and short INDELs with
+`Freebayes <https://github.com/ekg/freebayes>`_.
+
+The last approach but not the least is `BUSCO <http://busco.ezlab.org/>`_, that
+provides quantitative measures for the assessment of genome assembly based on
+expectations of gene content from near-universal single-copy orthologs selected
+from `OrthoDB <http://www.orthodb.org/>`_.
+
+
+========= ====================================================================
+Version   Description
+========= ====================================================================
+0.9.0     * Major refactoring to include apptainers, use wrappers
+0.8.5     * add multiqc and use newest version of sequana
+0.8.4     * update pipeline to use new pipetools features
+0.8.3     * fix requirements (spades -> spades.py)
+0.8.2     * fix readtag, update config to account for new coverage setup
+0.8.1 
+0.8.0     **First release.**
+========= ====================================================================
```

### Comparing `sequana_denovo-0.8.5/sequana_denovo.egg-info/PKG-INFO` & `sequana_denovo-0.9.0/sequana_denovo.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,141 +1,166 @@
-Metadata-Version: 1.2
+Metadata-Version: 2.1
 Name: sequana-denovo
-Version: 0.8.5
+Version: 0.9.0
 Summary: Denovo Assembly from FASTQ files
 Home-page: https://github.com/sequana/
 Author: thomas cokelaer
 Author-email: thomas.cokelaer@pasteur.fr
 Maintainer: thomas cokelaer
 Maintainer-email: thomas.cokelaer@pasteur.fr
 License: new BSD
-Description: This is is the **denovo** pipeline from the `Sequana <https://sequana.readthedocs.org>`_ projet
-        
-        :Overview: a de-novo assembly pipeline for short-read sequencing data
-        :Input: A set of FastQ files
-        :Output: Fasta, VCF, HTML report
-        :Status: production
-        :Citation: Cokelaer et al, (2017), ‘Sequana’: a Set of Snakemake NGS pipelines, Journal of Open Source Software, 2(16), 352, JOSS DOI doi:10.21105/joss.00352
-        
-        
-        Installation
-        ~~~~~~~~~~~~
-        
-        You must install Sequana first::
-        
-            pip install sequana
-        
-        Then, just install this package::
-        
-            pip install sequana_denovo
-        
-        
-        Usage
-        ~~~~~
-        
-        ::
-        
-            sequana_pipelines_denovo --help
-            sequana_pipelines_denovo --input-directory DATAPATH 
-        
-        This creates a directory with the pipeline and configuration file. You will then need 
-        to execute the pipeline::
-        
-            cd denovo
-            sh denovo.sh  # for a local run
-        
-        This launch a snakemake pipeline. If you are familiar with snakemake, you can 
-        retrieve the pipeline itself and its configuration files and then execute the pipeline yourself with specific parameters::
-        
-            snakemake -s denovo.rules -c config.yaml --cores 4 --stats stats.txt
-        
-        Or use `sequanix <https://sequana.readthedocs.io/en/master/sequanix.html>`_ interface.
-        
-        Requirements
-        ~~~~~~~~~~~~
-        
-        This pipelines requires the following executable(s):
-        
-        - spades
-        - busco
-        - bwa
-        - khmer : there is not executable called kmher but a set of executables (.e.g .normalize-by-median.py)
-        - freebayes
-        - picard
-        - prokka
-        - quast
-        - spades
-        - sambamba
-        - samtools
-        
-        
-        
-        .. image:: https://raw.githubusercontent.com/sequana/sequana_denovo/master/sequana_pipelines/denovo/dag.png
-        
-        
-        Details
-        ~~~~~~~~~
-        
-        
-        Snakemake *de-novo* assembly pipeline dedicates to small genome like bacteria.
-        It is based on `SPAdes <http://cab.spbu.ru/software/spades/>`_.
-        The assembler corrects reads and then assemble them using different size of kmer.
-        If the correct option is set, SPAdes corrects mismatches and short INDELs in
-        the contigs using BWA.
-        
-        The sequencing depth can be normalised with `khmer <https://github.com/dib-lab/khmer>`_.
-        Digital normalisation converts the existing high coverage regions into a Gaussian
-        distributions centered around a lower sequencing depth. To put it another way,
-        genome regions covered at 200x will be covered at 20x after normalisation. Thus,
-        some reads from high coverage regions are discarded to reduce the quantity of data.
-        Although the coverage is drastically reduce, the assembly will be as good or better
-        than assembling the unnormalised data. Furthermore, SPAdes with normalised data
-        is notably speeder and cost less memory than without digital normalisation.
-        Above all, khmer does this in fixed, low memory and without any reference
-        sequence needed.
-        
-        The pipeline assess the assembly with several tools and approach. The first one
-        is `Quast <http://quast.sourceforge.net/>`_, a tools for genome assemblies
-        evaluation and comparison. It provides a HTML report with useful metrics like
-        N50, number of mismatch and so on. Furthermore, it creates a viewer of contigs
-        called `Icarus <http://quast.sourceforge.net/icarus.html>`_.
-        
-        The second approach is to characterise coverage with sequana coverage and
-        to detect mismatchs and short INDELs with
-        `Freebayes <https://github.com/ekg/freebayes>`_.
-        
-        The last approach but not the least is `BUSCO <http://busco.ezlab.org/>`_, that
-        provides quantitative measures for the assessment of genome assembly based on
-        expectations of gene content from near-universal single-copy orthologs selected
-        from `OrthoDB <http://www.orthodb.org/>`_.
-        
-        
-        ========= ====================================================================
-        Version   Description
-        ========= ====================================================================
-        0.8.5     * add multiqc and use newest version of sequana
-        0.8.4     * update pipeline to use new pipetools features
-        0.8.3     * fix requirements (spades -> spades.py)
-        0.8.2     * fix readtag, update config to account for new coverage setup
-        0.8.1     
-        0.8.0     **First release.**
-        ========= ====================================================================
-        
 Keywords: snakemake, ngs, denovo, assembly, short read
 Platform: Linux
 Platform: Unix
 Platform: MacOsX
 Platform: Windows
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
+Provides-Extra: testing
+License-File: LICENSE
+
+
+.. image:: https://badge.fury.io/py/sequana-denovo.svg
+     :target: https://pypi.python.org/pypi/sequana_denovo
+
+.. image:: https://github.com/sequana/denovo/actions/workflows/main.yml/badge.svg
+   :target: https://github.com/sequana/denovo/actions/workflows/main.yml
+
+.. image:: https://coveralls.io/repos/github/sequana/denovo/badge.svg?branch=main
+    :target: https://coveralls.io/github/sequana/denovo?branch=main
+
+.. image:: https://img.shields.io/badge/python-3.8%20%7C%203.9%20%7C3.10-blue.svg
+    :target: https://pypi.python.org/pypi/sequana
+    :alt: Python 3.8 | 3.9 | 3.10
+
+.. image:: http://joss.theoj.org/papers/10.21105/joss.00352/status.svg
+   :target: http://joss.theoj.org/papers/10.21105/joss.00352
+   :alt: JOSS (journal of open source software) DOI
+
+This is is the **denovo** pipeline from the `Sequana <https://sequana.readthedocs.org>`_ projet
+
+
+:Overview: a de-novo assembly pipeline for short-read sequencing data
+:Input: A set of FastQ files
+:Output: Fasta, VCF, HTML report
+:Status: production
+:Citation: Cokelaer et al, (2017), ‘Sequana’: a Set of Snakemake NGS pipelines, Journal of Open Source Software, 2(16), 352, JOSS DOI doi:10.21105/joss.00352
+
+
+Installation
+~~~~~~~~~~~~
+
+**sequana_denovo** is based on Python3, just install the package as follows::
+
+    pip install sequana --upgrade
+
+You will need third-party software such as fastqc. Please see below for details.
+
+Usage
+~~~~~
+
+The following command will scan all files ending in .fastq.gz found in the local
+directory, create a directory called denovo/ where a snakemake pipeline is
+stored. Depending on the number of files and their sizes, the
+process may be long::
+
+::
+
+    sequana_denovo --help
+    sequana_denovo --input-directory DATAPATH 
+
+This creates a directory with the pipeline and configuration file. You will then need 
+to execute the pipeline::
+
+    cd denovo
+    sh denovo.sh  # for a local run
+
+This launch a snakemake pipeline. If you are familiar with snakemake, you can 
+retrieve the pipeline itself and its configuration files and then execute the pipeline yourself with specific parameters::
+
+    snakemake -s denovo.smk -c config.yaml --cores 4 --stats stats.txt
+
+Or use `sequanix <https://sequana.readthedocs.io/en/main/sequanix.html>`_ interface.
+
+Requirements
+~~~~~~~~~~~~
+
+This pipelines requires the following executable(s):
+
+- spades
+- busco
+- bwa
+- khmer : there is not executable called kmher but a set of executables (.e.g .normalize-by-median.py)
+- freebayes
+- picard
+- prokka
+- quast
+- spades
+- sambamba
+- samtools
+
+
+
+.. image:: https://raw.githubusercontent.com/sequana/sequana_denovo/main/sequana_pipelines/denovo/dag.png
+
+
+Details
+~~~~~~~~~
+
+
+Snakemake *de-novo* assembly pipeline dedicates to small genome like bacteria.
+It is based on `SPAdes <http://cab.spbu.ru/software/spades/>`_.
+The assembler corrects reads and then assemble them using different size of kmer.
+If the correct option is set, SPAdes corrects mismatches and short INDELs in
+the contigs using BWA.
+
+The sequencing depth can be normalised with `khmer <https://github.com/dib-lab/khmer>`_.
+Digital normalisation converts the existing high coverage regions into a Gaussian
+distributions centered around a lower sequencing depth. To put it another way,
+genome regions covered at 200x will be covered at 20x after normalisation. Thus,
+some reads from high coverage regions are discarded to reduce the quantity of data.
+Although the coverage is drastically reduce, the assembly will be as good or better
+than assembling the unnormalised data. Furthermore, SPAdes with normalised data
+is notably speeder and cost less memory than without digital normalisation.
+Above all, khmer does this in fixed, low memory and without any reference
+sequence needed.
+
+The pipeline assess the assembly with several tools and approach. The first one
+is `Quast <http://quast.sourceforge.net/>`_, a tools for genome assemblies
+evaluation and comparison. It provides a HTML report with useful metrics like
+N50, number of mismatch and so on. Furthermore, it creates a viewer of contigs
+called `Icarus <http://quast.sourceforge.net/icarus.html>`_.
+
+The second approach is to characterise coverage with sequana coverage and
+to detect mismatchs and short INDELs with
+`Freebayes <https://github.com/ekg/freebayes>`_.
+
+The last approach but not the least is `BUSCO <http://busco.ezlab.org/>`_, that
+provides quantitative measures for the assessment of genome assembly based on
+expectations of gene content from near-universal single-copy orthologs selected
+from `OrthoDB <http://www.orthodb.org/>`_.
+
+
+========= ====================================================================
+Version   Description
+========= ====================================================================
+0.9.0     * Major refactoring to include apptainers, use wrappers
+0.8.5     * add multiqc and use newest version of sequana
+0.8.4     * update pipeline to use new pipetools features
+0.8.3     * fix requirements (spades -> spades.py)
+0.8.2     * fix readtag, update config to account for new coverage setup
+0.8.1 
+0.8.0     **First release.**
+========= ====================================================================
```

### Comparing `sequana_denovo-0.8.5/sequana_denovo.egg-info/SOURCES.txt` & `sequana_denovo-0.9.0/sequana_denovo.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,22 @@
+LICENSE
 MANIFEST.in
 README.rst
 requirements.txt
 setup.cfg
 setup.py
 sequana_denovo.egg-info/PKG-INFO
 sequana_denovo.egg-info/SOURCES.txt
 sequana_denovo.egg-info/dependency_links.txt
 sequana_denovo.egg-info/entry_points.txt
 sequana_denovo.egg-info/not-zip-safe
 sequana_denovo.egg-info/requires.txt
 sequana_denovo.egg-info/top_level.txt
 sequana_pipelines/denovo/__init__.py
-sequana_pipelines/denovo/cluster_config.json
 sequana_pipelines/denovo/config.yaml
 sequana_pipelines/denovo/dag.png
-sequana_pipelines/denovo/denovo.rules
+sequana_pipelines/denovo/denovo.smk
 sequana_pipelines/denovo/main.py
 sequana_pipelines/denovo/multiqc_config.yaml
 sequana_pipelines/denovo/requirements.txt
-sequana_pipelines/denovo/data/__init__.py
+sequana_pipelines/denovo/schema.yaml
 test/test_main.py
```

### Comparing `sequana_denovo-0.8.5/sequana_pipelines/denovo/config.yaml` & `sequana_denovo-0.9.0/sequana_pipelines/denovo/config.yaml`

 * *Files 26% similar despite different names*

```diff
@@ -4,220 +4,293 @@
 # ==========================================[ Sections for the users ]========
 #
 # One of input_directory, input_pattern and input_samples must be provided
 # If input_directory provided, use it otherwise if input_pattern provided,
 # use it, otherwise use input_samples.
 # ============================================================================
 #
-input_directory: "%(input_directory)s"
+input_directory: ""
 input_readtag: _R[12]_
-input_pattern: '*fastq.gz'
+input_pattern: "*fastq.gz"
+assembler: "spades"
+
+apptainers:
+  blast: "https://zenodo.org/record/7848524/files/blast_2.12.0.img"
+  bwa: "https://zenodo.org/record/7341710/files/sequana_tools_0.14.5.img"
+  busco: "https://zenodo.org/record/7794877/files/busco_5.4.6.img"
+  digital_normalisation: "https://zenodo.org/record/7341710/files/sequana_tools_0.14.5.img"
+  freebayes: "https://zenodo.org/record/7341710/files/sequana_tools_0.14.5.img"
+  graphviz: "https://zenodo.org/record/7928262/files/graphviz_7.0.5.img"
+  quast: "https://zenodo.org/record/7848771/files/quast_5.2.0.img"
+  prokka: "https://zenodo.org/record/7946774/files/prokka_1.14.6.img"
+  sambamba: "https://zenodo.org/record/7341710/files/sequana_tools_0.14.5.img"
+  samtools: "https://zenodo.org/record/7341710/files/sequana_tools_0.14.5.img"
+  seqkit:  "https://zenodo.org/record/7821924/files/seqkit_2.4.0.img"
+  spades: "https://zenodo.org/record/7341710/files/sequana_tools_0.14.5.img"
+  unicycler: "https://zenodo.org/record/7335176/files/denovo_tools_0.0.2.img"
 
-##############################################################################
-# Sequencing information section
-#
-# :Parameters:
-#
-# - platform: name of the technology.
-# - instrument: name of the instrument.
-# - flowcell: name of the flowcell.
-#
-sequencing:
-    platform: Illumina
-    instrument: Unknown
-    flowcell: Unknown
 
 ##############################################################################
 # Khmer - Digital Normalisation
 #
 # :Parameters:
 #
 # - do: if unchecked, this rule is ignored.
 # - ksize: kmer size used to normalised the coverage.
 # - cutoff: when the median k-mer coverage level is above this number the read
 #       is not kept.
 # - max_memory_usage: maximum amount of memory to use for data structure.
 # - threads: number of threads to be used.
 # - options: any options recognised by normalize-by-median.py.
+# - resources: computing resources needed to run the job on a cluster
 #
 digital_normalisation:
-    do: yes
-    ksize: 20
-    cutoff: 20
-    max_memory_usage: 4e9
-    threads: 4
-    options: ''
+  do: yes
+  ksize: 20
+  cutoff: 20
+  max_memory_usage: 4e9
+  threads: 4
+  options: ""
+
+  resources:
+    mem: 4G
 
 ##############################################################################
 # Spades - De Novo Assembly
-# 
+#
 # :Parameters:
-# 
-# - k: comma-separated list of k-mer sizes (must be odd and less than 128).
-# - careful: tries to reduce number of mismatches and short indels.
-# - only_assembler: runs only assembling (without read error correction).
+#
+# - k: comma-separated list of k-mer sizes (must be odd and less than 128). 
+#      use quote (sequanix requirements)
+# - preset: any preset in this list ["", "meta", "sc", "isolate", "metaplasmid", "metaviral", "rna", "rnaviral"].
+# - options: any options recognised by spades.py.
 # - memory: RAM limit for SPAdes in Gb (terminates if exceeded).
 # - threads: number of threads to be used.
-# - options: any options recognised by spades.py.
-# 
+# - resources: computing resources needed to run the job on a cluster
+#
 spades:
-    k: 21,33,55,77,99,127
-    careful: true
-    only_assembler: false
-    memory: 64
-    threads: 8
-    options: ''
+  k: "21,33,55,77,99,127"
+  preset: ""
+  options: "--careful"
+  memory: 64
+  threads: 8
+  resources:
+    mem: 64G
+
+##############################################################################
+# Unicycler - De Novo Assembly
+#
+# :Parameters:
+#
+# - mode: any bridging mode in this list ["conservative", "normal", "bold"]
+# - options: any options recognised by unicycler.
+# - threads: number of threads to be used.
+# - resources: computing resources needed to run the job on a cluster
+#
+unicycler:
+  mode: "normal"
+  options: ""
+  threads: 8
+  resources:
+    mem: 64G
 
 ##############################################################################
 # Quast - Compute metrics to assess assembly
 #
 # :Parameters:
-# 
-# - reference: Reference genome file (optional).
-# - genes_file: Gene positions in the reference genome.
-# - map_reads: Map reads on reference file.
+#
+# - reference_file: Reference genome file (optional).
+# - annotation_file: Gene positions in the reference genome.
+# - options: any options recognised by quast.
 # - threads: Number of threads to be used.
-# - options: Any options recognised by quast.py.
-# 
+# - resources: computing resources needed to run the job on a cluster - options: Any options recognised by quast.py.
+#
 quast:
-    reference: ''
-    genes_file: ''
-    threads: 4
-    options: ''
+  reference_file: ""
+  annotation_file: ""
+  threads: 4
+  options: ""
 
 ##############################################################################
 # Prokka - Annotate the genome assembly
 #
 # :Parameters:
 #
 # - do: If unchecked, this rule is ignored.
 # - kingdom: Annotation mode (Archaea|Bacteria|Mitochondria|Viruses)
 # - genus: Genus name of the assembly.
 # - species: Species name of the assembly.
 # - threads: Number of threads used by Prokka.
 # - options: Any options recognised by Prokka.
 #
 prokka:
-    do: yes
-    kingdom: Bacteria
-    genus: ""
-    species: ""
+  do: yes
+  kingdom: Bacteria
+  genus: ""
+  species: ""
+  threads: 4
+  options: ""
+
+##############################################################################
+# Busco
+#
+# :Parameters:
+#   
+# - do: if unchecked, this rule is ignored
+# - lineage: Specify the name of the BUSCO lineage to be used.
+# - options: any options recognised by `busco` cli.
+# - threads: Number of threads to use.
+busco:
+    do: false
+    lineage: ''
+    options: '--offline'
     threads: 4
-    options: ""
 
 ##############################################################################
-# Format contigs name and remove contigs with a length lower than a threshold
-# 
+# Seqkit filter
+#
 # :Parameters:
-# 
+#
 # - threshold: when the contig length is lower than this number, the contig
 #       is not kept.
-# 
-format_contigs:
-    threshold: 500
+#
+seqkit_filter:
+  threshold: 500
+
 
 ##############################################################################
 # BWA - Mapping
 #
 # :Parameters:
 #
-# - reference_file: the name of the reference file.
-# - index_algorithm: the BWA index algorithm (is or bwtsw).
+# - index_algorithm: the BWA index algorithm (auto|is|bwtsw|rb2).
 # - options: any options recognised by BWA MEM tool.
 # - threads: number of threads to be used.
 # - tmp_directory: temporary directory
 #
-bwa_mem_assembly:
-    index_algorithm: is
-    options: -T 30
-    threads: 4
-    tmp_directory: ./tmp/
+bwa:
+  index_algorithm: is
+  options: -T 30
+  threads: 4
+  tmp_directory:
 
 ##############################################################################
 # Sambamba - Marks or removes duplicates
 #
 # :Parameters:
 #
 # - do: if unchecked, this rule is ignored.
 # - remove: boolean if you want remove or not duplicated reads.
 # - tmp_directory: set the temporary directory.
 #
 sambamba_markdup:
-    do: true
-    remove: false
-    tmp_directory: ./tmp/
+  do: true
+  remove: false
+  tmp_directory:
 
 ##############################################################################
-# Filter reads with a mapping score lower than an integer 
+# Filter reads with a mapping score lower than an integer
 #
 # :Parameters:
 #
 # - do: if unchecked, this rule is ignored.
 # - threshold: mapping score threshold (between 0 and 60).
 #
 sambamba_filter:
-    do: true
-    threshold: 30
+  do: true
+  threshold: 30
 
 ##############################################################################
-# Sequana coverage - Analyse the coverage of the mapping 
+# Sequana coverage - Analyse the coverage of the mapping
 #
 # :Parameters:
 #
 # - do: if unchecked, this rule is ignored.
 # - k: number of gaussian predicted.
 # - circular: if your genome is circular.
 # - window_size: window size to compute the running median.
 # - low_threshold: threshold to detect low coverage regions.
 # - high_threshold: threshold to detect high coverage regions.
 # - gc_window_size: window size to compute GC content.
 #
 sequana_coverage:
-    do: yes
-    mixture_models: 2
-    circular: false
-    window_size: 40001
-    chunksize: 5000000
-    low_threshold: -4.0
-    high_threshold: 4.0
-    gc_window_size: 201
-    double_threshold: 0.5
-    genbank_file: ''
-    reference_file: ''
-
+  do: yes
+  mixture_models: 2
+  circular: false
+  window_size: 40001
+  chunksize: 5000000
+  low_threshold: -4.0
+  high_threshold: 4.0
+  gc_window_size: 201
+  double_threshold: 0.5
+  resources:
+    mem: 12G
 
 ##############################################################################
 # Freebayes - Variant caller
 #
 # :Parameters:
 #
 # - do: if unchecked, this rule is ignored.
 # - ploidy: set the ploidy of your samples.
 # - options: any options recognised by freebayes.
 #
 freebayes:
-    do: yes
-    ploidy: 1
-    options: ''
+  do: yes
+  ploidy: 1
+  options: ""
 
 ##############################################################################
 # Filter VCF
 #
 # :Parameters:
 #
 # - freebayes_score: threshold for minimum freebayes score.
 # - frequency: threshold for minimum alternative allele frequency.
 # - min_depth: threshold for minimum coverage depth.
 # - forward_depth: threshold for minimum coverage depth of forward strand.
 # - reverse_depth: threshold for minimum coverage depth of reverse strand.
 # - strand_ratio: threshold for minimum strand ratio between 0 and 0.5.
 #
-freebayes_vcf_filter:
-    freebayes_score: 10
-    frequency: 0.7
-    min_depth: 6
-    forward_depth: 3
-    reverse_depth: 3
-    strand_ratio: 0.2
+vcf_filter:
+  freebayes_score: 10
+  frequency: 0.7
+  min_depth: 6
+  forward_depth: 3
+  reverse_depth: 3
+  strand_ratio: 0.2
+
+
+##############################################################################
+# SeqKit Head
+#
+# :Parameters:
+#
+# - n_first: Keep only n first contigs
+seqkit_head:
+  n_first: 100
+
+##############################################################################
+# Blast
+#
+# :Parameters:
+#
+# - do: if unchecked, this rule is ignored
+# - db_dir: Path to BLAST databases.
+# - evalue: Expectation value (E) threshold for saving hits.
+# - options: any options recognised by `blastn` cli (except --outfmt)
+# - threads: Number of threads to use.
+blast:
+  do: false
+  blastdb: ""
+  evalue: "1e-10"
+  outfmt: "6 qseqid sseqid pident length mismatch gapopen qstart qend sstart send evalue bitscore staxids stitle"
+  options: "-max_target_seqs 5"
+  threads: 4
+  resources:
+    mem: 12G
 
 multiqc:
-    options: "-p -f  "
+  options: -p -f
+  modules:
+  input_directory: .
+  config_file: "multiqc_config.yaml"
```

### Comparing `sequana_denovo-0.8.5/sequana_pipelines/denovo/dag.png` & `sequana_denovo-0.9.0/sequana_pipelines/denovo/dag.png`

 * *Files identical despite different names*

### Comparing `sequana_denovo-0.8.5/sequana_pipelines/denovo/main.py` & `sequana_denovo-0.9.0/sequana_pipelines/denovo/main.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,110 +1,132 @@
+#
+#  This file is part of Sequana software
+#
+#  Copyright (c) 2016-2021 - Sequana Development Team
+#
+#  Distributed under the terms of the 3-clause BSD license.
+#  The full license is in the LICENSE file, distributed with this software.
+#
+#  website: https://github.com/sequana/sequana
+#  documentation: http://sequana.readthedocs.io
+#
+##############################################################################
 import sys
 import os
 import argparse
 
 from sequana_pipetools.options import *
+from sequana_pipetools.options import before_pipeline
 from sequana_pipetools.misc import Colors
 from sequana_pipetools.info import sequana_epilog, sequana_prolog
+from sequana_pipetools import SequanaManager
 
 col = Colors()
 
 NAME = "denovo"
 
 
 class Options(argparse.ArgumentParser):
     def __init__(self, prog=NAME, epilog=None):
         usage = col.purple(sequana_prolog.format(**{"name": NAME}))
-        super(Options, self).__init__(usage=usage, prog=prog, description="",
+        super(Options, self).__init__(
+            usage=usage,
+            prog=prog,
+            description="",
             epilog=epilog,
-            formatter_class=argparse.ArgumentDefaultsHelpFormatter
+            formatter_class=argparse.ArgumentDefaultsHelpFormatter,
         )
 
         # add a new group of options to the parser
-        so = SlurmOptions()
+        so = SlurmOptions(memory=8000, profile="local")
         so.add_options(self)
 
         # add a snakemake group of options to the parser
         so = SnakemakeOptions(working_directory=NAME)
         so.add_options(self)
 
+        # add a data group of options to the parser
         so = InputOptions()
         so.add_options(self)
 
         so = GeneralOptions()
         so.add_options(self)
 
         pipeline_group = self.add_argument_group("pipeline")
         pipeline_group.add_argument("--quast-reference", default=None, type=str)
 
         pipeline_group = self.add_argument_group("section_prokka")
         pipeline_group.add_argument("--skip-prokka", action="store_true")
-        pipeline_group.add_argument("--prokka-kingdom", default="Bacteria",
-            type=str, choices=["Archaea", "Mitochondria", "Viruses", "Bacteria"])
+        pipeline_group.add_argument(
+            "--prokka-kingdom", default="Bacteria", type=str, choices=["Archaea", "Mitochondria", "Viruses", "Bacteria"]
+        )
 
         pipeline_group = self.add_argument_group("section_sequana_coverage")
         pipeline_group.add_argument("--sequana-coverage-circular", action="store_true")
 
         pipeline_group = self.add_argument_group("section_freebayes")
         pipeline_group.add_argument("--freebayes-ploidy", default=1)
 
         pipeline_group = self.add_argument_group("section_spades")
-        pipeline_group.add_argument("--spades-memory", default=64, 
-            help="max memory to be used in Gb")
+        pipeline_group.add_argument("--spades-memory", default=64, help="max memory to be used in Gb")
 
         pipeline_group = self.add_argument_group("section_digital_normalisation")
-        pipeline_group.add_argument("--digital-normalisation-max-memory-usage", 
-            default=4e9, 
-            help="maximum amount of memory to use for data  normalisation")
+        pipeline_group.add_argument(
+            "--digital-normalisation-max-memory-usage",
+            default=4e9,
+            help="maximum amount of memory to use for data  normalisation",
+        )
+
+        self.add_argument("--run", default=False, action="store_true",
+            help="execute the pipeline directly")
 
     def parse_args(self, *args):
         args_list = list(*args)
         if "--from-project" in args_list:
-            if len(args_list)>2:
-                msg = "WARNING [sequana]: With --from-project option, " + \
-                        "pipeline and data-related options will be ignored."
+            if len(args_list) > 2:
+                msg = (
+                    "WARNING [sequana]: With --from-project option, "
+                    + "pipeline and data-related options will be ignored."
+                )
                 print(col.error(msg))
             for action in self._actions:
                 if action.required is True:
                     action.required = False
         options = super(Options, self).parse_args(*args)
         return options
 
 
 def main(args=None):
 
     if args is None:
         args = sys.argv
 
     # whatever needs to be called by all pipeline before the options parsing
-    from sequana_pipetools.options import before_pipeline
     before_pipeline(NAME)
 
     # option parsing including common epilog
     options = Options(NAME, epilog=sequana_epilog).parse_args(args[1:])
 
-
-    from sequana.pipelines_common import SequanaManager
+    # use profile slurm if user set a slurm queue
+    if options.slurm_queue != "common":
+        options.profile = "slurm"
 
     # the real stuff is here
     manager = SequanaManager(options, NAME)
 
     # create the beginning of the command and the working directory
     manager.setup()
 
     # fill the config file with input parameters
     if options.from_project is None:
         cfg = manager.config.config
-        # EXAMPLE TOREPLACE WITH YOUR NEEDS
         cfg.input_directory = os.path.abspath(options.input_directory)
         cfg.input_pattern = options.input_pattern
         cfg.input_readtag = options.input_readtag
 
-        #manager.exists(cfg.general.reference_file)
-
         # ---------------------------------------------------- freebayes
         cfg.freebayes.ploidy = options.freebayes_ploidy
 
         # ----------------------------------------------------- quast
         if options.quast_reference:
             cfg.quast.reference = os.path.abspath(options.quast_reference)
 
@@ -117,18 +139,21 @@
 
         # ------------------------------------------------------ coverage
         if options.sequana_coverage_circular:
             cfg.sequana_coverage.circular = options.sequana_coverage_circular
 
         # ---------------------------------------------------------- spades
         cfg.spades.memory = options.spades_memory
+        cfg.spades.resources.mem = f"{options.spades_memory}G"
 
         # -------------------------------------------- digital normalisation
         cfg.digital_normalisation.max_memory_usage = options.digital_normalisation_max_memory_usage
 
     # finalise the command and save it; copy the snakemake. update the config
     # file and save it.
     manager.teardown()
 
+    if options.run:
+        subprocess.Popen(["sh", '{}.sh'.format(NAME)], cwd=options.workdir)
 
 if __name__ == "__main__":
     main()
```

### Comparing `sequana_denovo-0.8.5/sequana_pipelines/denovo/multiqc_config.yaml` & `sequana_denovo-0.9.0/sequana_pipelines/denovo/multiqc_config.yaml`

 * *Files identical despite different names*

### Comparing `sequana_denovo-0.8.5/setup.py` & `sequana_denovo-0.9.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,60 +2,47 @@
 # License: 3-clause BSD
 from setuptools import setup, find_namespace_packages
 from setuptools.command.develop import develop
 from setuptools.command.install import install
 import subprocess
 
 _MAJOR               = 0
-_MINOR               = 8
-_MICRO               = 5
+_MINOR               = 9
+_MICRO               = 0
 version              = '%d.%d.%d' % (_MAJOR, _MINOR, _MICRO)
 release              = '%d.%d' % (_MAJOR, _MINOR)
 
 metainfo = {
     'authors': {"main": ("thomas cokelaer", "thomas.cokelaer@pasteur.fr")},
     'version': version,
     'license' : 'new BSD',
     'url' : "https://github.com/sequana/",
     'description': "Denovo Assembly from FASTQ files" ,
     'platforms' : ['Linux', 'Unix', 'MacOsX', 'Windows'],
     'keywords' : ['snakemake, ngs, denovo, assembly, short read'],
     'classifiers' : [
-          #'Development Status :: 4 - Beta',
           'Development Status :: 5 - Production/Stable',
           'Intended Audience :: Education',
           'Intended Audience :: End Users/Desktop',
           'Intended Audience :: Developers',
           'Intended Audience :: Science/Research',
           'License :: OSI Approved :: BSD License',
           'Operating System :: OS Independent',
-          'Programming Language :: Python :: 3.5',
-          'Programming Language :: Python :: 3.6',
+          'Programming Language :: Python :: 3.7',
+          'Programming Language :: Python :: 3.8',
+          'Programming Language :: Python :: 3.9',
           'Topic :: Software Development :: Libraries :: Python Modules',
           'Topic :: Scientific/Engineering :: Bio-Informatics',
           'Topic :: Scientific/Engineering :: Information Analysis',
           'Topic :: Scientific/Engineering :: Mathematics',
           'Topic :: Scientific/Engineering :: Physics']
     }
 
 NAME = "denovo"
 
-class Install(install):
-    def run(self):
-        cmd = "sequana_completion --name {} --force ".format(NAME)
-        try: subprocess.run(cmd.split())
-        except:pass
-        install.run(self)
-
-class Develop(develop):
-    def run(self):
-        cmd = "sequana_completion --name {} --force ".format(NAME)
-        try:subprocess.run(cmd.split())
-        except:pass
-        develop.run(self)
 
 setup(
     name             = "sequana_{}".format(NAME),
     version          = version,
     maintainer       = metainfo['authors']['main'][0],
     maintainer_email = metainfo['authors']['main'][1],
     author           = metainfo['authors']['main'][0],
@@ -65,27 +52,34 @@
     description      = metainfo['description'],
     license          = metainfo['license'],
     platforms        = metainfo['platforms'],
     url              = metainfo['url'],
     classifiers      = metainfo['classifiers'],
 
     # package installation
-    packages = ["sequana_pipelines.denovo",
-        'sequana_pipelines.denovo.data' ],
+    packages = ["sequana_pipelines.denovo",],
 
     install_requires = open("requirements.txt").read(),
-
+    extras_require={
+        "testing": [
+            "pytest",
+            "pytest-cov",
+            "pytest-xdist",
+            "pytest-mock",
+            "pytest-timeout",
+            "pytest-runner",
+            "coveralls",
+        ],
+    },
     # This is recursive include of data files
     exclude_package_data = {"": ["__pycache__"]},
     package_data = {
-        '': ['*.yaml', "*.rules", "*.json", "requirements.txt", "*png"],
-        'sequana_pipelines.denovo.data' : ['*.*'], 
-        },
+        '': ['*.yaml', "*.rules", "*.json", "requirements.txt", "*png", "*.yml", "*.smk"],
+    },
 
     zip_safe=False,
 
     entry_points = {'console_scripts':[
-        'sequana_pipelines_denovo=sequana_pipelines.denovo.main:main',
         'sequana_denovo=sequana_pipelines.denovo.main:main']
     }
 
 )
```

### Comparing `sequana_denovo-0.8.5/test/test_main.py` & `sequana_denovo-0.9.0/test/test_main.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,45 +1,45 @@
 import easydev
 import os
 import tempfile
 import subprocess
 import sys
-from sequana.pipelines_common import get_pipeline_location as getpath
 
-sharedir = getpath('denovo')
+from . import test_dir
 
+sharedir = test_dir + "/data"
 
 def test_standalone_subprocess():
     directory = tempfile.TemporaryDirectory()
-    cmd = """sequana_pipelines_denovo --input-directory {}
+    cmd = """sequana_denovo --input-directory {}
           --working-directory --force""".format(sharedir, directory.name)
     subprocess.call(cmd.split())
 
 
 def test_standalone_script():
     directory = tempfile.TemporaryDirectory()
     import sequana_pipelines.denovo.main as m
     sys.argv = ["test", "--input-directory", sharedir, "--working-directory",
         directory.name, "--force"]
     m.main()
 
-def test_full():
+def _test_full():
 
     with tempfile.TemporaryDirectory() as directory:
         print(directory)
         wk = directory
 
-        cmd = "sequana_pipelines_denovo --input-directory {} "
+        cmd = "sequana_denovo --input-directory {} "
         cmd += "--working-directory {}  --force "
         cmd +=" --digital-normalisation-max-memory-usage 1e9"
         cmd +=" --skip-prokka"
         cmd = cmd.format(sharedir, wk)
         subprocess.call(cmd.split())
 
         stat = subprocess.call("sh denovo.sh".split(), cwd=wk)
 
         assert os.path.exists(wk + "/report_data/summary.html")
 
 def test_version():
-    cmd = "sequana_pipelines_denovo --version"
+    cmd = "sequana_denovo --version"
     subprocess.call(cmd.split())
```

