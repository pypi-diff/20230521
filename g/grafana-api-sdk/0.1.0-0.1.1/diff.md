# Comparing `tmp/grafana-api-sdk-0.1.0.tar.gz` & `tmp/grafana-api-sdk-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grafana-api-sdk-0.1.0.tar", last modified: Thu Apr 13 22:24:54 2023, max compression
+gzip compressed data, was "grafana-api-sdk-0.1.1.tar", last modified: Sun May 21 17:56:27 2023, max compression
```

## Comparing `grafana-api-sdk-0.1.0.tar` & `grafana-api-sdk-0.1.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:24:54.854884 grafana-api-sdk-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-13 22:24:21.000000 grafana-api-sdk-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-04-13 22:24:54.854884 grafana-api-sdk-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10484 2023-04-13 22:24:21.000000 grafana-api-sdk-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:24:54.854884 grafana-api-sdk-0.1.0/grafana_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-13 22:24:21.000000 grafana-api-sdk-0.1.0/grafana_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19022 2023-04-13 22:24:21.000000 grafana-api-sdk-0.1.0/grafana_api/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)    41670 2023-04-13 22:24:21.000000 grafana-api-sdk-0.1.0/grafana_api/alerting.py
--rw-r--r--   0 runner    (1001) docker     (123)    10994 2023-04-13 22:24:21.000000 grafana-api-sdk-0.1.0/grafana_api/alerting_notifications.py
--rw-r--r--   0 runner    (1001) docker     (123)    32117 2023-04-13 22:24:21.000000 grafana-api-sdk-0.1.0/grafana_api/alerting_provisioning.py
--rw-r--r--   0 runner    (1001) docker     (123)    12277 2023-04-13 22:24:21.000000 grafana-api-sdk-0.1.0/grafana_api/annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)     7097 2023-04-13 22:24:21.000000 grafana-api-sdk-0.1.0/grafana_api/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-04-13 22:24:21.000000 grafana-api-sdk-0.1.0/grafana_api/authentication.py
--rw-r--r--   0 runner    (1001) docker     (123)     8888 2023-04-13 22:24:21.000000 grafana-api-sdk-0.1.0/grafana_api/correlations.py
--rw-r--r--   0 runner    (1001) docker     (123)    22349 2023-04-13 22:24:21.000000 grafana-api-sdk-0.1.0/grafana_api/dashboard.py
--rw-r--r--   0 runner    (1001) docker     (123)    21121 2023-04-13 22:24:21.000000 grafana-api-sdk-0.1.0/grafana_api/datasource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-04-13 22:24:21.000000 grafana-api-sdk-0.1.0/grafana_api/external_group.py
--rw-r--r--   0 runner    (1001) docker     (123)    11383 2023-04-13 22:24:21.000000 grafana-api-sdk-0.1.0/grafana_api/folder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5528 2023-04-13 22:24:21.000000 grafana-api-sdk-0.1.0/grafana_api/legacy_alerting.py
--rw-r--r--   0 runner    (1001) docker     (123)     6462 2023-04-13 22:24:21.000000 grafana-api-sdk-0.1.0/grafana_api/legacy_playlist.py
--rw-r--r--   0 runner    (1001) docker     (123)    12277 2023-04-13 22:24:21.000000 grafana-api-sdk-0.1.0/grafana_api/library.py
--rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-04-13 22:24:21.000000 grafana-api-sdk-0.1.0/grafana_api/licensing.py
--rw-r--r--   0 runner    (1001) docker     (123)    25435 2023-04-13 22:24:21.000000 grafana-api-sdk-0.1.0/grafana_api/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    19500 2023-04-13 22:24:21.000000 grafana-api-sdk-0.1.0/grafana_api/organisation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-04-13 22:24:21.000000 grafana-api-sdk-0.1.0/grafana_api/other_http.py
--rw-r--r--   0 runner    (1001) docker     (123)     9395 2023-04-13 22:24:21.000000 grafana-api-sdk-0.1.0/grafana_api/playlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-04-13 22:24:21.000000 grafana-api-sdk-0.1.0/grafana_api/preferences.py
--rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-04-13 22:24:21.000000 grafana-api-sdk-0.1.0/grafana_api/query_history.py
--rw-r--r--   0 runner    (1001) docker     (123)    46835 2023-04-13 22:24:21.000000 grafana-api-sdk-0.1.0/grafana_api/rbac.py
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-04-13 22:24:21.000000 grafana-api-sdk-0.1.0/grafana_api/reporting.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-04-13 22:24:21.000000 grafana-api-sdk-0.1.0/grafana_api/search.py
--rw-r--r--   0 runner    (1001) docker     (123)    15711 2023-04-13 22:24:21.000000 grafana-api-sdk-0.1.0/grafana_api/service_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-04-13 22:24:21.000000 grafana-api-sdk-0.1.0/grafana_api/short_url.py
--rw-r--r--   0 runner    (1001) docker     (123)     6901 2023-04-13 22:24:21.000000 grafana-api-sdk-0.1.0/grafana_api/snapshot.py
--rw-r--r--   0 runner    (1001) docker     (123)    13474 2023-04-13 22:24:21.000000 grafana-api-sdk-0.1.0/grafana_api/team.py
--rw-r--r--   0 runner    (1001) docker     (123)    17682 2023-04-13 22:24:21.000000 grafana-api-sdk-0.1.0/grafana_api/user.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-13 22:24:54.854884 grafana-api-sdk-0.1.0/grafana_api_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-04-13 22:24:54.000000 grafana-api-sdk-0.1.0/grafana_api_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-13 22:24:54.000000 grafana-api-sdk-0.1.0/grafana_api_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-13 22:24:54.000000 grafana-api-sdk-0.1.0/grafana_api_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-13 22:24:54.000000 grafana-api-sdk-0.1.0/grafana_api_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-13 22:24:54.000000 grafana-api-sdk-0.1.0/grafana_api_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-13 22:24:54.854884 grafana-api-sdk-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-04-13 22:24:21.000000 grafana-api-sdk-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:56:27.044316 grafana-api-sdk-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-21 17:55:49.000000 grafana-api-sdk-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-05-21 17:56:27.044316 grafana-api-sdk-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10484 2023-05-21 17:55:49.000000 grafana-api-sdk-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:56:27.044316 grafana-api-sdk-0.1.1/grafana_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 17:55:49.000000 grafana-api-sdk-0.1.1/grafana_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19022 2023-05-21 17:55:49.000000 grafana-api-sdk-0.1.1/grafana_api/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41670 2023-05-21 17:55:49.000000 grafana-api-sdk-0.1.1/grafana_api/alerting.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10994 2023-05-21 17:55:49.000000 grafana-api-sdk-0.1.1/grafana_api/alerting_notifications.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34167 2023-05-21 17:55:49.000000 grafana-api-sdk-0.1.1/grafana_api/alerting_provisioning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12277 2023-05-21 17:55:49.000000 grafana-api-sdk-0.1.1/grafana_api/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7491 2023-05-21 17:55:49.000000 grafana-api-sdk-0.1.1/grafana_api/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4647 2023-05-21 17:55:49.000000 grafana-api-sdk-0.1.1/grafana_api/authentication.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8888 2023-05-21 17:55:49.000000 grafana-api-sdk-0.1.1/grafana_api/correlations.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22349 2023-05-21 17:55:49.000000 grafana-api-sdk-0.1.1/grafana_api/dashboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21121 2023-05-21 17:55:49.000000 grafana-api-sdk-0.1.1/grafana_api/datasource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-05-21 17:55:49.000000 grafana-api-sdk-0.1.1/grafana_api/external_group.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11383 2023-05-21 17:55:49.000000 grafana-api-sdk-0.1.1/grafana_api/folder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-05-21 17:55:49.000000 grafana-api-sdk-0.1.1/grafana_api/legacy_alerting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6462 2023-05-21 17:55:49.000000 grafana-api-sdk-0.1.1/grafana_api/legacy_playlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12277 2023-05-21 17:55:49.000000 grafana-api-sdk-0.1.1/grafana_api/library.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3258 2023-05-21 17:55:49.000000 grafana-api-sdk-0.1.1/grafana_api/licensing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25435 2023-05-21 17:55:49.000000 grafana-api-sdk-0.1.1/grafana_api/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19500 2023-05-21 17:55:49.000000 grafana-api-sdk-0.1.1/grafana_api/organisation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3594 2023-05-21 17:55:49.000000 grafana-api-sdk-0.1.1/grafana_api/other_http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9395 2023-05-21 17:55:49.000000 grafana-api-sdk-0.1.1/grafana_api/playlist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6208 2023-05-21 17:55:49.000000 grafana-api-sdk-0.1.1/grafana_api/preferences.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8930 2023-05-21 17:55:49.000000 grafana-api-sdk-0.1.1/grafana_api/query_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46835 2023-05-21 17:55:49.000000 grafana-api-sdk-0.1.1/grafana_api/rbac.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-05-21 17:55:49.000000 grafana-api-sdk-0.1.1/grafana_api/reporting.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-21 17:55:49.000000 grafana-api-sdk-0.1.1/grafana_api/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15711 2023-05-21 17:55:49.000000 grafana-api-sdk-0.1.1/grafana_api/service_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-05-21 17:55:49.000000 grafana-api-sdk-0.1.1/grafana_api/short_url.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6901 2023-05-21 17:55:49.000000 grafana-api-sdk-0.1.1/grafana_api/snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13474 2023-05-21 17:55:49.000000 grafana-api-sdk-0.1.1/grafana_api/team.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17682 2023-05-21 17:55:49.000000 grafana-api-sdk-0.1.1/grafana_api/user.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 17:56:27.044316 grafana-api-sdk-0.1.1/grafana_api_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11024 2023-05-21 17:56:27.000000 grafana-api-sdk-0.1.1/grafana_api_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-05-21 17:56:27.000000 grafana-api-sdk-0.1.1/grafana_api_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 17:56:27.000000 grafana-api-sdk-0.1.1/grafana_api_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-21 17:56:27.000000 grafana-api-sdk-0.1.1/grafana_api_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-21 17:56:27.000000 grafana-api-sdk-0.1.1/grafana_api_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 17:56:27.044316 grafana-api-sdk-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-21 17:55:49.000000 grafana-api-sdk-0.1.1/setup.py
```

### Comparing `grafana-api-sdk-0.1.0/LICENSE` & `grafana-api-sdk-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `grafana-api-sdk-0.1.0/PKG-INFO` & `grafana-api-sdk-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grafana-api-sdk
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Grafana API SDK
 Home-page: https://github.com/ZPascal/grafana_api_sdk
 Author: Pascal Zimmermann
 Author-email: info@theiotstudio.com
 Project-URL: Source, https://github.com/ZPascal/grafana_api_sdk
 Project-URL: Bug Tracker, https://github.com/ZPascal/grafana_api_sdk/issues
 Project-URL: Documentation, https://zpascal.github.io/grafana_api_sdk/
```

### Comparing `grafana-api-sdk-0.1.0/README.md` & `grafana-api-sdk-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `grafana-api-sdk-0.1.0/grafana_api/admin.py` & `grafana-api-sdk-0.1.1/grafana_api/admin.py`

 * *Files identical despite different names*

### Comparing `grafana-api-sdk-0.1.0/grafana_api/alerting.py` & `grafana-api-sdk-0.1.1/grafana_api/alerting.py`

 * *Files identical despite different names*

### Comparing `grafana-api-sdk-0.1.0/grafana_api/alerting_notifications.py` & `grafana-api-sdk-0.1.1/grafana_api/alerting_notifications.py`

 * *Files identical despite different names*

### Comparing `grafana-api-sdk-0.1.0/grafana_api/alerting_provisioning.py` & `grafana-api-sdk-0.1.1/grafana_api/alerting_provisioning.py`

 * *Files 6% similar despite different names*

```diff
@@ -57,19 +57,20 @@
                 raise Exception
             else:
                 return api_call
         else:
             logging.error("There is no uid defined.")
             raise ValueError
 
-    def add_alert_rule(self, alert_rule: AlertRule):
+    def add_alert_rule(self, alert_rule: AlertRule, disable_provenance: bool = False):
         """The method includes a functionality to create a new alert rule
 
         Args:
             alert_rule (AlertRule): Specify the alert rule
+            disable_provenance (bool): Specify if the provenance header should be set or not (default False)
 
         Raises:
             ValueError: Missed specifying a necessary value
             Exception: Unspecified error by executing the API call
 
         Returns:
             None
@@ -77,31 +78,33 @@
 
         if alert_rule is not None:
             api_call: dict = Api(self.grafana_api_model).call_the_api(
                 f"{APIEndpoints.ALERTING_PROVISIONING.value}/alert-rules",
                 RequestsMethods.POST,
                 json.dumps(self.__create_alert_rule_dictionary(alert_rule)),
                 response_status_code=True,
+                disable_provenance_header=disable_provenance,
             )
 
             if 200 <= api_call.get("status") >= 300:
                 logging.error(f"Check the error: {api_call}.")
                 raise Exception
             else:
                 logging.info("You successfully created the corresponding alert rule.")
         else:
             logging.error("There is no alert_rule defined.")
             raise ValueError
 
-    def update_alert_rule(self, uid: str, alert_rule: AlertRule):
+    def update_alert_rule(self, uid: str, alert_rule: AlertRule, disable_provenance: bool = False):
         """The method includes a functionality to update an existing alert rule
 
         Args:
             uid (str): Specify the alert rule uid
             alert_rule (AlertRule): Specify the alert rule
+            disable_provenance (bool): Specify if the provenance header should be set or not (default False)
 
         Raises:
             ValueError: Missed specifying a necessary value
             Exception: Unspecified error by executing the API call
 
         Returns:
             None
@@ -109,34 +112,36 @@
 
         if len(uid) != 0 and alert_rule is not None:
             api_call: dict = Api(self.grafana_api_model).call_the_api(
                 f"{APIEndpoints.ALERTING_PROVISIONING.value}/alert-rules/{uid}",
                 RequestsMethods.PUT,
                 json.dumps(self.__create_alert_rule_dictionary(alert_rule)),
                 response_status_code=True,
+                disable_provenance_header=disable_provenance,
             )
 
             if 200 <= api_call.get("status") >= 300:
                 logging.error(f"Check the error: {api_call}.")
                 raise Exception
             else:
                 logging.info("You successfully updated the corresponding alert rule.")
         else:
             logging.error("There is no uid or alert_rule defined.")
             raise ValueError
 
     def update_the_interval_of_a_alert_rule_group(
-        self, folder_uid: str, group: str, alert_rule_group_interval: int
+        self, folder_uid: str, group: str, alert_rule_group_interval: int, disable_provenance: bool = False
     ):
         """The method includes a functionality to update the interval of a alert rule group
 
         Args:
             folder_uid (str): Specify the folder uid
             group (str): Specify the group
             alert_rule_group_interval (int): Specify the alert rule group interval
+            disable_provenance (bool): Specify if the provenance header should be set or not (default False)
 
         Raises:
             ValueError: Missed specifying a necessary value
             Exception: Unspecified error by executing the API call
 
         Returns:
             None
@@ -144,14 +149,15 @@
 
         if len(folder_uid) != 0 and len(group) != 0 and alert_rule_group_interval != 0:
             api_call: dict = Api(self.grafana_api_model).call_the_api(
                 f"{APIEndpoints.ALERTING_PROVISIONING.value}/folder/{folder_uid}/rule-groups/{group}",
                 RequestsMethods.PUT,
                 json.dumps({"interval": alert_rule_group_interval}),
                 response_status_code=True,
+                disable_provenance_header=disable_provenance,
             )
 
             if 200 <= api_call.get("status") >= 300:
                 logging.error(f"Check the error: {api_call}.")
                 raise Exception
             else:
                 logging.info(
@@ -159,32 +165,34 @@
                 )
         else:
             logging.error(
                 "There is no folder_uid, group or alert_rule_group_interval defined."
             )
             raise ValueError
 
-    def delete_alert_rule(self, uid: str):
+    def delete_alert_rule(self, uid: str, disable_provenance: bool = False):
         """The method includes a functionality to delete an alert rule
 
         Args:
             uid (str): Specify the alert rule uid
+            disable_provenance (bool): Specify if the provenance header should be set or not (default False)
 
         Raises:
             ValueError: Missed specifying a necessary value
             Exception: Unspecified error by executing the API call
         Returns:
             None
         """
 
         if len(uid) != 0:
             api_call: dict = Api(self.grafana_api_model).call_the_api(
                 f"{APIEndpoints.ALERTING_PROVISIONING.value}/alert-rules/{uid}",
                 RequestsMethods.DELETE,
                 response_status_code=True,
+                disable_provenance_header=disable_provenance,
             )
 
             if 200 <= api_call.get("status") >= 300:
                 logging.error(f"Check the error: {api_call}.")
                 raise Exception
             else:
                 logging.info("You successfully deleted the corresponding alert rule.")
@@ -208,19 +216,20 @@
 
         if api_call == list():
             logging.error(f"Check the error: {api_call}.")
             raise Exception
         else:
             return api_call
 
-    def add_contact_point(self, embedded_contact_point: EmbeddedContactPoint):
+    def add_contact_point(self, embedded_contact_point: EmbeddedContactPoint, disable_provenance: bool = False):
         """The method includes a functionality to create a contact point
 
         Args:
             embedded_contact_point (EmbeddedContactPoint): Specify the embedded contact point
+            disable_provenance (bool): Specify if the provenance header should be set or not (default False)
 
         Raises:
             ValueError: Missed specifying a necessary value
             Exception: Unspecified error by executing the API call
 
         Returns:
             None
@@ -237,33 +246,35 @@
                         "settings": embedded_contact_point.settings,
                         "disableResolveMessage": embedded_contact_point.disable_resolve_message,
                         "provenance": embedded_contact_point.provenance,
                         "UID": embedded_contact_point.uid,
                     }
                 ),
                 response_status_code=True,
+                disable_provenance_header=disable_provenance,
             )
 
             if 200 <= api_call.get("status") >= 300:
                 logging.error(f"Check the error: {api_call}.")
                 raise Exception
             else:
                 logging.info("You successfully created a new contact point.")
         else:
             logging.error("There is no embedded_contact_point defined.")
             raise ValueError
 
     def update_contact_point(
-        self, uid: str, embedded_contact_point: EmbeddedContactPoint
+        self, uid: str, embedded_contact_point: EmbeddedContactPoint, disable_provenance: bool = False
     ):
         """The method includes a functionality to update a contact point
 
         Args:
             uid (str): Specify the uid of the contact point
             embedded_contact_point (EmbeddedContactPoint): Specify the embedded contact point
+            disable_provenance (bool): Specify if the provenance header should be set or not (default False)
 
         Raises:
             ValueError: Missed specifying a necessary value
             Exception: Unspecified error by executing the API call
 
         Returns:
             None
@@ -280,14 +291,15 @@
                         "settings": embedded_contact_point.settings,
                         "disableResolveMessage": embedded_contact_point.disable_resolve_message,
                         "provenance": embedded_contact_point.provenance,
                         "UID": embedded_contact_point.uid,
                     }
                 ),
                 response_status_code=True,
+                disable_provenance_header=disable_provenance,
             )
 
             if 200 <= api_call.get("status") >= 300:
                 logging.error(f"Check the error: {api_call}.")
                 raise Exception
             else:
                 logging.info("You successfully updated the contact point.")
@@ -342,19 +354,20 @@
 
         if 200 <= api_call.get("status") >= 300:
             logging.error(f"Check the error: {api_call}.")
             raise Exception
         else:
             return api_call
 
-    def add_notification_policies(self, route: Route):
+    def add_notification_policies(self, route: Route, disable_provenance: bool = False):
         """The method includes a functionality to set the notification policy tree
 
         Args:
             route (Route): Specify the alert rule routes
+            disable_provenance (bool): Specify if the provenance header should be set or not (default False)
 
         Raises:
             ValueError: Missed specifying a necessary value
             Exception: Unspecified error by executing the API call
 
         Returns:
             None
@@ -362,14 +375,15 @@
 
         if route is not None:
             api_call: dict = Api(self.grafana_api_model).call_the_api(
                 f"{APIEndpoints.ALERTING_PROVISIONING.value}/policies",
                 RequestsMethods.PUT,
                 json.dumps(self.__create_alert_route_dictionary(route)),
                 response_status_code=True,
+                disable_provenance_header=disable_provenance,
             )
 
             if 200 <= api_call.get("status") >= 300:
                 logging.error(f"Check the error: {api_call}.")
                 raise Exception
             else:
                 logging.info("You successfully added the notification policies.")
@@ -421,19 +435,20 @@
                 raise Exception
             else:
                 return api_call
         else:
             logging.error("There is no name defined.")
             raise ValueError
 
-    def add_mute_timing(self, mute_time_interval: MuteTimeInterval):
+    def add_mute_timing(self, mute_time_interval: MuteTimeInterval, disable_provenance: bool = False):
         """The method includes a functionality to create a mute timing
 
         Args:
             mute_time_interval (MuteTimeInterval): Specify the mute time interval
+            disable_provenance (bool): Specify if the provenance header should be set or not (default False)
 
         Raises:
             ValueError: Missed specifying a necessary value
             Exception: Unspecified error by executing the API call
 
         Returns:
             None
@@ -441,31 +456,33 @@
 
         if mute_time_interval is not None:
             api_call: dict = Api(self.grafana_api_model).call_the_api(
                 f"{APIEndpoints.ALERTING_PROVISIONING.value}/mute-timings",
                 RequestsMethods.POST,
                 json.dumps(self.__create_mute_timing_dictionary(mute_time_interval)),
                 response_status_code=True,
+                disable_provenance_header=disable_provenance,
             )
 
             if 200 <= api_call.get("status") >= 300:
                 logging.error(f"Check the error: {api_call}.")
                 raise Exception
             else:
                 logging.info("You successfully added the mute timing.")
         else:
             logging.error("There is no mute_time_interval defined.")
             raise ValueError
 
-    def update_mute_timing(self, name: str, mute_time_interval: MuteTimeInterval):
+    def update_mute_timing(self, name: str, mute_time_interval: MuteTimeInterval, disable_provenance: bool = False):
         """The method includes a functionality to update an existing mute timing
 
         Args:
             name (str): Specify the mute timing name
             mute_time_interval (MuteTimeInterval): Specify the mute time interval
+            disable_provenance (bool): Specify if the provenance header should be set or not (default False)
 
         Raises:
             ValueError: Missed specifying a necessary value
             Exception: Unspecified error by executing the API call
 
         Returns:
             None
@@ -473,14 +490,15 @@
 
         if len(name) != 0 and mute_time_interval is not None:
             api_call: dict = Api(self.grafana_api_model).call_the_api(
                 f"{APIEndpoints.ALERTING_PROVISIONING.value}/mute-timings/{name}",
                 RequestsMethods.PUT,
                 json.dumps(self.__create_mute_timing_dictionary(mute_time_interval)),
                 response_status_code=True,
+                disable_provenance_header=disable_provenance,
             )
 
             if 200 <= api_call.get("status") >= 300:
                 logging.error(f"Check the error: {api_call}.")
                 raise Exception
             else:
                 logging.info("You successfully updated the mute timing.")
@@ -563,20 +581,21 @@
                 raise Exception
             else:
                 return api_call
         else:
             logging.error("There is no name defined.")
             raise ValueError
 
-    def create_or_update_message_template(self, name: str, message_template: str):
+    def create_or_update_message_template(self, name: str, message_template: str, disable_provenance: bool = False):
         """The method includes a functionality to create or update a message template
 
         Args:
             name (str): Specify the message template name
             message_template (str): Specify the message template
+            disable_provenance (bool): Specify if the provenance header should be set or not (default False)
 
         Raises:
             ValueError: Missed specifying a necessary value
             Exception: Unspecified error by executing the API call
 
         Returns:
             None
@@ -584,14 +603,15 @@
 
         if len(name) != 0 and len(message_template) != 0:
             api_call: dict = Api(self.grafana_api_model).call_the_api(
                 f"{APIEndpoints.ALERTING_PROVISIONING.value}/templates/{name}",
                 RequestsMethods.PUT,
                 json.dumps({"template": message_template}),
                 response_status_code=True,
+                disable_provenance_header=disable_provenance,
             )
 
             if 200 <= api_call.get("status") >= 300:
                 logging.error(f"Check the error: {api_call}.")
                 raise Exception
             else:
                 logging.info("You successfully created/ updated the message template.")
```

### Comparing `grafana-api-sdk-0.1.0/grafana_api/annotations.py` & `grafana-api-sdk-0.1.1/grafana_api/annotations.py`

 * *Files identical despite different names*

### Comparing `grafana-api-sdk-0.1.0/grafana_api/api.py` & `grafana-api-sdk-0.1.1/grafana_api/api.py`

 * *Files 7% similar despite different names*

```diff
@@ -23,24 +23,26 @@
 
     def call_the_api(
         self,
         api_call: str,
         method: RequestsMethods = RequestsMethods.GET,
         json_complete: str = None,
         org_id_header: int = None,
+        disable_provenance_header: bool = False,
         response_status_code: bool = False,
     ) -> any:
         """The method execute a defined API call against the Grafana endpoints
 
         Args:
             api_call (str): Specify the API call endpoint
             method (RequestsMethods): Specify the used method (default GET)
             json_complete (str): Specify the inserted JSON as string
-            org_id_header (int): Specify the optional organization id for the corresponding API call
-            response_status_code (bool): Specify if the response should include the original status code
+            org_id_header (int): Specify the optional organization id as header for the corresponding API call
+            disable_provenance_header (bool): Specify the optional disable provenance as header for the corresponding API call (default False)
+            response_status_code (bool): Specify if the response should include the original status code (default False)
 
         Raises:
             Exception: Unspecified error by executing the API call
 
         Returns:
             api_call (any): Returns the value of the api call
         """
@@ -63,14 +65,17 @@
 
         headers["Content-Type"] = "application/json"
         headers["Accept"] = "application/json"
 
         if org_id_header is not None and type(org_id_header) == int:
             headers["X-Grafana-Org-Id"] = org_id_header
 
+        if type(disable_provenance_header) == bool and disable_provenance_header:
+            headers["X-Disable-Provenance"] = f"{disable_provenance_header}"
+
         http = urllib3.PoolManager(
             num_pools=self.grafana_api_model.num_pools,
             retries=self.grafana_api_model.retries,
             headers=headers,
             timeout=self.grafana_api_model.timeout,
             ssl_context=self.grafana_api_model.ssl_context,
         )
@@ -122,15 +127,15 @@
     def __check_the_api_call_response(
         response: any = None, response_status_code: bool = False
     ) -> any:
         """The method includes a functionality to check the output of API call method for errors
 
         Args:
             response (any): Specify the inserted response
-            response_status_code (bool): Specify if the original status code should be attached to the result
+            response_status_code (bool): Specify if the original status code should be attached to the result (default False)
 
         Raises:
             Exception: Unspecified error by executing the API call
 
         Returns:
             api_call (any): Returns the value of the api call
         """
```

### Comparing `grafana-api-sdk-0.1.0/grafana_api/authentication.py` & `grafana-api-sdk-0.1.1/grafana_api/authentication.py`

 * *Files identical despite different names*

### Comparing `grafana-api-sdk-0.1.0/grafana_api/correlations.py` & `grafana-api-sdk-0.1.1/grafana_api/correlations.py`

 * *Files identical despite different names*

### Comparing `grafana-api-sdk-0.1.0/grafana_api/dashboard.py` & `grafana-api-sdk-0.1.1/grafana_api/dashboard.py`

 * *Files identical despite different names*

### Comparing `grafana-api-sdk-0.1.0/grafana_api/datasource.py` & `grafana-api-sdk-0.1.1/grafana_api/datasource.py`

 * *Files identical despite different names*

### Comparing `grafana-api-sdk-0.1.0/grafana_api/external_group.py` & `grafana-api-sdk-0.1.1/grafana_api/external_group.py`

 * *Files identical despite different names*

### Comparing `grafana-api-sdk-0.1.0/grafana_api/folder.py` & `grafana-api-sdk-0.1.1/grafana_api/folder.py`

 * *Files identical despite different names*

### Comparing `grafana-api-sdk-0.1.0/grafana_api/legacy_alerting.py` & `grafana-api-sdk-0.1.1/grafana_api/legacy_alerting.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json
 import logging
+import re
 
 from .model import APIModel, APIEndpoints, RequestsMethods
 from .api import Api
 
 
 class Alerting:
     """The class includes all necessary methods to access the Grafana legacy alerting API endpoints
@@ -110,19 +111,29 @@
             ValueError: Missed specifying a necessary value
             Exception: Unspecified error by executing the API call
 
         Returns:
             api_call (dict): Returns an alert
         """
 
+        def _to_camel_case(input_value: str) -> str:
+            content = re.findall('[A-Z][^A-Z]*', input_value)
+            if content != list():
+                if len(content) != 1:
+                    return content[0].lower() + "".join(content[1:])
+                else:
+                    return content[0].lower()
+            return input_value
+
         if id != 0:
-            api_call: dict = Api(self.grafana_api_model).call_the_api(
+            api_call_raw: dict = Api(self.grafana_api_model).call_the_api(
                 f"{APIEndpoints.LEGACY_ALERTS.value}/{id}",
                 RequestsMethods.GET,
             )
+            api_call: dict = {_to_camel_case(k): v for k, v in api_call_raw.items()}
 
             if api_call == dict() or api_call.get("id") is None:
                 logging.error(f"Check the error: {api_call}.")
                 raise Exception
             else:
                 return api_call
         else:
```

### Comparing `grafana-api-sdk-0.1.0/grafana_api/legacy_playlist.py` & `grafana-api-sdk-0.1.1/grafana_api/legacy_playlist.py`

 * *Files identical despite different names*

### Comparing `grafana-api-sdk-0.1.0/grafana_api/library.py` & `grafana-api-sdk-0.1.1/grafana_api/library.py`

 * *Files identical despite different names*

### Comparing `grafana-api-sdk-0.1.0/grafana_api/licensing.py` & `grafana-api-sdk-0.1.1/grafana_api/licensing.py`

 * *Files identical despite different names*

### Comparing `grafana-api-sdk-0.1.0/grafana_api/model.py` & `grafana-api-sdk-0.1.1/grafana_api/model.py`

 * *Files identical despite different names*

### Comparing `grafana-api-sdk-0.1.0/grafana_api/organisation.py` & `grafana-api-sdk-0.1.1/grafana_api/organisation.py`

 * *Files identical despite different names*

### Comparing `grafana-api-sdk-0.1.0/grafana_api/other_http.py` & `grafana-api-sdk-0.1.1/grafana_api/other_http.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,22 +45,17 @@
 
         Raises:
             Exception: Unspecified error by executing the API call
 
         Returns:
             None
         """
+        api_call: dict = Api(self.grafana_api_model).call_the_api(f"{APIEndpoints.LOGIN.value}/ping")
 
-        api_call: str = (
-            Api(self.grafana_api_model)
-            .call_the_api(f"{APIEndpoints.LOGIN.value}/ping")
-            .data.decode("utf-8")
-        )
-
-        if api_call != "Logged in":
+        if api_call.get("message") != "Logged in":
             logging.error(f"Check the error: {api_call}.")
             raise Exception
         else:
             logging.info("You successfully destroyed the dashboard snapshot.")
 
     def get_health_status(self) -> dict:
         """The method includes a functionality to get the health information
```

### Comparing `grafana-api-sdk-0.1.0/grafana_api/playlist.py` & `grafana-api-sdk-0.1.1/grafana_api/playlist.py`

 * *Files identical despite different names*

### Comparing `grafana-api-sdk-0.1.0/grafana_api/preferences.py` & `grafana-api-sdk-0.1.1/grafana_api/preferences.py`

 * *Files identical despite different names*

### Comparing `grafana-api-sdk-0.1.0/grafana_api/query_history.py` & `grafana-api-sdk-0.1.1/grafana_api/query_history.py`

 * *Files identical despite different names*

### Comparing `grafana-api-sdk-0.1.0/grafana_api/rbac.py` & `grafana-api-sdk-0.1.1/grafana_api/rbac.py`

 * *Files identical despite different names*

### Comparing `grafana-api-sdk-0.1.0/grafana_api/reporting.py` & `grafana-api-sdk-0.1.1/grafana_api/reporting.py`

 * *Files identical despite different names*

### Comparing `grafana-api-sdk-0.1.0/grafana_api/search.py` & `grafana-api-sdk-0.1.1/grafana_api/search.py`

 * *Files identical despite different names*

### Comparing `grafana-api-sdk-0.1.0/grafana_api/service_account.py` & `grafana-api-sdk-0.1.1/grafana_api/service_account.py`

 * *Files identical despite different names*

### Comparing `grafana-api-sdk-0.1.0/grafana_api/short_url.py` & `grafana-api-sdk-0.1.1/grafana_api/short_url.py`

 * *Files identical despite different names*

### Comparing `grafana-api-sdk-0.1.0/grafana_api/snapshot.py` & `grafana-api-sdk-0.1.1/grafana_api/snapshot.py`

 * *Files identical despite different names*

### Comparing `grafana-api-sdk-0.1.0/grafana_api/team.py` & `grafana-api-sdk-0.1.1/grafana_api/team.py`

 * *Files identical despite different names*

### Comparing `grafana-api-sdk-0.1.0/grafana_api/user.py` & `grafana-api-sdk-0.1.1/grafana_api/user.py`

 * *Files identical despite different names*

### Comparing `grafana-api-sdk-0.1.0/grafana_api_sdk.egg-info/PKG-INFO` & `grafana-api-sdk-0.1.1/grafana_api_sdk.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grafana-api-sdk
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Grafana API SDK
 Home-page: https://github.com/ZPascal/grafana_api_sdk
 Author: Pascal Zimmermann
 Author-email: info@theiotstudio.com
 Project-URL: Source, https://github.com/ZPascal/grafana_api_sdk
 Project-URL: Bug Tracker, https://github.com/ZPascal/grafana_api_sdk/issues
 Project-URL: Documentation, https://zpascal.github.io/grafana_api_sdk/
```

### Comparing `grafana-api-sdk-0.1.0/grafana_api_sdk.egg-info/SOURCES.txt` & `grafana-api-sdk-0.1.1/grafana_api_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `grafana-api-sdk-0.1.0/setup.py` & `grafana-api-sdk-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     coverage_string: str = "![Coverage report](https://github.com/ZPascal/grafana_api_sdk/blob/main/docs/coverage.svg)"
     long_description: str = fh.read()
 
 long_description = long_description.replace(coverage_string, "")
 
 setuptools.setup(
     name="grafana-api-sdk",
-    version="0.1.0",
+    version="0.1.1",
     author="Pascal Zimmermann",
     author_email="info@theiotstudio.com",
     description="A Grafana API SDK",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ZPascal/grafana_api_sdk",
     project_urls={
```

