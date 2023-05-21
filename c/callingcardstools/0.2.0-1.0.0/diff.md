# Comparing `tmp/callingcardstools-0.2.0.tar.gz` & `tmp/callingcardstools-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "callingcardstools-0.2.0.tar", max compression
+gzip compressed data, was "callingcardstools-1.0.0.tar", max compression
```

## Comparing `callingcardstools-0.2.0.tar` & `callingcardstools-1.0.0.tar`

### file list

```diff
@@ -1,44 +1,40 @@
--rw-r--r--   0        0        0     1309 2022-10-31 18:01:58.218668 callingcardstools-0.2.0/LICENSE
--rw-r--r--   0        0        0     1607 2023-04-30 11:24:56.122405 callingcardstools-0.2.0/README.md
--rw-r--r--   0        0        0    13535 2023-04-30 11:24:56.122405 callingcardstools-0.2.0/callingcardstools/Alignment/AlignmentTagger.py
--rw-r--r--   0        0        0     4857 2023-04-30 11:24:56.122405 callingcardstools-0.2.0/callingcardstools/Alignment/SummaryParser.py
--rw-r--r--   0        0        0        0 2023-04-30 11:24:56.122405 callingcardstools-0.2.0/callingcardstools/Alignment/__init__.py
--rw-r--r--   0        0        0    12786 2023-05-19 17:42:53.279362 callingcardstools-0.2.0/callingcardstools/Alignment/mammals/Qbed.py
--rw-r--r--   0        0        0        0 2023-04-30 11:24:56.126405 callingcardstools-0.2.0/callingcardstools/Alignment/mammals/__init__.py
--rw-r--r--   0        0        0     4252 2023-05-19 18:02:51.599306 callingcardstools-0.2.0/callingcardstools/Alignment/mammals/combine_qc.py
--rw-r--r--   0        0        0    10112 2023-05-19 23:12:04.741087 callingcardstools-0.2.0/callingcardstools/Alignment/mammals/process_alignments.py
--rw-r--r--   0        0        0        0 2023-04-30 11:24:56.126405 callingcardstools-0.2.0/callingcardstools/Alignment/yeast/__init__.py
--rw-r--r--   0        0        0     6608 2023-04-30 11:24:56.126405 callingcardstools-0.2.0/callingcardstools/Alignment/yeast/legacy_makeccf.py
--rw-r--r--   0        0        0    11493 2023-05-06 17:03:46.674557 callingcardstools-0.2.0/callingcardstools/Alignment/yeast/process_alignments.py
--rw-r--r--   0        0        0    21657 2023-05-01 15:47:53.191669 callingcardstools-0.2.0/callingcardstools/BarcodeParser/BarcodeParser.py
--rw-r--r--   0        0        0        0 2023-04-30 11:24:56.126405 callingcardstools-0.2.0/callingcardstools/BarcodeParser/__init__.py
--rw-r--r--   0        0        0     2926 2023-04-30 11:24:56.126405 callingcardstools-0.2.0/callingcardstools/BarcodeParser/barcode_table_to_json.py
--rw-r--r--   0        0        0    10201 2023-05-19 17:20:46.908446 callingcardstools-0.2.0/callingcardstools/BarcodeParser/mammals/BarcodeQcCounter.py
--rw-r--r--   0        0        0        0 2023-05-17 01:18:35.723595 callingcardstools-0.2.0/callingcardstools/BarcodeParser/mammals/__init__.py
--rw-r--r--   0        0        0    16927 2023-05-19 01:02:55.853641 callingcardstools-0.2.0/callingcardstools/BarcodeParser/yeast/BarcodeQcCounter.py
--rw-r--r--   0        0        0       46 2023-05-01 17:33:43.247752 callingcardstools-0.2.0/callingcardstools/BarcodeParser/yeast/__init__.py
--rw-r--r--   0        0        0     4176 2023-05-16 01:30:55.105162 callingcardstools-0.2.0/callingcardstools/BarcodeParser/yeast/combine_qc.py
--rw-r--r--   0        0        0     4089 2023-05-15 17:07:35.496631 callingcardstools-0.2.0/callingcardstools/QC/StatusFlags.py
--rw-r--r--   0        0        0       61 2023-04-30 11:24:56.130406 callingcardstools-0.2.0/callingcardstools/QC/__init__.py
--rw-r--r--   0        0        0     4687 2023-05-06 03:13:36.036149 callingcardstools-0.2.0/callingcardstools/QC/create_status_coder.py
--rw-r--r--   0        0        0     9398 2023-04-30 11:24:56.130406 callingcardstools-0.2.0/callingcardstools/Reads/ReadParser.py
--rw-r--r--   0        0        0        0 2023-04-30 11:24:56.130406 callingcardstools-0.2.0/callingcardstools/Reads/__init__.py
--rw-r--r--   0        0        0    13817 2023-04-30 11:24:56.130406 callingcardstools-0.2.0/callingcardstools/Reads/legacy_split_fastq.py
--rw-r--r--   0        0        0    11471 2023-05-14 12:33:07.536131 callingcardstools-0.2.0/callingcardstools/Reads/split_fastq.py
--rw-r--r--   0        0        0     1064 2023-04-30 11:24:56.130406 callingcardstools-0.2.0/callingcardstools/Resources/PackageResources.py
--rw-r--r--   0        0        0       39 2023-04-30 11:24:56.134406 callingcardstools-0.2.0/callingcardstools/Resources/__init__.py
--rw-r--r--   0        0        0        0 2023-04-30 11:24:56.134406 callingcardstools-0.2.0/callingcardstools/Resources/human/__init__.py
--rw-r--r--   0        0        0     1508 2023-05-17 01:24:11.351142 callingcardstools-0.2.0/callingcardstools/Resources/human/barcode_details.json
--rw-r--r--   0        0        0     1219 2023-04-30 11:24:56.134406 callingcardstools-0.2.0/callingcardstools/Resources/human/chr_map.csv
--rw-r--r--   0        0        0        0 2023-04-30 11:24:56.134406 callingcardstools-0.2.0/callingcardstools/Resources/mouse/__init__.py
--rw-r--r--   0        0        0     1509 2023-04-30 11:24:56.134406 callingcardstools-0.2.0/callingcardstools/Resources/mouse/barcode_details.json
--rw-r--r--   0        0        0     2445 2023-04-30 11:24:56.134406 callingcardstools-0.2.0/callingcardstools/Resources/yeast/README.md
--rw-r--r--   0        0        0        0 2023-04-30 11:24:56.134406 callingcardstools-0.2.0/callingcardstools/Resources/yeast/__init__.py
--rw-r--r--   0        0        0     1315 2023-05-01 14:38:21.613557 callingcardstools-0.2.0/callingcardstools/Resources/yeast/barcode_details.json
--rw-r--r--   0        0        0 12689408 2023-04-30 11:24:56.278411 callingcardstools-0.2.0/callingcardstools/Resources/yeast/yeast.db
--rw-r--r--   0        0        0        1 2023-04-30 11:24:56.278411 callingcardstools-0.2.0/callingcardstools/__init__.py
--rw-r--r--   0        0        0     6389 2023-05-19 18:05:32.236311 callingcardstools-0.2.0/callingcardstools/__main__.py
--rw-r--r--   0        0        0     1994 2023-04-30 11:24:56.278411 callingcardstools-0.2.0/callingcardstools/utils.py
--rw-r--r--   0        0        0     1941 2023-05-19 23:13:40.505603 callingcardstools-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3054 1970-01-01 00:00:00.000000 callingcardstools-0.2.0/setup.py
--rw-r--r--   0        0        0     2599 1970-01-01 00:00:00.000000 callingcardstools-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1309 2022-10-31 18:01:58.218668 callingcardstools-1.0.0/LICENSE
+-rw-r--r--   0        0        0     1607 2023-05-21 18:24:18.687643 callingcardstools-1.0.0/README.md
+-rw-r--r--   0        0        0    13738 2023-05-21 18:24:18.687643 callingcardstools-1.0.0/callingcardstools/Alignment/AlignmentTagger.py
+-rw-r--r--   0        0        0     5289 2023-05-21 18:24:18.687643 callingcardstools-1.0.0/callingcardstools/Alignment/SummaryParser.py
+-rw-r--r--   0        0        0        0 2023-05-21 18:24:18.687643 callingcardstools-1.0.0/callingcardstools/Alignment/__init__.py
+-rw-r--r--   0        0        0    12666 2023-05-21 18:24:18.687643 callingcardstools-1.0.0/callingcardstools/Alignment/mammals/Qbed.py
+-rw-r--r--   0        0        0        0 2023-05-21 18:24:18.687643 callingcardstools-1.0.0/callingcardstools/Alignment/mammals/__init__.py
+-rw-r--r--   0        0        0     4252 2023-05-21 18:24:18.687643 callingcardstools-1.0.0/callingcardstools/Alignment/mammals/combine_qc.py
+-rw-r--r--   0        0        0    10112 2023-05-21 18:24:18.687643 callingcardstools-1.0.0/callingcardstools/Alignment/mammals/process_alignments.py
+-rw-r--r--   0        0        0        0 2023-05-21 18:24:18.687643 callingcardstools-1.0.0/callingcardstools/Alignment/yeast/__init__.py
+-rw-r--r--   0        0        0     6608 2023-05-21 18:24:18.687643 callingcardstools-1.0.0/callingcardstools/Alignment/yeast/legacy_makeccf.py
+-rw-r--r--   0        0        0    11462 2023-05-21 18:24:18.687643 callingcardstools-1.0.0/callingcardstools/Alignment/yeast/process_alignments.py
+-rw-r--r--   0        0        0    21855 2023-05-21 18:24:18.687643 callingcardstools-1.0.0/callingcardstools/BarcodeParser/BarcodeParser.py
+-rw-r--r--   0        0        0        0 2023-05-21 18:24:18.687643 callingcardstools-1.0.0/callingcardstools/BarcodeParser/__init__.py
+-rw-r--r--   0        0        0     9774 2023-05-21 18:24:18.687643 callingcardstools-1.0.0/callingcardstools/BarcodeParser/mammals/BarcodeQcCounter.py
+-rw-r--r--   0        0        0        0 2023-05-21 18:24:18.687643 callingcardstools-1.0.0/callingcardstools/BarcodeParser/mammals/__init__.py
+-rw-r--r--   0        0        0    16875 2023-05-21 18:24:18.687643 callingcardstools-1.0.0/callingcardstools/BarcodeParser/yeast/BarcodeQcCounter.py
+-rw-r--r--   0        0        0       46 2023-05-21 18:24:18.687643 callingcardstools-1.0.0/callingcardstools/BarcodeParser/yeast/__init__.py
+-rw-r--r--   0        0        0     3330 2023-05-21 18:24:18.687643 callingcardstools-1.0.0/callingcardstools/BarcodeParser/yeast/barcode_table_to_json.py
+-rw-r--r--   0        0        0     4151 2023-05-21 18:24:18.687643 callingcardstools-1.0.0/callingcardstools/BarcodeParser/yeast/combine_qc.py
+-rw-r--r--   0        0        0     4575 2023-05-21 18:24:18.687643 callingcardstools-1.0.0/callingcardstools/QC/StatusFlags.py
+-rw-r--r--   0        0        0       61 2023-05-21 18:24:18.687643 callingcardstools-1.0.0/callingcardstools/QC/__init__.py
+-rw-r--r--   0        0        0     5176 2023-05-21 18:24:18.687643 callingcardstools-1.0.0/callingcardstools/QC/create_status_coder.py
+-rw-r--r--   0        0        0    10262 2023-05-21 18:24:18.687643 callingcardstools-1.0.0/callingcardstools/Reads/ReadParser.py
+-rw-r--r--   0        0        0        0 2023-05-21 18:24:18.687643 callingcardstools-1.0.0/callingcardstools/Reads/__init__.py
+-rw-r--r--   0        0        0    13792 2023-05-21 18:24:18.687643 callingcardstools-1.0.0/callingcardstools/Reads/legacy_split_fastq.py
+-rw-r--r--   0        0        0    11439 2023-05-21 18:24:18.687643 callingcardstools-1.0.0/callingcardstools/Reads/split_fastq.py
+-rw-r--r--   0        0        0      948 2023-05-21 18:24:18.687643 callingcardstools-1.0.0/callingcardstools/Resources/Resources.py
+-rw-r--r--   0        0        0       32 2023-05-21 18:24:18.691643 callingcardstools-1.0.0/callingcardstools/Resources/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-21 18:24:18.691643 callingcardstools-1.0.0/callingcardstools/Resources/mammals/__init__.py
+-rw-r--r--   0        0        0     1508 2023-05-21 18:24:18.691643 callingcardstools-1.0.0/callingcardstools/Resources/mammals/barcode_details.json
+-rw-r--r--   0        0        0       77 2023-05-21 18:24:18.691643 callingcardstools-1.0.0/callingcardstools/Resources/yeast/README.md
+-rw-r--r--   0        0        0        0 2023-05-21 18:24:18.691643 callingcardstools-1.0.0/callingcardstools/Resources/yeast/__init__.py
+-rw-r--r--   0        0        0     1315 2023-05-21 18:24:18.691643 callingcardstools-1.0.0/callingcardstools/Resources/yeast/barcode_details.json
+-rw-r--r--   0        0        0        0 2023-05-21 18:24:18.691643 callingcardstools-1.0.0/callingcardstools/__init__.py
+-rw-r--r--   0        0        0     6430 2023-05-21 18:24:18.691643 callingcardstools-1.0.0/callingcardstools/__main__.py
+-rw-r--r--   0        0        0     1994 2023-05-21 18:24:18.691643 callingcardstools-1.0.0/callingcardstools/utils.py
+-rw-r--r--   0        0        0     1941 2023-05-21 18:25:53.650604 callingcardstools-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0     3018 1970-01-01 00:00:00.000000 callingcardstools-1.0.0/setup.py
+-rw-r--r--   0        0        0     2599 1970-01-01 00:00:00.000000 callingcardstools-1.0.0/PKG-INFO
```

### Comparing `callingcardstools-0.2.0/LICENSE` & `callingcardstools-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.2.0/README.md` & `callingcardstools-1.0.0/README.md`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.2.0/callingcardstools/Alignment/AlignmentTagger.py` & `callingcardstools-1.0.0/callingcardstools/Alignment/AlignmentTagger.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,37 +6,37 @@
 # outside dependencies
 import pysam
 # local dependendecies
 from callingcardstools.BarcodeParser.BarcodeParser import BarcodeParser
 
 __all__ = ['AlignmentTagger']
 
-logging.getLogger(__name__).addHandler(logging.NullHandler())
+logger = logging.getLogger(__name__)
 
 
 class AlignmentTagger(BarcodeParser):
     """Given an indexed fasta file (genome), id length and insertion length,
     this object can returned a read tagged with the RG, XS and XZ tags"""
 
     _fasta = ""
     _genome = ""
 
     def __init__(self, barcode_details_json: str, fasta_path: str) -> None:
-        """Create an AlignmentTagger object to facilitate adding tags to 
-        alignments and quantifying the number of hops
+        """Initializes the AlignmentTagger object with given barcode 
+        details and a fasta file.
 
         Args:
-            barcode_details_json (str): path to a json file containing
-            barcode details
-            fasta_path (str): path to the genome fasta file. Note that a fai
-             index file created by samtools faidx must
-            exist at the same location.
+            barcode_details_json (str): The path to a JSON file containing 
+                barcode details.
+            fasta_path (str): The path to the genome fasta file. A .fai index 
+                file created by samtools faidx must exist at the same location.
 
-        Returns:
-            AlignmentTagger object
+        Raises:
+            FileNotFoundError: Raised if the path to the fasta file or its
+                index file doesn't exist.
         """
         super().__init__(barcode_details_json)
         self.fasta = fasta_path
         # open the fasta file as a pysam.FastaFile obj
         self.open()
 
     def __del__(self):
@@ -91,24 +91,24 @@
 
     def extract_tag_dict(self, id: str) -> dict:
         """given an id string created by ReadParser, parse into a dictionary of
         tags
 
         Args:
             id (str): id line from a given read in a bam produced from a fastq
-            processed by (a script that uses) the ReadParser
+                processed by (a script that uses) the ReadParser
 
         Raises:
             IndexError: Raised if parsing of the id doesn't work as expected
 
         Returns:
             dict: For example, the id line
-            MN00200:647:000H533KW:1:11102:20080:1075_RT-AATTCACTACGTCAACA;RS-TaqAI;TF-ERT1
-            would be returned as
-             {'RT': 'AATTCACTACGTCAACA', 'RS': 'TaqAI', 'TF': 'ERT1'}
+                MN00200:647:000H533KW:1:11102:20080:1075_RT-AATTCACTACGTCAACA;RS-TaqAI;TF-ERT1
+                would be returned as 
+                {'RT': 'AATTCACTACGTCAACA', 'RS': 'TaqAI', 'TF': 'ERT1'}
         """
         try:
             tag_str = id.split('_')[1]
         except IndexError as exc:
             raise IndexError('No read ID present -- '
                              'expecting a string appended to the read '
                              'ID with a _ in the bam') from exc
@@ -120,47 +120,50 @@
                              f'should have format similar to '
                              f'RT-AATTCACTACGTCAACA;RS-TaqAI;TF-ERT1 where '
                              f'different tags are delimited by ; and '
                              f'tag-value pairs are delimited by - ') \
                 from exc
         return tag_dict
 
-    def tag_read(self, read, decompose_barcode: bool = True):
+    def tag_read(self, read, decompose_barcode: bool = True) -> dict:
         """given a AlignedSegment object, add RG, XS and XZ tags
 
         Args:
             read (AlignedSegment): An aligned segment object -- eg returned
-              in a for loop by interating over bam.fetch() object from pysam
+                in a for loop by interating over bam.fetch() object from pysam
             decompose_barcode (bool): if the barcode is appended as a
-             read identifer on the bam id line, rather than an already
-              decomposed tag string, then extract the barcode and evaluate 
-              it against expectations in the barcode_details json.
-              Default to True.
+                read identifer on the bam id line, rather than an already
+                decomposed tag string, then extract the barcode and evaluate 
+                it against expectations in the barcode_details json.
+                Default to True.
 
         Raises:
+            IndexError: Raised if no read ID is present.
             TypeError: Raised with the cigarstring is not parse-able in a
-             given read
+                given read
             ValueError: Raised when the insertion sequence indicies
-             are out of bounds
+                are out of bounds
 
         Returns:
-            AlignedSegment: The same read, but with RG, XS and XZ tags added
+            dict: A dictionary with key:value pairs
+                {'read': tagged_read, 'barcode_details': dictionary of barcode
+                detals}
         """
-        logging.debug(read.query_name)
+        logger.debug(read.query_name)
         # instantiate some dict objects
         tag_dict = dict()
         barcode_dict = dict()
 
         # decompose_barcode determines whether the function expects to see
         # an undecomposed barcode string in the id location of the read.id
         # or an already parsed barcode string
         if decompose_barcode:
             try:
                 tag_str = read.query_name.split('_')[1]
-                logging.debug(tag_str)
+                logger.debug(tag_str)
             except IndexError as exc:
                 raise IndexError('No read ID present -- '
                                  'expecting a string appended to the read '
                                  'ID with a _ in the bam') from exc
             barcode_dict = self.decompose_barcode(tag_str)
             for k, v in barcode_dict['details'].items():
                 bam_tag = v.get('bam_tag', None)
```

### Comparing `callingcardstools-0.2.0/callingcardstools/Alignment/SummaryParser.py` & `callingcardstools-1.0.0/callingcardstools/Alignment/SummaryParser.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,167 +1,168 @@
 # pylint:disable=W1203
 # standard library
 import os
 import logging
+from typing import Union
 
 # outside library
 import pandas as pd
 
-logging.getLogger(__name__).addHandler(logging.NullHandler())
+logger = logging.getLogger(__name__)
 
 __all__ = ['SummaryParser']
 
 
 class SummaryParser():
+    """
+    Class to parse summary data with provided grouping and ordering parameters.
+    Able to convert this data into qBED format, a variant of the 
+    BED format.
+    """
 
     _query_string = "status == 0"
 
     _summary_columns = {'id': str, 'status': int, 'mapq': int, 'flag': int, 'chr': str,
                         'strand': str, 'five_prime': str, 'insert_start': str,
                         'insert_stop': str, 'insert_seq': str, 'depth': int}
 
     _grouping_fields = {'chr', 'insert_start', 'insert_stop', 'strand'}
 
     _qbed_col_order = \
         ['chr', 'start', 'end', 'depth', 'strand']
 
     _summary = None
 
-    def __init__(self, summary: str or pd.DataFrame) -> None:
-        """_summary_
+    def __init__(self, summary: Union[str, pd.DataFrame]) -> None:
+        """
+        Initialize SummaryParser with given summary data.
 
         Args:
-            summary (str or pd.DataFrame): _description_
+            summary (Union[str, pd.DataFrame]): Either a path to a CSV 
+                file or an existing pandas DataFrame.
         """
         self.summary = summary
 
-        # switcher = {
-        #     'status': self._status_filter(*args, **kwargs),
-        #     'mapq': self._mapq_filter(*args, **kwargs),
-        #     'region': self._region_filter(*args, **kwargs),
-        #     'default': self.filterError(method)
-        # }
-
-        # switcher.get(method, "default")
-
-    # def filterError(self, method):
-    #     raise NotImplementedError(f"No filter method matches {method}")
-
-    # def _status_filter(self, query_string):
-    #     self.filter_string = query_string
-
-    # def _mapq_filter(self):
-    #     raise NotImplementedError
-
-    # def _region_filter(self):
-    #     raise NotImplementedError
-
     @property
     def query_string(self):
-        """_summary_"""
+        """
+        Query string for filtering summary data. Default is "status == 0".
+        """
         return self._query_string
 
     @query_string.setter
     def query_string(self, query_string: str):
         self._query_string = query_string
 
     @property
     def summary(self):
-        """_summary_"""
+        """
+        The summary data in DataFrame format.
+        """
         return self._summary
 
     @summary.setter
-    def summary(self, summary: str or pd.DataFrame):
+    def summary(self, summary: Union[str, pd.DataFrame]):
         # check input
         if isinstance(summary, str):
             # check genome and index paths
             if not os.path.exists(summary):
                 raise FileNotFoundError(f"Input file DNE: {summary}")
             summary = pd.read_csv(summary, dtype=self.summary_columns)
         elif isinstance(summary, pd.DataFrame):
-            logging.info(f'passed a dataframe to SummaryParser')
+            logger.info(f'passed a dataframe to SummaryParser')
         else:
             raise IOError(f'{summary} is not a data type recognized ' +
                           'as a summary by SummaryParser')
 
         if 'depth' not in summary.columns:
             summary['depth'] = 1
 
         self._verify(summary)
 
         self._summary = summary
 
     @property
     def summary_columns(self):
-        """_summary_"""
+        """
+        The expected structure (column names and data types) of 
+        the summary data.
+        """
         return self._summary_columns
 
     @summary_columns.setter
     def summary_columns(self, col_list: list):
         self._summary_columns = col_list
 
     @property
     def grouping_fields(self):
-        """_summary_"""
+        """
+        The set of fields to be used for grouping data in summary.
+        """
         return self._grouping_fields
 
     @grouping_fields.setter
     def grouping_fields(self, new_grouping_fields: dict):
         self.grouping_fields = new_grouping_fields
 
     @property
     def qbed_col_order(self):
-        """_summary_"""
+        """
+        Order of columns to be used when generating a DataFrame in qBED format.
+        """
         return self._qbed_col_order
 
     @qbed_col_order.setter
     def qbed_col_order(self, new_col_order: list):
         self._qbed_col_order = new_col_order
 
     def _verify(self, summary: pd.DataFrame) -> None:
-        """_summary_
+        """
+        Verifies that the provided summary DataFrame matches the 
+        expected structure.
 
         Args:
-            summary (pd.DataFrame): _description_
+            summary (pd.DataFrame): Summary data as a DataFrame.
 
         Raises:
-            ValueError: _description_
+            ValueError: Raised when the structure of the summary data does 
+                not match the expected structure.
         """
         if not len(set(self.summary_columns.keys()) - set(summary.columns)) == 0:
             raise ValueError(
                 f"The expected summary columns are "
                 f"{','.join(self.summary_columns)} in that order")
 
     def to_qbed(self) -> pd.DataFrame:
-        """_summary_
-
-        Args:
-            annotation (str): _description_
-
-        Raises:
-            AttributeError: _description_
+        """
+        Converts the summary data into a DataFrame in qBED format. It uses 
+        the query string to filter data, groups by the defined grouping fields, 
+        and orders columns as defined in qbed_col_order.
 
         Returns:
-            pd.DataFrame: _description_
+            pd.DataFrame: A DataFrame in qBED format.
         """
+
         local_grouping_fields = self.grouping_fields
 
         return self.summary\
             .query(self.query_string)[['chr', 'insert_start', 'insert_stop', 'depth', 'strand']]\
             .groupby(list(local_grouping_fields))['depth']\
             .agg(['sum'])\
             .reset_index()\
             .rename(columns={'sum': 'depth', 'insert_start': 'start', 'insert_stop': 'end'})[self.qbed_col_order]
 
     def write_qbed(self, output_path: str) -> None:
-        """_summary_
+        """
+        Writes the qBED-formatted DataFrame to a text file at the given path.
 
         Args:
-            output_path (str): _description_
+            output_path (str): The path to the file where the output 
+                should be written.
         """
         if not output_path[-4:] in ['.tsv', 'txt']:
-            logging.warning(
+            logger.warning(
                 f"output path {output_path} does not end with tsv or txt")
         self.to_qbed().to_csv(output_path,
                               sep="\t",
                               header=None,
                               index=False)
```

### Comparing `callingcardstools-0.2.0/callingcardstools/Alignment/mammals/Qbed.py` & `callingcardstools-1.0.0/callingcardstools/Alignment/mammals/Qbed.py`

 * *Files 6% similar despite different names*

```diff
@@ -77,28 +77,21 @@
     qc files.
     """
     
     _qbed_fields: list
     _qbed: DefaultDict
     _status_dict: DefaultDict
 
-    def __init__(self, pickle_path: str = None):
+    def __init__(self, pickle_path: str = None) -> None:
         """Create a ReadRecords object. This object will write records to
         a qbed file and a qc file.
 
         Args:
-           qbed_tmpfile (_type_): path to a tmp file for the qbed. intention
-             is for this to be tmp and then print the grouped/aggregated to
-             user output
-            qc_tmpfile (_type_): path to a file for the qc records. intention
-             is for this to be tmp, and then offer methods to summarize and
-             print summary to user output
-
-        Returns:
-            ReadRecords object
+            pickle_path: Path to a pickle file to load. If None, then
+                initialize a new ReadRecords object.
         """
         if pickle_path:
             if not os.path.exists(pickle_path):
                 msg = f"Path to pickle file {pickle_path} does not exist"
                 raise FileNotFoundError(msg)
             self.load(pickle_path)
         else:
@@ -183,25 +176,21 @@
             # Write
             writer.writeheader()
             writer.writerow({'srt_type': 'single_srt',
                             'count': single_srt_count})
             writer.writerow({'srt_type': 'multi_srt',
                             'count': multi_srt_count})
 
-
     # public methods ----------------------------------------------------------
-
-    def load(self, file_path: str):
+    
+    def load(self, file_path: str) -> None:
         """Load a BarcodeQcCounter object from a file using Pickle.
 
         Args:
             file_path (str): The file path where the object is stored.
-
-        Returns:
-            None
         """
         logger.info("loading Qbed object from %s", file_path)
         with open(file_path, "rb") as file:
             file_data = pickle.load(file)
             if not isinstance(file_data, Qbed):
                 raise TypeError(
                     f"{file_path} is not a Qbed object")
@@ -243,25 +232,27 @@
                insert_offset=1,
                annotation_tags: list = None) -> None:
         """write records to both the raw qbed tmpfile and raw qc tmpfile.
          Note that these tempfiles will be destroyed when the object is
          destroyed.
 
         Args:
-            tagged_read (dict): _description_
-             status (int): A value which reflects how the read performs
-             based on pre-defined quality metrics. A status of 0 is considered
-             a pass. A status of greater than 0 is a read which fails
-             at least 1 quality metric
+            tagged_read (dict): A pysam.AlignedSegment object which has been 
+                tagged with the appropriate calling cards tags based on the 
+                BarcodeParser object used to create the object.
+            status (int): A value which reflects how the read performs
+                based on pre-defined quality metrics. A status of 0 is considered
+                a pass. A status of greater than 0 is a read which fails
+                at least 1 quality metric
             insert_offset (int): number to add to tag XI value to calculate
-             the end coordinate. For instance, if the start coord is the first
-             T in TTAA, then the offset would be 4.
+                the end coordinate. For instance, if the start coord is the first
+                T in TTAA, then the offset would be 4.
             annotation_tags (list): List of strings. Values in list are tags to
-             extract from tagged_read dictionary. Values of tag will be added
-             to the annotation column of the qbed as a string delimited by '/'.
+                extract from tagged_read dictionary. Values of tag will be added
+                to the annotation column of the qbed as a string delimited by '/'.
         """
         if len({'read', 'barcode_details'}-tagged_read.keys()) > 0:
             raise KeyError('tagged_read must have keys '
                            '{"reads","barcode_details"}')
 
         if status == 0:
             # create the annotation field. If the annotation_tags list is not
@@ -286,15 +277,15 @@
               raw: bool = False) -> pd.DataFrame:
         """Translate the qbed object and status_dict to DataFrames and
         write to either a pickle or tsv file.
 
         Args:
             filename (str): The name of the file to write to.
             raw (bool): If True, write to a raw file. Otherwise,
-             write to a tsv file.
+                write to a tsv file.
 
         Returns:
             [pd.DataFrame, pd.DataFrame]: The qbed and status DataFrames
         """
         # create qbed DataFrame
         qbed_df = pd.DataFrame(columns=self.qbed_fields)
         single_srt_counter = 0
```

### Comparing `callingcardstools-0.2.0/callingcardstools/Alignment/mammals/combine_qc.py` & `callingcardstools-1.0.0/callingcardstools/Alignment/mammals/combine_qc.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.2.0/callingcardstools/Alignment/mammals/process_alignments.py` & `callingcardstools-1.0.0/callingcardstools/Alignment/mammals/process_alignments.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.2.0/callingcardstools/Alignment/yeast/legacy_makeccf.py` & `callingcardstools-1.0.0/callingcardstools/Alignment/yeast/legacy_makeccf.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.2.0/callingcardstools/Alignment/yeast/process_alignments.py` & `callingcardstools-1.0.0/callingcardstools/Alignment/yeast/process_alignments.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from callingcardstools.Alignment.AlignmentTagger import AlignmentTagger
 from callingcardstools.QC.create_status_coder import create_status_coder  # noqa
 from callingcardstools.Alignment.SummaryParser import SummaryParser
 from callingcardstools.QC.StatusFlags import StatusFlags
 
 __all__ = ['parse_args', 'process_alignments']
 
-logging.getLogger(__name__).addHandler(logging.NullHandler())
+logger = logging.getLogger(__name__)
 
 
 def parse_args(
         subparser: argparse.ArgumentParser,
         script_desc: str,
         common_args: argparse.ArgumentParser) -> argparse.ArgumentParser:
     """This is intended to be used as a subparser for a parent parser passed 
@@ -152,26 +152,26 @@
     try:
         output_dir = args.output_dir
     except AttributeError:
         output_dir = os.getcwd()
 
     output_basename = os.path.splitext(os.path.basename(args.bampath))[0]
 
-    logging.info("tagging reads...")
+    logger.info("tagging reads...")
     # temp_dir is automatically cleaned when context ends
     with tempfile.TemporaryDirectory() as temp_dir:
         # open files
-        logging.info("opening input bam file: %s", args.bampath)
+        logger.info("opening input bam file: %s", args.bampath)
         input_bamfile = pysam.AlignmentFile(  # pylint:disable=E1101
             args.bampath, "rb",
             require_index=True,
             threads=nthreads)
 
         # create tmp output bam files
-        logging.debug('creating tmp passing and failing bam in '
+        logger.debug('creating tmp passing and failing bam in '
                       'temp dir: %s', temp_dir)
         tmp_output_bampath_dict = \
             {x: os.path.join(
                 temp_dir,
                 'tmp_' + output_basename + '_' + x + out_suffix)
                 for x in ['passing', 'failing']}
 
@@ -244,15 +244,15 @@
                 for x in ['passing', 'failing']}
 
         tagged_bam_output_dict = \
             {k: pysam.AlignmentFile(v, "wb", header=new_header)
                 for k, v in output_bampath_dict.items()}
 
         # iterate over the reads to re-write
-        logging.info("re-writing bam with updated header...")
+        logger.info("re-writing bam with updated header...")
         for k, tmp_tagged_bam in tmp_tagged_bam_dict.items():
             # until_eof will include unmapped reads, also
             for read in tmp_tagged_bam.fetch(until_eof=True):
                 tagged_bam_output_dict[k].write(read)
             # close the temp bampath. Note that the whole temp directory
             # will be deleted when we leave the with
             # TempDirectory as ... clause
@@ -261,15 +261,15 @@
     for k, v in tagged_bam_output_dict.items():
         v.close()
         pysam.index(output_bampath_dict[k])
 
     # Close input
     input_bamfile.close()
 
-    logging.info('summarizing to summary_df and qbed...')
+    logger.info('summarizing to summary_df and qbed...')
     aln_summary_df = pd.DataFrame(read_summary)
     sp = SummaryParser(aln_summary_df)
     qbed_df = sp.to_qbed()
 
     qbed_df.to_csv(os.path.join(output_dir, output_basename + '.qbed'),
                    sep='\t',
                    index=False)
@@ -295,9 +295,9 @@
 
     if args.verbose_qc:
         aln_summary_df.to_csv(
             os.path.join(output_dir, output_basename + '_aln_info.tsv'),
             sep='\t',
             index=False)
 
-    logging.info('complete!')
+    logger.info('complete!')
     # return {'summary': aln_summary_df, 'qbed': qbed_df}
```

### Comparing `callingcardstools-0.2.0/callingcardstools/BarcodeParser/BarcodeParser.py` & `callingcardstools-1.0.0/callingcardstools/BarcodeParser/BarcodeParser.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 import random
 
 # outside package
 from edlib import align  # pylint:disable=E0611
 
 __all__ = ['BarcodeParser']
 
-logging.getLogger(__name__).addHandler(logging.NullHandler())
+logger = logging.getLogger(__name__)
 
 
 class BarcodeParser:
     """Using a json which describes acceptable values for given barcodes, 
     check the edit distance between the barcode components (substrings) and 
     the """
 
@@ -65,20 +65,20 @@
         # open json, read in as dict
         with open(new_barcode_details_json, 'r') as f1:  # pylint:disable=W1514
             barcode_dict = json.load(f1)
         # check keys
         if not len(required_keys - set(barcode_dict)) == 0:
             raise KeyError(f'the following keys are required: {required_keys}')
         # update the barcode_dict attribute
-        logging.info(
+        logger.info(
             "Updating the barcode dict to reflect "
             "the new barcode details json...")
         self.barcode_dict = barcode_dict
         # if that works, update the barcode_details_json path
-        logging.info("Success! Setting the barcode details json path")
+        logger.info("Success! Setting the barcode details json path")
         self._barcode_details_json = new_barcode_details_json
         # and update some properties
         self.max_r1 = self.__get_max_r1()
         self.max_mismatches = self.__calculate_max_mismatches()
 
     @property
     def key_dict(self):
@@ -139,15 +139,15 @@
     @property
     def insert_seq(self):
         """Getter for the insert seq sequence from the barcode details json. 
         Returns upper case.
 
         Raises:
             AttributeError: Raised if the current barcode details json does 
-            not have an insert seq key
+                not have an insert seq key
         """
         if self.key_dict['insert_seq'] in self.barcode_dict:
             return self.barcode_dict[self.key_dict['insert_seq']]
         else:
             raise AttributeError(f'Current barcode details '
                                  f'{self.barcode_details_json} does not '
                                  f'have an insert seq component')
@@ -264,28 +264,28 @@
         barcode zeroes. This allows the user to allow a number of mismatches 
         in each component, but to set a value less that the sum of those 
         allowances in the max_mismatch attribute to avoid a barcode with too 
         many total mismatches.
 
         Raises:
             TypeError: if the extracted or calculated max_mismatch value is not 
-            an integer
+                an integer
 
         Returns:
             int: an integer describing the total number of allowable mismatches 
-            between a barcode and a set of barcode components.
+                between a barcode and a set of barcode components.
         """
         max_mismatch = self.barcode_dict.get('max_mismatch', None)
 
         component_mismatch_sum = sum([
             self.barcode_dict['components'][k].get('match_allowance', 0)
             for k in self.barcode_dict['components'].keys()])
         if max_mismatch:
             if max_mismatch > component_mismatch_sum:
-                logging.info('max_mismatch in barcode_details: '
+                logger.info('max_mismatch in barcode_details: '
                              f'{max_mismatch} which is greater than the sum '
                              f'of component mismatch allowances: '
                              f'{component_mismatch_sum}')
         if not max_mismatch:
             max_mismatch = component_mismatch_sum
         if not isinstance(max_mismatch, int):
             raise TypeError('max_mismatch must be an integer. '
@@ -324,22 +324,22 @@
     def component_check(self, component_dict: dict) -> dict:
         """Determine if the barcode passes (True) or fails (False) given the 
         edit distances between it and the expected components, and the 
         allowable edit distance between a given component and the actual value.
 
         Args:
             component_dict (dict): a dictionary where the keys are component 
-            names and the values are the actual sequences, eg
-            {'r1_primer': 'TGATA', 'r1_transposon': 'AATTCACTACGTCAACA', 
-            'r2_transposon': 'ACCTGCTT', 'r2_restriction': 'TCGAGCGCCCGG'}
+                names and the values are the actual sequences, eg
+                {'r1_primer': 'TGATA', 'r1_transposon': 'AATTCACTACGTCAACA', 
+                'r2_transposon': 'ACCTGCTT', 'r2_restriction': 'TCGAGCGCCCGG'}
 
         Returns:
             dict: A dict of structure {"pass": Boolean, True if the barcode 
-            passes, "tf": Str, where the value is eithe "*" if unknown or a TF 
-            string from the barcode_details} 
+                passes, "tf": Str, where the value is either "*" 
+                if unknown or a TF string from the barcode_details} 
         """
         component_check_dict = {}
         for k, v in self.barcode_dict[self.key_dict['components']].items():
             # if the value of a given component is a list, create a dict
             # from from the list where the keys and values are the same.
             target_dict = {x: x for x in v['map']} \
                 if isinstance(v.get('map', None), list) \
@@ -398,15 +398,15 @@
         for component in self.barcode_dict['components'].keys():
             component_metrics = component_check_dict[component]
             # if the total_mismatches exceed the maximum number of mismatches
             # in a given barcode, set the passing value to false and exit the
             # loop
             if total_mismatches > self.max_mismatches:
                 passing = False
-                logging.debug('total_mismatches = {total_mismatches}; '
+                logger.debug('total_mismatches = {total_mismatches}; '
                               + 'max_mismatches = {self.max_mismatches}')
                 break
             # else, for a given component, extract the mismatch tolerance
             match_allowance = \
                 self.barcode_dict['components'][component]\
                     .get('match_allowance', 0)
             # if the edit dist exceeds the match_allowance, set the barcode to
@@ -421,15 +421,15 @@
             # note that if this is 0 it won't change anything, and move on to
             # the next component
             else:
                 if self.barcode_dict['components']\
                     .get(component, {})\
                         .get('require', True):
                     
-                    logging.debug(f'incrementing total mismatches '
+                    logger.debug(f'incrementing total mismatches '
                                   f'b/c of {component_metrics}')
                     
                     total_mismatches = (total_mismatches
                                         + component_metrics['dist'])
 
         return {'passing': passing, 'details': component_check_dict}
 
@@ -439,26 +439,28 @@
             component_dict: dict,
             match_type: Literal['edit_distance',
                                 'greedy'] = 'edit_distance') -> dict:
         """Given a match method, return a dictionary describing the
         best match between query and component_dict
 
         Args:
-            query (str): _description_
-            component_dict (dict): _description_
+            query (str): the string to compare to the component dict values
+            component_dict (dict): a dictionary where the keys are the
+                sequences to compare to the query and the values are the
+                names of the sequences
             match_type (str, optional): Either 'edit_distance' or 'greedy'.
-            Defaults to 'edit_distance'.
+                Defaults to 'edit_distance'.
 
         Returns:
             dict: A dictionary of structure
-            {'name': either the sequence match, or the name if map is a
-            named dictionary,
-            'dist': edit dist between query and best match --
-            always 0 or infinty if match is greedy depending on if exact
-            match is found or not. If not, return is 'name': '*', 'dist': inf}
+                {'name': either the sequence match, or the name if map is a
+                named dictionary,
+                'dist': edit dist between query and best match --
+                always 0 or infinty if match is greedy depending on if exact
+                match is found or not. If not, return is 'name': '*', 'dist': inf}
         """
         # if no match found, these are the default values. Note that if
         # the match type is not recognized, this function errors
         component_name = "*"
         dist = infinity
 
         # if the match_type is edit_distance, then return a dict with the
```

### Comparing `callingcardstools-0.2.0/callingcardstools/BarcodeParser/mammals/BarcodeQcCounter.py` & `callingcardstools-1.0.0/callingcardstools/BarcodeParser/mammals/BarcodeQcCounter.py`

 * *Files 6% similar despite different names*

```diff
@@ -151,22 +151,19 @@
         # combine the metrics dictionaries
         self._metrics = combine_dicts_additive(self._metrics, other.metrics)
         # combine the bc_status dictionaries
         self._bc_status = combine_dicts_bool(self._bc_status, other.bc_status)
 
     # public methods ----------------------------------------------------------
 
-    def load(self, file_path: str):
+    def load(self, file_path: str) -> None:
         """Load a BarcodeQcCounter object from a file using Pickle.
 
         Args:
             file_path (str): The file path where the object is stored.
-
-        Returns:
-            None
         """
         logger.info("loading BarcodeQcCounter object from %s", file_path)
         with open(file_path, "rb") as file:
             file_data = pickle.load(file)
             if not isinstance(file_data, BarcodeQcCounter):
                 raise TypeError(
                     f"{file_path} is not a BarcodeQcCounter object")
@@ -181,15 +178,15 @@
 
         Args:
             counters (Iterable[BarcodeQcCounter]): An iterable of
                 BarcodeQcCounter objects.
 
         Returns:
             BarcodeQcCounter: A new BarcodeQcCounter object with the
-              combined metrics.
+                combined metrics.
         """
         result = BarcodeQcCounter()
 
         for counter in counters:
             result._combine(counter)
 
         return result
@@ -234,26 +231,20 @@
               filename: str,
               suffix: str = "",
               raw: bool = False) -> None:
         """Write a pickle and/or a comma-delimited file summarizing the
         barcode QC metrics.
 
         Args:
-            raw (bool, optional): If True, pickles the object.
-                Defaults to False.
-            component_dict (dict, optional): A dictionary containing keys
-                for 'tf', 'pbs', and 'lrt2s', and their
-                respective lists of values. If provided, writes summaries
-                for each component. Defaults to None.
-            output_dirpath (str, optional): The output directory path where
-                the files will be saved. Defaults to the current directory.
             filename (str, optional): The base filename for the output files.
                 Defaults to "barcode_qc".
             suffix (str, optional): A suffix to be appended to the base
                 filename. Defaults to an empty string.
+            raw (bool, optional): If True, pickles the object.
+                Defaults to False.
         """
         # if raw is true, then pickle the object
         if raw:
             pickle_path = filename + '_' + suffix + '_barcode_qc.pkl'\
                 if suffix else filename + '_barcode_qc.pkl'
             logger.info("pickling barcode_qc object to %s{pick_path}")
             with open(pickle_path, "wb") as pickle_file:
@@ -276,19 +267,19 @@
                 ])
 
                 for pb_seq, lrt1_dict in self._metrics.items():
                     for lrt1_seq, lrt2_dict in lrt1_dict.items():
                         for lrt2_seq, srt_dict in lrt2_dict.items():
                             for srt_seq, count in srt_dict.items():
                                 bc_status = ("pass" if
-                                            (self._bc_status[pb_seq]
-                                            [lrt1_seq]
-                                            [lrt2_seq]
-                                            [srt_seq])
-                                            else "false")
+                                             (self._bc_status[pb_seq]
+                                              [lrt1_seq]
+                                              [lrt2_seq]
+                                              [srt_seq])
+                                             else "false")
                                 csv_writer.writerow([
                                     pb_seq,
                                     lrt1_seq,
                                     lrt2_seq,
                                     srt_seq,
                                     count,
                                     bc_status
```

### Comparing `callingcardstools-0.2.0/callingcardstools/BarcodeParser/yeast/BarcodeQcCounter.py` & `callingcardstools-1.0.0/callingcardstools/BarcodeParser/yeast/BarcodeQcCounter.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,22 +120,19 @@
         # Combine _r1_transposon_seq_dict dictionaries
         for r1_transposon_edit_dist, r1_transposon_seq_set in \
                 other.r1_transposon_dict.items():
             self._r1_transposon_seq_dict[r1_transposon_edit_dist]\
                 .update(r1_transposon_seq_set)
 
     # public methods ----------------------------------------------------------
-    def load(self, file_path: str):
+    def load(self, file_path: str) -> None:
         """Load a BarcodeQcCounter object from a file using Pickle.
 
         Args:
             file_path (str): The file path where the object is stored.
-
-        Returns:
-            None
         """
         logger.info("loading BarcodeQcCounter object from %s", file_path)
         with open(file_path, "rb") as file:
             file_data = pickle.load(file)
             if not isinstance(file_data, BarcodeQcCounter):
                 raise TypeError(
                     f"{file_path} is not a BarcodeQcCounter object")
@@ -150,15 +147,15 @@
 
         Args:
             counters (Iterable[BarcodeQcCounter]): An iterable of
                 BarcodeQcCounter objects.
 
         Returns:
             BarcodeQcCounter: A new BarcodeQcCounter object with the
-              combined metrics.
+                combined metrics.
         """
         result = BarcodeQcCounter()
 
         for counter in counters:
             result._combine(counter)
 
         return result
@@ -178,16 +175,16 @@
                r1_transposon_edit_dist: int,
                r2_restriction_enzyme_name: str) -> None:
         """Updates the metrics with given component and deviation tuples.
 
         Args:
             component_tuple (tuple): A tuple containing R1 primer,
                 R1 transposon, and R2 transposon sequences.
-            deviation_tuple (tuple): A tuple containing R1 primer,
-                R1 transposon, and R2 transposon edit distances.
+            r1_transposon_edit_dist (int): The edit distance between the
+                R1 transposon sequence and the expected R1 transposon
             r2_restriction_enzyme_name (str): The R2 restriction enzyme name.
         """
         (r1_primer_seq,
          r1_transposon_seq,
          r2_transposon_seq) = component_tuple
 
         (self._metrics
@@ -213,15 +210,15 @@
         """
         #
         r1_primer_summary = []
         r2_transposon_summary = []
         # only iterate over those reads which had an r1 transposon seq
         # edit distance of n or less
 
-        #r1_for_given_r2_dict = defaultdict(lambda: defaultdict(set))
+        # r1_for_given_r2_dict = defaultdict(lambda: defaultdict(set))
         r1_for_given_r2_dict = MiddleDefaultDict1(set)
         for i, r1_transposon_dict in self._metrics.items():
             # first level of iteration is over the r1 primer keys.
             # The dictionary is a nested dictionary with the keys being
             # r2_transposon sequences and values another dicitonary with
             # the restriciton enzyme and count
             for r1_primer_seq, r1_primer_dict in r1_transposon_dict.items():
@@ -340,15 +337,15 @@
         # if raw is true, then pickle the object
         if raw:
             pickle_path = os.path.join(
                 output_dirpath, filename + '_' + suffix + ".pickle")
             logger.info("pickling barcode_qc object to %s{pick_path}")
             with open(pickle_path, "wb") as pickle_file:
                 pickle.dump(self, pickle_file)
-                
+
         # if component_dict is passed
         if component_dict:
             # input checks
             if not isinstance(component_dict, dict):
                 raise TypeError("component_dict must be a dictionary")
             if not {'tf', 'r1_primer', 'r2_transposon'} == \
                     set(list(component_dict.keys())):
@@ -363,29 +360,29 @@
                     raise TypeError("component_dict values must be lists")
             if len({len(x) for x in component_dict.values()}) != 1:
                 raise ValueError("component_dict values must be lists of "
                                  "the same length")
             # extract summaries from the metrics
             r1_primer_summary, r2_transposon_summary = \
                 self._summarize_by_tf(component_dict)
-            
+
             # write r1_primer_summary to file
             append_suffix = '_' + suffix if suffix else ''
             r1_primer_basename = \
                 filename + "_r1_primer_summary" + append_suffix + ".csv"
             r1_primer_summary_path = os.path.join(
                 output_dirpath, r1_primer_basename)
             r1_primer_summary_df = pd.DataFrame(r1_primer_summary)
             logger.info("writing r1_primer_summary "
                         "to %s{r1_primer_summary_path}")
             r1_primer_summary_df.to_csv(r1_primer_summary_path, index=False)
-            
+
             # write r2_transposon summary to file
             r2_transposon_summary_basename = \
                 filename + "_r2_transposon_summary" + append_suffix + ".csv"
             r2_transposon_summary_path = os.path.join(
                 output_dirpath, r2_transposon_summary_basename)
             r2_transposon_summary_df = pd.DataFrame(r2_transposon_summary)
             logger.info("writing r2_transposon_summary "
                         "to %s{r2_transposon_summary_path}")
             r2_transposon_summary_df.to_csv(
-                r2_transposon_summary_path, index=False)
+                r2_transposon_summary_path, index=False)
```

### Comparing `callingcardstools-0.2.0/callingcardstools/BarcodeParser/yeast/combine_qc.py` & `callingcardstools-1.0.0/callingcardstools/BarcodeParser/yeast/combine_qc.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import argparse
 
 from .BarcodeQcCounter import BarcodeQcCounter
 from ..BarcodeParser import BarcodeParser
 
 __all__ = ['parse_args', 'combine_qc']
 
-logging.getLogger(__name__).addHandler(logging.NullHandler())
+logger = logging.getLogger(__name__)
 
 
 def parse_args(
         subparser: argparse.ArgumentParser,
         script_desc: str,
         common_args: argparse.ArgumentParser) -> argparse.ArgumentParser:
     """This is intended to be used as a subparser for a parent parser passed
```

### Comparing `callingcardstools-0.2.0/callingcardstools/QC/StatusFlags.py` & `callingcardstools-1.0.0/callingcardstools/QC/StatusFlags.py`

 * *Files 21% similar despite different names*

```diff
@@ -6,58 +6,94 @@
 from numpy import log2, ndarray
 from pandas import Series
 
 __all__ = ['StatusFlags']
 
 
 class StatusFlags(IntFlag):
-    """A barcode failure is 0x0, a mapq failure is 0x1 and a insert seq failure
-     is 0x2. A read that fails both barcode and mapq for instance would have
-     status 3.
+    """
+    A class used to represent different status flags for read alignment.
+    Each status flag corresponds to a different power of 2, allowing
+    combinations of flags to be represented as a sum of these powers.
+
+    Attributes:
+        BARCODE (int): Corresponds to a barcode failure.
+        MAPQ (int): Corresponds to a MAPQ failure.
+        INSERT_SEQ (int): Corresponds to an insert sequence failure.
+        FIVE_PRIME_CLIP (int): Corresponds to a failure due to 5' end
+            clipping in the read.
+        UNMAPPED (int): Corresponds to the read being unmapped.
+        NOT_PRIMARY (int): Corresponds to the read not being primary.
+        ALIGNER_QC_FAIL (int): Corresponds to the read failing aligner QC.
+        RESTRICTION_ENZYME (int): Corresponds to a failure due to
+            restriction enzyme.
     """
     BARCODE = 0x0
     MAPQ = 0x1
     INSERT_SEQ = 0x2
     FIVE_PRIME_CLIP = 0x3
     UNMAPPED = 0x4
     NOT_PRIMARY = 0x5
     ALIGNER_QC_FAIL = 0x6
     RESTRICTION_ENZYME = 0x7
 
-    def flag(self):
+    def flag(self) -> int:
+        """
+        Returns the power of 2 corresponding to the flag's value.
+
+        Returns:
+            int: The power of 2 corresponding to the flag's value.
+        """
         return 2**self.value
 
     @staticmethod
     def decompose(nums: Union[int, List[int], ndarray, Series],
-                  as_str: bool = True) -> List:
+                  as_str: bool = True) -> List[int]:
         """
-        Decompose a number, list, ndarray, or pandas Series of numbers
-            representing the sum of the powers of two into a list of those
-            powers of two. Optionally, return the string representation of
-            the powers of two according to the StatusFlags object.
+        Decomposes a number, list, ndarray, or pandas Series of numbers 
+        representing the sum of the powers of two into a list of those 
+        powers of two. Optionally, return the string representation of the 
+        powers of two according to the StatusFlags object.
 
         Args:
-            nums (Union[int, List[int], ndarray, pd.Series]):
-                The input number, list, ndarray, or pandas Series to decompose.
-            as_str (bool, optional): Whether to return the string
-                representation of the powers of two according to the
+            nums (Union[int, List[int], ndarray, pd.Series]): The input 
+                number, list, ndarray, or pandas Series to decompose.
+            as_str (bool, optional): Whether to return the string 
+                representation of the powers of two according to the 
                 StatusFlags object. Defaults to True.
 
         Returns:
-            List: A list representing the sum of the powers of two if
-                `as_str` is False, e.g., 10 decomposes into [2, 8].
-                If `as_str` is true, then the result would be
+            List: A list representing the sum of the powers of two if 
+                `as_str` is False, e.g., 10 decomposes into [2, 8]. If 
+                `as_str` is true, then the result would be 
                 ['MAPQ', 'RESTRICTION_ENZYME'].
 
         Raises:
-            TypeError: If the input type is neither int, list, numpy array,
+            TypeError: If the input type is neither int, list, numpy array, 
                 nor pandas Series.
             ValueError: If the input is a negative integer.
         """
         def decompose_single(num: int, as_str: bool = True) -> list:
+            """
+            Helper function to decompose a single integer into powers of 2.
+
+            Args:
+                num (int): The integer to decompose.
+                as_str (bool): Whether to return the string representation of 
+                    the powers of two according to the StatusFlags object. 
+                    Defaults to True.
+
+            Returns:
+                list: List of powers of two composing the input number. If 
+                    `as_str` is True, the powers of two are represented by 
+                    their corresponding flag names.
+
+            Raises:
+                ValueError: If the input integer is negative.
+            """
             # check input
             if num < 0:
                 raise ValueError("Invalid input, expected positive int")
             # if num is 0 and as_str is true, return NO_STATUS. otherwise, the
             # decomposed list will be empty
             if num == 0:
                 if as_str:
@@ -76,33 +112,7 @@
         if isinstance(nums, (list, ndarray, Series)):
             return [decompose_single(num, as_str) for num in nums]
         elif isinstance(nums, int):
             return decompose_single(nums, as_str)
         else:
             raise TypeError(
                 "Invalid input type, expected int, list, or numpy array")
-
-    # def decompose(num: int, as_str: bool = True) -> list:
-    #     """decompose a number which represents the sum of the powers of two
-    #         into a list of those powers of two. Optionally,
-
-    #     Args:
-    #         num (int): the flag to decompose, eg 10
-    #         as_str (bool, optional): whether to return the string
-    #             representation of the powers of two according to the
-    #             StatusFlag object. Defaults to True.
-
-    #     Returns:
-    #         list: list representing the sum of the powers of two if `as_str` is
-    #          False, eg 10 decomposes into [2,8]. If `as_str` is true, then the
-    #             result would be ['MAPQ', 'RESTRICTION_ENZYME']
-    #     """
-    #     # cite: https://codereview.stackexchange.com/a/201461
-    #     powers = []
-    #     while num != 0:
-    #         powers.append(log2(num & -num))
-    #         num = num & (num - 1)
-
-    #     if as_str:
-    #         powers = [StatusFlags(int(x)).name for x in powers]
-
-    #     return powers
```

### Comparing `callingcardstools-0.2.0/callingcardstools/QC/create_status_coder.py` & `callingcardstools-1.0.0/callingcardstools/QC/create_status_coder.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,50 +5,61 @@
 
 from pysam import AlignedSegment  # pylint:disable=E0611
 
 from callingcardstools.QC.StatusFlags import StatusFlags
 
 __all__ = ['create_status_coder']
 
-logging.getLogger(__name__).addHandler(logging.NullHandler())
+logger = logging.getLogger(__name__)
 
 
 def create_status_coder(
         insert_seqs: list = ['*'],
         mapq_threshold: int = 10,
         check_5_prime_clip: bool = False,
         check_passing: bool = True) -> Callable[[AlignedSegment], int]:
-    """A factory function which returns a function capable of determining
-     the status code of a read tagged by an AlignmentTagger object
+    """
+    A factory function which returns a function capable of determining the
+    status code of a read tagged by an AlignmentTagger object.
 
     Args:
-        insert_seqs (list): a list of acceptable insert sequences. Defaults to
-         ['*'], which will skip the insert seq check altogether.
-        mapq_threshold (int): a mapq_threshold. Less than this value will be
-        marked as failing the mapq threshold test. Default is 10.
-        check_passing (bool, optional): Whether to check the passing key
-            in the barcode_details dict. Defaults to True.
+        insert_seqs (list): A list of acceptable insert sequences. Defaults
+            to ['*'], which will skip the insert seq check altogether.
+        mapq_threshold (int): A mapq_threshold. Reads with map quality less
+            than this value will be marked as failing the mapq threshold test.
+            Default is 10.
+        check_5_prime_clip (bool): Whether to check for 5' end clipping in
+            the read. Defaults to False.
+        check_passing (bool, optional): Whether to check the passing key in
+            the barcode_details dict. Defaults to True.
 
     Returns:
-        Callable[[pysam.AlignedSegment], int]: A function which given a tagged
-         pysam AlignedSegment will return the status code for a the read
+        Callable[[AlignedSegment], int]: A function which given a tagged
+        pysam AlignedSegment will return the status code for the read.
     """
 
     def coder(read_details: AlignedSegment,
               status_code: int = 0) -> int:
-        """_summary_
+        """
+        Returns the status code for a given read after checking for various 
+        flags.
 
         Args:
-            read_details.get('read') (AlignedSegment): a pysam.AlignedSegment
-             object
-            status_code (int, optional): Initial status code.
-             Defaults to 0.
+            read_details (AlignedSegment): A pysam AlignedSegment object.
+            status_code (int, optional): Initial status code. Defaults to 0.
+
+        Raises:
+            ValueError: If read_details is not a dictionary or does not
+                contain expected keys.
+            KeyError: If required keys are not present in read_details.
+            ValueError: If the types of values in read_details do not 
+                match the expected types.
 
         Returns:
-            int: The status code for a given read
+            int: The status code for a given read.
         """
         if not isinstance(read_details, dict):
             raise ValueError('read_details must be a dictionary with '
                              'keys "read" which is a pysam.AlignedSegment and '
                              '"barcode_details" which is a dict')
         if not {'read', 'barcode_details'} - read_details.keys() == set():
             raise KeyError('"read" and "barcode_details" must be keys in'
@@ -94,13 +105,13 @@
                     status_code += StatusFlags.FIVE_PRIME_CLIP.flag()
         # check the insert sequence
         try:
             if insert_seqs != ["*"]:
                 if read_details.get('read').get_tag("XZ") not in insert_seqs:
                     status_code += StatusFlags.INSERT_SEQ.flag()
         except AttributeError as exc:
-            logging.debug(
+            logger.debug(
                 f"insert sequence not found in Barcode Parser. {exc}")
 
         return status_code
 
     return coder
```

### Comparing `callingcardstools-0.2.0/callingcardstools/Reads/ReadParser.py` & `callingcardstools-1.0.0/callingcardstools/Reads/ReadParser.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,27 +2,35 @@
 import gzip
 import logging
 
 from Bio import SeqIO
 
 from callingcardstools.BarcodeParser.BarcodeParser import BarcodeParser
 
-logging.getLogger(__name__).addHandler(logging.NullHandler())
+logger = logging.getLogger(__name__)
 
 __all__ = ['ReadParser']
 
 
 class ReadParser(BarcodeParser):
     """Given either single or paired end reads, use the provided barcode
      details json to examine expected read components
 
     Depending on the entries in the barcode details json, this class will parse
      the read(s), return the assembled components (this could include both what
      could be construed as a barcode as well as any other components), and the
      reads trimmed for the components labelled for trimming.
+    
+    Attributes:
+        r1_path (str): File path to Read 1.
+        r2_path (str): File path to Read 2.
+        r1_handle (_io.TextIOWrapper): File handle for Read 1.
+        r2_handle (_io.TextIOWrapper): File handle for Read 2.
+        cur_r1 (SeqRecord): Current read record for Read 1.
+        cur_r2 (SeqRecord): Current read record for Read 2.
 
     Example:
     ```
     >>> rb = ReadParser('/path/to/barcode_details.json')
     >>> r1 = next(SeqIO.parse('/path/to/r1.fq', format="fastq"))
     >>> r2 = next(SeqIO.parse('/path/to/r2.fq', format="fastq"))
     >>> read_dict = rb.process_read(r1,r2)
@@ -32,18 +40,22 @@
     _r2_path = ""
     _r1_handle = ""
     _r2_handle = ""
     _cur_r1 = ""
     _cur_r2 = ""
 
     def __init__(self, barcode_details_json: str = "", r1: str = "", r2: str = "") -> None:  # noqa
-        """_summary_
+        """Initializes the ReadParser with barcode details and optional 
+        read files.
 
         Args:
-            barcode_details_json (str, optional): _description_. Defaults to "".
+            barcode_details_json (str): The JSON file path containing 
+                barcode details.
+            r1 (str): The path to the Read 1 file.
+            r2 (str): The path to the Read 2 file.
         """
         if barcode_details_json:
             super().__init__(barcode_details_json)
         if r1:
             self.r1_path = r1
         if r2:
             self.r2_path = r2
@@ -114,22 +126,25 @@
         return self._cur_r2
 
     @cur_r2.setter
     def cur_r2(self, r2_seqrecord):
         self._cur_r2 = r2_seqrecord
 
     def fastq_path_parser(self, fq_path: str) -> bool:
-        """_summary_
+        """Checks if the FastQ file path is valid.
 
         Args:
-            fq_path (str): _description_
+            fq_path (str): The path to the FastQ file.
 
         Raises:
-            FileNotFoundError: _description_
-            IOError: raised if the accetable fastq extensions, .fq or .fastq
+            FileNotFoundError: If the FastQ file does not exist.
+            IOError: If the FastQ file extension is not .fastq, .fq, or .gz.
+
+        Returns:
+            bool: True if the file path is valid, otherwise False.
         """
         error_msg = 'fastq extension must be either .fastq or .fq. ' +\
             'it may be gzipped, eg .fq.gz'
         fq_extensions = {'.fastq', '.fq'}
 
         if not os.path.exists(fq_path):
             raise FileNotFoundError(f'{fq_path} Does Not Exist!')
@@ -137,18 +152,21 @@
             if os.path.splitext(fq_path)[1] == ".gz":
                 if not os.path.splitext(os.path.splitext(fq_path)[0])[1] in fq_extensions:  # noqa
                     raise IOError(error_msg)
             else:
                 raise IOError(error_msg)
 
     def open(self) -> None:
-        """_summary_
+        """Opens the read file(s).
+
+        If the file is gzipped, it is opened with gzip, otherwise it's opened normally.
+        In case of paired-end reads, both files are opened.
 
         Raises:
-            AttributeError: _description_
+            AttributeError: If the Read 1 file path is not set.
         """
         if not self.r1_path:
             raise AttributeError('R1 Not Set')
 
         elif os.path.splitext(self.r1_path)[1] == ".gz":
             self.r1_handle = SeqIO.parse(
                 gzip.open(self.r1_path, "rt"),
@@ -168,31 +186,30 @@
                     format='fastq')
             else:
                 self.r2_handle = SeqIO.parse(
                     self.r2_path,
                     format='fastq')
 
     def close(self) -> None:
-        """close file objects, if they are set
-        """
+        """close file objects, if they are set"""
         if self.r1_handle:
             self.r1_handle = ""
         if self.r2_handle:
             self.r2_handle = ""
 
     def next(self) -> None:
         """Iterate the reads and set cur_r1 and cur_r2 (if paired end) to the
          next read in hte file
 
         Raises:
             AttributeError: If R1 is not open
             StopIteration: If the end of file is reached in either
-             R1 or R2 (if it is set)
+                R1 or R2 (if it is set)
             ValueError: If after advancing the read ids for
-             R1 and r2 (if paired end) do not match
+                R1 and r2 (if paired end) do not match
         """
         r1_stop = False
         r2_stop = False
         if not self.r1_handle:
             raise AttributeError('R1 is not open -- cannot advance')
         elif not self.r2_handle:
             self.cur_r1 = next(self.r1_handle)
@@ -203,34 +220,34 @@
                 r1_stop = True
             try:
                 self.cur_r2 = next(self.r2_handle)
             except StopIteration:
                 r2_stop = True
             if r1_stop != r2_stop:
                 error_msg = 'The length of R1 and R2 is not the same'
-                logging.WARNING(error_msg)  # pylint:disable=E1102
+                logger.warning(error_msg)  # pylint:disable=E1102
                 raise IOError(error_msg)
             elif r1_stop or r2_stop:
                 raise StopIteration
             if self.cur_r1.id != self.cur_r2.id:
                 error_msg = f"r1 ID: {self.cur_r1.id} does not match r2 "\
                     f"fID: {self.cur_r2.id}"
-                logging.CRITICAL(error_msg)  # pylint:disable=E1102
+                logger.critical(error_msg)  # pylint:disable=E1102
                 raise ValueError(error_msg)
 
     def parse(self, set_name_to_empty: bool = True) -> dict:  # noqa
         """Using the barcode details, process a given read
 
         Args:
             set_name_to_empty (bool, optional): Set the name attribute to 
-            empty. SeqIO sets to ID if a name DNE. Defaults to True.
+                empty. SeqIO sets to ID if a name DNE. Defaults to True.
 
         Returns:
             dict: A dictionary with the r1 and r2 SeqRecord objects, the 
-            barcode and the unadulterated read ID
+                barcode and the unadulterated read ID
         """
         # extract this in case it is augmented with the barcode later on
         read_id = self.cur_r1.id
         # create the beginnigns out of the output dictionary
         read_dict = {
             'r1': self.cur_r1,
             'r2': self.cur_r2
```

### Comparing `callingcardstools-0.2.0/callingcardstools/Reads/legacy_split_fastq.py` & `callingcardstools-1.0.0/callingcardstools/Reads/legacy_split_fastq.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 import logging
 import csv
 from Bio import SeqIO,Seq
 
 
 __all__ = ['parse_args', 'legacy_split_fastq']
 
-logging.getLogger(__name__).addHandler(logging.NullHandler())
+logger = logging.getLogger(__name__)
 
 
 def read_barcode_file(barcode_filename):
     # This function reads in the experiment name, the primer barcode, and the transposon barcodes
     # from a file which is in the following format:
     # expt name \t primer barcode \t transposon barcode 1,transposon barcode 2, transposon barcode 3 etc.
     # It then returns a dictionary with key = a tuple (primer barcode, transposon barcode), value = expt_name
```

### Comparing `callingcardstools-0.2.0/callingcardstools/Reads/split_fastq.py` & `callingcardstools-1.0.0/callingcardstools/Reads/split_fastq.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from Bio import SeqIO
 
 from callingcardstools.Reads.ReadParser import ReadParser
 from callingcardstools.BarcodeParser.yeast import BarcodeQcCounter
 
 __all__ = ['parse_args', 'split_fastq']
 
-logging.getLogger(__name__).addHandler(logging.NullHandler())
+logger = logging.getLogger(__name__)
 
 
 def parse_args(
         subparser: argparse.ArgumentParser,
         script_desc: str,
         common_args: argparse.ArgumentParser) -> argparse.ArgumentParser:
     """This is intended to be used as a subparser for a parent parser passed
@@ -93,38 +93,38 @@
 
     return subparser
 
 
 def split_fastq(args: argparse.Namespace):
 
     # Check inputs
-    logging.info('checking input...')
+    logger.info('checking input...')
     input_path_list = [args.read1,
                        args.read2,
                        args.barcode_details,
                        args.output_dirpath]
     for input_path in input_path_list:
         if not os.path.exists(input_path):
             raise FileNotFoundError(f"Input file DNE: {input_path}")
 
     # create the BarcodeQcCounter object
-    logging.info('creating BarcodeQcCounter object...')
+    logger.info('creating BarcodeQcCounter object...')
     bc_counter = BarcodeQcCounter()
 
     # create the read parser object
     rp = ReadParser(args.barcode_details, args.read1, args.read2)
-    logging.info('opening fq files')
+    logger.info('opening fq files')
     rp.open()
     # if the split_key isn't in the barcode_details, then every passing
     # read goes into a file with that name
     if args.split_key not in rp.barcode_dict['components']:
         msg = f"{args.split_key} not found in barcode_dict['components']. " \
             f"all output is directed to " \
             f"{args.split_key}_{args.split_suffix}_R1,2.fq"
-        logging.info(msg)
+        logger.info(msg)
 
         determined_out = {
             'r1': open(f"{args.split_key}_{args.split_suffix}_R1.fq", "w"),  # pylint:disable=W1514 # noqa
             'r2': open(f"{args.split_key}_{args.split_suffix}_R2.fq", "w")  # pylint:disable=W1514 # noqa
         }
     # else the split_key is in barcode_details, create/open a fq output file
     # for each of the keys in barcode[components][split_key]
@@ -149,24 +149,24 @@
             args.output_dirpath,
             f"undetermined_{args.split_suffix}_R2.fq"), "w")
     }
 
     # if verbose_qc is true, for read paired read, record a line which
     # associates the fastq read ID with the barcode components
     if args.verbose_qc:
-        logging.info('opening id to barcode map...')
+        logger.info('opening id to barcode map...')
         additional_components = ['tf', 'restriction_enzyme']
         id_bc_map = open(os.path.join(
             args.output_dirpath, "id_bc_map.tsv"), "w")
         # write header
         id_bc_map.write(
             "\t".join(['id'] + list(rp.components) + additional_components))
         id_bc_map.write("\n")
 
-    logging.info('parsing fastq files...')
+    logger.info('parsing fastq files...')
     # iterate over reads, split reads whose barcode components
     # match expectation into the appropriate file, and reads which don't
     # fulfill barcode expectations into undetermined.fq
     while True:
         try:
             rp.next()
         except StopIteration:
@@ -260,8 +260,8 @@
                          output_dirpath=args.output_dirpath,
                          suffix=args.split_suffix)
     else:
         bc_counter.write(component_dict=component_dict,
                          output_dirpath=args.output_dirpath,
                          suffix=args.split_suffix)
 
-    logging.info('Done parsing the fastqs!')
+    logger.info('Done parsing the fastqs!')
```

### Comparing `callingcardstools-0.2.0/callingcardstools/Resources/human/barcode_details.json` & `callingcardstools-1.0.0/callingcardstools/Resources/mammals/barcode_details.json`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.2.0/callingcardstools/Resources/yeast/barcode_details.json` & `callingcardstools-1.0.0/callingcardstools/Resources/yeast/barcode_details.json`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.2.0/callingcardstools/__main__.py` & `callingcardstools-1.0.0/callingcardstools/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import sys
 import argparse
 from typing import Callable
 import logging
 from logging.config import dictConfig
 from importlib.metadata import version
 
-from .BarcodeParser import barcode_table_to_json
+from .BarcodeParser.yeast import barcode_table_to_json
 from .BarcodeParser.yeast import combine_qc as yeast_combine_qc
 from .Reads import legacy_split_fastq, split_fastq
 from .Alignment.yeast import legacy_makeccf
 from .Alignment.yeast import process_alignments as process_yeast_bam
 from .Alignment.mammals import process_alignments as process_mammals_bam
 from .Alignment.mammals import combine_qc as mammals_combine_qc
 
@@ -47,15 +47,15 @@
         'qBed format file of the passing reads, and a qc file which '
         'allows finer exploration of the barcode and alignment metrics',
 
         'process_mammals_bam': 'Iterate over the reads in an alignment file (bam) and '
         'separate reads into passing.bam and failing.bam, a '
         'qBed format file of the passing reads, and a qc file which '
         'allows finer exploration of the barcode and alignment metrics',
-        
+
         'mammals_combine_qc': 'Combine qbed and barcodeQC objects which may '
         'result from splitting the fastq and processing chunks in parallel',
     }
 
     # common options -- these can be applied to all scripts via the 'parent'---
     # argument -- see subparsers.add_parser for parse_bam below ---------------
     common_args = argparse.ArgumentParser(
@@ -144,18 +144,14 @@
         log_level = args.log_level.upper()
     except AttributeError:
         sys.exit(arg_parser.print_help())
 
     # set the logging details
     log_config = {
         "version": 1,
-        "root": {
-            "handlers": ["console"],
-            "level": f"{log_level}"
-        },
         "handlers": {
             "console": {
                 "formatter": "std_out",
                 "class": "logging.StreamHandler"
             }
         },
         "formatters": {
@@ -163,14 +159,20 @@
                 "format": "%(asctime)s : %(module)s : "
                 "%(funcName)s : line: %(lineno)d\n" +
                 "\tprocess details : %(process)d, %(processName)s\n" +
                 "\tthread details : %(thread)d, %(threadName)s\n" +
                 "\t%(levelname)s : %(message)s",
                 "datefmt": "%Y-%m-%d %H:%M:%S"
             }
+        },
+        "loggers": {
+            "": {
+                "level": f"{log_level}",
+                "handlers": ["console"]
+            }
         }
     }
     dictConfig(log_config)
     # log the cmd line arguments at the debug level
     logging.debug(sys.argv)
     logging.debug(str(args))
```

### Comparing `callingcardstools-0.2.0/callingcardstools/utils.py` & `callingcardstools-1.0.0/callingcardstools/utils.py`

 * *Files identical despite different names*

### Comparing `callingcardstools-0.2.0/pyproject.toml` & `callingcardstools-1.0.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 [tool.poetry]
 name = "callingCardsTools"
-version = "0.2.0"
+version = "1.0.0"
 description = "A collection of objects and functions to work with calling cards sequencing tools"
 authors = ["chase mateusiak <chase.mateusiak@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://cmatkhan.github.io/callingCardsTools/"
 repository = "https://github.com/cmatKhan/callingCardsTools"
 documentation = "https://cmatkhan.github.io/callingCardsTools/"
 exclude = ['Dockerfile', '*temp_*','docs', 'site', 'tests', '.git','.venv','.github', 'Resources/yeast/README.md']
 include = ["callingcardstools/Resources"]
 
 [tool.poetry.dependencies]
 python = ">=3.8"
 pandas = "^1.5.3"
-numpy = "^1.24.3"
 pysam = "^0.19.1"
 edlib = "^1.3.9"
 biopython = "^1.81"
+numpy = "^1.24.3"
 
 [tool.poetry.group.dev.dependencies]
 ipykernel = "^6.23.1"
 docutils = "^0.19"
 mkdocs = "^1.4.3"
 mkdocs-material = "^8.5.11"
 mkdocstrings = {extras = ["python"], version = "^0.19.1"}
```

### Comparing `callingcardstools-0.2.0/setup.py` & `callingcardstools-1.0.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,16 +8,15 @@
  'callingcardstools.Alignment.yeast',
  'callingcardstools.BarcodeParser',
  'callingcardstools.BarcodeParser.mammals',
  'callingcardstools.BarcodeParser.yeast',
  'callingcardstools.QC',
  'callingcardstools.Reads',
  'callingcardstools.Resources',
- 'callingcardstools.Resources.human',
- 'callingcardstools.Resources.mouse',
+ 'callingcardstools.Resources.mammals',
  'callingcardstools.Resources.yeast']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['biopython>=1.81,<2.0',
@@ -27,15 +26,15 @@
  'pysam>=0.19.1,<0.20.0']
 
 entry_points = \
 {'console_scripts': ['callingcardstools = callingcardstools:__main__.main']}
 
 setup_kwargs = {
     'name': 'callingcardstools',
-    'version': '0.2.0',
+    'version': '1.0.0',
     'description': 'A collection of objects and functions to work with calling cards sequencing tools',
     'long_description': "# Installation \n\n```\npip install callingcardstools\n```\n\nTo start using the command line tools, see the help message with:\n\n```\ncallingcardstools --help\n```\n\n# Development Installation\n\n1. install [poetry](https://python-poetry.org/)\n  - I prefer to set the default location of the virtual environment to the \n  project directory. You can set that as a global configuration for your \n  poetry installation like so: `poetry config virtualenvs.in-project true`\n\n2. git clone the repo\n\n3. cd into the repo and issue the command `poetry install`\n\n4. shell into the virtual environment with `poetry shell`\n\n5. build the package with `poetry build`\n\n6. install the callingcardstools packge into your virtual environment \n  `pip install dist/callingcardstools-...`\n  - Note: you could figure out how to use the pip install `-e` flag to \n  have an interactive development environment. I don't think that is compatible \n  with only the `pyproject.toml` file, but if you look it up, you'll find good \n  stackoverflow instructions on how to put a dummy `setup.py` file in to make \n  this possible\n\n7. Building the Dockerimage:\n\nCurrently the Dockerimage is built from a stable version on github\n\nNote that unless I set it up, you won't be able to push to my dockerhub repo. \nI think that is possible to do, though. If you wish to push to your own dockerhub, \nreplace the cmatkhan to your username.\n\n```bash\ndocker build -t cmatkhan/callingcardstools - < Dockerfile\n```\n\nwhere cmatkhan/callingcardstools is the tag. This will default to the version \n`latest`\n\nTo push:\n\n```bash\ndocker push cmatkhan/callingcardstools\n```",
     'author': 'chase mateusiak',
     'author_email': 'chase.mateusiak@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://cmatkhan.github.io/callingCardsTools/',
```

### Comparing `callingcardstools-0.2.0/PKG-INFO` & `callingcardstools-1.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: callingcardstools
-Version: 0.2.0
+Version: 1.0.0
 Summary: A collection of objects and functions to work with calling cards sequencing tools
 Home-page: https://cmatkhan.github.io/callingCardsTools/
 License: MIT
 Author: chase mateusiak
 Author-email: chase.mateusiak@gmail.com
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
```

