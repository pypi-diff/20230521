# Comparing `tmp/tkintertools-2.6.1.tar.gz` & `tmp/tkintertools-2.6.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkintertools-2.6.1.tar", last modified: Sun May 21 08:29:30 2023, max compression
+gzip compressed data, was "tkintertools-2.6.1.1.tar", last modified: Sun May 21 10:08:41 2023, max compression
```

## Comparing `tkintertools-2.6.1.tar` & `tkintertools-2.6.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-21 08:29:30.608759 tkintertools-2.6.1/
--rw-rw-rw-   0        0        0     7548 2023-05-20 23:03:00.000000 tkintertools-2.6.1/LICENSE
--rw-rw-rw-   0        0        0    26393 2023-05-21 08:29:30.607759 tkintertools-2.6.1/PKG-INFO
--rw-rw-rw-   0        0        0    25888 2023-05-21 08:23:58.000000 tkintertools-2.6.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-21 08:29:30.608759 tkintertools-2.6.1/setup.cfg
--rw-rw-rw-   0        0        0     1206 2023-05-21 08:28:45.000000 tkintertools-2.6.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-21 08:29:30.602758 tkintertools-2.6.1/tkintertools/
--rw-rw-rw-   0        0        0     1877 2023-05-20 20:35:35.000000 tkintertools-2.6.1/tkintertools/__init__.py
--rw-rw-rw-   0        0        0    60681 2023-05-21 06:47:19.000000 tkintertools-2.6.1/tkintertools/__main__.py
--rw-rw-rw-   0        0        0     1295 2023-05-20 20:58:40.000000 tkintertools-2.6.1/tkintertools/constants.py
--rw-rw-rw-   0        0        0      870 2023-05-14 13:27:34.000000 tkintertools-2.6.1/tkintertools/md.py
-drwxrwxrwx   0        0        0        0 2023-05-21 08:29:30.606759 tkintertools-2.6.1/tkintertools.egg-info/
--rw-rw-rw-   0        0        0    26393 2023-05-21 08:29:30.000000 tkintertools-2.6.1/tkintertools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      265 2023-05-21 08:29:30.000000 tkintertools-2.6.1/tkintertools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-21 08:29:30.000000 tkintertools-2.6.1/tkintertools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-05-21 08:29:30.000000 tkintertools-2.6.1/tkintertools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-21 10:08:41.589826 tkintertools-2.6.1.1/
+-rw-rw-rw-   0        0        0     7548 2023-05-20 23:03:00.000000 tkintertools-2.6.1.1/LICENSE
+-rw-rw-rw-   0        0        0    26443 2023-05-21 10:08:41.588826 tkintertools-2.6.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0    25936 2023-05-21 09:54:32.000000 tkintertools-2.6.1.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-21 10:08:41.589826 tkintertools-2.6.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1208 2023-05-21 10:07:51.000000 tkintertools-2.6.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-21 10:08:41.580824 tkintertools-2.6.1.1/tkintertools/
+-rw-rw-rw-   0        0        0     1877 2023-05-20 20:35:35.000000 tkintertools-2.6.1.1/tkintertools/__init__.py
+-rw-rw-rw-   0        0        0    60750 2023-05-21 10:02:16.000000 tkintertools-2.6.1.1/tkintertools/__main__.py
+-rw-rw-rw-   0        0        0     1295 2023-05-20 20:58:40.000000 tkintertools-2.6.1.1/tkintertools/constants.py
+-rw-rw-rw-   0        0        0      870 2023-05-14 13:27:34.000000 tkintertools-2.6.1.1/tkintertools/md.py
+drwxrwxrwx   0        0        0        0 2023-05-21 10:08:41.586825 tkintertools-2.6.1.1/tkintertools.egg-info/
+-rw-rw-rw-   0        0        0    26443 2023-05-21 10:08:41.000000 tkintertools-2.6.1.1/tkintertools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2023-05-21 10:08:41.000000 tkintertools-2.6.1.1/tkintertools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-21 10:08:41.000000 tkintertools-2.6.1.1/tkintertools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-21 10:08:41.000000 tkintertools-2.6.1.1/tkintertools.egg-info/top_level.txt
```

### Comparing `tkintertools-2.6.1/LICENSE` & `tkintertools-2.6.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tkintertools-2.6.1/PKG-INFO` & `tkintertools-2.6.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkintertools
-Version: 2.6.1
+Version: 2.6.1.1
 Summary: An auxiliary module of the tkinder module
 Home-page: https://gitcode.net/weixin_62651706/tkintertools
 Author: Xiaokang2022
 Author-email: 2951256653@qq.com
 License: MulanPSL-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)
@@ -182,15 +182,15 @@
 
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('LabelTest', 1000, 400)
-    canvas = tkt.Canvas(root, 1000, 400)
+    canvas = tkt.Canvas(root, 1000, 400, 0, 0)
 
 
     def colorful(x, y, width, height):  # type: (int, int, int, int) -> None
         """ Gradient colors """
         for i in range(width):
             color = tkt.color(('#FF0000', '#0000FF'), i/width)
             canvas.create_line(x+i, y, x+i, y+height, fill=color)
@@ -216,15 +216,15 @@
 
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('ButtonTest', 500, 500)
-    canvas = tkt.Canvas(root, 500, 500)
+    canvas = tkt.Canvas(root, 500, 500, 0, 0)
 
 
     def colorful(x, y, width, height):  # type: (int, int, int, int) -> None
         """ Gradient colors """
         for i in range(width):
             color = tkt.color(('#FF0000', '#0000FF'), i/width)
             canvas.create_line(x+i, y, x+i, y+height, fill=color)
@@ -250,15 +250,15 @@
 
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('CheckButtonTest', 500, 300)
-    canvas = tkt.Canvas(root, 500, 300)
+    canvas = tkt.Canvas(root, 500, 300, 0, 0)
 
 
     def colorful(x, y, width, height):  # type: (int, int, int, int) -> None
         """ Gradient colors """
         for i in range(width):
             color = tkt.color(('#FF0000', '#0000FF'), i/width)
             canvas.create_line(x+i, y, x+i, y+height, fill=color)
@@ -285,15 +285,15 @@
     
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('EntryTest', 500, 400)
-    canvas = tkt.Canvas(root, 500, 400)
+    canvas = tkt.Canvas(root, 500, 400, 0, 0)
 
 
     def colorful(x, y, width, height):  # type: (int, int, int, int) -> None
         """ Gradient colors """
         for i in range(width):
             color = tkt.color(('#FF0000', '#0000FF'), i/width)
             canvas.create_line(x+i, y, x+i, y+height, fill=color)
@@ -330,15 +330,15 @@
     
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('TextTest', 1000, 400)
-    canvas = tkt.Canvas(root, 1000, 400)
+    canvas = tkt.Canvas(root, 1000, 400, 0, 0)
 
 
     def colorful(x, y, width, height) -> None:  # type: (int, int, int, int) -> None
         """ Gradient colors """
         for i in range(width):
             color = tkt.color(('#FF0000', '#0000FF'), i/width)
             canvas.create_line(x+i, y, x+i, y+height, fill=color)
@@ -365,15 +365,15 @@
 
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('ProgressbarTest', 500, 500)
-    canvas = tkt.Canvas(root, 500, 500)
+    canvas = tkt.Canvas(root, 500, 500, 0, 0)
 
 
     def colorful(x, y, width, height) -> None:  # type: (int, int, int, int) -> None
         """ Gradient colors """
         for i in range(width):
             color = tkt.color(('#FF0000', '#0000FF'), i/width)
             canvas.create_line(x+i, y, x+i, y+height, fill=color)
@@ -426,15 +426,15 @@
     
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('MoveTest', 500, 500)
-    canvas = tkt.Canvas(root, 500, 500)
+    canvas = tkt.Canvas(root, 500, 500, 0, 0)
     rect = canvas.create_rectangle(50, 350, 150, 450)
 
 
     def move_window(switch=[True]):  # type: (list[bool]) -> None
         tkt.move(root, None, 1000 if switch[0] else -1000, 0, 800, mode='flat')
         switch[0] = not switch[0]
 
@@ -480,15 +480,15 @@
 
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('ColorTest', 500, 500)
-    canvas = tkt.Canvas(root, 500, 500)
+    canvas = tkt.Canvas(root, 500, 500, 0, 0)
 
 
     def colorful(x, y, width, height):  # type: (int, int, int, int) -> None
         """ Gradient colors """
         for i in range(width):
             color = tkt.color(('#FF0000', '#00FF00'), i/width)
             color_2 = tkt.color(('#FFFFFF', '#000000'), i/width)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tkintertools Version: 2.6.1 Summary: An auxiliary
+Metadata-Version: 2.1 Name: tkintertools Version: 2.6.1.1 Summary: An auxiliary
 module of the tkinder module Home-page: https://gitcode.net/weixin_62651706/
 tkintertools Author: Xiaokang2022 Author-email: 2951256653@qq.com License:
 MulanPSL-2.0 Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)
 Classifier: Operating System :: OS Independent Description-Content-Type: text/
 markdown License-File: LICENSE
                       ****** ðtkintertoolsð ******
@@ -82,91 +82,93 @@
 3. `Canvas`: ç»å¸ç±»
 ç»§æ¿äº`tkinter.Canvas`ï¼å å¥äºå¯¹ç»å¸èææ§ä»¶çæ¯æï¼åæ¶æ¯åç±»ååºäºä»¶ãç¼©æ¾æ§å¶çç®¡çèï¼ä¹å¯¹`tkinter.Canvas`çå®ä¾æ¹æ³æä¸å®çå¼å®¹æ§
 ### Virtual Canvas Widget/èæç»å¸æ§ä»¶ 1. `Label`: æ ç­¾æ§ä»¶
 æ ç­¾æ§ä»¶çåè½å`tkinter.Label`çåè½ç±»ä¼¼ï¼ä½æ´å çå¤åå
 ä¸é¢æ¯`Label`æ§ä»¶çå¤è§ï¼
 [LabelTest.png]
 æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('LabelTest', 1000,
-400) canvas = tkt.Canvas(root, 1000, 400) def colorful(x, y, width, height): #
-type: (int, int, int, int) -> None """ Gradient colors """ for i in range
-(width): color = tkt.color(('#FF0000', '#0000FF'), i/width) canvas.create_line
-(x+i, y, x+i, y+height, fill=color) colorful(510, 175, 480, 150) tkt.Label
-(canvas, 50, 50, 400, 100, text='NormalLabel\nHere is the text') tkt.Label
-(canvas, 50, 200, 400, 100, radius=20, text='RoundCornerLabel') tkt.Label
-(canvas, 550, 50, 400, 100, text='DisableLabel').set_live(False) tkt.Label
-(canvas, 550, 200, 400, 100, radius=20, text='TransparentLabel',
+400) canvas = tkt.Canvas(root, 1000, 400, 0, 0) def colorful(x, y, width,
+height): # type: (int, int, int, int) -> None """ Gradient colors """ for i in
+range(width): color = tkt.color(('#FF0000', '#0000FF'), i/width)
+canvas.create_line(x+i, y, x+i, y+height, fill=color) colorful(510, 175, 480,
+150) tkt.Label(canvas, 50, 50, 400, 100, text='NormalLabel\nHere is the text')
+tkt.Label(canvas, 50, 200, 400, 100, radius=20, text='RoundCornerLabel')
+tkt.Label(canvas, 550, 50, 400, 100, text='DisableLabel').set_live(False)
+tkt.Label(canvas, 550, 200, 400, 100, radius=20, text='TransparentLabel',
 color_fill=tkt.COLOR_NONE) root.mainloop() ```  2. `Button`: æé®æ§ä»¶
 æé®æ§ä»¶ç¸è¾äº`tkinter.Button`ï¼å¶èªç±åº¦æ´é«ï¼`tkinter.Button`åªæå¨æä¸çæ¶åæè½è§¦åç»å®çå³èäºä»¶ï¼è`Button`å´å¯ä»¥å¨é¼ æ ç§»è³æé®ä¸æ¹æ¶ãé¼ æ æä¸æ¶ãé¼ æ æ¾å¼æ¶é½å¯ä»¥ç»å®å³èäºä»¶
 ä¸é¢æ¯`Button`æ§ä»¶çå¤è§ï¼
 [ButtonTest.png]
 æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('ButtonTest', 500,
-500) canvas = tkt.Canvas(root, 500, 500) def colorful(x, y, width, height): #
-type: (int, int, int, int) -> None """ Gradient colors """ for i in range
-(width): color = tkt.color(('#FF0000', '#0000FF'), i/width) canvas.create_line
-(x+i, y, x+i, y+height, fill=color) colorful(50, 280, 400, 100) tkt.Button
-(canvas, 150, 135, 200, 50, text='NormalButton') tkt.Button(canvas, 100, 195,
-300, 50, radius=10, text='RoundCornerButton') tkt.Button(canvas, 150, 255, 200,
-50, text='DisableButton').set_live(False) tkt.Button(canvas, 100, 315, 300, 50,
-radius=10, text='TransparentButton', color_fill=tkt.COLOR_NONE) root.mainloop()
-```  3. `CheckButton`: å¤éæ¡æ§ä»¶
+500) canvas = tkt.Canvas(root, 500, 500, 0, 0) def colorful(x, y, width,
+height): # type: (int, int, int, int) -> None """ Gradient colors """ for i in
+range(width): color = tkt.color(('#FF0000', '#0000FF'), i/width)
+canvas.create_line(x+i, y, x+i, y+height, fill=color) colorful(50, 280, 400,
+100) tkt.Button(canvas, 150, 135, 200, 50, text='NormalButton') tkt.Button
+(canvas, 100, 195, 300, 50, radius=10, text='RoundCornerButton') tkt.Button
+(canvas, 150, 255, 200, 50, text='DisableButton').set_live(False) tkt.Button
+(canvas, 100, 315, 300, 50, radius=10, text='TransparentButton',
+color_fill=tkt.COLOR_NONE) root.mainloop() ```  3. `CheckButton`:
+å¤éæ¡æ§ä»¶
 å¤éæ¡æ§ä»¶ç¸å¯¹äº`tkinter`åçç`tkinter.CheckButton`å¨ä½¿ç¨æ¹é¢æ´å å°ç®åï¼åæ¶é¢å¼ä¹ä¸åäºä¸å°
 ä¸é¢æ¯`CheckButton`æ§ä»¶çå¤è§ï¼
 [CheckButtonTest.png]
 æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('CheckButtonTest',
-500, 300) canvas = tkt.Canvas(root, 500, 300) def colorful(x, y, width,
+500, 300) canvas = tkt.Canvas(root, 500, 300, 0, 0) def colorful(x, y, width,
 height): # type: (int, int, int, int) -> None """ Gradient colors """ for i in
 range(width): color = tkt.color(('#FF0000', '#0000FF'), i/width)
 canvas.create_line(x+i, y, x+i, y+height, fill=color) colorful(40, 190, 420,
 50) tkt.CheckButton(canvas, 50, 50, 30, text='NormalCheckButton', value=True)
 tkt.CheckButton(canvas, 50, 100, 30, text='DisableCheckButton',
 value=True).set_live(False) tkt.CheckButton(canvas, 50, 150, 30, radius=10,
 text='RoundCornerCheckButton') tkt.CheckButton(canvas, 50, 200, 30, radius=15,
 text='TransparentCheckButton', color_fill=tkt.COLOR_NONE) root.mainloop() ```
 4. `Entry`: è¾å¥æ¡æ§ä»¶
 è¾å¥æ¡æ§ä»¶å¯ä»¥è½»æ¾å°è®¾ç½®è¾å¥çææ¬ä½ç½®ï¼é å·¦ãå±ä¸­åé å³ï¼ï¼åæ¶ï¼å®å¯ä»¥å¨é¼ æ ç§»è³è¾å¥æ¡ä¸æ¹ãé¼ æ æªå¨è¾å¥æ¡ä¸æ¹ä¸¤ç§ç¶ææ¾ç¤ºä¸åçé»è®¤ææ¬
 ä¸é¢æ¯`Entry`æ§ä»¶çå¤è§ï¼
 [EntryTest.png]
 æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('EntryTest', 500,
-400) canvas = tkt.Canvas(root, 500, 400) def colorful(x, y, width, height): #
-type: (int, int, int, int) -> None """ Gradient colors """ for i in range
-(width): color = tkt.color(('#FF0000', '#0000FF'), i/width) canvas.create_line
-(x+i, y, x+i, y+height, fill=color) colorful(50, 193, 400, 100) tkt.Entry
-(canvas, 20, 20, 200, 30, text=('LeftEntry', 'Enter')) tkt.Entry(canvas, 20,
-55, 200, 30, text=( 'CenterEntry', 'Enter'), justify='center') tkt.Entry
-(canvas, 20, 90, 200, 30, text=( 'RightEntry', 'Enter'), justify='right')
-tkt.Entry(canvas, 270, 20, 200, 30, radius=8, text='LeftEntry') tkt.Entry
-(canvas, 270, 55, 200, 30, radius=8, text='CenterEntry', justify='center')
-tkt.Entry(canvas, 270, 90, 200, 30, radius=8, text='RightEntry',
-justify='right') tkt.Entry(canvas, 100, 150, 300, 35, text=('PasswordEntry',
-'Click To Enter'), justify='center', show='â') tkt.Entry(canvas, 100, 200,
-300, 35, text='DisableEntry', justify='center').set_live(False) tkt.Entry
-(canvas, 100, 250, 300, 35, text='TransparentEntry', justify='center',
-color_fill=tkt.COLOR_NONE) root.mainloop() ```  5. `Text`: ææ¬æ¡æ§ä»¶
+400) canvas = tkt.Canvas(root, 500, 400, 0, 0) def colorful(x, y, width,
+height): # type: (int, int, int, int) -> None """ Gradient colors """ for i in
+range(width): color = tkt.color(('#FF0000', '#0000FF'), i/width)
+canvas.create_line(x+i, y, x+i, y+height, fill=color) colorful(50, 193, 400,
+100) tkt.Entry(canvas, 20, 20, 200, 30, text=('LeftEntry', 'Enter')) tkt.Entry
+(canvas, 20, 55, 200, 30, text=( 'CenterEntry', 'Enter'), justify='center')
+tkt.Entry(canvas, 20, 90, 200, 30, text=( 'RightEntry', 'Enter'),
+justify='right') tkt.Entry(canvas, 270, 20, 200, 30, radius=8,
+text='LeftEntry') tkt.Entry(canvas, 270, 55, 200, 30, radius=8,
+text='CenterEntry', justify='center') tkt.Entry(canvas, 270, 90, 200, 30,
+radius=8, text='RightEntry', justify='right') tkt.Entry(canvas, 100, 150, 300,
+35, text=('PasswordEntry', 'Click To Enter'), justify='center', show='â')
+tkt.Entry(canvas, 100, 200, 300, 35, text='DisableEntry',
+justify='center').set_live(False) tkt.Entry(canvas, 100, 250, 300, 35,
+text='TransparentEntry', justify='center', color_fill=tkt.COLOR_NONE)
+root.mainloop() ```  5. `Text`: ææ¬æ¡æ§ä»¶
 ææ¬æ¡ç±»ä¼¼äºè¾å¥æ¡ï¼è¿éå°±ä¸åèµè¿°
 ä¸é¢æ¯`Text`æ§ä»¶çå¤è§ï¼
 [TextTest.png]
 æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('TextTest', 1000,
-400) canvas = tkt.Canvas(root, 1000, 400) def colorful(x, y, width, height) -
-> None: # type: (int, int, int, int) -> None """ Gradient colors """ for i in
-range(width): color = tkt.color(('#FF0000', '#0000FF'), i/width)
+400) canvas = tkt.Canvas(root, 1000, 400, 0, 0) def colorful(x, y, width,
+height) -> None: # type: (int, int, int, int) -> None """ Gradient colors """
+for i in range(width): color = tkt.color(('#FF0000', '#0000FF'), i/width)
 canvas.create_line(x+i, y, x+i, y+height, fill=color) colorful(510, 175, 480,
 150) tkt.Text(canvas, 50, 50, 400, 100, text=('NormalText(Left)', 'Click To
 Enter')) tkt.Text(canvas, 50, 200, 400, 100, radius=20, text='RoundCornerText
 (Center)', justify='center') tkt.Text(canvas, 550, 50, 400, 100,
 text='DisableText').set_live(False) tkt.Text(canvas, 550, 200, 400, 100,
 radius=20, text='TransparentText(Right)', justify='right',
 color_fill=tkt.COLOR_NONE) root.mainloop() ```  6. `Progressbar`:
 è¿åº¦æ¡æ§ä»¶
 è¿åº¦æ¡æ§ä»¶ç¸æ¯`tkinter.ttk.Progressbar`ï¼å¤è§ä¸çèªç±åº¦è¾å¤§
 ä¸é¢æ¯`Progressbar`æ§ä»¶çå¤è§ï¼
 [ProgressbarTest.png]
 æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('ProgressbarTest',
-500, 500) canvas = tkt.Canvas(root, 500, 500) def colorful(x, y, width, height)
--> None: # type: (int, int, int, int) -> None """ Gradient colors """ for i in
-range(width): color = tkt.color(('#FF0000', '#0000FF'), i/width)
+500, 500) canvas = tkt.Canvas(root, 500, 500, 0, 0) def colorful(x, y, width,
+height) -> None: # type: (int, int, int, int) -> None """ Gradient colors """
+for i in range(width): color = tkt.color(('#FF0000', '#0000FF'), i/width)
 canvas.create_line(x+i, y, x+i, y+height, fill=color) colorful(30, 290, 440,
 50) tkt.Progressbar(canvas, 50, 50, 400, 30) tkt.Progressbar(canvas, 50, 100,
 400, 30).load(.6667) tkt.Progressbar(canvas, 50, 150, 400, 30,
 borderwidth=5).load(1) (_ := tkt.Progressbar(canvas, 50, 200, 400, 30)).load
 (0.3333) _.set_live(False) tkt.Progressbar(canvas, 50, 250, 400, 30, color_bar=
 ( 'lightyellow', 'skyblue')).load(.5) tkt.Progressbar(canvas, 50, 300, 400, 30,
 color_bar=('', 'orange')).load(.1667) progressbar = tkt.Progressbar(canvas, 50,
@@ -182,18 +184,18 @@
 ç±»åçå¾ççæ¯æä¹æå¼ºåï¼å¯ä»¥å¨ä¸ä¾èµä»»ä½ç¬¬ä¸æ¹æ¨¡åæèåºçæåµä¸ï¼å¯¹
 png å¾çè¿è¡ç¼©æ¾ 2. `Singleton`: åä¾æ¨¡å¼ç±»
 åä¾æ¨¡å¼ï¼ä¸ç¨ä»ç»äºå§ï¼éè¿ç»§æ¿å®æ¥ä½¿ç¨ ### Tool Function/
 å·¥å·å½æ° 1. `move`: ç§»å¨å½æ°
 ç§»å¨å½æ°å¯ä»¥è½»æ¾å°æä¸å®çè§å¾ãç§»å¨éåº¦ãç§»å¨æ¶é´å»ç§»å¨`tkintertools`æ¨¡ååçææå¯¹è±¡ï¼åæ¶å¼å®¹äº`tkinter`åçå¯¹è±¡ï¼å³`tkinter`ä¸­çå¯¹è±¡ä¹å¯ä»¥å¾æ¹ä¾¿å°ç§»å¨ï¼çè³å®è¿å¯ä»¥ç§»å¨çªå£çä½ç½®ï¼
 [MoveTest.gif]
 æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('MoveTest', 500,
-500) canvas = tkt.Canvas(root, 500, 500) rect = canvas.create_rectangle(50,
-350, 150, 450) def move_window(switch=[True]): # type: (list[bool]) -> None
-tkt.move(root, None, 1000 if switch[0] else -1000, 0, 800, mode='flat') switch
-[0] = not switch[0] def move_button(switch=[True]) -> None: # type: (list
+500) canvas = tkt.Canvas(root, 500, 500, 0, 0) rect = canvas.create_rectangle
+(50, 350, 150, 450) def move_window(switch=[True]): # type: (list[bool]) -
+> None tkt.move(root, None, 1000 if switch[0] else -1000, 0, 800, mode='flat')
+switch[0] = not switch[0] def move_button(switch=[True]) -> None: # type: (list
 [bool]) -> None tkt.move(canvas, button, 200 if switch[0] else -200, 0, 500,
 mode='rebound') switch[0] = not switch[0] def move_rect(switch=[True]): # type:
 (list[bool]) -> None tkt.move(canvas, rect, 200 if switch[0] else -200, 0, 500,
 mode='smooth') switch[0] = not switch[0] tkt.Button(canvas, 50, 50, 200, 40,
 radius=10, text='MoveWindow', command=move_window) tkt.Button(canvas, 50, 100,
 200, 40, radius=10, text='MoveRect', command=move_rect) button = tkt.Button
 (canvas, 50, 150, 200, 40, radius=10, text='MoveButton', command=move_button)
@@ -204,19 +206,19 @@
     `center` : "    tkintertools    "
     `right`  : "        tkintertools"
 3. `color`: é¢è²å½æ°
 é¢è²å½æ°å¯ä»¥è½»æ¾æ±åºä¸ä¸ªé¢è²å°å¦å¤ä¸ä¸ªé¢è²çè¿æ¸¡é¢è²ï¼å æ­¤å¯ä»¥è½»æ¾å¾å°æ¸åè²çææï¼åæ¶ï¼æ¹åä¼ å¥çåæ°è¿å¯ä»¥å¾å°ä¼ å¥é¢è²çå¯¹æ¯è²
 ç¬¬äºå¼ å¾æ¯ test.py å¨å¾åæµè¯ä¸­ç»å¶çå¾æ¡
 [ColorTest.png] [Test_Draw.png]
 æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('ColorTest', 500,
-500) canvas = tkt.Canvas(root, 500, 500) def colorful(x, y, width, height): #
-type: (int, int, int, int) -> None """ Gradient colors """ for i in range
-(width): color = tkt.color(('#FF0000', '#00FF00'), i/width) color_2 = tkt.color
-(('#FFFFFF', '#000000'), i/width) canvas.create_line(x+i, y, x+i, y+height,
-fill=color) canvas.create_oval(250-i/3, 300-i/3, 250+i/3, 300 + i/3,
+500) canvas = tkt.Canvas(root, 500, 500, 0, 0) def colorful(x, y, width,
+height): # type: (int, int, int, int) -> None """ Gradient colors """ for i in
+range(width): color = tkt.color(('#FF0000', '#00FF00'), i/width) color_2 =
+tkt.color(('#FFFFFF', '#000000'), i/width) canvas.create_line(x+i, y, x+i,
+y+height, fill=color) canvas.create_oval(250-i/3, 300-i/3, 250+i/3, 300 + i/3,
 outline=color_2, width=2) colorful(50, 50, 400, 100) root.mainloop() ```  4.
 `askfont`: å­ä½éæ©å¯¹è¯æ¡
 `askfont`å½æ°å¯ä»¥æå¼é»è®¤çå­ä½éæ©çªå£ï¼è¿ä¸ªçªå£è½ç¶æ¯é»è®¤çï¼ä½å®å®éä¸æ æ³å¨`tkinter`ä¸­æå¼ï¼å ä¸º`tkinter`å¹¶æ²¡æå¯¹åºç
 API è½å¤åå°è¿ä¸ç¹ãä½æ¯ï¼`tkintertools`è°ç¨å¹¶å°è£äºåçç
 tcl çå½ä»¤ï¼ä½¿å¾å­ä½éæ©æ¡è½å¤è¢«æä»¬ä½¿ç¨ã
 [font.png]
 5. `SetProcessDpiAwareness`: DPI çº§å«è®¾ç½®å½æ°
```

### Comparing `tkintertools-2.6.1/README.md` & `tkintertools-2.6.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -168,15 +168,15 @@
 
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('LabelTest', 1000, 400)
-    canvas = tkt.Canvas(root, 1000, 400)
+    canvas = tkt.Canvas(root, 1000, 400, 0, 0)
 
 
     def colorful(x, y, width, height):  # type: (int, int, int, int) -> None
         """ Gradient colors """
         for i in range(width):
             color = tkt.color(('#FF0000', '#0000FF'), i/width)
             canvas.create_line(x+i, y, x+i, y+height, fill=color)
@@ -202,15 +202,15 @@
 
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('ButtonTest', 500, 500)
-    canvas = tkt.Canvas(root, 500, 500)
+    canvas = tkt.Canvas(root, 500, 500, 0, 0)
 
 
     def colorful(x, y, width, height):  # type: (int, int, int, int) -> None
         """ Gradient colors """
         for i in range(width):
             color = tkt.color(('#FF0000', '#0000FF'), i/width)
             canvas.create_line(x+i, y, x+i, y+height, fill=color)
@@ -236,15 +236,15 @@
 
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('CheckButtonTest', 500, 300)
-    canvas = tkt.Canvas(root, 500, 300)
+    canvas = tkt.Canvas(root, 500, 300, 0, 0)
 
 
     def colorful(x, y, width, height):  # type: (int, int, int, int) -> None
         """ Gradient colors """
         for i in range(width):
             color = tkt.color(('#FF0000', '#0000FF'), i/width)
             canvas.create_line(x+i, y, x+i, y+height, fill=color)
@@ -271,15 +271,15 @@
     
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('EntryTest', 500, 400)
-    canvas = tkt.Canvas(root, 500, 400)
+    canvas = tkt.Canvas(root, 500, 400, 0, 0)
 
 
     def colorful(x, y, width, height):  # type: (int, int, int, int) -> None
         """ Gradient colors """
         for i in range(width):
             color = tkt.color(('#FF0000', '#0000FF'), i/width)
             canvas.create_line(x+i, y, x+i, y+height, fill=color)
@@ -316,15 +316,15 @@
     
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('TextTest', 1000, 400)
-    canvas = tkt.Canvas(root, 1000, 400)
+    canvas = tkt.Canvas(root, 1000, 400, 0, 0)
 
 
     def colorful(x, y, width, height) -> None:  # type: (int, int, int, int) -> None
         """ Gradient colors """
         for i in range(width):
             color = tkt.color(('#FF0000', '#0000FF'), i/width)
             canvas.create_line(x+i, y, x+i, y+height, fill=color)
@@ -351,15 +351,15 @@
 
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('ProgressbarTest', 500, 500)
-    canvas = tkt.Canvas(root, 500, 500)
+    canvas = tkt.Canvas(root, 500, 500, 0, 0)
 
 
     def colorful(x, y, width, height) -> None:  # type: (int, int, int, int) -> None
         """ Gradient colors """
         for i in range(width):
             color = tkt.color(('#FF0000', '#0000FF'), i/width)
             canvas.create_line(x+i, y, x+i, y+height, fill=color)
@@ -412,15 +412,15 @@
     
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('MoveTest', 500, 500)
-    canvas = tkt.Canvas(root, 500, 500)
+    canvas = tkt.Canvas(root, 500, 500, 0, 0)
     rect = canvas.create_rectangle(50, 350, 150, 450)
 
 
     def move_window(switch=[True]):  # type: (list[bool]) -> None
         tkt.move(root, None, 1000 if switch[0] else -1000, 0, 800, mode='flat')
         switch[0] = not switch[0]
 
@@ -466,15 +466,15 @@
 
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('ColorTest', 500, 500)
-    canvas = tkt.Canvas(root, 500, 500)
+    canvas = tkt.Canvas(root, 500, 500, 0, 0)
 
 
     def colorful(x, y, width, height):  # type: (int, int, int, int) -> None
         """ Gradient colors """
         for i in range(width):
             color = tkt.color(('#FF0000', '#00FF00'), i/width)
             color_2 = tkt.color(('#FFFFFF', '#000000'), i/width)
```

#### html2text {}

```diff
@@ -75,91 +75,93 @@
 3. `Canvas`: ç»å¸ç±»
 ç»§æ¿äº`tkinter.Canvas`ï¼å å¥äºå¯¹ç»å¸èææ§ä»¶çæ¯æï¼åæ¶æ¯åç±»ååºäºä»¶ãç¼©æ¾æ§å¶çç®¡çèï¼ä¹å¯¹`tkinter.Canvas`çå®ä¾æ¹æ³æä¸å®çå¼å®¹æ§
 ### Virtual Canvas Widget/èæç»å¸æ§ä»¶ 1. `Label`: æ ç­¾æ§ä»¶
 æ ç­¾æ§ä»¶çåè½å`tkinter.Label`çåè½ç±»ä¼¼ï¼ä½æ´å çå¤åå
 ä¸é¢æ¯`Label`æ§ä»¶çå¤è§ï¼
 [LabelTest.png]
 æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('LabelTest', 1000,
-400) canvas = tkt.Canvas(root, 1000, 400) def colorful(x, y, width, height): #
-type: (int, int, int, int) -> None """ Gradient colors """ for i in range
-(width): color = tkt.color(('#FF0000', '#0000FF'), i/width) canvas.create_line
-(x+i, y, x+i, y+height, fill=color) colorful(510, 175, 480, 150) tkt.Label
-(canvas, 50, 50, 400, 100, text='NormalLabel\nHere is the text') tkt.Label
-(canvas, 50, 200, 400, 100, radius=20, text='RoundCornerLabel') tkt.Label
-(canvas, 550, 50, 400, 100, text='DisableLabel').set_live(False) tkt.Label
-(canvas, 550, 200, 400, 100, radius=20, text='TransparentLabel',
+400) canvas = tkt.Canvas(root, 1000, 400, 0, 0) def colorful(x, y, width,
+height): # type: (int, int, int, int) -> None """ Gradient colors """ for i in
+range(width): color = tkt.color(('#FF0000', '#0000FF'), i/width)
+canvas.create_line(x+i, y, x+i, y+height, fill=color) colorful(510, 175, 480,
+150) tkt.Label(canvas, 50, 50, 400, 100, text='NormalLabel\nHere is the text')
+tkt.Label(canvas, 50, 200, 400, 100, radius=20, text='RoundCornerLabel')
+tkt.Label(canvas, 550, 50, 400, 100, text='DisableLabel').set_live(False)
+tkt.Label(canvas, 550, 200, 400, 100, radius=20, text='TransparentLabel',
 color_fill=tkt.COLOR_NONE) root.mainloop() ```  2. `Button`: æé®æ§ä»¶
 æé®æ§ä»¶ç¸è¾äº`tkinter.Button`ï¼å¶èªç±åº¦æ´é«ï¼`tkinter.Button`åªæå¨æä¸çæ¶åæè½è§¦åç»å®çå³èäºä»¶ï¼è`Button`å´å¯ä»¥å¨é¼ æ ç§»è³æé®ä¸æ¹æ¶ãé¼ æ æä¸æ¶ãé¼ æ æ¾å¼æ¶é½å¯ä»¥ç»å®å³èäºä»¶
 ä¸é¢æ¯`Button`æ§ä»¶çå¤è§ï¼
 [ButtonTest.png]
 æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('ButtonTest', 500,
-500) canvas = tkt.Canvas(root, 500, 500) def colorful(x, y, width, height): #
-type: (int, int, int, int) -> None """ Gradient colors """ for i in range
-(width): color = tkt.color(('#FF0000', '#0000FF'), i/width) canvas.create_line
-(x+i, y, x+i, y+height, fill=color) colorful(50, 280, 400, 100) tkt.Button
-(canvas, 150, 135, 200, 50, text='NormalButton') tkt.Button(canvas, 100, 195,
-300, 50, radius=10, text='RoundCornerButton') tkt.Button(canvas, 150, 255, 200,
-50, text='DisableButton').set_live(False) tkt.Button(canvas, 100, 315, 300, 50,
-radius=10, text='TransparentButton', color_fill=tkt.COLOR_NONE) root.mainloop()
-```  3. `CheckButton`: å¤éæ¡æ§ä»¶
+500) canvas = tkt.Canvas(root, 500, 500, 0, 0) def colorful(x, y, width,
+height): # type: (int, int, int, int) -> None """ Gradient colors """ for i in
+range(width): color = tkt.color(('#FF0000', '#0000FF'), i/width)
+canvas.create_line(x+i, y, x+i, y+height, fill=color) colorful(50, 280, 400,
+100) tkt.Button(canvas, 150, 135, 200, 50, text='NormalButton') tkt.Button
+(canvas, 100, 195, 300, 50, radius=10, text='RoundCornerButton') tkt.Button
+(canvas, 150, 255, 200, 50, text='DisableButton').set_live(False) tkt.Button
+(canvas, 100, 315, 300, 50, radius=10, text='TransparentButton',
+color_fill=tkt.COLOR_NONE) root.mainloop() ```  3. `CheckButton`:
+å¤éæ¡æ§ä»¶
 å¤éæ¡æ§ä»¶ç¸å¯¹äº`tkinter`åçç`tkinter.CheckButton`å¨ä½¿ç¨æ¹é¢æ´å å°ç®åï¼åæ¶é¢å¼ä¹ä¸åäºä¸å°
 ä¸é¢æ¯`CheckButton`æ§ä»¶çå¤è§ï¼
 [CheckButtonTest.png]
 æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('CheckButtonTest',
-500, 300) canvas = tkt.Canvas(root, 500, 300) def colorful(x, y, width,
+500, 300) canvas = tkt.Canvas(root, 500, 300, 0, 0) def colorful(x, y, width,
 height): # type: (int, int, int, int) -> None """ Gradient colors """ for i in
 range(width): color = tkt.color(('#FF0000', '#0000FF'), i/width)
 canvas.create_line(x+i, y, x+i, y+height, fill=color) colorful(40, 190, 420,
 50) tkt.CheckButton(canvas, 50, 50, 30, text='NormalCheckButton', value=True)
 tkt.CheckButton(canvas, 50, 100, 30, text='DisableCheckButton',
 value=True).set_live(False) tkt.CheckButton(canvas, 50, 150, 30, radius=10,
 text='RoundCornerCheckButton') tkt.CheckButton(canvas, 50, 200, 30, radius=15,
 text='TransparentCheckButton', color_fill=tkt.COLOR_NONE) root.mainloop() ```
 4. `Entry`: è¾å¥æ¡æ§ä»¶
 è¾å¥æ¡æ§ä»¶å¯ä»¥è½»æ¾å°è®¾ç½®è¾å¥çææ¬ä½ç½®ï¼é å·¦ãå±ä¸­åé å³ï¼ï¼åæ¶ï¼å®å¯ä»¥å¨é¼ æ ç§»è³è¾å¥æ¡ä¸æ¹ãé¼ æ æªå¨è¾å¥æ¡ä¸æ¹ä¸¤ç§ç¶ææ¾ç¤ºä¸åçé»è®¤ææ¬
 ä¸é¢æ¯`Entry`æ§ä»¶çå¤è§ï¼
 [EntryTest.png]
 æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('EntryTest', 500,
-400) canvas = tkt.Canvas(root, 500, 400) def colorful(x, y, width, height): #
-type: (int, int, int, int) -> None """ Gradient colors """ for i in range
-(width): color = tkt.color(('#FF0000', '#0000FF'), i/width) canvas.create_line
-(x+i, y, x+i, y+height, fill=color) colorful(50, 193, 400, 100) tkt.Entry
-(canvas, 20, 20, 200, 30, text=('LeftEntry', 'Enter')) tkt.Entry(canvas, 20,
-55, 200, 30, text=( 'CenterEntry', 'Enter'), justify='center') tkt.Entry
-(canvas, 20, 90, 200, 30, text=( 'RightEntry', 'Enter'), justify='right')
-tkt.Entry(canvas, 270, 20, 200, 30, radius=8, text='LeftEntry') tkt.Entry
-(canvas, 270, 55, 200, 30, radius=8, text='CenterEntry', justify='center')
-tkt.Entry(canvas, 270, 90, 200, 30, radius=8, text='RightEntry',
-justify='right') tkt.Entry(canvas, 100, 150, 300, 35, text=('PasswordEntry',
-'Click To Enter'), justify='center', show='â') tkt.Entry(canvas, 100, 200,
-300, 35, text='DisableEntry', justify='center').set_live(False) tkt.Entry
-(canvas, 100, 250, 300, 35, text='TransparentEntry', justify='center',
-color_fill=tkt.COLOR_NONE) root.mainloop() ```  5. `Text`: ææ¬æ¡æ§ä»¶
+400) canvas = tkt.Canvas(root, 500, 400, 0, 0) def colorful(x, y, width,
+height): # type: (int, int, int, int) -> None """ Gradient colors """ for i in
+range(width): color = tkt.color(('#FF0000', '#0000FF'), i/width)
+canvas.create_line(x+i, y, x+i, y+height, fill=color) colorful(50, 193, 400,
+100) tkt.Entry(canvas, 20, 20, 200, 30, text=('LeftEntry', 'Enter')) tkt.Entry
+(canvas, 20, 55, 200, 30, text=( 'CenterEntry', 'Enter'), justify='center')
+tkt.Entry(canvas, 20, 90, 200, 30, text=( 'RightEntry', 'Enter'),
+justify='right') tkt.Entry(canvas, 270, 20, 200, 30, radius=8,
+text='LeftEntry') tkt.Entry(canvas, 270, 55, 200, 30, radius=8,
+text='CenterEntry', justify='center') tkt.Entry(canvas, 270, 90, 200, 30,
+radius=8, text='RightEntry', justify='right') tkt.Entry(canvas, 100, 150, 300,
+35, text=('PasswordEntry', 'Click To Enter'), justify='center', show='â')
+tkt.Entry(canvas, 100, 200, 300, 35, text='DisableEntry',
+justify='center').set_live(False) tkt.Entry(canvas, 100, 250, 300, 35,
+text='TransparentEntry', justify='center', color_fill=tkt.COLOR_NONE)
+root.mainloop() ```  5. `Text`: ææ¬æ¡æ§ä»¶
 ææ¬æ¡ç±»ä¼¼äºè¾å¥æ¡ï¼è¿éå°±ä¸åèµè¿°
 ä¸é¢æ¯`Text`æ§ä»¶çå¤è§ï¼
 [TextTest.png]
 æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('TextTest', 1000,
-400) canvas = tkt.Canvas(root, 1000, 400) def colorful(x, y, width, height) -
-> None: # type: (int, int, int, int) -> None """ Gradient colors """ for i in
-range(width): color = tkt.color(('#FF0000', '#0000FF'), i/width)
+400) canvas = tkt.Canvas(root, 1000, 400, 0, 0) def colorful(x, y, width,
+height) -> None: # type: (int, int, int, int) -> None """ Gradient colors """
+for i in range(width): color = tkt.color(('#FF0000', '#0000FF'), i/width)
 canvas.create_line(x+i, y, x+i, y+height, fill=color) colorful(510, 175, 480,
 150) tkt.Text(canvas, 50, 50, 400, 100, text=('NormalText(Left)', 'Click To
 Enter')) tkt.Text(canvas, 50, 200, 400, 100, radius=20, text='RoundCornerText
 (Center)', justify='center') tkt.Text(canvas, 550, 50, 400, 100,
 text='DisableText').set_live(False) tkt.Text(canvas, 550, 200, 400, 100,
 radius=20, text='TransparentText(Right)', justify='right',
 color_fill=tkt.COLOR_NONE) root.mainloop() ```  6. `Progressbar`:
 è¿åº¦æ¡æ§ä»¶
 è¿åº¦æ¡æ§ä»¶ç¸æ¯`tkinter.ttk.Progressbar`ï¼å¤è§ä¸çèªç±åº¦è¾å¤§
 ä¸é¢æ¯`Progressbar`æ§ä»¶çå¤è§ï¼
 [ProgressbarTest.png]
 æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('ProgressbarTest',
-500, 500) canvas = tkt.Canvas(root, 500, 500) def colorful(x, y, width, height)
--> None: # type: (int, int, int, int) -> None """ Gradient colors """ for i in
-range(width): color = tkt.color(('#FF0000', '#0000FF'), i/width)
+500, 500) canvas = tkt.Canvas(root, 500, 500, 0, 0) def colorful(x, y, width,
+height) -> None: # type: (int, int, int, int) -> None """ Gradient colors """
+for i in range(width): color = tkt.color(('#FF0000', '#0000FF'), i/width)
 canvas.create_line(x+i, y, x+i, y+height, fill=color) colorful(30, 290, 440,
 50) tkt.Progressbar(canvas, 50, 50, 400, 30) tkt.Progressbar(canvas, 50, 100,
 400, 30).load(.6667) tkt.Progressbar(canvas, 50, 150, 400, 30,
 borderwidth=5).load(1) (_ := tkt.Progressbar(canvas, 50, 200, 400, 30)).load
 (0.3333) _.set_live(False) tkt.Progressbar(canvas, 50, 250, 400, 30, color_bar=
 ( 'lightyellow', 'skyblue')).load(.5) tkt.Progressbar(canvas, 50, 300, 400, 30,
 color_bar=('', 'orange')).load(.1667) progressbar = tkt.Progressbar(canvas, 50,
@@ -175,18 +177,18 @@
 ç±»åçå¾ççæ¯æä¹æå¼ºåï¼å¯ä»¥å¨ä¸ä¾èµä»»ä½ç¬¬ä¸æ¹æ¨¡åæèåºçæåµä¸ï¼å¯¹
 png å¾çè¿è¡ç¼©æ¾ 2. `Singleton`: åä¾æ¨¡å¼ç±»
 åä¾æ¨¡å¼ï¼ä¸ç¨ä»ç»äºå§ï¼éè¿ç»§æ¿å®æ¥ä½¿ç¨ ### Tool Function/
 å·¥å·å½æ° 1. `move`: ç§»å¨å½æ°
 ç§»å¨å½æ°å¯ä»¥è½»æ¾å°æä¸å®çè§å¾ãç§»å¨éåº¦ãç§»å¨æ¶é´å»ç§»å¨`tkintertools`æ¨¡ååçææå¯¹è±¡ï¼åæ¶å¼å®¹äº`tkinter`åçå¯¹è±¡ï¼å³`tkinter`ä¸­çå¯¹è±¡ä¹å¯ä»¥å¾æ¹ä¾¿å°ç§»å¨ï¼çè³å®è¿å¯ä»¥ç§»å¨çªå£çä½ç½®ï¼
 [MoveTest.gif]
 æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('MoveTest', 500,
-500) canvas = tkt.Canvas(root, 500, 500) rect = canvas.create_rectangle(50,
-350, 150, 450) def move_window(switch=[True]): # type: (list[bool]) -> None
-tkt.move(root, None, 1000 if switch[0] else -1000, 0, 800, mode='flat') switch
-[0] = not switch[0] def move_button(switch=[True]) -> None: # type: (list
+500) canvas = tkt.Canvas(root, 500, 500, 0, 0) rect = canvas.create_rectangle
+(50, 350, 150, 450) def move_window(switch=[True]): # type: (list[bool]) -
+> None tkt.move(root, None, 1000 if switch[0] else -1000, 0, 800, mode='flat')
+switch[0] = not switch[0] def move_button(switch=[True]) -> None: # type: (list
 [bool]) -> None tkt.move(canvas, button, 200 if switch[0] else -200, 0, 500,
 mode='rebound') switch[0] = not switch[0] def move_rect(switch=[True]): # type:
 (list[bool]) -> None tkt.move(canvas, rect, 200 if switch[0] else -200, 0, 500,
 mode='smooth') switch[0] = not switch[0] tkt.Button(canvas, 50, 50, 200, 40,
 radius=10, text='MoveWindow', command=move_window) tkt.Button(canvas, 50, 100,
 200, 40, radius=10, text='MoveRect', command=move_rect) button = tkt.Button
 (canvas, 50, 150, 200, 40, radius=10, text='MoveButton', command=move_button)
@@ -197,19 +199,19 @@
     `center` : "    tkintertools    "
     `right`  : "        tkintertools"
 3. `color`: é¢è²å½æ°
 é¢è²å½æ°å¯ä»¥è½»æ¾æ±åºä¸ä¸ªé¢è²å°å¦å¤ä¸ä¸ªé¢è²çè¿æ¸¡é¢è²ï¼å æ­¤å¯ä»¥è½»æ¾å¾å°æ¸åè²çææï¼åæ¶ï¼æ¹åä¼ å¥çåæ°è¿å¯ä»¥å¾å°ä¼ å¥é¢è²çå¯¹æ¯è²
 ç¬¬äºå¼ å¾æ¯ test.py å¨å¾åæµè¯ä¸­ç»å¶çå¾æ¡
 [ColorTest.png] [Test_Draw.png]
 æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('ColorTest', 500,
-500) canvas = tkt.Canvas(root, 500, 500) def colorful(x, y, width, height): #
-type: (int, int, int, int) -> None """ Gradient colors """ for i in range
-(width): color = tkt.color(('#FF0000', '#00FF00'), i/width) color_2 = tkt.color
-(('#FFFFFF', '#000000'), i/width) canvas.create_line(x+i, y, x+i, y+height,
-fill=color) canvas.create_oval(250-i/3, 300-i/3, 250+i/3, 300 + i/3,
+500) canvas = tkt.Canvas(root, 500, 500, 0, 0) def colorful(x, y, width,
+height): # type: (int, int, int, int) -> None """ Gradient colors """ for i in
+range(width): color = tkt.color(('#FF0000', '#00FF00'), i/width) color_2 =
+tkt.color(('#FFFFFF', '#000000'), i/width) canvas.create_line(x+i, y, x+i,
+y+height, fill=color) canvas.create_oval(250-i/3, 300-i/3, 250+i/3, 300 + i/3,
 outline=color_2, width=2) colorful(50, 50, 400, 100) root.mainloop() ```  4.
 `askfont`: å­ä½éæ©å¯¹è¯æ¡
 `askfont`å½æ°å¯ä»¥æå¼é»è®¤çå­ä½éæ©çªå£ï¼è¿ä¸ªçªå£è½ç¶æ¯é»è®¤çï¼ä½å®å®éä¸æ æ³å¨`tkinter`ä¸­æå¼ï¼å ä¸º`tkinter`å¹¶æ²¡æå¯¹åºç
 API è½å¤åå°è¿ä¸ç¹ãä½æ¯ï¼`tkintertools`è°ç¨å¹¶å°è£äºåçç
 tcl çå½ä»¤ï¼ä½¿å¾å­ä½éæ©æ¡è½å¤è¢«æä»¬ä½¿ç¨ã
 [font.png]
 5. `SetProcessDpiAwareness`: DPI çº§å«è®¾ç½®å½æ°
```

### Comparing `tkintertools-2.6.1/setup.py` & `tkintertools-2.6.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """ 上传 pypi """
 
 import setuptools
 
 
 setuptools.setup(
     name='tkintertools',
-    version="2.6.1",
+    version="2.6.1.1",
     author='Xiaokang2022',
     license='MulanPSL-2.0',
     author_email='2951256653@qq.com',
     description='An auxiliary module of the tkinder module',
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     url='https://gitcode.net/weixin_62651706/tkintertools',
```

### Comparing `tkintertools-2.6.1/tkintertools/__init__.py` & `tkintertools-2.6.1.1/tkintertools/__init__.py`

 * *Files identical despite different names*

### Comparing `tkintertools-2.6.1/tkintertools/__main__.py` & `tkintertools-2.6.1.1/tkintertools/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
             tkinter.Tk.__init__(self, **kw)
 
         self.width = [100, 1]  # type: list[int]  # [初始宽度, 当前宽度]
         self.height = [100, 1]  # type: list[int]  # [初始高度, 当前高度]
         self._canvas = []  # type: list[Canvas]  # 子画布列表
 
         if width and height:
-            if x != None and y != None:  # BUG: 可能需要修改
+            if x is not None and y is not None:  # BUG: 可能需要修改
                 self.geometry('%dx%d+%d+%d' % (width, height, x, y))
             else:
                 self.geometry('%dx%d' % (width, height))
 
         self.title(title if title else None)
         self.protocol('WM_DELETE_WINDOW', shutdown if shutdown else None)
         self.bind('<Configure>', lambda _: self.__zoom())  # 开启窗口缩放检测
@@ -142,16 +142,16 @@
     """ 用于承载虚拟的画布控件，并处理部分绑定事件 """
 
     def __init__(
         self,
         master,  # type: Tk | Toplevel
         width,  # type: int
         height,  # type: int
-        x=0,  # type: int
-        y=0,  # type: int
+        x=None,  # type: int | None
+        y=None,  # type: int | None
         *,
         lock=True,  # type: bool
         expand=True,  # type: bool
         keep=False,  # type: bool
         **kw
     ):  # type: (...) -> None
         """
@@ -183,15 +183,16 @@
             self, master, width=width, height=height, highlightthickness=0, **kw)
 
         if not (kw.get('bg', None) or kw.get('background', None)):
             # Linux 系统上背景默认值不是 #F1F1F1，影响模块默认值的效果
             self.configure(bg=BACKGROUND)
 
         master._canvas.append(self)  # 将实例添加到 Tk 的画布列表中
-        self.place(x=x, y=y)
+        if x and y:
+            self.place(x=x, y=y)
 
         self.bind('<Motion>', self.__touch)  # 绑定鼠标触碰控件
         self.bind('<Any-Key>', self.__input)  # 绑定键盘输入字符（和Ctrl+v的代码顺序不可错）
         self.bind('<Button-1>', self.__click)  # 绑定鼠标左键按下
         self.bind('<B1-Motion>', self.__click)  # 绑定鼠标左键按下移动
         self.bind('<MouseWheel>', self.__mousewheel)  # 绑定鼠标滚轮滚动
         self.bind('<ButtonRelease-1>', self.__release)  # 绑定鼠标左键松开
@@ -515,15 +516,16 @@
 
         if type(font) != str:
             font = list(font)
             font[1] = int(font[1]*math.sqrt(canvas.rx*canvas.ry))
             canvas._font[self.text][1] = font[1]
             canvas.itemconfigure(self.text, font=font)
 
-    def state(self, mode=None):  # type: (Literal['normal', 'touch', 'click', 'disabled'] | None) -> None
+    # type: (Literal['normal', 'touch', 'click', 'disabled'] | None) -> None
+    def state(self, mode=None):
         """
         mode 参数为 None 时仅更新控件，否则改变虚拟控件的外观\n
         ---
         `normal`: 正常状态\n
         `touch`: 鼠标触碰时的状态\n
         `click`: 鼠标按下时的状态\n
         `disabled`: 禁用状态\n
@@ -622,27 +624,27 @@
                 return getattr(self, args[0])
 
         value = kw.get('text', None)
         text = kw.get('color_text', None)
         fill = kw.get('color_fill', None)
         outline = kw.get('color_outline', None)
 
-        if value != None:
+        if value is not None:
             if isinstance(self, CheckButton):
                 self.master.itemconfigure(self._text, text=value)
             else:
                 self.value = value
         if text:
             self.color_text = text
         if fill:
             self.color_fill = fill
         if outline:
             self.color_outline = outline
 
-        if isinstance(self, (Label, Button, Progressbar)) and value != None and not isinstance(self, CheckButton):
+        if isinstance(self, (Label, Button, Progressbar)) and value is not None and not isinstance(self, CheckButton):
             self.master.itemconfigure(self.text, text=value)
 
     def destroy(self):  # type: () -> None
         """ 摧毁控件释放内存 """
         self.live = False
         self.master._widget.remove(self)
 
@@ -1304,15 +1306,15 @@
         ### 缩放图片
         不会缩放该图片对象本身，只是返回一个缩放后的图片对象\n
         ---
         `rate_x`: 横向缩放倍率\n
         `rate_y`: 纵向缩放倍率\n
         `precision`: 精度到小数点后的位数（推荐 1.2），越大运算就越慢（默认值代表绝对精确）\n
         """
-        if precision != None:
+        if precision is not None:
             limit = round(10**precision)
             rate_x = Fraction(str(rate_x)).limit_denominator(limit)
             rate_y = Fraction(str(rate_y)).limit_denominator(limit)
             image = tkinter.PhotoImage.zoom(
                 self, rate_x.numerator, rate_y.numerator)
             image = image.subsample(rate_x.denominator, rate_y.denominator)
         else:
```

### Comparing `tkintertools-2.6.1/tkintertools/constants.py` & `tkintertools-2.6.1.1/tkintertools/constants.py`

 * *Files identical despite different names*

### Comparing `tkintertools-2.6.1/tkintertools/md.py` & `tkintertools-2.6.1.1/tkintertools/md.py`

 * *Files identical despite different names*

### Comparing `tkintertools-2.6.1/tkintertools.egg-info/PKG-INFO` & `tkintertools-2.6.1.1/tkintertools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tkintertools
-Version: 2.6.1
+Version: 2.6.1.1
 Summary: An auxiliary module of the tkinder module
 Home-page: https://gitcode.net/weixin_62651706/tkintertools
 Author: Xiaokang2022
 Author-email: 2951256653@qq.com
 License: MulanPSL-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)
@@ -182,15 +182,15 @@
 
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('LabelTest', 1000, 400)
-    canvas = tkt.Canvas(root, 1000, 400)
+    canvas = tkt.Canvas(root, 1000, 400, 0, 0)
 
 
     def colorful(x, y, width, height):  # type: (int, int, int, int) -> None
         """ Gradient colors """
         for i in range(width):
             color = tkt.color(('#FF0000', '#0000FF'), i/width)
             canvas.create_line(x+i, y, x+i, y+height, fill=color)
@@ -216,15 +216,15 @@
 
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('ButtonTest', 500, 500)
-    canvas = tkt.Canvas(root, 500, 500)
+    canvas = tkt.Canvas(root, 500, 500, 0, 0)
 
 
     def colorful(x, y, width, height):  # type: (int, int, int, int) -> None
         """ Gradient colors """
         for i in range(width):
             color = tkt.color(('#FF0000', '#0000FF'), i/width)
             canvas.create_line(x+i, y, x+i, y+height, fill=color)
@@ -250,15 +250,15 @@
 
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('CheckButtonTest', 500, 300)
-    canvas = tkt.Canvas(root, 500, 300)
+    canvas = tkt.Canvas(root, 500, 300, 0, 0)
 
 
     def colorful(x, y, width, height):  # type: (int, int, int, int) -> None
         """ Gradient colors """
         for i in range(width):
             color = tkt.color(('#FF0000', '#0000FF'), i/width)
             canvas.create_line(x+i, y, x+i, y+height, fill=color)
@@ -285,15 +285,15 @@
     
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('EntryTest', 500, 400)
-    canvas = tkt.Canvas(root, 500, 400)
+    canvas = tkt.Canvas(root, 500, 400, 0, 0)
 
 
     def colorful(x, y, width, height):  # type: (int, int, int, int) -> None
         """ Gradient colors """
         for i in range(width):
             color = tkt.color(('#FF0000', '#0000FF'), i/width)
             canvas.create_line(x+i, y, x+i, y+height, fill=color)
@@ -330,15 +330,15 @@
     
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('TextTest', 1000, 400)
-    canvas = tkt.Canvas(root, 1000, 400)
+    canvas = tkt.Canvas(root, 1000, 400, 0, 0)
 
 
     def colorful(x, y, width, height) -> None:  # type: (int, int, int, int) -> None
         """ Gradient colors """
         for i in range(width):
             color = tkt.color(('#FF0000', '#0000FF'), i/width)
             canvas.create_line(x+i, y, x+i, y+height, fill=color)
@@ -365,15 +365,15 @@
 
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('ProgressbarTest', 500, 500)
-    canvas = tkt.Canvas(root, 500, 500)
+    canvas = tkt.Canvas(root, 500, 500, 0, 0)
 
 
     def colorful(x, y, width, height) -> None:  # type: (int, int, int, int) -> None
         """ Gradient colors """
         for i in range(width):
             color = tkt.color(('#FF0000', '#0000FF'), i/width)
             canvas.create_line(x+i, y, x+i, y+height, fill=color)
@@ -426,15 +426,15 @@
     
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('MoveTest', 500, 500)
-    canvas = tkt.Canvas(root, 500, 500)
+    canvas = tkt.Canvas(root, 500, 500, 0, 0)
     rect = canvas.create_rectangle(50, 350, 150, 450)
 
 
     def move_window(switch=[True]):  # type: (list[bool]) -> None
         tkt.move(root, None, 1000 if switch[0] else -1000, 0, 800, mode='flat')
         switch[0] = not switch[0]
 
@@ -480,15 +480,15 @@
 
     <details><summary><b>源代码</b></summary>
 
     ```python
     import tkintertools as tkt
 
     root = tkt.Tk('ColorTest', 500, 500)
-    canvas = tkt.Canvas(root, 500, 500)
+    canvas = tkt.Canvas(root, 500, 500, 0, 0)
 
 
     def colorful(x, y, width, height):  # type: (int, int, int, int) -> None
         """ Gradient colors """
         for i in range(width):
             color = tkt.color(('#FF0000', '#00FF00'), i/width)
             color_2 = tkt.color(('#FFFFFF', '#000000'), i/width)
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: tkintertools Version: 2.6.1 Summary: An auxiliary
+Metadata-Version: 2.1 Name: tkintertools Version: 2.6.1.1 Summary: An auxiliary
 module of the tkinder module Home-page: https://gitcode.net/weixin_62651706/
 tkintertools Author: Xiaokang2022 Author-email: 2951256653@qq.com License:
 MulanPSL-2.0 Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)
 Classifier: Operating System :: OS Independent Description-Content-Type: text/
 markdown License-File: LICENSE
                       ****** ðtkintertoolsð ******
@@ -82,91 +82,93 @@
 3. `Canvas`: ç»å¸ç±»
 ç»§æ¿äº`tkinter.Canvas`ï¼å å¥äºå¯¹ç»å¸èææ§ä»¶çæ¯æï¼åæ¶æ¯åç±»ååºäºä»¶ãç¼©æ¾æ§å¶çç®¡çèï¼ä¹å¯¹`tkinter.Canvas`çå®ä¾æ¹æ³æä¸å®çå¼å®¹æ§
 ### Virtual Canvas Widget/èæç»å¸æ§ä»¶ 1. `Label`: æ ç­¾æ§ä»¶
 æ ç­¾æ§ä»¶çåè½å`tkinter.Label`çåè½ç±»ä¼¼ï¼ä½æ´å çå¤åå
 ä¸é¢æ¯`Label`æ§ä»¶çå¤è§ï¼
 [LabelTest.png]
 æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('LabelTest', 1000,
-400) canvas = tkt.Canvas(root, 1000, 400) def colorful(x, y, width, height): #
-type: (int, int, int, int) -> None """ Gradient colors """ for i in range
-(width): color = tkt.color(('#FF0000', '#0000FF'), i/width) canvas.create_line
-(x+i, y, x+i, y+height, fill=color) colorful(510, 175, 480, 150) tkt.Label
-(canvas, 50, 50, 400, 100, text='NormalLabel\nHere is the text') tkt.Label
-(canvas, 50, 200, 400, 100, radius=20, text='RoundCornerLabel') tkt.Label
-(canvas, 550, 50, 400, 100, text='DisableLabel').set_live(False) tkt.Label
-(canvas, 550, 200, 400, 100, radius=20, text='TransparentLabel',
+400) canvas = tkt.Canvas(root, 1000, 400, 0, 0) def colorful(x, y, width,
+height): # type: (int, int, int, int) -> None """ Gradient colors """ for i in
+range(width): color = tkt.color(('#FF0000', '#0000FF'), i/width)
+canvas.create_line(x+i, y, x+i, y+height, fill=color) colorful(510, 175, 480,
+150) tkt.Label(canvas, 50, 50, 400, 100, text='NormalLabel\nHere is the text')
+tkt.Label(canvas, 50, 200, 400, 100, radius=20, text='RoundCornerLabel')
+tkt.Label(canvas, 550, 50, 400, 100, text='DisableLabel').set_live(False)
+tkt.Label(canvas, 550, 200, 400, 100, radius=20, text='TransparentLabel',
 color_fill=tkt.COLOR_NONE) root.mainloop() ```  2. `Button`: æé®æ§ä»¶
 æé®æ§ä»¶ç¸è¾äº`tkinter.Button`ï¼å¶èªç±åº¦æ´é«ï¼`tkinter.Button`åªæå¨æä¸çæ¶åæè½è§¦åç»å®çå³èäºä»¶ï¼è`Button`å´å¯ä»¥å¨é¼ æ ç§»è³æé®ä¸æ¹æ¶ãé¼ æ æä¸æ¶ãé¼ æ æ¾å¼æ¶é½å¯ä»¥ç»å®å³èäºä»¶
 ä¸é¢æ¯`Button`æ§ä»¶çå¤è§ï¼
 [ButtonTest.png]
 æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('ButtonTest', 500,
-500) canvas = tkt.Canvas(root, 500, 500) def colorful(x, y, width, height): #
-type: (int, int, int, int) -> None """ Gradient colors """ for i in range
-(width): color = tkt.color(('#FF0000', '#0000FF'), i/width) canvas.create_line
-(x+i, y, x+i, y+height, fill=color) colorful(50, 280, 400, 100) tkt.Button
-(canvas, 150, 135, 200, 50, text='NormalButton') tkt.Button(canvas, 100, 195,
-300, 50, radius=10, text='RoundCornerButton') tkt.Button(canvas, 150, 255, 200,
-50, text='DisableButton').set_live(False) tkt.Button(canvas, 100, 315, 300, 50,
-radius=10, text='TransparentButton', color_fill=tkt.COLOR_NONE) root.mainloop()
-```  3. `CheckButton`: å¤éæ¡æ§ä»¶
+500) canvas = tkt.Canvas(root, 500, 500, 0, 0) def colorful(x, y, width,
+height): # type: (int, int, int, int) -> None """ Gradient colors """ for i in
+range(width): color = tkt.color(('#FF0000', '#0000FF'), i/width)
+canvas.create_line(x+i, y, x+i, y+height, fill=color) colorful(50, 280, 400,
+100) tkt.Button(canvas, 150, 135, 200, 50, text='NormalButton') tkt.Button
+(canvas, 100, 195, 300, 50, radius=10, text='RoundCornerButton') tkt.Button
+(canvas, 150, 255, 200, 50, text='DisableButton').set_live(False) tkt.Button
+(canvas, 100, 315, 300, 50, radius=10, text='TransparentButton',
+color_fill=tkt.COLOR_NONE) root.mainloop() ```  3. `CheckButton`:
+å¤éæ¡æ§ä»¶
 å¤éæ¡æ§ä»¶ç¸å¯¹äº`tkinter`åçç`tkinter.CheckButton`å¨ä½¿ç¨æ¹é¢æ´å å°ç®åï¼åæ¶é¢å¼ä¹ä¸åäºä¸å°
 ä¸é¢æ¯`CheckButton`æ§ä»¶çå¤è§ï¼
 [CheckButtonTest.png]
 æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('CheckButtonTest',
-500, 300) canvas = tkt.Canvas(root, 500, 300) def colorful(x, y, width,
+500, 300) canvas = tkt.Canvas(root, 500, 300, 0, 0) def colorful(x, y, width,
 height): # type: (int, int, int, int) -> None """ Gradient colors """ for i in
 range(width): color = tkt.color(('#FF0000', '#0000FF'), i/width)
 canvas.create_line(x+i, y, x+i, y+height, fill=color) colorful(40, 190, 420,
 50) tkt.CheckButton(canvas, 50, 50, 30, text='NormalCheckButton', value=True)
 tkt.CheckButton(canvas, 50, 100, 30, text='DisableCheckButton',
 value=True).set_live(False) tkt.CheckButton(canvas, 50, 150, 30, radius=10,
 text='RoundCornerCheckButton') tkt.CheckButton(canvas, 50, 200, 30, radius=15,
 text='TransparentCheckButton', color_fill=tkt.COLOR_NONE) root.mainloop() ```
 4. `Entry`: è¾å¥æ¡æ§ä»¶
 è¾å¥æ¡æ§ä»¶å¯ä»¥è½»æ¾å°è®¾ç½®è¾å¥çææ¬ä½ç½®ï¼é å·¦ãå±ä¸­åé å³ï¼ï¼åæ¶ï¼å®å¯ä»¥å¨é¼ æ ç§»è³è¾å¥æ¡ä¸æ¹ãé¼ æ æªå¨è¾å¥æ¡ä¸æ¹ä¸¤ç§ç¶ææ¾ç¤ºä¸åçé»è®¤ææ¬
 ä¸é¢æ¯`Entry`æ§ä»¶çå¤è§ï¼
 [EntryTest.png]
 æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('EntryTest', 500,
-400) canvas = tkt.Canvas(root, 500, 400) def colorful(x, y, width, height): #
-type: (int, int, int, int) -> None """ Gradient colors """ for i in range
-(width): color = tkt.color(('#FF0000', '#0000FF'), i/width) canvas.create_line
-(x+i, y, x+i, y+height, fill=color) colorful(50, 193, 400, 100) tkt.Entry
-(canvas, 20, 20, 200, 30, text=('LeftEntry', 'Enter')) tkt.Entry(canvas, 20,
-55, 200, 30, text=( 'CenterEntry', 'Enter'), justify='center') tkt.Entry
-(canvas, 20, 90, 200, 30, text=( 'RightEntry', 'Enter'), justify='right')
-tkt.Entry(canvas, 270, 20, 200, 30, radius=8, text='LeftEntry') tkt.Entry
-(canvas, 270, 55, 200, 30, radius=8, text='CenterEntry', justify='center')
-tkt.Entry(canvas, 270, 90, 200, 30, radius=8, text='RightEntry',
-justify='right') tkt.Entry(canvas, 100, 150, 300, 35, text=('PasswordEntry',
-'Click To Enter'), justify='center', show='â') tkt.Entry(canvas, 100, 200,
-300, 35, text='DisableEntry', justify='center').set_live(False) tkt.Entry
-(canvas, 100, 250, 300, 35, text='TransparentEntry', justify='center',
-color_fill=tkt.COLOR_NONE) root.mainloop() ```  5. `Text`: ææ¬æ¡æ§ä»¶
+400) canvas = tkt.Canvas(root, 500, 400, 0, 0) def colorful(x, y, width,
+height): # type: (int, int, int, int) -> None """ Gradient colors """ for i in
+range(width): color = tkt.color(('#FF0000', '#0000FF'), i/width)
+canvas.create_line(x+i, y, x+i, y+height, fill=color) colorful(50, 193, 400,
+100) tkt.Entry(canvas, 20, 20, 200, 30, text=('LeftEntry', 'Enter')) tkt.Entry
+(canvas, 20, 55, 200, 30, text=( 'CenterEntry', 'Enter'), justify='center')
+tkt.Entry(canvas, 20, 90, 200, 30, text=( 'RightEntry', 'Enter'),
+justify='right') tkt.Entry(canvas, 270, 20, 200, 30, radius=8,
+text='LeftEntry') tkt.Entry(canvas, 270, 55, 200, 30, radius=8,
+text='CenterEntry', justify='center') tkt.Entry(canvas, 270, 90, 200, 30,
+radius=8, text='RightEntry', justify='right') tkt.Entry(canvas, 100, 150, 300,
+35, text=('PasswordEntry', 'Click To Enter'), justify='center', show='â')
+tkt.Entry(canvas, 100, 200, 300, 35, text='DisableEntry',
+justify='center').set_live(False) tkt.Entry(canvas, 100, 250, 300, 35,
+text='TransparentEntry', justify='center', color_fill=tkt.COLOR_NONE)
+root.mainloop() ```  5. `Text`: ææ¬æ¡æ§ä»¶
 ææ¬æ¡ç±»ä¼¼äºè¾å¥æ¡ï¼è¿éå°±ä¸åèµè¿°
 ä¸é¢æ¯`Text`æ§ä»¶çå¤è§ï¼
 [TextTest.png]
 æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('TextTest', 1000,
-400) canvas = tkt.Canvas(root, 1000, 400) def colorful(x, y, width, height) -
-> None: # type: (int, int, int, int) -> None """ Gradient colors """ for i in
-range(width): color = tkt.color(('#FF0000', '#0000FF'), i/width)
+400) canvas = tkt.Canvas(root, 1000, 400, 0, 0) def colorful(x, y, width,
+height) -> None: # type: (int, int, int, int) -> None """ Gradient colors """
+for i in range(width): color = tkt.color(('#FF0000', '#0000FF'), i/width)
 canvas.create_line(x+i, y, x+i, y+height, fill=color) colorful(510, 175, 480,
 150) tkt.Text(canvas, 50, 50, 400, 100, text=('NormalText(Left)', 'Click To
 Enter')) tkt.Text(canvas, 50, 200, 400, 100, radius=20, text='RoundCornerText
 (Center)', justify='center') tkt.Text(canvas, 550, 50, 400, 100,
 text='DisableText').set_live(False) tkt.Text(canvas, 550, 200, 400, 100,
 radius=20, text='TransparentText(Right)', justify='right',
 color_fill=tkt.COLOR_NONE) root.mainloop() ```  6. `Progressbar`:
 è¿åº¦æ¡æ§ä»¶
 è¿åº¦æ¡æ§ä»¶ç¸æ¯`tkinter.ttk.Progressbar`ï¼å¤è§ä¸çèªç±åº¦è¾å¤§
 ä¸é¢æ¯`Progressbar`æ§ä»¶çå¤è§ï¼
 [ProgressbarTest.png]
 æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('ProgressbarTest',
-500, 500) canvas = tkt.Canvas(root, 500, 500) def colorful(x, y, width, height)
--> None: # type: (int, int, int, int) -> None """ Gradient colors """ for i in
-range(width): color = tkt.color(('#FF0000', '#0000FF'), i/width)
+500, 500) canvas = tkt.Canvas(root, 500, 500, 0, 0) def colorful(x, y, width,
+height) -> None: # type: (int, int, int, int) -> None """ Gradient colors """
+for i in range(width): color = tkt.color(('#FF0000', '#0000FF'), i/width)
 canvas.create_line(x+i, y, x+i, y+height, fill=color) colorful(30, 290, 440,
 50) tkt.Progressbar(canvas, 50, 50, 400, 30) tkt.Progressbar(canvas, 50, 100,
 400, 30).load(.6667) tkt.Progressbar(canvas, 50, 150, 400, 30,
 borderwidth=5).load(1) (_ := tkt.Progressbar(canvas, 50, 200, 400, 30)).load
 (0.3333) _.set_live(False) tkt.Progressbar(canvas, 50, 250, 400, 30, color_bar=
 ( 'lightyellow', 'skyblue')).load(.5) tkt.Progressbar(canvas, 50, 300, 400, 30,
 color_bar=('', 'orange')).load(.1667) progressbar = tkt.Progressbar(canvas, 50,
@@ -182,18 +184,18 @@
 ç±»åçå¾ççæ¯æä¹æå¼ºåï¼å¯ä»¥å¨ä¸ä¾èµä»»ä½ç¬¬ä¸æ¹æ¨¡åæèåºçæåµä¸ï¼å¯¹
 png å¾çè¿è¡ç¼©æ¾ 2. `Singleton`: åä¾æ¨¡å¼ç±»
 åä¾æ¨¡å¼ï¼ä¸ç¨ä»ç»äºå§ï¼éè¿ç»§æ¿å®æ¥ä½¿ç¨ ### Tool Function/
 å·¥å·å½æ° 1. `move`: ç§»å¨å½æ°
 ç§»å¨å½æ°å¯ä»¥è½»æ¾å°æä¸å®çè§å¾ãç§»å¨éåº¦ãç§»å¨æ¶é´å»ç§»å¨`tkintertools`æ¨¡ååçææå¯¹è±¡ï¼åæ¶å¼å®¹äº`tkinter`åçå¯¹è±¡ï¼å³`tkinter`ä¸­çå¯¹è±¡ä¹å¯ä»¥å¾æ¹ä¾¿å°ç§»å¨ï¼çè³å®è¿å¯ä»¥ç§»å¨çªå£çä½ç½®ï¼
 [MoveTest.gif]
 æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('MoveTest', 500,
-500) canvas = tkt.Canvas(root, 500, 500) rect = canvas.create_rectangle(50,
-350, 150, 450) def move_window(switch=[True]): # type: (list[bool]) -> None
-tkt.move(root, None, 1000 if switch[0] else -1000, 0, 800, mode='flat') switch
-[0] = not switch[0] def move_button(switch=[True]) -> None: # type: (list
+500) canvas = tkt.Canvas(root, 500, 500, 0, 0) rect = canvas.create_rectangle
+(50, 350, 150, 450) def move_window(switch=[True]): # type: (list[bool]) -
+> None tkt.move(root, None, 1000 if switch[0] else -1000, 0, 800, mode='flat')
+switch[0] = not switch[0] def move_button(switch=[True]) -> None: # type: (list
 [bool]) -> None tkt.move(canvas, button, 200 if switch[0] else -200, 0, 500,
 mode='rebound') switch[0] = not switch[0] def move_rect(switch=[True]): # type:
 (list[bool]) -> None tkt.move(canvas, rect, 200 if switch[0] else -200, 0, 500,
 mode='smooth') switch[0] = not switch[0] tkt.Button(canvas, 50, 50, 200, 40,
 radius=10, text='MoveWindow', command=move_window) tkt.Button(canvas, 50, 100,
 200, 40, radius=10, text='MoveRect', command=move_rect) button = tkt.Button
 (canvas, 50, 150, 200, 40, radius=10, text='MoveButton', command=move_button)
@@ -204,19 +206,19 @@
     `center` : "    tkintertools    "
     `right`  : "        tkintertools"
 3. `color`: é¢è²å½æ°
 é¢è²å½æ°å¯ä»¥è½»æ¾æ±åºä¸ä¸ªé¢è²å°å¦å¤ä¸ä¸ªé¢è²çè¿æ¸¡é¢è²ï¼å æ­¤å¯ä»¥è½»æ¾å¾å°æ¸åè²çææï¼åæ¶ï¼æ¹åä¼ å¥çåæ°è¿å¯ä»¥å¾å°ä¼ å¥é¢è²çå¯¹æ¯è²
 ç¬¬äºå¼ å¾æ¯ test.py å¨å¾åæµè¯ä¸­ç»å¶çå¾æ¡
 [ColorTest.png] [Test_Draw.png]
 æºä»£ç  ```python import tkintertools as tkt root = tkt.Tk('ColorTest', 500,
-500) canvas = tkt.Canvas(root, 500, 500) def colorful(x, y, width, height): #
-type: (int, int, int, int) -> None """ Gradient colors """ for i in range
-(width): color = tkt.color(('#FF0000', '#00FF00'), i/width) color_2 = tkt.color
-(('#FFFFFF', '#000000'), i/width) canvas.create_line(x+i, y, x+i, y+height,
-fill=color) canvas.create_oval(250-i/3, 300-i/3, 250+i/3, 300 + i/3,
+500) canvas = tkt.Canvas(root, 500, 500, 0, 0) def colorful(x, y, width,
+height): # type: (int, int, int, int) -> None """ Gradient colors """ for i in
+range(width): color = tkt.color(('#FF0000', '#00FF00'), i/width) color_2 =
+tkt.color(('#FFFFFF', '#000000'), i/width) canvas.create_line(x+i, y, x+i,
+y+height, fill=color) canvas.create_oval(250-i/3, 300-i/3, 250+i/3, 300 + i/3,
 outline=color_2, width=2) colorful(50, 50, 400, 100) root.mainloop() ```  4.
 `askfont`: å­ä½éæ©å¯¹è¯æ¡
 `askfont`å½æ°å¯ä»¥æå¼é»è®¤çå­ä½éæ©çªå£ï¼è¿ä¸ªçªå£è½ç¶æ¯é»è®¤çï¼ä½å®å®éä¸æ æ³å¨`tkinter`ä¸­æå¼ï¼å ä¸º`tkinter`å¹¶æ²¡æå¯¹åºç
 API è½å¤åå°è¿ä¸ç¹ãä½æ¯ï¼`tkintertools`è°ç¨å¹¶å°è£äºåçç
 tcl çå½ä»¤ï¼ä½¿å¾å­ä½éæ©æ¡è½å¤è¢«æä»¬ä½¿ç¨ã
 [font.png]
 5. `SetProcessDpiAwareness`: DPI çº§å«è®¾ç½®å½æ°
```

