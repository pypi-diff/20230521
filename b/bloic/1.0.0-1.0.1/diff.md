# Comparing `tmp/bloic-1.0.0.tar.gz` & `tmp/bloic-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bloic-1.0.0.tar", last modified: Thu May 18 15:09:38 2023, max compression
+gzip compressed data, was "bloic-1.0.1.tar", last modified: Sun May 21 14:35:43 2023, max compression
```

## Comparing `bloic-1.0.0.tar` & `bloic-1.0.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:09:38.403806 bloic-1.0.0/
--rw-rw-rw-   0 root         (0) root         (0)      810 2023-05-18 15:09:28.000000 bloic-1.0.0/.dockerignore
--rw-rw-rw-   0 root         (0) root         (0)      835 2023-05-18 15:09:28.000000 bloic-1.0.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)     1271 2023-05-18 15:09:28.000000 bloic-1.0.0/.gitlab-ci.yml
--rw-rw-rw-   0 root         (0) root         (0)      161 2023-05-18 15:09:28.000000 bloic-1.0.0/Dockerfile
--rw-rw-rw-   0 root         (0) root         (0)     1071 2023-05-18 15:09:28.000000 bloic-1.0.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2188 2023-05-18 15:09:38.403806 bloic-1.0.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     1577 2023-05-18 15:09:28.000000 bloic-1.0.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:09:38.401806 bloic-1.0.0/bloic/
--rw-rw-rw-   0 root         (0) root         (0)      132 2023-05-18 15:09:28.000000 bloic-1.0.0/bloic/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      165 2023-05-18 15:09:28.000000 bloic-1.0.0/bloic/__main__.py
--rw-r--r--   0 root         (0) root         (0)      160 2023-05-18 15:09:38.000000 bloic-1.0.0/bloic/_version.py
--rw-rw-rw-   0 root         (0) root         (0)     1858 2023-05-18 15:09:28.000000 bloic-1.0.0/bloic/entrypoint.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-18 15:09:38.403806 bloic-1.0.0/bloic.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2188 2023-05-18 15:09:38.000000 bloic-1.0.0/bloic.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      350 2023-05-18 15:09:38.000000 bloic-1.0.0/bloic.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-18 15:09:38.000000 bloic-1.0.0/bloic.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       55 2023-05-18 15:09:38.000000 bloic-1.0.0/bloic.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)       13 2023-05-18 15:09:38.000000 bloic-1.0.0/bloic.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-05-18 15:09:38.000000 bloic-1.0.0/bloic.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)      912 2023-05-18 15:09:28.000000 bloic-1.0.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)       26 2023-05-18 15:09:28.000000 bloic-1.0.0/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-18 15:09:38.403806 bloic-1.0.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 14:35:43.157767 bloic-1.0.1/
+-rw-rw-rw-   0 root         (0) root         (0)      810 2023-05-21 14:35:34.000000 bloic-1.0.1/.dockerignore
+-rw-rw-rw-   0 root         (0) root         (0)      887 2023-05-21 14:35:34.000000 bloic-1.0.1/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)     1337 2023-05-21 14:35:34.000000 bloic-1.0.1/.gitlab-ci.yml
+-rw-rw-rw-   0 root         (0) root         (0)      161 2023-05-21 14:35:34.000000 bloic-1.0.1/Dockerfile
+-rw-rw-rw-   0 root         (0) root         (0)     1071 2023-05-21 14:35:34.000000 bloic-1.0.1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2303 2023-05-21 14:35:43.156767 bloic-1.0.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1692 2023-05-21 14:35:34.000000 bloic-1.0.1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 14:35:43.155767 bloic-1.0.1/bloic/
+-rw-rw-rw-   0 root         (0) root         (0)      132 2023-05-21 14:35:34.000000 bloic-1.0.1/bloic/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      165 2023-05-21 14:35:34.000000 bloic-1.0.1/bloic/__main__.py
+-rw-r--r--   0 root         (0) root         (0)      160 2023-05-21 14:35:43.000000 bloic-1.0.1/bloic/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)     1924 2023-05-21 14:35:34.000000 bloic-1.0.1/bloic/entrypoint.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-21 14:35:43.156767 bloic-1.0.1/bloic.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2303 2023-05-21 14:35:43.000000 bloic-1.0.1/bloic.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      350 2023-05-21 14:35:43.000000 bloic-1.0.1/bloic.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-21 14:35:43.000000 bloic-1.0.1/bloic.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       56 2023-05-21 14:35:43.000000 bloic-1.0.1/bloic.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2023-05-21 14:35:43.000000 bloic-1.0.1/bloic.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-21 14:35:43.000000 bloic-1.0.1/bloic.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)      934 2023-05-21 14:35:34.000000 bloic-1.0.1/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       26 2023-05-21 14:35:34.000000 bloic-1.0.1/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-21 14:35:43.157767 bloic-1.0.1/setup.cfg
```

### Comparing `bloic-1.0.0/.dockerignore` & `bloic-1.0.1/.dockerignore`

 * *Files identical despite different names*

### Comparing `bloic-1.0.0/.gitignore` & `bloic-1.0.1/.gitignore`

 * *Files 6% similar despite different names*

```diff
@@ -74,8 +74,11 @@
 *.jfi
 *.gif
 *.raw
 *.webp
 *.png
 *.svg
 *.svgz
-*.pdf
+*.pdf
+
+# Version file (auto generated)
+bloic/_version.py
```

### Comparing `bloic-1.0.0/.gitlab-ci.yml` & `bloic-1.0.1/.gitlab-ci.yml`

 * *Files 4% similar despite different names*

```diff
@@ -48,18 +48,20 @@
     - if: $CI_COMMIT_TAG != null
 
 release:
   stage: release
   image: registry.gitlab.com/gitlab-org/release-cli:latest
   rules:
     - if: $CI_COMMIT_TAG != null
+  variables:
+    PYPI_PROJECT_NAME: bloic   
   script:
     - echo "Running the release job."
   release:
     tag_name: $CI_COMMIT_TAG
     name: '$CI_COMMIT_TAG'
     description: '$CI_COMMIT_TAG_MESSAGE'
     assets:
       links:
-        - name: ${CI_PROJECT_NAME}
-          url: https://pypi.org/project/${CI_PROJECT_NAME}/${CI_COMMIT_TAG}/
+        - name: ${PYPI_PROJECT_NAME} ${CI_COMMIT_TAG}
+          url: https://pypi.org/project/${PYPI_PROJECT_NAME}/${CI_COMMIT_TAG}/
           link_type: 'package'
```

### Comparing `bloic-1.0.0/LICENSE` & `bloic-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bloic-1.0.0/PKG-INFO` & `bloic-1.0.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bloic
-Version: 1.0.0
+Version: 1.0.1
 Summary: Tool to convert and resize image for blog post.
 Author: romaiiiiinnn
 License: MIT
 Project-URL: Homepage, https://gitlab.com/romaiiiinnn/blog-post-image-converter
 Project-URL: Bug Tracker, https://gitlab.com/romaiiiinnn/blog-post-image-converter/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: Console
@@ -44,17 +44,19 @@
 ```console
 Usage: bloic [OPTIONS] IMAGE_PATH
 
   Resizes an image based on a target width passed as a parameter, then
   converts it to the WebP format.
 
 Options:
+  --version                   Show the version and exit.
   -w, --width INTEGER RANGE   Target width of the image  [default: 1200; x>0]
   -o, --output-dir DIRECTORY  Output directory  [default: .]
   -d, --delete                Delete source image after conversion.
+  --help                      Show this message and exit.
 ```
 
 ### Examples
 
 Follwing command will create image named `image.webp` with a width of 1200px in current directory.
 
 #### With installed package
```

### Comparing `bloic-1.0.0/README.md` & `bloic-1.0.1/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -27,17 +27,19 @@
 ```console
 Usage: bloic [OPTIONS] IMAGE_PATH
 
   Resizes an image based on a target width passed as a parameter, then
   converts it to the WebP format.
 
 Options:
+  --version                   Show the version and exit.
   -w, --width INTEGER RANGE   Target width of the image  [default: 1200; x>0]
   -o, --output-dir DIRECTORY  Output directory  [default: .]
   -d, --delete                Delete source image after conversion.
+  --help                      Show this message and exit.
 ```
 
 ### Examples
 
 Follwing command will create image named `image.webp` with a width of 1200px in current directory.
 
 #### With installed package
```

### Comparing `bloic-1.0.0/bloic/entrypoint.py` & `bloic-1.0.1/bloic/entrypoint.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import os
 
 import click
 from PIL import Image
 
+from bloic import __version__
+
 
 @click.command()
+@click.version_option(__version__)
 @click.argument('image_path', type=click.Path(exists=True, dir_okay=False, resolve_path=True))
 @click.option('--width', '-w', type=click.IntRange(min=0, min_open=True), default=1200, show_default=True, help='Target width of the image')
 @click.option('--output-dir', '-o', type=click.Path(exists=True, file_okay=False, writable=True, resolve_path=True), default='.', show_default=True, help='Output directory')
 @click.option('--delete', '-d', is_flag=True, help='Delete source image after conversion.')
 def resize_image(image_path, width, output_dir, delete):
     """
     Resizes an image based on a target width passed as a parameter, then converts it to the WebP format.
```

### Comparing `bloic-1.0.0/bloic.egg-info/PKG-INFO` & `bloic-1.0.1/bloic.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bloic
-Version: 1.0.0
+Version: 1.0.1
 Summary: Tool to convert and resize image for blog post.
 Author: romaiiiiinnn
 License: MIT
 Project-URL: Homepage, https://gitlab.com/romaiiiinnn/blog-post-image-converter
 Project-URL: Bug Tracker, https://gitlab.com/romaiiiinnn/blog-post-image-converter/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: Environment :: Console
@@ -44,17 +44,19 @@
 ```console
 Usage: bloic [OPTIONS] IMAGE_PATH
 
   Resizes an image based on a target width passed as a parameter, then
   converts it to the WebP format.
 
 Options:
+  --version                   Show the version and exit.
   -w, --width INTEGER RANGE   Target width of the image  [default: 1200; x>0]
   -o, --output-dir DIRECTORY  Output directory  [default: .]
   -d, --delete                Delete source image after conversion.
+  --help                      Show this message and exit.
 ```
 
 ### Examples
 
 Follwing command will create image named `image.webp` with a width of 1200px in current directory.
 
 #### With installed package
```

### Comparing `bloic-1.0.0/pyproject.toml` & `bloic-1.0.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -11,25 +11,26 @@
     { name = "romaiiiiinnn" }
 ]
 description = "Tool to convert and resize image for blog post."
 readme = "README.md"
 license = {text = "MIT"}
 requires-python = ">=3.11"
 dependencies = [
-    "click==8.1.3"
+    "click==8.1.3",
+    "Pillow==9.5.0"
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
     "Environment :: Console",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Topic :: Utilities",
 ]
 [project.scripts]
-bloic = "bloic.entrypoint:check_ratio"
+bloic = "bloic.entrypoint:resize_image"
 
 [project.urls]
 "Homepage" = "https://gitlab.com/romaiiiinnn/blog-post-image-converter"
 "Bug Tracker" = "https://gitlab.com/romaiiiinnn/blog-post-image-converter/-/issues"
 
 [tool.setuptools_scm]
 write_to = "bloic/_version.py"
```

