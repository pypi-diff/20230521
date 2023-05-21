# Comparing `tmp/TACTUS-data-1.1.3.tar.gz` & `tmp/tactus-data-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TACTUS-data-1.1.3.tar", last modified: Mon May 15 20:44:22 2023, max compression
+gzip compressed data, was "tactus-data-1.2.0.tar", last modified: Fri May 19 21:26:58 2023, max compression
```

## Comparing `TACTUS-data-1.1.3.tar` & `tactus-data-1.2.0.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 20:44:22.737640 TACTUS-data-1.1.3/
--rw-rw-rw-   0        0        0     4033 2023-05-15 20:44:22.735643 TACTUS-data-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0     3619 2023-05-15 16:10:43.000000 TACTUS-data-1.1.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-15 20:44:22.695640 TACTUS-data-1.1.3/TACTUS_data.egg-info/
--rw-rw-rw-   0        0        0     4033 2023-05-15 20:44:22.000000 TACTUS-data-1.1.3/TACTUS_data.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      655 2023-05-15 20:44:22.000000 TACTUS-data-1.1.3/TACTUS_data.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 20:44:22.000000 TACTUS-data-1.1.3/TACTUS_data.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      103 2023-05-15 20:44:22.000000 TACTUS-data-1.1.3/TACTUS_data.egg-info/requires.txt
--rw-rw-rw-   0        0        0       37 2023-05-15 20:44:22.000000 TACTUS-data-1.1.3/TACTUS_data.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      756 2023-05-15 20:43:14.000000 TACTUS-data-1.1.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-15 20:44:22.737640 TACTUS-data-1.1.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-15 20:44:22.698639 TACTUS-data-1.1.3/tactus_data/
--rw-rw-rw-   0        0        0      449 2023-05-15 16:10:43.000000 TACTUS-data-1.1.3/tactus_data/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-15 20:44:22.704638 TACTUS-data-1.1.3/tactus_data/datasets/
--rw-rw-rw-   0        0        0        0 2023-05-15 16:10:39.000000 TACTUS-data-1.1.3/tactus_data/datasets/__init__.py
--rw-rw-rw-   0        0        0     5192 2023-05-15 16:10:39.000000 TACTUS-data-1.1.3/tactus_data/datasets/dataset.py
--rw-rw-rw-   0        0        0     4654 2023-05-15 16:10:39.000000 TACTUS-data-1.1.3/tactus_data/datasets/ut_interaction.py
-drwxrwxrwx   0        0        0        0 2023-05-15 20:44:22.728649 TACTUS-data-1.1.3/tactus_data/utils/
--rw-rw-rw-   0        0        0        0 2023-03-14 09:55:08.000000 TACTUS-data-1.1.3/tactus_data/utils/__init__.py
--rw-rw-rw-   0        0        0     9207 2023-05-15 16:10:39.000000 TACTUS-data-1.1.3/tactus_data/utils/data_augment.py
--rw-rw-rw-   0        0        0     2269 2023-05-15 16:10:39.000000 TACTUS-data-1.1.3/tactus_data/utils/retracker.py
--rw-rw-rw-   0        0        0    15447 2023-05-15 16:10:39.000000 TACTUS-data-1.1.3/tactus_data/utils/skeleton.py
--rw-rw-rw-   0        0        0     4408 2023-05-15 16:10:39.000000 TACTUS-data-1.1.3/tactus_data/utils/skeletonrollingwindow.py
--rw-rw-rw-   0        0        0     9338 2023-05-15 16:10:39.000000 TACTUS-data-1.1.3/tactus_data/utils/thread_videocapture.py
--rw-rw-rw-   0        0        0     4092 2023-05-15 16:10:39.000000 TACTUS-data-1.1.3/tactus_data/utils/visualisation.py
--rw-rw-rw-   0        0        0     1399 2023-05-15 16:10:39.000000 TACTUS-data-1.1.3/tactus_data/utils/yolov7.py
--rw-rw-rw-   0        0        0    11761 2023-05-15 16:10:39.000000 TACTUS-data-1.1.3/tactus_data/utils/yolov8.py
-drwxrwxrwx   0        0        0        0 2023-05-15 20:44:22.732650 TACTUS-data-1.1.3/test/
--rw-rw-rw-   0        0        0     2654 2023-05-15 16:10:39.000000 TACTUS-data-1.1.3/test/test_skeletonization.py
+drwxrwxrwx   0        0        0        0 2023-05-19 21:26:58.703713 tactus-data-1.2.0/
+-rw-rw-rw-   0        0        0     4033 2023-05-19 21:26:58.702713 tactus-data-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3619 2023-05-15 16:10:43.000000 tactus-data-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-19 21:26:58.583073 tactus-data-1.2.0/TACTUS_data.egg-info/
+-rw-rw-rw-   0        0        0     4033 2023-05-19 21:26:58.000000 tactus-data-1.2.0/TACTUS_data.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      829 2023-05-19 21:26:58.000000 tactus-data-1.2.0/TACTUS_data.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-19 21:26:58.000000 tactus-data-1.2.0/TACTUS_data.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      103 2023-05-19 21:26:58.000000 tactus-data-1.2.0/TACTUS_data.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       37 2023-05-19 21:26:58.000000 tactus-data-1.2.0/TACTUS_data.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      756 2023-05-19 21:25:54.000000 tactus-data-1.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-19 21:26:58.703713 tactus-data-1.2.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-19 21:26:58.591919 tactus-data-1.2.0/tactus_data/
+-rw-rw-rw-   0        0        0      449 2023-05-15 16:10:43.000000 tactus-data-1.2.0/tactus_data/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-19 21:26:58.615926 tactus-data-1.2.0/tactus_data/datasets/
+-rw-rw-rw-   0        0        0        0 2023-05-15 16:10:39.000000 tactus-data-1.2.0/tactus_data/datasets/__init__.py
+-rw-rw-rw-   0        0        0     5192 2023-05-15 16:10:39.000000 tactus-data-1.2.0/tactus_data/datasets/dataset.py
+-rw-rw-rw-   0        0        0     4654 2023-05-15 16:10:39.000000 tactus-data-1.2.0/tactus_data/datasets/ut_interaction.py
+drwxrwxrwx   0        0        0        0 2023-05-19 21:26:58.692710 tactus-data-1.2.0/tactus_data/utils/
+-rw-rw-rw-   0        0        0        0 2023-03-14 09:55:08.000000 tactus-data-1.2.0/tactus_data/utils/__init__.py
+-rw-rw-rw-   0        0        0     9207 2023-05-15 16:10:39.000000 tactus-data-1.2.0/tactus_data/utils/data_augment.py
+-rw-rw-rw-   0        0        0     2269 2023-05-15 16:10:39.000000 tactus-data-1.2.0/tactus_data/utils/retracker.py
+-rw-rw-rw-   0        0        0    15447 2023-05-15 16:10:39.000000 tactus-data-1.2.0/tactus_data/utils/skeleton.py
+-rw-rw-rw-   0        0        0     4452 2023-05-19 15:26:34.000000 tactus-data-1.2.0/tactus_data/utils/skeletonrollingwindow.py
+-rw-rw-rw-   0        0        0     9338 2023-05-15 16:10:39.000000 tactus-data-1.2.0/tactus_data/utils/thread_videocapture.py
+-rw-rw-rw-   0        0        0     4096 2023-05-19 15:59:45.000000 tactus-data-1.2.0/tactus_data/utils/visualisation.py
+-rw-rw-rw-   0        0        0     1399 2023-05-15 16:10:39.000000 tactus-data-1.2.0/tactus_data/utils/yolov7.py
+-rw-rw-rw-   0        0        0    11761 2023-05-15 16:10:39.000000 tactus-data-1.2.0/tactus_data/utils/yolov8.py
+drwxrwxrwx   0        0        0        0 2023-05-19 21:26:58.701712 tactus-data-1.2.0/test/
+-rw-rw-rw-   0        0        0     2654 2023-05-15 16:10:39.000000 tactus-data-1.2.0/test/test_skeletonization.py
```

### Comparing `TACTUS-data-1.1.3/PKG-INFO` & `tactus-data-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: TACTUS-data
-Version: 1.1.3
+Name: tactus-data
+Version: 1.2.0
 Summary: Threatening activities classification toward users' security
 Project-URL: repository, https://github.com/Cranfield-GDP3/TACTUS-data
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `TACTUS-data-1.1.3/README.md` & `tactus-data-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `TACTUS-data-1.1.3/TACTUS_data.egg-info/PKG-INFO` & `tactus-data-1.2.0/TACTUS_data.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: TACTUS-data
-Version: 1.1.3
+Name: tactus-data
+Version: 1.2.0
 Summary: Threatening activities classification toward users' security
 Project-URL: repository, https://github.com/Cranfield-GDP3/TACTUS-data
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `TACTUS-data-1.1.3/TACTUS_data.egg-info/SOURCES.txt` & `tactus-data-1.2.0/TACTUS_data.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -2,14 +2,19 @@
 pyproject.toml
 TACTUS_data.egg-info/PKG-INFO
 TACTUS_data.egg-info/SOURCES.txt
 TACTUS_data.egg-info/dependency_links.txt
 TACTUS_data.egg-info/requires.txt
 TACTUS_data.egg-info/top_level.txt
 tactus_data/__init__.py
+tactus_data.egg-info/PKG-INFO
+tactus_data.egg-info/SOURCES.txt
+tactus_data.egg-info/dependency_links.txt
+tactus_data.egg-info/requires.txt
+tactus_data.egg-info/top_level.txt
 tactus_data/datasets/__init__.py
 tactus_data/datasets/dataset.py
 tactus_data/datasets/ut_interaction.py
 tactus_data/utils/__init__.py
 tactus_data/utils/data_augment.py
 tactus_data/utils/retracker.py
 tactus_data/utils/skeleton.py
```

### Comparing `TACTUS-data-1.1.3/pyproject.toml` & `tactus-data-1.2.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
-name = "TACTUS-data"
+name = "tactus-data"
 # PEP 440 - Version Identification and Dependency Specification https://peps.python.org/pep-0440/
-version = "1.1.3"
+version = "1.2.0"
 description = "Threatening activities classification toward users' security"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Programming Language :: Python",
```

### Comparing `TACTUS-data-1.1.3/tactus_data/datasets/dataset.py` & `tactus-data-1.2.0/tactus_data/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `TACTUS-data-1.1.3/tactus_data/datasets/ut_interaction.py` & `tactus-data-1.2.0/tactus_data/datasets/ut_interaction.py`

 * *Files identical despite different names*

### Comparing `TACTUS-data-1.1.3/tactus_data/utils/data_augment.py` & `tactus-data-1.2.0/tactus_data/utils/data_augment.py`

 * *Files identical despite different names*

### Comparing `TACTUS-data-1.1.3/tactus_data/utils/retracker.py` & `tactus-data-1.2.0/tactus_data/utils/retracker.py`

 * *Files identical despite different names*

### Comparing `TACTUS-data-1.1.3/tactus_data/utils/skeleton.py` & `tactus-data-1.2.0/tactus_data/utils/skeleton.py`

 * *Files identical despite different names*

### Comparing `TACTUS-data-1.1.3/tactus_data/utils/skeletonrollingwindow.py` & `tactus-data-1.2.0/tactus_data/utils/skeletonrollingwindow.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,25 +40,27 @@
         normalized_keypoints = self._add_keypoints(skeleton)
         angles = self._add_angles()
         velocities = self._add_velocity()
         self.is_duplicated_rw.append(False)
 
         return normalized_keypoints, angles, velocities
 
-    def duplicate_last_entry(self, new_bbox_lbrt: Tuple[float, float, float, float]):
+    def duplicate_last_entry(self, new_bbox_lbrt: Tuple[float, float, float, float]) -> Skeleton:
         """
         duplicate the last entry of the rolling window.
         """
         self.skeleton = Skeleton(bbox_lbrt=new_bbox_lbrt)
         self.keypoints_rw.append(self.keypoints_rw[-1])
         self.height_rw.append(self.height_rw[-1])
         self.angles_rw.append(self.angles_rw[-1])
         self.velocities_rw.append(self.velocities_rw[-1])
         self.is_duplicated_rw.append(True)
 
+        return self.skeleton
+
     def is_duplicated(self) -> bool:
         """return wether or not the last entry is a duplicated entry."""
         return self.is_duplicated_rw[-1]
 
     def is_complete(self) -> bool:
         """return true if the rolling window is full"""
         return len(self.keypoints_rw) == self.window_size
```

### Comparing `TACTUS-data-1.1.3/tactus_data/utils/thread_videocapture.py` & `tactus-data-1.2.0/tactus_data/utils/thread_videocapture.py`

 * *Files identical despite different names*

### Comparing `TACTUS-data-1.1.3/tactus_data/utils/visualisation.py` & `tactus-data-1.2.0/tactus_data/utils/visualisation.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,24 +60,24 @@
     image = cv2.rectangle(image,
                           (x_left, y_bottom),
                           (x_right, y_top),
                           color=color, thickness=thickness)
 
     if label is not None:
         (txt_w, txt_h), baseline = cv2.getTextSize(label,
-                                                   cv2.FONT_HERSHEY_PLAIN,
+                                                   cv2.FONT_HERSHEY_SIMPLEX,
                                                    fontScale=fontScale, thickness=2)
 
         image = cv2.rectangle(image,
                               (x_left, y_top),
                               (x_left + txt_w, y_top - txt_h - baseline),
                               color=color, thickness=-1)
 
         image = cv2.putText(image, label, (x_left, y_top),
-                            fontFace=cv2.FONT_HERSHEY_PLAIN,
+                            fontFace=cv2.FONT_HERSHEY_SIMPLEX,
                             fontScale=fontScale, color=WHITE, thickness=2)
 
     return image
 
 
 def plot_joints(image: np.ndarray,
                 skeleton: Skeleton,
```

### Comparing `TACTUS-data-1.1.3/tactus_data/utils/yolov7.py` & `tactus-data-1.2.0/tactus_data/utils/yolov7.py`

 * *Files identical despite different names*

### Comparing `TACTUS-data-1.1.3/tactus_data/utils/yolov8.py` & `tactus-data-1.2.0/tactus_data/utils/yolov8.py`

 * *Files identical despite different names*

### Comparing `TACTUS-data-1.1.3/test/test_skeletonization.py` & `tactus-data-1.2.0/test/test_skeletonization.py`

 * *Files identical despite different names*

