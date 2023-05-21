# Comparing `tmp/lifx_cli-2.5.1.tar.gz` & `tmp/lifx_cli-2.5.2.tar.gz`

## Comparing `lifx_cli-2.5.1.tar` & `lifx_cli-2.5.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 lifx_cli-2.5.1/requirements.txt
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 lifx_cli-2.5.1/.github/workflows/pylint.yml
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 lifx_cli-2.5.1/.github/workflows/pytest.yml
--rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 lifx_cli-2.5.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 lifx_cli-2.5.1/src/lifx/__init__.py
--rwxr-xr-x   0        0        0     2098 2020-02-02 00:00:00.000000 lifx_cli-2.5.1/src/lifx/auth.py
--rwxr-xr-x   0        0        0     1930 2020-02-02 00:00:00.000000 lifx_cli-2.5.1/src/lifx/colors.py
--rw-r--r--   0        0        0     3196 2020-02-02 00:00:00.000000 lifx_cli-2.5.1/src/lifx/effects.py
--rwxr-xr-x   0        0        0    12261 2020-02-02 00:00:00.000000 lifx_cli-2.5.1/src/lifx/lifx.py
--rwxr-xr-x   0        0        0     3149 2020-02-02 00:00:00.000000 lifx_cli-2.5.1/src/lifx/lights.py
--rwxr-xr-x   0        0        0     1337 2020-02-02 00:00:00.000000 lifx_cli-2.5.1/src/lifx/scenes.py
--rwxr-xr-x   0        0        0     1261 2020-02-02 00:00:00.000000 lifx_cli-2.5.1/tests/lifx_cli_test.py
--rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 lifx_cli-2.5.1/tests/requirements.txt
--rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 lifx_cli-2.5.1/.gitignore
--rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 lifx_cli-2.5.1/LICENSE
--rw-r--r--   0        0        0     1831 2020-02-02 00:00:00.000000 lifx_cli-2.5.1/README.md
--rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 lifx_cli-2.5.1/pyproject.toml
--rw-r--r--   0        0        0     2368 2020-02-02 00:00:00.000000 lifx_cli-2.5.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1519 2020-02-02 00:00:00.000000 lifx_cli-2.5.2/increment_version.sh
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 lifx_cli-2.5.2/requirements.txt
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 lifx_cli-2.5.2/.github/workflows/pylint.yml
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 lifx_cli-2.5.2/.github/workflows/pytest.yml
+-rw-r--r--   0        0        0     1121 2020-02-02 00:00:00.000000 lifx_cli-2.5.2/.github/workflows/python-publish.yml
+-rwxr-xr-x   0        0        0     2098 2020-02-02 00:00:00.000000 lifx_cli-2.5.2/src/lifx/auth.py
+-rwxr-xr-x   0        0        0     1930 2020-02-02 00:00:00.000000 lifx_cli-2.5.2/src/lifx/colors.py
+-rw-r--r--   0        0        0     3196 2020-02-02 00:00:00.000000 lifx_cli-2.5.2/src/lifx/effects.py
+-rwxr-xr-x   0        0        0    12579 2020-02-02 00:00:00.000000 lifx_cli-2.5.2/src/lifx/lifx.py
+-rwxr-xr-x   0        0        0     3149 2020-02-02 00:00:00.000000 lifx_cli-2.5.2/src/lifx/lights.py
+-rwxr-xr-x   0        0        0     1337 2020-02-02 00:00:00.000000 lifx_cli-2.5.2/src/lifx/scenes.py
+-rwxr-xr-x   0        0        0     1262 2020-02-02 00:00:00.000000 lifx_cli-2.5.2/tests/lifx_cli_test.py
+-rw-r--r--   0        0        0        7 2020-02-02 00:00:00.000000 lifx_cli-2.5.2/tests/requirements.txt
+-rw-r--r--   0        0        0     3085 2020-02-02 00:00:00.000000 lifx_cli-2.5.2/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 lifx_cli-2.5.2/LICENSE
+-rw-r--r--   0        0        0     1830 2020-02-02 00:00:00.000000 lifx_cli-2.5.2/README.md
+-rw-r--r--   0        0        0      637 2020-02-02 00:00:00.000000 lifx_cli-2.5.2/pyproject.toml
+-rw-r--r--   0        0        0     2367 2020-02-02 00:00:00.000000 lifx_cli-2.5.2/PKG-INFO
```

### Comparing `lifx_cli-2.5.1/.github/workflows/pylint.yml` & `lifx_cli-2.5.2/.github/workflows/pylint.yml`

 * *Files 9% similar despite different names*

```diff
@@ -15,11 +15,12 @@
       with:
         python-version: ${{ matrix.python-version }}
     - name: Install dependencies
       run: |
         python -m pip install --upgrade pip
         pip install pylint
         pip install -r requirements.txt
+        pip install -r tests/requirements.txt
         pip install -e .
     - name: Analysing the code with pylint
       run: |
         pylint $(git ls-files '*.py') --fail-under=9.50
```

### Comparing `lifx_cli-2.5.1/.github/workflows/pytest.yml` & `lifx_cli-2.5.2/.github/workflows/pytest.yml`

 * *Files identical despite different names*

### Comparing `lifx_cli-2.5.1/.github/workflows/python-publish.yml` & `lifx_cli-2.5.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `lifx_cli-2.5.1/src/lifx/auth.py` & `lifx_cli-2.5.2/src/lifx/auth.py`

 * *Files identical despite different names*

### Comparing `lifx_cli-2.5.1/src/lifx/colors.py` & `lifx_cli-2.5.2/src/lifx/colors.py`

 * *Files identical despite different names*

### Comparing `lifx_cli-2.5.1/src/lifx/effects.py` & `lifx_cli-2.5.2/src/lifx/effects.py`

 * *Files identical despite different names*

### Comparing `lifx_cli-2.5.1/src/lifx/lifx.py` & `lifx_cli-2.5.2/src/lifx/lifx.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 ██      ██ ███████ ██   ██      ██████ ██      ██
 ██      ██ ██       ██ ██      ██      ██      ██
 ██      ██ █████     ███       ██      ██      ██
 ██      ██ ██       ██ ██      ██      ██      ██
 ███████ ██ ██      ██   ██      ██████ ███████ ██
 
 """
+VERSION = "2.5.2"
 
 
 def colors_sub_command(args):
     """Control the actions for the 'colors' sub-command."""
     colors = Colors()
 
     if isinstance(args, list):
@@ -37,15 +38,15 @@
     if list_colors:
         colors.color_information()
 
     if provided_color:
         colors.validate_color(provided_color)
 
 
-def effects_sub_command(args=None):
+def effects_sub_command(args):
     """Control the actions for the 'effects' sub-command."""
     effects = Effects()
 
     if isinstance(args, list):
         list_effects = args[0]
         light_id = args[1]
         group = args[2]
@@ -71,15 +72,15 @@
         effects.breathe_effect(light_id, group, color)
     elif pulse:
         effects.pulse_effect(light_id, group, color)
     elif stop:
         effects.stop_effect(light_id, group)
 
 
-def lights_sub_command(args=None):
+def lights_sub_command(args):
     """Control the actions for the 'lights' sub-command."""
     light = Lights()
 
     if isinstance(args, list):
         devices = args[0]
         light_id = args[1]
         toggle = args[2]
@@ -120,15 +121,15 @@
         state_attributes = {'power': power,
                             'brightness': brightness,
                             'duration': duration,
                             'infrared': infrared}
         light.set_state(light_id, group, color, state_attributes)
 
 
-def scenes_sub_command(args=None):
+def scenes_sub_command(args):
     """Control the actions for the 'scenes' sub-command."""
     scene = Scenes()
 
     if isinstance(args, list):
         scenes = args[0]
         scene_id = args[1]
     else:
@@ -156,14 +157,19 @@
 
     # Add the arguments
     job_options.add_argument('-c',
                              '--configure',
                              default=False,
                              action='store_true',
                              help='Add your LIFX token to the local authentication file: ~/.keys')
+    job_options.add_argument('-v',
+                             '--version',
+                             default=False,
+                             action='store_true',
+                             help='Print the version and exit.')
 
     # Add the 'lights' sub-command.
     light_job_options = job_options.add_subparsers(dest='command')
     light_command = light_job_options.add_parser('lights', help='Light specific functions.')
     light_command.add_argument('-l',
                                '--list',
                                default=False,
@@ -300,14 +306,18 @@
                                default=False,
                                dest='colors',
                                action='store',
                                help='Validate a color using the LIFX API.')
 
     args = job_options.parse_args()
 
+    if args.version:
+        print(f"Version: {VERSION}")
+        sys.exit(0)
+
     # Configure authentication.
     if args.configure:
         auth.configure()
 
     # The 'colors' sub-command.
     if args.command == 'colors':
         colors_sub_command(args)
```

### Comparing `lifx_cli-2.5.1/src/lifx/lights.py` & `lifx_cli-2.5.2/src/lifx/lights.py`

 * *Files identical despite different names*

### Comparing `lifx_cli-2.5.1/src/lifx/scenes.py` & `lifx_cli-2.5.2/src/lifx/scenes.py`

 * *Files identical despite different names*

### Comparing `lifx_cli-2.5.1/tests/lifx_cli_test.py` & `lifx_cli-2.5.2/tests/lifx_cli_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     src.lifx.lifx.colors_sub_command(cli_args)
     out, err = capsys.readouterr()
     assert "Saturation" in out
     assert err == ""
 
 
 def test_effects():
-    """Test the effects sub-command (lights will flash purple as Wes' home."""
+    """Test the effects sub-command (lights will flash purple as Wes' home)."""
     cli_args = [False, '917e85258fa3c3fe15816a04db6a9a15', True, ['purple'], True, False, False]
     with pytest.raises(SystemExit) as pytest_wrapped_e:
         src.lifx.lifx.effects_sub_command(cli_args)
     assert pytest_wrapped_e.type == SystemExit
     assert pytest_wrapped_e.value.code == 0
```

### Comparing `lifx_cli-2.5.1/.gitignore` & `lifx_cli-2.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `lifx_cli-2.5.1/LICENSE` & `lifx_cli-2.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `lifx_cli-2.5.1/README.md` & `lifx_cli-2.5.2/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 This is a work in progress to create a feature-rich LIFX CLI.
 
 **This project is not affiliated with or endorsed by LIFX.**
 
 ## Installation
 
 ```
-pip3 install lifx-cli
+pip install lifx-cli
 ```
 
 ## Authentication
 
 Authentication is done using your token stored in `~/.keys`. This can be configured manually or by running `lifx --configure`.
 
 **Example `~/.keys` *ini* file:**
```

### Comparing `lifx_cli-2.5.1/pyproject.toml` & `lifx_cli-2.5.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "lifx-cli"
-version = "2.5.1"
+version = "2.5.2"
 authors = [{name="Wes Henderson", email="info@necrux.com"}]
 description = "The Unofficial LIFX CLI"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
   'requests',
   'tabulate',
```

### Comparing `lifx_cli-2.5.1/PKG-INFO` & `lifx_cli-2.5.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lifx-cli
-Version: 2.5.1
+Version: 2.5.2
 Summary: The Unofficial LIFX CLI
 Project-URL: Homepage, https://github.com/necrux/lifx-cli
 Project-URL: Bug Tracker, https://github.com/necrux/lifx-cli/issues
 Author-email: Wes Henderson <info@necrux.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -19,15 +19,15 @@
 This is a work in progress to create a feature-rich LIFX CLI.
 
 **This project is not affiliated with or endorsed by LIFX.**
 
 ## Installation
 
 ```
-pip3 install lifx-cli
+pip install lifx-cli
 ```
 
 ## Authentication
 
 Authentication is done using your token stored in `~/.keys`. This can be configured manually or by running `lifx --configure`.
 
 **Example `~/.keys` *ini* file:**
```

