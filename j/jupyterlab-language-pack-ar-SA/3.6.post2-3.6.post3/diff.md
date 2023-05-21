# Comparing `tmp/jupyterlab_language_pack_ar_sa-3.6.post2.tar.gz` & `tmp/jupyterlab_language_pack_ar_sa-3.6.post3.tar.gz`

## Comparing `jupyterlab_language_pack_ar_sa-3.6.post2.tar` & `jupyterlab_language_pack_ar_sa-3.6.post3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ar_sa-3.6.post2/.copier-answers.yml
--rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ar_sa-3.6.post2/CONTRIBUTORS.md
--rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ar_sa-3.6.post2/jupyterlab_language_pack_ar_SA/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ar_sa-3.6.post2/jupyterlab_language_pack_ar_SA/locale/ar_SA/LC_MESSAGES/.gitkeep
--rw-r--r--   0        0        0     3783 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ar_sa-3.6.post2/jupyterlab_language_pack_ar_SA/locale/ar_SA/LC_MESSAGES/dask_labextension.po
--rw-r--r--   0        0        0     2254 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ar_sa-3.6.post2/jupyterlab_language_pack_ar_SA/locale/ar_SA/LC_MESSAGES/jupyter_archive.po
--rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ar_sa-3.6.post2/jupyterlab_language_pack_ar_SA/locale/ar_SA/LC_MESSAGES/jupyter_collaboration.po
--rw-r--r--   0        0        0     5015 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ar_sa-3.6.post2/jupyterlab_language_pack_ar_SA/locale/ar_SA/LC_MESSAGES/jupyter_resource_usage.po
--rw-r--r--   0        0        0   271271 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ar_sa-3.6.post2/jupyterlab_language_pack_ar_SA/locale/ar_SA/LC_MESSAGES/jupyterlab.po
--rw-r--r--   0        0        0    96410 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ar_sa-3.6.post2/jupyterlab_language_pack_ar_SA/locale/ar_SA/LC_MESSAGES/jupyterlab_git.po
--rw-r--r--   0        0        0    42964 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ar_sa-3.6.post2/jupyterlab_language_pack_ar_SA/locale/ar_SA/LC_MESSAGES/jupyterlab_lsp.po
--rw-r--r--   0        0        0     4377 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ar_sa-3.6.post2/jupyterlab_language_pack_ar_SA/locale/ar_SA/LC_MESSAGES/jupyterlab_search_replace.po
--rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ar_sa-3.6.post2/jupyterlab_language_pack_ar_SA/locale/ar_SA/LC_MESSAGES/jupyterlab_spreadsheet_editor.po
--rw-r--r--   0        0        0     3432 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ar_sa-3.6.post2/jupyterlab_language_pack_ar_SA/locale/ar_SA/LC_MESSAGES/jupyterlab_tour.po
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ar_sa-3.6.post2/jupyterlab_language_pack_ar_SA/locale/ar_SA/LC_MESSAGES/jupyterlab_widgets.po
--rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ar_sa-3.6.post2/jupyterlab_language_pack_ar_SA/locale/ar_SA/LC_MESSAGES/jupytext.po
--rw-r--r--   0        0        0     9914 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ar_sa-3.6.post2/jupyterlab_language_pack_ar_SA/locale/ar_SA/LC_MESSAGES/notebook.po
--rw-r--r--   0        0        0     4854 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ar_sa-3.6.post2/jupyterlab_language_pack_ar_SA/locale/ar_SA/LC_MESSAGES/retrolab.po
--rw-r--r--   0        0        0     3907 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ar_sa-3.6.post2/jupyterlab_language_pack_ar_SA/locale/ar_SA/LC_MESSAGES/spellchecker.po
--rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ar_sa-3.6.post2/.gitignore
--rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ar_sa-3.6.post2/LICENSE.txt
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ar_sa-3.6.post2/README.md
--rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ar_sa-3.6.post2/pyproject.toml
--rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ar_sa-3.6.post2/PKG-INFO
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ar_sa-3.6.post3/.copier-answers.yml
+-rw-r--r--   0        0        0      476 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ar_sa-3.6.post3/CONTRIBUTORS.md
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ar_sa-3.6.post3/jupyterlab_language_pack_ar_SA/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ar_sa-3.6.post3/jupyterlab_language_pack_ar_SA/locale/ar_SA/LC_MESSAGES/.gitkeep
+-rw-r--r--   0        0        0     3783 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ar_sa-3.6.post3/jupyterlab_language_pack_ar_SA/locale/ar_SA/LC_MESSAGES/dask_labextension.po
+-rw-r--r--   0        0        0     2254 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ar_sa-3.6.post3/jupyterlab_language_pack_ar_SA/locale/ar_SA/LC_MESSAGES/jupyter_archive.po
+-rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ar_sa-3.6.post3/jupyterlab_language_pack_ar_SA/locale/ar_SA/LC_MESSAGES/jupyter_collaboration.po
+-rw-r--r--   0        0        0     5015 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ar_sa-3.6.post3/jupyterlab_language_pack_ar_SA/locale/ar_SA/LC_MESSAGES/jupyter_resource_usage.po
+-rw-r--r--   0        0        0   271271 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ar_sa-3.6.post3/jupyterlab_language_pack_ar_SA/locale/ar_SA/LC_MESSAGES/jupyterlab.po
+-rw-r--r--   0        0        0    96410 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ar_sa-3.6.post3/jupyterlab_language_pack_ar_SA/locale/ar_SA/LC_MESSAGES/jupyterlab_git.po
+-rw-r--r--   0        0        0    42964 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ar_sa-3.6.post3/jupyterlab_language_pack_ar_SA/locale/ar_SA/LC_MESSAGES/jupyterlab_lsp.po
+-rw-r--r--   0        0        0     4377 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ar_sa-3.6.post3/jupyterlab_language_pack_ar_SA/locale/ar_SA/LC_MESSAGES/jupyterlab_search_replace.po
+-rw-r--r--   0        0        0     2331 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ar_sa-3.6.post3/jupyterlab_language_pack_ar_SA/locale/ar_SA/LC_MESSAGES/jupyterlab_spreadsheet_editor.po
+-rw-r--r--   0        0        0     3432 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ar_sa-3.6.post3/jupyterlab_language_pack_ar_SA/locale/ar_SA/LC_MESSAGES/jupyterlab_tour.po
+-rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ar_sa-3.6.post3/jupyterlab_language_pack_ar_SA/locale/ar_SA/LC_MESSAGES/jupyterlab_widgets.po
+-rw-r--r--   0        0        0     2357 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ar_sa-3.6.post3/jupyterlab_language_pack_ar_SA/locale/ar_SA/LC_MESSAGES/jupytext.po
+-rw-r--r--   0        0        0     9914 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ar_sa-3.6.post3/jupyterlab_language_pack_ar_SA/locale/ar_SA/LC_MESSAGES/notebook.po
+-rw-r--r--   0        0        0     4854 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ar_sa-3.6.post3/jupyterlab_language_pack_ar_SA/locale/ar_SA/LC_MESSAGES/retrolab.po
+-rw-r--r--   0        0        0     3907 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ar_sa-3.6.post3/jupyterlab_language_pack_ar_SA/locale/ar_SA/LC_MESSAGES/spellchecker.po
+-rw-r--r--   0        0        0     1883 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ar_sa-3.6.post3/.gitignore
+-rw-r--r--   0        0        0     1513 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ar_sa-3.6.post3/LICENSE.txt
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ar_sa-3.6.post3/README.md
+-rw-r--r--   0        0        0     1248 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ar_sa-3.6.post3/pyproject.toml
+-rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 jupyterlab_language_pack_ar_sa-3.6.post3/PKG-INFO
```

### Comparing `jupyterlab_language_pack_ar_sa-3.6.post2/jupyterlab_language_pack_ar_SA/locale/ar_SA/LC_MESSAGES/dask_labextension.po` & `jupyterlab_language_pack_ar_sa-3.6.post3/jupyterlab_language_pack_ar_SA/locale/ar_SA/LC_MESSAGES/dask_labextension.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ar_sa-3.6.post2/jupyterlab_language_pack_ar_SA/locale/ar_SA/LC_MESSAGES/jupyter_archive.po` & `jupyterlab_language_pack_ar_sa-3.6.post3/jupyterlab_language_pack_ar_SA/locale/ar_SA/LC_MESSAGES/jupyter_archive.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ar_sa-3.6.post2/jupyterlab_language_pack_ar_SA/locale/ar_SA/LC_MESSAGES/jupyter_collaboration.po` & `jupyterlab_language_pack_ar_sa-3.6.post3/jupyterlab_language_pack_ar_SA/locale/ar_SA/LC_MESSAGES/jupyter_collaboration.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ar_sa-3.6.post2/jupyterlab_language_pack_ar_SA/locale/ar_SA/LC_MESSAGES/jupyter_resource_usage.po` & `jupyterlab_language_pack_ar_sa-3.6.post3/jupyterlab_language_pack_ar_SA/locale/ar_SA/LC_MESSAGES/jupyter_resource_usage.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ar_sa-3.6.post2/jupyterlab_language_pack_ar_SA/locale/ar_SA/LC_MESSAGES/jupyterlab.po` & `jupyterlab_language_pack_ar_sa-3.6.post3/jupyterlab_language_pack_ar_SA/locale/ar_SA/LC_MESSAGES/jupyterlab.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ar_sa-3.6.post2/jupyterlab_language_pack_ar_SA/locale/ar_SA/LC_MESSAGES/jupyterlab_git.po` & `jupyterlab_language_pack_ar_sa-3.6.post3/jupyterlab_language_pack_ar_SA/locale/ar_SA/LC_MESSAGES/jupyterlab_git.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ar_sa-3.6.post2/jupyterlab_language_pack_ar_SA/locale/ar_SA/LC_MESSAGES/jupyterlab_lsp.po` & `jupyterlab_language_pack_ar_sa-3.6.post3/jupyterlab_language_pack_ar_SA/locale/ar_SA/LC_MESSAGES/jupyterlab_lsp.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ar_sa-3.6.post2/jupyterlab_language_pack_ar_SA/locale/ar_SA/LC_MESSAGES/jupyterlab_search_replace.po` & `jupyterlab_language_pack_ar_sa-3.6.post3/jupyterlab_language_pack_ar_SA/locale/ar_SA/LC_MESSAGES/jupyterlab_search_replace.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ar_sa-3.6.post2/jupyterlab_language_pack_ar_SA/locale/ar_SA/LC_MESSAGES/jupyterlab_spreadsheet_editor.po` & `jupyterlab_language_pack_ar_sa-3.6.post3/jupyterlab_language_pack_ar_SA/locale/ar_SA/LC_MESSAGES/jupyterlab_spreadsheet_editor.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ar_sa-3.6.post2/jupyterlab_language_pack_ar_SA/locale/ar_SA/LC_MESSAGES/jupyterlab_tour.po` & `jupyterlab_language_pack_ar_sa-3.6.post3/jupyterlab_language_pack_ar_SA/locale/ar_SA/LC_MESSAGES/jupyterlab_tour.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ar_sa-3.6.post2/jupyterlab_language_pack_ar_SA/locale/ar_SA/LC_MESSAGES/jupyterlab_widgets.po` & `jupyterlab_language_pack_ar_sa-3.6.post3/jupyterlab_language_pack_ar_SA/locale/ar_SA/LC_MESSAGES/jupyterlab_widgets.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ar_sa-3.6.post2/jupyterlab_language_pack_ar_SA/locale/ar_SA/LC_MESSAGES/jupytext.po` & `jupyterlab_language_pack_ar_sa-3.6.post3/jupyterlab_language_pack_ar_SA/locale/ar_SA/LC_MESSAGES/jupytext.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ar_sa-3.6.post2/jupyterlab_language_pack_ar_SA/locale/ar_SA/LC_MESSAGES/notebook.po` & `jupyterlab_language_pack_ar_sa-3.6.post3/jupyterlab_language_pack_ar_SA/locale/ar_SA/LC_MESSAGES/notebook.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ar_sa-3.6.post2/jupyterlab_language_pack_ar_SA/locale/ar_SA/LC_MESSAGES/retrolab.po` & `jupyterlab_language_pack_ar_sa-3.6.post3/jupyterlab_language_pack_ar_SA/locale/ar_SA/LC_MESSAGES/retrolab.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ar_sa-3.6.post2/jupyterlab_language_pack_ar_SA/locale/ar_SA/LC_MESSAGES/spellchecker.po` & `jupyterlab_language_pack_ar_sa-3.6.post3/jupyterlab_language_pack_ar_SA/locale/ar_SA/LC_MESSAGES/spellchecker.po`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ar_sa-3.6.post2/.gitignore` & `jupyterlab_language_pack_ar_sa-3.6.post3/.gitignore`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ar_sa-3.6.post2/LICENSE.txt` & `jupyterlab_language_pack_ar_sa-3.6.post3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ar_sa-3.6.post2/pyproject.toml` & `jupyterlab_language_pack_ar_sa-3.6.post3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `jupyterlab_language_pack_ar_sa-3.6.post2/PKG-INFO` & `jupyterlab_language_pack_ar_sa-3.6.post3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jupyterlab-language-pack-ar-SA
-Version: 3.6.post2
+Version: 3.6.post3
 Summary: JupyterLab Arabic (Saudi Arabia) Language Pack
 Author-email: Project Jupyter Contributors <jupyter@googlegroups.com>
 License: Copyright (c) 2023 Project Jupyter Contributors
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
         modification, are permitted provided that the following conditions are met:
```

