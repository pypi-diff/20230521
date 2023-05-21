# Comparing `tmp/sportsml-0.0.8.tar.gz` & `tmp/sportsml-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sportsml-0.0.8.tar", last modified: Sat Mar  4 00:33:52 2023, max compression
+gzip compressed data, was "sportsml-0.0.9.tar", last modified: Sat Mar 18 14:52:03 2023, max compression
```

## Comparing `sportsml-0.0.8.tar` & `sportsml-0.0.9.tar`

### file list

```diff
@@ -1,46 +1,65 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 00:33:52.750910 sportsml-0.0.8/
--rw-r--r--   0 root         (0) root         (0)      186 2023-03-04 00:33:52.749993 sportsml-0.0.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)       25 2023-03-04 00:33:44.000000 sportsml-0.0.8/README.md
--rw-rw-rw-   0 root         (0) root         (0)      530 2023-03-04 00:33:44.000000 sportsml-0.0.8/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-04 00:33:52.750910 sportsml-0.0.8/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       37 2023-03-04 00:33:44.000000 sportsml-0.0.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 00:33:52.740826 sportsml-0.0.8/sportsml/
--rw-rw-rw-   0 root         (0) root         (0)       21 2023-03-04 00:33:44.000000 sportsml-0.0.8/sportsml/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 00:33:52.743576 sportsml-0.0.8/sportsml/cli/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-04 00:33:44.000000 sportsml-0.0.8/sportsml/cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 00:33:52.743576 sportsml-0.0.8/sportsml/cli/conf/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-04 00:33:44.000000 sportsml-0.0.8/sportsml/cli/conf/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      517 2023-03-04 00:33:44.000000 sportsml-0.0.8/sportsml/cli/train.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 00:33:52.744493 sportsml-0.0.8/sportsml/models/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-04 00:33:44.000000 sportsml-0.0.8/sportsml/models/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3217 2023-03-04 00:33:44.000000 sportsml-0.0.8/sportsml/models/graph_mlp.py
--rw-rw-rw-   0 root         (0) root         (0)     2522 2023-03-04 00:33:44.000000 sportsml-0.0.8/sportsml/models/mlp.py
--rw-rw-rw-   0 root         (0) root         (0)      177 2023-03-04 00:33:44.000000 sportsml-0.0.8/sportsml/models/rf.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 00:33:52.746326 sportsml-0.0.8/sportsml/mongo/
--rw-rw-rw-   0 root         (0) root         (0)       76 2023-03-04 00:33:44.000000 sportsml-0.0.8/sportsml/mongo/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      848 2023-03-04 00:33:44.000000 sportsml-0.0.8/sportsml/mongo/averages.py
--rw-rw-rw-   0 root         (0) root         (0)      270 2023-03-04 00:33:44.000000 sportsml-0.0.8/sportsml/mongo/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 00:33:52.747243 sportsml-0.0.8/sportsml/nba/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-04 00:33:44.000000 sportsml-0.0.8/sportsml/nba/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 00:33:52.748160 sportsml-0.0.8/sportsml/nba/data/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-04 00:33:44.000000 sportsml-0.0.8/sportsml/nba/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4777 2023-03-04 00:33:44.000000 sportsml-0.0.8/sportsml/nba/data/datamodule.py
--rw-rw-rw-   0 root         (0) root         (0)     1445 2023-03-04 00:33:44.000000 sportsml-0.0.8/sportsml/nba/data/download.py
--rw-rw-rw-   0 root         (0) root         (0)      501 2023-03-04 00:33:44.000000 sportsml-0.0.8/sportsml/nba/data/features.py
--rw-rw-rw-   0 root         (0) root         (0)     1068 2023-03-04 00:33:44.000000 sportsml-0.0.8/sportsml/nba/data/nodes.py
--rw-rw-rw-   0 root         (0) root         (0)     4528 2023-03-04 00:33:44.000000 sportsml-0.0.8/sportsml/nba/data/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 00:33:52.749076 sportsml-0.0.8/sportsml/nfl/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-04 00:33:44.000000 sportsml-0.0.8/sportsml/nfl/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 00:33:52.749993 sportsml-0.0.8/sportsml/nfl/data/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-04 00:33:44.000000 sportsml-0.0.8/sportsml/nfl/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      953 2023-03-04 00:33:44.000000 sportsml-0.0.8/sportsml/nfl/data/download.py
--rw-rw-rw-   0 root         (0) root         (0)      799 2023-03-04 00:33:44.000000 sportsml-0.0.8/sportsml/nfl/data/features.py
--rw-rw-rw-   0 root         (0) root         (0)       51 2023-03-04 00:33:44.000000 sportsml-0.0.8/sportsml/nfl/data/names.py
--rw-rw-rw-   0 root         (0) root         (0)     4377 2023-03-04 00:33:44.000000 sportsml-0.0.8/sportsml/nfl/data/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-04 00:33:52.742659 sportsml-0.0.8/sportsml.egg-info/
--rw-r--r--   0 root         (0) root         (0)      186 2023-03-04 00:33:52.000000 sportsml-0.0.8/sportsml.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      876 2023-03-04 00:33:52.000000 sportsml-0.0.8/sportsml.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-04 00:33:52.000000 sportsml-0.0.8/sportsml.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      169 2023-03-04 00:33:52.000000 sportsml-0.0.8/sportsml.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      204 2023-03-04 00:33:52.000000 sportsml-0.0.8/sportsml.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        9 2023-03-04 00:33:52.000000 sportsml-0.0.8/sportsml.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-18 14:52:03.054054 sportsml-0.0.9/
+-rw-r--r--   0 root         (0) root         (0)      186 2023-03-18 14:52:03.053054 sportsml-0.0.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)       25 2023-03-18 14:51:53.000000 sportsml-0.0.9/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      530 2023-03-18 14:51:53.000000 sportsml-0.0.9/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-03-18 14:52:03.054054 sportsml-0.0.9/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       37 2023-03-18 14:51:53.000000 sportsml-0.0.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-18 14:52:03.041053 sportsml-0.0.9/sportsml/
+-rw-rw-rw-   0 root         (0) root         (0)       21 2023-03-18 14:51:53.000000 sportsml-0.0.9/sportsml/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-18 14:52:03.043053 sportsml-0.0.9/sportsml/cbb/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-18 14:51:53.000000 sportsml-0.0.9/sportsml/cbb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-18 14:52:03.044053 sportsml-0.0.9/sportsml/cbb/data/
+-rw-rw-rw-   0 root         (0) root         (0)     3900 2023-03-18 14:51:53.000000 sportsml-0.0.9/sportsml/cbb/data/datamodule.py
+-rw-rw-rw-   0 root         (0) root         (0)     1491 2023-03-18 14:51:53.000000 sportsml-0.0.9/sportsml/cbb/data/download.py
+-rw-rw-rw-   0 root         (0) root         (0)      227 2023-03-18 14:51:53.000000 sportsml-0.0.9/sportsml/cbb/data/features.py
+-rw-rw-rw-   0 root         (0) root         (0)     7245 2023-03-18 14:51:53.000000 sportsml-0.0.9/sportsml/cbb/data/nodes.py
+-rw-rw-rw-   0 root         (0) root         (0)      175 2023-03-18 14:51:53.000000 sportsml-0.0.9/sportsml/cbb/data/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-18 14:52:03.045053 sportsml-0.0.9/sportsml/cli/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-18 14:51:53.000000 sportsml-0.0.9/sportsml/cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-18 14:52:03.045053 sportsml-0.0.9/sportsml/cli/conf/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-18 14:51:53.000000 sportsml-0.0.9/sportsml/cli/conf/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      545 2023-03-18 14:51:53.000000 sportsml-0.0.9/sportsml/cli/train.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-18 14:52:03.045053 sportsml-0.0.9/sportsml/layers/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-18 14:51:53.000000 sportsml-0.0.9/sportsml/layers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-18 14:52:03.046054 sportsml-0.0.9/sportsml/layers/gnn/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-18 14:51:53.000000 sportsml-0.0.9/sportsml/layers/gnn/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-18 14:52:03.047053 sportsml-0.0.9/sportsml/layers/gnn/encoder/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-18 14:51:53.000000 sportsml-0.0.9/sportsml/layers/gnn/encoder/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      347 2023-03-18 14:51:53.000000 sportsml-0.0.9/sportsml/layers/gnn/encoder/mean.py
+-rw-rw-rw-   0 root         (0) root         (0)      432 2023-03-18 14:51:53.000000 sportsml-0.0.9/sportsml/layers/gnn/encoder/nn.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-18 14:52:03.047053 sportsml-0.0.9/sportsml/layers/gnn/predictor/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-18 14:51:53.000000 sportsml-0.0.9/sportsml/layers/gnn/predictor/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      877 2023-03-18 14:51:53.000000 sportsml-0.0.9/sportsml/layers/gnn/predictor/nn.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-18 14:52:03.048054 sportsml-0.0.9/sportsml/models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-18 14:51:53.000000 sportsml-0.0.9/sportsml/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2768 2023-03-18 14:51:53.000000 sportsml-0.0.9/sportsml/models/gnn.py
+-rw-rw-rw-   0 root         (0) root         (0)     2522 2023-03-18 14:51:53.000000 sportsml-0.0.9/sportsml/models/mlp.py
+-rw-rw-rw-   0 root         (0) root         (0)      177 2023-03-18 14:51:53.000000 sportsml-0.0.9/sportsml/models/rf.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-18 14:52:03.049054 sportsml-0.0.9/sportsml/mongo/
+-rw-rw-rw-   0 root         (0) root         (0)       76 2023-03-18 14:51:53.000000 sportsml-0.0.9/sportsml/mongo/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      848 2023-03-18 14:51:53.000000 sportsml-0.0.9/sportsml/mongo/averages.py
+-rw-rw-rw-   0 root         (0) root         (0)      270 2023-03-18 14:51:53.000000 sportsml-0.0.9/sportsml/mongo/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-18 14:52:03.050054 sportsml-0.0.9/sportsml/nba/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-18 14:51:53.000000 sportsml-0.0.9/sportsml/nba/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-18 14:52:03.051054 sportsml-0.0.9/sportsml/nba/data/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-18 14:51:53.000000 sportsml-0.0.9/sportsml/nba/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5902 2023-03-18 14:51:53.000000 sportsml-0.0.9/sportsml/nba/data/datamodule.py
+-rw-rw-rw-   0 root         (0) root         (0)     1445 2023-03-18 14:51:53.000000 sportsml-0.0.9/sportsml/nba/data/download.py
+-rw-rw-rw-   0 root         (0) root         (0)      489 2023-03-18 14:51:53.000000 sportsml-0.0.9/sportsml/nba/data/features.py
+-rw-rw-rw-   0 root         (0) root         (0)     1126 2023-03-18 14:51:53.000000 sportsml-0.0.9/sportsml/nba/data/nodes.py
+-rw-rw-rw-   0 root         (0) root         (0)     4572 2023-03-18 14:51:53.000000 sportsml-0.0.9/sportsml/nba/data/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-18 14:52:03.052054 sportsml-0.0.9/sportsml/nfl/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-18 14:51:53.000000 sportsml-0.0.9/sportsml/nfl/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-18 14:52:03.053054 sportsml-0.0.9/sportsml/nfl/data/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-03-18 14:51:53.000000 sportsml-0.0.9/sportsml/nfl/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      953 2023-03-18 14:51:53.000000 sportsml-0.0.9/sportsml/nfl/data/download.py
+-rw-rw-rw-   0 root         (0) root         (0)      799 2023-03-18 14:51:53.000000 sportsml-0.0.9/sportsml/nfl/data/features.py
+-rw-rw-rw-   0 root         (0) root         (0)       51 2023-03-18 14:51:53.000000 sportsml-0.0.9/sportsml/nfl/data/names.py
+-rw-rw-rw-   0 root         (0) root         (0)     4377 2023-03-18 14:51:53.000000 sportsml-0.0.9/sportsml/nfl/data/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-18 14:52:03.043053 sportsml-0.0.9/sportsml.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      186 2023-03-18 14:52:02.000000 sportsml-0.0.9/sportsml.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1289 2023-03-18 14:52:02.000000 sportsml-0.0.9/sportsml.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-03-18 14:52:02.000000 sportsml-0.0.9/sportsml.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      169 2023-03-18 14:52:02.000000 sportsml-0.0.9/sportsml.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      204 2023-03-18 14:52:02.000000 sportsml-0.0.9/sportsml.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-03-18 14:52:02.000000 sportsml-0.0.9/sportsml.egg-info/top_level.txt
```

### Comparing `sportsml-0.0.8/pyproject.toml` & `sportsml-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 [build-system]
 requires = ["setuptools", "setuptools-scm"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sportsml"
-version = "0.0.8"
+version = "0.0.9"
 description = "ML for sports"
 readme = "README.md"
-requires-python = ">=3.9"
+requires-python = ">=3.8"
 license = {text = "MIT license"}
 dynamic = ["dependencies"]
 
 [tool.setuptools.dynamic]
 dependencies = {file = ["requirements.txt"]}
 
 [project.scripts]
```

### Comparing `sportsml-0.0.8/sportsml/cli/train.py` & `sportsml-0.0.9/sportsml/cli/train.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,11 +8,12 @@
         pl.seed_everything(cfg.seed)
     trainer = hydra.utils.instantiate(cfg.trainer)
     model = hydra.utils.instantiate(cfg.model)
     dm = hydra.utils.instantiate(cfg.dm)
 
     trainer.fit(model, dm)
 
-    trainer.test(model, dm, ckpt_path='best')
+    if len(dm.test_ds):
+        trainer.test(model, dm, ckpt_path='best')
 
 if __name__ == "__main__":
     train()
```

### Comparing `sportsml-0.0.8/sportsml/models/mlp.py` & `sportsml-0.0.9/sportsml/models/mlp.py`

 * *Files identical despite different names*

### Comparing `sportsml-0.0.8/sportsml/mongo/averages.py` & `sportsml-0.0.9/sportsml/mongo/averages.py`

 * *Files identical despite different names*

### Comparing `sportsml-0.0.8/sportsml/nba/data/download.py` & `sportsml-0.0.9/sportsml/nba/data/download.py`

 * *Files identical despite different names*

### Comparing `sportsml-0.0.8/sportsml/nba/data/nodes.py` & `sportsml-0.0.9/sportsml/nba/data/nodes.py`

 * *Files 24% similar despite different names*

```diff
@@ -54,12 +54,14 @@
     19: 'PHX',
     20: 'POR',
     21: 'SAC',
     22: 'SAS',
     23: 'SEA',
     24: 'TOR',
     25: 'UTA',
-    26: 'VAN',
+    26: 'MEM',
     27: 'WAS',
     28: 'DET',
     29: 'CHH'
- }
+}
+
+team_abr_lookup = {v: k for k, v in team_abr_map.items()}
```

### Comparing `sportsml-0.0.8/sportsml/nba/data/utils.py` & `sportsml-0.0.9/sportsml/nba/data/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,21 +53,22 @@
     avg = games.copy().drop(STATS_COLUMNS+OPP_STATS_COLUMNS, axis=1)
     avg_stats = games.groupby(['SEASON_ID', 'TEAM_ABBREVIATION'])[STATS_COLUMNS + OPP_STATS_COLUMNS].expanding().mean().groupby(['SEASON_ID', 'TEAM_ABBREVIATION']).shift(1).droplevel([0, 1])
     rolling_stats = games.groupby(['SEASON_ID', 'TEAM_ABBREVIATION'])[STATS_COLUMNS + OPP_STATS_COLUMNS].rolling(5, 1, closed='left').mean().droplevel([0, 1])
     rolling_stats.columns = [f'{col}_rolling' for col in rolling_stats.columns]
     return avg.merge(avg_stats, left_index=True, right_index=True).merge(rolling_stats, left_index=True, right_index=True)
 
 
-def get_regular_season_games():
-    return pd.DataFrame(
-        client.nba.games.find({
-            'SEASON_ID': {'$regex': '^2'},
-            'GAME_ID': {'$regex': '^0'},
-        })
-    )
+def get_regular_season_games(query={}):
+    query.update({
+        'SEASON_ID': {'$regex': '^2'},
+        'GAME_ID': {'$regex': '^0'},
+    })
+    df = pd.DataFrame(client.nba.games.find(query)).sort_values('GAME_DATE')
+    return df
+
 
 
 def get_regular_season_averages(date):
     season_id = client.nba.games.find_one({'GAME_DATE': date}).get('SEASON_ID')
     result = list(
         client.nba.games.aggregate(
             [
```

### Comparing `sportsml-0.0.8/sportsml/nfl/data/download.py` & `sportsml-0.0.9/sportsml/nfl/data/download.py`

 * *Files identical despite different names*

### Comparing `sportsml-0.0.8/sportsml/nfl/data/features.py` & `sportsml-0.0.9/sportsml/nfl/data/features.py`

 * *Files identical despite different names*

### Comparing `sportsml-0.0.8/sportsml/nfl/data/utils.py` & `sportsml-0.0.9/sportsml/nfl/data/utils.py`

 * *Files identical despite different names*

### Comparing `sportsml-0.0.8/sportsml.egg-info/SOURCES.txt` & `sportsml-0.0.9/sportsml.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -4,19 +4,32 @@
 sportsml/__init__.py
 sportsml.egg-info/PKG-INFO
 sportsml.egg-info/SOURCES.txt
 sportsml.egg-info/dependency_links.txt
 sportsml.egg-info/entry_points.txt
 sportsml.egg-info/requires.txt
 sportsml.egg-info/top_level.txt
+sportsml/cbb/__init__.py
+sportsml/cbb/data/datamodule.py
+sportsml/cbb/data/download.py
+sportsml/cbb/data/features.py
+sportsml/cbb/data/nodes.py
+sportsml/cbb/data/utils.py
 sportsml/cli/__init__.py
 sportsml/cli/train.py
 sportsml/cli/conf/__init__.py
+sportsml/layers/__init__.py
+sportsml/layers/gnn/__init__.py
+sportsml/layers/gnn/encoder/__init__.py
+sportsml/layers/gnn/encoder/mean.py
+sportsml/layers/gnn/encoder/nn.py
+sportsml/layers/gnn/predictor/__init__.py
+sportsml/layers/gnn/predictor/nn.py
 sportsml/models/__init__.py
-sportsml/models/graph_mlp.py
+sportsml/models/gnn.py
 sportsml/models/mlp.py
 sportsml/models/rf.py
 sportsml/mongo/__init__.py
 sportsml/mongo/averages.py
 sportsml/mongo/client.py
 sportsml/nba/__init__.py
 sportsml/nba/data/__init__.py
```

