# Comparing `tmp/discoger-1.1.6.tar.gz` & `tmp/discoger-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discoger-1.1.6.tar", last modified: Mon May 15 10:51:00 2023, max compression
+gzip compressed data, was "discoger-1.2.0.tar", last modified: Sun May 21 20:10:34 2023, max compression
```

## Comparing `discoger-1.1.6.tar` & `discoger-1.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:51:00.371171 discoger-1.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-15 10:50:47.000000 discoger-1.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-05-15 10:51:00.371171 discoger-1.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-05-15 10:50:47.000000 discoger-1.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:51:00.371171 discoger-1.1.6/discoger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-15 10:50:47.000000 discoger-1.1.6/discoger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-15 10:50:47.000000 discoger-1.1.6/discoger/_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     9383 2023-05-15 10:50:47.000000 discoger-1.1.6/discoger/discoger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-15 10:51:00.371171 discoger-1.1.6/discoger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-05-15 10:51:00.000000 discoger-1.1.6/discoger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-15 10:51:00.000000 discoger-1.1.6/discoger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-15 10:51:00.000000 discoger-1.1.6/discoger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-15 10:51:00.000000 discoger-1.1.6/discoger.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-15 10:51:00.000000 discoger-1.1.6/discoger.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-15 10:51:00.000000 discoger-1.1.6/discoger.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-15 10:51:00.371171 discoger-1.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-05-15 10:50:47.000000 discoger-1.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:10:34.331069 discoger-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-21 20:10:15.000000 discoger-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-05-21 20:10:34.331069 discoger-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-05-21 20:10:15.000000 discoger-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:10:34.331069 discoger-1.2.0/discoger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 20:10:15.000000 discoger-1.2.0/discoger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-21 20:10:15.000000 discoger-1.2.0/discoger/_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9746 2023-05-21 20:10:15.000000 discoger-1.2.0/discoger/discoger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 20:10:34.331069 discoger-1.2.0/discoger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2786 2023-05-21 20:10:34.000000 discoger-1.2.0/discoger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-21 20:10:34.000000 discoger-1.2.0/discoger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 20:10:34.000000 discoger-1.2.0/discoger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-21 20:10:34.000000 discoger-1.2.0/discoger.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-21 20:10:34.000000 discoger-1.2.0/discoger.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-21 20:10:34.000000 discoger-1.2.0/discoger.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-21 20:10:34.331069 discoger-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-05-21 20:10:15.000000 discoger-1.2.0/setup.py
```

### Comparing `discoger-1.1.6/LICENSE` & `discoger-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `discoger-1.1.6/PKG-INFO` & `discoger-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: discoger
-Version: 1.1.6
+Version: 1.2.0
 Summary: Get notification from Discogs
 Home-page: https://github.com/beudbeud/discoger
 Author: Beudbeud
 Author-email: beudbeud@gmail.com
 License: GNU General Public License v3 (GPLv3)
-Download-URL: https://github.com/beudbeud/discoger/archive/1.1.6.tar.gz
+Download-URL: https://github.com/beudbeud/discoger/archive/1.2.0.tar.gz
 Description: # Discoger
         
         Discoger Bot is a Telegram bot that allows you to be notified when a new sale for a vinyl in your Discogs wantlist is available.
         
         ## Usage
         
         1. Search for the Telegram bot "Discoger" or click [this link](https://t.me/Discogers_bot) to open a conversation with the bot.
```

### Comparing `discoger-1.1.6/README.md` & `discoger-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `discoger-1.1.6/discoger/discoger.py` & `discoger-1.2.0/discoger/discoger.py`

 * *Files 2% similar despite different names*

```diff
@@ -176,14 +176,22 @@
         else:
             return data_last_sell
     except Exception as e:
         logging.debug("%s: for %s item" % (e, release_id))
         return None
 
 
+def check_price(release_id, type_sell):
+    if type_sell == 'master':
+        _info = d.master(release_id)
+    else:
+        _info = d.release(release_id)
+    return "%s %s" % (round(_info.price_suggestions.mint.value, 2), _info.price_suggestions.mint.currency)
+
+
 def check_discogs(chat_id=None):
     if chat_id:
         logging.info("Check user list %s" % (chat_id))
         scrap_data(chat_id)
     else:
         logging.info("Check all list")
         for x in database_dir.iterdir():
@@ -199,17 +207,18 @@
         item = db.search("release_list[%s]" % (str(i)))
         sell_type = item.get("type")
         if sell_type is None:
             sell_type = "release"
         data_last_sell = check_sales(item["release_id"], sell_type)
         if data_last_sell:
             if not item["last_sell"] or (item["last_sell"]["id"] != data_last_sell["id"] and item["last_sell"]["date"] < data_last_sell["date"]):
+                good_price = check_price(item["release_id"], sell_type)
                 logging.info("New item for %s - %s" % (item["artist"], item["title"]))
-                text = "New release for:\n%s - %s\ndate: %s\nprice: %s\n%s" % (item["artist"], item["title"], data_last_sell["date"], data_last_sell["price"], data_last_sell["url"])
-                bot.send_message(chat_id, text, disable_web_page_preview=False)
+                text = "New release for:\n%s - %s\nDate: %s\nPrice: %s\nGood price: %s\n%s" % (item["artist"], item["title"], data_last_sell["date"], data_last_sell["price"], good_price, data_last_sell["url"])
+                bot.send_message(chat_id, text, disable_web_page_preview=True)
                 db["release_list"][i]["last_sell"] = data_last_sell
             else:
                 logging.info("Not new item for %s - %s" % (db["release_list"][i]["artist"], db["release_list"][i]["title"]))
         else:
             logging.info("Nothing available for %s - %s" % (db["release_list"][i]["artist"], db["release_list"][i]["title"]))
     db.save()
```

### Comparing `discoger-1.1.6/discoger.egg-info/PKG-INFO` & `discoger-1.2.0/discoger.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: discoger
-Version: 1.1.6
+Version: 1.2.0
 Summary: Get notification from Discogs
 Home-page: https://github.com/beudbeud/discoger
 Author: Beudbeud
 Author-email: beudbeud@gmail.com
 License: GNU General Public License v3 (GPLv3)
-Download-URL: https://github.com/beudbeud/discoger/archive/1.1.6.tar.gz
+Download-URL: https://github.com/beudbeud/discoger/archive/1.2.0.tar.gz
 Description: # Discoger
         
         Discoger Bot is a Telegram bot that allows you to be notified when a new sale for a vinyl in your Discogs wantlist is available.
         
         ## Usage
         
         1. Search for the Telegram bot "Discoger" or click [this link](https://t.me/Discogers_bot) to open a conversation with the bot.
```

### Comparing `discoger-1.1.6/setup.py` & `discoger-1.2.0/setup.py`

 * *Files identical despite different names*

