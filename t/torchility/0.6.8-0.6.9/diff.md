# Comparing `tmp/torchility-0.6.8.tar.gz` & `tmp/torchility-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchility-0.6.8.tar", last modified: Mon May 15 08:02:25 2023, max compression
+gzip compressed data, was "torchility-0.6.9.tar", last modified: Mon May 15 12:12:54 2023, max compression
```

## Comparing `torchility-0.6.8.tar` & `torchility-0.6.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-05-15 08:02:25.452181 torchility-0.6.8/
--rw-r--r--   0 liuchen    (501) staff       (20)     1073 2020-01-28 04:19:18.000000 torchility-0.6.8/LICENSE
--rw-r--r--   0 liuchen    (501) staff       (20)     2074 2023-05-15 08:02:25.451704 torchility-0.6.8/PKG-INFO
--rw-r--r--   0 liuchen    (501) staff       (20)     1595 2023-03-20 06:35:45.000000 torchility-0.6.8/README.md
-drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-05-15 08:02:25.435612 torchility-0.6.8/examples/
--rw-r--r--   0 liuchen    (501) staff       (20)     1728 2023-05-13 05:23:14.000000 torchility-0.6.8/examples/1-mnist.py
--rw-r--r--   0 liuchen    (501) staff       (20)     2663 2023-03-28 13:54:47.000000 torchility-0.6.8/examples/2-mnist_callbacks.py
--rw-r--r--   0 liuchen    (501) staff       (20)     2223 2023-05-15 07:37:59.000000 torchility-0.6.8/examples/3-mnist_interpreter.py
--rw-r--r--   0 liuchen    (501) staff       (20)     1645 2023-05-15 07:55:10.000000 torchility-0.6.8/examples/4-mnist_model_analysis.py
--rw-r--r--   0 liuchen    (501) staff       (20)     1419 2022-05-28 01:44:42.000000 torchility-0.6.8/examples/5-mnist_lr_find.py
--rw-r--r--   0 liuchen    (501) staff       (20)     1962 2022-12-09 04:27:52.000000 torchility-0.6.8/examples/6-graph_node_clasification_DGL.py
--rw-r--r--   0 liuchen    (501) staff       (20)       38 2023-05-15 08:02:25.452448 torchility-0.6.8/setup.cfg
--rw-r--r--   0 liuchen    (501) staff       (20)     1117 2023-05-05 12:13:44.000000 torchility-0.6.8/setup.py
-drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-05-15 08:02:25.439312 torchility-0.6.8/torchility/
--rw-r--r--   0 liuchen    (501) staff       (20)      503 2023-05-15 08:01:49.000000 torchility-0.6.8/torchility/__init__.py
-drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-05-15 08:02:25.446736 torchility-0.6.8/torchility/callbacks/
--rw-r--r--   0 liuchen    (501) staff       (20)      101 2022-05-08 12:50:22.000000 torchility-0.6.8/torchility/callbacks/__init__.py
--rw-r--r--   0 liuchen    (501) staff       (20)     1191 2023-05-15 06:05:49.000000 torchility-0.6.8/torchility/callbacks/common.py
--rw-r--r--   0 liuchen    (501) staff       (20)     4840 2023-05-05 13:46:18.000000 torchility-0.6.8/torchility/callbacks/interpreters.py
--rw-r--r--   0 liuchen    (501) staff       (20)     3036 2023-03-19 07:43:59.000000 torchility-0.6.8/torchility/callbacks/performances.py
--rw-r--r--   0 liuchen    (501) staff       (20)     9501 2023-05-15 07:53:51.000000 torchility-0.6.8/torchility/callbacks/progress.py
--rw-r--r--   0 liuchen    (501) staff       (20)     1092 2023-05-15 07:41:02.000000 torchility-0.6.8/torchility/datamodule.py
--rw-r--r--   0 liuchen    (501) staff       (20)     2390 2021-06-09 14:49:55.000000 torchility-0.6.8/torchility/hooks.py
--rw-r--r--   0 liuchen    (501) staff       (20)      577 2021-06-10 07:05:35.000000 torchility-0.6.8/torchility/losses.py
--rw-r--r--   0 liuchen    (501) staff       (20)     5023 2023-05-15 07:26:34.000000 torchility-0.6.8/torchility/metrics.py
--rw-r--r--   0 liuchen    (501) staff       (20)     6612 2023-05-15 07:34:33.000000 torchility-0.6.8/torchility/tasks.py
--rw-r--r--   0 liuchen    (501) staff       (20)    10601 2023-05-15 05:43:20.000000 torchility-0.6.8/torchility/trainer.py
-drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-05-15 08:02:25.450911 torchility-0.6.8/torchility/utils/
--rw-r--r--   0 liuchen    (501) staff       (20)       96 2023-05-15 04:51:01.000000 torchility-0.6.8/torchility/utils/__init__.py
--rw-r--r--   0 liuchen    (501) staff       (20)     2512 2023-05-15 07:06:33.000000 torchility-0.6.8/torchility/utils/metric_utils.py
--rw-r--r--   0 liuchen    (501) staff       (20)     4222 2022-06-02 14:28:56.000000 torchility-0.6.8/torchility/utils/plots.py
--rw-r--r--   0 liuchen    (501) staff       (20)     6050 2023-05-05 01:14:22.000000 torchility-0.6.8/torchility/utils/utils.py
--rw-r--r--   0 liuchen    (501) staff       (20)     3014 2022-08-04 03:32:03.000000 torchility-0.6.8/torchility/utils/yaml_config.py
-drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-05-15 08:02:25.441696 torchility-0.6.8/torchility.egg-info/
--rw-r--r--   0 liuchen    (501) staff       (20)     2074 2023-05-15 08:02:25.000000 torchility-0.6.8/torchility.egg-info/PKG-INFO
--rw-r--r--   0 liuchen    (501) staff       (20)      853 2023-05-15 08:02:25.000000 torchility-0.6.8/torchility.egg-info/SOURCES.txt
--rw-r--r--   0 liuchen    (501) staff       (20)        1 2023-05-15 08:02:25.000000 torchility-0.6.8/torchility.egg-info/dependency_links.txt
--rw-r--r--   0 liuchen    (501) staff       (20)       83 2023-05-15 08:02:25.000000 torchility-0.6.8/torchility.egg-info/requires.txt
--rw-r--r--   0 liuchen    (501) staff       (20)       11 2023-05-15 08:02:25.000000 torchility-0.6.8/torchility.egg-info/top_level.txt
+drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-05-15 12:12:54.015920 torchility-0.6.9/
+-rw-r--r--   0 liuchen    (501) staff       (20)     1073 2020-01-28 04:19:18.000000 torchility-0.6.9/LICENSE
+-rw-r--r--   0 liuchen    (501) staff       (20)     2074 2023-05-15 12:12:54.014770 torchility-0.6.9/PKG-INFO
+-rw-r--r--   0 liuchen    (501) staff       (20)     1595 2023-03-20 06:35:45.000000 torchility-0.6.9/README.md
+drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-05-15 12:12:53.988128 torchility-0.6.9/examples/
+-rw-r--r--   0 liuchen    (501) staff       (20)     1728 2023-05-13 05:23:14.000000 torchility-0.6.9/examples/1-mnist.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     2663 2023-03-28 13:54:47.000000 torchility-0.6.9/examples/2-mnist_callbacks.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     2223 2023-05-15 07:37:59.000000 torchility-0.6.9/examples/3-mnist_interpreter.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     1645 2023-05-15 07:55:10.000000 torchility-0.6.9/examples/4-mnist_model_analysis.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     1419 2022-05-28 01:44:42.000000 torchility-0.6.9/examples/5-mnist_lr_find.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     1962 2022-12-09 04:27:52.000000 torchility-0.6.9/examples/6-graph_node_clasification_DGL.py
+-rw-r--r--   0 liuchen    (501) staff       (20)       38 2023-05-15 12:12:54.016115 torchility-0.6.9/setup.cfg
+-rw-r--r--   0 liuchen    (501) staff       (20)     1117 2023-05-05 12:13:44.000000 torchility-0.6.9/setup.py
+drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-05-15 12:12:53.992376 torchility-0.6.9/torchility/
+-rw-r--r--   0 liuchen    (501) staff       (20)      503 2023-05-15 12:09:07.000000 torchility-0.6.9/torchility/__init__.py
+drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-05-15 12:12:54.006213 torchility-0.6.9/torchility/callbacks/
+-rw-r--r--   0 liuchen    (501) staff       (20)      101 2022-05-08 12:50:22.000000 torchility-0.6.9/torchility/callbacks/__init__.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     1205 2023-05-15 08:23:01.000000 torchility-0.6.9/torchility/callbacks/common.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     4840 2023-05-05 13:46:18.000000 torchility-0.6.9/torchility/callbacks/interpreters.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     3036 2023-03-19 07:43:59.000000 torchility-0.6.9/torchility/callbacks/performances.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     9598 2023-05-15 12:11:12.000000 torchility-0.6.9/torchility/callbacks/progress.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     1102 2023-05-15 09:10:40.000000 torchility-0.6.9/torchility/datamodule.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     2390 2021-06-09 14:49:55.000000 torchility-0.6.9/torchility/hooks.py
+-rw-r--r--   0 liuchen    (501) staff       (20)      577 2021-06-10 07:05:35.000000 torchility-0.6.9/torchility/losses.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     5023 2023-05-15 07:26:34.000000 torchility-0.6.9/torchility/metrics.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     6694 2023-05-15 08:53:50.000000 torchility-0.6.9/torchility/tasks.py
+-rw-r--r--   0 liuchen    (501) staff       (20)    10682 2023-05-15 11:48:35.000000 torchility-0.6.9/torchility/trainer.py
+drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-05-15 12:12:54.013665 torchility-0.6.9/torchility/utils/
+-rw-r--r--   0 liuchen    (501) staff       (20)       96 2023-05-15 04:51:01.000000 torchility-0.6.9/torchility/utils/__init__.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     2525 2023-05-15 09:18:12.000000 torchility-0.6.9/torchility/utils/metric_utils.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     4222 2022-06-02 14:28:56.000000 torchility-0.6.9/torchility/utils/plots.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     6050 2023-05-05 01:14:22.000000 torchility-0.6.9/torchility/utils/utils.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     3014 2022-08-04 03:32:03.000000 torchility-0.6.9/torchility/utils/yaml_config.py
+drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-05-15 12:12:53.999542 torchility-0.6.9/torchility.egg-info/
+-rw-r--r--   0 liuchen    (501) staff       (20)     2074 2023-05-15 12:12:53.000000 torchility-0.6.9/torchility.egg-info/PKG-INFO
+-rw-r--r--   0 liuchen    (501) staff       (20)      853 2023-05-15 12:12:53.000000 torchility-0.6.9/torchility.egg-info/SOURCES.txt
+-rw-r--r--   0 liuchen    (501) staff       (20)        1 2023-05-15 12:12:53.000000 torchility-0.6.9/torchility.egg-info/dependency_links.txt
+-rw-r--r--   0 liuchen    (501) staff       (20)       83 2023-05-15 12:12:53.000000 torchility-0.6.9/torchility.egg-info/requires.txt
+-rw-r--r--   0 liuchen    (501) staff       (20)       11 2023-05-15 12:12:53.000000 torchility-0.6.9/torchility.egg-info/top_level.txt
```

### Comparing `torchility-0.6.8/LICENSE` & `torchility-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `torchility-0.6.8/PKG-INFO` & `torchility-0.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchility
-Version: 0.6.8
+Version: 0.6.9
 Summary: UNKNOWN
 Home-page: https://github.com/hitlic/torchility
 Author: hitlic
 Author-email: liuchen.lic@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `torchility-0.6.8/README.md` & `torchility-0.6.9/README.md`

 * *Files identical despite different names*

### Comparing `torchility-0.6.8/examples/1-mnist.py` & `torchility-0.6.9/examples/1-mnist.py`

 * *Files identical despite different names*

### Comparing `torchility-0.6.8/examples/2-mnist_callbacks.py` & `torchility-0.6.9/examples/2-mnist_callbacks.py`

 * *Files identical despite different names*

### Comparing `torchility-0.6.8/examples/3-mnist_interpreter.py` & `torchility-0.6.9/examples/3-mnist_interpreter.py`

 * *Files identical despite different names*

### Comparing `torchility-0.6.8/examples/4-mnist_model_analysis.py` & `torchility-0.6.9/examples/4-mnist_model_analysis.py`

 * *Files identical despite different names*

### Comparing `torchility-0.6.8/examples/5-mnist_lr_find.py` & `torchility-0.6.9/examples/5-mnist_lr_find.py`

 * *Files identical despite different names*

### Comparing `torchility-0.6.8/examples/6-graph_node_clasification_DGL.py` & `torchility-0.6.9/examples/6-graph_node_clasification_DGL.py`

 * *Files identical despite different names*

### Comparing `torchility-0.6.8/setup.py` & `torchility-0.6.9/setup.py`

 * *Files identical despite different names*

### Comparing `torchility-0.6.8/torchility/callbacks/common.py` & `torchility-0.6.9/torchility/callbacks/common.py`

 * *Files 14% similar despite different names*

```diff
@@ -24,12 +24,12 @@
 def reset_metrics(stage, task):    # 重置指标
     metrics = task.metrics[stage]
     metric_values = {}
     for metric in metrics:
         value = metric.compute()
         if isinstance(value, dict):
             for k, v in value.items():
-                metric_values[f"{metric.name}{k}"] = v
+                metric_values[f"{metric.name}{k}"] = v.item()
         else:
-            metric_values[metric.name] = value
+            metric_values[metric.name] = value.item()
         metric.reset()
     return metric_values
```

### Comparing `torchility-0.6.8/torchility/callbacks/interpreters.py` & `torchility-0.6.9/torchility/callbacks/interpreters.py`

 * *Files identical despite different names*

### Comparing `torchility-0.6.8/torchility/callbacks/performances.py` & `torchility-0.6.9/torchility/callbacks/performances.py`

 * *Files identical despite different names*

### Comparing `torchility-0.6.8/torchility/callbacks/progress.py` & `torchility-0.6.9/torchility/callbacks/progress.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,14 @@
         def on_train_batch_end(self, trainer, pl_module, outputs, batch, batch_idx, dataloader_idx):
             self.train_batch_id = batch_idx + 1
         def on_validation_batch_end(self, trainer, pl_module, outputs, batch, batch_idx, dataloader_idx):
             self.val_batch_id = batch_idx + 1
         def on_test_batch_end(self, trainer, pl_module, outputs, batch, batch_idx, dataloader_idx):
             self.test_batch_id = batch_idx + 1
     """
-
     def get_info(self, trainer, stage):
         """
         返回当前epoch数，总epoch数，当前batch总，总batch数。
         Args:
             trainer (Trainer): Trainer.
             stage (str): 'train', 'val' or 'test'.
         Returns:
@@ -49,31 +48,31 @@
         is_val_epoch = (trainer.current_epoch + 1) % trainer.check_val_every_n_epoch == 0
         total_val_batches = sum(trainer.num_val_batches) if is_val_epoch else 0
         return total_val_batches
 
     def get_epoch_loss(self, trainer, stage):
         cbk_metrics = trainer.callback_metrics
         if stage == 'train':
-            return {'loss': cbk_metrics['train_loss_epoch']}
+            return {'loss': cbk_metrics['train_loss_epoch'].item()}
         else:
-            return {self._loss_key(k):v for k,v in cbk_metrics.items() if f'{stage}_loss_epoch' in k}
+            return {self._loss_key(k): v.item() for k,v in cbk_metrics.items() if f'{stage}_loss_epoch' in k}
 
     def _loss_key(self, k):
         if '/dataloader_idx_' in k:
             return f"loss/{k.split('_')[-1]}"
-        elif k=='test_loss_epoch':
+        elif k in ['val_loss_epoch', 'test_loss_epoch']:
             return 'loss'
         else:
             return k
 
+
 class SimpleBar(ProgressBar, ProgressMix):
     """
-    仅输出文本信息的进度条
+    自定义进度显示
     """
-
     def __init__(self):
         self.train_batch_id = 0
         self.val_batch_id = 0
         self.test_batch_id = 0
 
     def disable(self):
         self.enable = True
@@ -114,17 +113,14 @@
         c_epoch, num_epoch, c_batch, num_batch  = self.get_info(trainer, 'val')
         progress = f"E:{c_epoch:>3d}/{num_epoch:<3d} B:{c_batch:>4d}/{num_batch:<4}"
         stage = '  VAL >'
         info = '  '.join([f'{k:>}: {v:0<6.4f}' for k, v in outputs.items()])
         print(f"{progress} {stage} {info}", end="\r", flush=True)
         return super().on_validation_batch_end(trainer, pl_module, outputs, batch, batch_idx, dataloader_idx)
 
-    def on_test_epoch_start(self, trainer, pl_module):
-        print('-' * 23)
-
     def on_test_batch_end(self, trainer, pl_module, outputs, batch, batch_idx: int, dataloader_idx: int = 0):
         self.test_batch_id = batch_idx + 1
         c_epoch, num_epoch, c_batch, num_batch = self.get_info(trainer, 'test')
         progress = f"E:{c_epoch:>3d}/{num_epoch:<3d} B:{c_batch:>4d}/{num_batch:<4}"
         stage = ' TEST >'
         info = '  '.join([f'{k:>}: {v:0<6.4f}' for k, v in outputs.items()])
         print(f"{progress} {stage} {info}", end="\r", flush=True)
@@ -133,20 +129,25 @@
     def on_test_epoch_end(self, trainer, pl_module):
         c_epoch, num_epoch, c_batch, num_batch = self.get_info(trainer, 'test')
         info_dict = self.get_epoch_loss(trainer, 'test')
         info_dict.update(trainer.test_epoch_metric_values)
         progress = f"E:{c_epoch:>3d}/{num_epoch:<3d} B:{c_batch:>4d}/{num_batch:<4}"
         stage = ' TEST >'
         info = '  '.join([f'{k:>}: {v:0<6.4f}' for k, v in info_dict.items()])
+        trainer.test_metrics = info_dict
         print(progress, stage, info)
 
 
 PrintProgressBar = SimpleBar
 
+
 class Progress(Callback, ProgressMix):
+    """
+    保存训练、验证过程中的指标数据，用于作为 trainer.fit 方法的返回结果
+    """
     def __init__(self, unit='epoch'):
         assert unit in ['epoch', 'step'], '`unit` must be epoch or step'
         self.unit = unit
 
         self.train_batch_id = 0
         self.val_batch_id = 0
         self.test_batch_id = 0
@@ -179,15 +180,15 @@
 
     def on_train_epoch_end(self, trainer, pl_module):
         if self.unit == 'epoch':
             info_dict = self.get_epoch_loss(trainer, 'train')
             info_dict.update(trainer.train_epoch_metric_values)
             self.curent_epoch['train_epoch'] = info_dict
         self.progress_info.append(self.curent_epoch)
-    
+
     def on_test_epoch_end(self, trainer, pl_module):
         if self.unit == 'epoch':
             info_dict = self.get_epoch_loss(trainer, 'test')
             info_dict.update(trainer.test_epoch_metric_values)
             self.curent_epoch['test_epoch'] = info_dict
 
     def on_train_end(self, trainer, pl_module):
```

### Comparing `torchility-0.6.8/torchility/datamodule.py` & `torchility-0.6.9/torchility/datamodule.py`

 * *Files 8% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         self.reset = reset > 0
 
     def train_dataloader(self) -> TRAIN_DATALOADERS:
         if self.reset:
             if hasattr(self.train_dl, 'reset'):
                 return self.train_dl.reset()
             else:
-                print('\nWARNING! Training dataloader should have a `reset` method which returns a NEW dataloader instance!!\n')
+                print('\n\033[91mWARNING! Training dataloader should have a `reset` method which returns a NEW dataloader instance!!\0\n')
         return self.train_dl
 
     def val_dataloader(self) -> EVAL_DATALOADERS:
         return self.val_dl
 
     def test_dataloader(self) -> EVAL_DATALOADERS:
         return self.test_dls
```

### Comparing `torchility-0.6.8/torchility/hooks.py` & `torchility-0.6.9/torchility/hooks.py`

 * *Files identical despite different names*

### Comparing `torchility-0.6.8/torchility/losses.py` & `torchility-0.6.9/torchility/losses.py`

 * *Files identical despite different names*

### Comparing `torchility-0.6.8/torchility/metrics.py` & `torchility-0.6.9/torchility/metrics.py`

 * *Files identical despite different names*

### Comparing `torchility-0.6.8/torchility/tasks.py` & `torchility-0.6.9/torchility/tasks.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,42 +43,46 @@
         metric_values['loss'] = loss
         return metric_values
 
     def validation_step(self, batch, batch_nb, dataloader_idx=0):             # 验证步
         loss, preds, targets, batch_size = self.do_forward(batch)
         self.log('val_loss', loss, prog_bar=True, on_step=True, on_epoch=True, batch_size=batch_size)
 
+        metric_values = {}
+        if self.multi_val_dataloaders:
+            metric_values[f'loss/{dataloader_idx}'] = loss
+        else:
+            metric_values['loss'] = loss
+
         preds, targets = detach_clone(preds), detach_clone(targets)
         if self.metrics:
             dl_idx = dataloader_idx if self.multi_val_dataloaders else -1
-            metric_values = self.do_metric(preds, targets, 'val', batch_size, dl_idx)
+            metric_values.update(self.do_metric(preds, targets, 'val', batch_size, dl_idx))
         self.messages['val_batch'] = (batch_nb, preds, targets)  # (batch_idx, preds, tagets)
 
-        if self.multi_val_dataloaders:
-            metric_values[f'loss/{dataloader_idx}'] = loss
-        else:
-            metric_values['loss'] = loss
         return metric_values
 
     def test_step(self, batch, batch_nb, dataloader_idx=0):                   # 测试步
         loss, preds, targets, batch_size = self.do_forward(batch, self.do_test_loss)
         if loss is not None:
             self.log('test_loss', loss, prog_bar=True, on_step=True, on_epoch=True, batch_size=batch_size)
 
-        preds, targets = detach_clone(preds), detach_clone(targets)
-        if self.metrics:
-            dl_idx = dataloader_idx if self.multi_test_dataloaders else -1
-            metric_values = self.do_metric(preds, targets, 'test', batch_size, dl_idx)
-        self.messages['test_batch'] = (batch_nb, preds, targets)  # (batch_idx, preds, tagets)
-
+        metric_values = {}
         if loss is not None:
             if self.multi_test_dataloaders:
                 metric_values[f'loss/{dataloader_idx}'] = loss
             else:
                 metric_values['loss'] = loss
+
+        preds, targets = detach_clone(preds), detach_clone(targets)
+        if self.metrics:
+            dl_idx = dataloader_idx if self.multi_test_dataloaders else -1
+            metric_values.update(self.do_metric(preds, targets, 'test', batch_size, dl_idx))
+        self.messages['test_batch'] = (batch_nb, preds, targets)  # (batch_idx, preds, tagets)
+
         return metric_values
 
     def predict_step(self, batch: Any, batch_idx: int, dataloader_idx: int = 0) -> Any:
         _, preds, _, _ = self.do_forward(batch, False, self.pred_dataloader_has_label)
         return preds
 
     def configure_optimizers(self):                         # 优化器
@@ -113,18 +117,18 @@
         for metric in metrics:
             if (metric.dl_idx >=0 and metric.dl_idx != dl_idx) or (stage not in metric.stages):
                 continue
             value = metric(preds, targets)
             if isinstance(value, dict):  # 一个函数中计算多个指标，返回一个字典
                 value_dict = {f"{stage}_{metric.name}{k}_step":v for k, v in value.items()}
                 for k, v in value.items():
-                    metric_values[f"{metric.name}{k}"] = v
+                    metric_values[f"{metric.name}{k}"] = v.item()
                 self.log_dict(value_dict, prog_bar=metric.on_bar, on_step=metric.on_step, on_epoch=False, batch_size=batch_size)
             else:
-                metric_values[f"{metric.name}"] = value
+                metric_values[f"{metric.name}"] = value.item()
                 self.log(f"{stage}_{metric.name}_step", value, prog_bar=metric.on_bar, on_step=metric.on_step, on_epoch=False, batch_size=batch_size)
         return metric_values
 
     def _batch_size(self, inputs):
         """检测batch size以用于输出日志"""
         if isinstance(inputs, (tuple, list)):
             data = inputs[0]
```

### Comparing `torchility-0.6.8/torchility/trainer.py` & `torchility-0.6.9/torchility/trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 from copy import deepcopy
 import torch
 import inspect
 from typing import Callable, Union
 from pytorch_lightning import Trainer as PLTrainer
 from pytorch_lightning import LightningModule
-from pytorch_lightning import LightningDataModule
 from pytorch_lightning.loggers import TensorBoardLogger
 from pytorch_lightning.callbacks import ProgressBar
 
 from torchmetrics import Metric
 
 from .callbacks import ResetMetrics, SimpleBar
 from .tasks import GeneralTaskModule
 from .callbacks import Progress
-from .utils import batches, set_attr
+from .utils import batches, set_metric_attr
 from .datamodule import GeneralDataModule
 
 def default_args(func):
     signature = inspect.signature(func)
     return {
         k: v.default
         for k, v in signature.parameters.items()
@@ -27,21 +26,19 @@
 class Trainer(PLTrainer):
     def __init__(self, model:torch.nn.Module=None,  # pytorch Module
         loss:Callable=None,                         # loss function
         optimizer:torch.optim.Optimizer=None,       # pytorch optimizer
         epochs:int=None,                            # max epochs
         metrics:Union[Callable, Metric]=(),         # instance of torchmetrics.Metric or other callable instance
         task_module: LightningModule=None,          # task_model
-        datamodule: LightningDataModule = None,     # PL data module
         default_bar=False,                          # 是否使用默认进度条
         reset_dl:int=0,                             # 每隔多个少epoch重置一次训练DataLoader，与reload_dataloaders_every_n_epochs相似
         task_kwargs:dict=None,                      # parameters dict of the task_module
         **pltrainer_kwargs                          # keyword arguments of pytorch_lightning Trainer
         ):
-
         self.init_params = default_args(PLTrainer)
         self.progress = None
         self.best_model = None   # 训练中最好的torch模型
 
         #   *************************************
         #   *    Task Configuration    --- LIC  *
         #   *************************************
@@ -89,15 +86,15 @@
             self.init_params['reload_dataloaders_every_n_epochs'] = reset_dl
 
         super().__init__(**self.init_params)
 
     def _prepare_metrics(self, metrics, just_for_test=False):
         metrics_ready = {'train': [], 'val':[], 'test':[]}
         for m in metrics:
-            m = set_attr(m)
+            m = set_metric_attr(m)
             if just_for_test:
                 metrics_ready['test'].append(m)
             else:
                 for stage in m.stages:
                     metrics_ready[stage].append(m.clone())
         del metrics
         return metrics_ready if not just_for_test else metrics_ready['test']
@@ -114,25 +111,33 @@
 
     def test(self, test_dls, ckpt_path='best', verbose=True, metrics=None, do_loss=True):  # pylint: disable=arguments-renamed
         """
         Args:
             metrics: 一旦提供了test的metrics，则会将trainer中用于test的metrics覆盖，也就是说可以指定仅用于test的metrics
             do_loss: 在测试时是否计算损失函数，当测试任务和训练任务数据不一致无法计算损失函数时，可设do_loss=False
         """
+        print('-' * 35)
+
         self.task_module.multi_test_dataloaders = False          # 是否使用多个测试dataloader
         if isinstance(test_dls, (list, tuple)) and len(test_dls) > 1:
             self.task_module.multi_test_dataloaders = True
 
         self.task_module.do_test_loss = do_loss
         if metrics is not None:  # 如果提供了仅用于test的metrics
             test_metrics = self._prepare_metrics(metrics, just_for_test=True)
             self.task_module.metrics['test'] = test_metrics
 
         dm = GeneralDataModule(test_dls=test_dls)
-        return super().test(self.task_module, datamodule=dm, ckpt_path=ckpt_path, verbose=verbose)
+        super().test(self.task_module, datamodule=dm, ckpt_path=ckpt_path, verbose=False)
+
+        if verbose:
+            for k, v in self.test_metrics.items():
+                print(f'{k}:\t {v}')
+        print('-' * 35, '\n')
+        return self.test_metrics
 
     def predict(self, pred_dl, has_label=False, ckpt_path='best', concat=True):  # pylint: disable=arguments-renamed
         self.task_module.pred_dataloader_has_label = has_label
         dm = GeneralDataModule(pred_dl=pred_dl)
         preds = super().predict(self.task_module, datamodule=dm, return_predictions=True, ckpt_path=ckpt_path)
         if concat:
             return torch.cat(preds, dim=0)
@@ -205,15 +210,14 @@
         opt = self.task_module.opt
         model =self.task_module.model
         for ckp_path in best_ckp_paths:
             self.task_module.load_from_checkpoint(ckp_path, model=model, loss=loss, optimizer=opt)
             best_models.append(deepcopy(self.task_module.model))
         return best_models
 
-
     def save_state_dict(self, path='best_model.pth', mode='best'):
         """
         Save state_dict of pytorch model.
         Args:
             path: path and filename of the state_dict file.
             mode: 'best' for the best model and others for current model.
         """
```

### Comparing `torchility-0.6.8/torchility/utils/metric_utils.py` & `torchility-0.6.9/torchility/utils/metric_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from ..metrics import MetricBase
 from torchmetrics import Metric
 
 
-def set_attr(metric, name=None, stages=None, dl_idx:int=None, on_step:bool=None, on_epoch:bool=None, on_bar:bool=None):
+def set_metric_attr(metric, name=None, stages=None, dl_idx:int=None, on_step:bool=None, on_epoch:bool=None, on_bar:bool=None):
     """
     Args:
         metric: 指标
         name: 指标名
         stages: 在哪些阶段运行，取值为 'train', 'val', 'test' 或者它们组成的列表，默认值 ['train', 'val', 'test']
         dl_idx: 验证或测试阶段使用多个dataloader时，指标运行在哪个dataloader之上，默认值 -1 表示所有的dataloader
         on_step: 是否将每个batch的指标值记入日志，默认值 True
         on_epoch: 是否将每个epoch的指标值记入日志，默认值 False
         on_bar: 指标是否在pytorch_lightning内置的进度条上显示，默认值 True
     """
-    # 默认属性
+    # 默认属性取值
     attr = {'name': None, 'stages': ['train', 'val', 'test'], 'dl_idx': -1,
             'on_step': True, 'on_epoch': False, 'on_bar': True}
 
     if isinstance(metric, (tuple, list)):
         assert len(metric) == 2, "'`metric` should be a tuple of (metric_name, metric_callable) or (metric_callable, metric_name)"
         if callable(metric[0]):      # (metric_callable, dataloader_idx)
             metric, name_ = metric
```

### Comparing `torchility-0.6.8/torchility/utils/plots.py` & `torchility-0.6.9/torchility/utils/plots.py`

 * *Files identical despite different names*

### Comparing `torchility-0.6.8/torchility/utils/utils.py` & `torchility-0.6.9/torchility/utils/utils.py`

 * *Files identical despite different names*

### Comparing `torchility-0.6.8/torchility/utils/yaml_config.py` & `torchility-0.6.9/torchility/utils/yaml_config.py`

 * *Files identical despite different names*

### Comparing `torchility-0.6.8/torchility.egg-info/PKG-INFO` & `torchility-0.6.9/torchility.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchility
-Version: 0.6.8
+Version: 0.6.9
 Summary: UNKNOWN
 Home-page: https://github.com/hitlic/torchility
 Author: hitlic
 Author-email: liuchen.lic@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `torchility-0.6.8/torchility.egg-info/SOURCES.txt` & `torchility-0.6.9/torchility.egg-info/SOURCES.txt`

 * *Files identical despite different names*

