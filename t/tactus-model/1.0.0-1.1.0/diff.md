# Comparing `tmp/TACTUS-model-1.0.0.tar.gz` & `tmp/tactus-model-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TACTUS-model-1.0.0.tar", last modified: Mon May 15 16:28:53 2023, max compression
+gzip compressed data, was "tactus-model-1.1.0.tar", last modified: Sun May 21 14:19:53 2023, max compression
```

## Comparing `TACTUS-model-1.0.0.tar` & `tactus-model-1.1.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-05-15 16:28:53.195921 TACTUS-model-1.0.0/
--rw-rw-rw-   0        0        0      709 2023-05-15 16:28:53.193928 TACTUS-model-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      293 2023-05-15 16:26:32.000000 TACTUS-model-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-15 16:28:53.171915 TACTUS-model-1.0.0/TACTUS_model.egg-info/
--rw-rw-rw-   0        0        0      709 2023-05-15 16:28:53.000000 TACTUS-model-1.0.0/TACTUS_model.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      388 2023-05-15 16:28:53.000000 TACTUS-model-1.0.0/TACTUS_model.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-15 16:28:53.000000 TACTUS-model-1.0.0/TACTUS_model.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-05-15 16:28:53.000000 TACTUS-model-1.0.0/TACTUS_model.egg-info/requires.txt
--rw-rw-rw-   0        0        0       28 2023-05-15 16:28:53.000000 TACTUS-model-1.0.0/TACTUS_model.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      645 2023-05-15 16:28:11.000000 TACTUS-model-1.0.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-15 16:28:53.195921 TACTUS-model-1.0.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-15 16:28:53.177919 TACTUS-model-1.0.0/tactus_model/
--rw-rw-rw-   0        0        0      148 2023-05-15 16:28:23.000000 TACTUS-model-1.0.0/tactus_model/__init__.py
--rw-rw-rw-   0        0        0    11802 2023-05-14 14:50:48.000000 TACTUS-model-1.0.0/tactus_model/hyperparam_tuning.py
-drwxrwxrwx   0        0        0        0 2023-05-15 16:28:53.189907 TACTUS-model-1.0.0/tactus_model/utils/
--rw-rw-rw-   0        0        0        0 2023-04-05 10:06:03.000000 TACTUS-model-1.0.0/tactus_model/utils/__init__.py
--rw-rw-rw-   0        0        0     6375 2023-05-14 14:00:10.000000 TACTUS-model-1.0.0/tactus_model/utils/classifier.py
--rw-rw-rw-   0        0        0     4537 2023-04-17 12:58:40.000000 TACTUS-model-1.0.0/tactus_model/utils/torch_mlp.py
--rw-rw-rw-   0        0        0     4284 2023-05-08 21:38:52.000000 TACTUS-model-1.0.0/tactus_model/utils/tracker.py
+drwxrwxrwx   0        0        0        0 2023-05-21 14:19:53.946813 tactus-model-1.1.0/
+-rw-rw-rw-   0        0        0      709 2023-05-21 14:19:53.945814 tactus-model-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2023-05-19 14:34:39.000000 tactus-model-1.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-21 14:19:53.916813 tactus-model-1.1.0/TACTUS_model.egg-info/
+-rw-rw-rw-   0        0        0      709 2023-05-21 14:19:53.000000 tactus-model-1.1.0/TACTUS_model.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      594 2023-05-21 14:19:53.000000 tactus-model-1.1.0/TACTUS_model.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-21 14:19:53.000000 tactus-model-1.1.0/TACTUS_model.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-05-21 14:19:53.000000 tactus-model-1.1.0/TACTUS_model.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       28 2023-05-21 14:19:53.000000 tactus-model-1.1.0/TACTUS_model.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      645 2023-05-19 17:28:40.000000 tactus-model-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-21 14:19:53.946813 tactus-model-1.1.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-21 14:19:53.929812 tactus-model-1.1.0/tactus_model/
+-rw-rw-rw-   0        0        0      148 2023-05-19 14:34:39.000000 tactus-model-1.1.0/tactus_model/__init__.py
+-rw-rw-rw-   0        0        0    12847 2023-05-21 14:11:57.000000 tactus-model-1.1.0/tactus_model/hyperparam_tuning.py
+-rw-rw-rw-   0        0        0     4517 2023-05-21 14:07:50.000000 tactus-model-1.1.0/tactus_model/model_eval.py
+drwxrwxrwx   0        0        0        0 2023-05-21 14:19:53.943818 tactus-model-1.1.0/tactus_model/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-05 10:06:03.000000 tactus-model-1.1.0/tactus_model/utils/__init__.py
+-rw-rw-rw-   0        0        0     6375 2023-05-19 14:34:39.000000 tactus-model-1.1.0/tactus_model/utils/classifier.py
+-rw-rw-rw-   0        0        0     4573 2023-05-19 14:47:33.000000 tactus-model-1.1.0/tactus_model/utils/torch_mlp.py
+-rw-rw-rw-   0        0        0     4862 2023-05-21 14:07:40.000000 tactus-model-1.1.0/tactus_model/utils/tracker.py
```

### Comparing `TACTUS-model-1.0.0/PKG-INFO` & `tactus-model-1.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: TACTUS-model
-Version: 1.0.0
+Name: tactus-model
+Version: 1.1.0
 Summary: Threatening activities classification toward users' security
 Project-URL: repository, https://github.com/Cranfield-GDP3/TACTUS-model
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `TACTUS-model-1.0.0/TACTUS_model.egg-info/PKG-INFO` & `tactus-model-1.1.0/TACTUS_model.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: TACTUS-model
-Version: 1.0.0
+Name: tactus-model
+Version: 1.1.0
 Summary: Threatening activities classification toward users' security
 Project-URL: repository, https://github.com/Cranfield-GDP3/TACTUS-model
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `TACTUS-model-1.0.0/pyproject.toml` & `tactus-model-1.1.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
-name = "TACTUS-model"
+name = "tactus-model"
 # PEP 440 - Version Identification and Dependency Specification https://peps.python.org/pep-0440/
-version = "1.0.0"
+version = "1.1.0"
 description = "Threatening activities classification toward users' security"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Programming Language :: Python",
```

### Comparing `TACTUS-model-1.0.0/tactus_model/hyperparam_tuning.py` & `tactus-model-1.1.0/tactus_model/hyperparam_tuning.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,34 +1,38 @@
 from typing import List, Dict, Tuple, Generator
 import json
 from pathlib import Path
 import numpy as np
+from imblearn.over_sampling import SMOTE
+from imblearn.under_sampling import RandomUnderSampler
 from tactus_data import data_augment, SMALL_ANGLES_LIST, MEDIUM_ANGLES_LIST
 from tactus_data.datasets.ut_interaction import data_split
 from tactus_data import Skeleton
 
 from tactus_model.utils.tracker import FeatureTracker
 from tactus_model.utils.classifier import Classifier, label_to_int
 
 DATA_AUGMENT_GRIDS = {
     "FLIP": {"horizontal_flip": [True, False]},
 }
 
-TRACKER_GRID = {  # grid size: 1
-    "window_size": [9],  # impact velocity
+TRACKER_GRID = {
+    "window_size": [9],
     "number_of_angles": [0],
 }
 
-CLASSIFIER_HYPERPARAMS = {  # grid size : 18
+CLASSIFIER_HYPERPARAMS = {
     "TorchMLP": {
         "batch_size": [256],
-        "num_epochs": [300],
+        "num_epochs": [30],
         "hidden_layer_sizes": [{"layer_sizes": [256, 128, 16], "dropout": [0.4, 0.2, 0.1]},
-                               {"layer_sizes": [1024, 512, 128, 16], "dropout": [0.5, 0.3, 0.2, 0.1]}],
-        "activation": ['Tanh', 'ReLU']
+                               {"layer_sizes": [1024, 512, 128, 16], "dropout": [0.5, 0.3, 0.2, 0.1]},
+                               {"layer_sizes": [512, 128, 64], "dropout": [0.2, 0.2, 0.1]},
+                               ],
+        "activation": ['ReLU']
     },
 }
 
 
 def get_classifier(
         classifier_grids: Dict[str, Dict] = None,
 ) -> Generator[Tuple[Classifier, str, dict], None, None]:
@@ -85,19 +89,40 @@
     if tracker_grid is None:
         tracker_grid = TRACKER_GRID
 
     for grid in data_augment.ParameterGrid(tracker_grid):
         yield grid
 
 
+def sample_data(X: List, Y: List, sampler: str):
+    """
+    Over/Under sample the data if the flag is set to the corresponding value, does nothing if flag = X
+    Args:
+        X: Data for the classifier
+        Y: Label for the classifier
+        sampler: Flag chosing the sample technique
+
+    Returns:
+        The sampled data
+    """
+    if sampler == "RUS":
+        sampler = RandomUnderSampler()
+    elif sampler == "SMOTE":
+        sampler = SMOTE()
+    else:
+        return X, Y
+    return sampler.fit_resample(X, Y)
+
+
 def train_grid_search(
         fps: int = 10,
         augment_grids: Dict[str, Dict] = None,
         tracker_grid: Dict[str, List] = None,
         classifier_grids: Dict[str, Dict] = None,
+        sampler: str = "RUS"
 ):
     """
     launch the training process
 
     Parameters
     ----------
     fps : int, optional
@@ -108,26 +133,31 @@
 
     model_id = 0
     for augment_grid in get_augment_grid(augment_grids):
         # augments data and saves it in files
         print("augments data with: ", augment_grid)
         delete_data_augment(train_videos + test_videos, fps)
 
-        for video_path in train_videos + test_videos:
+        for video_path in train_videos:
             original_data_path = video_path / f"{fps}fps" / "yolov7.json"
             data_augment.grid_augment(original_data_path, augment_grid)
 
+        for video_path in test_videos:
+            original_data_path = video_path / f"{fps}fps" / "yolov7.json"
+            data_augment.grid_augment(original_data_path, {})
+
         # compute features
         for tracker_params in get_tracker_params(tracker_grid):
             print("compute features with: ", tracker_params)
             angle_list = get_angle_list(tracker_params["number_of_angles"])
             window_size = tracker_params["window_size"]
 
             X, Y = generate_features(train_videos, fps, window_size, angle_list)
             X_test, Y_test = generate_features(test_videos, fps, window_size, angle_list)
+            X,Y = sample_data(X, Y, sampler)
 
             for classifier in get_classifier(classifier_grids):
                 print("fit classifier: ", classifier.name, " with ", classifier.hyperparams)
                 classifier.fit(X, Y)
                 classifier.window_size = window_size
                 classifier.fps = fps
                 classifier.angles_to_compute = angle_list
@@ -148,18 +178,18 @@
 
     eval_dict["augment_grid"] = augment_grid
     eval_dict["tracker_params"] = tracker_params
 
     eval_dict["classifier_name"] = classifier.name
     eval_dict["hyperparams"] = classifier.hyperparams
 
-    eval_dict["y_pred_train"] = classifier.predict(X).tolist()
+    eval_dict["y_pred_train"] = classifier.predict(X)
     eval_dict["y_true_train"] = Y
 
-    eval_dict["y_pred_test"] = classifier.predict(X_test).tolist()
+    eval_dict["y_pred_test"] = classifier.predict(X_test)
     eval_dict["y_true_test"] = Y_test
 
     filename = Path(f"data/models/evaluation/{model_id}.json")
     filename.parent.mkdir(parents=True, exist_ok=True)
     json.dump(eval_dict, filename.open(mode="w", encoding="utf8"))
 
 
@@ -241,26 +271,29 @@
 
     while i_frame < len(formatted_json["frames"]):
         frame = formatted_json["frames"][i_frame]
 
         for skeleton in frame["skeletons"]:
             # do not deal with untracked skeletons
             if "id_stupid" in skeleton:
+                skeleton_id = skeleton["id_stupid"]
+
                 keypoints = np.array(skeleton["keypoints"]).reshape((-1, 2))
-                feature_tracker.update_rolling_window(skeleton["id_stupid"], Skeleton(keypoints=keypoints))
+                feature_tracker.update_rolling_window(skeleton_id, Skeleton(keypoints=keypoints))
+
+                if feature_tracker[skeleton_id].is_complete():
+                    features = feature_tracker[skeleton_id].get_features()
 
-        for skeleton_id, (success, features) in feature_tracker.extract():
-            if success:
-                if skeleton_id == offender_id:
-                    label = compute_label(frame["frame_id"], labels["classes"], i_label)
-                else:
-                    label = "neutral"
+                    if skeleton_id == offender_id:
+                        label = compute_label(frame["frame_id"], labels["classes"], i_label)
+                    else:
+                        label = "neutral"
 
-                video_features.append(features)
-                video_labels.append(label_to_int(label))
+                    video_features.append(features)
+                    video_labels.append(label_to_int(label))
 
         # jump to the next action
         if i_label >= labels["classes"][i_label]["end_frame"]:
             if len(labels["classes"]) > i_label:
                 i_label += 1
                 i_frame = labels["classes"][i_label]["start_frame"] - window_size
                 feature_tracker.reset_rolling_windows()
```

### Comparing `TACTUS-model-1.0.0/tactus_model/utils/classifier.py` & `tactus-model-1.1.0/tactus_model/utils/classifier.py`

 * *Files identical despite different names*

### Comparing `TACTUS-model-1.0.0/tactus_model/utils/torch_mlp.py` & `tactus-model-1.1.0/tactus_model/utils/torch_mlp.py`

 * *Files 1% similar despite different names*

```diff
@@ -72,14 +72,16 @@
             for _, (x_batch, y_batch) in enumerate(dataloader):
                 y_pred = self.model(x_batch)
                 loss = self.loss_fn(y_pred, y_batch)
                 self.optimizer.zero_grad()
                 loss.backward()
                 self. optimizer.step()
 
+        torch.cuda.empty_cache()
+
     def predict(self, X):
         """
         predict using the fitted model
         """
         self.model.eval()
         if isinstance(X, List):
             X = torch.tensor(X, dtype=torch.float32, device=self.device)
```

### Comparing `TACTUS-model-1.0.0/tactus_model/utils/tracker.py` & `tactus-model-1.1.0/tactus_model/utils/tracker.py`

 * *Files 7% similar despite different names*

```diff
@@ -8,18 +8,18 @@
     1: SkeletonRollingWindow(...),
     2: SkeletonRollingWindow(...),
     6: SkeletonRollingWindow(...),
     12: SkeletonRollingWindow(...),
 }
 """
 from typing import Union, Generator, Tuple, List, Dict
+from collections import deque, Counter
 from collections.abc import Sequence
-import time
 import numpy as np
-from tactus_data import SkeletonRollingWindow
+from tactus_data import SkeletonRollingWindow, Skeleton
 
 
 class FeatureTracker:
     """
     High level interface with rolling windows of skeletons and their
     tracking with deepsort.
     """
@@ -41,20 +41,20 @@
     def update_rolling_window(self, track_id: int, skeleton: dict):
         """update a SkeletonRollingWindow from its ID"""
         if track_id not in self.rolling_windows:
             self.rolling_windows[track_id] = SkeletonRollingWindow(self.window_size, self.angles_to_compute)
 
         self.rolling_windows[track_id].add_skeleton(skeleton)
 
-    def duplicate_last_entry(self, track_id: int, new_bbox_lbrt: Tuple[float, float, float, float]):
+    def duplicate_last_entry(self, track_id: int, new_bbox_lbrt: Tuple[float, float, float, float]) -> Skeleton:
         """
         duplicate the last entry of a rolling window. That is useful
         to avoid gaps in the prediction.
         """
-        self.rolling_windows[track_id].duplicate_last_entry(new_bbox_lbrt)
+        return self.rolling_windows[track_id].duplicate_last_entry(new_bbox_lbrt)
 
     def delete_track_id(self, track_id: int):
         """
         delete a SkeletonRollingWindow from its ID.
 
         DeepSort can have unconfirmed track that are not taken into
         account in FeatureTracker. To avoid an error, we delete
@@ -80,42 +80,57 @@
 
 
 class PredTracker:
     """
     save the non-neutral predictions for each skeleton still present
     on the stream.
     """
-    def __init__(self):
+    def __init__(self, prediction_smoothing: int = 5):
         self.tracker: Dict[int, Dict] = {}
+        self.pred_rw_size = prediction_smoothing
 
     def init_track(self, track_id: int):
         """initialize the dictionary key"""
         self.tracker[track_id] = {"current_label": None,
-                                  "label_history": []}
+                                  "violent": False,
+                                  "pred_history": deque(maxlen=self.pred_rw_size)}
 
-    def add_pred(self, track_id: int, label: str, bbx: Tuple[int, int, int, int]):
+    def add_pred(self, track_id: int, label: str):
         """starts the tracking of a person from a prediction label"""
         if track_id not in self.tracker:
             self.init_track(track_id)
 
-        self.tracker[track_id]["current_label"] = label
-        self.tracker[track_id]["timestamp"] = time.time()
-        self.tracker[track_id]["box"] = bbx
-
-        if len(self.tracker[track_id]["label_history"]) > 0:
-            if label != self.tracker[track_id]["label_history"][-1]:
-                self.tracker[track_id]["label_history"].append(label)
+        self.tracker[track_id]["pred_history"].append(label)
+        smoothed_label = self.get_smoothed_pred(track_id)
+        self.tracker[track_id]["current_label"] = smoothed_label
+
+        if smoothed_label != "neutral":
+            self.tracker[track_id]["violent"] = True
 
     def delete_track_id(self, track_ids: Union[List[int], int]):
         """removes the track of a person"""
         if not isinstance(track_ids, Sequence):
             track_ids = [track_ids]
 
         for track_id in track_ids:
             if track_id in self.tracker:
                 del self.tracker[track_id]
 
+    def get_smoothed_pred(self, track_id: int) -> str:
+        """get the smoothed prediction"""
+        return most_common(self.tracker[track_id]["pred_history"])
+
+    def get_last_pred(self, track_id: int) -> str:
+        """return the last prediction made"""
+        return self.tracker[track_id]["current_label"]
+
     def __contains__(self, __track_id: int):
         return __track_id in self.tracker
 
     def __getitem__(self, __track_id: int):
         return self.tracker[__track_id]
+
+
+def most_common(lst):
+    """return the most common element of a list"""
+    counter = Counter(lst)
+    return counter.most_common(1)[0][0]
```

