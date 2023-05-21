# Comparing `tmp/pydrawise-2023.5.1.tar.gz` & `tmp/pydrawise-2023.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydrawise-2023.5.1.tar", last modified: Wed May 17 12:58:45 2023, max compression
+gzip compressed data, was "pydrawise-2023.5.2.tar", last modified: Sun May 21 01:37:02 2023, max compression
```

## Comparing `pydrawise-2023.5.1.tar` & `pydrawise-2023.5.2.tar`

### file list

```diff
@@ -1,42 +1,50 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:58:45.942150 pydrawise-2023.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-05-17 12:58:25.000000 pydrawise-2023.5.1/.devcontainer.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:58:45.938151 pydrawise-2023.5.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-17 12:58:25.000000 pydrawise-2023.5.1/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-17 12:58:25.000000 pydrawise-2023.5.1/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:58:45.938151 pydrawise-2023.5.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-17 12:58:25.000000 pydrawise-2023.5.1/.github/workflows/build-and-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-17 12:58:25.000000 pydrawise-2023.5.1/.github/workflows/publish-python.yml
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-17 12:58:25.000000 pydrawise-2023.5.1/.github/workflows/release-drafter.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-17 12:58:25.000000 pydrawise-2023.5.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-05-17 12:58:25.000000 pydrawise-2023.5.1/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:58:45.942150 pydrawise-2023.5.1/.vscode/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-17 12:58:25.000000 pydrawise-2023.5.1/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-17 12:58:25.000000 pydrawise-2023.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-05-17 12:58:45.942150 pydrawise-2023.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-17 12:58:25.000000 pydrawise-2023.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)    50702 2023-05-17 12:58:25.000000 pydrawise-2023.5.1/hydrawise.graphql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:58:45.942150 pydrawise-2023.5.1/pydrawise/
--rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-17 12:58:25.000000 pydrawise-2023.5.1/pydrawise/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-17 12:58:45.000000 pydrawise-2023.5.1/pydrawise/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-05-17 12:58:25.000000 pydrawise-2023.5.1/pydrawise/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)    10136 2023-05-17 12:58:25.000000 pydrawise-2023.5.1/pydrawise/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-17 12:58:25.000000 pydrawise-2023.5.1/pydrawise/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10434 2023-05-17 12:58:25.000000 pydrawise-2023.5.1/pydrawise/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-05-17 12:58:25.000000 pydrawise-2023.5.1/pydrawise/schema_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:58:45.942150 pydrawise-2023.5.1/pydrawise.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-05-17 12:58:45.000000 pydrawise-2023.5.1/pydrawise.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-17 12:58:45.000000 pydrawise-2023.5.1/pydrawise.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 12:58:45.000000 pydrawise-2023.5.1/pydrawise.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-17 12:58:45.000000 pydrawise-2023.5.1/pydrawise.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-17 12:58:45.000000 pydrawise-2023.5.1/pydrawise.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 12:58:45.000000 pydrawise-2023.5.1/pydrawise.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-05-17 12:58:25.000000 pydrawise-2023.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-17 12:58:25.000000 pydrawise-2023.5.1/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-17 12:58:25.000000 pydrawise-2023.5.1/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-17 12:58:25.000000 pydrawise-2023.5.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 12:58:45.942150 pydrawise-2023.5.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 12:58:45.942150 pydrawise-2023.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 12:58:25.000000 pydrawise-2023.5.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-05-17 12:58:25.000000 pydrawise-2023.5.1/tests/test_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     9594 2023-05-17 12:58:25.000000 pydrawise-2023.5.1/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-17 12:58:25.000000 pydrawise-2023.5.1/tests/test_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 01:37:02.324782 pydrawise-2023.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-05-21 01:36:46.000000 pydrawise-2023.5.2/.devcontainer.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 01:37:02.320783 pydrawise-2023.5.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-21 01:36:46.000000 pydrawise-2023.5.2/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-21 01:36:46.000000 pydrawise-2023.5.2/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 01:37:02.320783 pydrawise-2023.5.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-05-21 01:36:46.000000 pydrawise-2023.5.2/.github/workflows/build-and-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-21 01:36:46.000000 pydrawise-2023.5.2/.github/workflows/publish-python.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-21 01:36:46.000000 pydrawise-2023.5.2/.github/workflows/release-drafter.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1799 2023-05-21 01:36:46.000000 pydrawise-2023.5.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-05-21 01:36:46.000000 pydrawise-2023.5.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-21 01:36:46.000000 pydrawise-2023.5.2/.readthedocs.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 01:37:02.320783 pydrawise-2023.5.2/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-21 01:36:46.000000 pydrawise-2023.5.2/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-21 01:36:46.000000 pydrawise-2023.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-05-21 01:37:02.324782 pydrawise-2023.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-05-21 01:36:46.000000 pydrawise-2023.5.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 01:37:02.320783 pydrawise-2023.5.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-05-21 01:36:46.000000 pydrawise-2023.5.2/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 01:37:02.324782 pydrawise-2023.5.2/docs/reference/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-21 01:36:46.000000 pydrawise-2023.5.2/docs/reference/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-21 01:36:46.000000 pydrawise-2023.5.2/docs/reference/schema.md
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-21 01:36:46.000000 pydrawise-2023.5.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    50702 2023-05-21 01:36:46.000000 pydrawise-2023.5.2/hydrawise.graphql
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-21 01:36:46.000000 pydrawise-2023.5.2/mkdocs.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 01:37:02.324782 pydrawise-2023.5.2/pydrawise/
+-rw-r--r--   0 runner    (1001) docker     (123)      505 2023-05-21 01:36:46.000000 pydrawise-2023.5.2/pydrawise/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-21 01:37:02.000000 pydrawise-2023.5.2/pydrawise/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-05-21 01:36:46.000000 pydrawise-2023.5.2/pydrawise/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9503 2023-05-21 01:36:46.000000 pydrawise-2023.5.2/pydrawise/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-21 01:36:46.000000 pydrawise-2023.5.2/pydrawise/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10831 2023-05-21 01:36:46.000000 pydrawise-2023.5.2/pydrawise/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-05-21 01:36:46.000000 pydrawise-2023.5.2/pydrawise/schema_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 01:37:02.324782 pydrawise-2023.5.2/pydrawise.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-05-21 01:37:02.000000 pydrawise-2023.5.2/pydrawise.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-21 01:37:02.000000 pydrawise-2023.5.2/pydrawise.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 01:37:02.000000 pydrawise-2023.5.2/pydrawise.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-21 01:37:02.000000 pydrawise-2023.5.2/pydrawise.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-21 01:37:02.000000 pydrawise-2023.5.2/pydrawise.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 01:37:02.000000 pydrawise-2023.5.2/pydrawise.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1370 2023-05-21 01:36:46.000000 pydrawise-2023.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-21 01:36:46.000000 pydrawise-2023.5.2/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-21 01:36:46.000000 pydrawise-2023.5.2/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-21 01:36:46.000000 pydrawise-2023.5.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 01:37:02.324782 pydrawise-2023.5.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 01:37:02.324782 pydrawise-2023.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 01:36:46.000000 pydrawise-2023.5.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2341 2023-05-21 01:36:46.000000 pydrawise-2023.5.2/tests/test_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9623 2023-05-21 01:36:46.000000 pydrawise-2023.5.2/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-21 01:36:46.000000 pydrawise-2023.5.2/tests/test_schema.py
```

### Comparing `pydrawise-2023.5.1/.devcontainer.json` & `pydrawise-2023.5.2/.devcontainer.json`

 * *Files identical despite different names*

### Comparing `pydrawise-2023.5.1/.github/workflows/build-and-test.yml` & `pydrawise-2023.5.2/.github/workflows/build-and-test.yml`

 * *Files identical despite different names*

### Comparing `pydrawise-2023.5.1/.github/workflows/publish-python.yml` & `pydrawise-2023.5.2/.github/workflows/publish-python.yml`

 * *Files identical despite different names*

### Comparing `pydrawise-2023.5.1/.gitignore` & `pydrawise-2023.5.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pydrawise-2023.5.1/.pre-commit-config.yaml` & `pydrawise-2023.5.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pydrawise-2023.5.1/LICENSE` & `pydrawise-2023.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pydrawise-2023.5.1/hydrawise.graphql` & `pydrawise-2023.5.2/hydrawise.graphql`

 * *Files identical despite different names*

### Comparing `pydrawise-2023.5.1/pydrawise/auth.py` & `pydrawise-2023.5.2/pydrawise/auth.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,15 +13,19 @@
 DEFAULT_TIMEOUT = 60
 
 
 class Auth:
     """Authentication support for the Hydrawise GraphQL API."""
 
     def __init__(self, username: str, password: str) -> None:
-        """Initializer."""
+        """Initializer.
+
+        :param username: The username to use for authenticating with the Hydrawise service.
+        :param password: The password to use for authenticating with the Hydrawise service.
+        """
         self.__username = username
         self.__password = password
         self._lock = Lock()
         self._token: str | None = None
         self._token_type: str | None = None
         self._token_expires: datetime | None = None
         self._refresh_token: str | None = None
```

### Comparing `pydrawise-2023.5.1/pydrawise/client.py` & `pydrawise-2023.5.2/pydrawise/client.py`

 * *Files 7% similar despite different names*

```diff
@@ -45,15 +45,14 @@
     Should be instantiated with an Auth object that handles authentication and low-level transport.
     """
 
     def __init__(self, auth: Auth) -> None:
         """Initializes the client.
 
         :param auth: Handles authentication and transport.
-        :type auth: Auth
         """
         self._auth = auth
         self._schema = DSLSchema(_get_schema())
 
     async def _client(self) -> Client:
         headers = {"Authorization": await self._auth.token()}
         transport = AIOHTTPTransport(url=API_URL, headers=headers)
@@ -97,41 +96,38 @@
         result = await self._query(selector)
         return deserialize(list[Controller], result["me"]["controllers"])
 
     async def get_controller(self, controller_id: int) -> Controller:
         """Retrieves a single controller by its unique identifier.
 
         :param controller_id: Unique identifier for the controller to retrieve.
-        :type controller_id: int
         :rtype: Controller
         """
         selector = self._schema.Query.controller(controllerId=controller_id).select(
             *get_selectors(self._schema, Controller),
         )
         result = await self._query(selector)
         return deserialize(Controller, result["controller"])
 
     async def get_zones(self, controller: Controller) -> list[Zone]:
         """Retrieves zones associated with the given controller.
 
         :param controller: Controller whose zones to fetch.
-        :type controller: Controller
         :rtype: list[Zone]
         """
         selector = self._schema.Query.controller(controllerId=controller.id).select(
             self._schema.Controller.zones.select(*get_selectors(self._schema, Zone)),
         )
         result = await self._query(selector)
         return deserialize(list[Zone], result["controller"]["zones"])
 
     async def get_zone(self, zone_id: int) -> Zone:
         """Retrieves a zone by its unique identifier.
 
         :param zone_id: The zone's unique identifier.
-        :type zone_id: int
         :rtype: Zone
         """
         selector = self._schema.Query.zone(zoneId=zone_id).select(
             *get_selectors(self._schema, Zone)
         )
         result = await self._query(selector)
         return deserialize(Zone, result["zone"])
@@ -141,20 +137,17 @@
         zone: Zone,
         mark_run_as_scheduled: bool = False,
         custom_run_duration: int = 0,
     ):
         """Starts a zone's run cycle.
 
         :param zone: The zone to start.
-        :type zone: Zone
         :param mark_run_as_scheduled: Whether to mark the zone as having run as scheduled.
-        :type mark_run_as_scheduled: bool
         :param custom_run_duration: Duration (in seconds) to run the zone. If not
             specified (or zero), will run for its default configured time.
-        :type custom_run_duration: int
         """
         kwargs = {
             "zoneId": zone.id,
             "markRunAsScheduled": mark_run_as_scheduled,
         }
         if custom_run_duration > 0:
             kwargs["customRunDuration"] = custom_run_duration
@@ -164,15 +157,14 @@
         )
         await self._mutation(selector)
 
     async def stop_zone(self, zone: Zone):
         """Stops a zone.
 
         :param zone: The zone to stop.
-        :type zone: Zone
         """
         selector = self._schema.Mutation.stopZone.args(zoneId=zone.id).select(
             *get_selectors(self._schema, StatusCodeAndSummary),
         )
         await self._mutation(selector)
 
     async def start_all_zones(
@@ -180,20 +172,17 @@
         controller: Controller,
         mark_run_as_scheduled: bool = False,
         custom_run_duration: int = 0,
     ):
         """Starts all zones attached to a controller.
 
         :param controller: The controller whose zones to start.
-        :type controller: Controller
         :param mark_run_as_scheduled: Whether to mark the zones as having run as scheduled.
-        :type mark_run_as_scheduled: bool
         :param custom_run_duration: Duration (in seconds) to run the zones. If not
             specified (or zero), will run for each zone's default configured time.
-        :type custom_run_duration: int
         """
         kwargs = {
             "controllerId": controller.id,
             "markRunAsScheduled": mark_run_as_scheduled,
         }
         if custom_run_duration > 0:
             kwargs["customRunDuration"] = custom_run_duration
@@ -203,84 +192,76 @@
         )
         await self._mutation(selector)
 
     async def stop_all_zones(self, controller: Controller):
         """Stops all zones attached to a controller.
 
         :param controller: The controller whose zones to stop.
-        :type controller: Controller
         """
         selector = self._schema.Mutation.stopAllZones.args(
             controllerId=controller.id
         ).select(
             *get_selectors(self._schema, StatusCodeAndSummary),
         )
         await self._mutation(selector)
 
     async def suspend_zone(self, zone: Zone, until: datetime):
         """Suspends a zone's schedule.
 
         :param zone: The zone to suspend.
-        :type zone: Zone
         :param until: When the suspension should end.
-        :type until: datetime
         """
         selector = self._schema.Mutation.suspendZone.args(
             zoneId=zone.id,
             until=DateTime.to_json(until).value,
         ).select(
             *get_selectors(self._schema, StatusCodeAndSummary),
         )
         await self._mutation(selector)
 
     async def resume_zone(self, zone: Zone):
         """Resumes a zone's schedule.
 
         :param zone: The zone whose schedule to resume.
-        :type zone: Zone
         """
         selector = self._schema.Mutation.resumeZone.args(zoneId=zone.id).select(
             *get_selectors(self._schema, StatusCodeAndSummary),
         )
         await self._mutation(selector)
 
     async def suspend_all_zones(self, controller: Controller, until: datetime):
         """Suspends the schedule of all zones attached to a given controller.
 
         :param controller: The controller whose zones to suspend.
-        :type controller: Controller
         :param until: When the suspension should end.
-        :type until: datetime
         """
         selector = self._schema.Mutation.suspendAllZones.args(
             controllerId=controller.id,
             until=DateTime.to_json(until).value,
         ).select(
             *get_selectors(self._schema, StatusCodeAndSummary),
         )
         await self._mutation(selector)
 
     async def resume_all_zones(self, controller: Controller):
         """Resumes the schedule of all zones attached to the given controller.
 
         :param controller: The controller whose zones to resume.
-        :type controller: Controller
         """
         selector = self._schema.Mutation.resumeAllZones.args(
             controllerId=controller.id
         ).select(
             *get_selectors(self._schema, StatusCodeAndSummary),
         )
         await self._mutation(selector)
 
     async def delete_zone_suspension(self, suspension: ZoneSuspension):
         """Removes a specific zone suspension.
 
         Useful when there are multiple suspensions for a zone in effect.
 
         :param suspension: The suspension to delete.
-        :type suspension: ZoneSuspension
         """
         selector = self._schema.Mutation.deleteZoneSuspension.args(
             id=suspension.id
         ).select()
         await self._mutation(selector)
```

### Comparing `pydrawise-2023.5.1/pydrawise/schema.py` & `pydrawise-2023.5.2/pydrawise/schema.py`

 * *Files 7% similar despite different names*

```diff
@@ -80,18 +80,28 @@
         """Returns a GraphQL conversion for a DateTime."""
         return conversion(
             Conversion(DateTime.from_json, source=DateTime, target=datetime),
             Conversion(DateTime.to_json, source=datetime, target=DateTime),
         )
 
 
-duration_conversion = conversion(
-    Conversion(lambda d: timedelta(minutes=d), source=int, target=timedelta),
-    Conversion(lambda d: d.minutes, source=timedelta, target=int),
-)
+def _duration_conversion(unit: str) -> conversion:
+    assert unit in (
+        "days",
+        "seconds",
+        "microseconds",
+        "milliseconds",
+        "minutes",
+        "hours",
+        "weeks",
+    )
+    return conversion(
+        Conversion(lambda d: timedelta(**{unit: d}), source=int, target=timedelta),
+        Conversion(lambda d: getattr(d, unit), source=timedelta, target=int),
+    )
 
 
 @dataclass
 class BaseZone:
     """Basic zone information."""
 
     id: int
@@ -99,24 +109,24 @@
     name: str
 
 
 @dataclass
 class CycleAndSoakSettings:
     """Cycle and soak durations."""
 
-    cycle_duration: timedelta = field(metadata=duration_conversion)
-    soak_duration: timedelta = field(metadata=duration_conversion)
+    cycle_duration: timedelta = field(metadata=_duration_conversion("minutes"))
+    soak_duration: timedelta = field(metadata=_duration_conversion("minutes"))
 
 
 @dataclass
 class RunTimeGroup:
     """The runtime of a watering program group."""
 
     id: int
-    duration: timedelta = field(metadata=duration_conversion)
+    duration: timedelta = field(metadata=_duration_conversion("minutes"))
 
 
 @dataclass
 class AdvancedProgram:
     """An advanced watering program."""
 
     advanced_program_id: int
@@ -202,16 +212,17 @@
 @dataclass
 class ScheduledZoneRun:
     """A scheduled zone run."""
 
     id: str
     start_time: datetime = field(metadata=DateTime.conversion())
     end_time: datetime = field(metadata=DateTime.conversion())
-    normal_duration: timedelta = field(metadata=duration_conversion)
-    duration: timedelta = field(metadata=duration_conversion)
+    normal_duration: timedelta = field(metadata=_duration_conversion("minutes"))
+    duration: timedelta = field(metadata=_duration_conversion("minutes"))
+    remaining_time: timedelta = field(metadata=_duration_conversion("seconds"))
     status: RunStatus
 
 
 @dataclass
 class ScheduledZoneRuns:
     """Scheduled runs for a zone."""
 
@@ -323,15 +334,15 @@
     status: SensorStatus
 
 
 @dataclass
 class WaterTime:
     """A water time duration."""
 
-    value: timedelta = field(metadata=duration_conversion)
+    value: timedelta = field(metadata=_duration_conversion("minutes"))
 
 
 @dataclass
 class ControllerStatus:
     """Current status of a controller."""
 
     summary: str
@@ -359,14 +370,15 @@
 
 
 @dataclass
 class User:
     """A Hydrawise user account."""
 
     id: int
+    customer_id: int
     name: str
     email: str
     controllers: list[Controller] = field(
         default_factory=list, metadata=skip(deserialization=True)
     )
```

### Comparing `pydrawise-2023.5.1/pydrawise/schema_utils.py` & `pydrawise-2023.5.2/pydrawise/schema_utils.py`

 * *Files identical despite different names*

### Comparing `pydrawise-2023.5.1/pydrawise.egg-info/SOURCES.txt` & `pydrawise-2023.5.2/pydrawise.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,30 @@
 .devcontainer.json
 .gitignore
 .pre-commit-config.yaml
+.readthedocs.yaml
 LICENSE
 README.md
 hydrawise.graphql
+mkdocs.yml
 pyproject.toml
 pytest.ini
 requirements-test.txt
 requirements.txt
 setup.cfg
 .github/dependabot.yml
 .github/release-drafter.yml
 .github/workflows/build-and-test.yml
 .github/workflows/publish-python.yml
 .github/workflows/release-drafter.yml
 .vscode/settings.json
+docs/index.md
+docs/requirements.txt
+docs/reference/index.md
+docs/reference/schema.md
 pydrawise/__init__.py
 pydrawise/_version.py
 pydrawise/auth.py
 pydrawise/client.py
 pydrawise/exceptions.py
 pydrawise/schema.py
 pydrawise/schema_utils.py
```

### Comparing `pydrawise-2023.5.1/pyproject.toml` & `pydrawise-2023.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pydrawise-2023.5.1/tests/test_auth.py` & `pydrawise-2023.5.2/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `pydrawise-2023.5.1/tests/test_client.py` & `pydrawise-2023.5.2/tests/test_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,14 +110,15 @@
     }
 
 
 async def test_get_user(api: Hydrawise, mock_session):
     mock_session.execute.return_value = {
         "me": {
             "id": 1234,
+            "customerId": 1,
             "name": "My Name",
             "email": "me@asdf.com",
         }
     }
     user = await api.get_user()
     assert user.id == 1234
     assert user.name == "My Name"
```

