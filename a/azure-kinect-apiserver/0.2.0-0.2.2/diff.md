# Comparing `tmp/azure-kinect-apiserver-0.2.0.tar.gz` & `tmp/azure-kinect-apiserver-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/azure-kinect-apiserver/azure-kinect-apiserver/dist/.tmp-sye7w4ji/azure-kinect-apiserver-0.2.0.tar", last modified: Sun Mar 12 09:27:51 2023, max compression
+gzip compressed data, was "/home/runner/work/azure-kinect-apiserver/azure-kinect-apiserver/dist/.tmp-kl64orx7/azure-kinect-apiserver-0.2.2.tar", last modified: Sun May 21 19:38:04 2023, max compression
```

## Comparing `azure-kinect-apiserver-0.2.0.tar` & `azure-kinect-apiserver-0.2.2.tar`

### file list

```diff
@@ -1,111 +1,114 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 09:27:51.000000 azure-kinect-apiserver-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-03-12 09:27:51.000000 azure-kinect-apiserver-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-03-12 09:27:37.000000 azure-kinect-apiserver-0.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 09:27:51.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-03-12 09:27:37.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-03-12 09:27:37.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 09:27:51.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/apiserver/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-03-12 09:27:37.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/apiserver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14346 2023-03-12 09:27:37.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/apiserver/app.py
--rw-r--r--   0 runner    (1001) docker     (123)     6442 2023-03-12 09:27:37.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/apiserver/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 09:27:51.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-12 09:27:37.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 09:27:51.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/client/restful/
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-03-12 09:27:37.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/client/restful/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 09:27:51.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/client/restful/api/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-12 09:27:37.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/client/restful/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 09:27:51.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/client/restful/api/default/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-12 09:27:37.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/client/restful/api/default/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-03-12 09:27:37.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/client/restful/api/default/get_status_v1_azure_status_get.py
--rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-03-12 09:27:37.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/client/restful/api/default/root_get.py
--rw-r--r--   0 runner    (1001) docker     (123)     5567 2023-03-12 09:27:37.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/client/restful/api/default/single_shot_v1_azure_single_shot_get.py
--rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-03-12 09:27:37.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/client/restful/api/default/start_recording_v1_azure_start_post.py
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-03-12 09:27:37.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/client/restful/api/default/stop_recording_v1_azure_stop_post.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-03-12 09:27:37.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/client/restful/api/default/stop_single_shot_v1_azure_single_shot_delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-03-12 09:27:37.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/client/restful/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-03-12 09:27:37.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/client/restful/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 09:27:51.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/client/restful/models/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-03-12 09:27:37.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/client/restful/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-03-12 09:27:37.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/client/restful/models/http_validation_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-03-12 09:27:37.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/client/restful/models/validation_error.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-03-12 09:27:37.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/client/restful/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 09:27:51.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/cmd/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-03-12 09:27:37.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17413 2023-03-12 09:27:37.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/cmd/analyze.py
--rw-r--r--   0 runner    (1001) docker     (123)     4618 2023-03-12 09:27:37.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/cmd/calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-03-12 09:27:37.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/cmd/configure.py
--rw-r--r--   0 runner    (1001) docker     (123)     7488 2023-03-12 09:27:37.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/cmd/decode.py
--rw-r--r--   0 runner    (1001) docker     (123)    17441 2023-03-12 09:27:37.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/cmd/multical.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 09:27:51.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/common/
--rw-r--r--   0 runner    (1001) docker     (123)    16241 2023-03-12 09:27:37.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/common/Config.py
--rw-r--r--   0 runner    (1001) docker     (123)    11417 2023-03-12 09:27:37.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/common/DataModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-03-12 09:27:37.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/common/MulticalCamera.py
--rw-r--r--   0 runner    (1001) docker     (123)      312 2023-03-12 09:27:37.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16818 2023-03-12 09:27:37.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/common/functional.py
--rw-r--r--   0 runner    (1001) docker     (123)     7142 2023-03-12 09:27:37.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/common/point.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 09:27:51.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/decoder/
--rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-03-12 09:27:37.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/decoder/StateMachine.py
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-03-12 09:27:37.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/decoder/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12499 2023-03-12 09:27:37.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/decoder/aruco.py
--rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-03-12 09:27:37.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/decoder/wrapper.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 09:27:51.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/thirdparty/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-12 09:27:37.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/thirdparty/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 09:27:51.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/thirdparty/pyKinectAzure/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 09:27:51.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-03-12 09:27:39.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 09:27:51.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-03-12 09:27:39.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    33269 2023-03-12 09:27:39.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/_k4a.py
--rw-r--r--   0 runner    (1001) docker     (123)     9256 2023-03-12 09:27:39.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/_k4atypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     7401 2023-03-12 09:27:39.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/calibration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-03-12 09:27:39.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/capture.py
--rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-03-12 09:27:39.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-03-12 09:27:39.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     7675 2023-03-12 09:27:39.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-03-12 09:27:39.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/imu_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-03-12 09:27:39.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/transformation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 09:27:51.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4abt/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-03-12 09:27:39.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4abt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7301 2023-03-12 09:27:39.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4abt/_k4abt.py
--rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-03-12 09:27:39.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4abt/_k4abtTypes.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-03-12 09:27:39.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4abt/body.py
--rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-03-12 09:27:39.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4abt/body2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-03-12 09:27:39.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4abt/frame.py
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-03-12 09:27:39.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4abt/joint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-03-12 09:27:39.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4abt/joint2d.py
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-03-12 09:27:39.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4abt/tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 09:27:51.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4arecord/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-03-12 09:27:39.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4arecord/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18593 2023-03-12 09:27:39.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4arecord/_k4arecord.py
--rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-03-12 09:27:39.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4arecord/_k4arecordTypes.py
--rw-r--r--   0 runner    (1001) docker     (123)      828 2023-03-12 09:27:39.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4arecord/datablock.py
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-03-12 09:27:39.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4arecord/playback.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-03-12 09:27:39.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4arecord/record.py
--rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-03-12 09:27:39.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4arecord/record_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-03-12 09:27:39.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/pykinect.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 09:27:51.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/utils/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-03-12 09:27:39.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-03-12 09:27:39.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/utils/plot3dUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-03-12 09:27:39.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/utils/postProcessing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-03-12 09:27:39.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 09:27:51.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-03-12 09:27:51.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5154 2023-03-12 09:27:51.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-12 09:27:51.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-03-12 09:27:51.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-03-12 09:27:51.000000 azure-kinect-apiserver-0.2.0/azure_kinect_apiserver.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-12 09:27:51.000000 azure-kinect-apiserver-0.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-03-12 09:27:37.000000 azure-kinect-apiserver-0.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 09:27:51.000000 azure-kinect-apiserver-0.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-03-12 09:27:37.000000 azure-kinect-apiserver-0.2.0/tests/test_aruco.py
--rw-r--r--   0 runner    (1001) docker     (123)     7246 2023-03-12 09:27:37.000000 azure-kinect-apiserver-0.2.0/tests/test_chroma_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-03-12 09:27:37.000000 azure-kinect-apiserver-0.2.0/tests/test_client_restful.py
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-03-12 09:27:37.000000 azure-kinect-apiserver-0.2.0/tests/test_decode_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-03-12 09:27:37.000000 azure-kinect-apiserver-0.2.0/tests/test_decode_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-03-12 09:27:37.000000 azure-kinect-apiserver-0.2.0/tests/test_examine_multical_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-03-12 09:27:37.000000 azure-kinect-apiserver-0.2.0/tests/test_filter_chroma.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-03-12 09:27:37.000000 azure-kinect-apiserver-0.2.0/tests/test_filter_chroma_gui.py
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-03-12 09:27:37.000000 azure-kinect-apiserver-0.2.0/tests/test_multical_refinement.py
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-03-12 09:27:37.000000 azure-kinect-apiserver-0.2.0/tests/test_sync_timestamp.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-03-12 09:27:37.000000 azure-kinect-apiserver-0.2.0/tests/test_window_gui.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-03-12 09:27:37.000000 azure-kinect-apiserver-0.2.0/tests/test_wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:38:04.000000 azure-kinect-apiserver-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-05-21 19:38:04.000000 azure-kinect-apiserver-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:38:04.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:38:04.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/apiserver/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/apiserver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14960 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/apiserver/app.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/apiserver/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:38:04.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:38:04.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/client/restful/
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/client/restful/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:38:04.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/client/restful/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/client/restful/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:38:04.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/client/restful/api/default/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/client/restful/api/default/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/client/restful/api/default/get_status_v1_azure_status_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2301 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/client/restful/api/default/root_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5567 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/client/restful/api/default/single_shot_v1_azure_single_shot_get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/client/restful/api/default/start_recording_v1_azure_start_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/client/restful/api/default/stop_recording_v1_azure_stop_post.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/client/restful/api/default/stop_single_shot_v1_azure_single_shot_delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2673 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/client/restful/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/client/restful/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:38:04.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/client/restful/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/client/restful/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2131 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/client/restful/models/http_validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2091 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/client/restful/models/validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/client/restful/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:38:04.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/cmd/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17413 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/cmd/analyze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4679 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/cmd/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/cmd/configure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7407 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/cmd/decode.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17441 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/cmd/multical.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:38:04.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/common/
+-rw-r--r--   0 runner    (1001) docker     (123)    16228 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/common/Config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11417 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/common/DataModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5139 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/common/MulticalCamera.py
+-rw-r--r--   0 runner    (1001) docker     (123)      312 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19671 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/common/functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7138 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/common/point.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:38:04.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/decoder/
+-rw-r--r--   0 runner    (1001) docker     (123)     6753 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/decoder/StateMachine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/decoder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12499 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/decoder/aruco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3883 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/decoder/wrapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:38:04.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:38:04.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:38:04.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-21 19:37:47.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:38:04.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-05-21 19:37:47.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33269 2023-05-21 19:37:47.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/_k4a.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9256 2023-05-21 19:37:47.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/_k4atypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7401 2023-05-21 19:37:47.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-05-21 19:37:47.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/capture.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-05-21 19:37:47.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-05-21 19:37:47.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7675 2023-05-21 19:37:47.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-05-21 19:37:47.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/imu_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3643 2023-05-21 19:37:47.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/transformation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:38:04.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4abt/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-21 19:37:47.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4abt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7301 2023-05-21 19:37:47.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4abt/_k4abt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-05-21 19:37:47.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4abt/_k4abtTypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-21 19:37:47.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4abt/body.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2435 2023-05-21 19:37:47.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4abt/body2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3812 2023-05-21 19:37:47.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4abt/frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-05-21 19:37:47.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4abt/joint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-21 19:37:47.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4abt/joint2d.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-05-21 19:37:47.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4abt/tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:38:04.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4arecord/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-21 19:37:47.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4arecord/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18593 2023-05-21 19:37:47.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4arecord/_k4arecord.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1942 2023-05-21 19:37:47.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4arecord/_k4arecordTypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      828 2023-05-21 19:37:47.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4arecord/datablock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-21 19:37:47.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4arecord/playback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-05-21 19:37:47.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4arecord/record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2961 2023-05-21 19:37:47.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4arecord/record_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-05-21 19:37:47.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/pykinect.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:38:04.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-21 19:37:47.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-21 19:37:47.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/utils/plot3dUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-21 19:37:47.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/utils/postProcessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2267 2023-05-21 19:37:47.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:38:04.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-05-21 19:38:04.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5234 2023-05-21 19:38:04.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 19:38:04.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-21 19:38:04.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-21 19:38:04.000000 azure-kinect-apiserver-0.2.2/azure_kinect_apiserver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 19:38:04.000000 azure-kinect-apiserver-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      804 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 19:38:04.000000 azure-kinect-apiserver-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3958 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/tests/test_aruco.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7246 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/tests/test_chroma_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/tests/test_client_restful.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/tests/test_color_picker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/tests/test_colored_pc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/tests/test_decode_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/tests/test_decode_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/tests/test_examine_multical_result.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/tests/test_filter_chroma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/tests/test_filter_chroma_gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/tests/test_multical_refinement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/tests/test_open3d_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/tests/test_sync_timestamp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/tests/test_window_gui.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-21 19:37:46.000000 azure-kinect-apiserver-0.2.2/tests/test_wrapper.py
```

### Comparing `azure-kinect-apiserver-0.2.0/PKG-INFO` & `azure-kinect-apiserver-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-kinect-apiserver
-Version: 0.2.0
+Version: 0.2.2
 Summary: Azure Kinect APIServer
 Author: davidliyutong
 Author-email: davidliyutong@sjtu.edu.cn
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Azure Kinect APIServer
```

### Comparing `azure-kinect-apiserver-0.2.0/README.md` & `azure-kinect-apiserver-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/__main__.py` & `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/__main__.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/apiserver/app.py` & `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/apiserver/app.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import os
 import os.path as osp
 import signal
 import subprocess
 import threading
 from concurrent.futures import ThreadPoolExecutor
 from typing import Optional, Tuple, Dict, List
+import base64
 
 import cv2
 import numpy as np
 
 from azure_kinect_apiserver.common import KinectSystemCfg, probe_device, MulticalCameraInfo
 from azure_kinect_apiserver.thirdparty import pykinect
 
@@ -295,28 +296,37 @@
             res = []
             for i in range(len(self.device_list)):
                 res.append(executor.submit(self.__save_image__, self.option.data_path, tag, self.serial_map[i], current_frames[i], current_depth_frames[i], index))
             [r.result() for r in res]
 
         return current_frames, current_depth_frames, index, None
 
-    def single_shot_mem(self, tag: Optional[str], index: int) -> Tuple[List[np.ndarray], List[np.ndarray], int, Optional[Exception]]:
+    def single_shot_mem(self, index: int) -> Tuple[List[np.ndarray], List[np.ndarray], int, Optional[Exception]]:
         if not self.state["single_shot"]:
             err = self.enter_single_shot_mode()
             if err is not None:
                 return [], [], -1, err
 
         current_frames: List[Optional[np.ndarray]] = [None for _ in range(len(self.device_list))]
         current_depth_frames: List[Optional[np.ndarray]] = [None for _ in range(len(self.device_list))]
 
         for i in range(len(self.device_list)):
             self.__retrieve_frame__(self.device_list, current_frames, current_depth_frames, i)
 
         return current_frames, current_depth_frames, index, None
 
+    def single_shot_compressed(self, index: int) -> Tuple[List[bytes], List[bytes], int, Optional[Exception]]:
+        color_frames, depth_frames, index, err = self.single_shot_mem(index)
+        if err is not None:
+            return color_frames, depth_frames, index, err
+        else:
+            color_frames_compressed = [base64.b64encode(cv2.imencode('.jpg', frame)[1].tobytes()) for frame in color_frames]
+            depth_frames_compressed = [base64.b64encode(cv2.imencode('.png', frame)[1].tobytes()) for frame in depth_frames]
+            return color_frames_compressed, depth_frames_compressed, index, None
+
     def load_mulitcal_calibration(self, calibration_file: str):
         self.multical_calibration = MulticalCameraInfo(calibration_file)
         if not self.multical_calibration.valid:
             self.logger.warning("invalid multical calibration file")
             self.multical_calibration = None
         else:
             self.logger.info("load multical calibration file")
```

### Comparing `azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/apiserver/server.py` & `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/apiserver/server.py`

 * *Files 3% similar despite different names*

```diff
@@ -68,16 +68,16 @@
     global APPLICATION
     if save:
         _, _, index, err = APPLICATION.single_shot(tag, index)
         return make_response(200, single_shot=APPLICATION.state['single_shot'], depth=None, color=None, index=index, err=str(err))
     else:
         # 4 x 2160p color + depth consumes 210M bandwidth
         # TODO: use a better way to transfer data
-        color_frames, depth_frames, index, err = APPLICATION.single_shot_mem(tag, index)
-        return make_response(200, single_shot=APPLICATION.state['single_shot'], depth=base64.b64encode(pickle.dumps(depth_frames)), color=base64.b64encode(pickle.dumps(color_frames)), index=index,
+        color_frames, depth_frames, index, err = APPLICATION.single_shot_compressed(index)
+        return make_response(200, single_shot=APPLICATION.state['single_shot'], depth=depth_frames, color=color_frames, index=index,
                              ret=str(err))
 
 
 @controller.delete("/v1/azure/single_shot")
 def stop_single_shot():
     global APPLICATION
     APPLICATION.exit_single_shot_mode()
@@ -140,14 +140,15 @@
 
 def join_subprocesses():
     global SUBPROCESSES
     while True:
         if not SUBPROCESSES.empty():
             unique_id, p = SUBPROCESSES.get()
             p.join()
+
             del SUBPROCESSES_DESC[unique_id]
         else:
             time.sleep(60)
 
 
 # noinspection PyUnresolvedReferences
 def main(args):
@@ -187,15 +188,15 @@
             APPLICATION.exit_single_shot_mode()
         # noinspection PyProtectedMember
         os._exit(1)
 
 
 def entry_point(argv):
     parser = argparse.ArgumentParser()
-    parser.add_argument('--config', type=str, default='./azure_kinect_config.yaml', help='path to azure kinect config file')
+    parser.add_argument('--config', type=str, default='./config.yaml', help='path to azure kinect config file')
     parser.add_argument('--multical_calibration', type=str, default=None, help='path to multical calibration file, can be its parent directory')
     args = parser.parse_args(argv)
     main(args)
 
 
 if __name__ == '__main__':
     import sys
```

### Comparing `azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/client/restful/api/default/get_status_v1_azure_status_get.py` & `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/client/restful/api/default/get_status_v1_azure_status_get.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/client/restful/api/default/root_get.py` & `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/client/restful/api/default/root_get.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/client/restful/api/default/single_shot_v1_azure_single_shot_get.py` & `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/client/restful/api/default/single_shot_v1_azure_single_shot_get.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/client/restful/api/default/start_recording_v1_azure_start_post.py` & `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/client/restful/api/default/start_recording_v1_azure_start_post.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/client/restful/api/default/stop_recording_v1_azure_stop_post.py` & `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/client/restful/api/default/stop_recording_v1_azure_stop_post.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/client/restful/api/default/stop_single_shot_v1_azure_single_shot_delete.py` & `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/client/restful/api/default/stop_single_shot_v1_azure_single_shot_delete.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/client/restful/client.py` & `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/client/restful/client.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/client/restful/models/http_validation_error.py` & `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/client/restful/models/http_validation_error.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/client/restful/models/validation_error.py` & `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/client/restful/models/validation_error.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/client/restful/types.py` & `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/client/restful/types.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/cmd/analyze.py` & `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/cmd/analyze.py`

 * *Files 0% similar despite different names*

```diff
@@ -222,15 +222,15 @@
         if enable_finetune and cam_name in finetune_transform.keys():
             cropped_pc.transform(finetune_transform[cam_name])
 
         # convert to realworld
         cropped_pc.transform(cam_info.get_realworld_transmat())
 
         # crop by limits
-        cropped_pc = PointCloudHelper.crop_by_hsv_limits_reverse(cropped_pc, [35, 77], [43, 255], [46, 255])
+        cropped_pc = PointCloudHelper.crop_by_hsv_limits_reverse(cropped_pc, [35, 79], [43, 255], [46, 255])
         cropped_pc = PointCloudHelper.crop_by_xyz_limits(cropped_pc, xlim, ylim, zlim)
 
         # remove outliers
         # _, ind = cropped_pc.remove_radius_outlier(nb_points=50, radius=0.05)
         # cropped_pc = cropped_pc.select_by_index(ind)
         _, ind = cropped_pc.remove_statistical_outlier(nb_neighbors=50, std_ratio=2)
         cropped_pc = cropped_pc.select_by_index(ind)
```

### Comparing `azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/cmd/calibration.py` & `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/cmd/calibration.py`

 * *Files 3% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
 def interaction_loop(app: Application):
     tag = must_parse_cli_string("Please enter a tag for the calibration: ", default_value="cali_" + datetime.datetime.now().strftime("%Y%m%d_%H%M%S"))
     app.enter_single_shot_mode()
     print("--------\nPress 's' or Enter to take a single shot, 'c' or space to refresh preview, 'q' or ESC to quit\n--------")
     index = 0
     while True:
-        color_frames, depth_frames, _, err = app.single_shot_mem(tag, index)
+        color_frames, depth_frames, _, err = app.single_shot_mem(index)
         if err is not None:
             logging.error(f"error: {err}")
             break
 
         scale = int(color_frames[0].shape[0] / 360)
         color_preview = np.vstack([x[::scale, ::scale, :] for x in color_frames])
         cv2.putText(color_preview, f"tag: {tag}, index: {index}", (10, 20), cv2.FONT_HERSHEY_SIMPLEX, 0.5, (255, 255, 255), 1)
@@ -58,24 +58,25 @@
             app.single_shot(tag, index)
             index += 1
         elif k == ord('c') or k == ord(' '):
             continue
 
     with open(osp.join(app.option.data_path, tag, "calibration.json"), "w") as f:
         f.write('{}')
+    logging.info(f"calibration data saved to {osp.join(app.option.data_path, tag)}")
 
 
 def aruco_preview(app: Application):
     app.enter_single_shot_mode()
     ctx = ArucoDetectHelper(
         app.option.marker_length_m,
         getattr(cv2.aruco, app.option.marker_type),
     )
     while True:
-        color_frames, depth_frames, _, err = app.single_shot_mem(None, 0)
+        color_frames, depth_frames, _, err = app.single_shot_mem(0)
         if err is not None:
             logging.error(f"error: {err}")
             continue
 
         scale = int(color_frames[0].shape[0] / 540)
         color_frames = [ctx.preview_one_frame(x)[0] for x in color_frames]
         color_preview = np.vstack([x[::scale, ::scale, :] for x in color_frames])
@@ -114,15 +115,15 @@
         return aruco_preview(Application(cfg))
     else:
         return interaction_loop(Application(cfg))
 
 
 def entry_point(argv):
     parser = argparse.ArgumentParser()
-    parser.add_argument('--config', type=str, default='./azure_kinect_config.yaml')
+    parser.add_argument('--config', type=str, default='./config.yaml')
     parser.add_argument('--aruco_preview', action='store_true')
     print(argv)
 
     args = parser.parse_args(argv)
     return main(args)
```

### Comparing `azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/cmd/decode.py` & `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/cmd/decode.py`

 * *Files 2% similar despite different names*

```diff
@@ -175,13 +175,7 @@
             return 1
 
     else:
         data_dir = argv[0]
         args = argparse.Namespace()
         args.data_dir = data_dir
         return main(args)
-
-
-if __name__ == '__main__':
-    import sys
-
-    exit(entry_point(sys.argv[1:]))
```

### Comparing `azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/cmd/multical.py` & `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/cmd/multical.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/common/Config.py` & `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/common/Config.py`

 * *Files 0% similar despite different names*

```diff
@@ -249,15 +249,15 @@
         if err is not None:
             return args_list, err
         else:
             return [f"{self.exec_path} {x}" for x in args_list], None
 
     @staticmethod
     def configure_from_keyboard() -> bool:
-        output_dir = must_parse_cli_string('Output Directory', './azure_kinect_config.yaml')
+        output_dir = must_parse_cli_string('Output Directory', './config.yaml')
         data_path = must_parse_cli_string('Data Path', './azure_kinect_data')
         exec_path = must_parse_cli_string('Exec Path', 'k4arecorder')
         api_port = must_parse_cli_int('API Port', 1, 65535, 8080)
         api_interface = must_parse_cli_string('API Interface', '0.0.0.0')
         debug = must_parse_cli_bool('Debug', False)
 
         cams, err = probe_device(exec_path)
```

### Comparing `azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/common/DataModel.py` & `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/common/DataModel.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/common/MulticalCamera.py` & `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/common/MulticalCamera.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/common/functional.py` & `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/common/functional.py`

 * *Files 10% similar despite different names*

```diff
@@ -330,14 +330,56 @@
     pcd_points = np.asarray(point_cloud.points)
     pts = pcd_points[pts_sel]
     base, north, west = pts[0], pts[1], pts[2]
 
     return (base, north, west), None
 
 
+def get_nws_points_n(point_cloud: o3d.geometry.PointCloud, n: int) -> Tuple[List[Tuple[np.ndarray, np.ndarray, np.ndarray]], Optional[Exception]]:
+    vis1 = o3d.visualization.VisualizerWithEditing()
+    vis1.create_window('Please press Shift and click 3 Points: Base - North - West. Press Q to exit.')
+    logger.debug('Please press Shift and click 3 Points: Base - North - West. Press Q to exit.')
+    vis1.add_geometry(point_cloud)
+    vis1.update_renderer()
+    vis1.run()  # user picks points
+    vis1.destroy_window()
+
+    pts_sel = vis1.get_picked_points()
+    if len(pts_sel) != 3 * n:
+        return [(np.array([]), np.array([]), np.array([]))], Exception(f"Please select {3 * n} points")
+
+    res = []
+    pcd_points = np.asarray(point_cloud.points)
+    pts = pcd_points[pts_sel]
+    for i in range(n):
+        res.append((pts[i * 3], pts[i * 3 + 1], pts[i * 3 + 2]))
+
+    return res, None
+
+
+def get_color(point_cloud: o3d.geometry.PointCloud, n: int) -> Tuple[List[Tuple[np.ndarray, np.ndarray, np.ndarray]], Optional[Exception]]:
+    vis1 = o3d.visualization.VisualizerWithEditing()
+    vis1.create_window('Please press Shift and click 3 Points: Base - North - West. Press Q to exit.')
+    logger.debug('Please press Shift and click 3 Points: Base - North - West. Press Q to exit.')
+    vis1.add_geometry(point_cloud)
+    vis1.update_renderer()
+    vis1.run()  # user picks points
+    vis1.destroy_window()
+
+    pts_sel = vis1.get_picked_points()
+    if len(pts_sel) != n:
+        return [(np.array([]), np.array([]), np.array([]))], Exception(f"Please select {n} points")
+
+    colors = []
+    pcd_colors = np.asarray(point_cloud.colors)
+    pts = pcd_colors[pts_sel]
+
+    return pts, None
+
+
 def get_trans_mat_by_nws_combined(point_cloud: o3d.geometry.PointCloud) -> Tuple[np.ndarray, np.ndarray, Optional[Exception]]:
     """
     Get transformation matrix by north and west direction, with interaction
 
     :param pc_helper:
     :return:
     """
@@ -359,14 +401,52 @@
          [0, 1, 0]]
     ).T
     rot, trans = rigid_transform_3d(point_set_A, point_set_B)
 
     return rot, trans, None
 
 
+def get_marker_by_nws_combined(point_cloud: o3d.geometry.PointCloud, n: int = 1) -> Tuple[List[np.ndarray], Optional[Exception]]:
+    """
+    Get transformation matrix by north and west direction, with interaction
+
+    :param pc_helper:
+    :return:
+    """
+    points, err = get_nws_points_n(point_cloud, n)
+    if err is not None:
+        return [np.array([])], err
+
+    res = []
+    for (base, north, west) in points:
+        north_direction, west_direction = north - base, west - base
+        north_direction /= np.linalg.norm(north_direction)
+        west_direction /= np.linalg.norm(west_direction)
+
+        point_set_A = np.concatenate((
+            base[:, None],
+            (base + north_direction)[:, None],
+            (base + west_direction)[:, None],
+        ), axis=1)
+        point_set_B = np.array(
+            [[0, 0, 0],
+             [1, 0, 0],
+             [0, 1, 0]]
+        ).T
+        rot, trans = rigid_transform_3d(point_set_A, point_set_B)
+        T = np.eye(4)
+        T[:3, :3] = rot
+        T[:3, 3:4] = trans
+        T = np.linalg.inv(T)
+        T[:3, 3:4] = base[:, None]
+        res.append(T)
+
+    return res, None
+
+
 def get_workspace_limit_by_interaction(point_cloud: o3d.geometry.PointCloud) -> Tuple[List[np.ndarray], Optional[Exception]]:
     """
     Get workspace limit by interaction
 
     :param pc_helper:
     :return:
     """
```

### Comparing `azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/common/point.py` & `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/common/point.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,16 +107,16 @@
         if transform is not None:
             # inv_extrinsic = np.linalg.inv(transform)
             # pcd.transform(inv_extrinsic)
             pcd.transform(transform)
 
         # denoise
         if enable_denoise:
-            # _, ind = pcd.remove_radius_outlier(nb_points=denoise_nb_points, radius=denoise_radius)
-            # pcd = pcd.select_by_index(ind)
+            _, ind = pcd.remove_radius_outlier(nb_points=denoise_nb_points, radius=denoise_radius)
+            pcd = pcd.select_by_index(ind)
             _, ind = pcd.remove_statistical_outlier(nb_neighbors=denoise_nb_neighbors, std_ratio=denoise_std_ratio)
             pcd = pcd.select_by_index(ind)
 
         return pcd
 
     def vis(self, size=0.1):
         coordinate_frame = o3d.geometry.TriangleMesh()
```

### Comparing `azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/decoder/StateMachine.py` & `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/decoder/StateMachine.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/decoder/aruco.py` & `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/decoder/aruco.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/decoder/wrapper.py` & `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/decoder/wrapper.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/_k4a.py` & `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/_k4a.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/_k4atypes.py` & `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/_k4atypes.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/calibration.py` & `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/calibration.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/capture.py` & `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/capture.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/configuration.py` & `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/configuration.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/device.py` & `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/device.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/image.py` & `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/image.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/imu_sample.py` & `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/imu_sample.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/transformation.py` & `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4a/transformation.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4abt/_k4abt.py` & `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4abt/_k4abt.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4abt/_k4abtTypes.py` & `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4abt/_k4abtTypes.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4abt/body.py` & `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4abt/body.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4abt/body2d.py` & `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4abt/body2d.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4abt/frame.py` & `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4abt/frame.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4abt/joint.py` & `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4abt/joint.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4abt/joint2d.py` & `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4abt/joint2d.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4abt/tracker.py` & `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4abt/tracker.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4arecord/_k4arecord.py` & `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4arecord/_k4arecord.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4arecord/_k4arecordTypes.py` & `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4arecord/_k4arecordTypes.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4arecord/datablock.py` & `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4arecord/datablock.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4arecord/playback.py` & `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4arecord/playback.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4arecord/record.py` & `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4arecord/record.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4arecord/record_configuration.py` & `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/k4arecord/record_configuration.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/pykinect.py` & `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/pykinect.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/utils/plot3dUtils.py` & `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/utils/plot3dUtils.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/utils/postProcessing.py` & `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/utils/postProcessing.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.0/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/utils/utils.py` & `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/utils/utils.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.0/azure_kinect_apiserver.egg-info/PKG-INFO` & `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: azure-kinect-apiserver
-Version: 0.2.0
+Version: 0.2.2
 Summary: Azure Kinect APIServer
 Author: davidliyutong
 Author-email: davidliyutong@sjtu.edu.cn
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 # Azure Kinect APIServer
```

### Comparing `azure-kinect-apiserver-0.2.0/azure_kinect_apiserver.egg-info/SOURCES.txt` & `azure-kinect-apiserver-0.2.2/azure_kinect_apiserver.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -74,16 +74,19 @@
 azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/utils/__init__.py
 azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/utils/plot3dUtils.py
 azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/utils/postProcessing.py
 azure_kinect_apiserver/thirdparty/pyKinectAzure/pykinect_azure/utils/utils.py
 tests/test_aruco.py
 tests/test_chroma_filter.py
 tests/test_client_restful.py
+tests/test_color_picker.py
+tests/test_colored_pc.py
 tests/test_decode_file.py
 tests/test_decode_record.py
 tests/test_examine_multical_result.py
 tests/test_filter_chroma.py
 tests/test_filter_chroma_gui.py
 tests/test_multical_refinement.py
+tests/test_open3d_reader.py
 tests/test_sync_timestamp.py
 tests/test_window_gui.py
 tests/test_wrapper.py
```

### Comparing `azure-kinect-apiserver-0.2.0/setup.py` & `azure-kinect-apiserver-0.2.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 from setuptools import setup, find_packages
 
 requires = open("requirements.txt", "r").readlines() if os.path.exists("requirements.txt") else open("./azure_kinect_apiserver.egg-info/requires.txt", "r").readlines()
 print("#-------------------    ", str(os.listdir("./")))
 setup(
     name="azure-kinect-apiserver",
-    version="0.2.0",
+    version="0.2.2",
     author="davidliyutong",
     author_email="davidliyutong@sjtu.edu.cn",
     description="Azure Kinect APIServer",
     packages=find_packages() + ["azure_kinect_apiserver.thirdparty.pyKinectAzure." + pkg for pkg in find_packages('azure_kinect_apiserver/thirdparty/pyKinectAzure')],
     python_requires=">=3.7",
     install_requires=requires,
     long_description=open('README.md', encoding='utf-8').read(),
```

### Comparing `azure-kinect-apiserver-0.2.0/tests/test_aruco.py` & `azure-kinect-apiserver-0.2.2/tests/test_aruco.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.0/tests/test_chroma_filter.py` & `azure-kinect-apiserver-0.2.2/tests/test_chroma_filter.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.0/tests/test_decode_file.py` & `azure-kinect-apiserver-0.2.2/tests/test_decode_file.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.0/tests/test_filter_chroma.py` & `azure-kinect-apiserver-0.2.2/tests/test_filter_chroma.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.0/tests/test_filter_chroma_gui.py` & `azure-kinect-apiserver-0.2.2/tests/test_filter_chroma_gui.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.0/tests/test_window_gui.py` & `azure-kinect-apiserver-0.2.2/tests/test_window_gui.py`

 * *Files identical despite different names*

### Comparing `azure-kinect-apiserver-0.2.0/tests/test_wrapper.py` & `azure-kinect-apiserver-0.2.2/tests/test_wrapper.py`

 * *Files identical despite different names*

