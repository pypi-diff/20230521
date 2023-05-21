# Comparing `tmp/icatcher-0.0.8.tar.gz` & `tmp/icatcher-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "icatcher-0.0.8.tar", last modified: Thu Mar  9 09:41:56 2023, max compression
+gzip compressed data, was "icatcher-0.0.9.tar", last modified: Tue Mar 21 02:00:23 2023, max compression
```

## Comparing `icatcher-0.0.8.tar` & `icatcher-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-03-09 09:41:56.175681 icatcher-0.0.8/
--rw-rw-rw-   0        0        0    35823 2022-08-25 04:26:17.000000 icatcher-0.0.8/LICENSE
--rw-rw-rw-   0        0        0    51909 2023-03-09 09:41:56.175681 icatcher-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0    10122 2023-03-09 09:36:40.000000 icatcher-0.0.8/README.md
--rw-rw-rw-   0        0        0     1328 2023-03-09 09:40:41.000000 icatcher-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-09 09:41:56.175681 icatcher-0.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-09 09:41:56.144430 icatcher-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2023-03-09 09:41:56.152739 icatcher-0.0.8/src/icatcher/
--rw-rw-rw-   0        0        0       44 2023-03-09 09:40:41.000000 icatcher-0.0.8/src/icatcher/__init__.py
--rw-rw-rw-   0        0        0    25422 2023-03-09 09:26:36.000000 icatcher-0.0.8/src/icatcher/cli.py
--rw-rw-rw-   0        0        0     4644 2023-03-09 09:38:19.000000 icatcher-0.0.8/src/icatcher/draw.py
--rw-rw-rw-   0        0        0     4733 2023-02-02 10:55:03.000000 icatcher-0.0.8/src/icatcher/models.py
--rw-rw-rw-   0        0        0     6487 2023-02-14 13:32:12.000000 icatcher-0.0.8/src/icatcher/options.py
--rw-rw-rw-   0        0        0      911 2023-02-02 10:31:25.000000 icatcher-0.0.8/src/icatcher/parsers.py
--rw-rw-rw-   0        0        0     2016 2023-02-02 12:15:34.000000 icatcher-0.0.8/src/icatcher/video.py
-drwxrwxrwx   0        0        0        0 2023-03-09 09:41:56.171691 icatcher-0.0.8/src/icatcher.egg-info/
--rw-rw-rw-   0        0        0    51909 2023-03-09 09:41:56.000000 icatcher-0.0.8/src/icatcher.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      429 2023-03-09 09:41:56.000000 icatcher-0.0.8/src/icatcher.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-09 09:41:56.000000 icatcher-0.0.8/src/icatcher.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       47 2023-03-09 09:41:56.000000 icatcher-0.0.8/src/icatcher.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      122 2023-03-09 09:41:56.000000 icatcher-0.0.8/src/icatcher.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-03-09 09:41:56.000000 icatcher-0.0.8/src/icatcher.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-09 09:41:56.173686 icatcher-0.0.8/tests/
--rw-rw-rw-   0        0        0      425 2023-03-09 09:35:35.000000 icatcher-0.0.8/tests/test_basic.py
+drwxrwxrwx   0        0        0        0 2023-03-21 02:00:23.598953 icatcher-0.0.9/
+-rw-rw-rw-   0        0        0    35823 2022-08-25 04:26:17.000000 icatcher-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0    51909 2023-03-21 02:00:23.598953 icatcher-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0    10122 2023-03-09 09:36:40.000000 icatcher-0.0.9/README.md
+-rw-rw-rw-   0        0        0     1328 2023-03-21 01:40:11.000000 icatcher-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-03-21 02:00:23.598953 icatcher-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-03-21 02:00:23.529161 icatcher-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2023-03-21 02:00:23.579135 icatcher-0.0.9/src/icatcher/
+-rw-rw-rw-   0        0        0       44 2023-03-21 01:40:11.000000 icatcher-0.0.9/src/icatcher/__init__.py
+-rw-rw-rw-   0        0        0    25796 2023-03-21 01:54:19.000000 icatcher-0.0.9/src/icatcher/cli.py
+-rw-rw-rw-   0        0        0     4685 2023-03-10 04:48:55.000000 icatcher-0.0.9/src/icatcher/draw.py
+-rw-rw-rw-   0        0        0     4733 2023-02-02 10:55:03.000000 icatcher-0.0.9/src/icatcher/models.py
+-rw-rw-rw-   0        0        0     6610 2023-03-21 01:37:17.000000 icatcher-0.0.9/src/icatcher/options.py
+-rw-rw-rw-   0        0        0      911 2023-02-02 10:31:25.000000 icatcher-0.0.9/src/icatcher/parsers.py
+-rw-rw-rw-   0        0        0     2016 2023-02-02 12:15:34.000000 icatcher-0.0.9/src/icatcher/video.py
+drwxrwxrwx   0        0        0        0 2023-03-21 02:00:23.589219 icatcher-0.0.9/src/icatcher.egg-info/
+-rw-rw-rw-   0        0        0    51909 2023-03-21 02:00:23.000000 icatcher-0.0.9/src/icatcher.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      429 2023-03-21 02:00:23.000000 icatcher-0.0.9/src/icatcher.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-03-21 02:00:23.000000 icatcher-0.0.9/src/icatcher.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       47 2023-03-21 02:00:23.000000 icatcher-0.0.9/src/icatcher.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      122 2023-03-21 02:00:23.000000 icatcher-0.0.9/src/icatcher.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-03-21 02:00:23.000000 icatcher-0.0.9/src/icatcher.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-03-21 02:00:23.598953 icatcher-0.0.9/tests/
+-rw-rw-rw-   0        0        0      425 2023-03-14 15:02:09.000000 icatcher-0.0.9/tests/test_basic.py
```

### Comparing `icatcher-0.0.8/LICENSE` & `icatcher-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `icatcher-0.0.8/PKG-INFO` & `icatcher-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icatcher
-Version: 0.0.8
+Version: 0.0.9
 Summary: iCatcher+: Robust and automated annotation of infant gaze from videos collected in laboratory, field, and online studies.
 Author-email: Yotam Erel <erelyotam@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `icatcher-0.0.8/README.md` & `icatcher-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `icatcher-0.0.8/pyproject.toml` & `icatcher-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "icatcher"
-version = "0.0.8"
+version = "0.0.9"
 description = "iCatcher+: Robust and automated annotation of infant gaze from videos collected in laboratory, field, and online studies."
 readme = "README.md"
 authors = [{ name = "Yotam Erel", email = "erelyotam@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
@@ -32,15 +32,15 @@
 build = ["build", "twine"]
 dev = ["bumpver", "pytest"]
 
 [project.urls]
 Homepage = "https://github.com/yoterel/icatcher_plus"
 
 [tool.bumpver]
-current_version = "0.0.8"
+current_version = "0.0.9"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = false
 tag = false
 push = false
 
 [tool.bumpver.file_patterns]
```

### Comparing `icatcher-0.0.8/src/icatcher/cli.py` & `icatcher-0.0.9/src/icatcher/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,15 +52,15 @@
         self.color = False
         self.erasing = False
         self.noise = False
         self.model = "vgg16"
         self.dropout = 0.0
 
 
-def select_face(bboxes, frame, fc_model, fc_data_transforms, hor, ver):
+def select_face(bboxes, frame, fc_model, fc_data_transforms, hor, ver, device):
     """
     selects a correct face from candidates bbox in frame
     :param bboxes: the bounding boxes of candidates
     :param frame: the frame
     :param fc_model: a classifier model, if passed it is used to decide.
     :param fc_data_transforms: the transformations to apply to the images before fc_model sees them
     :param hor: the last known horizontal correct face location
@@ -80,15 +80,15 @@
             face_hor = (ratio[2] + ratio[3]) / 2
 
             centers.append([face_hor, face_ver])
             img = crop_img
             img = fc_data_transforms['val'](img)
             faces.append(img)
         centers = np.stack(centers)
-        faces = torch.stack(faces).to(fc_model.device)
+        faces = torch.stack(faces).to(device)
         output = fc_model(faces)
         _, preds = torch.max(output, 1)
         preds = preds.cpu().numpy()
         idxs = np.where(preds == 0)[0]
         if idxs.size == 0:
             bbox = None
         else:
@@ -209,16 +209,21 @@
     :return all nn models
     """
     GOODBOY = pooch.create(path=pooch.os_cache("icatcher_plus"),
                            base_url="https://osf.io/ycju8/download",
                            version=version,
                            version_dev="main",
                            env="ICATCHER_DATA_DIR",
-                           registry={"icatcher+_models.zip": "d78385b3a08f3d55ce75249142d15549e4c5552d5e1231cad3b69063bb778ce9"},
-                           urls={"icatcher+_models.zip":"https://osf.io/ycju8/download"})
+                           registry={"zip_content.txt": "d81bfb5a183edea6dc74f7f342d516a9843865570b9ecfbf481209ec5114110a",
+                                     "icatcher+_models.zip": "d78385b3a08f3d55ce75249142d15549e4c5552d5e1231cad3b69063bb778ce9"},
+                           urls={"zip_content.txt":"https://osf.io/v4w53/download",
+                                 "icatcher+_models.zip":"https://osf.io/ycju8/download"})
+    # zip_content_file = GOODBOY.fetch("zip_content.txt")
+    # with open(zip_content_file, "r") as f:
+        # zip_content = [x.strip() for x in f]
     file_paths = GOODBOY.fetch("icatcher+_models.zip",
                                processor=pooch.Unzip(),
                                progressbar=True)
     file_names = [Path(x).name for x in file_paths]
     face_detector_model_file = file_paths[file_names.index("face_model.caffemodel")]
     config_file = file_paths[file_names.index("config.prototxt")]
     path_to_gaze_model = file_paths[file_names.index("icatcher+_lookit.pth")]
@@ -389,15 +394,15 @@
                 from_tracker.append(False)
             else:
                 if cv2_bboxes:
                     from_tracker.append(False)
                 else:
                     from_tracker.append(True)
                     cv2_bboxes = [last_known_valid_bbox]
-                selected_bbox = select_face(cv2_bboxes, frame, face_classifier_model, face_classifier_data_transforms, hor, ver)
+                selected_bbox = select_face(cv2_bboxes, frame, face_classifier_model, face_classifier_data_transforms, hor, ver, opt.device)
                 crop, my_box = extract_crop(frame, selected_bbox, opt)
                 if selected_bbox is None:
                     answers.append(classes['nobabyface'])  # if selecting face fails, treat as away and mark invalid
                     confidences.append(-1)
                     image = np.zeros((1, opt.image_size, opt.image_size, 3), np.float64)
                     my_box = np.array([0, 0, 0, 0, 0])
                     image_sequence.append((image, True))
```

### Comparing `icatcher-0.0.8/src/icatcher/draw.py` & `icatcher-0.0.9/src/icatcher/draw.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,14 +104,15 @@
     if frame_number is not None:  # may fail if loc outside resolution
         frame = put_text(frame, str(frame_number), loc=(10,70))
     return frame
 
 def mask_regions(image, start_h, end_h, start_w, end_w):
     """
     masks a numpy image with black background outside of region of interest (roi)
+    :param image: numpy image h x w x c
     :param start_h: where does the roi height start
     :param end_h: where does the roi height end
     :param start_w: where does the roi width start
     :param end_w: where does the roi width end
     :return: masked image
     """
     h, w, _ = image.shape
```

### Comparing `icatcher-0.0.8/src/icatcher/models.py` & `icatcher-0.0.9/src/icatcher/models.py`

 * *Files identical despite different names*

### Comparing `icatcher-0.0.8/src/icatcher/options.py` & `icatcher-0.0.9/src/icatcher/options.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import argparse
 from pathlib import Path
+from . import version
 
 def parse_arguments():
-    parser = argparse.ArgumentParser()
+    parser = argparse.ArgumentParser(prog='icatcher')
     parser.add_argument("source", type=str, help="the source to use (path to video file, folder or webcam id)")
     parser.add_argument("--model", type=str, help="path to model that will be used for predictions "
                                                   "if not supplied will use model trained on the lookit dataset")
     parser.add_argument("--use_fc_model", action="store_true", help="if supplied, will use face classifier "
                                                                               "to decide which crop to use from every frame.")
     parser.add_argument("--fc_model", type=str, help="path to face classifier model that will be used for deciding "
                                                      "which crop should we select from every frame. "
@@ -43,14 +44,15 @@
     parser.add_argument("--video_filter", type=str,
                         help="provided file will be used to filter only test videos,"
                              " will assume certain file structure using the lookit/cali-bw/senegal datasets")
     parser.add_argument("--raw_dataset_path", type=str, help="path to raw dataset (required if --video_filter is passed")
     parser.add_argument("--raw_dataset_type", type=str, choices=["lookit", "cali-bw", "senegal", "generic"], default="lookit",
                         help="the type of dataset to preprocess")
     parser.add_argument("--illegal_transitions_path", type=str, help="path to CSV with illegal transitions to 'smooth' over")
+    parser.add_argument('--version', action='version', version="%(prog)s "+version)
     args = parser.parse_args()
     if args.model:
         args.model = Path(args.model)
     # if not args.model.is_file():
     #     raise FileNotFoundError("Model file not found")
     if args.crop_percent not in [x for x in range(100)]:
         raise ValueError("crop_video must be a percent between 0 - 99")
```

### Comparing `icatcher-0.0.8/src/icatcher/parsers.py` & `icatcher-0.0.9/src/icatcher/parsers.py`

 * *Files identical despite different names*

### Comparing `icatcher-0.0.8/src/icatcher/video.py` & `icatcher-0.0.9/src/icatcher/video.py`

 * *Files identical despite different names*

### Comparing `icatcher-0.0.8/src/icatcher.egg-info/PKG-INFO` & `icatcher-0.0.9/src/icatcher.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icatcher
-Version: 0.0.8
+Version: 0.0.9
 Summary: iCatcher+: Robust and automated annotation of infant gaze from videos collected in laboratory, field, and online studies.
 Author-email: Yotam Erel <erelyotam@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

