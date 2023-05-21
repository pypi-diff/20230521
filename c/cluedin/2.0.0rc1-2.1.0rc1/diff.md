# Comparing `tmp/cluedin-2.0.0rc1.tar.gz` & `tmp/cluedin-2.1.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cluedin-2.0.0rc1.tar", max compression
+gzip compressed data, was "cluedin-2.1.0rc1.tar", max compression
```

## Comparing `cluedin-2.0.0rc1.tar` & `cluedin-2.1.0rc1.tar`

### file list

```diff
@@ -1,11 +1,13 @@
--rw-r--r--   0        0        0     1093 2023-05-01 19:58:59.989579 cluedin-2.0.0rc1/LICENSE
--rw-r--r--   0        0        0     5472 2023-05-14 18:26:29.967372 cluedin-2.0.0rc1/cluedin/README.md
--rw-r--r--   0        0        0      173 2023-05-14 10:49:18.017492 cluedin-2.0.0rc1/cluedin/__init__.py
--rw-r--r--   0        0        0     3036 2023-05-14 18:11:54.236396 cluedin-2.0.0rc1/cluedin/account.py
--rw-r--r--   0        0        0     5735 2023-05-14 18:11:54.245612 cluedin-2.0.0rc1/cluedin/context.py
--rw-r--r--   0        0        0      119 2023-05-14 18:12:04.244035 cluedin-2.0.0rc1/cluedin/env.py
--rw-r--r--   0        0        0     2061 2023-05-14 18:11:54.236405 cluedin-2.0.0rc1/cluedin/gql.py
--rw-r--r--   0        0        0      492 2023-05-14 11:15:24.953207 cluedin-2.0.0rc1/cluedin/jwt.py
--rw-r--r--   0        0        0     3853 2023-05-14 18:11:54.236485 cluedin-2.0.0rc1/cluedin/public.py
--rw-r--r--   0        0        0      574 2023-05-13 22:10:06.320474 cluedin-2.0.0rc1/pyproject.toml
--rw-r--r--   0        0        0     6188 1970-01-01 00:00:00.000000 cluedin-2.0.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     1093 2023-05-01 19:58:59.989579 cluedin-2.1.0rc1/LICENSE
+-rw-r--r--   0        0        0     6887 2023-05-21 13:07:36.800967 cluedin-2.1.0rc1/cluedin/README.md
+-rw-r--r--   0        0        0      214 2023-05-21 12:33:01.908448 cluedin-2.1.0rc1/cluedin/__init__.py
+-rw-r--r--   0        0        0     9727 2023-05-20 19:26:50.338507 cluedin-2.1.0rc1/cluedin/account.py
+-rw-r--r--   0        0        0     5735 2023-05-14 19:14:24.796902 cluedin-2.1.0rc1/cluedin/context.py
+-rw-r--r--   0        0        0     1450 2023-05-21 13:07:14.463017 cluedin-2.1.0rc1/cluedin/entity.py
+-rw-r--r--   0        0        0      119 2023-05-14 19:14:24.797006 cluedin-2.1.0rc1/cluedin/env.py
+-rw-r--r--   0        0        0     2061 2023-05-14 19:14:24.797108 cluedin-2.1.0rc1/cluedin/gql.py
+-rw-r--r--   0        0        0      492 2023-05-14 19:14:24.797191 cluedin-2.1.0rc1/cluedin/jwt.py
+-rw-r--r--   0        0        0     3853 2023-05-14 19:14:24.797279 cluedin-2.1.0rc1/cluedin/public.py
+-rw-r--r--   0        0        0      669 2023-05-20 19:54:13.830640 cluedin-2.1.0rc1/cluedin/vocab.py
+-rw-r--r--   0        0        0      573 2023-05-21 14:27:36.205692 cluedin-2.1.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     7588 1970-01-01 00:00:00.000000 cluedin-2.1.0rc1/PKG-INFO
```

### Comparing `cluedin-2.0.0rc1/LICENSE` & `cluedin-2.1.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `cluedin-2.0.0rc1/cluedin/README.md` & `cluedin-2.1.0rc1/cluedin/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,55 +1,56 @@
 # CluedIn
 
 [cluedin](https://pypi.org/project/cluedin/) is a Python client for [CluedIn](https://www.cluedin.com/) API.
 
 ## Installation
 
 From [PyPi](https://pypi.org/project/cluedin/):
+
 ```shell
 pip install cluedin
 ```
 
 ## Quick start
 
 ### CluedIn context configuration
 
 Create a JSON file with context configuration to your CluedIn instance:
 
 In this file, parameters have the following meaning:
 
-* `protocol` - `http` if your CluedIn instance is not secured with a TLS certicate. Otherwise, `https` by default.
-* `domain` – CluedIn instance domain without the Organization prefix.
-* `org_name` – the name of Organization (a.k.a. Organization prefix).
-* `user_email` – the user's email.
-* `user_password` – the user's password.
-* `verify_tls` – `false`, if an unknown CA signs the TLS certificate. Otherwise, `true` by default.
+- `protocol` - `http` if your CluedIn instance is not secured with a TLS certicate. Otherwise, `https` by default.
+- `domain` – CluedIn instance domain without the Organization prefix.
+- `org_name` – the name of Organization (a.k.a. Organization prefix).
+- `user_email` – the user's email.
+- `user_password` – the user's password.
+- `verify_tls` – `false`, if an unknown CA signs the TLS certificate. Otherwise, `true` by default.
 
 Here is an example of a file for a CluedIn instance running locally from a [Home](https://cluedin-io.github.io/Home/) repository:
 
 ```json
 {
-    "protocol": "http",
-    "domain": "127.0.0.1.nip.io",
-    "org_name": "foobar",
-    "user_email": "admin@foobar.com",
-    "user_password": "Foobar23!"
+  "protocol": "http",
+  "domain": "127.0.0.1.nip.io",
+  "org_name": "foobar",
+  "user_email": "admin@foobar.com",
+  "user_password": "Foobar23!"
 }
 ```
 
 We add the protocol, but we can skip this parameter if the URL starts with `https`. Likewise, we can skip `verify_tls` because it only makes sense for HTTPs URLs.
 
 Alternatively, to provide email and password, you can obtain an API access token from CluedIn UI and provide it in the file:
 
 ```json
 {
-    "protocol": "http",
-    "domain": "127.0.0.1.nip.io",
-    "org_name": "foobar",
-    "access_token": "..."
+  "protocol": "http",
+  "domain": "127.0.0.1.nip.io",
+  "org_name": "foobar",
+  "access_token": "..."
 }
 ```
 
 When the configuration file exists, you can export its path to an environment variable:
 
 ```shell
 export CLUEDIN_CONTEXT=~/.cluedin/home.json
@@ -113,33 +114,47 @@
 
 ## API
 
 ### Environment
 
 - `CLUEDIN_REQUEST_TIMEOUT_IN_SECONDS` - CluedIn API request timeout (in seconds). If not set, then it defaults to `300` (5 minutes).
 
-### `Context`
+### Context
 
 - `Context.from_dict(cls, context_dict: dict) -> Context` – creates a new `Context` object from a `dict`.
 - `Context.from_json_file(file_path: str) -> Context` – creates a new `Context` object from a JSON-file.
 
 ### Account
 
 - `cluedin.account.get_users(context: Context, org_id: str = None) -> list` – returns all users for Organization.
 - `cluedin.account.is_organization_available_response(context: Context, org_name: str) -> dict` – checks if a given Organization name is available. This method returns a JSON-response serialized into a `dict`.
 - `cluedin.account.is_organization_available(context: Context, org_name: str) -> bool` – checks if a given Organization name is available. Returns a Boolean.
 - `cluedin.account.is_user_available_response(context: Context, user_email: str, org_name: str) -> dict` – checks, if a user with a given email can be created or this email is already reserved. This method returns a JSON-response serialized into a `dict`.
 - `cluedin.account.is_user_available(context: Context, user_email: str, org_name: str) -> bool` – checks, if a user with a given email can be created or this email is already reserved. This method returns a JSON-response serialized into a `dict`. Returns a Boolean.
+- `cluedin.account.get_invitation_code(context: Context, email: str) -> str` – returns an invitation code for a given email.
+- `cluedin.account.create_organization(context: Context, user_email: str, password: str, org_name: str, org_sub_domain: str = None, email_domain: str = None, allow_email_domain_signup: bool = True, new_account_access_key: str = None) -> dict` - creates a new Organization. This method returns a JSON-response serialized into a `dict`.
+- `cluedin.account.create_user(context: Context, user_email: str, user_password: str) -> requests.models.Response` – creates a new user. This method returns `requests.models.Response`.
+- `cluedin.account.create_admin_user(context: Context, user_email: str, user_password: str) -> requests.models.Response` – creates a new admin user. This method returns `requests.models.Response`.
+- `cluedin.account.get_user(context: Context, user_id: str = None) -> dict` – returns a user by ID. If `user_id` is nor provided, the current user is returned. This method returns a JSON-response serialized into a `dict`.
+
+### Entity
+
+- `cluedin.entity.get_entity_blob(context: Context, entity_id: str) -> str` – returns an entity blob by ID.
+- `cluedin.entity.get_entity_as_clue(context: Context, entity_id: str) -> str` – returns an entity as a clue by ID.
 
 ### GraphQL
 
 - `cluedin.gql.gql(context: Context, query: str, variables: dict = None) -> dict` – sends a GraphQL request and returns a response.
 - `cluedin.gql.entries(context: Context, query: str, variables: dict = None) -> list` – returns entries from a GraphQL search query. If cursor is requested in the GraphQL query (see the example above and tests), then it proceeds to next pages to return all results.
 
 ### JWT
 
 - `cluedin.jwt.get_jwt_payload(jwt: str) -> dict` – parses a JWT (JSON Web Token, a.k.a. access token or API token), and returns its payload serialized into a `dict`.
 
 ### Public API
 
 - `cluedin.public.post_clue(context: Context, clue: str, content_type: str = 'application/xml') -> str` – posts a clue in XML or JSON format. This method returns an operation result as a string.
 - `cluedin.public.restore_user_entities(context: Context) -> list` – if you accidentally deleted `/Infrastructure/User` entities, this method gets all users and restores entities for those who miss them.
+
+### Vocabulary
+
+- `cluedin.vocab.get_vocab_keys(context: Context) -> list` – gets all vocabulary keys.
```

### Comparing `cluedin-2.0.0rc1/cluedin/context.py` & `cluedin-2.1.0rc1/cluedin/context.py`

 * *Files identical despite different names*

### Comparing `cluedin-2.0.0rc1/cluedin/gql.py` & `cluedin-2.1.0rc1/cluedin/gql.py`

 * *Files identical despite different names*

### Comparing `cluedin-2.0.0rc1/cluedin/public.py` & `cluedin-2.1.0rc1/cluedin/public.py`

 * *Files identical despite different names*

### Comparing `cluedin-2.0.0rc1/pyproject.toml` & `cluedin-2.1.0rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cluedin"
-version = "2.0.0.rc1"
+version = "2.1.0rc1"
 description = "A Python client for CluedIn API."
 authors = ["Roman Klimenko <romaklimenko@gmail.com>"]
 readme = "cluedin/README.md"
 license = "MIT"
 keywords = ["cluedin", "mdm", "master data management"]
 maintainers = ["Roman Klimenko <romaklimenko@gmail.com>"]
 homepage = "https://github.com/romaklimenko/cluedin"
```

### Comparing `cluedin-2.0.0rc1/PKG-INFO` & `cluedin-2.1.0rc1/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cluedin
-Version: 2.0.0rc1
+Version: 2.1.0rc1
 Summary: A Python client for CluedIn API.
 Home-page: https://github.com/romaklimenko/cluedin
 License: MIT
 Keywords: cluedin,mdm,master data management
 Author: Roman Klimenko
 Author-email: romaklimenko@gmail.com
 Maintainer: Roman Klimenko
@@ -24,55 +24,56 @@
 # CluedIn
 
 [cluedin](https://pypi.org/project/cluedin/) is a Python client for [CluedIn](https://www.cluedin.com/) API.
 
 ## Installation
 
 From [PyPi](https://pypi.org/project/cluedin/):
+
 ```shell
 pip install cluedin
 ```
 
 ## Quick start
 
 ### CluedIn context configuration
 
 Create a JSON file with context configuration to your CluedIn instance:
 
 In this file, parameters have the following meaning:
 
-* `protocol` - `http` if your CluedIn instance is not secured with a TLS certicate. Otherwise, `https` by default.
-* `domain` – CluedIn instance domain without the Organization prefix.
-* `org_name` – the name of Organization (a.k.a. Organization prefix).
-* `user_email` – the user's email.
-* `user_password` – the user's password.
-* `verify_tls` – `false`, if an unknown CA signs the TLS certificate. Otherwise, `true` by default.
+- `protocol` - `http` if your CluedIn instance is not secured with a TLS certicate. Otherwise, `https` by default.
+- `domain` – CluedIn instance domain without the Organization prefix.
+- `org_name` – the name of Organization (a.k.a. Organization prefix).
+- `user_email` – the user's email.
+- `user_password` – the user's password.
+- `verify_tls` – `false`, if an unknown CA signs the TLS certificate. Otherwise, `true` by default.
 
 Here is an example of a file for a CluedIn instance running locally from a [Home](https://cluedin-io.github.io/Home/) repository:
 
 ```json
 {
-    "protocol": "http",
-    "domain": "127.0.0.1.nip.io",
-    "org_name": "foobar",
-    "user_email": "admin@foobar.com",
-    "user_password": "Foobar23!"
+  "protocol": "http",
+  "domain": "127.0.0.1.nip.io",
+  "org_name": "foobar",
+  "user_email": "admin@foobar.com",
+  "user_password": "Foobar23!"
 }
 ```
 
 We add the protocol, but we can skip this parameter if the URL starts with `https`. Likewise, we can skip `verify_tls` because it only makes sense for HTTPs URLs.
 
 Alternatively, to provide email and password, you can obtain an API access token from CluedIn UI and provide it in the file:
 
 ```json
 {
-    "protocol": "http",
-    "domain": "127.0.0.1.nip.io",
-    "org_name": "foobar",
-    "access_token": "..."
+  "protocol": "http",
+  "domain": "127.0.0.1.nip.io",
+  "org_name": "foobar",
+  "access_token": "..."
 }
 ```
 
 When the configuration file exists, you can export its path to an environment variable:
 
 ```shell
 export CLUEDIN_CONTEXT=~/.cluedin/home.json
@@ -136,26 +137,36 @@
 
 ## API
 
 ### Environment
 
 - `CLUEDIN_REQUEST_TIMEOUT_IN_SECONDS` - CluedIn API request timeout (in seconds). If not set, then it defaults to `300` (5 minutes).
 
-### `Context`
+### Context
 
 - `Context.from_dict(cls, context_dict: dict) -> Context` – creates a new `Context` object from a `dict`.
 - `Context.from_json_file(file_path: str) -> Context` – creates a new `Context` object from a JSON-file.
 
 ### Account
 
 - `cluedin.account.get_users(context: Context, org_id: str = None) -> list` – returns all users for Organization.
 - `cluedin.account.is_organization_available_response(context: Context, org_name: str) -> dict` – checks if a given Organization name is available. This method returns a JSON-response serialized into a `dict`.
 - `cluedin.account.is_organization_available(context: Context, org_name: str) -> bool` – checks if a given Organization name is available. Returns a Boolean.
 - `cluedin.account.is_user_available_response(context: Context, user_email: str, org_name: str) -> dict` – checks, if a user with a given email can be created or this email is already reserved. This method returns a JSON-response serialized into a `dict`.
 - `cluedin.account.is_user_available(context: Context, user_email: str, org_name: str) -> bool` – checks, if a user with a given email can be created or this email is already reserved. This method returns a JSON-response serialized into a `dict`. Returns a Boolean.
+- `cluedin.account.get_invitation_code(context: Context, email: str) -> str` – returns an invitation code for a given email.
+- `cluedin.account.create_organization(context: Context, user_email: str, password: str, org_name: str, org_sub_domain: str = None, email_domain: str = None, allow_email_domain_signup: bool = True, new_account_access_key: str = None) -> dict` - creates a new Organization. This method returns a JSON-response serialized into a `dict`.
+- `cluedin.account.create_user(context: Context, user_email: str, user_password: str) -> requests.models.Response` – creates a new user. This method returns `requests.models.Response`.
+- `cluedin.account.create_admin_user(context: Context, user_email: str, user_password: str) -> requests.models.Response` – creates a new admin user. This method returns `requests.models.Response`.
+- `cluedin.account.get_user(context: Context, user_id: str = None) -> dict` – returns a user by ID. If `user_id` is nor provided, the current user is returned. This method returns a JSON-response serialized into a `dict`.
+
+### Entity
+
+- `cluedin.entity.get_entity_blob(context: Context, entity_id: str) -> str` – returns an entity blob by ID.
+- `cluedin.entity.get_entity_as_clue(context: Context, entity_id: str) -> str` – returns an entity as a clue by ID.
 
 ### GraphQL
 
 - `cluedin.gql.gql(context: Context, query: str, variables: dict = None) -> dict` – sends a GraphQL request and returns a response.
 - `cluedin.gql.entries(context: Context, query: str, variables: dict = None) -> list` – returns entries from a GraphQL search query. If cursor is requested in the GraphQL query (see the example above and tests), then it proceeds to next pages to return all results.
 
 ### JWT
@@ -163,7 +174,11 @@
 - `cluedin.jwt.get_jwt_payload(jwt: str) -> dict` – parses a JWT (JSON Web Token, a.k.a. access token or API token), and returns its payload serialized into a `dict`.
 
 ### Public API
 
 - `cluedin.public.post_clue(context: Context, clue: str, content_type: str = 'application/xml') -> str` – posts a clue in XML or JSON format. This method returns an operation result as a string.
 - `cluedin.public.restore_user_entities(context: Context) -> list` – if you accidentally deleted `/Infrastructure/User` entities, this method gets all users and restores entities for those who miss them.
 
+### Vocabulary
+
+- `cluedin.vocab.get_vocab_keys(context: Context) -> list` – gets all vocabulary keys.
+
```

