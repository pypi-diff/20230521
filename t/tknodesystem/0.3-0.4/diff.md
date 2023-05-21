# Comparing `tmp/tknodesystem-0.3.tar.gz` & `tmp/tknodesystem-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tknodesystem-0.3.tar", last modified: Sat May 20 07:42:12 2023, max compression
+gzip compressed data, was "tknodesystem-0.4.tar", last modified: Sun May 21 13:36:59 2023, max compression
```

## Comparing `tknodesystem-0.3.tar` & `tknodesystem-0.4.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 07:42:12.262125 tknodesystem-0.3/
--rw-rw-rw-   0        0        0     1086 2023-05-17 15:31:54.000000 tknodesystem-0.3/LICENSE
--rw-rw-rw-   0        0        0     2621 2023-05-20 07:42:12.262125 tknodesystem-0.3/PKG-INFO
--rw-rw-rw-   0        0        0     2069 2023-05-20 06:28:49.000000 tknodesystem-0.3/README.md
--rw-rw-rw-   0        0        0      570 2023-05-20 07:42:12.262125 tknodesystem-0.3/setup.cfg
--rw-rw-rw-   0        0        0     1173 2023-05-20 07:41:50.000000 tknodesystem-0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-20 07:42:12.246496 tknodesystem-0.3/tknodesystem/
--rw-rw-rw-   0        0        0      278 2023-05-20 07:41:30.000000 tknodesystem-0.3/tknodesystem/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-20 07:42:12.262125 tknodesystem-0.3/tknodesystem/grid_images/
--rw-rw-rw-   0        0        0    58394 2023-05-12 09:24:10.000000 tknodesystem-0.3/tknodesystem/grid_images/grid_dot.png
--rw-rw-rw-   0        0        0    25170 2023-05-10 10:57:06.000000 tknodesystem-0.3/tknodesystem/grid_images/grid_lines.png
--rw-rw-rw-   0        0        0     9365 2023-05-12 08:37:01.000000 tknodesystem-0.3/tknodesystem/grid_images/no_grid.png
--rw-rw-rw-   0        0        0     4693 2023-05-20 06:06:47.000000 tknodesystem-0.3/tknodesystem/node.py
--rw-rw-rw-   0        0        0     3074 2023-05-15 11:25:51.000000 tknodesystem-0.3/tknodesystem/node_args.py
--rw-rw-rw-   0        0        0    11797 2023-05-19 11:52:04.000000 tknodesystem-0.3/tknodesystem/node_canvas.py
--rw-rw-rw-   0        0        0     9357 2023-05-20 07:37:26.000000 tknodesystem-0.3/tknodesystem/node_menu.py
--rw-rw-rw-   0        0        0     4549 2023-05-17 06:00:55.000000 tknodesystem-0.3/tknodesystem/node_socket.py
--rw-rw-rw-   0        0        0    31498 2023-05-20 06:34:42.000000 tknodesystem-0.3/tknodesystem/node_types.py
--rw-rw-rw-   0        0        0     4340 2023-05-20 06:06:53.000000 tknodesystem-0.3/tknodesystem/node_wire.py
-drwxrwxrwx   0        0        0        0 2023-05-20 07:42:12.262125 tknodesystem-0.3/tknodesystem.egg-info/
--rw-rw-rw-   0        0        0     2621 2023-05-20 07:42:12.000000 tknodesystem-0.3/tknodesystem.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      537 2023-05-20 07:42:12.000000 tknodesystem-0.3/tknodesystem.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0       40 2023-05-20 07:42:12.000000 tknodesystem-0.3/tknodesystem.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-05-20 07:42:12.000000 tknodesystem-0.3/tknodesystem.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-20 07:42:12.000000 tknodesystem-0.3/tknodesystem.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-21 13:36:59.105709 tknodesystem-0.4/
+-rw-rw-rw-   0        0        0     1086 2023-05-17 15:31:54.000000 tknodesystem-0.4/LICENSE
+-rw-rw-rw-   0        0        0     2621 2023-05-21 13:36:59.105709 tknodesystem-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     2069 2023-05-20 06:28:49.000000 tknodesystem-0.4/README.md
+-rw-rw-rw-   0        0        0      570 2023-05-21 13:36:59.105709 tknodesystem-0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1173 2023-05-21 13:36:37.000000 tknodesystem-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-21 13:36:59.027585 tknodesystem-0.4/tknodesystem/
+-rw-rw-rw-   0        0        0      278 2023-05-21 12:58:35.000000 tknodesystem-0.4/tknodesystem/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-21 13:36:59.090084 tknodesystem-0.4/tknodesystem/grid_images/
+-rw-rw-rw-   0        0        0    58394 2023-05-12 09:24:10.000000 tknodesystem-0.4/tknodesystem/grid_images/grid_dot.png
+-rw-rw-rw-   0        0        0    25170 2023-05-10 10:57:06.000000 tknodesystem-0.4/tknodesystem/grid_images/grid_lines.png
+-rw-rw-rw-   0        0        0     9365 2023-05-12 08:37:01.000000 tknodesystem-0.4/tknodesystem/grid_images/no_grid.png
+-rw-rw-rw-   0        0        0     4693 2023-05-20 06:06:47.000000 tknodesystem-0.4/tknodesystem/node.py
+-rw-rw-rw-   0        0        0     3096 2023-05-21 13:28:36.000000 tknodesystem-0.4/tknodesystem/node_args.py
+-rw-rw-rw-   0        0        0    11797 2023-05-19 11:52:04.000000 tknodesystem-0.4/tknodesystem/node_canvas.py
+-rw-rw-rw-   0        0        0     9357 2023-05-21 13:31:59.000000 tknodesystem-0.4/tknodesystem/node_menu.py
+-rw-rw-rw-   0        0        0     4549 2023-05-17 06:00:55.000000 tknodesystem-0.4/tknodesystem/node_socket.py
+-rw-rw-rw-   0        0        0    31644 2023-05-21 13:28:12.000000 tknodesystem-0.4/tknodesystem/node_types.py
+-rw-rw-rw-   0        0        0     4340 2023-05-20 06:06:53.000000 tknodesystem-0.4/tknodesystem/node_wire.py
+drwxrwxrwx   0        0        0        0 2023-05-21 13:36:59.058835 tknodesystem-0.4/tknodesystem.egg-info/
+-rw-rw-rw-   0        0        0     2621 2023-05-21 13:36:58.000000 tknodesystem-0.4/tknodesystem.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      537 2023-05-21 13:36:58.000000 tknodesystem-0.4/tknodesystem.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0       40 2023-05-21 13:36:58.000000 tknodesystem-0.4/tknodesystem.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-05-21 13:36:58.000000 tknodesystem-0.4/tknodesystem.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-21 13:36:58.000000 tknodesystem-0.4/tknodesystem.egg-info/top_level.txt
```

### Comparing `tknodesystem-0.3/LICENSE` & `tknodesystem-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tknodesystem-0.3/PKG-INFO` & `tknodesystem-0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tknodesystem
-Version: 0.3
+Version: 0.4
 Summary: Simple visual node system (DAG) with tkinter!
 Home-page: https://github.com/Akascape/TkNodeSystem
 Author: Akash Bora
 License: MIT
 Keywords: customtkinter,tkinter,tkinter-nodes,tknodes,tkinter-DAG,node-system,node-based-ui,tknodesystem,nodes
 Classifier: License :: OSI Approved :: MIT License 
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tknodesystem-0.3/README.md` & `tknodesystem-0.4/README.md`

 * *Files identical despite different names*

### Comparing `tknodesystem-0.3/setup.cfg` & `tknodesystem-0.4/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2074 6b6e 6f64 6573 7973 7465 6d0d   = tknodesystem.
-00000020: 0a76 6572 7369 6f6e 203d 2030 2e33 0d0a  .version = 0.3..
+00000020: 0a76 6572 7369 6f6e 203d 2030 2e34 0d0a  .version = 0.4..
 00000030: 6465 7363 7269 7074 696f 6e20 3d20 5369  description = Si
 00000040: 6d70 6c65 2056 6973 7561 6c20 4e6f 6465  mple Visual Node
 00000050: 2073 7973 7465 6d20 7769 7468 2054 6b69   system with Tki
 00000060: 6e74 6572 0d0a 6c6f 6e67 5f64 6573 6372  nter..long_descr
 00000070: 6970 7469 6f6e 203d 2066 696c 653a 2052  iption = file: R
 00000080: 4541 444d 452e 6d64 0d0a 6c6f 6e67 5f64  EADME.md..long_d
 00000090: 6573 6372 6970 7469 6f6e 5f63 6f6e 7465  escription_conte
```

### Comparing `tknodesystem-0.3/setup.py` & `tknodesystem-0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     """Opens and fetches text of long descrition file."""
     with open(path, 'r') as f:
         text = f.read()
     return text
 
 setup(
     name = 'tknodesystem',
-    version = '0.3',
+    version = '0.4',
     description = "Simple visual node system (DAG) with tkinter!",
     license = "MIT",
     readme = "README.md",
     long_description = get_long_description('README.md'),
     long_description_content_type = "text/markdown",
     author = 'Akash Bora',
     url = "https://github.com/Akascape/TkNodeSystem",
```

### Comparing `tknodesystem-0.3/tknodesystem/grid_images/grid_dot.png` & `tknodesystem-0.4/tknodesystem/grid_images/grid_dot.png`

 * *Files identical despite different names*

### Comparing `tknodesystem-0.3/tknodesystem/grid_images/grid_lines.png` & `tknodesystem-0.4/tknodesystem/grid_images/grid_lines.png`

 * *Files identical despite different names*

### Comparing `tknodesystem-0.3/tknodesystem/grid_images/no_grid.png` & `tknodesystem-0.4/tknodesystem/grid_images/no_grid.png`

 * *Files identical despite different names*

### Comparing `tknodesystem-0.3/tknodesystem/node.py` & `tknodesystem-0.4/tknodesystem/node.py`

 * *Files identical despite different names*

### Comparing `tknodesystem-0.3/tknodesystem/node_args.py` & `tknodesystem-0.4/tknodesystem/node_args.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
         return new_args
     
     def func_args(args):
         default_args = {'width': 100, 'height': 80, 'inputs': 2, 'border_color': '#37373D', 'text': None, 'socket_radius': 8,
                         'corner_radius': 25, 'border_width': 0, 'fg_color': '#37373D', 'text_color': 'white', 'font': ('', 10),
                         'highlightcolor': '#52d66c', 'hover': True, 'socket_color': 'green', 'socket_hover_color': 'grey50',
                         'x': None, 'y': None, 'multiside': False, 'output_socket_color': 'green', 'click_command': None,
-                        'socket_hover': True, 'num': None}
+                        'socket_hover': True, 'num': None, 'none_inputs': False}
 
         args.pop("canvas")
         args.pop("self")
         args.pop("__class__")
         args.pop("command")
         args.pop("x")
         args.pop("y")
```

### Comparing `tknodesystem-0.3/tknodesystem/node_canvas.py` & `tknodesystem-0.4/tknodesystem/node_canvas.py`

 * *Files identical despite different names*

### Comparing `tknodesystem-0.3/tknodesystem/node_menu.py` & `tknodesystem-0.4/tknodesystem/node_menu.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -155,17 +155,17 @@
     def place_dropdown(self, x=None, y=None):
         self.geometry('{}x{}+{}+{}'.format(self.width, self.height, x, y))
         self.fade_in()
         self.attributes('-alpha', self.alpha)
         
     def _iconify(self, x=None, y=None):
         self.focus_set()
-        self.search_entry.focus_set()
         self._deiconify()
         if self.focus_something: self.node[0].focus_set()
+        self.search_entry.focus_set()
         self.place_dropdown(x,y)
 
     def _attach_key_press(self, command):
         self.fade_out()
         self.withdraw()
         command()
```

### Comparing `tknodesystem-0.3/tknodesystem/node_socket.py` & `tknodesystem-0.4/tknodesystem/node_socket.py`

 * *Files identical despite different names*

### Comparing `tknodesystem-0.3/tknodesystem/node_types.py` & `tknodesystem-0.4/tknodesystem/node_types.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,15 +134,15 @@
                                   
         if len(kwargs)>0:
             raise ValueError("This option is not configurable:" + list(kwargs.keys())[0])
 
 class NodeOperation(Node):
     def __init__(self, canvas, width=100, height=None, inputs=2, border_color='white', text=None,
                  socket_radius=8, corner_radius=25, border_width=0, fg_color='#37373D', text_color='white', font=("",10),
-                 highlightcolor='#52d66c', hover=True, socket_color="green", socket_hover_color="grey50", x=0, y=0,
+                 highlightcolor='#52d66c', hover=True, socket_color="green", socket_hover_color="grey50", x=0, y=0, none_inputs=False,
                  multiside=False, command=None, output_socket_color="green", click_command=None, socket_hover=True, num=None):
 
         self.text = text
         self.canvas = canvas
         self.type = 'NodeOperation'
         
         if self.text is None:
@@ -186,14 +186,15 @@
         self.line2 = None
         self.line3 = None
         self.line4 = None
         self.line5 = None
         self.socket_colors = []
         self.connected_node = set()
         self.connected_node_first = None
+        self.none_values = none_inputs
         x_pos = x
         y_pos = y
             
         if type(socket_color) is list:
             self.socket_colors = socket_color
         else:
             for i in range(5):
@@ -220,14 +221,15 @@
         self.cellinput1 = None
         self.cellinput2 = None
         self.cellinput3 = None
         self.cellinput4 = None
         self.cellinput5 = None
         self.celloutput = None
         self.socket_nums = []
+        self.values_args = []
         
         self.output_ = NodeSocket(canvas, radius=socket_radius, center=(width+(width/2),height),
                                   fg_color=output_socket_color, hover_color=socket_hover_color, socket_num=num[0] if num else None,
                                   border_width=border_width, border_color=border_color, hover=socket_hover)
         self.canvas.tag_bind(self.output_.ID, '<Button-1>', self.connect_output)
         self.socket_nums.append(self.output_.socket_num)
         
@@ -420,45 +422,48 @@
     def update(self):
         """ update the output values """
         arguments = [self.cellinput1,
                      self.cellinput2,
                      self.cellinput3,
                      self.cellinput4,
                      self.cellinput5]
-        values_args = []
+        self.values_args = []
         if self.command:
             for i in arguments[0:self.inputs]:
                 if i is None:
-                    self.output_.value = None
-                    break
+                    self.values_args.append(None)
                 else:
-                    self.output_.value = 1
-                    values_args.append(i.output_.value)
-                    
-            if self.output_.value:
-                for i in values_args:
+                    self.values_args.append(i.output_.value)
+            
+            if not self.none_values:
+                for i in self.values_args:
                     if i is None:
                         self.output_.value = None
                         break
                     else:
                         self.output_.value = 1
-                        
-                if self.output_.value:
-                    self.output_.value = self.command(*values_args[0:self.inputs])
+            else:
+                self.output_.value = 1
+                
+            if self.output_.value:
+                self.output_.value = self.command(*self.values_args[0:self.inputs])
         else:
             self.output_.value = None
 
         if len(self.connected_node)>0:
             for i in self.connected_node:
                 i.update()
         
     def get(self):
         """ get the current value of node """
         return self.output_.value
     
+    def get_inputs(self):
+        return self.values_args
+    
     def destroy(self):
         if self.ID not in self.canvas.find_all(): return
         self.output_.value = None
         for i in self.id_list:
             self.canvas.delete(i)
 
         self.canvas.obj_list.remove(self)
```

### Comparing `tknodesystem-0.3/tknodesystem/node_wire.py` & `tknodesystem-0.4/tknodesystem/node_wire.py`

 * *Files identical despite different names*

### Comparing `tknodesystem-0.3/tknodesystem.egg-info/PKG-INFO` & `tknodesystem-0.4/tknodesystem.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tknodesystem
-Version: 0.3
+Version: 0.4
 Summary: Simple visual node system (DAG) with tkinter!
 Home-page: https://github.com/Akascape/TkNodeSystem
 Author: Akash Bora
 License: MIT
 Keywords: customtkinter,tkinter,tkinter-nodes,tknodes,tkinter-DAG,node-system,node-based-ui,tknodesystem,nodes
 Classifier: License :: OSI Approved :: MIT License 
 Classifier: Programming Language :: Python :: 3
```

### Comparing `tknodesystem-0.3/tknodesystem.egg-info/SOURCES.txt` & `tknodesystem-0.4/tknodesystem.egg-info/SOURCES.txt`

 * *Files identical despite different names*

