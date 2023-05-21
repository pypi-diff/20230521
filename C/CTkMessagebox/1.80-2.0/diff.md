# Comparing `tmp/CTkMessagebox-1.80.tar.gz` & `tmp/CTkMessagebox-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CTkMessagebox-1.80.tar", last modified: Fri Apr 14 12:50:29 2023, max compression
+gzip compressed data, was "CTkMessagebox-2.0.tar", last modified: Sun May 21 15:11:45 2023, max compression
```

## Comparing `CTkMessagebox-1.80.tar` & `CTkMessagebox-2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-14 12:50:29.080517 CTkMessagebox-1.80/
-drwxrwxrwx   0        0        0        0 2023-04-14 12:50:29.049269 CTkMessagebox-1.80/CTkMessagebox/
--rw-rw-rw-   0        0        0      233 2023-04-14 12:49:07.000000 CTkMessagebox-1.80/CTkMessagebox/__init__.py
--rw-rw-rw-   0        0        0    12818 2023-04-14 12:49:19.000000 CTkMessagebox-1.80/CTkMessagebox/ctkmessagebox.py
-drwxrwxrwx   0        0        0        0 2023-04-14 12:50:29.080517 CTkMessagebox-1.80/CTkMessagebox/icons/
--rw-rw-rw-   0        0        0    38437 2023-02-24 17:58:14.000000 CTkMessagebox-1.80/CTkMessagebox/icons/cancel.png
--rw-rw-rw-   0        0        0    31308 2023-02-24 17:40:20.000000 CTkMessagebox-1.80/CTkMessagebox/icons/check.png
--rw-rw-rw-   0        0        0    14921 2023-02-24 18:08:36.000000 CTkMessagebox-1.80/CTkMessagebox/icons/info.png
--rw-rw-rw-   0        0        0    15030 2023-04-14 12:27:30.000000 CTkMessagebox-1.80/CTkMessagebox/icons/question.png
--rw-rw-rw-   0        0        0    17104 2023-02-24 18:03:33.000000 CTkMessagebox-1.80/CTkMessagebox/icons/warning.png
-drwxrwxrwx   0        0        0        0 2023-04-14 12:50:29.064892 CTkMessagebox-1.80/CTkMessagebox.egg-info/
--rw-rw-rw-   0        0        0     5960 2023-04-14 12:50:29.000000 CTkMessagebox-1.80/CTkMessagebox.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      432 2023-04-14 12:50:29.000000 CTkMessagebox-1.80/CTkMessagebox.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       73 2023-04-14 12:50:29.000000 CTkMessagebox-1.80/CTkMessagebox.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       21 2023-04-14 12:50:29.000000 CTkMessagebox-1.80/CTkMessagebox.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-14 12:50:29.000000 CTkMessagebox-1.80/CTkMessagebox.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7048 2022-11-20 16:16:56.000000 CTkMessagebox-1.80/LICENSE
--rw-rw-rw-   0        0        0     5960 2023-04-14 12:50:29.080517 CTkMessagebox-1.80/PKG-INFO
--rw-rw-rw-   0        0        0     5261 2023-04-14 12:41:41.000000 CTkMessagebox-1.80/README.md
--rw-rw-rw-   0        0        0      626 2023-04-14 12:50:29.080517 CTkMessagebox-1.80/setup.cfg
--rw-rw-rw-   0        0        0     1362 2023-04-14 12:49:58.000000 CTkMessagebox-1.80/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-21 15:11:45.324717 CTkMessagebox-2.0/
+drwxrwxrwx   0        0        0        0 2023-05-21 15:11:45.283712 CTkMessagebox-2.0/CTkMessagebox/
+-rw-rw-rw-   0        0        0      232 2023-05-21 14:38:38.000000 CTkMessagebox-2.0/CTkMessagebox/__init__.py
+-rw-rw-rw-   0        0        0    13914 2023-05-21 15:02:20.000000 CTkMessagebox-2.0/CTkMessagebox/ctkmessagebox.py
+drwxrwxrwx   0        0        0        0 2023-05-21 15:11:45.322717 CTkMessagebox-2.0/CTkMessagebox/icons/
+-rw-rw-rw-   0        0        0    38437 2023-02-24 17:58:14.000000 CTkMessagebox-2.0/CTkMessagebox/icons/cancel.png
+-rw-rw-rw-   0        0        0    31308 2023-02-24 17:40:20.000000 CTkMessagebox-2.0/CTkMessagebox/icons/check.png
+-rw-rw-rw-   0        0        0    14921 2023-02-24 18:08:36.000000 CTkMessagebox-2.0/CTkMessagebox/icons/info.png
+-rw-rw-rw-   0        0        0    15030 2023-04-14 12:27:30.000000 CTkMessagebox-2.0/CTkMessagebox/icons/question.png
+-rw-rw-rw-   0        0        0    17104 2023-02-24 18:03:33.000000 CTkMessagebox-2.0/CTkMessagebox/icons/warning.png
+drwxrwxrwx   0        0        0        0 2023-05-21 15:11:45.301716 CTkMessagebox-2.0/CTkMessagebox.egg-info/
+-rw-rw-rw-   0        0        0     6291 2023-05-21 15:11:45.000000 CTkMessagebox-2.0/CTkMessagebox.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      432 2023-05-21 15:11:45.000000 CTkMessagebox-2.0/CTkMessagebox.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       73 2023-05-21 15:11:45.000000 CTkMessagebox-2.0/CTkMessagebox.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       21 2023-05-21 15:11:45.000000 CTkMessagebox-2.0/CTkMessagebox.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-21 15:11:45.000000 CTkMessagebox-2.0/CTkMessagebox.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7048 2022-11-20 16:16:56.000000 CTkMessagebox-2.0/LICENSE
+-rw-rw-rw-   0        0        0     6291 2023-05-21 15:11:45.325717 CTkMessagebox-2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5593 2023-05-21 15:11:13.000000 CTkMessagebox-2.0/README.md
+-rw-rw-rw-   0        0        0      625 2023-05-21 15:11:45.327717 CTkMessagebox-2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1361 2023-05-21 14:38:15.000000 CTkMessagebox-2.0/setup.py
```

### Comparing `CTkMessagebox-1.80/CTkMessagebox/ctkmessagebox.py` & `CTkMessagebox-2.0/CTkMessagebox/ctkmessagebox.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 CustomTkinter Messagebox
 Author: Akash Bora
-Version: 1.80
+Version: 2.0
 """
 
 import customtkinter
 from PIL import Image
 import os
 import sys
 import time
@@ -17,25 +17,27 @@
                  width: int = 400,
                  height: int = 200,
                  title: str = "CTkMessagebox",
                  message: str = "This is a CTkMessagebox!",
                  option_1: str = "OK",
                  option_2: str = None,
                  option_3: str = None,
+                 options: list = [],
                  border_width: int = 1,
                  border_color: str = "default",
                  button_color: str = "default",
                  bg_color: str = "default",
                  fg_color: str = "default",
                  text_color: str = "default",
                  title_color: str = "default",
                  button_text_color: str = "default",
                  button_width: int = None,
                  button_height: int = None,
-                 cancel_button_color: str = "#c42b1c",
+                 cancel_button_color: str = None,
+                 cancel_button: str = "circle", # types: circle, cross or none
                  button_hover_color: str = "default",
                  icon: str = "info",
                  icon_size: tuple = None,
                  corner_radius: int = 15,
                  font: tuple = None,
                  header: bool = False,
                  topmost: bool = True,
@@ -88,23 +90,31 @@
         self.grid_columnconfigure(0, weight=1)
         self.grid_rowconfigure(0, weight=1)    
         self.x = self.winfo_x()
         self.y = self.winfo_y()
         self._title = title
         self.message = message
         self.font = font
+        self.cancel_button = cancel_button
         self.round_corners = corner_radius if corner_radius<=30 else 30
         self.button_width = button_width if button_width else self.width/4
         self.button_height = button_height if button_height else 28
         if self.fade: self.attributes("-alpha", 0)
         
         if self.button_height>self.height/4: self.button_height = self.height/4 -20
         self.dot_color = cancel_button_color
         self.border_width = border_width if border_width<6 else 5
-    
+        
+        if type(options) is list and len(options)>0:
+            try:
+                option_1 = options[-1]
+                option_2 = options[-2]
+                option_3 = options[-3]
+            except IndexError: None
+            
         if bg_color=="default":
             self.bg_color = self._apply_appearance_mode(customtkinter.ThemeManager.theme["CTkFrame"]["fg_color"])
         else:
             self.bg_color = bg_color
 
         if fg_color=="default":
             self.fg_color = self._apply_appearance_mode(customtkinter.ThemeManager.theme["CTkFrame"]["top_fg_color"])
@@ -175,20 +185,27 @@
         if button_height:
             self.frame_top.grid_rowconfigure((0,1,3), weight=1)
         else:
             self.frame_top.grid_rowconfigure((0,1,2), weight=1)
             
         self.frame_top.bind("<B1-Motion>", self.move_window)
         self.frame_top.bind("<ButtonPress-1>", self.oldxyset)
-        
-        self.button_close = customtkinter.CTkButton(self.frame_top, corner_radius=10, width=10, height=10, hover=False,
-                                           text="", fg_color=self.dot_color, command=self.button_event)
-        self.button_close.configure(cursor="arrow")        
-        self.button_close.grid(row=0, column=3, sticky="ne", padx=10, pady=10)
 
+        if self.cancel_button=="cross":
+            self.button_close = customtkinter.CTkButton(self.frame_top, corner_radius=10, width=0, height=0, hover=False,
+                                                        text_color=self.dot_color if self.dot_color else self.title_color,
+                                                        text="✕", fg_color="transparent", command=self.button_event)
+            self.button_close.grid(row=0, column=3, sticky="ne", padx=5+self.border_width, pady=5+self.border_width)
+            self.button_close.configure(cursor="arrow")
+        elif self.cancel_button=="circle":
+            self.button_close = customtkinter.CTkButton(self.frame_top, corner_radius=10, width=10, height=10, hover=False,
+                                                        text="", fg_color=self.dot_color if self.dot_color else "#c42b1c", command=self.button_event)     
+            self.button_close.grid(row=0, column=3, sticky="ne", padx=10, pady=10)       
+            self.button_close.configure(cursor="arrow")
+            
         self.title_label = customtkinter.CTkLabel(self.frame_top, width=1, text=self._title, text_color=self.title_color, font=self.font)
         self.title_label.grid(row=0, column=0, columnspan=4, sticky="nw", padx=(15,30), pady=5)
         self.title_label.bind("<B1-Motion>", self.move_window)
         self.title_label.bind("<ButtonPress-1>", self.oldxyset)
         
         self.info = customtkinter.CTkButton(self.frame_top,  width=1, height=self.height/2, corner_radius=0, text=self.message, font=self.font,
                                             fg_color=self.fg_color, hover=False, text_color=self.text_color, image=self.icon)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `CTkMessagebox-1.80/CTkMessagebox/icons/cancel.png` & `CTkMessagebox-2.0/CTkMessagebox/icons/cancel.png`

 * *Files identical despite different names*

### Comparing `CTkMessagebox-1.80/CTkMessagebox/icons/check.png` & `CTkMessagebox-2.0/CTkMessagebox/icons/check.png`

 * *Files identical despite different names*

### Comparing `CTkMessagebox-1.80/CTkMessagebox/icons/info.png` & `CTkMessagebox-2.0/CTkMessagebox/icons/info.png`

 * *Files identical despite different names*

### Comparing `CTkMessagebox-1.80/CTkMessagebox/icons/question.png` & `CTkMessagebox-2.0/CTkMessagebox/icons/question.png`

 * *Files identical despite different names*

### Comparing `CTkMessagebox-1.80/CTkMessagebox/icons/warning.png` & `CTkMessagebox-2.0/CTkMessagebox/icons/warning.png`

 * *Files identical despite different names*

### Comparing `CTkMessagebox-1.80/CTkMessagebox.egg-info/PKG-INFO` & `CTkMessagebox-2.0/CTkMessagebox.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTkMessagebox
-Version: 1.80
+Version: 2.0
 Summary: A modern messagebox for customtkinter
 Home-page: https://github.com/Akascape/CTkMessagebox
 Author: Akash Bora
 License: Creative Commons Zero v1.0 Universal
 Keywords: customtkinter,customtkinter-dialog,customtkinter-messagebox,customtkinter-message-box,tkinter-messagebox,customtkinter-tkinter-messagebox,messagebox-widget,modern-tkinter-messagebox,ctkmessagebox
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Programming Language :: Python :: 3
@@ -30,14 +30,16 @@
 ```
 pip install CTkMessagebox
 ```
 
 [<img alt="GitHub repo size" src="https://img.shields.io/github/repo-size/Akascape/CTkMessagebox?&color=green&label=Source%20Code&logo=Python&logoColor=yellow&style=for-the-badge"  width="300">](https://github.com/Akascape/CTkMessagebox/archive/refs/heads/main.zip)
 
 [![PyPI](https://img.shields.io/pypi/v/CTkMessagebox?style=flat)](https://pypi.org/project/CTkMessagebox)
+[![Downloads](https://static.pepy.tech/badge/ctkmessagebox)](https://pepy.tech/project/ctkmessagebox)
+![Platform](https://img.shields.io/powershellgallery/p/Pester?color=blue)
 
 ## How it looks?
 ![Screenshot](https://user-images.githubusercontent.com/89206401/221258593-75058878-b598-40c3-828a-1d44a6cefb73.jpg)
 
 ## Example
 ```python
 from CTkMessagebox import CTkMessagebox
@@ -100,23 +102,25 @@
   | _fg_color_ | forground color of the messagebox [middle portion] |
   | _bg_color_  | background color of the messagebox |
   | **_title_** | title of the messagebox |
   | **_message_** | main message of the messagebox which will be shown at the center |
   | **_option_1_** | the text on the first button [Default is 'OK'] |
   | **_option_2_** | the text on the second button |
   | **_option_3_** | the text on the last button |
+  | _options_ | directly pass a list containing the options in order |
   | _button_color_ | color of the buttons |
   | _text_color_ | color of the message-text |
   | _title_color_ | color of the title-text |
   | _button_text_color_ | color of the button-text |
   | _button_hover_color_ | hover color of the buttons |
   | _button_width_ | width of the buttons in px |
   | _button_height_ | height of the buttons in px |
   | _border_width_ | width of the border around the main frame [Default is 1] |
   | _border_color_ | color of the frame border |
+  | _cancel_button_ | define the cancel button type: **circle, cross or None** |
   | _cancel_button_color_ | color of the **close** button, **set it to 'transparent' if you want to hide it** |
   | **_icon_** | icon that will be shown in the messagebox [Default is the 'info' icon] |
   | _icon_size_ | define the size of the icon image manually (tuple) |
   | _corner_radius_ | corner roundness of the messagebox window [**not applicable in linux**] |
   | _font_ | font of the messagebox text (tuple) |
   | _header_ | add the original header back if you don't like **overrideredirect** (bool) |
   | _topmost_ | disable the topmost window outside the app (bool) |
```

### Comparing `CTkMessagebox-1.80/LICENSE` & `CTkMessagebox-2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `CTkMessagebox-1.80/PKG-INFO` & `CTkMessagebox-2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CTkMessagebox
-Version: 1.80
+Version: 2.0
 Summary: A modern messagebox for customtkinter
 Home-page: https://github.com/Akascape/CTkMessagebox
 Author: Akash Bora
 License: Creative Commons Zero v1.0 Universal
 Keywords: customtkinter,customtkinter-dialog,customtkinter-messagebox,customtkinter-message-box,tkinter-messagebox,customtkinter-tkinter-messagebox,messagebox-widget,modern-tkinter-messagebox,ctkmessagebox
 Classifier: License :: CC0 1.0 Universal (CC0 1.0) Public Domain Dedication
 Classifier: Programming Language :: Python :: 3
@@ -30,14 +30,16 @@
 ```
 pip install CTkMessagebox
 ```
 
 [<img alt="GitHub repo size" src="https://img.shields.io/github/repo-size/Akascape/CTkMessagebox?&color=green&label=Source%20Code&logo=Python&logoColor=yellow&style=for-the-badge"  width="300">](https://github.com/Akascape/CTkMessagebox/archive/refs/heads/main.zip)
 
 [![PyPI](https://img.shields.io/pypi/v/CTkMessagebox?style=flat)](https://pypi.org/project/CTkMessagebox)
+[![Downloads](https://static.pepy.tech/badge/ctkmessagebox)](https://pepy.tech/project/ctkmessagebox)
+![Platform](https://img.shields.io/powershellgallery/p/Pester?color=blue)
 
 ## How it looks?
 ![Screenshot](https://user-images.githubusercontent.com/89206401/221258593-75058878-b598-40c3-828a-1d44a6cefb73.jpg)
 
 ## Example
 ```python
 from CTkMessagebox import CTkMessagebox
@@ -100,23 +102,25 @@
   | _fg_color_ | forground color of the messagebox [middle portion] |
   | _bg_color_  | background color of the messagebox |
   | **_title_** | title of the messagebox |
   | **_message_** | main message of the messagebox which will be shown at the center |
   | **_option_1_** | the text on the first button [Default is 'OK'] |
   | **_option_2_** | the text on the second button |
   | **_option_3_** | the text on the last button |
+  | _options_ | directly pass a list containing the options in order |
   | _button_color_ | color of the buttons |
   | _text_color_ | color of the message-text |
   | _title_color_ | color of the title-text |
   | _button_text_color_ | color of the button-text |
   | _button_hover_color_ | hover color of the buttons |
   | _button_width_ | width of the buttons in px |
   | _button_height_ | height of the buttons in px |
   | _border_width_ | width of the border around the main frame [Default is 1] |
   | _border_color_ | color of the frame border |
+  | _cancel_button_ | define the cancel button type: **circle, cross or None** |
   | _cancel_button_color_ | color of the **close** button, **set it to 'transparent' if you want to hide it** |
   | **_icon_** | icon that will be shown in the messagebox [Default is the 'info' icon] |
   | _icon_size_ | define the size of the icon image manually (tuple) |
   | _corner_radius_ | corner roundness of the messagebox window [**not applicable in linux**] |
   | _font_ | font of the messagebox text (tuple) |
   | _header_ | add the original header back if you don't like **overrideredirect** (bool) |
   | _topmost_ | disable the topmost window outside the app (bool) |
```

### Comparing `CTkMessagebox-1.80/README.md` & `CTkMessagebox-2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 ```
 pip install CTkMessagebox
 ```
 
 [<img alt="GitHub repo size" src="https://img.shields.io/github/repo-size/Akascape/CTkMessagebox?&color=green&label=Source%20Code&logo=Python&logoColor=yellow&style=for-the-badge"  width="300">](https://github.com/Akascape/CTkMessagebox/archive/refs/heads/main.zip)
 
 [![PyPI](https://img.shields.io/pypi/v/CTkMessagebox?style=flat)](https://pypi.org/project/CTkMessagebox)
+[![Downloads](https://static.pepy.tech/badge/ctkmessagebox)](https://pepy.tech/project/ctkmessagebox)
+![Platform](https://img.shields.io/powershellgallery/p/Pester?color=blue)
 
 ## How it looks?
 ![Screenshot](https://user-images.githubusercontent.com/89206401/221258593-75058878-b598-40c3-828a-1d44a6cefb73.jpg)
 
 ## Example
 ```python
 from CTkMessagebox import CTkMessagebox
@@ -85,23 +87,25 @@
   | _fg_color_ | forground color of the messagebox [middle portion] |
   | _bg_color_  | background color of the messagebox |
   | **_title_** | title of the messagebox |
   | **_message_** | main message of the messagebox which will be shown at the center |
   | **_option_1_** | the text on the first button [Default is 'OK'] |
   | **_option_2_** | the text on the second button |
   | **_option_3_** | the text on the last button |
+  | _options_ | directly pass a list containing the options in order |
   | _button_color_ | color of the buttons |
   | _text_color_ | color of the message-text |
   | _title_color_ | color of the title-text |
   | _button_text_color_ | color of the button-text |
   | _button_hover_color_ | hover color of the buttons |
   | _button_width_ | width of the buttons in px |
   | _button_height_ | height of the buttons in px |
   | _border_width_ | width of the border around the main frame [Default is 1] |
   | _border_color_ | color of the frame border |
+  | _cancel_button_ | define the cancel button type: **circle, cross or None** |
   | _cancel_button_color_ | color of the **close** button, **set it to 'transparent' if you want to hide it** |
   | **_icon_** | icon that will be shown in the messagebox [Default is the 'info' icon] |
   | _icon_size_ | define the size of the icon image manually (tuple) |
   | _corner_radius_ | corner roundness of the messagebox window [**not applicable in linux**] |
   | _font_ | font of the messagebox text (tuple) |
   | _header_ | add the original header back if you don't like **overrideredirect** (bool) |
   | _topmost_ | disable the topmost window outside the app (bool) |
```

### Comparing `CTkMessagebox-1.80/setup.cfg` & `CTkMessagebox-2.0/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2043 546b 4d65 7373 6167 6562 6f78   = CTkMessagebox
-00000020: 0d0a 7665 7273 696f 6e20 3d20 312e 3830  ..version = 1.80
-00000030: 0d0a 6465 7363 7269 7074 696f 6e20 3d20  ..description = 
-00000040: 4120 6d6f 6465 726e 206d 6573 7361 6765  A modern message
-00000050: 626f 7820 666f 7220 6375 7374 6f6d 746b  box for customtk
-00000060: 696e 7465 720d 0a6c 6f6e 675f 6465 7363  inter..long_desc
-00000070: 7269 7074 696f 6e20 3d20 6669 6c65 3a20  ription = file: 
-00000080: 5245 4144 4d45 2e6d 640d 0a6c 6f6e 675f  README.md..long_
-00000090: 6465 7363 7269 7074 696f 6e5f 636f 6e74  description_cont
-000000a0: 656e 745f 7479 7065 203d 2074 6578 742f  ent_type = text/
-000000b0: 6d61 726b 646f 776e 0d0a 7572 6c20 3d20  markdown..url = 
-000000c0: 6874 7470 733a 2f2f 6769 7468 7562 2e63  https://github.c
-000000d0: 6f6d 2f41 6b61 7363 6170 652f 4354 6b4d  om/Akascape/CTkM
-000000e0: 6573 7361 6765 626f 780d 0a61 7574 686f  essagebox..autho
-000000f0: 7220 3d20 416b 6173 6820 426f 7261 0d0a  r = Akash Bora..
-00000100: 6c69 6365 6e73 6520 3d20 4372 6561 7469  license = Creati
-00000110: 7665 2043 6f6d 6d6f 6e73 205a 6572 6f20  ve Commons Zero 
-00000120: 7631 2e30 2055 6e69 7665 7273 616c 0d0a  v1.0 Universal..
-00000130: 6c69 6365 6e73 655f 6669 6c65 203d 204c  license_file = L
-00000140: 4943 454e 5345 0d0a 636c 6173 7369 6669  ICENSE..classifi
-00000150: 6572 7320 3d20 0d0a 094c 6963 656e 7365  ers = ...License
-00000160: 203a 3a20 4343 3020 312e 3020 556e 6976   :: CC0 1.0 Univ
-00000170: 6572 7361 6c20 2843 4330 2031 2e30 2920  ersal (CC0 1.0) 
-00000180: 5075 626c 6963 2044 6f6d 6169 6e20 4465  Public Domain De
-00000190: 6469 6361 7469 6f6e 0d0a 094f 7065 7261  dication...Opera
-000001a0: 7469 6e67 2053 7973 7465 6d20 3a3a 204f  ting System :: O
-000001b0: 5320 496e 6465 7065 6e64 656e 740d 0a09  S Independent...
-000001c0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-000001d0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-000001e0: 3a20 3320 3a3a 204f 6e6c 790d 0a0d 0a5b  : 3 :: Only....[
-000001f0: 6f70 7469 6f6e 735d 0d0a 7079 7468 6f6e  options]..python
-00000200: 5f72 6571 7569 7265 7320 3d20 3e3d 332e  _requires = >=3.
-00000210: 360d 0a70 6163 6b61 6765 7320 3d20 0d0a  6..packages = ..
-00000220: 0943 546b 4d65 7373 6167 6562 6f78 0d0a  .CTkMessagebox..
-00000230: 0943 546b 4d65 7373 6167 6562 6f78 2e69  .CTkMessagebox.i
-00000240: 636f 6e73 0d0a 0d0a 5b65 6767 5f69 6e66  cons....[egg_inf
-00000250: 6f5d 0d0a 7461 675f 6275 696c 6420 3d20  o]..tag_build = 
-00000260: 0d0a 7461 675f 6461 7465 203d 2030 0d0a  ..tag_date = 0..
-00000270: 0d0a                                     ..
+00000020: 0d0a 7665 7273 696f 6e20 3d20 322e 300d  ..version = 2.0.
+00000030: 0a64 6573 6372 6970 7469 6f6e 203d 2041  .description = A
+00000040: 206d 6f64 6572 6e20 6d65 7373 6167 6562   modern messageb
+00000050: 6f78 2066 6f72 2063 7573 746f 6d74 6b69  ox for customtki
+00000060: 6e74 6572 0d0a 6c6f 6e67 5f64 6573 6372  nter..long_descr
+00000070: 6970 7469 6f6e 203d 2066 696c 653a 2052  iption = file: R
+00000080: 4541 444d 452e 6d64 0d0a 6c6f 6e67 5f64  EADME.md..long_d
+00000090: 6573 6372 6970 7469 6f6e 5f63 6f6e 7465  escription_conte
+000000a0: 6e74 5f74 7970 6520 3d20 7465 7874 2f6d  nt_type = text/m
+000000b0: 6172 6b64 6f77 6e0d 0a75 726c 203d 2068  arkdown..url = h
+000000c0: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+000000d0: 6d2f 416b 6173 6361 7065 2f43 546b 4d65  m/Akascape/CTkMe
+000000e0: 7373 6167 6562 6f78 0d0a 6175 7468 6f72  ssagebox..author
+000000f0: 203d 2041 6b61 7368 2042 6f72 610d 0a6c   = Akash Bora..l
+00000100: 6963 656e 7365 203d 2043 7265 6174 6976  icense = Creativ
+00000110: 6520 436f 6d6d 6f6e 7320 5a65 726f 2076  e Commons Zero v
+00000120: 312e 3020 556e 6976 6572 7361 6c0d 0a6c  1.0 Universal..l
+00000130: 6963 656e 7365 5f66 696c 6520 3d20 4c49  icense_file = LI
+00000140: 4345 4e53 450d 0a63 6c61 7373 6966 6965  CENSE..classifie
+00000150: 7273 203d 200d 0a09 4c69 6365 6e73 6520  rs = ...License 
+00000160: 3a3a 2043 4330 2031 2e30 2055 6e69 7665  :: CC0 1.0 Unive
+00000170: 7273 616c 2028 4343 3020 312e 3029 2050  rsal (CC0 1.0) P
+00000180: 7562 6c69 6320 446f 6d61 696e 2044 6564  ublic Domain Ded
+00000190: 6963 6174 696f 6e0d 0a09 4f70 6572 6174  ication...Operat
+000001a0: 696e 6720 5379 7374 656d 203a 3a20 4f53  ing System :: OS
+000001b0: 2049 6e64 6570 656e 6465 6e74 0d0a 0950   Independent...P
+000001c0: 726f 6772 616d 6d69 6e67 204c 616e 6775  rogramming Langu
+000001d0: 6167 6520 3a3a 2050 7974 686f 6e20 3a3a  age :: Python ::
+000001e0: 2033 203a 3a20 4f6e 6c79 0d0a 0d0a 5b6f   3 :: Only....[o
+000001f0: 7074 696f 6e73 5d0d 0a70 7974 686f 6e5f  ptions]..python_
+00000200: 7265 7175 6972 6573 203d 203e 3d33 2e36  requires = >=3.6
+00000210: 0d0a 7061 636b 6167 6573 203d 200d 0a09  ..packages = ...
+00000220: 4354 6b4d 6573 7361 6765 626f 780d 0a09  CTkMessagebox...
+00000230: 4354 6b4d 6573 7361 6765 626f 782e 6963  CTkMessagebox.ic
+00000240: 6f6e 730d 0a0d 0a5b 6567 675f 696e 666f  ons....[egg_info
+00000250: 5d0d 0a74 6167 5f62 7569 6c64 203d 200d  ]..tag_build = .
+00000260: 0a74 6167 5f64 6174 6520 3d20 300d 0a0d  .tag_date = 0...
+00000270: 0a                                       .
```

### Comparing `CTkMessagebox-1.80/setup.py` & `CTkMessagebox-2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     """Opens and fetches text of long descrition file."""
     with open(path, 'r') as f:
         text = f.read()
     return text
 
 setup(
     name = 'CTkMessagebox',
-    version = '1.80',
+    version = '2.0',
     description = "A modern messagebox for customtkinter",
     license = "Creative Commons Zero v1.0 Universal",
     readme = "README.md",
     long_description = get_long_description('README.md'),
     long_description_content_type = "text/markdown",
     author = 'Akash Bora',
     url = "https://github.com/Akascape/CTkMessagebox",
```

