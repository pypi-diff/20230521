# Comparing `tmp/RL_OM-0.0.2.tar.gz` & `tmp/RL_OM-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RL_OM-0.0.2.tar", last modified: Fri May 19 17:35:01 2023, max compression
+gzip compressed data, was "RL_OM-0.0.3.tar", last modified: Sun May 21 18:08:11 2023, max compression
```

## Comparing `RL_OM-0.0.2.tar` & `RL_OM-0.0.3.tar`

### file list

```diff
@@ -1,43 +1,44 @@
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-19 17:35:01.636726 RL_OM-0.0.2/
--rw-r--r--   0 magnus     (501) staff       (20)     1071 2023-05-09 10:38:37.000000 RL_OM-0.0.2/LICENSE
--rw-rw-r--   0 magnus     (501) staff       (20)      111 2023-04-27 10:12:58.000000 RL_OM-0.0.2/MANIFEST.in
--rw-r--r--   0 magnus     (501) staff       (20)     1086 2023-05-19 17:35:01.636575 RL_OM-0.0.2/PKG-INFO
--rw-r--r--   0 magnus     (501) staff       (20)      280 2023-05-09 10:48:44.000000 RL_OM-0.0.2/README.md
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-19 17:35:01.632713 RL_OM-0.0.2/RL_OM/
--rw-r--r--   0 magnus     (501) staff       (20)       22 2023-05-19 17:34:58.000000 RL_OM-0.0.2/RL_OM/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)    51908 2023-05-19 17:34:58.000000 RL_OM-0.0.2/RL_OM/_modidx.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-19 17:35:01.634188 RL_OM-0.0.2/RL_OM/agents/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-19 17:34:58.000000 RL_OM-0.0.2/RL_OM/agents/__init__.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-19 17:35:01.634429 RL_OM-0.0.2/RL_OM/agents/benchmark_agents/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-19 17:34:58.000000 RL_OM-0.0.2/RL_OM/agents/benchmark_agents/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)     4481 2023-05-19 17:34:58.000000 RL_OM-0.0.2/RL_OM/agents/benchmark_agents/eoq.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-19 17:35:01.634953 RL_OM-0.0.2/RL_OM/agents/networks/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-19 17:34:58.000000 RL_OM-0.0.2/RL_OM/agents/networks/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)      977 2023-05-19 17:34:58.000000 RL_OM-0.0.2/RL_OM/agents/networks/actors.py
--rw-r--r--   0 magnus     (501) staff       (20)     1308 2023-05-19 17:34:58.000000 RL_OM-0.0.2/RL_OM/agents/networks/base.py
--rw-r--r--   0 magnus     (501) staff       (20)     1247 2023-05-19 17:34:58.000000 RL_OM-0.0.2/RL_OM/agents/networks/critics.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-19 17:35:01.635214 RL_OM-0.0.2/RL_OM/agents/processors/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-19 17:34:58.000000 RL_OM-0.0.2/RL_OM/agents/processors/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)     4476 2023-05-19 17:34:58.000000 RL_OM-0.0.2/RL_OM/agents/processors/processors.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-19 17:35:01.635925 RL_OM-0.0.2/RL_OM/agents/rl_agents/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-19 17:34:58.000000 RL_OM-0.0.2/RL_OM/agents/rl_agents/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)    13638 2023-05-19 17:34:58.000000 RL_OM-0.0.2/RL_OM/agents/rl_agents/sac_gumbel.py
--rw-r--r--   0 magnus     (501) staff       (20)    19119 2023-05-19 17:34:58.000000 RL_OM-0.0.2/RL_OM/agents/rl_agents/sac_hybrid.py
--rw-r--r--   0 magnus     (501) staff       (20)    19557 2023-05-19 17:34:58.000000 RL_OM-0.0.2/RL_OM/agents/rl_agents/sac_hybrid_reversed.py
--rw-r--r--   0 magnus     (501) staff       (20)    19061 2023-05-19 17:34:58.000000 RL_OM-0.0.2/RL_OM/agents/rl_agents/sac_hybrid_separate.py
--rw-r--r--   0 magnus     (501) staff       (20)      142 2023-05-19 17:34:58.000000 RL_OM-0.0.2/RL_OM/core.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-19 17:35:01.636376 RL_OM-0.0.2/RL_OM/environments/
--rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-19 17:34:58.000000 RL_OM-0.0.2/RL_OM/environments/__init__.py
--rw-r--r--   0 magnus     (501) staff       (20)     2264 2023-05-19 17:34:58.000000 RL_OM-0.0.2/RL_OM/environments/calculation_functions.py
--rw-r--r--   0 magnus     (501) staff       (20)    10585 2023-05-19 17:34:58.000000 RL_OM-0.0.2/RL_OM/environments/multi_period_inventory.py
-drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-19 17:35:01.634036 RL_OM-0.0.2/RL_OM.egg-info/
--rw-r--r--   0 magnus     (501) staff       (20)     1086 2023-05-19 17:35:01.000000 RL_OM-0.0.2/RL_OM.egg-info/PKG-INFO
--rw-r--r--   0 magnus     (501) staff       (20)      932 2023-05-19 17:35:01.000000 RL_OM-0.0.2/RL_OM.egg-info/SOURCES.txt
--rw-r--r--   0 magnus     (501) staff       (20)        1 2023-05-19 17:35:01.000000 RL_OM-0.0.2/RL_OM.egg-info/dependency_links.txt
--rw-r--r--   0 magnus     (501) staff       (20)       32 2023-05-19 17:35:01.000000 RL_OM-0.0.2/RL_OM.egg-info/entry_points.txt
--rw-r--r--   0 magnus     (501) staff       (20)        1 2023-05-09 13:19:06.000000 RL_OM-0.0.2/RL_OM.egg-info/not-zip-safe
--rw-r--r--   0 magnus     (501) staff       (20)       25 2023-05-19 17:35:01.000000 RL_OM-0.0.2/RL_OM.egg-info/requires.txt
--rw-r--r--   0 magnus     (501) staff       (20)        6 2023-05-19 17:35:01.000000 RL_OM-0.0.2/RL_OM.egg-info/top_level.txt
--rw-r--r--   0 magnus     (501) staff       (20)      989 2023-05-19 17:34:45.000000 RL_OM-0.0.2/settings.ini
--rw-r--r--   0 magnus     (501) staff       (20)       38 2023-05-19 17:35:01.636771 RL_OM-0.0.2/setup.cfg
--rw-rw-r--   0 magnus     (501) staff       (20)     2596 2023-04-27 10:12:58.000000 RL_OM-0.0.2/setup.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-21 18:08:11.786834 RL_OM-0.0.3/
+-rw-r--r--   0 magnus     (501) staff       (20)     1071 2023-05-09 10:38:37.000000 RL_OM-0.0.3/LICENSE
+-rw-rw-r--   0 magnus     (501) staff       (20)      111 2023-04-27 10:12:58.000000 RL_OM-0.0.3/MANIFEST.in
+-rw-r--r--   0 magnus     (501) staff       (20)     1086 2023-05-21 18:08:11.786661 RL_OM-0.0.3/PKG-INFO
+-rw-r--r--   0 magnus     (501) staff       (20)      280 2023-05-09 10:48:44.000000 RL_OM-0.0.3/README.md
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-21 18:08:11.781911 RL_OM-0.0.3/RL_OM/
+-rw-r--r--   0 magnus     (501) staff       (20)       22 2023-05-21 18:05:47.000000 RL_OM-0.0.3/RL_OM/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)    63135 2023-05-21 18:05:47.000000 RL_OM-0.0.3/RL_OM/_modidx.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-21 18:08:11.783081 RL_OM-0.0.3/RL_OM/agents/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-21 18:05:47.000000 RL_OM-0.0.3/RL_OM/agents/__init__.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-21 18:08:11.783330 RL_OM-0.0.3/RL_OM/agents/benchmark_agents/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-21 18:05:47.000000 RL_OM-0.0.3/RL_OM/agents/benchmark_agents/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)     4481 2023-05-21 18:05:46.000000 RL_OM-0.0.3/RL_OM/agents/benchmark_agents/eoq.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-21 18:08:11.783928 RL_OM-0.0.3/RL_OM/agents/networks/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-21 18:05:47.000000 RL_OM-0.0.3/RL_OM/agents/networks/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)     1742 2023-05-21 18:05:46.000000 RL_OM-0.0.3/RL_OM/agents/networks/actors.py
+-rw-r--r--   0 magnus     (501) staff       (20)     1308 2023-05-21 18:05:46.000000 RL_OM-0.0.3/RL_OM/agents/networks/base.py
+-rw-r--r--   0 magnus     (501) staff       (20)     2613 2023-05-21 18:05:46.000000 RL_OM-0.0.3/RL_OM/agents/networks/critics.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-21 18:08:11.784228 RL_OM-0.0.3/RL_OM/agents/processors/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-21 18:05:47.000000 RL_OM-0.0.3/RL_OM/agents/processors/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)     4476 2023-05-21 18:05:46.000000 RL_OM-0.0.3/RL_OM/agents/processors/processors.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-21 18:08:11.785523 RL_OM-0.0.3/RL_OM/agents/rl_agents/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-21 18:05:47.000000 RL_OM-0.0.3/RL_OM/agents/rl_agents/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)    14217 2023-05-21 18:05:46.000000 RL_OM-0.0.3/RL_OM/agents/rl_agents/sac_discrete.py
+-rw-r--r--   0 magnus     (501) staff       (20)    13638 2023-05-21 18:05:46.000000 RL_OM-0.0.3/RL_OM/agents/rl_agents/sac_gumbel.py
+-rw-r--r--   0 magnus     (501) staff       (20)    19119 2023-05-21 18:05:46.000000 RL_OM-0.0.3/RL_OM/agents/rl_agents/sac_hybrid.py
+-rw-r--r--   0 magnus     (501) staff       (20)    19557 2023-05-21 18:05:46.000000 RL_OM-0.0.3/RL_OM/agents/rl_agents/sac_hybrid_reversed.py
+-rw-r--r--   0 magnus     (501) staff       (20)    19061 2023-05-21 18:05:46.000000 RL_OM-0.0.3/RL_OM/agents/rl_agents/sac_hybrid_separate.py
+-rw-r--r--   0 magnus     (501) staff       (20)      142 2023-05-21 18:05:46.000000 RL_OM-0.0.3/RL_OM/core.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-21 18:08:11.786356 RL_OM-0.0.3/RL_OM/environments/
+-rw-r--r--   0 magnus     (501) staff       (20)        0 2023-05-21 18:05:47.000000 RL_OM-0.0.3/RL_OM/environments/__init__.py
+-rw-r--r--   0 magnus     (501) staff       (20)     2264 2023-05-21 18:05:47.000000 RL_OM-0.0.3/RL_OM/environments/calculation_functions.py
+-rw-r--r--   0 magnus     (501) staff       (20)    10585 2023-05-21 18:05:46.000000 RL_OM-0.0.3/RL_OM/environments/multi_period_inventory.py
+drwxr-xr-x   0 magnus     (501) staff       (20)        0 2023-05-21 18:08:11.782942 RL_OM-0.0.3/RL_OM.egg-info/
+-rw-r--r--   0 magnus     (501) staff       (20)     1086 2023-05-21 18:08:11.000000 RL_OM-0.0.3/RL_OM.egg-info/PKG-INFO
+-rw-r--r--   0 magnus     (501) staff       (20)      971 2023-05-21 18:08:11.000000 RL_OM-0.0.3/RL_OM.egg-info/SOURCES.txt
+-rw-r--r--   0 magnus     (501) staff       (20)        1 2023-05-21 18:08:11.000000 RL_OM-0.0.3/RL_OM.egg-info/dependency_links.txt
+-rw-r--r--   0 magnus     (501) staff       (20)       32 2023-05-21 18:08:11.000000 RL_OM-0.0.3/RL_OM.egg-info/entry_points.txt
+-rw-r--r--   0 magnus     (501) staff       (20)        1 2023-05-09 13:19:06.000000 RL_OM-0.0.3/RL_OM.egg-info/not-zip-safe
+-rw-r--r--   0 magnus     (501) staff       (20)       25 2023-05-21 18:08:11.000000 RL_OM-0.0.3/RL_OM.egg-info/requires.txt
+-rw-r--r--   0 magnus     (501) staff       (20)        6 2023-05-21 18:08:11.000000 RL_OM-0.0.3/RL_OM.egg-info/top_level.txt
+-rw-r--r--   0 magnus     (501) staff       (20)      989 2023-05-21 18:06:56.000000 RL_OM-0.0.3/settings.ini
+-rw-r--r--   0 magnus     (501) staff       (20)       38 2023-05-21 18:08:11.786892 RL_OM-0.0.3/setup.cfg
+-rw-rw-r--   0 magnus     (501) staff       (20)     2596 2023-04-27 10:12:58.000000 RL_OM-0.0.3/setup.py
```

### Comparing `RL_OM-0.0.2/LICENSE` & `RL_OM-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.2/PKG-INFO` & `RL_OM-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RL_OM
-Version: 0.0.2
+Version: 0.0.3
 Summary: Reinforcement Learning Applications in Operations Management
 Home-page: https://github.com/majoma7/RL_OM
 Author: Magnus Maichle
 Author-email: magnus.maichle@uni-wuerzburg.de
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `RL_OM-0.0.2/RL_OM/_modidx.py` & `RL_OM-0.0.3/RL_OM/_modidx.py`

 * *Files 16% similar despite different names*

```diff
@@ -22,22 +22,34 @@
                                                    'RL_OM.agents.benchmark_agents.eoq.EOQPolicy.set_q_star': ( 'agents/benchmark_agents/eoq.html#eoqpolicy.set_q_star',
                                                                                                                'RL_OM/agents/benchmark_agents/eoq.py')},
             'RL_OM.agents.networks.actors': { 'RL_OM.agents.networks.actors.ActorNetwork': ( 'agents/networks/actors.html#actornetwork',
                                                                                              'RL_OM/agents/networks/actors.py'),
                                               'RL_OM.agents.networks.actors.ActorNetwork.__init__': ( 'agents/networks/actors.html#actornetwork.__init__',
                                                                                                       'RL_OM/agents/networks/actors.py'),
                                               'RL_OM.agents.networks.actors.ActorNetwork.forward': ( 'agents/networks/actors.html#actornetwork.forward',
-                                                                                                     'RL_OM/agents/networks/actors.py')},
+                                                                                                     'RL_OM/agents/networks/actors.py'),
+                                              'RL_OM.agents.networks.actors.ActorNetworkDiscrete': ( 'agents/networks/actors.html#actornetworkdiscrete',
+                                                                                                     'RL_OM/agents/networks/actors.py'),
+                                              'RL_OM.agents.networks.actors.ActorNetworkDiscrete.__init__': ( 'agents/networks/actors.html#actornetworkdiscrete.__init__',
+                                                                                                              'RL_OM/agents/networks/actors.py'),
+                                              'RL_OM.agents.networks.actors.ActorNetworkDiscrete.forward': ( 'agents/networks/actors.html#actornetworkdiscrete.forward',
+                                                                                                             'RL_OM/agents/networks/actors.py')},
             'RL_OM.agents.networks.base': { 'RL_OM.agents.networks.base.BaseNetwork': ( 'agents/networks/base.html#basenetwork',
                                                                                         'RL_OM/agents/networks/base.py'),
                                             'RL_OM.agents.networks.base.BaseNetwork.__init__': ( 'agents/networks/base.html#basenetwork.__init__',
                                                                                                  'RL_OM/agents/networks/base.py'),
                                             'RL_OM.agents.networks.base.BaseNetwork.forward': ( 'agents/networks/base.html#basenetwork.forward',
                                                                                                 'RL_OM/agents/networks/base.py')},
-            'RL_OM.agents.networks.critics': { 'RL_OM.agents.networks.critics.CriticNetworkStateAction': ( 'agents/networks/critics.html#criticnetworkstateaction',
+            'RL_OM.agents.networks.critics': { 'RL_OM.agents.networks.critics.CriticNetworkState': ( 'agents/networks/critics.html#criticnetworkstate',
+                                                                                                     'RL_OM/agents/networks/critics.py'),
+                                               'RL_OM.agents.networks.critics.CriticNetworkState.__init__': ( 'agents/networks/critics.html#criticnetworkstate.__init__',
+                                                                                                              'RL_OM/agents/networks/critics.py'),
+                                               'RL_OM.agents.networks.critics.CriticNetworkState.forward': ( 'agents/networks/critics.html#criticnetworkstate.forward',
+                                                                                                             'RL_OM/agents/networks/critics.py'),
+                                               'RL_OM.agents.networks.critics.CriticNetworkStateAction': ( 'agents/networks/critics.html#criticnetworkstateaction',
                                                                                                            'RL_OM/agents/networks/critics.py'),
                                                'RL_OM.agents.networks.critics.CriticNetworkStateAction.__init__': ( 'agents/networks/critics.html#criticnetworkstateaction.__init__',
                                                                                                                     'RL_OM/agents/networks/critics.py'),
                                                'RL_OM.agents.networks.critics.CriticNetworkStateAction.forward': ( 'agents/networks/critics.html#criticnetworkstateaction.forward',
                                                                                                                    'RL_OM/agents/networks/critics.py')},
             'RL_OM.agents.processors.processors': { 'RL_OM.agents.processors.processors.ClipNegative': ( 'agents/processors/processors.html#clipnegative',
                                                                                                          'RL_OM/agents/processors/processors.py'),
@@ -69,14 +81,68 @@
                                                                                                                       'RL_OM/agents/processors/processors.py'),
                                                     'RL_OM.agents.processors.processors.RoundAction': ( 'agents/processors/processors.html#roundaction',
                                                                                                         'RL_OM/agents/processors/processors.py'),
                                                     'RL_OM.agents.processors.processors.RoundAction.__call__': ( 'agents/processors/processors.html#roundaction.__call__',
                                                                                                                  'RL_OM/agents/processors/processors.py'),
                                                     'RL_OM.agents.processors.processors.RoundAction.__init__': ( 'agents/processors/processors.html#roundaction.__init__',
                                                                                                                  'RL_OM/agents/processors/processors.py')},
+            'RL_OM.agents.rl_agents.sac_discrete': { 'RL_OM.agents.rl_agents.sac_discrete.GumbelSoftmax': ( 'agents/rl_agents/sac_discrete.html#gumbelsoftmax',
+                                                                                                            'RL_OM/agents/rl_agents/sac_discrete.py'),
+                                                     'RL_OM.agents.rl_agents.sac_discrete.GumbelSoftmax.entropy': ( 'agents/rl_agents/sac_discrete.html#gumbelsoftmax.entropy',
+                                                                                                                    'RL_OM/agents/rl_agents/sac_discrete.py'),
+                                                     'RL_OM.agents.rl_agents.sac_discrete.GumbelSoftmax.log_prob': ( 'agents/rl_agents/sac_discrete.html#gumbelsoftmax.log_prob',
+                                                                                                                     'RL_OM/agents/rl_agents/sac_discrete.py'),
+                                                     'RL_OM.agents.rl_agents.sac_discrete.GumbelSoftmax.rsample': ( 'agents/rl_agents/sac_discrete.html#gumbelsoftmax.rsample',
+                                                                                                                    'RL_OM/agents/rl_agents/sac_discrete.py'),
+                                                     'RL_OM.agents.rl_agents.sac_discrete.GumbelSoftmax.sample': ( 'agents/rl_agents/sac_discrete.html#gumbelsoftmax.sample',
+                                                                                                                   'RL_OM/agents/rl_agents/sac_discrete.py'),
+                                                     'RL_OM.agents.rl_agents.sac_discrete.SAC_Discrete_Policy': ( 'agents/rl_agents/sac_discrete.html#sac_discrete_policy',
+                                                                                                                  'RL_OM/agents/rl_agents/sac_discrete.py'),
+                                                     'RL_OM.agents.rl_agents.sac_discrete.SAC_Discrete_Policy.__call__': ( 'agents/rl_agents/sac_discrete.html#sac_discrete_policy.__call__',
+                                                                                                                           'RL_OM/agents/rl_agents/sac_discrete.py'),
+                                                     'RL_OM.agents.rl_agents.sac_discrete.SAC_Discrete_Policy.__init__': ( 'agents/rl_agents/sac_discrete.html#sac_discrete_policy.__init__',
+                                                                                                                           'RL_OM/agents/rl_agents/sac_discrete.py'),
+                                                     'RL_OM.agents.rl_agents.sac_discrete.SAC_Discrete_Policy.compute_action_and_log_prob': ( 'agents/rl_agents/sac_discrete.html#sac_discrete_policy.compute_action_and_log_prob',
+                                                                                                                                              'RL_OM/agents/rl_agents/sac_discrete.py'),
+                                                     'RL_OM.agents.rl_agents.sac_discrete.SAC_Discrete_Policy.compute_action_and_log_prob_t': ( 'agents/rl_agents/sac_discrete.html#sac_discrete_policy.compute_action_and_log_prob_t',
+                                                                                                                                                'RL_OM/agents/rl_agents/sac_discrete.py'),
+                                                     'RL_OM.agents.rl_agents.sac_discrete.SAC_Discrete_Policy.distribution': ( 'agents/rl_agents/sac_discrete.html#sac_discrete_policy.distribution',
+                                                                                                                               'RL_OM/agents/rl_agents/sac_discrete.py'),
+                                                     'RL_OM.agents.rl_agents.sac_discrete.SAC_Discrete_Policy.draw_action': ( 'agents/rl_agents/sac_discrete.html#sac_discrete_policy.draw_action',
+                                                                                                                              'RL_OM/agents/rl_agents/sac_discrete.py'),
+                                                     'RL_OM.agents.rl_agents.sac_discrete.SAC_Discrete_Policy.entropy': ( 'agents/rl_agents/sac_discrete.html#sac_discrete_policy.entropy',
+                                                                                                                          'RL_OM/agents/rl_agents/sac_discrete.py'),
+                                                     'RL_OM.agents.rl_agents.sac_discrete.SAC_Discrete_Policy.get_weights': ( 'agents/rl_agents/sac_discrete.html#sac_discrete_policy.get_weights',
+                                                                                                                              'RL_OM/agents/rl_agents/sac_discrete.py'),
+                                                     'RL_OM.agents.rl_agents.sac_discrete.SAC_Discrete_Policy.parameters': ( 'agents/rl_agents/sac_discrete.html#sac_discrete_policy.parameters',
+                                                                                                                             'RL_OM/agents/rl_agents/sac_discrete.py'),
+                                                     'RL_OM.agents.rl_agents.sac_discrete.SAC_Discrete_Policy.reset': ( 'agents/rl_agents/sac_discrete.html#sac_discrete_policy.reset',
+                                                                                                                        'RL_OM/agents/rl_agents/sac_discrete.py'),
+                                                     'RL_OM.agents.rl_agents.sac_discrete.SAC_Discrete_Policy.set_weights': ( 'agents/rl_agents/sac_discrete.html#sac_discrete_policy.set_weights',
+                                                                                                                              'RL_OM/agents/rl_agents/sac_discrete.py'),
+                                                     'RL_OM.agents.rl_agents.sac_discrete.SAC_Discrete_Policy.use_cuda': ( 'agents/rl_agents/sac_discrete.html#sac_discrete_policy.use_cuda',
+                                                                                                                           'RL_OM/agents/rl_agents/sac_discrete.py'),
+                                                     'RL_OM.agents.rl_agents.sac_discrete.SAC_discrete': ( 'agents/rl_agents/sac_discrete.html#sac_discrete',
+                                                                                                           'RL_OM/agents/rl_agents/sac_discrete.py'),
+                                                     'RL_OM.agents.rl_agents.sac_discrete.SAC_discrete.__init__': ( 'agents/rl_agents/sac_discrete.html#sac_discrete.__init__',
+                                                                                                                    'RL_OM/agents/rl_agents/sac_discrete.py'),
+                                                     'RL_OM.agents.rl_agents.sac_discrete.SAC_discrete._alpha': ( 'agents/rl_agents/sac_discrete.html#sac_discrete._alpha',
+                                                                                                                  'RL_OM/agents/rl_agents/sac_discrete.py'),
+                                                     'RL_OM.agents.rl_agents.sac_discrete.SAC_discrete._alpha_np': ( 'agents/rl_agents/sac_discrete.html#sac_discrete._alpha_np',
+                                                                                                                     'RL_OM/agents/rl_agents/sac_discrete.py'),
+                                                     'RL_OM.agents.rl_agents.sac_discrete.SAC_discrete._loss': ( 'agents/rl_agents/sac_discrete.html#sac_discrete._loss',
+                                                                                                                 'RL_OM/agents/rl_agents/sac_discrete.py'),
+                                                     'RL_OM.agents.rl_agents.sac_discrete.SAC_discrete._next_q': ( 'agents/rl_agents/sac_discrete.html#sac_discrete._next_q',
+                                                                                                                   'RL_OM/agents/rl_agents/sac_discrete.py'),
+                                                     'RL_OM.agents.rl_agents.sac_discrete.SAC_discrete._post_load': ( 'agents/rl_agents/sac_discrete.html#sac_discrete._post_load',
+                                                                                                                      'RL_OM/agents/rl_agents/sac_discrete.py'),
+                                                     'RL_OM.agents.rl_agents.sac_discrete.SAC_discrete._update_alpha': ( 'agents/rl_agents/sac_discrete.html#sac_discrete._update_alpha',
+                                                                                                                         'RL_OM/agents/rl_agents/sac_discrete.py'),
+                                                     'RL_OM.agents.rl_agents.sac_discrete.SAC_discrete.fit': ( 'agents/rl_agents/sac_discrete.html#sac_discrete.fit',
+                                                                                                               'RL_OM/agents/rl_agents/sac_discrete.py')},
             'RL_OM.agents.rl_agents.sac_gumbel': { 'RL_OM.agents.rl_agents.sac_gumbel.GumbelSoftmax': ( 'agents/rl_agents/sac_gumbel.html#gumbelsoftmax',
                                                                                                         'RL_OM/agents/rl_agents/sac_gumbel.py'),
                                                    'RL_OM.agents.rl_agents.sac_gumbel.GumbelSoftmax.entropy': ( 'agents/rl_agents/sac_gumbel.html#gumbelsoftmax.entropy',
                                                                                                                 'RL_OM/agents/rl_agents/sac_gumbel.py'),
                                                    'RL_OM.agents.rl_agents.sac_gumbel.GumbelSoftmax.log_prob': ( 'agents/rl_agents/sac_gumbel.html#gumbelsoftmax.log_prob',
                                                                                                                  'RL_OM/agents/rl_agents/sac_gumbel.py'),
                                                    'RL_OM.agents.rl_agents.sac_gumbel.GumbelSoftmax.rsample': ( 'agents/rl_agents/sac_gumbel.html#gumbelsoftmax.rsample',
```

### Comparing `RL_OM-0.0.2/RL_OM/agents/benchmark_agents/eoq.py` & `RL_OM-0.0.3/RL_OM/agents/benchmark_agents/eoq.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.2/RL_OM/agents/networks/base.py` & `RL_OM-0.0.3/RL_OM/agents/networks/base.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.2/RL_OM/agents/processors/processors.py` & `RL_OM-0.0.3/RL_OM/agents/processors/processors.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.2/RL_OM/agents/rl_agents/sac_gumbel.py` & `RL_OM-0.0.3/RL_OM/agents/rl_agents/sac_gumbel.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.2/RL_OM/agents/rl_agents/sac_hybrid.py` & `RL_OM-0.0.3/RL_OM/agents/rl_agents/sac_hybrid.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.2/RL_OM/agents/rl_agents/sac_hybrid_reversed.py` & `RL_OM-0.0.3/RL_OM/agents/rl_agents/sac_hybrid_reversed.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.2/RL_OM/agents/rl_agents/sac_hybrid_separate.py` & `RL_OM-0.0.3/RL_OM/agents/rl_agents/sac_hybrid_separate.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.2/RL_OM/environments/calculation_functions.py` & `RL_OM-0.0.3/RL_OM/environments/calculation_functions.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.2/RL_OM/environments/multi_period_inventory.py` & `RL_OM-0.0.3/RL_OM/environments/multi_period_inventory.py`

 * *Files identical despite different names*

### Comparing `RL_OM-0.0.2/RL_OM.egg-info/PKG-INFO` & `RL_OM-0.0.3/RL_OM.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RL-OM
-Version: 0.0.2
+Version: 0.0.3
 Summary: Reinforcement Learning Applications in Operations Management
 Home-page: https://github.com/majoma7/RL_OM
 Author: Magnus Maichle
 Author-email: magnus.maichle@uni-wuerzburg.de
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
```

### Comparing `RL_OM-0.0.2/RL_OM.egg-info/SOURCES.txt` & `RL_OM-0.0.3/RL_OM.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -19,14 +19,15 @@
 RL_OM/agents/networks/__init__.py
 RL_OM/agents/networks/actors.py
 RL_OM/agents/networks/base.py
 RL_OM/agents/networks/critics.py
 RL_OM/agents/processors/__init__.py
 RL_OM/agents/processors/processors.py
 RL_OM/agents/rl_agents/__init__.py
+RL_OM/agents/rl_agents/sac_discrete.py
 RL_OM/agents/rl_agents/sac_gumbel.py
 RL_OM/agents/rl_agents/sac_hybrid.py
 RL_OM/agents/rl_agents/sac_hybrid_reversed.py
 RL_OM/agents/rl_agents/sac_hybrid_separate.py
 RL_OM/environments/__init__.py
 RL_OM/environments/calculation_functions.py
 RL_OM/environments/multi_period_inventory.py
```

### Comparing `RL_OM-0.0.2/settings.ini` & `RL_OM-0.0.3/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = RL_OM
 lib_name = %(repo)s
-version = 0.0.2
+version = 0.0.3
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = RL_OM
```

### Comparing `RL_OM-0.0.2/setup.py` & `RL_OM-0.0.3/setup.py`

 * *Files identical despite different names*

