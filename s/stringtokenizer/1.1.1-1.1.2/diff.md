# Comparing `tmp/stringtokenizer-1.1.1.tar.gz` & `tmp/stringtokenizer-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stringtokenizer-1.1.1.tar", last modified: Sat May 20 18:10:40 2023, max compression
+gzip compressed data, was "stringtokenizer-1.1.2.tar", last modified: Sun May 21 05:54:25 2023, max compression
```

## Comparing `stringtokenizer-1.1.1.tar` & `stringtokenizer-1.1.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0 tanmay    (1000) tanmay    (1000)        0 2023-05-20 18:10:40.592958 stringtokenizer-1.1.1/
--rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)     1444 2023-05-20 18:10:40.592626 stringtokenizer-1.1.1/PKG-INFO
--rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)      933 2023-05-20 18:09:24.000000 stringtokenizer-1.1.1/README.md
--rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)       38 2023-05-20 18:10:40.593043 stringtokenizer-1.1.1/setup.cfg
--rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)      448 2023-05-20 18:10:31.000000 stringtokenizer-1.1.1/setup.py
-drwxrwxrwx   0 tanmay    (1000) tanmay    (1000)        0 2023-05-20 18:10:40.590321 stringtokenizer-1.1.1/stringtokenizer/
--rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)       46 2023-05-17 18:44:19.000000 stringtokenizer-1.1.1/stringtokenizer/__init__.py
--rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)     1611 2023-05-18 09:51:18.000000 stringtokenizer-1.1.1/stringtokenizer/stringtokenizer.py
-drwxrwxrwx   0 tanmay    (1000) tanmay    (1000)        0 2023-05-20 18:10:40.592134 stringtokenizer-1.1.1/stringtokenizer.egg-info/
--rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)     1444 2023-05-20 18:10:40.000000 stringtokenizer-1.1.1/stringtokenizer.egg-info/PKG-INFO
--rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)      237 2023-05-20 18:10:40.000000 stringtokenizer-1.1.1/stringtokenizer.egg-info/SOURCES.txt
--rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)        1 2023-05-20 18:10:40.000000 stringtokenizer-1.1.1/stringtokenizer.egg-info/dependency_links.txt
--rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)       16 2023-05-20 18:10:40.000000 stringtokenizer-1.1.1/stringtokenizer.egg-info/top_level.txt
+drwxrwxrwx   0 tanmay    (1000) tanmay    (1000)        0 2023-05-21 05:54:25.678735 stringtokenizer-1.1.2/
+-rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)     1464 2023-05-21 05:54:25.678442 stringtokenizer-1.1.2/PKG-INFO
+-rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)      953 2023-05-21 05:54:17.000000 stringtokenizer-1.1.2/README.md
+-rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)       38 2023-05-21 05:54:25.678821 stringtokenizer-1.1.2/setup.cfg
+-rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)      448 2023-05-21 05:50:46.000000 stringtokenizer-1.1.2/setup.py
+drwxrwxrwx   0 tanmay    (1000) tanmay    (1000)        0 2023-05-21 05:54:25.675643 stringtokenizer-1.1.2/stringtokenizer/
+-rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)       46 2023-05-17 18:44:19.000000 stringtokenizer-1.1.2/stringtokenizer/__init__.py
+-rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)     1595 2023-05-21 05:49:54.000000 stringtokenizer-1.1.2/stringtokenizer/stringtokenizer.py
+drwxrwxrwx   0 tanmay    (1000) tanmay    (1000)        0 2023-05-21 05:54:25.677532 stringtokenizer-1.1.2/stringtokenizer.egg-info/
+-rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)     1464 2023-05-21 05:54:25.000000 stringtokenizer-1.1.2/stringtokenizer.egg-info/PKG-INFO
+-rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)      237 2023-05-21 05:54:25.000000 stringtokenizer-1.1.2/stringtokenizer.egg-info/SOURCES.txt
+-rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)        1 2023-05-21 05:54:25.000000 stringtokenizer-1.1.2/stringtokenizer.egg-info/dependency_links.txt
+-rwxrwxrwx   0 tanmay    (1000) tanmay    (1000)       16 2023-05-21 05:54:25.000000 stringtokenizer-1.1.2/stringtokenizer.egg-info/top_level.txt
```

### Comparing `stringtokenizer-1.1.1/PKG-INFO` & `stringtokenizer-1.1.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 Metadata-Version: 2.1
 Name: stringtokenizer
-Version: 1.1.1
+Version: 1.1.2
 Summary: A string tokenizer implementation
 Home-page: UNKNOWN
 Author: Tanmay Mandal
 License: UNKNOWN
-Description: This project is a python implementation of the StringTokenizer class present in java
+Description: **This project is a python implementation of the StringTokenizer class present in java**
         
         
-        How to import ?
+        __How to import ?__
         
         from stringtokenizer import StringTokenizer
         
         
-        How to declare object?
+        __How to declare object?__
         
         s1=StringTokenizer(st)-->uses default delimeter set
         
         s2=StringTokenizer(st,delim)-->uses provided delim set. Uses each character present in provided delim string as delimeters
         
         s3=StringTokenizer(st,delim,retdelim)-->same as no. 2 but returns delim as tokens depending on True/False of retdelim
         
         
-        Functions Contained and how to use?
+        __Functions Contained and how to use?__
         
         s1=StringTokenizer(st)
         
         s1.countTokens()-->returns number of tokens left to parse
         
         s1.hasMoreTokens()-->returns True/False depending on wheather any more tokens are left to parse
         
         s1.nextToken()-->returns next Token
         
         s1.nextToken(delim)-->returns next token based on the provided delim and updates the previously provided delim with the new ones
         
         
-        made by Tanmay Mandal
+        **made by Tanmay Mandal**
         for any query please mail on tanmay.mandal@zohomail.in
         
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `stringtokenizer-1.1.1/README.md` & `stringtokenizer-1.1.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-This project is a python implementation of the StringTokenizer class present in java
+**This project is a python implementation of the StringTokenizer class present in java**
 
 
-How to import ?
+__How to import ?__
 
 from stringtokenizer import StringTokenizer
 
 
-How to declare object?
+__How to declare object?__
 
 s1=StringTokenizer(st)-->uses default delimeter set
 
 s2=StringTokenizer(st,delim)-->uses provided delim set. Uses each character present in provided delim string as delimeters
 
 s3=StringTokenizer(st,delim,retdelim)-->same as no. 2 but returns delim as tokens depending on True/False of retdelim
 
 
-Functions Contained and how to use?
+__Functions Contained and how to use?__
 
 s1=StringTokenizer(st)
 
 s1.countTokens()-->returns number of tokens left to parse
 
 s1.hasMoreTokens()-->returns True/False depending on wheather any more tokens are left to parse
 
 s1.nextToken()-->returns next Token
 
 s1.nextToken(delim)-->returns next token based on the provided delim and updates the previously provided delim with the new ones
 
 
-made by Tanmay Mandal
+**made by Tanmay Mandal**
 for any query please mail on tanmay.mandal@zohomail.in
```

### Comparing `stringtokenizer-1.1.1/stringtokenizer/stringtokenizer.py` & `stringtokenizer-1.1.2/stringtokenizer/stringtokenizer.py`

 * *Files 14% similar despite different names*

```diff
@@ -40,14 +40,14 @@
         except Exception:
             r=False
         return r
     def countTokens(self):
         c=0
         temp=list(self.__tokens)
         try:
-            while self.hasMoreTokens():
+            while True:
                 self.nextToken()
                 c+=1
         except Exception:
             pass
         self.__tokens=temp
         return c
```

### Comparing `stringtokenizer-1.1.1/stringtokenizer.egg-info/PKG-INFO` & `stringtokenizer-1.1.2/stringtokenizer.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 Metadata-Version: 2.1
 Name: stringtokenizer
-Version: 1.1.1
+Version: 1.1.2
 Summary: A string tokenizer implementation
 Home-page: UNKNOWN
 Author: Tanmay Mandal
 License: UNKNOWN
-Description: This project is a python implementation of the StringTokenizer class present in java
+Description: **This project is a python implementation of the StringTokenizer class present in java**
         
         
-        How to import ?
+        __How to import ?__
         
         from stringtokenizer import StringTokenizer
         
         
-        How to declare object?
+        __How to declare object?__
         
         s1=StringTokenizer(st)-->uses default delimeter set
         
         s2=StringTokenizer(st,delim)-->uses provided delim set. Uses each character present in provided delim string as delimeters
         
         s3=StringTokenizer(st,delim,retdelim)-->same as no. 2 but returns delim as tokens depending on True/False of retdelim
         
         
-        Functions Contained and how to use?
+        __Functions Contained and how to use?__
         
         s1=StringTokenizer(st)
         
         s1.countTokens()-->returns number of tokens left to parse
         
         s1.hasMoreTokens()-->returns True/False depending on wheather any more tokens are left to parse
         
         s1.nextToken()-->returns next Token
         
         s1.nextToken(delim)-->returns next token based on the provided delim and updates the previously provided delim with the new ones
         
         
-        made by Tanmay Mandal
+        **made by Tanmay Mandal**
         for any query please mail on tanmay.mandal@zohomail.in
         
 Platform: UNKNOWN
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

