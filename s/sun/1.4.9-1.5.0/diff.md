# Comparing `tmp/sun-1.4.9.tar.gz` & `tmp/sun-1.5.0.tar.gz`

## Comparing `sun-1.4.9.tar` & `sun-1.5.0.tar`

### file list

```diff
@@ -1,59 +1,57 @@
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-02-24 12:40:44.000000 sun-1.4.9/
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-02-24 12:37:47.000000 sun-1.4.9/extra/
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-02-24 12:37:47.000000 sun-1.4.9/extra/xdg/
--rw-r--r--   0 dslackw   (1000) users      (100)      275 2023-02-24 12:37:47.000000 sun-1.4.9/extra/xdg/sun_daemon.desktop.sample
--rw-r--r--   0 dslackw   (1000) users      (100)      321 2023-02-24 12:37:47.000000 sun-1.4.9/extra/xdg/sun.desktop
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-02-24 12:37:47.000000 sun-1.4.9/extra/icon/
--rw-r--r--   0 dslackw   (1000) users      (100)     6188 2023-02-24 12:37:47.000000 sun-1.4.9/extra/icon/sun.png
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-02-24 12:37:47.000000 sun-1.4.9/extra/desktop/
--rw-r--r--   0 dslackw   (1000) users      (100)      231 2023-02-24 12:37:47.000000 sun-1.4.9/extra/desktop/sun.desktop
--rw-r--r--   0 dslackw   (1000) users      (100)    32402 2023-02-24 12:37:47.000000 sun-1.4.9/LICENSE.txt
--rw-r--r--   0 dslackw   (1000) users      (100)     5099 2023-02-24 12:37:47.000000 sun-1.4.9/CHANGES.md
--rw-r--r--   0 dslackw   (1000) users      (100)       58 2023-02-24 12:37:47.000000 sun-1.4.9/MANIFEST.in
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-02-24 12:40:41.000000 sun-1.4.9/sun/
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-02-24 12:37:47.000000 sun-1.4.9/sun/gtk/
--rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-02-24 12:37:47.000000 sun-1.4.9/sun/gtk/__init__.py
--rw-r--r--   0 dslackw   (1000) users      (100)     7628 2023-02-24 12:37:47.000000 sun-1.4.9/sun/gtk/status_icon.py
--rw-r--r--   0 dslackw   (1000) users      (100)     5452 2023-02-24 12:37:47.000000 sun-1.4.9/sun/utils.py
--rw-r--r--   0 dslackw   (1000) users      (100)     2211 2023-02-24 12:37:47.000000 sun-1.4.9/sun/daemon.py
--rw-r--r--   0 dslackw   (1000) users      (100)     1803 2023-02-24 12:37:47.000000 sun-1.4.9/sun/__metadata__.py
--rw-r--r--   0 dslackw   (1000) users      (100)     2145 2023-02-24 12:37:47.000000 sun-1.4.9/sun/licenses.py
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-02-24 12:40:41.000000 sun-1.4.9/sun/__pycache__/
--rw-r--r--   0 dslackw   (1000) users      (100)      140 2023-02-24 12:40:41.000000 sun-1.4.9/sun/__pycache__/__init__.cpython-39.pyc
--rw-r--r--   0 dslackw   (1000) users      (100)     1110 2023-02-24 12:40:41.000000 sun-1.4.9/sun/__pycache__/__metadata__.cpython-39.pyc
--rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-02-24 12:37:47.000000 sun-1.4.9/sun/__init__.py
--rw-r--r--   0 dslackw   (1000) users      (100)     2913 2023-02-24 12:37:47.000000 sun-1.4.9/sun/configs.py
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-02-24 12:37:47.000000 sun-1.4.9/sun/cli/
--rw-r--r--   0 dslackw   (1000) users      (100)     5171 2023-02-24 12:37:47.000000 sun-1.4.9/sun/cli/tool.py
--rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-02-24 12:37:47.000000 sun-1.4.9/sun/cli/__init__.py
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-02-24 12:37:47.000000 sun-1.4.9/slackbuild/
--rw-r--r--   0 dslackw   (1000) users      (100)      900 2023-02-24 12:37:47.000000 sun-1.4.9/slackbuild/slack-desc
--rw-r--r--   0 dslackw   (1000) users      (100)      515 2023-02-24 12:37:47.000000 sun-1.4.9/slackbuild/doinst.sh
--rw-r--r--   0 dslackw   (1000) users      (100)      448 2023-02-24 12:37:47.000000 sun-1.4.9/slackbuild/README
--rwxr-xr-x   0 dslackw   (1000) users      (100)     3574 2023-02-24 12:37:47.000000 sun-1.4.9/slackbuild/sun.SlackBuild
--rwxr-xr-x   0 dslackw   (1000) users      (100)     2792 2023-02-24 12:37:47.000000 sun-1.4.9/setup.py
--rw-r--r--   0 dslackw   (1000) users      (100)     3384 2023-02-24 12:37:47.000000 sun-1.4.9/README.rst
--rw-r--r--   0 dslackw   (1000) users      (100)       39 2023-02-24 12:37:47.000000 sun-1.4.9/requirements.txt
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-02-24 12:37:47.000000 sun-1.4.9/sbin/
--rwxr-xr-x   0 dslackw   (1000) users      (100)     2709 2023-02-24 12:37:47.000000 sun-1.4.9/sbin/sun_daemon
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-02-24 12:37:47.000000 sun-1.4.9/tests/
--rw-r--r--   0 dslackw   (1000) users      (100)      432 2023-02-24 12:37:47.000000 sun-1.4.9/tests/test_tools.py
--rw-r--r--   0 dslackw   (1000) users      (100)      195 2023-02-24 12:37:47.000000 sun-1.4.9/tests/test_utils.py
--rw-r--r--   0 dslackw   (1000) users      (100)      188 2023-02-24 12:37:47.000000 sun-1.4.9/tests/test_notify.py
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-02-24 12:40:41.000000 sun-1.4.9/sun.egg-info/
--rw-r--r--   0 dslackw   (1000) users      (100)        1 2023-02-24 12:40:41.000000 sun-1.4.9/sun.egg-info/dependency_links.txt
--rw-r--r--   0 dslackw   (1000) users      (100)      499 2023-02-24 12:40:41.000000 sun-1.4.9/sun.egg-info/SOURCES.txt
--rw-r--r--   0 dslackw   (1000) users      (100)       20 2023-02-24 12:40:41.000000 sun-1.4.9/sun.egg-info/top_level.txt
--rw-r--r--   0 dslackw   (1000) users      (100)       43 2023-02-24 12:40:41.000000 sun-1.4.9/sun.egg-info/requires.txt
--rw-r--r--   0 dslackw   (1000) users      (100)     4337 2023-02-24 12:40:41.000000 sun-1.4.9/sun.egg-info/PKG-INFO
--rwxr-xr-x   0 dslackw   (1000) users      (100)     1787 2023-02-24 12:37:47.000000 sun-1.4.9/install.sh
--rw-r--r--   0 dslackw   (1000) users      (100)      281 2023-02-24 12:37:47.000000 sun-1.4.9/.travis.yml
--rw-r--r--   0 dslackw   (1000) users      (100)       78 2023-02-24 12:37:47.000000 sun-1.4.9/.gitignore
--rw-r--r--   0 dslackw   (1000) users      (100)       80 2023-02-24 12:37:47.000000 sun-1.4.9/pytest.ini
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-02-24 12:37:47.000000 sun-1.4.9/conf/
--rw-r--r--   0 dslackw   (1000) users      (100)     2619 2023-02-24 12:37:47.000000 sun-1.4.9/conf/sun.toml
-drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-02-24 12:37:47.000000 sun-1.4.9/bin/
--rwxr-xr-x   0 dslackw   (1000) users      (100)     1196 2023-02-24 12:37:47.000000 sun-1.4.9/bin/sun_daemon
--rwxr-xr-x   0 dslackw   (1000) users      (100)     1135 2023-02-24 12:37:47.000000 sun-1.4.9/bin/sun
--rwxr-xr-x   0 dslackw   (1000) users      (100)     1207 2023-02-24 12:37:47.000000 sun-1.4.9/bin/sun_gtk
--rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-02-24 12:37:47.000000 sun-1.4.9/bin/__init__.py
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-21 17:29:28.000000 sun-1.5.0/
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-21 17:26:33.000000 sun-1.5.0/extra/
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-21 17:26:33.000000 sun-1.5.0/extra/xdg/
+-rw-r--r--   0 dslackw   (1000) users      (100)      275 2023-05-21 17:26:33.000000 sun-1.5.0/extra/xdg/sun_daemon.desktop.sample
+-rw-r--r--   0 dslackw   (1000) users      (100)      321 2023-05-21 17:26:33.000000 sun-1.5.0/extra/xdg/sun.desktop
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-21 17:26:33.000000 sun-1.5.0/extra/icon/
+-rw-r--r--   0 dslackw   (1000) users      (100)     6188 2023-05-21 17:26:33.000000 sun-1.5.0/extra/icon/sun.png
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-21 17:26:33.000000 sun-1.5.0/extra/desktop/
+-rw-r--r--   0 dslackw   (1000) users      (100)      231 2023-05-21 17:26:33.000000 sun-1.5.0/extra/desktop/sun.desktop
+-rw-r--r--   0 dslackw   (1000) users      (100)    32402 2023-05-21 17:26:33.000000 sun-1.5.0/LICENSE.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)     5227 2023-05-21 17:26:33.000000 sun-1.5.0/CHANGES.md
+-rw-r--r--   0 dslackw   (1000) users      (100)       58 2023-05-21 17:26:33.000000 sun-1.5.0/MANIFEST.in
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-21 17:29:22.000000 sun-1.5.0/sun/
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-21 17:26:33.000000 sun-1.5.0/sun/gtk/
+-rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-05-21 17:26:33.000000 sun-1.5.0/sun/gtk/__init__.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     7619 2023-05-21 17:26:33.000000 sun-1.5.0/sun/gtk/status_icon.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     6622 2023-05-21 17:26:33.000000 sun-1.5.0/sun/utils.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     2246 2023-05-21 17:26:33.000000 sun-1.5.0/sun/daemon.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     1853 2023-05-21 17:26:33.000000 sun-1.5.0/sun/__metadata__.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     2145 2023-05-21 17:26:33.000000 sun-1.5.0/sun/licenses.py
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-21 17:29:22.000000 sun-1.5.0/sun/__pycache__/
+-rw-r--r--   0 dslackw   (1000) users      (100)      140 2023-05-21 17:29:22.000000 sun-1.5.0/sun/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 dslackw   (1000) users      (100)     1155 2023-05-21 17:29:22.000000 sun-1.5.0/sun/__pycache__/__metadata__.cpython-39.pyc
+-rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-05-21 17:26:33.000000 sun-1.5.0/sun/__init__.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     3260 2023-05-21 17:26:33.000000 sun-1.5.0/sun/configs.py
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-21 17:26:33.000000 sun-1.5.0/sun/cli/
+-rw-r--r--   0 dslackw   (1000) users      (100)     5690 2023-05-21 17:26:33.000000 sun-1.5.0/sun/cli/tool.py
+-rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-05-21 17:26:33.000000 sun-1.5.0/sun/cli/__init__.py
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-21 17:26:33.000000 sun-1.5.0/slackbuild/
+-rw-r--r--   0 dslackw   (1000) users      (100)      900 2023-05-21 17:26:33.000000 sun-1.5.0/slackbuild/slack-desc
+-rw-r--r--   0 dslackw   (1000) users      (100)      543 2023-05-21 17:26:33.000000 sun-1.5.0/slackbuild/doinst.sh
+-rw-r--r--   0 dslackw   (1000) users      (100)      457 2023-05-21 17:26:33.000000 sun-1.5.0/slackbuild/README
+-rwxr-xr-x   0 dslackw   (1000) users      (100)     3619 2023-05-21 17:26:33.000000 sun-1.5.0/slackbuild/sun.SlackBuild
+-rwxr-xr-x   0 dslackw   (1000) users      (100)     2791 2023-05-21 17:26:33.000000 sun-1.5.0/setup.py
+-rw-r--r--   0 dslackw   (1000) users      (100)     3463 2023-05-21 17:26:33.000000 sun-1.5.0/README.rst
+-rw-r--r--   0 dslackw   (1000) users      (100)       39 2023-05-21 17:26:33.000000 sun-1.5.0/requirements.txt
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-21 17:26:33.000000 sun-1.5.0/sbin/
+-rwxr-xr-x   0 dslackw   (1000) users      (100)     2730 2023-05-21 17:26:33.000000 sun-1.5.0/sbin/sun_daemon
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-21 17:26:33.000000 sun-1.5.0/tests/
+-rw-r--r--   0 dslackw   (1000) users      (100)      596 2023-05-21 17:26:33.000000 sun-1.5.0/tests/test_tools.py
+-rw-r--r--   0 dslackw   (1000) users      (100)      853 2023-05-21 17:26:33.000000 sun-1.5.0/tests/test_utils.py
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-21 17:29:23.000000 sun-1.5.0/sun.egg-info/
+-rw-r--r--   0 dslackw   (1000) users      (100)        1 2023-05-21 17:29:23.000000 sun-1.5.0/sun.egg-info/dependency_links.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)      499 2023-05-21 17:29:23.000000 sun-1.5.0/sun.egg-info/SOURCES.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)       20 2023-05-21 17:29:23.000000 sun-1.5.0/sun.egg-info/top_level.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)       29 2023-05-21 17:29:23.000000 sun-1.5.0/sun.egg-info/requires.txt
+-rw-r--r--   0 dslackw   (1000) users      (100)     4411 2023-05-21 17:29:23.000000 sun-1.5.0/sun.egg-info/PKG-INFO
+-rwxr-xr-x   0 dslackw   (1000) users      (100)     1787 2023-05-21 17:26:33.000000 sun-1.5.0/install.sh
+-rw-r--r--   0 dslackw   (1000) users      (100)       78 2023-05-21 17:26:33.000000 sun-1.5.0/.gitignore
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-21 17:26:33.000000 sun-1.5.0/conf/
+-rw-r--r--   0 dslackw   (1000) users      (100)     1391 2023-05-21 17:26:33.000000 sun-1.5.0/conf/sun.toml
+-rw-r--r--   0 dslackw   (1000) users      (100)     1684 2023-05-21 17:26:33.000000 sun-1.5.0/conf/repositories.toml
+drwxr-xr-x   0 dslackw   (1000) users      (100)        0 2023-05-21 17:26:33.000000 sun-1.5.0/bin/
+-rwxr-xr-x   0 dslackw   (1000) users      (100)     1196 2023-05-21 17:26:33.000000 sun-1.5.0/bin/sun_daemon
+-rwxr-xr-x   0 dslackw   (1000) users      (100)     1130 2023-05-21 17:26:33.000000 sun-1.5.0/bin/sun
+-rwxr-xr-x   0 dslackw   (1000) users      (100)     1207 2023-05-21 17:26:33.000000 sun-1.5.0/bin/sun_gtk
+-rw-r--r--   0 dslackw   (1000) users      (100)        0 2023-05-21 17:26:33.000000 sun-1.5.0/bin/__init__.py
```

### Comparing `sun-1.4.9/extra/icon/sun.png` & `sun-1.5.0/extra/icon/sun.png`

 * *Files identical despite different names*

### Comparing `sun-1.4.9/LICENSE.txt` & `sun-1.5.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sun-1.4.9/CHANGES.md` & `sun-1.5.0/CHANGES.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 SUN (Slackware Update Notifier)
 ===============================
+Version 1.5.0 - (19/05/2023)
+### Fixed
+- Daemon notification message
+### Added
+- Configuration file /etc/sun/repositories.toml
+
 Version 1.4.9 - (22/02/2023)
 ### BugFixed
 - Time interval sleep
 
 - Version 1.4.8 - (22/02/2023)
 ### Updated
 - The daemon passed to the config file
```

### Comparing `sun-1.4.9/sun/gtk/status_icon.py` & `sun-1.5.0/sun/gtk/status_icon.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,27 +34,28 @@
     __email__,
     __author__,
     __version__,
     __website__,
     data_configs
 )
 
-
 from sun.utils import Utilities
 from sun.configs import Configs
 from sun.cli.tool import Tools
 
 
 class GtkStatusIcon(Configs):
 
     def __init__(self):
         super(Configs, self).__init__()
         self.data_configs: dict = data_configs
+        self.menu = None
         self.tool = Tools()
-        self.sun_icon: str = f'{self.data_configs["icon_path"]}{__all__}.png'
+
+        self.sun_icon: str = f'{self.data_configs["icon_path"]}/{__all__}.png'
         self.status_icon = Gtk.StatusIcon()
         self.status_icon.set_from_file(self.sun_icon)
         self.status_icon.connect('popup-menu', self.right_click_event)
 
     def right_click_event(self, icon, button, time):
         """ Handler menu and submenu. """
 
@@ -207,11 +208,10 @@
         title: str = 'SUN daemon'
         data: str = 'SUN daemon restarts...'
         data: str = self.tool.daemon_process('restart', data)
         self.message(data, title)
 
     def show_daemon_status(self, widget):
         """ Show message status about the daemon. """
-        daemon: str = 'sun_daemon'
         title: str = 'SUN daemon'
         data: str = ('SUN is running...' if self.tool.daemon_status() else 'SUN is not running')
         self.message(data, title)
```

### Comparing `sun-1.4.9/sun/daemon.py` & `sun-1.5.0/sun/daemon.py`

 * *Files 13% similar despite different names*

```diff
@@ -28,49 +28,48 @@
 / ___|| | | | \ | |
 \___ \| | | |  \| |
  ___) | |_| | |\  |
 |____/ \___/|_| \_|
 
 """
 
-
 import time
 import notify2
+
 from sun.cli.tool import Tools
 from sun.configs import Configs
-from sun.utils import Utilities
+from sun.utils import Fetch
 from sun.__metadata__ import __all__, data_configs
 
 
 class Notify(Configs):
     """ Main notify Class. """
 
     def __init__(self):
         super(Configs, self).__init__()
         self.tool = Tools()
-        self.utils = Utilities()
+        self.fetch = Fetch()
+
+        self.notify = None
+        self.icon = None
+        self.message: str = str()
+        self.count_packages: int = 0
+        self.title: str = f"{'':>10}Software Updates"
+        self.icon: str = f'{data_configs["icon_path"]}/{__all__}.png'
 
         notify2.uninit()
         notify2.init('sun')
 
-        self.data_configs = data_configs
-        self.count_packages: int = len(list(self.utils.fetch_updates()))
-
-        self.summary: str = f"{' ' * 10}Software Updates"
-        self.message: str = f"{' ' * 3}{self.count_packages} Software updates are available\n"
-
-        self.icon: str = f'{self.data_configs["icon_path"]}{__all__}.png'
-
-        self.n = notify2.Notification(self.summary, self.message, self.icon)
-        self.n.set_timeout(60000 * self.standby)
-
-    def show_notify(self):
-        """ Startup dbus message if packages. """
-        self.n.show()  # show notification
+    def set_notification_message(self):
+        self.count_packages: int = len(list(self.fetch.updates()))
+        self.message: str = f"{'':>3}{self.count_packages} Software updates are available\n"
+        self.notify = notify2.Notification(self.title, self.message, self.icon)
+        self.notify.set_timeout(60000 * self.standby)
 
-    def daemon(self):
+    def daemon(self) -> None:
         """ SUN daemon. """
         while True:
+            self.set_notification_message()
             if self.count_packages > 0:
-                self.show_notify()
+                self.notify.show()
 
             time.sleep(60 * self.interval)
```

### Comparing `sun-1.4.9/sun/__metadata__.py` & `sun-1.5.0/sun/__metadata__.py`

 * *Files 17% similar despite different names*

```diff
@@ -23,33 +23,34 @@
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 
 import os
 import shutil
 import platform
 import subprocess
+from pathlib import Path
 
 
 __all__: str = 'sun'
 __author__: str = 'dslackw'
 __copyright__: str = '2015-2022'
-__version_info__: tuple = (1, 4, 9)
+__version_info__: tuple = (1, 5, 0)
 __version__: str = '{0}.{1}.{2}'.format(*__version_info__)
 __license__: str = 'GNU General Public License v3 (GPLv3)'
-__email__: str = 'd.zlatanidis@gmail.com'
+__email__: str = 'dslackw@gmail.com'
 __website__: str = 'https://gitlab.com/dslackw/sun'
 
 
 data_configs: dict = {
-    'bin_path': '/usr/bin/',
-    'pkg_path': '/var/log/packages/',
-    'icon_path': '/usr/share/pixmaps/',
-    'desktop_path': '/usr/share/applications/',
-    'xdg_autostart': '/etc/xdg/autostart/',
-    'sun_conf_path': f'/etc/{__all__}/',
+    'bin_path': Path('/usr/bin/'),
+    'pkg_path': Path('/var/log/packages'),
+    'icon_path': Path('/usr/share/pixmaps'),
+    'desktop_path': Path('/usr/share/applications'),
+    'xdg_autostart': Path('/etc/xdg/autostart'),
+    'sun_conf_path': Path('/etc/', __all__),
     'arch': platform.machine(),
     'kernel': os.uname()[2],
     'cpu': platform.processor(),
     'mem': subprocess.getoutput('free -h').split(),
     'disk': shutil.disk_usage('/'),
     'uptime': subprocess.getoutput('uptime -p')
 }
```

### Comparing `sun-1.4.9/sun/licenses.py` & `sun-1.5.0/sun/licenses.py`

 * *Files identical despite different names*

### Comparing `sun-1.4.9/sun/configs.py` & `sun-1.5.0/sun/configs.py`

 * *Files 13% similar despite different names*

```diff
@@ -19,24 +19,29 @@
 # but WITHOUT ANY WARRANTY; without even the implied warranty of
 # MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE. See the
 # GNU General Public License for more details.
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 
-import os
 import tomli
-
+from pathlib import Path
 from sun.__metadata__ import data_configs, __all__
 
 
 class Configs:
 
+    # Configuration files.
     config_file: str = f'{__all__}.toml'
+    repositories_file: str = 'repositories.toml'
     config_path: str = data_configs['sun_conf_path']
+    slpkg_toml: Path = Path(config_path, config_file)
+    repositories_toml: Path = Path(config_path, repositories_file)
+    configs: dict = {}
+    repos: dict = {}
 
     # Default time configs.
     interval: int = 720
     standby: int = 3
 
     # Daemon default commands.
     sun_daemon_start: str = 'daemon -rB --pidfiles=~/.run --name=sun_daemon sun_daemon'
@@ -49,30 +54,33 @@
         {'NAME': 'Slackware',
          'HTTP_MIRROR': 'https://mirrors.slackware.com/slackware/slackware64-15.0/',
          'LOG_PATH': '/var/lib/slackpkg/', 'LOG_FILE': 'ChangeLog.txt',
          'PATTERN': 'Upgraded[.]|Rebuilt[.]|Added[.]|Removed[.]',
          'COMPARE': '^\w[Mon|Tue|Wed|Thu|Fri|Sat|Sun]'}
     ]
 
-    # Configuration file.
-    toml_file_path: str = f'{config_path}{config_file}'
+    try:
+        if slpkg_toml.is_file():
+            with open(slpkg_toml, 'rb') as conf:
+                configs: dict = tomli.load(conf)
+        else:
+            raise Exception(f"Error: Failed to find '{slpkg_toml}' file.")
 
-    try:  # Load configuration from /etc/sun/sun.toml file.
-        if os.path.isfile(toml_file_path):
-            with open(toml_file_path, 'rb') as conf:
-                configs = tomli.load(conf)
+        if repositories_toml.is_file():
+            with open(repositories_toml, 'rb') as conf:
+                repos: dict = tomli.load(conf)
         else:
-            raise Exception(f"Error: Failed to find '{toml_file_path}' file.")
+            raise Exception(f"Error: Failed to find '{repositories_toml}' file.")
 
         # Time configs.
         interval: int = configs['time']['INTERVAL']
         standby: int = configs['time']['STANDBY']
         # Daemon configs.
         sun_daemon_start: str = configs['daemon']['START']
         sun_daemon_stop: str = configs['daemon']['STOP']
         sun_daemon_restart: str = configs['daemon']['RESTART']
         sun_daemon_running: str = configs['daemon']['RUNNING']
         # Repositories configs.
-        repositories: list = configs['repository']
+        repositories: list = repos['repository']
 
     except (tomli.TOMLDecodeError, KeyError) as error:
         raise SystemExit(f"Error: {error}: in the config file '{config_path}{config_file}'.")
```

### Comparing `sun-1.4.9/sun/cli/tool.py` & `sun-1.5.0/sun/cli/tool.py`

 * *Files 13% similar despite different names*

```diff
@@ -22,126 +22,145 @@
 # You should have received a copy of the GNU General Public License
 # along with this program. If not, see <http://www.gnu.org/licenses/>.
 
 
 import sys
 import getpass
 import subprocess
-from sun.utils import Utilities
 from sun.configs import Configs
+from sun.utils import Utilities, Fetch
 from sun.__metadata__ import __version__, data_configs
 
 
 class Tools(Configs):
 
     def __init__(self):
         super(Configs, self).__init__()
         self.data_configs: dict = data_configs
         self.utils = Utilities()
+        self.fetch = Fetch()
 
     @staticmethod
-    def su():
-        """ Display message when sun execute as root. """
+    def su() -> None:
+        """ Root privileges not required. """
         if getpass.getuser() == 'root':
             raise SystemExit('sun: Error: It should not be run as root')
 
     @staticmethod
-    def usage():
-        """ SUN arguments. """
+    def usage() -> None:
+        """ Usage help menu. """
         args: str = (f'SUN (Slackware Update Notifier) - Version: {__version__}\n'
                      '\nUsage: sun [OPTIONS]\n'
                      '\nOptional arguments:\n'
                      '  help       Display this help and exit.\n'
                      '  start      Start sun daemon.\n'
                      '  stop       Stop sun daemon.\n'
                      '  restart    Restart sun daemon.\n'
                      '  check      Check for software updates.\n'
                      '  status     Sun daemon status.\n'
                      '  info       Os and machine information.\n'
                      '\nStart GTK icon from the terminal: sun start --gtk')
         print(args)
 
-    def check_updates(self):
-        """ Check and display upgraded packages. """
+    def check_updates(self) -> tuple:
+        """ Returns the count of the packages and the message. """
         message: str = 'No news is good news!'
-        packages: list = list(self.utils.fetch_updates())
+        packages: list = list(self.fetch.updates())
+        count_packages: int = len(packages)
+        count_repositories: int = len(set([repo.split(':')[0] for repo in packages]))
+        repositories_message: str = str()
 
-        count: int = len(packages)
-        count_repos = len(set([repo.split(':')[0] for repo in packages]))
+        if count_repositories > 1:
+            repositories_message: str = f'from {count_repositories} repositories'
 
-        message_repos: str = f'from {count_repos} repository'
-
-        if count_repos > 1:
-            message_repos: str = f'from {count_repos} repositories'
-
-        if count > 0:
-            message: str = f'{count} software updates are available {message_repos}\n'
+        if count_packages > 0:
+            message: str = f'{count_packages} software updates are available {repositories_message}\n'
 
         return message, packages
 
-    def print_updates(self):
-        """ Print updates for the terminal. """
+    def view_updates(self) -> None:
+        """ Prints the updates packages to the terminal. """
         message, packages = self.check_updates()
         print(message)
         if len(packages) > 0:
             [print(pkg) for pkg in packages]
 
-    def daemon_status(self):
-        """ Checks the sun_daemon running. """
+    def daemon_status(self) -> bool:
+        """ Returns the daemon status. """
         output = subprocess.run(self.sun_daemon_running, shell=True).returncode
         if output == 0:
             return True
 
-    def daemon_process(self, args, message):
-        """ Check subprocess output status. """
+    def daemon_process(self, arg: str, message: str) -> str:
+        """ Returns the daemon status message. """
         output: int = 1
 
         command: dict = {
             'start': self.sun_daemon_start,
             'stop': self.sun_daemon_stop,
             'restart': self.sun_daemon_restart
         }
 
-        if self.daemon_status() and args == 'start':
+        if self.daemon_status() and arg == 'start':
             message: str = 'SUN is already running'
-        elif not self.daemon_status() and args == 'stop':
+        elif not self.daemon_status() and arg == 'stop':
             message: str = 'SUN is not running'
-        elif not self.daemon_status() and args == 'restart':
+        elif not self.daemon_status() and arg == 'restart':
             message: str = 'SUN is not running'
         else:
-            output: int = subprocess.call(command[args], shell=True)
+            output: int = subprocess.call(command[arg], shell=True)
 
         if output > 0:
             message: str = f'FAILED [{output}]: {message}'
 
         return message
 
-    def cli(self):
-        """ The cli tool managing. """
-        self.su()
-        args: list = sys.argv
-        args.pop(0)
-
-        if len(args) == 1:
-
-            if args[0] == 'start':
-                print(self.daemon_process(args[0], 'Starting SUN daemon:  sun_daemon &'))
-            elif args[0] == 'stop':
-                print(self.daemon_process(args[0], 'Stopping SUN daemon:  sun_daemon'))
-            elif args[0] == 'restart':
-                print(self.daemon_process(args[0], 'Restarting SUN daemon:  sun_daemon'))
-            elif args[0] == 'check':
-                self.print_updates()
-            elif args[0] == 'status':
-                print('SUN is running...' if self.daemon_status() else 'SUN is not running')
-            elif args[0] == 'help':
-                self.usage()
-            elif args[0] == 'info':
-                print(self.utils.os_info())
-            else:
-                print("try: 'sun help'")
 
-        elif len(args) == 2 and args[0] == 'start' and args[1] == '--gtk':
+class Cli:
+    """ Command line control menu. """
+
+    def __init__(self):
+        self.args: list = []
+        self.tools = Tools()
+        self.utils = Utilities()
+
+    def menu(self) -> None:
+        self.tools.su()
+        self.args: list = sys.argv
+        self.args.pop(0)
+
+        process: dict = {
+            'start': self.view_start,
+            'stop': self.view_stop,
+            'restart': self.view_restart,
+            'status': self.view_status,
+            'check': self.tools.view_updates,
+            'info': self.view_info,
+            'help': self.tools.usage
+        }
+
+        if len(self.args) == 1:
+            try:
+                process[self.args[0]]()
+            except KeyError:
+                raise SystemExit("try: 'sun help'")
+
+        elif len(self.args) == 2 and self.args[0] == 'start' and self.args[1] == '--gtk':
             subprocess.call('sun_gtk &', shell=True)
 
         else:
             raise SystemExit("try: 'sun help'")
+
+    def view_start(self):
+        print(self.tools.daemon_process(self.args[0], 'Starting SUN daemon:  sun_daemon &'))
+
+    def view_stop(self):
+        print(self.tools.daemon_process(self.args[0], 'Stopping SUN daemon:  sun_daemon'))
+
+    def view_restart(self):
+        print(self.tools.daemon_process(self.args[0], 'Restarting SUN daemon:  sun_daemon'))
+
+    def view_status(self):
+        print('SUN is running...' if self.tools.daemon_status() else 'SUN is not running')
+
+    def view_info(self):
+        print(self.utils.os_info())
```

### Comparing `sun-1.4.9/slackbuild/slack-desc` & `sun-1.5.0/slackbuild/slack-desc`

 * *Files identical despite different names*

### Comparing `sun-1.4.9/slackbuild/sun.SlackBuild` & `sun-1.5.0/slackbuild/sun.SlackBuild`

 * *Files 2% similar despite different names*

```diff
@@ -72,33 +72,34 @@
 
 set -e
 
 rm -rf $PKG
 mkdir -p $TMP $PKG $OUTPUT
 cd $TMP
 rm -rf $PRGNAM-$VERSION
-tar xvf $CWD/$PRGNAM-$VERSION.tar.gz || tar xvf $CWD/v$VERSION.tar.gz \
-    || unzip $CWD/$PRGNAM-$VERSION.zip || unzip $CWD/v$VERSION.zip
+tar xvf $CWD/$PRGNAM-$VERSION.tar.gz || tar xvf $CWD/$PRGNAM-$VERSION.tar.bz2 \
+	|| unzip $CWD/$PRGNAM-$VERSION.zip
 cd $PRGNAM-$VERSION
 chown -R root:root .
 find -L . \
  \( -perm 777 -o -perm 775 -o -perm 750 -o -perm 711 -o -perm 555 \
   -o -perm 511 \) -exec chmod 755 {} \; -o \
  \( -perm 666 -o -perm 664 -o -perm 640 -o -perm 600 -o -perm 444 \
   -o -perm 440 -o -perm 400 \) -exec chmod 644 {} \;
 
 python3 setup.py install --root=$PKG
 
 # Install autostart enable-disable daemon script
 mkdir -p $PKG/usr/sbin
 cp sbin/sun_daemon $PKG/usr/sbin
 
-# Install configuration file
+# Install configuration files
 mkdir -p $PKG/etc/$PRGNAM
 install -D -m0644 conf/sun.toml $PKG/etc/sun/sun.toml.new
+install -D -m0644 conf/repositories.toml $PKG/etc/sun/sun.toml.new
 
 find $PKG -print0 | xargs -0 file | grep -e "executable" -e "shared object" | grep ELF \
   | cut -f 1 -d : | xargs strip --strip-unneeded 2> /dev/null || true
 
 mkdir -p $PKG/usr/doc/$PRGNAM-$VERSION
 cp -a README.rst CHANGES.md LICENSE.txt $PKG/usr/doc/$PRGNAM-$VERSION
 cat $CWD/$PRGNAM.SlackBuild > $PKG/usr/doc/$PRGNAM-$VERSION/$PRGNAM.SlackBuild
```

### Comparing `sun-1.4.9/setup.py` & `sun-1.5.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -29,17 +29,15 @@
     __all__, __version__,
     __email__, __author__,
     data_configs
 )
 
 INSTALLATION_REQUIREMENTS = []
 DOCS_REQUIREMENTS = []
-TESTS_REQUIREMENTS = [
-    'pytest>=5.3.2'
-]
+TESTS_REQUIREMENTS = []
 OPTIONAL_REQUIREMENTS = []
 
 
 setup(
     name=__all__,
     packages=['sun', 'sun/gtk', 'sun/cli'],
     scripts=['bin/sun_daemon', 'bin/sun', 'bin/sun_gtk'],
@@ -47,18 +45,18 @@
     description='Tray notification applet for informing about package updates '
                 'in Slackware',
     long_description=open('README.rst').read(),
     keywords=['tray', 'notify', 'slackware', 'desktop'],
     author=__author__,
     author_email=__email__,
     package_data={'': ['LICENSE.txt', 'README.rst', 'CHANGES.md']},
-    data_files=[(data_configs['icon_path'], ['extra/icon/sun.png']),
-                (data_configs['desktop_path'], ['extra/desktop/sun.desktop']),
-                (data_configs['xdg_autostart'], ['extra/xdg/sun_daemon.desktop.sample']),
-                (data_configs['xdg_autostart'], ['extra/xdg/sun.desktop'])],
+    data_files=[(str(data_configs['icon_path']), ['extra/icon/sun.png']),
+                (str(data_configs['desktop_path']), ['extra/desktop/sun.desktop']),
+                (str(data_configs['xdg_autostart']), ['extra/xdg/sun_daemon.desktop.sample']),
+                (str(data_configs['xdg_autostart']), ['extra/xdg/sun.desktop'])],
     url='https://gitlab.com/dslackw/sun',
     install_requires=INSTALLATION_REQUIREMENTS,
     extras_require={
         'optional': OPTIONAL_REQUIREMENTS,
         'docs': DOCS_REQUIREMENTS,
         'tests': TESTS_REQUIREMENTS,
     },
```

### Comparing `sun-1.4.9/README.rst` & `sun-1.5.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -25,25 +25,25 @@
 Installing
 ----------
 
 .. code-block:: bash
 
     Required root privileges
 
-    $ tar xvf sun-1.4.9.tar.gz
-    $ cd sun-1.4.9
+    $ tar xvf sun-1.5.0.tar.gz
+    $ cd sun-1.5.0
     $ ./install.sh
 
     Installed as Slackware package
 
 
 Usage
 -----
 
-| Edit the configuration :code:`/etc/sun/sun.toml` file and change the http mirror for your country.
+| Edit the configuration :code:`/etc/sun/repositories.toml` file and change a http mirror for your country.
 | NOTE: ftp mirrors not supported.
 
 
 GTK Icon
 --------
 
 .. image:: https://gitlab.com/dslackw/images/raw/master/sun/gtk_daemon.png
@@ -57,15 +57,15 @@
 
 CLI
 ---
 
 .. code-block:: bash
 
     $ sun help
-    SUN (Slackware Update Notifier) - Version: 1.4.9
+    SUN (Slackware Update Notifier) - Version: 1.5.0
 
     Usage: sun [OPTIONS]
 
     Optional arguments:
       help       Display this help and exit.
       start      Start sun daemon.
       stop       Stop sun daemon.
@@ -79,17 +79,17 @@
 
     $ sun start
     Starting SUN daemon:  /usr/bin/sun_daemon &
 
     $ sun check
     3 software updates are available from 1 repository
 
-    Slackware: samba-4.1.17-x86_64-1_slack14.1.txz
-    Slackware: mozilla-firefox-31.5.0esr-x86_64-1_slack14.1.txz
-    Slackware: mozilla-thunderbird-31.5.0-x86_64-1_slack14.1.txz
+    Slack: samba-4.1.17-x86_64-1_slack14.1.txz
+    Slack: mozilla-firefox-31.5.0esr-x86_64-1_slack14.1.txz
+    Slack: mozilla-thunderbird-31.5.0-x86_64-1_slack14.1.txz
 
     $ sun stop
     Stopping SUN daemon:  /usr/bin/sun_daemon
 
     $ sun status
     SUN is not running
 
@@ -122,19 +122,22 @@
 -------------------
 
 .. code-block:: bash
 
     /etc/sun/sun.toml
         General configuration of sun
 
+    /etc/sun/repositories.toml
+        Repositories configuration of sun
+
 
 Donate
 ------
 
-If you feel satisfied with this project and want to thanks me make a donation.
+If you feel satisfied with this project and want to thank me, treat me to a coffee ☕ !
 
 .. image:: https://gitlab.com/dslackw/images/raw/master/donate/paypaldonate.png
    :target: https://www.paypal.me/dslackw
 
 
 Copyright
 ---------
```

### Comparing `sun-1.4.9/sbin/sun_daemon` & `sun-1.5.0/sbin/sun_daemon`

 * *Files 10% similar despite different names*

```diff
@@ -27,58 +27,57 @@
  ____  _   _ _   _
 / ___|| | | | \ | |
 \___ \| | | |  \| |
  ___) | |_| | |\  |
 |____/ \___/|_| \_|
 """
 
-
-import os
 import sys
 import shutil
+from pathlib import Path
 
 
 def autostart():
     args: list = sys.argv
     args.pop(0)
 
-    xdg_autostart_path: str = '/etc/xdg/autostart/'
-    enable_file: str = f'{xdg_autostart_path}sun_daemon.desktop'
-    disable_file: str = f'{enable_file}.sample'
+    xdg_autostart_path: Path = Path('/etc/xdg/autostart')
+    enable_file: Path = Path(xdg_autostart_path, 'sun_daemon.desktop')
+    disable_file: Path = Path(xdg_autostart_path, 'sun_daemon.desktop.sample')
 
     message: str = 'The sun_daemon autostart is'
     message_enabled: str = f'{message} enabled.'
     message_disabled: str = f'{message} disabled.'
     message_already_enabled: str = f'{message} already enabled.'
     message_already_disabled: str = f'{message} already disabled.'
 
     if len(args) == 1 and args[0] == 'enable':
 
-        if os.path.isfile(disable_file):
+        if disable_file.is_file():
             shutil.move(disable_file, enable_file)
             print(message_enabled)
 
-        elif os.path.isfile(enable_file):
+        elif enable_file.is_file():
             print(message_already_enabled)
 
     elif len(args) == 1 and args[0] == 'disable':
 
-        if os.path.isfile(enable_file):
+        if enable_file.is_file():
             shutil.move(enable_file, disable_file)
             print(message_disabled)
 
-        elif os.path.isfile(disable_file):
+        elif disable_file.is_file():
             print(message_already_disabled)
 
     elif len(args) == 1 and args[0] == 'status':
 
-        if os.path.isfile(enable_file):
+        if enable_file.is_file():
             print(message_enabled)
 
-        elif os.path.isfile(disable_file):
+        elif disable_file.is_file():
             print(message_disabled)
 
     else:
         print("SUN (Slackware Update Notifier) sun_daemon autostart.\n"
               "\nUsage: sun_daemon [OPTIONS]\n"
               "\nOptional arguments:\n"
               "  enable      Enable autostart SUN daemon.\n"
```

### Comparing `sun-1.4.9/sun.egg-info/PKG-INFO` & `sun-1.5.0/sun.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: sun
-Version: 1.4.9
+Version: 1.5.0
 Summary: Tray notification applet for informing about package updates in Slackware
 Home-page: https://gitlab.com/dslackw/sun
 Author: dslackw
-Author-email: d.zlatanidis@gmail.com
+Author-email: dslackw@gmail.com
 License: UNKNOWN
 Keywords: tray,notify,slackware,desktop
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.7
@@ -51,25 +51,25 @@
 Installing
 ----------
 
 .. code-block:: bash
 
     Required root privileges
 
-    $ tar xvf sun-1.4.9.tar.gz
-    $ cd sun-1.4.9
+    $ tar xvf sun-1.5.0.tar.gz
+    $ cd sun-1.5.0
     $ ./install.sh
 
     Installed as Slackware package
 
 
 Usage
 -----
 
-| Edit the configuration :code:`/etc/sun/sun.toml` file and change the http mirror for your country.
+| Edit the configuration :code:`/etc/sun/repositories.toml` file and change a http mirror for your country.
 | NOTE: ftp mirrors not supported.
 
 
 GTK Icon
 --------
 
 .. image:: https://gitlab.com/dslackw/images/raw/master/sun/gtk_daemon.png
@@ -83,15 +83,15 @@
 
 CLI
 ---
 
 .. code-block:: bash
 
     $ sun help
-    SUN (Slackware Update Notifier) - Version: 1.4.9
+    SUN (Slackware Update Notifier) - Version: 1.5.0
 
     Usage: sun [OPTIONS]
 
     Optional arguments:
       help       Display this help and exit.
       start      Start sun daemon.
       stop       Stop sun daemon.
@@ -105,17 +105,17 @@
 
     $ sun start
     Starting SUN daemon:  /usr/bin/sun_daemon &
 
     $ sun check
     3 software updates are available from 1 repository
 
-    Slackware: samba-4.1.17-x86_64-1_slack14.1.txz
-    Slackware: mozilla-firefox-31.5.0esr-x86_64-1_slack14.1.txz
-    Slackware: mozilla-thunderbird-31.5.0-x86_64-1_slack14.1.txz
+    Slack: samba-4.1.17-x86_64-1_slack14.1.txz
+    Slack: mozilla-firefox-31.5.0esr-x86_64-1_slack14.1.txz
+    Slack: mozilla-thunderbird-31.5.0-x86_64-1_slack14.1.txz
 
     $ sun stop
     Stopping SUN daemon:  /usr/bin/sun_daemon
 
     $ sun status
     SUN is not running
 
@@ -148,19 +148,22 @@
 -------------------
 
 .. code-block:: bash
 
     /etc/sun/sun.toml
         General configuration of sun
 
+    /etc/sun/repositories.toml
+        Repositories configuration of sun
+
 
 Donate
 ------
 
-If you feel satisfied with this project and want to thanks me make a donation.
+If you feel satisfied with this project and want to thank me, treat me to a coffee ☕ !
 
 .. image:: https://gitlab.com/dslackw/images/raw/master/donate/paypaldonate.png
    :target: https://www.paypal.me/dslackw
 
 
 Copyright
 ---------
```

### Comparing `sun-1.4.9/install.sh` & `sun-1.5.0/install.sh`

 * *Files identical despite different names*

### Comparing `sun-1.4.9/bin/sun_daemon` & `sun-1.5.0/bin/sun_daemon`

 * *Files identical despite different names*

### Comparing `sun-1.4.9/bin/sun` & `sun-1.5.0/bin/sun`

 * *Files 5% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 / ___|| | | | \ | |
 \___ \| | | |  \| |
  ___) | |_| | |\  |
 |____/ \___/|_| \_|
 """
 
 
-from sun.cli.tool import Tools
+from sun.cli.tool import Cli
 
 
 try:
-    tool = Tools()
-    tool.cli()
+    cli = Cli()
+    cli.menu()
 except KeyboardInterrupt:
     raise SystemExit(1)
```

### Comparing `sun-1.4.9/bin/sun_gtk` & `sun-1.5.0/bin/sun_gtk`

 * *Files identical despite different names*

