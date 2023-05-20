# Comparing `tmp/aiotieba-reviewer-0.1.8.tar.gz` & `tmp/aiotieba-reviewer-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiotieba-reviewer-0.1.8.tar", last modified: Wed May  3 00:53:43 2023, max compression
+gzip compressed data, was "aiotieba-reviewer-0.2.0.tar", last modified: Sat May 20 23:39:46 2023, max compression
```

## Comparing `aiotieba-reviewer-0.1.8.tar` & `aiotieba-reviewer-0.2.0.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:53:43.238401 aiotieba-reviewer-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-03 00:53:23.000000 aiotieba-reviewer-0.1.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-05-03 00:53:43.234401 aiotieba-reviewer-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-05-03 00:53:23.000000 aiotieba-reviewer-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:53:43.230401 aiotieba-reviewer-0.1.8/aiotieba_reviewer/
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-03 00:53:23.000000 aiotieba-reviewer-0.1.8/aiotieba_reviewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-03 00:53:23.000000 aiotieba-reviewer-0.1.8/aiotieba_reviewer/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-03 00:53:23.000000 aiotieba-reviewer-0.1.8/aiotieba_reviewer/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    30093 2023-05-03 00:53:23.000000 aiotieba-reviewer-0.1.8/aiotieba_reviewer/database.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-03 00:53:23.000000 aiotieba-reviewer-0.1.8/aiotieba_reviewer/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     6396 2023-05-03 00:53:23.000000 aiotieba-reviewer-0.1.8/aiotieba_reviewer/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-05-03 00:53:23.000000 aiotieba-reviewer-0.1.8/aiotieba_reviewer/imgproc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-03 00:53:23.000000 aiotieba-reviewer-0.1.8/aiotieba_reviewer/perf_stat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-03 00:53:23.000000 aiotieba-reviewer-0.1.8/aiotieba_reviewer/punish.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:53:43.234401 aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-03 00:53:23.000000 aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:53:43.234401 aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/comment/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-03 00:53:23.000000 aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/comment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-05-03 00:53:23.000000 aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/comment/checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-03 00:53:23.000000 aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/comment/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:53:43.234401 aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/comments/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-03 00:53:23.000000 aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/comments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-03 00:53:23.000000 aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/comments/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-03 00:53:23.000000 aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/comments/producer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-05-03 00:53:23.000000 aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/comments/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     5384 2023-05-03 00:53:23.000000 aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/entry.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:53:43.234401 aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/post/
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-03 00:53:23.000000 aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/post/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-03 00:53:23.000000 aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/post/checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-03 00:53:23.000000 aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/post/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:53:43.234401 aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/posts/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-03 00:53:23.000000 aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/posts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-03 00:53:23.000000 aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/posts/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-05-03 00:53:23.000000 aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/posts/producer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-05-03 00:53:23.000000 aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/posts/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:53:43.234401 aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/thread/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-03 00:53:23.000000 aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/thread/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-05-03 00:53:23.000000 aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/thread/checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-05-03 00:53:23.000000 aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/thread/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:53:43.234401 aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/threads/
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-03 00:53:23.000000 aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/threads/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-03 00:53:23.000000 aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/threads/filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-03 00:53:23.000000 aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/threads/producer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-05-03 00:53:23.000000 aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/threads/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-03 00:53:23.000000 aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/user_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-03 00:53:23.000000 aiotieba-reviewer-0.1.8/aiotieba_reviewer/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:53:43.234401 aiotieba-reviewer-0.1.8/aiotieba_reviewer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-05-03 00:53:43.000000 aiotieba-reviewer-0.1.8/aiotieba_reviewer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-05-03 00:53:43.000000 aiotieba-reviewer-0.1.8/aiotieba_reviewer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 00:53:43.000000 aiotieba-reviewer-0.1.8/aiotieba_reviewer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-03 00:53:43.000000 aiotieba-reviewer-0.1.8/aiotieba_reviewer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-03 00:53:43.000000 aiotieba-reviewer-0.1.8/aiotieba_reviewer.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 00:53:43.234401 aiotieba-reviewer-0.1.8/examples/
--rw-r--r--   0 runner    (1001) docker     (123)    24229 2023-05-03 00:53:23.000000 aiotieba-reviewer-0.1.8/examples/cmd_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4124 2023-05-03 00:53:23.000000 aiotieba-reviewer-0.1.8/examples/reviewer_example.py
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-03 00:53:23.000000 aiotieba-reviewer-0.1.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 00:53:43.238401 aiotieba-reviewer-0.1.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:39:46.486733 aiotieba-reviewer-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-20 23:39:30.000000 aiotieba-reviewer-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-05-20 23:39:46.486733 aiotieba-reviewer-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2562 2023-05-20 23:39:30.000000 aiotieba-reviewer-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:39:46.478733 aiotieba-reviewer-0.2.0/aiotieba_reviewer/
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-20 23:39:30.000000 aiotieba-reviewer-0.2.0/aiotieba_reviewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-20 23:39:30.000000 aiotieba-reviewer-0.2.0/aiotieba_reviewer/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-20 23:39:30.000000 aiotieba-reviewer-0.2.0/aiotieba_reviewer/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30220 2023-05-20 23:39:30.000000 aiotieba-reviewer-0.2.0/aiotieba_reviewer/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-05-20 23:39:30.000000 aiotieba-reviewer-0.2.0/aiotieba_reviewer/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6638 2023-05-20 23:39:30.000000 aiotieba-reviewer-0.2.0/aiotieba_reviewer/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2681 2023-05-20 23:39:30.000000 aiotieba-reviewer-0.2.0/aiotieba_reviewer/imgproc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-20 23:39:30.000000 aiotieba-reviewer-0.2.0/aiotieba_reviewer/perf_stat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-20 23:39:30.000000 aiotieba-reviewer-0.2.0/aiotieba_reviewer/punish.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:39:46.482733 aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-20 23:39:30.000000 aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:39:46.482733 aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/comment/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-20 23:39:30.000000 aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/comment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-05-20 23:39:30.000000 aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/comment/checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1111 2023-05-20 23:39:30.000000 aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/comment/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:39:46.482733 aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/comments/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-20 23:39:30.000000 aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/comments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-20 23:39:30.000000 aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/comments/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-20 23:39:30.000000 aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/comments/producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-05-20 23:39:30.000000 aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/comments/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5659 2023-05-20 23:39:30.000000 aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:39:46.482733 aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/post/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-20 23:39:30.000000 aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/post/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1990 2023-05-20 23:39:30.000000 aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/post/checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1271 2023-05-20 23:39:30.000000 aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/post/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:39:46.482733 aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/posts/
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-20 23:39:30.000000 aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/posts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-20 23:39:30.000000 aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/posts/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1574 2023-05-20 23:39:30.000000 aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/posts/producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-05-20 23:39:30.000000 aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/posts/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:39:46.482733 aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/thread/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-20 23:39:30.000000 aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/thread/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-05-20 23:39:30.000000 aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/thread/checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1909 2023-05-20 23:39:30.000000 aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/thread/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:39:46.482733 aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/threads/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-20 23:39:30.000000 aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/threads/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-20 23:39:30.000000 aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/threads/filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-20 23:39:30.000000 aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/threads/producer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-05-20 23:39:30.000000 aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/threads/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-20 23:39:30.000000 aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/user_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-20 23:39:30.000000 aiotieba-reviewer-0.2.0/aiotieba_reviewer/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:39:46.482733 aiotieba-reviewer-0.2.0/aiotieba_reviewer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-05-20 23:39:46.000000 aiotieba-reviewer-0.2.0/aiotieba_reviewer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-05-20 23:39:46.000000 aiotieba-reviewer-0.2.0/aiotieba_reviewer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-20 23:39:46.000000 aiotieba-reviewer-0.2.0/aiotieba_reviewer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-20 23:39:46.000000 aiotieba-reviewer-0.2.0/aiotieba_reviewer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-20 23:39:46.000000 aiotieba-reviewer-0.2.0/aiotieba_reviewer.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-20 23:39:46.482733 aiotieba-reviewer-0.2.0/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    24244 2023-05-20 23:39:30.000000 aiotieba-reviewer-0.2.0/examples/cmd_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4070 2023-05-20 23:39:30.000000 aiotieba-reviewer-0.2.0/examples/reviewer_example.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-20 23:39:30.000000 aiotieba-reviewer-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-20 23:39:46.486733 aiotieba-reviewer-0.2.0/setup.cfg
```

### Comparing `aiotieba-reviewer-0.1.8/LICENSE` & `aiotieba-reviewer-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.1.8/PKG-INFO` & `aiotieba-reviewer-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiotieba-reviewer
-Version: 0.1.8
+Version: 0.2.0
 Summary: Reviewer Framework based on aiotieba
 Author-email: Starry-OvO <starry.qvq@gmail.com>
 Project-URL: Repository, https://github.com/Starry-OvO/aiotieba-reviewer/
 Project-URL: Documentation, https://review.aiotieba.cc/
 Keywords: baidu,tieba
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AsyncIO
@@ -43,26 +43,29 @@
 
 ## 教程
 
 [**云审查教程**](https://review.aiotieba.cc/tutorial/reviewer/)
 
 ## 客户名单
 
-*2023.05.02更新*
+*2023.05.20更新*
 
 |      吧名      | 关注用户数 | 最近24天日均访问量 | 日均主题帖数 | 日均回复数 |
 | :------------: | :--------: | :----------------: | :----------: | :--------: |
-|    抗压背锅    | 4,942,121  |      994,512       |    2,120     |   77,218   |
-|     孙笑川     | 3,990,805  |      738,723       |    5,832     |  260,811   |
-|    原神内鬼    |  589,938   |      492,120       |    1,122     |   36,464   |
-|      憨批      |   12,647   |      123,632       |    3,807     |   65,148   |
-|    lol半价     | 2,076,007  |       63,190       |     202      |   9,368    |
-|    天堂鸡汤    |  352,324   |       17,699       |     141      |   4,993    |
-|     vtuber     |  224,264   |       14,078       |     112      |   1,731    |
-|      嘉然      |   61,138   |       11,869       |      84      |   1,139    |
-| vtuber自由讨论 |   17,221   |       1,181        |      1       |     15     |
+|    抗压背锅    | 4,988,625  |      719,584       |    1,314     |   58,553   |
+|     孙笑川     | 4,073,427  |      645,815       |    5,241     |  224,603   |
+|    原神内鬼    |  594,645   |      376,348       |     787      |   28,587   |
+|      憨批      |   17,165   |      125,894       |    3,699     |   62,855   |
+|      禾野      |  363,088   |      106,555       |     966      |   8,602    |
+|    lol半价     | 2,078,647  |       68,593       |     258      |   22,063   |
+|      宫漫      | 1,597,685  |       18,857       |      70      |   1,110    |
+|    天堂鸡汤    |  357,856   |       16,914       |     126      |   4,848    |
+|     vtuber     |  224,576   |       15,538       |     108      |   1,982    |
+|      嘉然      |   61,135   |       10,796       |      76      |    990     |
+|    元气骑士    |  273,274   |       4,298        |      49      |    500     |
+| vtuber自由讨论 |   17,214   |       1,053        |      1       |     13     |
 
 ## 友情链接
 
 + [TiebaManager（吧务管理器 有用户界面）](https://github.com/dog194/TiebaManager)
 + [TiebaLite（第三方安卓客户端）](https://github.com/HuanCheng65/TiebaLite/tree/4.0-dev)
 + [贴吧protobuf定义文件合集](https://github.com/n0099/tbclient.protobuf)
```

### Comparing `aiotieba-reviewer-0.1.8/README.md` & `aiotieba-reviewer-0.2.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -21,26 +21,29 @@
 
 ## 教程
 
 [**云审查教程**](https://review.aiotieba.cc/tutorial/reviewer/)
 
 ## 客户名单
 
-*2023.05.02更新*
+*2023.05.20更新*
 
 |      吧名      | 关注用户数 | 最近24天日均访问量 | 日均主题帖数 | 日均回复数 |
 | :------------: | :--------: | :----------------: | :----------: | :--------: |
-|    抗压背锅    | 4,942,121  |      994,512       |    2,120     |   77,218   |
-|     孙笑川     | 3,990,805  |      738,723       |    5,832     |  260,811   |
-|    原神内鬼    |  589,938   |      492,120       |    1,122     |   36,464   |
-|      憨批      |   12,647   |      123,632       |    3,807     |   65,148   |
-|    lol半价     | 2,076,007  |       63,190       |     202      |   9,368    |
-|    天堂鸡汤    |  352,324   |       17,699       |     141      |   4,993    |
-|     vtuber     |  224,264   |       14,078       |     112      |   1,731    |
-|      嘉然      |   61,138   |       11,869       |      84      |   1,139    |
-| vtuber自由讨论 |   17,221   |       1,181        |      1       |     15     |
+|    抗压背锅    | 4,988,625  |      719,584       |    1,314     |   58,553   |
+|     孙笑川     | 4,073,427  |      645,815       |    5,241     |  224,603   |
+|    原神内鬼    |  594,645   |      376,348       |     787      |   28,587   |
+|      憨批      |   17,165   |      125,894       |    3,699     |   62,855   |
+|      禾野      |  363,088   |      106,555       |     966      |   8,602    |
+|    lol半价     | 2,078,647  |       68,593       |     258      |   22,063   |
+|      宫漫      | 1,597,685  |       18,857       |      70      |   1,110    |
+|    天堂鸡汤    |  357,856   |       16,914       |     126      |   4,848    |
+|     vtuber     |  224,576   |       15,538       |     108      |   1,982    |
+|      嘉然      |   61,135   |       10,796       |      76      |    990     |
+|    元气骑士    |  273,274   |       4,298        |      49      |    500     |
+| vtuber自由讨论 |   17,214   |       1,053        |      1       |     13     |
 
 ## 友情链接
 
 + [TiebaManager（吧务管理器 有用户界面）](https://github.com/dog194/TiebaManager)
 + [TiebaLite（第三方安卓客户端）](https://github.com/HuanCheng65/TiebaLite/tree/4.0-dev)
 + [贴吧protobuf定义文件合集](https://github.com/n0099/tbclient.protobuf)
```

### Comparing `aiotieba-reviewer-0.1.8/aiotieba_reviewer/client.py` & `aiotieba-reviewer-0.2.0/aiotieba_reviewer/client.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.1.8/aiotieba_reviewer/database.py` & `aiotieba-reviewer-0.2.0/aiotieba_reviewer/database.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,22 +20,25 @@
     """
 
     def decorator(func):
         async def wrapper(self: "MySQLDB", *args, **kwargs):
             try:
                 return await func(self, *args, **kwargs)
             except aiomysql.Error as err:
-                code = err.args[0]
-                if code == 2003:
-                    LOG().warning("无法连接数据库 将尝试自动建库")
-                    await self.create_database()
-                    await create_table_func(self)
-                elif code == 1146:
-                    LOG().warning("表不存在 将尝试自动建表")
-                    await create_table_func(self)
+                try:
+                    code = err.args[0]
+                    if code == 2003:
+                        LOG().warning("无法连接数据库 将尝试自动建库")
+                        await self.create_database()
+                        await create_table_func(self)
+                    elif code == 1146:
+                        LOG().warning("表不存在 将尝试自动建表")
+                        await create_table_func(self)
+                except Exception:
+                    pass
             return default_ret
 
         return wrapper
 
     return decorator
 
 
@@ -66,15 +69,15 @@
         self.fname = fname
         self._pool: aiomysql.Pool = None
 
     async def __aenter__(self) -> "MySQLDB":
         await self._create_pool()
         return self
 
-    async def __aexit__(self, exc_type, exc_val, exc_tb) -> None:
+    async def __aexit__(self, exc_type=None, exc_val=None, exc_tb=None) -> None:
         if self._pool is not None:
             self._pool.close()
             await self._pool.wait_closed()
 
     async def _create_pool(self) -> None:
         """
         创建连接池
```

### Comparing `aiotieba-reviewer-0.1.8/aiotieba_reviewer/executor.py` & `aiotieba-reviewer-0.2.0/aiotieba_reviewer/executor.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 import asyncio
-from typing import Awaitable, Callable, Optional, Protocol
+from typing import AsyncContextManager, Awaitable, Callable, Optional, Protocol
 
 from aiotieba import LOG
 
 from .client import get_client, get_fname
 from .enums import Ops
 from .punish import Punish
 
 
-class TypeDeleteList(Protocol):
+class TypeDeleteList(AsyncContextManager, Protocol):
     async def append(self, pid: int) -> None:
-        pass
+        ...
+
+    async def group_punish_executor(self, punish: Punish) -> Optional[Punish]:
+        ...
 
 
 class DeleteList(object):
     """
     待删除pid的列表
 
     execute_timeout (float): 插入元素后，若发现没有计划中的删除任务
@@ -35,101 +38,92 @@
 
     def __init__(self, execute_timeout: float = 10.0, maxlen=30) -> None:
         self._execute_timeout = execute_timeout
         self._maxlen = maxlen
         self._delete_task: asyncio.Task = None
         self._pids = []
 
+    async def __aenter__(self) -> "DeleteList":
+        return self
+
+    async def __aexit__(self, exc_type=None, exc_val=None, exc_tb=None) -> None:
+        if self._pids:
+            await self._delete_30()
+
     async def append(self, pid: int) -> None:
         """
         将一个pid推入待删除列表
 
         Args:
             pid (int)
         """
 
         self._pids.append(pid)
 
         if len(self._pids) >= self._maxlen:
             if not self._delete_task.done():
                 self._delete_task.cancel()
-            await self._delete_all()
+            await self._delete_30()
         else:
             if self._delete_task is None or self._delete_task.done():
                 self._delete_task = asyncio.create_task(self._delete_all_after_sleep())
 
-    async def _delete_all(self) -> None:
+    async def _delete_30(self) -> None:
         client = await get_client()
         pids = self._pids[:30]
         self._pids = self._pids[30:]
         await client.del_posts(get_fname(), pids)
 
     async def _delete_all_after_sleep(self) -> None:
         try:
             await asyncio.sleep(self._execute_timeout)
-            await self._delete_all()
+            await self._delete_30()
         except asyncio.CancelledError:
             return
 
+    async def group_punish_executor(self, punish: Punish) -> Optional[Punish]:
+        if day := punish.day:
+            client = await get_client()
+            await client.block(get_fname(), punish.obj.user.portrait, day=day, reason=punish.note)
 
-delete_list = DeleteList()
-
-
-def set_delete_list(_delete_list: TypeDeleteList) -> None:
-    """
-    设置删除列表
-
-    Args:
-        delete_list (TypeDeleteList)
-    """
-
-    global delete_list
-    delete_list = _delete_list
+        op = punish.op
+        if op == Ops.NORMAL:
+            return
+        if op == Ops.DELETE:
+            LOG().info(
+                f"Del {punish.obj.__class__.__name__}. text={punish.obj.text} user={punish.obj.user!r} note={punish.note}"
+            )
+            await self.append(punish.obj.pid)
+            return
+        if op == Ops.DEBUG:
+            LOG().info(
+                f"Debug {punish.obj.__class__.__name__}. obj={punish.obj} user={punish.obj.user!r} note={punish.note}"
+            )
+            return
+        if op == Ops.HIDE:
+            LOG().info(
+                f"Hide {punish.obj.__class__.__name__}. text={punish.obj.text} user={punish.obj.user!r} note={punish.note}"
+            )
+            client = await get_client()
+            await client.hide_thread(get_fname(), punish.obj.tid)
+            return
+        if op & Ops.PARENT == Ops.PARENT:
+            op &= ~Ops.PARENT
+            punish.op = op
+            return punish
+        if op & Ops.GRANDPARENT == Ops.GRANDPARENT:
+            op &= ~Ops.GRANDPARENT
+            op &= Ops.PARENT
+            punish.op = op
+            return punish
 
 
 TypePunishExecutor = Callable[[Punish], Awaitable[Optional[Punish]]]
 
 
-async def group_punish_executor(punish: Punish) -> Optional[Punish]:
-    if day := punish.day:
-        client = await get_client()
-        await client.block(get_fname(), punish.obj.user.portrait, day=day, reason=punish.note)
-
-    op = punish.op
-    if op == Ops.NORMAL:
-        return
-    if op == Ops.DELETE:
-        LOG().info(
-            f"Del {punish.obj.__class__.__name__}. text={punish.obj.text} user={punish.obj.user!r} note={punish.note}"
-        )
-        await delete_list.append(punish.obj.pid)
-        return
-    if op == Ops.DEBUG:
-        LOG().info(
-            f"Debug {punish.obj.__class__.__name__}. obj={punish.obj} user={punish.obj.user!r} note={punish.note}"
-        )
-        return
-    if op == Ops.HIDE:
-        LOG().info(
-            f"Hide {punish.obj.__class__.__name__}. text={punish.obj.text} user={punish.obj.user!r} note={punish.note}"
-        )
-        client = await get_client()
-        await client.hide_thread(get_fname(), punish.obj.tid)
-        return
-    if op & Ops.PARENT == Ops.PARENT:
-        op &= ~Ops.PARENT
-        punish.op = op
-        return punish
-    if op & Ops.GRANDPARENT == Ops.GRANDPARENT:
-        op &= ~Ops.GRANDPARENT
-        op &= Ops.PARENT
-        punish.op = op
-        return punish
-
-
 async def default_punish_executor(punish: Punish) -> Optional[Punish]:
     if day := punish.day:
         client = await get_client()
         await client.block(get_fname(), punish.obj.user.portrait, day=day, reason=punish.note)
 
     op = punish.op
     if op == Ops.NORMAL:
```

### Comparing `aiotieba-reviewer-0.1.8/aiotieba_reviewer/imgproc.py` & `aiotieba-reviewer-0.2.0/aiotieba_reviewer/imgproc.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.1.8/aiotieba_reviewer/perf_stat.py` & `aiotieba-reviewer-0.2.0/aiotieba_reviewer/perf_stat.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.1.8/aiotieba_reviewer/punish.py` & `aiotieba-reviewer-0.2.0/aiotieba_reviewer/punish.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/comment/checker.py` & `aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/comment/checker.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/comment/runner.py` & `aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/comment/runner.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/comments/producer.py` & `aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/comments/producer.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/comments/runner.py` & `aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/comments/runner.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/entry.py` & `aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/entry.py`

 * *Files 4% similar despite different names*

```diff
@@ -125,23 +125,36 @@
             for _comment in comments:
                 if _comment.pid == pid:
                     comment.checker.set_checker(True, False)(comment.checker.ori_checker)
                     return await comment.checker.checker(_comment)
             LOG().warning("Comment not exist")
 
 
-@contextlib.contextmanager
-def no_test(use_del_list=False) -> None:
+@contextlib.asynccontextmanager
+async def no_test(use_del_list=False) -> None:
     """
     取消测试模式以实际执行删封
 
     Args:
         use_del_list (bool): 是否使用更节省带宽但延迟更高的批量删除模式. Defaults to False.
     """
 
-    executor.punish_executor = executor.group_punish_executor if use_del_list else executor.default_punish_executor
     thread.runner.set_thread_runner(False)(thread.runner.ori_runner)
     threads.runner.set_threads_runner(False)(threads.runner.ori_runner)
-    yield
+
+    try:
+        if use_del_list:
+            async with executor.DeleteList() as del_list:
+                executor.punish_executor = del_list.group_punish_executor
+                yield
+        else:
+            executor.punish_executor = executor.default_punish_executor
+            yield
+
+    except Exception:
+        import traceback
+
+        LOG().critical(traceback.format_exc())
+
     executor.punish_executor = executor.default_punish_executor_test
     thread.runner.set_thread_runner(True)(thread.runner.ori_runner)
     threads.runner.set_threads_runner(True)(threads.runner.ori_runner)
```

### Comparing `aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/post/checker.py` & `aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/post/checker.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/post/runner.py` & `aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/post/runner.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/posts/producer.py` & `aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/posts/producer.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/posts/runner.py` & `aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/posts/runner.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/thread/checker.py` & `aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/thread/checker.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/thread/runner.py` & `aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/thread/runner.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/threads/producer.py` & `aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/threads/producer.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/threads/runner.py` & `aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/threads/runner.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.1.8/aiotieba_reviewer/reviewer/user_checker.py` & `aiotieba-reviewer-0.2.0/aiotieba_reviewer/reviewer/user_checker.py`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.1.8/aiotieba_reviewer.egg-info/PKG-INFO` & `aiotieba-reviewer-0.2.0/aiotieba_reviewer.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiotieba-reviewer
-Version: 0.1.8
+Version: 0.2.0
 Summary: Reviewer Framework based on aiotieba
 Author-email: Starry-OvO <starry.qvq@gmail.com>
 Project-URL: Repository, https://github.com/Starry-OvO/aiotieba-reviewer/
 Project-URL: Documentation, https://review.aiotieba.cc/
 Keywords: baidu,tieba
 Classifier: Development Status :: 4 - Beta
 Classifier: Framework :: AsyncIO
@@ -43,26 +43,29 @@
 
 ## 教程
 
 [**云审查教程**](https://review.aiotieba.cc/tutorial/reviewer/)
 
 ## 客户名单
 
-*2023.05.02更新*
+*2023.05.20更新*
 
 |      吧名      | 关注用户数 | 最近24天日均访问量 | 日均主题帖数 | 日均回复数 |
 | :------------: | :--------: | :----------------: | :----------: | :--------: |
-|    抗压背锅    | 4,942,121  |      994,512       |    2,120     |   77,218   |
-|     孙笑川     | 3,990,805  |      738,723       |    5,832     |  260,811   |
-|    原神内鬼    |  589,938   |      492,120       |    1,122     |   36,464   |
-|      憨批      |   12,647   |      123,632       |    3,807     |   65,148   |
-|    lol半价     | 2,076,007  |       63,190       |     202      |   9,368    |
-|    天堂鸡汤    |  352,324   |       17,699       |     141      |   4,993    |
-|     vtuber     |  224,264   |       14,078       |     112      |   1,731    |
-|      嘉然      |   61,138   |       11,869       |      84      |   1,139    |
-| vtuber自由讨论 |   17,221   |       1,181        |      1       |     15     |
+|    抗压背锅    | 4,988,625  |      719,584       |    1,314     |   58,553   |
+|     孙笑川     | 4,073,427  |      645,815       |    5,241     |  224,603   |
+|    原神内鬼    |  594,645   |      376,348       |     787      |   28,587   |
+|      憨批      |   17,165   |      125,894       |    3,699     |   62,855   |
+|      禾野      |  363,088   |      106,555       |     966      |   8,602    |
+|    lol半价     | 2,078,647  |       68,593       |     258      |   22,063   |
+|      宫漫      | 1,597,685  |       18,857       |      70      |   1,110    |
+|    天堂鸡汤    |  357,856   |       16,914       |     126      |   4,848    |
+|     vtuber     |  224,576   |       15,538       |     108      |   1,982    |
+|      嘉然      |   61,135   |       10,796       |      76      |    990     |
+|    元气骑士    |  273,274   |       4,298        |      49      |    500     |
+| vtuber自由讨论 |   17,214   |       1,053        |      1       |     13     |
 
 ## 友情链接
 
 + [TiebaManager（吧务管理器 有用户界面）](https://github.com/dog194/TiebaManager)
 + [TiebaLite（第三方安卓客户端）](https://github.com/HuanCheng65/TiebaLite/tree/4.0-dev)
 + [贴吧protobuf定义文件合集](https://github.com/n0099/tbclient.protobuf)
```

### Comparing `aiotieba-reviewer-0.1.8/aiotieba_reviewer.egg-info/SOURCES.txt` & `aiotieba-reviewer-0.2.0/aiotieba_reviewer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aiotieba-reviewer-0.1.8/examples/cmd_handler.py` & `aiotieba-reviewer-0.2.0/examples/cmd_handler.py`

 * *Files 0% similar despite different names*

```diff
@@ -245,15 +245,15 @@
         self.admins = {}
         self.time_recorder = TimerRecorder(3600 * 12, 10)
 
     async def __aenter__(self) -> "Listener":
         await self.listener.__aenter__()
         return self
 
-    async def __aexit__(self, exc_type, exc_val, exc_tb) -> None:
+    async def __aexit__(self, exc_type=None, exc_val=None, exc_tb=None) -> None:
         await asyncio.gather(
             *[c.__aexit__() for c in itertools.chain.from_iterable(self.admins.values())], self.listener.__aexit__()
         )
 
     async def run(self) -> None:
         while 1:
             try:
```

### Comparing `aiotieba-reviewer-0.1.8/examples/reviewer_example.py` & `aiotieba-reviewer-0.2.0/examples/reviewer_example.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import argparse
 import asyncio
 import re
 from typing import List, Optional, Tuple
 
 import aiotieba as tb
 from aiotieba.api.get_homepage import Thread_home, UserInfo_home
-from aiotieba.api.get_posts import UserInfo_pt
 from aiotieba.typing import Comment, Post, Thread
 from cacheout import Cache
 
 import aiotieba_reviewer as tbr
 from aiotieba_reviewer import Ops, Punish, TypeObj, imgproc
 
 sign_check_exp = re.compile(r'企鹅|扣扣', re.I)
@@ -35,15 +34,15 @@
 @tbr.reviewer.thread.set_checker()
 async def check_thread(thread: Thread) -> Optional[Punish]:
     # 水经验
     if thread.is_help:
         if re.search(r'氵|\+3|➕3|加三|加3|经验|jy', thread.text):
             return Punish(thread, Ops.DELETE, 1, note="单开水楼")
 
-    user: UserInfo_pt = thread.user
+    user = thread.user
 
     # 作图广告
     for at in thread.contents.ats:
         if at.user_id == 4928198503:
             if user.level == 1:
                 return Punish(thread, Ops.DELETE, 10, note="作图广告")
             else:
@@ -126,13 +125,13 @@
     args = parser.parse_args()
 
     async def main():
         tbr.set_BDUSS_key('starry')
         tbr.set_fname('孙笑川')
 
         if args.no_test:
-            with tbr.no_test():
+            async with tbr.no_test():
                 await tbr.run()
         else:
             await tbr.run(35.0)
 
     asyncio.run(main())
```

### Comparing `aiotieba-reviewer-0.1.8/pyproject.toml` & `aiotieba-reviewer-0.2.0/pyproject.toml`

 * *Files identical despite different names*

