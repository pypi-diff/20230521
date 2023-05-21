# Comparing `tmp/difference_finder-0.0.1.tar.gz` & `tmp/difference_finder-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "difference_finder-0.0.1.tar", last modified: Sat May 20 14:56:23 2023, max compression
+gzip compressed data, was "difference_finder-0.0.2.tar", last modified: Sat May 20 15:27:45 2023, max compression
```

## Comparing `difference_finder-0.0.1.tar` & `difference_finder-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 bispl-jeongsol  (1000) bispl-jeongsol  (1000)        0 2023-05-20 14:56:23.994260 difference_finder-0.0.1/
--rw-rw-r--   0 bispl-jeongsol  (1000) bispl-jeongsol  (1000)     4401 2023-05-20 14:56:23.994260 difference_finder-0.0.1/PKG-INFO
--rw-rw-r--   0 bispl-jeongsol  (1000) bispl-jeongsol  (1000)     3964 2023-05-20 14:38:27.000000 difference_finder-0.0.1/README.md
-drwxrwxr-x   0 bispl-jeongsol  (1000) bispl-jeongsol  (1000)        0 2023-05-20 14:56:23.994260 difference_finder-0.0.1/difference_finder/
--rw-rw-r--   0 bispl-jeongsol  (1000) bispl-jeongsol  (1000)       21 2023-05-20 14:43:56.000000 difference_finder-0.0.1/difference_finder/__init__.py
--rw-rw-r--   0 bispl-jeongsol  (1000) bispl-jeongsol  (1000)     1723 2023-05-20 12:40:53.000000 difference_finder-0.0.1/difference_finder/data.py
--rw-rw-r--   0 bispl-jeongsol  (1000) bispl-jeongsol  (1000)     2407 2023-05-20 13:06:33.000000 difference_finder-0.0.1/difference_finder/finder.py
--rw-rw-r--   0 bispl-jeongsol  (1000) bispl-jeongsol  (1000)     1514 2023-05-20 13:29:54.000000 difference_finder-0.0.1/difference_finder/metrics.py
--rw-rw-r--   0 bispl-jeongsol  (1000) bispl-jeongsol  (1000)     1834 2023-05-20 13:05:45.000000 difference_finder-0.0.1/difference_finder/processor.py
--rw-rw-r--   0 bispl-jeongsol  (1000) bispl-jeongsol  (1000)     1516 2023-05-20 11:07:27.000000 difference_finder-0.0.1/difference_finder/strategy.py
--rw-rw-r--   0 bispl-jeongsol  (1000) bispl-jeongsol  (1000)     2964 2023-05-20 12:42:22.000000 difference_finder-0.0.1/difference_finder/utils.py
-drwxrwxr-x   0 bispl-jeongsol  (1000) bispl-jeongsol  (1000)        0 2023-05-20 14:56:23.994260 difference_finder-0.0.1/difference_finder.egg-info/
--rw-rw-r--   0 bispl-jeongsol  (1000) bispl-jeongsol  (1000)     4401 2023-05-20 14:56:23.000000 difference_finder-0.0.1/difference_finder.egg-info/PKG-INFO
--rw-rw-r--   0 bispl-jeongsol  (1000) bispl-jeongsol  (1000)      383 2023-05-20 14:56:23.000000 difference_finder-0.0.1/difference_finder.egg-info/SOURCES.txt
--rw-rw-r--   0 bispl-jeongsol  (1000) bispl-jeongsol  (1000)        1 2023-05-20 14:56:23.000000 difference_finder-0.0.1/difference_finder.egg-info/dependency_links.txt
--rw-rw-r--   0 bispl-jeongsol  (1000) bispl-jeongsol  (1000)       18 2023-05-20 14:56:23.000000 difference_finder-0.0.1/difference_finder.egg-info/top_level.txt
--rw-rw-r--   0 bispl-jeongsol  (1000) bispl-jeongsol  (1000)       38 2023-05-20 14:56:23.994260 difference_finder-0.0.1/setup.cfg
--rw-rw-r--   0 bispl-jeongsol  (1000) bispl-jeongsol  (1000)      649 2023-05-20 14:56:05.000000 difference_finder-0.0.1/setup.py
+drwxrwxr-x   0 bispl-jeongsol  (1000) bispl-jeongsol  (1000)        0 2023-05-20 15:27:45.678479 difference_finder-0.0.2/
+-rw-rw-r--   0 bispl-jeongsol  (1000) bispl-jeongsol  (1000)     4452 2023-05-20 15:27:45.678479 difference_finder-0.0.2/PKG-INFO
+-rw-rw-r--   0 bispl-jeongsol  (1000) bispl-jeongsol  (1000)     4015 2023-05-20 15:01:28.000000 difference_finder-0.0.2/README.md
+drwxrwxr-x   0 bispl-jeongsol  (1000) bispl-jeongsol  (1000)        0 2023-05-20 15:27:45.678479 difference_finder-0.0.2/difference_finder/
+-rw-rw-r--   0 bispl-jeongsol  (1000) bispl-jeongsol  (1000)       21 2023-05-20 15:26:58.000000 difference_finder-0.0.2/difference_finder/__init__.py
+-rw-rw-r--   0 bispl-jeongsol  (1000) bispl-jeongsol  (1000)     1723 2023-05-20 12:40:53.000000 difference_finder-0.0.2/difference_finder/data.py
+-rw-rw-r--   0 bispl-jeongsol  (1000) bispl-jeongsol  (1000)     2827 2023-05-20 15:22:53.000000 difference_finder-0.0.2/difference_finder/finder.py
+-rw-rw-r--   0 bispl-jeongsol  (1000) bispl-jeongsol  (1000)     1514 2023-05-20 13:29:54.000000 difference_finder-0.0.2/difference_finder/metrics.py
+-rw-rw-r--   0 bispl-jeongsol  (1000) bispl-jeongsol  (1000)     1834 2023-05-20 13:05:45.000000 difference_finder-0.0.2/difference_finder/processor.py
+-rw-rw-r--   0 bispl-jeongsol  (1000) bispl-jeongsol  (1000)     1516 2023-05-20 11:07:27.000000 difference_finder-0.0.2/difference_finder/strategy.py
+-rw-rw-r--   0 bispl-jeongsol  (1000) bispl-jeongsol  (1000)     2964 2023-05-20 12:42:22.000000 difference_finder-0.0.2/difference_finder/utils.py
+drwxrwxr-x   0 bispl-jeongsol  (1000) bispl-jeongsol  (1000)        0 2023-05-20 15:27:45.678479 difference_finder-0.0.2/difference_finder.egg-info/
+-rw-rw-r--   0 bispl-jeongsol  (1000) bispl-jeongsol  (1000)     4452 2023-05-20 15:27:45.000000 difference_finder-0.0.2/difference_finder.egg-info/PKG-INFO
+-rw-rw-r--   0 bispl-jeongsol  (1000) bispl-jeongsol  (1000)      383 2023-05-20 15:27:45.000000 difference_finder-0.0.2/difference_finder.egg-info/SOURCES.txt
+-rw-rw-r--   0 bispl-jeongsol  (1000) bispl-jeongsol  (1000)        1 2023-05-20 15:27:45.000000 difference_finder-0.0.2/difference_finder.egg-info/dependency_links.txt
+-rw-rw-r--   0 bispl-jeongsol  (1000) bispl-jeongsol  (1000)       18 2023-05-20 15:27:45.000000 difference_finder-0.0.2/difference_finder.egg-info/top_level.txt
+-rw-rw-r--   0 bispl-jeongsol  (1000) bispl-jeongsol  (1000)       38 2023-05-20 15:27:45.678479 difference_finder-0.0.2/setup.cfg
+-rw-rw-r--   0 bispl-jeongsol  (1000) bispl-jeongsol  (1000)      649 2023-05-20 15:27:21.000000 difference_finder-0.0.2/setup.py
```

### Comparing `difference_finder-0.0.1/PKG-INFO` & `difference_finder-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: difference_finder
-Version: 0.0.1
+Version: 0.0.2
 Summary: Find difference between two images using pytorch.
 Home-page: https://github.com/jeongsol-kim/difference_finder
 Author: Jeongsol Kim
 Author-email: wjdthf3927@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -107,14 +107,19 @@
 ### pre-requisite
 - pytorch > 0.7.0
 - numpy
 - pillow
 - pytorch_msssim
 - lpips
 
+### Install
+```
+pip install difference-finder
+```
+
 ### Usage
 
 It would be simple. Just follow the three steps!
 
 1. Define 'Finder'
 2. Give two image paths to compare
 3. Done!
```

### Comparing `difference_finder-0.0.1/README.md` & `difference_finder-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -94,14 +94,19 @@
 ### pre-requisite
 - pytorch > 0.7.0
 - numpy
 - pillow
 - pytorch_msssim
 - lpips
 
+### Install
+```
+pip install difference-finder
+```
+
 ### Usage
 
 It would be simple. Just follow the three steps!
 
 1. Define 'Finder'
 2. Give two image paths to compare
 3. Done!
```

### Comparing `difference_finder-0.0.1/difference_finder/data.py` & `difference_finder-0.0.2/difference_finder/data.py`

 * *Files identical despite different names*

### Comparing `difference_finder-0.0.1/difference_finder/finder.py` & `difference_finder-0.0.2/difference_finder/finder.py`

 * *Files 3% similar despite different names*

```diff
@@ -50,16 +50,24 @@
             output = self.run_on_image(first_img, second_img)
             outputs.append(output)
         return outputs
     
     def run(self,
             img1: Union[Path, torch.Tensor],
             img2: Union[Path, torch.Tensor]):
-        
-        if img1.is_dir and img2.is_dir:
-            output = self.run_on_directory(img1, img2)
+
+        if isinstance(img1, Path) and isinstance(img2, Path):
+            if img1.is_dir() and img2.is_dir():
+                output = self.run_on_directory(img1, img2)
+            else:
+                loader = get_loader(files1=[img1],
+                                    files2=[img2],
+                                    transform=ToTensor(),
+                                    num_workers=0)
+                first_img, second_img = next(iter(loader))
+                output = self.run_on_image(first_img, second_img)
         else:
             output = self.run_on_image(img1, img2)
         return output
 
     def save_fn(self):
         pass
```

### Comparing `difference_finder-0.0.1/difference_finder/metrics.py` & `difference_finder-0.0.2/difference_finder/metrics.py`

 * *Files identical despite different names*

### Comparing `difference_finder-0.0.1/difference_finder/processor.py` & `difference_finder-0.0.2/difference_finder/processor.py`

 * *Files identical despite different names*

### Comparing `difference_finder-0.0.1/difference_finder/strategy.py` & `difference_finder-0.0.2/difference_finder/strategy.py`

 * *Files identical despite different names*

### Comparing `difference_finder-0.0.1/difference_finder/utils.py` & `difference_finder-0.0.2/difference_finder/utils.py`

 * *Files identical despite different names*

### Comparing `difference_finder-0.0.1/difference_finder.egg-info/PKG-INFO` & `difference_finder-0.0.2/difference_finder.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: difference-finder
-Version: 0.0.1
+Version: 0.0.2
 Summary: Find difference between two images using pytorch.
 Home-page: https://github.com/jeongsol-kim/difference_finder
 Author: Jeongsol Kim
 Author-email: wjdthf3927@gmail.com
 License: MIT
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -107,14 +107,19 @@
 ### pre-requisite
 - pytorch > 0.7.0
 - numpy
 - pillow
 - pytorch_msssim
 - lpips
 
+### Install
+```
+pip install difference-finder
+```
+
 ### Usage
 
 It would be simple. Just follow the three steps!
 
 1. Define 'Finder'
 2. Give two image paths to compare
 3. Done!
```

### Comparing `difference_finder-0.0.1/setup.py` & `difference_finder-0.0.2/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="difference_finder",
-    version="0.0.1",
+    version="0.0.2",
     license='MIT',
     author="Jeongsol Kim",
     author_email="wjdthf3927@gmail.com",
     description="Find difference between two images using pytorch.",
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url="https://github.com/jeongsol-kim/difference_finder",
```

