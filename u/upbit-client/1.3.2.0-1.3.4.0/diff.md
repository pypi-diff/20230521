# Comparing `tmp/upbit-client-1.3.2.0.tar.gz` & `tmp/upbit-client-1.3.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "upbit-client-1.3.2.0.tar", last modified: Tue Jul 12 11:32:02 2022, max compression
+gzip compressed data, was "upbit-client-1.3.4.0.tar", last modified: Sun May 21 15:33:12 2023, max compression
```

## Comparing `upbit-client-1.3.2.0.tar` & `upbit-client-1.3.4.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-12 11:32:02.908125 upbit-client-1.3.2.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1089 2022-07-12 11:31:51.000000 upbit-client-1.3.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     3592 2022-07-12 11:32:02.908125 upbit-client-1.3.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2909 2022-07-12 11:31:51.000000 upbit-client-1.3.2.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (121)      106 2022-07-12 11:32:02.908125 upbit-client-1.3.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1485 2022-07-12 11:31:51.000000 upbit-client-1.3.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-12 11:32:02.904125 upbit-client-1.3.2.0/upbit/
--rw-r--r--   0 runner    (1001) docker     (121)      459 2022-07-12 11:31:51.000000 upbit-client-1.3.2.0/upbit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2881 2022-07-12 11:31:51.000000 upbit-client-1.3.2.0/upbit/authentication.py
--rw-r--r--   0 runner    (1001) docker     (121)     1920 2022-07-12 11:31:51.000000 upbit-client-1.3.2.0/upbit/client.py
--rw-r--r--   0 runner    (1001) docker     (121)    22382 2022-07-12 11:31:51.000000 upbit-client-1.3.2.0/upbit/models.py
--rw-r--r--   0 runner    (1001) docker     (121)     1171 2022-07-12 11:31:51.000000 upbit-client-1.3.2.0/upbit/pkginfo.py
--rw-r--r--   0 runner    (1001) docker     (121)     2583 2022-07-12 11:31:51.000000 upbit-client-1.3.2.0/upbit/utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     5053 2022-07-12 11:31:51.000000 upbit-client-1.3.2.0/upbit/websocket.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-12 11:32:02.908125 upbit-client-1.3.2.0/upbit_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3592 2022-07-12 11:32:02.000000 upbit-client-1.3.2.0/upbit_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      341 2022-07-12 11:32:02.000000 upbit-client-1.3.2.0/upbit_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-12 11:32:02.000000 upbit-client-1.3.2.0/upbit_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       66 2022-07-12 11:32:02.000000 upbit-client-1.3.2.0/upbit_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-07-12 11:32:02.000000 upbit-client-1.3.2.0/upbit_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 15:33:12.183725 upbit-client-1.3.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-21 15:33:00.000000 upbit-client-1.3.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-05-21 15:33:12.183725 upbit-client-1.3.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-05-21 15:33:00.000000 upbit-client-1.3.4.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-21 15:33:12.183725 upbit-client-1.3.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-21 15:33:00.000000 upbit-client-1.3.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 15:33:12.179725 upbit-client-1.3.4.0/upbit/
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-21 15:33:00.000000 upbit-client-1.3.4.0/upbit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-05-21 15:33:00.000000 upbit-client-1.3.4.0/upbit/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-21 15:33:00.000000 upbit-client-1.3.4.0/upbit/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24115 2023-05-21 15:33:00.000000 upbit-client-1.3.4.0/upbit/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-21 15:33:00.000000 upbit-client-1.3.4.0/upbit/pkginfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-05-21 15:33:00.000000 upbit-client-1.3.4.0/upbit/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5053 2023-05-21 15:33:00.000000 upbit-client-1.3.4.0/upbit/websocket.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 15:33:12.183725 upbit-client-1.3.4.0/upbit_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3674 2023-05-21 15:33:12.000000 upbit-client-1.3.4.0/upbit_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      341 2023-05-21 15:33:12.000000 upbit-client-1.3.4.0/upbit_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 15:33:12.000000 upbit-client-1.3.4.0/upbit_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-21 15:33:12.000000 upbit-client-1.3.4.0/upbit_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-21 15:33:12.000000 upbit-client-1.3.4.0/upbit_client.egg-info/top_level.txt
```

### Comparing `upbit-client-1.3.2.0/LICENSE` & `upbit-client-1.3.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `upbit-client-1.3.2.0/PKG-INFO` & `upbit-client-1.3.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: upbit-client
-Version: 1.3.2.0
+Version: 1.3.4.0
 Summary: Upbit OPEN API Client
 Home-page: https://github.com/uJhin/upbit-client
+Download-URL: https://github.com/uJhin/upbit-client/releases
 Author: ujhin
 Author-email: ujhin942@gmail.com
 License: MIT License
-Download-URL: https://github.com/uJhin/upbit-client/releases
 Keywords: Upbit,upbit,upbit-client,Upbit-Client,Upbit_client,Upbit-api-connector,upbit-api-connector,Upbit_api_connector,upbit_api_connector
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: fido
 License-File: LICENSE
 
 .. image:: https://raw.githubusercontent.com/uJhin/upbit-client/main/logo/logo.png
     :align: center
@@ -151,9 +152,7 @@
 
 Donation
 *********
 .. image:: https://img.shields.io/badge/BTC-3NVw2seiTQddGQwc1apqudKxuTqebpyL3s-blue?style=flat-square&logo=bitcoin
   :alt: uJhin's BTC
 .. image:: https://img.shields.io/badge/ETH-0x60dd373f59862d9df776596889b997e24bee42eb-blue?style=flat-square&logo=ethereum
   :alt: uJhin's ETH
-
-
```

### Comparing `upbit-client-1.3.2.0/README.rst` & `upbit-client-1.3.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `upbit-client-1.3.2.0/setup.py` & `upbit-client-1.3.4.0/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,80 +14,88 @@
 000000d0: 6e66 6f2e 5041 434b 4147 455f 4e41 4d45  nfo.PACKAGE_NAME
 000000e0: 2c0d 0a20 2020 2076 6572 7369 6f6e 2020  ,..    version  
 000000f0: 3d20 706b 6769 6e66 6f2e 4355 5252 454e  = pkginfo.CURREN
 00000100: 545f 5645 5253 494f 4e2c 0d0a 2020 2020  T_VERSION,..    
 00000110: 7061 636b 6167 6573 203d 2066 696e 645f  packages = find_
 00000120: 7061 636b 6167 6573 2829 2c0d 0a20 2020  packages(),..   
 00000130: 2069 6e73 7461 6c6c 5f72 6571 7569 7265   install_require
-00000140: 7320 3d20 5b0d 0a20 2020 2020 2020 2027  s = [..        '
-00000150: 6272 6176 6164 6f3e 3d31 312e 302e 3227  bravado>=11.0.2'
-00000160: 2c0d 0a20 2020 2020 2020 2027 5079 4a57  ,..        'PyJW
-00000170: 543e 3d32 2e34 2e30 272c 0d0a 2020 2020  T>=2.4.0',..    
-00000180: 2020 2020 2777 6562 736f 636b 6574 733e      'websockets>
-00000190: 3d31 302e 3327 0d0a 2020 2020 5d2c 0d0a  =10.3'..    ],..
-000001a0: 2020 2020 6578 7472 6173 5f72 6571 7569      extras_requi
-000001b0: 7265 2020 3d20 7b0d 0a20 2020 2020 2020  re  = {..       
-000001c0: 2027 6669 646f 273a 205b 0d0a 2020 2020   'fido': [..    
-000001d0: 2020 2020 2020 2020 2766 6964 6f3e 3d34          'fido>=4
-000001e0: 2e32 2e31 270d 0a20 2020 2020 2020 205d  .2.1'..        ]
-000001f0: 0d0a 2020 2020 7d2c 0d0a 2020 2020 7079  ..    },..    py
-00000200: 7468 6f6e 5f72 6571 7569 7265 7320 3d20  thon_requires = 
-00000210: 273e 3d33 2e38 272c 0d0a 2020 2020 636c  '>=3.8',..    cl
-00000220: 6173 7369 6669 6572 7320 2020 2020 3d20  assifiers     = 
-00000230: 5b0d 0a20 2020 2020 2020 2027 5072 6f67  [..        'Prog
-00000240: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
-00000250: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
-00000260: 3827 2c0d 0a20 2020 2020 2020 2027 5072  8',..        'Pr
-00000270: 6f67 7261 6d6d 696e 6720 4c61 6e67 7561  ogramming Langua
-00000280: 6765 203a 3a20 5079 7468 6f6e 203a 3a20  ge :: Python :: 
-00000290: 332e 3927 2c0d 0a20 2020 2020 2020 2027  3.9',..        '
-000002a0: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
-000002b0: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
-000002c0: 3a20 332e 3130 272c 0d0a 2020 2020 5d2c  : 3.10',..    ],
-000002d0: 0d0a 2020 2020 6b65 7977 6f72 6473 2020  ..    keywords  
-000002e0: 2020 2020 2020 3d20 5b0d 0a20 2020 2020        = [..     
-000002f0: 2020 2027 5570 6269 7427 2c0d 0a20 2020     'Upbit',..   
-00000300: 2020 2020 2027 7570 6269 7427 2c0d 0a20       'upbit',.. 
-00000310: 2020 2020 2020 2027 7570 6269 742d 636c         'upbit-cl
-00000320: 6965 6e74 272c 0d0a 2020 2020 2020 2020  ient',..        
-00000330: 2755 7062 6974 2d43 6c69 656e 7427 2c0d  'Upbit-Client',.
-00000340: 0a20 2020 2020 2020 2027 5570 6269 745f  .        'Upbit_
-00000350: 636c 6965 6e74 272c 0d0a 2020 2020 2020  client',..      
-00000360: 2020 2755 7062 6974 2d61 7069 2d63 6f6e    'Upbit-api-con
-00000370: 6e65 6374 6f72 272c 0d0a 2020 2020 2020  nector',..      
-00000380: 2020 2775 7062 6974 2d61 7069 2d63 6f6e    'upbit-api-con
-00000390: 6e65 6374 6f72 272c 0d0a 2020 2020 2020  nector',..      
-000003a0: 2020 2755 7062 6974 5f61 7069 5f63 6f6e    'Upbit_api_con
-000003b0: 6e65 6374 6f72 272c 0d0a 2020 2020 2020  nector',..      
-000003c0: 2020 2775 7062 6974 5f61 7069 5f63 6f6e    'upbit_api_con
-000003d0: 6e65 6374 6f72 270d 0a20 2020 205d 2c0d  nector'..    ],.
-000003e0: 0a20 2020 2075 726c 2020 2020 2020 2020  .    url        
-000003f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000400: 2020 203d 2027 6874 7470 733a 2f2f 6769     = 'https://gi
-00000410: 7468 7562 2e63 6f6d 2f75 4a68 696e 2f75  thub.com/uJhin/u
-00000420: 7062 6974 2d63 6c69 656e 7427 2c0d 0a20  pbit-client',.. 
-00000430: 2020 2064 6f77 6e6c 6f61 645f 7572 6c20     download_url 
-00000440: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000450: 203d 2027 6874 7470 733a 2f2f 6769 7468   = 'https://gith
-00000460: 7562 2e63 6f6d 2f75 4a68 696e 2f75 7062  ub.com/uJhin/upb
-00000470: 6974 2d63 6c69 656e 742f 7265 6c65 6173  it-client/releas
-00000480: 6573 272c 0d0a 2020 2020 6c69 6365 6e73  es',..    licens
-00000490: 6520 2020 2020 2020 2020 2020 2020 2020  e               
-000004a0: 2020 2020 2020 2020 3d20 274d 4954 204c          = 'MIT L
-000004b0: 6963 656e 7365 272c 0d0a 2020 2020 6175  icense',..    au
-000004c0: 7468 6f72 2020 2020 2020 2020 2020 2020  thor            
-000004d0: 2020 2020 2020 2020 2020 2020 3d20 2775              = 'u
-000004e0: 6a68 696e 272c 0d0a 2020 2020 6175 7468  jhin',..    auth
-000004f0: 6f72 5f65 6d61 696c 2020 2020 2020 2020  or_email        
-00000500: 2020 2020 2020 2020 2020 3d20 2775 6a68            = 'ujh
-00000510: 696e 3934 3240 676d 6169 6c2e 636f 6d27  in942@gmail.com'
-00000520: 2c0d 0a20 2020 2064 6573 6372 6970 7469  ,..    descripti
-00000530: 6f6e 2020 2020 2020 2020 2020 2020 2020  on              
-00000540: 2020 2020 203d 2027 5570 6269 7420 4f50       = 'Upbit OP
-00000550: 454e 2041 5049 2043 6c69 656e 7427 2c0d  EN API Client',.
-00000560: 0a20 2020 206c 6f6e 675f 6465 7363 7269  .    long_descri
-00000570: 7074 696f 6e5f 636f 6e74 656e 745f 7479  ption_content_ty
-00000580: 7065 203d 2027 7465 7874 2f78 2d72 7374  pe = 'text/x-rst
-00000590: 272c 0d0a 2020 2020 6c6f 6e67 5f64 6573  ',..    long_des
-000005a0: 6372 6970 7469 6f6e 2020 2020 2020 2020  cription        
-000005b0: 2020 2020 2020 3d20 6c6f 6e67 5f64 6573        = long_des
-000005c0: 6372 6970 7469 6f6e 0d0a 290d 0a         cription..)..
+00000140: 7320 3d20 5b0d 0a20 2020 2020 2020 2020  s = [..         
+00000150: 2027 6272 6176 6164 6f3e 3d31 312e 302e   'bravado>=11.0.
+00000160: 3227 0d0a 2020 2020 2020 2020 2c20 2750  2'..        , 'P
+00000170: 794a 5754 3e3d 322e 342e 3027 0d0a 2020  yJWT>=2.4.0'..  
+00000180: 2020 2020 2020 2c20 2777 6562 736f 636b        , 'websock
+00000190: 6574 733e 3d31 302e 3327 0d0a 2020 2020  ets>=10.3'..    
+000001a0: 5d2c 0d0a 2020 2020 6578 7472 6173 5f72  ],..    extras_r
+000001b0: 6571 7569 7265 2020 3d20 7b0d 0a20 2020  equire  = {..   
+000001c0: 2020 2020 2027 6669 646f 273a 205b 0d0a       'fido': [..
+000001d0: 2020 2020 2020 2020 2020 2020 2766 6964              'fid
+000001e0: 6f3e 3d34 2e32 2e31 270d 0a20 2020 2020  o>=4.2.1'..     
+000001f0: 2020 205d 0d0a 2020 2020 7d2c 0d0a 2020     ]..    },..  
+00000200: 2020 7079 7468 6f6e 5f72 6571 7569 7265    python_require
+00000210: 7320 3d20 273e 3d33 2e38 272c 0d0a 2020  s = '>=3.8',..  
+00000220: 2020 636c 6173 7369 6669 6572 7320 2020    classifiers   
+00000230: 2020 3d20 5b0d 0a20 2020 2020 2020 2020    = [..         
+00000240: 2027 5072 6f67 7261 6d6d 696e 6720 4c61   'Programming La
+00000250: 6e67 7561 6765 203a 3a20 5079 7468 6f6e  nguage :: Python
+00000260: 203a 3a20 332e 3827 0d0a 2020 2020 2020   :: 3.8'..      
+00000270: 2020 2c20 2750 726f 6772 616d 6d69 6e67    , 'Programming
+00000280: 204c 616e 6775 6167 6520 3a3a 2050 7974   Language :: Pyt
+00000290: 686f 6e20 3a3a 2033 2e39 270d 0a20 2020  hon :: 3.9'..   
+000002a0: 2020 2020 202c 2027 5072 6f67 7261 6d6d       , 'Programm
+000002b0: 696e 6720 4c61 6e67 7561 6765 203a 3a20  ing Language :: 
+000002c0: 5079 7468 6f6e 203a 3a20 332e 3130 270d  Python :: 3.10'.
+000002d0: 0a20 2020 2020 2020 202c 2027 5072 6f67  .        , 'Prog
+000002e0: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
+000002f0: 203a 3a20 5079 7468 6f6e 203a 3a20 332e   :: Python :: 3.
+00000300: 3131 270d 0a20 2020 2020 2020 202c 2027  11'..        , '
+00000310: 5072 6f67 7261 6d6d 696e 6720 4c61 6e67  Programming Lang
+00000320: 7561 6765 203a 3a20 5079 7468 6f6e 203a  uage :: Python :
+00000330: 3a20 332e 3132 270d 0a20 2020 205d 2c0d  : 3.12'..    ],.
+00000340: 0a20 2020 206b 6579 776f 7264 7320 2020  .    keywords   
+00000350: 2020 2020 203d 205b 0d0a 2020 2020 2020       = [..      
+00000360: 2020 2020 2755 7062 6974 270d 0a20 2020      'Upbit'..   
+00000370: 2020 2020 202c 2027 7570 6269 7427 0d0a       , 'upbit'..
+00000380: 2020 2020 2020 2020 2c20 2775 7062 6974          , 'upbit
+00000390: 2d63 6c69 656e 7427 0d0a 2020 2020 2020  -client'..      
+000003a0: 2020 2c20 2755 7062 6974 2d43 6c69 656e    , 'Upbit-Clien
+000003b0: 7427 0d0a 2020 2020 2020 2020 2c20 2755  t'..        , 'U
+000003c0: 7062 6974 5f63 6c69 656e 7427 0d0a 2020  pbit_client'..  
+000003d0: 2020 2020 2020 2c20 2755 7062 6974 2d61        , 'Upbit-a
+000003e0: 7069 2d63 6f6e 6e65 6374 6f72 270d 0a20  pi-connector'.. 
+000003f0: 2020 2020 2020 202c 2027 7570 6269 742d         , 'upbit-
+00000400: 6170 692d 636f 6e6e 6563 746f 7227 0d0a  api-connector'..
+00000410: 2020 2020 2020 2020 2c20 2755 7062 6974          , 'Upbit
+00000420: 5f61 7069 5f63 6f6e 6e65 6374 6f72 270d  _api_connector'.
+00000430: 0a20 2020 2020 2020 202c 2027 7570 6269  .        , 'upbi
+00000440: 745f 6170 695f 636f 6e6e 6563 746f 7227  t_api_connector'
+00000450: 0d0a 2020 2020 5d2c 0d0a 2020 2020 7572  ..    ],..    ur
+00000460: 6c20 2020 2020 2020 2020 2020 2020 2020  l               
+00000470: 2020 2020 2020 2020 2020 2020 3d20 2768              = 'h
+00000480: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000490: 6d2f 754a 6869 6e2f 7570 6269 742d 636c  m/uJhin/upbit-cl
+000004a0: 6965 6e74 272c 0d0a 2020 2020 646f 776e  ient',..    down
+000004b0: 6c6f 6164 5f75 726c 2020 2020 2020 2020  load_url        
+000004c0: 2020 2020 2020 2020 2020 3d20 2768 7474            = 'htt
+000004d0: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+000004e0: 754a 6869 6e2f 7570 6269 742d 636c 6965  uJhin/upbit-clie
+000004f0: 6e74 2f72 656c 6561 7365 7327 2c0d 0a20  nt/releases',.. 
+00000500: 2020 206c 6963 656e 7365 2020 2020 2020     license      
+00000510: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000520: 203d 2027 4d49 5420 4c69 6365 6e73 6527   = 'MIT License'
+00000530: 2c0d 0a20 2020 2061 7574 686f 7220 2020  ,..    author   
+00000540: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000550: 2020 2020 203d 2027 756a 6869 6e27 2c0d       = 'ujhin',.
+00000560: 0a20 2020 2061 7574 686f 725f 656d 6169  .    author_emai
+00000570: 6c20 2020 2020 2020 2020 2020 2020 2020  l               
+00000580: 2020 203d 2027 756a 6869 6e39 3432 4067     = 'ujhin942@g
+00000590: 6d61 696c 2e63 6f6d 272c 0d0a 2020 2020  mail.com',..    
+000005a0: 6465 7363 7269 7074 696f 6e20 2020 2020  description     
+000005b0: 2020 2020 2020 2020 2020 2020 2020 3d20                = 
+000005c0: 2755 7062 6974 204f 5045 4e20 4150 4920  'Upbit OPEN API 
+000005d0: 436c 6965 6e74 272c 0d0a 2020 2020 6c6f  Client',..    lo
+000005e0: 6e67 5f64 6573 6372 6970 7469 6f6e 5f63  ng_description_c
+000005f0: 6f6e 7465 6e74 5f74 7970 6520 3d20 2774  ontent_type = 't
+00000600: 6578 742f 782d 7273 7427 2c0d 0a20 2020  ext/x-rst',..   
+00000610: 206c 6f6e 675f 6465 7363 7269 7074 696f   long_descriptio
+00000620: 6e20 2020 2020 2020 2020 2020 2020 203d  n              =
+00000630: 206c 6f6e 675f 6465 7363 7269 7074 696f   long_descriptio
+00000640: 6e0d 0a29 0d0a                           n..)..
```

### Comparing `upbit-client-1.3.2.0/upbit/authentication.py` & `upbit-client-1.3.4.0/upbit/authentication.py`

 * *Files identical despite different names*

### Comparing `upbit-client-1.3.2.0/upbit/client.py` & `upbit-client-1.3.4.0/upbit/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
     """
     Upbit Client
     Please read the official Upbit Client document.
     Documents: https://ujhin.github.io/upbit-client-docs/
 
     - Base URL: https://api.upbit.com
     - Base Path: /v1
-    - Upbit OPEN API Version: 1.3.2
+    - Upbit OPEN API Version: 1.3.4
     - Author: ujhin
     - Email: ujhin942@gmail.com
     - GitHub: https://github.com/uJhin
     - Official OPEN API Documents: https://docs.upbit.com
     - Official Support Email: open-api@upbit.com
     """
```

### Comparing `upbit-client-1.3.2.0/upbit/models.py` & `upbit-client-1.3.4.0/upbit/models.py`

 * *Files 10% similar despite different names*

```diff
@@ -227,31 +227,36 @@
         """
         [GET] 개별 입금 주소 조회
 
         ## 개별 입금 주소 조회
 
         [NOTE] 입금 주소 조회 요청 API 유의사항
 
-        입금 주소 생성 요청 이후 아직 발급되지 않은 상태일 경우 deposit_address가 null일 수 있습니다.
+        입금 주소 생성 요청 이후 아직 발급되지 않은 상태일 경우 `deposit_address` 가 `null` 일 수 있습니다.
+        * 네트워크가 일치하지 않는 경우 정상 입출금이 진행되지 않을 수 있습니다.
+        사용하는 주소와 네트워크가 정확히 일치하는지 재확인 후 이용을 부탁드립니다.
 
-        :param currency: Currency symbol
+        :param currency: Currency 코드
         :type currency: str
+
+        :param net_type: 입금 네트워크
+        :type net_type: str
         """
 
         future = self.__client.Deposit.Deposit_coin_address(**kwargs)
         return HTTPFutureExtractor.future_extraction(future)
 
     def Deposit_coin_addresses(self) -> dict:
         """
         [GET] 전체 입금 주소 조회
 
         ## 내가 보유한 자산 리스트를 보여줍니다.
         [NOTE] 입금 주소 조회 요청 API 유의사항
 
-        입금 주소 생성 요청 이후 아직 발급되지 않은 상태일 경우 deposit_address가 null일 수 있습니다.
+        입금 주소 생성 요청 이후 아직 발급되지 않은 상태일 경우 `deposit_address` 가 `null` 일 수 있습니다.
         """
 
         future = self.__client.Deposit.Deposit_coin_addresses()
         return HTTPFutureExtractor.future_extraction(future)
 
     def Deposit_generate_coin_address(self, **kwargs) -> dict:
         """
@@ -259,21 +264,23 @@
 
         입금 주소 생성을 요청한다.
 
         [NOTE] 입금 주소 생성 요청 API 유의사항
         
         입금 주소의 생성은 서버에서 비동기적으로 이뤄집니다.
         비동기적 생성 특성상 요청과 동시에 입금 주소가 발급되지 않을 수 있습니다.
-        주소 발급 요청 시 결과로 Response1이 반환되며 주소 발급 완료 이전까지 계속 Response1이 반환됩니다.
-        주소가 발급된 이후부터는 새로운 주소가 발급되는 것이 아닌 이전에 발급된 주소가 Response2 형태로 반환됩니다.
+        주소 발급 요청 시 결과로 `Response1` 이 반환되며 주소 발급 완료 이전까지 계속 `Response1` 이 반환됩니다.
+        주소가 발급된 이후부터는 새로운 주소가 발급되는 것이 아닌 이전에 발급된 주소가 `Response2` 형태로 반환됩니다.
         정상적으로 주소가 생성되지 않는다면 일정 시간 이후 해당 API를 다시 호출해주시길 부탁드립니다.
 
-
         :param currency: Currency 코드
         :type currency: str
+
+        :param net_type: 입금 네트워크
+        :type net_type: str
         """
 
         future = self.__client.Deposit.Deposit_generate_coin_address(**kwargs)
         return HTTPFutureExtractor.future_extraction(future)
 
     def Deposit_info(self, **kwargs) -> dict:
         """
@@ -588,16 +595,19 @@
 
     def Withdraw_chance(self, **kwargs) -> dict:
         """
         [GET] 출금 가능 정보
 
         ## 해당 통화의 가능한 출금 정보를 확인한다.
 
-        :param currency: Currency Symbol
+        :param currency: 자산 코드
         :type currency: str
+
+        :param net_type: 출금 네트워크
+        :type net_type: str
         """
 
         future = self.__client.Withdraw.Withdraw_chance(**kwargs)
         return HTTPFutureExtractor.future_extraction(future)
 
     def Withdraw_coin(self, **kwargs) -> dict:
         """
@@ -605,18 +615,23 @@
 
         ## 코인 출금을 요청한다.
 
         [NOTE] 바로출금 이용 시 유의사항
 
         업비트 회원의 주소가 아닌 주소로 바로출금을 요청하는 경우, 출금이 정상적으로 수행되지 않습니다.
         반드시 주소를 확인 후 출금을 진행하시기 바랍니다.
+        * 네트워크가 일치하지 않는 경우 정상 입출금이 진행되지 않을 수 있습니다.
+        사용하는 주소와 네트워크가 정확히 일치하는지 재확인 후 이용을 부탁드립니다.
 
-        :param currency: Currency 코드
+        :param currency: 자산 코드
         :type currency: str
 
+        :param net_type: 출금 네트워크
+        :type net_type: str
+
         :param amount: 출금 수량
         :type amount: str
 
         :param address: 출금 가능 주소에 등록된 출금 주소
         :type address: str
 
         :param secondary_address: 2차 출금 주소 (필요한 코인에 한해서) (optional)
@@ -699,7 +714,27 @@
 
         :param amount: 출금 원화 수량
         :type amount: str
         """
 
         future = self.__client.Withdraw.Withdraw_krw(**kwargs)
         return HTTPFutureExtractor.future_extraction(future)
+
+    def Withdraw_coin_addresses(self, **kwargs) -> dict:
+        """
+        [GET] 출금 허용 주소 리스트 조회
+
+        ## 등록된 출금 허용 주소 목록을 조회한다.
+
+        [NOTE] 출금 기능을 이용하기 위해서는 주소 등록이 필요합니다.
+
+        Open API를 통해 디지털 자산을 출금하기 위해서는 출금 허용 주소 등록이 필요합니다.
+        * 네트워크가 일치하지 않는 경우 정상 입출금이 진행되지 않을 수 있습니다.
+        사용하는 주소와 네트워크가 정확히 일치하는지 재확인 후 이용을 부탁드립니다.
+
+        ### 출금 허용 주소 등록 방법
+        업비트 웹 > [MY] > [Open API 관리] > [디지털 자산 출금주소 관리] 페이지에서 진행하실 수 있습니다.
+        """
+
+        future = self.__client.Withdraw.Withdraw_coin_addresses(**kwargs)
+        return HTTPFutureExtractor.future_extraction(future)
+
```

### Comparing `upbit-client-1.3.2.0/upbit/pkginfo.py` & `upbit-client-1.3.4.0/upbit/pkginfo.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 [Upbit Client]
 
 Please read the official Upbit Client document.
 Documents: https://ujhin.github.io/upbit-client-docs/
 
-- Upbit OPEN API Version: 1.3.2
+- Upbit OPEN API Version: 1.3.4
 - Author: ujhin
 - Email: ujhin942@gmail.com
 - GitHub: https://github.com/uJhin
 - Official OPEN API Documents: https://docs.upbit.com
 - Official Support Email: open-api@upbit.com
 """
 
@@ -24,15 +24,15 @@
     data = resp.json()
     versions = data["releases"].keys()
     return sorted(versions, key=LooseVersion, reverse=True)
 
 
 PACKAGE_NAME     = "upbit-client"
 
-OPEN_API_VERSION = "1.3.2"
+OPEN_API_VERSION = "1.3.4"
 CURRENT_VERSION  = OPEN_API_VERSION+".0"
 
 RELEASED_VERSION = _get_versions(PACKAGE_NAME)
 LATEST_VERSION   = RELEASED_VERSION[0]
 
 
 if LATEST_VERSION != CURRENT_VERSION:
```

### Comparing `upbit-client-1.3.2.0/upbit/utils.py` & `upbit-client-1.3.4.0/upbit/utils.py`

 * *Files identical despite different names*

### Comparing `upbit-client-1.3.2.0/upbit/websocket.py` & `upbit-client-1.3.4.0/upbit/websocket.py`

 * *Files identical despite different names*

### Comparing `upbit-client-1.3.2.0/upbit_client.egg-info/PKG-INFO` & `upbit-client-1.3.4.0/upbit_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: upbit-client
-Version: 1.3.2.0
+Version: 1.3.4.0
 Summary: Upbit OPEN API Client
 Home-page: https://github.com/uJhin/upbit-client
+Download-URL: https://github.com/uJhin/upbit-client/releases
 Author: ujhin
 Author-email: ujhin942@gmail.com
 License: MIT License
-Download-URL: https://github.com/uJhin/upbit-client/releases
 Keywords: Upbit,upbit,upbit-client,Upbit-Client,Upbit_client,Upbit-api-connector,upbit-api-connector,Upbit_api_connector,upbit_api_connector
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: fido
 License-File: LICENSE
 
 .. image:: https://raw.githubusercontent.com/uJhin/upbit-client/main/logo/logo.png
     :align: center
@@ -151,9 +152,7 @@
 
 Donation
 *********
 .. image:: https://img.shields.io/badge/BTC-3NVw2seiTQddGQwc1apqudKxuTqebpyL3s-blue?style=flat-square&logo=bitcoin
   :alt: uJhin's BTC
 .. image:: https://img.shields.io/badge/ETH-0x60dd373f59862d9df776596889b997e24bee42eb-blue?style=flat-square&logo=ethereum
   :alt: uJhin's ETH
-
-
```

