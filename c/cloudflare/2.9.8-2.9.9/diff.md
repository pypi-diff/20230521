# Comparing `tmp/cloudflare-2.9.8.tar.gz` & `tmp/cloudflare-2.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudflare-2.9.8.tar", last modified: Thu Mar 31 04:00:14 2022, max compression
+gzip compressed data, was "cloudflare-2.9.9.tar", last modified: Sat Apr  2 04:27:37 2022, max compression
```

## Comparing `cloudflare-2.9.8.tar` & `cloudflare-2.9.9.tar`

### file list

```diff
@@ -1,60 +1,60 @@
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-03-31 04:00:14.833720 cloudflare-2.9.8/
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-03-31 04:00:14.820458 cloudflare-2.9.8/CloudFlare/
--rw-r--r--   0 martin     (501) staff       (20)      149 2022-03-31 03:59:09.000000 cloudflare-2.9.8/CloudFlare/__init__.py
--rw-r--r--   0 martin     (501) staff       (20)     2665 2022-03-01 00:39:24.000000 cloudflare-2.9.8/CloudFlare/api_decode_from_web.py
--rw-r--r--   0 martin     (501) staff       (20)     1773 2020-02-06 02:13:26.000000 cloudflare-2.9.8/CloudFlare/api_extras.py
--rw-r--r--   0 martin     (501) staff       (20)    27357 2022-03-30 23:17:18.000000 cloudflare-2.9.8/CloudFlare/api_v4.py
--rw-r--r--   0 martin     (501) staff       (20)    45375 2022-03-31 00:04:28.000000 cloudflare-2.9.8/CloudFlare/cloudflare.py
--rw-r--r--   0 martin     (501) staff       (20)     2055 2020-01-16 20:01:18.000000 cloudflare-2.9.8/CloudFlare/exceptions.py
--rw-r--r--   0 martin     (501) staff       (20)     1374 2020-01-19 00:13:37.000000 cloudflare-2.9.8/CloudFlare/logging_helper.py
--rw-r--r--   0 martin     (501) staff       (20)     2546 2020-06-24 00:38:21.000000 cloudflare-2.9.8/CloudFlare/network.py
--rw-r--r--   0 martin     (501) staff       (20)     3975 2022-03-30 23:00:48.000000 cloudflare-2.9.8/CloudFlare/read_configs.py
--rw-r--r--   0 martin     (501) staff       (20)     2169 2020-07-22 00:18:18.000000 cloudflare-2.9.8/CloudFlare/utils.py
--rw-r--r--   0 martin     (501) staff       (20)     1094 2019-11-20 18:33:03.000000 cloudflare-2.9.8/LICENSE
--rw-r--r--   0 martin     (501) staff       (20)       83 2019-11-20 18:33:03.000000 cloudflare-2.9.8/MANIFEST.in
--rw-r--r--   0 martin     (501) staff       (20)    52745 2022-03-31 04:00:14.834569 cloudflare-2.9.8/PKG-INFO
--rw-r--r--   0 martin     (501) staff       (20)    42259 2022-03-30 23:02:47.000000 cloudflare-2.9.8/README.rst
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-03-31 04:00:14.821828 cloudflare-2.9.8/cli4/
--rw-r--r--   0 martin     (501) staff       (20)        0 2019-11-20 18:33:03.000000 cloudflare-2.9.8/cli4/__init__.py
--rwxr-xr-x   0 martin     (501) staff       (20)      302 2020-01-15 21:29:49.000000 cloudflare-2.9.8/cli4/__main__.py
--rw-r--r--   0 martin     (501) staff       (20)     3816 2022-03-30 20:48:59.000000 cloudflare-2.9.8/cli4/cli4.1
--rw-r--r--   0 martin     (501) staff       (20)    18829 2022-02-17 17:33:19.000000 cloudflare-2.9.8/cli4/cli4.py
--rw-r--r--   0 martin     (501) staff       (20)     5567 2020-06-23 01:22:51.000000 cloudflare-2.9.8/cli4/converters.py
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-03-31 04:00:14.823922 cloudflare-2.9.8/cloudflare.egg-info/
--rw-r--r--   0 martin     (501) staff       (20)    52745 2022-03-31 04:00:14.000000 cloudflare-2.9.8/cloudflare.egg-info/PKG-INFO
--rw-r--r--   0 martin     (501) staff       (20)     1521 2022-03-31 04:00:14.000000 cloudflare-2.9.8/cloudflare.egg-info/SOURCES.txt
--rw-r--r--   0 martin     (501) staff       (20)        1 2022-03-31 04:00:14.000000 cloudflare-2.9.8/cloudflare.egg-info/dependency_links.txt
--rw-r--r--   0 martin     (501) staff       (20)       45 2022-03-31 04:00:14.000000 cloudflare-2.9.8/cloudflare.egg-info/entry_points.txt
--rw-r--r--   0 martin     (501) staff       (20)       41 2022-03-31 04:00:14.000000 cloudflare-2.9.8/cloudflare.egg-info/requires.txt
--rw-r--r--   0 martin     (501) staff       (20)       25 2022-03-31 04:00:14.000000 cloudflare-2.9.8/cloudflare.egg-info/top_level.txt
-drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-03-31 04:00:14.833393 cloudflare-2.9.8/examples/
--rw-r--r--   0 martin     (501) staff       (20)        0 2019-11-20 18:33:03.000000 cloudflare-2.9.8/examples/__init__.py
--rwxr-xr-x   0 martin     (501) staff       (20)     2783 2021-07-21 10:22:01.000000 cloudflare-2.9.8/examples/example_account_rules_lists_items.py
--rwxr-xr-x   0 martin     (501) staff       (20)     1989 2020-06-22 19:30:28.000000 cloudflare-2.9.8/examples/example_always_use_https.py
--rwxr-xr-x   0 martin     (501) staff       (20)     1876 2020-06-22 19:30:32.000000 cloudflare-2.9.8/examples/example_are_zones_ipv6.py
--rwxr-xr-x   0 martin     (501) staff       (20)      558 2020-06-22 19:30:35.000000 cloudflare-2.9.8/examples/example_are_zones_ipv6_simple.py
--rwxr-xr-x   0 martin     (501) staff       (20)     2673 2020-06-22 19:32:47.000000 cloudflare-2.9.8/examples/example_certificates.py
--rwxr-xr-x   0 martin     (501) staff       (20)     3935 2020-06-22 19:30:46.000000 cloudflare-2.9.8/examples/example_create_zone_and_populate.py
--rwxr-xr-x   0 martin     (501) staff       (20)     2280 2020-06-23 01:43:49.000000 cloudflare-2.9.8/examples/example_custom_hostnames.py
--rwxr-xr-x   0 martin     (501) staff       (20)     2034 2020-06-22 19:33:41.000000 cloudflare-2.9.8/examples/example_delete_zone_entry.py
--rwxr-xr-x   0 martin     (501) staff       (20)     1366 2020-06-22 19:30:58.000000 cloudflare-2.9.8/examples/example_dns_export.py
--rwxr-xr-x   0 martin     (501) staff       (20)     1476 2021-07-21 10:53:55.000000 cloudflare-2.9.8/examples/example_dns_import.py
--rwxr-xr-x   0 martin     (501) staff       (20)     1459 2020-06-22 19:31:06.000000 cloudflare-2.9.8/examples/example_dnssec_settings.py
--rwxr-xr-x   0 martin     (501) staff       (20)     2328 2020-07-15 01:45:23.000000 cloudflare-2.9.8/examples/example_graphql.py
--rwxr-xr-x   0 martin     (501) staff       (20)      981 2020-07-15 01:43:04.000000 cloudflare-2.9.8/examples/example_graphql.sh
--rwxr-xr-x   0 martin     (501) staff       (20)      763 2020-06-22 19:30:09.000000 cloudflare-2.9.8/examples/example_ips.py
--rwxr-xr-x   0 martin     (501) staff       (20)      454 2020-06-22 19:31:11.000000 cloudflare-2.9.8/examples/example_list_api_from_web.py
--rwxr-xr-x   0 martin     (501) staff       (20)     2187 2022-03-30 20:17:02.000000 cloudflare-2.9.8/examples/example_page_rules.py
--rwxr-xr-x   0 martin     (501) staff       (20)      440 2019-11-20 18:33:03.000000 cloudflare-2.9.8/examples/example_page_rules.sh
--rwxr-xr-x   0 martin     (501) staff       (20)     1204 2020-06-22 19:31:15.000000 cloudflare-2.9.8/examples/example_paging_thru_zones.py
--rwxr-xr-x   0 martin     (501) staff       (20)      780 2019-11-20 18:33:03.000000 cloudflare-2.9.8/examples/example_paging_thru_zones.sh
--rwxr-xr-x   0 martin     (501) staff       (20)     3388 2020-06-22 19:31:19.000000 cloudflare-2.9.8/examples/example_proxied.py
--rwxr-xr-x   0 martin     (501) staff       (20)     1827 2020-06-22 19:31:25.000000 cloudflare-2.9.8/examples/example_settings.py
--rw-r--r--   0 martin     (501) staff       (20)     1104 2022-03-30 20:34:37.000000 cloudflare-2.9.8/examples/example_show_account_email.py
--rwxr-xr-x   0 martin     (501) staff       (20)     4273 2020-06-22 19:36:58.000000 cloudflare-2.9.8/examples/example_update_dynamic_dns.py
--rwxr-xr-x   0 martin     (501) staff       (20)     5512 2020-06-22 19:37:32.000000 cloudflare-2.9.8/examples/example_user.py
--rwxr-xr-x   0 martin     (501) staff       (20)      677 2020-06-22 19:31:40.000000 cloudflare-2.9.8/examples/example_with_usage.py
--rwxr-xr-x   0 martin     (501) staff       (20)      420 2020-04-09 00:38:19.000000 cloudflare-2.9.8/examples/example_zone_search.sh
--rwxr-xr-x   0 martin     (501) staff       (20)     2436 2020-06-22 21:24:44.000000 cloudflare-2.9.8/examples/example_zones.py
--rw-r--r--   0 martin     (501) staff       (20)       38 2022-03-31 04:00:14.835159 cloudflare-2.9.8/setup.cfg
--rwxr-xr-x   0 martin     (501) staff       (20)     2186 2022-03-30 20:48:59.000000 cloudflare-2.9.8/setup.py
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-04-02 04:27:37.506605 cloudflare-2.9.9/
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-04-02 04:27:37.494604 cloudflare-2.9.9/CloudFlare/
+-rw-r--r--   0 martin     (501) staff       (20)      149 2022-04-02 04:26:32.000000 cloudflare-2.9.9/CloudFlare/__init__.py
+-rw-r--r--   0 martin     (501) staff       (20)     2665 2022-03-01 00:39:24.000000 cloudflare-2.9.9/CloudFlare/api_decode_from_web.py
+-rw-r--r--   0 martin     (501) staff       (20)     1773 2020-02-06 02:13:26.000000 cloudflare-2.9.9/CloudFlare/api_extras.py
+-rw-r--r--   0 martin     (501) staff       (20)    27357 2022-03-30 23:17:18.000000 cloudflare-2.9.9/CloudFlare/api_v4.py
+-rw-r--r--   0 martin     (501) staff       (20)    45375 2022-03-31 00:04:28.000000 cloudflare-2.9.9/CloudFlare/cloudflare.py
+-rw-r--r--   0 martin     (501) staff       (20)     2055 2020-01-16 20:01:18.000000 cloudflare-2.9.9/CloudFlare/exceptions.py
+-rw-r--r--   0 martin     (501) staff       (20)     1374 2020-01-19 00:13:37.000000 cloudflare-2.9.9/CloudFlare/logging_helper.py
+-rw-r--r--   0 martin     (501) staff       (20)     2546 2020-06-24 00:38:21.000000 cloudflare-2.9.9/CloudFlare/network.py
+-rw-r--r--   0 martin     (501) staff       (20)     4108 2022-04-02 04:26:17.000000 cloudflare-2.9.9/CloudFlare/read_configs.py
+-rw-r--r--   0 martin     (501) staff       (20)     2169 2020-07-22 00:18:18.000000 cloudflare-2.9.9/CloudFlare/utils.py
+-rw-r--r--   0 martin     (501) staff       (20)     1094 2019-11-20 18:33:03.000000 cloudflare-2.9.9/LICENSE
+-rw-r--r--   0 martin     (501) staff       (20)       83 2019-11-20 18:33:03.000000 cloudflare-2.9.9/MANIFEST.in
+-rw-r--r--   0 martin     (501) staff       (20)    53623 2022-04-02 04:27:37.507452 cloudflare-2.9.9/PKG-INFO
+-rw-r--r--   0 martin     (501) staff       (20)    42993 2022-04-01 17:33:58.000000 cloudflare-2.9.9/README.rst
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-04-02 04:27:37.495845 cloudflare-2.9.9/cli4/
+-rw-r--r--   0 martin     (501) staff       (20)        0 2019-11-20 18:33:03.000000 cloudflare-2.9.9/cli4/__init__.py
+-rwxr-xr-x   0 martin     (501) staff       (20)      302 2020-01-15 21:29:49.000000 cloudflare-2.9.9/cli4/__main__.py
+-rw-r--r--   0 martin     (501) staff       (20)     3816 2022-03-30 20:48:59.000000 cloudflare-2.9.9/cli4/cli4.1
+-rw-r--r--   0 martin     (501) staff       (20)    18829 2022-02-17 17:33:19.000000 cloudflare-2.9.9/cli4/cli4.py
+-rw-r--r--   0 martin     (501) staff       (20)     5567 2020-06-23 01:22:51.000000 cloudflare-2.9.9/cli4/converters.py
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-04-02 04:27:37.497377 cloudflare-2.9.9/cloudflare.egg-info/
+-rw-r--r--   0 martin     (501) staff       (20)    53623 2022-04-02 04:27:37.000000 cloudflare-2.9.9/cloudflare.egg-info/PKG-INFO
+-rw-r--r--   0 martin     (501) staff       (20)     1521 2022-04-02 04:27:37.000000 cloudflare-2.9.9/cloudflare.egg-info/SOURCES.txt
+-rw-r--r--   0 martin     (501) staff       (20)        1 2022-04-02 04:27:37.000000 cloudflare-2.9.9/cloudflare.egg-info/dependency_links.txt
+-rw-r--r--   0 martin     (501) staff       (20)       45 2022-04-02 04:27:37.000000 cloudflare-2.9.9/cloudflare.egg-info/entry_points.txt
+-rw-r--r--   0 martin     (501) staff       (20)       41 2022-04-02 04:27:37.000000 cloudflare-2.9.9/cloudflare.egg-info/requires.txt
+-rw-r--r--   0 martin     (501) staff       (20)       25 2022-04-02 04:27:37.000000 cloudflare-2.9.9/cloudflare.egg-info/top_level.txt
+drwxr-xr-x   0 martin     (501) staff       (20)        0 2022-04-02 04:27:37.506298 cloudflare-2.9.9/examples/
+-rw-r--r--   0 martin     (501) staff       (20)        0 2019-11-20 18:33:03.000000 cloudflare-2.9.9/examples/__init__.py
+-rwxr-xr-x   0 martin     (501) staff       (20)     2783 2021-07-21 10:22:01.000000 cloudflare-2.9.9/examples/example_account_rules_lists_items.py
+-rwxr-xr-x   0 martin     (501) staff       (20)     1989 2020-06-22 19:30:28.000000 cloudflare-2.9.9/examples/example_always_use_https.py
+-rwxr-xr-x   0 martin     (501) staff       (20)     1876 2020-06-22 19:30:32.000000 cloudflare-2.9.9/examples/example_are_zones_ipv6.py
+-rwxr-xr-x   0 martin     (501) staff       (20)      558 2020-06-22 19:30:35.000000 cloudflare-2.9.9/examples/example_are_zones_ipv6_simple.py
+-rwxr-xr-x   0 martin     (501) staff       (20)     2673 2020-06-22 19:32:47.000000 cloudflare-2.9.9/examples/example_certificates.py
+-rwxr-xr-x   0 martin     (501) staff       (20)     3935 2020-06-22 19:30:46.000000 cloudflare-2.9.9/examples/example_create_zone_and_populate.py
+-rwxr-xr-x   0 martin     (501) staff       (20)     2280 2020-06-23 01:43:49.000000 cloudflare-2.9.9/examples/example_custom_hostnames.py
+-rwxr-xr-x   0 martin     (501) staff       (20)     2034 2020-06-22 19:33:41.000000 cloudflare-2.9.9/examples/example_delete_zone_entry.py
+-rwxr-xr-x   0 martin     (501) staff       (20)     1366 2020-06-22 19:30:58.000000 cloudflare-2.9.9/examples/example_dns_export.py
+-rwxr-xr-x   0 martin     (501) staff       (20)     1476 2021-07-21 10:53:55.000000 cloudflare-2.9.9/examples/example_dns_import.py
+-rwxr-xr-x   0 martin     (501) staff       (20)     1459 2020-06-22 19:31:06.000000 cloudflare-2.9.9/examples/example_dnssec_settings.py
+-rwxr-xr-x   0 martin     (501) staff       (20)     2328 2020-07-15 01:45:23.000000 cloudflare-2.9.9/examples/example_graphql.py
+-rwxr-xr-x   0 martin     (501) staff       (20)      981 2020-07-15 01:43:04.000000 cloudflare-2.9.9/examples/example_graphql.sh
+-rwxr-xr-x   0 martin     (501) staff       (20)      763 2020-06-22 19:30:09.000000 cloudflare-2.9.9/examples/example_ips.py
+-rwxr-xr-x   0 martin     (501) staff       (20)      454 2020-06-22 19:31:11.000000 cloudflare-2.9.9/examples/example_list_api_from_web.py
+-rwxr-xr-x   0 martin     (501) staff       (20)     2187 2022-03-30 20:17:02.000000 cloudflare-2.9.9/examples/example_page_rules.py
+-rwxr-xr-x   0 martin     (501) staff       (20)      440 2019-11-20 18:33:03.000000 cloudflare-2.9.9/examples/example_page_rules.sh
+-rwxr-xr-x   0 martin     (501) staff       (20)     1204 2020-06-22 19:31:15.000000 cloudflare-2.9.9/examples/example_paging_thru_zones.py
+-rwxr-xr-x   0 martin     (501) staff       (20)      780 2019-11-20 18:33:03.000000 cloudflare-2.9.9/examples/example_paging_thru_zones.sh
+-rwxr-xr-x   0 martin     (501) staff       (20)     3388 2020-06-22 19:31:19.000000 cloudflare-2.9.9/examples/example_proxied.py
+-rwxr-xr-x   0 martin     (501) staff       (20)     1827 2020-06-22 19:31:25.000000 cloudflare-2.9.9/examples/example_settings.py
+-rw-r--r--   0 martin     (501) staff       (20)     1104 2022-03-30 20:34:37.000000 cloudflare-2.9.9/examples/example_show_account_email.py
+-rwxr-xr-x   0 martin     (501) staff       (20)     4273 2020-06-22 19:36:58.000000 cloudflare-2.9.9/examples/example_update_dynamic_dns.py
+-rwxr-xr-x   0 martin     (501) staff       (20)     5512 2020-06-22 19:37:32.000000 cloudflare-2.9.9/examples/example_user.py
+-rwxr-xr-x   0 martin     (501) staff       (20)      677 2020-06-22 19:31:40.000000 cloudflare-2.9.9/examples/example_with_usage.py
+-rwxr-xr-x   0 martin     (501) staff       (20)      420 2020-04-09 00:38:19.000000 cloudflare-2.9.9/examples/example_zone_search.sh
+-rwxr-xr-x   0 martin     (501) staff       (20)     2436 2020-06-22 21:24:44.000000 cloudflare-2.9.9/examples/example_zones.py
+-rw-r--r--   0 martin     (501) staff       (20)       38 2022-04-02 04:27:37.508126 cloudflare-2.9.9/setup.cfg
+-rwxr-xr-x   0 martin     (501) staff       (20)     2186 2022-03-30 20:48:59.000000 cloudflare-2.9.9/setup.py
```

### Comparing `cloudflare-2.9.8/CloudFlare/api_decode_from_web.py` & `cloudflare-2.9.9/CloudFlare/api_decode_from_web.py`

 * *Files identical despite different names*

### Comparing `cloudflare-2.9.8/CloudFlare/api_extras.py` & `cloudflare-2.9.9/CloudFlare/api_extras.py`

 * *Files identical despite different names*

### Comparing `cloudflare-2.9.8/CloudFlare/api_v4.py` & `cloudflare-2.9.9/CloudFlare/api_v4.py`

 * *Files identical despite different names*

### Comparing `cloudflare-2.9.8/CloudFlare/cloudflare.py` & `cloudflare-2.9.9/CloudFlare/cloudflare.py`

 * *Files identical despite different names*

### Comparing `cloudflare-2.9.8/CloudFlare/exceptions.py` & `cloudflare-2.9.9/CloudFlare/exceptions.py`

 * *Files identical despite different names*

### Comparing `cloudflare-2.9.8/CloudFlare/logging_helper.py` & `cloudflare-2.9.9/CloudFlare/logging_helper.py`

 * *Files identical despite different names*

### Comparing `cloudflare-2.9.8/CloudFlare/network.py` & `cloudflare-2.9.9/CloudFlare/network.py`

 * *Files identical despite different names*

### Comparing `cloudflare-2.9.8/CloudFlare/read_configs.py` & `cloudflare-2.9.9/CloudFlare/read_configs.py`

 * *Files 11% similar despite different names*

```diff
@@ -27,55 +27,58 @@
             '.cloudflare.cfg',
             os.path.expanduser('~/.cloudflare.cfg'),
             os.path.expanduser('~/.cloudflare/cloudflare.cfg')
         ])
     except Exception as e:
         raise Exception("%s: configuration file error" % (profile))
 
+    if len(cp.sections()) == 0 and profile != None:
+        # no config file and yet a config name provided - not acceptable!
+        raise Exception("%s: configuration section provided however config file missing" % (profile))
+
     # Is it CloudFlare or Cloudflare? (A legacy issue)
     if profile is None:
-        if len(cp.sections()) > 0:
-            if 'CloudFlare' in cp:
-                profile = 'CloudFlare'
-            if 'Cloudflare' in cp:
-                profile = 'Cloudflare'
+        if cp.has_section('CloudFlare'):
+            profile = 'CloudFlare'
+        if cp.has_section('Cloudflare'):
+            profile = 'Cloudflare'
 
     ## still not found - then set to to CloudFlare for legacy reasons
     if profile == None:
         profile = "CloudFlare"
+
     config['profile'] = profile
 
     if len(cp.sections()) > 0:
         # we have a configuration file - lets use it
-        try:
-            # grab the section - as we will use it for all values
-            section = cp[profile]
-        except Exception as e:
-            # however section name is missing - this is an error
-            raise Exception("%s: configuration section missing" % (profile))
+
+        if not cp.has_section(profile):
+            raise Exception("%s: configuration section missing - configuration file only has these sections: %s" % (profile, ','.join(cp.sections())))
 
         for option in ['email', 'token', 'certtoken', 'extras', 'base_url']:
-            if option not in config or config[option] is None:
-                try:
-                    if option == 'extras':
-                        config[option] = re.sub(r"\s+", ' ', section.get(option))
-                    else:
-                        config[option] = re.sub(r"\s+", '', section.get(option))
-                    if config[option] == '':
-                        config.pop(option)
-                except (configparser.NoOptionError, configparser.NoSectionError):
-                    pass
-                except Exception as e:
-                    pass
+            try:
+                config_value = cp.get(profile, option)
+                if option == 'extras':
+                    config[option] = re.sub(r"\s+", ' ', config_value)
+                else:
+                    config[option] = re.sub(r"\s+", '', config_value)
+                if config[option] == None or config[option] == '':
+                    config.pop(option)
+            except (configparser.NoOptionError, configparser.NoSectionError):
+                pass
+            except Exception as e:
+                pass
+
             # do we have an override for specific calls? (i.e. token.post or email.get etc)
             for method in ['get', 'patch', 'post', 'put', 'delete']:
                 option_for_method = option + '.' + method
                 try:
-                    config[option_for_method] = re.sub(r"\s+", '', section.get(option_for_method))
-                    if config[option_for_method] == '':
+                    config_value = cp.get(profile, option_for_method)
+                    config[option_for_method] = re.sub(r"\s+", '', config_value)
+                    if config[option] == None or config[option] == '':
                         config.pop(option_for_method)
                 except (configparser.NoOptionError, configparser.NoSectionError) as e:
                     pass
                 except Exception as e:
                     pass
 
     # do any final cleanup - only needed for extras (which are multiline)
```

### Comparing `cloudflare-2.9.8/CloudFlare/utils.py` & `cloudflare-2.9.9/CloudFlare/utils.py`

 * *Files identical despite different names*

### Comparing `cloudflare-2.9.8/LICENSE` & `cloudflare-2.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudflare-2.9.8/PKG-INFO` & `cloudflare-2.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: cloudflare
-Version: 2.9.8
+Version: 2.9.9
 Summary: Python wrapper for the Cloudflare v4 API
 Home-page: https://github.com/cloudflare/python-cloudflare
 Author: Martin J. Levy
 Author-email: martin@cloudflare.com
 License: MIT
 Description: cloudflare-python
         =================
@@ -874,16 +874,16 @@
                "key_type": "ECDSAP256SHA256",
                "modified_on": "2016-05-01T22:42:15.591158Z",
                "public_key": "mdsswUyr3DPW132mOi8V9xESWE8jTo0dxCjjnopKl+GqJxpVXckHAeF+KkxLbxILfDLUT0rAK9iUzy1L53eKGQ==",
                "status": "pending"
            }
            $
         
-        Zone file upload and download CLI examples (uses BIND format files)
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+        Zone file upload (i.e. import) CLI examples (uses BIND format files)
+        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
         
         Refer to `Import DNS records <https://api.cloudflare.com/#dns-records-for-a-zone-import-dns-records>`__ on API documentation for this feature.
         
         .. code:: bash
         
            $ cat zone.txt
            example.com.            IN      SOA     somewhere.example.com. someone.example.com. (
@@ -903,14 +903,32 @@
            $ cli4 --post file=@zone.txt /zones/:example.com/dns_records/import
            {
                "recs_added": 4,
                "total_records_parsed": 4
            }
            $
         
+        Zone file upload (i.e. import) Python examples (uses BIND format files)
+        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+        
+        Because ``import`` is a reserved word in Python there needs to be a slight workaround to calling this within code.
+        
+        ::
+        
+               #
+               # "import" is a reserved word and hence this code - it's ugly; but correct.
+               #
+               dns_records_import = getattr(cf.zones.dns_records, 'import')
+               r = dns_records_import.post(zone_id, files={'file':fd})
+        
+        See (examples/example_dns_import.py)[examples/example_dns_import.py] for working code.
+        
+        Zone file download (i.e. export) CLI examples (uses BIND format files)
+        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+        
         The following is documented within the **Advanced** option of the DNS page within the Cloudflare portal.
         
         ::
         
            $ cli4 /zones/:example.com/dns_records/export | egrep -v '^;;|^$'
            $ORIGIN .
            @       3600    IN      SOA     example.com.    root.example.com.       (
```

### Comparing `cloudflare-2.9.8/README.rst` & `cloudflare-2.9.9/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -866,16 +866,16 @@
        "key_type": "ECDSAP256SHA256",
        "modified_on": "2016-05-01T22:42:15.591158Z",
        "public_key": "mdsswUyr3DPW132mOi8V9xESWE8jTo0dxCjjnopKl+GqJxpVXckHAeF+KkxLbxILfDLUT0rAK9iUzy1L53eKGQ==",
        "status": "pending"
    }
    $
 
-Zone file upload and download CLI examples (uses BIND format files)
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+Zone file upload (i.e. import) CLI examples (uses BIND format files)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 Refer to `Import DNS records <https://api.cloudflare.com/#dns-records-for-a-zone-import-dns-records>`__ on API documentation for this feature.
 
 .. code:: bash
 
    $ cat zone.txt
    example.com.            IN      SOA     somewhere.example.com. someone.example.com. (
@@ -895,14 +895,32 @@
    $ cli4 --post file=@zone.txt /zones/:example.com/dns_records/import
    {
        "recs_added": 4,
        "total_records_parsed": 4
    }
    $
 
+Zone file upload (i.e. import) Python examples (uses BIND format files)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
+Because ``import`` is a reserved word in Python there needs to be a slight workaround to calling this within code.
+
+::
+
+       #
+       # "import" is a reserved word and hence this code - it's ugly; but correct.
+       #
+       dns_records_import = getattr(cf.zones.dns_records, 'import')
+       r = dns_records_import.post(zone_id, files={'file':fd})
+
+See (examples/example_dns_import.py)[examples/example_dns_import.py] for working code.
+
+Zone file download (i.e. export) CLI examples (uses BIND format files)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+
 The following is documented within the **Advanced** option of the DNS page within the Cloudflare portal.
 
 ::
 
    $ cli4 /zones/:example.com/dns_records/export | egrep -v '^;;|^$'
    $ORIGIN .
    @       3600    IN      SOA     example.com.    root.example.com.       (
```

### Comparing `cloudflare-2.9.8/cli4/cli4.1` & `cloudflare-2.9.9/cli4/cli4.1`

 * *Files identical despite different names*

### Comparing `cloudflare-2.9.8/cli4/cli4.py` & `cloudflare-2.9.9/cli4/cli4.py`

 * *Files identical despite different names*

### Comparing `cloudflare-2.9.8/cli4/converters.py` & `cloudflare-2.9.9/cli4/converters.py`

 * *Files identical despite different names*

### Comparing `cloudflare-2.9.8/cloudflare.egg-info/PKG-INFO` & `cloudflare-2.9.9/cloudflare.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: cloudflare
-Version: 2.9.8
+Version: 2.9.9
 Summary: Python wrapper for the Cloudflare v4 API
 Home-page: https://github.com/cloudflare/python-cloudflare
 Author: Martin J. Levy
 Author-email: martin@cloudflare.com
 License: MIT
 Description: cloudflare-python
         =================
@@ -874,16 +874,16 @@
                "key_type": "ECDSAP256SHA256",
                "modified_on": "2016-05-01T22:42:15.591158Z",
                "public_key": "mdsswUyr3DPW132mOi8V9xESWE8jTo0dxCjjnopKl+GqJxpVXckHAeF+KkxLbxILfDLUT0rAK9iUzy1L53eKGQ==",
                "status": "pending"
            }
            $
         
-        Zone file upload and download CLI examples (uses BIND format files)
-        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+        Zone file upload (i.e. import) CLI examples (uses BIND format files)
+        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
         
         Refer to `Import DNS records <https://api.cloudflare.com/#dns-records-for-a-zone-import-dns-records>`__ on API documentation for this feature.
         
         .. code:: bash
         
            $ cat zone.txt
            example.com.            IN      SOA     somewhere.example.com. someone.example.com. (
@@ -903,14 +903,32 @@
            $ cli4 --post file=@zone.txt /zones/:example.com/dns_records/import
            {
                "recs_added": 4,
                "total_records_parsed": 4
            }
            $
         
+        Zone file upload (i.e. import) Python examples (uses BIND format files)
+        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+        
+        Because ``import`` is a reserved word in Python there needs to be a slight workaround to calling this within code.
+        
+        ::
+        
+               #
+               # "import" is a reserved word and hence this code - it's ugly; but correct.
+               #
+               dns_records_import = getattr(cf.zones.dns_records, 'import')
+               r = dns_records_import.post(zone_id, files={'file':fd})
+        
+        See (examples/example_dns_import.py)[examples/example_dns_import.py] for working code.
+        
+        Zone file download (i.e. export) CLI examples (uses BIND format files)
+        ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+        
         The following is documented within the **Advanced** option of the DNS page within the Cloudflare portal.
         
         ::
         
            $ cli4 /zones/:example.com/dns_records/export | egrep -v '^;;|^$'
            $ORIGIN .
            @       3600    IN      SOA     example.com.    root.example.com.       (
```

### Comparing `cloudflare-2.9.8/cloudflare.egg-info/SOURCES.txt` & `cloudflare-2.9.9/cloudflare.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloudflare-2.9.8/examples/example_account_rules_lists_items.py` & `cloudflare-2.9.9/examples/example_account_rules_lists_items.py`

 * *Files identical despite different names*

### Comparing `cloudflare-2.9.8/examples/example_always_use_https.py` & `cloudflare-2.9.9/examples/example_always_use_https.py`

 * *Files identical despite different names*

### Comparing `cloudflare-2.9.8/examples/example_are_zones_ipv6.py` & `cloudflare-2.9.9/examples/example_are_zones_ipv6.py`

 * *Files identical despite different names*

### Comparing `cloudflare-2.9.8/examples/example_are_zones_ipv6_simple.py` & `cloudflare-2.9.9/examples/example_are_zones_ipv6_simple.py`

 * *Files identical despite different names*

### Comparing `cloudflare-2.9.8/examples/example_certificates.py` & `cloudflare-2.9.9/examples/example_certificates.py`

 * *Files identical despite different names*

### Comparing `cloudflare-2.9.8/examples/example_create_zone_and_populate.py` & `cloudflare-2.9.9/examples/example_create_zone_and_populate.py`

 * *Files identical despite different names*

### Comparing `cloudflare-2.9.8/examples/example_custom_hostnames.py` & `cloudflare-2.9.9/examples/example_custom_hostnames.py`

 * *Files identical despite different names*

### Comparing `cloudflare-2.9.8/examples/example_delete_zone_entry.py` & `cloudflare-2.9.9/examples/example_delete_zone_entry.py`

 * *Files identical despite different names*

### Comparing `cloudflare-2.9.8/examples/example_dns_export.py` & `cloudflare-2.9.9/examples/example_dns_export.py`

 * *Files identical despite different names*

### Comparing `cloudflare-2.9.8/examples/example_dns_import.py` & `cloudflare-2.9.9/examples/example_dns_import.py`

 * *Files identical despite different names*

### Comparing `cloudflare-2.9.8/examples/example_dnssec_settings.py` & `cloudflare-2.9.9/examples/example_dnssec_settings.py`

 * *Files identical despite different names*

### Comparing `cloudflare-2.9.8/examples/example_graphql.py` & `cloudflare-2.9.9/examples/example_graphql.py`

 * *Files identical despite different names*

### Comparing `cloudflare-2.9.8/examples/example_graphql.sh` & `cloudflare-2.9.9/examples/example_graphql.sh`

 * *Files identical despite different names*

### Comparing `cloudflare-2.9.8/examples/example_ips.py` & `cloudflare-2.9.9/examples/example_ips.py`

 * *Files identical despite different names*

### Comparing `cloudflare-2.9.8/examples/example_page_rules.py` & `cloudflare-2.9.9/examples/example_page_rules.py`

 * *Files identical despite different names*

### Comparing `cloudflare-2.9.8/examples/example_paging_thru_zones.py` & `cloudflare-2.9.9/examples/example_paging_thru_zones.py`

 * *Files identical despite different names*

### Comparing `cloudflare-2.9.8/examples/example_paging_thru_zones.sh` & `cloudflare-2.9.9/examples/example_paging_thru_zones.sh`

 * *Files identical despite different names*

### Comparing `cloudflare-2.9.8/examples/example_proxied.py` & `cloudflare-2.9.9/examples/example_proxied.py`

 * *Files identical despite different names*

### Comparing `cloudflare-2.9.8/examples/example_settings.py` & `cloudflare-2.9.9/examples/example_settings.py`

 * *Files identical despite different names*

### Comparing `cloudflare-2.9.8/examples/example_show_account_email.py` & `cloudflare-2.9.9/examples/example_show_account_email.py`

 * *Files identical despite different names*

### Comparing `cloudflare-2.9.8/examples/example_update_dynamic_dns.py` & `cloudflare-2.9.9/examples/example_update_dynamic_dns.py`

 * *Files identical despite different names*

### Comparing `cloudflare-2.9.8/examples/example_user.py` & `cloudflare-2.9.9/examples/example_user.py`

 * *Files identical despite different names*

### Comparing `cloudflare-2.9.8/examples/example_with_usage.py` & `cloudflare-2.9.9/examples/example_with_usage.py`

 * *Files identical despite different names*

### Comparing `cloudflare-2.9.8/examples/example_zones.py` & `cloudflare-2.9.9/examples/example_zones.py`

 * *Files identical despite different names*

### Comparing `cloudflare-2.9.8/setup.py` & `cloudflare-2.9.9/setup.py`

 * *Files identical despite different names*

