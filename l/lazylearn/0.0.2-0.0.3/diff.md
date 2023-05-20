# Comparing `tmp/lazylearn-0.0.2.tar.gz` & `tmp/lazylearn-0.0.3.tar.gz`

## Comparing `lazylearn-0.0.2.tar` & `lazylearn-0.0.3.tar`

### file list

```diff
@@ -1,35 +1,52 @@
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 lazylearn-0.0.2/Pipfile
--rw-r--r--   0        0        0    74533 2020-02-02 00:00:00.000000 lazylearn-0.0.2/Pipfile.lock
--rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 lazylearn-0.0.2/.github/workflows/verify.yaml
--rw-r--r--   0        0        0    59514 2020-02-02 00:00:00.000000 lazylearn-0.0.2/doc/logo/grayscale_transparent.png
--rw-r--r--   0        0        0    62685 2020-02-02 00:00:00.000000 lazylearn-0.0.2/doc/logo/original.png
--rw-r--r--   0        0        0    66560 2020-02-02 00:00:00.000000 lazylearn-0.0.2/doc/logo/transparent.png
--rw-r--r--   0        0        0    71882 2020-02-02 00:00:00.000000 lazylearn-0.0.2/doc/logo/transparent_small.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lazylearn-0.0.2/python/src/lazylearn/__init__.py
--rw-r--r--   0        0        0      359 2020-02-02 00:00:00.000000 lazylearn-0.0.2/python/src/lazylearn/lazylearn.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lazylearn-0.0.2/python/src/lazylearn/errors/__init__.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 lazylearn-0.0.2/python/src/lazylearn/errors/errors.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lazylearn-0.0.2/python/src/lazylearn/ingestion/__init__.py
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 lazylearn-0.0.2/python/src/lazylearn/ingestion/ingestion_pipeline.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lazylearn-0.0.2/python/src/lazylearn/ingestion/ingestion_pipeline_steps/__init__.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 lazylearn-0.0.2/python/src/lazylearn/ingestion/ingestion_pipeline_steps/data_parser_step.py
--rw-r--r--   0        0        0     2437 2020-02-02 00:00:00.000000 lazylearn-0.0.2/python/src/lazylearn/ingestion/ingestion_pipeline_steps/interpreter_step.py
--rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 lazylearn-0.0.2/python/src/lazylearn/ingestion/ingestion_pipeline_steps/summary_stats_step.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lazylearn-0.0.2/python/src/lazylearn/models/__init__.py
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 lazylearn-0.0.2/python/src/lazylearn/models/models.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lazylearn-0.0.2/python/src/lazylearn/pipeline/__init__.py
--rw-r--r--   0        0        0      793 2020-02-02 00:00:00.000000 lazylearn-0.0.2/python/src/lazylearn/pipeline/pipeline.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lazylearn-0.0.2/python/src/lazylearn/preprocessing/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lazylearn-0.0.2/python/src/lazylearn/preprocessing/encoding/__init__.py
--rw-r--r--   0        0        0      396 2020-02-02 00:00:00.000000 lazylearn-0.0.2/python/src/lazylearn/preprocessing/encoding/encoders.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 lazylearn-0.0.2/python/src/test/test_mock.py
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 lazylearn-0.0.2/python/src/test/ingestion/ingestion_pipeline_steps/test_data_parser_step.py
--rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 lazylearn-0.0.2/python/src/test/ingestion/ingestion_pipeline_steps/test_interpreter_step.py
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 lazylearn-0.0.2/python/src/test/ingestion/ingestion_pipeline_steps/test_summary_stats_step.py
--rwxr-xr-x   0        0        0      743 2020-02-02 00:00:00.000000 lazylearn-0.0.2/shell/check.sh
--rwxr-xr-x   0        0        0      382 2020-02-02 00:00:00.000000 lazylearn-0.0.2/shell/tidy.sh
--rw-r--r--   0        0        0     3137 2020-02-02 00:00:00.000000 lazylearn-0.0.2/.gitignore
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 lazylearn-0.0.2/LICENSE
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 lazylearn-0.0.2/README.md
--rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 lazylearn-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 lazylearn-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 lazylearn-0.0.3/Pipfile
+-rw-r--r--   0        0        0    75211 2020-02-02 00:00:00.000000 lazylearn-0.0.3/Pipfile.lock
+-rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 lazylearn-0.0.3/.github/workflows/verify.yaml
+-rw-r--r--   0        0        0    59514 2020-02-02 00:00:00.000000 lazylearn-0.0.3/doc/logo/grayscale_transparent.png
+-rw-r--r--   0        0        0    62685 2020-02-02 00:00:00.000000 lazylearn-0.0.3/doc/logo/original.png
+-rw-r--r--   0        0        0    66560 2020-02-02 00:00:00.000000 lazylearn-0.0.3/doc/logo/transparent.png
+-rw-r--r--   0        0        0    71882 2020-02-02 00:00:00.000000 lazylearn-0.0.3/doc/logo/transparent_small.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lazylearn-0.0.3/python/src/lazylearn/__init__.py
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 lazylearn-0.0.3/python/src/lazylearn/lazylearn.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lazylearn-0.0.3/python/src/lazylearn/errors/__init__.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 lazylearn-0.0.3/python/src/lazylearn/errors/errors.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lazylearn-0.0.3/python/src/lazylearn/ingestion/__init__.py
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 lazylearn-0.0.3/python/src/lazylearn/ingestion/ingestion_pipeline.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lazylearn-0.0.3/python/src/lazylearn/ingestion/ingestion_pipeline_steps/__init__.py
+-rw-r--r--   0        0        0      868 2020-02-02 00:00:00.000000 lazylearn-0.0.3/python/src/lazylearn/ingestion/ingestion_pipeline_steps/data_parser_step.py
+-rw-r--r--   0        0        0     4195 2020-02-02 00:00:00.000000 lazylearn-0.0.3/python/src/lazylearn/ingestion/ingestion_pipeline_steps/interpreter_step.py
+-rw-r--r--   0        0        0      673 2020-02-02 00:00:00.000000 lazylearn-0.0.3/python/src/lazylearn/ingestion/ingestion_pipeline_steps/summary_stats_step.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lazylearn-0.0.3/python/src/lazylearn/ingestion/utils/__init__.py
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 lazylearn-0.0.3/python/src/lazylearn/ingestion/utils/csv.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lazylearn-0.0.3/python/src/lazylearn/model_selection/__init__.py
+-rw-r--r--   0        0        0      471 2020-02-02 00:00:00.000000 lazylearn-0.0.3/python/src/lazylearn/model_selection/splitters.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lazylearn-0.0.3/python/src/lazylearn/models/__init__.py
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 lazylearn-0.0.3/python/src/lazylearn/models/models.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lazylearn-0.0.3/python/src/lazylearn/pipeline/__init__.py
+-rw-r--r--   0        0        0     1925 2020-02-02 00:00:00.000000 lazylearn-0.0.3/python/src/lazylearn/pipeline/pipeline.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lazylearn-0.0.3/python/src/lazylearn/preprocessing/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lazylearn-0.0.3/python/src/lazylearn/preprocessing/encoding/__init__.py
+-rw-r--r--   0        0        0     2512 2020-02-02 00:00:00.000000 lazylearn-0.0.3/python/src/lazylearn/preprocessing/encoding/encoders.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lazylearn-0.0.3/python/src/lazylearn/preprocessing/imputation/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lazylearn-0.0.3/python/src/lazylearn/preprocessing/time/__init__.py
+-rw-r--r--   0        0        0     1217 2020-02-02 00:00:00.000000 lazylearn-0.0.3/python/src/lazylearn/preprocessing/time/date_processor.py
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 lazylearn-0.0.3/python/src/lazylearn/preprocessing/time/duration.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lazylearn-0.0.3/python/src/lazylearn/regression/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lazylearn-0.0.3/python/src/lazylearn/regression/models/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lazylearn-0.0.3/python/src/lazylearn/regression/models/randomforest/__init__.py
+-rw-r--r--   0        0        0     1425 2020-02-02 00:00:00.000000 lazylearn-0.0.3/python/src/lazylearn/regression/models/randomforest/randomforest.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lazylearn-0.0.3/python/src/lazylearn/regression/models/randomforest/random_forest_steps/__init__.py
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 lazylearn-0.0.3/python/src/lazylearn/regression/models/randomforest/random_forest_steps/regressor_step.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lazylearn-0.0.3/python/src/lazylearn/regression/models/xgboost/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lazylearn-0.0.3/python/src/lazylearn/strategies/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lazylearn-0.0.3/python/src/lazylearn/strategies/strategy_builder.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 lazylearn-0.0.3/python/src/test/test_mock.py
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 lazylearn-0.0.3/python/src/test/ingestion/ingestion_pipeline_steps/test_data_parser_step.py
+-rw-r--r--   0        0        0      588 2020-02-02 00:00:00.000000 lazylearn-0.0.3/python/src/test/ingestion/ingestion_pipeline_steps/test_interpreter_step.py
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 lazylearn-0.0.3/python/src/test/ingestion/ingestion_pipeline_steps/test_summary_stats_step.py
+-rwxr-xr-x   0        0        0      743 2020-02-02 00:00:00.000000 lazylearn-0.0.3/shell/check.sh
+-rwxr-xr-x   0        0        0      382 2020-02-02 00:00:00.000000 lazylearn-0.0.3/shell/tidy.sh
+-rw-r--r--   0        0        0     3137 2020-02-02 00:00:00.000000 lazylearn-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 lazylearn-0.0.3/LICENSE
+-rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 lazylearn-0.0.3/README.md
+-rw-r--r--   0        0        0      885 2020-02-02 00:00:00.000000 lazylearn-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 lazylearn-0.0.3/PKG-INFO
```

### Comparing `lazylearn-0.0.2/Pipfile.lock` & `lazylearn-0.0.3/Pipfile.lock`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9848921394799054%*

 * *Differences: {"'_meta'": "{'hash': {'sha256': "*

 * *            "'79fdea66262af3a139c4e3e40343f2bccbbe3bba979276d5158119df01dc3583'}}",*

 * * "'default'": "{'ipykernel': {'hashes': "*

 * *              "['sha256:1aba0ae8453e15e9bc6b24e497ef6840114afcdb832ae597f32137fa19d42a6f', "*

 * *              "'sha256:77aeffab056c21d16f1edccdc9e5ccbf7d96eb401bd6703610a21be8b068aadc'], "*

 * *              "'version': '==6.23.1'}, 'nbconvert': {'hashes': "*

 * *              "['sha256:51b6c77b507b177b73f6729dba15676e42c4e92bcb00edc8cc982ee72e7d89d7', "*

 * *        […]*

```diff
@@ -1,11 +1,11 @@
 {
     "_meta": {
         "hash": {
-            "sha256": "a5dc7a8a6ec4078ce0d03261251f9452d7c5d70fca4102d184df59b32b1a8a1c"
+            "sha256": "79fdea66262af3a139c4e3e40343f2bccbbe3bba979276d5158119df01dc3583"
         },
         "pipfile-spec": 6,
         "requires": {
             "python_version": "3.10"
         },
         "sources": [
             {
@@ -257,19 +257,19 @@
                 "sha256:90b77e79eaa3eba6de819a0c442c0b4ceefc341a7a2ab77d7562bf49f425c5c2"
             ],
             "markers": "python_version >= '3.5'",
             "version": "==3.4"
         },
         "ipykernel": {
             "hashes": [
-                "sha256:1ae6047c1277508933078163721bbb479c3e7292778a04b4bacf0874550977d6",
-                "sha256:302558b81f1bc22dc259fb2a0c5c7cf2f4c0bdb21b50484348f7bafe7fb71421"
+                "sha256:1aba0ae8453e15e9bc6b24e497ef6840114afcdb832ae597f32137fa19d42a6f",
+                "sha256:77aeffab056c21d16f1edccdc9e5ccbf7d96eb401bd6703610a21be8b068aadc"
             ],
             "markers": "python_version >= '3.8'",
-            "version": "==6.22.0"
+            "version": "==6.23.1"
         },
         "ipython": {
             "hashes": [
                 "sha256:7dff3fad32b97f6488e02f87b970f309d082f758d7b7fc252e3b19ee0e432dbb",
                 "sha256:ffca270240fbd21b06b2974e14a86494d6d29290184e788275f55e0b55914926"
             ],
             "markers": "python_version >= '3.9'",
@@ -502,19 +502,19 @@
                 "sha256:d447f0e5a4cfe79d462459aec1b3dc5c2e9152597262be8ee27f7d4c02566a0d"
             ],
             "markers": "python_full_version >= '3.7.0'",
             "version": "==0.7.4"
         },
         "nbconvert": {
             "hashes": [
-                "sha256:78685362b11d2e8058e70196fe83b09abed8df22d3e599cf271f4d39fdc48b9e",
-                "sha256:d2e95904666f1ff77d36105b9de4e0801726f93b862d5b28f69e93d99ad3b19c"
+                "sha256:51b6c77b507b177b73f6729dba15676e42c4e92bcb00edc8cc982ee72e7d89d7",
+                "sha256:af5064a9db524f9f12f4e8be7f0799524bd5b14c1adea37e34e83c95127cc818"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==7.3.1"
+            "version": "==7.4.0"
         },
         "nbformat": {
             "hashes": [
                 "sha256:46dac64c781f1c34dfd8acba16547024110348f9fc7eab0f31981c2a3dc48d1f",
                 "sha256:d910082bd3e0bffcf07eabf3683ed7dda0727a326c446eeb2922abe102e65162"
             ],
             "markers": "python_version >= '3.7'",
@@ -648,19 +648,19 @@
                 "sha256:87683d47965c1da65cdacaf31c8441d12b8044cdec9aca500cd78fc2c683afca",
                 "sha256:9649af414d74d4df115d5d718f82acb59c9d418196b7b4290ed47a12ce62df56"
             ],
             "version": "==0.7.5"
         },
         "platformdirs": {
             "hashes": [
-                "sha256:47692bc24c1958e8b0f13dd727307cff1db103fca36399f457da8e05f222fdc4",
-                "sha256:7954a68d0ba23558d753f73437c55f89027cf8f5108c19844d4b82e5af396335"
+                "sha256:412dae91f52a6f84830f39a8078cecd0e866cb72294a5c66808e74d5e88d251f",
+                "sha256:e2378146f1964972c03c085bb5662ae80b2b8c06226c54b2ff4aa9483e8a13a5"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.5.0"
+            "version": "==3.5.1"
         },
         "prometheus-client": {
             "hashes": [
                 "sha256:0836af6eb2c8f4fed712b2f279f6c0a8bbab29f9f4aa15276b91c7cb0d1616ab",
                 "sha256:a03e35b359f14dd1630898543e2120addfdeacd1a6069c1367ae90fd93ad3f48"
             ],
             "markers": "python_version >= '3.6'",
@@ -1056,28 +1056,28 @@
                 "sha256:8cff3a8f066c2ec677c06dbc7b45619804a6938478d9d73c284b29d14ecb0627"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==1.2.1"
         },
         "tornado": {
             "hashes": [
-                "sha256:1285f0691143f7ab97150831455d4db17a267b59649f7bd9700282cba3d5e771",
-                "sha256:3455133b9ff262fd0a75630af0a8ee13564f25fb4fd3d9ce239b8a7d3d027bf8",
-                "sha256:5e2f49ad371595957c50e42dd7e5c14d64a6843a3cf27352b69c706d1b5918af",
-                "sha256:81c17e0cc396908a5e25dc8e9c5e4936e6dfd544c9290be48bd054c79bcad51e",
-                "sha256:90f569a35a8ec19bde53aa596952071f445da678ec8596af763b9b9ce07605e6",
-                "sha256:9661aa8bc0e9d83d757cd95b6f6d1ece8ca9fd1ccdd34db2de381e25bf818233",
-                "sha256:a27a1cfa9997923f80bdd962b3aab048ac486ad8cfb2f237964f8ab7f7eb824b",
-                "sha256:b4e7b956f9b5e6f9feb643ea04f07e7c6b49301e03e0023eedb01fa8cf52f579",
-                "sha256:d7117f3c7ba5d05813b17a1f04efc8e108a1b811ccfddd9134cc68553c414864",
-                "sha256:db181eb3df8738613ff0a26f49e1b394aade05034b01200a63e9662f347d4415",
-                "sha256:ffdce65a281fd708da5a9def3bfb8f364766847fa7ed806821a69094c9629e8a"
+                "sha256:05615096845cf50a895026f749195bf0b10b8909f9be672f50b0fe69cba368e4",
+                "sha256:0c325e66c8123c606eea33084976c832aa4e766b7dff8aedd7587ea44a604cdf",
+                "sha256:29e71c847a35f6e10ca3b5c2990a52ce38b233019d8e858b755ea6ce4dcdd19d",
+                "sha256:4b927c4f19b71e627b13f3db2324e4ae660527143f9e1f2e2fb404f3a187e2ba",
+                "sha256:5b17b1cf5f8354efa3d37c6e28fdfd9c1c1e5122f2cb56dac121ac61baa47cbe",
+                "sha256:6a0848f1aea0d196a7c4f6772197cbe2abc4266f836b0aac76947872cd29b411",
+                "sha256:7efcbcc30b7c654eb6a8c9c9da787a851c18f8ccd4a5a3a95b05c7accfa068d2",
+                "sha256:834ae7540ad3a83199a8da8f9f2d383e3c3d5130a328889e4cc991acc81e87a0",
+                "sha256:b46a6ab20f5c7c1cb949c72c1994a4585d2eaa0be4853f50a03b5031e964fc7c",
+                "sha256:c2de14066c4a38b4ecbbcd55c5cc4b5340eb04f1c5e81da7451ef555859c833f",
+                "sha256:c367ab6c0393d71171123ca5515c61ff62fe09024fa6bf299cd1339dc9456829"
             ],
             "markers": "python_version >= '3.8'",
-            "version": "==6.3.1"
+            "version": "==6.3.2"
         },
         "tqdm": {
             "hashes": [
                 "sha256:1871fb68a86b8fb3b59ca4cdd3dcccbc7e6d613eeed31f4c332531977b89beb5",
                 "sha256:c4f53a17fe37e132815abceec022631be8ffe1b9381c2e6e30aa70edc99e9671"
             ],
             "index": "pypi",
@@ -1130,14 +1130,26 @@
         "widgetsnbextension": {
             "hashes": [
                 "sha256:be3228a73bbab189a16be2d4a3cd89ecbd4e31948bfdc64edac17dcdee3cd99c",
                 "sha256:ea67c17a7cd4ae358f8f46c3b304c40698bc0423732e3f273321ee141232c8be"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==4.0.7"
+        },
+        "xgboost": {
+            "hashes": [
+                "sha256:1d1dda6b84ea50a2ea1ed18390e93e275d57dc4cffd682014dc30ae5a116c92b",
+                "sha256:63474265a0194f27889c6fb54e5939ad21bcd5fcfaca7b6a89e143be42ed7ad1",
+                "sha256:9eed5629c9008c36d65db6869defac31de635f766f215fc4b09b6a389c637f27",
+                "sha256:ac17664ff24ea1c160a0d50aff521b654f0911f4684a88bbb46a074c46c9e3f1",
+                "sha256:af3227dbd839a8e2a215844a6276eae027d5f83a9cb501148dfcdb047a195411",
+                "sha256:ca9e8455343cc3f1fddc825209ad00623bc82de0364097b31d649bca6a5f8fb4"
+            ],
+            "index": "pypi",
+            "version": "==1.7.5"
         }
     },
     "develop": {
         "black": {
             "hashes": [
                 "sha256:064101748afa12ad2291c2b91c960be28b817c0c7eaa35bec09cc63aa56493c5",
                 "sha256:0945e13506be58bf7db93ee5853243eb368ace1c08a24c65ce108986eac65915",
@@ -1238,19 +1250,19 @@
                 "sha256:d8af70af76652554bd134c22b3e8a1cc46ed7d91edcdd721ef1a0c51a84a5293"
             ],
             "markers": "python_version >= '3.7'",
             "version": "==0.11.1"
         },
         "platformdirs": {
             "hashes": [
-                "sha256:47692bc24c1958e8b0f13dd727307cff1db103fca36399f457da8e05f222fdc4",
-                "sha256:7954a68d0ba23558d753f73437c55f89027cf8f5108c19844d4b82e5af396335"
+                "sha256:412dae91f52a6f84830f39a8078cecd0e866cb72294a5c66808e74d5e88d251f",
+                "sha256:e2378146f1964972c03c085bb5662ae80b2b8c06226c54b2ff4aa9483e8a13a5"
             ],
             "markers": "python_version >= '3.7'",
-            "version": "==3.5.0"
+            "version": "==3.5.1"
         },
         "pluggy": {
             "hashes": [
                 "sha256:4224373bacce55f955a878bf9cfa763c1e360858e330072059e10bad68531159",
                 "sha256:74134bbf457f031a36d68416e1509f34bd5ccc019f0bcc952c7b909d06b37bd3"
             ],
             "markers": "python_version >= '3.6'",
```

### Comparing `lazylearn-0.0.2/.github/workflows/verify.yaml` & `lazylearn-0.0.3/.github/workflows/verify.yaml`

 * *Files identical despite different names*

### Comparing `lazylearn-0.0.2/doc/logo/grayscale_transparent.png` & `lazylearn-0.0.3/doc/logo/grayscale_transparent.png`

 * *Files identical despite different names*

### Comparing `lazylearn-0.0.2/doc/logo/original.png` & `lazylearn-0.0.3/doc/logo/original.png`

 * *Files identical despite different names*

### Comparing `lazylearn-0.0.2/doc/logo/transparent.png` & `lazylearn-0.0.3/doc/logo/transparent.png`

 * *Files identical despite different names*

### Comparing `lazylearn-0.0.2/doc/logo/transparent_small.png` & `lazylearn-0.0.3/doc/logo/transparent_small.png`

 * *Files identical despite different names*

### Comparing `lazylearn-0.0.2/python/src/lazylearn/ingestion/ingestion_pipeline.py` & `lazylearn-0.0.3/python/src/lazylearn/ingestion/ingestion_pipeline.py`

 * *Files identical despite different names*

### Comparing `lazylearn-0.0.2/python/src/lazylearn/ingestion/ingestion_pipeline_steps/data_parser_step.py` & `lazylearn-0.0.3/python/src/lazylearn/ingestion/ingestion_pipeline_steps/data_parser_step.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+import pandas as pd
 from errors.errors import DataSourceError
+from ingestion.utils.csv import csv_check
 from pandas import DataFrame
 from pipeline.pipeline import IngestionPipeline, PipelineStep
 
 
 class DataSourceParser(PipelineStep):
     def apply(self, pipeline: IngestionPipeline):
         """
@@ -13,9 +15,12 @@
         :param pipeline: parent IngestionPipeline
         :return:
         """
         assert pipeline.raw_data is not None
 
         if isinstance(pipeline.raw_data, DataFrame):
             pipeline.df = pipeline.raw_data
+        # check if raw data is a path to a csv file and read it into csv
+        elif csv_check(pipeline.df):
+            pipeline.df = pd.read_csv(pipeline.raw_data)
         else:
             raise DataSourceError
```

### Comparing `lazylearn-0.0.2/python/src/lazylearn/ingestion/ingestion_pipeline_steps/summary_stats_step.py` & `lazylearn-0.0.3/python/src/lazylearn/ingestion/ingestion_pipeline_steps/summary_stats_step.py`

 * *Files identical despite different names*

### Comparing `lazylearn-0.0.2/python/src/test/ingestion/ingestion_pipeline_steps/test_interpreter_step.py` & `lazylearn-0.0.3/python/src/test/ingestion/ingestion_pipeline_steps/test_interpreter_step.py`

 * *Files identical despite different names*

### Comparing `lazylearn-0.0.2/python/src/test/ingestion/ingestion_pipeline_steps/test_summary_stats_step.py` & `lazylearn-0.0.3/python/src/test/ingestion/ingestion_pipeline_steps/test_summary_stats_step.py`

 * *Files identical despite different names*

### Comparing `lazylearn-0.0.2/shell/check.sh` & `lazylearn-0.0.3/shell/check.sh`

 * *Files identical despite different names*

### Comparing `lazylearn-0.0.2/.gitignore` & `lazylearn-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `lazylearn-0.0.2/LICENSE` & `lazylearn-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lazylearn-0.0.2/README.md` & `lazylearn-0.0.3/README.md`

 * *Files 27% similar despite different names*

```diff
@@ -1,26 +1,39 @@
 
 <img width="500" src="doc/logo/transparent_small.png">
 
 **lazy-learn** is a high-level Python interface for automated machine learning (AutoML). While there are many AutoML libraries available each typically solves a niche area of the overall ML pipeline without providing a covering and approachable end-to-end system.
 
 The aim of lazy-learn is exactly that. Given a dataset, easy-learn will analyse types and distributions of attributes, preprocess, feature-engineer and ultimately train models to be used for further evaluation or inference. 
 
+## Upcoming features
+
+Current stable version is 0.0.3. The upcoming updates will support:
+- Abstract construction of model architectures
+- XGBoost, LightGBM, Adaboost and Catboost architectures
+- Time partitioning of datasets
+- Automated Hyperparameter Optimisation (HPO)
+- Text features
+- An interface to AutoGluon
+- Outlier detection and handling
+- Automated suggestions of performance metrics
+
 ## Usage
 
 Using lazy-learn revolves around the `LazyLearner` class. You can think of it as a kind of project, and it is the wrapper for any experiment within lazy-learn.
 
 ## Installation
 
 ### Dependencies
 
 lazy-learn requires:
 
 - pandas
 - scikit-learn
+- xgboost
 
 ### User Installation 
 ```
 pip install lazy-learn
 ```
 
 ## Help and Support
```

### Comparing `lazylearn-0.0.2/pyproject.toml` & `lazylearn-0.0.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "lazylearn"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Frederik P. Høngaard", email="mail@frederikhoengaard.com" },
 ]
 description = "lazy-learn is a high-level Python interface for automated machine learning (AutoML) for the lazy data scientist. While there are many AutoML libraries available each typically solves a niche area of the overall ML pipeline without providing a covering and approachable end-to-end system. lazy-learn aims at providing the most approachable and fastest access to building baseline models."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `lazylearn-0.0.2/PKG-INFO` & `lazylearn-0.0.3/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazylearn
-Version: 0.0.2
+Version: 0.0.3
 Summary: lazy-learn is a high-level Python interface for automated machine learning (AutoML) for the lazy data scientist. While there are many AutoML libraries available each typically solves a niche area of the overall ML pipeline without providing a covering and approachable end-to-end system. lazy-learn aims at providing the most approachable and fastest access to building baseline models.
 Project-URL: Homepage, https://github.com/frederikhoengaard/lazy-learn
 Author-email: "Frederik P. Høngaard" <mail@frederikhoengaard.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -14,26 +14,39 @@
 
 <img width="500" src="doc/logo/transparent_small.png">
 
 **lazy-learn** is a high-level Python interface for automated machine learning (AutoML). While there are many AutoML libraries available each typically solves a niche area of the overall ML pipeline without providing a covering and approachable end-to-end system.
 
 The aim of lazy-learn is exactly that. Given a dataset, easy-learn will analyse types and distributions of attributes, preprocess, feature-engineer and ultimately train models to be used for further evaluation or inference. 
 
+## Upcoming features
+
+Current stable version is 0.0.3. The upcoming updates will support:
+- Abstract construction of model architectures
+- XGBoost, LightGBM, Adaboost and Catboost architectures
+- Time partitioning of datasets
+- Automated Hyperparameter Optimisation (HPO)
+- Text features
+- An interface to AutoGluon
+- Outlier detection and handling
+- Automated suggestions of performance metrics
+
 ## Usage
 
 Using lazy-learn revolves around the `LazyLearner` class. You can think of it as a kind of project, and it is the wrapper for any experiment within lazy-learn.
 
 ## Installation
 
 ### Dependencies
 
 lazy-learn requires:
 
 - pandas
 - scikit-learn
+- xgboost
 
 ### User Installation 
 ```
 pip install lazy-learn
 ```
 
 ## Help and Support
```

