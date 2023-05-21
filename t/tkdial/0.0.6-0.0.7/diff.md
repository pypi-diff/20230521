# Comparing `tmp/tkdial-0.0.6.tar.gz` & `tmp/tkdial-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkdial-0.0.6.tar", last modified: Wed Apr 19 12:03:37 2023, max compression
+gzip compressed data, was "tkdial-0.0.7.tar", last modified: Sun May 21 12:31:12 2023, max compression
```

## Comparing `tkdial-0.0.6.tar` & `tkdial-0.0.7.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 12:03:37.618637 tkdial-0.0.6/
--rw-rw-rw-   0        0        0     7048 2022-11-20 16:16:56.000000 tkdial-0.0.6/LICENSE
--rw-rw-rw-   0        0        0    19517 2023-04-19 12:03:37.619217 tkdial-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0    18917 2023-04-19 12:00:40.000000 tkdial-0.0.6/README.md
--rw-rw-rw-   0        0        0      598 2023-04-19 12:03:37.620216 tkdial-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1179 2023-04-19 12:03:15.000000 tkdial-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-19 12:03:37.590552 tkdial-0.0.6/tkdial/
--rw-rw-rw-   0        0        0      415 2023-04-19 08:59:42.000000 tkdial-0.0.6/tkdial/__init__.py
--rw-rw-rw-   0        0        0     9266 2023-04-19 11:57:14.000000 tkdial-0.0.6/tkdial/imageknob.py
--rw-rw-rw-   0        0        0    15120 2023-04-18 10:20:00.000000 tkdial-0.0.6/tkdial/jogwheel.py
--rw-rw-rw-   0        0        0    14988 2023-04-18 09:34:10.000000 tkdial-0.0.6/tkdial/meter.py
--rw-rw-rw-   0        0        0     9627 2023-04-18 09:33:53.000000 tkdial-0.0.6/tkdial/scrollknob.py
--rw-rw-rw-   0        0        0    17769 2023-04-18 09:34:03.000000 tkdial-0.0.6/tkdial/tkdial.py
-drwxrwxrwx   0        0        0        0 2023-04-19 12:03:37.616793 tkdial-0.0.6/tkdial.egg-info/
--rw-rw-rw-   0        0        0    19517 2023-04-19 12:03:37.000000 tkdial-0.0.6/tkdial.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      297 2023-04-19 12:03:37.000000 tkdial-0.0.6/tkdial.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       66 2023-04-19 12:03:37.000000 tkdial-0.0.6/tkdial.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-04-19 12:03:37.000000 tkdial-0.0.6/tkdial.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-19 12:03:37.000000 tkdial-0.0.6/tkdial.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-21 12:31:12.238883 tkdial-0.0.7/
+-rw-rw-rw-   0        0        0     7048 2022-11-20 16:16:56.000000 tkdial-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0    19529 2023-05-21 12:31:12.238883 tkdial-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0    18925 2023-05-21 12:28:41.000000 tkdial-0.0.7/README.md
+-rw-rw-rw-   0        0        0      600 2023-05-21 12:31:12.254509 tkdial-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1181 2023-05-21 12:30:34.000000 tkdial-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-21 12:31:12.228350 tkdial-0.0.7/tkdial/
+-rw-rw-rw-   0        0        0      415 2023-05-21 12:25:09.000000 tkdial-0.0.7/tkdial/__init__.py
+-rw-rw-rw-   0        0        0     9277 2023-05-21 12:22:49.000000 tkdial-0.0.7/tkdial/imageknob.py
+-rw-rw-rw-   0        0        0    15131 2023-05-21 12:22:36.000000 tkdial-0.0.7/tkdial/jogwheel.py
+-rw-rw-rw-   0        0        0    14999 2023-05-21 12:21:49.000000 tkdial-0.0.7/tkdial/meter.py
+-rw-rw-rw-   0        0        0     9638 2023-05-21 12:22:22.000000 tkdial-0.0.7/tkdial/scrollknob.py
+-rw-rw-rw-   0        0        0    17780 2023-05-21 12:22:14.000000 tkdial-0.0.7/tkdial/tkdial.py
+drwxrwxrwx   0        0        0        0 2023-05-21 12:31:12.238883 tkdial-0.0.7/tkdial.egg-info/
+-rw-rw-rw-   0        0        0    19529 2023-05-21 12:31:12.000000 tkdial-0.0.7/tkdial.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      297 2023-05-21 12:31:12.000000 tkdial-0.0.7/tkdial.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       66 2023-05-21 12:31:12.000000 tkdial-0.0.7/tkdial.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-05-21 12:31:12.000000 tkdial-0.0.7/tkdial.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-21 12:31:12.000000 tkdial-0.0.7/tkdial.egg-info/top_level.txt
```

### Comparing `tkdial-0.0.6/LICENSE` & `tkdial-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `tkdial-0.0.6/PKG-INFO` & `tkdial-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tkdial
-Version: 0.0.6
+Version: 0.0.7
 Summary: Rotatory dial-knob widgets for Tkinter.
 Home-page: https://github.com/Akascape/TkDial
-Author: Akascape
+Author: Akash Bora
 License: Creative Commons Zero v1.0 Universal
 Keywords: tkinter,tkinter-dial,tkinter-widget,tkinter-knob,tkinter-meter,tkinter-dial-knob,dial-knob-widget,tkinter-gui
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -406,15 +406,15 @@
 customknob.grid()
 
 app.mainloop()
 ```
 
 ![customknob](https://user-images.githubusercontent.com/89206401/233058156-007f967e-796c-40f1-9c91-419d990fb725.png)
 
-Styles:
+### Styles:
 ```python
 # Note: images are not provided, only for reference
 import customtkinter
 from tkdial import ImageKnob
 
 app = customtkinter.CTk()
 
@@ -461,14 +461,14 @@
 ### Methods:
   | Methods   | Description |
   |-----------|-------------|
   | _.get()_ | get the current value of the widget |
   | _.set()_ | set the value of the widget |
   | _.configure()_ | configure parameters of the widget | 
 
-Note: Images should be cropped in fixed ratio and saved with transparency(png).
+Note: Images should be cropped in fixed ratio (1:1) and saved with transparency(png).
 
 ## Conclusion
 This library is focused to create some circular widgets that can be used with **Tkinter/Customtkinter** easily.
 I hope it will be helpful in UI development with python.
 
 [<img src="https://img.shields.io/badge/LICENSE-CC0_v0.1-informational?&color=blue&style=for-the-badge" width="200">](https://github.com/Akascape/TkDial/blob/main/LICENSE)
```

### Comparing `tkdial-0.0.6/README.md` & `tkdial-0.0.7/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -391,15 +391,15 @@
 customknob.grid()
 
 app.mainloop()
 ```
 
 ![customknob](https://user-images.githubusercontent.com/89206401/233058156-007f967e-796c-40f1-9c91-419d990fb725.png)
 
-Styles:
+### Styles:
 ```python
 # Note: images are not provided, only for reference
 import customtkinter
 from tkdial import ImageKnob
 
 app = customtkinter.CTk()
 
@@ -446,14 +446,14 @@
 ### Methods:
   | Methods   | Description |
   |-----------|-------------|
   | _.get()_ | get the current value of the widget |
   | _.set()_ | set the value of the widget |
   | _.configure()_ | configure parameters of the widget | 
 
-Note: Images should be cropped in fixed ratio and saved with transparency(png).
+Note: Images should be cropped in fixed ratio (1:1) and saved with transparency(png).
 
 ## Conclusion
 This library is focused to create some circular widgets that can be used with **Tkinter/Customtkinter** easily.
 I hope it will be helpful in UI development with python.
 
-[<img src="https://img.shields.io/badge/LICENSE-CC0_v0.1-informational?&color=blue&style=for-the-badge" width="200">](https://github.com/Akascape/TkDial/blob/main/LICENSE)
+[<img src="https://img.shields.io/badge/LICENSE-CC0_v0.1-informational?&color=blue&style=for-the-badge" width="200">](https://github.com/Akascape/TkDial/blob/main/LICENSE)
```

### Comparing `tkdial-0.0.6/setup.cfg` & `tkdial-0.0.7/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2074 6b64 6961 6c0d 0a76 6572 7369   = tkdial..versi
-00000020: 6f6e 203d 2030 2e30 2e36 0d0a 6465 7363  on = 0.0.6..desc
+00000020: 6f6e 203d 2030 2e30 2e37 0d0a 6465 7363  on = 0.0.7..desc
 00000030: 7269 7074 696f 6e20 3d20 546b 696e 7465  ription = Tkinte
 00000040: 7220 4469 616c 2061 6e64 204b 6e6f 6220  r Dial and Knob 
 00000050: 5769 6467 6574 730d 0a6c 6f6e 675f 6465  Widgets..long_de
 00000060: 7363 7269 7074 696f 6e20 3d20 6669 6c65  scription = file
 00000070: 3a20 5245 4144 4d45 2e6d 640d 0a6c 6f6e  : README.md..lon
 00000080: 675f 6465 7363 7269 7074 696f 6e5f 636f  g_description_co
 00000090: 6e74 656e 745f 7479 7065 203d 2074 6578  ntent_type = tex
 000000a0: 742f 6d61 726b 646f 776e 0d0a 7572 6c20  t/markdown..url 
 000000b0: 3d20 6874 7470 733a 2f2f 6769 7468 7562  = https://github
 000000c0: 2e63 6f6d 2f41 6b61 7363 6170 652f 546b  .com/Akascape/Tk
 000000d0: 4469 616c 0d0a 6175 7468 6f72 203d 2041  Dial..author = A
-000000e0: 6b61 7363 6170 650d 0a6c 6963 656e 7365  kascape..license
-000000f0: 203d 2043 7265 6174 6976 6520 436f 6d6d   = Creative Comm
-00000100: 6f6e 7320 5a65 726f 2076 312e 3020 556e  ons Zero v1.0 Un
-00000110: 6976 6572 7361 6c0d 0a6c 6963 656e 7365  iversal..license
-00000120: 5f66 696c 6520 3d20 4c49 4345 4e53 450d  _file = LICENSE.
-00000130: 0a63 6c61 7373 6966 6965 7273 203d 200d  .classifiers = .
-00000140: 0a09 4c69 6365 6e73 6520 3a3a 2043 4330  ..License :: CC0
-00000150: 2031 2e30 2055 6e69 7665 7273 616c 2028   1.0 Universal (
-00000160: 4343 3020 312e 3029 2050 7562 6c69 6320  CC0 1.0) Public 
-00000170: 446f 6d61 696e 2044 6564 6963 6174 696f  Domain Dedicatio
-00000180: 6e0d 0a09 4f70 6572 6174 696e 6720 5379  n...Operating Sy
-00000190: 7374 656d 203a 3a20 4f53 2049 6e64 6570  stem :: OS Indep
-000001a0: 656e 6465 6e74 0d0a 0950 726f 6772 616d  endent...Program
-000001b0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-000001c0: 2050 7974 686f 6e20 3a3a 2033 203a 3a20   Python :: 3 :: 
-000001d0: 4f6e 6c79 0d0a 0d0a 5b6f 7074 696f 6e73  Only....[options
-000001e0: 5d0d 0a70 7974 686f 6e5f 7265 7175 6972  ]..python_requir
-000001f0: 6573 203d 203e 3d33 2e36 0d0a 7061 636b  es = >=3.6..pack
-00000200: 6167 6573 203d 2074 6b64 6961 6c0d 0a69  ages = tkdial..i
-00000210: 6e73 7461 6c6c 5f72 6571 7569 7265 7320  nstall_requires 
-00000220: 3d20 636f 6c6f 7572 0d0a 0d0a 5b65 6767  = colour....[egg
-00000230: 5f69 6e66 6f5d 0d0a 7461 675f 6275 696c  _info]..tag_buil
-00000240: 6420 3d20 0d0a 7461 675f 6461 7465 203d  d = ..tag_date =
-00000250: 2030 0d0a 0d0a                            0....
+000000e0: 6b61 7368 2042 6f72 610d 0a6c 6963 656e  kash Bora..licen
+000000f0: 7365 203d 2043 7265 6174 6976 6520 436f  se = Creative Co
+00000100: 6d6d 6f6e 7320 5a65 726f 2076 312e 3020  mmons Zero v1.0 
+00000110: 556e 6976 6572 7361 6c0d 0a6c 6963 656e  Universal..licen
+00000120: 7365 5f66 696c 6520 3d20 4c49 4345 4e53  se_file = LICENS
+00000130: 450d 0a63 6c61 7373 6966 6965 7273 203d  E..classifiers =
+00000140: 200d 0a09 4c69 6365 6e73 6520 3a3a 2043   ...License :: C
+00000150: 4330 2031 2e30 2055 6e69 7665 7273 616c  C0 1.0 Universal
+00000160: 2028 4343 3020 312e 3029 2050 7562 6c69   (CC0 1.0) Publi
+00000170: 6320 446f 6d61 696e 2044 6564 6963 6174  c Domain Dedicat
+00000180: 696f 6e0d 0a09 4f70 6572 6174 696e 6720  ion...Operating 
+00000190: 5379 7374 656d 203a 3a20 4f53 2049 6e64  System :: OS Ind
+000001a0: 6570 656e 6465 6e74 0d0a 0950 726f 6772  ependent...Progr
+000001b0: 616d 6d69 6e67 204c 616e 6775 6167 6520  amming Language 
+000001c0: 3a3a 2050 7974 686f 6e20 3a3a 2033 203a  :: Python :: 3 :
+000001d0: 3a20 4f6e 6c79 0d0a 0d0a 5b6f 7074 696f  : Only....[optio
+000001e0: 6e73 5d0d 0a70 7974 686f 6e5f 7265 7175  ns]..python_requ
+000001f0: 6972 6573 203d 203e 3d33 2e36 0d0a 7061  ires = >=3.6..pa
+00000200: 636b 6167 6573 203d 2074 6b64 6961 6c0d  ckages = tkdial.
+00000210: 0a69 6e73 7461 6c6c 5f72 6571 7569 7265  .install_require
+00000220: 7320 3d20 636f 6c6f 7572 0d0a 0d0a 5b65  s = colour....[e
+00000230: 6767 5f69 6e66 6f5d 0d0a 7461 675f 6275  gg_info]..tag_bu
+00000240: 696c 6420 3d20 0d0a 7461 675f 6461 7465  ild = ..tag_date
+00000250: 203d 2030 0d0a 0d0a                       = 0....
```

### Comparing `tkdial-0.0.6/setup.py` & `tkdial-0.0.7/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,21 +4,21 @@
     """Opens and fetches text of long descrition file."""
     with open(path, 'r') as f:
         text = f.read()
     return text
 
 setup(
     name = 'tkdial',
-    version = '0.0.6',
+    version = '0.0.7',
     description = "Rotatory dial-knob widgets for Tkinter.",
     license = "Creative Commons Zero v1.0 Universal",
     readme = "README.md",
     long_description = get_long_description('README.md'),
     long_description_content_type = "text/markdown",
-    author = 'Akascape',
+    author = 'Akash Bora',
     url = "https://github.com/Akascape/TkDial",
     classifiers = [
         "License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication",
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
     keywords = ['tkinter', 'tkinter-dial', 'tkinter-widget',
```

### Comparing `tkdial-0.0.6/tkdial/imageknob.py` & `tkdial-0.0.7/tkdial/imageknob.py`

 * *Files 0% similar despite different names*

```diff
@@ -51,15 +51,15 @@
         self.knob_image = image
         self.scale_image = scale_image
         self.progress = progress
         self.progress_color = progress_color
         
         if not self.bg:
             try:
-                if master.winfo_name()=="!ctkframe":
+                if master.winfo_name().startswith("!ctkframe"):
                     # get bg_color of customtkinter frames
                     self.bg = master._apply_appearance_mode(master.cget("fg_color"))
                 else:
                     self.bg = master.cget("bg")
             except:  
                 self.bg = "white"
```

### Comparing `tkdial-0.0.6/tkdial/jogwheel.py` & `tkdial-0.0.7/tkdial/jogwheel.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         self.state = state
         self.__x = radius/2
         self.__y = radius/2
         self.progress = progress
 
         if not self.bg:
             try:
-                if master.winfo_name()=="!ctkframe":
+                if master.winfo_name().startswith("!ctkframe"):
                     # get bg_color of customtkinter frames
                     self.bg = master._apply_appearance_mode(master.cget("fg_color"))
                 else:
                     self.bg = master.cget("bg")
             except:  
                 self.bg = "white"
```

### Comparing `tkdial-0.0.6/tkdial/meter.py` & `tkdial-0.0.7/tkdial/meter.py`

 * *Files 0% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         self.command = command
         self.state = state
         self.__x = radius/2
         self.__y = radius/2
 
         if not self.bg:
             try:
-                if master.winfo_name()=="!ctkframe":
+                if master.winfo_name().startswith("!ctkframe"):
                     # get bg_color of customtkinter frames
                     self.bg = master._apply_appearance_mode(master.cget("fg_color"))
                 else:
                     self.bg = master.cget("bg")
             except:  
                 self.bg = "white"
```

### Comparing `tkdial-0.0.6/tkdial/scrollknob.py` & `tkdial-0.0.7/tkdial/scrollknob.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         self.value = self.start
         self.state = state
         self.integer = integer
         self.command = command
         
         if not self.bg:
             try:
-                if master.winfo_name()=="!ctkframe":
+                if master.winfo_name().startswith("!ctkframe"):
                     # get bg_color of customtkinter frames
                     self.bg = master._apply_appearance_mode(master.cget("fg_color"))
                 else:
                     self.bg = master.cget("bg")
             except:  
                 self.bg = "white"
```

### Comparing `tkdial-0.0.6/tkdial/tkdial.py` & `tkdial-0.0.7/tkdial/tkdial.py`

 * *Files 1% similar despite different names*

```diff
@@ -129,15 +129,15 @@
             ("blue", "blue"): (0, 0, 255, False),
             ("cyan", "cyan"):(0, 255, 255, True),
             ("pink", "pink"): (255, 0, 255, False),
             ("yellow", "yellow"): (255, 255, 0, False)
         }
         if not self.__bg:
             try:
-                if master.winfo_name()=="!ctkframe":
+                if master.winfo_name().startswith("!ctkframe"):
                     # get bg_color of customtkinter frames
                     self.__bg = master._apply_appearance_mode(master.cget("fg_color"))
                 else:
                     self.__bg = master.cget("bg")
             except:  
                 self.__bg = "white"
```

### Comparing `tkdial-0.0.6/tkdial.egg-info/PKG-INFO` & `tkdial-0.0.7/tkdial.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: tkdial
-Version: 0.0.6
+Version: 0.0.7
 Summary: Rotatory dial-knob widgets for Tkinter.
 Home-page: https://github.com/Akascape/TkDial
-Author: Akascape
+Author: Akash Bora
 License: Creative Commons Zero v1.0 Universal
 Keywords: tkinter,tkinter-dial,tkinter-widget,tkinter-knob,tkinter-meter,tkinter-dial-knob,dial-knob-widget,tkinter-gui
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -406,15 +406,15 @@
 customknob.grid()
 
 app.mainloop()
 ```
 
 ![customknob](https://user-images.githubusercontent.com/89206401/233058156-007f967e-796c-40f1-9c91-419d990fb725.png)
 
-Styles:
+### Styles:
 ```python
 # Note: images are not provided, only for reference
 import customtkinter
 from tkdial import ImageKnob
 
 app = customtkinter.CTk()
 
@@ -461,14 +461,14 @@
 ### Methods:
   | Methods   | Description |
   |-----------|-------------|
   | _.get()_ | get the current value of the widget |
   | _.set()_ | set the value of the widget |
   | _.configure()_ | configure parameters of the widget | 
 
-Note: Images should be cropped in fixed ratio and saved with transparency(png).
+Note: Images should be cropped in fixed ratio (1:1) and saved with transparency(png).
 
 ## Conclusion
 This library is focused to create some circular widgets that can be used with **Tkinter/Customtkinter** easily.
 I hope it will be helpful in UI development with python.
 
 [<img src="https://img.shields.io/badge/LICENSE-CC0_v0.1-informational?&color=blue&style=for-the-badge" width="200">](https://github.com/Akascape/TkDial/blob/main/LICENSE)
```

