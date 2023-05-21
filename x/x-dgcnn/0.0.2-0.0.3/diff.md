# Comparing `tmp/x-dgcnn-0.0.2.tar.gz` & `tmp/x-dgcnn-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "x-dgcnn-0.0.2.tar", last modified: Mon May 15 22:35:27 2023, max compression
+gzip compressed data, was "x-dgcnn-0.0.3.tar", last modified: Sun May 21 11:51:09 2023, max compression
```

## Comparing `x-dgcnn-0.0.2.tar` & `x-dgcnn-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.178404 x-dgcnn-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-15 22:35:16.000000 x-dgcnn-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-15 22:35:27.178404 x-dgcnn-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-15 22:35:16.000000 x-dgcnn-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-15 22:35:27.178404 x-dgcnn-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-15 22:35:16.000000 x-dgcnn-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.178404 x-dgcnn-0.0.2/x_dgcnn/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-15 22:35:16.000000 x-dgcnn-0.0.2/x_dgcnn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-15 22:35:16.000000 x-dgcnn-0.0.2/x_dgcnn/route.py
--rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-05-15 22:35:16.000000 x-dgcnn-0.0.2/x_dgcnn/x_dgcnn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 22:35:27.178404 x-dgcnn-0.0.2/x_dgcnn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-15 22:35:27.000000 x-dgcnn-0.0.2/x_dgcnn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-15 22:35:27.000000 x-dgcnn-0.0.2/x_dgcnn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 22:35:27.000000 x-dgcnn-0.0.2/x_dgcnn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-15 22:35:27.000000 x-dgcnn-0.0.2/x_dgcnn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-15 22:35:27.000000 x-dgcnn-0.0.2/x_dgcnn.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:51:09.297028 x-dgcnn-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-21 11:50:55.000000 x-dgcnn-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-21 11:51:09.297028 x-dgcnn-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-05-21 11:50:55.000000 x-dgcnn-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 11:51:09.297028 x-dgcnn-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-21 11:50:55.000000 x-dgcnn-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:51:09.293028 x-dgcnn-0.0.3/x_dgcnn/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-21 11:50:55.000000 x-dgcnn-0.0.3/x_dgcnn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8835 2023-05-21 11:50:55.000000 x-dgcnn-0.0.3/x_dgcnn/dgcnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-21 11:50:55.000000 x-dgcnn-0.0.3/x_dgcnn/route.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:51:09.293028 x-dgcnn-0.0.3/x_dgcnn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-21 11:51:09.000000 x-dgcnn-0.0.3/x_dgcnn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-21 11:51:09.000000 x-dgcnn-0.0.3/x_dgcnn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 11:51:09.000000 x-dgcnn-0.0.3/x_dgcnn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-21 11:51:09.000000 x-dgcnn-0.0.3/x_dgcnn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-21 11:51:09.000000 x-dgcnn-0.0.3/x_dgcnn.egg-info/top_level.txt
```

### Comparing `x-dgcnn-0.0.2/LICENSE` & `x-dgcnn-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `x-dgcnn-0.0.2/PKG-INFO` & `x-dgcnn-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: x-dgcnn
-Version: 0.0.2
+Version: 0.0.3
 Summary: X-DGCNN - Pytorch
 Home-page: https://github.com/kentechx/x-dgcnn
 Author: Kaidi Shen
 License: MIT
 Keywords: 3D segmentation,3D classification,point cloud understanding
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `x-dgcnn-0.0.2/setup.py` & `x-dgcnn-0.0.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     name='x-dgcnn',
     packages=find_packages(),
-    version='0.0.2',
+    version='0.0.3',
     license='MIT',
     description='X-DGCNN - Pytorch',
     author='Kaidi Shen',
     url='https://github.com/kentechx/x-dgcnn',
     long_description_content_type='text/markdown',
     keywords=[
         '3D segmentation',
```

### Comparing `x-dgcnn-0.0.2/x_dgcnn/route.py` & `x-dgcnn-0.0.3/x_dgcnn/route.py`

 * *Files identical despite different names*

### Comparing `x-dgcnn-0.0.2/x_dgcnn/x_dgcnn.py` & `x-dgcnn-0.0.3/x_dgcnn/dgcnn.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,254 +1,270 @@
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
 from einops import repeat, rearrange, einsum, reduce
-from x_dgcnn.route import subset_topk
+from .route import subset_topk
 
 
 def exists(val):
     return val is not None
 
 
-def pairwise_dists(x, y=None):
-    # x: (b, n, d)
-    # y: (b, m, d) or None
-    if exists(y):
-        xty = -2 * einsum(x, y, 'b n d, b m d -> b n m')
-        xx = reduce(x ** 2, 'b n d -> b n 1', 'sum')
-        yy = reduce(y ** 2, 'b m d -> b 1 m', 'sum')
-        pair_dists = xx + xty + yy  # (b, n, m)
-    else:
-        inner = -2 * einsum(x, x, 'b n d, b m d -> b n m')
-        xx = reduce(x ** 2, 'b n d -> b n 1', 'sum')
-        pair_dists = xx + inner + xx.transpose(2, 1)  # (b, n, m)
-    return pair_dists
-
-
-def knn(x, k):
-    # x: (b, n, d)
-    neg_pdists = -1. * pairwise_dists(x)
-    topk_ind = neg_pdists.topk(k=k, dim=-1)[1]  # (batch_size, num_points, k)
-    return topk_ind
+class InstanceNorm1d(nn.Module):  # instance norm, done in the last dimension
+
+    def __init__(self, dim, eps=1e-5):
+        super().__init__()
+        self.eps = eps
+        self.g = nn.Parameter(torch.ones(1, 1, dim))
+        self.b = nn.Parameter(torch.zeros(1, 1, dim))
+
+    def forward(self, x):
+        var = x.var(dim=1, unbiased=False, keepdim=True)
+        mean = x.mean(dim=1, keepdim=True)
+        return self.g * (x - mean) / (var + self.eps) ** 0.5 + self.b
 
 
 class EdgeConv(nn.Module):
     def __init__(self, k, dims=(64, 64)):
         super().__init__()
         self.k = k
 
-        dims = (dims[0] * 2, *dims)
-        self.mlp = nn.Sequential(*[
-            nn.Sequential(nn.Linear(in_d, out_d, bias=False),
-                          nn.LayerNorm(out_d),
-                          nn.GELU())
-            for in_d, out_d in zip(dims[:-1], dims[1:])
-        ])
+        dims = (dims[0] * 2, *dims[1:])
+        if len(dims) > 2:
+            self.mlp = nn.Sequential(*[
+                nn.Sequential(nn.Linear(in_d, out_d, bias=False),
+                              nn.LayerNorm(out_d),
+                              nn.GELU())
+                for in_d, out_d in zip(dims[:-2], dims[1:-1])
+            ])
+            self.mlp.append(nn.Linear(dims[-2], dims[-1], bias=False))
+        else:
+            self.mlp = nn.Linear(dims[0], dims[1], bias=False)
+        self.norm = nn.LayerNorm(dims[-1])
+        self.act = nn.GELU()
 
     def route(self, x, neighbor_ind=None):
         # x: (b, n, d)
         d = x.shape[-1]
         if not exists(neighbor_ind):
-            neighbor_ind = knn(x, k=self.k)  # (b, n, k)
+            neighbor_ind = torch.cdist(x, x).topk(self.k, dim=-1, largest=False)[1]  # (b, n, k)
 
         x = repeat(x, 'b n d -> b n k d', k=self.k)
         neighbor_ind = repeat(neighbor_ind, 'b n k -> b n k d', d=d)
         neighbor_x = x.gather(1, neighbor_ind)  # (b, n, k, d)
 
         # (b, n, k, d) -> (b, n, k, 2*d)
         graph_feature = torch.cat([neighbor_x - x, x], dim=-1)
         return graph_feature
 
     def forward(self, x, neighbor_ind=None):
         # x: (b, n, d)
         x = self.route(x, neighbor_ind)  # (b, n, k, 2*d)
 
-        x = rearrange(x, 'b n k d -> b (n k) d')
         x = self.mlp(x)
-        x = rearrange(x, 'b (n k) d -> b n k d', k=self.k)
         x = x.max(dim=2, keepdim=False)[0]  # (b, n, k, d) -> (b, n, d)
+        x = self.act(self.norm(x))
         return x
 
 
 class SpatialTransformNet(nn.Module):
     """
     Spatial transformer network
     """
 
-    def __init__(self, k, dims=(3, 64, 128)):
+    def __init__(self, k, in_dim=3, head_bn=True):
         super().__init__()
         self.k = k
 
+        dims = (in_dim, 64, 128)
         self.block = EdgeConv(k=k, dims=dims)
 
-        self.mlp1 = nn.Sequential(
-            nn.Linear(dims[-1], 1024, bias=False),
-            nn.LayerNorm(1024),
-            nn.GELU(),
-        )
+        norm = nn.BatchNorm1d if head_bn else nn.LayerNorm
+        self.lin = nn.Linear(dims[-1], 1024, bias=False)
 
-        self.mlp2 = nn.Sequential(
-            nn.Linear(1024, 256, bias=False),
-            nn.LayerNorm(256),
+        self.norm = norm(1024)
+        self.act = nn.GELU()
+
+        self.head = nn.Sequential(
+            nn.Linear(1024, 512, bias=False),
+            norm(512),
             nn.GELU(),
+            nn.Linear(512, 256, bias=False),
+            norm(256),
+            nn.GELU(),
+            nn.Linear(256, 9)
         )
 
-        self.transform = nn.Linear(256, 9)
-        torch.nn.init.constant_(self.transform.weight, 0)
-        torch.nn.init.eye_(self.transform.bias.view(3, 3))
+        torch.nn.init.constant_(self.head[-1].weight, 0)
+        torch.nn.init.eye_(self.head[-1].bias.view(3, 3))
 
-    def forward(self, x):
+    def forward(self, x, neighbor_ind=None):
         # x: (b, n, d)
-        x = self.block(x)  # (b, n, d) -> (b, n, d)
-        x = self.mlp1(x)  # (b, n, d) -> (b, n, 1024)
+        x = self.block(x, neighbor_ind)  # (b, n, d) -> (b, n, d)
+
+        x = self.lin(x)  # (b, n, d) -> (b, n, 1024)
         x = x.max(dim=1, keepdim=False)[0]  # (b, n, 1024) -> (b, 1024)
-        x = self.mlp2(x)  # (b, 1024) -> (b, 1024)
+        x = self.act(self.norm(x))
 
-        x = self.transform(x)  # (b, 256) -> (b, 9)
-        x = x.reshape(-1, 3, 3)  # (b, 9) -> (b, 3, 3)
+        x = self.head(x)  # (b, 1024) -> (b, 9)
         return x
 
 
 class DGCNN_Cls(nn.Module):
     def __init__(
             self,
             *,
             k,
             in_dim,
             out_dim,
             dims=(64, 64, 128, 256),
             emb_dim=1024,
             dynamic=True,
             dropout=0,
+            head_bn=True,  # if using batchnorm in head, disable it if the batch size is 1
     ):
         super().__init__()
         self.k = k
         self.dynamic = dynamic
 
         dims = (in_dim, *dims)
         self.blocks = nn.ModuleList(
             [EdgeConv(k=k, dims=(di, do)) for di, do in zip(dims[:-1], dims[1:])]
         )
 
-        self.mlp1 = nn.Sequential(
-            nn.Linear(sum(dims[1:]), emb_dim, bias=False),
-            nn.LayerNorm(emb_dim),
-            nn.GELU(),
-        )
+        self.lin = nn.Linear(sum(dims[1:]), emb_dim, bias=False)
 
         self.dropout = nn.Dropout(dropout) if dropout > 0 else nn.Identity()
 
-        self.mlp2 = nn.Sequential(
+        # BN is a linear operator on the feature space, whereas LN projects
+        # the feature space onto a (d-2)-dimensional sphere which the mlp
+        # head does not prefer.
+        norm = nn.BatchNorm1d if head_bn else nn.LayerNorm
+        self.norm = norm(emb_dim * 2)
+        self.head = nn.Sequential(
             nn.Linear(emb_dim * 2, 512, bias=False),
-            nn.LayerNorm(512),
+            norm(512),
             nn.GELU(),
             nn.Dropout(dropout) if dropout > 0 else nn.Identity(),
             nn.Linear(512, 256, bias=False),
-            nn.LayerNorm(256),
+            norm(256),
             nn.GELU(),
             nn.Dropout(dropout) if dropout > 0 else nn.Identity(),
             nn.Linear(256, out_dim),
         )
 
     def forward(self, x, xyz):
         # x: (b, n, d)
         # xyz: (b, n, 3), spatial coordinates
-        neighbor_ind = knn(xyz, k=self.k)  # (b, n, k)
+        neighbor_ind = torch.cdist(xyz, xyz).topk(self.k, dim=-1, largest=False)[1]  # (b, n, k)
 
         # go through all EdgeConv blocks
         xs = [self.blocks[0](x, neighbor_ind)]
         for block in self.blocks[1:]:
             x = block(xs[-1], None if self.dynamic else neighbor_ind)
             xs.append(x)
         x = torch.cat(xs, dim=-1)  # (b, n, sum(dims))
 
         # max & mean pooling
-        x = self.mlp1(x)  # (b, n, sum(dims)) -> (b, n, emb_dim)
+        x = self.lin(x)  # (b, n, sum(dims)) -> (b, n, emb_dim)
         x1 = x.max(dim=1, keepdim=False)[0]  # (b, n, emb_dim) -> (b, emb_dim)
         x2 = x.mean(dim=1, keepdim=False)  # (b, n, emb_dim) -> (b, emb_dim)
         x = torch.cat((x1, x2), dim=-1)  # (b, 2 * emb_dim)
 
         # mlp
-        x = self.mlp2(self.dropout(x))  # (b, 2 * emb_dim) -> (b, out_dim)
+        x = self.head(self.dropout(self.norm(x)))  # (b, 2 * emb_dim) -> (b, out_dim)
 
         return x
 
 
 class DGCNN_Seg(nn.Module):
     def __init__(
             self,
             *,
             k,
             in_dim,
             out_dim,
             emb_dim=1024,
             n_category=0,
-            category_dim=64,
             depth=3,
+            stn: SpatialTransformNet = None,
             dynamic=True,
             dropout=0,
     ):
         super().__init__()
         self.k = k
         self.dynamic = dynamic
 
-        # category embedding
-        if n_category > 0:
-            self.category_emb = nn.Embedding(n_category, category_dim)
+        # if using stn, put other features behind xyz
+        self.stn = stn
 
         # EdgeConv blocks
         assert depth >= 2, 'depth must be >= 2'
         self.blocks = nn.ModuleList(
             [EdgeConv(k=k, dims=(in_dim, 64, 64))]
         )
         for _ in range(depth - 2):
             self.blocks.append(EdgeConv(k=k, dims=(64, 64, 64)))
         self.blocks.append(EdgeConv(k=k, dims=(64, 64)))
 
-        # mlp1
-        self.mlp1 = nn.Sequential(
-            nn.Linear(depth * 64, emb_dim, bias=False),
-            nn.LayerNorm(emb_dim),
-            nn.GELU(),
-        )
-
+        # global linear
+        self.lin = nn.Linear(depth * 64, emb_dim, bias=False)
+        self.norm = nn.LayerNorm(emb_dim)
+        self.act = nn.GELU()
         self.dropout = nn.Dropout(dropout) if dropout > 0 else nn.Identity()
 
-        # mlp2
-        dim = emb_dim + depth * 64 + (category_dim if n_category > 0 else 0)
-        self.mlp2 = nn.Sequential(
+        # head
+        dim = emb_dim + depth * 64
+        self.mlp = nn.Sequential(
             nn.Linear(dim, 256, bias=False),
-            nn.LayerNorm(256),
+            InstanceNorm1d(256),
             nn.GELU(),
             nn.Dropout(dropout) if dropout > 0 else nn.Identity(),
-            nn.Linear(256, 128, bias=False),
-            nn.LayerNorm(128),
+            nn.Linear(256, 256, bias=False),
+            InstanceNorm1d(256),
             nn.GELU(),
             nn.Dropout(dropout) if dropout > 0 else nn.Identity(),
-            nn.Linear(128, out_dim),
+            nn.Linear(256, 128, bias=False),
+            InstanceNorm1d(128),
+            nn.GELU(),
         )
 
+        # category embedding
+        if n_category > 0:
+            self.category_emb = nn.Embedding(n_category, 128)
+        self.head = nn.Linear(128, out_dim)
+
     def forward(self, x, xyz, category=None):
         # x: (b, n, d)
         # xyz: (b, n, 3), spatial coordinates
         n = x.size(1)
-        neighbor_ind = knn(xyz, k=self.k)  # (b, n, k)
+        neighbor_ind = torch.cdist(xyz, xyz).topk(self.k, dim=-1, largest=False)[1]  # (b, n, k)
+
+        if exists(self.stn):
+            transform = self.stn(x, neighbor_ind).reshape(-1, 3, 3)
+            if x.size(2) > 3:
+                x = torch.cat([torch.bmm(x[:, :, :3], transform), x[:, :, 3:]], dim=-1)
+            else:
+                assert x.size(2) == 3
+                x = torch.bmm(x, transform)
 
         xs = [self.blocks[0](x, neighbor_ind)]
         for block in self.blocks[1:]:
             x = block(xs[-1], None if self.dynamic else neighbor_ind)
             xs.append(x)
         x = torch.cat(xs, dim=-1)  # (b, n, depth * 64)
 
         # global feature
-        x = self.mlp1(x)  # (b, n, d2) -> (b, n, emb_dim)
+        x = self.lin(x)  # (b, n, d2) -> (b, n, emb_dim)
         x = x.max(1)[0]  # (b, n, emb_dim) -> (b, emb_dim)
-        x = self.dropout(x)  # (b, emb_dim)
-        if exists(category):
-            x = torch.cat((x, self.category_emb(category)), dim=-1)
+        x = self.dropout(self.act(self.norm(x)))  # (b, emb_dim)
 
         # local feature
         x = repeat(x, 'b d -> b n d', n=n)  # (b, emb_dim) -> (b, n, emb_dim)
         x = torch.cat((x, *xs), dim=-1)  # (b, n, emb_dim + depth * 64)
-        x = self.mlp2(x)  # (b, n, emb_dim + depth * 64) -> (b, n, out_dim)
+        x = self.mlp(x)  # (b, n, emb_dim + depth * 64) -> (b, n, 128)
+
+        if exists(category):
+            x = x + self.category_emb(category).unsqueeze(1)  # (b, n, 128) -> (b, n, 128)
+        x = self.head(x)  # (b, n, 128) -> (b, n, out_dim)
         return x
```

### Comparing `x-dgcnn-0.0.2/x_dgcnn.egg-info/PKG-INFO` & `x-dgcnn-0.0.3/x_dgcnn.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: x-dgcnn
-Version: 0.0.2
+Version: 0.0.3
 Summary: X-DGCNN - Pytorch
 Home-page: https://github.com/kentechx/x-dgcnn
 Author: Kaidi Shen
 License: MIT
 Keywords: 3D segmentation,3D classification,point cloud understanding
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

