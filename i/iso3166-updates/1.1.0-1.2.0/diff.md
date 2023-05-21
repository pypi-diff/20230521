# Comparing `tmp/iso3166-updates-1.1.0.tar.gz` & `tmp/iso3166-updates-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iso3166-updates-1.1.0.tar", last modified: Sun May 14 18:02:32 2023, max compression
+gzip compressed data, was "iso3166-updates-1.2.0.tar", last modified: Sun May 21 14:46:30 2023, max compression
```

## Comparing `iso3166-updates-1.1.0.tar` & `iso3166-updates-1.2.0.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:02:32.526196 iso3166-updates-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-14 18:02:14.000000 iso3166-updates-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    19669 2023-05-14 18:02:32.526196 iso3166-updates-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    16133 2023-05-14 18:02:14.000000 iso3166-updates-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:02:32.526196 iso3166-updates-1.1.0/iso3166_updates/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-14 18:02:14.000000 iso3166-updates-1.1.0/iso3166_updates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24256 2023-05-14 18:02:14.000000 iso3166-updates-1.1.0/iso3166_updates/iso3166_updates.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-14 18:02:32.526196 iso3166-updates-1.1.0/iso3166_updates.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    19669 2023-05-14 18:02:32.000000 iso3166-updates-1.1.0/iso3166_updates.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-14 18:02:32.000000 iso3166-updates-1.1.0/iso3166_updates.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 18:02:32.000000 iso3166-updates-1.1.0/iso3166_updates.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-14 18:02:26.000000 iso3166-updates-1.1.0/iso3166_updates.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-14 18:02:32.000000 iso3166-updates-1.1.0/iso3166_updates.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-14 18:02:32.000000 iso3166-updates-1.1.0/iso3166_updates.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-14 18:02:32.526196 iso3166-updates-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-05-14 18:02:14.000000 iso3166-updates-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:46:30.256738 iso3166-updates-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-05-21 14:46:13.000000 iso3166-updates-1.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    19674 2023-05-21 14:46:30.256738 iso3166-updates-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    16138 2023-05-21 14:46:13.000000 iso3166-updates-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:46:30.256738 iso3166-updates-1.2.0/iso3166_updates/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-21 14:46:13.000000 iso3166-updates-1.2.0/iso3166_updates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25188 2023-05-21 14:46:13.000000 iso3166-updates-1.2.0/iso3166_updates/iso3166_updates.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 14:46:30.256738 iso3166-updates-1.2.0/iso3166_updates.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19674 2023-05-21 14:46:30.000000 iso3166-updates-1.2.0/iso3166_updates.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-21 14:46:30.000000 iso3166-updates-1.2.0/iso3166_updates.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 14:46:30.000000 iso3166-updates-1.2.0/iso3166_updates.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 14:46:23.000000 iso3166-updates-1.2.0/iso3166_updates.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-21 14:46:30.000000 iso3166-updates-1.2.0/iso3166_updates.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-21 14:46:30.000000 iso3166-updates-1.2.0/iso3166_updates.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-21 14:46:30.256738 iso3166-updates-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2989 2023-05-21 14:46:13.000000 iso3166-updates-1.2.0/setup.py
```

### Comparing `iso3166-updates-1.1.0/LICENSE` & `iso3166-updates-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `iso3166-updates-1.1.0/PKG-INFO` & `iso3166-updates-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iso3166-updates
-Version: 1.1.0
+Version: 1.2.0
 Summary: A Python package that pulls the latest updates & changes to all ISO3166 listed countries.
 Home-page: https://github.com/amckenna41/iso3166-updates
 Author: AJ McKenna, https://github.com/amckenna41
 Author-email: amckenna41@qub.ac.uk
 Maintainer: AJ McKenna
 License: MIT
 Download-URL: https://github.com/amckenna41/iso3166-updates/archive/refs/heads/main.zip
@@ -25,39 +25,39 @@
         </div>
         
         > Automated scripts and API that check for any updates/changes to the ISO 3166-1 and ISO 3166-2 country codes and naming conventions, as per the ISO 3166 newsletter (https://www.iso.org/iso-3166-country-codes.html) and Online Browsing Platform (OBP) (https://www.iso.org/obp/ui). Available via a Python software package and API; a demo of both is available [here][demo].
         
         Table of Contents
         -----------------
           * [Introduction](#introduction)
-          * [API][#API]
-          * [Staying up to date](#stayinguptodate)
+          * [API](#api)
+          * [Staying up to date](#staying-up-to-date)
           * [Requirements](#requirements)
           * [Installation](#installation)
           * [Usage](#usage)
           * [Directories](#Directories)
           * [Issues](#Issues)
           * [Contact](#contact)
           * [References](#references)
         
         Introduction
         ------------
         `iso3166-updates` is a repo that consists of a series of scripts that check for any updates/changes to the ISO 3166-2 country codes and subdivision naming conventions, as per the ISO 3166 newsletter (https://www.iso.org/iso-3166-country-codes.html). The ISO 3166 standard by the ISO (International Organization for Standardisation) defines codes for the names of countries, dependent territories, special areas of geographical interest, consolidated into the ISO 3166-1 standard [[1]](#references), and their principal subdivisions (e.g., provinces, states, departments, regions), which comprise the ISO 3166-2 standard [[2]](#references). 
         
         The ISO 3166-1 was first published in 1974 and currently comprises 249 countries, 193 of which are sovereign states that are members of the United Nations [[1]](#references). The ISO 3166-2 was first published in 1998 and as of 29 November 2022 there are 5,043 codes defined in it [[2]](#references).
         
-        ## Problem Statement:
+        ### Problem Statement:
         
         The ISO is a very dynamic organisation and regularly change/update/remove entries within its library of standards, including the ISO 3166. Additions/changes/deletions to country/territorial codes occur less often in the ISO 3166-1, but changes are more frequent for the ISO 3166-2 codes due to there being thousands more entries, thus it can be difficult to keep up with any changes to these codes. These changes can occur for a variety of geopolitical and bureaucratic reasons and are usually communicated via Newsletters on the ISO platform, their Online Browsing Platform (OBP) or via a database, which usually costs money to subscribe to [[3]](#references). Usually these updates are conveyed at the end of the year, with amendments and updates occasionally published at various times throughout the year [[4]](#references). 
         
         This software and accompanying API makes it extremely easy to check for any new or historic updates to a country or set of country's ISO 3166-2 codes for free, with an easy-to-use interface and Python package and API, ensuring that you get the most up-to-date and accurate ISO 3166-2 codes and naming conventions.
         
         <strong> The earliest date for any ISO 3166 updates is 2000-06-21, and the most recent is 2022-11-29. </strong>
         
-        ## Intended Audience:
+        ### Intended Audience:
         
         This software and accompanying API is for anyone working with country data at the ISO 3166 level. It's of high importance that the data that you are working with is correct and up-to-date, especially with consistent changes being posted every year since 2000 (excluding 2001 and 2006). Also, it's aimed not just at developers of ISO 3166 applications but for anyone working in that space, hence the creation of an easy-to-use API (https://iso3166-updates.com). 
         
         API
         ---
         An API is available that can be used to extract any applicable updates for a country via a URL. The API is available at the URL:
```

### Comparing `iso3166-updates-1.1.0/README.md` & `iso3166-updates-1.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -15,39 +15,39 @@
 </div>
 
 > Automated scripts and API that check for any updates/changes to the ISO 3166-1 and ISO 3166-2 country codes and naming conventions, as per the ISO 3166 newsletter (https://www.iso.org/iso-3166-country-codes.html) and Online Browsing Platform (OBP) (https://www.iso.org/obp/ui). Available via a Python software package and API; a demo of both is available [here][demo].
 
 Table of Contents
 -----------------
   * [Introduction](#introduction)
-  * [API][#API]
-  * [Staying up to date](#stayinguptodate)
+  * [API](#api)
+  * [Staying up to date](#staying-up-to-date)
   * [Requirements](#requirements)
   * [Installation](#installation)
   * [Usage](#usage)
   * [Directories](#Directories)
   * [Issues](#Issues)
   * [Contact](#contact)
   * [References](#references)
 
 Introduction
 ------------
 `iso3166-updates` is a repo that consists of a series of scripts that check for any updates/changes to the ISO 3166-2 country codes and subdivision naming conventions, as per the ISO 3166 newsletter (https://www.iso.org/iso-3166-country-codes.html). The ISO 3166 standard by the ISO (International Organization for Standardisation) defines codes for the names of countries, dependent territories, special areas of geographical interest, consolidated into the ISO 3166-1 standard [[1]](#references), and their principal subdivisions (e.g., provinces, states, departments, regions), which comprise the ISO 3166-2 standard [[2]](#references). 
 
 The ISO 3166-1 was first published in 1974 and currently comprises 249 countries, 193 of which are sovereign states that are members of the United Nations [[1]](#references). The ISO 3166-2 was first published in 1998 and as of 29 November 2022 there are 5,043 codes defined in it [[2]](#references).
 
-## Problem Statement:
+### Problem Statement:
 
 The ISO is a very dynamic organisation and regularly change/update/remove entries within its library of standards, including the ISO 3166. Additions/changes/deletions to country/territorial codes occur less often in the ISO 3166-1, but changes are more frequent for the ISO 3166-2 codes due to there being thousands more entries, thus it can be difficult to keep up with any changes to these codes. These changes can occur for a variety of geopolitical and bureaucratic reasons and are usually communicated via Newsletters on the ISO platform, their Online Browsing Platform (OBP) or via a database, which usually costs money to subscribe to [[3]](#references). Usually these updates are conveyed at the end of the year, with amendments and updates occasionally published at various times throughout the year [[4]](#references). 
 
 This software and accompanying API makes it extremely easy to check for any new or historic updates to a country or set of country's ISO 3166-2 codes for free, with an easy-to-use interface and Python package and API, ensuring that you get the most up-to-date and accurate ISO 3166-2 codes and naming conventions.
 
 <strong> The earliest date for any ISO 3166 updates is 2000-06-21, and the most recent is 2022-11-29. </strong>
 
-## Intended Audience:
+### Intended Audience:
 
 This software and accompanying API is for anyone working with country data at the ISO 3166 level. It's of high importance that the data that you are working with is correct and up-to-date, especially with consistent changes being posted every year since 2000 (excluding 2001 and 2006). Also, it's aimed not just at developers of ISO 3166 applications but for anyone working in that space, hence the creation of an easy-to-use API (https://iso3166-updates.com). 
 
 API
 ---
 An API is available that can be used to extract any applicable updates for a country via a URL. The API is available at the URL:
```

### Comparing `iso3166-updates-1.1.0/iso3166_updates/iso3166_updates.py` & `iso3166-updates-1.2.0/iso3166_updates/iso3166_updates.py`

 * *Files 5% similar despite different names*

```diff
@@ -89,14 +89,46 @@
     if (isinstance(alpha2_codes, list) and len(alpha2_codes) == 1 and ',' in alpha2_codes[0]):
         alpha2_codes = alpha2_codes[0].replace(' ', '').split(',')
 
     #if single str input for Year param then convert to array, remove whitespace
     if (isinstance(year, str)):
         year = year.replace(' ', '').split(',')
 
+    def convert_to_alpha2(alpha3_code):
+        """ 
+        Convert an ISO3166 country's 3 letter alpha-3 code into its 2 letter
+        alpha-2 counterpart. 
+
+        Parameters 
+        ----------
+        :alpha3_code: str
+            3 letter ISO3166 country code.
+        
+        Returns
+        -------
+        :iso3166.countries_by_alpha3[alpha3_code].alpha2: str
+            2 letter ISO3166 country code. 
+        """
+        #return error if 3 letter alpha-3 code not found
+        if not (alpha3_code in list(iso3166.countries_by_alpha3.keys())):
+            return None
+        else:
+            #use iso3166 package to find corresponding alpha-2 code from its alpha-3
+            return iso3166.countries_by_alpha3[alpha3_code].alpha2
+    
+    #if 3 letter alpha-3 codes input then convert to corresponding alpha-2, else raise error
+    if (alpha2_codes != []):
+        for code in range(0, len(alpha2_codes)):
+            if (len(alpha2_codes[code]) == 3): 
+                temp_alpha2_code = convert_to_alpha2(alpha2_codes[code])
+                if not (temp_alpha2_code is None):
+                    alpha2_codes[code] = temp_alpha2_code
+                else:
+                    raise ValueError("Invalid alpha-3 code input, cannot convert into corresponding alpha-2 code: {}.".format(alpha2_codes[code]))
+
     #use all ISO3166 codes if invalid alpha-2 code input, otherwise convert alpha-2 to array
     if (alpha2_codes == []):
         alpha2_codes = sorted(list(iso3166.countries_by_alpha2.keys()))
 
     #sort codes in alphabetical order
     alpha2_codes.sort()
     alpha2_codes = [code.upper() for code in alpha2_codes]
@@ -151,15 +183,15 @@
         
         export_fname = export_filename + '-' + alpha2  
 
         #skip to next iteration if alpha-2 not valid
         if (alpha2 not in list(iso3166.countries_by_alpha2.keys())):
             continue
 
-        print("ISO Code: {} ({})".format(alpha2, wiki_base_url + alpha2))
+        print("ISO 3166 Code: {} ({})".format(alpha2, wiki_base_url + alpha2))
 
         all_changes[alpha2] = {}
 
         #get html content from wiki of ISO3166 page, raise exception if status code != 200
         try:
             page = requests.get(wiki_base_url + alpha2, headers=USER_AGENT_HEADER)
             page.raise_for_status()
@@ -222,21 +254,14 @@
             #convert date column to datetime object
             iso3166_df['Date Issued'] = pd.to_datetime(iso3166_df["Date Issued"])
             #sort and order by date, newest to oldest
             iso3166_df = iso3166_df.sort_values(by=['Date Issued'], ascending=False)
             #convert date column back to string 
             iso3166_df['Date Issued'] = iso3166_df['Date Issued'].astype(str)
 
-            def convert_date_format(row):
-                """ convert date in rows of df into dd-mm-yyyy data format from date object. """
-                return datetime.datetime.strptime(row.replace('\n', ''), '%Y-%m-%d').strftime('%d-%m-%Y')
-
-            #convert date column into dd-mm-yyyy format  
-            iso3166_df["Date Issued"] = iso3166_df["Date Issued"].apply(convert_date_format)
-
             #export to csv, append extension if applicable
             if (export_csv): 
                 if (os.path.splitext(export_json_filename)[1] != ".csv"):
                     export_fname = export_fname + ".csv"
                 iso3166_df.to_csv(os.path.join(export_folder, export_fname), index=False)
         
             #add ISO updates to object of all ISO3166 updates, convert to json
```

### Comparing `iso3166-updates-1.1.0/iso3166_updates.egg-info/PKG-INFO` & `iso3166-updates-1.2.0/iso3166_updates.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iso3166-updates
-Version: 1.1.0
+Version: 1.2.0
 Summary: A Python package that pulls the latest updates & changes to all ISO3166 listed countries.
 Home-page: https://github.com/amckenna41/iso3166-updates
 Author: AJ McKenna, https://github.com/amckenna41
 Author-email: amckenna41@qub.ac.uk
 Maintainer: AJ McKenna
 License: MIT
 Download-URL: https://github.com/amckenna41/iso3166-updates/archive/refs/heads/main.zip
@@ -25,39 +25,39 @@
         </div>
         
         > Automated scripts and API that check for any updates/changes to the ISO 3166-1 and ISO 3166-2 country codes and naming conventions, as per the ISO 3166 newsletter (https://www.iso.org/iso-3166-country-codes.html) and Online Browsing Platform (OBP) (https://www.iso.org/obp/ui). Available via a Python software package and API; a demo of both is available [here][demo].
         
         Table of Contents
         -----------------
           * [Introduction](#introduction)
-          * [API][#API]
-          * [Staying up to date](#stayinguptodate)
+          * [API](#api)
+          * [Staying up to date](#staying-up-to-date)
           * [Requirements](#requirements)
           * [Installation](#installation)
           * [Usage](#usage)
           * [Directories](#Directories)
           * [Issues](#Issues)
           * [Contact](#contact)
           * [References](#references)
         
         Introduction
         ------------
         `iso3166-updates` is a repo that consists of a series of scripts that check for any updates/changes to the ISO 3166-2 country codes and subdivision naming conventions, as per the ISO 3166 newsletter (https://www.iso.org/iso-3166-country-codes.html). The ISO 3166 standard by the ISO (International Organization for Standardisation) defines codes for the names of countries, dependent territories, special areas of geographical interest, consolidated into the ISO 3166-1 standard [[1]](#references), and their principal subdivisions (e.g., provinces, states, departments, regions), which comprise the ISO 3166-2 standard [[2]](#references). 
         
         The ISO 3166-1 was first published in 1974 and currently comprises 249 countries, 193 of which are sovereign states that are members of the United Nations [[1]](#references). The ISO 3166-2 was first published in 1998 and as of 29 November 2022 there are 5,043 codes defined in it [[2]](#references).
         
-        ## Problem Statement:
+        ### Problem Statement:
         
         The ISO is a very dynamic organisation and regularly change/update/remove entries within its library of standards, including the ISO 3166. Additions/changes/deletions to country/territorial codes occur less often in the ISO 3166-1, but changes are more frequent for the ISO 3166-2 codes due to there being thousands more entries, thus it can be difficult to keep up with any changes to these codes. These changes can occur for a variety of geopolitical and bureaucratic reasons and are usually communicated via Newsletters on the ISO platform, their Online Browsing Platform (OBP) or via a database, which usually costs money to subscribe to [[3]](#references). Usually these updates are conveyed at the end of the year, with amendments and updates occasionally published at various times throughout the year [[4]](#references). 
         
         This software and accompanying API makes it extremely easy to check for any new or historic updates to a country or set of country's ISO 3166-2 codes for free, with an easy-to-use interface and Python package and API, ensuring that you get the most up-to-date and accurate ISO 3166-2 codes and naming conventions.
         
         <strong> The earliest date for any ISO 3166 updates is 2000-06-21, and the most recent is 2022-11-29. </strong>
         
-        ## Intended Audience:
+        ### Intended Audience:
         
         This software and accompanying API is for anyone working with country data at the ISO 3166 level. It's of high importance that the data that you are working with is correct and up-to-date, especially with consistent changes being posted every year since 2000 (excluding 2001 and 2006). Also, it's aimed not just at developers of ISO 3166 applications but for anyone working in that space, hence the creation of an easy-to-use API (https://iso3166-updates.com). 
         
         API
         ---
         An API is available that can be used to extract any applicable updates for a country via a URL. The API is available at the URL:
```

### Comparing `iso3166-updates-1.1.0/setup.cfg` & `iso3166-updates-1.2.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = iso3166-updates
-version = 1.1.0
+version = 1.2.0
 description = A Python package that pulls the latest updates & changes to all ISO3166 listed countries.
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = AJ McKenna
 author_email = amckenna41@qub.ac.uk
 url = https://github.com/amckenna41/iso3166-updates
 download_url = https://github.com/amckenna41/iso3166-updates/archive/refs/heads/main.zip
```

### Comparing `iso3166-updates-1.1.0/setup.py` & `iso3166-updates-1.2.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import pathlib
 from setuptools import setup, find_packages
 import sys
 # import iso3166_updates
 
 #software metadata
 __name__ = 'iso3166-updates'
-__version__ = "1.1.0"
+__version__ = "1.2.0"
 __description__ = "A Python package that pulls the latest updates & changes to all ISO3166 listed countries."
 __author__ = 'AJ McKenna, https://github.com/amckenna41'
 __authorEmail__ = 'amckenna41@qub.ac.uk'
 __license__ = 'MIT'
 __url__ = 'https://github.com/amckenna41/iso3166-updates'
 __download_url__ = "https://github.com/amckenna41/iso3166-updates/archive/refs/heads/main.zip"
 __status__ = 'Development'
```

