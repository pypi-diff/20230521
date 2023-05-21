# Comparing `tmp/tkintertools-2.6.0.tar.gz` & `tmp/tkintertools-2.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tkintertools-2.6.0.tar", last modified: Tue Mar 28 05:27:26 2023, max compression
+gzip compressed data, was "tkintertools-2.6.1.tar", last modified: Sun May 21 08:29:30 2023, max compression
```

## Comparing `tkintertools-2.6.0.tar` & `tkintertools-2.6.1.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-03-28 05:27:26.135968 tkintertools-2.6.0/
--rw-rw-rw-   0        0        0     7543 2022-12-08 13:06:04.000000 tkintertools-2.6.0/LICENSE
--rw-rw-rw-   0        0        0    18420 2023-03-28 05:27:26.133969 tkintertools-2.6.0/PKG-INFO
--rw-rw-rw-   0        0        0    17938 2023-03-28 05:24:17.000000 tkintertools-2.6.0/README.md
--rw-rw-rw-   0        0        0       42 2023-03-28 05:27:26.135968 tkintertools-2.6.0/setup.cfg
--rw-rw-rw-   0        0        0     1456 2023-03-28 05:19:50.000000 tkintertools-2.6.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-03-28 05:27:26.124963 tkintertools-2.6.0/tkintertools/
--rw-rw-rw-   0        0        0     1826 2023-03-25 14:48:52.000000 tkintertools-2.6.0/tkintertools/__init__.py
--rw-rw-rw-   0        0        0    54960 2023-03-28 05:13:15.000000 tkintertools-2.6.0/tkintertools/__main__.py
--rw-rw-rw-   0        0        0     1169 2023-03-24 11:49:37.000000 tkintertools-2.6.0/tkintertools/constants.py
-drwxrwxrwx   0        0        0        0 2023-03-28 05:27:26.129971 tkintertools-2.6.0/tkintertools.egg-info/
--rw-rw-rw-   0        0        0    18420 2023-03-28 05:27:26.000000 tkintertools-2.6.0/tkintertools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2023-03-28 05:27:26.000000 tkintertools-2.6.0/tkintertools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-28 05:27:26.000000 tkintertools-2.6.0/tkintertools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2023-03-28 05:27:26.000000 tkintertools-2.6.0/tkintertools.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-21 08:29:30.608759 tkintertools-2.6.1/
+-rw-rw-rw-   0        0        0     7548 2023-05-20 23:03:00.000000 tkintertools-2.6.1/LICENSE
+-rw-rw-rw-   0        0        0    26393 2023-05-21 08:29:30.607759 tkintertools-2.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0    25888 2023-05-21 08:23:58.000000 tkintertools-2.6.1/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-21 08:29:30.608759 tkintertools-2.6.1/setup.cfg
+-rw-rw-rw-   0        0        0     1206 2023-05-21 08:28:45.000000 tkintertools-2.6.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-21 08:29:30.602758 tkintertools-2.6.1/tkintertools/
+-rw-rw-rw-   0        0        0     1877 2023-05-20 20:35:35.000000 tkintertools-2.6.1/tkintertools/__init__.py
+-rw-rw-rw-   0        0        0    60681 2023-05-21 06:47:19.000000 tkintertools-2.6.1/tkintertools/__main__.py
+-rw-rw-rw-   0        0        0     1295 2023-05-20 20:58:40.000000 tkintertools-2.6.1/tkintertools/constants.py
+-rw-rw-rw-   0        0        0      870 2023-05-14 13:27:34.000000 tkintertools-2.6.1/tkintertools/md.py
+drwxrwxrwx   0        0        0        0 2023-05-21 08:29:30.606759 tkintertools-2.6.1/tkintertools.egg-info/
+-rw-rw-rw-   0        0        0    26393 2023-05-21 08:29:30.000000 tkintertools-2.6.1/tkintertools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      265 2023-05-21 08:29:30.000000 tkintertools-2.6.1/tkintertools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-21 08:29:30.000000 tkintertools-2.6.1/tkintertools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2023-05-21 08:29:30.000000 tkintertools-2.6.1/tkintertools.egg-info/top_level.txt
```

### Comparing `tkintertools-2.6.0/LICENSE` & `tkintertools-2.6.1/LICENSE`

 * *Files 0% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 
    THIS LICENSE IS WRITTEN IN BOTH CHINESE AND ENGLISH, AND THE CHINESE VERSION AND ENGLISH VERSION SHALL HAVE THE SAME LEGAL EFFECT. IN THE CASE OF DIVERGENCE BETWEEN THE CHINESE AND ENGLISH VERSIONS, THE CHINESE VERSION SHALL PREVAIL.
 
 END OF THE TERMS AND CONDITIONS
 
 =======================================================================================
 
-Copyright (c) 2022 小康2022
+Copyright (c) 2022-2023 小康2022
 
 [tkintertools] is licensed under Mulan PSL v2.
 
 You can use this software according to the terms and conditions of the Mulan PSL v2.
 
 You may obtain a copy of Mulan PSL v2 at:
```

### Comparing `tkintertools-2.6.0/setup.py` & `tkintertools-2.6.1/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,32 @@
 """ 上传 pypi """
 
 import setuptools
 
-from tkintertools import __version__
-
-mode = 0
-# 0 : 正式版
-# 1 : 开发版
-# 2 : 测试版
-
-name = ('tkintertools', 'tkintertools_dev', 'tkintertools_test')[mode]
-version = __version__ if mode == 0 else input(
-    '输入%s版本号: ' % ('开发' if mode == 1 else '测试'))
 
 setuptools.setup(
-    name=name,
-    version=version,
+    name='tkintertools',
+    version="2.6.1",
     author='Xiaokang2022',
+    license='MulanPSL-2.0',
     author_email='2951256653@qq.com',
     description='An auxiliary module of the tkinder module',
     long_description=open('README.md', encoding='utf-8').read(),
     long_description_content_type='text/markdown',
     url='https://gitcode.net/weixin_62651706/tkintertools',
     packages=setuptools.find_packages(),
     classifiers=[
         'Programming Language :: Python :: 3',
         'License :: OSI Approved :: Mulan Permissive Software License v2 (MulanPSL-2.0)',
         'Operating System :: OS Independent',
     ],
 )
 
 # python -m pip install --user --upgrade setuptools wheel [检查更新]
+
 # python setup.py sdist bdist_wheel [打包]
 # twine upload dist/* [上传]
 
 # pip install -U pypistats [数据分析]
 # pip install socksio [数据分析]
 
 # pypistats overall tkintertools [数据分析]
```

### Comparing `tkintertools-2.6.0/tkintertools/__init__.py` & `tkintertools-2.6.1/tkintertools/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -12,39 +12,42 @@
 * Gradient colors and contrast colors
 * Text with controllable length and alignment
 * Convenient, inheritable singleton pattern class
 * Display clear window and its contents
 
 Contents
 --------
-* Container Widget: `Tk`, `Toplevel`, `Canvas`
-* Virtual Widget: `Label`, `Button`, `CheckButton`, `Entry`, `Text`, `Progressbar`
-* Tool Class: `PhotoImage`, `Singleton`
-* Tool Function: `move`, `text`, `color`, `askfont`, `SetProcessDpiAwareness`
+* Container Widgets: `Tk`, `Toplevel`, `Canvas`
+* Virtual Canvas Widgets: `Label`, `Button`, `CheckButton`, `Entry`, `Text`, `Progressbar`
+* Tool Classes: `PhotoImage`, `Singleton`
+* Tool Functions: `move`, `text`, `color`, `askfont`, `SetProcessDpiAwareness`
 
 More
 ----
 * GitCode: https://gitcode.net/weixin_62651706/tkintertools
 * GitHub(Mirror): https://github.com/XiaoKang2022-CSDN/tkintertools
 * Tutorials: https://xiaokang2022.blog.csdn.net/article/details/127374661
 """
 
-import sys  # 检测 Python 版本
+import sys
 
-if sys.version_info < (3, 10):
-    # 版本检测，低版本缺失部分语法
-    error_info = '\n\033[31mOperation Requirements: \033[32m\nPython version shall not be less than\033[33m 3.10.0!\033[0m'
+if sys.version_info < (3, 7):  # Version Check
+    error_info = '\n\033[31mOperation Requirements: \033[32m\nPython version shall not be less than\033[33m 3.7.0 !\033[0m'
     raise RuntimeError(error_info)
 
 from .__main__ import (Button, Canvas, CheckButton, Entry, Label, PhotoImage,
                        Progressbar, SetProcessDpiAwareness, Singleton, Text,
                        Tk, Toplevel, askfont, color, move, text)
 from .constants import *
 
 __author__ = 'Xiaokang2022<2951256653@qq.com>'
-__version__ = '2.6.0'
+__version__ = '2.6.1'
 __all__ = [
+    # Container Widgets
     'Tk', 'Toplevel', 'Canvas',
+    # Virtual Canvas Widgets
     'Label', 'Button', 'CheckButton', 'Entry', 'Text', 'Progressbar',
+    # Tool Classes
     'PhotoImage', 'Singleton',
+    # Tool Functions
     'move', 'text', 'color', 'askfont', 'SetProcessDpiAwareness'
 ]
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `tkintertools-2.6.0/tkintertools/__main__.py` & `tkintertools-2.6.1/tkintertools/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,78 +1,87 @@
 """ Main File """
 
 import math  # 数学函数
+import sys  # DPI 兼容
 import tkinter  # 基础模块
-from ctypes import OleDLL  # DPI兼容
 from fractions import Fraction  # 图片缩放
-from typing import Callable, Generator, Iterable, Literal  # 类型提示
+from typing import Any, Callable, Generator, Iterable  # 类型提示
+
+try:  # NOTE: 为了兼容 Python3.7，从 typing_extensions 引入 Literal 而不是 typing
+    from typing_extensions import Literal
+except ImportError:
+    pass
+
+if sys.platform == 'win32':  # 仅在 Windows 平台下支持设置 DPI 级别
+    from ctypes import WinDLL
+else:
+    WinDLL = None
 
 from .constants import *
 
 
 class Tk(tkinter.Tk):
-    """ 创建窗口，并处理缩放操作 """
+    """ 创建一个主窗口 """
 
     def __init__(
         self,
-        title: str | None = None,
-        width: int | None = None,
-        height: int | None = None,
-        x: int | None = None,
-        y: int | None = None,
+        title=None,  # type: str | None
+        width=None,  # type: int | None
+        height=None,  # type: int | None
+        x=None,  # type: int | None
+        y=None,  # type: int | None
         *,
-        shutdown: Callable | None = None,
+        shutdown=None,  # type: Callable | None
         **kw
-    ) -> None:
+    ):  # type: (...) -> None
         """
-        `title`: 窗口标题
-        `width`: 窗口宽度
-        `height`: 窗口高度
-        `x`: 窗口左上角横坐标
-        `y`: 窗口左上角纵坐标
-        `shutdown`: 关闭窗口之前执行的函数，但会覆盖原关闭操作
-        `**kw`: 与 tkinter.Tk 类的参数相同
+        `title`: 窗口标题\n
+        `width`: 窗口宽度\n
+        `height`: 窗口高度\n
+        `x`: 窗口左上角横坐标\n
+        `y`: 窗口左上角纵坐标\n
+        `shutdown`: 关闭窗口之前执行的函数，但会覆盖原关闭操作\n
+        `**kw`: 与 tkinter.Tk 类的参数相同\n
         """
         if type(self) == Tk:  # NOTE:方便后面的 Toplevel 类继承
             tkinter.Tk.__init__(self, **kw)
 
-        self.width: list[int] = [100, 1]  # [初始宽度, 当前宽度]
-        self.height: list[int] = [100, 1]  # [初始高度, 当前高度]
-        self._canvas: list[Canvas] = []  # 子画布列表
+        self.width = [100, 1]  # type: list[int]  # [初始宽度, 当前宽度]
+        self.height = [100, 1]  # type: list[int]  # [初始高度, 当前高度]
+        self._canvas = []  # type: list[Canvas]  # 子画布列表
 
         if width and height:
-            if x != None and y != None:
+            if x != None and y != None:  # BUG: 可能需要修改
                 self.geometry('%dx%d+%d+%d' % (width, height, x, y))
             else:
                 self.geometry('%dx%d' % (width, height))
 
         self.title(title if title else None)
         self.protocol('WM_DELETE_WINDOW', shutdown if shutdown else None)
-
         self.bind('<Configure>', lambda _: self.__zoom())  # 开启窗口缩放检测
 
-    def canvas(self) -> tuple:
-        """ `Tk`类的`Canvas`元组 """
+    def canvas(self):  # type: () -> tuple[Canvas]
+        """ 返回`Tk`类的`Canvas`元组 """
         return tuple(self._canvas)
 
-    def __zoom(self) -> None:
-        """ 缩放检测 """
+    def __zoom(self):  # type: () -> None
+        """ 内部方法：缩放检测 """
         width, height = map(int, self.geometry().split('+')[0].split('x'))
         # NOTE: 此处必须用 geometry 方法，直接用 Event 或者 winfo 会有画面异常的 bug
 
         if width == self.width[1] and height == self.height[1]:  # 没有大小的改变
             return
 
         for canvas in self._canvas:
             if canvas.expand and canvas._lock:
                 canvas.zoom(width/self.width[1], height/self.height[1])
 
         self.width[1], self.height[1] = width, height  # 更新窗口当前的宽高值
 
-    def wm_geometry(self, newGeometry: str | None = None) -> str | None:
+    def wm_geometry(self, newGeometry=None):  # type: (str | None) -> str | None
         # 重写: 添加修改初始宽高值的功能并兼容不同的DPI缩放
         if newGeometry:
             width, height, _width, _height, * \
                 _ = map(int, (newGeometry+'+0+0').replace('+', 'x').split('x'))
             self.width, self.height = [width]*2, [height]*2
             geometry = '%dx%d+%d+%d' % (width, height, _width, _height)
             if not _:
@@ -81,121 +90,139 @@
         geometry = tkinter.Tk.wm_geometry(self, newGeometry)
         width, height, _width, _height, * \
             _ = map(int, (geometry+'+0+0').replace('+', 'x').split('x'))
         return '%dx%d+%d+%d' % (width, height, _width, _height)
 
     geometry = wm_geometry
 
-    def mainloop(self, n: int = 0, *, dpi_awareness: Literal[0, 1, 2] = 1) -> None:
+    def mainloop(
+        self,
+        n=0,  # type: int
+        *,
+        dpi_awareness=1  # type: Literal[1, 2, 3]
+    ):  # type: (...) -> None
         """
-        Call the mainloop of Tk.\n
+        根（主）窗口的消息循环\n
         `dpi_awareness`: 程序的DPI级别，值可以为0、1和2，程序默认为0，默认值为1
         """
-        OleDLL('shcore').SetProcessDpiAwareness(dpi_awareness)
+        SetProcessDpiAwareness(dpi_awareness)
         return tkinter.Tk.mainloop(self, n)
 
 
 class Toplevel(tkinter.Toplevel, Tk):
-    """ 类似于`tkinter.Toplevel`，同时增加了`Tk`的功能 """
+    """ 创建一个子窗口 """
 
     def __init__(
         self,
-        master: Tk,
-        title: str | None = None,
-        width: int | None = None,
-        height: int | None = None,
-        x: int | None = None,
-        y: int | None = None,
+        master=None,  # type: Tk | None
+        title=None,  # type: str | None
+        width=None,  # type: int | None
+        height=None,  # type: int | None
+        x=None,  # type: int | None
+        y=None,  # type: int | None
         *,
-        shutdown: Callable | None = None,
+        shutdown=None,  # type: Callable | None
         **kw
-    ) -> None:
+    ):  # type: (...) -> None
         """
-        `master`: 父窗口
-        `title`: 窗口标题
-        `width`: 窗口宽度
-        `height`: 窗口高度
-        `x`: 窗口左上角横坐标
-        `y`: 窗口左上角纵坐标
-        `shutdown`: 关闭窗口之前执行的函数，但会覆盖关闭操作
-        `**kw`: 与 tkinter.Toplevel 类的参数相同
+        `master`: 父窗口\n
+        `title`: 窗口标题\n
+        `width`: 窗口宽度\n
+        `height`: 窗口高度\n
+        `x`: 窗口左上角横坐标\n
+        `y`: 窗口左上角纵坐标\n
+        `shutdown`: 关闭窗口之前执行的函数，但会覆盖关闭操作\n
+        `**kw`: 与 tkinter.Toplevel 类的参数相同\n
         """
         tkinter.Toplevel.__init__(self, master, **kw)
         Tk.__init__(self, title, width, height, x, y, shutdown=shutdown, **kw)
         self.focus_set()
 
 
 class Canvas(tkinter.Canvas):
     """ 用于承载虚拟的画布控件，并处理部分绑定事件 """
 
     def __init__(
         self,
-        master: Tk,
-        width: int,
-        height: int,
+        master,  # type: Tk | Toplevel
+        width,  # type: int
+        height,  # type: int
+        x=0,  # type: int
+        y=0,  # type: int
         *,
-        lock: bool = True,
-        expand: bool = True,
-        keep: bool = False,
+        lock=True,  # type: bool
+        expand=True,  # type: bool
+        keep=False,  # type: bool
         **kw
-    ) -> None:
+    ):  # type: (...) -> None
         """
-        `master`: 父控件
-        `width`: 画布宽度
-        `height`: 画布高度
-        `lock`: 画布内控件的功能锁，False 时功能暂时失效
-        `expand`: 画布内控件是否能缩放
-        `keep`: 保持画布比例不变
-        `**kw`: 与 tkinter.Canvas 类的参数相同
+        `master`: 父控件\n
+        `width`: 画布宽度\n
+        `height`: 画布高度\n
+        `x`: 画布左上角的横坐标\n
+        `y`: 画布左上角的纵坐标\n
+        `lock`: 画布内控件的功能锁，False 时功能暂时失效\n
+        `expand`: 画布内控件是否能缩放\n
+        `keep`: 画布比例是否保持不变\n
+        `**kw`: 与 tkinter.Canvas 类的参数相同\n
         """
         self.width = [width]*2  # [初始宽度, 当前宽度]
         self.height = [height]*2  # [初始高度, 当前高度]
         self._lock = lock
         self.expand = expand
         self.keep = keep
 
+        self.master = master  # type: Tk | Toplevel  # NOTE: 此语句虽冗余，实则为类型提示
+
         self.rx = 1.  # 横向放缩比率
         self.ry = 1.  # 纵向放缩比率
-        self._widget: list[BaseWidget] = []  # 子控件列表（与事件绑定有关）
+        self._widget = []  # type: list[BaseWidget]  # 子控件列表（与事件绑定有关）
         self._font = {}  # type: dict[tkinter._CanvasItemId, float]
         self._image = {}  # type: dict[tkinter._CanvasItemId, list]
 
         tkinter.Canvas.__init__(
             self, master, width=width, height=height, highlightthickness=0, **kw)
 
+        if not (kw.get('bg', None) or kw.get('background', None)):
+            # Linux 系统上背景默认值不是 #F1F1F1，影响模块默认值的效果
+            self.configure(bg=BACKGROUND)
+
         master._canvas.append(self)  # 将实例添加到 Tk 的画布列表中
+        self.place(x=x, y=y)
 
         self.bind('<Motion>', self.__touch)  # 绑定鼠标触碰控件
         self.bind('<Any-Key>', self.__input)  # 绑定键盘输入字符（和Ctrl+v的代码顺序不可错）
         self.bind('<Button-1>', self.__click)  # 绑定鼠标左键按下
         self.bind('<B1-Motion>', self.__click)  # 绑定鼠标左键按下移动
         self.bind('<MouseWheel>', self.__mousewheel)  # 绑定鼠标滚轮滚动
         self.bind('<ButtonRelease-1>', self.__release)  # 绑定鼠标左键松开
         self.bind('<<Paste>>', lambda _: self.__paste())  # 绑定粘贴快捷键
 
-    def widget(self) -> tuple:
-        """ `Canvas`类的子控件元组 """
+    def widget(self):  # type: () -> tuple[BaseWidget]
+        """ 返回`Canvas`类的`BaseWidget`元组 """
         return tuple(self._widget)
 
-    def lock(self, value: bool | None = None) -> bool | None:
+    def lock(self, value=None):  # type: (bool | None) -> bool | None
         """
-        设置画布锁
-        `value`: 布尔值，True则可操作，False反之，None则返回当前值
+        设置画布锁\n
+        ---
+        `value`: 布尔值，True则可操作，False反之，None则返回当前值\n
         """
         if value is None:
             return self._lock
         self._lock = value
         if value and self.expand:
             self.zoom()
 
-    def zoom(self, rate_x: float | None = None, rate_y: float | None = None) -> None:
+    def zoom(self, rate_x=None, rate_y=None):  # type: (float | None, float | None) -> None
         """
-        缩放画布及其内部的所有元素
-        `rate_x`: 横向缩放比率，默认值表示自动更新缩放（根据窗口缩放程度）
-        `rate_y`: 纵向缩放比率，默认值同上
+        缩放画布及其内部的所有元素\n
+        ---
+        `rate_x`: 横向缩放比率，默认值表示自动更新缩放（根据窗口缩放程度）\n
+        `rate_y`: 纵向缩放比率，默认值同上\n
         """
         if not rate_x:
             rate_x = self.master.width[1]/self.master.width[0]/self.rx
         if not rate_y:
             rate_y = self.master.height[1]/self.master.height[0]/self.ry
 
         if self.keep:  # 维持比例
@@ -235,160 +262,167 @@
 
         for item in self._image:  # 图像大小缩放（采用相对的绝对缩放）
             if self._image[item][0] and self._image[item][0].extension != 'gif':
                 self._image[item][1] = self._image[item][0].zoom(
                     temp_x*rate_x, temp_y*rate_y, 1.2)
                 self.itemconfigure(item, image=self._image[item][1])
 
-    def __touch(self, event: tkinter.Event, flag: bool = True) -> None:
-        """ 鼠标触碰控件事件 """
+    def __touch(self, event, flag=True):  # type: (tkinter.Event, bool) -> None
+        """ 内部方法：鼠标触碰控件事件 """
         if self._lock:
             for widget in self._widget[::-1]:
                 if widget.live and widget.touch(event) and flag:
                     if isinstance(widget, TextWidget):
                         self.configure(cursor='xterm')
                     elif isinstance(widget, Button):
                         self.configure(cursor='hand2')
                     else:
                         self.configure(cursor='arrow')
                     flag = False
             if flag:
                 self.configure(cursor='arrow')
 
-    def __click(self, event: tkinter.Event) -> None:
-        """ 鼠标左键按下事件 """
+    def __click(self, event):  # type: (tkinter.Event) -> None
+        """ 内部方法：鼠标左键按下事件 """
         if self._lock:
             for widget in self._widget[::-1]:
-                if widget.live and isinstance(widget, Button | TextWidget):
+                if widget.live and isinstance(widget, (Button, TextWidget)):
                     widget.click(event)  # NOTE: 无需 return，按下空白区域也有作用
                     self.focus_set()
 
-    def __release(self, event: tkinter.Event) -> None:
-        """ 鼠标左键松开事件 """
+    def __release(self, event):  # type: (tkinter.Event) -> None
+        """ 内部方法：鼠标左键松开事件 """
         if self._lock:
             for widget in self._widget[::-1]:
                 if widget.live and isinstance(widget, Button):
                     if widget.touch(event):
                         return widget.execute(event)
 
-    def __mousewheel(self, event: tkinter.Event) -> None:
-        """ 鼠标滚轮滚动事件 """
+    def __mousewheel(self, event):  # type: (tkinter.Event) -> None
+        """ 内部方法：鼠标滚轮滚动事件 """
         if self._lock:
             for widget in self._widget[::-1]:
                 if widget.live and isinstance(widget, Text):
                     if widget.scroll(event):
                         return
 
-    def __input(self, event: tkinter.Event) -> None:
-        """ 键盘输入字符事件 """
+    def __input(self, event):  # type: (tkinter.Event) -> None
+        """ 内部方法：键盘输入字符事件 """
         if self._lock:
             for widget in self._widget[::-1]:
                 if widget.live and isinstance(widget, TextWidget):
                     if widget.input(event):
                         return
 
-    def __paste(self) -> None:
-        """ 快捷键粘贴事件 """
+    def __paste(self):  # type: () -> None
+        """ 内部方法：快捷键粘贴事件 """
         if self._lock:
             for widget in self._widget[::-1]:
                 if widget.live and isinstance(widget, TextWidget):
                     if widget.paste():
                         return
 
-    def create_text(self, *args, **kw):
+    def create_text(self, *args, **kw):  # type: (...) -> tkinter._CanvasItemId
         # 重写：添加对 text 类型的 _CanvasItemId 的字体大小的控制
         font = kw.get('font')
         if not font:
             kw['font'] = FONT, SIZE
         elif isinstance(font, str):
             kw['font'] = font, SIZE
         item = tkinter.Canvas.create_text(self, *args, **kw)
         self._font[item] = list(kw['font'])
         return item
 
-    def create_image(self, *args, **kw):
+    def create_image(self, *args, **kw):  # type: (...) -> tkinter._CanvasItemId
         # 重写：添加对 image 类型的 _CanvasItemId 的图像大小的控制
         item = tkinter.Canvas.create_image(self, *args, **kw)
         self._image[item] = [kw.get('image'), None]
         return item
 
     def itemconfigure(
         self,
         tagOrId,  # type: str | tkinter._CanvasItemId
         **kw
-    ) -> dict[str, tuple[str, str, str, str, str]] | None:
-        # 重写：创建空image的_CanvasItemId时漏去对图像大小的控制
+    ):  # type: (...) -> dict[str, tuple[str, str, str, str, str]] | None
+        # 重写：创建空 image 的 _CanvasItemId 时漏去对图像大小的控制
         if type(kw.get('image')) == PhotoImage:
             self._image[tagOrId] = [kw.get('image'), None]
         return tkinter.Canvas.itemconfigure(self, tagOrId, **kw)
 
-    def place(self, *args, **kw) -> None:
+    def place(self, *args, **kw):  # type: (...) -> None  # BUG: 缩放就会恢复原样
         # 重写：增加一些特定功能
         self.width[0] = kw.get('wdith', self.width[0])
         self.height[0] = kw.get('height', self.height[0])
         return tkinter.Canvas.place(self, *args, **kw)
 
-    def destroy(self) -> None:
+    def destroy(self):  # type: () -> None
         # 重写：兼容
         self.master._canvas.remove(self)
         for widget in self.widget():
             widget.destroy()
         return tkinter.Canvas.destroy(self)
 
 
 class BaseWidget:
-    """ 虚拟画布控件基类 """
+    """ 内部类：虚拟画布控件基类 """
 
     def __init__(
         self,
-        canvas: Canvas,
-        x: float,
-        y: float,
-        width: float,
-        height: float,
-        radius: float,
-        text: str,
-        justify: str,
-        borderwidth: float,
-        font: tuple[str, int, str],
+        canvas,  # type:  Canvas
+        x,  # type: float
+        y,  # type: float
+        width,  # type: float
+        height,  # type: float
+        radius,  # type: float
+        text,  # type: str
+        justify,  # type: str
+        borderwidth,  # type: float
+        font,  # type: tuple[str, int, str]
         image,  # type: PhotoImage | None
-        color_text: tuple[str, str, str],
-        color_fill: tuple[str, str, str],
-        color_outline: tuple[str, str, str]
-    ) -> None:
+        color_text,  # type: tuple[str, str, str]
+        color_fill,  # type: tuple[str, str, str]
+        color_outline  # type: tuple[str, str, str]
+    ):  # type: (...) -> None
         """
         ### 标准参数
-        `canvas`: 父画布容器控件
-        `x`: 控件左上角的横坐标
-        `y`: 控件左上角的纵坐标
-        `width`: 控件的宽度
-        `height`: 控件的高度
-        `radius`: 控件圆角化半径
-        `text`: 控件显示的文本，对于文本控件而言，可以为一个元组：(默认文本, 鼠标触碰文本)
-        `justify`: 文本的对齐方式
-        `borderwidth`: 外框的宽度
-        `font`: 控件的字体设定 (字体, 大小, 样式)
-        `image`: 控件的背景（支持 png 类型，大小必须小于控件，否则会溢出）
-        `color_text`: 控件文本的颜色
-        `color_fill`: 控件内部的颜色
-        `color_outline`: 控件外框的颜色
+        标准参数是所有控件都有的\n
+        ---
+        `canvas`: 父画布容器控件\n
+        `x`: 控件左上角的横坐标\n
+        `y`: 控件左上角的纵坐标\n
+        `width`: 控件的宽度\n
+        `height`: 控件的高度\n
+        `radius`: 控件圆角化半径\n
+        `text`: 控件显示的文本，对于文本控件而言，可以为一个元组：(默认文本, 鼠标触碰文本)\n
+        `justify`: 文本的对齐方式\n
+        `borderwidth`: 外框的宽度\n
+        `font`: 控件的字体设定 (字体, 大小, 样式)\n
+        `image`: 控件的背景（支持 png 类型，大小必须小于控件，否则会溢出）\n
+        `color_text`: 控件文本的颜色\n
+        `color_fill`: 控件内部的颜色\n
+        `color_outline`: 控件外框的颜色\n
+        ---
         ### 特定参数
-        `command`: 按钮控件的关联函数
-        `show`: 文本控件的显示文本
-        `limit`: 文本控件的输入字数限制，为负数时表示没有字数限制
-        `read`: 文本控件的只读模式
-        `cursor`: 输入提示符的字符，默认为一竖线
+        特定参数只有某些控件类才有\n
+        ---
+        `command`: 按钮控件的关联函数\n
+        `show`: 文本控件的显示文本\n
+        `limit`: 文本控件的输入字数限制，为负数时表示没有字数限制\n
+        `read`: 文本控件的只读模式\n
+        `cursor`: 输入提示符的字符，默认为一竖线\n
+        ---
         ### 详细说明
-        字体的值为一个包含两个或三个值的元组，共两种形式
-        形式一: `(字体名称, 字体大小)`
-        形式二: `(字体名称, 字体大小, 字体样式)`
-
-        颜色为一个包含三个或四个 RGB 颜色字符串的元组，共两种形式
-        不使用禁用功能时: `(正常颜色, 触碰颜色, 交互颜色)`
-        需使用禁用功能时: `(正常颜色, 触碰颜色, 交互颜色, 禁用颜色)`
+        1. 字体的值为一个包含两个或三个值的元组或者单个的字符串，共三种形式\n
+            * 形式一: `字体名称`
+            * 形式二: `(字体名称, 字体大小)`
+            * 形式三: `(字体名称, 字体大小, 字体样式)`
+        2. 颜色为一个包含三个或四个 RGB 颜色字符串的元组，共两种形式\n
+            * 不使用禁用功能时: `(正常颜色, 触碰颜色, 交互颜色)`
+            * 需使用禁用功能时: `(正常颜色, 触碰颜色, 交互颜色, 禁用颜色)`
+            * 特别地，进度条控件的参数`color_bar`为: `(底色, 进度条颜色)`
         """
         self.master = canvas
         self.value = text
         self.justify = justify
         self.font = font
         self.photoimage = image
         self.color_text = list(color_text)
@@ -403,18 +437,18 @@
         self.x1, self.y1 = x, y  # 控件左上角坐标
         self.x2, self.y2 = x+width, y+height  # 控件左下角坐标
         self.width, self.height = width, height  # 控件的宽高值
         self.radius = radius  # 边角圆弧半径
         self.live = True  # 控件活跃标志
         self._state = 'normal'  # 控件的状态
         self.pre_state = None  # 记录之前的状态
-        self.command_ex: dict[str, Callable | None] = {
+        self.command_ex = {
             'normal': None, 'touch': None,
             'click': None, 'disabled': None
-        }
+        }  # type: dict[str, Callable | None]
 
         canvas._widget.append(self)  # 将实例添加到父画布控件
 
         if radius:
             if 2 * radius > width:
                 radius = width // 2
                 self.radius = radius
@@ -481,21 +515,22 @@
 
         if type(font) != str:
             font = list(font)
             font[1] = int(font[1]*math.sqrt(canvas.rx*canvas.ry))
             canvas._font[self.text][1] = font[1]
             canvas.itemconfigure(self.text, font=font)
 
-    def state(self, mode: Literal['normal', 'touch', 'click', 'disabled'] | None = None) -> None:
+    def state(self, mode=None):  # type: (Literal['normal', 'touch', 'click', 'disabled'] | None) -> None
         """
-        mode 参数为 None 时仅更新控件，否则改变虚拟控件的外观
-        `normal`: 正常状态
-        `touch`: 鼠标触碰时的状态
-        `click`: 鼠标按下时的状态
-        `disabled`: 禁用状态
+        mode 参数为 None 时仅更新控件，否则改变虚拟控件的外观\n
+        ---
+        `normal`: 正常状态\n
+        `touch`: 鼠标触碰时的状态\n
+        `click`: 鼠标按下时的状态\n
+        `disabled`: 禁用状态\n
         """
         if mode:
             self._state, self.pre_state = mode, self._state
             if self._state == self.pre_state:  # 保持状态时直接跳过
                 return
 
         if self._state == 'normal':
@@ -504,15 +539,15 @@
             mode = 1
         elif self._state == 'click':
             mode = 2
         else:
             mode = 3
 
         self.master.itemconfigure(self.text, fill=self.color_text[mode])
-        if isinstance(self, Text):
+        if isinstance(self, (Text, CheckButton)):
             self.master.itemconfigure(self._text, fill=self.color_text[mode])
 
         if self.radius:
             for item in self.inside:  # 修改色块
                 self.master.itemconfigure(item, fill=self.color_fill[mode])
 
             # 修改线条
@@ -530,19 +565,20 @@
             else:
                 self.master.itemconfigure(
                     self.rect, fill=self.color_fill[mode])
 
         if self.command_ex[self._state]:
             self.command_ex[self._state]()
 
-    def move(self, dx: float, dy: float) -> None:
+    def move(self, dx, dy):  # type: (float, float) -> None
         """
-        移动控件的位置
-        `dx`: 横向移动长度（单位：像素）
-        `dy`: 纵向移动长度
+        移动控件的位置\n
+        ---
+        `dx`: 横向移动长度（单位：像素）\n
+        `dy`: 纵向移动长度\n
         """
         self.x1 += dx
         self.x2 += dx
         self.y1 += dy
         self.y2 += dy
 
         if self.radius:
@@ -552,128 +588,118 @@
             self.master.move(self.rect, dx, dy)
 
         self.master.move(self.image, dx, dy)
         self.master.move(self.text, dx, dy)
 
         if isinstance(self, TextWidget):
             self.master.move(self._cursor, dx, dy)
-        if isinstance(self, Text):
+        if isinstance(self, (Text, CheckButton)):
             self.master.move(self._text, dx, dy)
         if isinstance(self, Progressbar):
             self.master.move(self.bar, dx, dy)
 
-    def moveto(self, x: float, y: float) -> None:
+    def moveto(self, x, y):  # type: (float, float) -> None
         """
-        改变控件的位置
-        `x`: 改变到的横坐标（单位：像素）
-        `y`: 改变到的纵坐标
+        改变控件的位置（以控件左上角为基准）\n
+        ---
+        `x`: 改变到的横坐标（单位：像素）\n
+        `y`: 改变到的纵坐标\n
         """
-        self.x1, self.x2 = x, x+self.width
-        self.y1, self.y2 = y, y+self.height
-
-        if self.radius:
-            for item in self.inside+self.outside:
-                self.master.moveto(item, x, y)
-        else:
-            self.master.moveto(self.rect, x, y)
-
-        self.master.moveto(self.image, x, y)
-        self.master.moveto(self.text, x, y)
+        self.move(x - self.x1, y - self.y1)
 
-        if isinstance(self, TextWidget):
-            self.master.moveto(self._cursor, x, y)
-        if isinstance(self, Text):
-            self.master.moveto(self._text, x, y)
-        if isinstance(self, Progressbar):
-            self.master.moveto(self.bar, x, y)
-
-    def configure(self, *args, **kw) -> str | tuple | None:
+    def configure(self, *args, **kw):  # type: (...) -> str | tuple | None
         """
-        修改或查询原有参数的值，可供修改或查询的参数有
+        修改或查询原有参数的值，可供修改或查询的参数有\n
         1. 所有控件: `color_text`、`color_fill`、`color_outline`
-        2. 非文本控件: `text`
+        2. 非文本控件: `text`\n
+        注意：颜色修改不会立即生效，可通过鼠标经过生效，或者调用 state 方法立即刷新状态！
         """
         if args:
             if args[0] == 'text':
+                if isinstance(self, CheckButton):
+                    return self.master.itemcget(self._text, 'text')
                 return self.value
             else:
                 return getattr(self, args[0])
 
         value = kw.get('text', None)
         text = kw.get('color_text', None)
         fill = kw.get('color_fill', None)
         outline = kw.get('color_outline', None)
 
         if value != None:
-            self.value = value
+            if isinstance(self, CheckButton):
+                self.master.itemconfigure(self._text, text=value)
+            else:
+                self.value = value
         if text:
             self.color_text = text
         if fill:
             self.color_fill = fill
         if outline:
             self.color_outline = outline
 
-        if isinstance(self, Label | Button | Progressbar) and value != None:
+        if isinstance(self, (Label, Button, Progressbar)) and value != None and not isinstance(self, CheckButton):
             self.master.itemconfigure(self.text, text=value)
 
-    def destroy(self) -> None:
+    def destroy(self):  # type: () -> None
         """ 摧毁控件释放内存 """
         self.live = False
         self.master._widget.remove(self)
 
         if self.radius:
             for item in self.inside+self.outside:
                 self.master.delete(item)
         else:
             self.master.delete(self.rect)
 
         if isinstance(self, TextWidget):
             self.master.delete(self._cursor)
-        if isinstance(self, Text):
+        if isinstance(self, (Text, CheckButton)):
             self.master.delete(self._text)
         if isinstance(self, Progressbar):
             self.master.delete(self.bar)
 
         self.master.delete(self.image)
         self.master.delete(self.text)
 
-    def set_live(self, boolean: bool | None = None) -> bool | None:
+    def set_live(self, boolean=None):  # type: (bool | None) -> bool | None
         """ 设定或查询live值 """
         if boolean is None:
             return self.live
         else:
             self.live = boolean
             if boolean:
                 self.state('normal')
             else:
                 self.state('disabled')
 
 
 class TextWidget(BaseWidget):
-    """ 文本类控件基类 """
+    """ 内部类：文本类控件基类 """
 
     def __init__(
         self,
-        canvas: Canvas,
-        x: int,
-        y: int,
-        width: int,
-        height: int,
-        radius: float,
-        text: tuple[str] | str,
-        limit: int,
-        justify: str,
-        icursor: str,
-        borderwidth: int,
-        font: tuple[str, int, str],
+        canvas,  # type: Canvas
+        x,  # type: int
+        y,  # type: int
+        width,  # type: int
+        height,  # type: int
+        radius,  # type: float
+        text,  # type: tuple[str] | str
+        limit,  # type: int
+        justify,  # type: str
+        icursor,  # type: str
+        borderwidth,  # type: int
+        font,  # type: tuple[str, int, str]
         image,  # type: PhotoImage | None
-        color_text: tuple[str, str, str],
-        color_fill: tuple[str, str, str],
-        color_outline: tuple[str, str, str]
-    ) -> None:
+        color_text,  # type: tuple[str, str, str]
+        color_fill,  # type: tuple[str, str, str]
+        color_outline  # type: tuple[str, str, str]
+    ):  # type: (...) -> None
 
         self.canvas = canvas
         self.limit = limit
         self.icursor = icursor
 
         self.interval = 300  # 光标闪烁间
         self.flag = False  # 光标闪烁标志
@@ -685,266 +711,280 @@
 
         # 提示光标 NOTE:位置顺序不可乱动，font不可乱改
         self._cursor = canvas.create_text(0, 0, fill=color_text[2], font=font)
         canvas._font[self._cursor][1] = canvas._font[self.text][1]
         font = canvas.itemcget(self.text, 'font')
         canvas.itemconfigure(self._cursor, font=font)
 
-    def touch_on(self) -> None:
-        """ 鼠标悬停状态 """
+    def touch_on(self):  # type: () -> None
+        """ 内部方法：鼠标悬停状态 """
         if self._state != 'click':
             self.state('touch')
 
             if self.master.itemcget(self.text, 'text') == self._value[1]:
                 self.master.itemconfigure(self.text, text=self._value[2])
 
-    def touch_off(self) -> None:
-        """ 鼠标离开状态 """
+    def touch_off(self):  # type: () -> None
+        """ 内部方法：鼠标离开状态 """
         if self._state != 'click':
             self.state('normal')
 
             if self.master.itemcget(self.text, 'text') == self._value[2]:
                 self.master.itemconfigure(self.text, text=self._value[1])
 
-    def click(self, event: tkinter.Event) -> None:
-        """ 交互状态检测 """
+    def click(self, event):  # type: (tkinter.Event) -> None
+        """ 内部方法：交互状态检测 """
         if self.x1 <= event.x <= self.x2 and self.y1 <= event.y <= self.y2:
             if self._state != 'click':
                 self.click_on()
         else:
             self.click_off()
 
     def touch(
         self,  # type: Entry | Text
-        event: tkinter.Event
-    ) -> bool:
-        """ 触碰状态检测 """
+        event  # type: tkinter.Event
+    ):  # type: (...) -> bool
+        """ 内部方法：触碰状态检测 """
         condition = self.x1 <= event.x <= self.x2 and self.y1 <= event.y <= self.y2
         self.touch_on() if condition else self.touch_off()
         return condition
 
-    def cursor_flash(self) -> None:
-        """ 鼠标光标闪烁 """
+    def cursor_flash(self):  # type: () -> None
+        """ 内部方法：鼠标光标闪烁 """
         if self.interval >= 300:
             self.interval, self.flag = 0, not self.flag
             if self.flag:
                 self.master.itemconfigure(self._cursor, text=self.icursor)
             else:
                 self.master.itemconfigure(self._cursor, text='')
 
         if self._state == 'click':
             self.interval += 10
             self.master.after(10, self.cursor_flash)
         else:
             self.interval, self.flag = 300, False  # 恢复默认值
             self.master.itemconfigure(self._cursor, text='')
 
-    def cursor_update(self, text: str = ' ') -> None:
-        """ 鼠标光标更新 """
+    def cursor_update(self, text=' '):  # type: (str) -> None
+        """ 内部方法：鼠标光标更新 """
         self.interval, self.flag = 300, False  # 恢复默认值
         if isinstance(self, Entry):
             self.master.coords(self._cursor, self.master.bbox(
                 self.text)[2], self.y1+self.height * self.master.ry / 2)  # BUG
         elif isinstance(self, Text):
             _pos = self.master.bbox(self._text)
             self.master.coords(self._cursor, _pos[2], _pos[1])
         self.master.itemconfigure(
             self._cursor, text='' if not text else self.icursor)
 
-    def paste(self) -> bool:
-        """ 快捷键粘贴 """
+    def paste(self):  # type: () -> bool
+        """ 内部方法：快捷键粘贴 """
         condition = self._state == 'click' and not getattr(self, 'show', None)
         if condition:
             self.append(self.master.clipboard_get())
         return condition
 
-    def clear(self) -> None:
-        """ 清空文本类控件的内容 """
+    def clear(self):  # type: () -> None
+        """ 内部方法：清空文本类控件的内容 """
         if isinstance(self, Text):
-            (event := tkinter.Event).keysym = 'BackSpace'
+            event = tkinter.Event()
+            event.keysym = 'BackSpace'
             self.click_on()
             for _ in range(len(self.value)):
                 self.input(event, True)
             self.click_off()
         else:
             self.value = self._value[0] = ''
             self.master.itemconfigure(self.text, text='')
 
-    def get(self) -> str:
-        """ 获取输入框的值 """
+    def get(self):  # type: () -> str
+        """ 内部方法：获取输入框的值 """
         return self.value
 
-    def set(self, value: str) -> None:
+    def set(self, value):  # type: (str) -> None
         """ 设置输入框的值 """
         self.value = self._value[0] = value
         self.master.itemconfigure(self.text, text=self._value[0])
 
-    def append(self, value: str) -> None:
+    def append(self, value):  # type: (str) -> None
         """ 添加输入框的值 """
-        (event := tkinter.Event).keysym = None
+        event = tkinter.Event()
+        event.keysym = None
         self.click_on()
         for s in value:
             event.char = s
             self.input(event, True)
         self.click_off()
 
 
 class Label(BaseWidget):
     """ 创建一个虚拟的标签控件，用于显示少量文本 """
 
     def __init__(
         self,
-        canvas: Canvas,
-        x: int,
-        y: int,
-        width: int,
-        height: int,
+        canvas,  # type: Canvas
+        x,  # type: int
+        y,  # type: int
+        width,  # type: int
+        height,  # type: int
         *,
-        radius: float = RADIUS,
-        text: str = '',
-        borderwidth: int = BORDERWIDTH,
-        justify: str = tkinter.CENTER,
-        font: tuple[str, int, str] = (FONT, SIZE),
+        radius=RADIUS,  # type: float
+        text='',  # type: str
+        borderwidth=BORDERWIDTH,  # type: int
+        justify='center',  # type: Literal['left', 'center', 'right']
+        font=(FONT, SIZE),  # type: tuple[str, int, str]
         image=None,  # type: PhotoImage | None
-        color_text: tuple[str, str, str] = COLOR_TEXT,
-        color_fill: tuple[str, str, str] = COLOR_BUTTON_FILL,
-        color_outline: tuple[str, str, str] = COLOR_BUTTON_OUTLINE
-    ) -> None:
+        color_text=COLOR_TEXT,  # type: tuple[str, str, str]
+        color_fill=COLOR_BUTTON_FILL,  # type: tuple[str, str, str]
+        color_outline=COLOR_BUTTON_OUTLINE  # type: tuple[str, str, str]
+    ):  # type: (...) -> None
         BaseWidget.__init__(self, canvas, x, y, width, height, radius, text, justify,
                             borderwidth, font, image, color_text, color_fill, color_outline)
 
-    def touch(self, event: tkinter.Event) -> bool:
+    def touch(self, event):  # type: (tkinter.Event) -> bool
         """ 触碰状态检测 """
         condition = self.x1 <= event.x <= self.x2 and self.y1 <= event.y <= self.y2
         self.state('touch' if condition else 'normal')
         return condition
 
 
 class Button(BaseWidget):
     """ 创建一个虚拟的按钮，并执行关联函数 """
 
     def __init__(
         self,
-        canvas: Canvas,
-        x: int,
-        y: int,
-        width: int,
-        height: int,
+        canvas,  # type: Canvas
+        x,  # type: int
+        y,  # type: int
+        width,  # type: int
+        height,  # type: int
         *,
-        radius: float = RADIUS,
-        text: str = '',
-        borderwidth: int = BORDERWIDTH,
-        justify: str = tkinter.CENTER,
-        font: tuple[str, int, str] = (FONT, SIZE),
-        command: Callable | None = None,
+        radius=RADIUS,  # type: float
+        text='',  # type: str
+        borderwidth: int = BORDERWIDTH,  # type: int
+        justify='center',  # type: Literal['left', 'center', 'right']
+        font=(FONT, SIZE),  # type: tuple[str, int, str]
+        command=None,  # type: Callable | None
         image=None,  # type: PhotoImage | None
-        color_text: tuple[str, str, str] = COLOR_TEXT,
-        color_fill: tuple[str, str, str] = COLOR_BUTTON_FILL,
-        color_outline: tuple[str, str, str] = COLOR_BUTTON_OUTLINE
-    ) -> None:
+        color_text=COLOR_TEXT,  # type: tuple[str, str, str]
+        color_fill=COLOR_BUTTON_FILL,  # type: tuple[str, str, str]
+        color_outline=COLOR_BUTTON_OUTLINE,  # type: tuple[str, str, str]
+    ):  # type: (...) -> None
         BaseWidget.__init__(self, canvas, x, y, width, height, radius, text, justify,
                             borderwidth, font, image, color_text, color_fill, color_outline)
         self.command = command
 
-    def execute(self, event: tkinter.Event) -> None:
+    def execute(self, event):  # type: (tkinter.Event) -> None
         """ 执行关联函数 """
         condition = self.x1 <= event.x <= self.x2 and self.y1 <= event.y <= self.y2
         if condition and self.command:
             self.command()
 
-    def click(self, event: tkinter.Event) -> None:
+    def click(self, event):  # type: (tkinter.Event) -> None
         """ 交互状态检测 """
         if self.x1 <= event.x <= self.x2 and self.y1 <= event.y <= self.y2:
             self.state('click')
         else:
             self.state('normal')
 
-    def touch(self, event: tkinter.Event) -> bool:
+    def touch(self, event):  # type: (tkinter.Event) -> bool
         """ 触碰状态检测 """
         condition = self.x1 <= event.x <= self.x2 and self.y1 <= event.y <= self.y2
         self.state('touch' if condition else 'normal')
         return condition
 
 
 class CheckButton(Button):
     """ 创建一个复选框 """
 
     def __init__(
         self,
-        canvas: Canvas,
-        x: int,
-        y: int,
-        length: int,
+        canvas,  # type: Canvas
+        x,  # type: int
+        y,  # type: int
+        length,  # type: int
         *,
-        radius: float = RADIUS,
-        borderwidth: int = BORDERWIDTH,
+        radius=RADIUS,  # type: float
+        text='',  # type: str
+        value=False,  # type: bool
+        borderwidth=BORDERWIDTH,  # type: int
+        justify='right',  # type: Literal['right', 'left']
         image=None,  # type: PhotoImage | None
-        color_text: tuple[str, str, str] = COLOR_TEXT,
-        color_fill: tuple[str, str, str] = COLOR_BUTTON_FILL,
-        color_outline: tuple[str, str, str] = COLOR_BUTTON_OUTLINE
-    ) -> None:
+        color_text=COLOR_TEXT,  # type: tuple[str, str, str]
+        color_fill=COLOR_BUTTON_FILL,  # type: tuple[str, str, str]
+        color_outline=COLOR_BUTTON_OUTLINE  # type: tuple[str, str, str]
+    ):  # type: (...) -> None
         Button.__init__(self, canvas, x, y, length, length, radius=radius, borderwidth=borderwidth, image=image,
                         color_text=color_text, color_fill=color_fill, color_outline=color_outline)
+        if justify == 'right':
+            self._text = canvas.create_text(
+                x+1.25*length, y+length/2, text=text, anchor='w')
+        else:
+            self._text = canvas.create_text(
+                x-0.25*length, y+length/2, text=text, anchor='e')
         self.command = lambda: self.set(not bool(self.value))
+        if value:
+            self.command()
 
-    def get(self) -> bool:
+    def get(self):  # type: () -> bool
         """ 获取复选框状态 """
         return bool(self.value)
 
-    def set(self, value: bool) -> None:
+    def set(self, value):  # type: (bool) -> None
         """ 设置复选框状态 """
-        self.configure(text=TICK if value else '')
+        self.value = TICK if value else ''
+        self.master.itemconfigure(self.text, text=self.value)
 
 
 class Entry(TextWidget):
     """ 创建一个虚拟的输入框控件，可输入单行少量字符，并获取这些字符 """
 
     def __init__(
         self,
-        canvas: Canvas,
-        x: int,
-        y: int,
-        width: int,
-        height: int,
+        canvas,  # type: Canvas
+        x,  # type: int
+        y,  # type: int
+        width,  # type: int
+        height,  # type: int
         *,
-        radius: float = RADIUS,
-        text: tuple[str] | str = '',
-        show: str | None = None,
-        limit: int = LIMIT,
-        cursor: str = CURSOR,
-        borderwidth: int = BORDERWIDTH,
-        justify: str = tkinter.LEFT,
-        font: tuple[str, int, str] = (FONT, SIZE),
+        radius=RADIUS,  # type: float
+        text='',  # type: tuple[str, str] | str
+        show=None,  # type: str | None
+        limit=LIMIT,  # type: int
+        cursor=CURSOR,  # type: str
+        borderwidth=BORDERWIDTH,  # type: int
+        justify='left',  # type: Literal['left', 'center', 'right']
+        font=(FONT, SIZE),  # type: tuple[str, int, str]
         image=None,  # type: PhotoImage | None
-        color_text: tuple[str, str, str] = COLOR_TEXT,
-        color_fill: tuple[str, str, str] = COLOR_TEXT_FILL,
-        color_outline: tuple[str, str, str] = COLOR_TEXT_OUTLINE
-    ) -> None:
+        color_text=COLOR_TEXT,  # type: tuple[str, str, str]
+        color_fill=COLOR_TEXT_FILL,  # type: tuple[str, str, str]
+        color_outline=COLOR_TEXT_OUTLINE  # type: tuple[str, str, str]
+    ):  # type: (...) -> None
         TextWidget.__init__(self, canvas, x, y, width, height, radius, text, limit, justify,
                             cursor, borderwidth, font, image, color_text, color_fill, color_outline)
         self.master.itemconfigure(self.text, text=self._value[1])
         self.show = show
 
-    def click_on(self) -> None:
+    def click_on(self):  # type: () -> None
         """ 控件获得焦点 """
         self.state('click')
         self.master.itemconfigure(self.text, text=self._value[0])
         self.cursor_update('')
         self.cursor_flash()
 
-    def click_off(self) -> None:
+    def click_off(self):  # type: () -> None
         """ 控件失去焦点 """
         self.state('normal')
 
         if self.value == '':
             self.master.itemconfigure(self.text, text=self._value[1])
         else:
             self.master.itemconfigure(self.text, text=self._value[0])
 
-    def input(self, event: tkinter.Event, flag: bool = False) -> None:
+    def input(self, event, flag=False):  # type: (tkinter.Event, bool) -> None
         """ 文本输入 """
         if self._state == 'click' or flag:
             if event.keysym == 'BackSpace':  # 按下退格键
                 self.value = self.value[:-1]
             elif len(self.value) == self.limit:  # 达到字数限制
                 return True
             elif len(event.char):
@@ -960,15 +1000,15 @@
 
             # 更新显示
             self.master.itemconfigure(self.text, text=self._value[0])
             self.update_text()
             self.cursor_update()
             return True
 
-    def update_text(self) -> None:
+    def update_text(self):  # type: () -> None
         """ 更新控件 """
         while True:
             pos = self.master.bbox(self.text)
             if pos[2] > self.x2-self.radius-2 or pos[0] < self.x1+self.radius+1:
                 self._value[0] = self._value[0][1:]
                 self.master.itemconfigure(self.text, text=self._value[0])
             else:
@@ -976,33 +1016,33 @@
 
 
 class Text(TextWidget):
     """ 创建一个透明的虚拟文本框，用于输入多行文本和显示多行文本（只读模式）"""
 
     def __init__(
         self,
-        canvas: Canvas,
-        x: int,
-        y: int,
-        width: int,
-        height: int,
+        canvas,  # type: Canvas
+        x,  # type: int
+        y,  # type: int
+        width,  # type: int
+        height,  # type: int
         *,
-        radius: float = RADIUS,
-        text: tuple[str] | str = '',
-        limit: int = LIMIT,
-        read: bool = False,
-        cursor: bool = CURSOR,
-        borderwidth: int = BORDERWIDTH,
-        justify: str = tkinter.LEFT,
-        font: tuple[str, int, str] = (FONT, SIZE),
+        radius=RADIUS,  # type: float
+        text='',  # type: tuple[str, str] | str
+        limit=LIMIT,  # type: int
+        read=False,  # type: bool
+        cursor=CURSOR,  # type: str
+        borderwidth=BORDERWIDTH,  # type: int
+        justify='left',  # type: Literal['left', 'center', 'right']
+        font=(FONT, SIZE),  # type: tuple[str, int, str]
         image=None,  # type: PhotoImage | None
-        color_text: tuple[str, str, str] = COLOR_TEXT,
-        color_fill: tuple[str, str, str] = COLOR_TEXT_FILL,
-        color_outline: tuple[str, str, str] = COLOR_TEXT_OUTLINE
-    ) -> None:
+        color_text=COLOR_TEXT,  # type: tuple[str, str, str]
+        color_fill=COLOR_TEXT_FILL,  # type: tuple[str, str, str]
+        color_outline=COLOR_TEXT_OUTLINE  # type: tuple[str, str, str]
+    ):  # type: (...) -> None
         TextWidget.__init__(self, canvas, x, y, width, height, radius, text, limit, justify,
                             cursor, borderwidth, font, image, color_text, color_fill, color_outline)
 
         _x = x + (width-radius-3 if justify == 'right' else width /
                   2 if justify == 'center' else radius+2)
         _anchor = 'n' if justify == 'center' else 'ne' if justify == 'right' else 'nw'
 
@@ -1017,36 +1057,36 @@
 
         # 修改多行文本靠左显示
         self.master.coords(self.text, _x, y+radius+2)
         self.master.itemconfigure(
             self.text, text=self._value[1], anchor=_anchor)
         self.master.itemconfigure(self._cursor, anchor='n')
 
-    def click_on(self) -> None:
+    def click_on(self):  # type: () -> None
         """ 控件获得焦点 """
         if not self.read:
             self.state('click')
             *__, _ = [''] + self._value[0].rsplit('\n', 1)
             self.master.itemconfigure(self.text, text=''.join(__))
             self.master.itemconfigure(self._text, text=_)
             self.cursor_update('')
             self.cursor_flash()
 
-    def click_off(self) -> None:
+    def click_off(self):  # type: () -> None
         """ 控件失去焦点 """
         self.state('normal')
 
         if self.value == '':
             self.master.itemconfigure(self.text, text=self._value[1])
         else:
             *__, _ = [''] + self._value[0].rsplit('\n', 1)
             self.master.itemconfigure(self.text, text=''.join(__))
             self.master.itemconfigure(self._text, text=_)
 
-    def input(self, event: tkinter.Event, flag: bool = False) -> bool:
+    def input(self, event, flag=False):  # type: (tkinter.Event, bool) -> bool
         """ 文本输入 """
         if self._state == 'click' or flag:
             if event.keysym == 'BackSpace':  # 按下退格键
                 self.input_backspace()
             elif len(self.value) == self.limit:  # 达到字数限制
                 return True
             elif event.keysym == 'Tab':  # 按下Tab键
@@ -1072,15 +1112,15 @@
             # 更新表面显示值
             text = self.master.itemcget(self.text, 'text')
             _text = self.master.itemcget(self._text, 'text')
             self._value[0] = text+'\n'+_text
 
             return True
 
-    def input_return(self) -> None:
+    def input_return(self):  # type: () -> None
         """ 回车键功能 """
         self.value += '\n'
 
         # 相关数据获取
         text = self.master.itemcget(self.text, 'text')
         _text = self.master.itemcget(self._text, 'text')
         _pos = self.master.bbox(self._text)
@@ -1091,15 +1131,15 @@
             self.master.move(self._text, 0, _pos[3] - _pos[1])
             self.master.itemconfigure(
                 self.text, text=text+bool(text)*'\n'+_text)
         else:  # 文本框已经被填满了
             text = text.split('\n', 1)[-1]
             self.master.itemconfigure(self.text, text=text+'\n'+_text)
 
-    def input_backspace(self) -> None:
+    def input_backspace(self):  # type: () -> None
         """ 退格键功能 """
         if not self.value:  # 没有内容，删个毛啊
             return
 
         _text = self.master.itemcget(self._text, 'text')
         self.value = self.value[:-1]
 
@@ -1109,146 +1149,168 @@
             _ = self.value.rsplit('\n', 1)[-1]
             self.master.itemconfigure(self._text, text=_)
 
             # 内容未超出框的大小
             if self.value == self.master.itemcget(self.text, 'text'):
                 _pos = self.master.bbox(self._text)
                 self.master.move(self._text, 0, _pos[1] - _pos[3])
-                __ = self.value.removesuffix(_)[:-('\n' in self.value)]
+                # NOTE: 为了兼容Python3.7/3.8,放弃使用str.removesuffix方法，以temp取而代之
+                temp = self.value[:-
+                                  len(_)] if self.value.endswith(_) else self.value
+                __ = temp[:-('\n' in self.value)]
             else:  # 内容已经超出框框的大小啦
                 text = self.master.itemcget(self.text, 'text')
-                __ = self.value.removesuffix(
-                    text)[:-1].rsplit('\n', 1)[-1]+'\n'+text.removesuffix(_)[:-1]
+                temp = self.value[:-len(text)
+                                  ] if self.value.endswith(text) else self.value
+                temp2 = text[:len(_)] if text.endswith(_) else text
+                __ = temp[:-1].rsplit('\n', 1)[-1]+'\n'+temp2[:-1]
 
             self.master.itemconfigure(self.text, text=__)
 
 
 class Progressbar(BaseWidget):
     """ 虚拟的进度条，可以直观的方式显示任务进度 """
 
     def __init__(
         self,
-        canvas: Canvas,
-        x: int,
-        y: int,
-        width: int,
-        height: int,
+        canvas,  # type: Canvas
+        x,  # type: int
+        y,  # type: int
+        width,  # type: int
+        height,  # type: int
         *,
-        borderwidth: int = BORDERWIDTH,
-        justify: str = tkinter.CENTER,
-        font: tuple[str, int, str] = (FONT, SIZE),
+        borderwidth=BORDERWIDTH,  # type: int
+        justify='center',  # type: Literal['left', 'center', 'right']
+        font=(FONT, SIZE),  # type: tuple[str, int, str]
         image=None,  # type: PhotoImage | None
-        color_text: tuple[str, str, str] = COLOR_TEXT,
-        color_outline: tuple[str, str, str] = COLOR_TEXT_OUTLINE,
-        color_bar: tuple[str, str] = COLOR_BAR
-    ) -> None:
+        color_text=COLOR_TEXT,  # type: tuple[str, str, str]
+        color_outline=COLOR_TEXT_OUTLINE,  # type: tuple[str, str, str]
+        color_bar=COLOR_BAR  # type: tuple[str, str]
+    ):  # type: (...) -> None
         self.bottom = canvas.create_rectangle(
             x, y, x+width, y+height, width=borderwidth, fill=color_bar[0])
         self.bar = canvas.create_rectangle(
             x, y, x, y+height, width=borderwidth, outline='', fill=color_bar[1])
 
         BaseWidget.__init__(self, canvas, x, y, width, height, 0, '0.00%', justify,
                             borderwidth, font, image, color_text, COLOR_NONE, color_outline)
 
         self.color_fill = list(color_bar)
 
-    def touch(self, event: tkinter.Event) -> bool:
+    def touch(self, event):  # type: (tkinter.Event) -> bool
         """ 触碰状态检测 """
         condition = self.x1 <= event.x <= self.x2 and self.y1 <= event.y <= self.y2
         self.state('touch' if condition else 'normal')
         return condition
 
-    def load(self, percentage: float) -> None:
+    def load(self, percentage):  # type: (float) -> None
         """
-        进度条加载，并更新外观
-        `percentage`: 进度条的值，范围 0~1
+        进度条加载，并更新外观\n
+        ---
+        `percentage`: 进度条的值，范围 0 ~ 1\n
         """
         percentage = 0 if percentage < 0 else 1 if percentage > 1 else percentage
         x2 = self.x1 + self.width * percentage * self.master.rx
         self.master.coords(self.bar, self.x1, self.y1, x2, self.y2)
         self.configure(text='%.2f%%' % (percentage * 100))
 
 
 class PhotoImage(tkinter.PhotoImage):
     """ 生成图片并进行相应的一些处理 """
 
     def __init__(
         self,
-        file: str | bytes,
+        file,  # type: str | bytes
         **kw
-    ) -> None:
+    ):  # type: (...) -> None
         """
-        `file`: 图片文件的路径
-        `**kw`: 与 tkinter.PhotoImage 的参数相同
+        初始化参数\n
+        ---
+        `file`: 图片文件的路径\n
+        `**kw`: 与 tkinter.PhotoImage 的参数相同\n
         """
         self.file = file  # 图片文件的路径
         self.extension = file.rsplit('.', 1)[-1]  # 文件扩展名
         self._item = {}  # type: dict[tkinter._CanvasItemId, Canvas | None]
 
         if self.extension == 'gif':  # 动态图片
-            self.image: list[tkinter.PhotoImage] = []
+            self.image = []  # type: list[tkinter.PhotoImage]
         else:  # 静态图片
             self.image = tkinter.PhotoImage.__init__(self, file=file, **kw)
 
-    def parse(self, start: int = 0) -> Generator[int, None, None]:
+    def parse(self, start=0):  # type: (int) -> Generator[int, None, None]
         """
-        解析动图，返回一个生成器
-        `start`: 动图解析的起始索引（帧数-1）
+        ### 解析动图
+        解析并得到动图的每一帧动画，该方法返回一个生成器\n
+        ---
+        `start`: 动图解析的起始索引（帧数-1）\n
         """
         try:
             while True:
                 self.image.append(tkinter.PhotoImage(
                     file=self.file, format='gif -index %d' % start))
                 value = yield start  # 抛出索引
                 start += value if value else 1
         except tkinter.TclError:
             return
 
     def play(
         self,
-        canvas: Canvas,
+        canvas,  # type: Canvas
         item,  # type: tkinter._CanvasItemId
-        interval: int,
+        interval,  # type: int
         **kw
-    ) -> None:
+    ):  # type: (...) -> None
         """
-        播放动图，canvas.lock为False会暂停
-        `canvas`: 播放动画的画布
-        `item`: 播放动画的 _CanvasItemId（create_text 的返回值）
-        `interval`: 每帧动画的间隔时间
+        ### 播放动图
+        播放动图，设置 canvas.lock 为 False 会暂停\n
+        ---
+        `canvas`: 播放动画的画布\n
+        `item`: 播放动画的 _CanvasItemId（create_text 的返回值）\n
+        `interval`: 每帧动画的间隔时间\n
         """
         if kw.get('_ind', None) is None:  # 初始化的判定
             self._item[item], kw['ind'] = canvas, -1
         if not self._item[item]:  # 终止播放的判定
             return
         if canvas._lock:  # 暂停播放的判定
             canvas.itemconfigure(item, image=self.image[kw['_ind']])
+        _ind = kw['_ind']+1
         canvas.after(interval, lambda: self.play(  # 迭代执行函数
-            canvas, item, interval, _ind=0 if (_ind := kw['_ind']+1) == len(self.image) else _ind))
+            canvas, item, interval, _ind=0 if _ind == len(self.image) else _ind))
 
     def stop(
         self,
         item,  # type: tkinter._CanvasItemId
-        clear: bool = False
-    ) -> None:
+        clear=False  # type: bool
+    ):  # type: (...) -> None
         """
-        终止动图的播放
-        `item`: 播放动画的 _CanvasItemId（create_text 的返回值）
-        `clear`: 清除图片的标识
+        ### 终止播放
+        终止对应动图的播放，且无法重新播放\n
+        ---
+        `item`: 播放动画的 _CanvasItemId（create_text 的返回值）\n
+        `clear`: 清除图片的标识, True 就清除图片\n
         """
         self._item[item] = None
         if clear:  # 清除背景
             self._item[item].itemconfigure(item, image=None)
 
-    def zoom(self, rate_x: float, rate_y: float, precision: float | None = None) -> tkinter.PhotoImage:
-        """
-        缩放图片
-        `rate_x`: 横向缩放倍率
-        `rate_y`: 纵向缩放倍率
-        `precision`: 精度到小数点后的位数（推荐 1.2），越大运算就越慢（默认值代表绝对精确）
+    def zoom(
+        self,
+        rate_x,  # type: float
+        rate_y,  # type: float
+        precision=None  # type: float | None
+    ):  # type: (...) -> tkinter.PhotoImage
+        """
+        ### 缩放图片
+        不会缩放该图片对象本身，只是返回一个缩放后的图片对象\n
+        ---
+        `rate_x`: 横向缩放倍率\n
+        `rate_y`: 纵向缩放倍率\n
+        `precision`: 精度到小数点后的位数（推荐 1.2），越大运算就越慢（默认值代表绝对精确）\n
         """
         if precision != None:
             limit = round(10**precision)
             rate_x = Fraction(str(rate_x)).limit_denominator(limit)
             rate_y = Fraction(str(rate_y)).limit_denominator(limit)
             image = tkinter.PhotoImage.zoom(
                 self, rate_x.numerator, rate_y.numerator)
@@ -1272,35 +1334,37 @@
     def __new__(cls, *args, **kw):
         if not cls._instance:
             cls._instance = object.__new__(cls)
         return cls._instance
 
 
 def move(
-    master: Tk | Canvas | tkinter.Misc | tkinter.BaseWidget | None,
-    widget: Canvas | BaseWidget | tkinter.BaseWidget,
-    dx: int,
-    dy: int,
-    times: int,
+    master,  # type: Tk | Canvas | tkinter.Misc | tkinter.BaseWidget | None
+    widget,  # type: Canvas | BaseWidget | tkinter.BaseWidget
+    dx,  # type: int
+    dy,  # type: int
+    times,  # type: int
     *,
-    mode: Iterable | Literal['smooth', 'rebound', 'flat'],
-    frames: int = FRAMES,
-    end: Callable | None = None,
-    _ind: int = 0
-) -> None:
+    # type: tuple[Callable[[float], float], float, float] | Literal['smooth', 'rebound', 'flat']  # NOTE
+    mode,
+    frames=FRAMES,  # type: int
+    end=None,  # type: Callable | None
+    _ind=0  # type: int
+):  # type: (...) -> None
     """
     ### 移动函数
     以特定方式移动由 Place 布局的某个控件或某些控件的集合或图像\n
-    `master`: 控件所在的父控件
-    `widget`: 要移动位置的控件
-    `dx`: 横向移动的距离（单位：像素）
-    `dy`: 纵向移动的距离（单位：像素）
-    `times`: 移动总时长（单位：毫秒）
-    `mode`: 移动速度模式，为 smooth（顺滑）、rebound（回弹）和 flat（平移）这三种，或者为元组 (函数, 起始值, 终止值) 的形式
-    `frames`: 帧数，越大移动就越流畅，但计算越慢（范围为 1~100）
+    ---
+    `master`: 控件所在的父控件\n
+    `widget`: 要移动位置的控件\n
+    `dx`: 横向移动的距离（单位：像素）\n
+    `dy`: 纵向移动的距离（单位：像素）\n
+    `times`: 移动总时长（单位：毫秒）\n
+    `mode`: 移动速度模式，为 smooth（顺滑）、rebound（回弹）和 flat（平移）这三种，或者为元组 (函数, 起始值, 终止值) 的形式\n
+    `frames`: 帧数，越大移动就越流畅，但计算越慢（范围为 1 ~ 100）\n
     `end`: 移动结束时执行的函数
     """
     if _ind:  # 记忆值
         dis = mode
     elif mode == 'flat':  # 平滑模式
         return move(master, widget, dx, dy, times, mode=(lambda _: 1, 0, 1), frames=frames, end=end)
     elif mode == 'smooth':  # 流畅模式
@@ -1334,44 +1398,46 @@
 
     master.after(
         round(times/frames),
         lambda: move(master, widget, dx, dy, times, mode=dis, frames=frames, end=end, _ind=_ind+1))  # 间隔一定时间执行函数
 
 
 def text(
-    length: int,
-    string: str,
-    position: Literal['left', 'center', 'right'] = 'center'
-) -> str:
+    length,  # type: int
+    string,  # type: str
+    position='center'  # type: Literal['left', 'center', 'right']
+):  # type: (...) -> str
     """
-    ### 文本函数
+    ### 文本对齐函数
     可将目标字符串改为目标长度并居中对齐，ASCII 码字符算 1 个长度，中文及其他字符算 2 个\n
-    `length`: 目标长度
-    `string`: 要修改的字符串
-    `position`: 文本处于该长度范围的位置，可选 left（靠左）、center（居中）和 right（靠右）这三个值
+    ---
+    `length`: 目标长度\n
+    `string`: 要修改的字符串\n
+    `position`: 文本处于该长度范围的位置，可选 left（靠左）、center（居中）和 right（靠右）这三个值\n
     """
     length -= sum(1 + (ord(i) >= 256) for i in string)  # 计算空格总个数
     if position == 'left':  # 靠左
         return ' '*length+string
     elif position == 'right':  # 靠右
         return string+length*' '
     else:  # 居中
         length, key = divmod(length, 2)
         return ' '*length+string+(length+key)*' '
 
 
 def color(
-    color: Iterable[str] | str,
-    proportion: float = 1.
-) -> str:
+    color,  # type: Iterable[str] | str
+    proportion=1.  # type: float
+):  # type: (...) -> str
     """
     ### 颜色函数
     按一定比例给出已有 RGB 颜色字符串的渐变 RGB 颜色字符串，或颜色的对比色\n
-    `color`: 颜色元组或列表 (初始颜色, 目标颜色)，或者一个颜色字符串（此时返回对比色）
-    `proportion`: 改变比例（浮点数，范围为 0~1）
+    ---
+    `color`: 颜色元组或列表 (初始颜色, 目标颜色)，或者一个颜色字符串（此时返回其对比色）\n
+    `proportion`: 改变比例（浮点数，范围为 0 ~ 1）\n
     """
     rgb, _rgb = [[None]*3, [None]*3], 0
 
     if isinstance(color, str):  # 对比色的情况处理
         color = color, '#%06X' % (16777216-int(color[1:], 16))
 
     for i, c in enumerate(color):  # 解析颜色的 RGB
@@ -1383,37 +1449,46 @@
         _rgb <<= 8
         _rgb += c + round((_c - c) * proportion)
 
     return '#%06X' % _rgb
 
 
 def askfont(
-    root: tkinter.Tk | tkinter.Canvas | Tk | Toplevel | Canvas,
-    bind: Callable | None = None,
-    initfont: tuple | str = ''
-) -> None:
+    root,  # type: tkinter.Tk | tkinter.Canvas | Tk | Toplevel | Canvas
+    bind=None,  # type: Callable[[str], Any] | None
+    initfont=''  # type: tuple[str, int, str] | tuple[str, int] | str
+):  # type: (...) -> None
     """
     ### 字体选择对话框
-    显示用于选择字体的对话框窗口\n
-    `root`: 父容器控件
-    `bind`: 关联函数，传入参数为 font
-    `initfont`: 初始字体，格式为 font 参数默认格式
+    弹出选择字体的默认对话框窗口\n
+    注意：由于 tkinter 模块无法直接打开该窗口，所以此处添加了这个函数\n
+    ---
+    `root`: 父容器控件\n
+    `bind`: 关联函数，有且仅有一个参数 font\n
+    `initfont`: 初始字体，格式为 font 参数默认格式\n
     """
     args = []
     if bind:
         args += ['-command', root.register(bind)]
     if initfont:
         if isinstance(initfont, tuple):
             initfont = ' '.join(str(i) for i in initfont)
         args += ['-font', initfont]
     if args:
         root.tk.call('tk', 'fontchooser', 'configure', *args)
     root.tk.call('tk', 'fontchooser', 'show')
 
 
-def SetProcessDpiAwareness(awareness: Literal[0, 1, 2] = PROCESS_SYSTEM_DPI_AWARE) -> None:
+def SetProcessDpiAwareness(
+    awareness=PROCESS_SYSTEM_DPI_AWARE  # type: Literal[0, 1, 2]
+):  # type: (...) -> None
     """
-    ### 设定程序DPI级别
-    设定窗口程序的DPI级别，让系统知道该对程序如何缩放\n
-    `awareness`: DPI级别，值可以为0、1和2，程序默认为0，默认值为1
+    ### 设定程序 DPI 级别
+    设定窗口程序的 DPI 级别，让系统知道该如何对程序进行缩放，以提升高缩放倍数情况下的清晰度\n
+    注意：
+    * 此函数仅在 Windows 平台上生效！
+    * tkintertools 程序已内置该功能，该函数不应在 tkintertools 程序中使用，而应该在 tkinter 程序中使用！
+    ---
+    `awareness`: DPI 级别，值可以为 0、1 和 2，本来默认为 0，此处更改默认值为 1\n
     """
-    OleDLL('shcore').SetProcessDpiAwareness(awareness)
+    if WinDLL:
+        WinDLL('shcore').SetProcessDpiAwareness(awareness)
```

