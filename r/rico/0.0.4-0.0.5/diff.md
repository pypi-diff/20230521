# Comparing `tmp/rico-0.0.4.tar.gz` & `tmp/rico-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rico-0.0.4.tar", last modified: Sat May 13 14:32:50 2023, max compression
+gzip compressed data, was "rico-0.0.5.tar", last modified: Sun May 21 09:50:45 2023, max compression
```

## Comparing `rico-0.0.4.tar` & `rico-0.0.5.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1070 2023-05-13 14:32:24.337670 rico-0.0.4/LICENSE
--rw-r--r--   0        0        0       53 2023-05-13 14:32:24.337670 rico-0.0.4/README.md
--rw-r--r--   0        0        0     2692 2023-05-13 14:32:50.094163 rico-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      106 2023-05-13 14:32:24.337670 rico-0.0.4/src/rico/__init__.py
--rw-r--r--   0        0        0      340 2023-05-13 14:32:24.337670 rico-0.0.4/src/rico/_version.py
--rw-r--r--   0        0        0     1075 2023-05-13 14:32:24.337670 rico-0.0.4/src/rico/core.py
--rw-r--r--   0        0        0     5109 2023-05-13 14:32:24.337670 rico-0.0.4/src/rico/html.py
--rw-r--r--   0        0        0       18 2023-05-13 14:32:24.337670 rico-0.0.4/tests/__init__.py
--rw-r--r--   0        0        0      751 2023-05-13 14:32:24.337670 rico-0.0.4/tests/test_core.py
--rw-r--r--   0        0        0     7879 2023-05-13 14:32:24.337670 rico-0.0.4/tests/test_html.py
--rw-r--r--   0        0        0     1280 1970-01-01 00:00:00.000000 rico-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-21 09:50:12.834578 rico-0.0.5/LICENSE
+-rw-r--r--   0        0        0      715 2023-05-21 09:50:12.834578 rico-0.0.5/README.md
+-rw-r--r--   0        0        0     2937 2023-05-21 09:50:45.610880 rico-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      391 2023-05-21 09:50:12.834578 rico-0.0.5/src/rico/__init__.py
+-rw-r--r--   0        0        0      340 2023-05-21 09:50:12.834578 rico-0.0.5/src/rico/_version.py
+-rw-r--r--   0        0        0    10646 2023-05-21 09:50:12.834578 rico-0.0.5/src/rico/content.py
+-rw-r--r--   0        0        0     6861 2023-05-21 09:50:12.834578 rico-0.0.5/src/rico/html.py
+-rw-r--r--   0        0        0       18 2023-05-21 09:50:12.834578 rico-0.0.5/tests/__init__.py
+-rw-r--r--   0        0        0    11383 2023-05-21 09:50:12.834578 rico-0.0.5/tests/test_content.py
+-rw-r--r--   0        0        0     8843 2023-05-21 09:50:12.834578 rico-0.0.5/tests/test_html.py
+-rw-r--r--   0        0        0     2138 1970-01-01 00:00:00.000000 rico-0.0.5/PKG-INFO
```

### Comparing `rico-0.0.4/LICENSE` & `rico-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `rico-0.0.4/pyproject.toml` & `rico-0.0.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "rico"
 dynamic = []
-description = "Rich content to HTML as easy as doc.print(x)."
+description = "Rich content to HTML as easy as Doc([df, plot])."
 authors = [
     { name = "Evgeny Ivanov", email = "ivanov.evgeny.n@gmail.com" },
 ]
 dependencies = []
 requires-python = ">=3.10"
 readme = "README.md"
 classifiers = [
@@ -18,33 +18,40 @@
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: Scientific/Engineering",
     "Topic :: Scientific/Engineering :: Visualization",
     "Topic :: Text Processing",
     "Topic :: Text Processing :: Markup",
     "Topic :: Text Processing :: Markup :: HTML",
+    "Topic :: Text Processing :: Markup :: Markdown",
 ]
-version = "0.0.4"
+version = "0.0.5"
 
 [project.license]
 text = "MIT"
 
+[project.urls]
+source = "https://github.com/e10v/rico"
+
 [project.optional-dependencies]
 altair = [
     "altair>=4.2",
     "vl-convert-python>=0.8",
 ]
+markdown = [
+    "markdown>=3.3",
+]
 pyplot = [
     "matplotlib>=3.5",
 ]
 seaborn = [
     "seaborn>=0.12",
 ]
 complete = [
-    "rico[altair,pyplot,seaborn]",
+    "rico[altair,markdown,pyplot,seaborn]",
 ]
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
@@ -131,19 +138,23 @@
     "TID",
     "TRY",
     "UP",
     "W",
 ]
 ignore = [
     "ANN101",
+    "ANN102",
     "ANN204",
     "ANN401",
     "B006",
+    "N817",
+    "PGH003",
     "PT001",
     "SLF001",
+    "TRY003",
 ]
 
 [tool.ruff.per-file-ignores]
 "tests/*" = [
     "ANN201",
     "D100",
     "D103",
@@ -158,7 +169,10 @@
 ]
 
 [tool.ruff.pydocstyle]
 convention = "google"
 ignore-decorators = [
     "typing.overload",
 ]
+
+[tool.ruff.pylint]
+max-args = 8
```

### Comparing `rico-0.0.4/src/rico/html.py` & `rico-0.0.5/src/rico/html.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 """HTML parser and serializer."""
 
 from __future__ import annotations
 
 import html.parser
-import xml.etree.ElementTree as ET  # noqa: N817
+import xml.etree.ElementTree as ET
 
 
-TAGS_WITHOUT_INDENT = {"pre"}
+TAGS_EMPTY = {
+    "area", "base", "basefont", "br", "col", "embed", "frame", "hr", "img",
+    "input", "isindex", "link", "meta", "param", "path", "source", "track", "wbr",
+}
 
-# Copy of xml.etree.ElementTree.HTML_EMPTY
-HTML_EMPTY = {
-    "area", "base", "basefont", "br", "col", "embed", "frame", "hr",
-    "img", "input", "isindex", "link", "meta", "param", "source",
-    "track", "wbr",
+TAGS_INLINE = {
+    "a", "abbr", "b", "bdi", "bdo", "br", "cite", "code", "data", "dfn", "em",
+    "i", "kbd", "mark", "q", "rp", "rt", "ruby", "s", "samp", "small", "span",
+    "strong", "sub", "sup", "time", "u", "var", "wbr",
 }
 
+TAGS_NOT_ESCAPED = {"script", "style"}
+TAGS_PRE_FORMATTED = {"pre"}
+
 
 class HTMLParser(html.parser.HTMLParser):
     """Simple HTML parser. Returns a list of instances of ET.Element on close().
 
     Assigns None values to boolean attributes.
 
     Ignores comments, doctype declaration and processing instructions.
@@ -70,29 +75,29 @@
 
 
 def indent_html(
     element: ET.Element,
     space: str = "  ",
     level: int = 0,
 ) -> ET.Element:
-    """Indent an HTML document.
+    """Indent an HTML element.
 
     Tnsert newlines and indentation space after elements.
-    Create a new document instead of updating inplace.
+    Create a new element instead of updating inplace.
     Do not indent elements inside <pre> tag.
 
     Args:
         element: The element to indent.
         space: The whitespace to insert for each indentation level.
         level: The initial indentation level. Should always be 0.
 
     Returns:
-        The indented HTML document.
+        The indented HTML element.
     """
-    if element.tag in TAGS_WITHOUT_INDENT or not len(element):
+    if element.tag.lower() in TAGS_PRE_FORMATTED or not len(element):
         return element
 
     indented_element = ET.Element(element.tag, attrib=element.attrib)
     indented_element.text = element.text
     indented_element.tail = element.tail
 
     if not element.text or not element.text.strip():
@@ -108,14 +113,56 @@
 
     if not indented_child.tail or not indented_child.tail.strip():  # pyright: ignore [reportUnboundVariable]  # noqa: E501
         indented_child.tail = "\n" + space * level  # pyright: ignore [reportUnboundVariable]  # noqa: E501
 
     return indented_element
 
 
+def strip_html(element: ET.Element) -> ET.Element:
+    """Strip an HTML element.
+
+    Remove unnecessary whitespaces from the element by strippping elements'
+    text and tail.
+    Do not strip elements inside <pre> tag or inside inline tags.
+
+    Args:
+        element: The element to strip.
+
+    Returns:
+        The stripped HTML element.
+    """
+    stripped_element = ET.Element(element.tag, attrib=element.attrib)
+    stripped_element.text = element.text
+    stripped_element.tail = element.tail
+
+    if element.tag.lower() in TAGS_INLINE | TAGS_PRE_FORMATTED:
+        for child in element:
+            stripped_element.append(child)
+    else:
+        for child in element:
+            stripped_element.append(strip_html(child))
+
+        if stripped_element.text:
+            if len(stripped_element) == 0 and (
+                not stripped_element.tail or
+                not stripped_element.tail.strip()
+            ):
+                stripped_element.text = stripped_element.text.strip()
+            else:
+                stripped_element.text = stripped_element.text.lstrip()
+
+    if stripped_element.tail:
+        if len(stripped_element) == 0 and not stripped_element.text:
+            stripped_element.tail = stripped_element.tail.strip()
+        else:
+            stripped_element.tail = stripped_element.tail.rstrip()
+
+    return stripped_element
+
+
 def _escape_cdata(text: str) -> str:
     """Copy of xml.etree.ElementTree._escape_cdata."""
     if "&" in text:
         text = text.replace("&", "&amp;")
     if "<" in text:
         text = text.replace("<", "&lt;")
     if ">" in text:
@@ -128,47 +175,53 @@
         text = text.replace("&", "&amp;")
     if ">" in text:
         text = text.replace(">", "&gt;")
     if '"' in text:
         text = text.replace('"', "&quot;")
     return text
 
-def serialize_html(element: ET.Element, indent_space: str | None = None) -> str:
+def serialize_html(
+    element: ET.Element,
+    indent_space: str | None = None,
+    strip: bool = False,
+) -> str:
     """Serialize an HTML document to a string.
 
     Indent the document if `indent_space` is not None.
 
     Serialize attributes with None values as boolean.
 
     Args:
         element: The HTML document.
         indent_space: The whitespace for indentation.
+        strip: If True, strip unnecessary whitespace.
 
     Returns:
         The serialized HTML document.
     """
+    if strip:
+        element = strip_html(element)
+
     if indent_space is not None:
         element = indent_html(element, space=indent_space)
 
     attrib = "".join(
         f' {k}="{_escape_attrib_html(v)}"'
         if v is not None  # pyright: ignore [reportUnnecessaryComparison]
+        # Serialize attributes with None values as boolean.
         else f" {k}"
         for k, v in element.items()
     )
 
-    tag = f"<{element.tag}{attrib}>"
+    opening_tag = f"<{element.tag}{attrib}>"
     ltag = element.tag.lower()
 
     if element.text is not None:
-        if ltag == "script" or ltag == "style":
-            text = element.text
-        else:
-            text = _escape_cdata(element.text)
+        text = element.text if ltag in TAGS_NOT_ESCAPED else _escape_cdata(element.text)
     else:
         text = ""
 
     children = "".join(serialize_html(e) for e in element)
-    closing_tag = f"</{element.tag}>" if ltag not in HTML_EMPTY else ""
+    closing_tag = f"</{element.tag}>" if ltag not in TAGS_EMPTY else ""
     tail = _escape_cdata(element.tail) if element.tail is not None else ""
 
-    return f"{tag}{text}{children}{closing_tag}{tail}"
+    return opening_tag + text + children + closing_tag + tail
```

