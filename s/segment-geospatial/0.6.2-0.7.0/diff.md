# Comparing `tmp/segment-geospatial-0.6.2.tar.gz` & `tmp/segment-geospatial-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "segment-geospatial-0.6.2.tar", last modified: Wed May 17 18:31:23 2023, max compression
+gzip compressed data, was "segment-geospatial-0.7.0.tar", last modified: Sun May 21 02:28:41 2023, max compression
```

## Comparing `segment-geospatial-0.6.2.tar` & `segment-geospatial-0.7.0.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:31:23.676997 segment-geospatial-0.6.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-17 18:31:13.000000 segment-geospatial-0.6.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-17 18:31:13.000000 segment-geospatial-0.6.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5896 2023-05-17 18:31:23.676997 segment-geospatial-0.6.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-05-17 18:31:13.000000 segment-geospatial-0.6.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-17 18:31:13.000000 segment-geospatial-0.6.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:31:23.672997 segment-geospatial-0.6.2/samgeo/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-17 18:31:13.000000 segment-geospatial-0.6.2/samgeo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    68522 2023-05-17 18:31:13.000000 segment-geospatial-0.6.2/samgeo/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    26835 2023-05-17 18:31:13.000000 segment-geospatial-0.6.2/samgeo/samgeo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 18:31:23.676997 segment-geospatial-0.6.2/segment_geospatial.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5896 2023-05-17 18:31:23.000000 segment-geospatial-0.6.2/segment_geospatial.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-17 18:31:23.000000 segment-geospatial-0.6.2/segment_geospatial.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-17 18:31:23.000000 segment-geospatial-0.6.2/segment_geospatial.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 18:31:23.000000 segment-geospatial-0.6.2/segment_geospatial.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-17 18:31:23.000000 segment-geospatial-0.6.2/segment_geospatial.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-17 18:31:23.000000 segment-geospatial-0.6.2/segment_geospatial.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-17 18:31:23.676997 segment-geospatial-0.6.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-17 18:31:13.000000 segment-geospatial-0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 02:28:41.673598 segment-geospatial-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-21 02:28:27.000000 segment-geospatial-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-21 02:28:27.000000 segment-geospatial-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5993 2023-05-21 02:28:41.673598 segment-geospatial-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5226 2023-05-21 02:28:27.000000 segment-geospatial-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-21 02:28:27.000000 segment-geospatial-0.7.0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 02:28:41.673598 segment-geospatial-0.7.0/samgeo/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-21 02:28:27.000000 segment-geospatial-0.7.0/samgeo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71643 2023-05-21 02:28:27.000000 segment-geospatial-0.7.0/samgeo/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28939 2023-05-21 02:28:27.000000 segment-geospatial-0.7.0/samgeo/samgeo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-05-21 02:28:27.000000 segment-geospatial-0.7.0/samgeo/text_sam.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 02:28:41.673598 segment-geospatial-0.7.0/segment_geospatial.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5993 2023-05-21 02:28:41.000000 segment-geospatial-0.7.0/segment_geospatial.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      387 2023-05-21 02:28:41.000000 segment-geospatial-0.7.0/segment_geospatial.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-21 02:28:41.000000 segment-geospatial-0.7.0/segment_geospatial.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 02:28:41.000000 segment-geospatial-0.7.0/segment_geospatial.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-05-21 02:28:41.000000 segment-geospatial-0.7.0/segment_geospatial.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-21 02:28:41.000000 segment-geospatial-0.7.0/segment_geospatial.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-05-21 02:28:41.677598 segment-geospatial-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-21 02:28:27.000000 segment-geospatial-0.7.0/setup.py
```

### Comparing `segment-geospatial-0.6.2/LICENSE` & `segment-geospatial-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `segment-geospatial-0.6.2/PKG-INFO` & `segment-geospatial-0.7.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: segment-geospatial
-Version: 0.6.2
+Version: 0.7.0
 Summary: Meta AI' Segment Anything Model (SAM) for Geospatial Data
 Home-page: https://github.com/opengeos/segment-geospatial
 Author: Qiusheng Wu
 Author-email: giswqs@gmail.com
 License: MIT license
 Keywords: samgeo
 Classifier: Intended Audience :: Developers
@@ -49,14 +49,15 @@
 -   Visualize segmentation results on interactive maps
 
 ## Examples
 
 -   [Segmenting satellite imagery](https://samgeo.gishub.org/examples/satellite)
 -   [Automatically generating object masks](https://samgeo.gishub.org/examples/automatic_mask_generator)
 -   [Segmenting satellite imagery with input prompts](https://samgeo.gishub.org/examples/input_prompts)
+-   [Using segment-geospatial with ArcGIS Pro](https://samgeo.gishub.org/examples/input_prompts)
 
 ## Demos
 
 -   Automatic mask generator
 
 ![](https://i.imgur.com/I1IhDgz.gif)
```

### Comparing `segment-geospatial-0.6.2/README.md` & `segment-geospatial-0.7.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -27,14 +27,15 @@
 -   Visualize segmentation results on interactive maps
 
 ## Examples
 
 -   [Segmenting satellite imagery](https://samgeo.gishub.org/examples/satellite)
 -   [Automatically generating object masks](https://samgeo.gishub.org/examples/automatic_mask_generator)
 -   [Segmenting satellite imagery with input prompts](https://samgeo.gishub.org/examples/input_prompts)
+-   [Using segment-geospatial with ArcGIS Pro](https://samgeo.gishub.org/examples/input_prompts)
 
 ## Demos
 
 -   Automatic mask generator
 
 ![](https://i.imgur.com/I1IhDgz.gif)
```

### Comparing `segment-geospatial-0.6.2/samgeo/common.py` & `segment-geospatial-0.7.0/samgeo/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -649,14 +649,18 @@
     Args:
         filename (str): The vector file path.
         output (str, optional): The output geojson file path. Defaults to None.
 
     Returns:
         dict: The geojson dictionary.
     """
+
+    if not filename.startswith("http"):
+        filename = download_file(filename)
+
     gdf = gpd.read_file(filename, **kwargs)
     if output is None:
         return gdf.__geo_interface__
     else:
         gdf.to_file(output, driver="GeoJSON")
 
 
@@ -1392,20 +1396,32 @@
         plt.Rectangle((x0, y0), w, h, edgecolor="green", facecolor=(0, 0, 0, 0), lw=2)
     )
 
 
 def overlay_images(
     image1,
     image2,
-    opacity=0.5,
+    alpha=0.5,
     backend="TkAgg",
     height_ratios=[10, 1],
     show_args1={},
     show_args2={},
 ):
+    """Overlays two images using a slider to control the opacity of the top image.
+
+    Args:
+        image1 (str | np.ndarray): The first input image at the bottom represented as a NumPy array or the path to the image.
+        image2 (_type_): The second input image on top represented as a NumPy array or the path to the image.
+        alpha (float, optional): The alpha value of the top image. Defaults to 0.5.
+        backend (str, optional): The backend of the matplotlib plot. Defaults to "TkAgg".
+        height_ratios (list, optional): The height ratios of the two subplots. Defaults to [10, 1].
+        show_args1 (dict, optional): The keyword arguments to pass to the imshow() function for the first image. Defaults to {}.
+        show_args2 (dict, optional): The keyword arguments to pass to the imshow() function for the second image. Defaults to {}.
+
+    """
     import sys
     import matplotlib
     import matplotlib.widgets as mpwidgets
 
     if "google.colab" in sys.modules:
         backend = "inline"
         print(
@@ -1432,25 +1448,23 @@
     # Load the two images
     x = plt.imread(image1)
     y = plt.imread(image2)
 
     # Create the plot
     fig, (ax0, ax1) = plt.subplots(2, 1, gridspec_kw={"height_ratios": height_ratios})
     img0 = ax0.imshow(x, **show_args1)
-    img1 = ax0.imshow(y, alpha=opacity, **show_args2)
+    img1 = ax0.imshow(y, alpha=alpha, **show_args2)
 
     # Define the update function
     def update(value):
         img1.set_alpha(value)
         fig.canvas.draw_idle()
 
     # Create the slider
-    slider0 = mpwidgets.Slider(
-        ax=ax1, label="opacity", valmin=0, valmax=1, valinit=opacity
-    )
+    slider0 = mpwidgets.Slider(ax=ax1, label="alpha", valmin=0, valmax=1, valinit=alpha)
     slider0.on_changed(update)
 
     # Display the plot
     plt.show()
 
 
 def blend_images(
@@ -2101,7 +2115,73 @@
     geojson_str = json.dumps(feature_collection)
 
     if output is not None:
         with open(output, "w") as f:
             f.write(geojson_str)
     else:
         return geojson_str
+
+
+def show_canvas(image, fg_color=(0, 255, 0), bg_color=(0, 0, 255), radius=5):
+    """Show a canvas to collect foreground and background points.
+
+    Args:
+        image (str | np.ndarray): The input image.
+        fg_color (tuple, optional): The color for the foreground points. Defaults to (0, 255, 0).
+        bg_color (tuple, optional): The color for the background points. Defaults to (0, 0, 255).
+        radius (int, optional): The radius of the points. Defaults to 5.
+
+    Returns:
+        tuple: A tuple of two lists of foreground and background points.
+    """
+    if isinstance(image, str):
+        if image.startswith("http"):
+            image = download_file(image)
+
+        image = cv2.imread(image)
+    elif isinstance(image, np.ndarray):
+        pass
+    else:
+        raise ValueError("Input image must be a URL or a NumPy array.")
+
+    # Create an empty list to store the mouse click coordinates
+    left_clicks = []
+    right_clicks = []
+
+    # Create a mouse callback function
+    def get_mouse_coordinates(event, x, y, flags, param):
+        if event == cv2.EVENT_LBUTTONDOWN:
+            # Append the coordinates to the mouse_clicks list
+            left_clicks.append((x, y))
+
+            # Draw a green circle at the mouse click coordinates
+            cv2.circle(image, (x, y), radius, fg_color, -1)
+
+            # Show the updated image with the circle
+            cv2.imshow("Image", image)
+
+        elif event == cv2.EVENT_RBUTTONDOWN:
+            # Append the coordinates to the mouse_clicks list
+            right_clicks.append((x, y))
+
+            # Draw a red circle at the mouse click coordinates
+            cv2.circle(image, (x, y), radius, bg_color, -1)
+
+            # Show the updated image with the circle
+            cv2.imshow("Image", image)
+
+    # Create a window to display the image
+    cv2.namedWindow("Image")
+
+    # Set the mouse callback function for the window
+    cv2.setMouseCallback("Image", get_mouse_coordinates)
+
+    # Display the image in the window
+    cv2.imshow("Image", image)
+
+    # Wait for a key press to exit
+    cv2.waitKey(0)
+
+    # Destroy the window
+    cv2.destroyAllWindows()
+
+    return left_clicks, right_clicks
```

### Comparing `segment-geospatial-0.6.2/samgeo/samgeo.py` & `segment-geospatial-0.7.0/samgeo/samgeo.py`

 * *Files 3% similar despite different names*

```diff
@@ -305,33 +305,39 @@
         """
 
         import matplotlib.pyplot as plt
 
         if self.batch:
             self.objects = cv2.imread(self.masks)
         else:
-
             if self.objects is None:
                 self.save_masks(foreground=foreground, **kwargs)
 
         plt.figure(figsize=figsize)
         plt.imshow(self.objects, cmap=cmap)
         plt.axis(axis)
         plt.show()
 
     def show_anns(
-        self, figsize=(12, 10), axis="off", alpha=0.35, output=None, **kwargs
+        self,
+        figsize=(12, 10),
+        axis="off",
+        alpha=0.35,
+        output=None,
+        blend=True,
+        **kwargs,
     ):
         """Show the annotations (objects with random color) on the input image.
 
         Args:
             figsize (tuple, optional): The figure size. Defaults to (12, 10).
             axis (str, optional): Whether to show the axis. Defaults to "off".
             alpha (float, optional): The alpha value for the annotations. Defaults to 0.35.
             output (str, optional): The path to the output image. Defaults to None.
+            blend (bool, optional): Whether to show the input image. Defaults to True.
         """
 
         import matplotlib.pyplot as plt
 
         anns = self.masks
 
         if self.image is None:
@@ -370,15 +376,20 @@
             kwargs["bbox_inches"] = "tight"
 
         plt.axis(axis)
 
         self.annotations = (img[:, :, 0:3] * 255).astype(np.uint8)
 
         if output is not None:
-            array = blend_images(self.annotations, self.image, alpha=alpha, show=False)
+            if blend:
+                array = blend_images(
+                    self.annotations, self.image, alpha=alpha, show=False
+                )
+            else:
+                array = self.annotations
             array_to_image(array, output, self.source)
 
     def set_image(self, image, image_format="RGB"):
         """Set the input image as a numpy array.
 
         Args:
             image (np.ndarray): The input image as a numpy array.
@@ -486,14 +497,20 @@
 
         if isinstance(point_coords, str):
             point_coords = vector_to_geojson(point_coords)
 
         if isinstance(point_coords, dict):
             point_coords = geojson_to_coords(point_coords)
 
+        if hasattr(self, "point_coords"):
+            point_coords = self.point_coords
+
+        if hasattr(self, "point_labels"):
+            point_labels = self.point_labels
+
         if point_crs is not None:
             point_coords = coords_to_xy(self.image, point_coords, point_crs)
 
         if isinstance(point_coords, list):
             point_coords = np.array(point_coords)
 
         if point_labels is None:
@@ -525,18 +542,58 @@
         if output is not None:
             self.save_prediction(output, index, mask_multiplier, dtype, **kwargs)
 
         if return_results:
             return masks, scores, logits
 
     def show_map(self, basemap="SATELLITE", repeat_mode=True, out_dir=None, **kwargs):
+        """Show the interactive map.
+
+        Args:
+            basemap (str, optional): The basemap. It can be one of the following: SATELLITE, ROADMAP, TERRAIN, HYBRID.
+            repeat_mode (bool, optional): Whether to use the repeat mode for draw control. Defaults to True.
+            out_dir (str, optional): The path to the output directory. Defaults to None.
+
+        Returns:
+            leafmap.Map: The map object.
+        """
         return sam_map_gui(
             self, basemap=basemap, repeat_mode=repeat_mode, out_dir=out_dir, **kwargs
         )
 
+    def show_canvas(self, fg_color=(0, 255, 0), bg_color=(0, 0, 255), radius=5):
+        """Show a canvas to collect foreground and background points.
+
+        Args:
+            image (str | np.ndarray): The input image.
+            fg_color (tuple, optional): The color for the foreground points. Defaults to (0, 255, 0).
+            bg_color (tuple, optional): The color for the background points. Defaults to (0, 0, 255).
+            radius (int, optional): The radius of the points. Defaults to 5.
+
+        Returns:
+            tuple: A tuple of two lists of foreground and background points.
+        """
+
+        if self.image is None:
+            raise ValueError("Please run set_image() first.")
+
+        image = self.image
+        fg_points, bg_points = show_canvas(image, fg_color, bg_color, radius)
+        self.fg_points = fg_points
+        self.bg_points = bg_points
+        point_coords = fg_points + bg_points
+        point_labels = [1] * len(fg_points) + [0] * len(bg_points)
+        self.point_coords = point_coords
+        self.point_labels = point_labels
+
+    def clear_cuda_cache(self):
+        """Clear the CUDA cache."""
+        if torch.cuda.is_available():
+            torch.cuda.empty_cache()
+
     def image_to_image(self, image, **kwargs):
         return image_to_image(image, self, **kwargs)
 
     def download_tms_as_tiff(self, source, pt1, pt2, zoom, dist):
         image = draw_tile(source, pt1[0], pt1[1], pt2[0], pt2[1], zoom, dist)
         return image
```

### Comparing `segment-geospatial-0.6.2/segment_geospatial.egg-info/PKG-INFO` & `segment-geospatial-0.7.0/segment_geospatial.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: segment-geospatial
-Version: 0.6.2
+Version: 0.7.0
 Summary: Meta AI' Segment Anything Model (SAM) for Geospatial Data
 Home-page: https://github.com/opengeos/segment-geospatial
 Author: Qiusheng Wu
 Author-email: giswqs@gmail.com
 License: MIT license
 Keywords: samgeo
 Classifier: Intended Audience :: Developers
@@ -49,14 +49,15 @@
 -   Visualize segmentation results on interactive maps
 
 ## Examples
 
 -   [Segmenting satellite imagery](https://samgeo.gishub.org/examples/satellite)
 -   [Automatically generating object masks](https://samgeo.gishub.org/examples/automatic_mask_generator)
 -   [Segmenting satellite imagery with input prompts](https://samgeo.gishub.org/examples/input_prompts)
+-   [Using segment-geospatial with ArcGIS Pro](https://samgeo.gishub.org/examples/input_prompts)
 
 ## Demos
 
 -   Automatic mask generator
 
 ![](https://i.imgur.com/I1IhDgz.gif)
```

### Comparing `segment-geospatial-0.6.2/setup.py` & `segment-geospatial-0.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,10 +53,10 @@
     keywords="samgeo",
     name="segment-geospatial",
     packages=find_packages(include=["samgeo", "samgeo.*"]),
     setup_requires=setup_requirements,
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/opengeos/segment-geospatial",
-    version='0.6.2',
+    version='0.7.0',
     zip_safe=False,
 )
```

