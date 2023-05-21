# Comparing `tmp/lightweight_charts-1.0.6.tar.gz` & `tmp/lightweight_charts-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightweight_charts-1.0.6.tar", last modified: Sat May 20 00:45:54 2023, max compression
+gzip compressed data, was "lightweight_charts-1.0.7.tar", last modified: Sun May 21 14:46:21 2023, max compression
```

## Comparing `lightweight_charts-1.0.6.tar` & `lightweight_charts-1.0.7.tar`

### file list

```diff
@@ -1,20 +1,19 @@
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-20 00:45:54.438778 lightweight_charts-1.0.6/
--rw-r--r--   0 louis      (501) staff       (20)     1066 2023-05-10 19:09:20.000000 lightweight_charts-1.0.6/LICENSE
--rw-r--r--   0 louis      (501) staff       (20)     6069 2023-05-20 00:45:54.438517 lightweight_charts-1.0.6/PKG-INFO
--rw-r--r--   0 louis      (501) staff       (20)     5723 2023-05-20 00:24:46.000000 lightweight_charts-1.0.6/README.md
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-20 00:45:54.435255 lightweight_charts-1.0.6/lightweight_charts/
--rw-r--r--   0 louis      (501) staff       (20)       47 2023-05-14 13:49:11.000000 lightweight_charts-1.0.6/lightweight_charts/__init__.py
--rw-r--r--   0 louis      (501) staff       (20)    10197 2023-05-19 22:53:50.000000 lightweight_charts-1.0.6/lightweight_charts/chart.py
--rw-r--r--   0 louis      (501) staff       (20)    31274 2023-05-20 00:36:42.000000 lightweight_charts-1.0.6/lightweight_charts/js.py
--rw-r--r--   0 louis      (501) staff       (20)   141259 2023-05-09 19:50:25.000000 lightweight_charts-1.0.6/lightweight_charts/pkg.py
--rw-r--r--   0 louis      (501) staff       (20)     2546 2023-05-19 22:53:50.000000 lightweight_charts-1.0.6/lightweight_charts/pywebview.py
--rw-r--r--   0 louis      (501) staff       (20)     2133 2023-05-18 22:28:08.000000 lightweight_charts-1.0.6/lightweight_charts/util.py
--rw-r--r--   0 louis      (501) staff       (20)     2347 2023-05-19 23:40:38.000000 lightweight_charts-1.0.6/lightweight_charts/widgets.py
-drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-20 00:45:54.437962 lightweight_charts-1.0.6/lightweight_charts.egg-info/
--rw-r--r--   0 louis      (501) staff       (20)     6069 2023-05-20 00:45:54.000000 lightweight_charts-1.0.6/lightweight_charts.egg-info/PKG-INFO
--rw-r--r--   0 louis      (501) staff       (20)      434 2023-05-20 00:45:54.000000 lightweight_charts-1.0.6/lightweight_charts.egg-info/SOURCES.txt
--rw-r--r--   0 louis      (501) staff       (20)        1 2023-05-20 00:45:54.000000 lightweight_charts-1.0.6/lightweight_charts.egg-info/dependency_links.txt
--rw-r--r--   0 louis      (501) staff       (20)       17 2023-05-20 00:45:54.000000 lightweight_charts-1.0.6/lightweight_charts.egg-info/requires.txt
--rw-r--r--   0 louis      (501) staff       (20)       19 2023-05-20 00:45:54.000000 lightweight_charts-1.0.6/lightweight_charts.egg-info/top_level.txt
--rw-r--r--   0 louis      (501) staff       (20)       38 2023-05-20 00:45:54.438876 lightweight_charts-1.0.6/setup.cfg
--rw-r--r--   0 louis      (501) staff       (20)      609 2023-05-20 00:24:46.000000 lightweight_charts-1.0.6/setup.py
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-21 14:46:21.784977 lightweight_charts-1.0.7/
+-rw-r--r--   0 louis      (501) staff       (20)     1066 2023-05-10 19:09:20.000000 lightweight_charts-1.0.7/LICENSE
+-rw-r--r--   0 louis      (501) staff       (20)     6202 2023-05-21 14:46:21.784636 lightweight_charts-1.0.7/PKG-INFO
+-rw-r--r--   0 louis      (501) staff       (20)     5856 2023-05-20 15:23:42.000000 lightweight_charts-1.0.7/README.md
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-21 14:46:21.781636 lightweight_charts-1.0.7/lightweight_charts/
+-rw-r--r--   0 louis      (501) staff       (20)       47 2023-05-14 13:49:11.000000 lightweight_charts-1.0.7/lightweight_charts/__init__.py
+-rw-r--r--   0 louis      (501) staff       (20)     3034 2023-05-20 21:15:48.000000 lightweight_charts-1.0.7/lightweight_charts/chart.py
+-rw-r--r--   0 louis      (501) staff       (20)    23947 2023-05-21 14:30:57.000000 lightweight_charts-1.0.7/lightweight_charts/js.py
+-rw-r--r--   0 louis      (501) staff       (20)   148472 2023-05-20 23:46:07.000000 lightweight_charts-1.0.7/lightweight_charts/pkg.py
+-rw-r--r--   0 louis      (501) staff       (20)     2083 2023-05-21 12:37:38.000000 lightweight_charts-1.0.7/lightweight_charts/util.py
+-rw-r--r--   0 louis      (501) staff       (20)     1932 2023-05-20 19:56:58.000000 lightweight_charts-1.0.7/lightweight_charts/widgets.py
+drwxr-xr-x   0 louis      (501) staff       (20)        0 2023-05-21 14:46:21.784136 lightweight_charts-1.0.7/lightweight_charts.egg-info/
+-rw-r--r--   0 louis      (501) staff       (20)     6202 2023-05-21 14:46:21.000000 lightweight_charts-1.0.7/lightweight_charts.egg-info/PKG-INFO
+-rw-r--r--   0 louis      (501) staff       (20)      402 2023-05-21 14:46:21.000000 lightweight_charts-1.0.7/lightweight_charts.egg-info/SOURCES.txt
+-rw-r--r--   0 louis      (501) staff       (20)        1 2023-05-21 14:46:21.000000 lightweight_charts-1.0.7/lightweight_charts.egg-info/dependency_links.txt
+-rw-r--r--   0 louis      (501) staff       (20)       17 2023-05-21 14:46:21.000000 lightweight_charts-1.0.7/lightweight_charts.egg-info/requires.txt
+-rw-r--r--   0 louis      (501) staff       (20)       19 2023-05-21 14:46:21.000000 lightweight_charts-1.0.7/lightweight_charts.egg-info/top_level.txt
+-rw-r--r--   0 louis      (501) staff       (20)       38 2023-05-21 14:46:21.785082 lightweight_charts-1.0.7/setup.cfg
+-rw-r--r--   0 louis      (501) staff       (20)      609 2023-05-21 14:35:24.000000 lightweight_charts-1.0.7/setup.py
```

### Comparing `lightweight_charts-1.0.6/LICENSE` & `lightweight_charts-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `lightweight_charts-1.0.6/PKG-INFO` & `lightweight_charts-1.0.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightweight_charts
-Version: 1.0.6
+Version: 1.0.7
 Summary: Python framework for TradingView's Lightweight Charts JavaScript library.
 Home-page: https://github.com/louisnw01/lightweight-charts-python
 Author: louisnw
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -14,15 +14,15 @@
 
 [![PyPi Release](https://img.shields.io/pypi/v/lightweight-charts?color=32a852&label=PyPi)](https://pypi.org/project/lightweight-charts/)
 [![Made with Python](https://img.shields.io/badge/Python-3.9+-c7a002?logo=python&logoColor=white)](https://python.org "Go to Python homepage")
 [![License](https://img.shields.io/github/license/louisnw01/lightweight-charts-python?color=9c2400)](https://github.com/louisnw01/lightweight-charts-python/blob/main/LICENSE)
 [![Documentation](https://img.shields.io/badge/documentation-006ee3)](https://lightweight-charts-python.readthedocs.io/en/latest/docs.html)
 
 
-![cover](cover.png)
+![cover](https://raw.githubusercontent.com/louisnw01/lightweight-charts-python/main/cover.png)
 
 lightweight-charts-python aims to provide a simple and pythonic way to access and implement [TradingView's Lightweight Charts](https://www.tradingview.com/lightweight-charts/).
 
 ## Installation
 ```
 pip install lightweight_charts
 ```
@@ -50,15 +50,15 @@
     # Columns: | time | open | high | low | close | volume (if volume is enabled) |
     df = pd.read_csv('ohlcv.csv')
     chart.set(df)
     
     chart.show(block=True)
 
 ```
-![setting_data image](https://github.com/louisnw01/lightweight-charts-python/blob/main/examples/1_setting_data/setting_data.png)
+![setting_data image](https://raw.githubusercontent.com/louisnw01/lightweight-charts-python/main/examples/1_setting_data/setting_data.png)
 ___
 
 ### 2. Updating bars in real-time:
 
 ```python
 import pandas as pd
 from time import sleep
@@ -84,15 +84,15 @@
             chart.marker(text='The price crossed $20!')
             
         last_close = series['close']
         sleep(0.1)
 
 ```
 
-![live data gif](https://github.com/louisnw01/lightweight-charts-python/blob/main/examples/2_live_data/live_data.gif)
+![live data gif](https://github.com/louisnw01/lightweight-charts-python/blob/main/examples/2_live_data/live_data.gif?raw=true)
 ___
 
 ### 3. Updating bars from tick data in real-time:
 
 ```python
 import pandas as pd
 from time import sleep
@@ -114,15 +114,15 @@
     
     for i, tick in df2.iterrows():
         chart.update_from_tick(tick)
             
         sleep(0.3)
 
 ```
-![tick data gif](https://github.com/louisnw01/lightweight-charts-python/blob/main/examples/3_tick_data/tick_data.gif)
+![tick data gif](https://raw.githubusercontent.com/louisnw01/lightweight-charts-python/main/examples/3_tick_data/tick_data.gif)
 ___
 
 ### 4. Line Indicators:
 
 ```python
 import pandas as pd
 from lightweight_charts import Chart
@@ -148,15 +148,15 @@
     line = chart.create_line()
     sma_data = calculate_sma(df)
     line.set(sma_data)
     
     chart.show(block=True)
 
 ```
-![line indicators image](https://github.com/louisnw01/lightweight-charts-python/blob/main/examples/4_line_indicators/line_indicators.png)
+![line indicators image](https://raw.githubusercontent.com/louisnw01/lightweight-charts-python/main/examples/4_line_indicators/line_indicators.png)
 ___
 
 ### 5. Styling:
 
 ```python
 import pandas as pd
 from lightweight_charts import Chart
@@ -185,15 +185,15 @@
     chart.legend(visible=True, font_size=14)
 
     chart.set(df)
 
     chart.show(block=True)
 
 ```
-![styling image](https://github.com/louisnw01/lightweight-charts-python/blob/main/examples/5_styling/styling.png)
+![styling image](https://raw.githubusercontent.com/louisnw01/lightweight-charts-python/main/examples/5_styling/styling.png)
 ___
 
 ### 6. Callbacks:
 
 ```python
 import pandas as pd
 from lightweight_charts import Chart
@@ -211,20 +211,19 @@
     chart.set(df)
 
     chart.subscribe_click(on_click)
 
     chart.show(block=True)
 
 ```
-![callbacks gif](https://github.com/louisnw01/lightweight-charts-python/blob/main/examples/6_callbacks/callbacks.gif)
+![callbacks gif](https://raw.githubusercontent.com/louisnw01/lightweight-charts-python/main/examples/6_callbacks/callbacks.gif)
 ___
 
 [![Documentation](https://img.shields.io/badge/documentation-006ee3)](https://lightweight-charts-python.readthedocs.io/en/latest/docs.html)
 
 ___
 
 _This package is an independent creation and has not been endorsed, sponsored, or approved by TradingView. The author of this package does not have any official relationship with TradingView, and the package does not represent the views or opinions of TradingView._
 
 
 
 
-
```

### Comparing `lightweight_charts-1.0.6/README.md` & `lightweight_charts-1.0.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [![PyPi Release](https://img.shields.io/pypi/v/lightweight-charts?color=32a852&label=PyPi)](https://pypi.org/project/lightweight-charts/)
 [![Made with Python](https://img.shields.io/badge/Python-3.9+-c7a002?logo=python&logoColor=white)](https://python.org "Go to Python homepage")
 [![License](https://img.shields.io/github/license/louisnw01/lightweight-charts-python?color=9c2400)](https://github.com/louisnw01/lightweight-charts-python/blob/main/LICENSE)
 [![Documentation](https://img.shields.io/badge/documentation-006ee3)](https://lightweight-charts-python.readthedocs.io/en/latest/docs.html)
 
 
-![cover](cover.png)
+![cover](https://raw.githubusercontent.com/louisnw01/lightweight-charts-python/main/cover.png)
 
 lightweight-charts-python aims to provide a simple and pythonic way to access and implement [TradingView's Lightweight Charts](https://www.tradingview.com/lightweight-charts/).
 
 ## Installation
 ```
 pip install lightweight_charts
 ```
@@ -38,15 +38,15 @@
     # Columns: | time | open | high | low | close | volume (if volume is enabled) |
     df = pd.read_csv('ohlcv.csv')
     chart.set(df)
     
     chart.show(block=True)
 
 ```
-![setting_data image](https://github.com/louisnw01/lightweight-charts-python/blob/main/examples/1_setting_data/setting_data.png)
+![setting_data image](https://raw.githubusercontent.com/louisnw01/lightweight-charts-python/main/examples/1_setting_data/setting_data.png)
 ___
 
 ### 2. Updating bars in real-time:
 
 ```python
 import pandas as pd
 from time import sleep
@@ -72,15 +72,15 @@
             chart.marker(text='The price crossed $20!')
             
         last_close = series['close']
         sleep(0.1)
 
 ```
 
-![live data gif](https://github.com/louisnw01/lightweight-charts-python/blob/main/examples/2_live_data/live_data.gif)
+![live data gif](https://github.com/louisnw01/lightweight-charts-python/blob/main/examples/2_live_data/live_data.gif?raw=true)
 ___
 
 ### 3. Updating bars from tick data in real-time:
 
 ```python
 import pandas as pd
 from time import sleep
@@ -102,15 +102,15 @@
     
     for i, tick in df2.iterrows():
         chart.update_from_tick(tick)
             
         sleep(0.3)
 
 ```
-![tick data gif](https://github.com/louisnw01/lightweight-charts-python/blob/main/examples/3_tick_data/tick_data.gif)
+![tick data gif](https://raw.githubusercontent.com/louisnw01/lightweight-charts-python/main/examples/3_tick_data/tick_data.gif)
 ___
 
 ### 4. Line Indicators:
 
 ```python
 import pandas as pd
 from lightweight_charts import Chart
@@ -136,15 +136,15 @@
     line = chart.create_line()
     sma_data = calculate_sma(df)
     line.set(sma_data)
     
     chart.show(block=True)
 
 ```
-![line indicators image](https://github.com/louisnw01/lightweight-charts-python/blob/main/examples/4_line_indicators/line_indicators.png)
+![line indicators image](https://raw.githubusercontent.com/louisnw01/lightweight-charts-python/main/examples/4_line_indicators/line_indicators.png)
 ___
 
 ### 5. Styling:
 
 ```python
 import pandas as pd
 from lightweight_charts import Chart
@@ -173,15 +173,15 @@
     chart.legend(visible=True, font_size=14)
 
     chart.set(df)
 
     chart.show(block=True)
 
 ```
-![styling image](https://github.com/louisnw01/lightweight-charts-python/blob/main/examples/5_styling/styling.png)
+![styling image](https://raw.githubusercontent.com/louisnw01/lightweight-charts-python/main/examples/5_styling/styling.png)
 ___
 
 ### 6. Callbacks:
 
 ```python
 import pandas as pd
 from lightweight_charts import Chart
@@ -199,18 +199,17 @@
     chart.set(df)
 
     chart.subscribe_click(on_click)
 
     chart.show(block=True)
 
 ```
-![callbacks gif](https://github.com/louisnw01/lightweight-charts-python/blob/main/examples/6_callbacks/callbacks.gif)
+![callbacks gif](https://raw.githubusercontent.com/louisnw01/lightweight-charts-python/main/examples/6_callbacks/callbacks.gif)
 ___
 
 [![Documentation](https://img.shields.io/badge/documentation-006ee3)](https://lightweight-charts-python.readthedocs.io/en/latest/docs.html)
 
 ___
 
 _This package is an independent creation and has not been endorsed, sponsored, or approved by TradingView. The author of this package does not have any official relationship with TradingView, and the package does not represent the views or opinions of TradingView._
 
 
-
```

### Comparing `lightweight_charts-1.0.6/lightweight_charts/util.py` & `lightweight_charts-1.0.7/lightweight_charts/util.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,75 +17,60 @@
         super().__init__(message)
         self.msg = message
 
     def __str__(self):
         return f'{self.msg}'
 
 
+class IDGen(list):
+    def generate(self):
+        var = ''.join(choices(ascii_lowercase, k=8))
+        if var not in self:
+            self.append(var)
+            return var
+        self.generate()
+
+
 def _valid_color(string):
     if string[:3] == 'rgb' or string[:4] == 'rgba' or string[0] == '#':
         return True
     raise ColorError('Colors must be in the format of either rgb, rgba or hex.')
 
 
-LINE_TYPE = Literal['solid', 'dotted', 'dashed', 'large_dashed', 'sparse_dotted']
-
-POSITION = Literal['above', 'below', 'inside']
-
-SHAPE = Literal['arrow_up', 'arrow_down', 'circle', 'square']
-
-CROSSHAIR_MODE = Literal['normal', 'magnet']
+def _js_bool(b: bool): return 'true' if b is True else 'false' if b is False else None
 
-PRICE_SCALE_MODE = Literal['normal', 'logarithmic', 'percentage', 'index100']
 
+LINE_STYLE = Literal['solid', 'dotted', 'dashed', 'large_dashed', 'sparse_dotted']
 
-def _line_type(lt: LINE_TYPE):
-    return {
-        'solid': 'Solid',
-        'dotted': 'Dotted',
-        'dashed': 'Dashed',
-        'large_dashed': 'LargeDashed',
-        'sparse_dotted': 'SparseDotted',
-        None: None,
-    }[lt]
+MARKER_POSITION = Literal['above', 'below', 'inside']
 
+MARKER_SHAPE = Literal['arrow_up', 'arrow_down', 'circle', 'square']
 
-def _position(p: POSITION):
-    return {
-        'above': 'aboveBar',
-        'below': 'belowBar',
-        'inside': 'inBar',
-        None: None,
-    }[p]
-
+CROSSHAIR_MODE = Literal['normal', 'magnet']
 
-def _shape(shape: SHAPE):
-    return {
-        'arrow_up': 'arrowUp',
-        'arrow_down': 'arrowDown',
-        'circle': 'Circle',
-        'square': 'Square',
-        None: None,
-    }[shape]
+PRICE_SCALE_MODE = Literal['normal', 'logarithmic', 'percentage', 'index100']
 
 
-def _crosshair_mode(mode: CROSSHAIR_MODE): return mode.title() if mode else None
+def _line_style(line: LINE_STYLE):
+    js = 'LightweightCharts.LineStyle.'
+    return js+line[:line.index('_')].title() + line[line.index('_') + 1:].title() if '_' in line else js+line.title()
 
 
-def _js_bool(b: bool): return 'true' if b is True else 'false' if b is False else None
+def _crosshair_mode(mode: CROSSHAIR_MODE):
+    return f'LightweightCharts.CrosshairMode.{mode.title()}' if mode else None
 
 
 def _price_scale_mode(mode: PRICE_SCALE_MODE):
-    return 'IndexedTo100' if mode == 'index100' else mode.title() if mode else None
+    return f"LightweightCharts.PriceScaleMode.{'IndexedTo100' if mode == 'index100' else mode.title() if mode else None}"
 
 
-class IDGen:
-    def __init__(self):
-        self.list = []
+def _marker_shape(shape: MARKER_SHAPE):
+    return shape[:shape.index('_')]+shape[shape.index('_')+1:].title() if '_' in shape else shape.title()
 
-    def generate(self):
-        var = ''.join(choices(ascii_lowercase, k=8))
-        if var in self.list:
-            self.generate()
-        else:
-            self.list.append(var)
-            return var
+
+def _marker_position(p: MARKER_POSITION):
+    return {
+        'above': 'aboveBar',
+        'below': 'belowBar',
+        'inside': 'inBar',
+        None: None,
+    }[p]
```

### Comparing `lightweight_charts-1.0.6/lightweight_charts/widgets.py` & `lightweight_charts-1.0.7/lightweight_charts/widgets.py`

 * *Files 20% similar despite different names*

```diff
@@ -17,50 +17,37 @@
         try:
             self.webview: wx.html2.WebView = wx.html2.WebView.New(parent)
         except NameError:
             raise ModuleNotFoundError('wx.html2 was not found, and must be installed to use WxChart.')
 
         super().__init__(volume_enabled, inner_width=inner_width, inner_height=inner_height)
 
-        self.webview.AddScriptMessageHandler('wx_msg')
+        self._script_func = self.webview.RunScript
         self._js_api_code = 'window.wx_msg.postMessage'
-        self.webview.Bind(wx.html2.EVT_WEBVIEW_SCRIPT_MESSAGE_RECEIVED, lambda e: self._js_api.onClick(eval(e.GetString())))
 
+        self.webview.AddScriptMessageHandler('wx_msg')
+        self.webview.Bind(wx.html2.EVT_WEBVIEW_SCRIPT_MESSAGE_RECEIVED, lambda e: self._js_api.onClick(eval(e.GetString())))
         self.webview.Bind(wx.html2.EVT_WEBVIEW_LOADED, self._on_js_load)
         self.webview.SetPage(self._html, '')
+        self._create_chart()
 
-    def run_script(self, script): self.webview.RunScript(script)
-
-    def _on_js_load(self, e):
-        self.loaded = True
-        for func, args, kwargs in self.js_queue:
-            if 'SUB' in func:
-                c_id = args[0]
-                args = args[1:]
-                getattr(self._subcharts[c_id], func.replace('SUB', ''))(*args)
-            else:
-                getattr(self, func)(*args)
+    def _on_js_load(self, e): super()._on_js_load()
 
     def get_webview(self): return self.webview
 
 
 class QtChart(LWC):
     def __init__(self, widget=None, volume_enabled: bool = True, inner_width: float = 1.0, inner_height: float = 1.0):
         try:
             self.webview = QWebEngineView(widget)
         except NameError:
             raise ModuleNotFoundError('QWebEngineView was not found, and must be installed to use QtChart.')
-
         super().__init__(volume_enabled, inner_width=inner_width, inner_height=inner_height)
 
+        self._script_func = self.webview.page().runJavaScript
+
         self.webview.loadFinished.connect(self._on_js_load)
         self.webview.page().setHtml(self._html)
-
-    def run_script(self, script): self.webview.page().runJavaScript(script)
-
-    def _on_js_load(self):
-        self.loaded = True
-        for func, args, kwargs in self.js_queue:
-            getattr(super(), func)(*args, **kwargs)
+        self._create_chart()
 
     def get_webview(self): return self.webview
```

### Comparing `lightweight_charts-1.0.6/lightweight_charts.egg-info/PKG-INFO` & `lightweight_charts-1.0.7/lightweight_charts.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightweight-charts
-Version: 1.0.6
+Version: 1.0.7
 Summary: Python framework for TradingView's Lightweight Charts JavaScript library.
 Home-page: https://github.com/louisnw01/lightweight-charts-python
 Author: louisnw
 License: MIT
 Platform: UNKNOWN
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
@@ -14,15 +14,15 @@
 
 [![PyPi Release](https://img.shields.io/pypi/v/lightweight-charts?color=32a852&label=PyPi)](https://pypi.org/project/lightweight-charts/)
 [![Made with Python](https://img.shields.io/badge/Python-3.9+-c7a002?logo=python&logoColor=white)](https://python.org "Go to Python homepage")
 [![License](https://img.shields.io/github/license/louisnw01/lightweight-charts-python?color=9c2400)](https://github.com/louisnw01/lightweight-charts-python/blob/main/LICENSE)
 [![Documentation](https://img.shields.io/badge/documentation-006ee3)](https://lightweight-charts-python.readthedocs.io/en/latest/docs.html)
 
 
-![cover](cover.png)
+![cover](https://raw.githubusercontent.com/louisnw01/lightweight-charts-python/main/cover.png)
 
 lightweight-charts-python aims to provide a simple and pythonic way to access and implement [TradingView's Lightweight Charts](https://www.tradingview.com/lightweight-charts/).
 
 ## Installation
 ```
 pip install lightweight_charts
 ```
@@ -50,15 +50,15 @@
     # Columns: | time | open | high | low | close | volume (if volume is enabled) |
     df = pd.read_csv('ohlcv.csv')
     chart.set(df)
     
     chart.show(block=True)
 
 ```
-![setting_data image](https://github.com/louisnw01/lightweight-charts-python/blob/main/examples/1_setting_data/setting_data.png)
+![setting_data image](https://raw.githubusercontent.com/louisnw01/lightweight-charts-python/main/examples/1_setting_data/setting_data.png)
 ___
 
 ### 2. Updating bars in real-time:
 
 ```python
 import pandas as pd
 from time import sleep
@@ -84,15 +84,15 @@
             chart.marker(text='The price crossed $20!')
             
         last_close = series['close']
         sleep(0.1)
 
 ```
 
-![live data gif](https://github.com/louisnw01/lightweight-charts-python/blob/main/examples/2_live_data/live_data.gif)
+![live data gif](https://github.com/louisnw01/lightweight-charts-python/blob/main/examples/2_live_data/live_data.gif?raw=true)
 ___
 
 ### 3. Updating bars from tick data in real-time:
 
 ```python
 import pandas as pd
 from time import sleep
@@ -114,15 +114,15 @@
     
     for i, tick in df2.iterrows():
         chart.update_from_tick(tick)
             
         sleep(0.3)
 
 ```
-![tick data gif](https://github.com/louisnw01/lightweight-charts-python/blob/main/examples/3_tick_data/tick_data.gif)
+![tick data gif](https://raw.githubusercontent.com/louisnw01/lightweight-charts-python/main/examples/3_tick_data/tick_data.gif)
 ___
 
 ### 4. Line Indicators:
 
 ```python
 import pandas as pd
 from lightweight_charts import Chart
@@ -148,15 +148,15 @@
     line = chart.create_line()
     sma_data = calculate_sma(df)
     line.set(sma_data)
     
     chart.show(block=True)
 
 ```
-![line indicators image](https://github.com/louisnw01/lightweight-charts-python/blob/main/examples/4_line_indicators/line_indicators.png)
+![line indicators image](https://raw.githubusercontent.com/louisnw01/lightweight-charts-python/main/examples/4_line_indicators/line_indicators.png)
 ___
 
 ### 5. Styling:
 
 ```python
 import pandas as pd
 from lightweight_charts import Chart
@@ -185,15 +185,15 @@
     chart.legend(visible=True, font_size=14)
 
     chart.set(df)
 
     chart.show(block=True)
 
 ```
-![styling image](https://github.com/louisnw01/lightweight-charts-python/blob/main/examples/5_styling/styling.png)
+![styling image](https://raw.githubusercontent.com/louisnw01/lightweight-charts-python/main/examples/5_styling/styling.png)
 ___
 
 ### 6. Callbacks:
 
 ```python
 import pandas as pd
 from lightweight_charts import Chart
@@ -211,20 +211,19 @@
     chart.set(df)
 
     chart.subscribe_click(on_click)
 
     chart.show(block=True)
 
 ```
-![callbacks gif](https://github.com/louisnw01/lightweight-charts-python/blob/main/examples/6_callbacks/callbacks.gif)
+![callbacks gif](https://raw.githubusercontent.com/louisnw01/lightweight-charts-python/main/examples/6_callbacks/callbacks.gif)
 ___
 
 [![Documentation](https://img.shields.io/badge/documentation-006ee3)](https://lightweight-charts-python.readthedocs.io/en/latest/docs.html)
 
 ___
 
 _This package is an independent creation and has not been endorsed, sponsored, or approved by TradingView. The author of this package does not have any official relationship with TradingView, and the package does not represent the views or opinions of TradingView._
 
 
 
 
-
```

### Comparing `lightweight_charts-1.0.6/setup.py` & `lightweight_charts-1.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md', 'r', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='lightweight_charts',
-    version='1.0.6',
+    version='1.0.7',
     packages=find_packages(),
     python_requires='>=3.9',
     install_requires=[
         'pandas',
         'pywebview',
     ],
     author='louisnw',
```

