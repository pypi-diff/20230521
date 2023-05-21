# Comparing `tmp/dnadb-0.5.0.tar.gz` & `tmp/dnadb-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dnadb-0.5.0.tar", last modified: Tue May 16 01:20:49 2023, max compression
+gzip compressed data, was "dnadb-0.6.0.tar", last modified: Sun May 21 18:38:17 2023, max compression
```

## Comparing `dnadb-0.5.0.tar` & `dnadb-0.6.0.tar`

### file list

```diff
@@ -1,29 +1,30 @@
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-16 01:20:49.209688 dnadb-0.5.0/
--rw-r--r--   0 dwl2x     (1000) users      (100)     1070 2023-03-27 04:24:58.000000 dnadb-0.5.0/LICENSE
--rw-r--r--   0 dwl2x     (1000) users      (100)     1802 2023-05-16 01:20:49.209688 dnadb-0.5.0/PKG-INFO
--rw-r--r--   0 dwl2x     (1000) users      (100)       43 2023-03-27 04:27:38.000000 dnadb-0.5.0/README.md
--rw-r--r--   0 dwl2x     (1000) users      (100)      742 2023-05-15 22:10:37.000000 dnadb-0.5.0/pyproject.toml
--rw-r--r--   0 dwl2x     (1000) users      (100)       38 2023-05-16 01:20:49.209688 dnadb-0.5.0/setup.cfg
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-16 01:20:49.205688 dnadb-0.5.0/src/
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-16 01:20:49.209688 dnadb-0.5.0/src/dnadb/
--rw-r--r--   0 dwl2x     (1000) users      (100)       22 2023-05-15 22:10:42.000000 dnadb-0.5.0/src/dnadb/__init__.py
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-16 01:20:49.209688 dnadb-0.5.0/src/dnadb/datasets/
--rw-r--r--   0 dwl2x     (1000) users      (100)      255 2023-03-27 05:49:34.000000 dnadb-0.5.0/src/dnadb/datasets/__init__.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     7303 2023-05-14 15:51:22.000000 dnadb-0.5.0/src/dnadb/datasets/dataset.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     1392 2023-04-03 19:22:40.000000 dnadb-0.5.0/src/dnadb/datasets/greengenes.py
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-16 01:20:49.209688 dnadb-0.5.0/src/dnadb/datasets/silva/
--rw-r--r--   0 dwl2x     (1000) users      (100)     5538 2023-05-14 21:04:53.000000 dnadb-0.5.0/src/dnadb/datasets/silva/__init__.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     6022 2023-05-15 03:13:49.000000 dnadb-0.5.0/src/dnadb/datasets/silva/taxonomy_map.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     2234 2023-05-10 12:52:14.000000 dnadb-0.5.0/src/dnadb/db.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     4815 2023-05-11 20:35:23.000000 dnadb-0.5.0/src/dnadb/dna.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     5232 2023-05-15 04:51:39.000000 dnadb-0.5.0/src/dnadb/fasta.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     6017 2023-05-15 04:51:34.000000 dnadb-0.5.0/src/dnadb/fastq.py
--rw-r--r--   0 dwl2x     (1000) users      (100)        0 2023-05-09 22:29:41.000000 dnadb-0.5.0/src/dnadb/otu.py
--rw-r--r--   0 dwl2x     (1000) users      (100)    20115 2023-05-16 00:50:00.000000 dnadb-0.5.0/src/dnadb/taxonomy.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     1473 2023-04-01 17:43:32.000000 dnadb-0.5.0/src/dnadb/utils.py
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-16 01:20:49.209688 dnadb-0.5.0/src/dnadb.egg-info/
--rw-r--r--   0 dwl2x     (1000) users      (100)     1802 2023-05-16 01:20:49.000000 dnadb-0.5.0/src/dnadb.egg-info/PKG-INFO
--rw-r--r--   0 dwl2x     (1000) users      (100)      519 2023-05-16 01:20:49.000000 dnadb-0.5.0/src/dnadb.egg-info/SOURCES.txt
--rw-r--r--   0 dwl2x     (1000) users      (100)        1 2023-05-16 01:20:49.000000 dnadb-0.5.0/src/dnadb.egg-info/dependency_links.txt
--rw-r--r--   0 dwl2x     (1000) users      (100)       64 2023-05-16 01:20:49.000000 dnadb-0.5.0/src/dnadb.egg-info/requires.txt
--rw-r--r--   0 dwl2x     (1000) users      (100)        6 2023-05-16 01:20:49.000000 dnadb-0.5.0/src/dnadb.egg-info/top_level.txt
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-21 18:38:17.236162 dnadb-0.6.0/
+-rw-r--r--   0 dwl2x     (1000) users      (100)     1070 2023-03-27 04:24:58.000000 dnadb-0.6.0/LICENSE
+-rw-r--r--   0 dwl2x     (1000) users      (100)     1802 2023-05-21 18:38:17.236162 dnadb-0.6.0/PKG-INFO
+-rw-r--r--   0 dwl2x     (1000) users      (100)       43 2023-03-27 04:27:38.000000 dnadb-0.6.0/README.md
+-rw-r--r--   0 dwl2x     (1000) users      (100)      742 2023-05-21 18:37:54.000000 dnadb-0.6.0/pyproject.toml
+-rw-r--r--   0 dwl2x     (1000) users      (100)       38 2023-05-21 18:38:17.236162 dnadb-0.6.0/setup.cfg
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-21 18:38:17.236162 dnadb-0.6.0/src/
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-21 18:38:17.236162 dnadb-0.6.0/src/dnadb/
+-rw-r--r--   0 dwl2x     (1000) users      (100)       22 2023-05-21 18:37:47.000000 dnadb-0.6.0/src/dnadb/__init__.py
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-21 18:38:17.236162 dnadb-0.6.0/src/dnadb/datasets/
+-rw-r--r--   0 dwl2x     (1000) users      (100)      255 2023-03-27 05:49:34.000000 dnadb-0.6.0/src/dnadb/datasets/__init__.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     7303 2023-05-14 15:51:22.000000 dnadb-0.6.0/src/dnadb/datasets/dataset.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     1392 2023-04-03 19:22:40.000000 dnadb-0.6.0/src/dnadb/datasets/greengenes.py
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-21 18:38:17.236162 dnadb-0.6.0/src/dnadb/datasets/silva/
+-rw-r--r--   0 dwl2x     (1000) users      (100)     5538 2023-05-14 21:04:53.000000 dnadb-0.6.0/src/dnadb/datasets/silva/__init__.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     6022 2023-05-15 03:13:49.000000 dnadb-0.6.0/src/dnadb/datasets/silva/taxonomy_map.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     2252 2023-05-21 14:19:04.000000 dnadb-0.6.0/src/dnadb/db.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     4815 2023-05-11 20:35:23.000000 dnadb-0.6.0/src/dnadb/dna.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     7774 2023-05-21 15:17:15.000000 dnadb-0.6.0/src/dnadb/fasta.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     5991 2023-05-21 14:19:54.000000 dnadb-0.6.0/src/dnadb/fastq.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)    10992 2023-05-21 18:28:55.000000 dnadb-0.6.0/src/dnadb/sample.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)    20094 2023-05-21 14:21:18.000000 dnadb-0.6.0/src/dnadb/taxonomy.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)       84 2023-05-21 14:17:53.000000 dnadb-0.6.0/src/dnadb/types.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     1473 2023-04-01 17:43:32.000000 dnadb-0.6.0/src/dnadb/utils.py
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-21 18:38:17.236162 dnadb-0.6.0/src/dnadb.egg-info/
+-rw-r--r--   0 dwl2x     (1000) users      (100)     1802 2023-05-21 18:38:17.000000 dnadb-0.6.0/src/dnadb.egg-info/PKG-INFO
+-rw-r--r--   0 dwl2x     (1000) users      (100)      541 2023-05-21 18:38:17.000000 dnadb-0.6.0/src/dnadb.egg-info/SOURCES.txt
+-rw-r--r--   0 dwl2x     (1000) users      (100)        1 2023-05-21 18:38:17.000000 dnadb-0.6.0/src/dnadb.egg-info/dependency_links.txt
+-rw-r--r--   0 dwl2x     (1000) users      (100)       64 2023-05-21 18:38:17.000000 dnadb-0.6.0/src/dnadb.egg-info/requires.txt
+-rw-r--r--   0 dwl2x     (1000) users      (100)        6 2023-05-21 18:38:17.000000 dnadb-0.6.0/src/dnadb.egg-info/top_level.txt
```

### Comparing `dnadb-0.5.0/LICENSE` & `dnadb-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dnadb-0.5.0/PKG-INFO` & `dnadb-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dnadb
-Version: 0.5.0
+Version: 0.6.0
 Summary: A library for handling DNA files.
 Author-email: David Ludwig <davidludwigii@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 DLii-Research
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dnadb-0.5.0/pyproject.toml` & `dnadb-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dnadb"
-version = "0.5.0"
+version = "0.6.0"
 authors = [
   { name="David Ludwig", email="davidludwigii@gmail.com" },
 ]
 description = "A library for handling DNA files."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.8"
```

### Comparing `dnadb-0.5.0/src/dnadb/datasets/dataset.py` & `dnadb-0.6.0/src/dnadb/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.5.0/src/dnadb/datasets/greengenes.py` & `dnadb-0.6.0/src/dnadb/datasets/greengenes.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.5.0/src/dnadb/datasets/silva/__init__.py` & `dnadb-0.6.0/src/dnadb/datasets/silva/__init__.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.5.0/src/dnadb/datasets/silva/taxonomy_map.py` & `dnadb-0.6.0/src/dnadb/datasets/silva/taxonomy_map.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.5.0/src/dnadb/db.py` & `dnadb-0.6.0/src/dnadb/db.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from lmdbm import Lmdb
 from pathlib import Path
-from typing import Callable, TypeVar, Union
+from typing import TypeVar, Union
+
+from .types import int_t
 
 T = TypeVar("T")
 
 class DbFactory:
     """
     A factory for creating LMDB-backed databases of FASTA entries.
     """
-    def __init__(self, path: Union[str, Path], chunk_size: int = 10000):
+    def __init__(self, path: Union[str, Path], chunk_size: int_t = 10000):
         self.path = Path(path)
         if self.path.suffix != ".db":
             self.path = Path(str(self.path) + ".db")
         self.db = Lmdb.open(str(self.path), "n", lock=True)
         self.buffer: dict[Union[str, bytes], bytes] = {}
         self.chunk_size = chunk_size
         self.is_closed = False
```

### Comparing `dnadb-0.5.0/src/dnadb/dna.py` & `dnadb-0.6.0/src/dnadb/dna.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.5.0/src/dnadb/fasta.py` & `dnadb-0.6.0/src/dnadb/fastq.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,172 +1,207 @@
 from dataclasses import dataclass
-from functools import singledispatchmethod
 import io
 import numpy as np
+import numpy.typing as npt
 from pathlib import Path
 from typing import Generator, Iterable, Tuple, Union
 
 from .db import DbFactory, DbWrapper
-from .taxonomy import TaxonomyEntry
+from .types import int_t
 from .utils import open_file
 
-_int_t = Union[int, np.int32, np.int64]
+def phred_encode(probabilities: npt.ArrayLike, encoding: int_t = 33) -> str:
+    scores = (-10 * np.log10(np.array(probabilities))).astype(int)
+    return ''.join((chr(score + encoding)) for score in scores)
+
+
+def phred_decode(qualities: str, encoding: int_t = 33) -> npt.NDArray[np.float64]:
+    scores = np.array([(ord(token) - encoding) for token in qualities])
+    return 10**(scores / -10)
+
 
 @dataclass(frozen=True, order=True)
-class FastaEntry:
+class FastqHeader:
     """
-    A container class to represent a FASTA entry
+    A class representation of the header of a FASTQ entry.
     """
-    __slots__ = ("identifier", "sequence", "extra")
+    __slots__ = (
+        "instrument",
+        "run_number",
+        "flowcell_id",
+        "lane",
+        "tile",
+        "pos",
+        "read_type",
+        "is_filtered",
+        "control_number",
+        "sequence_index"
+    )
+
+    instrument: str
+    run_number: int_t
+    flowcell_id: str
+    lane: int_t
+    tile: int_t
+    pos: Tuple[int, int]
+    read_type: int_t
+    is_filtered: bool
+    control_number: int_t
+    sequence_index: str
+
+    @classmethod
+    def deserialize(cls, sequence_id: bytes):
+        return cls.from_str(sequence_id.decode())
+
+    @classmethod
+    def from_str(cls, sequence_id: str) -> "FastqHeader":
+        # Split up the sequence ID information
+        left, right = sequence_id.strip()[1:].split(' ')
+        left = left.split(':')
+        right = right.split(':')
+        return cls(
+            instrument=left[0],
+            run_number=int(left[1]),
+            flowcell_id=left[2],
+            lane=int(left[3]),
+            tile=int(left[4]),
+            pos=tuple(map(int, left[5:])),
+            read_type=int(right[0]),
+            is_filtered=right[1] == 'Y',
+            control_number=int(right[2]),
+            sequence_index=right[3]
+        )
 
-    identifier: str
+    # Serialize a FastqHeader object to a byte string
+    def serialize(self) -> bytes:
+        return str(self).encode()
+
+    def __str__(self):
+        sequence_id = '@'
+        sequence_id += ':'.join(map(str, [
+            self.instrument,
+            self.run_number,
+            self.flowcell_id,
+            self.lane,
+            self.tile,
+            *self.pos
+        ]))
+        sequence_id += ' '
+        sequence_id += ':'.join(map(str, [
+            self.read_type,
+            'Y' if self.is_filtered else 'N',
+            self.control_number,
+            self.sequence_index
+        ]))
+        return sequence_id
+
+
+@dataclass(frozen=True, order=True)
+class FastqEntry:
+    """
+    A class representation of a FASTQ entry containing the sequnce identifier, sequence, and quality
+    scores.
+    """
+    __slots__ = ("header_str", "sequence", "quality_scores")
+
+    header_str: str
     sequence: str
-    extra: str
+    quality_scores: str
 
     @classmethod
-    def deserialize(cls, entry: bytes) -> "FastaEntry":
-        """
-        Deserialize a FASTA entry from a byte string
-        """
+    def deserialize(cls, entry: bytes) -> "FastqEntry":
         return cls(*entry.decode().split('\x00'))
 
     @classmethod
-    def from_str(cls, entry: str) -> "FastaEntry":
-        """
-        Create a FASTA entry from a string
-        """
-        header, *sequence_parts = entry.split('\n')
-        header_line = header[1:].rstrip().split(maxsplit=1)
-        identifier = header_line[0]
-        extra = header_line[1] if len(header_line) > 1 else ""
-        sequence = "".join(sequence_parts)
-        return cls(identifier, sequence, extra)
+    def from_str(cls, entry: str) -> "FastqEntry":
+        header, sequence, _, quality_scores= entry.rstrip().split('\n')
+        return cls(header, sequence, quality_scores)
 
     def serialize(self) -> bytes:
-        return "\x00".join((self.identifier, self.sequence, self.extra)).encode()
+        return '\x00'.join((self.header_str, self.sequence, self.quality_scores)).encode()
+
+    @property
+    def header(self):
+        return FastqHeader.from_str(self.header_str)
 
     def __str__(self):
-        header_line = f"{self.identifier} {self.extra}".rstrip()
-        return f">{header_line}\n{self.sequence}"
+        return f"{self.header_str}\n{self.sequence}\n+\n{self.quality_scores}"
 
 
-class FastaDbFactory(DbFactory):
+class FastqDbFactory(DbFactory):
     """
     A factory for creating LMDB-backed databases of FASTA entries.
     """
-    __slots__ = ("num_entries", "has_ambiguous_bases")
-
-    def __init__(self, path: Union[str, Path], chunk_size: int = 10000):
+    def __init__(self, path: Union[str, Path], chunk_size: int_t = 10000):
         super().__init__(path, chunk_size)
         self.num_entries = np.int32(0)
-        self.has_ambiguous_bases = False
 
-    def write_entry(self, entry: FastaEntry):
+    def write_entry(self, entry: FastqEntry):
         """
         Create a new FASTA LMDB database from a FASTA file.
         """
-        self.write(f"id_{entry.identifier}", np.int32(self.num_entries).tobytes())
         self.write(str(self.num_entries), entry.serialize())
         self.num_entries += 1
 
-    def write_entries(self, entries: Iterable[FastaEntry]):
+    def write_entries(self, entries: Iterable[FastqEntry]):
         for entry in entries:
             self.write_entry(entry)
 
     def before_close(self):
         self.write("length", self.num_entries.tobytes())
         super().before_close()
 
 
-class FastaDb(DbWrapper):
-    """
-    An LMDB-backed database of FASTA entries.
-    """
-    def __init__(self, fasta_db_path: Union[str, Path]):
-        super().__init__(fasta_db_path)
+class FastqDb(DbWrapper):
+    def __init__(self, fastq_db_path: Union[str, Path]):
+        super().__init__(fastq_db_path)
         self.length = np.frombuffer(self.db["length"], dtype=np.int32, count=1)[0]
 
     def __len__(self):
         return self.length
 
-    @singledispatchmethod
-    def __contains__(self, sequence_index: _int_t) -> bool:
+    def __contains__(self, sequence_index: int_t) -> bool:
         return str(sequence_index) in self.db
 
-    @__contains__.register
-    def _(self, sequence_id: str) -> bool:
-        return f"id_{sequence_id}" in self.db
-
-    @__contains__.register
-    def _(self, entry: FastaEntry) -> bool:
-        return entry.identifier in self
-
     def __iter__(self):
         for i in range(len(self)):
             yield self[i]
 
-    @singledispatchmethod
-    def __getitem__(self, sequence_index: _int_t) -> FastaEntry:
-        return FastaEntry.deserialize(self.db[str(sequence_index)])
-
-    @__getitem__.register
-    def _(self, sequence_id: str) -> FastaEntry:
-        index = np.frombuffer(self.db[f"id_{sequence_id}"], dtype=np.int32, count=1)[0]
-        return self[index]
+    def __getitem__(self, sequence_index: int_t) -> FastqEntry:
+        return FastqEntry.deserialize(self.db[str(sequence_index)])
 
 
 def entries(
-    sequences: Union[io.TextIOBase, Iterable[FastaEntry], str, Path]
-) -> Iterable[FastaEntry]:
+    sequences: Union[io.TextIOBase, Iterable[FastqEntry], str, Path]
+) -> Iterable[FastqEntry]:
     """
-    Create an iterator over a FASTA file or iterable of FASTA entries.
+    Create an iterator over a FASTQ file or iterable of FASTQ entries.
     """
     if isinstance(sequences, (str, Path)):
         with open_file(sequences, 'r') as buffer:
             yield from read(buffer)
     elif isinstance(sequences, io.TextIOBase):
         yield from read(sequences)
     else:
         yield from sequences
+    raise TypeError(f"Unsupported type: {type(sequences)}")
 
 
-def entries_with_taxonomy(
-    sequences: Iterable[FastaEntry],
-    taxonomies: Iterable[TaxonomyEntry],
-) -> Generator[Tuple[FastaEntry, TaxonomyEntry], None, None]:
-    """
-    Efficiently iterate over a FASTA file with a corresponding taxonomy file
-    """
-    labels = {}
-    taxonomy_iterator = iter(taxonomies)
-    taxonomy: TaxonomyEntry
-    for sequence in sequences:
-        while sequence.identifier not in labels:
-            taxonomy = next(taxonomy_iterator)
-            labels[taxonomy.identifier] = taxonomy
-        taxonomy = labels[sequence.identifier]
-        del labels[sequence.identifier]
-        yield sequence, taxonomy
-
-
-def read(buffer: io.TextIOBase) -> Generator[FastaEntry, None, None]:
-    """
-    Read entries from a FASTA file buffer.
-    """
-    entry_str = buffer.readline()
-    for line in buffer:
-        if line.startswith('>'):
-            yield FastaEntry.from_str(entry_str)
-            entry_str = ""
-        entry_str += line
-    if len(entry_str) > 0:
-        yield FastaEntry.from_str(entry_str)
+def read(buffer: io.TextIOBase) -> Generator[FastqEntry, None, None]:
+    """
+    Read entries from a FASTQ file buffer.
+    """
+    line = buffer.readline()
+    while len(line) > 0:
+        entry_str = "".join((line, *(buffer.readline() for _ in range(3))))
+        yield FastqEntry.from_str(entry_str)
+        line = buffer.readline()
 
 
-def write(buffer: io.TextIOBase, entries: Iterable[FastaEntry]) -> int:
+def write(buffer: io.TextIOBase, entries: Iterable[FastqEntry]) -> int:
     """
-    Write entries to a FASTA file.
+    Write entries to a FASTQ file.
     """
     bytes_written = 0
     for entry in entries:
         bytes_written += buffer.write(str(entry) + '\n')
     return bytes_written
```

### Comparing `dnadb-0.5.0/src/dnadb/fastq.py` & `dnadb-0.6.0/src/dnadb/fasta.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,208 +1,240 @@
 from dataclasses import dataclass
+from functools import singledispatchmethod
 import io
 import numpy as np
-import numpy.typing as npt
 from pathlib import Path
-from typing import Generator, Iterable, Tuple, Union
+from typing import Generator, Iterable, Optional, Tuple, Union
 
 from .db import DbFactory, DbWrapper
+from .taxonomy import TaxonomyEntry
+from .types import int_t
 from .utils import open_file
 
-_int_t = Union[int, np.int32, np.int64]
-
-def phred_encode(probabilities: npt.ArrayLike, encoding: _int_t = 33) -> str:
-    scores = (-10 * np.log10(np.array(probabilities))).astype(int)
-    return ''.join((chr(score + encoding)) for score in scores)
-
-
-def phred_decode(qualities: str, encoding: _int_t = 33) -> npt.NDArray[np.float64]:
-    scores = np.array([(ord(token) - encoding) for token in qualities])
-    return 10**(scores / -10)
-
-
 @dataclass(frozen=True, order=True)
-class FastqHeader:
+class FastaEntry:
     """
-    A class representation of the header of a FASTQ entry.
+    A container class to represent a FASTA entry
     """
-    __slots__ = (
-        "instrument",
-        "run_number",
-        "flowcell_id",
-        "lane",
-        "tile",
-        "pos",
-        "read_type",
-        "is_filtered",
-        "control_number",
-        "sequence_index"
-    )
-
-    instrument: str
-    run_number: _int_t
-    flowcell_id: str
-    lane: _int_t
-    tile: _int_t
-    pos: Tuple[int, int]
-    read_type: _int_t
-    is_filtered: bool
-    control_number: _int_t
-    sequence_index: str
-
-    @classmethod
-    def deserialize(cls, sequence_id: bytes):
-        return cls.from_str(sequence_id.decode())
+    __slots__ = ("identifier", "sequence", "extra")
 
-    @classmethod
-    def from_str(cls, sequence_id: str) -> "FastqHeader":
-        # Split up the sequence ID information
-        left, right = sequence_id.strip()[1:].split(' ')
-        left = left.split(':')
-        right = right.split(':')
-        return cls(
-            instrument=left[0],
-            run_number=int(left[1]),
-            flowcell_id=left[2],
-            lane=int(left[3]),
-            tile=int(left[4]),
-            pos=tuple(map(int, left[5:])),
-            read_type=int(right[0]),
-            is_filtered=right[1] == 'Y',
-            control_number=int(right[2]),
-            sequence_index=right[3]
-        )
-
-    # Serialize a FastqHeader object to a byte string
-    def serialize(self) -> bytes:
-        return str(self).encode()
-
-    def __str__(self):
-        sequence_id = '@'
-        sequence_id += ':'.join(map(str, [
-            self.instrument,
-            self.run_number,
-            self.flowcell_id,
-            self.lane,
-            self.tile,
-            *self.pos
-        ]))
-        sequence_id += ' '
-        sequence_id += ':'.join(map(str, [
-            self.read_type,
-            'Y' if self.is_filtered else 'N',
-            self.control_number,
-            self.sequence_index
-        ]))
-        return sequence_id
-
-
-@dataclass(frozen=True, order=True)
-class FastqEntry:
-    """
-    A class representation of a FASTQ entry containing the sequnce identifier, sequence, and quality
-    scores.
-    """
-    __slots__ = ("header_str", "sequence", "quality_scores")
-
-    header_str: str
+    identifier: str
     sequence: str
-    quality_scores: str
+    extra: str
 
     @classmethod
-    def deserialize(cls, entry: bytes) -> "FastqEntry":
+    def deserialize(cls, entry: bytes) -> "FastaEntry":
+        """
+        Deserialize a FASTA entry from a byte string
+        """
         return cls(*entry.decode().split('\x00'))
 
     @classmethod
-    def from_str(cls, entry: str) -> "FastqEntry":
-        header, sequence, _, quality_scores= entry.rstrip().split('\n')
-        return cls(header, sequence, quality_scores)
+    def from_str(cls, entry: str) -> "FastaEntry":
+        """
+        Create a FASTA entry from a string
+        """
+        header, *sequence_parts = entry.split('\n')
+        header_line = header[1:].rstrip().split(maxsplit=1)
+        identifier = header_line[0]
+        extra = header_line[1] if len(header_line) > 1 else ""
+        sequence = "".join(sequence_parts)
+        return cls(identifier, sequence, extra)
 
     def serialize(self) -> bytes:
-        return '\x00'.join((self.header_str, self.sequence, self.quality_scores)).encode()
-
-    @property
-    def header(self):
-        return FastqHeader.from_str(self.header_str)
+        return "\x00".join((self.identifier, self.sequence, self.extra)).encode()
 
     def __str__(self):
-        return f"{self.header_str}\n{self.sequence}\n+\n{self.quality_scores}"
+        header_line = f"{self.identifier} {self.extra}".rstrip()
+        return f">{header_line}\n{self.sequence}"
 
 
-class FastqDbFactory(DbFactory):
+class FastaDbFactory(DbFactory):
     """
     A factory for creating LMDB-backed databases of FASTA entries.
     """
-    def __init__(self, path: Union[str, Path], chunk_size: _int_t = 10000):
+    __slots__ = ("num_entries", "has_ambiguous_bases")
+
+    def __init__(self, path: Union[str, Path], chunk_size: int = 10000):
         super().__init__(path, chunk_size)
         self.num_entries = np.int32(0)
+        self.has_ambiguous_bases = False
 
-    def write_entry(self, entry: FastqEntry):
+    def write_entry(self, entry: FastaEntry):
         """
         Create a new FASTA LMDB database from a FASTA file.
         """
+        self.write(f"id_{entry.identifier}", np.int32(self.num_entries).tobytes())
         self.write(str(self.num_entries), entry.serialize())
         self.num_entries += 1
 
-    def write_entries(self, entries: Iterable[FastqEntry]):
+    def write_entries(self, entries: Iterable[FastaEntry]):
         for entry in entries:
             self.write_entry(entry)
 
     def before_close(self):
         self.write("length", self.num_entries.tobytes())
         super().before_close()
 
 
-class FastqDb(DbWrapper):
-    def __init__(self, fastq_db_path: Union[str, Path]):
-        super().__init__(fastq_db_path)
+class FastaDb(DbWrapper):
+    """
+    An LMDB-backed database of FASTA entries.
+    """
+    def __init__(self, fasta_db_path: Union[str, Path]):
+        super().__init__(fasta_db_path)
         self.length = np.frombuffer(self.db["length"], dtype=np.int32, count=1)[0]
 
     def __len__(self):
         return self.length
 
-    def __contains__(self, sequence_index: _int_t) -> bool:
+    @singledispatchmethod
+    def __contains__(self, sequence_index: int_t) -> bool:
         return str(sequence_index) in self.db
 
+    @__contains__.register
+    def _(self, sequence_id: str) -> bool:
+        return f"id_{sequence_id}" in self.db
+
+    @__contains__.register
+    def _(self, entry: FastaEntry) -> bool:
+        return entry.identifier in self
+
     def __iter__(self):
         for i in range(len(self)):
             yield self[i]
 
-    def __getitem__(self, sequence_index: _int_t) -> FastqEntry:
-        return FastqEntry.deserialize(self.db[str(sequence_index)])
+    @singledispatchmethod
+    def __getitem__(self, sequence_index: int_t) -> FastaEntry:
+        return FastaEntry.deserialize(self.db[str(sequence_index)])
+
+    @__getitem__.register
+    def _(self, sequence_id: str) -> FastaEntry:
+        index = np.frombuffer(self.db[f"id_{sequence_id}"], dtype=np.int32, count=1)[0]
+        return self[index]
+
+
+class FastaIndexDbFactory(DbFactory):
+    """
+    A factory for creating a FastaIndexDb.
+    """
+    def __init__(self, path: Union[str, Path], chunk_size: int = 10000):
+        super().__init__(path, chunk_size)
+        self.num_entries = np.int64(0)
+
+    def write_entry(self, fasta_entry_or_fasta_id: Union[str, FastaEntry], key: Optional[str] = None):
+        if isinstance(fasta_entry_or_fasta_id, FastaEntry):
+            fasta_identifier = fasta_entry_or_fasta_id.identifier
+        else:
+            fasta_identifier = fasta_entry_or_fasta_id
+
+        self.write(f"id_{fasta_identifier}", np.int64(self.num_entries).tobytes())
+        self.write(str(self.num_entries), fasta_identifier.encode())
+        if key is not None:
+            self.write(f"key_{key}", np.int64(self.num_entries).tobytes())
+            self.write(f"key_index_{self.num_entries}", key.encode())
+        self.num_entries += 1
+
+    def write_entries(self, fasta_entries_or_fasta_ids: Iterable[Union[str, FastaEntry]]):
+        for entry in fasta_entries_or_fasta_ids:
+            self.write_entry(entry)
+
+    def before_close(self):
+        self.write("length", self.num_entries.tobytes())
+        return super().before_close()
+
+
+class FastaIndexDb(DbWrapper):
+    """
+    An LMDB-backed database maintaining an index that maps indices/keys to FASTA identifiers.
+    """
+    def __init__(self, path: Union[str, Path]):
+        super().__init__(path)
+        self.length = np.frombuffer(self.db["length"], dtype=np.int64, count=1)[0]
+
+    def contains_fasta_id(self, fasta_id: str) -> bool:
+        return f"id_{fasta_id}" in self.db
+
+    def contains_index(self, index: int) -> bool:
+        return index >= 0 and index < self.length
+
+    def contains_key(self, key: str) -> bool:
+        return f"key_{key}" in self.db
+
+    def fasta_id_to_index(self, fasta_id: str) -> int:
+        return np.frombuffer(self.db[f"id_{fasta_id}"], dtype=np.int64, count=1)[0]
+
+    def fasta_id_to_key(self, fasta_id: str) -> str:
+        return self.index_to_key(self.fasta_id_to_index(fasta_id))
+
+    def index_to_fasta_id(self, index: int) -> str:
+        return self.db[str(index)].decode()
+
+    def index_to_key(self, index: int) -> str:
+        return self.db[f"key_index_{index}"].decode()
+
+    def key_to_fasta_id(self, key: str) -> str:
+        return self.index_to_fasta_id(self.key_to_index(key))
+
+    def key_to_index(self, key: str) -> int:
+        return np.frombuffer(self.db[f"key_{key}"], dtype=np.int64, count=1)[0]
+
+    def __len__(self):
+        return self.length
 
 
 def entries(
-    sequences: Union[io.TextIOBase, Iterable[FastqEntry], str, Path]
-) -> Iterable[FastqEntry]:
+    sequences: Union[io.TextIOBase, Iterable[FastaEntry], str, Path]
+) -> Iterable[FastaEntry]:
     """
-    Create an iterator over a FASTQ file or iterable of FASTQ entries.
+    Create an iterator over a FASTA file or iterable of FASTA entries.
     """
     if isinstance(sequences, (str, Path)):
         with open_file(sequences, 'r') as buffer:
             yield from read(buffer)
     elif isinstance(sequences, io.TextIOBase):
         yield from read(sequences)
     else:
         yield from sequences
-    raise TypeError(f"Unsupported type: {type(sequences)}")
 
 
-def read(buffer: io.TextIOBase) -> Generator[FastqEntry, None, None]:
-    """
-    Read entries from a FASTQ file buffer.
-    """
-    line = buffer.readline()
-    while len(line) > 0:
-        entry_str = "".join((line, *(buffer.readline() for _ in range(3))))
-        yield FastqEntry.from_str(entry_str)
-        line = buffer.readline()
+def entries_with_taxonomy(
+    sequences: Iterable[FastaEntry],
+    taxonomies: Iterable[TaxonomyEntry],
+) -> Generator[Tuple[FastaEntry, TaxonomyEntry], None, None]:
+    """
+    Efficiently iterate over a FASTA file with a corresponding taxonomy file
+    """
+    labels = {}
+    taxonomy_iterator = iter(taxonomies)
+    taxonomy: TaxonomyEntry
+    for sequence in sequences:
+        while sequence.identifier not in labels:
+            taxonomy = next(taxonomy_iterator)
+            labels[taxonomy.identifier] = taxonomy
+        taxonomy = labels[sequence.identifier]
+        del labels[sequence.identifier]
+        yield sequence, taxonomy
+
+
+def read(buffer: io.TextIOBase) -> Generator[FastaEntry, None, None]:
+    """
+    Read entries from a FASTA file buffer.
+    """
+    entry_str = buffer.readline()
+    for line in buffer:
+        if line.startswith('>'):
+            yield FastaEntry.from_str(entry_str)
+            entry_str = ""
+        entry_str += line
+    if len(entry_str) > 0:
+        yield FastaEntry.from_str(entry_str)
 
 
-def write(buffer: io.TextIOBase, entries: Iterable[FastqEntry]) -> int:
+def write(buffer: io.TextIOBase, entries: Iterable[FastaEntry]) -> int:
     """
-    Write entries to a FASTQ file.
+    Write entries to a FASTA file.
     """
     bytes_written = 0
     for entry in entries:
         bytes_written += buffer.write(str(entry) + '\n')
     return bytes_written
```

### Comparing `dnadb-0.5.0/src/dnadb/taxonomy.py` & `dnadb-0.6.0/src/dnadb/taxonomy.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,18 +5,17 @@
 import numpy as np
 import numpy.typing as npt
 from pathlib import Path
 import re
 from typing import Dict, Generator, Iterable, List, Optional, Tuple, Union
 
 from .db import DbFactory, DbWrapper
+from .types import int_t
 from .utils import open_file
 
-_int_t = Union[int, np.int32, np.int64]
-
 RANKS = ("Kingdom", "Phylum", "Class", "Order", "Family", "Genus", "Species")
 RANK_PREFIXES = ''.join(rank[0] for rank in RANKS).lower()
 
 # Utility Functions --------------------------------------------------------------------------------
 
 def split_taxonomy(taxonomy: str) -> Tuple[str, ...]:
     """
@@ -140,34 +139,34 @@
 
     def contains_label(self, label: str) -> bool:
         """
         Check if a taxonomy label exists in the database.
         """
         return label in self.db
 
-    def count(self, label_index: _int_t) -> int:
+    def count(self, label_index: int_t) -> int:
         """
         Get the number of sequences with a given label index.
         """
         return int(np.frombuffer(self.db[f"count_{label_index}"], dtype=np.int32, count=1)[0])
 
     def counts(self) -> Generator[int, None, None]:
         """
         Get the number of sequences for each label index.
         """
         for i in range(self.length):
             yield self.count(i)
 
-    def fasta_id_with_label(self, label_index: _int_t, fasta_index: _int_t) -> str:
+    def fasta_id_with_label(self, label_index: int_t, fasta_index: int_t) -> str:
         """
         Get the FASTA identifier for a given label and index.
         """
         return self.db[f"{label_index}_{fasta_index}"].decode()
 
-    def fasta_ids_with_label(self, label_index: _int_t) -> Generator[str, None, None]:
+    def fasta_ids_with_label(self, label_index: int_t) -> Generator[str, None, None]:
         """
         Get the FASTA identifiers for a given label.
         """
         for i in range(self.count(label_index)):
             yield self.fasta_id_with_label(label_index, i)
 
     def fasta_id_to_index(self, fasta_identifier: str) -> int:
@@ -178,15 +177,15 @@
 
     def fasta_id_to_label(self, fasta_identifier: str) -> str:
         """
         Get the taxonomy label for a given FASTA identifier.
         """
         return self.label(self.fasta_id_to_index(fasta_identifier))
 
-    def label(self, label_index: _int_t) -> str:
+    def label(self, label_index: int_t) -> str:
         """
         Get the taxonomy label for a given index.
         """
         return self.db[str(label_index)].decode()
 
     def labels(self) -> Generator[str, None, None]:
         """
```

### Comparing `dnadb-0.5.0/src/dnadb/utils.py` & `dnadb-0.6.0/src/dnadb/utils.py`

 * *Files identical despite different names*

### Comparing `dnadb-0.5.0/src/dnadb.egg-info/PKG-INFO` & `dnadb-0.6.0/src/dnadb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dnadb
-Version: 0.5.0
+Version: 0.6.0
 Summary: A library for handling DNA files.
 Author-email: David Ludwig <davidludwigii@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 DLii-Research
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `dnadb-0.5.0/src/dnadb.egg-info/SOURCES.txt` & `dnadb-0.6.0/src/dnadb.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 README.md
 pyproject.toml
 src/dnadb/__init__.py
 src/dnadb/db.py
 src/dnadb/dna.py
 src/dnadb/fasta.py
 src/dnadb/fastq.py
-src/dnadb/otu.py
+src/dnadb/sample.py
 src/dnadb/taxonomy.py
+src/dnadb/types.py
 src/dnadb/utils.py
 src/dnadb.egg-info/PKG-INFO
 src/dnadb.egg-info/SOURCES.txt
 src/dnadb.egg-info/dependency_links.txt
 src/dnadb.egg-info/requires.txt
 src/dnadb.egg-info/top_level.txt
 src/dnadb/datasets/__init__.py
```

