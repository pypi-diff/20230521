# Comparing `tmp/hydro_raster-0.0.5.tar.gz` & `tmp/hydro_raster-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hydro_raster-0.0.5.tar", last modified: Sat Sep 17 23:02:44 2022, max compression
+gzip compressed data, was "dist/hydro_raster-0.0.6.tar", last modified: Sun May 21 19:36:22 2023, max compression
```

## Comparing `hydro_raster-0.0.5.tar` & `hydro_raster-0.0.6.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 ming       (502) staff       (20)        0 2022-09-17 23:02:44.000000 hydro_raster-0.0.5/
--rw-r--r--   0 ming       (502) staff       (20)      168 2022-04-01 15:19:17.000000 hydro_raster-0.0.5/MANIFEST.in
--rw-r--r--   0 ming       (502) staff       (20)     3813 2022-09-17 23:02:44.000000 hydro_raster-0.0.5/PKG-INFO
--rw-r--r--   0 ming       (502) staff       (20)     2605 2022-06-08 17:17:02.000000 hydro_raster-0.0.5/README.md
-drwxr-xr-x   0 ming       (502) staff       (20)        0 2022-09-17 23:02:44.000000 hydro_raster-0.0.5/hydro_raster/
--rw-r--r--   0 ming       (502) staff       (20)    29376 2022-09-17 22:22:25.000000 hydro_raster-0.0.5/hydro_raster/Raster.py
--rwxr-xr-x   0 ming       (502) staff       (20)     7778 2022-02-09 21:10:07.000000 hydro_raster-0.0.5/hydro_raster/Tutorial.py
--rwxr-xr-x   0 ming       (502) staff       (20)     5591 2022-03-31 07:48:36.000000 hydro_raster-0.0.5/hydro_raster/Tutorial_carlisle.py
--rwxr-xr-x   0 ming       (502) staff       (20)      819 2022-03-11 11:19:47.000000 hydro_raster-0.0.5/hydro_raster/__init__.py
--rwxr-xr-x   0 ming       (502) staff       (20)    28075 2022-03-08 16:36:39.000000 hydro_raster-0.0.5/hydro_raster/channel_geometry.py
--rwxr-xr-x   0 ming       (502) staff       (20)    13311 2022-03-08 16:37:26.000000 hydro_raster-0.0.5/hydro_raster/convert_coords.py
--rwxr-xr-x   0 ming       (502) staff       (20)     4356 2021-04-01 10:31:37.000000 hydro_raster-0.0.5/hydro_raster/coords_interp.py
--rwxr-xr-x   0 ming       (502) staff       (20)     8015 2022-02-09 21:09:04.000000 hydro_raster-0.0.5/hydro_raster/demo_functions.py
--rw-r--r--   0 ming       (502) staff       (20)    15510 2022-04-20 11:56:37.000000 hydro_raster-0.0.5/hydro_raster/grid_show.py
--rw-r--r--   0 ming       (502) staff       (20)    19664 2021-03-29 15:04:20.000000 hydro_raster-0.0.5/hydro_raster/interp_line2surface.py
--rwxr-xr-x   0 ming       (502) staff       (20)     8854 2022-06-08 17:19:06.000000 hydro_raster-0.0.5/hydro_raster/remove_block.py
--rwxr-xr-x   0 ming       (502) staff       (20)     4099 2021-01-08 17:33:28.000000 hydro_raster-0.0.5/hydro_raster/river_bed_exmaple.py
-drwxr-xr-x   0 ming       (502) staff       (20)        0 2022-09-17 23:02:44.000000 hydro_raster-0.0.5/hydro_raster/sample/
--rw-r--r--   0 ming       (502) staff       (20)  6300262 2021-05-26 13:44:17.000000 hydro_raster-0.0.5/hydro_raster/sample/CA1_5m.tif
--rw-r--r--   0 ming       (502) staff       (20)        5 2022-03-08 17:05:24.000000 hydro_raster-0.0.5/hydro_raster/sample/CA1_overhead_features.cpg
--rw-r--r--   0 ming       (502) staff       (20)      226 2022-03-08 17:47:50.000000 hydro_raster-0.0.5/hydro_raster/sample/CA1_overhead_features.dbf
--rw-r--r--   0 ming       (502) staff       (20)      417 2022-03-08 17:05:24.000000 hydro_raster-0.0.5/hydro_raster/sample/CA1_overhead_features.prj
--rw-r--r--   0 ming       (502) staff       (20)      659 2022-03-08 17:05:24.000000 hydro_raster-0.0.5/hydro_raster/sample/CA1_overhead_features.qmd
--rw-r--r--   0 ming       (502) staff       (20)      644 2022-03-08 17:47:50.000000 hydro_raster-0.0.5/hydro_raster/sample/CA1_overhead_features.shp
--rw-r--r--   0 ming       (502) staff       (20)      132 2022-03-08 17:47:50.000000 hydro_raster-0.0.5/hydro_raster/sample/CA1_overhead_features.shx
--rw-r--r--   0 ming       (502) staff       (20)    19968 2022-07-10 21:45:03.000000 hydro_raster-0.0.5/hydro_raster/spatial_analysis.py
-drwxr-xr-x   0 ming       (502) staff       (20)        0 2022-09-17 23:02:44.000000 hydro_raster-0.0.5/hydro_raster.egg-info/
--rw-r--r--   0 ming       (502) staff       (20)     3813 2022-09-17 23:02:44.000000 hydro_raster-0.0.5/hydro_raster.egg-info/PKG-INFO
--rw-r--r--   0 ming       (502) staff       (20)      906 2022-09-17 23:02:44.000000 hydro_raster-0.0.5/hydro_raster.egg-info/SOURCES.txt
--rw-r--r--   0 ming       (502) staff       (20)        1 2022-09-17 23:02:44.000000 hydro_raster-0.0.5/hydro_raster.egg-info/dependency_links.txt
--rw-r--r--   0 ming       (502) staff       (20)       53 2022-09-17 23:02:44.000000 hydro_raster-0.0.5/hydro_raster.egg-info/requires.txt
--rw-r--r--   0 ming       (502) staff       (20)       13 2022-09-17 23:02:44.000000 hydro_raster-0.0.5/hydro_raster.egg-info/top_level.txt
--rw-r--r--   0 ming       (502) staff       (20)       38 2022-09-17 23:02:44.000000 hydro_raster-0.0.5/setup.cfg
--rwxr-xr-x   0 ming       (502) staff       (20)     2073 2022-09-17 22:38:40.000000 hydro_raster-0.0.5/setup.py
+drwxr-xr-x   0 ming       (502) staff       (20)        0 2023-05-21 19:36:22.000000 hydro_raster-0.0.6/
+-rw-r--r--   0 ming       (502) staff       (20)      168 2022-04-01 15:19:17.000000 hydro_raster-0.0.6/MANIFEST.in
+-rw-r--r--   0 ming       (502) staff       (20)     3813 2023-05-21 19:36:22.000000 hydro_raster-0.0.6/PKG-INFO
+-rw-r--r--   0 ming       (502) staff       (20)     2605 2022-06-08 17:17:02.000000 hydro_raster-0.0.6/README.md
+drwxr-xr-x   0 ming       (502) staff       (20)        0 2023-05-21 19:36:22.000000 hydro_raster-0.0.6/hydro_raster/
+-rw-r--r--   0 ming       (502) staff       (20)    32106 2023-05-21 19:31:51.000000 hydro_raster-0.0.6/hydro_raster/Raster.py
+-rwxr-xr-x   0 ming       (502) staff       (20)     7778 2022-02-09 21:10:07.000000 hydro_raster-0.0.6/hydro_raster/Tutorial.py
+-rwxr-xr-x   0 ming       (502) staff       (20)     5591 2022-03-31 07:48:36.000000 hydro_raster-0.0.6/hydro_raster/Tutorial_carlisle.py
+-rwxr-xr-x   0 ming       (502) staff       (20)      819 2022-03-11 11:19:47.000000 hydro_raster-0.0.6/hydro_raster/__init__.py
+-rwxr-xr-x   0 ming       (502) staff       (20)    28075 2022-03-08 16:36:39.000000 hydro_raster-0.0.6/hydro_raster/channel_geometry.py
+-rwxr-xr-x   0 ming       (502) staff       (20)    13311 2022-03-08 16:37:26.000000 hydro_raster-0.0.6/hydro_raster/convert_coords.py
+-rwxr-xr-x   0 ming       (502) staff       (20)     4356 2021-04-01 10:31:37.000000 hydro_raster-0.0.6/hydro_raster/coords_interp.py
+-rwxr-xr-x   0 ming       (502) staff       (20)     8015 2022-02-09 21:09:04.000000 hydro_raster-0.0.6/hydro_raster/demo_functions.py
+-rw-r--r--   0 ming       (502) staff       (20)    15428 2023-02-06 10:21:38.000000 hydro_raster-0.0.6/hydro_raster/grid_show.py
+-rw-r--r--   0 ming       (502) staff       (20)    19664 2021-03-29 15:04:20.000000 hydro_raster-0.0.6/hydro_raster/interp_line2surface.py
+-rwxr-xr-x   0 ming       (502) staff       (20)     8854 2022-06-08 17:19:06.000000 hydro_raster-0.0.6/hydro_raster/remove_block.py
+-rwxr-xr-x   0 ming       (502) staff       (20)     4099 2021-01-08 17:33:28.000000 hydro_raster-0.0.6/hydro_raster/river_bed_exmaple.py
+drwxr-xr-x   0 ming       (502) staff       (20)        0 2023-05-21 19:36:22.000000 hydro_raster-0.0.6/hydro_raster/sample/
+-rw-r--r--   0 ming       (502) staff       (20)  6300262 2021-05-26 13:44:17.000000 hydro_raster-0.0.6/hydro_raster/sample/CA1_5m.tif
+-rw-r--r--   0 ming       (502) staff       (20)        5 2022-03-08 17:05:24.000000 hydro_raster-0.0.6/hydro_raster/sample/CA1_overhead_features.cpg
+-rw-r--r--   0 ming       (502) staff       (20)      226 2022-03-08 17:47:50.000000 hydro_raster-0.0.6/hydro_raster/sample/CA1_overhead_features.dbf
+-rw-r--r--   0 ming       (502) staff       (20)      417 2022-03-08 17:05:24.000000 hydro_raster-0.0.6/hydro_raster/sample/CA1_overhead_features.prj
+-rw-r--r--   0 ming       (502) staff       (20)      659 2022-03-08 17:05:24.000000 hydro_raster-0.0.6/hydro_raster/sample/CA1_overhead_features.qmd
+-rw-r--r--   0 ming       (502) staff       (20)      644 2022-03-08 17:47:50.000000 hydro_raster-0.0.6/hydro_raster/sample/CA1_overhead_features.shp
+-rw-r--r--   0 ming       (502) staff       (20)      132 2022-03-08 17:47:50.000000 hydro_raster-0.0.6/hydro_raster/sample/CA1_overhead_features.shx
+-rw-r--r--   0 ming       (502) staff       (20)    19968 2022-07-10 21:45:03.000000 hydro_raster-0.0.6/hydro_raster/spatial_analysis.py
+drwxr-xr-x   0 ming       (502) staff       (20)        0 2023-05-21 19:36:22.000000 hydro_raster-0.0.6/hydro_raster.egg-info/
+-rw-r--r--   0 ming       (502) staff       (20)     3813 2023-05-21 19:36:22.000000 hydro_raster-0.0.6/hydro_raster.egg-info/PKG-INFO
+-rw-r--r--   0 ming       (502) staff       (20)      906 2023-05-21 19:36:22.000000 hydro_raster-0.0.6/hydro_raster.egg-info/SOURCES.txt
+-rw-r--r--   0 ming       (502) staff       (20)        1 2023-05-21 19:36:22.000000 hydro_raster-0.0.6/hydro_raster.egg-info/dependency_links.txt
+-rw-r--r--   0 ming       (502) staff       (20)       53 2023-05-21 19:36:22.000000 hydro_raster-0.0.6/hydro_raster.egg-info/requires.txt
+-rw-r--r--   0 ming       (502) staff       (20)       13 2023-05-21 19:36:22.000000 hydro_raster-0.0.6/hydro_raster.egg-info/top_level.txt
+-rw-r--r--   0 ming       (502) staff       (20)       38 2023-05-21 19:36:22.000000 hydro_raster-0.0.6/setup.cfg
+-rwxr-xr-x   0 ming       (502) staff       (20)     2073 2023-02-06 10:23:37.000000 hydro_raster-0.0.6/setup.py
```

### Comparing `hydro_raster-0.0.5/PKG-INFO` & `hydro_raster-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydro_raster
-Version: 0.0.5
+Version: 0.0.6
 Summary: To process raster data for hydro-logical/dynamic modelling
 Home-page: https://github.com/mingxiaodong/hydro-raster
 Author: Xiaodong Ming
 Author-email: x.ming@lboro.ac.uk
 License: LICENSE.txt
 Description: hydro_raster
         --------
```

### Comparing `hydro_raster-0.0.5/README.md` & `hydro_raster-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `hydro_raster-0.0.5/hydro_raster/Raster.py` & `hydro_raster-0.0.6/hydro_raster/Raster.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,23 +106,26 @@
         
         # shape and cellsize
         self.shape = self.array.shape
         if array.shape != (header['nrows'], header['ncols']):
             raise ValueError(('shape of array is not consistent with '
                               'nrows and ncols in header'))
         self.cellsize = header['cellsize']
+        self.NODATA_value = header['NODATA_value']
         
         # num_valid_cells
         self.num_valid_cells = np.sum(~np.isnan(self.array))
         self.size = self.array.size
         
         # summary
         self.get_summary()
         
         self.to_rasterio = self.write_tif
+        
+        self.copy = self.duplicate
 
             
 #%%============================= Spatial analyst ==============================   
     def get_summary(self):
         """Get information summary of the object
 
         Returns
@@ -136,14 +139,29 @@
         if hasattr(self, 'crs'):
             summary['crs'] = self.crs.data
         if hasattr(self, 'source_file'):
             summary['source_file'] = self.source_file
         self._summary = summary
         return summary
 
+    def to_int(self, dtype='int32'):
+        """Convert data array to int type
+        nan value will be replaced as NODATA_value, default: -9999 
+        
+
+        Returns
+        -------
+        None.
+
+        """
+        new_obj = self.copy()
+        new_obj.array[np.isnan(self.array)] = self.NODATA_value
+        new_obj.array = np.around(new_obj.array).astype(dtype)
+        return new_obj
+
     def set_crs(self, crs):
         """set reference coordinate system
         Parameters
         ----------
         crs : int|string|rasterio.crs object
             epsg code|wkt|asterio.crs object
         """
@@ -152,78 +170,116 @@
         elif type(crs) is int:
             self.crs = rio.crs.CRS.from_epsg(crs)
         elif type(crs) is rio.crs.CRS:
             self.crs = crs
         else:
             raise IOError('crs must be int|string|rasterio.crs object')
 
-    def rect_clip(self, clip_extent):
+    def rect_clip(self, clip_extent, match_extent=False, return_slice=False):
         """clip raster according to a rectangle extent
 
         Args:
             clip_extent: list of [left, right, bottom, top]
+            match_extent: logical. If True, the x- and y- llcorner coordiantes
+              in header will be adjusted to match the coordinates of extent.
+              And the clip extent must be within the original extent.
+              Otherwise, the header will follow the original object.
+            return_slice: logical. If True, the slices of object to clip array
+              will be returned as an additional return value.
 
         Return:
             Raster: a new raster object
         """
-        X = clip_extent[0:2]
-        Y = clip_extent[2:4]
-        rows, cols = sp.map2sub(X, Y, self.header)
-        x_centre, y_centre = sp.sub2map(rows, cols, self.header)
-        xllcorner = min(x_centre)-0.5*self.header['cellsize']
-        yllcorner = min(y_centre)-0.5*self.header['cellsize']
+        X = np.array(clip_extent[0:2])
+        Y = np.array(clip_extent[2:4])
+        cellsize = self.cellsize
         header_new = copy.deepcopy(self.header)
-        if max(rows) >= self.header['nrows']:
-            max_row = self.header['nrows']
-        else:
-            max_row = max(rows)+1
-        if max(cols) >= self.header['ncols']:
-            max_col = self.header['ncols']
-        else:
-            max_col = max(cols)+1
-        if min(rows) <= 0:
-            min_row = 0
-        else:
-            min_row = min(rows) 
-        if min(cols) <= 0:
-            min_col = 0
-        else:
-            min_col = min(cols) 
-        array_new = self.array[min_row:max_row,
-                               min_col:max_col]
+
+        if match_extent:
+            insider_flag = (clip_extent[0] >= self.extent[0]) * \
+                           (clip_extent[1] <= self.extent[1]) * \
+                           (clip_extent[2] >= self.extent[2]) * \
+                           (clip_extent[3] <= self.extent[3])
+            if insider_flag is False:
+                raise ValueError(('clip extent is beyond the extent of '
+                                 'original raster'))
+            xllcorner = X.min()
+            yllcorner = Y.min()
+            nrows = np.around((Y.max()-yllcorner)/cellsize).astype('int')
+            ncols = np.around((X.max()-xllcorner)/cellsize).astype('int')
+            row0, col0 = sp.map2sub(xllcorner+cellsize/2, 
+                                    yllcorner+cellsize/2, self.header)
+            min_row = row0-nrows
+            max_row = row0
+            min_col = col0
+            max_col = col0+ncols
+        else:
+            X_centre = np.array([X.min()+cellsize/2, X.max()-cellsize/2])
+            Y_centre = np.array([Y.min()+cellsize/2, Y.max()-cellsize/2])
+            rows, cols = sp.map2sub(X_centre, Y_centre, self.header)
+            # get x and y centre coords in the original raster
+            x_centre, y_centre = sp.sub2map(rows, cols, self.header)
+            xllcorner = min(x_centre)-cellsize/2
+            yllcorner = min(y_centre)-cellsize/2
+            if max(rows) >= self.header['nrows']:
+                max_row = self.header['nrows']
+            else:
+                max_row = max(rows)+1
+            if max(cols) >= self.header['ncols']:
+                max_col = self.header['ncols']
+            else:
+                max_col = max(cols)+1
+            if min(rows) <= 0:
+                min_row = 0
+            else:
+                min_row = min(rows) 
+            if min(cols) <= 0:
+                min_col = 0
+            else:
+                min_col = min(cols)
+        loc = (slice(min_row, max_row), slice(min_col, max_col))
+        array_new = self.array[loc]
         header_new['nrows'] = array_new.shape[0]
         header_new['ncols'] = array_new.shape[1]
         header_new['xllcorner'] = xllcorner
         header_new['yllcorner'] = yllcorner
         obj_new = Raster(array=array_new, header=header_new)
         if hasattr(self, 'crs'):
             obj_new.crs = self.crs
-        return obj_new
+        if return_slice:
+            return obj_new, loc
+        else:
+            return obj_new
     
     def clip(self, clip_mask=None):
         """clip raster according to a mask
 
         Args:
             mask: 1. string name of a shapefile or 2. 2-col numpy array giving
                 X and Y coords in each column to shape the mask polygon
         
         Return:
             Raster: a new raster object
         """
         from rasterio import mask
         ds_rio = self.to_rasterio_ds()
         if type(clip_mask) is str:
-            with shapefile.Reader(clip_mask) as shp:
-                shapes_geojson = shp.__geo_interface__
+            try:
+                with shapefile.Reader(clip_mask) as shp:
+                    shapes_geojson = shp.__geo_interface__
+            except:
+                ds_rio.close()
+                raise IOError(f'cannot find {clip_mask}')
             shape_geoms = [x['geometry'] for x in shapes_geojson['features']]
             shape_geoms = [x for x in shape_geoms if x != None]
         elif type(clip_mask) is np.ndarray:
             shape_geoms = {'type':'Polygon', 'coordinates':[clip_mask]}
             shape_geoms = [shape_geoms]
         else:
+            ds_rio.close()
             raise IOError('mask must be either a string or a numpy array')
         
         out_image, out_transform = mask.mask(ds_rio, shape_geoms, crop=True) #
         ds_rio.close()
         array_new = out_image[0]
         cellsize = out_transform[0]
         xllcorner = out_transform[2]
@@ -316,16 +372,16 @@
         from rasterio.enums import Resampling
         method_list = ['nearest', 'bilinear', 'cubic', 'cubic_spline',
                        'lanczos', 'average', 'mode', 'gauss', 'max', 'min',
                        'med', 'q1', 'q3']
         ind = method_list.index(method)
         upscale_factor = self.cellsize/new_cellsize
         ds_rio = self.to_rasterio_ds()
-        new_shape = (1, int(ds_rio.height * upscale_factor),
-                        int(ds_rio.width * upscale_factor))
+        new_shape = (1, np.around(ds_rio.height * upscale_factor).astype('int'),
+                        np.around(ds_rio.width * upscale_factor).astype('int'))
         resampling_method = Resampling(ind)
         data = ds_rio.read(out_shape=new_shape, resampling=resampling_method)
         data = data[0]
         # scale image transform
         transform = ds_rio.transform * ds_rio.transform.scale(
                     (ds_rio.width / data.shape[-1]),
                     (ds_rio.height / data.shape[-2]))
@@ -530,32 +586,38 @@
             self.write_asc(output_file, compression=True)
         elif output_file.endswith('.tif'):
             self.write_tif(output_file)
         else:
             self.write_asc(output_file, compression)
         
     
-    def write_tif(self, output_file, src_epsg=27700):
+    def write_tif(self, output_file, src_epsg=27700, dtype='float64'):
         """ Convert to a rasterio dataset
         
         Args:
             output_file: a string to give output file name
             src_epsg: int scalar to give EPSG code of the coordinate reference
                 system of the original dataset, default is 27700 for BNG
 
         """
         
         if output_file.endswith('.tif'):
             filename = output_file
         else:
             filename = output_file+'.tif'
-        if not hasattr(self, 'meta'):
-            self.get_meta(src_epsg)
-        meta = self.meta # dictionary
-        array_data = self.array+0.0
+        if 'int' in dtype:
+            new_obj = self.to_int(dtype)
+            array_data = new_obj.array+0
+            new_obj.get_meta(src_epsg)
+            meta = new_obj.meta
+        else:
+            array_data = self.array+0.0
+            if not hasattr(self, 'meta'):
+                self.get_meta(src_epsg)
+            meta = self.meta # dictionary
         meta['dtype'] = array_data.dtype.name
         nomask = np.isnan(array_data)
         array_data[nomask] = meta['nodata']
         with rio.open(filename, 'w', **meta) as out_f:
             out_f.write(array_data, 1)
         meta['dtype'] = self.array.dtype.name
     
@@ -720,14 +782,15 @@
     
     def duplicate(self):
         """ duplicate the Raster object and return a new one so that change 
         the new object will not affect the original one
         """
         obj_duplicate = copy.deepcopy(self)
         return obj_duplicate
+    
 #%%
 def merge(obj_origin, obj_target, resample_method='bilinear'):
     """Merge the obj_origin to obj_target
 
     assign grid values in the origin Raster to the cooresponding grid cells in
     the target object. If cellsize are not equal, the origin Raster will be
     firstly resampled to the target object.
```

### Comparing `hydro_raster-0.0.5/hydro_raster/Tutorial.py` & `hydro_raster-0.0.6/hydro_raster/Tutorial.py`

 * *Files identical despite different names*

### Comparing `hydro_raster-0.0.5/hydro_raster/Tutorial_carlisle.py` & `hydro_raster-0.0.6/hydro_raster/Tutorial_carlisle.py`

 * *Files identical despite different names*

### Comparing `hydro_raster-0.0.5/hydro_raster/__init__.py` & `hydro_raster-0.0.6/hydro_raster/__init__.py`

 * *Files identical despite different names*

### Comparing `hydro_raster-0.0.5/hydro_raster/channel_geometry.py` & `hydro_raster-0.0.6/hydro_raster/channel_geometry.py`

 * *Files identical despite different names*

### Comparing `hydro_raster-0.0.5/hydro_raster/convert_coords.py` & `hydro_raster-0.0.6/hydro_raster/convert_coords.py`

 * *Files identical despite different names*

### Comparing `hydro_raster-0.0.5/hydro_raster/coords_interp.py` & `hydro_raster-0.0.6/hydro_raster/coords_interp.py`

 * *Files identical despite different names*

### Comparing `hydro_raster-0.0.5/hydro_raster/demo_functions.py` & `hydro_raster-0.0.6/hydro_raster/demo_functions.py`

 * *Files identical despite different names*

### Comparing `hydro_raster-0.0.5/hydro_raster/grid_show.py` & `hydro_raster-0.0.6/hydro_raster/grid_show.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,14 @@
         **kwargs: keywords argument of function imshow
 
     """
     if raster_obj is not None:
         array = raster_obj.array
         header = raster_obj.header
     # change NODATA_value to nan
-    np.warnings.filterwarnings('ignore')
     array = array+0
     ind = array == header['NODATA_value']
     if ind.sum()>0:
         array = array.astype('float32')
         array[ind] = np.nan
     # adjust tick label and axis label
     map_extent = sp.header2extent(header)    
@@ -105,15 +104,14 @@
                                 'labelspacing':0.1}, 
                      scale_ratio=1,
                      alpha=1)
     """
     if raster_obj is not None:
         array = raster_obj.array
         header = raster_obj.header
-    np.warnings.filterwarnings('ignore')
     ind = array == header['NODATA_value']
     array = array.astype('float64')+0
     array[ind] = np.nan
     # create color ranks
     array, newcmp, norm= _set_color_rank(array, breaks, color)
     map_extent = sp.header2extent(header)
     if ax is None:
```

### Comparing `hydro_raster-0.0.5/hydro_raster/interp_line2surface.py` & `hydro_raster-0.0.6/hydro_raster/interp_line2surface.py`

 * *Files identical despite different names*

### Comparing `hydro_raster-0.0.5/hydro_raster/remove_block.py` & `hydro_raster-0.0.6/hydro_raster/remove_block.py`

 * *Files identical despite different names*

### Comparing `hydro_raster-0.0.5/hydro_raster/river_bed_exmaple.py` & `hydro_raster-0.0.6/hydro_raster/river_bed_exmaple.py`

 * *Files identical despite different names*

### Comparing `hydro_raster-0.0.5/hydro_raster/sample/CA1_5m.tif` & `hydro_raster-0.0.6/hydro_raster/sample/CA1_5m.tif`

 * *Files identical despite different names*

### Comparing `hydro_raster-0.0.5/hydro_raster/sample/CA1_overhead_features.qmd` & `hydro_raster-0.0.6/hydro_raster/sample/CA1_overhead_features.qmd`

 * *Files identical despite different names*

### Comparing `hydro_raster-0.0.5/hydro_raster/sample/CA1_overhead_features.shp` & `hydro_raster-0.0.6/hydro_raster/sample/CA1_overhead_features.shp`

 * *Files identical despite different names*

### Comparing `hydro_raster-0.0.5/hydro_raster/spatial_analysis.py` & `hydro_raster-0.0.6/hydro_raster/spatial_analysis.py`

 * *Files identical despite different names*

### Comparing `hydro_raster-0.0.5/hydro_raster.egg-info/PKG-INFO` & `hydro_raster-0.0.6/hydro_raster.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hydro-raster
-Version: 0.0.5
+Version: 0.0.6
 Summary: To process raster data for hydro-logical/dynamic modelling
 Home-page: https://github.com/mingxiaodong/hydro-raster
 Author: Xiaodong Ming
 Author-email: x.ming@lboro.ac.uk
 License: LICENSE.txt
 Description: hydro_raster
         --------
```

### Comparing `hydro_raster-0.0.5/hydro_raster.egg-info/SOURCES.txt` & `hydro_raster-0.0.6/hydro_raster.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hydro_raster-0.0.5/setup.py` & `hydro_raster-0.0.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from os import path
 here = path.abspath(path.dirname(__file__))
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
       name='hydro_raster',
-      version='0.0.5',
+      version='0.0.6',
       description='To process raster data for hydro-logical/dynamic modelling',
       url='https://github.com/mingxiaodong/hydro-raster',
       author='Xiaodong Ming',
       author_email='x.ming@lboro.ac.uk',
       long_description=long_description,
       long_description_content_type='text/markdown',
       classifiers=['Development Status :: 3 - Alpha',
```

