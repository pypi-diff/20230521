# Comparing `tmp/FreeTVG-karjakak-3.2.4.tar.gz` & `tmp/FreeTVG-karjakak-3.2.4rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FreeTVG-karjakak-3.2.4.tar", last modified: Sat May 20 18:14:31 2023, max compression
+gzip compressed data, was "FreeTVG-karjakak-3.2.4rc1.tar", last modified: Wed May 17 13:02:46 2023, max compression
```

## Comparing `FreeTVG-karjakak-3.2.4.tar` & `FreeTVG-karjakak-3.2.4rc1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-05-20 18:14:31.725280 FreeTVG-karjakak-3.2.4/
-drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-05-20 18:14:31.720464 FreeTVG-karjakak-3.2.4/FreeTVG_karjakak.egg-info/
--rw-r--r--   0 karja      (501) staff       (20)     1448 2023-05-20 18:14:31.000000 FreeTVG-karjakak-3.2.4/FreeTVG_karjakak.egg-info/PKG-INFO
--rw-r--r--   0 karja      (501) staff       (20)      463 2023-05-20 18:14:31.000000 FreeTVG-karjakak-3.2.4/FreeTVG_karjakak.egg-info/SOURCES.txt
--rw-r--r--   0 karja      (501) staff       (20)        1 2023-05-20 18:14:31.000000 FreeTVG-karjakak-3.2.4/FreeTVG_karjakak.egg-info/dependency_links.txt
--rw-r--r--   0 karja      (501) staff       (20)       29 2023-05-20 18:14:31.000000 FreeTVG-karjakak-3.2.4/FreeTVG_karjakak.egg-info/entry_points.txt
--rw-r--r--   0 karja      (501) staff       (20)      151 2023-05-20 18:14:31.000000 FreeTVG-karjakak-3.2.4/FreeTVG_karjakak.egg-info/requires.txt
--rw-r--r--   0 karja      (501) staff       (20)        4 2023-05-20 18:14:31.000000 FreeTVG-karjakak-3.2.4/FreeTVG_karjakak.egg-info/top_level.txt
--rw-r--r--   0 karja      (501) staff       (20)     1082 2021-04-02 20:37:42.000000 FreeTVG-karjakak-3.2.4/LICENSE.txt
--rw-r--r--   0 karja      (501) staff       (20)     1448 2023-05-20 18:14:31.725400 FreeTVG-karjakak-3.2.4/PKG-INFO
--rw-r--r--   0 karja      (501) staff       (20)      821 2022-12-10 03:07:59.000000 FreeTVG-karjakak-3.2.4/README.md
-drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-05-20 18:14:31.723319 FreeTVG-karjakak-3.2.4/TVG/
--rw-r--r--   0 karja      (501) staff       (20)   146133 2023-05-20 17:27:17.000000 FreeTVG-karjakak-3.2.4/TVG/FreeTVG.py
--rw-r--r--   0 karja      (501) staff       (20)   360883 2023-05-17 06:38:49.000000 FreeTVG-karjakak-3.2.4/TVG/Tutorial TVG.pdf
--rw-r--r--   0 karja      (501) staff       (20)       46 2022-11-22 15:46:43.000000 FreeTVG-karjakak-3.2.4/TVG/__init__.py
-drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-05-20 18:14:31.723974 FreeTVG-karjakak-3.2.4/TVG/structure/
--rw-r--r--   0 karja      (501) staff       (20)       82 2023-05-14 08:59:37.000000 FreeTVG-karjakak-3.2.4/TVG/structure/__init__.py
--rw-r--r--   0 karja      (501) staff       (20)    14894 2023-05-16 16:03:03.000000 FreeTVG-karjakak-3.2.4/TVG/structure/frame_layouts.py
-drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-05-20 18:14:31.725134 FreeTVG-karjakak-3.2.4/TVG/utility/
--rw-r--r--   0 karja      (501) staff       (20)      923 2023-05-16 14:56:03.000000 FreeTVG-karjakak-3.2.4/TVG/utility/RegMail.py
--rw-r--r--   0 karja      (501) staff       (20)       84 2023-05-15 12:31:08.000000 FreeTVG-karjakak-3.2.4/TVG/utility/__init__.py
--rw-r--r--   0 karja      (501) staff       (20)     6357 2023-05-20 18:13:14.000000 FreeTVG-karjakak-3.2.4/TVG/utility/mdh.py
--rw-r--r--   0 karja      (501) staff       (20)      103 2021-11-12 16:03:29.000000 FreeTVG-karjakak-3.2.4/pyproject.toml
--rw-r--r--   0 karja      (501) staff       (20)      976 2023-05-20 18:14:31.725802 FreeTVG-karjakak-3.2.4/setup.cfg
+drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-05-17 13:02:46.908078 FreeTVG-karjakak-3.2.4rc1/
+drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-05-17 13:02:46.903821 FreeTVG-karjakak-3.2.4rc1/FreeTVG_karjakak.egg-info/
+-rw-r--r--   0 karja      (501) staff       (20)     1451 2023-05-17 13:02:46.000000 FreeTVG-karjakak-3.2.4rc1/FreeTVG_karjakak.egg-info/PKG-INFO
+-rw-r--r--   0 karja      (501) staff       (20)      463 2023-05-17 13:02:46.000000 FreeTVG-karjakak-3.2.4rc1/FreeTVG_karjakak.egg-info/SOURCES.txt
+-rw-r--r--   0 karja      (501) staff       (20)        1 2023-05-17 13:02:46.000000 FreeTVG-karjakak-3.2.4rc1/FreeTVG_karjakak.egg-info/dependency_links.txt
+-rw-r--r--   0 karja      (501) staff       (20)       29 2023-05-17 13:02:46.000000 FreeTVG-karjakak-3.2.4rc1/FreeTVG_karjakak.egg-info/entry_points.txt
+-rw-r--r--   0 karja      (501) staff       (20)      136 2023-05-17 13:02:46.000000 FreeTVG-karjakak-3.2.4rc1/FreeTVG_karjakak.egg-info/requires.txt
+-rw-r--r--   0 karja      (501) staff       (20)        4 2023-05-17 13:02:46.000000 FreeTVG-karjakak-3.2.4rc1/FreeTVG_karjakak.egg-info/top_level.txt
+-rw-r--r--   0 karja      (501) staff       (20)     1082 2021-04-02 20:37:42.000000 FreeTVG-karjakak-3.2.4rc1/LICENSE.txt
+-rw-r--r--   0 karja      (501) staff       (20)     1451 2023-05-17 13:02:46.908167 FreeTVG-karjakak-3.2.4rc1/PKG-INFO
+-rw-r--r--   0 karja      (501) staff       (20)      821 2022-12-10 03:07:59.000000 FreeTVG-karjakak-3.2.4rc1/README.md
+drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-05-17 13:02:46.906424 FreeTVG-karjakak-3.2.4rc1/TVG/
+-rw-r--r--   0 karja      (501) staff       (20)   146705 2023-05-17 04:29:32.000000 FreeTVG-karjakak-3.2.4rc1/TVG/FreeTVG.py
+-rw-r--r--   0 karja      (501) staff       (20)   360883 2023-05-17 06:38:49.000000 FreeTVG-karjakak-3.2.4rc1/TVG/Tutorial TVG.pdf
+-rw-r--r--   0 karja      (501) staff       (20)       46 2022-11-22 15:46:43.000000 FreeTVG-karjakak-3.2.4rc1/TVG/__init__.py
+drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-05-17 13:02:46.906986 FreeTVG-karjakak-3.2.4rc1/TVG/structure/
+-rw-r--r--   0 karja      (501) staff       (20)       82 2023-05-14 08:59:37.000000 FreeTVG-karjakak-3.2.4rc1/TVG/structure/__init__.py
+-rw-r--r--   0 karja      (501) staff       (20)    14894 2023-05-16 16:03:03.000000 FreeTVG-karjakak-3.2.4rc1/TVG/structure/frame_layouts.py
+drwxr-xr-x   0 karja      (501) staff       (20)        0 2023-05-17 13:02:46.907804 FreeTVG-karjakak-3.2.4rc1/TVG/utility/
+-rw-r--r--   0 karja      (501) staff       (20)      923 2023-05-16 14:56:03.000000 FreeTVG-karjakak-3.2.4rc1/TVG/utility/RegMail.py
+-rw-r--r--   0 karja      (501) staff       (20)       84 2023-05-15 12:31:08.000000 FreeTVG-karjakak-3.2.4rc1/TVG/utility/__init__.py
+-rw-r--r--   0 karja      (501) staff       (20)     5786 2023-05-17 12:57:53.000000 FreeTVG-karjakak-3.2.4rc1/TVG/utility/mdh.py
+-rw-r--r--   0 karja      (501) staff       (20)      103 2021-11-12 16:03:29.000000 FreeTVG-karjakak-3.2.4rc1/pyproject.toml
+-rw-r--r--   0 karja      (501) staff       (20)      963 2023-05-17 13:02:46.908459 FreeTVG-karjakak-3.2.4rc1/setup.cfg
```

### Comparing `FreeTVG-karjakak-3.2.4/FreeTVG_karjakak.egg-info/PKG-INFO` & `FreeTVG-karjakak-3.2.4rc1/FreeTVG_karjakak.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FreeTVG-karjakak
-Version: 3.2.4
+Version: 3.2.4rc1
 Summary: Tree View Gui for outline treeview note.
 Home-page: https://github.com/kakkarja/FreeTVG#latest-notice
 Author: karjakak
 Author-email: kakkarja.github@gmail.com
 License: MIT License
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: MacOS X
```

### Comparing `FreeTVG-karjakak-3.2.4/LICENSE.txt` & `FreeTVG-karjakak-3.2.4rc1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `FreeTVG-karjakak-3.2.4/PKG-INFO` & `FreeTVG-karjakak-3.2.4rc1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FreeTVG-karjakak
-Version: 3.2.4
+Version: 3.2.4rc1
 Summary: Tree View Gui for outline treeview note.
 Home-page: https://github.com/kakkarja/FreeTVG#latest-notice
 Author: karjakak
 Author-email: kakkarja.github@gmail.com
 License: MIT License
 Classifier: Environment :: Win32 (MS Windows)
 Classifier: Environment :: MacOS X
```

### Comparing `FreeTVG-karjakak-3.2.4/README.md` & `FreeTVG-karjakak-3.2.4rc1/README.md`

 * *Files identical despite different names*

### Comparing `FreeTVG-karjakak-3.2.4/TVG/FreeTVG.py` & `FreeTVG-karjakak-3.2.4rc1/TVG/FreeTVG.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,17 +52,18 @@
 
 from excptr import DEFAULTDIR, DEFAULTFILE, DIRPATH, excp, excpcls
 
 from .structure import Lay1, Lay2, Lay3, Lay4, Lay5, Lay6, Lay7, Lay8, Scribe
 from .utility.mdh import convhtml
 from .utility.RegMail import composemail, wrwords
 
-if platform.startswith("win"):
+try:
     from ctypes import windll, byref, sizeof, c_int
-
+except:
+    pass
 
 __all__ = ["main"]
 
 
 DEFAULTDIR = os.path.join(DIRPATH, "FreeTVG_TRACE")
 if not os.path.exists(DEFAULTDIR):
     os.mkdir(DEFAULTDIR)
@@ -1722,34 +1723,21 @@
             if "}" in self.text["font"]:
                 fon = self.text["font"].partition("}")[0].replace("{", "")
                 fon = f"{add}{fon}"
             else:
                 fon = self.text["font"].partition(" ")[0]
                 fon = f"{add}{fon}"
 
-            ans = messagebox.askyesno(
-                "Preview", "Do you want to preview? ('no' will go to web for printing)"
+            convhtml(
+                self._utilspdf(),
+                self.filename,
+                fon,
+                self.text.cget("background")[1:],
+                self.text.cget("foreground"),
             )
-            if ans:
-                style = convhtml(
-                    self._utilspdf(),
-                    self.filename,
-                    fon,
-                    self.text.cget("background")[1:],
-                    self.text.cget("foreground"),
-                )
-            else:
-                style = convhtml(
-                    self._utilspdf(),
-                    self.filename,
-                    fon,
-                    self.text.cget("background")[1:],
-                    self.text.cget("foreground"),
-                    preview=False,
-                )
             del px, ck, sty, add, fon
 
     def spaces(self):
         """Mostly used by other functions to clear an obselete spaces.
         To appropriate the display better.
         """
 
@@ -2691,19 +2679,27 @@
                         self.disab(dis=False)
                         self.spaces()
                         if self.editorsel:
                             self.editorsel = None
                 except Exception as a:
                     messagebox.showerror("TreeViewGui", f"{a}", parent=self.root)
                 if self.text.cget("state") == DISABLED:
+                    self.chktempo()
                     self._mdbuttons()
             self.store = None
             self.text.edit_reset()
             self.infobar()
 
+    def chktempo(self):
+        """Checking Add-On expression attribute"""
+
+        if self._addon and hasattr(self, "toptempo"):
+            self.toptempo.destroy()
+            self.__delattr__("toptempo")
+
     def tvgexit(self, event=None):
         """Exit mode for TVG and setting everything back to default"""
 
         if self.FREEZE is False:
             if self.checkfile():
                 with open(os.path.join(self.glop.parent, "lastopen.tvg"), "wb") as lop:
                     lop.write(str({"lop": self.filename}).encode())
@@ -3038,45 +3034,55 @@
                     messagebox.showwarning(
                         "TreeViewGui",
                         "Please unfolding first!",
                         parent=self.root,
                     )
                 self.spaces()
 
+    def _ckwrds(self, wrd: str):
+        if self._addon:
+            nums = len(wrd)
+            if nums >= 101:
+                raise Exception(f"{nums} charcters, is exceeding than 100 chars!")
+
+            for i in wrd:
+                if i not in tuple("0123456789*/-+()%."):
+                    raise ValueError(f"{i!r} is not acceptable expression!")
+
+            ck = re.compile(r"[\W+]{2}")
+            if ck := ck.search(wrd):
+                raise ValueError(f"These {ck.group()!r} are not allowed!")
+            del ck, nums
+
     def exprsum(self, event=None):
         """Expression Calculation for Editor mode"""
 
         if self.lock is False and self.text.cget("state") == NORMAL:
             self.lock = True
             self.FREEZE = True
 
             err = None
-            stor_tuple = tuple()
 
             @excp(2, DEFAULTFILE)
             def calc(event=None):
-                nonlocal err, stor_tuple
+                nonlocal err
                 try:
                     if gw := wid.get():
-                        if not stor_tuple or gw != stor_tuple[0]:
-                            lab["text"] = _ckwrds(gw)
-                            if err:
-                                err = None
-                            stor_tuple = gw, lab["text"]
-                        else:
-                            lab["text"] = stor_tuple[1]
-                        del gw
+                        self._ckwrds(gw)
+                        ms = EvalExp(gw, None)
+                        lab["text"] = ms.evlex()
+                        if err:
+                            err = None
+                        del ms, gw
                     else:
                         raise ValueError("Expression is empty!")
                 except Exception as e:
                     if err is None:
                         err = 1
                     messagebox.showerror("Error Message", e)
-                    lab.focus()
-                    wid.focus()
 
             @excp(2, DEFAULTFILE)
             def utilins(lab: str):
                 gtx = (
                     self.text.get(
                         f"{self.text.index(INSERT)} linestart",
                         f"{self.text.index(INSERT)} lineend",
@@ -3115,18 +3121,41 @@
                         else:
                             self.text.insert(
                                 self.text.index(f"{self.text.index(INSERT)} lineend"),
                                 f" {lab}",
                             )
 
             @excp(2, DEFAULTFILE)
+            def updatelab():
+                try:
+                    ms = None
+                    if gw := wid.get():
+                        self._ckwrds(gw)
+                        ms = EvalExp(gw, None)
+                    if lab["text"] != (ms := ms.evlex()):
+                        lab["text"] = ms
+                except:
+                    calc()
+                finally:
+                    del ms, gw
+
+            @excp(2, DEFAULTFILE)
             def insert():
                 if isinstance(lab["text"], int | float):
-                    calc()
-                    self.labcop = f"{lab['text']:,.2f}"
+                    updatelab()
+                    match self.labcop:
+                        case lc if lc is None:
+                            self.labcop = f"{lab['text']:,.2f}"
+                        case lc if self.text.get(
+                            f"{INSERT} - {len(lc)}c", INSERT
+                        ) == lc:
+                            self.text.delete(f"{INSERT} - {len(lc)}c", INSERT)
+                            self.labcop = f"{lab['text']:,.2f}"
+                        case _:
+                            self.labcop = f"{lab['text']:,.2f}"
                     utilins(self.labcop)
                     lab["text"] = "click for result"
 
                 elif bool(wid.get()):
                     nonlocal err
 
                     calc()
@@ -3172,26 +3201,33 @@
                 def fcs(self):
                     if self.grab_status() is not None:
                         self.grab_release()
                         self.attributes("-topmost", 1)
                     else:
                         self.after(1000, self.fcs)
 
+            mas = Toplevel(self.root)
+            mas.withdraw()
+            self.__setattr__("toptempo", mas)
             self.__setattr__("labcop", None)
-            d = MyDialog(self.root)
+            d = MyDialog(mas)
             self.lock = False
             self.root.update()
             self.unlock = True
             self.FREEZE = True
+            if hasattr(self, "toptempo"):
+                mas.destroy()
+                self.__delattr__("toptempo")
             self.__delattr__("labcop")
-            del wid, lab, d, err, stor_entry
+            del wid, lab, d, mas, err
         else:
-            messagebox.showinfo(
-                "TreeViewGui", "Only work for Editor mode", parent=self.root
-            )
+            if self.lock is False and not hasattr(self, "toptempo"):
+                messagebox.showinfo(
+                    "TreeViewGui", "Only work for Editor mode", parent=self.root
+                )
 
     def _indconv(self, n: int):
         return f"{float(n)}", f"{float(n + 1)}"
 
     def _ckfoldtvg(self):
         pth = self.glop.absolute().joinpath("fold.tvg")
         if os.path.exists(pth):
@@ -3390,39 +3426,14 @@
                         messagebox.showinfo(
                             "TreeViewGui", "Configuring aborted!", parent=self.root
                         )
 
             TreeViewGui.FREEZE = False
 
 
-def _ckwrds(wrd: str):
-    if _addon:
-        try:
-            nums = len(wrd)
-            values = tuple("0123456789*/-+()%.")
-            ck = None
-
-            if nums >= 101:
-                raise ValueError(f"{nums} charcters, is exceeding than 100 chars!")
-
-            for i in wrd:
-                if i not in values:
-                    raise ValueError(f"{i!r} is not acceptable expression!")
-
-            ck = EvalExp(wrd, None)
-            ck = ck.evlex()
-            return ck
-        except ValueError:
-            raise
-        except:
-            raise ValueError(f"These expression {wrd!r} are not allowed!")
-        finally:
-            del wrd, ck, nums, values
-
-
 @excp(m=2, filenm=DEFAULTFILE)
 def askfile(root):
     """Asking file for creating or opening initial app start"""
 
     files = [
         file.rpartition("_")[0] for file in os.listdir(os.getcwd()) if "_tvg" in file
     ]
```

### Comparing `FreeTVG-karjakak-3.2.4/TVG/Tutorial TVG.pdf` & `FreeTVG-karjakak-3.2.4rc1/TVG/Tutorial TVG.pdf`

 * *Files identical despite different names*

### Comparing `FreeTVG-karjakak-3.2.4/TVG/structure/frame_layouts.py` & `FreeTVG-karjakak-3.2.4rc1/TVG/structure/frame_layouts.py`

 * *Files identical despite different names*

### Comparing `FreeTVG-karjakak-3.2.4/TVG/utility/RegMail.py` & `FreeTVG-karjakak-3.2.4rc1/TVG/utility/RegMail.py`

 * *Files identical despite different names*

### Comparing `FreeTVG-karjakak-3.2.4/TVG/utility/mdh.py` & `FreeTVG-karjakak-3.2.4rc1/TVG/utility/mdh.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 import re
 import subprocess
 from pathlib import Path
 from sys import platform
 
 import markdown
-import webview
 
 __all__ = [""]
 
 
 extensions = [
     "pymdownx.extra",
     "pymdownx.caret",
@@ -28,33 +27,23 @@
     "pymdownx.keys": {"strict": True},
     "pymdownx.tasklist": {
         "clickable_checkbox": True,
     },
 }
 
 
-def convhtml(
-    text: str,
-    filename: str,
-    font: str,
-    bg: str = None,
-    fg: str = None,
-    preview: bool = True,
-):
+def convhtml(text: str, filename: str, font: str, bg: str = None, fg: str = None):
     # Converting your TVG to html and printable directly from browser.
 
     try:
         gettext = text.split("\n")
         tohtml = []
         background = bg if bg else "gold"
         foreground = fg if fg else "black"
         kbfg = "333" if foreground == "black" else "eee"
-        startupinfo = None
-        window = None
-        pointer_event = None
 
         for i in gettext:
             if i != "\n":
                 sp = re.match(r"\s+", i)
                 if sp:
                     sp = sp.span()[1] - 4
                     txt = re.search(r"-", i)
@@ -104,34 +93,30 @@
     vertical-align: middle;
 }
 
 .strikethrough:checked + span {
     text-decoration: line-through;
 }
 """
-        if preview:
-            pointer_event = """body { pointer-events: none; }"""
 
         cssstyle = f"""<!DOCTYPE html>
 <html>
-<button class="button" onclick="javascript:window.print();">Print</button>
+<button class="button"  onclick="javascript:window.print();">Print</button>
 <header>
 <meta charset="UTF-8">
 <h1>
 <strong>
 {filename}
 </strong>
 </h1>
 </header>
 <style>
 {setfont}
 {kbd}
 {tasklist}
-{pointer_event if preview else ""}
-
 """
         printed = """@media print {
 .button { display: none; }
 
 body { 
     background-color: white !important;
     color: black !important;
@@ -199,23 +184,16 @@
                 "msedge",
                 f"'\"{Path(f'{filename}.html').absolute()}\"'",
             ]
             startupinfo = subprocess.STARTUPINFO()
             startupinfo.dwFlags |= subprocess.STARTF_USESHOWWINDOW
             subprocess.run(pro, startupinfo=startupinfo)
         else:
-            if preview:
-                window = webview.create_window("TVG", html=cssstyle)
-                webview.start()
-            else:
-                pro = ["open", "-a", "Safari", f"{Path(f'{filename}.html').absolute()}"]
-                subprocess.run(pro)
-    except Exception as e:
-        raise e
-    finally:
+            pro = ["open", "-a", "Safari", f"{Path(f'{filename}.html').absolute()}"]
+            subprocess.run(pro)
         del (
             text,
             filename,
             font,
             bg,
             fg,
             gettext,
@@ -225,13 +203,10 @@
             kbfg,
             chg,
             setfont,
             cssstyle,
             printed,
             nxt,
             pro,
-            startupinfo,
-            pointer_event,
-            window,
-            preview,
-            pointer_event,
         )
+    except Exception as e:
+        raise e
```

### Comparing `FreeTVG-karjakak-3.2.4/setup.cfg` & `FreeTVG-karjakak-3.2.4rc1/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = FreeTVG-karjakak
-version = 3.2.4
+version = 3.2.4rc1
 author = karjakak
 author_email = kakkarja.github@gmail.com
 description = Tree View Gui for outline treeview note.
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/kakkarja/FreeTVG#latest-notice
 license = MIT License
@@ -25,15 +25,14 @@
 	markdown>=3.3.4
 	pymdown-extensions>=9.0
 	treeview-karjakak>=1.8.1
 	excptr-karjakak>=0.1.0
 	demoji>=1.1.0
 	tomlkit>=0.11.6
 	darkdetect>=0.8.0
-	pywebview>=4.1
 
 [options.package_data]
 * = *.pdf
 
 [options.entry_points]
 gui_scripts = 
 	TVG = TVG:main
```

