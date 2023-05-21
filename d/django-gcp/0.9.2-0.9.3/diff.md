# Comparing `tmp/django_gcp-0.9.2.tar.gz` & `tmp/django_gcp-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_gcp-0.9.2.tar", max compression
+gzip compressed data, was "django_gcp-0.9.3.tar", max compression
```

## Comparing `django_gcp-0.9.2.tar` & `django_gcp-0.9.3.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0     1080 2023-05-18 07:55:48.665574 django_gcp-0.9.2/LICENSE
--rw-r--r--   0        0        0     3746 2023-05-18 07:55:48.665574 django_gcp-0.9.2/README.md
--rw-r--r--   0        0        0       58 2023-05-18 07:55:48.665574 django_gcp-0.9.2/django_gcp/__init__.py
--rw-r--r--   0        0        0      627 2023-05-18 07:55:48.665574 django_gcp-0.9.2/django_gcp/apps.py
--rw-r--r--   0        0        0        0 2023-05-18 07:55:48.665574 django_gcp-0.9.2/django_gcp/events/__init__.py
--rw-r--r--   0        0        0       63 2023-05-18 07:55:48.665574 django_gcp-0.9.2/django_gcp/events/signals.py
--rw-r--r--   0        0        0     7279 2023-05-18 07:55:48.665574 django_gcp-0.9.2/django_gcp/events/utils.py
--rw-r--r--   0        0        0     1703 2023-05-18 07:55:48.665574 django_gcp-0.9.2/django_gcp/events/views.py
--rw-r--r--   0        0        0     1450 2023-05-18 07:55:48.665574 django_gcp-0.9.2/django_gcp/exceptions.py
--rw-r--r--   0        0        0      189 2023-05-18 07:55:48.665574 django_gcp-0.9.2/django_gcp/logging/__init__.py
--rw-r--r--   0        0        0     2212 2023-05-18 07:55:48.665574 django_gcp-0.9.2/django_gcp/logging/error_reporting.py
--rw-r--r--   0        0        0     1765 2023-05-18 07:55:48.665574 django_gcp-0.9.2/django_gcp/logging/structured_logs.py
--rw-r--r--   0        0        0        0 2023-05-18 07:55:48.665574 django_gcp-0.9.2/django_gcp/management/__init__.py
--rw-r--r--   0        0        0        0 2023-05-18 07:55:48.665574 django_gcp-0.9.2/django_gcp/management/commands/__init__.py
--rw-r--r--   0        0        0      816 2023-05-18 07:55:48.665574 django_gcp-0.9.2/django_gcp/management/commands/_base.py
--rw-r--r--   0        0        0     1637 2023-05-18 07:55:48.665574 django_gcp-0.9.2/django_gcp/management/commands/cleanup_tmp_files.py
--rw-r--r--   0        0        0     1760 2023-05-18 07:55:48.665574 django_gcp-0.9.2/django_gcp/management/commands/task_manager.py
--rw-r--r--   0        0        0       96 2023-05-18 07:55:48.665574 django_gcp-0.9.2/django_gcp/metadata/__init__.py
--rw-r--r--   0        0        0     3410 2023-05-18 07:55:48.665574 django_gcp-0.9.2/django_gcp/metadata/metadata.py
--rw-r--r--   0        0        0      170 2023-05-18 07:55:48.665574 django_gcp-0.9.2/django_gcp/signals.py
--rw-r--r--   0        0        0        0 2023-05-18 07:55:48.665574 django_gcp-0.9.2/django_gcp/static/.gitignore
--rw-r--r--   0        0        0     2630 2023-05-18 07:55:48.665574 django_gcp-0.9.2/django_gcp/static/django_gcp/cloud_object_widget.css
--rw-r--r--   0        0        0     7686 2023-05-18 07:55:48.665574 django_gcp-0.9.2/django_gcp/static/django_gcp/cloud_object_widget.js
--rw-r--r--   0        0        0      328 2023-05-18 07:55:48.665574 django_gcp-0.9.2/django_gcp/storage/__init__.py
--rw-r--r--   0        0        0     1431 2023-05-18 07:55:48.665574 django_gcp-0.9.2/django_gcp/storage/compress.py
--rw-r--r--   0        0        0    22857 2023-05-18 07:55:48.665574 django_gcp-0.9.2/django_gcp/storage/fields.py
--rw-r--r--   0        0        0     2595 2023-05-18 07:55:48.665574 django_gcp-0.9.2/django_gcp/storage/forms.py
--rw-r--r--   0        0        0    14266 2023-05-18 07:55:48.665574 django_gcp-0.9.2/django_gcp/storage/gcloud.py
--rw-r--r--   0        0        0     6373 2023-05-18 07:55:48.665574 django_gcp-0.9.2/django_gcp/storage/operations.py
--rw-r--r--   0        0        0     4427 2023-05-18 07:55:48.665574 django_gcp-0.9.2/django_gcp/storage/settings.py
--rw-r--r--   0        0        0     3202 2023-05-18 07:55:48.665574 django_gcp-0.9.2/django_gcp/storage/utils.py
--rw-r--r--   0        0        0     1942 2023-05-18 07:55:48.665574 django_gcp-0.9.2/django_gcp/storage/widgets.py
--rw-r--r--   0        0        0      192 2023-05-18 07:55:48.665574 django_gcp-0.9.2/django_gcp/tasks/__init__.py
--rw-r--r--   0        0        0     1124 2023-05-18 07:55:48.665574 django_gcp-0.9.2/django_gcp/tasks/_patch_cloud_scheduler.py
--rw-r--r--   0        0        0     1106 2023-05-18 07:55:48.665574 django_gcp-0.9.2/django_gcp/tasks/_patch_cloud_tasks.py
--rw-r--r--   0        0        0      350 2023-05-18 07:55:48.665574 django_gcp-0.9.2/django_gcp/tasks/helpers.py
--rw-r--r--   0        0        0     8860 2023-05-18 07:55:48.665574 django_gcp-0.9.2/django_gcp/tasks/manager.py
--rw-r--r--   0        0        0     1307 2023-05-18 07:55:48.665574 django_gcp-0.9.2/django_gcp/tasks/serializers.py
--rw-r--r--   0        0        0    11797 2023-05-18 07:55:48.665574 django_gcp-0.9.2/django_gcp/tasks/tasks.py
--rw-r--r--   0        0        0     1836 2023-05-18 07:55:48.669574 django_gcp-0.9.2/django_gcp/tasks/views.py
--rw-r--r--   0        0        0        0 2023-05-18 07:55:48.669574 django_gcp-0.9.2/django_gcp/templates/django_gcp/.gitignore
--rw-r--r--   0        0        0     2571 2023-05-18 07:55:48.669574 django_gcp-0.9.2/django_gcp/templates/django_gcp/cloud_object_widget.html
--rw-r--r--   0        0        0      491 2023-05-18 07:55:48.669574 django_gcp-0.9.2/django_gcp/urls.py
--rw-r--r--   0        0        0     1651 2023-05-18 07:55:48.677574 django_gcp-0.9.2/pyproject.toml
--rw-r--r--   0        0        0     5086 1970-01-01 00:00:00.000000 django_gcp-0.9.2/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-05-21 09:38:49.572470 django_gcp-0.9.3/LICENSE
+-rw-r--r--   0        0        0     3746 2023-05-21 09:38:49.572470 django_gcp-0.9.3/README.md
+-rw-r--r--   0        0        0       58 2023-05-21 09:38:49.572470 django_gcp-0.9.3/django_gcp/__init__.py
+-rw-r--r--   0        0        0      627 2023-05-21 09:38:49.572470 django_gcp-0.9.3/django_gcp/apps.py
+-rw-r--r--   0        0        0        0 2023-05-21 09:38:49.572470 django_gcp-0.9.3/django_gcp/events/__init__.py
+-rw-r--r--   0        0        0       63 2023-05-21 09:38:49.572470 django_gcp-0.9.3/django_gcp/events/signals.py
+-rw-r--r--   0        0        0     7279 2023-05-21 09:38:49.572470 django_gcp-0.9.3/django_gcp/events/utils.py
+-rw-r--r--   0        0        0     1703 2023-05-21 09:38:49.572470 django_gcp-0.9.3/django_gcp/events/views.py
+-rw-r--r--   0        0        0     1450 2023-05-21 09:38:49.572470 django_gcp-0.9.3/django_gcp/exceptions.py
+-rw-r--r--   0        0        0      189 2023-05-21 09:38:49.572470 django_gcp-0.9.3/django_gcp/logging/__init__.py
+-rw-r--r--   0        0        0     2212 2023-05-21 09:38:49.572470 django_gcp-0.9.3/django_gcp/logging/error_reporting.py
+-rw-r--r--   0        0        0     1765 2023-05-21 09:38:49.572470 django_gcp-0.9.3/django_gcp/logging/structured_logs.py
+-rw-r--r--   0        0        0        0 2023-05-21 09:38:49.572470 django_gcp-0.9.3/django_gcp/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-21 09:38:49.572470 django_gcp-0.9.3/django_gcp/management/commands/__init__.py
+-rw-r--r--   0        0        0      816 2023-05-21 09:38:49.572470 django_gcp-0.9.3/django_gcp/management/commands/_base.py
+-rw-r--r--   0        0        0     1637 2023-05-21 09:38:49.572470 django_gcp-0.9.3/django_gcp/management/commands/cleanup_tmp_files.py
+-rw-r--r--   0        0        0     1760 2023-05-21 09:38:49.572470 django_gcp-0.9.3/django_gcp/management/commands/task_manager.py
+-rw-r--r--   0        0        0       96 2023-05-21 09:38:49.572470 django_gcp-0.9.3/django_gcp/metadata/__init__.py
+-rw-r--r--   0        0        0     3410 2023-05-21 09:38:49.572470 django_gcp-0.9.3/django_gcp/metadata/metadata.py
+-rw-r--r--   0        0        0      170 2023-05-21 09:38:49.572470 django_gcp-0.9.3/django_gcp/signals.py
+-rw-r--r--   0        0        0        0 2023-05-21 09:38:49.572470 django_gcp-0.9.3/django_gcp/static/.gitignore
+-rw-r--r--   0        0        0     2630 2023-05-21 09:38:49.572470 django_gcp-0.9.3/django_gcp/static/django_gcp/cloud_object_widget.css
+-rw-r--r--   0        0        0     7686 2023-05-21 09:38:49.572470 django_gcp-0.9.3/django_gcp/static/django_gcp/cloud_object_widget.js
+-rw-r--r--   0        0        0      328 2023-05-21 09:38:49.572470 django_gcp-0.9.3/django_gcp/storage/__init__.py
+-rw-r--r--   0        0        0     1431 2023-05-21 09:38:49.572470 django_gcp-0.9.3/django_gcp/storage/compress.py
+-rw-r--r--   0        0        0    23057 2023-05-21 09:38:49.572470 django_gcp-0.9.3/django_gcp/storage/fields.py
+-rw-r--r--   0        0        0     2595 2023-05-21 09:38:49.572470 django_gcp-0.9.3/django_gcp/storage/forms.py
+-rw-r--r--   0        0        0    14266 2023-05-21 09:38:49.572470 django_gcp-0.9.3/django_gcp/storage/gcloud.py
+-rw-r--r--   0        0        0     6373 2023-05-21 09:38:49.572470 django_gcp-0.9.3/django_gcp/storage/operations.py
+-rw-r--r--   0        0        0     4427 2023-05-21 09:38:49.572470 django_gcp-0.9.3/django_gcp/storage/settings.py
+-rw-r--r--   0        0        0     3202 2023-05-21 09:38:49.572470 django_gcp-0.9.3/django_gcp/storage/utils.py
+-rw-r--r--   0        0        0     1942 2023-05-21 09:38:49.572470 django_gcp-0.9.3/django_gcp/storage/widgets.py
+-rw-r--r--   0        0        0      192 2023-05-21 09:38:49.572470 django_gcp-0.9.3/django_gcp/tasks/__init__.py
+-rw-r--r--   0        0        0     1124 2023-05-21 09:38:49.572470 django_gcp-0.9.3/django_gcp/tasks/_patch_cloud_scheduler.py
+-rw-r--r--   0        0        0     1106 2023-05-21 09:38:49.572470 django_gcp-0.9.3/django_gcp/tasks/_patch_cloud_tasks.py
+-rw-r--r--   0        0        0      350 2023-05-21 09:38:49.572470 django_gcp-0.9.3/django_gcp/tasks/helpers.py
+-rw-r--r--   0        0        0     8860 2023-05-21 09:38:49.572470 django_gcp-0.9.3/django_gcp/tasks/manager.py
+-rw-r--r--   0        0        0     1307 2023-05-21 09:38:49.572470 django_gcp-0.9.3/django_gcp/tasks/serializers.py
+-rw-r--r--   0        0        0    11797 2023-05-21 09:38:49.572470 django_gcp-0.9.3/django_gcp/tasks/tasks.py
+-rw-r--r--   0        0        0     1836 2023-05-21 09:38:49.572470 django_gcp-0.9.3/django_gcp/tasks/views.py
+-rw-r--r--   0        0        0        0 2023-05-21 09:38:49.572470 django_gcp-0.9.3/django_gcp/templates/django_gcp/.gitignore
+-rw-r--r--   0        0        0     2571 2023-05-21 09:38:49.572470 django_gcp-0.9.3/django_gcp/templates/django_gcp/cloud_object_widget.html
+-rw-r--r--   0        0        0      491 2023-05-21 09:38:49.572470 django_gcp-0.9.3/django_gcp/urls.py
+-rw-r--r--   0        0        0     1651 2023-05-21 09:38:49.576470 django_gcp-0.9.3/pyproject.toml
+-rw-r--r--   0        0        0     5086 1970-01-01 00:00:00.000000 django_gcp-0.9.3/PKG-INFO
```

### Comparing `django_gcp-0.9.2/LICENSE` & `django_gcp-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `django_gcp-0.9.2/README.md` & `django_gcp-0.9.3/README.md`

 * *Files identical despite different names*

### Comparing `django_gcp-0.9.2/django_gcp/apps.py` & `django_gcp-0.9.3/django_gcp/apps.py`

 * *Files identical despite different names*

### Comparing `django_gcp-0.9.2/django_gcp/events/utils.py` & `django_gcp-0.9.3/django_gcp/events/utils.py`

 * *Files identical despite different names*

### Comparing `django_gcp-0.9.2/django_gcp/events/views.py` & `django_gcp-0.9.3/django_gcp/events/views.py`

 * *Files identical despite different names*

### Comparing `django_gcp-0.9.2/django_gcp/exceptions.py` & `django_gcp-0.9.3/django_gcp/exceptions.py`

 * *Files identical despite different names*

### Comparing `django_gcp-0.9.2/django_gcp/logging/error_reporting.py` & `django_gcp-0.9.3/django_gcp/logging/error_reporting.py`

 * *Files identical despite different names*

### Comparing `django_gcp-0.9.2/django_gcp/logging/structured_logs.py` & `django_gcp-0.9.3/django_gcp/logging/structured_logs.py`

 * *Files identical despite different names*

### Comparing `django_gcp-0.9.2/django_gcp/management/commands/_base.py` & `django_gcp-0.9.3/django_gcp/management/commands/_base.py`

 * *Files identical despite different names*

### Comparing `django_gcp-0.9.2/django_gcp/management/commands/cleanup_tmp_files.py` & `django_gcp-0.9.3/django_gcp/management/commands/cleanup_tmp_files.py`

 * *Files identical despite different names*

### Comparing `django_gcp-0.9.2/django_gcp/management/commands/task_manager.py` & `django_gcp-0.9.3/django_gcp/management/commands/task_manager.py`

 * *Files identical despite different names*

### Comparing `django_gcp-0.9.2/django_gcp/metadata/metadata.py` & `django_gcp-0.9.3/django_gcp/metadata/metadata.py`

 * *Files identical despite different names*

### Comparing `django_gcp-0.9.2/django_gcp/static/django_gcp/cloud_object_widget.css` & `django_gcp-0.9.3/django_gcp/static/django_gcp/cloud_object_widget.css`

 * *Files identical despite different names*

### Comparing `django_gcp-0.9.2/django_gcp/static/django_gcp/cloud_object_widget.js` & `django_gcp-0.9.3/django_gcp/static/django_gcp/cloud_object_widget.js`

 * *Files identical despite different names*

### Comparing `django_gcp-0.9.2/django_gcp/storage/compress.py` & `django_gcp-0.9.3/django_gcp/storage/compress.py`

 * *Files identical despite different names*

### Comparing `django_gcp-0.9.2/django_gcp/storage/fields.py` & `django_gcp-0.9.3/django_gcp/storage/fields.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,61 +19,77 @@
 
 # 32 megabyte default size chosen to be consistent with Cloud Run's
 # largest request size
 DEFAULT_MAX_SIZE_BYTES = 32 * 1024 * 1024
 
 DEFAULT_OVERWRITE_MODE = "never"
 
+OVERWRITE_MODES = [
+    "never",
+    "update",
+    "update-versioned",
+    "add",
+    "add-versioned",
+    "add-update",
+    "add-update-versioned",
+]
+
 DEFAULT_OVERRIDE_BLOBFIELD_VALUE = False
 
 
 class BlobField(models.JSONField):
     """A FileField replacement with cloud store object-specific features
 
     Features such as metadata fetching/synchronisation and direct uploads are enabled.
 
-    ObjectField allows storage classes to be declared in settings. This enables:
+    BlobField allows storage classes to be declared in settings. This enables:
     - storages to be switched without database migrations (supporting integration
       and release preview type workflows plus cloud migration)
-    - eaiser way of using different buckets for different ObjectFields without
+    - eaiser way of using different buckets for different BlobFields without
       defining a Storage class for each bucket
 
-    ObjectField is built on JSONField to allow more complex information to be stored
+    BlobField is built on JSONField to allow more complex information to be stored
     and queried. Examples might include:
      - cached object generation or metageneration,
      - cached object metadata, or
      - status of direct uploads
 
-    ObjectField does not inherit directly from FileField to avoid the burden of strict
+    BlobField does not inherit directly from FileField to avoid the burden of strict
     compatibility with legacy or irrelevant-to-cloud-storage behaviour (like django
     admin overriding formfields or coping with edge cases around name and path handling).
     We do this to support a clear and maintainable implementation.
 
-    ObjectField can read FileField entries: since FileField stores the path as a string,
-    that's valid JSON so can be accepted by ObjectField, greatly simplifying migration.
-    Once a model instance has been updated, its entry will be a JSON object and so will
-    no longer be trivially reversible to a valid FileField entry without a custom migration.
-
     :param ingress_to: A string defining the path within the bucket to which direct uploads
     will be ingressed, if temporary_ingress=True. These uploaded files will be moved to their
     ultimate path in the store on save of the model.
     :param accept_mimetype: A string passed to widgets, suitable for use in the `accept` attribute
     of an html filepicker. This will allow you to narrow down, eg to `image/*` or an even more
     specific mimetype. No validation is done at the field level that objects actually are of this
     type (because the python mimetypes module doesn't accept wildcard mimetypes and we don't want to
     go on a wild goose chase just for this small feature).
+
     :param get_destination_path: A callable to determine the destination path of the blob.
     The blob should already have been successfully uploaded to the temporary location
     in GCP prior to creation of this model instance. This function is then called in the
     pre_save stage of the new model instance, so it has access to all the model fields in
     order to construct the destination filename. Note this EXCLUDES the id, if the model has an
     autoincrementing ID field that gets created on save, because that can't be known prior to
     the save.
+
     :param max_size_bytes: The maximum size in bytes of files that can be uploaded.
 
+    :overwrite_mode: One of `OVERWRITE_MODES` determining the circumstances under which overwrite
+    is allowed. overwrite mode behaves as follows:
+    - never: Never allows overwrite
+    - update: Only when updating an object
+    - update-versioned: Only when updating an object and the bucket has object versioning
+    - add: Only when adding an object (we're not sure why you'd want this, here for completeness)
+    - add-versioned: Only when adding an object to a versioned bucket (again, for completeness)
+    - add-update: Always allow (ie when adding or updating an object)
+    - add-update-versioned: When adding or updating an object to a versioned bucket
     """
 
     description = _("A GCP Cloud Storage object")
     empty_values = [None, "", [], ()]
 
     def __init__(
         self,
@@ -166,17 +182,17 @@
 
         # An escape hatch allowing you to set the path directly. This is dangerous and should only be done
         # explicitly for the purpose of data migration and manipulation. You should never allow an untrusted
         # client to set paths directly, because knowing the path of a pre-existing object allows you to assume
         # access to it. Tip: You can use django's override_settings context manager to set this temporarily.
         if getattr(settings, "GCP_STORAGE_OVERRIDE_BLOBFIELD_VALUE", DEFAULT_OVERRIDE_BLOBFIELD_VALUE):
             logger.warning(
-                "Overriding %s value with path %s",
+                "Overriding %s value to %s",
                 self.__class__.__name__,
-                getattr(value, "path", None),
+                value,
             )
             new_value = value
         else:
             # There are six scenarios to deal with:
             adding_blank = add and value is None
             adding_valid = add and value is not None
             updating_valid_to_valid = not add and self._get_valid_to_valid(model_instance)
@@ -354,30 +370,21 @@
                     id="fields.E202",
                     hint="Remove the leading slash.",
                 )
             ]
         return []
 
     def _check_overwrite_mode(self):
-        allowable_modes = [
-            "never",
-            "update",
-            "update-versioned",
-            "add",
-            "add-versioned",
-            "add-update",
-            "add-update-versioned",
-        ]
-        if self.overwrite_mode not in allowable_modes:
+        if self.overwrite_mode not in OVERWRITE_MODES:
             return [
                 checks.Error(
                     "{self.__class__.__name__}'s 'overwrite_mode' is invalid",
                     obj=self,
                     id="fields.E202",
-                    hint=f"Try one of: {allowable_modes}",
+                    hint=f"Try one of: {OVERWRITE_MODES}",
                 )
             ]
         return []
 
     def _check_explicit(self):
         if self._primary_key_set_explicitly or self._choices_set_explicitly:
             return [
```

### Comparing `django_gcp-0.9.2/django_gcp/storage/forms.py` & `django_gcp-0.9.3/django_gcp/storage/forms.py`

 * *Files identical despite different names*

### Comparing `django_gcp-0.9.2/django_gcp/storage/gcloud.py` & `django_gcp-0.9.3/django_gcp/storage/gcloud.py`

 * *Files identical despite different names*

### Comparing `django_gcp-0.9.2/django_gcp/storage/operations.py` & `django_gcp-0.9.3/django_gcp/storage/operations.py`

 * *Files identical despite different names*

### Comparing `django_gcp-0.9.2/django_gcp/storage/settings.py` & `django_gcp-0.9.3/django_gcp/storage/settings.py`

 * *Files identical despite different names*

### Comparing `django_gcp-0.9.2/django_gcp/storage/utils.py` & `django_gcp-0.9.3/django_gcp/storage/utils.py`

 * *Files identical despite different names*

### Comparing `django_gcp-0.9.2/django_gcp/storage/widgets.py` & `django_gcp-0.9.3/django_gcp/storage/widgets.py`

 * *Files identical despite different names*

### Comparing `django_gcp-0.9.2/django_gcp/tasks/_patch_cloud_scheduler.py` & `django_gcp-0.9.3/django_gcp/tasks/_patch_cloud_scheduler.py`

 * *Files identical despite different names*

### Comparing `django_gcp-0.9.2/django_gcp/tasks/_patch_cloud_tasks.py` & `django_gcp-0.9.3/django_gcp/tasks/_patch_cloud_tasks.py`

 * *Files identical despite different names*

### Comparing `django_gcp-0.9.2/django_gcp/tasks/manager.py` & `django_gcp-0.9.3/django_gcp/tasks/manager.py`

 * *Files identical despite different names*

### Comparing `django_gcp-0.9.2/django_gcp/tasks/serializers.py` & `django_gcp-0.9.3/django_gcp/tasks/serializers.py`

 * *Files identical despite different names*

### Comparing `django_gcp-0.9.2/django_gcp/tasks/tasks.py` & `django_gcp-0.9.3/django_gcp/tasks/tasks.py`

 * *Files identical despite different names*

### Comparing `django_gcp-0.9.2/django_gcp/tasks/views.py` & `django_gcp-0.9.3/django_gcp/tasks/views.py`

 * *Files identical despite different names*

### Comparing `django_gcp-0.9.2/django_gcp/templates/django_gcp/cloud_object_widget.html` & `django_gcp-0.9.3/django_gcp/templates/django_gcp/cloud_object_widget.html`

 * *Files identical despite different names*

### Comparing `django_gcp-0.9.2/pyproject.toml` & `django_gcp-0.9.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-gcp"
-version = "0.9.2"
+version = "0.9.3"
 description = "Utilities to run Django on Google Cloud Platform"
 authors = ["Tom Clark"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
```

### Comparing `django_gcp-0.9.2/PKG-INFO` & `django_gcp-0.9.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-gcp
-Version: 0.9.2
+Version: 0.9.3
 Summary: Utilities to run Django on Google Cloud Platform
 Home-page: https://github.com/octue/django-gcp
 License: MIT
 Keywords: django,google,cloud,gcloud,gcp
 Author: Tom Clark
 Requires-Python: >=3.9,<3.11
 Classifier: Development Status :: 4 - Beta
```

