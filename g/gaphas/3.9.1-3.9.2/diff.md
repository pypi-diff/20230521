# Comparing `tmp/gaphas-3.9.1.tar.gz` & `tmp/gaphas-3.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gaphas-3.9.1.tar", max compression
+gzip compressed data, was "gaphas-3.9.2.tar", max compression
```

## Comparing `gaphas-3.9.1.tar` & `gaphas-3.9.2.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0    10175 2022-12-17 14:32:05.060337 gaphas-3.9.1/LICENSE
--rw-r--r--   0        0        0     9701 2022-12-17 14:32:05.060337 gaphas-3.9.1/README.md
--rw-r--r--   0        0        0     1195 2022-12-17 14:32:05.064338 gaphas-3.9.1/gaphas/__init__.py
--rw-r--r--   0        0        0      376 2022-12-17 14:32:05.064338 gaphas-3.9.1/gaphas/aspect/__init__.py
--rw-r--r--   0        0        0      201 2022-12-17 14:32:05.064338 gaphas-3.9.1/gaphas/aspect/connector.py
--rw-r--r--   0        0        0      140 2022-12-17 14:32:05.064338 gaphas-3.9.1/gaphas/aspect/handlemove.py
--rw-r--r--   0        0        0       69 2022-12-17 14:32:05.064338 gaphas-3.9.1/gaphas/aspect/move.py
--rw-r--r--   0        0        0     8860 2022-12-17 14:32:05.064338 gaphas-3.9.1/gaphas/canvas.py
--rw-r--r--   0        0        0     8972 2022-12-17 14:32:05.064338 gaphas-3.9.1/gaphas/connections.py
--rw-r--r--   0        0        0     5357 2022-12-17 14:32:05.064338 gaphas-3.9.1/gaphas/connector.py
--rw-r--r--   0        0        0    16757 2022-12-17 14:32:05.068338 gaphas-3.9.1/gaphas/constraint.py
--rw-r--r--   0        0        0      816 2022-12-17 14:32:05.068338 gaphas-3.9.1/gaphas/cursor.py
--rw-r--r--   0        0        0     4083 2022-12-17 14:32:05.068338 gaphas-3.9.1/gaphas/decorators.py
--rw-r--r--   0        0        0    17898 2022-12-17 14:32:05.068338 gaphas-3.9.1/gaphas/geometry.py
--rw-r--r--   0        0        0     8080 2022-12-17 14:32:05.068338 gaphas-3.9.1/gaphas/guide.py
--rw-r--r--   0        0        0     2800 2022-12-17 14:32:05.068338 gaphas-3.9.1/gaphas/handle.py
--rw-r--r--   0        0        0     4768 2022-12-17 14:32:05.068338 gaphas-3.9.1/gaphas/handlemove.py
--rw-r--r--   0        0        0    13292 2022-12-17 14:32:05.068338 gaphas-3.9.1/gaphas/item.py
--rw-r--r--   0        0        0     4022 2022-12-17 14:32:05.068338 gaphas-3.9.1/gaphas/matrix.py
--rw-r--r--   0        0        0     2312 2022-12-17 14:32:05.068338 gaphas-3.9.1/gaphas/model.py
--rw-r--r--   0        0        0     1380 2022-12-17 14:32:05.068338 gaphas-3.9.1/gaphas/move.py
--rw-r--r--   0        0        0      661 2022-12-17 14:32:05.068338 gaphas-3.9.1/gaphas/painter/__init__.py
--rw-r--r--   0        0        0     1305 2022-12-17 14:32:05.068338 gaphas-3.9.1/gaphas/painter/boundingboxpainter.py
--rw-r--r--   0        0        0      867 2022-12-17 14:32:05.068338 gaphas-3.9.1/gaphas/painter/chain.py
--rw-r--r--   0        0        0     4747 2022-12-17 14:32:05.068338 gaphas-3.9.1/gaphas/painter/freehand.py
--rw-r--r--   0        0        0     2986 2022-12-17 14:32:05.068338 gaphas-3.9.1/gaphas/painter/handlepainter.py
--rw-r--r--   0        0        0     1115 2022-12-17 14:32:05.068338 gaphas-3.9.1/gaphas/painter/itempainter.py
--rw-r--r--   0        0        0      801 2022-12-17 14:32:05.068338 gaphas-3.9.1/gaphas/painter/painter.py
--rw-r--r--   0        0        0     3581 2022-12-17 14:32:05.068338 gaphas-3.9.1/gaphas/port.py
--rw-r--r--   0        0        0     5420 2022-12-17 14:32:05.068338 gaphas-3.9.1/gaphas/position.py
--rw-r--r--   0        0        0    11310 2022-12-17 14:32:05.068338 gaphas-3.9.1/gaphas/quadtree.py
--rw-r--r--   0        0        0     7566 2022-12-17 14:32:05.068338 gaphas-3.9.1/gaphas/segment.py
--rw-r--r--   0        0        0     2523 2022-12-17 14:32:05.068338 gaphas-3.9.1/gaphas/selection.py
--rw-r--r--   0        0        0      268 2022-12-17 14:32:05.068338 gaphas-3.9.1/gaphas/solver/__init__.py
--rw-r--r--   0        0        0     4088 2022-12-17 14:32:05.068338 gaphas-3.9.1/gaphas/solver/constraint.py
--rw-r--r--   0        0        0     6955 2022-12-17 14:32:05.068338 gaphas-3.9.1/gaphas/solver/solver.py
--rw-r--r--   0        0        0     7443 2022-12-17 14:32:05.068338 gaphas-3.9.1/gaphas/solver/variable.py
--rw-r--r--   0        0        0     6436 2022-12-17 14:32:05.068338 gaphas-3.9.1/gaphas/table.py
--rw-r--r--   0        0        0     1070 2022-12-17 14:32:05.068338 gaphas-3.9.1/gaphas/tool/__init__.py
--rw-r--r--   0        0        0     1225 2022-12-17 14:32:05.068338 gaphas-3.9.1/gaphas/tool/hover.py
--rw-r--r--   0        0        0     6662 2022-12-17 14:32:05.068338 gaphas-3.9.1/gaphas/tool/itemtool.py
--rw-r--r--   0        0        0     1990 2022-12-17 14:32:05.068338 gaphas-3.9.1/gaphas/tool/placement.py
--rw-r--r--   0        0        0     2577 2022-12-17 14:32:05.068338 gaphas-3.9.1/gaphas/tool/rubberband.py
--rw-r--r--   0        0        0     2731 2022-12-17 14:32:05.068338 gaphas-3.9.1/gaphas/tool/scroll.py
--rw-r--r--   0        0        0      475 2022-12-17 14:32:05.068338 gaphas-3.9.1/gaphas/tool/viewfocus.py
--rw-r--r--   0        0        0     2975 2022-12-17 14:32:05.068338 gaphas-3.9.1/gaphas/tool/zoom.py
--rw-r--r--   0        0        0     9143 2022-12-17 14:32:05.068338 gaphas-3.9.1/gaphas/tree.py
--rw-r--r--   0        0        0      629 2022-12-17 14:32:05.068338 gaphas-3.9.1/gaphas/types.py
--rw-r--r--   0        0        0     3625 2022-12-17 14:32:05.068338 gaphas-3.9.1/gaphas/util.py
--rw-r--r--   0        0        0      177 2022-12-17 14:32:05.068338 gaphas-3.9.1/gaphas/view/__init__.py
--rw-r--r--   0        0        0    16643 2022-12-17 14:32:05.068338 gaphas-3.9.1/gaphas/view/gtkview.py
--rw-r--r--   0        0        0     4074 2022-12-17 14:32:05.068338 gaphas-3.9.1/gaphas/view/scrolling.py
--rw-r--r--   0        0        0     2845 2022-12-17 14:32:05.068338 gaphas-3.9.1/pyproject.toml
--rw-r--r--   0        0        0    10783 1970-01-01 00:00:00.000000 gaphas-3.9.1/setup.py
--rw-r--r--   0        0        0    10998 1970-01-01 00:00:00.000000 gaphas-3.9.1/PKG-INFO
+-rw-r--r--   0        0        0    10175 2022-12-21 14:51:19.820837 gaphas-3.9.2/LICENSE
+-rw-r--r--   0        0        0     9701 2022-12-21 14:51:19.820837 gaphas-3.9.2/README.md
+-rw-r--r--   0        0        0     1195 2022-12-21 14:51:19.824837 gaphas-3.9.2/gaphas/__init__.py
+-rw-r--r--   0        0        0      376 2022-12-21 14:51:19.824837 gaphas-3.9.2/gaphas/aspect/__init__.py
+-rw-r--r--   0        0        0      201 2022-12-21 14:51:19.824837 gaphas-3.9.2/gaphas/aspect/connector.py
+-rw-r--r--   0        0        0      140 2022-12-21 14:51:19.824837 gaphas-3.9.2/gaphas/aspect/handlemove.py
+-rw-r--r--   0        0        0       69 2022-12-21 14:51:19.824837 gaphas-3.9.2/gaphas/aspect/move.py
+-rw-r--r--   0        0        0     8860 2022-12-21 14:51:19.824837 gaphas-3.9.2/gaphas/canvas.py
+-rw-r--r--   0        0        0     8972 2022-12-21 14:51:19.824837 gaphas-3.9.2/gaphas/connections.py
+-rw-r--r--   0        0        0     5357 2022-12-21 14:51:19.824837 gaphas-3.9.2/gaphas/connector.py
+-rw-r--r--   0        0        0    16757 2022-12-21 14:51:19.824837 gaphas-3.9.2/gaphas/constraint.py
+-rw-r--r--   0        0        0      816 2022-12-21 14:51:19.824837 gaphas-3.9.2/gaphas/cursor.py
+-rw-r--r--   0        0        0     4083 2022-12-21 14:51:19.824837 gaphas-3.9.2/gaphas/decorators.py
+-rw-r--r--   0        0        0    17898 2022-12-21 14:51:19.824837 gaphas-3.9.2/gaphas/geometry.py
+-rw-r--r--   0        0        0     8079 2022-12-21 14:51:19.824837 gaphas-3.9.2/gaphas/guide.py
+-rw-r--r--   0        0        0     2800 2022-12-21 14:51:19.824837 gaphas-3.9.2/gaphas/handle.py
+-rw-r--r--   0        0        0     4768 2022-12-21 14:51:19.824837 gaphas-3.9.2/gaphas/handlemove.py
+-rw-r--r--   0        0        0    13292 2022-12-21 14:51:19.824837 gaphas-3.9.2/gaphas/item.py
+-rw-r--r--   0        0        0     4022 2022-12-21 14:51:19.824837 gaphas-3.9.2/gaphas/matrix.py
+-rw-r--r--   0        0        0     2312 2022-12-21 14:51:19.824837 gaphas-3.9.2/gaphas/model.py
+-rw-r--r--   0        0        0     1380 2022-12-21 14:51:19.824837 gaphas-3.9.2/gaphas/move.py
+-rw-r--r--   0        0        0      661 2022-12-21 14:51:19.824837 gaphas-3.9.2/gaphas/painter/__init__.py
+-rw-r--r--   0        0        0     1305 2022-12-21 14:51:19.824837 gaphas-3.9.2/gaphas/painter/boundingboxpainter.py
+-rw-r--r--   0        0        0      867 2022-12-21 14:51:19.824837 gaphas-3.9.2/gaphas/painter/chain.py
+-rw-r--r--   0        0        0     4746 2022-12-21 14:51:19.824837 gaphas-3.9.2/gaphas/painter/freehand.py
+-rw-r--r--   0        0        0     2986 2022-12-21 14:51:19.824837 gaphas-3.9.2/gaphas/painter/handlepainter.py
+-rw-r--r--   0        0        0     1115 2022-12-21 14:51:19.824837 gaphas-3.9.2/gaphas/painter/itempainter.py
+-rw-r--r--   0        0        0      801 2022-12-21 14:51:19.824837 gaphas-3.9.2/gaphas/painter/painter.py
+-rw-r--r--   0        0        0     3581 2022-12-21 14:51:19.824837 gaphas-3.9.2/gaphas/port.py
+-rw-r--r--   0        0        0     5420 2022-12-21 14:51:19.824837 gaphas-3.9.2/gaphas/position.py
+-rw-r--r--   0        0        0    11310 2022-12-21 14:51:19.824837 gaphas-3.9.2/gaphas/quadtree.py
+-rw-r--r--   0        0        0     7566 2022-12-21 14:51:19.824837 gaphas-3.9.2/gaphas/segment.py
+-rw-r--r--   0        0        0     2523 2022-12-21 14:51:19.824837 gaphas-3.9.2/gaphas/selection.py
+-rw-r--r--   0        0        0      268 2022-12-21 14:51:19.824837 gaphas-3.9.2/gaphas/solver/__init__.py
+-rw-r--r--   0        0        0     4088 2022-12-21 14:51:19.824837 gaphas-3.9.2/gaphas/solver/constraint.py
+-rw-r--r--   0        0        0     7211 2022-12-21 14:51:19.824837 gaphas-3.9.2/gaphas/solver/solver.py
+-rw-r--r--   0        0        0     7443 2022-12-21 14:51:19.824837 gaphas-3.9.2/gaphas/solver/variable.py
+-rw-r--r--   0        0        0     6436 2022-12-21 14:51:19.824837 gaphas-3.9.2/gaphas/table.py
+-rw-r--r--   0        0        0     1070 2022-12-21 14:51:19.824837 gaphas-3.9.2/gaphas/tool/__init__.py
+-rw-r--r--   0        0        0     1365 2022-12-21 14:51:19.824837 gaphas-3.9.2/gaphas/tool/hover.py
+-rw-r--r--   0        0        0     6662 2022-12-21 14:51:19.824837 gaphas-3.9.2/gaphas/tool/itemtool.py
+-rw-r--r--   0        0        0     1990 2022-12-21 14:51:19.824837 gaphas-3.9.2/gaphas/tool/placement.py
+-rw-r--r--   0        0        0     2577 2022-12-21 14:51:19.824837 gaphas-3.9.2/gaphas/tool/rubberband.py
+-rw-r--r--   0        0        0     2731 2022-12-21 14:51:19.824837 gaphas-3.9.2/gaphas/tool/scroll.py
+-rw-r--r--   0        0        0      475 2022-12-21 14:51:19.824837 gaphas-3.9.2/gaphas/tool/viewfocus.py
+-rw-r--r--   0        0        0     2975 2022-12-21 14:51:19.824837 gaphas-3.9.2/gaphas/tool/zoom.py
+-rw-r--r--   0        0        0     9143 2022-12-21 14:51:19.824837 gaphas-3.9.2/gaphas/tree.py
+-rw-r--r--   0        0        0      629 2022-12-21 14:51:19.824837 gaphas-3.9.2/gaphas/types.py
+-rw-r--r--   0        0        0     3625 2022-12-21 14:51:19.824837 gaphas-3.9.2/gaphas/util.py
+-rw-r--r--   0        0        0      177 2022-12-21 14:51:19.824837 gaphas-3.9.2/gaphas/view/__init__.py
+-rw-r--r--   0        0        0    16643 2022-12-21 14:51:19.824837 gaphas-3.9.2/gaphas/view/gtkview.py
+-rw-r--r--   0        0        0     4074 2022-12-21 14:51:19.824837 gaphas-3.9.2/gaphas/view/scrolling.py
+-rw-r--r--   0        0        0     2146 2022-12-21 14:51:19.824837 gaphas-3.9.2/pyproject.toml
+-rw-r--r--   0        0        0    10783 1970-01-01 00:00:00.000000 gaphas-3.9.2/setup.py
+-rw-r--r--   0        0        0    10998 1970-01-01 00:00:00.000000 gaphas-3.9.2/PKG-INFO
```

### Comparing `gaphas-3.9.1/LICENSE` & `gaphas-3.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gaphas-3.9.1/README.md` & `gaphas-3.9.2/README.md`

 * *Files identical despite different names*

### Comparing `gaphas-3.9.1/gaphas/__init__.py` & `gaphas-3.9.2/gaphas/__init__.py`

 * *Files identical despite different names*

### Comparing `gaphas-3.9.1/gaphas/canvas.py` & `gaphas-3.9.2/gaphas/canvas.py`

 * *Files identical despite different names*

### Comparing `gaphas-3.9.1/gaphas/connections.py` & `gaphas-3.9.2/gaphas/connections.py`

 * *Files identical despite different names*

### Comparing `gaphas-3.9.1/gaphas/connector.py` & `gaphas-3.9.2/gaphas/connector.py`

 * *Files identical despite different names*

### Comparing `gaphas-3.9.1/gaphas/constraint.py` & `gaphas-3.9.2/gaphas/constraint.py`

 * *Files identical despite different names*

### Comparing `gaphas-3.9.1/gaphas/cursor.py` & `gaphas-3.9.2/gaphas/cursor.py`

 * *Files identical despite different names*

### Comparing `gaphas-3.9.1/gaphas/decorators.py` & `gaphas-3.9.2/gaphas/decorators.py`

 * *Files identical despite different names*

### Comparing `gaphas-3.9.1/gaphas/geometry.py` & `gaphas-3.9.2/gaphas/geometry.py`

 * *Files identical despite different names*

### Comparing `gaphas-3.9.1/gaphas/guide.py` & `gaphas-3.9.2/gaphas/guide.py`

 * *Files 0% similar despite different names*

```diff
@@ -232,15 +232,14 @@
     """
 
     view: GtkView
     item: Item
     handle: Handle
 
     def move(self, pos: Pos) -> None:
-
         super().move(pos)  # type: ignore[misc]
 
         item = self.item
         view = self.view
         model = view.model
         assert model
```

### Comparing `gaphas-3.9.1/gaphas/handle.py` & `gaphas-3.9.2/gaphas/handle.py`

 * *Files identical despite different names*

### Comparing `gaphas-3.9.1/gaphas/handlemove.py` & `gaphas-3.9.2/gaphas/handlemove.py`

 * *Files identical despite different names*

### Comparing `gaphas-3.9.1/gaphas/item.py` & `gaphas-3.9.2/gaphas/item.py`

 * *Files identical despite different names*

### Comparing `gaphas-3.9.1/gaphas/matrix.py` & `gaphas-3.9.2/gaphas/matrix.py`

 * *Files identical despite different names*

### Comparing `gaphas-3.9.1/gaphas/model.py` & `gaphas-3.9.2/gaphas/model.py`

 * *Files identical despite different names*

### Comparing `gaphas-3.9.1/gaphas/move.py` & `gaphas-3.9.2/gaphas/move.py`

 * *Files identical despite different names*

### Comparing `gaphas-3.9.1/gaphas/painter/__init__.py` & `gaphas-3.9.2/gaphas/painter/__init__.py`

 * *Files identical despite different names*

### Comparing `gaphas-3.9.1/gaphas/painter/boundingboxpainter.py` & `gaphas-3.9.2/gaphas/painter/boundingboxpainter.py`

 * *Files identical despite different names*

### Comparing `gaphas-3.9.1/gaphas/painter/chain.py` & `gaphas-3.9.2/gaphas/painter/chain.py`

 * *Files identical despite different names*

### Comparing `gaphas-3.9.1/gaphas/painter/freehand.py` & `gaphas-3.9.2/gaphas/painter/freehand.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 from cairo import Context as CairoContext
 
 from gaphas.item import Item
 from gaphas.painter.painter import ItemPainterType
 
 
 class FreeHandCairoContext:
-
     KAPPA = 0.5522847498
 
     def __init__(self, cr, sloppiness=0.5):
         self.cr = cr
         self.sloppiness = sloppiness  # In range 0.0 .. 2.0
 
     def __getattr__(self, key):
```

### Comparing `gaphas-3.9.1/gaphas/painter/handlepainter.py` & `gaphas-3.9.2/gaphas/painter/handlepainter.py`

 * *Files identical despite different names*

### Comparing `gaphas-3.9.1/gaphas/painter/itempainter.py` & `gaphas-3.9.2/gaphas/painter/itempainter.py`

 * *Files identical despite different names*

### Comparing `gaphas-3.9.1/gaphas/painter/painter.py` & `gaphas-3.9.2/gaphas/painter/painter.py`

 * *Files identical despite different names*

### Comparing `gaphas-3.9.1/gaphas/port.py` & `gaphas-3.9.2/gaphas/port.py`

 * *Files identical despite different names*

### Comparing `gaphas-3.9.1/gaphas/position.py` & `gaphas-3.9.2/gaphas/position.py`

 * *Files identical despite different names*

### Comparing `gaphas-3.9.1/gaphas/quadtree.py` & `gaphas-3.9.2/gaphas/quadtree.py`

 * *Files identical despite different names*

### Comparing `gaphas-3.9.1/gaphas/segment.py` & `gaphas-3.9.2/gaphas/segment.py`

 * *Files identical despite different names*

### Comparing `gaphas-3.9.1/gaphas/selection.py` & `gaphas-3.9.2/gaphas/selection.py`

 * *Files identical despite different names*

### Comparing `gaphas-3.9.1/gaphas/solver/constraint.py` & `gaphas-3.9.2/gaphas/solver/constraint.py`

 * *Files identical despite different names*

### Comparing `gaphas-3.9.1/gaphas/solver/solver.py` & `gaphas-3.9.2/gaphas/solver/solver.py`

 * *Files 4% similar despite different names*

```diff
@@ -129,14 +129,19 @@
         if not self._solving:
             if c in self._marked_cons:
                 self._marked_cons.remove(c)
             self._marked_cons.append(c)
         elif self._marked_cons.count(c) < self._resolve_limit:
             self._marked_cons.append(c)
 
+    @property
+    def needs_solving(self) -> bool:
+        """Return if there are constraints that need solving."""
+        return bool(self._marked_cons)
+
     def solve(self) -> None:  # sourcery skip: while-to-for
         """
         Example:
 
         >>> from gaphas.constraint import EquationConstraint
         >>> a, b, c = Variable(1.0), Variable(2.0), Variable(3.0)
         >>> s = Solver()
@@ -160,14 +165,15 @@
         >>> b._value
         -3.0
         >>> a.value = 10
         >>> s.solve()
         >>> c._value
         10.0
         """
+        # NB. marked_cons is updated during the solving process
         marked_cons = self._marked_cons
         notify = self._notify
         try:
             self._solving = True
 
             # Solve each constraint. Using a counter makes it
             # possible to also solve constraints that are marked as
@@ -175,14 +181,16 @@
             # sourcery: skip
             n = 0
             while n < len(marked_cons):
                 c = marked_cons[n]
                 c.solve()
                 notify(c)
                 n += 1
+
+            self._marked_cons = []
         finally:
             self._solving = False
 
 
 def find_containing_constraint(
     constraint: Constraint, constraints: Collection[Constraint]
 ) -> Optional[Constraint]:
```

### Comparing `gaphas-3.9.1/gaphas/solver/variable.py` & `gaphas-3.9.2/gaphas/solver/variable.py`

 * *Files identical despite different names*

### Comparing `gaphas-3.9.1/gaphas/table.py` & `gaphas-3.9.2/gaphas/table.py`

 * *Files identical despite different names*

### Comparing `gaphas-3.9.1/gaphas/tool/__init__.py` & `gaphas-3.9.2/gaphas/tool/__init__.py`

 * *Files identical despite different names*

### Comparing `gaphas-3.9.1/gaphas/tool/itemtool.py` & `gaphas-3.9.2/gaphas/tool/itemtool.py`

 * *Files identical despite different names*

### Comparing `gaphas-3.9.1/gaphas/tool/placement.py` & `gaphas-3.9.2/gaphas/tool/placement.py`

 * *Files identical despite different names*

### Comparing `gaphas-3.9.1/gaphas/tool/rubberband.py` & `gaphas-3.9.2/gaphas/tool/rubberband.py`

 * *Files identical despite different names*

### Comparing `gaphas-3.9.1/gaphas/tool/scroll.py` & `gaphas-3.9.2/gaphas/tool/scroll.py`

 * *Files identical despite different names*

### Comparing `gaphas-3.9.1/gaphas/tool/zoom.py` & `gaphas-3.9.2/gaphas/tool/zoom.py`

 * *Files identical despite different names*

### Comparing `gaphas-3.9.1/gaphas/tree.py` & `gaphas-3.9.2/gaphas/tree.py`

 * *Files identical despite different names*

### Comparing `gaphas-3.9.1/gaphas/types.py` & `gaphas-3.9.2/gaphas/types.py`

 * *Files identical despite different names*

### Comparing `gaphas-3.9.1/gaphas/util.py` & `gaphas-3.9.2/gaphas/util.py`

 * *Files identical despite different names*

### Comparing `gaphas-3.9.1/gaphas/view/gtkview.py` & `gaphas-3.9.2/gaphas/view/gtkview.py`

 * *Files identical despite different names*

### Comparing `gaphas-3.9.1/gaphas/view/scrolling.py` & `gaphas-3.9.2/gaphas/view/scrolling.py`

 * *Files identical despite different names*

### Comparing `gaphas-3.9.1/pyproject.toml` & `gaphas-3.9.2/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gaphas"
-version = "3.9.1"
+version = "3.9.2"
 description="Gaphas is a GTK+ based diagramming widget"
 authors = [
     "Arjan J. Molenaar <gaphor@gmail.com>",
     "Dan Yeaw <dan@yeaw.me>"
 ]
 license = "Apache-2.0"
 
@@ -32,60 +32,19 @@
 sphinx = { version = ">=4.3,<6.0", optional = true }
 sphinx-rtd-theme = { version = "^1.0", optional = true }
 gaphor = { version = "^2.7", python = "^3.9, <3.11", optional = true }
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.2"
 pytest-cov = "^4.0"
-tox = "^4.0"
 pytest-archon = "^0.0.2"
 
 [tool.poetry.extras]
 docs = [ "sphinx", "sphinx-rtd-theme", "gaphor" ]
 
-[tool.tox]
-legacy_tox_ini = """
-[tox]
-isolated_build = true
-envlist = clean, py39, py310, py311, report
-tox_pyenv_fallback = false
-
-[gh-actions]
-python =
-    3.9: py39
-    3.10: py310
-    3.11: py311
-
-[testenv]
-whitelist_externals =
-    xvfb-run
-commands =
-    xvfb-run pytest --cov=gaphas --cov-append --cov-report=term-missing {posargs}
-deps =
-    pytest
-    pytest-cov
-    pytest-archon
-depends =
-    {py39,py310, py311}: clean
-    report: py39,py310,py311
-passenv = TEST_GTK_VERSION
-
-[testenv:report]
-deps = coverage[toml]
-skip_install = true
-commands =
-    coverage report
-    coverage html
-
-[testenv:clean]
-deps = coverage[toml]
-skip_install = true
-commands = coverage erase
-"""
-
 [tool.pytest.ini_options]
 testpaths = ["tests"]
 addopts = ["--import-mode=importlib"]
 
 [tool.isort]
 multi_line_output = 3
 include_trailing_comma = true
```

### Comparing `gaphas-3.9.1/setup.py` & `gaphas-3.9.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 extras_require = \
 {'docs': ['sphinx>=4.3,<6.0', 'sphinx-rtd-theme>=1.0,<2.0'],
  'docs:python_version >= "3.9" and python_version < "3.11"': ['gaphor>=2.7,<3.0']}
 
 setup_kwargs = {
     'name': 'gaphas',
-    'version': '3.9.1',
+    'version': '3.9.2',
     'description': 'Gaphas is a GTK+ based diagramming widget',
     'long_description': '# Gaphas\n[![Build state](https://github.com/gaphor/gaphas/workflows/build/badge.svg)](https://github.com/gaphor/gaphas/actions)\n[![Maintainability](https://api.codeclimate.com/v1/badges/e9837cc647b72119fd11/maintainability)](https://codeclimate.com/github/gaphor/gaphas/maintainability)\n[![Test Coverage](https://api.codeclimate.com/v1/badges/e9837cc647b72119fd11/test_coverage)](https://codeclimate.com/github/gaphor/gaphas/test_coverage)\n![Docs build state](https://readthedocs.org/projects/gaphas/badge/?version=latest)\n[![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)\n[![standard-readme compliant](https://img.shields.io/badge/readme%20style-standard-brightgreen.svg?style=flat)](https://github.com/RichardLitt/standard-readme)\n[![Gitter](https://img.shields.io/gitter/room/nwjs/nw.js.svg)](https://gitter.im/Gaphor/Lobby?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge)\n[![All Contributors](https://img.shields.io/badge/all_contributors-9-orange.svg?style=flat-square)](#contributors)\n\n> Gaphas is the diagramming widget library for Python.\n\n![Gaphas Demo](https://raw.githubusercontent.com/gaphor/gaphas/main/docs/images/gaphas-demo.gif)\n\nGaphas is a library that provides the user interface component (widget) for drawing diagrams. Diagrams can be drawn to screen and then easily exported to a variety of formats, including SVG and PDF. Want to build an app with chart-like diagrams? Then Gaphas is for you! Use this library to build a tree, network, flowchart, or other diagrams.\n\nThis library is currently being used by [Gaphor](https://github.com/gaphor/gaphor) for UML drawing,\n[RAFCON](https://github.com/DLR-RM/RAFCON) for state-machine based robot control, and [ASCEND](http://ascend4.org/) for solving mathematical models.\n\n## 📑 Table of Contents\n\n- [Background](#background)\n- [Install](#install)\n- [Usage](#usage)\n- [Contributing](#contributing)\n- [License](#license)\n\n## 📜 Background\n\nGaphas was built to provide the foundational diagramming portions of [Gaphor](https://github.com/gaphor/gaphor). Since Gaphor is built on GTK and Cairo, [PyGObject](https://pygobject.readthedocs.io/) provides access to the GUI toolkit and [PyCairo](https://pycairo.readthedocs.io/) to the 2D graphics library. However, there wasn\'t a project that abstracted these technologies to easily create a diagramming tool. Hence, Gaphas was created as a library to allow others to create a diagramming tool using GTK and Cairo.\n\nHere is how it works:\n\n- Items (Canvas items) can be added to a Canvas.\n- The Canvas maintains the tree structure (parent-child relationships between items).\n- A constraint solver is used to maintain item constraints and inter-item constraints.\n- The item (and user) should not be bothered with things like bounding-box calculations.\n- Very modular--e.g., handle support could be swapped in and swapped out.\n- Rendering using Cairo.\n\nThe main portions of the library include:\n\n- canvas - The main canvas class (container for Items).\n- items - Objects placed on a Canvas.\n- solver - A constraint solver to define the layout and connection of items.\n- gtkview - A view to be used in GTK applications that interacts with users with tools.\n- painters - The workers used to paint items.\n- tools - Tools are used to handle user events (such as mouse movement and button presses).\n- aspects - Provides an intermediate step between tools and items.\n\nGaphas contains default implementations for `Canvas` and `Item`s. There are protocols in place\nto allow you to make your own canvas.\n\n## 💾 Install\n\nTo install Gaphas, simply use pip:\n\n```bash\n$ pip install gaphas\n```\n\nUse of a\n[virtual environment](https://virtualenv.pypa.io/en/latest/) is highly recommended.\n\n### Development\n\nTo setup a development environment with Linux:\n\n```bash\n$ sudo apt-get install -y python3-dev python3-gi python3-gi-cairo\n    gir1.2-gtk-3.0 libgirepository1.0-dev libcairo2-dev\n$ pip install poetry\n$ poetry install\n```\n\n## 🔦 Usage\n\nAPI docs and tutorials can be found on [Read the Docs](https://gaphas.readthedocs.io).\n\n## ♥ Contributing\n\nThanks goes to these wonderful people ([emoji key](https://github.com/kentcdodds/all-contributors#emoji-key)):\n\n<!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->\n<!-- prettier-ignore -->\n<table><tr><td align="center"><a href="https://github.com/amolenaar"><img src="https://avatars0.githubusercontent.com/u/96249?v=4" width="100px;" alt="Arjan Molenaar"/><br /><sub><b>Arjan Molenaar</b></sub></a><br /><a href="https://github.com/gaphor/gaphas/commits?author=amolenaar" title="Code">💻</a> <a href="https://github.com/gaphor/gaphas/issues?q=author%3Aamolenaar" title="Bug reports">🐛</a> <a href="https://github.com/gaphor/gaphas/commits?author=amolenaar" title="Documentation">📖</a> <a href="#review-amolenaar" title="Reviewed Pull Requests">👀</a> <a href="#question-amolenaar" title="Answering Questions">💬</a> <a href="#plugin-amolenaar" title="Plugin/utility libraries">🔌</a></td><td align="center"><a href="https://ghuser.io/danyeaw"><img src="https://avatars1.githubusercontent.com/u/10014976?v=4" width="100px;" alt="Dan Yeaw"/><br /><sub><b>Dan Yeaw</b></sub></a><br /><a href="https://github.com/gaphor/gaphas/commits?author=danyeaw" title="Code">💻</a> <a href="https://github.com/gaphor/gaphas/commits?author=danyeaw" title="Tests">⚠️</a> <a href="#review-danyeaw" title="Reviewed Pull Requests">👀</a> <a href="https://github.com/gaphor/gaphas/issues?q=author%3Adanyeaw" title="Bug reports">🐛</a> <a href="#question-danyeaw" title="Answering Questions">💬</a> <a href="#infra-danyeaw" title="Infrastructure (Hosting, Build-Tools, etc)">🚇</a> <a href="https://github.com/gaphor/gaphas/commits?author=danyeaw" title="Documentation">📖</a></td><td align="center"><a href="https://github.com/wrobell"><img src="https://avatars2.githubusercontent.com/u/105664?v=4" width="100px;" alt="wrobell"/><br /><sub><b>wrobell</b></sub></a><br /><a href="https://github.com/gaphor/gaphas/commits?author=wrobell" title="Code">💻</a> <a href="https://github.com/gaphor/gaphas/commits?author=wrobell" title="Tests">⚠️</a> <a href="#review-wrobell" title="Reviewed Pull Requests">👀</a></td><td align="center"><a href="https://github.com/jlstevens"><img src="https://avatars3.githubusercontent.com/u/890576?v=4" width="100px;" alt="Jean-Luc Stevens"/><br /><sub><b>Jean-Luc Stevens</b></sub></a><br /><a href="https://github.com/gaphor/gaphas/commits?author=jlstevens" title="Code">💻</a> <a href="https://github.com/gaphor/gaphas/issues?q=author%3Ajlstevens" title="Bug reports">🐛</a> <a href="https://github.com/gaphor/gaphas/commits?author=jlstevens" title="Documentation">📖</a></td><td align="center"><a href="http://www.franework.de"><img src="https://avatars1.githubusercontent.com/u/1144966?v=4" width="100px;" alt="Franz Steinmetz"/><br /><sub><b>Franz Steinmetz</b></sub></a><br /><a href="https://github.com/gaphor/gaphas/commits?author=franzlst" title="Code">💻</a> <a href="https://github.com/gaphor/gaphas/issues?q=author%3Afranzlst" title="Bug reports">🐛</a></td><td align="center"><a href="https://github.com/adrianboguszewski"><img src="https://avatars3.githubusercontent.com/u/4547501?v=4" width="100px;" alt="Adrian Boguszewski"/><br /><sub><b>Adrian Boguszewski</b></sub></a><br /><a href="https://github.com/gaphor/gaphas/commits?author=adrianboguszewski" title="Code">💻</a></td><td align="center"><a href="https://github.com/Rbelder"><img src="https://avatars3.githubusercontent.com/u/15119522?v=4" width="100px;" alt="Rico Belder"/><br /><sub><b>Rico Belder</b></sub></a><br /><a href="https://github.com/gaphor/gaphas/issues?q=author%3ARbelder" title="Bug reports">🐛</a> <a href="#review-Rbelder" title="Reviewed Pull Requests">👀</a></td></tr><tr><td align="center"><a href="http://www.boduch.ca"><img src="https://avatars2.githubusercontent.com/u/114619?v=4" width="100px;" alt="Adam Boduch"/><br /><sub><b>Adam Boduch</b></sub></a><br /><a href="https://github.com/gaphor/gaphas/issues?q=author%3Aadamboduch" title="Bug reports">🐛</a></td><td align="center"><a href="https://github.com/janettech"><img src="https://avatars3.githubusercontent.com/u/13398384?v=4" width="100px;" alt="Janet Jose"/><br /><sub><b>Janet Jose</b></sub></a><br /><a href="https://github.com/gaphor/gaphas/commits?author=janettech" title="Documentation">📖</a></td></tr></table>\n\n<!-- ALL-CONTRIBUTORS-LIST:END -->\n\nThis project follows the [all-contributors](https://github.com/kentcdodds/all-contributors) specification. Contributions of any kind are welcome!\n\n1. Check for open issues or open a fresh issue to start a discussion around a feature idea or a bug.\n    There is a [first-timers-only](https://github.com/gaphor/gaphas/issues?utf8=%E2%9C%93&q=is%3Aissue+is%3Aopen+label%3Afirst-timers-only) tag for issues that should be ideal for people who are not very familiar with the codebase yet.\n2. Fork [the repository](https://github.com/gaphor/gaphas) on GitHub to    start making your changes to the **main**       branch (or branch off of it).\n3. Write a test which shows that the bug was fixed or that the feature\n   works as expected.\n4. Send a pull request and bug the maintainers until it gets merged and\n   published. :smile:\n\nSee [the contributing file](CONTRIBUTING.md)!\n\n## © License\n\nCopyright © Arjan Molenaar and Dan Yeaw\n\nLicensed under the [Apache License 2.0](LICENSE).\n\nSummary: You can do what you like with Gaphas, as long as you include the required notices. This permissive license contains a patent license from the contributors of the code.\n',
     'author': 'Arjan J. Molenaar',
     'author_email': 'gaphor@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://gaphas.readthedocs.io/',
```

### Comparing `gaphas-3.9.1/PKG-INFO` & `gaphas-3.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gaphas
-Version: 3.9.1
+Version: 3.9.2
 Summary: Gaphas is a GTK+ based diagramming widget
 Home-page: https://gaphas.readthedocs.io/
 License: Apache-2.0
 Keywords: gtk,diagram,gaphas
 Author: Arjan J. Molenaar
 Author-email: gaphor@gmail.com
 Requires-Python: >=3.9,<4.0
```

