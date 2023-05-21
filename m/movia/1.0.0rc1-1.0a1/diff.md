# Comparing `tmp/movia-1.0.0rc1.tar.gz` & `tmp/movia-1.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "movia-1.0.0rc1.tar", last modified: Sun May 21 09:19:17 2023, max compression
+gzip compressed data, was "movia-1.0a1.tar", last modified: Mon Mar 13 10:04:13 2023, max compression
```

## Comparing `movia-1.0.0rc1.tar` & `movia-1.0a1.tar`

### file list

```diff
@@ -1,199 +1,114 @@
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-05-21 09:19:17.606709 movia-1.0.0rc1/
--rw-------   0 robin     (1000) robin     (1000)    20796 2023-05-17 13:25:01.000000 movia-1.0.0rc1/.pylintrc
--rw-r--r--   0 robin     (1000) robin     (1000)    34519 2023-03-28 15:30:25.000000 movia-1.0.0rc1/LICENSE
--rw-rw-r--   0 robin     (1000) robin     (1000)     5038 2023-05-21 09:19:17.606709 movia-1.0.0rc1/PKG-INFO
--rw-------   0 robin     (1000) robin     (1000)     3465 2023-05-21 09:04:48.000000 movia-1.0.0rc1/README.rst
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-05-21 09:19:17.410706 movia-1.0.0rc1/cutcutcodec/
--rw-------   0 robin     (1000) robin     (1000)      118 2023-05-21 08:34:12.000000 movia-1.0.0rc1/cutcutcodec/__init__.py
--rw-------   0 robin     (1000) robin     (1000)     1193 2023-05-21 08:14:57.000000 movia-1.0.0rc1/cutcutcodec/__main__.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-05-21 09:19:17.410706 movia-1.0.0rc1/cutcutcodec/core/
--rw-------   0 robin     (1000) robin     (1000)       23 2023-03-28 15:30:31.000000 movia-1.0.0rc1/cutcutcodec/core/__init__.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-05-21 09:19:17.414706 movia-1.0.0rc1/cutcutcodec/core/analysis/
--rw-------   0 robin     (1000) robin     (1000)       23 2023-03-28 15:30:31.000000 movia-1.0.0rc1/cutcutcodec/core/analysis/__init__.py
--rw-------   0 robin     (1000) robin     (1000)     1715 2023-05-21 08:14:53.000000 movia-1.0.0rc1/cutcutcodec/core/analysis/_helper_properties.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-05-21 09:19:17.414706 movia-1.0.0rc1/cutcutcodec/core/analysis/audio/
--rw-rw-r--   0 robin     (1000) robin     (1000)       23 2023-04-10 08:12:25.000000 movia-1.0.0rc1/cutcutcodec/core/analysis/audio/__init__.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-05-21 09:19:17.414706 movia-1.0.0rc1/cutcutcodec/core/analysis/audio/properties/
--rw-rw-r--   0 robin     (1000) robin     (1000)       23 2023-04-10 08:13:07.000000 movia-1.0.0rc1/cutcutcodec/core/analysis/audio/properties/__init__.py
--rw-rw-r--   0 robin     (1000) robin     (1000)     2607 2023-05-21 08:14:51.000000 movia-1.0.0rc1/cutcutcodec/core/analysis/audio/properties/duration.py
--rw-------   0 robin     (1000) robin     (1000)    23018 2023-05-21 08:14:52.000000 movia-1.0.0rc1/cutcutcodec/core/analysis/ffprobe.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-05-21 09:19:17.418706 movia-1.0.0rc1/cutcutcodec/core/analysis/graph/
--rw-rw-r--   0 robin     (1000) robin     (1000)       23 2023-05-11 12:22:45.000000 movia-1.0.0rc1/cutcutcodec/core/analysis/graph/__init__.py
--rw-rw-r--   0 robin     (1000) robin     (1000)     2982 2023-05-21 08:14:49.000000 movia-1.0.0rc1/cutcutcodec/core/analysis/graph/find.py
--rw-rw-r--   0 robin     (1000) robin     (1000)     2789 2023-05-21 08:14:48.000000 movia-1.0.0rc1/cutcutcodec/core/analysis/graph/time_backprop.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-05-21 09:19:17.418706 movia-1.0.0rc1/cutcutcodec/core/analysis/video/
--rw-------   0 robin     (1000) robin     (1000)       23 2023-03-28 15:30:31.000000 movia-1.0.0rc1/cutcutcodec/core/analysis/video/__init__.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-05-21 09:19:17.426706 movia-1.0.0rc1/cutcutcodec/core/analysis/video/properties/
--rw-------   0 robin     (1000) robin     (1000)       23 2023-03-28 15:30:31.000000 movia-1.0.0rc1/cutcutcodec/core/analysis/video/properties/__init__.py
--rw-------   0 robin     (1000) robin     (1000)     5618 2023-05-21 07:58:02.000000 movia-1.0.0rc1/cutcutcodec/core/analysis/video/properties/duration.py
--rw-------   0 robin     (1000) robin     (1000)     5324 2023-05-21 07:54:33.000000 movia-1.0.0rc1/cutcutcodec/core/analysis/video/properties/nb_frames.py
--rw-------   0 robin     (1000) robin     (1000)     3474 2023-05-21 07:50:05.000000 movia-1.0.0rc1/cutcutcodec/core/analysis/video/properties/rate.py
--rw-------   0 robin     (1000) robin     (1000)     7608 2023-05-21 07:48:12.000000 movia-1.0.0rc1/cutcutcodec/core/analysis/video/properties/timestamps.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-05-21 09:19:17.434706 movia-1.0.0rc1/cutcutcodec/core/classes/
--rw-------   0 robin     (1000) robin     (1000)       23 2023-03-28 15:30:31.000000 movia-1.0.0rc1/cutcutcodec/core/classes/__init__.py
--rw-------   0 robin     (1000) robin     (1000)     1314 2023-05-21 07:45:25.000000 movia-1.0.0rc1/cutcutcodec/core/classes/container.py
--rw-------   0 robin     (1000) robin     (1000)      976 2023-05-21 07:44:30.000000 movia-1.0.0rc1/cutcutcodec/core/classes/filter.py
--rw-------   0 robin     (1000) robin     (1000)     3617 2023-05-21 07:44:19.000000 movia-1.0.0rc1/cutcutcodec/core/classes/frame.py
--rw-------   0 robin     (1000) robin     (1000)     4785 2023-05-21 07:43:53.000000 movia-1.0.0rc1/cutcutcodec/core/classes/frame_audio.py
--rw-------   0 robin     (1000) robin     (1000)    11858 2023-05-21 07:43:45.000000 movia-1.0.0rc1/cutcutcodec/core/classes/frame_video.py
--rw-rw-r--   0 robin     (1000) robin     (1000)     1368 2023-05-21 07:41:10.000000 movia-1.0.0rc1/cutcutcodec/core/classes/meta_filter.py
--rw-------   0 robin     (1000) robin     (1000)     4803 2023-05-21 07:41:06.000000 movia-1.0.0rc1/cutcutcodec/core/classes/node.py
--rw-------   0 robin     (1000) robin     (1000)     6676 2023-05-21 08:36:17.000000 movia-1.0.0rc1/cutcutcodec/core/classes/stream.py
--rw-------   0 robin     (1000) robin     (1000)     4732 2023-05-21 07:41:04.000000 movia-1.0.0rc1/cutcutcodec/core/classes/stream_audio.py
--rw-------   0 robin     (1000) robin     (1000)     4542 2023-05-21 08:36:43.000000 movia-1.0.0rc1/cutcutcodec/core/classes/stream_video.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-05-21 09:19:17.458707 movia-1.0.0rc1/cutcutcodec/core/compilation/
--rw-------   0 robin     (1000) robin     (1000)       23 2023-03-28 15:30:31.000000 movia-1.0.0rc1/cutcutcodec/core/compilation/__init__.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-05-21 09:19:17.470707 movia-1.0.0rc1/cutcutcodec/core/compilation/export/
--rw-------   0 robin     (1000) robin     (1000)       23 2023-03-28 15:30:31.000000 movia-1.0.0rc1/cutcutcodec/core/compilation/export/__init__.py
--rw-------   0 robin     (1000) robin     (1000)    29498 2023-05-21 07:40:59.000000 movia-1.0.0rc1/cutcutcodec/core/compilation/export/compatibility.py
--rw-------   0 robin     (1000) robin     (1000)     4530 2023-05-21 07:40:58.000000 movia-1.0.0rc1/cutcutcodec/core/compilation/export/default.py
--rw-------   0 robin     (1000) robin     (1000)     1793 2023-05-21 07:40:58.000000 movia-1.0.0rc1/cutcutcodec/core/compilation/export/encodec.py
--rw-------   0 robin     (1000) robin     (1000)      280 2023-03-28 15:30:31.000000 movia-1.0.0rc1/cutcutcodec/core/compilation/export/muxer.py
--rw-rw-r--   0 robin     (1000) robin     (1000)     3419 2023-05-21 07:40:57.000000 movia-1.0.0rc1/cutcutcodec/core/compilation/export/rate.py
--rw-------   0 robin     (1000) robin     (1000)    17310 2023-05-21 07:41:03.000000 movia-1.0.0rc1/cutcutcodec/core/compilation/graph_to_ast.py
--rw-------   0 robin     (1000) robin     (1000)     2888 2023-05-21 07:41:02.000000 movia-1.0.0rc1/cutcutcodec/core/compilation/graph_to_json.py
--rw-------   0 robin     (1000) robin     (1000)     8095 2023-05-21 08:38:21.000000 movia-1.0.0rc1/cutcutcodec/core/compilation/graph_to_tree.py
--rw-------   0 robin     (1000) robin     (1000)     3981 2023-05-21 07:41:01.000000 movia-1.0.0rc1/cutcutcodec/core/compilation/json_to_graph.py
--rw-rw-r--   0 robin     (1000) robin     (1000)    24456 2023-05-21 07:41:00.000000 movia-1.0.0rc1/cutcutcodec/core/compilation/sympy_to_torch.py
--rw-------   0 robin     (1000) robin     (1000)     5759 2023-05-21 07:40:59.000000 movia-1.0.0rc1/cutcutcodec/core/compilation/tree_to_graph.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-05-21 09:19:17.470707 movia-1.0.0rc1/cutcutcodec/core/edit/
--rw-------   0 robin     (1000) robin     (1000)      216 2023-03-28 15:30:31.000000 movia-1.0.0rc1/cutcutcodec/core/edit/__init__.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-05-21 09:19:17.474707 movia-1.0.0rc1/cutcutcodec/core/edit/operation/
--rw-------   0 robin     (1000) robin     (1000)      158 2023-03-28 15:30:31.000000 movia-1.0.0rc1/cutcutcodec/core/edit/operation/__init__.py
--rw-------   0 robin     (1000) robin     (1000)     2368 2023-05-21 07:40:56.000000 movia-1.0.0rc1/cutcutcodec/core/edit/operation/add.py
--rw-------   0 robin     (1000) robin     (1000)    22705 2023-05-21 07:40:56.000000 movia-1.0.0rc1/cutcutcodec/core/edit/operation/remove.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-05-21 09:19:17.474707 movia-1.0.0rc1/cutcutcodec/core/edit/resource_estimation/
--rw-------   0 robin     (1000) robin     (1000)       23 2023-03-28 15:30:31.000000 movia-1.0.0rc1/cutcutcodec/core/edit/resource_estimation/__init__.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-05-21 09:19:17.474707 movia-1.0.0rc1/cutcutcodec/core/edit/simplify/
--rw-------   0 robin     (1000) robin     (1000)       23 2023-03-28 15:30:31.000000 movia-1.0.0rc1/cutcutcodec/core/edit/simplify/__init__.py
--rw-------   0 robin     (1000) robin     (1000)     1515 2023-05-21 08:35:27.000000 movia-1.0.0rc1/cutcutcodec/core/exceptions.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-05-21 09:19:17.482707 movia-1.0.0rc1/cutcutcodec/core/filters/
--rw-------   0 robin     (1000) robin     (1000)       23 2023-03-28 15:30:31.000000 movia-1.0.0rc1/cutcutcodec/core/filters/__init__.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-05-21 09:19:17.486707 movia-1.0.0rc1/cutcutcodec/core/filters/basic/
--rw-------   0 robin     (1000) robin     (1000)       23 2023-03-28 15:30:31.000000 movia-1.0.0rc1/cutcutcodec/core/filters/basic/__init__.py
--rw-rw-r--   0 robin     (1000) robin     (1000)    19937 2023-05-21 08:39:49.000000 movia-1.0.0rc1/cutcutcodec/core/filters/basic/add.py
--rw-rw-r--   0 robin     (1000) robin     (1000)     2742 2023-05-21 07:40:55.000000 movia-1.0.0rc1/cutcutcodec/core/filters/basic/chain.py
--rw-rw-r--   0 robin     (1000) robin     (1000)     9916 2023-05-21 07:40:54.000000 movia-1.0.0rc1/cutcutcodec/core/filters/basic/cut.py
--rw-rw-r--   0 robin     (1000) robin     (1000)     1527 2023-05-21 07:40:54.000000 movia-1.0.0rc1/cutcutcodec/core/filters/basic/identity.py
--rw-rw-r--   0 robin     (1000) robin     (1000)     5175 2023-05-21 07:40:53.000000 movia-1.0.0rc1/cutcutcodec/core/filters/basic/resize.py
--rw-------   0 robin     (1000) robin     (1000)     4413 2023-05-21 07:40:53.000000 movia-1.0.0rc1/cutcutcodec/core/filters/basic/translate.py
--rw-------   0 robin     (1000) robin     (1000)     3308 2023-05-21 07:40:53.000000 movia-1.0.0rc1/cutcutcodec/core/filters/basic/truncate.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-05-21 09:19:17.486707 movia-1.0.0rc1/cutcutcodec/core/generation/
--rw-------   0 robin     (1000) robin     (1000)       23 2023-03-28 15:30:31.000000 movia-1.0.0rc1/cutcutcodec/core/generation/__init__.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-05-21 09:19:17.498707 movia-1.0.0rc1/cutcutcodec/core/generation/audio/
--rw-------   0 robin     (1000) robin     (1000)       23 2023-03-28 15:30:31.000000 movia-1.0.0rc1/cutcutcodec/core/generation/audio/__init__.py
--rw-------   0 robin     (1000) robin     (1000)     2176 2023-05-21 07:40:52.000000 movia-1.0.0rc1/cutcutcodec/core/generation/audio/empty.py
--rw-rw-r--   0 robin     (1000) robin     (1000)     5552 2023-05-21 07:40:52.000000 movia-1.0.0rc1/cutcutcodec/core/generation/audio/equation.py
--rw-------   0 robin     (1000) robin     (1000)     9198 2023-05-21 07:40:51.000000 movia-1.0.0rc1/cutcutcodec/core/generation/audio/noise.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-05-21 09:19:17.502707 movia-1.0.0rc1/cutcutcodec/core/generation/video/
--rw-------   0 robin     (1000) robin     (1000)       23 2023-03-28 15:30:31.000000 movia-1.0.0rc1/cutcutcodec/core/generation/video/__init__.py
--rw-------   0 robin     (1000) robin     (1000)     2068 2023-05-21 07:40:51.000000 movia-1.0.0rc1/cutcutcodec/core/generation/video/empty.py
--rw-------   0 robin     (1000) robin     (1000)    10051 2023-05-21 07:40:50.000000 movia-1.0.0rc1/cutcutcodec/core/generation/video/equation.py
--rw-------   0 robin     (1000) robin     (1000)     3758 2023-05-21 07:40:50.000000 movia-1.0.0rc1/cutcutcodec/core/generation/video/noise.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-05-21 09:19:17.506707 movia-1.0.0rc1/cutcutcodec/core/interfaces/
--rw-rw-r--   0 robin     (1000) robin     (1000)       23 2023-05-09 07:53:03.000000 movia-1.0.0rc1/cutcutcodec/core/interfaces/__init__.py
--rw-rw-r--   0 robin     (1000) robin     (1000)     2508 2023-05-21 07:40:49.000000 movia-1.0.0rc1/cutcutcodec/core/interfaces/seedable.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-05-21 09:19:17.510707 movia-1.0.0rc1/cutcutcodec/core/io/
--rw-------   0 robin     (1000) robin     (1000)       23 2023-03-28 15:30:31.000000 movia-1.0.0rc1/cutcutcodec/core/io/__init__.py
--rw-------   0 robin     (1000) robin     (1000)    30890 2023-05-21 07:40:49.000000 movia-1.0.0rc1/cutcutcodec/core/io/read.py
--rw-rw-r--   0 robin     (1000) robin     (1000)    12886 2023-05-21 07:40:48.000000 movia-1.0.0rc1/cutcutcodec/core/io/scheduler.py
--rw-------   0 robin     (1000) robin     (1000)    14332 2023-05-21 07:40:48.000000 movia-1.0.0rc1/cutcutcodec/core/io/write.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-05-21 09:19:17.510707 movia-1.0.0rc1/cutcutcodec/core/optimisation/
--rw-------   0 robin     (1000) robin     (1000)       23 2023-03-28 15:30:31.000000 movia-1.0.0rc1/cutcutcodec/core/optimisation/__init__.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-05-21 09:19:17.514707 movia-1.0.0rc1/cutcutcodec/core/optimisation/cache/
--rw-------   0 robin     (1000) robin     (1000)       23 2023-03-28 15:30:31.000000 movia-1.0.0rc1/cutcutcodec/core/optimisation/cache/__init__.py
--rw-------   0 robin     (1000) robin     (1000)      853 2023-05-21 07:40:47.000000 movia-1.0.0rc1/cutcutcodec/core/optimisation/cache/basic.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-05-21 09:19:17.518708 movia-1.0.0rc1/cutcutcodec/core/optimisation/cache/clean/
--rw-rw-r--   0 robin     (1000) robin     (1000)       23 2023-05-11 05:59:15.000000 movia-1.0.0rc1/cutcutcodec/core/optimisation/cache/clean/__init__.py
--rw-rw-r--   0 robin     (1000) robin     (1000)     3305 2023-05-21 07:40:47.000000 movia-1.0.0rc1/cutcutcodec/core/optimisation/cache/clean/graph.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-05-21 09:19:17.518708 movia-1.0.0rc1/cutcutcodec/core/optimisation/cache/hashes/
--rw-rw-r--   0 robin     (1000) robin     (1000)       23 2023-05-11 05:54:50.000000 movia-1.0.0rc1/cutcutcodec/core/optimisation/cache/hashes/__init__.py
--rw-------   0 robin     (1000) robin     (1000)     3401 2023-05-21 07:40:46.000000 movia-1.0.0rc1/cutcutcodec/core/optimisation/cache/hashes/graph.py
--rw-------   0 robin     (1000) robin     (1000)     1202 2023-05-21 07:40:47.000000 movia-1.0.0rc1/cutcutcodec/core/optimisation/cache/singleton.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-05-21 09:19:17.518708 movia-1.0.0rc1/cutcutcodec/core/optimisation/cuda/
--rw-------   0 robin     (1000) robin     (1000)       23 2023-03-28 15:30:31.000000 movia-1.0.0rc1/cutcutcodec/core/optimisation/cuda/__init__.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-05-21 09:19:17.530708 movia-1.0.0rc1/cutcutcodec/core/optimisation/parallel/
--rw-rw-r--   0 robin     (1000) robin     (1000)       23 2023-04-08 09:51:10.000000 movia-1.0.0rc1/cutcutcodec/core/optimisation/parallel/__init__.py
--rw-rw-r--   0 robin     (1000) robin     (1000)     2460 2023-05-21 07:40:46.000000 movia-1.0.0rc1/cutcutcodec/core/optimisation/parallel/buffer.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-05-21 09:19:17.538708 movia-1.0.0rc1/cutcutcodec/gui/
--rw-r--r--   0 robin     (1000) robin     (1000)       23 2023-03-28 15:30:31.000000 movia-1.0.0rc1/cutcutcodec/gui/__init__.py
--rw-------   0 robin     (1000) robin     (1000)     1236 2023-05-21 07:40:45.000000 movia-1.0.0rc1/cutcutcodec/gui/__main__.py
--rw-------   0 robin     (1000) robin     (1000)     2594 2023-05-10 18:03:44.000000 movia-1.0.0rc1/cutcutcodec/gui/actions.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-05-21 09:19:17.538708 movia-1.0.0rc1/cutcutcodec/gui/app/
--rw-r--r--   0 robin     (1000) robin     (1000)       23 2023-03-28 15:30:31.000000 movia-1.0.0rc1/cutcutcodec/gui/app/__init__.py
--rw-------   0 robin     (1000) robin     (1000)    10536 2023-05-21 07:40:43.000000 movia-1.0.0rc1/cutcutcodec/gui/app/app.py
--rw-------   0 robin     (1000) robin     (1000)     1855 2023-05-21 08:42:32.000000 movia-1.0.0rc1/cutcutcodec/gui/base.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-05-21 09:19:17.546708 movia-1.0.0rc1/cutcutcodec/gui/edit_node_state/
--rw-------   0 robin     (1000) robin     (1000)      134 2023-03-28 15:30:31.000000 movia-1.0.0rc1/cutcutcodec/gui/edit_node_state/__init__.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-05-21 09:19:17.558708 movia-1.0.0rc1/cutcutcodec/gui/edit_node_state/all/
--rw-------   0 robin     (1000) robin     (1000)       23 2023-03-28 15:30:31.000000 movia-1.0.0rc1/cutcutcodec/gui/edit_node_state/all/__init__.py
--rw-------   0 robin     (1000) robin     (1000)     3025 2023-05-21 07:40:40.000000 movia-1.0.0rc1/cutcutcodec/gui/edit_node_state/all/container_input_ffmpeg.py
--rw-rw-r--   0 robin     (1000) robin     (1000)     3293 2023-05-21 07:40:40.000000 movia-1.0.0rc1/cutcutcodec/gui/edit_node_state/all/filter_cut.py
--rw-------   0 robin     (1000) robin     (1000)     1691 2023-05-21 07:40:40.000000 movia-1.0.0rc1/cutcutcodec/gui/edit_node_state/all/filter_translate.py
--rw-------   0 robin     (1000) robin     (1000)     1648 2023-05-21 07:40:39.000000 movia-1.0.0rc1/cutcutcodec/gui/edit_node_state/all/filter_truncate.py
--rw-rw-r--   0 robin     (1000) robin     (1000)     3377 2023-05-21 07:40:39.000000 movia-1.0.0rc1/cutcutcodec/gui/edit_node_state/all/generator_audio_equation.py
--rw-------   0 robin     (1000) robin     (1000)      720 2023-05-21 07:40:39.000000 movia-1.0.0rc1/cutcutcodec/gui/edit_node_state/all/generator_audio_noise.py
--rw-------   0 robin     (1000) robin     (1000)     3492 2023-05-21 07:40:39.000000 movia-1.0.0rc1/cutcutcodec/gui/edit_node_state/all/generator_video_equation.py
--rw-------   0 robin     (1000) robin     (1000)      713 2023-05-21 07:40:39.000000 movia-1.0.0rc1/cutcutcodec/gui/edit_node_state/all/generator_video_noise.py
--rw-------   0 robin     (1000) robin     (1000)     3035 2023-05-21 08:41:44.000000 movia-1.0.0rc1/cutcutcodec/gui/edit_node_state/base.py
--rw-------   0 robin     (1000) robin     (1000)      962 2023-05-21 07:40:42.000000 movia-1.0.0rc1/cutcutcodec/gui/edit_node_state/default.py
--rw-------   0 robin     (1000) robin     (1000)     1596 2023-05-21 07:40:42.000000 movia-1.0.0rc1/cutcutcodec/gui/edit_node_state/documentation.py
--rw-------   0 robin     (1000) robin     (1000)     3164 2023-05-21 07:40:42.000000 movia-1.0.0rc1/cutcutcodec/gui/edit_node_state/general.py
--rw-------   0 robin     (1000) robin     (1000)     1825 2023-05-21 07:40:41.000000 movia-1.0.0rc1/cutcutcodec/gui/edit_node_state/interface.py
--rw-------   0 robin     (1000) robin     (1000)     1542 2023-05-21 07:40:41.000000 movia-1.0.0rc1/cutcutcodec/gui/edit_node_state/loader.py
--rw-------   0 robin     (1000) robin     (1000)     2532 2023-05-21 08:41:26.000000 movia-1.0.0rc1/cutcutcodec/gui/edit_node_state/main.py
--rw-------   0 robin     (1000) robin     (1000)     1138 2023-05-21 08:41:50.000000 movia-1.0.0rc1/cutcutcodec/gui/edition_tabs.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-05-21 09:19:17.566708 movia-1.0.0rc1/cutcutcodec/gui/entry/
--rw-------   0 robin     (1000) robin     (1000)       23 2023-03-28 15:30:31.000000 movia-1.0.0rc1/cutcutcodec/gui/entry/__init__.py
--rw-------   0 robin     (1000) robin     (1000)     4581 2023-05-21 08:44:34.000000 movia-1.0.0rc1/cutcutcodec/gui/entry/base.py
--rw-------   0 robin     (1000) robin     (1000)      412 2023-05-21 07:40:38.000000 movia-1.0.0rc1/cutcutcodec/gui/entry/filters.py
--rw-------   0 robin     (1000) robin     (1000)      539 2023-05-21 07:40:38.000000 movia-1.0.0rc1/cutcutcodec/gui/entry/generators.py
--rw-------   0 robin     (1000) robin     (1000)     4065 2023-05-21 07:40:38.000000 movia-1.0.0rc1/cutcutcodec/gui/entry/project_files.py
--rw-------   0 robin     (1000) robin     (1000)     1366 2023-05-21 08:41:49.000000 movia-1.0.0rc1/cutcutcodec/gui/entry_tabs.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-05-21 09:19:17.578709 movia-1.0.0rc1/cutcutcodec/gui/export/
--rw-------   0 robin     (1000) robin     (1000)       23 2023-03-28 15:30:31.000000 movia-1.0.0rc1/cutcutcodec/gui/export/__init__.py
--rw-rw-r--   0 robin     (1000) robin     (1000)     1772 2023-05-21 08:41:22.000000 movia-1.0.0rc1/cutcutcodec/gui/export/_helper.py
--rw-rw-r--   0 robin     (1000) robin     (1000)     8285 2023-05-21 08:41:20.000000 movia-1.0.0rc1/cutcutcodec/gui/export/container.py
--rw-rw-r--   0 robin     (1000) robin     (1000)     1379 2023-05-21 08:41:18.000000 movia-1.0.0rc1/cutcutcodec/gui/export/doc.py
--rw-rw-r--   0 robin     (1000) robin     (1000)     8335 2023-05-21 08:41:17.000000 movia-1.0.0rc1/cutcutcodec/gui/export/encodec.py
--rw-rw-r--   0 robin     (1000) robin     (1000)     5270 2023-05-21 08:41:15.000000 movia-1.0.0rc1/cutcutcodec/gui/export/main.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-05-21 09:19:17.582708 movia-1.0.0rc1/cutcutcodec/gui/graph/
--rw-------   0 robin     (1000) robin     (1000)       23 2023-03-28 15:30:31.000000 movia-1.0.0rc1/cutcutcodec/gui/graph/__init__.py
--rw-------   0 robin     (1000) robin     (1000)     5767 2023-05-21 08:41:13.000000 movia-1.0.0rc1/cutcutcodec/gui/graph/edge_properties.py
--rw-------   0 robin     (1000) robin     (1000)    20225 2023-05-21 08:45:00.000000 movia-1.0.0rc1/cutcutcodec/gui/graph/graph_editor.py
--rw-------   0 robin     (1000) robin     (1000)     8784 2023-05-21 07:40:36.000000 movia-1.0.0rc1/cutcutcodec/gui/graph/layout.py
--rw-------   0 robin     (1000) robin     (1000)     5475 2023-05-21 08:41:47.000000 movia-1.0.0rc1/cutcutcodec/gui/main.py
--rw-------   0 robin     (1000) robin     (1000)      720 2023-05-10 17:44:50.000000 movia-1.0.0rc1/cutcutcodec/gui/menu.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-05-21 09:19:17.582708 movia-1.0.0rc1/cutcutcodec/gui/preferences/
--rw-rw-r--   0 robin     (1000) robin     (1000)       23 2023-05-10 17:33:08.000000 movia-1.0.0rc1/cutcutcodec/gui/preferences/__init__.py
--rw-rw-r--   0 robin     (1000) robin     (1000)     7509 2023-05-21 08:41:11.000000 movia-1.0.0rc1/cutcutcodec/gui/preferences/audio_settings.py
--rw-rw-r--   0 robin     (1000) robin     (1000)     1330 2023-05-21 08:41:09.000000 movia-1.0.0rc1/cutcutcodec/gui/preferences/main.py
--rw-rw-r--   0 robin     (1000) robin     (1000)     7997 2023-05-21 08:41:08.000000 movia-1.0.0rc1/cutcutcodec/gui/preferences/video_settings.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-05-21 09:19:17.586709 movia-1.0.0rc1/cutcutcodec/gui/timeline/
--rw-------   0 robin     (1000) robin     (1000)       23 2023-03-28 15:30:31.000000 movia-1.0.0rc1/cutcutcodec/gui/timeline/__init__.py
--rw-rw-r--   0 robin     (1000) robin     (1000)      850 2023-05-21 08:41:06.000000 movia-1.0.0rc1/cutcutcodec/gui/timeline/main.py
--rw-rw-r--   0 robin     (1000) robin     (1000)    10202 2023-05-21 08:41:05.000000 movia-1.0.0rc1/cutcutcodec/gui/timeline/slider.py
--rw-rw-r--   0 robin     (1000) robin     (1000)     2650 2023-05-21 08:41:04.000000 movia-1.0.0rc1/cutcutcodec/gui/timeline/tracks.py
--rw-------   0 robin     (1000) robin     (1000)      741 2023-05-21 08:41:46.000000 movia-1.0.0rc1/cutcutcodec/gui/toolbar.py
--rw-------   0 robin     (1000) robin     (1000)      606 2023-03-28 15:30:31.000000 movia-1.0.0rc1/cutcutcodec/gui/tools.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-05-21 09:19:17.594709 movia-1.0.0rc1/cutcutcodec/gui/video_preview/
--rw-rw-r--   0 robin     (1000) robin     (1000)       23 2023-05-07 06:02:12.000000 movia-1.0.0rc1/cutcutcodec/gui/video_preview/__init__.py
--rw-rw-r--   0 robin     (1000) robin     (1000)     3817 2023-05-21 07:40:35.000000 movia-1.0.0rc1/cutcutcodec/gui/video_preview/audio_player.py
--rw-rw-r--   0 robin     (1000) robin     (1000)     3948 2023-05-21 08:41:03.000000 movia-1.0.0rc1/cutcutcodec/gui/video_preview/control.py
--rw-rw-r--   0 robin     (1000) robin     (1000)    10532 2023-05-21 08:41:01.000000 movia-1.0.0rc1/cutcutcodec/gui/video_preview/frame_extractor.py
--rw-rw-r--   0 robin     (1000) robin     (1000)     4716 2023-05-21 08:40:59.000000 movia-1.0.0rc1/cutcutcodec/gui/video_preview/main.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-05-21 09:19:17.598709 movia-1.0.0rc1/cutcutcodec/testing/
--rw-------   0 robin     (1000) robin     (1000)      171 2023-05-21 07:40:34.000000 movia-1.0.0rc1/cutcutcodec/testing/__init__.py
--rwx--x--x   0 robin     (1000) robin     (1000)      232 2023-05-21 07:40:34.000000 movia-1.0.0rc1/cutcutcodec/testing/__main__.py
--rw-------   0 robin     (1000) robin     (1000)     1720 2023-05-21 08:45:26.000000 movia-1.0.0rc1/cutcutcodec/testing/generation.py
--rw-------   0 robin     (1000) robin     (1000)     1517 2023-05-21 07:40:34.000000 movia-1.0.0rc1/cutcutcodec/testing/runtests.py
--rw-------   0 robin     (1000) robin     (1000)      569 2023-05-21 08:14:55.000000 movia-1.0.0rc1/cutcutcodec/utils.py
-drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-05-21 09:19:17.606709 movia-1.0.0rc1/movia.egg-info/
--rw-rw-r--   0 robin     (1000) robin     (1000)     5038 2023-05-21 09:19:17.000000 movia-1.0.0rc1/movia.egg-info/PKG-INFO
--rw-rw-r--   0 robin     (1000) robin     (1000)     6215 2023-05-21 09:19:17.000000 movia-1.0.0rc1/movia.egg-info/SOURCES.txt
--rw-rw-r--   0 robin     (1000) robin     (1000)        1 2023-05-21 09:19:17.000000 movia-1.0.0rc1/movia.egg-info/dependency_links.txt
--rw-rw-r--   0 robin     (1000) robin     (1000)      173 2023-05-21 09:19:17.000000 movia-1.0.0rc1/movia.egg-info/entry_points.txt
--rw-rw-r--   0 robin     (1000) robin     (1000)      204 2023-05-21 09:19:17.000000 movia-1.0.0rc1/movia.egg-info/requires.txt
--rw-rw-r--   0 robin     (1000) robin     (1000)       12 2023-05-21 09:19:17.000000 movia-1.0.0rc1/movia.egg-info/top_level.txt
--rw-rw-r--   0 robin     (1000) robin     (1000)       38 2023-05-21 09:19:17.606709 movia-1.0.0rc1/setup.cfg
--rw-------   0 robin     (1000) robin     (1000)     3878 2023-05-21 09:18:53.000000 movia-1.0.0rc1/setup.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-03-13 10:04:13.899839 movia-1.0a1/
+-rw-r--r--   0 robin     (1000) robin     (1000)    34519 2022-12-05 11:30:47.000000 movia-1.0a1/LICENSE
+-rw-rw-r--   0 robin     (1000) robin     (1000)     4113 2023-03-13 10:04:13.895839 movia-1.0a1/PKG-INFO
+-rw-------   0 robin     (1000) robin     (1000)     2466 2023-03-12 23:41:34.000000 movia-1.0a1/README.rst
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-03-13 10:04:13.771842 movia-1.0a1/movia/
+-rw-r--r--   0 robin     (1000) robin     (1000)      115 2023-03-13 09:57:14.000000 movia-1.0a1/movia/__init__.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     1268 2023-03-06 22:24:38.000000 movia-1.0a1/movia/__main__.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-03-13 10:04:13.779842 movia-1.0a1/movia/core/
+-rw-r--r--   0 robin     (1000) robin     (1000)       23 2022-12-05 11:30:20.000000 movia-1.0a1/movia/core/__init__.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-03-13 10:04:13.783842 movia-1.0a1/movia/core/analysis/
+-rw-r--r--   0 robin     (1000) robin     (1000)       23 2022-12-05 11:30:34.000000 movia-1.0a1/movia/core/analysis/__init__.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     2970 2023-02-21 21:31:11.000000 movia-1.0a1/movia/core/analysis/streams.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-03-13 10:04:13.783842 movia-1.0a1/movia/core/analysis/video/
+-rw-r--r--   0 robin     (1000) robin     (1000)       23 2022-12-05 11:30:29.000000 movia-1.0a1/movia/core/analysis/video/__init__.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-03-13 10:04:13.795842 movia-1.0a1/movia/core/analysis/video/properties/
+-rw-r--r--   0 robin     (1000) robin     (1000)       23 2022-12-05 11:30:29.000000 movia-1.0a1/movia/core/analysis/video/properties/__init__.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     5958 2023-01-15 15:56:54.000000 movia-1.0a1/movia/core/analysis/video/properties/duration.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     4115 2023-03-11 16:13:19.000000 movia-1.0a1/movia/core/analysis/video/properties/framerate.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     5152 2023-01-15 15:56:50.000000 movia-1.0a1/movia/core/analysis/video/properties/nb_frames.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     3827 2023-01-15 15:56:48.000000 movia-1.0a1/movia/core/analysis/video/properties/parser.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    14907 2023-01-15 15:56:46.000000 movia-1.0a1/movia/core/analysis/video/properties/timestamps.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-03-13 10:04:13.799841 movia-1.0a1/movia/core/classes/
+-rw-r--r--   0 robin     (1000) robin     (1000)       23 2022-12-05 11:30:20.000000 movia-1.0a1/movia/core/classes/__init__.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     1302 2023-03-10 08:40:10.000000 movia-1.0a1/movia/core/classes/container.py
+-rw-r--r--   0 robin     (1000) robin     (1000)      965 2023-02-10 08:33:37.000000 movia-1.0a1/movia/core/classes/filter.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     4228 2023-02-10 12:27:07.000000 movia-1.0a1/movia/core/classes/node.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     5006 2023-03-04 13:32:43.000000 movia-1.0a1/movia/core/classes/stream.py
+-rw-------   0 robin     (1000) robin     (1000)     4166 2023-03-04 13:08:40.000000 movia-1.0a1/movia/core/classes/stream_audio.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     4133 2023-03-04 13:09:02.000000 movia-1.0a1/movia/core/classes/stream_video.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-03-13 10:04:13.807841 movia-1.0a1/movia/core/compilation/
+-rw-r--r--   0 robin     (1000) robin     (1000)       23 2022-12-05 11:30:27.000000 movia-1.0a1/movia/core/compilation/__init__.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-03-13 10:04:13.811841 movia-1.0a1/movia/core/compilation/export/
+-rw-rw-r--   0 robin     (1000) robin     (1000)       23 2023-03-11 15:36:53.000000 movia-1.0a1/movia/core/compilation/export/__init__.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    30589 2023-03-12 17:52:58.000000 movia-1.0a1/movia/core/compilation/export/compatibility.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     4357 2023-03-12 18:30:42.000000 movia-1.0a1/movia/core/compilation/export/default.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)      653 2023-03-12 18:25:54.000000 movia-1.0a1/movia/core/compilation/export/encodec.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)      280 2023-03-12 18:01:03.000000 movia-1.0a1/movia/core/compilation/export/muxer.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)      986 2023-03-12 18:53:47.000000 movia-1.0a1/movia/core/compilation/export/rate_audio.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     1124 2023-03-12 16:32:11.000000 movia-1.0a1/movia/core/compilation/export/rate_video.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)    15006 2023-03-12 16:11:46.000000 movia-1.0a1/movia/core/compilation/graph_to_ast.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     7842 2023-03-11 15:20:27.000000 movia-1.0a1/movia/core/compilation/graph_to_tree.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     5343 2023-03-08 17:30:41.000000 movia-1.0a1/movia/core/compilation/tree_to_graph.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-03-13 10:04:13.811841 movia-1.0a1/movia/core/edit/
+-rw-r--r--   0 robin     (1000) robin     (1000)      216 2023-02-03 16:32:38.000000 movia-1.0a1/movia/core/edit/__init__.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-03-13 10:04:13.815841 movia-1.0a1/movia/core/edit/operation/
+-rw-rw-r--   0 robin     (1000) robin     (1000)      158 2023-02-03 16:34:25.000000 movia-1.0a1/movia/core/edit/operation/__init__.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     2362 2023-03-06 22:29:20.000000 movia-1.0a1/movia/core/edit/operation/add.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)    22507 2023-03-06 22:37:35.000000 movia-1.0a1/movia/core/edit/operation/remove.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     1273 2023-01-07 17:41:19.000000 movia-1.0a1/movia/core/exceptions.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-03-13 10:04:13.815841 movia-1.0a1/movia/core/filters/
+-rw-r--r--   0 robin     (1000) robin     (1000)       23 2022-12-05 11:30:18.000000 movia-1.0a1/movia/core/filters/__init__.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-03-13 10:04:13.819841 movia-1.0a1/movia/core/filters/basic/
+-rw-r--r--   0 robin     (1000) robin     (1000)       23 2022-12-05 11:30:18.000000 movia-1.0a1/movia/core/filters/basic/__init__.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     4621 2023-03-10 21:57:08.000000 movia-1.0a1/movia/core/filters/basic/truncate.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-03-13 10:04:13.819841 movia-1.0a1/movia/core/generation/
+-rw-r--r--   0 robin     (1000) robin     (1000)       23 2022-12-05 11:30:27.000000 movia-1.0a1/movia/core/generation/__init__.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-03-13 10:04:13.823841 movia-1.0a1/movia/core/generation/audio/
+-rw-rw-r--   0 robin     (1000) robin     (1000)       23 2023-01-09 19:53:13.000000 movia-1.0a1/movia/core/generation/audio/__init__.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     2021 2023-02-15 15:34:59.000000 movia-1.0a1/movia/core/generation/audio/empty.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     3040 2023-02-15 15:35:27.000000 movia-1.0a1/movia/core/generation/audio/noise.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-03-13 10:04:13.831841 movia-1.0a1/movia/core/generation/video/
+-rw-r--r--   0 robin     (1000) robin     (1000)       23 2022-12-05 11:30:25.000000 movia-1.0a1/movia/core/generation/video/__init__.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     2142 2023-02-15 15:22:43.000000 movia-1.0a1/movia/core/generation/video/empty.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    12941 2023-02-16 08:56:25.000000 movia-1.0a1/movia/core/generation/video/equation.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     4592 2023-02-16 08:56:38.000000 movia-1.0a1/movia/core/generation/video/noise.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-03-13 10:04:13.835841 movia-1.0a1/movia/core/io/
+-rw-r--r--   0 robin     (1000) robin     (1000)       23 2022-12-05 11:30:23.000000 movia-1.0a1/movia/core/io/__init__.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    29782 2023-02-15 15:39:40.000000 movia-1.0a1/movia/core/io/read.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    20239 2023-03-12 13:20:11.000000 movia-1.0a1/movia/core/io/write.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-03-13 10:04:13.843840 movia-1.0a1/movia/gui/
+-rw-r--r--   0 robin     (1000) robin     (1000)       23 2022-12-05 11:30:41.000000 movia-1.0a1/movia/gui/__init__.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     1461 2023-02-15 17:07:40.000000 movia-1.0a1/movia/gui/actions.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-03-13 10:04:13.847840 movia-1.0a1/movia/gui/app/
+-rw-r--r--   0 robin     (1000) robin     (1000)       23 2022-12-05 11:30:41.000000 movia-1.0a1/movia/gui/app/__init__.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     6958 2023-03-12 17:17:41.000000 movia-1.0a1/movia/gui/app/app.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     1750 2023-02-09 20:52:27.000000 movia-1.0a1/movia/gui/base.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     1033 2023-02-02 14:45:30.000000 movia-1.0a1/movia/gui/edition_tabs.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-03-13 10:04:13.867840 movia-1.0a1/movia/gui/entry/
+-rw-rw-r--   0 robin     (1000) robin     (1000)       23 2023-02-09 20:40:42.000000 movia-1.0a1/movia/gui/entry/__init__.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     4716 2023-03-12 23:54:04.000000 movia-1.0a1/movia/gui/entry/base.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)      386 2023-02-10 13:26:10.000000 movia-1.0a1/movia/gui/entry/filters.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)      527 2023-02-11 06:51:40.000000 movia-1.0a1/movia/gui/entry/generators.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     3948 2023-02-21 21:36:32.000000 movia-1.0a1/movia/gui/entry/project_files.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     1330 2023-02-10 08:16:32.000000 movia-1.0a1/movia/gui/entry_tabs.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-03-13 10:04:13.867840 movia-1.0a1/movia/gui/export/
+-rw-rw-r--   0 robin     (1000) robin     (1000)       23 2023-02-15 16:48:48.000000 movia-1.0a1/movia/gui/export/__init__.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)    26382 2023-03-12 18:51:01.000000 movia-1.0a1/movia/gui/export/settings.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-03-13 10:04:13.875840 movia-1.0a1/movia/gui/graph/
+-rw-rw-r--   0 robin     (1000) robin     (1000)       23 2023-01-14 21:58:00.000000 movia-1.0a1/movia/gui/graph/__init__.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     5056 2023-02-05 22:21:29.000000 movia-1.0a1/movia/gui/graph/edge_properties.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)    20179 2023-02-09 20:03:15.000000 movia-1.0a1/movia/gui/graph/graph_editor.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     8773 2023-03-06 22:37:40.000000 movia-1.0a1/movia/gui/graph/layout.py
+-rw-r--r--   0 robin     (1000) robin     (1000)     3192 2023-02-15 17:06:56.000000 movia-1.0a1/movia/gui/main.py
+-rw-r--r--   0 robin     (1000) robin     (1000)      517 2023-02-15 16:22:54.000000 movia-1.0a1/movia/gui/menu.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-03-13 10:04:13.895839 movia-1.0a1/movia/gui/node_properties/
+-rw-rw-r--   0 robin     (1000) robin     (1000)       23 2023-02-02 09:10:01.000000 movia-1.0a1/movia/gui/node_properties/__init__.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     4624 2023-02-09 20:05:41.000000 movia-1.0a1/movia/gui/node_properties/container_input_ffmpeg.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     2673 2023-03-10 22:20:26.000000 movia-1.0a1/movia/gui/node_properties/filter_truncate.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     4581 2023-02-08 10:19:07.000000 movia-1.0a1/movia/gui/node_properties/generator_video_equation.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)     7206 2023-02-26 23:05:58.000000 movia-1.0a1/movia/gui/node_properties/node_properties.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-03-13 10:04:13.895839 movia-1.0a1/movia/gui/timeline/
+-rw-rw-r--   0 robin     (1000) robin     (1000)       23 2023-01-14 21:57:36.000000 movia-1.0a1/movia/gui/timeline/__init__.py
+-rw-r--r--   0 robin     (1000) robin     (1000)      590 2023-02-15 16:23:21.000000 movia-1.0a1/movia/gui/toolbar.py
+-rw-r--r--   0 robin     (1000) robin     (1000)    16538 2023-03-12 16:39:40.000000 movia-1.0a1/movia/gui/video_viewer.py
+-rw-rw-r--   0 robin     (1000) robin     (1000)      555 2023-02-09 21:09:03.000000 movia-1.0a1/movia/utils.py
+drwxrwxr-x   0 robin     (1000) robin     (1000)        0 2023-03-13 10:04:13.779842 movia-1.0a1/movia.egg-info/
+-rw-rw-r--   0 robin     (1000) robin     (1000)     4113 2023-03-13 10:04:13.000000 movia-1.0a1/movia.egg-info/PKG-INFO
+-rw-rw-r--   0 robin     (1000) robin     (1000)     2809 2023-03-13 10:04:13.000000 movia-1.0a1/movia.egg-info/SOURCES.txt
+-rw-rw-r--   0 robin     (1000) robin     (1000)        1 2023-03-13 10:04:13.000000 movia-1.0a1/movia.egg-info/dependency_links.txt
+-rw-rw-r--   0 robin     (1000) robin     (1000)       46 2023-03-13 10:04:13.000000 movia-1.0a1/movia.egg-info/entry_points.txt
+-rw-rw-r--   0 robin     (1000) robin     (1000)      127 2023-03-13 10:04:13.000000 movia-1.0a1/movia.egg-info/requires.txt
+-rw-rw-r--   0 robin     (1000) robin     (1000)        6 2023-03-13 10:04:13.000000 movia-1.0a1/movia.egg-info/top_level.txt
+-rw-rw-r--   0 robin     (1000) robin     (1000)       38 2023-03-13 10:04:13.899839 movia-1.0a1/setup.cfg
+-rw-r--r--   0 robin     (1000) robin     (1000)     3174 2023-03-13 09:46:20.000000 movia-1.0a1/setup.py
```

### Comparing `movia-1.0.0rc1/LICENSE` & `movia-1.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `movia-1.0.0rc1/README.rst` & `movia-1.0a1/README.rst`

 * *Files 23% similar despite different names*

```diff
@@ -1,77 +1,76 @@
 .. rst syntax: https://deusyss.developpez.com/tutoriels/Python/SphinxDoc/
-.. version conv: https://peps.python.org/pep-0440/
 .. icons: https://specifications.freedesktop.org/icon-naming-spec/latest/ar01s04.html or https://www.pythonguis.com/faq/built-in-qicons-pyqt/
 .. pyqtdoc: https://www.riverbankcomputing.com/static/Docs/PyQt6/
 
-***********
-cutcutcodec
-***********
 
 .. image:: https://github.com/pytest-dev/pytest/workflows/test/badge.svg
     :target: https://github.com/pytest-dev/pytest/actions?query=workflow%3Atest
 
 .. image:: https://img.shields.io/badge/linting-pylint-yellowgreen
     :target: https://github.com/PyCQA/pylint
 
 .. image:: https://img.shields.io/badge/code%20style-black-000000.svg
     :target: https://github.com/psf/black
 
+**************************************
+movia, a light video editing software!
+**************************************
 
 Decsription
 -----------
 
-This software proposes a graphic interface powered by pyqt6 (run ``cutcutcodec-qt``).
-The kernel is written in python and is easily integrated in other projects (module ``cutcutcodec.core``).
+This software proposes a graphic interface powered by pyqt6 (run ``movia``).
+The kernel is written in python and is easily integrated in other projects (module ``movia.core``).
 
 This software is **light**, **fast** and **highly configurable** for the following reasons:
 
 1. Based on ffmpeg, this software supports an incredible number of formats and codecs.
 2. Thanks to operations on the assembly graph, it is able to perform nbr_opti optimization operations.
 3. nbr_tests unit tests ensure an excelent kernel reliability.
 4. Unlike other software that offers a timeline, this one allows you to edit an editing graph. This representation is more general and thus allows a greater flexibility.
 5. A compiled version without graphical interface allows to allocate all the resources of the computer to the export.
 6. This software generates at the time of the export a python code which can be edited. This offers an infinite number of possibilities!
 
-
 Installation
 ------------
 
-cutcutcodec has hard dependency on the pygraphviz library and on the ffmpeg package (version >= 4). You should install it first, please refer to the `pygraphviz installation guide <https://pygraphviz.github.io/documentation/stable/install.html>`_ and according to your Linux distribution, to the `FFmpeg download page <https://ffmpeg.org/download.html>`_.
+Dependencies
+^^^^^^^^^^^^
 
-In many cases, these commands should work:
+* `ffmpeg5 <https://ubuntuhandbook.org/index.php/2022/02/install-ffmpeg-5-0-ubuntu/>`_
 
 .. code:: bash
 
-    $ sudo apt install ffmpeg
-    $ sudo apt install graphviz graphviz-dev
-
-Although it is installed automatically, it is better to install **av** manually to avoid redundancy. Please refer to the `PyAv installation guide <https://pyav.org/docs/develop/overview/installation.html>`_.
+    sudo add-apt-repository ppa:savoury1/ffmpeg4
+    sudo add-apt-repository ppa:savoury1/ffmpeg5
+    sudo apt update
+    sudo apt full-upgrade
+    sudo apt install ffmpeg
 
-In many cases, these commands should work:
+* `pygraphviz <https://pygraphviz.github.io/documentation/stable/install.html>`_
 
 .. code:: bash
 
-    $ sudo apt install libavformat-dev libavcodec-dev libavdevice-dev libavutil-dev libswscale-dev libswresample-dev libavfilter-dev
-    $ pip install av --no-binary av
+    sudo apt install graphviz graphviz-dev pygraphviz
 
-To install cutcutcodec using `PyPI <https://pypi.org/project/cutcutcodec/>`_, run the following command:
+Depos
+^^^^^
 
 .. code:: bash
 
-    $ pip install cutcutcodec[gui]
+    git clone https://framagit.org/robinechuca/movia.git
+    cd movia/
+    python -m pip install -e ./
 
-To install cutcutcodec from `Framagit <https://framagit.org/robinechuca/cutcutcodec>`_ source, clone cutcutcodec using ``git`` and install it using ``pip``.:
+Run
+^^^
 
 .. code:: bash
 
-    git clone https://framagit.org/robinechuca/cutcutcodec.git
-    cd cutcutcodec/
-    pip install -e ./[optional]
-
-In a terminal, simply write the command ``cutcutcodec-qt`` to launch the GUI and the command ``cutcutcodec-test`` for launch the test banchmark.
+    movia
 
 
 What's new ?
 ------------
 
-For the complete list of changes, refer to the `git commits <https://framagit.org/robinechuca/cutcutcodec/-/network/main?ref_type=heads>`_.
+Nothing new for the moment.
```

### Comparing `movia-1.0.0rc1/cutcutcodec/core/analysis/video/properties/duration.py` & `movia-1.0a1/movia/core/analysis/video/properties/duration.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,160 +3,178 @@
 """
 ** Finds the duration of a video stream. **
 -------------------------------------------
 
 This allows not only the characteristics of the files but also the tags if there are any.
 """
 
-from fractions import Fraction
 import collections
 import pathlib
 import typing
 
 import cv2 # pip install opencv-contrib-python-headless
 
-from cutcutcodec.core.analysis._helper_properties import _check_pathexists_index, _mix_and_check
-from cutcutcodec.core.analysis.ffprobe import (_decode_duration_ffmpeg, _estimate_duration_ffmpeg,
-    _map_index_rel_to_abs)
-from cutcutcodec.core.exceptions import MissingStreamError, MissingInformation
+from movia.core.exceptions import MissingStreamError, MissingInformation
+from movia.core.analysis.video.properties.parser import (_check_pathexists_index,
+    _decode_duration_frames_ffmpeg, _mix_and_check, _parse_ffprobe_res)
 
 
 
-def _decode_duration_cv2(filename: str, index: int) -> Fraction:
+def _decode_duration_ffmpeg(filename: str, index: int) -> float:
     """
     ** Extract the duration by the complete decoding of the stream. **
 
     Slow but 100% accurate method.
 
     Examples
     --------
-    >>> from cutcutcodec.core.analysis.video.properties.duration import _decode_duration_cv2
-    >>> _decode_duration_cv2("cutcutcodec/examples/video.mp4", 0)
-    Fraction(16, 1)
+    >>> from movia.core.analysis.video.properties.duration import _decode_duration_ffmpeg
+    >>> _decode_duration_ffmpeg("movia/examples/video.mp4", 0)
+    16.0
+    >>>
+    """
+    duration, _ = _decode_duration_frames_ffmpeg(filename, index)
+    return duration
+
+def _decode_duration_cv2(filename: str, index: int) -> float:
+    """
+    ** Extract the duration by the complete decoding of the stream. **
+
+    Slow but 100% accurate method.
+
+    Examples
+    --------
+    >>> from movia.core.analysis.video.properties.duration import _decode_duration_cv2
+    >>> _decode_duration_cv2("movia/examples/video.mp4", 0)
+    16.0
     >>>
     """
     cap = cv2.VideoCapture(filename, index)
     if not cap.isOpened():
         raise MissingStreamError(f"impossible to open '{filename}' stream {index} with 'cv2'")
-    if (fps := Fraction(cap.get(cv2.CAP_PROP_FPS)).limit_denominator(1001)) <= 0:
+    if (fps := float(cap.get(cv2.CAP_PROP_FPS))) <= 0:
         one_over_fps = 0
     else:
         one_over_fps = 1 / fps
-    duration = Fraction(0)
+    duration = .0
     while True:
-        duration = (
-            Fraction(round(cap.get(cv2.CAP_PROP_POS_MSEC))) / 1000
-            or duration + one_over_fps
-        )
+        duration = (1e-3 * float(cap.get(cv2.CAP_PROP_POS_MSEC))) or (duration + one_over_fps)
         if not cap.read()[0]:
             break
     cap.release()
     if not duration:
         raise MissingStreamError(f"'cv2' did not find duration '{filename}' stream {index}")
-    return duration + one_over_fps
+    return round(duration + one_over_fps, 3)
 
+def _estimate_duration_ffmpeg(filename: str, index: int) -> float:
+    """
+    ** Extract the duration from the metadata. **
+
+    Very fast method but inaccurate. It doesn't work all the time.
 
-def _estimate_duration_cv2(filename: str, index: int) -> Fraction:
+    Examples
+    --------
+    >>> from movia.core.analysis.video.properties.duration import _estimate_duration_ffmpeg
+    >>> _estimate_duration_ffmpeg("movia/examples/video.mp4", 0)
+    16.0
+    >>>
+    """
+    cmd = [
+        "ffprobe",
+        "-v", "error",
+        "-select_streams", f"v:{index}",
+        "-show_entries", "format=duration",
+        "-of", "default=noprint_wrappers=1:nokey=1",
+        filename,
+    ]
+    duration = _parse_ffprobe_res(cmd, filename, index)
+    try:
+        duration = float(duration)
+    except ValueError as err:
+        raise MissingInformation(
+            f"'ffprobe' did not get a correct duration in '{filename}' stream {index}"
+        ) from err
+    if duration <= 0:
+        raise MissingInformation(
+            f"'ffprobe' finds a duration of {duration} in '{filename}' stream {index}"
+        )
+    return duration
+
+def _estimate_duration_cv2(filename: str, index: int) -> float:
     """
     ** Extract the duration from the metadata. **
 
     Very fast method but inaccurate. It doesn't work all the time.
 
     Examples
     --------
-    >>> from cutcutcodec.core.analysis.video.properties.duration import _estimate_duration_cv2
-    >>> _estimate_duration_cv2("cutcutcodec/examples/video.mp4", 0)
-    Fraction(16, 1)
+    >>> from movia.core.analysis.video.properties.duration import _estimate_duration_cv2
+    >>> _estimate_duration_cv2("movia/examples/video.mp4", 0)
+    16.0
     >>>
     """
     cap = cv2.VideoCapture(filename, index)
     if not cap.isOpened():
         raise MissingStreamError(f"impossible to open '{filename}' stream {index} with 'cv2'")
-    frames = round(cap.get(cv2.CAP_PROP_FRAME_COUNT))
-    fps = Fraction(cap.get(cv2.CAP_PROP_FPS)).limit_denominator(1001)
+    frames = float(cap.get(cv2.CAP_PROP_FRAME_COUNT))
+    fps = float(cap.get(cv2.CAP_PROP_FPS))
     duration = frames / fps if fps and frames else 0
     cap.release()
     if duration <= 0:
         raise MissingInformation(
             f"'cv2' does not detect any duration in '{filename}' stream {index}"
         )
     return duration
 
-
-def get_duration_video(
+def get_duration(
     filename: typing.Union[str, bytes, pathlib.Path],
     index: int=0,
     *,
     backend: typing.Union[None, str]=None,
     accurate: bool=False,
-) -> Fraction:
+) -> float:
     """
     ** Recovers the total duration of a video stream. **
 
     The duration includes the display time o the last frame.
 
     Parameters
     ----------
     filename : pathlike
         The pathlike of the file containing a video stream.
     index : int
-        The relative index of the video stream being considered,
-        by default the first video stream encountered is selected.
+        The index of the video stream being considered,
+        by default the first stream encountered is selected.
     backend : str, optional
         - None (default) : Try to read the stream by trying differents backends.
         - 'ffmpeg' : Uses the modules ``pip3 install ffmpeg-python``
             which are using the ``ffmpeg`` program in the background.
         - 'cv2' : Uses the module ``pip3 install opencv-contrib-python-headless``.
     accurate : boolean, optional
         If True, recovers the duration by fully decoding all the frames in the video.
         It is very accurate but very slow. If False (default),
         first tries to get the duration from the file metadata.
         It's not accurate but very fast.
 
     Returns
     -------
-    duration : Fraction
+    duration : float
         The total duration of the considerated video stream.
 
     Raises
     ------
     MissingStreamError
         If the file does not contain a playable video stream.
     MissingInformation
         If the information is unavailable.
-
-    Examples
-    --------
-    >>> from cutcutcodec.core.analysis.video.properties.duration import get_duration_video
-    >>> get_duration_video("cutcutcodec/examples/video.mp4")
-    Fraction(16, 1)
-    >>> get_duration_video("cutcutcodec/examples/intro.mkv")
-    Fraction(9809, 1000)
-    >>>
     """
     _check_pathexists_index(filename, index)
 
     return _mix_and_check(
         backend, accurate, (str(pathlib.Path(filename)), index),
         collections.OrderedDict([
-            (
-                (lambda filename, index: _estimate_duration_ffmpeg(
-                    filename, _map_index_rel_to_abs(filename, index, "video"))
-                ),
-                {"accurate": False, "backend": "ffmpeg"}
-            ),
-            (
-                (lambda filename, index: _decode_duration_ffmpeg(
-                    filename, _map_index_rel_to_abs(filename, index, "video"), accurate=False)
-                ),
-                {"accurate": False, "backend": "ffmpeg"}
-            ),
+            (_estimate_duration_ffmpeg, {"accurate": False, "backend": "ffmpeg"}),
             (_estimate_duration_cv2, {"accurate": False, "backend": "cv2"}),
-            (
-                (lambda filename, index: _decode_duration_ffmpeg(
-                    filename, _map_index_rel_to_abs(filename, index, "video"), accurate=True)
-                ),
-                {"accurate": True, "backend": "ffmpeg"}
-            ),
+            (_decode_duration_ffmpeg, {"accurate": True, "backend": "ffmpeg"}),
             (_decode_duration_cv2, {"accurate": True, "backend": "cv2"}),
         ])
     )
```

### Comparing `movia-1.0.0rc1/cutcutcodec/core/analysis/video/properties/nb_frames.py` & `movia-1.0a1/movia/core/analysis/video/properties/nb_frames.py`

 * *Files 20% similar despite different names*

```diff
@@ -9,51 +9,45 @@
 
 import collections
 import pathlib
 import typing
 
 import cv2 # pip install opencv-contrib-python-headless
 
-from cutcutcodec.core.analysis._helper_properties import _check_pathexists_index, _mix_and_check
-from cutcutcodec.core.analysis.ffprobe import (_estimate_len_ffmpeg, _map_index_rel_to_abs,
-    get_slices_metadata)
-from cutcutcodec.core.exceptions import MissingStreamError, MissingInformation
-
+from movia.core.exceptions import MissingStreamError, MissingInformation
+from movia.core.analysis.video.properties.parser import (_check_pathexists_index,
+    _decode_duration_frames_ffmpeg, _mix_and_check, _parse_ffprobe_res)
 
 
 def _count_frames_ffmpeg(filename: str, index: int) -> int:
     """
     ** Count the number of frames with the ffmpeg decoder. **
 
     Slow but 100% accurate method.
 
     Examples
     --------
-    >>> from cutcutcodec.core.analysis.video.properties.nb_frames import _count_frames_ffmpeg
-    >>> _count_frames_ffmpeg("cutcutcodec/examples/video.mp4", 0)
+    >>> from movia.core.analysis.video.properties.nb_frames import _count_frames_ffmpeg
+    >>> _count_frames_ffmpeg("movia/examples/video.mp4", 0)
     400
     >>>
     """
-    _, infos = get_slices_metadata(filename, slice_type="frame")
-    if index >= len(infos):
-        raise MissingInformation(f"'ffmpeg' did not decode '{filename}' stream {index}")
-    frames = infos[index].shape[0]
+    _, frames = _decode_duration_frames_ffmpeg(filename, index)
     return frames
 
-
 def _count_frames_cv2(filename: str, index: int) -> int:
     """
     ** Count the number of frames with the cv2 decoder. **
 
     Slow but 100% accurate method.
 
     Examples
     --------
-    >>> from cutcutcodec.core.analysis.video.properties.nb_frames import _count_frames_cv2
-    >>> _count_frames_cv2("cutcutcodec/examples/video.mp4", 0)
+    >>> from movia.core.analysis.video.properties.nb_frames import _count_frames_cv2
+    >>> _count_frames_cv2("movia/examples/video.mp4", 0)
     400
     >>>
     """
     cap = cv2.VideoCapture(filename, index)
     if not cap.isOpened():
         raise MissingStreamError(f"impossible to open '{filename}' stream {index} with 'cv2'")
     frames = 0
@@ -62,38 +56,58 @@
             break
         frames += 1
     cap.release()
     if not frames:
         raise MissingStreamError(f"'cv2' did not find any frames '{filename}' stream {index}")
     return frames
 
+def _estimate_frames_ffmpeg(filename: str, index: int) -> int:
+    """
+    ** Extract the number of frames from the metadata. **
+
+    Very fast method but inaccurate. It doesn't work all the time.
+
+    Examples
+    --------
+    >>> from movia.core.analysis.video.properties.nb_frames import _estimate_frames_ffmpeg
+    >>> _estimate_frames_ffmpeg("movia/examples/video.mp4", 0)
+    400
+    >>>
+    """
+    cmd = [
+        "ffprobe", "-v", "error",
+        "-select_streams", f"v:{index}", "-show_entries", "stream=nb_frames",
+        "-of", "default=nokey=1:noprint_wrappers=1",
+        filename,
+    ]
+    frames = _parse_ffprobe_res(cmd, filename, index)
+    return int(frames)
 
 def _estimate_frames_cv2(filename: str, index: int) -> int:
     """
     ** Extract the number of frames from the metadata. **
 
     Very fast method but inaccurate. It doesn't work all the time.
 
     Examples
     --------
-    >>> from cutcutcodec.core.analysis.video.properties.nb_frames import _estimate_frames_cv2
-    >>> _estimate_frames_cv2("cutcutcodec/examples/video.mp4", 0)
+    >>> from movia.core.analysis.video.properties.nb_frames import _estimate_frames_cv2
+    >>> _estimate_frames_cv2("movia/examples/video.mp4", 0)
     400
     >>>
     """
     cap = cv2.VideoCapture(filename, index)
     if not cap.isOpened():
         raise MissingStreamError(f"impossible to open '{filename}' stream {index} with 'cv2'")
     frames = int(cap.get(cv2.CAP_PROP_FRAME_COUNT))
     cap.release()
     if frames <= 0: # we saw a case at -553402322211286528
         raise MissingInformation(f"'cv2' does not detect any frame in '{filename}' stream {index}")
     return frames
 
-
 def get_nb_frames(
     filename: typing.Union[str, bytes, pathlib.Path],
     index: int=0,
     *,
     backend: typing.Union[None, str]=None,
     accurate: bool=False,
 ) -> int:
@@ -101,15 +115,15 @@
     ** Recovers the number of frames present in a video stream. **
 
     Parameters
     ----------
     filename : pathlike
         The pathlike of the file containing a video stream.
     index : int
-        The relative index of the video stream being considered,
+        The index of the video stream being considered,
         by default the first stream encountered is selected.
     backend : str, optional
         - None (default) : Try to read the stream by trying differents backends.
         - 'ffmpeg' : Uses the modules ``pip3 install ffmpeg-python``
             which are using the ``ffmpeg`` program in the background.
         - 'cv2' : Uses the module ``pip3 install opencv-contrib-python-headless``.
     accurate : boolean, optional
@@ -125,38 +139,19 @@
 
     Raises
     ------
     MissingStreamError
         If the file does not contain a playable video stream.
     MissingInformation
         If the information is unavailable.
-
-    Examples
-    --------
-    >>> from cutcutcodec.core.analysis.video.properties.nb_frames import get_nb_frames
-    >>> get_nb_frames("cutcutcodec/examples/video.mp4")
-    400
-    >>> get_nb_frames("cutcutcodec/examples/intro.mkv")
-    294
-    >>>
     """
     _check_pathexists_index(filename, index)
 
     return _mix_and_check(
         backend, accurate, (str(pathlib.Path(filename)), index),
         collections.OrderedDict([
-            (
-                (lambda filename, index: _estimate_len_ffmpeg(
-                    filename, _map_index_rel_to_abs(filename, index, "video"))
-                ),
-                {"accurate": False, "backend": "ffmpeg"}
-            ),
+            (_estimate_frames_ffmpeg, {"accurate": False, "backend": "ffmpeg"}),
             (_estimate_frames_cv2, {"accurate": False, "backend": "cv2"}),
-            (
-                (lambda filename, index: _count_frames_ffmpeg(
-                    filename, _map_index_rel_to_abs(filename, index, "video"))
-                ),
-                {"accurate": True, "backend": "ffmpeg"}
-            ),
+            (_count_frames_ffmpeg, {"accurate": True, "backend": "ffmpeg"}),
             (_count_frames_cv2, {"accurate": True, "backend": "cv2"}),
         ])
     )
```

### Comparing `movia-1.0.0rc1/cutcutcodec/core/analysis/video/properties/rate.py` & `movia-1.0a1/movia/core/analysis/video/properties/framerate.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,101 +5,124 @@
 -----------------------------------------------------
 
 This information is collected in the metadata of the file.
 Its access is fast but its value is not always accurate.
 Especially since the framerate is not always constant within the same stream.
 """
 
-from fractions import Fraction
-import collections
+import fractions
+import numbers
 import pathlib
+import re
 import typing
 
 import cv2 # pip install opencv-contrib-python-headless
 
-from cutcutcodec.core.analysis._helper_properties import _check_pathexists_index, _mix_and_check
-from cutcutcodec.core.analysis.ffprobe import _estimate_rate_ffmpeg
-from cutcutcodec.core.analysis.ffprobe import _map_index_rel_to_abs
-from cutcutcodec.core.exceptions import MissingStreamError, MissingInformation
+from movia.core.exceptions import MissingStreamError, MissingInformation
+from movia.core.analysis.video.properties.parser import _parse_ffprobe_res
 
 
 
-def _estimate_rate_cv2(filename: str, index: int) -> Fraction:
+def _estimate_fps_cv2(filename: str, index: int) -> float:
     """
     ** Retrieves via cv2, the metadata concerning the fps. **
 
     This function is fast because it reads only the header of the file.
 
     Examples
     --------
-    >>> from cutcutcodec.core.analysis.video.properties.rate import _estimate_rate_cv2
-    >>> _estimate_rate_cv2("cutcutcodec/examples/video.mp4", 0)
-    Fraction(25, 1)
+    >>> from movia.core.analysis.video.properties.framerate import _estimate_fps_cv2
+    >>> _estimate_fps_cv2("movia/examples/video.mp4", 0)
+    25.0
     >>>
     """
     cap = cv2.VideoCapture(filename, index)
     if not cap.isOpened():
         raise MissingStreamError(f"impossible to open '{filename}' stream {index} with 'cv2'")
-    fps = Fraction(cap.get(cv2.CAP_PROP_FPS)).limit_denominator(1001)
+    fps = float(cap.get(cv2.CAP_PROP_FPS))
     cap.release()
     if fps <= 0:
         raise MissingInformation(f"'cv2' finds an fps of {fps} in '{filename}' stream {index}")
     return fps
 
 
-def get_rate_video(
+def _estimate_fps_ffmpeg(filename: str, index: int) -> fractions.Fraction:
+    """
+    ** Retrieves via ffmpeg, the metadata concerning the fps. **
+
+    This function is fast because it reads only the header of the file.
+
+    ffprobe -v quiet -print_format json -show_streams -select_streams v:0 video.mp4
+
+    Examples
+    --------
+    >>> from movia.core.analysis.video.properties.framerate import _estimate_fps_ffmpeg
+    >>> _estimate_fps_ffmpeg("movia/examples/video.mp4", 0)
+    Fraction(25, 1)
+    >>>
+    """
+    cmd = [
+        "ffprobe", "-v", "error",
+        "-select_streams", f"v:{index}", "-show_entries", "stream=r_frame_rate,avg_frame_rate",
+        "-of", "default=nokey=1:noprint_wrappers=1",
+        filename,
+    ]
+    fps_str = _parse_ffprobe_res(cmd, filename, index)
+    for match in re.finditer(r"\d+(/\d+)?", fps_str):
+        try:
+            return fractions.Fraction(match.group())
+        except ZeroDivisionError:
+            continue
+    raise MissingInformation(
+            f"'ffprobe' did not get a correct framerate in '{filename}' stream {index}"
+        )
+
+
+def get_fps(
     filename: typing.Union[str, bytes, pathlib.Path],
     index: int=0,
     *,
     backend: typing.Union[None, str]=None
-) -> Fraction:
+) -> numbers.Real:
     """
     ** Reads in the metadata, the average frequency of the frames. **
 
     Parameters
     ----------
     filename : pathlike
         The pathlike of the file containing a video stream.
     index : int
-        The relative index of the video stream being considered,
+        The index of the video stream being considered,
         by default the first stream encountered is selected.
     backend : str, optional
         - None (default) : Try to read the stream by trying differents backends.
         - 'ffmpeg' : Uses the modules ``pip install ffmpeg-python``
             which are using the ``ffmpeg`` program in the background.
         - 'cv2' : Uses the module ``pip install opencv-contrib-python-headless``.
 
     Returns
     -------
-    fps : Fraction
+    fps : numbers.Real
         The average frequency of the frames in hz.
 
     Raises
     ------
     MissingStreamError
         If the file does not contain a playable video stream.
     MissingInformation
         If the information is unavailable.
-
-    Examples
-    --------
-    >>> from cutcutcodec.core.analysis.video.properties.rate import get_rate_video
-    >>> get_rate_video("cutcutcodec/examples/video.mp4")
-    Fraction(25, 1)
-    >>> get_rate_video("cutcutcodec/examples/intro.mkv")
-    Fraction(30000, 1001)
-    >>>
     """
-    _check_pathexists_index(filename, index)
-
-    return _mix_and_check(
-        backend, False, (str(pathlib.Path(filename)), index),
-        collections.OrderedDict([
-            (
-                (lambda filename, index: _estimate_rate_ffmpeg(
-                    filename, _map_index_rel_to_abs(filename, index, "video"))
-                ),
-                {"accurate": False, "backend": "ffmpeg"}
-            ),
-            (_estimate_rate_cv2, {"accurate": False, "backend": "cv2"}),
-        ])
-    )
+    assert pathlib.Path(filename).exists(), filename
+    assert isinstance(index, numbers.Integral), index.__class__.__name__
+    assert backend is None or backend in {"ffmpeg", "cv2"}, backend
+
+    filename = str(pathlib.Path(filename))
+
+    if backend == "ffmpeg":
+        return _estimate_fps_ffmpeg(filename, index)
+    if backend == "cv2":
+        return _estimate_fps_cv2(filename, index)
+
+    try:
+        return _estimate_fps_ffmpeg(filename, index)
+    except (MissingStreamError, MissingInformation):
+        return _estimate_fps_cv2(filename, index)
```

### Comparing `movia-1.0.0rc1/cutcutcodec/core/classes/container.py` & `movia-1.0a1/movia/core/classes/container.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,16 +3,16 @@
 """
 ** Defines the entry and exit points of the assembly graph. **
 --------------------------------------------------------------
 """
 
 import typing
 
-from cutcutcodec.core.classes.node import Node
-from cutcutcodec.core.classes.stream import Stream
+from movia.core.classes.node import Node
+from movia.core.classes.stream import Stream
 
 
 
 class ContainerInput(Node):
     """
     ** Entry point of an assembly graph. **
     """
```

### Comparing `movia-1.0.0rc1/cutcutcodec/core/classes/node.py` & `movia-1.0a1/movia/core/classes/node.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 #!/usr/bin/env python3
 
 """
 ** General node of the assembly graph. **
 -----------------------------------------
 """
 
+
 import abc
 import typing
 
-from cutcutcodec.core.classes.stream import Stream
+from movia.core.classes.stream import Stream
 
 
 
 class Node(abc.ABC):
     """
     ** General node of the assembly graph. **
 
@@ -56,15 +57,15 @@
 
     def __setstate__(self, streams_state) -> None:
         """
         ** Allows ``pickle`` to recreate the object identically. **
 
         Parameters
         ----------
-        streams_state : tuple[typing.Iterable[cutcutcodec.core.classes.stream.Stream], dict]
+        streams_state : tuple[typing.Iterable[movia.core.classes.stream.Stream], dict]
             These are the input streams and the other arguments.
         """
         assert isinstance(streams_state, tuple), streams_state.__class__.__name__
         assert len(streams_state) == 2, streams_state
         in_streams, state = streams_state
         self.setstate(in_streams, state)
 
@@ -98,48 +99,34 @@
             Even if this is not optimal in terms of memory and speed,
             the objects must be explicit so that they can be easily manipulated
             when the assembly graph is optimized.
             The keys must be of type str and the dictionary must to be jsonisable.
         """
         raise NotImplementedError
 
-    def in_select(self, type_: str) -> tuple[Stream, ...]:
-        """
-        ** Select the incoming streams of a specific type. **
-        """
-        assert isinstance(type_, str), type_.__class__.__name__
-        return tuple(s for s in self._in_streams if s.type == type_)
-
     @property
     def in_streams(self) -> tuple[Stream, ...]:
         """
-        ** The incoming streams on the node. **
+        ** The streams arriving on the node. **
         """
         return self._in_streams
 
-    def out_select(self, type_: str) -> tuple[Stream, ...]:
-        """
-        ** Select the outgoing streams of a specific type. **
-        """
-        assert isinstance(type_, str), type_.__class__.__name__
-        return tuple(s for s in self._out_streams if s.type == type_)
-
     @property
     def out_streams(self) -> tuple[Stream, ...]:
         """
-        ** The outgoing streams on the node. **
+        ** The streams comin back on the node. **
         """
         return self._out_streams
 
     @abc.abstractmethod
     def setstate(self, in_streams: typing.Iterable[Stream], state: dict) -> None:
         """
         ** Allows to completely change the internal state of the node. **
 
         Parameters
         ----------
         in_streams
-            Same as ``cutcutcodec.core.classes.stream.Stream.in_streams``.
+            Same as ``movia.core.classes.stream.Stream.in_streams``.
         state : dict
             The internal state returned by the ``getstate`` method of the same class.
         """
         raise NotImplementedError
```

### Comparing `movia-1.0.0rc1/cutcutcodec/core/classes/stream.py` & `movia-1.0a1/movia/core/classes/stream.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,57 +1,49 @@
 #!/usr/bin/env python3
 
 """
 ** Defines the structure of an abstract multimedia stream. **
 -------------------------------------------------------------
 """
 
-from fractions import Fraction
+
 import abc
+import math
 import numbers
-import typing
 
 
 
 class Stream(abc.ABC):
     """
     Attributes
     ----------
-    beginning : Fraction
+    beginning : numbers.Real
         The stream beginning instant in second (readonly).
-    duration : Fraction or inf
+    duration : numbers.Real
         The duration of the flow in seconds, it can be infinite (readonly).
         This value needs to be accurate.
     index : int
         The stream index from the parent node (0 to n-1) (readonly).
     is_time_continuous : boolean
         True if the data is continuous in the time domain, False if it is discrete (readonly).
-    node : cutcutcodec.core.classes.node.Node
+    node : movia.core.classes.node.Node
         The node where this stream comes from (readonly).
         Allows back propagation in the assembly graph.
-    node_main : cutcutcodec.core.classes.node.Node
-        The node used for the compilation. This node has the same output_streams
-        as ``node`` but not nescessary the same input_streams and te same properties.
-        It can be used for factorisation (read and write).
     """
 
     def __init__(self, node):
         """
         Parameters
         ----------
-        node : cutcutcodec.core.classes.node.Node
+        node : movia.core.classes.node.Node
             The node where this stream comes from.
             The audit must be conducted in the children's classes.
             It is not done here in order to avoid cyclic imports.
-        node_main : cutcutcodec.core.classes.node.Node
-            In the case this streams comes from ``cutcutcodec.core.filters.meta_filter.MetaFilter``,
-            `node_main` is the meta filter while `node` is the subgraph of the meta-filter.
         """
         self._node = node
-        self._node_main = node
 
     def __eq__(self, other) -> bool:
         """
         ** 2 streams are equivalent if their parent nodes are similar. **
         """
         if self.__class__ != other.__class__:
             return False
@@ -75,28 +67,26 @@
     def _stream_from_parent_node(node, index):
         """
         ** Return the equivalent stream contained in the parent node. **
         """
         return node.out_streams[index]
 
     @property
-    @abc.abstractmethod
-    def beginning(self) -> Fraction:
+    def beginning(self) -> numbers.Real:
         """
         ** The stream beginning instant in second. **
         """
-        raise NotImplementedError
+        return 0
 
     @property
-    @abc.abstractmethod
-    def duration(self) -> typing.Union[Fraction, float]:
+    def duration(self) -> numbers.Real:
         """
-        ** The duration of the flow in seconds, positive fraction or infinite **
+        ** Default infinite flow duration, can be overwritten. **
         """
-        raise NotImplementedError
+        return math.inf
 
     @property
     def index(self) -> int:
         """
         ** The stream index from the parent node (0 to n-1). **
         """
         indexs = [index for index, stream in enumerate(self.node.out_streams) if stream is self]
@@ -116,77 +106,50 @@
     def node(self):
         """
         ** The node where this stream comes from. **
         """
         return self._node
 
     @property
-    def node_main(self):
-        """
-        ** The global node, can be an alias to the classic node. **
-        """
-        return self._node_main
-
-    @node_main.setter
-    def node_main(self, new_node):
-        """
-        ** Change the node if this stream is already present in the new node at the same place. **
-        """
-        for i, stream in enumerate(new_node.out_streams):
-            if stream is self:
-                if self.index != i:
-                    raise AttributeError(
-                        f"the index of the stream {self} in the node {self.node} is {self.index}, "
-                        f"but it is {i} in the node {new_node}"
-                    )
-                self._node_main = new_node
-                return
-        raise AttributeError(f"the stream {self} is not in the node {new_node}")
-
-    @property
     @abc.abstractmethod
     def type(self) -> str:
         """
         ** The type of stream, 'audio', 'subtitle' or 'video'. **
         """
         raise NotImplementedError
 
 
 class StreamWrapper(Stream):
     """
     ** Allows to dynamically transfer the methods of an instanced stream. **
 
     Attribute
     ---------
-    stream : cutcutcodec.core.classes.stream.Stream
+    stream : movia.core.classes.stream.Stream
         The stream containing the properties to be transferred (readonly).
         This stream is one of the input streams of the parent node.
     """
 
     def __init__(self, node, index: numbers.Integral):
         """
         Parameters
         ----------
-        node : cutcutcodec.core.classes.node.Node
-            The parent node, transmitted to ``cutcutcodec.core.classes.stream.Stream``.
+        node : movia.core.classes.node.Node
+            The parent node, transmitted to ``movia.core.classes.stream.Stream``.
         index : number.Integral
             The index of the stream among all the input streams of the ``node``.
             0 for the first, 1 for the second ...
         """
         super().__init__(node)
         assert isinstance(index, numbers.Integral) and index >= 0, index
         assert len(node.in_streams) > index, f"only {len(node.in_streams)} streams, no {index}"
         self._index = int(index)
 
     @property
-    def beginning(self) -> Fraction:
-        return self.stream.beginning
-
-    @property
-    def duration(self) -> typing.Union[Fraction, float]:
+    def duration(self) -> numbers.Real:
         return self.stream.duration
 
     @property
     def index(self) -> int:
         """
         ** The stream index from the parent node (0 to n-1). **
         """
```

### Comparing `movia-1.0.0rc1/cutcutcodec/core/classes/stream_audio.py` & `movia-1.0a1/movia/core/classes/stream_audio.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,132 +2,126 @@
 
 """
 ** Defines the structure of an abstract audio stream. **
 --------------------------------------------------------
 """
 
 import abc
-from fractions import Fraction
 import numbers
 import typing
 
-from cutcutcodec.core.classes.filter import Filter
-from cutcutcodec.core.classes.frame_audio import FrameAudio
-from cutcutcodec.core.classes.stream import Stream, StreamWrapper
+import numpy as np
+
+from movia.core.classes.filter import Filter
+from movia.core.classes.stream import Stream, StreamWrapper
+from movia.core.exceptions import OutOfTimeRange
 
 
 
 class StreamAudio(Stream):
     """
     ** Representation of any audio stream. **
 
     Attributes
     ----------
     channels : int
         The number of tracks (readonly).
     """
 
-    @abc.abstractmethod
-    def _snapshot(self, timestamp: Fraction, rate: int, samples: int) -> FrameAudio:
-        raise NotImplementedError
-
     @property
     @abc.abstractmethod
     def channels(self) -> int:
         """
         ** The number of channels in this audio stream. **
         """
         raise NotImplementedError
 
-    def snapshot(self,
-        timestamp: numbers.Real,
-        rate: typing.Optional[numbers.Integral]=None,
-        samples: numbers.Integral=1,
-    ) -> FrameAudio:
+    @abc.abstractmethod
+    def _snapshot(self, timestamp: np.ndarray[numbers.Real]) -> np.ndarray[numbers.Real]:
+        raise NotImplementedError
+
+    def snapshot(
+        self, timestamp: typing.Union[numbers.Real, np.ndarray[numbers.Real]]
+    ) -> np.ndarray[numbers.Real]:
         """
         ** Extract the closest values to the requested date. **
 
         Parameters
         ----------
-        timestamp : numbers.Real
-            The absolute time expressed in seconds, not relative to the beginning of the audio.
-            Is the instant of the first sample of the returned frame.
-            For avoid the inacuracies of round, it is recomended to use fractional number.
-        rate : numbers.Integral, optional
-            If samples == 1, this argument is ignored. Otherwise is the samplerate of the frame.
-            If provide and samples != 1, allows to deduce the timestamps of the non 0 samples.
-            If non provide and samples != 1, try to call the `rate` attribute of the stream.
-        samples : numbers.Integral, default=1
-            The number of audio samples per channels to catch.
+        timestamps : numbers.Real or np.ndarray[numbers.Real]
+            The time expressed in seconds since the beginning of the audio.
+            Vector in 0 or 1 dimension.
 
         Returns
         -------
-        samples : FrameAudio
+        sample : np.ndarray[numbers.Real]
             Audio samples corresponding to the times provided.
             This vector is of shape (nbr_channels, *timestamp_shape).
             The values are between -1 and 1.
 
         Raises
         ------
-        cutcutcodec.core.exception.OutOfTimeRange
-            If we try to get a frame out of the definition range.
-            The valid range is [self.beginning, self.beginning+self.duration].
-            The range taken is [timestamp, timestamp + samples/rate[.
-        AttributeError
-            If the `rate` attribute has to be defined but is not provides or deductable.
-        """
-        # verifications on input
-        assert isinstance(samples, numbers.Integral), samples.__class__.__name__
-        samples = int(samples)
-        assert samples > 0, samples
-        if rate is None:
-            if samples != 1:
-                if (rate := getattr(self, "rate", None)) is None:
-                    raise ValueError("rate attribute has to be provide")
-            else:
-                rate = 1 # ignore default unused stupid value
-        assert isinstance(rate, numbers.Integral), rate.__class__.__name__
-        rate = int(rate)
-        assert rate > 0, rate
-        assert isinstance(timestamp, numbers.Real), timestamp.__class__.__name__
-        timestamp = Fraction(timestamp)
-
-        # extract samples
-        frame = self._snapshot(timestamp, rate, samples)
-
-        # result verification
-        assert isinstance(frame, FrameAudio), frame.__class__.__name__
-        return frame
+        movia.core.exception.OutOfTimeRange
+            If we try to read a sample at a negative time or after the end of the stream.
+        """
+        # cast
+        timestamp = np.asarray(timestamp)
+        if timestamp.ndim != 1:
+            return self.snapshot(timestamp.ravel()).reshape((-1, *timestamp.shape))
+
+        # verification
+        if timestamp.dtype == np.dtype("O"):
+            assert all(isinstance(o, numbers.Real) for o in timestamp), timestamp
+            timestamp = timestamp.astype(np.float64)
+        else:
+            assert issubclass(timestamp.dtype.type, numbers.Real), timestamp.dtype.type
+        t_min = np.min(timestamp)
+        if t_min < 0:
+            raise OutOfTimeRange(f"there is no audio frame at timestamp {t_min} (need >= 0)")
+
+        # evaluation
+        sample = self._snapshot(timestamp)
+
+        # verification
+        assert sample.shape[1:] == timestamp.shape, (sample.shape, timestamp.shape)
+        if sample.dtype == np.dtype("O"):
+            assert all(isinstance(o, numbers.Real) for o in sample), sample
+        else:
+            assert issubclass(sample.dtype.type, numbers.Real), sample.dtype.type
+        sample_no_nan = np.nan_to_num(sample)
+        assert -1 <= np.min(sample_no_nan) and np.max(sample_no_nan) <= 1, \
+            (np.nanmin(sample), np.nanmax(sample))
+
+        return sample
 
     @property
     def type(self) -> str:
         return "audio"
 
-
 class StreamAudioWrapper(StreamWrapper, StreamAudio):
     """
     ** Allows to dynamically transfer the methods of an instanced audio stream. **
 
     This can be very useful for implementing filters.
     """
 
     def __init__(self, node: Filter, index: numbers.Integral):
         """
         Parameters
         ----------
-        filter : cutcutcodec.core.classes.filter.Filter
-            The parent node, transmitted to ``cutcutcodec.core.classes.stream.Stream``.
+        filter : movia.core.classes.filter.Filter
+            The parent node, transmitted to ``movia.core.classes.stream.Stream``.
         index : number.Integral
             The index of the audio stream among all the input streams of the ``node``.
             0 for the first, 1 for the second ...
         """
         assert isinstance(node, Filter), node.__class__.__name__
         assert len(node.in_streams) > index, f"only {len(node.in_streams)} streams, no {index}"
         assert isinstance(node.in_streams[index], StreamAudio), "the stream must be audio type"
         super().__init__(node, index)
 
-    def _snapshot(self, timestamp: Fraction, rate: int, samples: int) -> FrameAudio:
-        return self.stream._snapshot(timestamp, rate, samples)
+    def _snapshot(self, timestamp: np.ndarray[numbers.Real]) -> np.ndarray[numbers.Real]:
+        return self.stream._snapshot(timestamp)
 
     @property
     def channels(self) -> int:
         return self.stream.channels
```

### Comparing `movia-1.0.0rc1/cutcutcodec/core/classes/stream_video.py` & `movia-1.0a1/movia/core/classes/stream_video.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,127 +1,134 @@
 #!/usr/bin/env python3
 
 """
 ** Defines the structure of an abstract video stream. **
 --------------------------------------------------------
 """
 
-from fractions import Fraction
 import abc
-import math
 import numbers
-import typing
 
-import torch
+import av
 
-from cutcutcodec.core.classes.filter import Filter
-from cutcutcodec.core.classes.frame_video import FrameVideo
-from cutcutcodec.core.classes.stream import Stream, StreamWrapper
+from movia.core.classes.filter import Filter
+from movia.core.classes.stream import Stream, StreamWrapper
+from movia.core.exceptions import OutOfTimeRange
 
 
 
 class StreamVideo(Stream):
     """
     ** Representation of any video stream. **
 
     Attributes
     ----------
+    height : int
+        Height of the image in pixels (readonly).
     is_space_continuous : boolean
         True if the data is continuous in the spacial domain, False if it is discrete (readonly).
+    width : int
+        Width of the image in pixels (readonly).
     """
 
-    def _snapshot(self, timestamp: Fraction, shape: tuple[int, int]) -> FrameVideo:
+    def _snapshot(self, timestamp: float) -> av.video.frame.VideoFrame:
+        raise NotImplementedError
+
+    @property
+    def height(self) -> int:
+        """
+        ** Height of all images in the stream. **
+        """
+        if self.is_space_continuous and hasattr(self.node, "shape"):
+            return self.node.shape[0]
         raise NotImplementedError
 
     @property
     @abc.abstractmethod
     def is_space_continuous(self) -> bool:
         """
         ** True if the data is continuous in the spacial domain, False if it is discrete. **
         """
         raise NotImplementedError
 
-    def snapshot(self,
-        timestamp: numbers.Real,
-        shape: typing.Union[tuple[numbers.Integral, numbers.Integral], list[numbers.Integral]],
-        *, channels=None
-    ) -> FrameVideo:
+    def snapshot(self, timestamp: numbers.Real) -> av.video.frame.VideoFrame:
         """
         ** Extract the closest frame to the requested date. **
 
         Parameters
         ----------
         timestamp : numbers.Real
-            The absolute time expressed in seconds, not relative to the beginning of the video.
-            For avoid the inacuracies of round, it is recomended to use fractional number.
-        shape : int and int
-            The pixel dimensions of the returned frame.
-            The convention adopted is the numpy convention (height, width).
-        channels : int, optional
-            Impose the numbers of channels, apply convertion if nescessary.
-            For the interpretation of the layers,
-            see ``cutcutcodec.core.classes.frame_video.FrameVideo``.
+            The time expressed in seconds since the beginning of the video.
 
         Returns
         -------
-        frame : cutcutcodec.core.classes.frame_video.FrameVideo
+        frame : av.frame.Frame
             Video frame with metadata.
 
         Raises
         ------
-        cutcutcodec.core.exception.OutOfTimeRange
-            If we try to get a frame out of the definition range.
-            The valid range is [self.beginning, self.beginning+self.duration[.
+        movia.core.exception.OutOfTimeRange
+            If we try to read a frame at a negative time or after the end of the stream.
         """
         assert isinstance(timestamp, numbers.Real), timestamp.__class__.__name__
-        assert isinstance(shape, (tuple, list)), shape.__class__.__name__
-        assert len(shape) == 2, len(shape)
-        assert all(isinstance(s, numbers.Integral) and s >= 1 for s in shape), shape
-        shape = (int(shape[0]), int(shape[1]))
-        if math.isnan(timestamp): # default transparent video frame
-            frame = FrameVideo(0, torch.zeros((*shape, 2), dtype=torch.uint8))
-        else:
-            frame = self._snapshot(Fraction(timestamp), shape)
-        if channels is not None:
-            frame = frame.convert(channels)
-        assert isinstance(frame, FrameVideo), frame.__class__.__name__
+        if timestamp < 0:
+            raise OutOfTimeRange(f"the timestamp must be positive or zero, it is {timestamp}")
+        frame = self._snapshot(float(timestamp))
+        assert isinstance(frame, av.video.frame.VideoFrame), frame.__class__.__name__
         return frame
 
     @property
     def type(self) -> str:
         return "video"
 
+    @property
+    def width(self) -> int:
+        """
+        ** Width of all images in the stream. **
+        """
+        if self.is_space_continuous and hasattr(self.node, "shape"):
+            return self.node.shape[1]
+        raise NotImplementedError
+
 
 class StreamVideoWrapper(StreamWrapper, StreamVideo):
     """
     ** Allows to dynamically transfer the methods of an instanced video stream. **
 
     This can be very useful for implementing filters.
 
     Attribute
     ---------
-    stream : cutcutcodec.core.classes.stream_video.StreamVideo
+    stream : movia.core.classes.stream_video.StreamVideo
         The video stream containing the properties to be transferred (readonly).
         This stream is one of the input streams of the parent node.
     """
 
     def __init__(self, node: Filter, index: numbers.Integral):
         """
         Parameters
         ----------
-        filter : cutcutcodec.core.classes.filter.Filter
-            The parent node, transmitted to ``cutcutcodec.core.classes.stream.Stream``.
+        filter : movia.core.classes.filter.Filter
+            The parent node, transmitted to ``movia.core.classes.stream.Stream``.
         index : number.Integral
             The index of the video stream among all the input streams of the ``node``.
             0 for the first, 1 for the second ...
         """
         assert isinstance(node, Filter), node.__class__.__name__
         assert len(node.in_streams) > index, f"only {len(node.in_streams)} streams, no {index}"
         assert isinstance(node.in_streams[index], StreamVideo), "the stream must be video type"
         super().__init__(node, index)
 
-    def _snapshot(self, timestamp: Fraction, shape: tuple[int, int]) -> FrameVideo:
-        return self.stream._snapshot(timestamp, shape)
+    def _snapshot(self, timestamp: float) -> av.video.frame.VideoFrame:
+        return self.stream._snapshot(timestamp)
+
+    @property
+    def height(self) -> int:
+        return self.stream.height
 
     @property
     def is_space_continuous(self) -> bool:
         return self.stream.is_space_continuous
+
+    @property
+    def width(self) -> int:
+        return self.stream.width
```

### Comparing `movia-1.0.0rc1/cutcutcodec/core/compilation/export/compatibility.py` & `movia-1.0a1/movia/core/compilation/export/compatibility.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,24 +3,26 @@
 """
 ** Allows you to choose a format and codecs. **
 -----------------------------------------------
 
 The information collected here concerns the encoding and not the decoding.
 """
 
+
+import typing
+
 import itertools
 import multiprocessing.pool
 import os
 import re
 import subprocess
-import typing
 
 import numpy as np
 
-from cutcutcodec.core.optimisation.cache.singleton import MetaSingleton
+from movia.core.optimisation.cache.singleton import MetaSingleton
 
 
 
 def _check_encoder_compatibility(encodec_muxer_kind: tuple[str, str, str]) -> bool:
     """
     ** Pickable version for chec an encoder / codec compatibility with a specific muxer. **
     """
@@ -31,15 +33,15 @@
             "-f", "rawvideo", "-r", "24", "-pix_fmt", "yuv420p", "-s", "32x32", "-i", "pipe:",
             "-c:v", encodec, "-strict", "experimental", "-f", muxer, os.devnull,
         ]
         data = os.urandom(7680) # 32 pxl * 32 pxl * 12 bits / pxl * 5 frames
     elif kind == "audio":
         cmd = [
             "timeout", "30", "ffmpeg", "-v", "error", "-y",
-            "-f", "s8", "-ar", "48000", "-ac", "2", "-i", "pipe:",
+            "-f", "s8", "-ar", "48000", "-ac", "2", "-i", "pipe:", # 44100 not always supported
             "-c:a", encodec, "-strict", "experimental", "-f", muxer, os.devnull,
         ]
         data = os.urandom(9600) # 2 channels * 100 ms
     elif kind == "subtitle":
         cmd = [
             "timeout", "30", "ffmpeg", "-v", "error", "-y",
             "-f", "srt", "-i", "pipe:",
@@ -62,17 +64,17 @@
 
     def __init__(self):
         self.codecs_cache = WriteInfos.codecs_init()
         self.encoders_cache = WriteInfos.encoders_init()
         self.muxers_cache = WriteInfos.muxers_init()
         self._compatibilites = {} # all tested combinaisons of (encodec, format) -> is_compatible
 
-    def check_compatibilities(
+    def check_compatibilites(
         self, encodecs: list[str], muxers: list[str]
-    ) -> np.ndarray[bool]:
+    ) -> np.ndarray:
         """
         ** Asynchronously checks codec combinations. **
 
         Parameters
         ----------
         encodecs : list[str]
             The codec or encoder names.
@@ -80,42 +82,23 @@
             The muxer (format) names.
 
         Returns
         -------
         compatibility_matrix : np.ndarray[bool]
             The 2d boolean compatibility matrix.
             Item (i, j) is True if encodecs[i] is compatible with muxers[j].
-
-        Examples
-        --------
-        >>> from cutcutcodec.core.compilation.export.compatibility import WriteInfos
-        >>> WriteInfos().check_compatibilities(["h264", "libx265", "opus"], ["matroska", "ogg"])
-        array([[ True, False],
-               [ True, False],
-               [ True,  True]])
-        >>> WriteInfos().check_compatibilities([], [])
-        array([], shape=(1, 0), dtype=bool)
-        >>> WriteInfos().check_compatibilities(["opus"], [])
-        array([], shape=(1, 0), dtype=bool)
-        >>> WriteInfos().check_compatibilities([], ["ogg"])
-        array([], shape=(1, 0), dtype=bool)
-        >>>
         """
         assert isinstance(encodecs, list), encodecs.__class__.__name__
         assert all(isinstance(ec, str) for ec in encodecs), encodecs
         assert set(encodecs).issubset(self.codecs|self.encoders), \
             set(encodecs)-(self.codecs|self.encoders)
         assert isinstance(muxers, list), muxers.__class__.__name__
         assert all(isinstance(f, str) for f in muxers), muxers
         assert set(muxers).issubset(self.muxers), set(muxers)-self.muxers
 
-        # case empty:
-        if len(encodecs) == 0 or len(muxers) == 0:
-            return np.asarray([[]], dtype=bool) # oblige for keep 2d array homogeneous
-
         # makes checks
         if (ecs_ms := [
             ec_m for ec_m in itertools.product(encodecs, muxers) if ec_m not in self._compatibilites
         ]): # only for optimisation
             encodecs_cache = {**self.codecs_cache, **self.encoders_cache}
             with multiprocessing.pool.ThreadPool() as pool: # subprocess release the GIL
                 for encodec_and_muxer, is_compatible in zip(
@@ -139,15 +122,15 @@
     @property
     def codecs(self) -> set[str]:
         """
         ** Returns all eligible codecs. **
 
         Examples
         --------
-        >>> from cutcutcodec.core.compilation.export.compatibility import WriteInfos
+        >>> from movia.core.compilation.export.compatibility import WriteInfos
         >>> codecs = WriteInfos().codecs
         >>> "av1" in codecs
         True
         >>> "vorbis" in codecs
         True
         >>> "subrip" in codecs
         True
@@ -197,15 +180,15 @@
     @property
     def encoders(self) -> set[str]:
         """
         ** Returns all eligible encoders. **
 
         Examples
         --------
-        >>> from cutcutcodec.core.compilation.export.compatibility import WriteInfos
+        >>> from movia.core.compilation.export.compatibility import WriteInfos
         >>> encoders = WriteInfos().encoders
         >>> "libaom-av1" in encoders
         True
         >>> "libvorbis" in encoders
         True
         >>> "srt" in encoders
         True
@@ -256,32 +239,47 @@
 
     def get_codecs_for_muxer(self, muxer: str) -> set[str]:
         """
         ** Search all available codecs for a given muxer. **
 
         Examples
         --------
-        >>> from cutcutcodec.core.compilation.export.compatibility import WriteInfos
+        >>> from movia.core.compilation.export.compatibility import WriteInfos
         >>> sorted(WriteInfos().get_codecs_for_muxer("ogg"))
         ['flac', 'opus', 'speex', 'theora', 'vorbis', 'vp8']
         >>>
         """
         assert isinstance(muxer, str), muxer.__class__.__name__
         assert muxer in self.muxers, f"{muxer} not in {self.muxers}"
 
         if "codecs" not in self.muxers_cache[muxer]:
             all_codecs = list(self.codecs)
-            mask = self.check_compatibilities(all_codecs, [muxer])[:, 0]
+            mask = self.check_compatibilites(all_codecs, [muxer])[:, 0]
             codecs = set(np.asarray(all_codecs, dtype=object)[mask])
             self.muxers_cache[muxer]["codecs"] = codecs
         return self.muxers_cache[muxer]["codecs"]
 
     def get_encoder_doc(self, encoder: str) -> str:
         r"""
         ** Retrive the ffmpeg documentation of this encoder. **
+
+        Examples
+        --------
+        >>> from pprint import pprint
+        >>> from movia.core.compilation.export.compatibility import WriteInfos
+        >>> pprint(WriteInfos().get_encoder_doc("libvorbis"))
+        ('Encoder libvorbis [libvorbis]:\n'
+         '    General capabilities: dr1 delay small \n'
+         '    Threading capabilities: none\n'
+         '    Supported sample formats: fltp\n'
+         'libvorbis AVOptions:\n'
+         '  -iblock            <double>     E...A...... Sets the impulse block bias '
+         '(from -15 to 0) (default 0)\n'
+         '\n')
+        >>>
         """
         assert isinstance(encoder, str), encoder.__class__.__name__
         assert encoder in self.encoders, f"{encoder} not in {self.encoders}"
 
         if self.encoders_cache[encoder].get("doc") is None:
             self.encoders_cache[encoder]["doc"] = subprocess.run(
                 ["ffmpeg", "-v", "error", "-h", f"encoder={encoder}"],
@@ -291,35 +289,57 @@
 
     def get_encoders_for_muxer(self, muxer: str) -> set[str]:
         """
         ** Search all available encoders for a given muxer. **
 
         Examples
         --------
-        >>> from cutcutcodec.core.compilation.export.compatibility import WriteInfos
+        >>> from movia.core.compilation.export.compatibility import WriteInfos
         >>> sorted(WriteInfos().get_encoders_for_muxer("ogg"))
         ['flac', 'libopus', 'libspeex', 'libtheora', 'libvorbis', 'libvpx', 'opus', 'vorbis']
         >>>
         """
         assert isinstance(muxer, str), muxer.__class__.__name__
         assert muxer in self.muxers, f"{muxer} not in {self.muxers}"
 
         if "encoders" not in self.muxers_cache[muxer]:
             all_encoders = [
                 encoder for codec in self.get_codecs_for_muxer(muxer)
                 for encoder in CodecInfos(codec).encoders
             ] # more optimised than list(self.encoders)
-            mask = self.check_compatibilities(all_encoders, [muxer])[:, 0]
+            mask = self.check_compatibilites(all_encoders, [muxer])[:, 0]
             encoders = set(np.asarray(all_encoders, dtype=object)[mask])
             self.muxers_cache[muxer]["encoders"] = encoders
         return self.muxers_cache[muxer]["encoders"]
 
     def get_muxer_doc(self, muxer: str) -> str:
         r"""
         ** Retrive the ffmpeg documentation of this format. **
+
+        Examples
+        --------
+        >>> from pprint import pprint
+        >>> from movia.core.compilation.export.compatibility import WriteInfos
+        >>> pprint(WriteInfos().get_muxer_doc("ogg"))
+        ('Muxer ogg [Ogg]:\n'
+         '    Common extensions: ogg.\n'
+         '    Mime type: application/ogg.\n'
+         '    Default video codec: theora.\n'
+         '    Default audio codec: vorbis.\n'
+         'Ogg (audio/video/Speex/Opus) muxer AVOptions:\n'
+         '  -serial_offset     <int>        E.......... serial number offset (from 0 '
+         'to INT_MAX) (default 0)\n'
+         '  -oggpagesize       <int>        E.......... Set preferred Ogg page size. '
+         '(from 0 to 65025) (default 0)\n'
+         '  -pagesize          <int>        E.......... preferred page size in bytes '
+         '(deprecated) (from 0 to 65025) (default 0)\n'
+         '  -page_duration     <int64>      E.......... preferred page duration, in '
+         'microseconds (from 0 to I64_MAX) (default 1000000)\n'
+         '\n')
+        >>>
         """
         assert isinstance(muxer, str), muxer.__class__.__name__
         assert muxer in self.muxers, f"{muxer} not in {self.muxers}"
 
         doc = self.muxers_cache[muxer].get("doc") or subprocess.run(
             ["ffmpeg", "-v", "error", "-h", f"muxer={muxer}"],
             capture_output=True, check=True,
@@ -329,36 +349,36 @@
 
     def get_muxers_for_codec(self, codec: str) -> set[str]:
         """
         ** Search all available codecs for a given format. **
 
         Examples
         --------
-        >>> from cutcutcodec.core.compilation.export.compatibility import WriteInfos
+        >>> from movia.core.compilation.export.compatibility import WriteInfos
         >>> sorted(WriteInfos().get_muxers_for_codec("av1")) # doctest +ELLIPSIS
         ['asf', 'asf_stream', 'avi', ..., 'vob', 'webm', 'wtv']
         >>>
         """
         assert isinstance(codec, str), codec.__class__.__name__
         assert codec in self.codecs, f"{codec} not in {self.codecs}"
 
         all_muxers = list(self.muxers)
-        mask = self.check_compatibilities([codec], all_muxers)[0, :]
+        mask = self.check_compatibilites([codec], all_muxers)[0, :]
         muxers = set(np.asarray(all_muxers, dtype=object)[mask])
         self.codecs_cache[codec]["muxers"] = muxers
         return muxers
 
     @property
     def muxers(self) -> set[str]:
         """
         ** Returns all eligible muxers. **
 
         Examples
         --------
-        >>> from cutcutcodec.core.compilation.export.compatibility import WriteInfos
+        >>> from movia.core.compilation.export.compatibility import WriteInfos
         >>> muxers = WriteInfos().muxers
         >>> "ogg" in muxers
         True
         >>> "matroska" in muxers
         True
         >>>
         """
@@ -410,17 +430,17 @@
 
         Notes
         -----
         No real tests are performed, it is just a documentation parsing.
 
         Examples
         --------
-        >>> from cutcutcodec.core.compilation.export.compatibility import CodecInfos
-        >>> sorted(CodecInfos("opus").encoders)
-        ['libopus', 'opus']
+        >>> from movia.core.compilation.export.compatibility import CodecInfos
+        >>> sorted(CodecInfos("av1").encoders)
+        ['libaom-av1', 'librav1e', 'libsvtav1']
         >>>
         """
         return self.infos.codecs_cache[self.name]["encoders"]
 
     @property
     def decoding_supported(self):
         """
@@ -459,15 +479,15 @@
     @property
     def long_name(self) -> str:
         """
         ** The complete verbose long name of the encoder. **
 
         Examples
         --------
-        >>> from cutcutcodec.core.compilation.export.compatibility import CodecInfos
+        >>> from movia.core.compilation.export.compatibility import CodecInfos
         >>> CodecInfos("aac").long_name
         'AAC (Advanced Audio Coding) (decoders: aac aac_fixed )'
         >>>
         """
         return self.infos.codecs_cache[self.name]["long_name"]
 
     @property
@@ -487,15 +507,15 @@
     @property
     def type(self) -> str:
         """
         ** The kind of encodable flux video, audio or subtitle. **
 
         Examples
         --------
-        >>> from cutcutcodec.core.compilation.export.compatibility import CodecInfos
+        >>> from movia.core.compilation.export.compatibility import CodecInfos
         >>> CodecInfos("av1").type
         'video'
         >>> CodecInfos("vorbis").type
         'audio'
         >>> CodecInfos("subrip").type
         'subtitle'
         >>>
@@ -521,36 +541,51 @@
 
         Notes
         -----
         No real tests are performed, it is just a documentation parsing.
 
         Examples
         --------
-        >>> from cutcutcodec.core.compilation.export.compatibility import EncoderInfos
+        >>> from movia.core.compilation.export.compatibility import EncoderInfos
         >>> EncoderInfos("libaom-av1").codec
         'av1'
         >>>
         """
         return self.infos.encoders_cache[self.name]["codec"]
 
     @property
     def doc(self) -> str:
-        """
+        r"""
         ** The ffmpeg documentation about this encoder. **
+
+        Examples
+        --------
+        >>> from pprint import pprint
+        >>> from movia.core.compilation.export.compatibility import EncoderInfos
+        >>> pprint(EncoderInfos("libvorbis").doc)
+        ('Encoder libvorbis [libvorbis]:\n'
+         '    General capabilities: dr1 delay small \n'
+         '    Threading capabilities: none\n'
+         '    Supported sample formats: fltp\n'
+         'libvorbis AVOptions:\n'
+         '  -iblock            <double>     E...A..... Sets the impulse block bias '
+         '(from -15 to 0) (default 0)\n'
+         '\n')
+        >>>
         """
         return self.infos.get_encoder_doc(self.name)
 
     @property
     def experimental(self) -> bool:
         """
         ** True if the encoder is experimental. **
 
         Examples
         --------
-        >>> from cutcutcodec.core.compilation.export.compatibility import EncoderInfos
+        >>> from movia.core.compilation.export.compatibility import EncoderInfos
         >>> EncoderInfos("libx264").experimental
         False
         >>>
         """
         return self.infos.encoders_cache[self.name]["experimental"]
 
     @property
@@ -565,52 +600,35 @@
         ** Get the complete dictionary. **
         """
         return {
             "doc": self.doc,
             "experimental": self.experimental,
             "frame_level_multithreading": self.frame_level_multithreading,
             "long_name": self.long_name,
-            "rates": self.rates,
             "slice_level_multithreading": self.slice_level_multithreading,
             "supports_direct_rendering_method": self.supports_direct_rendering_method,
             "supports_draw_horiz_band": self.supports_draw_horiz_band,
             "type": self.type,
         }
 
     @property
     def long_name(self) -> str:
         """
         ** The complete verbose long name of the encoder. **
 
         Examples
         --------
-        >>> from cutcutcodec.core.compilation.export.compatibility import EncoderInfos
+        >>> from movia.core.compilation.export.compatibility import EncoderInfos
         >>> EncoderInfos("aac").long_name
         'AAC (Advanced Audio Coding)'
         >>>
         """
         return self.infos.encoders_cache[self.name]["long_name"]
 
     @property
-    def rates(self) -> set[int]:
-        """
-        ** The audio compatible sample rates. **
-
-        Examples
-        --------
-        >>> from cutcutcodec.core.compilation.export.compatibility import EncoderInfos
-        >>> sorted(EncoderInfos("libopus").rates)
-        [8000, 12000, 16000, 24000, 48000]
-        >>>
-        """
-        if (match := re.search(r"sample rates: (?P<rates>(?:\d+\s)+)", self.doc)) is None:
-            return set()
-        return set(map(int, match["rates"].split()))
-
-    @property
     def slice_level_multithreading(self) -> bool:
         """
         ** True if the encoder accepts slice level multithreading. **
         """
         return self.infos.encoders_cache[self.name]["slice_level_multithreading"]
 
     @property
@@ -630,18 +648,18 @@
     @property
     def type(self) -> str:
         """
         ** The kind of encodable flux video, audio or subtitle. **
 
         Examples
         --------
-        >>> from cutcutcodec.core.compilation.export.compatibility import EncoderInfos
+        >>> from movia.core.compilation.export.compatibility import EncoderInfos
         >>> EncoderInfos("libaom-av1").type
         'video'
-        >>> EncoderInfos("libopus").type
+        >>> EncoderInfos("libvorbis").type
         'audio'
         >>> EncoderInfos("srt").type
         'subtitle'
         >>>
         """
         return self.infos.encoders_cache[self.name]["type"]
 
@@ -660,68 +678,89 @@
     @property
     def codecs(self) -> set[str]:
         """
         ** Tests all codecs to find the compatibles. **
         """
         return self.infos.get_codecs_for_muxer(self.name)
 
-    def contains_encodecs(self, encodecs: typing.Iterable[str]) -> bool:
+    def contains_codecs(self, codecs: typing.Iterable[str]) -> bool:
         """
         ** Returns True if this muxer support all the given codecs. **
 
         Examples
         --------
-        >>> from cutcutcodec.core.compilation.export.compatibility import MuxerInfos
-        >>> MuxerInfos("ogg").contains_encodecs(["theora", "vorbis"])
+        >>> from movia.core.compilation.export.compatibility import MuxerInfos
+        >>> MuxerInfos("ogg").contains_codecs(["theora", "vorbis"])
         True
-        >>> MuxerInfos("ogg").contains_encodecs(["h264"])
+        >>> MuxerInfos("ogg").contains_codecs(["h264"])
         False
         >>>
         """
-        assert hasattr(encodecs, "__iter__"), encodecs.__class__.__name__
-        encodecs = list(encodecs)
-        assert all(isinstance(e, str) for e in encodecs), encodecs
-        assert set(encodecs).issubset(self.infos.codecs|self.infos.encoders), \
-            set(encodecs)-(self.infos.codecs|self.infos.encoders)
-        return self.infos.check_compatibilities(encodecs, [self.name]).all()
+        assert hasattr(codecs, "__iter__"), codecs.__class__.__name__
+        codecs = list(codecs)
+        assert all(isinstance(codec, str) for codec in codecs), codecs
+        assert set(codecs).issubset(self.infos.codecs), set(codecs)-self.infos.codecs
+        return self.infos.check_compatibilites(codecs, [self.name]).all()
 
     @property
     def default_codecs(self) -> dict[str, str]:
         """
         ** Extract the default codecs from the documentation. **
 
         Notes
         -----
         No real tests are performed, it is just a documentation parsing.
 
         Examples
         --------
         >>> from pprint import pprint
-        >>> from cutcutcodec.core.compilation.export.compatibility import MuxerInfos
+        >>> from movia.core.compilation.export.compatibility import MuxerInfos
         >>> pprint(MuxerInfos("matroska").default_codecs)
         {'audio': 'vorbis', 'subtitle': 'ass', 'video': 'h264'}
         >>>
         """
         pattern = r"Default (?P<type>audio|video|subtitle) codec: (?P<codec>[a-z0-9_\-]{2,})\."
         default = {
             match["type"]: match["codec"] for match in re.finditer(pattern, self.doc)
             if match["codec"] in self.infos.codecs
         }
         if not default:
             return {}
         codecs = list(default.values())
         codecs_rank = {c: i for i, c in enumerate(codecs)}
-        codecs_ok = self.infos.check_compatibilities(codecs, [self.name])[:, 0]
+        codecs_ok = self.infos.check_compatibilites(codecs, [self.name])[:, 0]
         default = {t: c for t, c in default.items() if codecs_ok[codecs_rank[c]]}
         return default
 
     @property
     def doc(self) -> str:
-        """
+        r"""
         ** The ffmpeg documentation about this codec. **
+
+        Examples
+        --------
+        >>> from pprint import pprint
+        >>> from movia.core.compilation.export.compatibility import MuxerInfos
+        >>> pprint(MuxerInfos("ogg").doc)
+        ('Muxer ogg [Ogg]:\n'
+         '    Common extensions: ogg.\n'
+         '    Mime type: application/ogg.\n'
+         '    Default video codec: theora.\n'
+         '    Default audio codec: vorbis.\n'
+         'Ogg (audio/video/Speex/Opus) muxer AVOptions:\n'
+         '  -serial_offset     <int>        E.......... serial number offset (from 0 '
+         'to INT_MAX) (default 0)\n'
+         '  -oggpagesize       <int>        E.......... Set preferred Ogg page size. '
+         '(from 0 to 65025) (default 0)\n'
+         '  -pagesize          <int>        E.......... preferred page size in bytes '
+         '(deprecated) (from 0 to 65025) (default 0)\n'
+         '  -page_duration     <int64>      E.......... preferred page duration, in '
+         'microseconds (from 0 to I64_MAX) (default 1000000)\n'
+         '\n')
+        >>>
         """
         return self.infos.get_muxer_doc(self.name)
 
     @property
     def encoders(self) -> set[str]:
         """
         ** Tests all encoders to find the compatibles. **
@@ -731,15 +770,15 @@
     @property
     def extensions(self) -> set[str]:
         """
         ** Get all suffixs for this format. **
 
         Examples
         --------
-        >>> from cutcutcodec.core.compilation.export.compatibility import MuxerInfos
+        >>> from movia.core.compilation.export.compatibility import MuxerInfos
         >>> MuxerInfos("matroska").extensions
         {'.mkv'}
         >>> sorted(MuxerInfos("mpeg").extensions)
         ['.mpeg', '.mpg']
         >>>
 
         Notes
@@ -765,15 +804,15 @@
         Raises
         ------
         KeyError
             If the extension is not associate to any muxer.
 
         Examples
         --------
-        >>> from cutcutcodec.core.compilation.export.compatibility import MuxerInfos
+        >>> from movia.core.compilation.export.compatibility import MuxerInfos
         >>> MuxerInfos.from_suffix(".mkv").name
         'matroska'
         >>>
         """
         assert isinstance(suffix, str), suffix.__class__.__name__
 
         # get all avalaible extensions
@@ -788,40 +827,25 @@
             raise KeyError(f"{suffix} not in {sorted(all_suffix)}")
         muxers = all_suffix[suffix.lower()]
         if len(muxers) == 1:
             return cls(muxers.pop())
 
         # if we have to choose
         muxers = [cls(name) for name in muxers]
-
-        # 1 choice, if one of the muxer supports only this extension
-        if len(criteria := [m for m in muxers if m.extensions == {suffix}]) == 1:
-            return criteria.pop()
-        if len(criteria) > 0:
-            muxers = criteria
-
-        # 2 choice, the variety of available type.
-        cost = {"audio": 2, "video": 4, "subtitle": 1}
-        best = max(criteria := [{cost[CodecInfos(c).type] for c in m.codecs} for m in muxers])
-        if len(criteria := [m for m, cost in zip(muxers, criteria) if cost == best]) == 1:
-            return criteria.pop()
-        muxers = criteria
-
-        # 3 choice, the number of available codecs
-        best = max(criteria := [len(m.codecs) for m in muxers])
-        if len(criteria := [m for m, cost in zip(muxers, criteria) if cost == best]) == 1:
-            return criteria.pop()
-        muxers = criteria
-
-        # 4 choice, the lenght of the documentation
-        best = max(criteria := [len(m.doc) for m in muxers])
-        if len(criteria := [m for m, cost in zip(muxers, criteria) if cost == best]) == 1:
-            return criteria.pop()
-
-        raise NotImplementedError(f"no more criteria for choose {criteria} for {suffix}")
+        # 1 choice, the number of available codecs
+        criteria = [len(mux.codecs) for mux in muxers]
+        best = max(criteria)
+        if len([c for c in criteria if c == best]) == 1:
+            return muxers[criteria.index(best)]
+        # 2 choice, the lenght of the documentation
+        criteria = [len(mux.doc) for mux in muxers]
+        best = max(criteria)
+        if len([c for c in criteria if c == best]) == 1:
+            return muxers[criteria.index(best)]
+        raise NotImplementedError
 
     def get_all(self) -> dict[str]:
         """
         ** Get the complete dictionary. **
         """
         return {
             "codecs": self.codecs,
@@ -834,13 +858,13 @@
     @property
     def long_name(self) -> str:
         """
         ** The complete verbose long name of the codec. **
 
         Examples
         --------
-        >>> from cutcutcodec.core.compilation.export.compatibility import MuxerInfos
+        >>> from movia.core.compilation.export.compatibility import MuxerInfos
         >>> MuxerInfos("avi").long_name
         'AVI (Audio Video Interleaved)'
         >>>
         """
         return self.infos.muxers_cache[self.name]["long_name"]
```

### Comparing `movia-1.0.0rc1/cutcutcodec/core/compilation/graph_to_ast.py` & `movia-1.0a1/movia/core/compilation/graph_to_ast.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,29 +5,27 @@
 ---------------------------------------------------------------------
 """
 
 import ast
 import inspect
 import pathlib
 import re
-import time
 import unidecode
 
 import networkx
 
-from cutcutcodec.core.classes.container import ContainerOutput
-from cutcutcodec.core.classes.node import Node
-from cutcutcodec.utils import get_project_root
+from movia.core.classes.node import Node
+from movia.utils import get_project_root
 
 
 
 def _node_to_ast(
     node_name: str, graph: networkx.MultiDiGraph
 ) -> tuple[ast.FunctionDef, list[ast.ImportFrom]]:
-    '''
+    """
     ** Creates the ast Function of this node. **
 
     Parameters
     ----------
     node_name : str
         The node name to compile.
     graph : networkx.MultiDiGraph
@@ -35,74 +33,67 @@
 
     Returns
     -------
     func : ast.FunctionDef
         The ast fonction corresponding to the part of this branch,
         including the fourch node or the input node.
     modules : list[ast.ImportFrom]
-        The cutcutcodec modules requiers for this branch.
+        The movia modules requiers for this branch.
 
     Notes
     -----
     * No check for performances reasons.
     * Input / Ouput pickalisable, no modification inplace for alow parralelisation.
 
     Examples
     --------
     >>> import ast
-    >>> from cutcutcodec.core.classes.container import ContainerOutput
-    >>> from cutcutcodec.core.compilation.graph_to_ast import _node_to_ast
-    >>> from cutcutcodec.core.compilation.tree_to_graph import tree_to_graph
-    >>> from cutcutcodec.core.filters.basic.translate import FilterTranslate
-    >>> from cutcutcodec.core.generation.audio.noise import GeneratorAudioNoise
+    >>> from movia.core.classes.container import ContainerOutput
+    >>> from movia.core.compilation.graph_to_ast import _node_to_ast
+    >>> from movia.core.compilation.tree_to_graph import tree_to_graph
+    >>> from movia.core.filters.basic.truncate import FilterTruncate
+    >>> from movia.core.generation.audio.noise import GeneratorAudioNoise
     >>>
     >>> gen = GeneratorAudioNoise.default()
-    >>> filter_2 = FilterTranslate(gen.out_streams, 10)
-    >>> filter_1 = FilterTranslate(filter_2.out_streams, -5)
+    >>> filter_2 = FilterTruncate(gen.out_streams, 10)
+    >>> filter_1 = FilterTruncate(filter_2.out_streams, 1)
     >>> graph = tree_to_graph(ContainerOutput(filter_1.out_streams))
     >>>
     >>> func, modules = _node_to_ast("container_output_1", graph)
     >>> print(ast.unparse(func))
-    def get_container_output_1(filter_translate_1: Node) -> ContainerOutput:
-        """** Creation of the node 'container_output_1'. **"""
+    def get_container_output_1(filter_truncate_1: Node) -> ContainerOutput:
         container_output_1 = ContainerOutput.__new__(ContainerOutput)
-        container_output_1.setstate([filter_translate_1.out_streams[0]], state={})
+        container_output_1.setstate([filter_truncate_1.out_streams[0]], state={})
         return container_output_1
-    >>> func, modules = _node_to_ast("filter_translate_1", graph)
+    >>> func, modules = _node_to_ast("filter_truncate_1", graph)
     >>> print(ast.unparse(func))
-    def get_filter_translate_1(filter_translate_2: Node) -> FilterTranslate:
-        """** Creation of the node 'filter_translate_1'. **"""
-        filter_translate_1 = FilterTranslate.__new__(FilterTranslate)
-        filter_translate_1.setstate([filter_translate_2.out_streams[0]], state={'delay': '-5'})
-        return filter_translate_1
+    def get_filter_truncate_1(filter_truncate_2: Node) -> FilterTruncate:
+        filter_truncate_1 = FilterTruncate.__new__(FilterTruncate)
+        filter_truncate_1.setstate([filter_truncate_2.out_streams[0]], state={'duration_max': '1'})
+        return filter_truncate_1
     >>> func, modules = _node_to_ast("generator_audio_noise_1", graph)
     >>> print(ast.unparse(func))
     def get_generator_audio_noise_1() -> GeneratorAudioNoise:
-        """** Creation of the node 'generator_audio_noise_1'. **"""
         generator_audio_noise_1 = GeneratorAudioNoise.__new__(GeneratorAudioNoise)
         generator_audio_noise_1.setstate([], state={'seed': 0.0})
         return generator_audio_noise_1
     >>>
-    '''
+    """
     modules = []
     body = []
     name = _node_name_to_var_name(node_name)
 
-    # typing annotation returns type and doctring
+    # typing annotaion returns type
     returns = ast.Name(id=graph.nodes[node_name]["class"].__name__, ctx=ast.Load())
     modules.append(_class_to_ast(graph.nodes[node_name]["class"]))
-    body.append(ast.Expr(value=ast.Str(f"** Creation of the node {repr(node_name)}. **")))
 
     # node creation statement
     in_var_index = [
         (_node_name_to_var_name(src), int(key.split("->")[0]))
-        for src, key in sorted(
-            ((src, key) for src, _, key in graph.in_edges(node_name, keys=True)),
-            key=lambda src_key: int(src_key[1].split("->")[1]),
-        )
+        for src, _, key in graph.in_edges(node_name, keys=True)
     ]
     state = ast.parse(repr(graph.nodes[node_name]["state"]), mode="eval").body
     body.append(
         ast.Assign(
             targets=[ast.Name(id=node_name, ctx=ast.Store())],
             value=ast.Call(
                 func=ast.Attribute(
@@ -139,14 +130,15 @@
                             for var, ind in in_var_index
                         ],
                         ctx=ast.Load(),
                     )
                 ],
                 keywords=[ast.keyword(arg="state", value=state)],
             ),
+            type_ignores=[],
         )
     )
 
     # return statement
     body.append(
         ast.Return(value=ast.Name(id=name, ctx=ast.Load()))
     )
@@ -182,37 +174,37 @@
     ----------
     cls : type
         The class to import.
 
     Returns
     -------
     imp : ast.ImportFrom
-        The parsed location of this class in the cutcutcodec module.
+        The parsed location of this class in the movia module.
 
     Raises
     ------
     TypeError
-        If the class is not a cutcutcodec accessible class.
+        If the class is not a movia accessible class.
 
     Examples
     --------
     >>> import ast
-    >>> from cutcutcodec.core.compilation.graph_to_ast import _class_to_ast
-    >>> from cutcutcodec.core.classes.node import Node
+    >>> from movia.core.compilation.graph_to_ast import _class_to_ast
+    >>> from movia.core.classes.node import Node
     >>> print(ast.unparse(_class_to_ast(Node)))
-    from cutcutcodec.core.classes.node import Node
+    from movia.core.classes.node import Node
     >>>
     """
     if (source := inspect.getsourcefile(cls)) is None:
         raise TypeError(f"impossible to locate {cls}")
     source = pathlib.Path(source).resolve()
     root = get_project_root()
     if not source.is_relative_to(root):
-        raise TypeError(f"class {cls} ({source}) is not a cutcutcodec class ({root})")
-    rel_source = "cutcutcodec" / source.relative_to(root)
+        raise TypeError(f"class {cls} ({source}) is not a movia class ({root})")
+    rel_source = "movia" / source.relative_to(root)
     rel_source = rel_source.with_suffix("")
     imp = ast.ImportFrom(
         module=".".join(rel_source.parts), names=[ast.alias(cls.__name__)], level=0
     )
     return imp
 
 
@@ -234,15 +226,15 @@
     -----
     This algorithm is in o(n*log(n)).
 
     Examples
     --------
     >>> import ast
     >>> from pprint import pprint
-    >>> from cutcutcodec.core.compilation.graph_to_ast import _mod_sort_factor
+    >>> from movia.core.compilation.graph_to_ast import _mod_sort_factor
     >>> mods = [
     ...     ast.ImportFrom(module="a.b", names=[ast.alias("f_1")], level=0),
     ...     ast.ImportFrom(module="b", names=[ast.alias("f_2")], level=0),
     ...     ast.ImportFrom(module="b", names=[ast.alias("f_1")], level=0),
     ...     ast.ImportFrom(module="a", names=[ast.alias("f_1")], level=0),
     ...     ast.ImportFrom(module="a", names=[ast.alias("f_2")], level=0),
     ...     ast.ImportFrom(module="a", names=[ast.alias("f_2")], level=0),
@@ -291,15 +283,15 @@
     Returns
     -------
     func_name
         The normalized name in chamel case.
 
     Examples
     --------
-    >>> from cutcutcodec.core.compilation.graph_to_ast import _node_name_to_var_name
+    >>> from movia.core.compilation.graph_to_ast import _node_name_to_var_name
     >>> _node_name_to_var_name("Éléphant  2spaceCamelCase_snake__To")
     'elephant_2space_camel_case_snake_to'
     >>> _node_name_to_var_name("0")
     '_0'
     >>>
     """
     assert isinstance(name, str), name.__class__.__name__
@@ -312,15 +304,15 @@
         name = name.replace("__", "_")
     if name[0].isdigit():
         name = "_" + name
     return name
 
 
 def graph_to_ast(graph: networkx.MultiDiGraph) -> ast.Module:
-    '''
+    """
     ** Creates the complete source code module from the assembly graph. **
 
     Parameters
     ----------
     graph : networkx.MultiDiGraph
         The assembly graph.
 
@@ -329,137 +321,92 @@
     module : ast.Module
         The syntaxical graph of an equivalent code.
         The function ``get_complete_tree`` returns the graph.
 
     Examples
     --------
     >>> import ast
-    >>> from cutcutcodec.core.classes.container import ContainerOutput
-    >>> from cutcutcodec.core.compilation.graph_to_ast import graph_to_ast
-    >>> from cutcutcodec.core.compilation.tree_to_graph import tree_to_graph
-    >>> from cutcutcodec.core.generation.audio.noise import GeneratorAudioNoise
+    >>> from movia.core.classes.container import ContainerOutput
+    >>> from movia.core.compilation.graph_to_ast import graph_to_ast
+    >>> from movia.core.compilation.tree_to_graph import tree_to_graph
+    >>> from movia.core.generation.audio.noise import GeneratorAudioNoise
     >>> graph = tree_to_graph(ContainerOutput(GeneratorAudioNoise.default().out_streams))
     >>> graph_to_ast(graph) # doctest: +ELLIPSIS
     <ast.Module object at ...>
     >>> print(ast.unparse(_))
-    """
-    ** Autogenerated project exportation script. **
-    -----------------------------------------------
-    <BLANKLINE>
-    Creation: ...
-    Graph: MultiDiGraph with 2 nodes and 1 edges
-    """
-    from cutcutcodec.core.classes.container import ContainerOutput
-    from cutcutcodec.core.classes.node import Node
-    from cutcutcodec.core.generation.audio.noise import GeneratorAudioNoise
+    from movia.core.classes.container import ContainerOutput
+    from movia.core.classes.node import Node
+    from movia.core.generation.audio.noise import GeneratorAudioNoise
     <BLANKLINE>
     def get_container_output_1(generator_audio_noise_1: Node) -> ContainerOutput:
-        """** Creation of the node 'container_output_1'. **"""
         container_output_1 = ContainerOutput.__new__(ContainerOutput)
         container_output_1.setstate([generator_audio_noise_1.out_streams[0]], state={})
         return container_output_1
     <BLANKLINE>
     def get_generator_audio_noise_1() -> GeneratorAudioNoise:
-        """** Creation of the node 'generator_audio_noise_1'. **"""
         generator_audio_noise_1 = GeneratorAudioNoise.__new__(GeneratorAudioNoise)
         generator_audio_noise_1.setstate([], state={'seed': 0.0})
         return generator_audio_noise_1
     <BLANKLINE>
     def get_complete_tree() -> ContainerOutput:
-        """** Retrives the complete assembly graph. **"""
         generator_audio_noise_1 = get_generator_audio_noise_1()
         container_output_1 = get_container_output_1(generator_audio_noise_1)
         return container_output_1
     if __name__ == '__main__':
         get_complete_tree().write()
     >>>
-    '''
+    """
     assert isinstance(graph, networkx.MultiDiGraph), graph.__class__.__name__
 
     body = []
     imps = []
 
-    # get_final node_name
-    final_var = [n for n, data in graph.nodes.data() if issubclass(data["class"], ContainerOutput)]
-    if len(final_var) != 1:
-        raise RuntimeError(f"must have exactly one ContainerOutput node, {final_var} founded")
-    final_var = _node_name_to_var_name(final_var.pop())
-
-    # extract each final lines in arbitrary order
-    sequence = [] # (ast_func, in_args_set, out_var)
+    sequence = [] # index 0 -> bottom, output, index final -> top
     for node in sorted(graph): # sorted for repetability
-        ast_func, imp = _node_to_ast(node, graph)
-        body.append(ast_func)
+        func, imp = _node_to_ast(node, graph)
+        body.append(func)
         imps.extend(imp)
-        sequence.append(
-            (
-                ast_func, # ast.FunctionDef
-                {ast_arg.arg for ast_arg in ast_func.args.args}, # set[str], input variable
-                _node_name_to_var_name(node), # str, output variable
-            )
-        )
 
-    # sorted func call position in an executable sequence order o(n**2)
-    sorted_sequence = [] # index final -> bottom, output; index 0 -> top
-    defines_out = set()
-    while sequence:
-        for i, (_, in_args_set, out_var) in enumerate(sequence.copy()):
-            if in_args_set.issubset(defines_out):
-                sorted_sequence.append(sequence.pop(i))
-                defines_out.add(out_var)
-                break
-        else:
-            raise RuntimeError("cycle found")
-        if out_var == final_var:
-            break
+        # locate func call position in an executable sequence order o(n**2)
+        out_var = _node_name_to_var_name(node)
+        ref = 0
+        for i, (_, args, _) in enumerate(sequence):
+            if out_var in args: # if func[i] input need curent node func output
+                ref = i + 1
+        sequence.insert(ref, (func, {ast_arg.arg for ast_arg in func.args.args}, out_var))
 
     # import management and simplification
     imps = _mod_sort_factor(imps)
     body = imps + body
 
     # main func management
     tree_body = []
-    for ast_func, in_args_set, out_var in sorted_sequence:
-        tree_body.append(
+    for func, args, out_var in sequence:
+        tree_body.insert(
+            0,
             ast.Assign(
                 targets=[ast.Name(id=out_var, ctx=ast.Store())],
                 value=ast.Call(
-                    func=ast.Name(id=ast_func.name, ctx=ast.Load()),
-                    args=[ast.Name(id=arg, ctx=ast.Load()) for arg in sorted(in_args_set)],
+                    func=ast.Name(id=func.name, ctx=ast.Load()),
+                    args=[ast.Name(id=arg, ctx=ast.Load()) for arg in sorted(args)],
                     keywords=[],
                 ),
             ),
         )
-    tree_body.append(ast.Return(value=ast.Name(id=sorted_sequence[-1][2], ctx=ast.Load())))
-    tree_body.insert(0, ast.Expr(value=ast.Str("** Retrives the complete assembly graph. **")))
+    tree_body.append(ast.Return(value=ast.Name(id=sequence[0][2], ctx=ast.Load())))
     body.append(
         ast.FunctionDef(
             name="get_complete_tree",
             args=ast.arguments(posonlyargs=[], args=[], kwonlyargs=[], kw_defaults=[], defaults=[]),
             body=tree_body,
             decorator_list=[],
-            returns=sorted_sequence[-1][0].returns,
+            returns=sequence[0][0].returns,
         )
     )
 
-    # doctstring creation
-    body.insert(
-        0,
-        ast.Expr(
-            value=ast.Str(
-                "\n"
-                "** Autogenerated project exportation script. **\n"
-                "-----------------------------------------------\n"
-                "\n"
-                f"Creation: {time.ctime()}\n"
-                f"Graph: {graph}\n"
-            ),
-        ),
-    )
-
     # main script execution
     body.append(
         ast.If(
             test=ast.Compare(
                 left=ast.Name(id="__name__", ctx=ast.Load()),
                 ops=[ast.Eq()],
                 comparators=[ast.Constant(value="__main__")],
```

### Comparing `movia-1.0.0rc1/cutcutcodec/core/compilation/graph_to_tree.py` & `movia-1.0a1/movia/core/compilation/graph_to_tree.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,75 +1,76 @@
 #!/usr/bin/env python3
 
 """
 ** Compile an assembly graph into an evaluable tree **
 ------------------------------------------------------
 """
 
+
 import typing
 
 import networkx
 
-from cutcutcodec.core.classes.container import ContainerOutput
-from cutcutcodec.core.classes.node import Node
-from cutcutcodec.core.classes.stream import Stream
-from cutcutcodec.core.optimisation.cache.clean.graph import clean_graph
+from movia.core.classes.container import ContainerOutput
+from movia.core.classes.node import Node
+from movia.core.classes.stream import Stream
+from movia.core.optimisation.cache.hashes import compute_nodes_hash
 
 
 
 def _tree_from_node(node_name: str, graph: networkx.MultiDiGraph) -> None:
     """
     ** Recursively retrieve the node corresponding to the node of the graph. **
 
     Complete the ``tree`` attribute for this node and for the out streams of this node.
     This function is recursive, so all ancestors are also completed.
 
     Parameters
     ----------
-    node_name : str
+    node : str
         The name of the node that allows to determine the corresponding subgraph.
     graph : networkx.MultiDiGraph
         The complete assembly graph.
 
     Notes
     -----
     If the node is a terminal node, it is the complete dynamic tree.
     """
     assert isinstance(graph, networkx.MultiDiGraph), graph.__class__.__name__
     assert isinstance(node_name, str), node_name.__class__.__name__
-    assert node_name in graph.nodes, sorted(graph.nodes)
+    assert node_name in graph.nodes(), sorted(graph.nodes())
 
     # create node and recursively the parent nodes
     node = graph.nodes[node_name]
-    if "tree" not in node["cache"][1]:
+    if node["tree"] is None:
         for pred in graph.predecessors(node_name):
             _tree_from_node(pred, graph) # editing by pointer
         in_edges = graph.in_edges(node_name, keys=True)
         if sorted(int(k.split("->")[1]) for _, _, k in in_edges) != list(range(len(in_edges))):
             raise IndexError(
                 f"the streams ({in_edges}) arriving on {node_name} are not correctly incremented"
             )
         in_streams = [
-            graph.edges[edge_name]["cache"][1]["tree"] for edge_name in
+            graph.edges[edge_name]["tree"] for edge_name in
             sorted(in_edges, key=lambda src_dst_key: int(src_dst_key[2].split("->")[1]))
         ] # the streams that arrive on the current node
-        node["cache"][1]["tree"] = new_node(node["class"], in_streams, node["state"])
-        assert node["cache"][1]["tree"].in_streams == tuple(in_streams), \
+        node["tree"] = new_node(node["class"], in_streams, node["state"])
+        assert node["tree"].in_streams == tuple(in_streams), \
             f"the node {node_name} does not have the specified input streams"
 
     # complete out streams
     for out_edge_name in graph.out_edges(node_name, keys=True):
         out_edge = graph.edges[out_edge_name]
-        if "tree" not in out_edge["cache"][1]:
+        if out_edge["tree"] is None:
             index = int(out_edge_name[2].split("->")[0])
-            assert index < len(node["cache"][1]["tree"].out_streams), (
-                f"the {out_edge_name[0]} node has only {len(node['cache'][1]['tree'].out_streams)} "
+            assert index < len(node["tree"].out_streams), (
+                f"the {out_edge_name[0]} node has only {len(node['tree'].out_streams)} "
                 f"output streams, impossible to access stream index {index}"
             )
-            out_edge["cache"][1]["tree"] = node["cache"][1]["tree"].out_streams[index]
+            out_edge["tree"] = node["tree"].out_streams[index]
 
 
 def graph_to_tree(graph: networkx.MultiDiGraph) -> ContainerOutput:
     """
     ** Creates the dynamic tree from the assembly graph. **
 
     The abstract dynamic tree alows the evaluation of the complete pipeline.
@@ -77,70 +78,70 @@
     Parameters
     ----------
     graph : networkx.MultiDiGraph
         The assembly graph.
 
     Returns
     -------
-    container_out : cutcutcodec.core.classes.container.ContainerOutput
+    container_out : movia.core.classes.container.ContainerOutput
         An evaluable multimedia muxer.
 
     Examples
     --------
-    >>> from cutcutcodec.core.classes.container import ContainerOutput
-    >>> from cutcutcodec.core.compilation.graph_to_tree import graph_to_tree
-    >>> from cutcutcodec.core.compilation.tree_to_graph import tree_to_graph
-    >>> from cutcutcodec.core.generation.audio.noise import GeneratorAudioNoise
+    >>> from movia.core.classes.container import ContainerOutput
+    >>> from movia.core.compilation.graph_to_tree import graph_to_tree
+    >>> from movia.core.compilation.tree_to_graph import tree_to_graph
+    >>> from movia.core.generation.audio.noise import GeneratorAudioNoise
     >>> tree = tree_to_graph(ContainerOutput(GeneratorAudioNoise.default().out_streams))
     >>> graph_to_tree(tree) # doctest: +ELLIPSIS
-    <cutcutcodec.core.classes.container.ContainerOutput object at ...>
+    <movia.core.classes.container.ContainerOutput object at ...>
     >>>
     """
     # verification and extraction of the termination node
     assert isinstance(graph, networkx.MultiDiGraph), graph.__class__.__name__
     out_nodes = [n for n in graph.nodes if issubclass(graph.nodes[n]["class"], ContainerOutput)]
     assert len(out_nodes) == 1, f"only one output node is possible, not {len(out_nodes)}"
     out_node = out_nodes.pop()
-    assert issubclass(graph.nodes[out_node]["class"], ContainerOutput), \
+    assert issubclass(graph.nodes()[out_node]["class"], ContainerOutput), \
         graph.nodes[out_node]["class"].__name__
 
     # fill
-    update_trees(graph) # compute and add missing "tree" nodes
-    container_out = graph.nodes[out_node]["cache"][1]["tree"]
+    update_tree(graph)
+    container_out = graph.nodes[out_node]["tree"]
     return container_out
 
 
 def new_node(node_class: type, in_streams: typing.Iterable[Stream], state: dict) -> Node:
     """
     ** Instantiates and initializes a new node. **
 
     Parameters
     ----------
     node_class : type
         The uninstantiated class describing the node to be created.
-        This class must be inherited from the ``cutcutcodec.core.classes.node.Node`` class.
+        This class must be inherited from the ``movia.core.classes.node.Node`` class.
     in_streams : typing.Iterable[Stream]
-        See ``cutcutcodec.core.classes.node.Node.setstate``.
+        See ``movia.core.classes.node.Node.setstate``.
     state : dict
-        See ``cutcutcodec.core.classes.node.Node.setstate``.
+        See ``movia.core.classes.node.Node.setstate``.
 
     Returns
     -------
     node : Node
         A new instantiated and initialized node.
     """
     assert isinstance(node_class, type), f"{node_class} must be a class, not an object"
     assert issubclass(node_class, Node), f"{node_class.__name__} class does not inherit from Node"
 
     node = node_class.__new__(node_class)
     node.setstate(in_streams, state)
     return node
 
 
-def update_trees(graph: networkx.MultiDiGraph) -> None:
+def update_tree(graph: networkx.MultiDiGraph) -> None:
     """
     ** Updates on each node the ``tree`` attribute. **
 
     From the assembly graph, this function reconstructs the dynamic instances
     and is able to perform the calculations.
     By adding to each node the attribute ``tree``,
     it allows not only to keep the graph structure but also
@@ -152,47 +153,48 @@
     ----------
     graph : networkx.MultiDiGraph
         The assembly graph who is going to have the updated ``tree`` attributes.
 
     Examples
     --------
     >>> import pprint
-    >>> from cutcutcodec.core.classes.container import ContainerOutput
-    >>> from cutcutcodec.core.compilation.graph_to_tree import update_trees
-    >>> from cutcutcodec.core.compilation.tree_to_graph import tree_to_graph
-    >>> from cutcutcodec.core.filters.basic.truncate import FilterTruncate
-    >>> from cutcutcodec.core.generation.audio.noise import GeneratorAudioNoise
-    >>> container_out = ContainerOutput(
-    ...     FilterTruncate(GeneratorAudioNoise.default().out_streams, 1).out_streams
-    ... )
-    >>> graph = tree_to_graph(container_out)
-    >>> update_trees(graph)
-    >>> pprint.pprint(dict(graph.nodes("cache"))) # doctest: +ELLIPSIS
-    {'container_output_1': ('93c8085e4619bd1d5a04a71e005441f5',
-                            {'tree': <cutcutcodec.core.classes.container.ContainerOutput...>}),
-     'filter_truncate_1': ('8725be07b5f831cf9d9d5e9e7bb5b5ac',
-                           {'tree': <cutcutcodec.core.filters.basic.truncate.FilterTruncate...>}),
-     'generator_audio_noise_1': ('b60c0f567ed5ef0ded54d08ea1f6c80a',
-                                 {'tree': <...GeneratorAudioNoise...>})}
-    >>> pprint.pprint(list(graph.edges(keys=True, data=True))) # doctest: +ELLIPSIS
-    [('filter_truncate_1',
-      'container_output_1',
-      '0->0',
-      {'cache': ('8725be07b5f831cf9d9d5e9e7bb5b5ac|0',
-                 {'tree': <...filters.basic.cut._StreamAudioCut...>})}),
-     ('generator_audio_noise_1',
-      'filter_truncate_1',
-      '0->0',
-      {'cache': ('b60c0f567ed5ef0ded54d08ea1f6c80a|0',
-                 {'tree': <...generation.audio.noise._StreamAudioNoiseUniform...>})})]
+    >>> import networkx as nx
+    >>> from movia.core.classes.container import ContainerOutput
+    >>> from movia.core.compilation.graph_to_tree import update_tree
+    >>> from movia.core.compilation.tree_to_graph import tree_to_graph
+    >>> from movia.core.io.read import ContainerInputFFMPEG
+    >>> with ContainerInputFFMPEG("movia/examples/video.mp4") as container_in:
+    ...     container_out = ContainerOutput(container_in.out_streams)
+    ...     graph = tree_to_graph(container_out)
+    ...
+    >>> pprint.pprint(nx.get_node_attributes(graph, 'tree'))
+    {}
+    >>> pprint.pprint(nx.get_edge_attributes(graph, 'tree'))
+    {}
+    >>> update_tree(graph)
+    >>> pprint.pprint(nx.get_node_attributes(graph, 'tree')) # doctest: +ELLIPSIS
+    {'container_input_ffmpeg_1': <movia.core.io.read.ContainerInputFFMPEG object at ...>,
+     'container_output_1': <movia.core.classes.container.ContainerOutput object at ...>}
+    >>> pprint.pprint(nx.get_edge_attributes(graph, 'tree')) # doctest: +ELLIPSIS
+    {(...): <movia.core.io.read._StreamVideoFFMPEG object at ...>}
     >>>
     """
     assert isinstance(graph, networkx.MultiDiGraph), graph.__class__.__name__
 
-    # delete obsolete cache and create field ["cache"][1]
-    graph = clean_graph(graph)
+    # clean obsolete tree and declaration
+    hashes = compute_nodes_hash(graph)
+    for node_name, new_hash in hashes.items():
+        node = graph.nodes[node_name]
+        if node.get("hash", None) == new_hash: # if hash match
+            for (*edge, tree) in graph.out_edges(node_name, keys=True, data="tree", default=None):
+                graph.add_edge(*edge, tree=tree)
+        else: # obsolete case (need update)
+            node["hash"] = new_hash
+            node["tree"] = None
+            for edge_name in graph.out_edges(node_name, keys=True):
+                graph.add_edge(*edge_name, tree=None)
 
     # complete graph
-    out_nodes = [node for node in graph.nodes if graph.out_degree(node) == 0]
+    out_nodes = [node for node in graph.nodes() if graph.out_degree(node) == 0]
     assert out_nodes, "the graph is empty or contains cycle"
     for node_name in out_nodes:
         _tree_from_node(node_name, graph)
```

### Comparing `movia-1.0.0rc1/cutcutcodec/core/compilation/tree_to_graph.py` & `movia-1.0a1/movia/core/compilation/tree_to_graph.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,65 +1,66 @@
 #!/usr/bin/env python3
 
 """
-** Create the graph from an ``cutcutcodec.core.classes.container.ContainerOutput``. **
+** Create the graph from an ``movia.core.classes.container.ContainerOutput``. **
 --------------------------------------------------------------------------------
 """
 
+
 import re
 
 import networkx
 
-from cutcutcodec.core.classes.container import ContainerOutput
-from cutcutcodec.core.classes.node import Node
+from movia.core.classes.container import ContainerOutput
+from movia.core.classes.node import Node
 
 
 
 def _complete_graph(graph: networkx.MultiDiGraph, node: Node, *, _names: dict) -> None:
     """
     ** Adds to the graph, all nodes and arcs from the provided node. **
 
     This function is recursive.
 
     Parameters
     ----------
     graph : networkx.MultiDiGraph
         The graph on which we add the node.
-    node : cutcutcodec.core.classes.node.Node
+    node : movia.core.classes.node.Node
         The node to add to the graph.
 
     Notes
     -----
     The graph is modified inplace.
     """
     if id(node) in _names:
         if _names[id(node)] in graph:
             return None
 
     current_node_name = _node_name(graph, node, _names=_names)
     graph.add_node(current_node_name, **{"class": node.__class__, "state": node.getstate()})
 
     for index_dst, stream in enumerate(node.in_streams):
-        new_node_name = _node_name(graph, stream.node_main, _names=_names)
-        _complete_graph(graph, stream.node_main, _names=_names)
+        new_node_name = _node_name(graph, stream.node, _names=_names)
+        _complete_graph(graph, stream.node, _names=_names)
         key = f"{stream.index}->{index_dst}"
         graph.add_edge(new_node_name, current_node_name, key)
 
     return None
 
 
 def _node_name(graph: networkx.MultiDiGraph, node: Node, *, _names: dict) -> str:
     """
     ** Find a nice new name to identify the new node in the graph. **
 
     Parameters
     ----------
     graph : networkx.MultiDiGraph
         The graph in which we want to add this new node.
-    node : cutcutcodec.core.classes.node.Node
+    node : movia.core.classes.node.Node
         The node that we want to name.
 
     Returns
     -------
     name : str
         A new name not yet used in the graph.
     """
@@ -79,15 +80,15 @@
     """
     ** Compiles a node in an existing assembly graph context. **
 
     Parameters
     ----------
     graph : networkx.MultiDiGraph
         The graph on which we add the node.
-    node : cutcutcodec.core.classes.node.Node
+    node : movia.core.classes.node.Node
         The node that we want to name and extract properties.
 
     Returns
     -------
     name : str
         The name of the node, this name is not already present in the graph.
     attrs : dict[str]
@@ -96,22 +97,22 @@
     Notes
     -----
     The graph remains unchanged, it is only used for analysis.
 
     Examples
     --------
     >>> from pprint import pprint
-    >>> from cutcutcodec.core.classes.container import ContainerOutput
-    >>> from cutcutcodec.core.compilation.tree_to_graph import tree_to_graph, new_node
-    >>> from cutcutcodec.core.generation.audio.noise import GeneratorAudioNoise
+    >>> from movia.core.classes.container import ContainerOutput
+    >>> from movia.core.compilation.tree_to_graph import tree_to_graph, new_node
+    >>> from movia.core.generation.audio.noise import GeneratorAudioNoise
     >>> node = GeneratorAudioNoise.default()
     >>> graph = tree_to_graph(ContainerOutput(node.out_streams))
     >>> pprint(new_node(graph, node))
     ('generator_audio_noise_2',
-     {'class': <class 'cutcutcodec.core.generation.audio.noise.GeneratorAudioNoise'>,
+     {'class': <class 'movia.core.generation.audio.noise.GeneratorAudioNoise'>,
       'state': {'seed': 0.0}})
     >>>
     """
     assert isinstance(graph, networkx.MultiDiGraph), graph.__class__.__name__
     assert isinstance(node, Node), node.__class__.__name__
 
     name = _node_name(graph, node, _names={})
@@ -125,47 +126,38 @@
     ** Creates the graph from an implicit dynamic tree. **
 
     The generated assembly graph abstracts and simplifies the modification of the pipeline.
     Gives a representation of the assembly tree in the form of a manipulable graph.
 
     Parameters
     ----------
-    container_out : cutcutcodec.core.classes.container.ContainerOutput
+    container_out : movia.core.classes.container.ContainerOutput
         The output of the dynamic graph.
 
     Returns
     -------
     assembly_graph : networkx.MultiDiGraph
         The strictly equivalent assembly graph.
 
     Examples
     --------
     >>> from pprint import pprint
-    >>> from cutcutcodec.core.classes.container import ContainerOutput
-    >>> from cutcutcodec.core.compilation.tree_to_graph import tree_to_graph
-    >>> from cutcutcodec.core.filters.basic.chain import FilterChain
-    >>> from cutcutcodec.core.filters.basic.truncate import FilterTruncate
-    >>> from cutcutcodec.core.generation.audio.noise import GeneratorAudioNoise
-    >>>
-    >>> (s_audio_0,) = FilterTruncate(GeneratorAudioNoise(0).out_streams, 10).out_streams
-    >>> (s_audio_1,) = GeneratorAudioNoise(.5).out_streams
-    >>> (s_chain_audio,) = FilterChain([s_audio_0, s_audio_1]).out_streams
-    >>> graph = tree_to_graph(ContainerOutput([s_chain_audio]))
-    >>>
-    >>> pprint(sorted(graph.nodes))
-    ['container_output_1',
-     'filter_chain_1',
-     'filter_truncate_1',
-     'generator_audio_noise_1',
-     'generator_audio_noise_2']
-    >>> pprint(sorted(graph.edges))
-    [('filter_chain_1', 'container_output_1', '0->0'),
-     ('filter_truncate_1', 'filter_chain_1', '0->0'),
-     ('generator_audio_noise_1', 'filter_truncate_1', '0->0'),
-     ('generator_audio_noise_2', 'filter_chain_1', '0->1')]
+    >>> from movia.core.classes.container import ContainerOutput
+    >>> from movia.core.compilation.graph_to_tree import graph_to_tree
+    >>> from movia.core.compilation.tree_to_graph import tree_to_graph
+    >>> from movia.core.io.read import ContainerInputFFMPEG
+    >>> container_out = ContainerOutput(ContainerInputFFMPEG.default().out_streams)
+    >>> graph = tree_to_graph(container_out)
+    >>> pprint(list(graph.nodes))
+    ['container_output_1', 'container_input_ffmpeg_1']
+    >>> pprint(list(graph.edges))
+    [('container_input_ffmpeg_1', 'container_output_1', '0->0'),
+     ('container_input_ffmpeg_1', 'container_output_1', '1->1'),
+     ('container_input_ffmpeg_1', 'container_output_1', '2->2'),
+     ('container_input_ffmpeg_1', 'container_output_1', '3->3')]
     >>>
     """
     assert isinstance(container_out, ContainerOutput), container_out.__class__.__name__
 
     graph = networkx.MultiDiGraph(title="assembly graph")
     _complete_graph(graph, container_out, _names={})
```

### Comparing `movia-1.0.0rc1/cutcutcodec/core/edit/operation/add.py` & `movia-1.0a1/movia/core/edit/operation/add.py`

 * *Files 4% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     return edge
 
 
 def add_node(graph: networkx.MultiDiGraph, node: str, attrs: dict[str]) -> None:
     """
     ** Adds a node to the graph. **
 
-    The parameters can be compute by ``cutcutcodec.core.compilation.tree_to_graph.new_node``.
+    The parameters can be compute by ``movia.core.compilation.tree_to_graph.new_node``.
 
     Parameters
     ----------
     graph : graph : network.MultiDiGraph
         The assembly graph which does not yet contain the edge to be added.
         The operations on this graph will be performed in-place.
     node : str
```

### Comparing `movia-1.0.0rc1/cutcutcodec/core/edit/operation/remove.py` & `movia-1.0a1/movia/core/edit/operation/remove.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 import networkx
 
 
 
 def remove_edge(
     graph: networkx.MultiDiGraph, edge: tuple[str, str, str]
-) -> dict[tuple[str, str, str], typing.Union[None, tuple[str, str, str]]]:
+) -> dict[tuple[str, str, str], typing.Optional[tuple[str, str, str]]]:
     """
     ** Deletes an edge from the graph. **
 
     Parameters
     ----------
     graph : network.MultiDiGraph
         The assembly graph containing the edge to be deleted.
@@ -36,19 +36,19 @@
     ------
     KeyError
         If the edge is not in the graph.
 
     Examples
     --------
     >>> from pprint import pprint
-    >>> from cutcutcodec.core.classes.container import ContainerOutput
-    >>> from cutcutcodec.core.compilation.tree_to_graph import tree_to_graph
-    >>> from cutcutcodec.core.edit.operation.remove import remove_edge
-    >>> from cutcutcodec.core.io.read import ContainerInputFFMPEG
-    >>> with ContainerInputFFMPEG("cutcutcodec/examples/intro.mkv") as container:
+    >>> from movia.core.classes.container import ContainerOutput
+    >>> from movia.core.compilation.tree_to_graph import tree_to_graph
+    >>> from movia.core.edit.operation.remove import remove_edge
+    >>> from movia.core.io.read import ContainerInputFFMPEG
+    >>> with ContainerInputFFMPEG("movia/examples/intro.mkv") as container:
     ...     tree = ContainerOutput(container.out_streams)
     ...
     >>> graph = tree_to_graph(tree)
     >>> pprint(list(graph.edges))
     [('container_input_ffmpeg_1', 'container_output_1', '0->0'),
      ('container_input_ffmpeg_1', 'container_output_1', '1->1'),
      ('container_input_ffmpeg_1', 'container_output_1', '2->2'),
@@ -89,15 +89,15 @@
         graph.add_edge(*edge_name, **attr)
 
     return transformations
 
 
 def remove_edges(
     graph: networkx.MultiDiGraph, edges: typing.Iterable[tuple[str, str, str]]
-) -> dict[tuple[str, str, str], typing.Union[None, tuple[str, str, str]]]:
+) -> dict[tuple[str, str, str], typing.Optional[tuple[str, str, str]]]:
     """
     ** Deletes several edges from the graph. **
 
     Parameters
     ----------
     graph : network.MultiDiGraph
         The assembly graph containing the edges to be deleted.
@@ -116,19 +116,19 @@
     ------
     KeyError
         If one of the edges is not in the graph.
 
     Examples
     --------
     >>> from pprint import pprint
-    >>> from cutcutcodec.core.classes.container import ContainerOutput
-    >>> from cutcutcodec.core.compilation.tree_to_graph import tree_to_graph
-    >>> from cutcutcodec.core.edit.operation.remove import remove_edges
-    >>> from cutcutcodec.core.io.read import ContainerInputFFMPEG
-    >>> with ContainerInputFFMPEG("cutcutcodec/examples/intro.mkv") as container:
+    >>> from movia.core.classes.container import ContainerOutput
+    >>> from movia.core.compilation.tree_to_graph import tree_to_graph
+    >>> from movia.core.edit.operation.remove import remove_edges
+    >>> from movia.core.io.read import ContainerInputFFMPEG
+    >>> with ContainerInputFFMPEG("movia/examples/intro.mkv") as container:
     ...     tree = ContainerOutput(container.out_streams)
     ...
     >>> graph = tree_to_graph(tree)
     >>> pprint(list(graph.edges))
     [('container_input_ffmpeg_1', 'container_output_1', '0->0'),
      ('container_input_ffmpeg_1', 'container_output_1', '1->1'),
      ('container_input_ffmpeg_1', 'container_output_1', '2->2'),
@@ -175,24 +175,24 @@
     trans = {**{old: new for new, old in inv_trans.items()}, **{el: None for el in del_list}}
 
     return trans
 
 
 def remove_element(
     graph: networkx.MultiDiGraph, element: typing.Union[str, tuple[str, str, str]]
-) -> dict[typing.Union[str, tuple[str, str, str]], typing.Union[None, tuple[str, str, str]]]:
+) -> dict[typing.Union[str, tuple[str, str, str]], typing.Optional[tuple[str, str, str]]]:
     """
-    ** Alias to ``cutcutcodec.core.edit.operation.remove.remove_elements``. **
+    ** Alias to ``movia.core.edit.operation.remove.remove_elements``. **
     """
     return remove_elements(graph, [element])
 
 
 def remove_elements(
     graph: networkx.MultiDiGraph, elements: typing.Iterable[typing.Union[str, tuple[str, str, str]]]
-) -> dict[typing.Union[str, tuple[str, str, str]], typing.Union[None, tuple[str, str, str]]]:
+) -> dict[typing.Union[str, tuple[str, str, str]], typing.Optional[tuple[str, str, str]]]:
     """
     ** Deletes several nodes or edges from the graph. **
 
     Parameters
     ----------
     graph : network.MultiDiGraph
         The assembly graph containing the nodes and edges to be deleted.
@@ -211,21 +211,21 @@
     ------
     KeyError
         If one of the elements is not in the graph.
 
     Examples
     --------
     >>> from pprint import pprint
-    >>> from cutcutcodec.core.classes.container import ContainerOutput
-    >>> from cutcutcodec.core.compilation.tree_to_graph import tree_to_graph
-    >>> from cutcutcodec.core.edit.operation.remove import remove_elements
-    >>> from cutcutcodec.core.io.read import ContainerInputFFMPEG
+    >>> from movia.core.classes.container import ContainerOutput
+    >>> from movia.core.compilation.tree_to_graph import tree_to_graph
+    >>> from movia.core.edit.operation.remove import remove_elements
+    >>> from movia.core.io.read import ContainerInputFFMPEG
     >>> with (
-    ...     ContainerInputFFMPEG("cutcutcodec/examples/intro.mkv") as container_1,
-    ...     ContainerInputFFMPEG("cutcutcodec/examples/intro.mkv") as container_2,
+    ...     ContainerInputFFMPEG("movia/examples/intro.mkv") as container_1,
+    ...     ContainerInputFFMPEG("movia/examples/intro.mkv") as container_2,
     ... ):
     ...     tree = ContainerOutput([*container_1.out_streams, *container_2.out_streams])
     ...
     >>> graph = tree_to_graph(tree)
     >>> pprint(list(graph.edges))
     [('container_input_ffmpeg_1', 'container_output_1', '0->0'),
      ('container_input_ffmpeg_1', 'container_output_1', '1->1'),
@@ -281,15 +281,15 @@
     transformations = {**transformations, **remove_nodes(graph, nodes)}
 
     return transformations
 
 
 def remove_node(
     graph: networkx.MultiDiGraph, node: str
-) -> dict[typing.Union[str, tuple[str, str, str]], typing.Union[None, tuple[str, str, str]]]:
+) -> dict[typing.Union[str, tuple[str, str, str]], typing.Optional[tuple[str, str, str]]]:
     """
     ** Deletes a node from the graph. **
 
     Also deletes the edges linked to this node.
 
     Parameters
     ----------
@@ -310,21 +310,21 @@
     ------
     KeyError
         If the node is not in the graph.
 
     Examples
     --------
     >>> from pprint import pprint
-    >>> from cutcutcodec.core.classes.container import ContainerOutput
-    >>> from cutcutcodec.core.compilation.tree_to_graph import tree_to_graph
-    >>> from cutcutcodec.core.edit.operation.remove import remove_node
-    >>> from cutcutcodec.core.io.read import ContainerInputFFMPEG
+    >>> from movia.core.classes.container import ContainerOutput
+    >>> from movia.core.compilation.tree_to_graph import tree_to_graph
+    >>> from movia.core.edit.operation.remove import remove_node
+    >>> from movia.core.io.read import ContainerInputFFMPEG
     >>> with (
-    ...     ContainerInputFFMPEG("cutcutcodec/examples/intro.mkv") as container_1,
-    ...     ContainerInputFFMPEG("cutcutcodec/examples/intro.mkv") as container_2,
+    ...     ContainerInputFFMPEG("movia/examples/intro.mkv") as container_1,
+    ...     ContainerInputFFMPEG("movia/examples/intro.mkv") as container_2,
     ... ):
     ...     tree = ContainerOutput([*container_1.out_streams, *container_2.out_streams])
     ...
     >>> graph = tree_to_graph(tree)
     >>> pprint(list(graph.edges))
     [('container_input_ffmpeg_1', 'container_output_1', '0->0'),
      ('container_input_ffmpeg_1', 'container_output_1', '1->1'),
@@ -375,15 +375,15 @@
     graph.remove_node(node)
 
     return transformations
 
 
 def remove_nodes(
     graph: networkx.MultiDiGraph, nodes: typing.Iterable[str]
-) -> dict[typing.Union[str, tuple[str, str, str]], typing.Union[None, tuple[str, str, str]]]:
+) -> dict[typing.Union[str, tuple[str, str, str]], typing.Optional[tuple[str, str, str]]]:
     """
     ** Deletes several nodes from the graph. **
 
     Parameters
     ----------
     graph : network.MultiDiGraph
         The assembly graph containing the nodes to be deleted.
@@ -402,22 +402,22 @@
     ------
     KeyError
         If one of the nodes is not in the graph.
 
     Examples
     --------
     >>> from pprint import pprint
-    >>> from cutcutcodec.core.classes.container import ContainerOutput
-    >>> from cutcutcodec.core.compilation.tree_to_graph import tree_to_graph
-    >>> from cutcutcodec.core.edit.operation.remove import remove_nodes
-    >>> from cutcutcodec.core.io.read import ContainerInputFFMPEG
+    >>> from movia.core.classes.container import ContainerOutput
+    >>> from movia.core.compilation.tree_to_graph import tree_to_graph
+    >>> from movia.core.edit.operation.remove import remove_nodes
+    >>> from movia.core.io.read import ContainerInputFFMPEG
     >>> with (
-    ...     ContainerInputFFMPEG("cutcutcodec/examples/intro.mkv") as container_1,
-    ...     ContainerInputFFMPEG("cutcutcodec/examples/intro.mkv") as container_2,
-    ...     ContainerInputFFMPEG("cutcutcodec/examples/intro.mkv") as container_3,
+    ...     ContainerInputFFMPEG("movia/examples/intro.mkv") as container_1,
+    ...     ContainerInputFFMPEG("movia/examples/intro.mkv") as container_2,
+    ...     ContainerInputFFMPEG("movia/examples/intro.mkv") as container_3,
     ... ):
     ...     tree = ContainerOutput(
     ...         [*container_1.out_streams, *container_2.out_streams, *container_3.out_streams]
     ...     )
     ...
     >>> graph = tree_to_graph(tree)
     >>> pprint(list(graph.edges))
```

### Comparing `movia-1.0.0rc1/cutcutcodec/core/exceptions.py` & `movia-1.0a1/movia/core/exceptions.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,57 +1,45 @@
 #!/usr/bin/env python3
 
 """
-** Groups the exceptions specific to ``cutcutcodec``. **
+** Groups the exceptions specific to ``movia``. **
 --------------------------------------------------
 
 Rather than returning too general exceptions, these exceptions allow a much more precise debugging.
 """
 
 
-
-class CutcutcodecException(Exception):
+class MoviaException(Exception):
     """
     ** Base class for exceptions specific to this module. **
     """
 
-
-class MissingFrameError(CutcutcodecException, OSError):
+class MissingFrameError(MoviaException, OSError):
     """
     ** When a frame is missing in a stream. **
 
     This exception can be thrown if the reded frames have a strange behavior.
     """
 
-
-class MissingInformation(CutcutcodecException, ValueError):
+class MissingInformation(MoviaException, ValueError):
     """
     ** When information is unreadable or missing from the metadata. **
 
     It can be raised when trying to access a tag that is not defined
     or that returns a surprising value.
     """
 
-
-class MissingStreamError(CutcutcodecException, OSError):
+class MissingStreamError(MoviaException, OSError):
     """
     ** When a stream is missing in a file. **
 
     This exception can be raised when looking for a video,
     audio or image stream in a media that does not contain any or that is unreadable.
     """
 
-
-class OutOfTimeRange(CutcutcodecException, EOFError):
+class OutOfTimeRange(MoviaException, EOFError):
     """
     ** Access outside the definition range **
 
     This exception is raised when accessing or writing
     outside the range in which the stream is defined.
     """
-
-class IncompatibleSettings(CutcutcodecException, RuntimeError):
-    """
-    ** When parameters are incompatible with each other. **
-
-    This exception may mean that a choice is not possible.
-    """
```

### Comparing `movia-1.0.0rc1/cutcutcodec/core/generation/audio/empty.py` & `movia-1.0a1/movia/core/generation/video/empty.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,77 +1,81 @@
 #!/usr/bin/env python3
 
 """
-** Dedicated to tests, it is an empty audio stream containing no samples. **
-----------------------------------------------------------------------------
+** Dedicated to tests, it is an empty video stream containing no frames. **
+---------------------------------------------------------------------------
 """
 
-from fractions import Fraction
+
+import numbers
 import typing
 
-from cutcutcodec.core.classes.container import ContainerInput
-from cutcutcodec.core.classes.frame_audio import FrameAudio
-from cutcutcodec.core.classes.stream import Stream
-from cutcutcodec.core.classes.stream_audio import StreamAudio
-from cutcutcodec.core.exceptions import OutOfTimeRange
+import av
+
+from movia.core.classes.container import ContainerInput
+from movia.core.classes.stream import Stream
+from movia.core.classes.stream_video import StreamVideo
+from movia.core.exceptions import OutOfTimeRange
 
 
 
-class GeneratorAudioEmpty(ContainerInput):
+class GeneratorVideoEmpty(ContainerInput):
     """
-    ** Contains an empty audio stream. **
+    ** Contains an empty video stream. **
 
     Examples
     --------
-    >>> from cutcutcodec.core.exceptions import OutOfTimeRange
-    >>> from cutcutcodec.core.generation.audio.empty import GeneratorAudioEmpty
-    >>> (stream,) = GeneratorAudioEmpty().out_streams
+    >>> from movia.core.exceptions import OutOfTimeRange
+    >>> from movia.core.generation.video.empty import GeneratorVideoEmpty
+    >>> (stream,) = GeneratorVideoEmpty().out_streams
     >>> try:
-    ...     stream.snapshot(0)
+    ...     _ = stream.snapshot(0)
+    ...     print("unreachable")
     ... except OutOfTimeRange as err:
     ...     print(err)
     ...
-    this stream does not contain any samples
+    this stream does not contain any frames
     >>>
     """
 
     def __init__(self):
-        out_streams = [_StreamAudioEmpty(self)]
+        out_streams = [_StreamVideoEmpty(self)]
         super().__init__(out_streams)
 
     @classmethod
     def default(cls):
         return cls()
 
     def getstate(self) -> dict:
         return {}
 
     def setstate(self, in_streams: typing.Iterable[Stream], state: dict) -> None:
         assert state == {}, state
-        GeneratorAudioEmpty.__init__(self)
+        GeneratorVideoEmpty.__init__(self)
 
 
-class _StreamAudioEmpty(StreamAudio):
+class _StreamVideoEmpty(StreamVideo):
     """
-    ** An audio stream containing no sample. **
+    ** A video stream containing no frames. **
     """
 
-    is_time_continuous = True
+    is_space_continuous = False
+    is_time_continuous = False
 
-    def __init__(self, node: GeneratorAudioEmpty):
-        assert isinstance(node, GeneratorAudioEmpty), node.__class__.__name__
+    def __init__(self, node: GeneratorVideoEmpty):
+        assert isinstance(node, GeneratorVideoEmpty), node.__class__.__name__
         super().__init__(node)
 
-    def _snapshot(self, timestamp: Fraction, rate: int, samples: int) -> FrameAudio:
-        raise OutOfTimeRange("this stream does not contain any samples")
+    def _snapshot(self, timestamp: float) -> av.video.frame.VideoFrame:
+        raise OutOfTimeRange("this stream does not contain any frames")
 
     @property
-    def beginning(self) -> Fraction:
-        return Fraction(0)
+    def duration(self) -> numbers.Real:
+        return 0
 
     @property
-    def channels(self) -> int:
-        raise KeyError("it makes no sense to give a number of channels to an absence of sample")
+    def height(self) -> int:
+        raise KeyError("it makes no sense to give a dimension to an absence of frames")
 
     @property
-    def duration(self) -> typing.Union[Fraction, float]:
-        return Fraction(0)
+    def width(self) -> int:
+        raise KeyError("it makes no sense to give a dimension to an absence of frames")
```

### Comparing `movia-1.0.0rc1/cutcutcodec/core/generation/video/empty.py` & `movia-1.0a1/movia/core/generation/audio/empty.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,74 +1,76 @@
 #!/usr/bin/env python3
 
 """
-** Dedicated to tests, it is an empty video stream containing no frames. **
----------------------------------------------------------------------------
+** Dedicated to tests, it is an empty audio stream containing no samples. **
+----------------------------------------------------------------------------
 """
 
-from fractions import Fraction
+
+import numbers
 import typing
 
-from cutcutcodec.core.classes.container import ContainerInput
-from cutcutcodec.core.classes.frame_video import FrameVideo
-from cutcutcodec.core.classes.stream import Stream
-from cutcutcodec.core.classes.stream_video import StreamVideo
-from cutcutcodec.core.exceptions import OutOfTimeRange
+import numpy as np
+
+from movia.core.classes.container import ContainerInput
+from movia.core.classes.stream import Stream
+from movia.core.classes.stream_audio import StreamAudio
+from movia.core.exceptions import OutOfTimeRange
 
 
 
-class GeneratorVideoEmpty(ContainerInput):
+class GeneratorAudioEmpty(ContainerInput):
     """
-    ** Contains an empty video stream. **
+    ** Contains an empty audio stream. **
 
     Examples
     --------
-    >>> from cutcutcodec.core.exceptions import OutOfTimeRange
-    >>> from cutcutcodec.core.generation.video.empty import GeneratorVideoEmpty
-    >>> (stream,) = GeneratorVideoEmpty().out_streams
+    >>> from movia.core.exceptions import OutOfTimeRange
+    >>> from movia.core.generation.audio.empty import GeneratorAudioEmpty
+    >>> (stream,) = GeneratorAudioEmpty().out_streams
     >>> try:
-    ...     stream.snapshot(0, (1, 1))
+    ...     _ = stream.snapshot(0)
+    ...     print("unreachable")
     ... except OutOfTimeRange as err:
     ...     print(err)
     ...
-    this stream does not contain any frames
+    this stream does not contain any samples
     >>>
     """
 
     def __init__(self):
-        out_streams = [_StreamVideoEmpty(self)]
+        out_streams = [_StreamAudioEmpty(self)]
         super().__init__(out_streams)
 
     @classmethod
     def default(cls):
         return cls()
 
     def getstate(self) -> dict:
         return {}
 
     def setstate(self, in_streams: typing.Iterable[Stream], state: dict) -> None:
         assert state == {}, state
-        GeneratorVideoEmpty.__init__(self)
+        GeneratorAudioEmpty.__init__(self)
 
 
-class _StreamVideoEmpty(StreamVideo):
+class _StreamAudioEmpty(StreamAudio):
     """
-    ** A video stream containing no frames. **
+    ** An audio stream containing no sample. **
     """
 
-    is_space_continuous = False
-    is_time_continuous = False
+    is_time_continuous = True
 
-    def __init__(self, node: GeneratorVideoEmpty):
-        assert isinstance(node, GeneratorVideoEmpty), node.__class__.__name__
+    def __init__(self, node: GeneratorAudioEmpty):
+        assert isinstance(node, GeneratorAudioEmpty), node.__class__.__name__
         super().__init__(node)
 
-    def _snapshot(self, timestamp: Fraction, shape: tuple[int, int]) -> FrameVideo:
-        raise OutOfTimeRange("this stream does not contain any frames")
+    def _snapshot(self, timestamp: np.ndarray[numbers.Real]) -> np.ndarray[numbers.Real]:
+        raise OutOfTimeRange("this stream does not contain any samples")
 
     @property
-    def beginning(self) -> Fraction:
-        return Fraction(0)
+    def channels(self) -> int:
+        raise KeyError("it makes no sense to give a number of channels to an absence of sample")
 
     @property
-    def duration(self) -> typing.Union[Fraction, float]:
-        return Fraction(0)
+    def duration(self) -> numbers.Real:
+        return 0
```

### Comparing `movia-1.0.0rc1/cutcutcodec/core/io/read.py` & `movia-1.0a1/movia/core/io/read.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,33 @@
 #!/usr/bin/env python3
 
 """
 ** Decodes the streams of a multimedia file based on ffmpeg. **
 ---------------------------------------------------------------
 """
 
-from fractions import Fraction
-import logging
-import math
+
+import fractions
 import numbers
 import pathlib
-import threading
 import typing
 
 import av
 import numpy as np
-import torch
 
-from cutcutcodec.core.analysis.audio.properties.duration import get_duration_audio
-from cutcutcodec.core.analysis.ffprobe import _estimate_rate_ffmpeg
-from cutcutcodec.core.analysis.ffprobe import get_streams_type
-from cutcutcodec.core.classes.container import ContainerInput
-from cutcutcodec.core.classes.frame_audio import FrameAudio
-from cutcutcodec.core.classes.frame_video import FrameVideo
-from cutcutcodec.core.classes.stream import Stream
-from cutcutcodec.core.classes.stream_audio import StreamAudio
-from cutcutcodec.core.classes.stream_video import StreamVideo
-from cutcutcodec.core.exceptions import MissingInformation, MissingStreamError, OutOfTimeRange
-from cutcutcodec.core.filters.basic.resize import resize_keep_ratio
-from cutcutcodec.utils import get_project_root
+from movia.core.analysis.streams import get_streams_type
+from movia.core.analysis.video.properties.framerate import get_fps
+from movia.core.analysis.video.properties.nb_frames import get_nb_frames
+from movia.core.classes.container import ContainerInput
+from movia.core.classes.stream import Stream
+from movia.core.classes.stream_audio import StreamAudio
+from movia.core.classes.stream_video import StreamVideo
+from movia.core.exceptions import (MissingInformation, MissingFrameError, MissingStreamError,
+    OutOfTimeRange)
+from movia.utils import get_project_root
 
 
 
 class ContainerInputFFMPEG(ContainerInput):
     """
     ** Allows to decode a multimedia file with ffmpeg. **
 
@@ -49,27 +44,30 @@
         ``av.error.InvalidDataError: [Errno 1094995529] Invalid data found when processing input;
         last error log: [libdav1d] Error parsing OBU data``
     Which happens when reading a multi-stream file sparingly, The instances of
     ``av.container.InputContainer`` are new for each stream.
 
     Examples
     --------
-    >>> from cutcutcodec.core.io.read import ContainerInputFFMPEG
-    >>> with ContainerInputFFMPEG("cutcutcodec/examples/intro.mkv") as container:
+    >>> import numpy as np
+    >>> from movia.core.classes.stream_audio import StreamAudio
+    >>> from movia.core.classes.stream_video import StreamVideo
+    >>> from movia.core.io.read import ContainerInputFFMPEG
+    >>> with ContainerInputFFMPEG("movia/examples/intro.mkv") as container:
     ...     for stream in container.out_streams:
-    ...         if stream.type == "video":
-    ...             stream.snapshot(0, (stream.height, stream.width)).shape
-    ...         elif stream.type == "audio":
-    ...             stream.snapshot(0, rate=2, samples=3)
+    ...         if isinstance(stream, StreamVideo):
+    ...             stream.snapshot(0).format
+    ...         if isinstance(stream, StreamAudio):
+    ...             stream.snapshot(np.array([0.0, 1.0]))
     ...
-    (720, 1280, 3)
-    (360, 640, 3)
-    FrameAudio(Fraction(0, 1), 2, [[        nan  0.18039602 -0.34764948]
-                                   [        nan -0.07235986  0.07892987]])
-    FrameAudio(Fraction(0, 1), 2, [[        nan  0.06998454 -0.24758172]])
+    <av.VideoFormat yuv420p, 1280x720>
+    <av.VideoFormat yuv420p, 640x360>
+    array([[        nan, -0.34764948],
+           [        nan,  0.07892987]], dtype=float32)
+    array([[        nan, -0.24758172]], dtype=float32)
     >>>
     """
 
     def __init__(self, filename: typing.Union[str, bytes, pathlib.Path], **av_kwargs):
         """
         Parameters
         ----------
@@ -133,15 +131,15 @@
         ContainerInputFFMPEG.__init__(self, state["filename"], **state["av_kwargs"])
 
     def close(self):
         """
         ** Close the file. **
         """
         for stream in self.out_streams:
-            stream.reset()
+            stream.close()
 
     @property
     def av_kwargs(self) -> dict[str]:
         """
         ** The parameters passed to ``av.open``. **
         """
         return self._av_kwargs
@@ -150,674 +148,692 @@
     def filename(self) -> pathlib.Path:
         """
         ** The path to the physical file that contains the extracted video stream. **
         """
         return self._filename
 
 
-class _StreamFFMPEGBase(Stream):
+class _StreamAudioFFMPEG(StreamAudio):
     """
-    ** Factorise share methods between audio and video. **
+    Attributes
+    ----------
+    duration : numbers.Real
+        The exact duration of the stream (readonly).
+        This date corresponds to the end of the last sample.
+    metadata : dict
+        The metadata associated with this stream (readonly).
+    samplerate : int
+        The frequency in Hz of the samples (readonly).
+    time_base : fractions.Fraction
+        The unit of time (in fractional seconds) in which timestamps are expressed (readonly).
     """
 
     is_time_continuous = False
 
     def __init__(self, node: ContainerInputFFMPEG):
         """
         Parameters
         ----------
-        node : cutcutcodec.core.io.read.ContainerInputFFMPEG
+        node : movia.core.io.read.ContainerInputFFMPEG
             Simply allows to keep the graph structure.
         """
         assert isinstance(node, ContainerInputFFMPEG), node.__class__.__name__
         super().__init__(node)
 
         self._av_container = None
-        self._duration = None
-        self._frame_iter = None
+        self._frame_iter = None # we can't recreate it every time because we lose the last frames
+        self._array_buff = [None, None]
         self._prec_frame = self._next_frame = None
-        self._rate = None # optimise about 100 ms par call
+        self._duration = None
 
-    def _seek_backward(self, position: Fraction) -> None:
+    def __iter__(self):
         """
-        ** Moves backwards in the file. **
-
-        This method guarantees to move before the required position.
-        If this is not possible, we move to the very beginning of the file.
-        After, we always have ``self.get_current_range()[0] <= position``.
+        ** Yields all frames and array of this stream starting from the current position. **
         """
-        if self.type == "audio":
-            dec = Fraction(self.av_container.streams[self.index].frame_size, self.rate)
-        elif self.type == "video":
-            dec = 1 / self.rate
-        else:
-            dec = 0
-        for pos in (position, position-10, 0):
-            stream = self.av_container.streams[self.index] # must be define in 'for' because reset
+        if self._prec_frame is None:
+            self._update_prec_next()
+        yield self._prec_frame, self._extract_array_prec()
+        if self._next_frame is not self._prec_frame:
+            yield self._next_frame, self._extract_array_next()
+        while True:
             try:
-                self.av_container.seek(
-                    max(0, math.floor((pos - 2*dec) / stream.time_base)),
-                    backward=True, # if there is not a keyframe at the given offset
-                    stream=stream
-                )
-            except av.error.PermissionError: # happens sometimes
-                self.reset()
+                yield self._update_prec_next(), self._extract_array_next()
+            except OutOfTimeRange:
                 break
-            self._prec_frame = self._next_frame = None # takes into account the new position
 
-            # verification and rough adjustment
-            try:
-                if self.get_current_range()[0] <= position:
-                    break
-            except OutOfTimeRange: # if this exception is throw, reset is just done
-                continue
-        else:
-            self.reset()
+    def _extract_array_next(self):
+        if self._array_buff[1] is None:
+            self._array_buff[1] = _clip_convert(self._next_frame.to_ndarray(format="bgr24"))
+        return self._array_buff[1]
+
+    def _extract_array_prec(self):
+        if self._array_buff[0] is None:
+            if self._prec_frame is None:
+                self._update_prec_next()
+            self._array_buff[0] = _clip_convert(self._prec_frame.to_ndarray(format="bgr24"))
+        return self._array_buff[0]
 
-    def _seek_forward(self, position: Fraction) -> None:
+    def _seek_backward(self, position: numbers.Real):
         """
-        ** Moves forwardwards in the file. **
+        ** Moves backwards in the file. **
 
-        The displacement, if some cases, can be very approximate.
+        This method guarantees to move before the required position.
+        If this is not possible, we move to the very beginning of the file.
         """
-        stream = self.av_container.streams[self.index]
-        if stream.type == "audio":
-            dec = Fraction(stream.frame_size, self.rate)
-        elif stream.type == "video":
-            dec = 1 / self.rate
-        else:
-            dec = 0
+        if self._prec_frame is None:
+            self._update_prec_next()
+
+        # adjusted displacement
+        seek_request = max(0, int(
+            (position - self._prec_frame.samples/self._prec_frame.rate)
+            / self._prec_frame.time_base
+        ))
         self.av_container.seek(
-            max(0, math.floor((position - dec) / stream.time_base)),
+            seek_request,
             backward=True, # if there is not a keyframe at the given offset
-            stream=stream
+            stream=self.av_container.streams[self.index]
         )
-        self._prec_frame = self._next_frame = None # takes into account the new position
+        self._frame_iter = None # takes into account the new position
+        self._array_buff = [None, None]
+        self._prec_frame = self._next_frame = None
+        self._update_prec_next()
 
-    @property
-    def av_container(self) -> av.container.Container:
+        # verification and rough adjustment
+        if seek_request != 0:
+            if position > _frame_dates(self._prec_frame)[0]:
+                self._seek_backward(0)
+
+    def _seek_forward(self, position: numbers.Real):
         """
-        ** Allows to read the file at the last moment. **
+        ** Moves forwardwards in the file. **
+
+        The displacement, if any, can be very approximate.
         """
-        if self._av_container is None:
-            self._av_container = av.open(str(self.node.filename), "r", **self.node.av_kwargs)
-        return self._av_container
+        self.av_container.seek(
+            max(0, round(position)),
+            backward=True, # if there is not a keyframe at the given offset
+            stream=self.av_container.streams[self.index]
+        )
 
-    @property
-    def beginning(self) -> Fraction:
-        return Fraction(0)
+    def _snapshot(self, timestamp: np.ndarray[numbers.Real]) -> np.ndarray[numbers.Real]:
+        # borns extraction and simple verification
+        # must be accurate to avoid confusion for the final time
+        t_min = np.min(timestamp)
+        t_max = np.max(timestamp)
+        t_max = fractions.Fraction(t_max).limit_denominator(self.time_base.denominator)
+
+        # seeking if nescessary
+        self.seek(t_min) # seeks only for backward or big forward jump
+
+        # retrive and decode reference samples
+        references = []
+        for frame, array in self:
+            references.append((frame.is_corrupt, _frame_dates(frame), frame.rate, array))
+            if references[-1][1][1] > t_max + self.time_base: # a sample covers [t0, t0+dt[
+                break
+        else: # if the last frame is reached
+            if t_max >= references[-1][1][1]:
+                raise OutOfTimeRange(
+                    f"there is no audio frame at timestamp {t_max} "
+                    f"(need timestamp < {_frame_dates(self._next_frame)[1]})"
+                )
 
-    @property
-    def frame_iter(self) -> typing.Iterable[av.audio.frame.AudioFrame]:
-        """
-        ** Allows to read the file at the last moment. **
-        """
-        if self._frame_iter is None:
-            self._frame_iter = iter(self.av_container.decode(self.av_container.streams[self.index]))
-        return self._frame_iter
+        # verifications
+        if any(is_corrupt for is_corrupt, _, _, _ in references):
+            raise NotImplementedError("an audio frame is corrupted, this case is not handled")
+        if any(rate != self.samplerate for _, _, rate, _ in references):
+            raise NotImplementedError(f"samplerate ({self.samplerate}) doesn't match the frames")
+        cum_shifts = np.cumsum( # cumulative algebraic shifts
+            [
+                tf_prec-ti_next # the algebraic shifts
+                for (_, (_, tf_prec), _, _), (_, (ti_next, _), _, _)
+                in zip(references[:-1], references[1:])
+            ]
+        )
+        if any(np.abs(cum_shifts) >= self._av_container.streams[self.index].time_base):
+            raise MissingFrameError(
+                "there seems to be a gap between some frames, "
+                "here are the cumulative shifts between frames "
+                f"({', '.join(f'{s}={float(s):.4f}' for s in cum_shifts)})"
+            )
 
-    @property
-    def next_frame(self) -> typing.Union[None, av.audio.frame.AudioFrame]:
-        """
-        ** The next frame if exists, None else. **
-        """
-        if self._next_frame is None:
-            self._prec_frame = self.prec_frame # iter if needed ("=" is for pylint W0104)
-            try:
-                self._next_frame = next(self.frame_iter)
-            except (StopIteration, av.error.EOFError):
-                self._next_frame = self._frame_iter = None
-                if self._duration is None: # facultative, it is just optimisation
-                    t_start, t_end = frame_dates(self._prec_frame)
-                    self._duration = t_start + Fraction(1, self.rate) if t_end is None else t_end
-        return self._next_frame
+        # assembling references and get the nerest reference
+        t_ref = float(references[0][1][0])
+        samples_ref = np.concatenate([s for _, _, _, s in references], axis=1)
+        indexs = np.rint((timestamp-t_ref)*self.samplerate).astype(int) # not floor float inaccuracy
+        np.maximum(indexs, 0, out=indexs) # some stream doesn't start at t=0
+        np.minimum(indexs, samples_ref.shape[1]-1, out=indexs) # prevention agains IndexError
+        samples = np.where(timestamp<t_ref, np.nan, samples_ref[:, indexs])
+        return samples
+
+    def _update_prec_next(self) -> av.audio.frame.AudioFrame:
+        """
+        ** Iterates on the next audio frame. **
+
+        Returns
+        -------
+        _next_frame : av.audio.frame.AudioFrame
+            The newly decoded frame.
 
-    @property
-    def prec_frame(self) -> av.audio.frame.AudioFrame:
-        """
-        ** The frame at the current position. **
+        Raises
+        ------
+        OutOfTimeRange
+            If the last audio frame has already been reached.
         """
+        self._prec_frame, self._array_buff[0] = self._next_frame, self._array_buff[1]
+        try:
+            self._next_frame = next(self.frame_iter)
+        except StopIteration as err:
+            raise OutOfTimeRange("there is no audio frame left to read") from err
+        self._array_buff[1] = None
         if self._prec_frame is None:
-            try:
-                self._prec_frame = next(self.frame_iter)
-            except (StopIteration, av.error.EOFError) as err:
-                self.reset()
-                raise OutOfTimeRange("there is no frame left to read") from err
-        return self._prec_frame
+            self._prec_frame = self._next_frame
+        return self._next_frame
 
     @property
-    def rate(self) -> Fraction:
-        """
-        ** Theorical image or sample frequency in the metadata. **
-        """
-        if self._rate is None:
-            self._rate = _estimate_rate_ffmpeg(self.node.filename, self.index)
-        return self._rate
-
-    def reset(self) -> None:
+    def av_container(self) -> av.container.Container:
         """
-        ** Close the file and delete all internal state. **
+        ** Allows to read the file at the last moment. **
         """
-        if self._av_container is not None:
-            self._prec_frame = self._next_frame = None
-            self._frame_iter = None
-            self._av_container.close()
-            self._av_container = None
-
-
-class _StreamAudioFFMPEG(StreamAudio, _StreamFFMPEGBase):
-    """
-    Attributes
-    ----------
-    duration : Fraction
-        The exact duration of the stream (readonly).
-        This date corresponds to the end of the last sample.
-    rate : int
-        The frequency in Hz of the samples (readonly).
-    """
-
-    def __init__(self, node: ContainerInputFFMPEG):
-        super().__init__(node)
-        self._duration = None
-        self._lock = threading.Lock()
-
-    def _snapshot(self, timestamp: Fraction, rate: int, samples: int) -> FrameAudio:
-        if timestamp < 0:
-            raise OutOfTimeRange(f"there is no audio frame at timestamp {timestamp} (need >= 0)")
-
-        # resample if needeed
-        if samples != 1 and rate != self.rate:
-            frame = self._snapshot(
-                timestamp,
-                rate=self.rate,
-                samples=math.floor(samples*Fraction(self.rate, rate))
-            )
-            indexs = torch.arange(samples, dtype=torch.int64)
-            indexs *= self.rate
-            indexs //= rate
-            frame = FrameAudio(timestamp, rate, frame[:, indexs])
-            return frame
-
-        # decode concerned frames
-        slices = []
-        end = timestamp + Fraction(samples, rate) # apparition of last sample
-        with self._lock:
-            self.seek(timestamp)
-            while True:
-                try:
-                    prec_frame = self.prec_frame
-                except OutOfTimeRange as err:
-                    raise OutOfTimeRange(
-                        f"stream start {self.beginning} and end {self.beginning + self.duration}, "
-                        f"no stream at timestamp {timestamp} to {timestamp} + {samples}/{rate}"
-                    ) from err
-                if prec_frame.is_corrupt:
-                    logging.warning("the frame at %f seconds is corrupted", prec_frame.time)
-                    continue
-                dates = frame_dates(prec_frame)
-                slices.append((dates[0], prec_frame.to_ndarray()))
-                if end <= dates[1]:
-                    break
-                self._prec_frame, self._next_frame = self.next_frame, None # iter in stream
-
-        slices = [
-            (round((start - timestamp) * rate), _convert_audio_samples(array))
-            for start, array in slices
-        ] # time to index
-        drift_max = self.av_container.streams[self.index].time_base
-        drift_max = 2 if drift_max is None else math.ceil(drift_max*rate)
-        slices = _fix_drift(slices, drift_max, samples)
-
-        # create the new empty audio frame
-        dtypes = {a.dtype for _, a in slices}
-        dtypes = sorted(
-            dtypes, key=lambda t: {torch.float16: 2, torch.float32: 1, torch.float64: 0}
-        ) + [torch.float32] # if slice = []
-        frame = FrameAudio(
-            timestamp, rate, torch.full((self.channels, samples), torch.nan, dtype=dtypes[0])
-        )
-
-        # positionning of each slices
-        for index, array in slices:
-            if index < 0:
-                array = array[:, -index:]
-                index = 0
-            if index + array.shape[1] > samples: # if slice to long
-                array = array[:, :max(0, samples-index)]
-            if array.shape[1]:
-                frame[:, index:index+array.shape[1]] = array
-
-        # print(frame)
-
-        return frame
+        if self._av_container is None:
+            self._av_container = av.open(str(self.node.filename), "r", **self.node.av_kwargs)
+        return self._av_container
 
     @property
     def channels(self) -> int:
         """
         ** The number of channels in this audio stream. **
 
         Examples
         --------
-        >>> from cutcutcodec.core.io.read import ContainerInputFFMPEG
-        >>> with ContainerInputFFMPEG("cutcutcodec/examples/audio.ogg") as container:
+        >>> from movia.core.io.read import ContainerInputFFMPEG
+        >>> with ContainerInputFFMPEG("movia/examples/audio.ogg") as container:
         ...     (stream,) = container.out_streams
         ...     stream.channels
         ...
         1
         >>>
         """
         return self.av_container.streams[self.index].codec_context.channels
 
+    def close(self):
+        """
+        ** Close the file. **
+        """
+        if self._av_container is not None:
+            self._av_container.close()
+
     @property
-    def duration(self) -> typing.Union[Fraction, float]:
+    def duration(self) -> numbers.Real:
         """
         ** The exact duration in seconds. **
 
         Examples
         --------
-        >>> from cutcutcodec.core.io.read import ContainerInputFFMPEG
-        >>> with ContainerInputFFMPEG("cutcutcodec/examples/audio.ogg") as container:
+        >>> from movia.core.io.read import ContainerInputFFMPEG
+        >>> with ContainerInputFFMPEG("movia/examples/audio.ogg") as container:
         ...     (stream,) = container.out_streams
         ...     stream.duration
         ...
         Fraction(16, 1)
         >>>
         """
         if self._duration is not None:
             return self._duration
-        # seek approximative
-        rel_index = len(
-            [
-                None for i, s in enumerate(self.node.out_streams)
-                if i < self.index and s.type == "audio"
-            ]
-        )
-        with self._lock:
-            self.seek(get_duration_audio(self.node.filename, rel_index, accurate=False) - 10)
-            # decoding until reaching the last frame
-            while self.next_frame is not None:
-                self._prec_frame, self._next_frame = self.next_frame, None # iter in stream
-            # get the time of the last frame + the frame duration
-            self._duration = frame_dates(self._prec_frame)[1]
+
+        while True:
+            try:
+                self._update_prec_next()
+            except OutOfTimeRange:
+                break
+        self._duration = _frame_dates(self._next_frame)[1]
         return self._duration
 
-    def get_current_range(self) -> tuple[Fraction, Fraction]:
+    @property
+    def frame_iter(self) -> typing.Iterable:
         """
-        ** Returns the time interval cover by the current frame. **
+        ** Allows to read the file at the last moment. **
         """
-        if (next_frame := self.next_frame) is None:
-            return frame_dates(self.prec_frame)
-        return frame_dates(self.prec_frame)[0], frame_dates(next_frame)[0]
+        if self._frame_iter is None:
+            self._frame_iter = iter(
+                self.av_container.decode(self.av_container.streams[self.index])
+            )
+        return self._frame_iter
 
     @property
-    def rate(self) -> int:
+    def metadata(self) -> int:
         """
-        ** Theorical image or sample frequency in the metadata. **
-        """
-        return int(super().rate)
+        ** The metadata associated with this stream. **
 
-    def seek(self, position: Fraction) -> None:
+        Examples
+        --------
+        >>> from movia.core.io.read import ContainerInputFFMPEG
+        >>> with ContainerInputFFMPEG("movia/examples/audio.ogg") as container:
+        ...     (stream,) = container.out_streams
+        ...     stream.metadata
+        ...
+        {'encoder': 'Lavc59.37.100 libvorbis'}
+        >>>
         """
-        ** Moves into the file until reaching the frame at this position. **
-
-        If you are already well placed, this has no effect.
-        Allows backward even a little bit, but only jump forward if the jump is big enough.
-
-        Parameters
-        ----------
-        position : fraction.Fraction
-            The target position such as ``self.prec_frame.time <= position < self.next_frame.time``.
-            This position is expressed in seconds.
+        return self.av_container.streams[self.index].metadata
 
-        Raises
-        ------
-        OutOfTimeRange
-            If the required position is out of the definition range.
+    @property
+    def samplerate(self) -> int:
+        """
+        ** The frequency of the samples. **
 
         Examples
         --------
-        >>> from fractions import Fraction
-        >>> from cutcutcodec.core.io.read import ContainerInputFFMPEG
-        >>> with ContainerInputFFMPEG("cutcutcodec/examples/audio.ogg") as container:
+        >>> from movia.core.io.read import ContainerInputFFMPEG
+        >>> with ContainerInputFFMPEG("movia/examples/audio.ogg") as container:
         ...     (stream,) = container.out_streams
-        ...     stream.seek(Fraction(15))
-        ...     stream.get_current_range()
-        ...     stream.seek(Fraction(5))
-        ...     stream.get_current_range()
+        ...     stream.samplerate
         ...
-        (Fraction(1872, 125), Fraction(1876, 125))
-        (Fraction(624, 125), Fraction(628, 125))
+        16000
         >>>
         """
-        assert isinstance(position, Fraction), position.__class__.__name__
+        return self.av_container.streams[self.index].codec_context.rate
+
+    def seek(self, position: numbers.Real):
+        """
+        ** Moves into the file. **
+
+        If you are already well placed, this has no effect.
+        Allows backward even a little bit, but only forward if the jump is big enough.
+        """
+        assert isinstance(position, numbers.Real), position.__class__.__name__
+        if self._prec_frame is None:
+            self._update_prec_next()
 
         # case need to seek
-        if position > self.get_current_range()[1] + 10: # forward if jump more 10 seconds
+        if (
+            position - 10 > (
+                _frame_dates(self._next_frame)[0]
+                + fractions.Fraction(self._next_frame.samples, self._next_frame.rate)
+            )
+        ): # take a leap forward (jump > 10 s)
             self._seek_forward(position) # very approximative
-        if position < self.get_current_range()[0]:
+        if position < _frame_dates(self._prec_frame)[0]:
             self._seek_backward(position) # guaranteed to be before
 
         # fine adjustment
-        while self.get_current_range()[1] <= position:
-            self._prec_frame, self._next_frame = self.next_frame, None # iter in stream
+        while (
+            _frame_dates(self._next_frame)[0]
+            + fractions.Fraction(self._next_frame.samples, self._next_frame.rate)
+            < position
+        ):
+            self._update_prec_next()
+
+    @property
+    def time_base(self) -> fractions.Fraction:
+        """
+        ** The unit of time (in fractional seconds) in which timestamps are expressed. **
+
+        Examples
+        --------
+        >>> from movia.core.io.read import ContainerInputFFMPEG
+        >>> with ContainerInputFFMPEG("movia/examples/audio.ogg") as container:
+        ...     (stream,) = container.out_streams
+        ...     stream.time_base
+        ...
+        Fraction(1, 16000)
+        >>>
+        """
+        return self.av_container.streams[self.index].time_base
 
 
-class _StreamVideoFFMPEG(StreamVideo, _StreamFFMPEGBase):
+class _StreamVideoFFMPEG(StreamVideo):
     """
     Attributes
     ----------
-    height : int
-        The dimension i (vertical) of the encoded frames in pxl (readonly).
-    duration : Fraction
-        The exact duration of the complete stream (readonly).
-        the time include the duration of the last frame.
-    width : int
-        The dimension j (horizontal) of the encoded frames in pxl (readonly).
+    duration : numbers.Real
+        The exact duration of the stream (readonly).
+        This date corresponds to the end of the last frame.
+    framerate : numbers.Real
+        Theoretical image frequency in the metadata (readonly).
+    nb_frames : int
+        The exact number of frames present in this stream (readonly).
+    time_base : fractions.Fraction
+        The unit of time (in fractional seconds) in which timestamps are expressed (readonly).
     """
 
     is_space_continuous = False
+    is_time_continuous = False
 
     def __init__(self, node: ContainerInputFFMPEG):
+        """
+        Parameters
+        ----------
+        node : movia.core.io.read.ContainerInputFFMPEG
+            Simply allows to keep the graph structure.
+        """
+        assert isinstance(node, ContainerInputFFMPEG), node.__class__.__name__
         super().__init__(node)
-        self._duration = None
+
+        self._av_container = None
         self._key_times = None
-        self._lock = threading.Lock()
+        self._frame_iter = None # we can't recreate it every time because we lose the last frames
+        self._prec_frame = self._next_frame = None
+        self._duration = None
+
+    def __iter__(self):
+        """
+        ** Yields all frames of this stream starting from the current position. **
+        """
+        if self._next_frame is None:
+            self._update_prec_next()
+        yield self._next_frame
+        while True:
+            try:
+                yield self._update_prec_next()
+            except OutOfTimeRange:
+                break
+
+    def _snapshot(self, timestamp: float) -> av.video.frame.VideoFrame:
+        # ideal case (select the nearest)
+        if self._prec_frame is None:
+            self._update_prec_next()
+        if self._prec_frame.time <= timestamp <= self._next_frame.time:
+            delta_prec = timestamp - self._prec_frame.time
+            delta_next = self._next_frame.time - timestamp
+            return self._prec_frame if delta_prec <= delta_next else self._next_frame
+
+        key_prec, key_next = _born(self.key_times, timestamp)
+        if key_prec is None:
+            raise OutOfTimeRange(f"there is no frame at timestamp {timestamp} (need >= {key_next})")
+
+        # case need seek (backward or big displacement)
+        if (
+            self._prec_frame.time > timestamp # back to the past
+            or self._next_frame.time < key_prec - .5 # take a leap forward (jump > 500 ms)
+        ):
+            self.av_container.seek(
+                1 + int(key_prec / self.av_container.streams[self.index].time_base),
+                backward=True, # if there is not a keyframe at the given offset
+                any_frame=False, # seek to any frame, not just a keyframe
+                stream=self.av_container.streams[self.index]
+            )
+            self._frame_iter = None # takes into account the new position
+
+        # decoding until reaching the right frame
+        try:
+            while timestamp > self._update_prec_next().time:
+                continue
+        except OutOfTimeRange as err: # management of the time overrun of the last frame
+            if timestamp >= self._next_frame.time + 1/self.framerate:
+                raise err
+            return self._next_frame
+        return self._snapshot(timestamp)
+
+    def _update_prec_next(self) -> av.video.frame.VideoFrame:
+        """
+        ** Iterates on the next frame. **
+
+        Raises
+        ------
+        OutOfTimeRange
+            If the last frame has already been reached.
+        """
+        self._prec_frame = self._next_frame
+        try:
+            self._next_frame = next(self.frame_iter)
+        except StopIteration as err:
+            raise OutOfTimeRange("there is no frame left to read") from err
+        if self._prec_frame is None:
+            self._prec_frame = self._next_frame
+        return self._next_frame
+
+    @property
+    def av_container(self) -> av.container.Container:
+        """
+        ** Allows to read the file at the last moment. **
+        """
+        if self._av_container is None:
+            self._av_container = av.open(str(self.node.filename), "r", **self.node.av_kwargs)
+        return self._av_container
 
-    def _snapshot(self, timestamp: Fraction, shape: tuple[int, int]) -> FrameVideo:
-        if timestamp < 0:
-            raise OutOfTimeRange(f"there is no audio frame at timestamp {timestamp} (need >= 0)")
-        with self._lock:
-            self.seek(timestamp) # adjust position
-            frame_av = self.prec_frame
-            frame_np = frame_av.to_ndarray(format="bgr24")
-        if frame_np.shape[:2] != shape: # cv2 two time faster than torch
-            frame_np = resize_keep_ratio(frame_np, shape)
-        return FrameVideo(frame_dates(frame_av)[0], frame_np)
+    def close(self):
+        """
+        ** Close the file. **
+        """
+        if self._av_container is not None:
+            self._av_container.close()
 
     @property
-    def duration(self) -> typing.Union[Fraction, float]:
+    def duration(self) -> numbers.Real:
         """
         ** The exact duration in seconds. **
 
         Examples
         --------
-        >>> from cutcutcodec.core.io.read import ContainerInputFFMPEG
-        >>> with ContainerInputFFMPEG("cutcutcodec/examples/video.mp4") as container:
+        >>> from movia.core.io.read import ContainerInputFFMPEG
+        >>> with ContainerInputFFMPEG("movia/examples/video.mp4") as container:
         ...     (stream,) = container.out_streams
         ...     stream.duration
         ...
-        Fraction(16, 1)
+        16.0
         >>>
         """
         if self._duration is not None:
             return self._duration
-        with self._lock:
-            # jump if need
-            key_times = self.get_key_times()
-            if frame_dates(self.prec_frame)[0] < key_times[-1]:
-                self.seek(key_times[-1])
-            # decoding until reaching the last frame
-            while self.next_frame is not None:
-                self._prec_frame, self._next_frame = self.next_frame, None # iter in stream
-            # get the time of the last frame + the frame duration
-            self._duration = frame_dates(self._prec_frame)[0] + 1/self.rate
+        self._snapshot(self.key_times[-1])
+        self._duration = self.key_times[-1]
+        for frame in self:
+            self._duration = frame.time
+        assert self._duration is not None
+        self._duration += 1/self.framerate # duration of the last frame
         return self._duration
 
-    def get_key_times(self) -> np.ndarray[Fraction]:
+    @property
+    def frame_iter(self) -> typing.Iterable:
         """
         ** Allows to read the file at the last moment. **
+        """
+        if self._frame_iter is None:
+            self._frame_iter = iter(
+                self.av_container.decode(self.av_container.streams[self.index])
+            )
+        return self._frame_iter
 
-        Examples
-        --------
-        >>> from cutcutcodec.core.io.read import ContainerInputFFMPEG
-        >>> with ContainerInputFFMPEG("cutcutcodec/examples/video.mp4") as container:
-        ...     (stream,) = container.out_streams
-        ...     stream.get_key_times()
-        ...
-        array([Fraction(0, 1), Fraction(10, 1)], dtype=object)
-        >>>
+    @property
+    def framerate(self) -> numbers.Real:
+        """
+        ** Theoretical image frequency in the metadata. **
+        """
+        rel_index = [
+            i for i, s_ in enumerate(
+                s for s in self.node.out_streams if isinstance(s, _StreamVideoFFMPEG)
+            ) if s_ is self
+        ].pop()
+        return get_fps(self.node.filename, rel_index)
+
+    @property
+    def height(self) -> int:
+        return self.av_container.streams[self.index].height
+
+    @property
+    def key_times(self) -> np.ndarray[np.float32]:
+        """
+        ** Allows to read the file at the last moment. **
         """
         if self._key_times is None:
-            try:
-                self._key_times = np.fromiter(
-                    (
-                        frame_dates(frame)[0] for frame in _extract_key_frames(
-                            self.av_container.streams[self.index]
-                        )
-                    ),
-                    dtype=object,
-                )
-            except MissingInformation as err:
-                raise MissingInformation("the timestamp is not known for all keyframes") from err
+            self._key_times = np.fromiter(
+                (
+                    frame.time for frame in _extract_key_frames(
+                        self.av_container.streams[self.index]
+                    )
+                ),
+                dtype=np.float32,
+            )
             if len(self._key_times) == 0:
                 raise MissingStreamError(
                     f"can not decode any frames of {self.node.filename} stream {self.index}"
                 )
+            if np.any(np.isnan(self._key_times)):
+                raise MissingInformation("the timestamp is not known for all keyframes")
         return self._key_times
 
-    def get_current_range(self) -> tuple[Fraction, Fraction]:
-        """
-        ** Returns the time interval cover by the current frame. **
-        """
-        start_time = frame_dates(self.prec_frame)[0]
-        if (next_frame := self.next_frame) is None:
-            return start_time, start_time + 1/self.rate
-        return start_time, frame_dates(next_frame)[0]
-
     @property
-    def height(self) -> int:
+    def nb_frames(self) -> int:
         """
-        ** The vertical size of the native frame in pxl. **
+        ** The exact number of frames present in this stream. **
         """
-        return self.av_container.streams[self.index].height
+        rel_index = [
+            i for i, s_ in enumerate(
+                s for s in self.node.out_streams if isinstance(s, _StreamVideoFFMPEG)
+            ) if s_ is self
+        ].pop()
+        return get_nb_frames(self.node.filename, rel_index, accurate=True)
 
-    def seek(self, position: Fraction) -> None:
+    @property
+    def time_base(self) -> fractions.Fraction:
         """
-        ** Moves into the file until reaching the frame at this position. **
-
-        If you are already well placed, this has no effect.
-        Allows backward even a little bit, but only jump forward if the jump is big enough.
-
-        Parameters
-        ----------
-        position : fraction.Fraction
-            The target position such as ``self.prec_frame.time <= position < self.next_frame.time``.
-            This position is expressed in seconds.
-
-        Raises
-        ------
-        OutOfTimeRange
-            If the required position is out of the definition range.
+        ** The unit of time (in fractional seconds) in which timestamps are expressed. **
 
         Examples
         --------
-        >>> from fractions import Fraction
-        >>> from cutcutcodec.core.io.read import ContainerInputFFMPEG
-        >>> with ContainerInputFFMPEG("cutcutcodec/examples/video.mp4") as container:
+        >>> from movia.core.io.read import ContainerInputFFMPEG
+        >>> with ContainerInputFFMPEG("movia/examples/video.mp4") as container:
         ...     (stream,) = container.out_streams
-        ...     stream.seek(Fraction(15))
-        ...     stream.get_current_range()
-        ...     stream.seek(Fraction(5))
-        ...     stream.get_current_range()
+        ...     stream.time_base
         ...
-        (Fraction(15, 1), Fraction(376, 25))
-        (Fraction(5, 1), Fraction(126, 25))
+        Fraction(1, 12800)
         >>>
         """
-        assert isinstance(position, Fraction), position.__class__.__name__
-
-        # case need to seek
-        if position > self.get_current_range()[1] + 100/self.rate: # forward if jump more 100 frames
-            self._seek_forward(position) # very approximative
-        if position < self.get_current_range()[0]:
-            self._seek_backward(position) # guaranteed to be before
-
-        # fine adjustment
-        while self.get_current_range()[1] <= position:
-            self._prec_frame, self._next_frame = self.next_frame, None # iter in stream
+        return self.av_container.streams[self.index].time_base
 
     @property
     def width(self) -> int:
-        """
-        ** The horizontal size of the native frame in pxl. **
-        """
         return self.av_container.streams[self.index].width
 
 
-def _convert_audio_samples(audio_samples: np.ndarray[numbers.Real]) -> torch.Tensor:
+def _born(refs, val):
+    """
+    ** Search the 2 values that encadre the number. **
+
+    The interval sought is the upper one.
+
+    Parameters
+    ----------
+    refs : np.ndarray
+        The list in ascending order of key values.
+    val : numbers.Real
+        The value to be placed among the other values.
+
+    Examples
+    --------
+    >>> import numpy as np
+    >>> from movia.core.io.read import _born
+    >>> _born(np.array([0, 2]), -1)
+    (None, 0)
+    >>> _born(np.array([0, 2]), 0)
+    (0, 2)
+    >>> _born(np.array([0, 2]), 1)
+    (0, 2)
+    >>> _born(np.array([0, 2]), 2)
+    (2, None)
+    >>> _born(np.array([0, 2]), 3)
+    (2, None)
+    >>> _born(np.array([0]), -1)
+    (None, 0)
+    >>> _born(np.array([0]), 0)
+    (0, None)
+    >>> _born(np.array([0]), 1)
+    (0, None)
+    >>>
+    """
+    if val < refs[0]:
+        return None, refs[0]
+    if val >= refs[-1]:
+        return refs[-1], None
+    ind_sup = np.argmin(refs <= val)
+    return refs[ind_sup-1], refs[ind_sup]
+
+
+def _clip_convert(audio_samples: np.ndarray[numbers.Real]) -> np.ndarray[numbers.Real]:
     """
     ** Converts sound samples into float between -1 and 1. **
 
     Minimizes copying and reallocations.
-    The values are not clamped.
 
     Examples
     --------
     >>> import numpy as np
-    >>> from cutcutcodec.core.io.read import _convert_audio_samples
-    >>> _convert_audio_samples(np.array([-1.5, -1.0, -.5, .5, 1.0, 1.5], dtype=np.float64))
-    tensor([-1.5000, -1.0000, -0.5000,  0.5000,  1.0000,  1.5000],
-           dtype=torch.float64)
-    >>> _convert_audio_samples(np.array([-1.5, -1.0, -.5, .5, 1.0, 1.5], dtype=np.float32))
-    tensor([-1.5000, -1.0000, -0.5000,  0.5000,  1.0000,  1.5000])
-    >>> _convert_audio_samples(np.array([-1.5, -1.0, -.5, .5, 1.0, 1.5], dtype=np.float16))
-    tensor([-1.5000, -1.0000, -0.5000,  0.5000,  1.0000,  1.5000],
-           dtype=torch.float16)
-    >>> _convert_audio_samples(
-    ...     np.array([-2147483648, -1073741824, 1073741824, 2147483647], dtype=np.int32)
-    ... )
-    tensor([-1.0000, -0.5000,  0.5000,  1.0000], dtype=torch.float64)
-    >>> _convert_audio_samples(np.array([-32768, -16384, 16384, 32767], dtype=np.int16))
-    tensor([-1.0000, -0.5000,  0.5000,  1.0000], dtype=torch.float64)
-    >>> _convert_audio_samples(np.array([0, 64, 192, 255], dtype=np.uint8))
-    tensor([-1.0000, -0.4980,  0.5059,  1.0000], dtype=torch.float64)
+    >>> from movia.core.io.read import _clip_convert
+    >>> _clip_convert(np.array([-1.5, -1.0, -.5, .5, 1.0, 1.5], dtype=np.float64))
+    array([-1. , -1. , -0.5,  0.5,  1. ,  1. ])
+    >>> _clip_convert(np.array([-1.5, -1.0, -.5, .5, 1.0, 1.5], dtype=np.float32))
+    array([-1. , -1. , -0.5,  0.5,  1. ,  1. ], dtype=float32)
+    >>> _clip_convert(np.array([-1.5, -1.0, -.5, .5, 1.0, 1.5], dtype=np.float16))
+    array([-1. , -1. , -0.5,  0.5,  1. ,  1. ], dtype=float16)
+    >>> _clip_convert(np.array([-2147483648, -1073741824, 1073741824, 2147483647], dtype=np.int32))
+    array([-1. , -0.5,  0.5,  1. ])
+    >>> _clip_convert(np.array([-32768, -16384, 16384, 32767], dtype=np.int16))
+    array([-1.        , -0.49999237,  0.50002289,  1.        ])
+    >>> _clip_convert(np.array([0, 64, 192, 255], dtype=np.uint8))
+    array([-1.        , -0.49803922,  0.50588235,  1.        ])
     >>>
     """
     assert isinstance(audio_samples, np.ndarray), audio_samples.__class__.__name__
-    audio_samples = torch.from_numpy(audio_samples)
-    if not audio_samples.dtype.is_floating_point:
-        iinfo = torch.iinfo(audio_samples.dtype)
-        audio_samples = audio_samples.to(dtype=torch.float64)
-        audio_samples -= .5*float(iinfo.min + iinfo.max)
-        audio_samples /= .5*float(iinfo.max - iinfo.min)
+    if issubclass(audio_samples.dtype.type, numbers.Integral):
+        iinfo = np.iinfo(audio_samples.dtype)
+        audio_samples = audio_samples.astype(np.float64)
+        audio_samples -= .5*np.float64(iinfo.min + iinfo.max)
+        audio_samples /= .5*np.float64(iinfo.max - iinfo.min)
+    else:
+        np.clip(audio_samples, -1, 1, out=audio_samples)
     return audio_samples
 
 
-def _extract_key_frames(av_stream: av.video.stream.VideoStream):
+def _extract_key_frames(av_stream):
     """
     ** Extract the list of key frames. **
 
     Examples
     --------
     >>> import av
-    >>> from cutcutcodec.core.io.read import _extract_key_frames
-    >>> with av.open("cutcutcodec/examples/video.mp4") as av_container:
+    >>> from movia.core.io.read import _extract_key_frames
+    >>> with av.open("movia/examples/video.mp4") as av_container:
     ...     key_frames = list(_extract_key_frames(av_container.streams.video[0]))
     ...
     >>> [f.time for f in key_frames]
     [0.0, 10.0]
     >>>
     """
     assert isinstance(av_stream, av.video.stream.VideoStream), av_stream.__class__.__name__
     av_stream.container.seek(0, backward=True, any_frame=False, stream=av_stream)
     av_stream.codec_context.skip_frame = "NONKEY"
     yield from av_stream.container.decode(av_stream)
     av_stream.container.seek(0, backward=True, any_frame=False, stream=av_stream)
     av_stream.codec_context.skip_frame = "DEFAULT"
 
 
-def _fix_drift(
-    slices: list[tuple[int, torch.Tensor]], drift_max: int, samples: int
-) -> list[tuple[int, torch.Tensor]]:
-    """
-    ** Slightly shifts the audio frames so that they follow each other perfectly. **
-
-    Changes the values inplace as possible.
-
-    Parameters
-    ----------
-    slices : list[tuple[int, torch.Tensor]]
-        The list of the (index, frame) to shift a bit.
-    drift_max : int
-        The maximum authorized translation.
-    samples: int
-        The final index. In the case where there is a hole at the beginning or at the very end,
-        this makes it possible to translate the entirety of the frames by a maximum value of
-        `drift_max`/2 in order to fill the hole.
-    """
-    if not slices:
-        return []
-
-    # drift each slices for perfect concatenation
-    slices.sort(key=lambda i_a: i_a[0])
-    for i in range(1, len(slices)):
-        prec_end = slices[i-1][0] + slices[i-1][1].shape[1]
-        curr_start = slices[i][0]
-        if abs(curr_start-prec_end) <= drift_max: # if drift ok
-            slices[i] = (prec_end, slices[i][1])
-        else:
-            logging.warning("audio frame drift detected")
-
-    # global drift
-    if not (drift_max := drift_max//2):
-        return slices
-    drift = min(0, -slices[0][0]) + max(0, samples - (slices[-1][0]+slices[-1][1].shape[1]))
-    if drift and abs(drift) <= drift_max:
-        slices = [(ind+drift, frame) for ind, frame in slices]
-
-    return slices
-
-
-def frame_dates(frame: av.frame.Frame) -> tuple[Fraction, typing.Union[None, Fraction]]:
+def _frame_dates(frame: av.frame.Frame) -> tuple[numbers.Real, numbers.Real]:
     """
     ** Returns the accurate time interval of the given frame. **
 
-    Parameters
-    ----------
-    frame : av.frame.Frame
-        The audio or video frame witch we extract the timing information.
-
-    Returns
-    -------
-    t_start : Fraction
-        The display time of the frame. for audio frame, it corressponds to
-        the time of the first sample.
-    t_end : Fraction or None
-        For audio frame only, the time to switch off the last sample.
-
     Examples
     --------
     >>> import av
-    >>> from cutcutcodec.core.io.read import frame_dates
-    >>> with av.open("cutcutcodec/examples/video.mp4") as av_container:
-    ...     frame_dates(next(av_container.decode(av_container.streams.video[0])))
-    ...     frame_dates(next(av_container.decode(av_container.streams.video[0])))
+    >>> from movia.core.io.read import _frame_dates
+    >>> with av.open("movia/examples/video.mp4") as av_container:
+    ...     frame = next(av_container.decode(av_container.streams.video[0]))
+    ...     _frame_dates(frame)
     ...
-    (Fraction(0, 1), None)
-    (Fraction(1, 25), None)
-    >>> with av.open("cutcutcodec/examples/audio.ogg") as av_container:
-    ...     frame_dates(next(av_container.decode(av_container.streams.audio[0])))
-    ...     frame_dates(next(av_container.decode(av_container.streams.audio[0])))
+    (Fraction(0, 1), Fraction(0, 1))
+    >>> with av.open("movia/examples/audio.ogg") as av_container:
+    ...     frame = next(av_container.decode(av_container.streams.audio[0]))
+    ...     _frame_dates(frame)
     ...
     (Fraction(0, 1), Fraction(4, 125))
-    (Fraction(4, 125), Fraction(8, 125))
     >>>
-
-    Notes
-    -----
-    For audio frame, include the duration of the last sample.
-    For video frame, the duration of the frame is unmknonw.
     """
     assert isinstance(frame, av.frame.Frame), frame.__class__.__name__
 
-    if (time_base := frame.time_base) is None:
-        start_time = Fraction(frame.time)
-    elif (pts := frame.pts) is not None:
-        start_time = pts * time_base
-    elif (dts := frame.dts) is not None:
-        start_time = dts * time_base
+    if (pts := frame.pts) is None or (time_base := frame.time_base) is None:
+        start_time = frame.time
     else:
-        raise MissingInformation(f"unable to catch the time of the frame {frame}")
+        start_time = pts * time_base
     if isinstance(frame, av.audio.frame.AudioFrame):
-        stop_time = start_time + Fraction(frame.samples, frame.rate)
+        stop_time = start_time + fractions.Fraction(frame.samples, frame.rate)
         return start_time, stop_time
-    return start_time, None
+    return start_time, start_time
```

### Comparing `movia-1.0.0rc1/cutcutcodec/gui/app/app.py` & `movia-1.0a1/movia/gui/app/app.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,31 +1,26 @@
 #!/usr/bin/env python3
 
 """
 ** Interface between windows and data. **
 -----------------------------------------
 """
 
-import logging
 import pathlib
 import threading
 import typing
 
 import networkx
 
-from cutcutcodec.core.analysis.ffprobe import get_streams_type
-from cutcutcodec.core.classes.container import ContainerOutput
-from cutcutcodec.core.classes.node import Node
-from cutcutcodec.core.classes.stream import Stream
-from cutcutcodec.core.compilation.graph_to_json import graph_to_json
-from cutcutcodec.core.compilation.graph_to_tree import graph_to_tree, update_trees
-from cutcutcodec.core.compilation.json_to_graph import json_to_graph
-from cutcutcodec.core.compilation.tree_to_graph import tree_to_graph
-from cutcutcodec.core.generation.audio.noise import GeneratorAudioNoise
-from cutcutcodec.core.generation.video.noise import GeneratorVideoNoise
+from movia.core.classes.container import ContainerOutput
+from movia.core.classes.node import Node
+from movia.core.classes.stream import Stream
+from movia.core.compilation.graph_to_tree import graph_to_tree, update_tree
+from movia.core.compilation.tree_to_graph import tree_to_graph
+from movia.core.filters.basic.truncate import FilterTruncate
 
 
 
 class App:
     """
     ** Contains the shared data. **
 
@@ -38,44 +33,35 @@
     project_files : list[str]
         All the paths of the imported files.
     """
 
     def __init__(self):
         self._persistant = {} # all for the state.
         self._compile_lock = threading.Lock()
-        self._graph = tree_to_graph(
-            ContainerOutput(
-                [
-                    GeneratorAudioNoise().out_streams[0],
-                    GeneratorVideoNoise().out_streams[0],
-                ]
-            )
-        )
+        self._graph = tree_to_graph(ContainerOutput(FilterTruncate.default().out_streams))
         self.global_vars = {}
 
     def __getstate__(self) -> dict:
         """
-        ** Allows to help serialization and saving. **
+        ** Allows to help serialization. **
         """
         return {
-            "export_settings": self.export_settings,
-            "graph": graph_to_json(self.graph),
+            "graph": self.graph,
             "project_files": self.project_files,
+            "export_settings": self.export_settings
         }
 
     def __setstate__(self, state: dict):
         """
         ** Allows deserialization. **
         """
         assert isinstance(state, dict), state.__class__.__name__
 
-        self._persistant["export_settings"] = state.get("export_settings", {})
-        if (graph := state.get("graph", None)) is not None:
-            graph = json_to_graph(graph)
-        self.graph = graph
+        self.export_settings = state.get("export_settings", {})
+        self.graph = state.get("graph", None)
         self.project_files = state.get("project_files", [])
 
     @property
     def export_settings(self) -> dict[str]:
         """
         ** The exporation parameters. **
 
@@ -83,80 +69,35 @@
         -----
         * Modifications are inplace.
         * Need to replace the "default" values.
         """
         export_settings = self._persistant.get("export_settings", {})
         export_settings["parent"] = export_settings.get("parent", str(pathlib.Path.cwd()))
         if "stem" not in export_settings:
-            export_settings["stem"] = "cutcutcodec_project"
+            export_settings["stem"] = "movia_project"
             while (pathlib.Path(export_settings["parent"]) / export_settings["stem"]).exists():
                 export_settings["stem"] += "_bis"
         export_settings["suffix"] = export_settings.get("suffix", "")
         export_settings["muxer"] = export_settings.get("muxer", "default")
         export_settings["muxer_settings"] = export_settings.get("muxer_settings", {})
-
-        tree = self.tree()
-
-        # codecs
-        export_settings["codecs"] = export_settings.get("codecs", {"audio": [], "video": []})
-        export_settings["codecs"]["audio"].extend(["default" for _ in tree.in_select("audio")])
-        export_settings["codecs"]["video"].extend(["default" for _ in tree.in_select("video")])
-        export_settings["codecs"]["audio"] = (
-            export_settings["codecs"]["audio"][:len(tree.in_select("audio"))]
-        )
-        export_settings["codecs"]["video"] = (
-            export_settings["codecs"]["video"][:len(tree.in_select("video"))]
-        )
-
-        # encoders
-        export_settings["encoders"] = export_settings.get("encoders", {"audio": [], "video": []})
-        export_settings["encoders"]["audio"].extend(["default" for _ in tree.in_select("audio")])
-        export_settings["encoders"]["video"].extend(["default" for _ in tree.in_select("video")])
-        export_settings["encoders"]["audio"] = (
-            export_settings["encoders"]["audio"][:len(tree.in_select("audio"))]
-        )
-        export_settings["encoders"]["video"] = (
-            export_settings["encoders"]["video"][:len(tree.in_select("video"))]
-        )
-
-        # encoders_settings
-        export_settings["encoders_settings"] = (
-            export_settings.get("encoders_settings", {"audio": [], "video": []})
+        export_settings["codecs"] = ( # list
+            export_settings.get("codecs", ["default" for _ in self.tree().in_streams])
+            [:len(self.tree().in_streams)]
+        )
+        export_settings["encoders"] = ( # list
+            export_settings.get("encoders", ["default" for _ in self.tree().in_streams])
+            [:len(self.tree().in_streams)]
+        )
+        export_settings["encoders_settings"] = ( # list
+            export_settings.get("encoders_settings", [{} for _ in self.tree().in_streams])
+            [:len(self.tree().in_streams)]
         )
-        export_settings["encoders_settings"]["audio"].extend([{} for _ in tree.in_select("audio")])
-        export_settings["encoders_settings"]["video"].extend([{} for _ in tree.in_select("video")])
-        export_settings["encoders_settings"]["audio"] = (
-            export_settings["encoders_settings"]["audio"][:len(tree.in_select("audio"))]
-        )
-        export_settings["encoders_settings"]["video"] = (
-            export_settings["encoders_settings"]["video"][:len(tree.in_select("video"))]
-        )
-
-        # fps, samplerate and shapes
-        export_settings["rates"] = export_settings.get("rates", {"audio": [], "video": []})
-        export_settings["rates"]["audio"].extend(["default" for _ in tree.in_select("audio")])
-        export_settings["rates"]["video"].extend(["default" for _ in tree.in_select("video")])
-        export_settings["rates"]["audio"] = (
-            export_settings["rates"]["audio"][:len(tree.in_select("audio"))]
-        )
-        export_settings["rates"]["video"] = (
-            export_settings["rates"]["video"][:len(tree.in_select("video"))]
-        )
-        export_settings["shapes"] = export_settings.get("shapes", [])
-        export_settings["shapes"].extend(["default" for _ in tree.in_select("video")])
-
         self._persistant["export_settings"] = export_settings # for inplace edition, not setter
         return export_settings
 
-    def get_save_file(self) -> typing.Union[None, pathlib.Path]:
-        """
-        ** The path for the saving file, None if it is not define. **
-        """
-        return self._persistant.get("save_file", None)
-
     @property
     def graph(self) -> networkx.MultiDiGraph:
         """
         ** The assembly graph. **
         """
         return self._graph
 
@@ -170,64 +111,44 @@
             self._graph = graph
 
     @property
     def project_files(self) -> list[str]:
         """
         ** The list of absolute paths of the imported files. **
         """
-        return self._persistant.get("project_files", []).copy()
+        return self._persistant.get("project_files", [])
 
     @project_files.setter
-    def project_files(self, files: list[typing.Union[str, pathlib.Path]]):
+    def project_files(self, values: list[typing.Union[str, pathlib.Path]]):
         """
         ** Performs verification and standardization. **
         """
-        assert isinstance(files, list), files.__class__.__name__
-        assert all(isinstance(p, (str, pathlib.Path)) for p in files), files
-        files = [pathlib.Path(p) for p in files]
-        for file in files:
-            if not file.is_file():
-                logging.warning("the file %s is not an existing file", str(file))
-                continue
-            assert get_streams_type(file, ignore_errors=True), \
-                f"unable to detect any audio, video or subtitile stream in {file}"
+        assert isinstance(values, list), values.__class__.__name__
+        assert all(isinstance(p, (str, pathlib.Path)) for p in values), values
+
+        # normalize paths
+        project_files_ = [str(pathlib.Path(p).resolve()) for p in values]
 
-        # removes redundancy and keeps the order
+        # removes redundancy by keeping the order
         red = set()
-        files_ = []
-        for path in files:
+        project_files = []
+        for path in project_files_:
             if path in red:
                 continue
             red.add(path)
-            files_.append(path)
-        self._persistant["project_files"] = [str(p) for p in files_]
-
-    def redo(self):
-        """
-        ** Allows you to move forward in the steps. **
-        """
-        print("redo")
-
-    def set_save_file(self, file: typing.Union[None, str, pathlib.Path]):
-        """
-        ** Update the path of the file for saving project. **
-        """
-        if file is None:
-            self._persistant["save_file"] = None
-        assert isinstance(file, (str, pathlib.Path)), file.__class__.__name__
-        file = pathlib.Path(file)
-        self._persistant["save_file"] = file # str for jsonisable
+            project_files.append(path)
+        self._persistant["project_files"] = project_files
 
     def tree(self) -> ContainerOutput:
         """
         ** Returns the node associated with the complete graph. **
 
         Returns
         -------
-        container_output : cutcutcodec.core.classes.container.ContainerOutput
+        container_output : movia.core.classes.container.ContainerOutput
             The terminal node of the assembly graph.
         """
         with self._compile_lock:
             container_output = graph_to_tree(self.graph)
         return container_output
 
     def tree_edge(self, edge: tuple[str, str, str]) -> Stream:
@@ -250,42 +171,48 @@
         """
         assert isinstance(edge, tuple), edge.__class__.__name__
         assert len(edge) == 3, edge
         for name in edge:
             assert isinstance(name, str), name.__class__.__name__
         with self._compile_lock:
             assert self.graph.has_edge(*edge)
-            update_trees(self.graph)
+            update_tree(self.graph)
             src, dst, key = edge
-            tree = self.graph.edges[src, dst, key]["cache"][1]["tree"]
+            tree = self.graph.edges[src, dst, key]["tree"]
         return tree
 
     def tree_node(self, node: str) -> Node:
         """
         ** Returns the updated tree of this node. **
 
         Parameters
         ----------
         node : str
             The name of the node in the graph.
 
         Returns
         -------
-        cutcutcodec.core.classes.node.Node
+        movia.core.classes.node.Node
             The dynamic tree corresponding to this node.
 
         Notes
         -----
         All the ``tree`` attributes are updated to the current state of the assembly graph.
         """
         assert isinstance(node, str), node.__class__.__name__
         with self._compile_lock:
             assert node in self.graph
-            update_trees(self.graph)
-            tree = self.graph.nodes[node]["cache"][1]["tree"]
+            update_tree(self.graph)
+            tree = self.graph.nodes[node]["tree"]
         return tree
 
     def undo(self):
         """
         ** Return to the previous step. **
         """
         print("undo")
+
+    def redo(self):
+        """
+        ** Allows you to move forward in the steps. **
+        """
+        print("redo")
```

### Comparing `movia-1.0.0rc1/cutcutcodec/gui/base.py` & `movia-1.0a1/movia/gui/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,61 +3,58 @@
 """
 ** Allows to unify widgets by giving them interesting common properties. **
 ---------------------------------------------------------------------------
 """
 
 
 
-class CutcutcodecWidget:
+class MoviaWidget:
     """
     ** Allows to unify widgets by giving them interesting common properties. **
     """
 
     @property
     def app(self):
         """
-        ** from cutcutcodec.gui.base import CutcutcodecWidget. **
+        ** from movia.gui.base import MoviaWidget. **
         """
         return self.main_window.app
 
     @property
     def main_window(self):
         """
         ** Get the mother window of this descendant widget. **
         """
         ancestor = self
         ultimate_ancestor = self.parent
         while ultimate_ancestor is not None:
             ancestor, ultimate_ancestor = ultimate_ancestor, ultimate_ancestor.parent
-        if not isinstance(ancestor, CutcutcodecWidget):
+        if not isinstance(ancestor, MoviaWidget):
             raise TypeError(
-                f"all ancestors of {self.__class__.__name__} "
-                "must inherit from ``CutcutcodecWidget``"
+                f"all ancestors of {self.__class__.__name__} must inherit from ``MoviaWidget``"
             )
         return ancestor
 
     @property
     def parent(self):
         """
         ** Return the mother window. **
         """
         if (parent := getattr(self, "_parent", None)) is not None:
-            if not isinstance(parent, CutcutcodecWidget):
-                raise TypeError(
-                    f"{parent.__class__.__name__} must inherit from ``CutcutcodecWidget``"
-                )
+            if not isinstance(parent, MoviaWidget):
+                raise TypeError(f"{parent.__class__.__name__} must inherit from ``MoviaWidget``")
         return parent
 
     def refresh(self):
         """
         ** Updates this widget and all child widgets. **
 
         This method can be re-implemented.
         """
         childs = (
             child for attr, child in self.__dict__.items()
             if not attr.startswith("__")
             and child is not self.parent
-            and isinstance(child, CutcutcodecWidget)
+            and isinstance(child, MoviaWidget)
         )
         for child in childs:
             child.refresh()
```

### Comparing `movia-1.0.0rc1/cutcutcodec/gui/edit_node_state/all/filter_truncate.py` & `movia-1.0a1/movia/gui/node_properties/filter_truncate.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,50 +1,75 @@
 #!/usr/bin/env python3
 
 """
-** Properties of a ``cutcutcodec.core.filter.basic.truncate.FilterTruncate``. **
+** Properties of a ``movia.core.filter.basic.truncate.FilterTruncate``. **
 --------------------------------------------------------------------------
 """
 
-from fractions import Fraction
+import fractions
+import math
 
 from PyQt6 import QtWidgets
 
-from cutcutcodec.gui.edit_node_state.base import EditBase
+from movia.gui.base import MoviaWidget
 
 
 
-class EditFilterTruncate(EditBase):
+class FilterTruncateWidget(MoviaWidget, QtWidgets.QWidget):
     """
     ** Allows to view and modify the properties of a filter of type ``FilterTruncate``.
     """
 
     def __init__(self, parent, node_name):
-        super().__init__(parent, node_name)
-        self._duration_max_textbox = QtWidgets.QLineEdit(self)
+        super().__init__(parent)
+        self._parent = parent
+        self.node_name = node_name
+        self._duration_max_textbox = None
 
         grid_layout = QtWidgets.QGridLayout()
         self.init_duration_max(grid_layout)
         self.setLayout(grid_layout)
 
     def _validate_duration_max(self, text):
         """
         ** Check that the av kwargs are correct and update the color. **
         """
+        duration_max = {"inf": math.inf, "oo": math.inf}.get(text, text)
         try:
-            duration_max = Fraction(text)
+            duration_max = fractions.Fraction(duration_max)
+        except OverflowError:
+            pass
         except ValueError:
             self._duration_max_textbox.setStyleSheet("background:red;")
             return
-        self.try_set_state(
-            self.get_new_state({"duration_max": str(duration_max)}), self._duration_max_textbox
-        )
+        else:
+            duration_max = str(duration_max)
+
+        backup_duration_max = self.app.graph.nodes[self.node_name]["state"]["duration_max"]
+        self.app.graph.nodes[self.node_name]["state"]["duration_max"] = duration_max
+        try:
+            self.app.tree_node(self.node_name)
+        except AssertionError as err:
+            self.app.graph.nodes[self.node_name]["state"]["duration_max"] = backup_duration_max
+            self._duration_max_textbox.setStyleSheet("background:red;")
+            QtWidgets.QMessageBox.warning(
+                None, "Invalid duration", f"Unable to change the duration {duration_max} : {err}"
+            )
+            return
+        self._duration_max_textbox.setStyleSheet("background:none;")
+        print(f"update duration_max of {self.node_name}: {duration_max}")
+        self.main_window.refresh()
 
     def init_duration_max(self, grid_layout, ref_span=0):
         """
         ** Displays and allows to modify the av kwargs. **
         """
+        state = self.app.graph.nodes[self.node_name]["state"]
+
         grid_layout.addWidget(QtWidgets.QLabel("Duration Max (second):"))
-        self._duration_max_textbox.setText(self.state["duration_max"])
+        self._duration_max_textbox = QtWidgets.QLineEdit()
+        self._duration_max_textbox.setText(state["duration_max"])
         self._duration_max_textbox.textChanged.connect(self._validate_duration_max)
         grid_layout.addWidget(self._duration_max_textbox, ref_span, 1)
-        return ref_span + 1
+        ref_span += 1
+
+        return ref_span
```

### Comparing `movia-1.0.0rc1/cutcutcodec/gui/edit_node_state/base.py` & `movia-1.0a1/movia/gui/main.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,91 +1,108 @@
 #!/usr/bin/env python3
 
 """
-** Allows you to unify all node editing windows. **
----------------------------------------------------
-
-Defines several accessors that allow to lighten the code of child classes.
+** Entry point of the graphic interface. **
+-------------------------------------------
 """
 
-from PyQt6 import QtWidgets
 
-from cutcutcodec.gui.base import CutcutcodecWidget
+import pathlib
+import pickle
+import typing
+
+from PyQt6 import QtCore, QtWidgets
 
+from movia.gui.actions import create_actions
+from movia.gui.app.app import App
+from movia.gui.base import MoviaWidget
+from movia.gui.edition_tabs import EditionTabs
+from movia.gui.entry_tabs import EntryTabs
+from movia.gui.export.settings import WindowsExportSettings
+from movia.gui.menu import fill_menu
+from movia.gui.toolbar import MainToolBar
+from movia.gui.video_viewer import VideoViewer
 
 
-class EditBase(CutcutcodecWidget, QtWidgets.QWidget):
+
+class MainWindow(MoviaWidget, QtWidgets.QMainWindow):
     """
-    ** Common base class for all node editing classes. **
+    ** The main window for video editing interface. **
     """
 
-    def __init__(self, parent, node_name):
-        super().__init__(parent)
-        self._parent = parent
-        assert node_name in self.app.graph.nodes, (node_name, set(self.app.graph.nodes))
-        self.node_name = node_name
-        self.ref = [] # for keeping the reference of the interfaces
+    def __init__(self):
+        super().__init__()
+        self._parent = None
+
+        self._app = App()
+
+        self.actions = create_actions(self)
+
+        # declaration
+        self.setWindowTitle("Movia")
+        self.sub_windows = {
+            "toolbar": MainToolBar(self, self.actions),
+            "entry_tabs": EntryTabs(self),
+            "video_viewer": VideoViewer(self),
+            "edition_tabs": EditionTabs(self),
+        }
+        fill_menu(self.menuBar(), self.actions)
+
+        # location
+        self.addToolBar(self.sub_windows["toolbar"])
+        h_splitter = QtWidgets.QSplitter(QtCore.Qt.Orientation.Horizontal, self)
+        h_splitter.addWidget(self.sub_windows["entry_tabs"])
+        h_splitter.addWidget(self.sub_windows["video_viewer"])
+        v_splitter = QtWidgets.QSplitter(QtCore.Qt.Orientation.Vertical, self)
+        v_splitter.addWidget(h_splitter)
+        v_splitter.addWidget(self.sub_windows["edition_tabs"])
+        self.setCentralWidget(v_splitter)
 
-    def get_new_state(self, changes: dict[str]) -> dict[str]:
+    @property
+    def app(self):
         """
-        ** Returns a copy of the old state with the new attribute. **
+        ** Allows to rewrite this method of the parent class. **
         """
-        return {k: changes.get(k, o) for k, o in self.state.items()}
+        return self._app
 
-    def get_class(self) -> type:
+    def closeEvent(self, event):
         """
-        ** Returns the node class. **
+        ** Takes precautions before properly releasing resources. **
         """
-        return self.app.graph.nodes[self.node_name]["class"]
+        print("save")
+        event.accept()
 
-    @property
-    def state(self) -> dict[str]:
+    def crash(self, msg):
         """
-        ** Returns a pointer of the node state. **
+        ** Displays a critical error message. **
         """
-        return self.app.graph.nodes[self.node_name]["state"]
+        QtWidgets.QMessageBox.critical(None, "Application crashed", msg)
 
-    def try_set_state(self, new_state: dict[str], textbox=None) -> bool:
+    def export(self):
+        """
+        ** Brings up the export window. **
         """
-        ** If possible, try to apply the change to the node. **
+        WindowsExportSettings(self).exec()
 
-        In case of AssertionError, the changes are not applied
-        and a popup window appears to display the error message.
+    def load_project(self, project_file: typing.Union[str, pathlib.Path]):
+        """
+        ** Allows to open and load a file representing a project. **
 
         Parameters
         ----------
-        new_state : dict
-            The new different state.
-        textbox : PyQt6.QWidget, optional
-            Must accepts the method setStyleSheet for changing the bakground color.
-
-        Returns
-        -------
-        failed : boolean
-            False if succes and True if AssertionError raise in check.
-        """
-        old_state = self.state.copy()
-        assert set(new_state) == set(old_state), (new_state, old_state)
-
-        # search and format differences
-        changes = {k: (o, new_state[k]) for k, o in old_state.items() if o != new_state[k]}
-        changes_str = "\n".join(f"change {k} from {o} to {n}" for k, (o, n) in changes.items())
-
-        # apply changes
-        self.app.graph.nodes[self.node_name]["state"] = new_state
-        try:
-            self.app.tree_node(self.node_name)
-            self.main_window.refresh() # maybe can cause indirect errors
-        except AssertionError as err:
-            self.app.graph.nodes[self.node_name]["state"] = old_state
-            if textbox is not None:
-                textbox.setStyleSheet("background:red;")
-            QtWidgets.QMessageBox.warning(
-                None,
-                f"Invalid state of {self.node_name}",
-                f"{changes_str}\n\n{err}"
-            )
-            return True
-        if textbox is not None:
-            textbox.setStyleSheet("background:none;")
-        print(changes_str)
-        return False
+        project_file : pathlike
+            The name or path of the file.
+        """
+        assert isinstance(project_file, (str, pathlib.Path)), project_file.__class__.__name__
+        project_file = pathlib.Path(project_file)
+        with project_file.open("rb") as file:
+            app_state = pickle.load(file)
+        self.app.__setstate__(app_state)
+        self.refresh()
+
+    def refresh(self):
+        """
+        ** Updates the elements of this widget and child widgets. **
+        """
+        self.sub_windows["entry_tabs"].refresh()
+        self.sub_windows["video_viewer"].refresh()
+        self.sub_windows["edition_tabs"].refresh()
```

### Comparing `movia-1.0.0rc1/cutcutcodec/gui/entry/base.py` & `movia-1.0a1/movia/gui/entry/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,46 +1,47 @@
 #!/usr/bin/env python3
 
 """
 ** Defines the global style and behavior of the tabs of the entries table. **
 -----------------------------------------------------------------------------
 """
 
-import importlib
+import importlib.machinery
+import importlib.util
 import inspect
 import logging
 import re
 import typing
 
 from PyQt6 import QtCore, QtGui, QtWidgets
 import numpy as np
 
-from cutcutcodec.core.classes.node import Node
-from cutcutcodec.core.compilation.tree_to_graph import new_node
-from cutcutcodec.gui.base import CutcutcodecWidget
-from cutcutcodec.utils import get_project_root
+from movia.core.classes.node import Node
+from movia.core.compilation.tree_to_graph import new_node
+from movia.gui.base import MoviaWidget
+from movia.utils import get_project_root
 
 
 
-class Entry(CutcutcodecWidget, QtWidgets.QListWidget):
+class Entry(MoviaWidget, QtWidgets.QListWidget):
     """
     ** Allows to visualize the entries and to unify some functionalities. **
     """
 
     def __init__(self,
         parent,
         sub_dirs: list[str],
         excluded_clsn: set[str],
         classnames: typing.Union[type, tuple[type]]
     ):
         """
         Parameters
         ----------
         sub_dirs : list[str]
-            The name of the folders to explore from the ``cutcutcodec/core/`` directory.
+            The name of the folders to explore from the ``movia/core/`` directory.
         excluded_clsn : set[str]
             All classes to be excluded from the widget.
         classnames : typing.Union[type, tuple[type]]
             Valid classes for object selection.
         """
         super().__init__(parent)
         self._parent = parent
@@ -65,17 +66,20 @@
         if len(self.selectedItems()) != 1:
             logging.error("can drag and drop only one item, not %d", len(self.selectedItems()))
             self.app.global_vars["drag_an_drop"] = None
             event.ignore()
             return
 
         classname, path = [i.data(3) for i in self.selectedItems()].pop()
-        mod = importlib.import_module(
-            ".".join(("cutcutcodec" / path.relative_to(get_project_root()).with_suffix("")).parts)
+        mod_name = ".".join(("movia" / path.relative_to(get_project_root()).with_suffix("")).parts)
+        spec = importlib.util.spec_from_loader(
+            mod_name, importlib.machinery.SourceFileLoader(mod_name, str(path))
         )
+        mod = importlib.util.module_from_spec(spec)
+        spec.loader.exec_module(mod)
 
         generator_cls = dict(inspect.getmembers(mod))[classname]
         node_name, attrs = new_node(self.app.graph, generator_cls.default())
         self.app.global_vars["drag_an_drop"] = (node_name, attrs)
         event.accept()
 
     def refresh(self):
@@ -84,21 +88,19 @@
         """
         self.clear()
 
         # complete the elements
         elements = {}
         for filepath in (
             file for sub_dir in self.sub_dirs
-            for file in (get_project_root() / "core" / sub_dir).rglob("*.py")
+            for file in (get_project_root()/"core"/sub_dir).rglob("*.py")
         ):
-            mod = importlib.import_module(
-                ".".join(
-                    ("cutcutcodec" / filepath.relative_to(get_project_root()).with_suffix("")).parts
-                )
-            )
+            spec = importlib.util.spec_from_file_location("foo", filepath)
+            mod = importlib.util.module_from_spec(spec)
+            spec.loader.exec_module(mod)
             for classname, node_cls in inspect.getmembers(mod):
                 if (
                     inspect.isclass(node_cls)
                     and issubclass(node_cls, Node)
                     and issubclass(node_cls, self.classnames)
                     and classname not in self.excluded_clsn
                 ):
```

### Comparing `movia-1.0.0rc1/cutcutcodec/gui/entry/generators.py` & `movia-1.0a1/movia/gui/entry/generators.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 #!/usr/bin/env python3
 
 """
 ** Allows to view and add all generators. **
 --------------------------------------------
 """
 
-from cutcutcodec.core.classes.container import ContainerInput
-from cutcutcodec.gui.entry.base import Entry
+from movia.core.classes.container import ContainerInput
+from movia.gui.entry.base import Entry
 
 
 
 class Generators(Entry):
     """
     ** Generators visualization window. **
     """
```

### Comparing `movia-1.0.0rc1/cutcutcodec/gui/entry/project_files.py` & `movia-1.0a1/movia/gui/entry/project_files.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 #!/usr/bin/env python3
 
 """
 ** Allows to view and copy/drop new files. **
 ---------------------------------------------
 """
 
+
 import inspect
 import logging
 import pathlib
 
 import numpy as np
 from PyQt6 import QtCore, QtGui, QtWidgets
 
-from cutcutcodec.core.analysis.ffprobe import get_streams_type
-from cutcutcodec.core.io.read import ContainerInputFFMPEG
-from cutcutcodec.gui.entry.base import Entry
+from movia.core.analysis.streams import get_streams_type
+from movia.core.io.read import ContainerInputFFMPEG
+from movia.gui.entry.base import Entry
 
 
 
 class ProjectFiles(Entry):
     """
     ** Imported files visualization window. **
     """
@@ -109,16 +110,12 @@
             img = np.zeros((128, 128, 3), dtype=np.uint8)
             icon = QtGui.QIcon(QtGui.QPixmap(QtGui.QImage(
                 img.data, img.shape[1], img.shape[0], 3*img.shape[1],
                 QtGui.QImage.Format.Format_BGR888
             )))
             item = QtWidgets.QListWidgetItem(icon, pathlib.Path(file).name, parent=self)
             item.setData(
-                3,
-                (
-                    ContainerInputFFMPEG.__name__,
-                    pathlib.Path(inspect.getsourcefile(ContainerInputFFMPEG)).resolve(),
-                ),
+                3, (ContainerInputFFMPEG.__name__, inspect.getsourcefile(ContainerInputFFMPEG))
             ) # 0 for text, 1 for icon, 2 for text, 3 is free!
             item.setData(4, file)
             self.addItem(item)
             self._item2index[item.text()] = index
```

### Comparing `movia-1.0.0rc1/cutcutcodec/gui/entry_tabs.py` & `movia-1.0a1/movia/gui/entry_tabs.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,22 +3,22 @@
 """
 ** The widget that contains all the elements to pick from to add them to the timeline. **
 -----------------------------------------------------------------------------------------
 """
 
 from PyQt6 import QtWidgets
 
-from cutcutcodec.gui.base import CutcutcodecWidget
-from cutcutcodec.gui.entry.filters import Filters
-from cutcutcodec.gui.entry.generators import Generators
-from cutcutcodec.gui.entry.project_files import ProjectFiles
+from movia.gui.base import MoviaWidget
+from movia.gui.entry.filters import Filters
+from movia.gui.entry.generators import Generators
+from movia.gui.entry.project_files import ProjectFiles
 
 
 
-class EntryTabs(CutcutcodecWidget, QtWidgets.QWidget):
+class EntryTabs(MoviaWidget, QtWidgets.QWidget):
     """
     ** Contains the different selection windows. **
     """
 
     def __init__(self, parent):
         super().__init__(parent)
         self._parent = parent
@@ -30,16 +30,16 @@
 
         # location
         tabs = QtWidgets.QTabWidget()
         tabs.addTab(self.project_files, "Project Files")
         tabs.addTab(self.generators, "Generators")
         tabs.addTab(self.filters, "Filters")
         layout = QtWidgets.QVBoxLayout()
-        layout.addWidget(tabs)
         self.setLayout(layout)
+        layout.addWidget(tabs)
 
     def refresh(self):
         """
         ** Updates the elements of this widget and child widgets. **
         """
         self.project_files.refresh()
         self.generators.refresh()
```

### Comparing `movia-1.0.0rc1/cutcutcodec/gui/graph/edge_properties.py` & `movia-1.0a1/movia/gui/graph/edge_properties.py`

 * *Files 15% similar despite different names*

```diff
@@ -5,20 +5,22 @@
 --------------------------------------------------------
 """
 
 import math
 
 from PyQt6 import QtCore, QtWidgets
 
-from cutcutcodec.gui.base import CutcutcodecWidget
-from cutcutcodec.gui.edit_node_state.main import EditNodeWindow
+from movia.core.classes.stream_audio import StreamAudio
+from movia.core.classes.stream_video import StreamVideo
+from movia.gui.base import MoviaWidget
+from movia.gui.node_properties.node_properties import WindowNodeProperties
 
 
 
-class WindowEdgeProperties(CutcutcodecWidget, QtWidgets.QDialog):
+class WindowEdgeProperties(MoviaWidget, QtWidgets.QDialog):
     """
     ** Show the edge properties. **
     """
 
     def __init__(self, parent, edge_name):
         super().__init__(parent)
         self._parent = parent
@@ -83,69 +85,48 @@
         title = QtWidgets.QLabel("Stream Properties")
         title.setAlignment(QtCore.Qt.AlignmentFlag.AlignCenter)
         title.setStyleSheet("font-weight: bold")
         grid_layout.addWidget(title, ref_span, 0, 1, 2)
         ref_span += 1
 
         # the general type
-        grid_layout.addWidget(QtWidgets.QLabel("Type:"), ref_span, 0)
-        grid_layout.addWidget(QtWidgets.QLabel(stream.type.title()), ref_span, 1)
-        ref_span += 1
+        if issubclass(stream.__class__, StreamAudio):
+            grid_layout.addWidget(QtWidgets.QLabel("Type:"), ref_span, 0)
+            grid_layout.addWidget(QtWidgets.QLabel("Audio"), ref_span, 1)
+            ref_span += 1
+        elif issubclass(stream.__class__, StreamVideo):
+            grid_layout.addWidget(QtWidgets.QLabel("Type:"), ref_span, 0)
+            grid_layout.addWidget(QtWidgets.QLabel("Video"), ref_span, 1)
+            ref_span += 1
 
         # all ancestors
         ancestors = " <-- ".join(c.__name__ for c in stream.__class__.__mro__[-2::-1])
         grid_layout.addWidget(QtWidgets.QLabel("Ancestors:"), ref_span, 0)
         grid_layout.addWidget(QtWidgets.QLabel(ancestors), ref_span, 1)
         ref_span += 1
 
-        # beginning
-        beginning = float(stream.beginning)
-        if beginning == math.inf:
-            beginning = "infinite"
-        else:
-            beginning = (
-                f"{round(beginning//3600):0>2}:{round(beginning%3600//60):0>2}:{beginning%60:.3f} "
-                f"({stream.beginning} seconds)"
-            )
-        grid_layout.addWidget(QtWidgets.QLabel("Beginning:"), ref_span, 0)
-        grid_layout.addWidget(QtWidgets.QLabel(beginning), ref_span, 1)
-        ref_span += 1
-
         # duration
         duration = float(stream.duration)
         if duration == math.inf:
             duration = "infinite"
         else:
             duration = (
-                f"{round(duration//3600):0>2}:{round(duration%3600//60):0>2}:{duration%60:.3f} "
-                f"({stream.duration} seconds)"
+                f"{round(duration//3600):0>2}:{round(duration%3600//60):0>2}:{duration%60:.3f}"
             )
         grid_layout.addWidget(QtWidgets.QLabel("Duration:"), ref_span, 0)
         grid_layout.addWidget(QtWidgets.QLabel(duration), ref_span, 1)
         ref_span += 1
 
         # time continuous
         continuous = {True: "yes", False: "no"}[stream.is_time_continuous]
         grid_layout.addWidget(QtWidgets.QLabel("Time is continuous:"), ref_span, 0)
         grid_layout.addWidget(QtWidgets.QLabel(continuous), ref_span, 1)
         ref_span += 1
 
-        # space continuous
-        if stream.type == "video":
-            continuous = {True: "yes", False: "no"}[stream.is_space_continuous]
-            grid_layout.addWidget(QtWidgets.QLabel("Space is continuous:"), ref_span, 0)
-            grid_layout.addWidget(QtWidgets.QLabel(continuous), ref_span, 1)
-            ref_span += 1
-
-        # channels
-        if stream.type == "audio":
-            grid_layout.addWidget(QtWidgets.QLabel("Channels:"), ref_span, 0)
-            grid_layout.addWidget(QtWidgets.QLabel(str(stream.channels)), ref_span, 1)
-            ref_span += 1
-
         return ref_span
 
     def open_procreator(self):
         """
         ** Created and opens the property window for the parent node. **
         """
-        EditNodeWindow(self, self.edge_name[0]).exec()
+        node_win = WindowNodeProperties(self, self.edge_name[0])
+        node_win.exec()
```

### Comparing `movia-1.0.0rc1/cutcutcodec/gui/graph/graph_editor.py` & `movia-1.0a1/movia/gui/graph/graph_editor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 #!/usr/bin/env python3
 
 """
 ** Allows you to view and edit the assembly graph with a ``block`` view. **
 ---------------------------------------------------------------------------
 """
 
+
 import math
 import numbers
 import typing
 
 from PyQt6 import QtCore, QtGui, QtWidgets
 
-from cutcutcodec.core.edit.operation.add import add_edge, add_node
-from cutcutcodec.core.edit.operation.remove import remove_element
-from cutcutcodec.gui.base import CutcutcodecWidget
-from cutcutcodec.gui.graph.edge_properties import WindowEdgeProperties
-from cutcutcodec.gui.graph.layout import (compute_positions, clear_positions,
-    create_and_init_agraph, draw, has_positions, same_structure)
-from cutcutcodec.gui.edit_node_state.main import EditNodeWindow
+from movia.core.edit.operation.add import add_edge, add_node
+from movia.core.edit.operation.remove import remove_element
+from movia.gui.base import MoviaWidget
+from movia.gui.graph.edge_properties import WindowEdgeProperties
+from movia.gui.graph.layout import (compute_positions, clear_positions, create_and_init_agraph,
+    draw, has_positions, same_structure)
+from movia.gui.node_properties.node_properties import WindowNodeProperties
 
 
 
-class GraphEditor(CutcutcodecWidget, QtWidgets.QWidget):
+class GraphEditor(MoviaWidget, QtWidgets.QWidget):
     """
     ** Viewing and editing the assembly graph. **
     """
 
     def __init__(self, parent):
         super().__init__(parent)
         self._parent = parent
@@ -50,15 +51,15 @@
     def dragEnterEvent(self, event):
         """
         ** Drag and drop selection. **
         """
         if not event.mimeData().hasFormat("application/x-qabstractitemmodeldatalist"):
             event.ignore()
             return
-        if self.app.global_vars.get("drag_an_drop", None) is None:
+        if self.app.global_vars["drag_an_drop"] is None:
             event.ignore()
             return
         event.accept()
 
     def dropEvent(self, _):
         """
         ** Drag and drop management. **
@@ -102,15 +103,15 @@
     def refresh(self):
         """
         ** Updates the elements of this widget and child widgets. **
         """
         self.graph_viewer.refresh()
 
 
-class GraphToolBar(CutcutcodecWidget, QtWidgets.QToolBar):
+class GraphToolBar(MoviaWidget, QtWidgets.QToolBar):
     """
     ** This is the toolbar related to graph editing. **
     """
 
     def __init__(self, parent):
         super().__init__(parent)
         self._parent = parent
@@ -140,15 +141,15 @@
         """
         print(f"zoom out (dpi {self.parent.dpi}->", end="")
         self.parent.dpi = max(20, self.parent.dpi / 1.2)
         print(f"{self.parent.dpi})")
         self.parent.refresh()
 
 
-class GraphViewer(CutcutcodecWidget, QtWidgets.QLabel):
+class GraphViewer(MoviaWidget, QtWidgets.QLabel):
     """
     ** Draw the assembly graph. **
     """
 
     def __init__(self, parent):
         super().__init__(parent)
         self._parent = parent
@@ -522,15 +523,15 @@
         """
         name, dist = self.select(event)
         if dist <= 20:
             old_state, self.state = self.state, "loading"
             if isinstance(name, tuple): # element is edge
                 graph_win = WindowEdgeProperties(self, name)
             else: # element is node
-                graph_win = EditNodeWindow(self, name)
+                graph_win = WindowNodeProperties(self, name)
             graph_win.exec()
             self.state = old_state
 
     @property
     def state(self) -> str:
         """
         ** Returns the graph viewer state. **
```

### Comparing `movia-1.0.0rc1/cutcutcodec/gui/graph/layout.py` & `movia-1.0a1/movia/gui/graph/layout.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 
 Note
 ----
 Requires  the ``pygraphviz`` python module and the installation is not very simple.
 See ``https://pygraphviz.github.io/documentation/stable/install.html``.
 """
 
+
 import numbers
 
 import cv2
 import networkx
 import numpy as np
 try:
     import pygraphviz
@@ -112,15 +113,15 @@
     Also initializes node and edge formatting parameters.
     The positioning parameters are not calculated here.
 
     Parameters
     ----------
     graph : networkx.MultiDiGraph
         The assembly graph generated for example by the function
-        ``cutcutcodec.core.compilation.fraph.to_graph.tree_to_graph``.
+        ``movia.core.compilation.fraph.to_graph.tree_to_graph``.
 
     Returns
     -------
     agraph : pygraphviz.AGraph
         The equivalent graphviz version.
     """
     assert isinstance(graph, networkx.MultiDiGraph), graph.__class__.__name__
@@ -160,15 +161,15 @@
     ** Allows to calculate the picture of the graph. **
 
     Parameters
     ----------
     agraph : pygraphviz.AGraph
         The graph you want to draw.
         The graph must be ready. That is to say that the function
-        ``cutcutcodec.gui.graph.layout.compute_positions`` has been called.
+        ``movia.gui.graph.layout.compute_positions`` has been called.
     dpi : int
         The resolution. 100 gives a 'normal' size.
     form : str
         The format of the image. For example "png", jpg", "svg"...
 
     Returns
     -------
```

### Comparing `movia-1.0.0rc1/cutcutcodec/gui/menu.py` & `movia-1.0a1/movia/gui/menu.py`

 * *Files 26% similar despite different names*

```diff
@@ -9,20 +9,15 @@
 
 def fill_menu(menu, actions):
     """
     ** Adds fields to the empty menu. **
     """
 
     file_menu = menu.addMenu("File")
-    file_menu.addAction(actions["open"])
-    file_menu.addAction(actions["save"])
-    file_menu.addAction(actions["save_as"])
-    file_menu.addSeparator()
     file_menu.addAction(actions["import"])
     file_menu.addAction(actions["export"])
+    file_menu.addSeparator()
 
     edit_menu = menu.addMenu("Edit")
     edit_menu.addAction(actions["refresh"])
     edit_menu.addAction(actions["undo"])
     edit_menu.addAction(actions["redo"])
-    edit_menu.addSeparator()
-    edit_menu.addAction(actions["preferences"])
```

### Comparing `movia-1.0.0rc1/cutcutcodec/gui/toolbar.py` & `movia-1.0a1/movia/gui/toolbar.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,33 +3,28 @@
 """
 ** Definition of the toolbar. **
 --------------------------------
 """
 
 from PyQt6 import QtWidgets
 
-from cutcutcodec.gui.base import CutcutcodecWidget
+from movia.gui.base import MoviaWidget
 
 
 
-class MainToolBar(CutcutcodecWidget, QtWidgets.QToolBar):
+class MainToolBar(MoviaWidget, QtWidgets.QToolBar):
     """
     ** Main window menu bar. **
     """
 
     def __init__(self, parent, actions):
         super().__init__(parent)
         self._parent = parent
 
-        self.addAction(actions["import"])
-        self.addAction(actions["open"])
-        self.addAction(actions["save"])
-
-        self.addSeparator()
-
+        # location
         self.addAction(actions["refresh"])
         self.addAction(actions["undo"])
         self.addAction(actions["redo"])
 
         self.addSeparator()
 
         self.addAction(actions["export"])
```

### Comparing `movia-1.0.0rc1/cutcutcodec/utils.py` & `movia-1.0a1/movia/utils.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,18 +11,18 @@
 
 def get_project_root() -> pathlib.Path:
     """
     ** Returns project root folder. **
 
     Examples
     --------
-    >>> from cutcutcodec.utils import get_project_root
+    >>> from movia.utils import get_project_root
     >>> root = get_project_root()
     >>> root.is_dir()
     True
     >>> root.name
-    'cutcutcodec'
+    'movia'
     >>> sorted(p.name for p in root.iterdir())
-    ['__init__.py', '__main__.py', '__pycache__', 'core', 'examples', 'gui', 'testing', 'utils.py']
+    ['__init__.py', '__main__.py', '__pycache__', 'core', 'examples', 'gui', 'tests', 'utils.py']
     >>>
     """
     return pathlib.Path(__file__).parent
```

### Comparing `movia-1.0.0rc1/setup.py` & `movia-1.0a1/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,114 +1,85 @@
 #!/usr/bin/env python3
 
 """
 ** Configuration file for pip. **
 ---------------------------------
 """
 
-import sys
+import setuptools
 
-from setuptools import find_packages, setup
-
-import cutcutcodec
-
-
-if sys.version_info < (3, 9):
-    print(
-        "cutcutcodec requires Python 3.9 or newer. "
-        f"Python {sys.version_info[0]}.{sys.version_info[1]} detected"
-    )
-    sys.exit(-1)
+import movia
 
 
 with open("README.rst", "r", encoding="utf-8") as file:
     long_description = file.read()
 
-
-setup(
+setuptools.setup(
     name="movia",
-    version=cutcutcodec.__version__,
+    version=movia.__version__,
     author="Robin RICHARD (robinechuca)",
     author_email="serveurpython.oz@gmail.com",
     description="video editing softwear",
     long_description=long_description,
     long_description_content_type="text/x-rst",
-    url="https://framagit.org/robinechuca/cutcutcodec/-/blob/main/README.md",
-    data_files=[
-        ("cutcutcodec/", ["README.rst", ".pylintrc"]),
-    ],
-    packages=find_packages(),
-    install_requires=[ # dependences: apt install graphviz-dev ffmpeg
+    url="https://framagit.org/robinechuca/movia/-/blob/main/README.md",
+    packages=setuptools.find_packages(),
+    install_requires=[
         "av", # apt install ffmpeg python3-av
+        "black",
         "click", # apt install python3-click
         "networkx", # apt install python3-networkx
         "numpy >= 1.22", # apt install python3-numpy
         "opencv-contrib-python-headless", # apt install python3-opencv
+        "pdoc3",
+        "pygraphviz", # apt install graphviz graphviz-dev pygraphviz https://pygraphviz.github.io/documentation/stable/install.html
+        "pyqt6", # apt install python3-pyqt6[.sip]
         "sympy", # apt install python3-sympy
-        "torch >= 1.8",
-        "tqdm", # apt install python3-tqdm
         "unidecode", # apt install python3-unidecode
     ],
     extras_require={
-        "gui": [
-            "black", # apt install black python3-pyls-black
-            "pdoc3",
-            "pygraphviz", # https://pygraphviz.github.io/documentation/stable/install.html
-            "pyqt6", # apt install python3-pyqt6[.sip]
-            "pyqtgraph",
-        ], # apt install pylint, python3-pylint-common, python3-pytest
-        "optional": [
-            "black",
-            "pdoc3",
-            "pygraphviz",
-            "pylint",
-            "pyqt6",
-            "pyqtgraph",
-            "pytest",
-        ],
+        "dev": ["pylint", "pytest"] # apt install pylint, python3-pylint-common, python3-pytest
     },
     entry_points={
         "console_scripts": [
-            "cutcutcodec=cutcutcodec.__main__:main",
-            "cutcutcodec-test=cutcutcodec.testing.runtests:test",
-        ],
-        "gui_scripts": [
-            "cutcutcodec-qt=cutcutcodec.gui.__main__:main",
+            "movia=movia.__main__:main",
         ]
     },
     classifiers=[
         "Development Status :: 2 - Pre-Alpha",
         "Environment :: X11 Applications :: Qt",
         "Intended Audience :: Customer Service",
         "License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)",
         "Natural Language :: English",
         "Operating System :: POSIX :: Linux",
         "Programming Language :: Python :: 3",
         "Topic :: Multimedia",
+        "Topic :: Multimedia :: Graphics :: Capture",
         "Topic :: Multimedia :: Graphics :: Editors",
         "Topic :: Multimedia :: Graphics :: Graphics Conversion",
         "Topic :: Multimedia :: Sound/Audio",
         "Topic :: Multimedia :: Sound/Audio :: Analysis",
         "Topic :: Multimedia :: Sound/Audio :: Conversion",
         "Topic :: Multimedia :: Sound/Audio :: Mixers",
         "Topic :: Multimedia :: Sound/Audio :: Players",
         "Topic :: Multimedia :: Video",
+        "Topic :: Multimedia :: Video :: Capture",
         "Topic :: Multimedia :: Video :: Conversion",
         "Topic :: Multimedia :: Video :: Display",
         "Topic :: Multimedia :: Video :: Non-Linear Editor",
         "Topic :: Scientific/Engineering :: Image Processing",
     ],
     keywords=[
         "video",
         "editing",
         "ffmpeg",
         "graphical",
     ],
     python_requires=">=3.9,<3.12",
     project_urls={
-        "Source Repository": "https://framagit.org/robinechuca/movia",
+        "Source Repository": "https://framagit.org/robinechuca/movia/",
         # "Bug Tracker": "https://github.com/engineerjoe440/ElectricPy/issues",
         # "Documentation": "http://python-docs.ddns.net/raisin/",
         # "Packaging tutorial": "https://packaging.python.org/tutorials/distributing-packages/",
         },
     include_package_data=True,
 )
```

