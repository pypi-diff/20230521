# Comparing `tmp/toui-2.2.0.tar.gz` & `tmp/toui-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toui-2.2.0.tar", last modified: Fri May 19 13:00:16 2023, max compression
+gzip compressed data, was "toui-2.3.0.tar", last modified: Sun May 21 08:43:28 2023, max compression
```

## Comparing `toui-2.2.0.tar` & `toui-2.3.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-05-19 13:00:16.673609 toui-2.2.0/
--rw-rw-rw-   0        0        0     1094 2023-05-04 15:56:54.000000 toui-2.2.0/LICENSE
--rw-rw-rw-   0        0        0       16 2023-05-04 15:56:54.000000 toui-2.2.0/MANIFEST.in
--rw-rw-rw-   0        0        0     2994 2023-05-19 13:00:16.672291 toui-2.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     2621 2023-05-15 13:27:02.000000 toui-2.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-19 13:00:16.487424 toui-2.2.0/examples/
--rw-rw-rw-   0        0        0        0 2023-05-04 15:56:54.000000 toui-2.2.0/examples/__init__.py
--rw-rw-rw-   0        0        0      910 2023-05-04 15:56:54.000000 toui-2.2.0/examples/advanced_example_1_toui_blueprint.py
--rw-rw-rw-   0        0        0      556 2023-05-04 15:56:54.000000 toui-2.2.0/examples/example_1_simple_website.py
--rw-rw-rw-   0        0        0      535 2023-05-04 15:56:54.000000 toui-2.2.0/examples/example_2_simple_desktop_app.py
--rw-rw-rw-   0        0        0      762 2023-05-04 15:56:54.000000 toui-2.2.0/examples/example_3_updating_page.py
--rw-rw-rw-   0        0        0      699 2023-05-04 15:56:54.000000 toui-2.2.0/examples/example_4_function_with_arg.py
--rw-rw-rw-   0        0        0      995 2023-05-04 15:56:54.000000 toui-2.2.0/examples/example_5_user_variables.py
--rw-rw-rw-   0        0        0      162 2023-05-04 15:56:54.000000 toui-2.2.0/examples/example_6_quick_website.py
--rw-rw-rw-   0        0        0      166 2023-05-04 15:56:54.000000 toui-2.2.0/examples/example_7_quick_desktop_app.py
-drwxrwxrwx   0        0        0        0 2023-05-19 13:00:16.494627 toui-2.2.0/images/
--rw-rw-rw-   0        0        0    29049 2023-05-04 15:56:54.000000 toui-2.2.0/images/logo.png
--rw-rw-rw-   0        0        0       42 2023-05-19 13:00:16.674605 toui-2.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1637 2023-05-19 12:59:06.000000 toui-2.2.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-19 13:00:16.660330 toui-2.2.0/toui/
--rw-rw-rw-   0        0        0      266 2023-05-19 12:56:31.000000 toui-2.2.0/toui/__init__.py
--rw-rw-rw-   0        0        0      431 2023-05-04 15:56:54.000000 toui-2.2.0/toui/_defaults.py
--rw-rw-rw-   0        0        0     1272 2023-05-15 13:04:45.000000 toui-2.2.0/toui/_helpers.py
--rw-rw-rw-   0        0        0    10419 2023-05-19 12:50:07.000000 toui-2.2.0/toui/_javascript_templates.py
--rw-rw-rw-   0        0        0     6450 2023-05-15 13:04:45.000000 toui-2.2.0/toui/_signals.py
--rw-rw-rw-   0        0        0    27251 2023-05-17 05:39:09.000000 toui-2.2.0/toui/apps.py
--rw-rw-rw-   0        0        0    21033 2023-05-19 12:54:37.000000 toui-2.2.0/toui/elements.py
--rw-rw-rw-   0        0        0      316 2023-05-15 13:04:45.000000 toui-2.2.0/toui/exceptions.py
--rw-rw-rw-   0        0        0    17082 2023-05-15 13:04:45.000000 toui-2.2.0/toui/pages.py
--rw-rw-rw-   0        0        0     2350 2023-05-04 15:56:54.000000 toui-2.2.0/toui/structure.py
-drwxrwxrwx   0        0        0        0 2023-05-19 13:00:16.671280 toui-2.2.0/toui.egg-info/
--rw-rw-rw-   0        0        0     2994 2023-05-19 13:00:16.000000 toui-2.2.0/toui.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      707 2023-05-19 13:00:16.000000 toui-2.2.0/toui.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-19 13:00:16.000000 toui-2.2.0/toui.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      196 2023-05-19 13:00:16.000000 toui-2.2.0/toui.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-19 13:00:16.000000 toui-2.2.0/toui.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-21 08:43:28.377112 toui-2.3.0/
+-rw-rw-rw-   0        0        0     1094 2023-05-04 15:56:54.000000 toui-2.3.0/LICENSE
+-rw-rw-rw-   0        0        0       16 2023-05-04 15:56:54.000000 toui-2.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     2994 2023-05-21 08:43:28.377112 toui-2.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2621 2023-05-15 13:27:02.000000 toui-2.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-21 08:43:27.926295 toui-2.3.0/examples/
+-rw-rw-rw-   0        0        0        0 2023-05-04 15:56:54.000000 toui-2.3.0/examples/__init__.py
+-rw-rw-rw-   0        0        0      910 2023-05-04 15:56:54.000000 toui-2.3.0/examples/advanced_example_1_toui_blueprint.py
+-rw-rw-rw-   0        0        0      556 2023-05-04 15:56:54.000000 toui-2.3.0/examples/example_1_simple_website.py
+-rw-rw-rw-   0        0        0      535 2023-05-04 15:56:54.000000 toui-2.3.0/examples/example_2_simple_desktop_app.py
+-rw-rw-rw-   0        0        0      762 2023-05-04 15:56:54.000000 toui-2.3.0/examples/example_3_updating_page.py
+-rw-rw-rw-   0        0        0      699 2023-05-04 15:56:54.000000 toui-2.3.0/examples/example_4_function_with_arg.py
+-rw-rw-rw-   0        0        0      995 2023-05-04 15:56:54.000000 toui-2.3.0/examples/example_5_user_variables.py
+-rw-rw-rw-   0        0        0      162 2023-05-04 15:56:54.000000 toui-2.3.0/examples/example_6_quick_website.py
+-rw-rw-rw-   0        0        0      166 2023-05-04 15:56:54.000000 toui-2.3.0/examples/example_7_quick_desktop_app.py
+drwxrwxrwx   0        0        0        0 2023-05-21 08:43:27.942813 toui-2.3.0/images/
+-rw-rw-rw-   0        0        0    29049 2023-05-04 15:56:54.000000 toui-2.3.0/images/logo.png
+-rw-rw-rw-   0        0        0       42 2023-05-21 08:43:28.377112 toui-2.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1635 2023-05-21 08:35:49.000000 toui-2.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-21 08:43:28.345535 toui-2.3.0/toui/
+-rw-rw-rw-   0        0        0      266 2023-05-21 08:35:19.000000 toui-2.3.0/toui/__init__.py
+-rw-rw-rw-   0        0        0      431 2023-05-04 15:56:54.000000 toui-2.3.0/toui/_defaults.py
+-rw-rw-rw-   0        0        0     1272 2023-05-15 13:04:45.000000 toui-2.3.0/toui/_helpers.py
+-rw-rw-rw-   0        0        0    10987 2023-05-21 08:30:10.000000 toui-2.3.0/toui/_javascript_templates.py
+-rw-rw-rw-   0        0        0     6450 2023-05-15 13:04:45.000000 toui-2.3.0/toui/_signals.py
+-rw-rw-rw-   0        0        0    27737 2023-05-21 08:22:11.000000 toui-2.3.0/toui/apps.py
+-rw-rw-rw-   0        0        0    21814 2023-05-21 08:07:45.000000 toui-2.3.0/toui/elements.py
+-rw-rw-rw-   0        0        0      316 2023-05-15 13:04:45.000000 toui-2.3.0/toui/exceptions.py
+-rw-rw-rw-   0        0        0    18018 2023-05-21 08:27:48.000000 toui-2.3.0/toui/pages.py
+-rw-rw-rw-   0        0        0     2350 2023-05-04 15:56:54.000000 toui-2.3.0/toui/structure.py
+drwxrwxrwx   0        0        0        0 2023-05-21 08:43:28.369948 toui-2.3.0/toui.egg-info/
+-rw-rw-rw-   0        0        0     2994 2023-05-21 08:43:27.000000 toui-2.3.0/toui.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      707 2023-05-21 08:43:27.000000 toui-2.3.0/toui.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-21 08:43:27.000000 toui-2.3.0/toui.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      196 2023-05-21 08:43:27.000000 toui-2.3.0/toui.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-21 08:43:27.000000 toui-2.3.0/toui.egg-info/top_level.txt
```

### Comparing `toui-2.2.0/LICENSE` & `toui-2.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `toui-2.2.0/PKG-INFO` & `toui-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toui
-Version: 2.2.0
+Version: 2.3.0
 Summary: Creates user interfaces (websites and desktop apps) from HTML easily
 Author: Mubarak Almehairbi
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `toui-2.2.0/README.md` & `toui-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `toui-2.2.0/examples/advanced_example_1_toui_blueprint.py` & `toui-2.3.0/examples/advanced_example_1_toui_blueprint.py`

 * *Files identical despite different names*

### Comparing `toui-2.2.0/examples/example_1_simple_website.py` & `toui-2.3.0/examples/example_1_simple_website.py`

 * *Files identical despite different names*

### Comparing `toui-2.2.0/examples/example_2_simple_desktop_app.py` & `toui-2.3.0/examples/example_2_simple_desktop_app.py`

 * *Files identical despite different names*

### Comparing `toui-2.2.0/examples/example_3_updating_page.py` & `toui-2.3.0/examples/example_3_updating_page.py`

 * *Files identical despite different names*

### Comparing `toui-2.2.0/examples/example_4_function_with_arg.py` & `toui-2.3.0/examples/example_4_function_with_arg.py`

 * *Files identical despite different names*

### Comparing `toui-2.2.0/examples/example_5_user_variables.py` & `toui-2.3.0/examples/example_5_user_variables.py`

 * *Files identical despite different names*

### Comparing `toui-2.2.0/images/logo.png` & `toui-2.3.0/images/logo.png`

 * *Files identical despite different names*

### Comparing `toui-2.2.0/setup.py` & `toui-2.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 with open("README.md", "r") as file:
     long_description = file.read()
 
 small = False
 if "--small" in sys.argv:
     small = True
-    sys.argv.remove('--small')  
+    sys.argv.remove('--small')
 
 name = "ToUI"
 version = __version__
 author = "Mubarak Almehairbi"
 description = "Creates user interfaces (websites and desktop apps) from HTML easily"
 package_name = "toui"
 requirements = []
```

### Comparing `toui-2.2.0/toui/_helpers.py` & `toui-2.3.0/toui/_helpers.py`

 * *Files identical despite different names*

### Comparing `toui-2.2.0/toui/_javascript_templates.py` & `toui-2.3.0/toui/_javascript_templates.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,17 +15,28 @@
 _touiFiles = {}
 _pywebviewIsLoaded = false
 async function _toPy(...args) {
     var func = args.shift()
     if (_appType === "DesktopApp" && _pywebviewIsLoaded == false) {
         await _waitForPywebview()
     }
+
+    var selector_to_element = false
+    for (var i = 0; i < args.length; i++) {
+        if (args[i] instanceof HTMLElement) {
+            args[i] = {type: "element",
+                       selector: _getElementSelector(args[i])}
+            selector_to_element = true
+        }
+    }
+
     var json = {type: "page",
                 func: func,
                 args: args,
+                "selector-to-element": selector_to_element,
                 url: urlPath}
     _manageProperties()
     json['html'] = _getDoc()
     json['uid'] = await _getUid()
     var jsonstring = JSON.stringify(json)
     if (socket.readyState === 0) {
         socket.onopen = async function() {
@@ -83,14 +94,19 @@
         if (input_element.checked == true) {
             input_element.setAttribute("checked", "")
         } else {
             input_element.removeAttribute("checked")
         }
     }
 
+    var textarea_elements = document.getElementsByTagName("textarea")
+    for (var textarea_element of textarea_elements) {
+        textarea_element.setAttribute("value", textarea_element.value)
+        }
+
     var select_elements = document.getElementsByTagName("select")
     for (var select_element of select_elements) {
         select_element.setAttribute("value", select_element.value)
         for (var i = 0; i < select_element.options.length; i++) {
             option = select_element.options[i]
             if (i == select_element.selectedIndex) {
                 option.setAttribute("selected", "")
```

### Comparing `toui-2.2.0/toui/_signals.py` & `toui-2.3.0/toui/_signals.py`

 * *Files identical despite different names*

### Comparing `toui-2.2.0/toui/apps.py` & `toui-2.3.0/toui/apps.py`

 * *Files 1% similar despite different names*

```diff
@@ -590,20 +590,30 @@
             new_html = data_dict['html']
             new_page = Page(url=url)
             new_page.from_str(new_html)
             new_page._app = self
             new_page._signal_mode = True
             new_page._ws = ws
             new_page._inherit_functions()
+            selector_to_element = data_dict['selector-to-element']
+            if selector_to_element:
+                for index, arg in enumerate(args):
+                    if type(arg) is dict:
+                        if arg.get('type') == "element":
+                            args[index] = new_page.get_element_from_selector(arg['selector'])
             if "uid" in data_dict:
                 new_page._uid = data_dict['uid']
             session['user page'] = new_page
-            if new_page._func_exists(func):
-                new_page._call_func(func, *args)
-            del session['user page']
+            try:
+                if new_page._func_exists(func):
+                    new_page._call_func(func, *args)
+                del session['user page']
+            except Exception as e:
+                del session['user page']
+                raise e
             e = time.time()
             debug(f"TIME: {e - s}s")
 
     def _confirm_user_database_created(self):
         if self._user_cls is None:
             raise ToUINotAddedError("You have not created the user database yet. To create it, call the method: `add_user_database`.")
```

### Comparing `toui-2.2.0/toui/elements.py` & `toui-2.3.0/toui/elements.py`

 * *Files 2% similar despite different names*

```diff
@@ -263,14 +263,29 @@
             element._parent_element = self
             element._selector = {"selector": selector_to_str(tag_name=tag_name, class_name=class_name,
                                                              name=name, attrs=attrs),
                                  "number": tag_num,
                                  "parent": self._selector}
             elements_list.append(element)
         return elements_list
+    
+    def get_selector(self) -> str:
+        """
+        Gets the CSS selector of an element.
+
+        Returns
+        -------
+        str
+
+        None:
+            If the element is not part of a page.
+
+        """
+        selector = self._element.name + ''.join([f'[{attr}="{value}"]' for attr, value in self._element.attrs.items()])
+        return selector
 
     def get_attr(self, name):
         """
         Gets the value of an HTML element attribute.
 
         Parameters
         ----------
@@ -589,15 +604,15 @@
         if type(content) is Element:
             for func in content._functions.values():
                 if self._parent_page:
                     self._parent_page.add_function(func)
                 else:
                     self._functions[func.__name__] = func
 
-    def on(self, event, func_or_name, *func_args, quotes=True):
+    def on(self, event, func_or_name, *func_args, quotes=True, return_itself=False):
         """
         Creates an HTML event attribute and adds a Python function to it.
 
         If you want to add JavaScript code instead of a single function, use `Element.set_attr` method
         instead.
 
         Parameters
@@ -617,14 +632,17 @@
         func_args
             The arguments of the function. Each argument will be automatically converted to a
             string.
 
         quotes: bool, default = True
             If ``True``, each argument will be surrounded by double quotes.
 
+        return_itsef: bool, default=False
+            If ``True``, the first argument of the function will be the element itself.
+
         Examples
         --------
 
         Adding a function to a button:
 
         >>> def printValueType(value):
         ...     value_type = type(value)
@@ -651,26 +669,28 @@
         >>> #<class 'int'>
 
         """
         if quotes:
             args = ",".join([f'"{arg}"' for arg in func_args])
         else:
             args = ",".join([f'{obj_converter(arg)}' for arg in func_args])
+        if return_itself:
+            args = "this, " + args
         if callable(func_or_name):
             name = func_or_name.__name__
             if self._parent_page:
                 self._parent_page.add_function(func_or_name)
             else:
                 self._functions[func_or_name.__name__] = func_or_name
         else:
             name = func_or_name
         value = f"{name}({args})"
         self.set_attr(name=f"on{event}", value=value)
 
-    def onclick(self, func_or_name, *func_args, quotes=True):
+    def onclick(self, func_or_name, *func_args, quotes=True, return_itself=False):
         """
         Creates the HTML event attribute ``onclick`` and adds a Python function to it.
 
         If you want to add JavaScript code instead of a single function, use `Element.set_attr` method
         instead.
 
         Parameters
@@ -686,20 +706,23 @@
         func_args
             The arguments of the function. Each argument will be automatically converted to a
             string.
 
         quotes: bool, default = True
             If ``True``, each argument will be surrounded by double quotes.
 
+        return_itsef: bool, default=False
+            If ``True``, the first argument of the function will be the element itself.
+
         See Also
         --------
         Element.on
 
         """
-        self.on('click', func_or_name, *func_args, quotes=quotes)
+        self.on('click', func_or_name, *func_args, quotes=quotes, return_itself=return_itself)
 
     def _from_bs4_tag_no_copy(self, bs4_tag):
         self._element = bs4_tag
 
 
 class IFrameElement(Element):
     """
```

### Comparing `toui-2.2.0/toui/pages.py` & `toui-2.3.0/toui/pages.py`

 * *Files 2% similar despite different names*

```diff
@@ -334,14 +334,45 @@
             element._parent_page = self
             element._signal_mode = self._signal_mode
             element._selector = {"selector": selector_to_str(tag_name=tag_name, class_name=class_name,
                                                              name=name, attrs=attrs),
                                  "number": tag_num}
             elements_list.append(element)
         return elements_list
+    
+    def get_element_from_selector(self, selector, do_copy=False):
+        """
+        Gets an element from its CSS selector.
+
+        Parameters
+        ----------
+        selector: str
+
+        do_copy: bool, default = False
+            If ``True``, the element will be copied.
+
+        Returns
+        -------
+        element: Element
+            If the element was found, an `Element` object will be returned. Otherwise ``None``
+            will be returned.
+
+        """
+        bs4_tag = self._html.select_one(selector=selector)
+        if bs4_tag is None:
+            return None
+        element = Element()
+        if do_copy:
+            element.from_bs4_tag(bs4_tag)
+        else:
+            element._from_bs4_tag_no_copy(bs4_tag)
+        element._parent_page = self
+        element._signal_mode = self._signal_mode
+        element._selector = {"selector": selector}
+        return element
 
     def get_html_element(self) -> Element:
         """
         Gets the first ``<html>`` element.
 
         Returns
         -------
```

### Comparing `toui-2.2.0/toui/structure.py` & `toui-2.3.0/toui/structure.py`

 * *Files identical despite different names*

### Comparing `toui-2.2.0/toui.egg-info/PKG-INFO` & `toui-2.3.0/toui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: toui
-Version: 2.2.0
+Version: 2.3.0
 Summary: Creates user interfaces (websites and desktop apps) from HTML easily
 Author: Mubarak Almehairbi
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `toui-2.2.0/toui.egg-info/SOURCES.txt` & `toui-2.3.0/toui.egg-info/SOURCES.txt`

 * *Files identical despite different names*

