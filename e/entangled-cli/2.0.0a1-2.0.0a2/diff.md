# Comparing `tmp/entangled_cli-2.0.0a1.tar.gz` & `tmp/entangled_cli-2.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "entangled_cli-2.0.0a1.tar", max compression
+gzip compressed data, was "entangled_cli-2.0.0a2.tar", max compression
```

## Comparing `entangled_cli-2.0.0a1.tar` & `entangled_cli-2.0.0a2.tar`

### file list

```diff
@@ -1,24 +1,32 @@
--rw-r--r--   0        0        0    11357 2023-05-17 22:57:15.407443 entangled_cli-2.0.0a1/LICENSE
--rw-r--r--   0        0        0     3636 2023-05-17 23:13:17.696662 entangled_cli-2.0.0a1/README.md
--rw-r--r--   0        0        0        1 2023-05-14 17:38:11.126821 entangled_cli-2.0.0a1/entangled/__init__.py
--rw-r--r--   0        0        0     2366 2023-05-17 17:35:19.862137 entangled_cli-2.0.0a1/entangled/code_reader.py
--rw-r--r--   0        0        0      152 2023-05-17 21:41:45.725411 entangled_cli-2.0.0a1/entangled/commands/__init__.py
--rw-r--r--   0        0        0     1792 2023-05-17 22:10:53.164879 entangled_cli-2.0.0a1/entangled/commands/stitch.py
--rw-r--r--   0        0        0     1231 2023-05-17 22:10:53.121878 entangled_cli-2.0.0a1/entangled/commands/sync.py
--rw-r--r--   0        0        0     2476 2023-05-17 22:08:53.540161 entangled_cli-2.0.0a1/entangled/commands/tangle.py
--rw-r--r--   0        0        0     1292 2023-05-17 22:10:53.132879 entangled_cli-2.0.0a1/entangled/commands/watch.py
--rw-r--r--   0        0        0     3722 2023-05-17 17:32:13.252459 entangled_cli-2.0.0a1/entangled/config.py
--rw-r--r--   0        0        0        1 2023-05-11 21:20:21.892775 entangled_cli-2.0.0a1/entangled/data/defaults.toml
--rw-r--r--   0        0        0     3664 2023-05-17 15:57:42.155557 entangled_cli-2.0.0a1/entangled/document.py
--rw-r--r--   0        0        0      738 2023-05-13 22:41:01.900313 entangled_cli-2.0.0a1/entangled/error.py
--rw-r--r--   0        0        0     5115 2023-05-17 21:48:49.929944 entangled_cli-2.0.0a1/entangled/filedb.py
--rw-r--r--   0        0        0     1315 2023-05-17 22:08:29.608018 entangled_cli-2.0.0a1/entangled/main.py
--rw-r--r--   0        0        0     3692 2023-05-16 14:41:22.598769 entangled_cli-2.0.0a1/entangled/markdown_reader.py
--rw-r--r--   0        0        0     5509 2023-05-17 17:32:13.331459 entangled_cli-2.0.0a1/entangled/parsing.py
--rw-r--r--   0        0        0     2440 2023-05-17 17:21:17.574754 entangled_cli-2.0.0a1/entangled/properties.py
--rw-r--r--   0        0        0        0 2023-05-17 22:09:32.399394 entangled_cli-2.0.0a1/entangled/py.typed
--rw-r--r--   0        0        0     5398 2023-05-17 15:57:42.313557 entangled_cli-2.0.0a1/entangled/transaction.py
--rw-r--r--   0        0        0      760 2023-05-15 20:56:23.150699 entangled_cli-2.0.0a1/entangled/utility.py
--rw-r--r--   0        0        0       30 2023-05-15 06:18:06.572120 entangled_cli-2.0.0a1/entangled/version.py
--rw-r--r--   0        0        0     1067 2023-05-17 23:16:22.656798 entangled_cli-2.0.0a1/pyproject.toml
--rw-r--r--   0        0        0     4189 1970-01-01 00:00:00.000000 entangled_cli-2.0.0a1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-19 23:39:32.943040 entangled_cli-2.0.0a2/LICENSE
+-rw-r--r--   0        0        0     3636 2023-05-19 23:39:32.943040 entangled_cli-2.0.0a2/README.md
+-rw-r--r--   0        0        0        1 2023-05-19 23:39:32.943040 entangled_cli-2.0.0a2/entangled/__init__.py
+-rw-r--r--   0        0        0     2366 2023-05-19 23:39:32.943040 entangled_cli-2.0.0a2/entangled/code_reader.py
+-rw-r--r--   0        0        0      152 2023-05-19 23:39:32.943040 entangled_cli-2.0.0a2/entangled/commands/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-19 23:39:32.943040 entangled_cli-2.0.0a2/entangled/commands/init.py
+-rw-r--r--   0        0        0     1764 2023-05-19 23:39:32.943040 entangled_cli-2.0.0a2/entangled/commands/stitch.py
+-rw-r--r--   0        0        0     1184 2023-05-19 23:39:32.943040 entangled_cli-2.0.0a2/entangled/commands/sync.py
+-rw-r--r--   0        0        0     1587 2023-05-19 23:39:32.943040 entangled_cli-2.0.0a2/entangled/commands/tangle.py
+-rw-r--r--   0        0        0     1292 2023-05-19 23:39:32.943040 entangled_cli-2.0.0a2/entangled/commands/watch.py
+-rw-r--r--   0        0        0     2490 2023-05-19 23:39:32.943040 entangled_cli-2.0.0a2/entangled/config/__init__.py
+-rw-r--r--   0        0        0     1275 2023-05-19 23:39:32.943040 entangled_cli-2.0.0a2/entangled/config/language.py
+-rw-r--r--   0        0        0      606 2023-05-19 23:39:32.943040 entangled_cli-2.0.0a2/entangled/config/version.py
+-rw-r--r--   0        0        0     1775 2023-05-19 23:39:32.943040 entangled_cli-2.0.0a2/entangled/construct.py
+-rw-r--r--   0        0        0        1 2023-05-19 23:39:32.943040 entangled_cli-2.0.0a2/entangled/data/defaults.toml
+-rw-r--r--   0        0        0     3664 2023-05-19 23:39:32.943040 entangled_cli-2.0.0a2/entangled/document.py
+-rw-r--r--   0        0        0      738 2023-05-19 23:39:32.943040 entangled_cli-2.0.0a2/entangled/error.py
+-rw-r--r--   0        0        0     5186 2023-05-19 23:39:32.943040 entangled_cli-2.0.0a2/entangled/filedb.py
+-rw-r--r--   0        0        0      652 2023-05-19 23:39:32.947041 entangled_cli-2.0.0a2/entangled/hooks/__init__.py
+-rw-r--r--   0        0        0      653 2023-05-19 23:39:32.947041 entangled_cli-2.0.0a2/entangled/hooks/base.py
+-rw-r--r--   0        0        0     1494 2023-05-19 23:39:32.947041 entangled_cli-2.0.0a2/entangled/hooks/build.py
+-rw-r--r--   0        0        0     1455 2023-05-19 23:39:32.947041 entangled_cli-2.0.0a2/entangled/main.py
+-rw-r--r--   0        0        0     4003 2023-05-19 23:39:32.947041 entangled_cli-2.0.0a2/entangled/markdown_reader.py
+-rw-r--r--   0        0        0     5507 2023-05-19 23:39:32.947041 entangled_cli-2.0.0a2/entangled/parsing.py
+-rw-r--r--   0        0        0     2440 2023-05-19 23:39:32.947041 entangled_cli-2.0.0a2/entangled/properties.py
+-rw-r--r--   0        0        0        0 2023-05-19 23:39:32.947041 entangled_cli-2.0.0a2/entangled/py.typed
+-rw-r--r--   0        0        0     1067 2023-05-19 23:39:32.947041 entangled_cli-2.0.0a2/entangled/tangle.py
+-rw-r--r--   0        0        0     5460 2023-05-19 23:39:32.947041 entangled_cli-2.0.0a2/entangled/transaction.py
+-rw-r--r--   0        0        0      834 2023-05-19 23:39:32.947041 entangled_cli-2.0.0a2/entangled/utility.py
+-rw-r--r--   0        0        0       30 2023-05-19 23:39:32.947041 entangled_cli-2.0.0a2/entangled/version.py
+-rw-r--r--   0        0        0     1170 2023-05-19 23:39:32.947041 entangled_cli-2.0.0a2/pyproject.toml
+-rw-r--r--   0        0        0     4300 1970-01-01 00:00:00.000000 entangled_cli-2.0.0a2/PKG-INFO
```

### Comparing `entangled_cli-2.0.0a1/LICENSE` & `entangled_cli-2.0.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `entangled_cli-2.0.0a1/README.md` & `entangled_cli-2.0.0a2/README.md`

 * *Files identical despite different names*

### Comparing `entangled_cli-2.0.0a1/entangled/code_reader.py` & `entangled_cli-2.0.0a2/entangled/code_reader.py`

 * *Files identical despite different names*

### Comparing `entangled_cli-2.0.0a1/entangled/commands/stitch.py` & `entangled_cli-2.0.0a2/entangled/commands/stitch.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,16 +6,14 @@
 
 from ..config import config
 from ..code_reader import CodeReader
 from ..markdown_reader import MarkdownReader
 from ..document import ReferenceMap, Content, PlainText, ReferenceId
 from ..transaction import transaction, TransactionMode
 
-from .tangle import tangle
-
 
 def stitch_markdown(reference_map: ReferenceMap, content: list[Content]) -> str:
     def get(item: Content):
         match item:
             case PlainText(s):
                 return s
             case ReferenceId():
```

### Comparing `entangled_cli-2.0.0a1/entangled/commands/sync.py` & `entangled_cli-2.0.0a2/entangled/commands/sync.py`

 * *Files 10% similar despite different names*

```diff
@@ -21,15 +21,14 @@
     with file_db(readonly=True) as db:
         changed = set(db.changed())
 
         if not all(f in db for f in input_file_list):
             return tangle
 
         if not changed:
-            logging.info("Nothing to be done")
             return None
 
         if changed.isdisjoint(db.managed):
             logging.info("Tangling")
             return tangle
 
         if changed.issubset(db.managed):
```

### Comparing `entangled_cli-2.0.0a1/entangled/commands/watch.py` & `entangled_cli-2.0.0a2/entangled/commands/watch.py`

 * *Files identical despite different names*

### Comparing `entangled_cli-2.0.0a1/entangled/document.py` & `entangled_cli-2.0.0a2/entangled/document.py`

 * *Files identical despite different names*

### Comparing `entangled_cli-2.0.0a1/entangled/error.py` & `entangled_cli-2.0.0a2/entangled/error.py`

 * *Files identical despite different names*

### Comparing `entangled_cli-2.0.0a1/entangled/filedb.py` & `entangled_cli-2.0.0a2/entangled/filedb.py`

 * *Files 4% similar despite different names*

```diff
@@ -123,14 +123,16 @@
     def __contains__(self, path: Path) -> bool:
         return path in self._files
 
     def __getitem__(self, path: Path) -> FileStat:
         return self._files[path]
 
     def __delitem__(self, path: Path):
+        if path in self._target:
+            self._target.remove(path)
         del self._files[path]
 
     @property
     def files(self) -> Iterable[Path]:
         return self._files.keys()
 
     def check(self, path: Path, content: str) -> bool:
```

### Comparing `entangled_cli-2.0.0a1/entangled/main.py` & `entangled_cli-2.0.0a2/entangled/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 import argh  # type: ignore
 import logging
+import sys
+
 
 try:
     from rich.logging import RichHandler
     from rich.highlighter import RegexHighlighter
 
     WITH_RICH = True
 except ImportError:
@@ -40,19 +42,24 @@
 
     logging.info("Welcome to Entangled (https://entangled.github.io/)")
 
 
 def cli():
     import argparse
 
-    parser = argparse.ArgumentParser()
-    parser.add_argument(
-        "-d", "--debug", action="store_true", help="enable debug messages"
-    )
-    argh.add_commands(parser, [tangle, stitch, sync, watch])
-    args = parser.parse_args()
-    configure(args.debug)
-    argh.dispatch(parser)
+    try:
+        parser = argparse.ArgumentParser()
+        parser.add_argument(
+            "-d", "--debug", action="store_true", help="enable debug messages"
+        )
+        argh.add_commands(parser, [tangle, stitch, sync, watch])
+        args = parser.parse_args()
+        configure(args.debug)
+        argh.dispatch(parser)
+    except KeyboardInterrupt:
+        logging.info("Goodbye")
+        sys.exit(0)
 
 
 if __name__ == "__main__":
-    cli()
+        cli()
+
```

### Comparing `entangled_cli-2.0.0a1/entangled/markdown_reader.py` & `entangled_cli-2.0.0a2/entangled/markdown_reader.py`

 * *Files 11% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import re
 import mawk
 
 from .config import config
 from .utility import first
 from .document import TextLocation, CodeBlock, ReferenceMap, Content, PlainText
 from .properties import read_properties, get_attribute, get_classes, get_id
+from .hooks.base import HookBase
 
 
 @dataclass
 class MarkdownError(Exception):
     location: TextLocation
     what: str
 
@@ -22,43 +23,47 @@
 
 
 class MarkdownReader(mawk.RuleSet):
     """Reads a Markdown file, and splits it up into code blocks and other
     content. The contents of the code blocks get stored in `reference_map`.
     """
 
-    def __init__(self, filename: str, refs: Optional[ReferenceMap] = None):
+    def __init__(self, filename: str, refs: Optional[ReferenceMap] = None, hooks: Optional[list[HookBase]] = None):
         self.location = TextLocation(filename)
         self.reference_map = refs or ReferenceMap()
         self.content: list[Content] = []
         self.inside_codeblock: bool = False
         self.current_content: list[str] = []
+        self.hooks = hooks or []
 
     def flush_plain_text(self):
         self.content.append(PlainText("\n".join(self.current_content)))
         self.current_content = []
 
     @mawk.always
     def on_next_line(self, _):
         self.location.line_number += 1
 
-    @mawk.on_match(r"^(?P<indent>\s*)```\s*{(?P<properties>[^{}]*)}\s*$")
+    @mawk.on_match(config.markers.open)
     def on_open_codeblock(self, m: re.Match) -> Optional[list[str]]:
         if self.inside_codeblock:
             return None
         self.current_codeblock_indent = m["indent"]
         self.current_codeblock_location = copy(self.location)
         self.current_codeblock_properties = read_properties(m["properties"])
         self.current_content.append(m[0])
         self.flush_plain_text()
         self.inside_codeblock = True
         return []
 
-    @mawk.on_match(r"^(?P<indent>\s*)```\s*$")
+    @mawk.on_match(config.markers.close)
     def on_close_codeblock(self, m: re.Match):
+        if not self.inside_codeblock:
+            return
+        
         if len(m["indent"]) < len(self.current_codeblock_indent):
             raise MarkdownError(self.location, "indentation error")
 
         if m["indent"] != self.current_codeblock_indent:
             return  # treat this as code-block content
 
         # add block to reference-map
@@ -70,25 +75,31 @@
 
         if ref_name is None or language is None:
             self.flush_plain_text()
         else:
             ref = self.reference_map.new_id(
                 self.current_codeblock_location.filename, ref_name
             )
-            self.reference_map[ref] = CodeBlock(
+            code = CodeBlock(
                 language,
                 self.current_codeblock_properties,
                 self.current_codeblock_indent,
                 "\n".join(self.current_content),
                 self.current_codeblock_location,
             )
+            self.reference_map[ref] = code
             if target_file is not None:
                 self.reference_map.targets.add(target_file)
             self.content.append(ref)
             self.current_content = []
+
+            for h in self.hooks:
+                if h.condition(self.current_codeblock_properties):
+                    h.on_read(ref, code)
+            
         self.current_content.append(m[0])
         self.inside_codeblock = False
         return []
 
     @mawk.always
     def add_line(self, line: str):
         self.current_content.append(line)
```

### Comparing `entangled_cli-2.0.0a1/entangled/parsing.py` & `entangled_cli-2.0.0a2/entangled/parsing.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,21 +66,19 @@
     failures: list[Failure]
 
     @property
     def expected(self):
         return " | ".join(str(f) for f in self.failures)
 
 
-class Parser(Generic[T], ABC):
+class Parser(Generic[T]):
     """Base class for parsers."""
-
-    @abstractmethod
     def read(self, inp: str) -> tuple[T, str]:
         """Read a string and return an object the remainder of the string."""
-        ...
+        raise NotImplementedError()
 
     def __rshift__(self, f: Callable[[T], Parser[U]]) -> Parser[U]:
         return bind(self, f)
 
     def then(self, p: Parser[U]) -> Parser[U]:
         return bind(self, lambda _: p)
```

### Comparing `entangled_cli-2.0.0a1/entangled/properties.py` & `entangled_cli-2.0.0a2/entangled/properties.py`

 * *Files identical despite different names*

### Comparing `entangled_cli-2.0.0a1/entangled/transaction.py` & `entangled_cli-2.0.0a2/entangled/transaction.py`

 * *Files 1% similar despite different names*

```diff
@@ -41,14 +41,15 @@
 
     def conflict(self, _) -> Optional[str]:
         if self.target.exists():
             return f"{self.target} already exists and is not managed by Entangled"
         return None
 
     def run(self, db: FileDB):
+        self.target.parent.mkdir(parents=True, exist_ok=True)
         with open(self.target, "w") as f:
             f.write(self.content)
         db.update(self.target, self.sources)
         if self.sources != []:
             db.managed.add(self.target)
 
     def __str__(self):
```

### Comparing `entangled_cli-2.0.0a1/entangled/utility.py` & `entangled_cli-2.0.0a2/entangled/utility.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,16 @@
-from typing import Iterable, Optional, TypeVar, TypeGuard
+from typing import Iterable, Optional, TypeVar, TypeGuard, Union
+from dataclasses import is_dataclass
 from contextlib import contextmanager
 import os
 from pathlib import Path
 
+import typing
+import types
+
 
 T = TypeVar("T")
 
 
 @contextmanager
 def pushd(wd: Path):
     olddir = os.getcwd()
@@ -32,7 +36,9 @@
 
 
 def cat_maybes(it: Iterable[Optional[T]]) -> Iterable[T]:
     def pred(x: Optional[T]) -> TypeGuard[T]:
         return x is not None
 
     return filter(pred, it)
+
+
```

### Comparing `entangled_cli-2.0.0a1/pyproject.toml` & `entangled_cli-2.0.0a2/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 [tool.poetry]
 name = "entangled-cli"
-version = "2.0.0-alpha-1"
-description = "Python port of Entangled"
+version = "2.0.0-alpha-2"
+description = "Literate Programming toolbox"
+repository = "https://github.com/entangled/entangled.py"
+homepage = "https://entangled.github.io/"
 authors = ["Johan Hidding <j.hidding@esciencecenter.nl>"]
 license = "Apache 2"
 readme = "README.md"
 packages = [
     { include = "entangled" }
 ]
```

### Comparing `entangled_cli-2.0.0a1/PKG-INFO` & `entangled_cli-2.0.0a2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 Metadata-Version: 2.1
 Name: entangled-cli
-Version: 2.0.0a1
-Summary: Python port of Entangled
+Version: 2.0.0a2
+Summary: Literate Programming toolbox
+Home-page: https://entangled.github.io/
 License: Apache 2
 Author: Johan Hidding
 Author-email: j.hidding@esciencecenter.nl
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: argh (>=0.28.1,<0.29.0)
 Requires-Dist: filelock (>=3.12.0,<4.0.0)
 Requires-Dist: mawk (>=0.1.3,<0.2.0)
 Requires-Dist: watchdog (>=3.0.0,<4.0.0)
+Project-URL: Repository, https://github.com/entangled/entangled.py
 Description-Content-Type: text/markdown
 
 # Entangled
 Entangled is a solution for Literate Programming, a technique in which the programmer writes a human narrative first, then implementing the program in code blocks.
 Literate programming was introduced by Donald Knuth in 1984 and has since then found several surges in popularity. One thing holding back the popularity of literate programming is the lack of maintainability under increasing program complexity. Entangled solves this issue by offering a two-way synchronisation mechanism. You can edit and debug your code as normal in your favourite IDE or text editor. Entangled will make sure that your Markdown files stay up-to-date with your code and vice-versa. Because Entangled works with Markdown, you can use it with most static document generators. To summarise, you keep using:
 
 - your favourite **editor**: Entangled runs as a daemon in the background, keeping your text files synchronised.
```

