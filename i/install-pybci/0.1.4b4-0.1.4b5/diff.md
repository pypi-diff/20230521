# Comparing `tmp/install-pybci-0.1.4b4.tar.gz` & `tmp/install-pybci-0.1.4b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "install-pybci-0.1.4b4.tar", last modified: Fri May 19 15:43:34 2023, max compression
+gzip compressed data, was "install-pybci-0.1.4b5.tar", last modified: Sun May 21 11:14:36 2023, max compression
```

## Comparing `install-pybci-0.1.4b4.tar` & `install-pybci-0.1.4b5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:43:34.848661 install-pybci-0.1.4b4/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-19 15:42:53.000000 install-pybci-0.1.4b4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-19 15:42:53.000000 install-pybci-0.1.4b4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7932 2023-05-19 15:43:34.844661 install-pybci-0.1.4b4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6970 2023-05-19 15:42:53.000000 install-pybci-0.1.4b4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:43:34.844661 install-pybci-0.1.4b4/install_pybci.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7932 2023-05-19 15:43:34.000000 install-pybci-0.1.4b4/install_pybci.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-19 15:43:34.000000 install-pybci-0.1.4b4/install_pybci.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 15:43:34.000000 install-pybci-0.1.4b4/install_pybci.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-19 15:43:34.000000 install-pybci-0.1.4b4/install_pybci.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-19 15:43:34.000000 install-pybci-0.1.4b4/install_pybci.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:43:34.844661 install-pybci-0.1.4b4/pybci/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:43:34.844661 install-pybci-0.1.4b4/pybci/Configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-19 15:42:53.000000 install-pybci-0.1.4b4/pybci/Configuration/EpochSettings.py
--rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-19 15:42:53.000000 install-pybci-0.1.4b4/pybci/Configuration/FeatureSettings.py
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-19 15:42:53.000000 install-pybci-0.1.4b4/pybci/Configuration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:43:34.844661 install-pybci-0.1.4b4/pybci/ThreadClasses/
--rw-r--r--   0 runner    (1001) docker     (123)     9433 2023-05-19 15:42:53.000000 install-pybci-0.1.4b4/pybci/ThreadClasses/AsyncDataReceiverThread.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-05-19 15:42:53.000000 install-pybci-0.1.4b4/pybci/ThreadClasses/ClassifierThread.py
--rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-05-19 15:42:53.000000 install-pybci-0.1.4b4/pybci/ThreadClasses/DataReceiverThread.py
--rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-05-19 15:42:53.000000 install-pybci-0.1.4b4/pybci/ThreadClasses/FeatureProcessorThread.py
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-19 15:42:53.000000 install-pybci-0.1.4b4/pybci/ThreadClasses/MarkerThread.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-19 15:42:53.000000 install-pybci-0.1.4b4/pybci/ThreadClasses/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 15:43:34.844661 install-pybci-0.1.4b4/pybci/Utils/
--rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-05-19 15:42:53.000000 install-pybci-0.1.4b4/pybci/Utils/Classifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     7119 2023-05-19 15:42:53.000000 install-pybci-0.1.4b4/pybci/Utils/FeatureExtractor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-05-19 15:42:53.000000 install-pybci-0.1.4b4/pybci/Utils/LSLScanner.py
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-19 15:42:53.000000 install-pybci-0.1.4b4/pybci/Utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-19 15:42:53.000000 install-pybci-0.1.4b4/pybci/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13841 2023-05-19 15:42:53.000000 install-pybci-0.1.4b4/pybci/pybci.py
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-19 15:42:53.000000 install-pybci-0.1.4b4/pybci/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-19 15:43:34.848661 install-pybci-0.1.4b4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-05-19 15:42:53.000000 install-pybci-0.1.4b4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:14:36.533807 install-pybci-0.1.4b5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-21 11:14:04.000000 install-pybci-0.1.4b5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-21 11:14:04.000000 install-pybci-0.1.4b5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7291 2023-05-21 11:14:36.533807 install-pybci-0.1.4b5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6329 2023-05-21 11:14:04.000000 install-pybci-0.1.4b5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:14:36.533807 install-pybci-0.1.4b5/install_pybci.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7291 2023-05-21 11:14:36.000000 install-pybci-0.1.4b5/install_pybci.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      731 2023-05-21 11:14:36.000000 install-pybci-0.1.4b5/install_pybci.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 11:14:36.000000 install-pybci-0.1.4b5/install_pybci.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-21 11:14:36.000000 install-pybci-0.1.4b5/install_pybci.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-21 11:14:36.000000 install-pybci-0.1.4b5/install_pybci.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:14:36.533807 install-pybci-0.1.4b5/pybci/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:14:36.533807 install-pybci-0.1.4b5/pybci/Configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-21 11:14:05.000000 install-pybci-0.1.4b5/pybci/Configuration/EpochSettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-21 11:14:05.000000 install-pybci-0.1.4b5/pybci/Configuration/FeatureSettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-21 11:14:05.000000 install-pybci-0.1.4b5/pybci/Configuration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:14:36.533807 install-pybci-0.1.4b5/pybci/ThreadClasses/
+-rw-r--r--   0 runner    (1001) docker     (123)     9433 2023-05-21 11:14:05.000000 install-pybci-0.1.4b5/pybci/ThreadClasses/AsyncDataReceiverThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-05-21 11:14:05.000000 install-pybci-0.1.4b5/pybci/ThreadClasses/ClassifierThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-05-21 11:14:05.000000 install-pybci-0.1.4b5/pybci/ThreadClasses/DataReceiverThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5176 2023-05-21 11:14:05.000000 install-pybci-0.1.4b5/pybci/ThreadClasses/FeatureProcessorThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-05-21 11:14:05.000000 install-pybci-0.1.4b5/pybci/ThreadClasses/MarkerThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 11:14:05.000000 install-pybci-0.1.4b5/pybci/ThreadClasses/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 11:14:36.533807 install-pybci-0.1.4b5/pybci/Utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     4781 2023-05-21 11:14:05.000000 install-pybci-0.1.4b5/pybci/Utils/Classifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7119 2023-05-21 11:14:05.000000 install-pybci-0.1.4b5/pybci/Utils/FeatureExtractor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5554 2023-05-21 11:14:05.000000 install-pybci-0.1.4b5/pybci/Utils/LSLScanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-21 11:14:05.000000 install-pybci-0.1.4b5/pybci/Utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-21 11:14:05.000000 install-pybci-0.1.4b5/pybci/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14618 2023-05-21 11:14:05.000000 install-pybci-0.1.4b5/pybci/pybci.py
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-21 11:14:05.000000 install-pybci-0.1.4b5/pybci/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 11:14:36.533807 install-pybci-0.1.4b5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     4966 2023-05-21 11:14:05.000000 install-pybci-0.1.4b5/setup.py
```

### Comparing `install-pybci-0.1.4b4/LICENSE` & `install-pybci-0.1.4b5/LICENSE`

 * *Files identical despite different names*

### Comparing `install-pybci-0.1.4b4/PKG-INFO` & `install-pybci-0.1.4b5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: install-pybci
-Version: 0.1.4b4
+Version: 0.1.4b5
 Summary: A Python interface to create a BCI with the Lab Streaming Layer, scikit-learn and tensorflow packages
 Home-page: https://github.com/lmbooth/pybci
 Author: Liam Booth
 Author-email: liambooth123@hotmail.co.uk
 License: MIT
 Keywords: machine learning and data synchronisation on the Lab Streaming Layer
 Classifier: Development Status :: 4 - Beta
@@ -20,82 +20,69 @@
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/install-pybci)](https://pypi.org/project/install-pybci)  [![Documentation Status](https://readthedocs.org/projects/pybci/badge/?version=latest)](https://pybci.readthedocs.io/en/latest/?badge=latest)
 
-![Alt Text](https://github.com/LMBooth/pybci/blob/main/docs/Images/pyBCITitle.png)
+[![Alt Text](https://github.com/LMBooth/pybci/blob/main/docs/Images/pyBCITitle.png)](https://github.com/LMBooth/pybci)
 
-A Python interface to create a Brain Computer Interface (BCI) with the [Lab Streaming Layer](https://github.com/sccn/labstreaminglayer), [scikit-learn](https://scikit-learn.org/stable/#) and [TensorFlow](https://www.tensorflow.org/install) packages, leveraging packages like [AntroPy](https://github.com/raphaelvallat/antropy), [SciPy](https://scipy.org/) and [NumPy](https://numpy.org/) for time and/or frequency based feature extraction.
+A Python package to create a Brain Computer Interface (BCI) with data synchronisation and pipelining handled by the [Lab Streaming Layer](https://github.com/sccn/labstreaminglayer), machine learning with [scikit-learn](https://scikit-learn.org/stable/#) and [TensorFlow](https://www.tensorflow.org/install), leveraging packages like [AntroPy](https://github.com/raphaelvallat/antropy), [SciPy](https://scipy.org/) and [NumPy](https://numpy.org/) for generic time and/or frequency based feature extraction or optionally have the users own custom feature extraction class used.
 
-The goal of PyBCI is to help create quick iteration pipelines for testing potential human machine and brain computer interfaces, namely applied machine learning models and feature extraction techniques.
+The goal of PyBCI is to help create quick iteration pipelines for testing potential human machine and brain computer interfaces, namely testing applied machine learning models, data processing, and feature extraction techniques for LSL enabled devices and training stimuli.
 
 ## Installation
 For stable releases use: ```pip install install-pybci```
-(currently can only install-pybci due to pybci name similarities with another package on pypi)
 
 For unstable dev installations and up-to-date git pushes use: ```pip install --index-url https://test.pypi.org/simple/ install-pybci```
 
+(currently using install-pybci due to pybci having name too similar with another package on pypi)
 
-[ReadTheDocs available here!](https://pybci.readthedocs.io/en/latest/) (In development)
+[ReadTheDocs available here!](https://pybci.readthedocs.io/en/latest/)      [Examples found here!](https://github.com/LMBooth/pybci/tree/main/pybci/Examples)
 
 ## Basic implementation
 ```python
 import time
 from pybci import PyBCI
-bci = PyBCI()
-while not bci.connected:
+bci = PyBCI(minimumEpochsRequired = 4)
+while not bci.connected: # check to see if lsl marker and datastream are available
     bci.Connect()
     time.sleep(1)
-bci.TrainMode()
-while(True):
-    currentMarkers = bci.ReceivedMarkerCount()
-    time.sleep(1) # wait for marker updates
-    if len(currentMarkers) > 1:  # check there is more then one marker type received
-        if min([currentMarkers[key][1] for key in currentMarkers]) > 10:
-            bci.TestMode()
-            break 
+bci.TrainMode() # now both marker and datastreams available start training on received epochs
+accuracy = 0
 try:
-    while True:
-        classInfo = bci.CurrentClassifierInfo() # when in train mode only y_pred returned
-        guess = [key for key, value in currentMarkers.items() if value[0] == classInfo["y_pred"]]
+    while(True): # training based on couple epochs more then min threshold for classifying
+        currentMarkers = bci.ReceivedMarkerCount() # check to see how many received epochs, if markers sent to close together will be ignored till done processing
+        time.sleep(1) # wait for marker updates
+        print("Markers received: " + str(currentMarkers) +" Class accuracy: " + str(accuracy), end="\r")
+        if len(currentMarkers) > 1:  # check there is more then one marker type received
+            if min([currentMarkers[key][1] for key in currentMarkers]) > bci.minimumEpochsRequired:
+                classInfo = bci.CurrentClassifierInfo() # hangs if called too early
+                accuracy = classInfo["accuracy"]
+            if min([currentMarkers[key][1] for key in currentMarkers]) > bci.minimumEpochsRequired+1:  
+                bci.TestMode()
+                break
+    while True: # now sufficient epochs gathered start testing
+        markerGuess = bci.CurrentClassifierMarkerGuess() # when in test mode only y_pred returned
+        guess = [key for key, value in currentMarkers.items() if value[0] == markerGuess]
         print("Current marker estimation: " + str(guess), end="\r")
+        time.sleep(0.5)
 except KeyboardInterrupt: # allow user to break while loop
     pass
 ```
 
 ## Background Information
-PyBCI is a python based brain computer interface software designed to receive a varying number, be it singular or multiple, [Lab Streaming Layer](https://github.com/sccn/labstreaminglayer) enabled physiological sensor data streams. An understanding of time-series data analysis, the lab streaming layer protocol, and machine learning techniques are a must to integrate innovative ideas with this interface.
-An LSL marker stream is required to train the model, where a received marker [epochs](https://www.google.com/search?q=epochs+definition&rlz=1C1CHBF_en-GBGB921GB921&sxsrf=APwXEddAlMkYQ6MqziIvXbvsCxl3SjySNA%3A1684343462996&ei=pgplZJK2PJiigAaErrWwCw&oq=epochs+def&gs_lcp=Cgxnd3Mtd2l6LXNlcnAQAxgAMg0IABCKBRCRAhBGEPkBMgUIABCABDIFCAAQgAQyBQgAEIAEMggIABAWEB4QDzIICAAQFhAeEA8yBggAEBYQHjIGCAAQFhAeMgYIABAWEB4yCQgAEBYQHhDxBDoHCCMQsAMQJzoKCAAQRxDWBBCwAzoHCCMQigUQJzoHCAAQigUQQzoNCAAQigUQsQMQgwEQQzoICAAQigUQkQJKBAhBGABQmAZYwQhgzw5oAXABeACAAYYBiAHBA5IBAzEuM5gBAKABAcgBCsABAQ&sclient=gws-wiz-serp) the data received on the accepted datastreams based on a configurable time window around certain markers - where custom marker strings can optionally have its epoch timewindow split and overlapped to count for more then one marker, example: a baseline marker may have one marker sent for a 60 second window, where as target actions may only be ~0.5s long, so to conform when testing the model and giving a standardised window length would be desirable to split the 60s window after the received baseline marker in to ~0.5s windows. By overlapping windows we try to account for potential missed signal patterns/aliasing, as a rule of thumb it would be advised when testing a model to have an overlap >= than 50%, [see Shannon nyquist criterion](https://en.wikipedia.org/wiki/Nyquist%E2%80%93Shannon_sampling_theorem).
+PyBCI is a python based brain computer interface software designed to receive a varying number, be it singular or multiple, Lab Streaming Layer enabled physiological sensor data streams. An understanding of time-series data analysis, the lab streaming layer protocol, and machine learning techniques are a must to integrate innovative ideas with this interface. An LSL marker stream is required to train the model, where a received marker epochs the data received on the accepted datastreams based on a configurable time window around certain markers - where custom marker strings can optionally have its epoch timewindow split and overlapped to count for more then one marker, example: a baseline marker may have one marker sent for a 60 second window, where as target actions may only be ~0.5s long, so to conform when testing the model and giving a standardised window length would be desirable to split the 60s window after the received baseline marker in to ~0.5s windows. By overlapping windows we try to account for potential missed signal patterns/aliasing, as a rule of thumb it would be advised when testing a model to have an overlap >= than 50%, see Shannon nyquist criterion.
 
-Once the data has been epoched it is sent for feature extraction, there is a general feature extraction class which can be configured for general time and/or frequency analysis based features, data streams types like "EEG" and "EMG". (DevNOTE: looking to write class for basic pupil labs example to be passed, or solely samples + channels, or other custom classes passed to selected marker streams >:] )
+Once the data has been epoched it is sent for feature extraction, there is a general feature extraction class which can be configured for general time and/or frequency analysis based features, data streams types like "EEG" and "EMG", since data analysis, preprocessing and feature extraction between devices can vary greatly, this is why custom feature extraction classes can be created for each data stream maker type. 
 
 Finally a passable, customisable sklearn or tensorflow classifier can be giving to the bci class, once a defined number of epochs have been obtained for each received epoch/marker type the classifier can begin to fit the model. It's advised to use bci.ReceivedMarkerCount() to get the number of received training epochs received, once the min num epochs received of each type is >= pybci.minimumEpochsRequired (default 10 of each epoch) the mdoel will begin to fit. Once fit classifier info can be queried with CurrentClassifierInfo, when a desired accuracy is met or number of epochs TestMode() can be called. Once in test mode you can query (sould change function to own function and queue for quering testthread) what pybci estimates the current bci epoch is(typically bseline is used for no state).
 
-If you have no LSL available hardware, a psuedo time-series signal can be created with the script found in [mainSend.py PsuedoLSLStreamGenerator folder](https://github.com/LMBooth/pybci/tree/main/pybci/Examples/PsuedoLSLStreamGenerator/mainSend.py). 
+The [examples folder](https://github.com/LMBooth/pybci/tree/main/pybci/Examples) found on the github has a [pseudo LSL data generator and marker creator](https://github.com/LMBooth/pybci/tree/main/pybci/Examples/PsuedoLSLStreamGenerator) in the [mainSend.py](https://github.com/LMBooth/pybci/tree/main/pybci/Examples/PsuedoLSLStreamGenerator/mainSend.py) file so the examples can run without the need of LSL capable hardware. 
+
 
 
-## Theory of Operation
-1. Requirements Prior Initialising with ```python bci = PyBCI() ```
-    - The bci must have >=1 LSL datastream with an accepted dataType ("EEG", "EMG", "Gaze") {hopefully configurable in the future t pass custom fature decoding class}
-    - The bci must have ==1 LSL markerstream selected (if more then one LSL marker stream on system set the desired ML training marker stream with PyBCI(markerStream="yourMarkerStream")). Warning: If None set picks first available in list.
-2. Initialising BCI software
-    - [Optional Configurations](https://pybci.readthedocs.io/en/latest/api/PyBCI.html) for ```python PyBCI() ```
-    - Once configuration settings are set various threads are created.
-        - The marker stream has its own thread which recieves markers from the target LSL marker stream and when in train mode pushes this marker to the available datastreams. 
-        - Each data stream has its own thread created responsible for pipleining received data on FIFO's and slicing approprialey based on globalEpochSettings and customEpochSettings.
-        - FeaturesExtractor
-        - Classifier
-    
-3. ML Training:
-  
-4. ML Testing:
 
 ## ToDo!
-- 
-### Future Work
-- Add simple gaze decoding from pupil-labs
-- Create example to output classification on LSL and make test train configurable on pure LSL markers 
-- custom class passable for data decoding, use general and gaze for inpiration. 
+- Combine multiple data streams for multi modal bci!
 
-## Curently in Alpha, come back in a few days for updates!
+## Curently in Beta, come back in a few days for updates!
```

### Comparing `install-pybci-0.1.4b4/README.md` & `install-pybci-0.1.4b5/install_pybci.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,77 +1,88 @@
+Metadata-Version: 2.1
+Name: install-pybci
+Version: 0.1.4b5
+Summary: A Python interface to create a BCI with the Lab Streaming Layer, scikit-learn and tensorflow packages
+Home-page: https://github.com/lmbooth/pybci
+Author: Liam Booth
+Author-email: liambooth123@hotmail.co.uk
+License: MIT
+Keywords: machine learning and data synchronisation on the Lab Streaming Layer
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: Topic :: System :: Networking
+Classifier: Topic :: Scientific/Engineering
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: Microsoft :: Windows
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Operating System :: MacOS
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/install-pybci)](https://pypi.org/project/install-pybci)  [![Documentation Status](https://readthedocs.org/projects/pybci/badge/?version=latest)](https://pybci.readthedocs.io/en/latest/?badge=latest)
 
-![Alt Text](https://github.com/LMBooth/pybci/blob/main/docs/Images/pyBCITitle.png)
+[![Alt Text](https://github.com/LMBooth/pybci/blob/main/docs/Images/pyBCITitle.png)](https://github.com/LMBooth/pybci)
 
-A Python interface to create a Brain Computer Interface (BCI) with the [Lab Streaming Layer](https://github.com/sccn/labstreaminglayer), [scikit-learn](https://scikit-learn.org/stable/#) and [TensorFlow](https://www.tensorflow.org/install) packages, leveraging packages like [AntroPy](https://github.com/raphaelvallat/antropy), [SciPy](https://scipy.org/) and [NumPy](https://numpy.org/) for time and/or frequency based feature extraction.
+A Python package to create a Brain Computer Interface (BCI) with data synchronisation and pipelining handled by the [Lab Streaming Layer](https://github.com/sccn/labstreaminglayer), machine learning with [scikit-learn](https://scikit-learn.org/stable/#) and [TensorFlow](https://www.tensorflow.org/install), leveraging packages like [AntroPy](https://github.com/raphaelvallat/antropy), [SciPy](https://scipy.org/) and [NumPy](https://numpy.org/) for generic time and/or frequency based feature extraction or optionally have the users own custom feature extraction class used.
 
-The goal of PyBCI is to help create quick iteration pipelines for testing potential human machine and brain computer interfaces, namely applied machine learning models and feature extraction techniques.
+The goal of PyBCI is to help create quick iteration pipelines for testing potential human machine and brain computer interfaces, namely testing applied machine learning models, data processing, and feature extraction techniques for LSL enabled devices and training stimuli.
 
 ## Installation
 For stable releases use: ```pip install install-pybci```
-(currently can only install-pybci due to pybci name similarities with another package on pypi)
 
 For unstable dev installations and up-to-date git pushes use: ```pip install --index-url https://test.pypi.org/simple/ install-pybci```
 
+(currently using install-pybci due to pybci having name too similar with another package on pypi)
 
-[ReadTheDocs available here!](https://pybci.readthedocs.io/en/latest/) (In development)
+[ReadTheDocs available here!](https://pybci.readthedocs.io/en/latest/)      [Examples found here!](https://github.com/LMBooth/pybci/tree/main/pybci/Examples)
 
 ## Basic implementation
 ```python
 import time
 from pybci import PyBCI
-bci = PyBCI()
-while not bci.connected:
+bci = PyBCI(minimumEpochsRequired = 4)
+while not bci.connected: # check to see if lsl marker and datastream are available
     bci.Connect()
     time.sleep(1)
-bci.TrainMode()
-while(True):
-    currentMarkers = bci.ReceivedMarkerCount()
-    time.sleep(1) # wait for marker updates
-    if len(currentMarkers) > 1:  # check there is more then one marker type received
-        if min([currentMarkers[key][1] for key in currentMarkers]) > 10:
-            bci.TestMode()
-            break 
+bci.TrainMode() # now both marker and datastreams available start training on received epochs
+accuracy = 0
 try:
-    while True:
-        classInfo = bci.CurrentClassifierInfo() # when in train mode only y_pred returned
-        guess = [key for key, value in currentMarkers.items() if value[0] == classInfo["y_pred"]]
+    while(True): # training based on couple epochs more then min threshold for classifying
+        currentMarkers = bci.ReceivedMarkerCount() # check to see how many received epochs, if markers sent to close together will be ignored till done processing
+        time.sleep(1) # wait for marker updates
+        print("Markers received: " + str(currentMarkers) +" Class accuracy: " + str(accuracy), end="\r")
+        if len(currentMarkers) > 1:  # check there is more then one marker type received
+            if min([currentMarkers[key][1] for key in currentMarkers]) > bci.minimumEpochsRequired:
+                classInfo = bci.CurrentClassifierInfo() # hangs if called too early
+                accuracy = classInfo["accuracy"]
+            if min([currentMarkers[key][1] for key in currentMarkers]) > bci.minimumEpochsRequired+1:  
+                bci.TestMode()
+                break
+    while True: # now sufficient epochs gathered start testing
+        markerGuess = bci.CurrentClassifierMarkerGuess() # when in test mode only y_pred returned
+        guess = [key for key, value in currentMarkers.items() if value[0] == markerGuess]
         print("Current marker estimation: " + str(guess), end="\r")
+        time.sleep(0.5)
 except KeyboardInterrupt: # allow user to break while loop
     pass
 ```
 
 ## Background Information
-PyBCI is a python based brain computer interface software designed to receive a varying number, be it singular or multiple, [Lab Streaming Layer](https://github.com/sccn/labstreaminglayer) enabled physiological sensor data streams. An understanding of time-series data analysis, the lab streaming layer protocol, and machine learning techniques are a must to integrate innovative ideas with this interface.
-An LSL marker stream is required to train the model, where a received marker [epochs](https://www.google.com/search?q=epochs+definition&rlz=1C1CHBF_en-GBGB921GB921&sxsrf=APwXEddAlMkYQ6MqziIvXbvsCxl3SjySNA%3A1684343462996&ei=pgplZJK2PJiigAaErrWwCw&oq=epochs+def&gs_lcp=Cgxnd3Mtd2l6LXNlcnAQAxgAMg0IABCKBRCRAhBGEPkBMgUIABCABDIFCAAQgAQyBQgAEIAEMggIABAWEB4QDzIICAAQFhAeEA8yBggAEBYQHjIGCAAQFhAeMgYIABAWEB4yCQgAEBYQHhDxBDoHCCMQsAMQJzoKCAAQRxDWBBCwAzoHCCMQigUQJzoHCAAQigUQQzoNCAAQigUQsQMQgwEQQzoICAAQigUQkQJKBAhBGABQmAZYwQhgzw5oAXABeACAAYYBiAHBA5IBAzEuM5gBAKABAcgBCsABAQ&sclient=gws-wiz-serp) the data received on the accepted datastreams based on a configurable time window around certain markers - where custom marker strings can optionally have its epoch timewindow split and overlapped to count for more then one marker, example: a baseline marker may have one marker sent for a 60 second window, where as target actions may only be ~0.5s long, so to conform when testing the model and giving a standardised window length would be desirable to split the 60s window after the received baseline marker in to ~0.5s windows. By overlapping windows we try to account for potential missed signal patterns/aliasing, as a rule of thumb it would be advised when testing a model to have an overlap >= than 50%, [see Shannon nyquist criterion](https://en.wikipedia.org/wiki/Nyquist%E2%80%93Shannon_sampling_theorem).
+PyBCI is a python based brain computer interface software designed to receive a varying number, be it singular or multiple, Lab Streaming Layer enabled physiological sensor data streams. An understanding of time-series data analysis, the lab streaming layer protocol, and machine learning techniques are a must to integrate innovative ideas with this interface. An LSL marker stream is required to train the model, where a received marker epochs the data received on the accepted datastreams based on a configurable time window around certain markers - where custom marker strings can optionally have its epoch timewindow split and overlapped to count for more then one marker, example: a baseline marker may have one marker sent for a 60 second window, where as target actions may only be ~0.5s long, so to conform when testing the model and giving a standardised window length would be desirable to split the 60s window after the received baseline marker in to ~0.5s windows. By overlapping windows we try to account for potential missed signal patterns/aliasing, as a rule of thumb it would be advised when testing a model to have an overlap >= than 50%, see Shannon nyquist criterion.
 
-Once the data has been epoched it is sent for feature extraction, there is a general feature extraction class which can be configured for general time and/or frequency analysis based features, data streams types like "EEG" and "EMG". (DevNOTE: looking to write class for basic pupil labs example to be passed, or solely samples + channels, or other custom classes passed to selected marker streams >:] )
+Once the data has been epoched it is sent for feature extraction, there is a general feature extraction class which can be configured for general time and/or frequency analysis based features, data streams types like "EEG" and "EMG", since data analysis, preprocessing and feature extraction between devices can vary greatly, this is why custom feature extraction classes can be created for each data stream maker type. 
 
 Finally a passable, customisable sklearn or tensorflow classifier can be giving to the bci class, once a defined number of epochs have been obtained for each received epoch/marker type the classifier can begin to fit the model. It's advised to use bci.ReceivedMarkerCount() to get the number of received training epochs received, once the min num epochs received of each type is >= pybci.minimumEpochsRequired (default 10 of each epoch) the mdoel will begin to fit. Once fit classifier info can be queried with CurrentClassifierInfo, when a desired accuracy is met or number of epochs TestMode() can be called. Once in test mode you can query (sould change function to own function and queue for quering testthread) what pybci estimates the current bci epoch is(typically bseline is used for no state).
 
-If you have no LSL available hardware, a psuedo time-series signal can be created with the script found in [mainSend.py PsuedoLSLStreamGenerator folder](https://github.com/LMBooth/pybci/tree/main/pybci/Examples/PsuedoLSLStreamGenerator/mainSend.py). 
+The [examples folder](https://github.com/LMBooth/pybci/tree/main/pybci/Examples) found on the github has a [pseudo LSL data generator and marker creator](https://github.com/LMBooth/pybci/tree/main/pybci/Examples/PsuedoLSLStreamGenerator) in the [mainSend.py](https://github.com/LMBooth/pybci/tree/main/pybci/Examples/PsuedoLSLStreamGenerator/mainSend.py) file so the examples can run without the need of LSL capable hardware. 
+
 
 
-## Theory of Operation
-1. Requirements Prior Initialising with ```python bci = PyBCI() ```
-    - The bci must have >=1 LSL datastream with an accepted dataType ("EEG", "EMG", "Gaze") {hopefully configurable in the future t pass custom fature decoding class}
-    - The bci must have ==1 LSL markerstream selected (if more then one LSL marker stream on system set the desired ML training marker stream with PyBCI(markerStream="yourMarkerStream")). Warning: If None set picks first available in list.
-2. Initialising BCI software
-    - [Optional Configurations](https://pybci.readthedocs.io/en/latest/api/PyBCI.html) for ```python PyBCI() ```
-    - Once configuration settings are set various threads are created.
-        - The marker stream has its own thread which recieves markers from the target LSL marker stream and when in train mode pushes this marker to the available datastreams. 
-        - Each data stream has its own thread created responsible for pipleining received data on FIFO's and slicing approprialey based on globalEpochSettings and customEpochSettings.
-        - FeaturesExtractor
-        - Classifier
-    
-3. ML Training:
-  
-4. ML Testing:
 
 ## ToDo!
-- 
-### Future Work
-- Add simple gaze decoding from pupil-labs
-- Create example to output classification on LSL and make test train configurable on pure LSL markers 
-- custom class passable for data decoding, use general and gaze for inpiration. 
+- Combine multiple data streams for multi modal bci!
 
-## Curently in Alpha, come back in a few days for updates!
+## Curently in Beta, come back in a few days for updates!
```

### Comparing `install-pybci-0.1.4b4/install_pybci.egg-info/PKG-INFO` & `install-pybci-0.1.4b5/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,101 +1,64 @@
-Metadata-Version: 2.1
-Name: install-pybci
-Version: 0.1.4b4
-Summary: A Python interface to create a BCI with the Lab Streaming Layer, scikit-learn and tensorflow packages
-Home-page: https://github.com/lmbooth/pybci
-Author: Liam Booth
-Author-email: liambooth123@hotmail.co.uk
-License: MIT
-Keywords: machine learning and data synchronisation on the Lab Streaming Layer
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: System :: Networking
-Classifier: Topic :: Scientific/Engineering
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: Microsoft :: Windows
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Operating System :: MacOS
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/install-pybci)](https://pypi.org/project/install-pybci)  [![Documentation Status](https://readthedocs.org/projects/pybci/badge/?version=latest)](https://pybci.readthedocs.io/en/latest/?badge=latest)
 
-![Alt Text](https://github.com/LMBooth/pybci/blob/main/docs/Images/pyBCITitle.png)
+[![Alt Text](https://github.com/LMBooth/pybci/blob/main/docs/Images/pyBCITitle.png)](https://github.com/LMBooth/pybci)
 
-A Python interface to create a Brain Computer Interface (BCI) with the [Lab Streaming Layer](https://github.com/sccn/labstreaminglayer), [scikit-learn](https://scikit-learn.org/stable/#) and [TensorFlow](https://www.tensorflow.org/install) packages, leveraging packages like [AntroPy](https://github.com/raphaelvallat/antropy), [SciPy](https://scipy.org/) and [NumPy](https://numpy.org/) for time and/or frequency based feature extraction.
+A Python package to create a Brain Computer Interface (BCI) with data synchronisation and pipelining handled by the [Lab Streaming Layer](https://github.com/sccn/labstreaminglayer), machine learning with [scikit-learn](https://scikit-learn.org/stable/#) and [TensorFlow](https://www.tensorflow.org/install), leveraging packages like [AntroPy](https://github.com/raphaelvallat/antropy), [SciPy](https://scipy.org/) and [NumPy](https://numpy.org/) for generic time and/or frequency based feature extraction or optionally have the users own custom feature extraction class used.
 
-The goal of PyBCI is to help create quick iteration pipelines for testing potential human machine and brain computer interfaces, namely applied machine learning models and feature extraction techniques.
+The goal of PyBCI is to help create quick iteration pipelines for testing potential human machine and brain computer interfaces, namely testing applied machine learning models, data processing, and feature extraction techniques for LSL enabled devices and training stimuli.
 
 ## Installation
 For stable releases use: ```pip install install-pybci```
-(currently can only install-pybci due to pybci name similarities with another package on pypi)
 
 For unstable dev installations and up-to-date git pushes use: ```pip install --index-url https://test.pypi.org/simple/ install-pybci```
 
+(currently using install-pybci due to pybci having name too similar with another package on pypi)
 
-[ReadTheDocs available here!](https://pybci.readthedocs.io/en/latest/) (In development)
+[ReadTheDocs available here!](https://pybci.readthedocs.io/en/latest/)      [Examples found here!](https://github.com/LMBooth/pybci/tree/main/pybci/Examples)
 
 ## Basic implementation
 ```python
 import time
 from pybci import PyBCI
-bci = PyBCI()
-while not bci.connected:
+bci = PyBCI(minimumEpochsRequired = 4)
+while not bci.connected: # check to see if lsl marker and datastream are available
     bci.Connect()
     time.sleep(1)
-bci.TrainMode()
-while(True):
-    currentMarkers = bci.ReceivedMarkerCount()
-    time.sleep(1) # wait for marker updates
-    if len(currentMarkers) > 1:  # check there is more then one marker type received
-        if min([currentMarkers[key][1] for key in currentMarkers]) > 10:
-            bci.TestMode()
-            break 
+bci.TrainMode() # now both marker and datastreams available start training on received epochs
+accuracy = 0
 try:
-    while True:
-        classInfo = bci.CurrentClassifierInfo() # when in train mode only y_pred returned
-        guess = [key for key, value in currentMarkers.items() if value[0] == classInfo["y_pred"]]
+    while(True): # training based on couple epochs more then min threshold for classifying
+        currentMarkers = bci.ReceivedMarkerCount() # check to see how many received epochs, if markers sent to close together will be ignored till done processing
+        time.sleep(1) # wait for marker updates
+        print("Markers received: " + str(currentMarkers) +" Class accuracy: " + str(accuracy), end="\r")
+        if len(currentMarkers) > 1:  # check there is more then one marker type received
+            if min([currentMarkers[key][1] for key in currentMarkers]) > bci.minimumEpochsRequired:
+                classInfo = bci.CurrentClassifierInfo() # hangs if called too early
+                accuracy = classInfo["accuracy"]
+            if min([currentMarkers[key][1] for key in currentMarkers]) > bci.minimumEpochsRequired+1:  
+                bci.TestMode()
+                break
+    while True: # now sufficient epochs gathered start testing
+        markerGuess = bci.CurrentClassifierMarkerGuess() # when in test mode only y_pred returned
+        guess = [key for key, value in currentMarkers.items() if value[0] == markerGuess]
         print("Current marker estimation: " + str(guess), end="\r")
+        time.sleep(0.5)
 except KeyboardInterrupt: # allow user to break while loop
     pass
 ```
 
 ## Background Information
-PyBCI is a python based brain computer interface software designed to receive a varying number, be it singular or multiple, [Lab Streaming Layer](https://github.com/sccn/labstreaminglayer) enabled physiological sensor data streams. An understanding of time-series data analysis, the lab streaming layer protocol, and machine learning techniques are a must to integrate innovative ideas with this interface.
-An LSL marker stream is required to train the model, where a received marker [epochs](https://www.google.com/search?q=epochs+definition&rlz=1C1CHBF_en-GBGB921GB921&sxsrf=APwXEddAlMkYQ6MqziIvXbvsCxl3SjySNA%3A1684343462996&ei=pgplZJK2PJiigAaErrWwCw&oq=epochs+def&gs_lcp=Cgxnd3Mtd2l6LXNlcnAQAxgAMg0IABCKBRCRAhBGEPkBMgUIABCABDIFCAAQgAQyBQgAEIAEMggIABAWEB4QDzIICAAQFhAeEA8yBggAEBYQHjIGCAAQFhAeMgYIABAWEB4yCQgAEBYQHhDxBDoHCCMQsAMQJzoKCAAQRxDWBBCwAzoHCCMQigUQJzoHCAAQigUQQzoNCAAQigUQsQMQgwEQQzoICAAQigUQkQJKBAhBGABQmAZYwQhgzw5oAXABeACAAYYBiAHBA5IBAzEuM5gBAKABAcgBCsABAQ&sclient=gws-wiz-serp) the data received on the accepted datastreams based on a configurable time window around certain markers - where custom marker strings can optionally have its epoch timewindow split and overlapped to count for more then one marker, example: a baseline marker may have one marker sent for a 60 second window, where as target actions may only be ~0.5s long, so to conform when testing the model and giving a standardised window length would be desirable to split the 60s window after the received baseline marker in to ~0.5s windows. By overlapping windows we try to account for potential missed signal patterns/aliasing, as a rule of thumb it would be advised when testing a model to have an overlap >= than 50%, [see Shannon nyquist criterion](https://en.wikipedia.org/wiki/Nyquist%E2%80%93Shannon_sampling_theorem).
+PyBCI is a python based brain computer interface software designed to receive a varying number, be it singular or multiple, Lab Streaming Layer enabled physiological sensor data streams. An understanding of time-series data analysis, the lab streaming layer protocol, and machine learning techniques are a must to integrate innovative ideas with this interface. An LSL marker stream is required to train the model, where a received marker epochs the data received on the accepted datastreams based on a configurable time window around certain markers - where custom marker strings can optionally have its epoch timewindow split and overlapped to count for more then one marker, example: a baseline marker may have one marker sent for a 60 second window, where as target actions may only be ~0.5s long, so to conform when testing the model and giving a standardised window length would be desirable to split the 60s window after the received baseline marker in to ~0.5s windows. By overlapping windows we try to account for potential missed signal patterns/aliasing, as a rule of thumb it would be advised when testing a model to have an overlap >= than 50%, see Shannon nyquist criterion.
 
-Once the data has been epoched it is sent for feature extraction, there is a general feature extraction class which can be configured for general time and/or frequency analysis based features, data streams types like "EEG" and "EMG". (DevNOTE: looking to write class for basic pupil labs example to be passed, or solely samples + channels, or other custom classes passed to selected marker streams >:] )
+Once the data has been epoched it is sent for feature extraction, there is a general feature extraction class which can be configured for general time and/or frequency analysis based features, data streams types like "EEG" and "EMG", since data analysis, preprocessing and feature extraction between devices can vary greatly, this is why custom feature extraction classes can be created for each data stream maker type. 
 
 Finally a passable, customisable sklearn or tensorflow classifier can be giving to the bci class, once a defined number of epochs have been obtained for each received epoch/marker type the classifier can begin to fit the model. It's advised to use bci.ReceivedMarkerCount() to get the number of received training epochs received, once the min num epochs received of each type is >= pybci.minimumEpochsRequired (default 10 of each epoch) the mdoel will begin to fit. Once fit classifier info can be queried with CurrentClassifierInfo, when a desired accuracy is met or number of epochs TestMode() can be called. Once in test mode you can query (sould change function to own function and queue for quering testthread) what pybci estimates the current bci epoch is(typically bseline is used for no state).
 
-If you have no LSL available hardware, a psuedo time-series signal can be created with the script found in [mainSend.py PsuedoLSLStreamGenerator folder](https://github.com/LMBooth/pybci/tree/main/pybci/Examples/PsuedoLSLStreamGenerator/mainSend.py). 
+The [examples folder](https://github.com/LMBooth/pybci/tree/main/pybci/Examples) found on the github has a [pseudo LSL data generator and marker creator](https://github.com/LMBooth/pybci/tree/main/pybci/Examples/PsuedoLSLStreamGenerator) in the [mainSend.py](https://github.com/LMBooth/pybci/tree/main/pybci/Examples/PsuedoLSLStreamGenerator/mainSend.py) file so the examples can run without the need of LSL capable hardware. 
+
 
 
-## Theory of Operation
-1. Requirements Prior Initialising with ```python bci = PyBCI() ```
-    - The bci must have >=1 LSL datastream with an accepted dataType ("EEG", "EMG", "Gaze") {hopefully configurable in the future t pass custom fature decoding class}
-    - The bci must have ==1 LSL markerstream selected (if more then one LSL marker stream on system set the desired ML training marker stream with PyBCI(markerStream="yourMarkerStream")). Warning: If None set picks first available in list.
-2. Initialising BCI software
-    - [Optional Configurations](https://pybci.readthedocs.io/en/latest/api/PyBCI.html) for ```python PyBCI() ```
-    - Once configuration settings are set various threads are created.
-        - The marker stream has its own thread which recieves markers from the target LSL marker stream and when in train mode pushes this marker to the available datastreams. 
-        - Each data stream has its own thread created responsible for pipleining received data on FIFO's and slicing approprialey based on globalEpochSettings and customEpochSettings.
-        - FeaturesExtractor
-        - Classifier
-    
-3. ML Training:
-  
-4. ML Testing:
 
 ## ToDo!
-- 
-### Future Work
-- Add simple gaze decoding from pupil-labs
-- Create example to output classification on LSL and make test train configurable on pure LSL markers 
-- custom class passable for data decoding, use general and gaze for inpiration. 
+- Combine multiple data streams for multi modal bci!
 
-## Curently in Alpha, come back in a few days for updates!
+## Curently in Beta, come back in a few days for updates!
```

### Comparing `install-pybci-0.1.4b4/install_pybci.egg-info/SOURCES.txt` & `install-pybci-0.1.4b5/install_pybci.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `install-pybci-0.1.4b4/pybci/Configuration/EpochSettings.py` & `install-pybci-0.1.4b5/pybci/Configuration/EpochSettings.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.1.4b4/pybci/ThreadClasses/AsyncDataReceiverThread.py` & `install-pybci-0.1.4b5/pybci/ThreadClasses/AsyncDataReceiverThread.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.1.4b4/pybci/ThreadClasses/ClassifierThread.py` & `install-pybci-0.1.4b5/pybci/ThreadClasses/ClassifierThread.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.1.4b4/pybci/ThreadClasses/DataReceiverThread.py` & `install-pybci-0.1.4b5/pybci/ThreadClasses/DataReceiverThread.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.1.4b4/pybci/ThreadClasses/FeatureProcessorThread.py` & `install-pybci-0.1.4b5/pybci/ThreadClasses/FeatureProcessorThread.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.1.4b4/pybci/ThreadClasses/MarkerThread.py` & `install-pybci-0.1.4b5/pybci/ThreadClasses/MarkerThread.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.1.4b4/pybci/Utils/Classifier.py` & `install-pybci-0.1.4b5/pybci/Utils/Classifier.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.1.4b4/pybci/Utils/FeatureExtractor.py` & `install-pybci-0.1.4b5/pybci/Utils/FeatureExtractor.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.1.4b4/pybci/Utils/LSLScanner.py` & `install-pybci-0.1.4b5/pybci/Utils/LSLScanner.py`

 * *Files identical despite different names*

### Comparing `install-pybci-0.1.4b4/pybci/pybci.py` & `install-pybci-0.1.4b5/pybci/pybci.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,26 +6,14 @@
 from .ThreadClasses.ClassifierThread import ClassifierThread
 from .Configuration.EpochSettings import GlobalEpochSettings, IndividualEpochSetting
 from .Configuration.FeatureSettings import GeneralFeatureChoices
 import queue, threading, copy
 import tensorflow as tf
 
 class PyBCI:
-    """The PyBCI object stores data from available lsl time series data streams (EEG, pupilometry, EMG, etc.)
-     and holds a configurable number of samples based on lsl marker strings.
-     If no marker strings are available on the LSL the class will close and return an error.
-     Optional Inputs:
-        dataStreams = List of strings, allows user to set custom acceptable EEG stream definitions, if None defaults to streamTypes scan
-        markerStream = List of strings, allows user to set custom acceptable Marker stream definitions, if None defaults to markerTypes scan
-        streamTypes = List of strings, allows user to set custom acceptable EEG type definitions, ignored if dataStreams not None
-        markerTypes = List of strings, allows user to set custom acceptable Marker type definitions, ignored if markerStream not None
-        printDebug = boolean, if true prints LSLScanner debug information
-    TODO:
-        Need to add option to pass theoretical maximum sample rate to AsyncDatastreams to acount for theoretical max window limits
-    """
     printDebug = True   # boolean, used to toggle print statements from LSLScanner class
     globalEpochSettings = GlobalEpochSettings()
     customEpochSettings = {}
     minimumEpochsRequired = 10
     markerThread = []
     dataThreads = []
     streamChsDropDict= {}
@@ -35,14 +23,32 @@
     epochCounts = {} # holds markers received, their target ids and number received of each
     classifierInformation = []
 
     def __init__(self, dataStreams = None, markerStream= None, streamTypes = None, markerTypes = None, printDebug = True,
                  globalEpochSettings = GlobalEpochSettings(), customEpochSettings = {}, streamChsDropDict = {},
                  streamCustomFeatureExtract = {},
                  minimumEpochsRequired = 10, clf= None, model = None):
+        """
+        The PyBCI object stores data from available lsl time series data streams (EEG, pupilometry, EMG, etc.)
+        and holds a configurable number of samples based on lsl marker strings.
+        If no marker strings are available on the LSL the class will close and return an error.
+        Parameters:
+        dataStreams (List of strings): Allows user to set custom acceptable EEG stream definitions, if None defaults to streamTypes scan
+        markerStream (List of strings): Allows user to set custom acceptable Marker stream definitions, if None defaults to markerTypes scan
+        streamTypes (List of strings): Allows user to set custom acceptable EEG type definitions, ignored if dataStreams not None
+        markerTypes (List of strings): Allows user to set custom acceptable Marker type definitions, ignored if markerStream not None
+        printDebug (bool): If true prints LSLScanner debug information
+        globalEpochSettings (GlobalEpochSettings): Sets global timing settings for epochs.
+        customEpochSettings (dict {marker name string:IndividualEpochSettings()}): Sets individual timing settings for epochs.
+        streamChsDropDict (dict {datastream name string: list(ints)}): Keys for dict should be respective datastreams with corresponding list of which channels to drop.
+        streamCustomFeatureExtract (dict {datastream type string: customClass()}): allows dict to be passed of datastream type with custom feature extractor class for analysing data.
+        minimumEpochsRequired (Int): minimm number of required epochs before model fitting begins, must be of each type of received markers and mroe then 1 type of marker to classify.
+        clf (ClassifierMixin): Allows custom Sklearn model to be passed.
+        model (model):Allows custom tensorflow model to be passed.
+        """
         self.streamCustomFeatureExtract = streamCustomFeatureExtract
         self.globalEpochSettings = globalEpochSettings
         self.customEpochSettings = customEpochSettings
         self.streamChsDropDict = streamChsDropDict
         self.lslScanner = LSLScanner(self, dataStreams, markerStream,streamTypes, markerTypes)
         self.printDebug = printDebug
         self.ConfigureMachineLearning(minimumEpochsRequired,  clf, model) # configure first, connect second
```

### Comparing `install-pybci-0.1.4b4/setup.py` & `install-pybci-0.1.4b5/setup.py`

 * *Files identical despite different names*

