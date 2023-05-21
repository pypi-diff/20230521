# Comparing `tmp/synapticflow-0.0.3.tar.gz` & `tmp/synapticflow-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synapticflow-0.0.3.tar", max compression
+gzip compressed data, was "synapticflow-0.0.4.tar", max compression
```

## Comparing `synapticflow-0.0.3.tar` & `synapticflow-0.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    35149 2023-03-27 09:01:56.624062 synapticflow-0.0.3/LICENSE
--rw-r--r--   0        0        0     3224 2023-05-19 18:52:23.078528 synapticflow-0.0.3/README.md
--rw-r--r--   0        0        0     1202 2023-05-19 20:06:03.249236 synapticflow-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      269 2023-05-19 20:05:58.347482 synapticflow-0.0.3/synapticflow/__init__.py
--rw-r--r--   0        0        0       23 2023-05-18 16:57:01.512954 synapticflow-0.0.3/synapticflow/decision/__init__.py
--rw-r--r--   0        0        0     1464 2023-05-18 16:57:01.513061 synapticflow-0.0.3/synapticflow/decision/decision.py
--rw-r--r--   0        0        0       23 2023-05-18 16:57:01.513202 synapticflow-0.0.3/synapticflow/encoding/__init__.py
--rw-r--r--   0        0        0    10258 2023-05-18 21:55:51.403569 synapticflow-0.0.3/synapticflow/encoding/encoders.py
--rw-r--r--   0        0        0       51 2023-05-18 16:57:01.513461 synapticflow-0.0.3/synapticflow/learning/__init__.py
--rw-r--r--   0        0        0    22956 2023-05-18 21:48:21.478245 synapticflow-0.0.3/synapticflow/learning/learning_rules.py
--rw-r--r--   0        0        0     1252 2023-05-18 16:57:01.513703 synapticflow-0.0.3/synapticflow/learning/rewards.py
--rw-r--r--   0        0        0      102 2023-05-18 16:57:01.513880 synapticflow-0.0.3/synapticflow/network/__init__.py
--rw-r--r--   0        0        0    11840 2023-05-18 21:51:10.445427 synapticflow-0.0.3/synapticflow/network/connections.py
--rw-r--r--   0        0        0     4766 2023-05-18 16:57:01.514217 synapticflow-0.0.3/synapticflow/network/monitors.py
--rw-r--r--   0        0        0     7874 2023-05-18 16:57:01.514367 synapticflow-0.0.3/synapticflow/network/network.py
--rw-r--r--   0        0        0    87912 2023-05-19 19:41:44.825988 synapticflow-0.0.3/synapticflow/network/neural_populations.py
--rw-r--r--   0        0        0       23 2023-05-18 16:57:01.515139 synapticflow-0.0.3/synapticflow/plotting/__init__.py
--rw-r--r--   0        0        0      463 2023-05-18 16:57:01.515777 synapticflow-0.0.3/synapticflow/plotting/plotting.py
--rw-r--r--   0        0        0    16715 2023-05-19 18:46:34.831952 synapticflow-0.0.3/synapticflow/plotting/visualization.py
--rw-r--r--   0        0        0       19 2023-05-19 18:53:07.864217 synapticflow-0.0.3/synapticflow/synapticflow.py
--rw-r--r--   0        0        0      303 2023-05-18 16:57:01.515915 synapticflow-0.0.3/synapticflow/utils.py
--rw-r--r--   0        0        0     4329 1970-01-01 00:00:00.000000 synapticflow-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-03-27 09:01:56.624062 synapticflow-0.0.4/LICENSE
+-rw-r--r--   0        0        0     3224 2023-05-21 04:10:05.738713 synapticflow-0.0.4/README.md
+-rw-r--r--   0        0        0     1202 2023-05-21 20:12:27.675134 synapticflow-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      269 2023-05-21 20:12:25.868657 synapticflow-0.0.4/synapticflow/__init__.py
+-rw-r--r--   0        0        0       23 2023-05-18 16:57:01.512954 synapticflow-0.0.4/synapticflow/decision/__init__.py
+-rw-r--r--   0        0        0     1464 2023-05-18 16:57:01.513061 synapticflow-0.0.4/synapticflow/decision/decision.py
+-rw-r--r--   0        0        0       23 2023-05-18 16:57:01.513202 synapticflow-0.0.4/synapticflow/encoding/__init__.py
+-rw-r--r--   0        0        0    10258 2023-05-21 04:10:05.739497 synapticflow-0.0.4/synapticflow/encoding/encoders.py
+-rw-r--r--   0        0        0       51 2023-05-18 16:57:01.513461 synapticflow-0.0.4/synapticflow/learning/__init__.py
+-rw-r--r--   0        0        0    22956 2023-05-21 04:10:05.740070 synapticflow-0.0.4/synapticflow/learning/learning_rules.py
+-rw-r--r--   0        0        0     1252 2023-05-18 16:57:01.513703 synapticflow-0.0.4/synapticflow/learning/rewards.py
+-rw-r--r--   0        0        0      102 2023-05-18 16:57:01.513880 synapticflow-0.0.4/synapticflow/network/__init__.py
+-rw-r--r--   0        0        0    12989 2023-05-21 20:08:41.240624 synapticflow-0.0.4/synapticflow/network/connections.py
+-rw-r--r--   0        0        0     4766 2023-05-18 16:57:01.514217 synapticflow-0.0.4/synapticflow/network/monitors.py
+-rw-r--r--   0        0        0     7874 2023-05-18 16:57:01.514367 synapticflow-0.0.4/synapticflow/network/network.py
+-rw-r--r--   0        0        0    87912 2023-05-21 04:10:05.742433 synapticflow-0.0.4/synapticflow/network/neural_populations.py
+-rw-r--r--   0        0        0       23 2023-05-18 16:57:01.515139 synapticflow-0.0.4/synapticflow/plotting/__init__.py
+-rw-r--r--   0        0        0      463 2023-05-18 16:57:01.515777 synapticflow-0.0.4/synapticflow/plotting/plotting.py
+-rw-r--r--   0        0        0    16715 2023-05-21 04:10:05.743240 synapticflow-0.0.4/synapticflow/plotting/visualization.py
+-rw-r--r--   0        0        0       19 2023-05-21 04:10:05.743431 synapticflow-0.0.4/synapticflow/synapticflow.py
+-rw-r--r--   0        0        0      303 2023-05-18 16:57:01.515915 synapticflow-0.0.4/synapticflow/utils.py
+-rw-r--r--   0        0        0     4329 1970-01-01 00:00:00.000000 synapticflow-0.0.4/PKG-INFO
```

### Comparing `synapticflow-0.0.3/LICENSE` & `synapticflow-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `synapticflow-0.0.3/README.md` & `synapticflow-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `synapticflow-0.0.3/pyproject.toml` & `synapticflow-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "synapticflow"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
     "Arsham Gholamzadeh Khoee <arsham.gh97@gmail.com>",
     "Mobin Nesari <mobinnesari81@gmail.com>",
     "Mohammad Mehdi Begmaz <mohammadmehdi.begmaz@gmail.com>",
     "Negar Sourati <negarsourati@gmail.com>"
 ]
 maintainers =[
```

### Comparing `synapticflow-0.0.3/synapticflow/decision/decision.py` & `synapticflow-0.0.4/synapticflow/decision/decision.py`

 * *Files identical despite different names*

### Comparing `synapticflow-0.0.3/synapticflow/encoding/encoders.py` & `synapticflow-0.0.4/synapticflow/encoding/encoders.py`

 * *Files identical despite different names*

### Comparing `synapticflow-0.0.3/synapticflow/learning/learning_rules.py` & `synapticflow-0.0.4/synapticflow/learning/learning_rules.py`

 * *Files identical despite different names*

### Comparing `synapticflow-0.0.3/synapticflow/learning/rewards.py` & `synapticflow-0.0.4/synapticflow/learning/rewards.py`

 * *Files identical despite different names*

### Comparing `synapticflow-0.0.3/synapticflow/network/connections.py` & `synapticflow-0.0.4/synapticflow/network/connections.py`

 * *Files 10% similar despite different names*

```diff
@@ -118,14 +118,22 @@
 
         Returns
         -------
         None
 
         """
     
+    @abstractmethod
+    def compute(self, s: torch.Tensor) -> None:
+        """
+        Compute pre-activations of downstream neurons given spikes of upstream neurons.
+
+        :param s: Incoming spikes.
+        """
+    
 class Connection(AbstractConnection):
     def __init__(
         self,
         pre: NeuralPopulation,
         post: NeuralPopulation,
         w: torch.Tensor = None,
         d: torch.Tensor = None,
@@ -192,14 +200,22 @@
     def update(self, **kwargs) -> None:
         # language=rst
         """
         Compute connection's update rule.
         """
         super().update(**kwargs)
 
+    def compute(self, s: torch.Tensor) -> None:
+        spike_trace = torch.flatten(s)
+        if self.b is None:
+            post = spike_trace.view(1, -1).float() @ self.w
+        else:
+            post = spike_trace.view(1, -1).float() @ self.w + self.b
+        return post.view(*self.post.shape)
+
 class SparseConnection(AbstractConnection):
     def __init__(self, 
                  pre: NeuralPopulation, 
                  post: NeuralPopulation,
                  w: torch.Tensor = None,
                  d: torch.Tensor = None,
                  d_min: float = 0.0,
@@ -271,14 +287,22 @@
 
     def update(self, **kwargs) -> None:
         # language=rst
         """
         Compute connection's update rule.
         """
         super().update(**kwargs)
+        
+    def compute(self, s: torch.Tensor) -> None:
+        spike_trace = torch.flatten(s)
+        if self.b is None:
+            post = spike_trace.view(1, -1).float() @ self.w
+        else:
+            post = spike_trace.view(1, -1).float() @ self.w + self.b
+        return post.view(*self.post.shape)
 
 class RandomConnection(AbstractConnection):
     def __init__(
         self,
         pre: NeuralPopulation,
         post: NeuralPopulation,
         w: torch.Tensor = None,
@@ -345,8 +369,17 @@
 
     def update(self, **kwargs) -> None:
         # language=rst
         """
         Compute connection's update rule.
         """
         super().update(**kwargs)
+        
+    def compute(self, s: torch.Tensor) -> None:
+        
+        spike_trace = torch.flatten(s)
+        if self.b is None:
+            post = spike_trace.view(1, -1).float() @ self.w
+        else:
+            post = spike_trace.view(1, -1).float() @ self.w + self.b
+        return post.view(*self.post.shape)
```

### Comparing `synapticflow-0.0.3/synapticflow/network/monitors.py` & `synapticflow-0.0.4/synapticflow/network/monitors.py`

 * *Files identical despite different names*

### Comparing `synapticflow-0.0.3/synapticflow/network/network.py` & `synapticflow-0.0.4/synapticflow/network/network.py`

 * *Files identical despite different names*

### Comparing `synapticflow-0.0.3/synapticflow/network/neural_populations.py` & `synapticflow-0.0.4/synapticflow/network/neural_populations.py`

 * *Files identical despite different names*

### Comparing `synapticflow-0.0.3/synapticflow/plotting/visualization.py` & `synapticflow-0.0.4/synapticflow/plotting/visualization.py`

 * *Files identical despite different names*

### Comparing `synapticflow-0.0.3/PKG-INFO` & `synapticflow-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synapticflow
-Version: 0.0.3
+Version: 0.0.4
 Summary: A powerful Python package for simulating spiking neural networks (SNNs) using PyTorch with GPU acceleration.
 Keywords: Delay Learning,RSTDP,STDP,Spiking Neural Network (SNN)
 Author: Arsham Gholamzadeh Khoee
 Author-email: arsham.gh97@gmail.com
 Maintainer: Arsham Gholamzadeh Khoee
 Maintainer-email: arsham.gh97@gmail.com
 Classifier: License :: OSI Approved :: MIT License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: synapticflow Version: 0.0.3 Summary: A powerful
+Metadata-Version: 2.1 Name: synapticflow Version: 0.0.4 Summary: A powerful
 Python package for simulating spiking neural networks (SNNs) using PyTorch with
 GPU acceleration. Keywords: Delay Learning,RSTDP,STDP,Spiking Neural Network
 (SNN) Author: Arsham Gholamzadeh Khoee Author-email: arsham.gh97@gmail.com
 Maintainer: Arsham Gholamzadeh Khoee Maintainer-email: arsham.gh97@gmail.com
 Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python :: 2 Classifier:
 Programming Language :: Python :: 2.7 Classifier: Programming Language ::
```

