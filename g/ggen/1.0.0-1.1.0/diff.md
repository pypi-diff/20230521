# Comparing `tmp/ggen-1.0.0.tar.gz` & `tmp/ggen-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ggen-1.0.0.tar", last modified: Fri May 19 19:20:48 2023, max compression
+gzip compressed data, was "ggen-1.1.0.tar", last modified: Sun May 21 03:35:08 2023, max compression
```

## Comparing `ggen-1.0.0.tar` & `ggen-1.1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 hass877  (297237) users      (100)        0 2023-05-19 19:20:48.613736 ggen-1.0.0/
--rw-r--r--   0 hass877  (297237) users      (100)     1070 2023-05-19 19:00:10.000000 ggen-1.0.0/LICENSE
--rw-r--r--   0 hass877  (297237) users      (100)    15073 2023-05-19 19:20:48.610214 ggen-1.0.0/PKG-INFO
--rw-r--r--   0 hass877  (297237) users      (100)    14619 2023-05-19 19:00:10.000000 ggen-1.0.0/README.md
-drwxr-xr-x   0 hass877  (297237) users      (100)        0 2023-05-19 19:20:48.515737 ggen-1.0.0/ggen/
--rw-r--r--   0 hass877  (297237) users      (100)      114 2023-05-19 19:00:10.000000 ggen-1.0.0/ggen/__init__.py
--rw-r--r--   0 hass877  (297237) users      (100)     7090 2023-05-19 19:00:10.000000 ggen-1.0.0/ggen/driver_mod.py
--rw-r--r--   0 hass877  (297237) users      (100)     6885 2023-05-19 19:00:10.000000 ggen-1.0.0/ggen/gen_exodus.py
--rw-r--r--   0 hass877  (297237) users      (100)     5479 2023-05-19 19:00:10.000000 ggen-1.0.0/ggen/gen_phys_grids.py
--rw-r--r--   0 hass877  (297237) users      (100)     8450 2023-05-19 19:00:10.000000 ggen-1.0.0/ggen/gen_rll_grid.py
--rw-r--r--   0 hass877  (297237) users      (100)     9852 2023-05-19 19:00:10.000000 ggen-1.0.0/ggen/gen_scrip_file.py
--rw-r--r--   0 hass877  (297237) users      (100)     6014 2023-05-19 19:00:10.000000 ggen-1.0.0/ggen/get_face_area.py
--rw-r--r--   0 hass877  (297237) users      (100)     5681 2023-05-19 19:00:10.000000 ggen-1.0.0/ggen/ggrids.py
--rw-r--r--   0 hass877  (297237) users      (100)     2556 2023-05-19 19:00:10.000000 ggen-1.0.0/ggen/main.py
--rw-r--r--   0 hass877  (297237) users      (100)     3027 2023-05-19 19:00:10.000000 ggen-1.0.0/ggen/utils.py
-drwxr-xr-x   0 hass877  (297237) users      (100)        0 2023-05-19 19:20:48.596221 ggen-1.0.0/ggen.egg-info/
--rw-r--r--   0 hass877  (297237) users      (100)    15073 2023-05-19 19:20:47.000000 ggen-1.0.0/ggen.egg-info/PKG-INFO
--rw-r--r--   0 hass877  (297237) users      (100)      382 2023-05-19 19:20:48.000000 ggen-1.0.0/ggen.egg-info/SOURCES.txt
--rw-r--r--   0 hass877  (297237) users      (100)        1 2023-05-19 19:20:47.000000 ggen-1.0.0/ggen.egg-info/dependency_links.txt
--rw-r--r--   0 hass877  (297237) users      (100)       40 2023-05-19 19:20:47.000000 ggen-1.0.0/ggen.egg-info/entry_points.txt
--rw-r--r--   0 hass877  (297237) users      (100)       57 2023-05-19 19:20:47.000000 ggen-1.0.0/ggen.egg-info/requires.txt
--rw-r--r--   0 hass877  (297237) users      (100)        5 2023-05-19 19:20:47.000000 ggen-1.0.0/ggen.egg-info/top_level.txt
--rw-r--r--   0 hass877  (297237) users      (100)       38 2023-05-19 19:20:48.616548 ggen-1.0.0/setup.cfg
--rw-r--r--   0 hass877  (297237) users      (100)     1117 2023-05-19 19:17:57.000000 ggen-1.0.0/setup.py
+drwxr-xr-x   0 hass877  (619644916) PNL\Domain Users (2016721313)        0 2023-05-21 03:35:08.491329 ggen-1.1.0/
+-rw-r--r--   0 hass877  (619644916) PNL\Domain Users (2016721313)     1070 2023-05-12 22:14:41.000000 ggen-1.1.0/LICENSE
+-rw-r--r--   0 hass877  (619644916) PNL\Domain Users (2016721313)    15073 2023-05-21 03:35:08.490853 ggen-1.1.0/PKG-INFO
+-rw-r--r--   0 hass877  (619644916) PNL\Domain Users (2016721313)    14619 2023-05-14 01:08:26.000000 ggen-1.1.0/README.md
+drwxr-xr-x   0 hass877  (619644916) PNL\Domain Users (2016721313)        0 2023-05-21 03:35:08.485033 ggen-1.1.0/ggen/
+-rw-r--r--   0 hass877  (619644916) PNL\Domain Users (2016721313)      114 2023-05-12 22:14:41.000000 ggen-1.1.0/ggen/__init__.py
+-rw-r--r--   0 hass877  (619644916) PNL\Domain Users (2016721313)     7090 2023-05-12 22:14:41.000000 ggen-1.1.0/ggen/driver_mod.py
+-rw-r--r--   0 hass877  (619644916) PNL\Domain Users (2016721313)     6885 2023-05-12 22:14:41.000000 ggen-1.1.0/ggen/gen_exodus.py
+-rw-r--r--   0 hass877  (619644916) PNL\Domain Users (2016721313)     5479 2023-05-12 22:14:41.000000 ggen-1.1.0/ggen/gen_phys_grids.py
+-rw-r--r--   0 hass877  (619644916) PNL\Domain Users (2016721313)     8450 2023-05-18 19:49:14.000000 ggen-1.1.0/ggen/gen_rll_grid.py
+-rw-r--r--   0 hass877  (619644916) PNL\Domain Users (2016721313)     9912 2023-05-19 23:26:23.000000 ggen-1.1.0/ggen/gen_scrip_file.py
+-rw-r--r--   0 hass877  (619644916) PNL\Domain Users (2016721313)     6014 2023-05-12 22:14:41.000000 ggen-1.1.0/ggen/get_face_area.py
+-rw-r--r--   0 hass877  (619644916) PNL\Domain Users (2016721313)     5681 2023-05-12 22:14:41.000000 ggen-1.1.0/ggen/ggrids.py
+-rw-r--r--   0 hass877  (619644916) PNL\Domain Users (2016721313)     2556 2023-05-12 22:14:41.000000 ggen-1.1.0/ggen/main.py
+-rw-r--r--   0 hass877  (619644916) PNL\Domain Users (2016721313)     3027 2023-05-12 22:14:41.000000 ggen-1.1.0/ggen/utils.py
+drwxr-xr-x   0 hass877  (619644916) PNL\Domain Users (2016721313)        0 2023-05-21 03:35:08.490149 ggen-1.1.0/ggen.egg-info/
+-rw-r--r--   0 hass877  (619644916) PNL\Domain Users (2016721313)    15073 2023-05-21 03:35:08.000000 ggen-1.1.0/ggen.egg-info/PKG-INFO
+-rw-r--r--   0 hass877  (619644916) PNL\Domain Users (2016721313)      382 2023-05-21 03:35:08.000000 ggen-1.1.0/ggen.egg-info/SOURCES.txt
+-rw-r--r--   0 hass877  (619644916) PNL\Domain Users (2016721313)        1 2023-05-21 03:35:08.000000 ggen-1.1.0/ggen.egg-info/dependency_links.txt
+-rw-r--r--   0 hass877  (619644916) PNL\Domain Users (2016721313)       40 2023-05-21 03:35:08.000000 ggen-1.1.0/ggen.egg-info/entry_points.txt
+-rw-r--r--   0 hass877  (619644916) PNL\Domain Users (2016721313)       57 2023-05-21 03:35:08.000000 ggen-1.1.0/ggen.egg-info/requires.txt
+-rw-r--r--   0 hass877  (619644916) PNL\Domain Users (2016721313)        5 2023-05-21 03:35:08.000000 ggen-1.1.0/ggen.egg-info/top_level.txt
+-rw-r--r--   0 hass877  (619644916) PNL\Domain Users (2016721313)       38 2023-05-21 03:35:08.491460 ggen-1.1.0/setup.cfg
+-rw-r--r--   0 hass877  (619644916) PNL\Domain Users (2016721313)     1117 2023-05-21 03:07:45.000000 ggen-1.1.0/setup.py
```

### Comparing `ggen-1.0.0/LICENSE` & `ggen-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ggen-1.0.0/PKG-INFO` & `ggen-1.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ggen
-Version: 1.0.0
+Version: 1.1.0
 Summary: Package for generating grid meshes and performing conservative remapping
 Home-page: https://github.com/TaufiqHassan/ggen
 Author: Taufiq Hassan
 Author-email: taufiq.hassan@pnnl.gov
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
```

### Comparing `ggen-1.0.0/README.md` & `ggen-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `ggen-1.0.0/ggen/driver_mod.py` & `ggen-1.1.0/ggen/driver_mod.py`

 * *Files identical despite different names*

### Comparing `ggen-1.0.0/ggen/gen_exodus.py` & `ggen-1.1.0/ggen/gen_exodus.py`

 * *Files identical despite different names*

### Comparing `ggen-1.0.0/ggen/gen_phys_grids.py` & `ggen-1.1.0/ggen/gen_phys_grids.py`

 * *Files identical despite different names*

### Comparing `ggen-1.0.0/ggen/gen_rll_grid.py` & `ggen-1.1.0/ggen/gen_rll_grid.py`

 * *Files identical despite different names*

### Comparing `ggen-1.0.0/ggen/gen_scrip_file.py` & `ggen-1.1.0/ggen/gen_scrip_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,15 @@
                 dir_path = get_dir_path(self.fdir)
                 data = xr.open_dataset(dir_path / str(self.file))
             n_lon = data.dims[self.xdim]
             n_lat = data.dims[self.ydim]
             dir_path = get_dir_path(self.path)
             fname = dir_path / str('RLL'+str(n_lat)+'x'+str(n_lon)+'_SCRIP.nc')
             if not Path(fname).is_file():
-                coord, modf, faces, n_lat, n_lon, rank = gen_RLL(res=self.nResolution,fdir=self.fdir,file=self.file).get_rll()
+                coord, modf, faces, n_lat, n_lon, rank = gen_RLL(res=self.nResolution,fdir=self.fdir,file=self.file,xdim=self.xdim,ydim=self.ydim).get_rll()
                 dims = np.array([n_lon, n_lat],dtype=np.int32)
             else:
                 self.logger.info(str(fname)+' already exists!\n Using it.')
                 return fname
         elif (self.grid != None):
             dir_path = get_dir_path(self.path)
             fname = dir_path / str(str(self.grid)[:-3]+'.nc')
@@ -105,15 +105,15 @@
                 return dir_path / str(str(self.grid))
         elif ('x' in self.nResolution):
             n_lon=int(self.nResolution.split('x')[1])
             n_lat=int(self.nResolution.split('x')[0])
             dir_path = get_dir_path(self.path)
             fname = dir_path / str('RLL'+str(n_lat)+'x'+str(n_lon)+'_SCRIP.nc')
             if not Path(fname).is_file():
-                coord, modf, faces, n_lat, n_lon, rank = gen_RLL(res=self.nResolution,fdir=self.fdir,file=self.file).get_rll()
+                coord, modf, faces, n_lat, n_lon, rank = gen_RLL(res=self.nResolution,fdir=self.fdir,file=self.file,xdim=self.xdim,ydim=self.ydim).get_rll()
                 dims = np.array([n_lon, n_lat],dtype=np.int32)
             else:
                 self.logger.info(str(fname)+' already exists!\n Using it.')
                 return fname
         else:
             dir_path = get_dir_path(self.path)
             fname = dir_path / str('ne'+str(self.nResolution)+'pg2_SCRIP.nc')
```

### Comparing `ggen-1.0.0/ggen/get_face_area.py` & `ggen-1.1.0/ggen/get_face_area.py`

 * *Files identical despite different names*

### Comparing `ggen-1.0.0/ggen/ggrids.py` & `ggen-1.1.0/ggen/ggrids.py`

 * *Files identical despite different names*

### Comparing `ggen-1.0.0/ggen/main.py` & `ggen-1.1.0/ggen/main.py`

 * *Files identical despite different names*

### Comparing `ggen-1.0.0/ggen/utils.py` & `ggen-1.1.0/ggen/utils.py`

 * *Files identical despite different names*

### Comparing `ggen-1.0.0/ggen.egg-info/PKG-INFO` & `ggen-1.1.0/ggen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ggen
-Version: 1.0.0
+Version: 1.1.0
 Summary: Package for generating grid meshes and performing conservative remapping
 Home-page: https://github.com/TaufiqHassan/ggen
 Author: Taufiq Hassan
 Author-email: taufiq.hassan@pnnl.gov
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
```

### Comparing `ggen-1.0.0/setup.py` & `ggen-1.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     'netCDF4',
     'nco',
     'tempest-remap'
 ]
 
 setup(
     name='ggen',
-    version='1.0.0',
+    version='1.1.0',
     description="Package for generating grid meshes and performing conservative remapping",
     long_description=readme,
     long_description_content_type='text/markdown',
     author="Taufiq Hassan",
     author_email='taufiq.hassan@pnnl.gov',
     url='https://github.com/TaufiqHassan/ggen',
     entry_points={
```

