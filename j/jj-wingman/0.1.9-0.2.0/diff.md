# Comparing `tmp/jj_wingman-0.1.9.tar.gz` & `tmp/jj_wingman-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jj_wingman-0.1.9.tar", last modified: Mon Nov 21 20:03:50 2022, max compression
+gzip compressed data, was "jj_wingman-0.2.0.tar", last modified: Sun May 21 21:46:22 2023, max compression
```

## Comparing `jj_wingman-0.1.9.tar` & `jj_wingman-0.2.0.tar`

### file list

```diff
@@ -1,22 +1,25 @@
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2022-11-21 20:03:50.435978 jj_wingman-0.1.9/
--rw-rw-r--   0 jet       (1000) jet       (1000)     1074 2022-10-05 13:54:34.000000 jj_wingman-0.1.9/LICENSE.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)    14567 2022-11-21 20:03:50.435978 jj_wingman-0.1.9/PKG-INFO
--rw-rw-r--   0 jet       (1000) jet       (1000)    12812 2022-10-27 17:06:12.000000 jj_wingman-0.1.9/README.md
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2022-11-21 20:03:50.435978 jj_wingman-0.1.9/jj_wingman.egg-info/
--rw-rw-r--   0 jet       (1000) jet       (1000)    14567 2022-11-21 20:03:50.000000 jj_wingman-0.1.9/jj_wingman.egg-info/PKG-INFO
--rw-rw-r--   0 jet       (1000) jet       (1000)      400 2022-11-21 20:03:50.000000 jj_wingman-0.1.9/jj_wingman.egg-info/SOURCES.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)        1 2022-11-21 20:03:50.000000 jj_wingman-0.1.9/jj_wingman.egg-info/dependency_links.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)      116 2022-11-21 20:03:50.000000 jj_wingman-0.1.9/jj_wingman.egg-info/entry_points.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)       25 2022-11-21 20:03:50.000000 jj_wingman-0.1.9/jj_wingman.egg-info/requires.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)        8 2022-11-21 20:03:50.000000 jj_wingman-0.1.9/jj_wingman.egg-info/top_level.txt
--rw-rw-r--   0 jet       (1000) jet       (1000)      821 2022-11-21 20:03:46.000000 jj_wingman-0.1.9/pyproject.toml
--rw-rw-r--   0 jet       (1000) jet       (1000)       38 2022-11-21 20:03:50.435978 jj_wingman-0.1.9/setup.cfg
--rw-rw-r--   0 jet       (1000) jet       (1000)      908 2022-11-21 19:55:24.000000 jj_wingman-0.1.9/setup.py
-drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2022-11-21 20:03:50.435978 jj_wingman-0.1.9/wingman/
--rw-rw-r--   0 jet       (1000) jet       (1000)      218 2022-11-21 19:53:59.000000 jj_wingman-0.1.9/wingman/__init__.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     2846 2022-11-21 19:53:57.000000 jj_wingman-0.1.9/wingman/cli_scripts.py
--rw-rw-r--   0 jet       (1000) jet       (1000)      288 2022-11-21 19:54:55.000000 jj_wingman-0.1.9/wingman/config.yaml
--rw-rw-r--   0 jet       (1000) jet       (1000)     9912 2022-10-24 15:21:42.000000 jj_wingman-0.1.9/wingman/neural_blocks.py
--rw-rw-r--   0 jet       (1000) jet       (1000)     2802 2022-10-05 14:43:05.000000 jj_wingman-0.1.9/wingman/replay_buffer.py
--rw-rw-r--   0 jet       (1000) jet       (1000)      729 2022-10-05 14:40:43.000000 jj_wingman-0.1.9/wingman/utils.py
--rw-rw-r--   0 jet       (1000) jet       (1000)    13531 2022-11-11 17:21:15.000000 jj_wingman-0.1.9/wingman/wingman.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-21 21:46:22.902831 jj_wingman-0.2.0/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1074 2022-11-26 07:59:06.000000 jj_wingman-0.2.0/LICENSE.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)    15185 2023-05-21 21:46:22.902831 jj_wingman-0.2.0/PKG-INFO
+-rw-rw-r--   0 jet       (1000) jet       (1000)    13489 2023-03-07 18:53:37.000000 jj_wingman-0.2.0/README.md
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-21 21:46:22.902831 jj_wingman-0.2.0/jj_wingman.egg-info/
+-rw-rw-r--   0 jet       (1000) jet       (1000)    15185 2023-05-21 21:46:22.000000 jj_wingman-0.2.0/jj_wingman.egg-info/PKG-INFO
+-rw-rw-r--   0 jet       (1000) jet       (1000)      464 2023-05-21 21:46:22.000000 jj_wingman-0.2.0/jj_wingman.egg-info/SOURCES.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)        1 2023-05-21 21:46:22.000000 jj_wingman-0.2.0/jj_wingman.egg-info/dependency_links.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)      116 2023-05-21 21:46:22.000000 jj_wingman-0.2.0/jj_wingman.egg-info/entry_points.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)       19 2023-05-21 21:46:22.000000 jj_wingman-0.2.0/jj_wingman.egg-info/requires.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)        8 2023-05-21 21:46:22.000000 jj_wingman-0.2.0/jj_wingman.egg-info/top_level.txt
+-rw-rw-r--   0 jet       (1000) jet       (1000)      927 2023-05-21 21:46:10.000000 jj_wingman-0.2.0/pyproject.toml
+-rw-rw-r--   0 jet       (1000) jet       (1000)       38 2023-05-21 21:46:22.902831 jj_wingman-0.2.0/setup.cfg
+-rw-rw-r--   0 jet       (1000) jet       (1000)       92 2023-03-07 18:49:10.000000 jj_wingman-0.2.0/setup.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-21 21:46:22.902831 jj_wingman-0.2.0/test/
+-rw-rw-r--   0 jet       (1000) jet       (1000)     2737 2023-05-21 21:40:50.000000 jj_wingman-0.2.0/test/test_replay_buffer.py
+drwxrwxr-x   0 jet       (1000) jet       (1000)        0 2023-05-21 21:46:22.902831 jj_wingman-0.2.0/wingman/
+-rw-rw-r--   0 jet       (1000) jet       (1000)      218 2022-12-10 02:36:58.000000 jj_wingman-0.2.0/wingman/__init__.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     4130 2023-03-07 18:48:06.000000 jj_wingman-0.2.0/wingman/cli_scripts.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)      288 2022-11-26 07:59:06.000000 jj_wingman-0.2.0/wingman/config.yaml
+-rw-rw-r--   0 jet       (1000) jet       (1000)    10106 2023-03-07 18:50:52.000000 jj_wingman-0.2.0/wingman/neural_blocks.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)      777 2023-03-07 18:47:29.000000 jj_wingman-0.2.0/wingman/print_utils.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     5675 2023-05-21 21:06:37.000000 jj_wingman-0.2.0/wingman/replay_buffer.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)     1033 2023-03-07 18:51:03.000000 jj_wingman-0.2.0/wingman/utils.py
+-rw-rw-r--   0 jet       (1000) jet       (1000)    15009 2023-03-07 18:51:08.000000 jj_wingman-0.2.0/wingman/wingman.py
```

### Comparing `jj_wingman-0.1.9/LICENSE.txt` & `jj_wingman-0.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jj_wingman-0.1.9/PKG-INFO` & `jj_wingman-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 Metadata-Version: 2.1
 Name: jj_wingman
-Version: 0.1.9
+Version: 0.2.0
 Summary: Wingman library for AI projects.
-Home-page: https://github.com/jjshoots/Wingman
-Author: Jet
 Author-email: Jet <taijunjet@hotmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
@@ -47,27 +45,34 @@
 - Building blocks for popular torch modules
 - Smoothly handling commandline arguments and `*.yaml` config files
 
 ## Installation
 
 `pip3 install jj-wingman`
 
+> Wingman does not come with a PyTorch requirement by default, so all torch-functionality is by default disabled.
+> If you wish to use the PyTorch functionality of Wingman, install a compatible Pytorch version for your machine.
+> This is typically done via:
+> `pip3 install torch`
+
 ## Philosophy
 
 Wingman is designed to be very horizontally integrated into your deep learning projects.
 Instead of wrapping your models with wrappers or designing your models around Wingman, Wingman adapts to your projects, and you are the decider on when and where Wingman comes into play.
 
 ## Modules
 
 Wingman has several core modules and static functions, all of which can be used independently or in conjunction.
 
 
+<br>
+
 ### `from wingman import Wingman`
 
-This is the core module for Wingman, Wingman requires a bare minimum `config.yaml` file somewhere accessible in your project directory.
+This is the core module for Wingman, Wingman requires a bare minimum `config.yaml` file somewhere accessible in your project directory, this can be generated by running `wingman-generate-yaml [optional filename]` on the commandline.
 A bare minimum yaml file is as follows:
 
 ```yaml
 # wingman required params
 debug: false
 
 weights_directory: 'weights'
@@ -124,15 +129,15 @@
     model = Model(cfg.YOUR_PARAM, cfg.YOUR_OTHER_PARAM).to(cfg.device)
     optim = optimizer.AdamW(model.parameters(), lr=cfg.YOUR_LEARNING_RATE_PARAM, amsgrad=True)
 
     # we can check if we have trained this model before, and if we have, just load it
     # this checking is done using the `version_number` param, if `latest=True` is set,
     # Wingman automatically searches for the latest model checkpoint,
     # otherwise, Wingman uses the checkpoint specified by `mark_number`
-    have_file, weight_file, optim_file = self.get_weight_files(latest=True)
+    have_file, weight_file, optim_file = wm.get_weight_files(latest=True)
     if have_file:
         # Wingman simply returns a string of where the weight files are
         # no unnecessary wrapping!
         model.load_state_dict(torch.load(model_file))
         optim.load_state_dict(torch.load(optim_file))
 
     # let's run some training:
@@ -154,14 +159,21 @@
         update_weights, model_file, optim_file = wm.checkpoint(loss, training_step)
         if update_weights:
             # if Wingman deems that the weights should be checkpointed, it returns
             # a string of where the weight files should go for it to be found later
             torch.save(model.state_dict(), model_file)
             torch.save(optim.state_dict(), optim_file)
 ```
+#### Weights Directory Compression
+
+If you train a lot of models, the weights directory can start to use a lot of disk space.
+Running `wingman-compress-weights [optional directory name]` on the commandline will remove all redundant mark numbers and delete all empty files.
+
+
+<br>
 
 ### `from wingman import NeuralBlocks`
 
 Neural blocks is a module for quickly prototyping neural network architectures.
 It offers several easier methods of defining standardized modules:
 
 #### Simple 3-layer MLP with ReLU activation
@@ -253,14 +265,17 @@
     (1): LeakyReLU(negative_slope=0.01)
   )
 )
 ```
 
 The Neural Blocks module also has functions that can generate single modules, refer to the file itself for more details.
 
+
+<br>
+
 ### `from wingman import ReplayBuffer`
 
 This is a replay buffer designed around Torch's Dataloader class for reinforcement learning projects.
 This allows easy bootstrapping of the Dataloader's excellent shuffling and pre-batching capabilities.
 In addition, all the data is stored as a numpy array in a contiguous block of memory, allowing very fast retrieval.
 ReplayBuffer also doesn't put any limits on tuple length per transition; some people prefer to store $\{S, A, R, S'\}$, some prefer to store $\{S, A, R, S', A'\}$ - ReplayBuffer doesn't care!
 The length of the tuple can be as long or as short as you want, as long as every tuple fed in is the same length and each element of the tuple is the same shape.
@@ -302,14 +317,17 @@
     observations = gpuize(stuff[0], "cuda:0")
     actions = gpuize(stuff[1], "cuda:0")
     rewards = gpuize(stuff[2], "cuda:0")
     next_states = gpuize(stuff[3], "cuda:0")
     dones = gpuize(stuff[4], "cuda:0")
 ```
 
+
+<br>
+
 ### `from wingman import gpuize, cpuize`
 
 These are quality of life standalone functions.
 
 ```python
 >>> import numpy as np
 >>> from wingman import gpuize, cpuize
@@ -327,16 +345,16 @@
 
 tensor([[0.2839, 0.5094, 0.5543, 0.4561, 0.8252],
         [0.7744, 0.2090, 0.8622, 0.6907, 0.9486],
         [0.7008, 0.9278, 0.9839, 0.7695, 0.7289],
         [0.4770, 0.5497, 0.2211, 0.7244, 0.4257],
         [0.7833, 0.8489, 0.6853, 0.6188, 0.1356]], device='cuda:0')
 
->>> pae = cpuize(bar)
->>> print(pae)
+>>> baz = cpuize(bar)
+>>> print(baz)
 
 [[0.28392764 0.50936983 0.55433616 0.45614518 0.82523046]
  [0.77437072 0.20900382 0.86220494 0.69071239 0.94863786]
  [0.70082865 0.92780018 0.98392965 0.76945165 0.72886401]
  [0.47702485 0.54968522 0.22110942 0.72436276 0.42574472]
  [0.78330221 0.84888837 0.68529167 0.61878902 0.13556213]]
 ```
```

### Comparing `jj_wingman-0.1.9/README.md` & `jj_wingman-0.2.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -11,27 +11,34 @@
 - Building blocks for popular torch modules
 - Smoothly handling commandline arguments and `*.yaml` config files
 
 ## Installation
 
 `pip3 install jj-wingman`
 
+> Wingman does not come with a PyTorch requirement by default, so all torch-functionality is by default disabled.
+> If you wish to use the PyTorch functionality of Wingman, install a compatible Pytorch version for your machine.
+> This is typically done via:
+> `pip3 install torch`
+
 ## Philosophy
 
 Wingman is designed to be very horizontally integrated into your deep learning projects.
 Instead of wrapping your models with wrappers or designing your models around Wingman, Wingman adapts to your projects, and you are the decider on when and where Wingman comes into play.
 
 ## Modules
 
 Wingman has several core modules and static functions, all of which can be used independently or in conjunction.
 
 
+<br>
+
 ### `from wingman import Wingman`
 
-This is the core module for Wingman, Wingman requires a bare minimum `config.yaml` file somewhere accessible in your project directory.
+This is the core module for Wingman, Wingman requires a bare minimum `config.yaml` file somewhere accessible in your project directory, this can be generated by running `wingman-generate-yaml [optional filename]` on the commandline.
 A bare minimum yaml file is as follows:
 
 ```yaml
 # wingman required params
 debug: false
 
 weights_directory: 'weights'
@@ -88,15 +95,15 @@
     model = Model(cfg.YOUR_PARAM, cfg.YOUR_OTHER_PARAM).to(cfg.device)
     optim = optimizer.AdamW(model.parameters(), lr=cfg.YOUR_LEARNING_RATE_PARAM, amsgrad=True)
 
     # we can check if we have trained this model before, and if we have, just load it
     # this checking is done using the `version_number` param, if `latest=True` is set,
     # Wingman automatically searches for the latest model checkpoint,
     # otherwise, Wingman uses the checkpoint specified by `mark_number`
-    have_file, weight_file, optim_file = self.get_weight_files(latest=True)
+    have_file, weight_file, optim_file = wm.get_weight_files(latest=True)
     if have_file:
         # Wingman simply returns a string of where the weight files are
         # no unnecessary wrapping!
         model.load_state_dict(torch.load(model_file))
         optim.load_state_dict(torch.load(optim_file))
 
     # let's run some training:
@@ -118,14 +125,21 @@
         update_weights, model_file, optim_file = wm.checkpoint(loss, training_step)
         if update_weights:
             # if Wingman deems that the weights should be checkpointed, it returns
             # a string of where the weight files should go for it to be found later
             torch.save(model.state_dict(), model_file)
             torch.save(optim.state_dict(), optim_file)
 ```
+#### Weights Directory Compression
+
+If you train a lot of models, the weights directory can start to use a lot of disk space.
+Running `wingman-compress-weights [optional directory name]` on the commandline will remove all redundant mark numbers and delete all empty files.
+
+
+<br>
 
 ### `from wingman import NeuralBlocks`
 
 Neural blocks is a module for quickly prototyping neural network architectures.
 It offers several easier methods of defining standardized modules:
 
 #### Simple 3-layer MLP with ReLU activation
@@ -217,14 +231,17 @@
     (1): LeakyReLU(negative_slope=0.01)
   )
 )
 ```
 
 The Neural Blocks module also has functions that can generate single modules, refer to the file itself for more details.
 
+
+<br>
+
 ### `from wingman import ReplayBuffer`
 
 This is a replay buffer designed around Torch's Dataloader class for reinforcement learning projects.
 This allows easy bootstrapping of the Dataloader's excellent shuffling and pre-batching capabilities.
 In addition, all the data is stored as a numpy array in a contiguous block of memory, allowing very fast retrieval.
 ReplayBuffer also doesn't put any limits on tuple length per transition; some people prefer to store $\{S, A, R, S'\}$, some prefer to store $\{S, A, R, S', A'\}$ - ReplayBuffer doesn't care!
 The length of the tuple can be as long or as short as you want, as long as every tuple fed in is the same length and each element of the tuple is the same shape.
@@ -266,14 +283,17 @@
     observations = gpuize(stuff[0], "cuda:0")
     actions = gpuize(stuff[1], "cuda:0")
     rewards = gpuize(stuff[2], "cuda:0")
     next_states = gpuize(stuff[3], "cuda:0")
     dones = gpuize(stuff[4], "cuda:0")
 ```
 
+
+<br>
+
 ### `from wingman import gpuize, cpuize`
 
 These are quality of life standalone functions.
 
 ```python
 >>> import numpy as np
 >>> from wingman import gpuize, cpuize
@@ -291,16 +311,16 @@
 
 tensor([[0.2839, 0.5094, 0.5543, 0.4561, 0.8252],
         [0.7744, 0.2090, 0.8622, 0.6907, 0.9486],
         [0.7008, 0.9278, 0.9839, 0.7695, 0.7289],
         [0.4770, 0.5497, 0.2211, 0.7244, 0.4257],
         [0.7833, 0.8489, 0.6853, 0.6188, 0.1356]], device='cuda:0')
 
->>> pae = cpuize(bar)
->>> print(pae)
+>>> baz = cpuize(bar)
+>>> print(baz)
 
 [[0.28392764 0.50936983 0.55433616 0.45614518 0.82523046]
  [0.77437072 0.20900382 0.86220494 0.69071239 0.94863786]
  [0.70082865 0.92780018 0.98392965 0.76945165 0.72886401]
  [0.47702485 0.54968522 0.22110942 0.72436276 0.42574472]
  [0.78330221 0.84888837 0.68529167 0.61878902 0.13556213]]
 ```
```

### Comparing `jj_wingman-0.1.9/jj_wingman.egg-info/PKG-INFO` & `jj_wingman-0.2.0/jj_wingman.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 Metadata-Version: 2.1
 Name: jj-wingman
-Version: 0.1.9
+Version: 0.2.0
 Summary: Wingman library for AI projects.
-Home-page: https://github.com/jjshoots/Wingman
-Author: Jet
 Author-email: Jet <taijunjet@hotmail.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
         in the Software without restriction, including without limitation the rights
         to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
@@ -47,27 +45,34 @@
 - Building blocks for popular torch modules
 - Smoothly handling commandline arguments and `*.yaml` config files
 
 ## Installation
 
 `pip3 install jj-wingman`
 
+> Wingman does not come with a PyTorch requirement by default, so all torch-functionality is by default disabled.
+> If you wish to use the PyTorch functionality of Wingman, install a compatible Pytorch version for your machine.
+> This is typically done via:
+> `pip3 install torch`
+
 ## Philosophy
 
 Wingman is designed to be very horizontally integrated into your deep learning projects.
 Instead of wrapping your models with wrappers or designing your models around Wingman, Wingman adapts to your projects, and you are the decider on when and where Wingman comes into play.
 
 ## Modules
 
 Wingman has several core modules and static functions, all of which can be used independently or in conjunction.
 
 
+<br>
+
 ### `from wingman import Wingman`
 
-This is the core module for Wingman, Wingman requires a bare minimum `config.yaml` file somewhere accessible in your project directory.
+This is the core module for Wingman, Wingman requires a bare minimum `config.yaml` file somewhere accessible in your project directory, this can be generated by running `wingman-generate-yaml [optional filename]` on the commandline.
 A bare minimum yaml file is as follows:
 
 ```yaml
 # wingman required params
 debug: false
 
 weights_directory: 'weights'
@@ -124,15 +129,15 @@
     model = Model(cfg.YOUR_PARAM, cfg.YOUR_OTHER_PARAM).to(cfg.device)
     optim = optimizer.AdamW(model.parameters(), lr=cfg.YOUR_LEARNING_RATE_PARAM, amsgrad=True)
 
     # we can check if we have trained this model before, and if we have, just load it
     # this checking is done using the `version_number` param, if `latest=True` is set,
     # Wingman automatically searches for the latest model checkpoint,
     # otherwise, Wingman uses the checkpoint specified by `mark_number`
-    have_file, weight_file, optim_file = self.get_weight_files(latest=True)
+    have_file, weight_file, optim_file = wm.get_weight_files(latest=True)
     if have_file:
         # Wingman simply returns a string of where the weight files are
         # no unnecessary wrapping!
         model.load_state_dict(torch.load(model_file))
         optim.load_state_dict(torch.load(optim_file))
 
     # let's run some training:
@@ -154,14 +159,21 @@
         update_weights, model_file, optim_file = wm.checkpoint(loss, training_step)
         if update_weights:
             # if Wingman deems that the weights should be checkpointed, it returns
             # a string of where the weight files should go for it to be found later
             torch.save(model.state_dict(), model_file)
             torch.save(optim.state_dict(), optim_file)
 ```
+#### Weights Directory Compression
+
+If you train a lot of models, the weights directory can start to use a lot of disk space.
+Running `wingman-compress-weights [optional directory name]` on the commandline will remove all redundant mark numbers and delete all empty files.
+
+
+<br>
 
 ### `from wingman import NeuralBlocks`
 
 Neural blocks is a module for quickly prototyping neural network architectures.
 It offers several easier methods of defining standardized modules:
 
 #### Simple 3-layer MLP with ReLU activation
@@ -253,14 +265,17 @@
     (1): LeakyReLU(negative_slope=0.01)
   )
 )
 ```
 
 The Neural Blocks module also has functions that can generate single modules, refer to the file itself for more details.
 
+
+<br>
+
 ### `from wingman import ReplayBuffer`
 
 This is a replay buffer designed around Torch's Dataloader class for reinforcement learning projects.
 This allows easy bootstrapping of the Dataloader's excellent shuffling and pre-batching capabilities.
 In addition, all the data is stored as a numpy array in a contiguous block of memory, allowing very fast retrieval.
 ReplayBuffer also doesn't put any limits on tuple length per transition; some people prefer to store $\{S, A, R, S'\}$, some prefer to store $\{S, A, R, S', A'\}$ - ReplayBuffer doesn't care!
 The length of the tuple can be as long or as short as you want, as long as every tuple fed in is the same length and each element of the tuple is the same shape.
@@ -302,14 +317,17 @@
     observations = gpuize(stuff[0], "cuda:0")
     actions = gpuize(stuff[1], "cuda:0")
     rewards = gpuize(stuff[2], "cuda:0")
     next_states = gpuize(stuff[3], "cuda:0")
     dones = gpuize(stuff[4], "cuda:0")
 ```
 
+
+<br>
+
 ### `from wingman import gpuize, cpuize`
 
 These are quality of life standalone functions.
 
 ```python
 >>> import numpy as np
 >>> from wingman import gpuize, cpuize
@@ -327,16 +345,16 @@
 
 tensor([[0.2839, 0.5094, 0.5543, 0.4561, 0.8252],
         [0.7744, 0.2090, 0.8622, 0.6907, 0.9486],
         [0.7008, 0.9278, 0.9839, 0.7695, 0.7289],
         [0.4770, 0.5497, 0.2211, 0.7244, 0.4257],
         [0.7833, 0.8489, 0.6853, 0.6188, 0.1356]], device='cuda:0')
 
->>> pae = cpuize(bar)
->>> print(pae)
+>>> baz = cpuize(bar)
+>>> print(baz)
 
 [[0.28392764 0.50936983 0.55433616 0.45614518 0.82523046]
  [0.77437072 0.20900382 0.86220494 0.69071239 0.94863786]
  [0.70082865 0.92780018 0.98392965 0.76945165 0.72886401]
  [0.47702485 0.54968522 0.22110942 0.72436276 0.42574472]
  [0.78330221 0.84888837 0.68529167 0.61878902 0.13556213]]
 ```
```

### Comparing `jj_wingman-0.1.9/pyproject.toml` & `jj_wingman-0.2.0/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -2,30 +2,36 @@
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jj_wingman"
-version = "0.1.9"
+version = "0.2.0"
 authors = [
   { name="Jet", email="taijunjet@hotmail.com" },
 ]
 description = "Wingman library for AI projects."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
-dependencies = ["numpy", "torch", "wandb", "pyyaml"]
+dependencies = ["numpy", "wandb", "pyyaml"]
 keywords = ["Machine Learning"]
 license = { file="./LICENSE.txt" }
 
+[tool.setuptools]
+include-package-data = true
+
+[tool.setuptools.packages.find]
+include = ["wingman", "wingman.*"]
+
 [project.scripts]
 wingman-generate-yaml = "wingman:generate_yaml"
 wingman-compress-weights = "wingman:compress_weights"
 
 [project.urls]
 "Homepage" = "https://github.com/jjshoots/Wingman"
```

### Comparing `jj_wingman-0.1.9/wingman/neural_blocks.py` & `jj_wingman-0.2.0/wingman/neural_blocks.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,16 @@
-#!/usr/bin/env python3
+"""Easy creation of neural networks."""
 from typing import List, Optional
 
-import torch.nn as nn
+try:
+    import torch.nn as nn
+except ImportError as e:
+    raise ImportError(
+        "Could not import torch, this is not bundled as part of Wingman and has to be installed manually."
+    ) from e
 
 
 class NeuralBlocks:
     """NeuralBlocks."""
 
     def __init__(self):
         """__init__."""
```

### Comparing `jj_wingman-0.1.9/wingman/wingman.py` & `jj_wingman-0.2.0/wingman/wingman.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,22 @@
-#!/usr/bin/env python3
+"""The core of Wingman."""
+from __future__ import annotations
+
 import argparse
 import math
 import os
 import time
-from typing import Optional, Tuple
+from typing import Tuple
 
 import numpy as np
-import torch
 import wandb
 import yaml
 
+from .print_utils import cstr, wm_print
+
 
 class Wingman:
     """Wingman.
 
     Class to handle checkpointing of loss and handling of weights files.
     Minimal example:
 
@@ -61,44 +64,35 @@
         self.cfg = self.__yaml_to_args()
 
         # make sure that logging_interval is positive
         assert (
             self.cfg.logging_interval > 0
         ), f"logging_interval must be a positive number, got {self.cfg.logging_interval}."
 
-        # the interval before we save things
-        self.logging_interval = self.cfg.logging_interval
-
-        # maximum skips allowed before save to intermediary
-        self.max_skips = self.cfg.max_skips
+        # the logger
+        self.log = dict()
 
         # runtime variables
         self.num_losses = 0
         self.cumulative_loss = 0
         self.lowest_loss = math.inf
-        self.next_log_step = self.logging_interval
+        self.next_log_step = self.cfg.logging_interval
         self.previous_checkpoint_step = 0
         self.skips = 0
 
-        # the logger
-        self.log = dict()
-
-        # minimum required before new weight file is made
-        self.greater_than = self.cfg.greater_than
-
         # weight file variables
         self.directory = os.path.dirname(__file__)
         self.version_number = self.cfg.version_number
         self.mark_number = self.cfg.mark_number
+        self.previous_mark_number = -1
 
         # directory itself
         self.version_directory = os.path.join(
             self.cfg.weights_directory, f"Version{self.version_number}"
         )
-        self.version_dir_print = self.version_directory.split("/")[-2]
 
         # file paths
         self.model_file = os.path.join(
             self.version_directory,
             f"weights{self.mark_number}.pth",
         )
         self.optim_file = os.path.join(
@@ -107,47 +101,63 @@
         )
         self.status_file = os.path.join(
             self.version_directory,
             "lowest_loss.npy",
         )
         self.intermediary_file = os.path.join(
             self.version_directory,
-            "weights_intermediary.pth",
+            "weights-1.pth",
         )
 
-        print("--------------𓆩𓆪--------------")
-        print(f"Using Device {self.device}")
-        print(f"Saving weights to {self.version_directory}...")
+        wm_print("--------------𓆩𓆪--------------")
+        wm_print(f"Using device {cstr(self.device, 'HEADER')}")
+        wm_print(f"Saving weights to {cstr(self.version_directory, 'HEADER')}...")
 
-        # record that we're in a new training session
+        # check to record that we're in a new training session
+        self.fresh_directory = False
         if not os.path.isdir(self.version_directory):
-            print("Weights directory not found, generating new one in 3 seconds...")
+            self.fresh_directory = True
+            wm_print(
+                cstr(
+                    "New training instance detected, generating weights directory in 3 seconds...",
+                    "WARNING",
+                )
+            )
             time.sleep(3)
             os.makedirs(self.version_directory)
 
     def __get_device(self):
         """__get_device."""
-        device = "cpu"
-        if torch.cuda.is_available():
-            device = torch.device("cuda:0")
+        from warnings import warn
 
-        self.device = device
-        return device
+        try:
+            import torch
+
+            if torch.cuda.is_available():
+                self.device = torch.device("cuda:0")
+            else:
+                self.device = "cpu"
+        except ImportError:
+            warn(
+                "Could not import torch, this is not bundled as part of Wingman and has to be installed manually."
+            )
+            self.device = "Not Found!"
+
+        return self.device
 
     def __yaml_to_args(self):
         """__yaml_to_args.
 
         Reads the yaml file provided at init and converts it to commandline arguments.
 
         """
         # parse the arguments
         parser = argparse.ArgumentParser(description=self.experiment_description)
 
         with open(self.config_yaml) as f:
-
             # read in the file
             config = yaml.load(f, Loader=yaml.FullLoader)
 
             # checks that we have the default params in the file
             assertation_list = [
                 "debug",
                 "weights_directory",
@@ -161,22 +171,24 @@
                 "wandb_name",
                 "wandb_notes",
                 "wandb_id",
                 "wandb_entity",
                 "wandb_project",
             ]
             for item in assertation_list:
-                assert item in config, f"Missing parameter {item} in config file."
+                assert item in config, cstr(
+                    f"Missing parameter {item} in config file.", "FAIL"
+                )
 
-            for item in config:
-                # exclusively for version number only
-                if item == "version_number":
-                    if config[item] is None:
-                        config[item] = np.random.randint(999999)
+            # override version number if needed
+            if config["version_number"] is None:
+                config["version_number"] = np.random.randint(999999)
 
+            # add all to argparse
+            for item in config:
                 parser.add_argument(
                     f"--{item}",
                     type=type(config[item]),
                     nargs="?",
                     const=True,
                     default=config[item],
                     help="None",
@@ -214,120 +226,136 @@
             cfg = wandb.config
         else:
             # otherwise just merge settings with args
             cfg = argparse.Namespace(**config)
 
         return cfg
 
-    def checkpoint(self, loss: float, step: int) -> Tuple[bool, str, str]:
+    def checkpoint(self, loss: float, step: int | None = None) -> Tuple[bool, str, str]:
         """checkpoint.
 
         Records training every logging_interval steps.
 
         Returns three things:
         - indicator on whether we should save weights
         - directory of where the weight files should be saved
         - directory of where the optim files should be saved
 
         Args:
             loss (float): learning loss of the model as a detached float
-            step (int): step number
+            step (int | None): step number, automatically incremented if None
 
         Returns:
-            Tuple[bool, str, str]:
+            Tuple[bool, str, str]: to_update, weights_file, optim_file
         """
-        # indicator on whether we need to save the weights
-        update = False
+        # if step is None, we automatically increment
+        if step is None:
+            step = self.previous_checkpoint_step + 1
 
         # check that our step didn't go in reverse
-        assert (
-            step >= self.previous_checkpoint_step
-        ), f"We can't step backwards! Got step {step} but the previous logging step was {self.previous_checkpoint_step}."
+        assert step >= self.previous_checkpoint_step, cstr(
+            f"We can't step backwards! Got step {step} but the previous logging step was {self.previous_checkpoint_step}.",
+            "FAIL",
+        )
         self.previous_checkpoint_step = step
 
-        # accumulate the loss
+        """ACCUMULATE LOSS"""
         self.cumulative_loss += loss
         self.num_losses += 1.0
 
-        # check if n steps have passed and it is not the first step, we save here
-        if step >= self.next_log_step:
-            # compute the next time we need to log
-            self.next_log_step = (
-                int(step / self.logging_interval) + 1
-            ) * self.logging_interval
-
-            # record the losses and reset the cumulative
-            avg_loss = self.cumulative_loss / self.num_losses
-            self.cumulative_loss = 0.0
-            self.num_losses = 0.0
-
-            # always print on n intervals
-            print(
-                f"Step {step}; Average Loss {avg_loss:.5f}; Lowest Average Loss {self.lowest_loss:.5f}"
-            )
-
-            # log to wandb if needed
-            if self.cfg.wandb:
-                self.wandb_log()
-
-            # perform a save if we have found a new lowest loss
-            if avg_loss < self.lowest_loss:
-                # redefine the new lowest loss
-                self.lowest_loss = avg_loss
+        # if we haven't passed the required number of steps
+        if step < self.next_log_step:
+            return False, self.model_file, self.optim_file
+
+        # log to wandb if needed, but only on the logging steps
+        if self.cfg.wandb:
+            self.wandb_log()
+
+        """GET NEW AVG LOSS"""
+        # record the losses and reset the cumulative
+        avg_loss = self.cumulative_loss / self.num_losses
+        self.cumulative_loss = 0.0
+        self.num_losses = 0.0
+
+        # compute the next time we need to log
+        self.next_log_step = (
+            int(step / self.cfg.logging_interval) + 1
+        ) * self.cfg.logging_interval
+
+        # always print on n intervals
+        wm_print(
+            f"Step {cstr(step, 'OKCYAN')}; Average Loss {cstr(f'{avg_loss:.5f}', 'OKCYAN')}; Lowest Average Loss {cstr(f'{self.lowest_loss:.5f}', 'OKCYAN')}"
+        )
 
-                # reset the number of skips
+        """CHECK IF NEW LOSS IS BETTER"""
+        # if we don't meet the criteria for saving
+        if avg_loss >= self.lowest_loss - self.cfg.greater_than:
+            # accumulate skips
+            if self.skips < self.cfg.max_skips:
+                self.skips += 1
+                return False, self.model_file, self.optim_file
+            else:
+                # save the network to intermediary if we crossed the max number of skips
+                wm_print(
+                    f"Passed {self.cfg.max_skips} intervals without saving so far, saving weights to: {cstr(self.intermediary_file, 'OKCYAN')}"
+                )
                 self.skips = 0
+                return True, self.intermediary_file, self.optim_file
 
-                # increment the mark number
-                if self.cfg.increment:
-                    # regenerate the weights_file path
-                    self.model_file = os.path.join(
-                        self.version_directory,
-                        f"weights{self.mark_number}.pth",
-                    )
-                    self.mark_number += 1
+        """NEW LOSS IS BETTER"""
+        # redefine the new lowest loss and reset the skips
+        self.lowest_loss = avg_loss
+        self.skips = 0
 
-                print(
-                    f"New lowest point, saving weights to: {self.version_dir_print}/weights{self.mark_number}.pth"
+        # increment means return the files with incremented mark number
+        if self.cfg.increment:
+            # check if we are safe to increment mark numbers and regenerate weights file
+            if self.previous_mark_number == -1 or os.path.isfile(self.model_file):
+                self.previous_mark_number = self.mark_number
+                self.model_file = os.path.join(
+                    self.version_directory,
+                    f"weights{self.mark_number}.pth",
                 )
+                self.mark_number += 1
 
-                # record the lowest running loss in the status file
-                np.save(self.status_file, self.lowest_loss)
-
-                update = True
             else:
-                # save the network to intermediary if we crossed the max number of skips
-                if self.skips >= self.max_skips:
-                    self.skips = 0
-                    print(
-                        f"Passed {self.max_skips} intervals without saving so far, saving weights to: /weights_intermediary.pth"
+                wm_print(
+                    cstr(
+                        "Didn't save weights file for the previous mark number (self.mark_number), not incrementing mark number.",
+                        "WARNING",
                     )
+                )
+                self.mark_number = self.previous_mark_number
+
+        # record the lowest running loss in the status file
+        np.save(self.status_file, self.lowest_loss)
 
-                    return True, self.intermediary_file, self.optim_file
-                else:
-                    self.skips += 1
+        wm_print(
+            f"New lowest point, saving weights to: {cstr(self.model_file, 'OKGREEN')}"
+        )
 
-        return update, self.model_file, self.optim_file
+        return True, self.model_file, self.optim_file
 
     def wandb_log(self) -> None:
         """wandb_log.
 
         Logs the internal log to WandB.
         Start logging by adding things to it using:
         ```
         wm.log["foo"] = "bar"
         ```
 
         Returns:
             None:
         """
-        assert isinstance(
-            self.log, dict
-        ), f"log must be dictionary, currently it is {self.log}."
-        wandb.log(self.log)
+        assert isinstance(self.log, dict), cstr(
+            f"log must be dictionary, currently it is {self.log}.", "FAIL"
+        )
+        if self.cfg.wandb:
+            wandb.log(self.log)
 
     def write_auxiliary(
         self, data: np.ndarray, variable_name: str, precision: str = "%1.3f"
     ) -> None:
         """write_auxiliary.
 
         Args:
@@ -339,75 +367,79 @@
             None:
         """
         assert len(data.shape) == 1, "Data must be only 1 dimensional ndarray"
         filename = os.path.join(self.version_directory, f"{variable_name}.csv")
         with open(filename, "ab") as f:
             np.savetxt(f, [data], delimiter=",", fmt=precision)
 
-    def get_weight_files(
-        self, latest: bool = True
-    ) -> Tuple[bool, Optional[str], Optional[str]]:
+    def get_weight_files(self, latest: bool = True) -> Tuple[bool, str, str]:
         """get_weight_files.
 
         Returns three things:
         - indicator on whether we have weight files
         - directory of where the weight files are
         - directory of where the optim files are
 
         Args:
             latest (bool): whether we want the latest file or the one determined by `mark_number`
 
         Returns:
-            Tuple[bool, Optional[str], Optional[str]]:
+            Tuple[bool, str, str]: have_file, weights_file, optim_file
         """
-        have_file = False
-
         # if we don't need the latest file, get the one specified
         if not latest:
             if os.path.isfile(self.model_file):
                 self.model_file = os.path.join(
                     self.version_directory,
                     f"weights{self.mark_number}.pth",
                 )
-                have_file = True
-                return have_file, self.model_file, self.optim_file
+                return True, self.model_file, self.optim_file
+            else:
+                raise ValueError(
+                    cstr(
+                        f"Mark number {self.mark_number} was requested, but it doesn't exist.",
+                        "FAIL",
+                    )
+                )
 
         # while the file exists, try to look for a file one version later
+        self.mark_number = 0
         while os.path.isfile(self.model_file):
             self.mark_number += 1
             self.model_file = os.path.join(
                 self.version_directory,
                 f"weights{self.mark_number}.pth",
             )
 
         # once the file version doesn't exist, decrement by one and use that file
-        self.mark_number -= 1 if self.mark_number > 0 else 0
+        self.mark_number = max(self.mark_number - 1, 0)
         self.model_file = os.path.join(
             self.version_directory,
             f"weights{self.mark_number}.pth",
         )
 
-        # if there's no files, ignore, otherwise, print the file
-        if os.path.isfile(self.model_file):
+        # if the file doesn't exist, notify and ignore
+        if not os.path.isfile(self.model_file):
+            if not self.fresh_directory:
+                wm_print(
+                    cstr(
+                        "No weights file found, generating new one during training.",
+                        "WARNING",
+                    )
+                )
+            self.fresh_directory = False
+
+            return False, self.model_file, self.optim_file
+        else:
             # hitch a ride to update the lowest running loss
             self.lowest_loss = np.load(self.status_file).item()
 
-            print(
-                f"Using weights file: /{self.version_dir_print}/weights{self.mark_number}.pth"
+            wm_print(
+                f"Using weights file: {cstr(f'{self.version_directory}/weights{self.mark_number}.pth', 'OKGREEN')}"
             )
+            wm_print(f"Lowest Running Loss for Net: {cstr(self.lowest_loss, 'OKCYAN')}")
 
-            print(f"Lowest Running Loss for Net: {self.lowest_loss}")
+            # check if the optim file exists
+            if not os.path.isfile(self.optim_file):
+                wm_print(cstr("Optim file not found, please be careful!", "WARNING"))
 
-            have_file = True
-        else:
-            print("No weights file found, generating new one during training.")
-            have_file = False
-
-        # check if the optim file exists
-        if not os.path.isfile(self.optim_file):
-            print("Optim file not found, please be careful!")
-
-        # return depending on whether we've found the file
-        if have_file:
-            return have_file, self.model_file, self.optim_file
-        else:
-            return have_file, None, None
+            return True, self.model_file, self.optim_file
```

