# Comparing `tmp/issue_db_api-0.9.2.tar.gz` & `tmp/issue_db_api-0.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "issue_db_api-0.9.2.tar", last modified: Mon May 15 12:02:55 2023, max compression
+gzip compressed data, was "issue_db_api-0.9.3.tar", last modified: Sun May 21 10:06:37 2023, max compression
```

## Comparing `issue_db_api-0.9.2.tar` & `issue_db_api-0.9.3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-15 12:02:55.872726 issue_db_api-0.9.2/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       82 2023-04-20 09:20:00.000000 issue_db_api-0.9.2/.gitignore
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     1069 2023-04-20 08:15:34.000000 issue_db_api-0.9.2/LICENSE
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      103 2023-04-20 08:15:34.000000 issue_db_api-0.9.2/MANIFEST.in
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      551 2023-05-15 12:02:55.872726 issue_db_api-0.9.2/PKG-INFO
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      200 2023-04-20 08:15:34.000000 issue_db_api-0.9.2/README.md
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-15 12:02:55.868726 issue_db_api-0.9.2/issue_db_api/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      519 2023-05-15 11:58:40.000000 issue_db_api-0.9.2/issue_db_api/Cargo.toml
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       25 2023-05-04 14:06:56.000000 issue_db_api-0.9.2/issue_db_api/__init__.py
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     9283 2023-05-15 12:02:30.000000 issue_db_api-0.9.2/issue_db_api/issue_api.pyi
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-15 12:02:55.872726 issue_db_api-0.9.2/issue_db_api/src/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)    46895 2023-05-15 10:40:01.000000 issue_db_api-0.9.2/issue_db_api/src/api_core.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     1049 2023-05-04 13:53:55.000000 issue_db_api-0.9.2/issue_db_api/src/comments.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     5322 2023-05-11 12:05:05.000000 issue_db_api-0.9.2/issue_db_api/src/config.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     3788 2023-05-04 13:53:55.000000 issue_db_api-0.9.2/issue_db_api/src/embedding.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     2105 2023-05-12 10:30:49.000000 issue_db_api-0.9.2/issue_db_api/src/errors.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     1622 2023-05-15 10:43:58.000000 issue_db_api-0.9.2/issue_db_api/src/files.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     6635 2023-05-11 12:09:47.000000 issue_db_api-0.9.2/issue_db_api/src/issues.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      571 2023-04-20 08:15:34.000000 issue_db_api-0.9.2/issue_db_api/src/labels.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)    41834 2023-05-15 11:58:40.000000 issue_db_api-0.9.2/issue_db_api/src/lib.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)    10983 2023-05-04 13:53:55.000000 issue_db_api-0.9.2/issue_db_api/src/models.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     3910 2023-05-01 16:59:08.000000 issue_db_api-0.9.2/issue_db_api/src/query.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     7669 2023-05-15 11:58:40.000000 issue_db_api-0.9.2/issue_db_api/src/repository.rs
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-15 12:02:55.872726 issue_db_api-0.9.2/issue_db_api/src/schemas/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     5031 2023-04-20 08:15:34.000000 issue_db_api-0.9.2/issue_db_api/src/schemas/raw_issue_response.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       27 2023-04-20 08:15:34.000000 issue_db_api-0.9.2/issue_db_api/src/schemas.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     1626 2023-05-04 13:53:55.000000 issue_db_api-0.9.2/issue_db_api/src/tags.rs
--rw-rw-r--   0 jesse     (1000) jesse     (1000)     2583 2023-05-11 11:58:07.000000 issue_db_api-0.9.2/issue_db_api/src/util.rs
-drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-15 12:02:55.868726 issue_db_api-0.9.2/issue_db_api.egg-info/
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      551 2023-05-15 12:02:55.000000 issue_db_api-0.9.2/issue_db_api.egg-info/PKG-INFO
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      774 2023-05-15 12:02:55.000000 issue_db_api-0.9.2/issue_db_api.egg-info/SOURCES.txt
--rw-rw-r--   0 jesse     (1000) jesse     (1000)        1 2023-05-15 12:02:55.000000 issue_db_api-0.9.2/issue_db_api.egg-info/dependency_links.txt
--rw-rw-r--   0 jesse     (1000) jesse     (1000)        1 2023-04-20 09:21:05.000000 issue_db_api-0.9.2/issue_db_api.egg-info/not-zip-safe
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       13 2023-05-15 12:02:55.000000 issue_db_api-0.9.2/issue_db_api.egg-info/top_level.txt
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      529 2023-05-15 12:02:30.000000 issue_db_api-0.9.2/pyproject.toml
--rw-rw-r--   0 jesse     (1000) jesse     (1000)       38 2023-05-15 12:02:55.872726 issue_db_api-0.9.2/setup.cfg
--rw-rw-r--   0 jesse     (1000) jesse     (1000)      253 2023-04-20 08:15:34.000000 issue_db_api-0.9.2/setup.py
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-21 10:06:37.386626 issue_db_api-0.9.3/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       82 2023-04-20 09:20:00.000000 issue_db_api-0.9.3/.gitignore
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     1069 2023-04-20 08:15:34.000000 issue_db_api-0.9.3/LICENSE
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      103 2023-04-20 08:15:34.000000 issue_db_api-0.9.3/MANIFEST.in
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      551 2023-05-21 10:06:37.386626 issue_db_api-0.9.3/PKG-INFO
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      200 2023-04-20 08:15:34.000000 issue_db_api-0.9.3/README.md
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-21 10:06:37.382626 issue_db_api-0.9.3/issue_db_api/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      519 2023-05-21 10:01:40.000000 issue_db_api-0.9.3/issue_db_api/Cargo.toml
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       25 2023-05-04 14:06:56.000000 issue_db_api-0.9.3/issue_db_api/__init__.py
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     9333 2023-05-21 09:55:20.000000 issue_db_api-0.9.3/issue_db_api/issue_api.pyi
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-21 10:06:37.386626 issue_db_api-0.9.3/issue_db_api/src/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)    47215 2023-05-21 10:01:27.000000 issue_db_api-0.9.3/issue_db_api/src/api_core.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     1049 2023-05-04 13:53:55.000000 issue_db_api-0.9.3/issue_db_api/src/comments.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     5322 2023-05-11 12:05:05.000000 issue_db_api-0.9.3/issue_db_api/src/config.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     3788 2023-05-04 13:53:55.000000 issue_db_api-0.9.3/issue_db_api/src/embedding.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     2105 2023-05-12 10:30:49.000000 issue_db_api-0.9.3/issue_db_api/src/errors.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     1622 2023-05-15 10:43:58.000000 issue_db_api-0.9.3/issue_db_api/src/files.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     6635 2023-05-11 12:09:47.000000 issue_db_api-0.9.3/issue_db_api/src/issues.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      571 2023-04-20 08:15:34.000000 issue_db_api-0.9.3/issue_db_api/src/labels.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)    41834 2023-05-15 11:58:40.000000 issue_db_api-0.9.3/issue_db_api/src/lib.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)    10983 2023-05-04 13:53:55.000000 issue_db_api-0.9.3/issue_db_api/src/models.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     3910 2023-05-01 16:59:08.000000 issue_db_api-0.9.3/issue_db_api/src/query.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     7669 2023-05-15 11:58:40.000000 issue_db_api-0.9.3/issue_db_api/src/repository.rs
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-21 10:06:37.386626 issue_db_api-0.9.3/issue_db_api/src/schemas/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     5031 2023-04-20 08:15:34.000000 issue_db_api-0.9.3/issue_db_api/src/schemas/raw_issue_response.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       27 2023-04-20 08:15:34.000000 issue_db_api-0.9.3/issue_db_api/src/schemas.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     1626 2023-05-04 13:53:55.000000 issue_db_api-0.9.3/issue_db_api/src/tags.rs
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)     2583 2023-05-11 11:58:07.000000 issue_db_api-0.9.3/issue_db_api/src/util.rs
+drwxrwxr-x   0 jesse     (1000) jesse     (1000)        0 2023-05-21 10:06:37.382626 issue_db_api-0.9.3/issue_db_api.egg-info/
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      551 2023-05-21 10:06:37.000000 issue_db_api-0.9.3/issue_db_api.egg-info/PKG-INFO
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      774 2023-05-21 10:06:37.000000 issue_db_api-0.9.3/issue_db_api.egg-info/SOURCES.txt
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)        1 2023-05-21 10:06:37.000000 issue_db_api-0.9.3/issue_db_api.egg-info/dependency_links.txt
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)        1 2023-04-20 09:21:05.000000 issue_db_api-0.9.3/issue_db_api.egg-info/not-zip-safe
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       13 2023-05-21 10:06:37.000000 issue_db_api-0.9.3/issue_db_api.egg-info/top_level.txt
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      529 2023-05-21 10:01:40.000000 issue_db_api-0.9.3/pyproject.toml
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)       38 2023-05-21 10:06:37.386626 issue_db_api-0.9.3/setup.cfg
+-rw-rw-r--   0 jesse     (1000) jesse     (1000)      253 2023-04-20 08:15:34.000000 issue_db_api-0.9.3/setup.py
```

### Comparing `issue_db_api-0.9.2/LICENSE` & `issue_db_api-0.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.9.2/PKG-INFO` & `issue_db_api-0.9.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: issue_db_api
-Version: 0.9.2
+Version: 0.9.3
 Author: Jesse Maarleveld
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `issue_db_api-0.9.2/issue_db_api/Cargo.toml` & `issue_db_api-0.9.3/issue_db_api/Cargo.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "issue-api-client"
-version = "0.9.1"
+version = "0.9.2"
 edition = "2021"
 
 [lib]
 name = "issue_api"
 crate-type = ["cdylib"]
 
 [features]
```

### Comparing `issue_db_api-0.9.2/issue_db_api/issue_api.pyi` & `issue_db_api-0.9.3/issue_db_api/issue_api.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -127,14 +127,17 @@
         ...
 
     def tag(self, name: str) -> Query:
         ...
 
     def not_tag(self, name: str) -> Query:
         ...
+    
+    def to_json(self) -> object:
+        ...
 
 
 class Label:
 
     def __init__(self,
                  existence: bool,
                  executive: bool,
```

### Comparing `issue_db_api-0.9.2/issue_db_api/src/api_core.rs` & `issue_db_api-0.9.3/issue_db_api/src/api_core.rs`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 use std::collections::HashMap;
 use std::io::Cursor;
+use std::time::Duration;
 
 #[cfg(feature = "blocking")]
 use reqwest::blocking::multipart;
 
 use serde_json::{Map, Value};
 use lazy_init::Lazy;
 
@@ -16,14 +17,17 @@
 use crate::tags::UnboundTag;
 use crate::util::initialize_lazy_field;
 use crate::errors::APIResult;
 use crate::errors::*;
 use crate::files::UnboundFile;
 use crate::models::{ModelInfo, UnboundModelConfig, UnboundModelVersion, UnboundTestRun};
 
+const CONNECT_TIMEOUT: Duration = Duration::new(30, 0);
+const READ_WRITE_TIMEOUT: Duration = Duration::new(10 * 60, 0);
+
 //////////////////////////////////////////////////////////////////////////////////////////////////
 //////////////////////////////////////////////////////////////////////////////////////////////////
 // Core Structs
 //////////////////////////////////////////////////////////////////////////////////////////////////
 
 /// The IssueAPI struct provides a low-level wrapper around the issues API.
 /// This struct provides basics means of session management,
@@ -271,14 +275,16 @@
         read_only_api.login(username, password)?;
         Ok(read_only_api)
     }
 
     pub(crate) fn new_read_only(url: String, allow_self_signed: bool) -> APIResult<Self> {
         let client = reqwest::blocking::ClientBuilder::new()
             .danger_accept_invalid_certs(allow_self_signed)
+            .timeout(READ_WRITE_TIMEOUT)
+            .connect_timeout(CONNECT_TIMEOUT)
             .build()?;
         Ok(
             IssueAPI{
                 url,
                 token: None,
                 client,
                 allow_unsafe_ssl: allow_self_signed
@@ -453,14 +459,16 @@
         where
             I: serde::Serialize,
             S: std::io::Write
     {
         let url = self.get_endpoint(suffix);
         let client = reqwest::ClientBuilder::new()
             .danger_accept_invalid_certs(self.allow_unsafe_ssl)
+            .timeout(READ_WRITE_TIMEOUT)
+            .connect_timeout(CONNECT_TIMEOUT)
             .build()?;
         let rt = tokio::runtime::Builder::new_current_thread().enable_all().build()?;
         let result: APIResult<()> = rt.block_on(async {
             let mut stream = client
                 .get(url)
                 .json(&payload)
                 .send()
```

### Comparing `issue_db_api-0.9.2/issue_db_api/src/comments.rs` & `issue_db_api-0.9.3/issue_db_api/src/comments.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.9.2/issue_db_api/src/config.rs` & `issue_db_api-0.9.3/issue_db_api/src/config.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.9.2/issue_db_api/src/embedding.rs` & `issue_db_api-0.9.3/issue_db_api/src/embedding.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.9.2/issue_db_api/src/errors.rs` & `issue_db_api-0.9.3/issue_db_api/src/errors.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.9.2/issue_db_api/src/files.rs` & `issue_db_api-0.9.3/issue_db_api/src/files.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.9.2/issue_db_api/src/issues.rs` & `issue_db_api-0.9.3/issue_db_api/src/issues.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.9.2/issue_db_api/src/labels.rs` & `issue_db_api-0.9.3/issue_db_api/src/labels.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.9.2/issue_db_api/src/lib.rs` & `issue_db_api-0.9.3/issue_db_api/src/lib.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.9.2/issue_db_api/src/models.rs` & `issue_db_api-0.9.3/issue_db_api/src/models.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.9.2/issue_db_api/src/query.rs` & `issue_db_api-0.9.3/issue_db_api/src/query.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.9.2/issue_db_api/src/repository.rs` & `issue_db_api-0.9.3/issue_db_api/src/repository.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.9.2/issue_db_api/src/schemas/raw_issue_response.rs` & `issue_db_api-0.9.3/issue_db_api/src/schemas/raw_issue_response.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.9.2/issue_db_api/src/tags.rs` & `issue_db_api-0.9.3/issue_db_api/src/tags.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.9.2/issue_db_api/src/util.rs` & `issue_db_api-0.9.3/issue_db_api/src/util.rs`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.9.2/issue_db_api.egg-info/PKG-INFO` & `issue_db_api-0.9.3/issue_db_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: issue-db-api
-Version: 0.9.2
+Version: 0.9.3
 Author: Jesse Maarleveld
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `issue_db_api-0.9.2/issue_db_api.egg-info/SOURCES.txt` & `issue_db_api-0.9.3/issue_db_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `issue_db_api-0.9.2/pyproject.toml` & `issue_db_api-0.9.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.setuptools.packages.find]
 where=["."]
 include = ["issue_db_api"]
 
 [project]
 name = "issue_db_api"
-version = "0.9.2"
+version = "0.9.3"
 authors = [
     {name = "Jesse Maarleveld"},
 ]
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Rust",
```

