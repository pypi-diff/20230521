# Comparing `tmp/django_ses-3.4.1.tar.gz` & `tmp/django_ses-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_ses-3.4.1.tar", max compression
+gzip compressed data, was "django_ses-3.5.0.tar", max compression
```

## Comparing `django_ses-3.4.1.tar` & `django_ses-3.5.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0     1057 2023-04-25 21:41:20.616224 django_ses-3.4.1/LICENSE
--rw-r--r--   0        0        0    22619 2023-04-25 21:41:20.616224 django_ses-3.4.1/README.rst
--rw-r--r--   0        0        0    14037 2023-04-25 21:41:20.616224 django_ses-3.4.1/django_ses/__init__.py
--rw-r--r--   0        0        0      232 2023-04-25 21:41:20.616224 django_ses-3.4.1/django_ses/admin.py
--rw-r--r--   0        0        0      181 2023-04-25 21:41:20.616224 django_ses-3.4.1/django_ses/apps.py
--rw-r--r--   0        0        0       65 2023-04-25 21:41:20.616224 django_ses-3.4.1/django_ses/deprecation.py
--rw-r--r--   0        0        0        0 2023-04-25 21:41:20.616224 django_ses-3.4.1/django_ses/management/__init__.py
--rw-r--r--   0        0        0        0 2023-04-25 21:41:20.616224 django_ses-3.4.1/django_ses/management/commands/__init__.py
--rw-r--r--   0        0        0     2328 2023-04-25 21:41:20.616224 django_ses-3.4.1/django_ses/management/commands/get_ses_statistics.py
--rw-r--r--   0        0        0     2700 2023-04-25 21:41:20.616224 django_ses-3.4.1/django_ses/management/commands/ses_email_address.py
--rw-r--r--   0        0        0      897 2023-04-25 21:41:20.616224 django_ses-3.4.1/django_ses/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2023-04-25 21:41:20.616224 django_ses-3.4.1/django_ses/migrations/__init__.py
--rw-r--r--   0        0        0      455 2023-04-25 21:41:20.616224 django_ses-3.4.1/django_ses/models.py
--rw-r--r--   0        0        0     2677 2023-04-25 21:41:20.616224 django_ses-3.4.1/django_ses/settings.py
--rw-r--r--   0        0        0      290 2023-04-25 21:41:20.616224 django_ses-3.4.1/django_ses/signals.py
--rw-r--r--   0        0        0     4894 2023-04-25 21:41:20.616224 django_ses-3.4.1/django_ses/templates/django_ses/send_stats.html
--rw-r--r--   0        0        0      157 2023-04-25 21:41:20.616224 django_ses-3.4.1/django_ses/urls.py
--rw-r--r--   0        0        0     9218 2023-04-25 21:41:20.616224 django_ses-3.4.1/django_ses/utils.py
--rw-r--r--   0        0        0    20602 2023-04-25 21:41:20.616224 django_ses-3.4.1/django_ses/views.py
--rw-r--r--   0        0        0        0 2023-04-25 21:41:20.616224 django_ses-3.4.1/example/__init__.py
--rw-r--r--   0        0        0       90 2023-04-25 21:41:20.616224 django_ses-3.4.1/example/local_settings.template.py
--rw-r--r--   0        0        0      215 2023-04-25 21:41:20.616224 django_ses-3.4.1/example/middleware.py
--rw-r--r--   0        0        0     2173 2023-04-25 21:41:20.616224 django_ses-3.4.1/example/settings.py
--rw-r--r--   0        0        0      295 2023-04-25 21:41:20.616224 django_ses-3.4.1/example/templates/base.html
--rw-r--r--   0        0        0      220 2023-04-25 21:41:20.616224 django_ses-3.4.1/example/templates/index.html
--rw-r--r--   0        0        0      756 2023-04-25 21:41:20.616224 django_ses-3.4.1/example/templates/send-email.html
--rw-r--r--   0        0        0      818 2023-04-25 21:41:20.616224 django_ses-3.4.1/example/urls.py
--rw-r--r--   0        0        0      885 2023-04-25 21:41:20.616224 django_ses-3.4.1/example/views.py
--rw-r--r--   0        0        0     1560 2023-04-25 21:41:20.616224 django_ses-3.4.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-25 21:41:20.616224 django_ses-3.4.1/tests/__init__.py
--rw-r--r--   0        0        0    15650 2023-04-25 21:41:20.616224 django_ses-3.4.1/tests/test_backend.py
--rw-r--r--   0        0        0     2481 2023-04-25 21:41:20.616224 django_ses-3.4.1/tests/test_commands.py
--rw-r--r--   0        0        0     2609 2023-04-25 21:41:20.616224 django_ses-3.4.1/tests/test_settings.py
--rw-r--r--   0        0        0     5200 2023-04-25 21:41:20.616224 django_ses-3.4.1/tests/test_stats.py
--rw-r--r--   0        0        0      366 2023-04-25 21:41:20.616224 django_ses-3.4.1/tests/test_urls.py
--rw-r--r--   0        0        0    12140 2023-04-25 21:41:20.616224 django_ses-3.4.1/tests/test_verifier.py
--rw-r--r--   0        0        0    13333 2023-04-25 21:41:20.616224 django_ses-3.4.1/tests/test_views.py
--rw-r--r--   0        0        0      115 2023-04-25 21:41:20.616224 django_ses-3.4.1/tests/utils.py
--rw-r--r--   0        0        0    24336 1970-01-01 00:00:00.000000 django_ses-3.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1057 2023-05-21 15:47:53.955430 django_ses-3.5.0/LICENSE
+-rw-r--r--   0        0        0    22619 2023-05-21 15:47:53.955430 django_ses-3.5.0/README.rst
+-rw-r--r--   0        0        0    14037 2023-05-21 15:47:53.955430 django_ses-3.5.0/django_ses/__init__.py
+-rw-r--r--   0        0        0      232 2023-05-21 15:47:53.955430 django_ses-3.5.0/django_ses/admin.py
+-rw-r--r--   0        0        0      181 2023-05-21 15:47:53.955430 django_ses-3.5.0/django_ses/apps.py
+-rw-r--r--   0        0        0       65 2023-05-21 15:47:53.955430 django_ses-3.5.0/django_ses/deprecation.py
+-rw-r--r--   0        0        0        0 2023-05-21 15:47:53.955430 django_ses-3.5.0/django_ses/management/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-21 15:47:53.955430 django_ses-3.5.0/django_ses/management/commands/__init__.py
+-rw-r--r--   0        0        0     2328 2023-05-21 15:47:53.955430 django_ses-3.5.0/django_ses/management/commands/get_ses_statistics.py
+-rw-r--r--   0        0        0     2700 2023-05-21 15:47:53.955430 django_ses-3.5.0/django_ses/management/commands/ses_email_address.py
+-rw-r--r--   0        0        0      897 2023-05-21 15:47:53.955430 django_ses-3.5.0/django_ses/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2023-05-21 15:47:53.955430 django_ses-3.5.0/django_ses/migrations/__init__.py
+-rw-r--r--   0        0        0      455 2023-05-21 15:47:53.959430 django_ses-3.5.0/django_ses/models.py
+-rw-r--r--   0        0        0     2677 2023-05-21 15:47:53.959430 django_ses-3.5.0/django_ses/settings.py
+-rw-r--r--   0        0        0      290 2023-05-21 15:47:53.959430 django_ses-3.5.0/django_ses/signals.py
+-rw-r--r--   0        0        0     4894 2023-05-21 15:47:53.959430 django_ses-3.5.0/django_ses/templates/django_ses/send_stats.html
+-rw-r--r--   0        0        0      157 2023-05-21 15:47:53.959430 django_ses-3.5.0/django_ses/urls.py
+-rw-r--r--   0        0        0     9942 2023-05-21 15:47:53.959430 django_ses-3.5.0/django_ses/utils.py
+-rw-r--r--   0        0        0    20602 2023-05-21 15:47:53.959430 django_ses-3.5.0/django_ses/views.py
+-rw-r--r--   0        0        0        0 2023-05-21 15:47:53.959430 django_ses-3.5.0/example/__init__.py
+-rw-r--r--   0        0        0       90 2023-05-21 15:47:53.959430 django_ses-3.5.0/example/local_settings.template.py
+-rw-r--r--   0        0        0      215 2023-05-21 15:47:53.959430 django_ses-3.5.0/example/middleware.py
+-rw-r--r--   0        0        0     2173 2023-05-21 15:47:53.959430 django_ses-3.5.0/example/settings.py
+-rw-r--r--   0        0        0      295 2023-05-21 15:47:53.959430 django_ses-3.5.0/example/templates/base.html
+-rw-r--r--   0        0        0      220 2023-05-21 15:47:53.959430 django_ses-3.5.0/example/templates/index.html
+-rw-r--r--   0        0        0      756 2023-05-21 15:47:53.959430 django_ses-3.5.0/example/templates/send-email.html
+-rw-r--r--   0        0        0      818 2023-05-21 15:47:53.959430 django_ses-3.5.0/example/urls.py
+-rw-r--r--   0        0        0      885 2023-05-21 15:47:53.959430 django_ses-3.5.0/example/views.py
+-rw-r--r--   0        0        0     1560 2023-05-21 15:47:53.959430 django_ses-3.5.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-21 15:47:53.959430 django_ses-3.5.0/tests/__init__.py
+-rw-r--r--   0        0        0    15650 2023-05-21 15:47:53.959430 django_ses-3.5.0/tests/test_backend.py
+-rw-r--r--   0        0        0     2481 2023-05-21 15:47:53.959430 django_ses-3.5.0/tests/test_commands.py
+-rw-r--r--   0        0        0     2609 2023-05-21 15:47:53.959430 django_ses-3.5.0/tests/test_settings.py
+-rw-r--r--   0        0        0     5200 2023-05-21 15:47:53.959430 django_ses-3.5.0/tests/test_stats.py
+-rw-r--r--   0        0        0      366 2023-05-21 15:47:53.959430 django_ses-3.5.0/tests/test_urls.py
+-rw-r--r--   0        0        0    12227 2023-05-21 15:47:53.959430 django_ses-3.5.0/tests/test_verifier.py
+-rw-r--r--   0        0        0    13333 2023-05-21 15:47:53.959430 django_ses-3.5.0/tests/test_views.py
+-rw-r--r--   0        0        0      115 2023-05-21 15:47:53.959430 django_ses-3.5.0/tests/utils.py
+-rw-r--r--   0        0        0    24135 1970-01-01 00:00:00.000000 django_ses-3.5.0/PKG-INFO
```

### Comparing `django_ses-3.4.1/LICENSE` & `django_ses-3.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django_ses-3.4.1/README.rst` & `django_ses-3.5.0/README.rst`

 * *Files identical despite different names*

### Comparing `django_ses-3.4.1/django_ses/__init__.py` & `django_ses-3.5.0/django_ses/__init__.py`

 * *Files identical despite different names*

### Comparing `django_ses-3.4.1/django_ses/management/commands/get_ses_statistics.py` & `django_ses-3.5.0/django_ses/management/commands/get_ses_statistics.py`

 * *Files identical despite different names*

### Comparing `django_ses-3.4.1/django_ses/management/commands/ses_email_address.py` & `django_ses-3.5.0/django_ses/management/commands/ses_email_address.py`

 * *Files identical despite different names*

### Comparing `django_ses-3.4.1/django_ses/migrations/0001_initial.py` & `django_ses-3.5.0/django_ses/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django_ses-3.4.1/django_ses/settings.py` & `django_ses-3.5.0/django_ses/settings.py`

 * *Files identical despite different names*

### Comparing `django_ses-3.4.1/django_ses/templates/django_ses/send_stats.html` & `django_ses-3.5.0/django_ses/templates/django_ses/send_stats.html`

 * *Files identical despite different names*

### Comparing `django_ses-3.4.1/django_ses/utils.py` & `django_ses-3.5.0/django_ses/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 import base64
 import logging
+import re
 import warnings
 from builtins import bytes
-
-from django_ses.deprecation import RemovedInDjangoSES20Warning
-
+from urllib.error import URLError
 from urllib.parse import urlparse
 from urllib.request import urlopen
-from urllib.error import URLError
 
 from django.core.exceptions import ImproperlyConfigured
+
 from django_ses import settings
+from django_ses.deprecation import RemovedInDjangoSES20Warning
 
 logger = logging.getLogger(__name__)
 
 _CERT_CACHE = {}
 
+SES_REGEX_CERT_URL = re.compile(
+    "(?i)^https://sns\.[a-z0-9\-]+\.amazonaws\.com(\.cn)?/SimpleNotificationService\-[a-z0-9]+\.pem$"
+)
+
 
 def clear_cert_cache():
     """Clear the certificate cache.
 
     This one-liner exists to discourage imports and direct usage of
     _CERT_CACHE.
 
@@ -179,47 +183,60 @@
         if not cert_url.startswith("https://"):
             logger.warning('Untrusted certificate URL: "%s"', cert_url)
             return None
 
         url_obj = urlparse(cert_url)
         for trusted_domain in settings.EVENT_CERT_DOMAINS:
             parts = trusted_domain.split(".")
+            if "amazonaws.com" in trusted_domain:
+                if not SES_REGEX_CERT_URL.match(cert_url):
+                    if len(parts) < 4:
+                        return None
+                    else:
+                        logger.warning('Possible security risk for: "%s"', cert_url)
+                        logger.warning(
+                            "It is strongly recommended to configure the full domain in EVENT_CERT_DOMAINS. "
+                            "See v3.5.0 release notes for more details."
+                        )
+
             if url_obj.netloc.split(".")[-len(parts) :] == parts:
                 return cert_url
 
         return None
 
     def _get_bytes_to_sign(self):
         """
         Creates the message used for signing SNS notifications.
         This is used to verify the bounce message when it is received.
         """
 
         # Depending on the message type the fields to add to the message
         # differ so we handle that here.
-        msg_type = self._data.get('Type')
-        if msg_type == 'Notification':
+        msg_type = self._data.get("Type")
+        if msg_type == "Notification":
             fields_to_sign = [
-                'Message',
-                'MessageId',
-                'Subject',
-                'Timestamp',
-                'TopicArn',
-                'Type',
+                "Message",
+                "MessageId",
+                "Subject",
+                "Timestamp",
+                "TopicArn",
+                "Type",
             ]
-        elif (msg_type == 'SubscriptionConfirmation' or
-              msg_type == 'UnsubscribeConfirmation'):
+        elif (
+            msg_type == "SubscriptionConfirmation"
+            or msg_type == "UnsubscribeConfirmation"
+        ):
             fields_to_sign = [
-                'Message',
-                'MessageId',
-                'SubscribeURL',
-                'Timestamp',
-                'Token',
-                'TopicArn',
-                'Type',
+                "Message",
+                "MessageId",
+                "SubscribeURL",
+                "Timestamp",
+                "Token",
+                "TopicArn",
+                "Type",
             ]
         else:
             # Unrecognized type
             logger.warning('Unrecognized SNS message Type: "%s"', msg_type)
             return None
 
         bytes_to_sign = []
@@ -233,22 +250,22 @@
             bytes_to_sign.append(f"{field}\n{field_value}\n")
 
         return "".join(bytes_to_sign).encode()
 
 
 def BounceMessageVerifier(*args, **kwargs):
     warnings.warn(
-        'utils.BounceMessageVerifier is deprecated. It is renamed to EventMessageVerifier.',
+        "utils.BounceMessageVerifier is deprecated. It is renamed to EventMessageVerifier.",
         RemovedInDjangoSES20Warning,
     )
 
     # parameter name is renamed from bounce_dict to notification.
-    if 'bounce_dict' in kwargs:
-        kwargs['notification'] = kwargs['bounce_dict']
-        del kwargs['bounce_dict']
+    if "bounce_dict" in kwargs:
+        kwargs["notification"] = kwargs["bounce_dict"]
+        del kwargs["bounce_dict"]
 
     return EventMessageVerifier(*args, **kwargs)
 
 
 def verify_event_message(notification):
     """
     Verify an SES/SNS event notification message.
@@ -258,35 +275,36 @@
 
 
 def verify_bounce_message(msg):
     """
     Verify an SES/SNS bounce(event) notification message.
     """
     warnings.warn(
-        'utils.verify_bounce_message is deprecated. It is renamed to verify_event_message.',
+        "utils.verify_bounce_message is deprecated. It is renamed to verify_event_message.",
         RemovedInDjangoSES20Warning,
     )
     return verify_event_message(msg)
 
 
 def confirm_sns_subscription(notification):
     logger.info(
-        'Received subscription confirmation: TopicArn: %s',
-        notification.get('TopicArn'),
+        "Received subscription confirmation: TopicArn: %s",
+        notification.get("TopicArn"),
         extra={
-            'notification': notification,
+            "notification": notification,
         },
     )
 
     # Get the subscribe url and hit the url to confirm the subscription.
-    subscribe_url = notification.get('SubscribeURL')
+    subscribe_url = notification.get("SubscribeURL")
     try:
         urlopen(subscribe_url).read()
     except URLError as e:
         # Some kind of error occurred when confirming the request.
         logger.error(
-            'Could not confirm subscription: "%s"', e,
+            'Could not confirm subscription: "%s"',
+            e,
             extra={
-                'notification': notification,
+                "notification": notification,
             },
             exc_info=True,
         )
```

### Comparing `django_ses-3.4.1/django_ses/views.py` & `django_ses-3.5.0/django_ses/views.py`

 * *Files identical despite different names*

### Comparing `django_ses-3.4.1/example/settings.py` & `django_ses-3.5.0/example/settings.py`

 * *Files identical despite different names*

### Comparing `django_ses-3.4.1/example/templates/send-email.html` & `django_ses-3.5.0/example/templates/send-email.html`

 * *Files identical despite different names*

### Comparing `django_ses-3.4.1/example/urls.py` & `django_ses-3.5.0/example/urls.py`

 * *Files identical despite different names*

### Comparing `django_ses-3.4.1/example/views.py` & `django_ses-3.5.0/example/views.py`

 * *Files identical despite different names*

### Comparing `django_ses-3.4.1/pyproject.toml` & `django_ses-3.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-ses"
-version = "3.4.1"
+version = "3.5.0"
 description = "A Django email backend for Amazon's Simple Email Service"
 authors = [
     "Harry Marr <harry@hmarr.com>",
     "Wes Winham <winhamwr@gmail.com>",
     "Ross Lawley <ross.lawley@gmail.com>",
     "Paul Craciunoiu <paul@craciunoiu.net>",
 ]
```

### Comparing `django_ses-3.4.1/tests/test_backend.py` & `django_ses-3.5.0/tests/test_backend.py`

 * *Files identical despite different names*

### Comparing `django_ses-3.4.1/tests/test_commands.py` & `django_ses-3.5.0/tests/test_commands.py`

 * *Files identical despite different names*

### Comparing `django_ses-3.4.1/tests/test_settings.py` & `django_ses-3.5.0/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `django_ses-3.4.1/tests/test_stats.py` & `django_ses-3.5.0/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `django_ses-3.4.1/tests/test_verifier.py` & `django_ses-3.5.0/tests/test_verifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -122,20 +122,23 @@
             verifier.certificate
             request_get.assert_called_once()
 
     def test_get_cert_url(self):
         """
         Test url trust verification
         """
+        cert_url = (
+            "https://sns.test-example.amazonaws.com/SimpleNotificationService-abcd.pem"
+        )
         verifier = BounceMessageVerifier(
             {
-                "SigningCertURL": "https://amazonaws.com/",
+                "SigningCertURL": cert_url,
             }
         )
-        self.assertEqual(verifier._get_cert_url(), "https://amazonaws.com/")
+        self.assertEqual(verifier._get_cert_url(), cert_url)
 
     def test_http_cert_url(self):
         """
         Test url trust verification. Non-https urls should be rejected.
         """
         verifier = BounceMessageVerifier(
             {
```

### Comparing `django_ses-3.4.1/tests/test_views.py` & `django_ses-3.5.0/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `django_ses-3.4.1/PKG-INFO` & `django_ses-3.5.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-ses
-Version: 3.4.1
+Version: 3.5.0
 Summary: A Django email backend for Amazon's Simple Email Service
 Home-page: https://github.com/django-ses/django-ses
 License: MIT
 Author: Harry Marr
 Author-email: harry@hmarr.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
@@ -19,18 +19,14 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: bounce
 Provides-Extra: events
 Requires-Dist: boto3 (>=1.0.0)
 Requires-Dist: cryptography (>=36.0.2) ; extra == "bounce" or extra == "events"
 Requires-Dist: django (>=2.2)
 Requires-Dist: importlib-metadata (>=1) ; python_version < "3.8"
```

