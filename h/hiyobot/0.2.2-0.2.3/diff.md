# Comparing `tmp/hiyobot-0.2.2.tar.gz` & `tmp/hiyobot-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hiyobot-0.2.2.tar", last modified: Sat May 13 13:22:40 2023, max compression
+gzip compressed data, was "hiyobot-0.2.3.tar", last modified: Sun May 21 11:17:24 2023, max compression
```

## Comparing `hiyobot-0.2.2.tar` & `hiyobot-0.2.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:22:40.843711 hiyobot-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-05-13 13:22:21.000000 hiyobot-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-05-13 13:22:40.843711 hiyobot-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1616 2023-05-13 13:22:21.000000 hiyobot-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:22:40.843711 hiyobot-0.2.2/hiyobot/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-13 13:22:21.000000 hiyobot-0.2.2/hiyobot/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:22:40.843711 hiyobot-0.2.2/hiyobot/hackchat/
--rw-r--r--   0 runner    (1001) docker     (123)     8700 2023-05-13 13:22:21.000000 hiyobot-0.2.2/hiyobot/hackchat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:22:40.843711 hiyobot-0.2.2/hiyobot/zhangchat/
--rw-r--r--   0 runner    (1001) docker     (123)     8830 2023-05-13 13:22:21.000000 hiyobot-0.2.2/hiyobot/zhangchat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-13 13:22:40.843711 hiyobot-0.2.2/hiyobot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-05-13 13:22:40.000000 hiyobot-0.2.2/hiyobot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-13 13:22:40.000000 hiyobot-0.2.2/hiyobot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-13 13:22:40.000000 hiyobot-0.2.2/hiyobot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-13 13:22:40.000000 hiyobot-0.2.2/hiyobot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-13 13:22:40.000000 hiyobot-0.2.2/hiyobot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-13 13:22:40.843711 hiyobot-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-05-13 13:22:21.000000 hiyobot-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:17:24.686437 hiyobot-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    18092 2023-05-21 11:17:10.000000 hiyobot-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-05-21 11:17:24.686437 hiyobot-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1766 2023-05-21 11:17:10.000000 hiyobot-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:17:24.686437 hiyobot-0.2.3/hiyobot/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-21 11:17:10.000000 hiyobot-0.2.3/hiyobot/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:17:24.686437 hiyobot-0.2.3/hiyobot/hackchat/
+-rw-r--r--   0 runner    (1001) docker     (123)     9025 2023-05-21 11:17:10.000000 hiyobot-0.2.3/hiyobot/hackchat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:17:24.686437 hiyobot-0.2.3/hiyobot/zhangchat/
+-rw-r--r--   0 runner    (1001) docker     (123)     9146 2023-05-21 11:17:10.000000 hiyobot-0.2.3/hiyobot/zhangchat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:17:24.686437 hiyobot-0.2.3/hiyobot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-05-21 11:17:24.000000 hiyobot-0.2.3/hiyobot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-21 11:17:24.000000 hiyobot-0.2.3/hiyobot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 11:17:24.000000 hiyobot-0.2.3/hiyobot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-21 11:17:24.000000 hiyobot-0.2.3/hiyobot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-21 11:17:24.000000 hiyobot-0.2.3/hiyobot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 11:17:24.686437 hiyobot-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1987 2023-05-21 11:17:10.000000 hiyobot-0.2.3/setup.py
```

### Comparing `hiyobot-0.2.2/LICENSE` & `hiyobot-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `hiyobot-0.2.2/PKG-INFO` & `hiyobot-0.2.3/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hiyobot
-Version: 0.2.2
+Version: 0.2.3
 Summary: A simple bot framework for Hack.chat.
 Home-page: https://github.com/Hiyoteam/hiyobot
 Author: MaggieLOL
 Author-email: tanhanzesnd@gmail.com
 License: GPL-2.0
 Keywords: bot hack.chat hack.chat-bot
 Classifier: Development Status :: 3 - Alpha
@@ -14,19 +14,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Hiyobot
 一个简单hack.chat机器人框架。    
 If your native language is not Chinese, please jump [here](https://deepl.com/) .     
-<img src="https://img.shields.io/badge/Powered%20By-Python-blue.svg"></img>     
-<img src="https://img.shields.io/badge/Powered%20By-websocket_client-blue.svg"></img>    
-<img src="https://img.shields.io/badge/Document%20version-0.0.2-green.svg"></img>
-<img src="https://img.shields.io/pypi/v/hiyobot"></img>     
-<img src="https://github.com/Hiyoteam/hiyobot/actions/workflows/python-publish.yml/badge.svg"></img>          
+<img src="https://img.shields.io/badge/Powered%20By-Python-blue.svg"></img> <img src="https://img.shields.io/badge/Powered%20By-websocket_client-blue.svg"></img> <img src="https://img.shields.io/badge/Document%20version-0.0.2-green.svg"></img> <img src="https://img.shields.io/pypi/v/hiyobot"></img> <img src="https://github.com/Hiyoteam/hiyobot/actions/workflows/python-publish.yml/badge.svg"></img> <img src="https://static.pepy.tech/personalized-badge/hiyobot?period=total&units=international_system&left_color=grey&right_color=blue&left_text=pypi%20downloads"></img>  
+
 
 # 如何安装？
 在你的控制台里面输入`pip3 install hiyobot --upgrade`，如果你使用镜像源，可能无法获取到最新的构建，需要加上`-i https://pypi.org/simple`的参数。输出应该是这样的：
 ```
 Collecting hiyobot
   Downloading hiyobot-<version>-py3-none-any.whl (8.3 kB)
 Requirement already satisfied: websocket-client in c:\users\administrator\appdata\local\programs\python\python310\lib\site-packages (from hiyobot) (1.3.2)
```

### Comparing `hiyobot-0.2.2/README.md` & `hiyobot-0.2.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 # Hiyobot
 一个简单hack.chat机器人框架。    
 If your native language is not Chinese, please jump [here](https://deepl.com/) .     
-<img src="https://img.shields.io/badge/Powered%20By-Python-blue.svg"></img>     
-<img src="https://img.shields.io/badge/Powered%20By-websocket_client-blue.svg"></img>    
-<img src="https://img.shields.io/badge/Document%20version-0.0.2-green.svg"></img>
-<img src="https://img.shields.io/pypi/v/hiyobot"></img>     
-<img src="https://github.com/Hiyoteam/hiyobot/actions/workflows/python-publish.yml/badge.svg"></img>          
+<img src="https://img.shields.io/badge/Powered%20By-Python-blue.svg"></img> <img src="https://img.shields.io/badge/Powered%20By-websocket_client-blue.svg"></img> <img src="https://img.shields.io/badge/Document%20version-0.0.2-green.svg"></img> <img src="https://img.shields.io/pypi/v/hiyobot"></img> <img src="https://github.com/Hiyoteam/hiyobot/actions/workflows/python-publish.yml/badge.svg"></img> <img src="https://static.pepy.tech/personalized-badge/hiyobot?period=total&units=international_system&left_color=grey&right_color=blue&left_text=pypi%20downloads"></img>  
+
 
 # 如何安装？
 在你的控制台里面输入`pip3 install hiyobot --upgrade`，如果你使用镜像源，可能无法获取到最新的构建，需要加上`-i https://pypi.org/simple`的参数。输出应该是这样的：
 ```
 Collecting hiyobot
   Downloading hiyobot-<version>-py3-none-any.whl (8.3 kB)
 Requirement already satisfied: websocket-client in c:\users\administrator\appdata\local\programs\python\python310\lib\site-packages (from hiyobot) (1.3.2)
@@ -20,8 +17,8 @@
 暂无
 
 # 注释
  - HiyoBot PYPI版本取决于Hack.chat子集版本。
  - HiyoBot子集使用： 如在Hack.chat编写机器人:`from hiyobot import hackchat as hcbot`, 在ZhangChat(chat.zhangsoft.eu.org or chat.zhangsoft.cf)编写机器人:`from hiyobot import zhangchat as zhcbot`
  - 目前支持的聊天室： Hack.chat(hackchat),ZhangChat(zhangchat)
  - 如其他子集使用方式与Hack.chat集不同，即开设子文档。（暂无）
- - 我们会始终欢迎您的PR/Issues！
+ - 我们会始终欢迎您的PR/Issues！
```

### Comparing `hiyobot-0.2.2/hiyobot/hackchat/__init__.py` & `hiyobot-0.2.3/hiyobot/hackchat/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,16 @@
-import websocket,ssl,json,threading,uuid,time,logging,re,traceback
+import websocket,ssl,json,threading,uuid,time,logging,re,traceback,inspect,asyncio
 from functools import wraps
-HIYOBOT_VERSION=(0,2,2)
+HIYOBOT_VERSION=(0,2,3)
 MAX_RECV_LOG_LIMIT=100 #0 for no limit
+def _isasync(func):
+    if inspect.isasyncgenfunction(func) or inspect.iscoroutinefunction(func):
+        return True
+    else:
+        return False
 class Bot:
     """
     Simple Hack.chat bot class.
     """
     def __init__(self,channel,nick,password=None,joinoncreate=True) -> None:
         """
         Init the Bot.
@@ -30,15 +35,18 @@
         Add a new event.
         """
         def decorate(func):
             @wraps(func)
             def wrapper(session, data,*args, **kwargs):
                 if matcher.match_all(data):
                     logging.debug(f"Matched! Function={func} Matcher={matcher}")
-                    return func(session=session, data=data, *args, **kwargs)
+                    if _isasync(func):
+                        return asyncio.run(func(session=session,data=data,*args,**kwargs))
+                    else:
+                        return func(session=session, data=data, *args, **kwargs)
                 else:
                     return None
             self.events.append(wrapper)
             return wrapper
         return decorate
     def _pingThread(self):
         while 1:
```

### Comparing `hiyobot-0.2.2/hiyobot/zhangchat/__init__.py` & `hiyobot-0.2.3/hiyobot/zhangchat/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,16 @@
-import websocket,ssl,json,threading,uuid,time,logging,re,traceback
+import websocket,ssl,json,threading,uuid,time,logging,re,traceback,inspect,asyncio
 from functools import wraps
-HIYOBOT_VERSION=(0,2,2)
+HIYOBOT_VERSION=(0,2,3)
 MAX_RECV_LOG_LIMIT=100 #0 for no limit
+def _isasync(func):
+    if inspect.isasyncgenfunction(func) or inspect.iscoroutinefunction(func):
+        return True
+    else:
+        return False
 class Bot:
     """
     Simple Hack.chat bot class.
     """
     def __init__(self,channel,nick,password=None,joinoncreate=True) -> None:
         """
         Init the Bot.
@@ -28,17 +33,20 @@
     def on(self,matcher):
         """
         Add a new event.
         """
         def decorate(func):
             @wraps(func)
             def wrapper(session, data,*args, **kwargs):
-                if matcher.match_all(data.__dict__):
+                if matcher.match_all(data):
                     logging.debug(f"Matched! Function={func} Matcher={matcher}")
-                    return func(session=session, data=data, *args, **kwargs)
+                    if _isasync(func):
+                        return asyncio.run(func(session=session,data=data,*args,**kwargs))
+                    else:
+                        return func(session=session, data=data, *args, **kwargs)
                 else:
                     return None
             self.events.append(wrapper)
             return wrapper
         return decorate
     def _pingThread(self):
         while 1:
```

### Comparing `hiyobot-0.2.2/hiyobot.egg-info/PKG-INFO` & `hiyobot-0.2.3/hiyobot.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hiyobot
-Version: 0.2.2
+Version: 0.2.3
 Summary: A simple bot framework for Hack.chat.
 Home-page: https://github.com/Hiyoteam/hiyobot
 Author: MaggieLOL
 Author-email: tanhanzesnd@gmail.com
 License: GPL-2.0
 Keywords: bot hack.chat hack.chat-bot
 Classifier: Development Status :: 3 - Alpha
@@ -14,19 +14,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Hiyobot
 一个简单hack.chat机器人框架。    
 If your native language is not Chinese, please jump [here](https://deepl.com/) .     
-<img src="https://img.shields.io/badge/Powered%20By-Python-blue.svg"></img>     
-<img src="https://img.shields.io/badge/Powered%20By-websocket_client-blue.svg"></img>    
-<img src="https://img.shields.io/badge/Document%20version-0.0.2-green.svg"></img>
-<img src="https://img.shields.io/pypi/v/hiyobot"></img>     
-<img src="https://github.com/Hiyoteam/hiyobot/actions/workflows/python-publish.yml/badge.svg"></img>          
+<img src="https://img.shields.io/badge/Powered%20By-Python-blue.svg"></img> <img src="https://img.shields.io/badge/Powered%20By-websocket_client-blue.svg"></img> <img src="https://img.shields.io/badge/Document%20version-0.0.2-green.svg"></img> <img src="https://img.shields.io/pypi/v/hiyobot"></img> <img src="https://github.com/Hiyoteam/hiyobot/actions/workflows/python-publish.yml/badge.svg"></img> <img src="https://static.pepy.tech/personalized-badge/hiyobot?period=total&units=international_system&left_color=grey&right_color=blue&left_text=pypi%20downloads"></img>  
+
 
 # 如何安装？
 在你的控制台里面输入`pip3 install hiyobot --upgrade`，如果你使用镜像源，可能无法获取到最新的构建，需要加上`-i https://pypi.org/simple`的参数。输出应该是这样的：
 ```
 Collecting hiyobot
   Downloading hiyobot-<version>-py3-none-any.whl (8.3 kB)
 Requirement already satisfied: websocket-client in c:\users\administrator\appdata\local\programs\python\python310\lib\site-packages (from hiyobot) (1.3.2)
```

### Comparing `hiyobot-0.2.2/setup.py` & `hiyobot-0.2.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='hiyobot', # 你的项目名称
-    version="0.2.2", # 你的项目版本
+    version="0.2.3", # 你的项目版本
     description='A simple bot framework for Hack.chat.', # 你的项目简介
     long_description=open('README.md').read(), # 你的项目详细介绍，一般从README.md文件中读取
     long_description_content_type='text/markdown', # 你的项目详细介绍的格式，一般为markdown格式
     url='https://github.com/Hiyoteam/hiyobot', # 你的项目主页，一般为github仓库地址
     author='MaggieLOL', # 你的姓名或者团队名称
     author_email='tanhanzesnd@gmail.com', # 你的邮箱或者团队邮箱
     license='GPL-2.0', # 你的项目使用的许可证，一般为MIT或者其他开源许可证
```

