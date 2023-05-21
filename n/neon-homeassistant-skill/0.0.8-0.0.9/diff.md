# Comparing `tmp/neon_homeassistant_skill-0.0.8.tar.gz` & `tmp/neon_homeassistant_skill-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon_homeassistant_skill-0.0.8.tar", max compression
+gzip compressed data, was "neon_homeassistant_skill-0.0.9.tar", max compression
```

## Comparing `neon_homeassistant_skill-0.0.8.tar` & `neon_homeassistant_skill-0.0.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0    10947 2023-02-06 23:19:30.522507 neon_homeassistant_skill-0.0.8/LICENSE
--rw-r--r--   0        0        0     1100 2023-03-06 02:56:43.956713 neon_homeassistant_skill-0.0.8/README.md
--rw-r--r--   0        0        0    12949 2023-03-08 04:59:17.228789 neon_homeassistant_skill-0.0.8/neon_homeassistant_skill/__init__.py
--rw-r--r--   0        0        0       55 2023-02-11 03:27:58.879381 neon_homeassistant_skill-0.0.8/neon_homeassistant_skill/dialog/en-us/acknowledge.dialog
--rw-r--r--   0        0        0      109 2023-02-11 03:27:58.879512 neon_homeassistant_skill-0.0.8/neon_homeassistant_skill/dialog/en-us/area.dashboard.opened.dialog
--rw-r--r--   0        0        0      108 2023-02-11 03:27:58.879643 neon_homeassistant_skill-0.0.8/neon_homeassistant_skill/dialog/en-us/area.not.found.dialog
--rw-r--r--   0        0        0      151 2023-02-06 23:19:30.523723 neon_homeassistant_skill-0.0.8/neon_homeassistant_skill/dialog/en-us/device.not.found.dialog
--rw-r--r--   0        0        0      148 2023-02-11 03:27:58.879772 neon_homeassistant_skill-0.0.8/neon_homeassistant_skill/dialog/en-us/device.status.dialog
--rw-r--r--   0        0        0       68 2023-02-06 23:19:30.523803 neon_homeassistant_skill-0.0.8/neon_homeassistant_skill/dialog/en-us/device.turned.off.dialog
--rw-r--r--   0        0        0       65 2023-02-06 23:19:30.524252 neon_homeassistant_skill-0.0.8/neon_homeassistant_skill/dialog/en-us/device.turned.on.dialog
--rw-r--r--   0        0        0       75 2023-02-06 23:19:30.524646 neon_homeassistant_skill-0.0.8/neon_homeassistant_skill/dialog/en-us/ha.dashboard.closed.dialog
--rw-r--r--   0        0        0      114 2023-02-06 23:19:30.524841 neon_homeassistant_skill-0.0.8/neon_homeassistant_skill/dialog/en-us/ha.dashboard.opened.dialog
--rw-r--r--   0        0        0      128 2023-02-06 23:19:30.525261 neon_homeassistant_skill-0.0.8/neon_homeassistant_skill/dialog/en-us/lights.current.brightness.dialog
--rw-r--r--   0        0        0       87 2023-02-06 23:19:30.525481 neon_homeassistant_skill-0.0.8/neon_homeassistant_skill/dialog/en-us/lights.status.not.available.dialog
--rw-r--r--   0        0        0      149 2023-02-11 03:27:58.879895 neon_homeassistant_skill-0.0.8/neon_homeassistant_skill/dialog/en-us/vacuum.action.not.found.dialog
--rw-r--r--   0        0        0       51 2023-03-09 01:10:00.320457 neon_homeassistant_skill-0.0.8/neon_homeassistant_skill/vocab/en-us/close.dashboard.intent
--rw-r--r--   0        0        0      137 2023-02-11 03:27:58.880498 neon_homeassistant_skill-0.0.8/neon_homeassistant_skill/vocab/en-us/lights.decrease.brightness.intent
--rw-r--r--   0        0        0      124 2023-02-11 03:27:58.880655 neon_homeassistant_skill-0.0.8/neon_homeassistant_skill/vocab/en-us/lights.get.brightness.intent
--rw-r--r--   0        0        0      120 2023-02-11 03:27:58.880816 neon_homeassistant_skill-0.0.8/neon_homeassistant_skill/vocab/en-us/lights.get.color.intent
--rw-r--r--   0        0        0      132 2023-02-11 03:27:58.880967 neon_homeassistant_skill-0.0.8/neon_homeassistant_skill/vocab/en-us/lights.increase.brightness.intent
--rw-r--r--   0        0        0      208 2023-02-11 03:27:58.881127 neon_homeassistant_skill-0.0.8/neon_homeassistant_skill/vocab/en-us/lights.set.brightness.intent
--rw-r--r--   0        0        0       97 2023-02-11 03:27:58.881324 neon_homeassistant_skill-0.0.8/neon_homeassistant_skill/vocab/en-us/lights.set.color.intent
--rw-r--r--   0        0        0       57 2023-02-11 03:27:58.881483 neon_homeassistant_skill-0.0.8/neon_homeassistant_skill/vocab/en-us/open.dashboard.intent
--rw-r--r--   0        0        0      358 2023-02-13 03:18:07.315612 neon_homeassistant_skill-0.0.8/neon_homeassistant_skill/vocab/en-us/sensor.intent
--rw-r--r--   0        0        0       49 2023-02-11 03:27:58.881785 neon_homeassistant_skill-0.0.8/neon_homeassistant_skill/vocab/en-us/show.area.dashboard.intent
--rw-r--r--   0        0        0      140 2023-02-11 03:27:58.881940 neon_homeassistant_skill-0.0.8/neon_homeassistant_skill/vocab/en-us/stop.intent
--rw-r--r--   0        0        0      204 2023-02-11 03:27:58.882295 neon_homeassistant_skill-0.0.8/neon_homeassistant_skill/vocab/en-us/turn.off.intent
--rw-r--r--   0        0        0      196 2023-02-11 03:27:58.882520 neon_homeassistant_skill-0.0.8/neon_homeassistant_skill/vocab/en-us/turn.on.intent
--rw-r--r--   0        0        0     1081 2023-03-08 04:51:38.201654 neon_homeassistant_skill-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     2216 1970-01-01 00:00:00.000000 neon_homeassistant_skill-0.0.8/setup.py
--rw-r--r--   0        0        0     1807 1970-01-01 00:00:00.000000 neon_homeassistant_skill-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0    10947 2023-02-06 23:19:30.522507 neon_homeassistant_skill-0.0.9/LICENSE
+-rw-r--r--   0        0        0     1100 2023-03-06 02:56:43.956713 neon_homeassistant_skill-0.0.9/README.md
+-rw-r--r--   0        0        0    12954 2023-03-15 04:10:11.820165 neon_homeassistant_skill-0.0.9/neon_homeassistant_skill/__init__.py
+-rw-r--r--   0        0        0       55 2023-02-11 03:27:58.879381 neon_homeassistant_skill-0.0.9/neon_homeassistant_skill/dialog/en-us/acknowledge.dialog
+-rw-r--r--   0        0        0      109 2023-02-11 03:27:58.879512 neon_homeassistant_skill-0.0.9/neon_homeassistant_skill/dialog/en-us/area.dashboard.opened.dialog
+-rw-r--r--   0        0        0      108 2023-02-11 03:27:58.879643 neon_homeassistant_skill-0.0.9/neon_homeassistant_skill/dialog/en-us/area.not.found.dialog
+-rw-r--r--   0        0        0      151 2023-02-06 23:19:30.523723 neon_homeassistant_skill-0.0.9/neon_homeassistant_skill/dialog/en-us/device.not.found.dialog
+-rw-r--r--   0        0        0      148 2023-02-11 03:27:58.879772 neon_homeassistant_skill-0.0.9/neon_homeassistant_skill/dialog/en-us/device.status.dialog
+-rw-r--r--   0        0        0       68 2023-02-06 23:19:30.523803 neon_homeassistant_skill-0.0.9/neon_homeassistant_skill/dialog/en-us/device.turned.off.dialog
+-rw-r--r--   0        0        0       65 2023-02-06 23:19:30.524252 neon_homeassistant_skill-0.0.9/neon_homeassistant_skill/dialog/en-us/device.turned.on.dialog
+-rw-r--r--   0        0        0       75 2023-02-06 23:19:30.524646 neon_homeassistant_skill-0.0.9/neon_homeassistant_skill/dialog/en-us/ha.dashboard.closed.dialog
+-rw-r--r--   0        0        0      114 2023-02-06 23:19:30.524841 neon_homeassistant_skill-0.0.9/neon_homeassistant_skill/dialog/en-us/ha.dashboard.opened.dialog
+-rw-r--r--   0        0        0      128 2023-02-06 23:19:30.525261 neon_homeassistant_skill-0.0.9/neon_homeassistant_skill/dialog/en-us/lights.current.brightness.dialog
+-rw-r--r--   0        0        0       87 2023-02-06 23:19:30.525481 neon_homeassistant_skill-0.0.9/neon_homeassistant_skill/dialog/en-us/lights.status.not.available.dialog
+-rw-r--r--   0        0        0      149 2023-02-11 03:27:58.879895 neon_homeassistant_skill-0.0.9/neon_homeassistant_skill/dialog/en-us/vacuum.action.not.found.dialog
+-rw-r--r--   0        0        0       51 2023-03-09 01:10:00.320457 neon_homeassistant_skill-0.0.9/neon_homeassistant_skill/vocab/en-us/close.dashboard.intent
+-rw-r--r--   0        0        0      137 2023-02-11 03:27:58.880498 neon_homeassistant_skill-0.0.9/neon_homeassistant_skill/vocab/en-us/lights.decrease.brightness.intent
+-rw-r--r--   0        0        0      124 2023-02-11 03:27:58.880655 neon_homeassistant_skill-0.0.9/neon_homeassistant_skill/vocab/en-us/lights.get.brightness.intent
+-rw-r--r--   0        0        0      120 2023-02-11 03:27:58.880816 neon_homeassistant_skill-0.0.9/neon_homeassistant_skill/vocab/en-us/lights.get.color.intent
+-rw-r--r--   0        0        0      132 2023-02-11 03:27:58.880967 neon_homeassistant_skill-0.0.9/neon_homeassistant_skill/vocab/en-us/lights.increase.brightness.intent
+-rw-r--r--   0        0        0      190 2023-03-15 03:34:01.985935 neon_homeassistant_skill-0.0.9/neon_homeassistant_skill/vocab/en-us/lights.set.brightness.intent
+-rw-r--r--   0        0        0       96 2023-03-15 18:13:48.365174 neon_homeassistant_skill-0.0.9/neon_homeassistant_skill/vocab/en-us/lights.set.color.intent
+-rw-r--r--   0        0        0       57 2023-02-11 03:27:58.881483 neon_homeassistant_skill-0.0.9/neon_homeassistant_skill/vocab/en-us/open.dashboard.intent
+-rw-r--r--   0        0        0      358 2023-02-13 03:18:07.315612 neon_homeassistant_skill-0.0.9/neon_homeassistant_skill/vocab/en-us/sensor.intent
+-rw-r--r--   0        0        0       44 2023-03-15 03:32:03.781707 neon_homeassistant_skill-0.0.9/neon_homeassistant_skill/vocab/en-us/show.area.dashboard.intent
+-rw-r--r--   0        0        0      140 2023-02-11 03:27:58.881940 neon_homeassistant_skill-0.0.9/neon_homeassistant_skill/vocab/en-us/stop.intent
+-rw-r--r--   0        0        0      204 2023-02-11 03:27:58.882295 neon_homeassistant_skill-0.0.9/neon_homeassistant_skill/vocab/en-us/turn.off.intent
+-rw-r--r--   0        0        0      196 2023-02-11 03:27:58.882520 neon_homeassistant_skill-0.0.9/neon_homeassistant_skill/vocab/en-us/turn.on.intent
+-rw-r--r--   0        0        0     1081 2023-03-15 18:12:13.825594 neon_homeassistant_skill-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2216 1970-01-01 00:00:00.000000 neon_homeassistant_skill-0.0.9/setup.py
+-rw-r--r--   0        0        0     1807 1970-01-01 00:00:00.000000 neon_homeassistant_skill-0.0.9/PKG-INFO
```

### Comparing `neon_homeassistant_skill-0.0.8/LICENSE` & `neon_homeassistant_skill-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `neon_homeassistant_skill-0.0.8/README.md` & `neon_homeassistant_skill-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `neon_homeassistant_skill-0.0.8/neon_homeassistant_skill/__init__.py` & `neon_homeassistant_skill-0.0.9/neon_homeassistant_skill/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import asyncio
 
 from mycroft.messagebus.message import Message
 from mycroft.skills.core import MycroftSkill, intent_handler
 from mycroft.util.log import LOG
 from pfzy import fuzzy_match
 
-__version__ = "0.0.8"
+__version__ = "0.0.9"
 
 
 # https://github.com/OpenVoiceOS/ovos-PHAL-plugin-homeassistant/blob/master/ovos_PHAL_plugin_homeassistant/__init__.py
 class NeonHomeAssistantSkill(MycroftSkill):
     """Home Assistant skill for Neon OS. Requires the PHAL Home Assistant plugin."""
 
     def __init__(self):
@@ -196,15 +196,15 @@
             self.bus.emit(Message("ovos.phal.plugin.homeassistant.call.supported.function", call_data))
             self.speak_dialog("acknowledge")
         else:
             self.speak_dialog("device.not.found", data={"device": device})
 
     @intent_handler("show.area.dashboard.intent")
     def handle_show_area_dashboard_intent(self, message):
-        area = message.get("area")
+        area = message.data.get("area")
         if area:
             self.bus.emit(Message("ovos.phal.plugin.homeassistant.show.area.dashboard"), {"area": area})
             self.speak_dialog("area.dashboard.opened", data={"area": area})
         else:
             self.speak_dialog("area.not.found")
 
     # @intent_handler("vacuum.action.intent")  # TODO: Find an intent that doesn't conflict with OCP
```

### Comparing `neon_homeassistant_skill-0.0.8/pyproject.toml` & `neon_homeassistant_skill-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "poetry_core>=1.0.0" ]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "neon-homeassistant-skill"
-version = "0.0.8"
+version = "0.0.9"
 description = "A Neon AI Skill for Home Assistant, which integrates with ovos-PHAL-plugin-homeassistant."
 authors = [ "Mike Gray <mike@graywind.org>" ]
 readme = "README.md"
 license = "Apache-2.0"
 include = ["neon_homeassistant_skill/dialog/*", "neon_homeassistant_skill/vocab/*"]
 
 [tool.poetry.dependencies]
```

### Comparing `neon_homeassistant_skill-0.0.8/setup.py` & `neon_homeassistant_skill-0.0.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 {'console_scripts': ['neon-homeassistant-skill = '
                      'neon_homeassistant_skill:NeonHomeAssistantSkill'],
  'ovos.plugin.skill': ['neon_homeassistant_skill.mikejgray = '
                        'neon_homeassistant_skill:NeonHomeAssistantSkill']}
 
 setup_kwargs = {
     'name': 'neon-homeassistant-skill',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': 'A Neon AI Skill for Home Assistant, which integrates with ovos-PHAL-plugin-homeassistant.',
     'long_description': "# Home Assistant Neon Skill\n\nUses [PHAL Home Assistant plugin](https://github.com/OpenVoiceOS/ovos-PHAL-plugin-homeassistant)\n\nStill a work in progress - PRs and issues welcome\n\nAvailable on PyPi: `pip install neon-homeassistant-skill`\n\n## Installation on Neon\n\nInstall ovos-PHAL-plugin-homeassistant [per their documentation](https://github.com/OpenVoiceOS/ovos-PHAL-plugin-homeassistant)\nNote that Neon uses a YAML configuration, not a JSON file, so edit ~/.config/neon/neon.yaml and make the following update for a minimal installation:\n\n```yaml\nPHAL:\n  ovos-PHAL-plugin-homeassistant:\n    host: http://<HA_IP_OR_HOSTNAME>:8123\n    api_key: <HA_LONG_LIVED_TOKEN>\n```\n\nYou can also say `open home assistant dashboard` on a device with a screen, like the Mark 2, and use the OAuth login flow from the PHAL plugin.\n\nSSH to the Neon device\n\n```shell\nosm install https://github.com/mikejgray/neon-homeassistant-skill\n```\n\n## Upcoming Features\n\n- Start OAuth workflow with voice\n- Start an instance of the ovos-PHAL-plugin-homeassistant if PHAL isn't already running\n- Vacuum functions\n- HVAC functions\n",
     'author': 'Mike Gray',
     'author_email': 'mike@graywind.org',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `neon_homeassistant_skill-0.0.8/PKG-INFO` & `neon_homeassistant_skill-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-homeassistant-skill
-Version: 0.0.8
+Version: 0.0.9
 Summary: A Neon AI Skill for Home Assistant, which integrates with ovos-PHAL-plugin-homeassistant.
 License: Apache-2.0
 Author: Mike Gray
 Author-email: mike@graywind.org
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

