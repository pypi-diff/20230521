# Comparing `tmp/carica-1.3.3.tar.gz` & `tmp/carica-1.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "carica-1.3.3.tar", last modified: Wed Jul 20 23:07:09 2022, max compression
+gzip compressed data, was "carica-1.3.4.tar", last modified: Sun May 21 21:55:47 2023, max compression
```

## Comparing `carica-1.3.3.tar` & `carica-1.3.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 23:07:09.699832 carica-1.3.3/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-07-20 23:06:48.000000 carica-1.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    16009 2022-07-20 23:07:09.699832 carica-1.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    15330 2022-07-20 23:06:48.000000 carica-1.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      190 2022-07-20 23:06:48.000000 carica-1.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)      878 2022-07-20 23:07:09.703832 carica-1.3.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 23:07:09.699832 carica-1.3.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 23:07:09.699832 carica-1.3.3/src/carica/
--rw-r--r--   0 runner    (1001) docker     (121)      228 2022-07-20 23:06:48.000000 carica-1.3.3/src/carica/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    27959 2022-07-20 23:06:48.000000 carica-1.3.3/src/carica/carica.py
--rw-r--r--   0 runner    (1001) docker     (121)     3335 2022-07-20 23:06:48.000000 carica-1.3.3/src/carica/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 23:07:09.699832 carica-1.3.3/src/carica/interface/
--rw-r--r--   0 runner    (1001) docker     (121)     3772 2022-07-20 23:06:48.000000 carica-1.3.3/src/carica/interface/Serializable.py
--rw-r--r--   0 runner    (1001) docker     (121)      269 2022-07-20 23:06:48.000000 carica-1.3.3/src/carica/interface/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 23:07:09.699832 carica-1.3.3/src/carica/models/
--rw-r--r--   0 runner    (1001) docker     (121)      127 2022-07-20 23:06:48.000000 carica-1.3.3/src/carica/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    20278 2022-07-20 23:06:48.000000 carica-1.3.3/src/carica/models/dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (121)     2974 2022-07-20 23:06:48.000000 carica-1.3.3/src/carica/models/path.py
--rw-r--r--   0 runner    (1001) docker     (121)     1932 2022-07-20 23:06:48.000000 carica-1.3.3/src/carica/models/timedelta.py
--rw-r--r--   0 runner    (1001) docker     (121)     8021 2022-07-20 23:06:48.000000 carica-1.3.3/src/carica/typeChecking.py
--rw-r--r--   0 runner    (1001) docker     (121)      879 2022-07-20 23:06:48.000000 carica-1.3.3/src/carica/util.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-07-20 23:07:09.699832 carica-1.3.3/src/carica.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    16009 2022-07-20 23:07:09.000000 carica-1.3.3/src/carica.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      516 2022-07-20 23:07:09.000000 carica-1.3.3/src/carica.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-07-20 23:07:09.000000 carica-1.3.3/src/carica.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       23 2022-07-20 23:07:09.000000 carica-1.3.3/src/carica.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        7 2022-07-20 23:07:09.000000 carica-1.3.3/src/carica.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:55:47.100978 carica-1.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-21 21:55:29.000000 carica-1.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15974 2023-05-21 21:55:47.100978 carica-1.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    15295 2023-05-21 21:55:29.000000 carica-1.3.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-21 21:55:29.000000 carica-1.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-21 21:55:47.104978 carica-1.3.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:55:47.100978 carica-1.3.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:55:47.100978 carica-1.3.4/src/carica/
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-21 21:55:29.000000 carica-1.3.4/src/carica/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27967 2023-05-21 21:55:29.000000 carica-1.3.4/src/carica/carica.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3335 2023-05-21 21:55:29.000000 carica-1.3.4/src/carica/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:55:47.100978 carica-1.3.4/src/carica/interface/
+-rw-r--r--   0 runner    (1001) docker     (123)     3680 2023-05-21 21:55:29.000000 carica-1.3.4/src/carica/interface/Serializable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-21 21:55:29.000000 carica-1.3.4/src/carica/interface/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:55:47.100978 carica-1.3.4/src/carica/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-21 21:55:29.000000 carica-1.3.4/src/carica/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20387 2023-05-21 21:55:29.000000 carica-1.3.4/src/carica/models/dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-05-21 21:55:29.000000 carica-1.3.4/src/carica/models/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1932 2023-05-21 21:55:29.000000 carica-1.3.4/src/carica/models/timedelta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8001 2023-05-21 21:55:29.000000 carica-1.3.4/src/carica/typeChecking.py
+-rw-r--r--   0 runner    (1001) docker     (123)      939 2023-05-21 21:55:29.000000 carica-1.3.4/src/carica/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 21:55:47.100978 carica-1.3.4/src/carica.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    15974 2023-05-21 21:55:47.000000 carica-1.3.4/src/carica.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-05-21 21:55:47.000000 carica-1.3.4/src/carica.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 21:55:47.000000 carica-1.3.4/src/carica.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-21 21:55:47.000000 carica-1.3.4/src/carica.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-21 21:55:47.000000 carica-1.3.4/src/carica.egg-info/top_level.txt
```

### Comparing `carica-1.3.3/LICENSE` & `carica-1.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `carica-1.3.3/PKG-INFO` & `carica-1.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carica
-Version: 1.3.3
+Version: 1.3.4
 Summary: Python module that populates variables from TOML config documents, and generates config documents from python variables.
 Home-page: https://github.com/Trimatix/carica
 Author: Jasper Law
 Author-email: trimatix.music@gmail.com
 Project-URL: Bug Tracker, https://github.com/Trimatix/carica/issues
 Keywords: config,cfg,python,toml,generate,auto-generate,orm
 Classifier: Programming Language :: Python :: 3.8
@@ -22,15 +22,15 @@
     alt="Carica Logo"
   />
 </p>
 <h1 align="center">Carica - A Python Configurator</h1>
 <p align="center">
   <a href="https://github.com/Trimatix/Carica/actions"
     ><img
-      src="https://img.shields.io/github/workflow/status/GOF2BountyBot/GOF2BountyBot/BASED"
+      src="https://img.shields.io/github/actions/workflow/status/Trimatix/Carica/testing.yml?branch=main"
       alt="GitHub Actions workflow status"
   /></a>
   <a href="https://github.com/Trimatix/Carica/projects/1?card_filter_query=label%3Abug"
     ><img
       src="https://img.shields.io/github/issues-search?color=eb4034&label=bug%20reports&query=repo%3ATrimatix%2FCarica%20is%3Aopen%20label%3Abug"
       alt="GitHub open bug reports"
   /></a>
@@ -330,17 +330,15 @@
 
 Projects which prefer strong typing may implement the `carica.ISerializable` interface to enforce this pattern with inheritence. Carica will validate serialized objects against the `carica.PrimativeType` type alias, which is also exposed for use.
 
 ### Example
 
 *cfg.py*
 ```py
-from carica import ISerializable
-
-class MySerializableType(ISerializable):
+class MySerializableType:
     def __init__(self, myField):
         self.myField = myField
 
     def serialize(self, **kwargs):
         return {"myField": self.myField}
 
     @classmethod
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: carica Version: 1.3.3 Summary: Python module that
+Metadata-Version: 2.1 Name: carica Version: 1.3.4 Summary: Python module that
 populates variables from TOML config documents, and generates config documents
 from python variables. Home-page: https://github.com/Trimatix/carica Author:
 Jasper Law Author-email: trimatix.music@gmail.com Project-URL: Bug Tracker,
 https://github.com/Trimatix/carica/issues Keywords:
 config,cfg,python,toml,generate,auto-generate,orm Classifier: Programming
 Language :: Python :: 3.8 Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Operating System :: OS Independent Requires-
@@ -124,77 +124,77 @@
 `deserialize` must be a class method, and should transform a serialized object
 representation into a new object. Carica enforces this pattern on non-primative
 types using the `SerializableType` type protocol, which allows for duck-typed
 serializable types. This protocol is exposed for use with `isinstance`.
 Projects which prefer strong typing may implement the `carica.ISerializable`
 interface to enforce this pattern with inheritence. Carica will validate
 serialized objects against the `carica.PrimativeType` type alias, which is also
-exposed for use. ### Example *cfg.py* ```py from carica import ISerializable
-class MySerializableType(ISerializable): def __init__(self, myField):
-self.myField = myField def serialize(self, **kwargs): return {"myField":
-self.myField} @classmethod def deserialize(self, data, **kwargs): return
-MySerializableClass(data["myField"]) mySerializableVar = MySerializableClass
-("hello") ``` #### Default config generation ```py >>> import cfg >>> import
-carica >>> carica.makeDefaultCfg(cfg) Created defaultCfg.toml ``` The above
-code will produce the following file: *defaultCfg.toml* ```toml
-[mySerializableVar] myField = "hello" ``` #### Config file loading
-*myConfig.toml* ```toml [mySerializableVar] myField = "some changed value" ```
-```py >>> import cfg >>> import carica >>> carica.loadCfg(cfg, "myConfig.toml")
-Config successfully loaded: myConfig.toml >>> cfg.mySerializableVar.myField
-some changed value ``` ### Premade models Carica provides serializable models
-that are ready to use (or extend) in your code. These models can be found in
-the `carica.models` package, which is imported by default. ####
-SerializableDataClass Removes the need to write boilerplate serializing
-functionality for dataclasses. This class is intended to be extended, adding
-definitions for your dataclass's fields. Extensions of `SerializableDataClass`
-**must** themselves be decorated with `@dataclasses.dataclass` in order to
-function correctly. #### SerializablePath An OS-agnostic filesystem path,
-extending `pathlib.Path`. The serializing/deserializing behaviour added by this
-class is minimal, a serialized `SerializablePath` is simply the string
-representation of the path, for readability. All other behaviour of
-`pathlib.Path` applies, for example. `SerializablePath` can be instantiated
-from a single path: `SerializablePath("my/directory/path")`, or from path
-segments: `SerializablePath("my", "file", "path.toml")`. ####
-SerializableTimedelta `datetime.datetime` is already considered a primitive
-type by TomlKit, and so no serializability needs to be added for you to use
-this class in your configs. However, `datetime.timedelta` is not serializable
-by default. `SerializableTimedelta` solves this issue as a serializable
-subclass. As a subclass, all `timedelta` behaiour applies, including the usual
-constructor. In addition, `SerializableTimedelta.fromTimedelta` is a
-convenience class method that accepts a `datetime.timedelta` and constructs a
-new `SerializableTimedelta` from it. #### Premade models example The
-recommended usage pattern for `SerializableDataClass` is to separate your
-models into a separate module/package, allowing for 'schema' definition as
-python code. This pattern is not necessary, model definition *can* be done in
-your config file. *configSchema.py* ```py from carica.models import
-SerializableDataClass from dataclasses import dataclass @dataclass class
-UserDataField(SerializableDataClass): name: str validation_regex: str ```
-*config.py* ```py from carica.models import SerializablePath,
-SerializableTimedelta from configSchema import UserDataField from datetime
-import datetime new_user_required_fields = [ UserDataField( name = "user-name"
-validation_regex = "[a-z]+" ), UserDataField( name = "password"
-validation_regex = "\\b(?!password\\b)\\w+" ) ] database_path =
-SerializablePath("default/path.csv") birthday = datetime(day=1, month=1,
-year=1500) connection_timeout = SerializableTimedelta(minutes=5) ``` ## Planned
-features - Preceeding comments: This functionality is 'complete' in that it
-functions as intended and passes all unit tests, however an issue needs to be
-worked aruond before the feature can be enabled: In order to disambiguate
-between variables and table fields, the TOML spec requires that arrays and
-tables be placed at the end of a document. Carica currently depends upon
-documents being rendered with variables appearing in the same order as they
-appear in the python config module, which is not guaranteed. This leads to
-trailing and otherwise misplaced preceeding comments. - Config mutation: Carica
-should allow for loading an existing config, changing some values, and then
-updating the TOML document with new values. This should retain all formatting
-from the original document, including variable ordering and any comments that
-are not present in the python module. ## Limitations - No support for schema
-migration - No support for asynchronous object serializing/deserializing -
-Imperfect estimation of variables defined in python modules: Listing the
-variables defined within a scope is not a known feature of python, and so
-Carica estimates this information by iterating over the tokens in your module.
-Carica does not build an AST of your python module. This means that certain
-name definition structures will result in false positives/negatives. This
-behaviour has not been extensively tested, but once such false positive has
-been identified: When invoking a callable (such as a class or function) with a
-keyword argument on a new, unindented line, the argument name will be falsely
-identified as a variable name. E.g: ```py my_variable = dict(key1=value1,
-key2=value2) ``` produces `my_variable` and `key2` as variable names.
+exposed for use. ### Example *cfg.py* ```py class MySerializableType: def
+__init__(self, myField): self.myField = myField def serialize(self, **kwargs):
+return {"myField": self.myField} @classmethod def deserialize(self, data,
+**kwargs): return MySerializableClass(data["myField"]) mySerializableVar =
+MySerializableClass("hello") ``` #### Default config generation ```py >>>
+import cfg >>> import carica >>> carica.makeDefaultCfg(cfg) Created
+defaultCfg.toml ``` The above code will produce the following file:
+*defaultCfg.toml* ```toml [mySerializableVar] myField = "hello" ``` #### Config
+file loading *myConfig.toml* ```toml [mySerializableVar] myField = "some
+changed value" ``` ```py >>> import cfg >>> import carica >>> carica.loadCfg
+(cfg, "myConfig.toml") Config successfully loaded: myConfig.toml >>>
+cfg.mySerializableVar.myField some changed value ``` ### Premade models Carica
+provides serializable models that are ready to use (or extend) in your code.
+These models can be found in the `carica.models` package, which is imported by
+default. #### SerializableDataClass Removes the need to write boilerplate
+serializing functionality for dataclasses. This class is intended to be
+extended, adding definitions for your dataclass's fields. Extensions of
+`SerializableDataClass` **must** themselves be decorated with
+`@dataclasses.dataclass` in order to function correctly. #### SerializablePath
+An OS-agnostic filesystem path, extending `pathlib.Path`. The serializing/
+deserializing behaviour added by this class is minimal, a serialized
+`SerializablePath` is simply the string representation of the path, for
+readability. All other behaviour of `pathlib.Path` applies, for example.
+`SerializablePath` can be instantiated from a single path: `SerializablePath
+("my/directory/path")`, or from path segments: `SerializablePath("my", "file",
+"path.toml")`. #### SerializableTimedelta `datetime.datetime` is already
+considered a primitive type by TomlKit, and so no serializability needs to be
+added for you to use this class in your configs. However, `datetime.timedelta`
+is not serializable by default. `SerializableTimedelta` solves this issue as a
+serializable subclass. As a subclass, all `timedelta` behaiour applies,
+including the usual constructor. In addition,
+`SerializableTimedelta.fromTimedelta` is a convenience class method that
+accepts a `datetime.timedelta` and constructs a new `SerializableTimedelta`
+from it. #### Premade models example The recommended usage pattern for
+`SerializableDataClass` is to separate your models into a separate module/
+package, allowing for 'schema' definition as python code. This pattern is not
+necessary, model definition *can* be done in your config file.
+*configSchema.py* ```py from carica.models import SerializableDataClass from
+dataclasses import dataclass @dataclass class UserDataField
+(SerializableDataClass): name: str validation_regex: str ``` *config.py* ```py
+from carica.models import SerializablePath, SerializableTimedelta from
+configSchema import UserDataField from datetime import datetime
+new_user_required_fields = [ UserDataField( name = "user-name" validation_regex
+= "[a-z]+" ), UserDataField( name = "password" validation_regex = "\\b
+(?!password\\b)\\w+" ) ] database_path = SerializablePath("default/path.csv")
+birthday = datetime(day=1, month=1, year=1500) connection_timeout =
+SerializableTimedelta(minutes=5) ``` ## Planned features - Preceeding comments:
+This functionality is 'complete' in that it functions as intended and passes
+all unit tests, however an issue needs to be worked aruond before the feature
+can be enabled: In order to disambiguate between variables and table fields,
+the TOML spec requires that arrays and tables be placed at the end of a
+document. Carica currently depends upon documents being rendered with variables
+appearing in the same order as they appear in the python config module, which
+is not guaranteed. This leads to trailing and otherwise misplaced preceeding
+comments. - Config mutation: Carica should allow for loading an existing
+config, changing some values, and then updating the TOML document with new
+values. This should retain all formatting from the original document, including
+variable ordering and any comments that are not present in the python module.
+## Limitations - No support for schema migration - No support for asynchronous
+object serializing/deserializing - Imperfect estimation of variables defined in
+python modules: Listing the variables defined within a scope is not a known
+feature of python, and so Carica estimates this information by iterating over
+the tokens in your module. Carica does not build an AST of your python module.
+This means that certain name definition structures will result in false
+positives/negatives. This behaviour has not been extensively tested, but once
+such false positive has been identified: When invoking a callable (such as a
+class or function) with a keyword argument on a new, unindented line, the
+argument name will be falsely identified as a variable name. E.g: ```py
+my_variable = dict(key1=value1, key2=value2) ``` produces `my_variable` and
+`key2` as variable names.
```

### Comparing `carica-1.3.3/README.md` & `carica-1.3.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     alt="Carica Logo"
   />
 </p>
 <h1 align="center">Carica - A Python Configurator</h1>
 <p align="center">
   <a href="https://github.com/Trimatix/Carica/actions"
     ><img
-      src="https://img.shields.io/github/workflow/status/GOF2BountyBot/GOF2BountyBot/BASED"
+      src="https://img.shields.io/github/actions/workflow/status/Trimatix/Carica/testing.yml?branch=main"
       alt="GitHub Actions workflow status"
   /></a>
   <a href="https://github.com/Trimatix/Carica/projects/1?card_filter_query=label%3Abug"
     ><img
       src="https://img.shields.io/github/issues-search?color=eb4034&label=bug%20reports&query=repo%3ATrimatix%2FCarica%20is%3Aopen%20label%3Abug"
       alt="GitHub open bug reports"
   /></a>
@@ -313,17 +313,15 @@
 
 Projects which prefer strong typing may implement the `carica.ISerializable` interface to enforce this pattern with inheritence. Carica will validate serialized objects against the `carica.PrimativeType` type alias, which is also exposed for use.
 
 ### Example
 
 *cfg.py*
 ```py
-from carica import ISerializable
-
-class MySerializableType(ISerializable):
+class MySerializableType:
     def __init__(self, myField):
         self.myField = myField
 
     def serialize(self, **kwargs):
         return {"myField": self.myField}
 
     @classmethod
```

#### html2text {}

```diff
@@ -114,77 +114,77 @@
 `deserialize` must be a class method, and should transform a serialized object
 representation into a new object. Carica enforces this pattern on non-primative
 types using the `SerializableType` type protocol, which allows for duck-typed
 serializable types. This protocol is exposed for use with `isinstance`.
 Projects which prefer strong typing may implement the `carica.ISerializable`
 interface to enforce this pattern with inheritence. Carica will validate
 serialized objects against the `carica.PrimativeType` type alias, which is also
-exposed for use. ### Example *cfg.py* ```py from carica import ISerializable
-class MySerializableType(ISerializable): def __init__(self, myField):
-self.myField = myField def serialize(self, **kwargs): return {"myField":
-self.myField} @classmethod def deserialize(self, data, **kwargs): return
-MySerializableClass(data["myField"]) mySerializableVar = MySerializableClass
-("hello") ``` #### Default config generation ```py >>> import cfg >>> import
-carica >>> carica.makeDefaultCfg(cfg) Created defaultCfg.toml ``` The above
-code will produce the following file: *defaultCfg.toml* ```toml
-[mySerializableVar] myField = "hello" ``` #### Config file loading
-*myConfig.toml* ```toml [mySerializableVar] myField = "some changed value" ```
-```py >>> import cfg >>> import carica >>> carica.loadCfg(cfg, "myConfig.toml")
-Config successfully loaded: myConfig.toml >>> cfg.mySerializableVar.myField
-some changed value ``` ### Premade models Carica provides serializable models
-that are ready to use (or extend) in your code. These models can be found in
-the `carica.models` package, which is imported by default. ####
-SerializableDataClass Removes the need to write boilerplate serializing
-functionality for dataclasses. This class is intended to be extended, adding
-definitions for your dataclass's fields. Extensions of `SerializableDataClass`
-**must** themselves be decorated with `@dataclasses.dataclass` in order to
-function correctly. #### SerializablePath An OS-agnostic filesystem path,
-extending `pathlib.Path`. The serializing/deserializing behaviour added by this
-class is minimal, a serialized `SerializablePath` is simply the string
-representation of the path, for readability. All other behaviour of
-`pathlib.Path` applies, for example. `SerializablePath` can be instantiated
-from a single path: `SerializablePath("my/directory/path")`, or from path
-segments: `SerializablePath("my", "file", "path.toml")`. ####
-SerializableTimedelta `datetime.datetime` is already considered a primitive
-type by TomlKit, and so no serializability needs to be added for you to use
-this class in your configs. However, `datetime.timedelta` is not serializable
-by default. `SerializableTimedelta` solves this issue as a serializable
-subclass. As a subclass, all `timedelta` behaiour applies, including the usual
-constructor. In addition, `SerializableTimedelta.fromTimedelta` is a
-convenience class method that accepts a `datetime.timedelta` and constructs a
-new `SerializableTimedelta` from it. #### Premade models example The
-recommended usage pattern for `SerializableDataClass` is to separate your
-models into a separate module/package, allowing for 'schema' definition as
-python code. This pattern is not necessary, model definition *can* be done in
-your config file. *configSchema.py* ```py from carica.models import
-SerializableDataClass from dataclasses import dataclass @dataclass class
-UserDataField(SerializableDataClass): name: str validation_regex: str ```
-*config.py* ```py from carica.models import SerializablePath,
-SerializableTimedelta from configSchema import UserDataField from datetime
-import datetime new_user_required_fields = [ UserDataField( name = "user-name"
-validation_regex = "[a-z]+" ), UserDataField( name = "password"
-validation_regex = "\\b(?!password\\b)\\w+" ) ] database_path =
-SerializablePath("default/path.csv") birthday = datetime(day=1, month=1,
-year=1500) connection_timeout = SerializableTimedelta(minutes=5) ``` ## Planned
-features - Preceeding comments: This functionality is 'complete' in that it
-functions as intended and passes all unit tests, however an issue needs to be
-worked aruond before the feature can be enabled: In order to disambiguate
-between variables and table fields, the TOML spec requires that arrays and
-tables be placed at the end of a document. Carica currently depends upon
-documents being rendered with variables appearing in the same order as they
-appear in the python config module, which is not guaranteed. This leads to
-trailing and otherwise misplaced preceeding comments. - Config mutation: Carica
-should allow for loading an existing config, changing some values, and then
-updating the TOML document with new values. This should retain all formatting
-from the original document, including variable ordering and any comments that
-are not present in the python module. ## Limitations - No support for schema
-migration - No support for asynchronous object serializing/deserializing -
-Imperfect estimation of variables defined in python modules: Listing the
-variables defined within a scope is not a known feature of python, and so
-Carica estimates this information by iterating over the tokens in your module.
-Carica does not build an AST of your python module. This means that certain
-name definition structures will result in false positives/negatives. This
-behaviour has not been extensively tested, but once such false positive has
-been identified: When invoking a callable (such as a class or function) with a
-keyword argument on a new, unindented line, the argument name will be falsely
-identified as a variable name. E.g: ```py my_variable = dict(key1=value1,
-key2=value2) ``` produces `my_variable` and `key2` as variable names.
+exposed for use. ### Example *cfg.py* ```py class MySerializableType: def
+__init__(self, myField): self.myField = myField def serialize(self, **kwargs):
+return {"myField": self.myField} @classmethod def deserialize(self, data,
+**kwargs): return MySerializableClass(data["myField"]) mySerializableVar =
+MySerializableClass("hello") ``` #### Default config generation ```py >>>
+import cfg >>> import carica >>> carica.makeDefaultCfg(cfg) Created
+defaultCfg.toml ``` The above code will produce the following file:
+*defaultCfg.toml* ```toml [mySerializableVar] myField = "hello" ``` #### Config
+file loading *myConfig.toml* ```toml [mySerializableVar] myField = "some
+changed value" ``` ```py >>> import cfg >>> import carica >>> carica.loadCfg
+(cfg, "myConfig.toml") Config successfully loaded: myConfig.toml >>>
+cfg.mySerializableVar.myField some changed value ``` ### Premade models Carica
+provides serializable models that are ready to use (or extend) in your code.
+These models can be found in the `carica.models` package, which is imported by
+default. #### SerializableDataClass Removes the need to write boilerplate
+serializing functionality for dataclasses. This class is intended to be
+extended, adding definitions for your dataclass's fields. Extensions of
+`SerializableDataClass` **must** themselves be decorated with
+`@dataclasses.dataclass` in order to function correctly. #### SerializablePath
+An OS-agnostic filesystem path, extending `pathlib.Path`. The serializing/
+deserializing behaviour added by this class is minimal, a serialized
+`SerializablePath` is simply the string representation of the path, for
+readability. All other behaviour of `pathlib.Path` applies, for example.
+`SerializablePath` can be instantiated from a single path: `SerializablePath
+("my/directory/path")`, or from path segments: `SerializablePath("my", "file",
+"path.toml")`. #### SerializableTimedelta `datetime.datetime` is already
+considered a primitive type by TomlKit, and so no serializability needs to be
+added for you to use this class in your configs. However, `datetime.timedelta`
+is not serializable by default. `SerializableTimedelta` solves this issue as a
+serializable subclass. As a subclass, all `timedelta` behaiour applies,
+including the usual constructor. In addition,
+`SerializableTimedelta.fromTimedelta` is a convenience class method that
+accepts a `datetime.timedelta` and constructs a new `SerializableTimedelta`
+from it. #### Premade models example The recommended usage pattern for
+`SerializableDataClass` is to separate your models into a separate module/
+package, allowing for 'schema' definition as python code. This pattern is not
+necessary, model definition *can* be done in your config file.
+*configSchema.py* ```py from carica.models import SerializableDataClass from
+dataclasses import dataclass @dataclass class UserDataField
+(SerializableDataClass): name: str validation_regex: str ``` *config.py* ```py
+from carica.models import SerializablePath, SerializableTimedelta from
+configSchema import UserDataField from datetime import datetime
+new_user_required_fields = [ UserDataField( name = "user-name" validation_regex
+= "[a-z]+" ), UserDataField( name = "password" validation_regex = "\\b
+(?!password\\b)\\w+" ) ] database_path = SerializablePath("default/path.csv")
+birthday = datetime(day=1, month=1, year=1500) connection_timeout =
+SerializableTimedelta(minutes=5) ``` ## Planned features - Preceeding comments:
+This functionality is 'complete' in that it functions as intended and passes
+all unit tests, however an issue needs to be worked aruond before the feature
+can be enabled: In order to disambiguate between variables and table fields,
+the TOML spec requires that arrays and tables be placed at the end of a
+document. Carica currently depends upon documents being rendered with variables
+appearing in the same order as they appear in the python config module, which
+is not guaranteed. This leads to trailing and otherwise misplaced preceeding
+comments. - Config mutation: Carica should allow for loading an existing
+config, changing some values, and then updating the TOML document with new
+values. This should retain all formatting from the original document, including
+variable ordering and any comments that are not present in the python module.
+## Limitations - No support for schema migration - No support for asynchronous
+object serializing/deserializing - Imperfect estimation of variables defined in
+python modules: Listing the variables defined within a scope is not a known
+feature of python, and so Carica estimates this information by iterating over
+the tokens in your module. Carica does not build an AST of your python module.
+This means that certain name definition structures will result in false
+positives/negatives. This behaviour has not been extensively tested, but once
+such false positive has been identified: When invoking a callable (such as a
+class or function) with a keyword argument on a new, unindented line, the
+argument name will be falsely identified as a variable name. E.g: ```py
+my_variable = dict(key1=value1, key2=value2) ``` produces `my_variable` and
+`key2` as variable names.
```

### Comparing `carica-1.3.3/setup.cfg` & `carica-1.3.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `carica-1.3.3/src/carica/carica.py` & `carica-1.3.4/src/carica/carica.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 
     def hasPre(self):
         return self.preComments != []
 
 
 @runtime_checkable
 class _TKItemWithValue(Protocol):
-    def value(self): ...
+    def unwrap(self) -> Any: ...
 
 
 def _partialModuleVariables(module: ModuleType) -> Dict[str, ConfigVariable]:
     """Estimate The set of variables defined in the given module.
     Attempts to ignore other name types, such as functions, classes and imports.
     Names cannot be indented, and multiple assignment is not supported - variable declarations must be on their own lines.
 
@@ -456,25 +456,25 @@
             elif badNameHandling == ErrorHandling.LOG:
                 log(f"[WARNING] Ignoring unrecognised config variable name: {varName}")
 
         else:
             # Get the type of the default value (or the type override) for this variable
             defaultType = defaults[varName].loadedType
 
-            # Get the value for the variable that is defined in the config file
-            # This check ignores any config attributes that do not have a value, for example comments and whitespace.
-            if isinstance(config[varName], _TKItemWithValue):
-                newValue: Any = cast(_TKItemWithValue, config[varName]).value
-            else:
-                continue
+            newValue = config[varName]
 
             # Convert incompatible types, e.g TOMLDocument
             if isinstance(newValue, INCOMPATIBLE_TOML_TYPES):
                 newValue = convertIncompatibleTomlTypes(newValue)
 
+            # Get the value for the variable that is defined in the config file
+            # This check ignores any config attributes that do not have a value, for example comments and whitespace.
+            if isinstance(config[varName], _TKItemWithValue):
+                newValue: Any = cast(_TKItemWithValue, config[varName]).unwrap()
+
             # deserialize serializable variables
             if issubclass(defaultType, SerializableType):
                 newValue = defaultType.deserialize(newValue, c_badTypeHandling=badTypeHandling, c_variableTrace=[varName])
 
             # Handle variables of different types to that which is defined in the python module
             if not isinstance(newValue, defaultType):
```

### Comparing `carica-1.3.3/src/carica/exceptions.py` & `carica-1.3.4/src/carica/exceptions.py`

 * *Files identical despite different names*

### Comparing `carica-1.3.3/src/carica/interface/Serializable.py` & `carica-1.3.4/src/carica/interface/Serializable.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 from __future__ import annotations
 from abc import ABC, abstractmethod
-from typing import Generic, Iterable, Mapping, Type, TypeVar, Union, Protocol, runtime_checkable, Optional
+from typing import Generic, Iterable, Mapping, Set, Tuple, Type, TypeVar, Union, Protocol, runtime_checkable, Optional
 from datetime import datetime
 
 # All types acceptable as toml data. Tomlkit handles serializing of datetime objects automatically.
 # Iterable includes set, list and tuple. It also includes dict and str!
 # this type is Optional, because None is allowed in toml, but there is no NoneType exposed in python for use in the Union.
 PrimativeType = Optional[Union[int, float, str, bool, datetime, Iterable["PrimativeType"], Mapping[str, "PrimativeType"]]]
-# PrimativeType as a shallow set
-primativeTypes = {int, float, str, bool, Iterable, Mapping, datetime, type(None)}
-# PrimativeTypes as a shallow tuple
-primativeTypesTuple = tuple(primativeTypes)
+# PrimativeType as a shallow tuple
+primativeTypes: Tuple[Type, ...] = (int, float, str, bool, Iterable, Mapping, datetime, type(None))
 
 TClass = TypeVar("TClass")
 
 @runtime_checkable
 class SerializableType(Protocol):
     """A type protocol representing any object with `serialize` and `deserialize` methods defined.
     Since this is a runtime checkable protocol class, isinstance() and issubclass() work for duck typing. That is,
@@ -66,17 +64,15 @@
         :return: A new object as specified by data
         :rtype: ISerializable
         """
         raise NotImplementedError()
     
 
 # All types which are themselves primative, or can be serialized into primative types, as a shallow set
-serializableTypes = primativeTypes.copy()
-serializableTypes.add(SerializableType)
-serializableTypesTuple = tuple(serializableTypes)
+serializableTypes: Tuple[Type] = tuple(t for t in primativeTypes) + (SerializableType,)
 
 TClass = TypeVar("TClass")
 TSerialized = TypeVar("TSerialized", bound=PrimativeType)
 
 class SerializesToType(SerializableType, Generic[TSerialized]):
     def serialize(self, **kwargs) -> TSerialized: ...
```

### Comparing `carica-1.3.3/src/carica/models/dataclasses.py` & `carica-1.3.4/src/carica/models/dataclasses.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from dataclasses import Field, dataclass, _MISSING_TYPE, fields
-from carica.interface import SerializableType, PrimativeType, primativeTypesTuple, SerializesToDict
+from carica.interface import SerializableType, PrimativeType, primativeTypes, SerializesToDict
 from carica.typeChecking import objectIsShallowSerializable, objectIsDeepSerializable, _DeserializedTypeOverrideProxy, _CallableDeserializedTypeOverrideProxy
 from carica.carica import BadTypeHandling, BadTypeBehaviour, ErrorHandling, VariableTrace, log, _serialize
 from carica import exceptions
 import typing
 import traceback
 from typing import Any, Dict, List, Mapping, Set, Tuple, Union, cast, TypeVar
 # ignoring a warning here because private type _BaseGenericAlias can't be imported right now.
@@ -179,15 +179,15 @@
         if issubclass(fieldType, SerializableType):
             if deserializeSerializable:
                 return fieldType.deserialize(serializedValue, **deserializerKwargs)
             else:
                 return serializedValue
 
         # Otherwise do nothing
-        elif issubclass(fieldType, primativeTypesTuple):
+        elif issubclass(fieldType, primativeTypes):
             if isinstance(serializedValue, fieldType):
                 return _handleTypeCasts(serializedValue, fieldName, fieldType, c_badTypeHandling)
             raise TypeError(f"Expected type of {fieldType} for field {fieldName}, " \
                             + f"but received serialized type {type(serializedValue).__name__}")
 
     # Handle generics other than Union (e.g List)
     elif isinstance(fieldType, _BaseGenericAlias):
@@ -357,15 +357,15 @@
     def serialize(self, **kwargs) -> Dict[str, PrimativeType]:
         """Serialize this object into a dictionary, to be recreated completely.
 
         :return: A dictionary mapping field names to serialized values
         :rtype: Dict[str, PrimativeType]
         """
 
-        return {k: _serialize(v) for k, v in self._fieldItems()}
+        return {k: _serialize(v, [k]) for k, v in self._fieldItems()}
 
 
     @classmethod
     def deserialize(cls, data: Mapping[str, PrimativeType], deserializeValues: bool = True, c_variableTrace: VariableTrace = [], **kwargs):
         """Recreate a serialized SerializableDataClass object. If `deserializeValues` is `True`,
         values fields which are serializable types will be automatically deserialized.
 
@@ -379,11 +379,12 @@
 
         for k, v in data.items():
             if not isinstance(k, str):
                 raise exceptions.NonStringMappingKey(k, path=c_variableTrace)
             data[k] = _deserializeField(k, cls._overriddenTypeOfFieldNamed(k), v, c_variableTrace=c_variableTrace + [k], 
                                         deserializeSerializable=deserializeValues, **kwargs)
 
-        constructorArgs = inspect.signature(cls.__init__).parameters
+        # TODO: Unknown pyright warning - this code functions as expected
+        constructorArgs = inspect.signature(cls.__init__).parameters # type: ignore[reportGeneralTypeIssues]
         classKwargs = {k: v for k, v in kwargs.items() if k in constructorArgs}
 
         return cls(**data, **classKwargs)
```

### Comparing `carica-1.3.3/src/carica/models/path.py` & `carica-1.3.4/src/carica/models/path.py`

 * *Files identical despite different names*

### Comparing `carica-1.3.3/src/carica/models/timedelta.py` & `carica-1.3.4/src/carica/models/timedelta.py`

 * *Files identical despite different names*

### Comparing `carica-1.3.3/src/carica/typeChecking.py` & `carica-1.3.4/src/carica/typeChecking.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import Any, Iterable, List, Mapping, TypeVar, Union, cast, Callable
 # ignoring a warning here because private type _BaseGenericAlias can't be imported right now.
 # it is a necessary import to unify over user-defined and special generics.
 from typing import _BaseGenericAlias # type: ignore
-from carica.interface import serializableTypesTuple, primativeTypesTuple
+from carica.interface import serializableTypes, primativeTypes
 from carica import exceptions
 from wrapt import ObjectProxy, CallableObjectProxy
 
 TypeHint = Union[type, _BaseGenericAlias]
 
 class _DeserializedTypeOverrideProxy(ObjectProxy):
     def __init__(self, wrapped, typeOverride: TypeHint):
@@ -52,15 +52,15 @@
     True
     ```
 
     :param Any o: The object whose type to check
     :return: True if o itself is a primative type, False otherwise
     :rtype: bool
     """
-    return isinstance(o, primativeTypesTuple)
+    return isinstance(o, primativeTypes)
 
 
 def objectIsDeepPrimative(o: Any) -> bool:
     """Decide if a class is a primative type, including any objects potentially contained within it.
     I.e:
     ```
     >>> objectIsDeepPrimative(1)
@@ -115,15 +115,15 @@
     True
     ```
 
     :param Any o: The object whose type to check
     :return: True if o itself is a primative or serializable type, False otherwise
     :rtype: bool
     """
-    return isinstance(o, serializableTypesTuple)
+    return isinstance(o, serializableTypes)
 
 
 def objectIsDeepSerializable(o: Any) -> bool:
     """Decide if a class is a primative or serializable type, including any objects potentially contained within it.
     I.e:
     ```
     >>> objectIsDeepSerializable(1)
```

### Comparing `carica-1.3.3/src/carica/util.py` & `carica-1.3.4/src/carica/util.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from typing import Any, Dict, List, Union, cast
 from tomlkit.container import Container as TKContainer
-from tomlkit.items import AoT
+from tomlkit.items import Array, AoT, Table
 
-INCOMPATIBLE_TOML_TYPES = (TKContainer, AoT)
+INCOMPATIBLE_TOML_TYPES = (TKContainer, Table, Array, AoT)
 
-def convertIncompatibleTomlTypes(doc: Union[TKContainer, AoT]) -> Union[List[Any], Dict[str, Any]]:
+def convertIncompatibleTomlTypes(doc: Union[TKContainer, AoT, Array, Table]) -> Union[List[Any], Dict[str, Any]]:
     """Recursively converts tomlkit tables/lists of tables into dictionaries/lists of dictionaries
 
     :param doc: The item to convert
     :type doc: Union[TKContainer, AoT]
     :return: doc recursively converted to python types instead of TOMLKit Containers/AoTs
     """
-    if isinstance(doc, TKContainer):
+    if isinstance(doc, (TKContainer, Table)):
         # Not sure why mypy doesn't pick up on Container inheriting from dict
         return {k: convertIncompatibleTomlTypes(v) for k, v in  cast(dict, doc).items()}
-    elif isinstance(doc, AoT):
+    elif isinstance(doc, (Array, AoT)):
         return [convertIncompatibleTomlTypes(v) for v in doc]
     else:
         return doc
```

### Comparing `carica-1.3.3/src/carica.egg-info/PKG-INFO` & `carica-1.3.4/src/carica.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: carica
-Version: 1.3.3
+Version: 1.3.4
 Summary: Python module that populates variables from TOML config documents, and generates config documents from python variables.
 Home-page: https://github.com/Trimatix/carica
 Author: Jasper Law
 Author-email: trimatix.music@gmail.com
 Project-URL: Bug Tracker, https://github.com/Trimatix/carica/issues
 Keywords: config,cfg,python,toml,generate,auto-generate,orm
 Classifier: Programming Language :: Python :: 3.8
@@ -22,15 +22,15 @@
     alt="Carica Logo"
   />
 </p>
 <h1 align="center">Carica - A Python Configurator</h1>
 <p align="center">
   <a href="https://github.com/Trimatix/Carica/actions"
     ><img
-      src="https://img.shields.io/github/workflow/status/GOF2BountyBot/GOF2BountyBot/BASED"
+      src="https://img.shields.io/github/actions/workflow/status/Trimatix/Carica/testing.yml?branch=main"
       alt="GitHub Actions workflow status"
   /></a>
   <a href="https://github.com/Trimatix/Carica/projects/1?card_filter_query=label%3Abug"
     ><img
       src="https://img.shields.io/github/issues-search?color=eb4034&label=bug%20reports&query=repo%3ATrimatix%2FCarica%20is%3Aopen%20label%3Abug"
       alt="GitHub open bug reports"
   /></a>
@@ -330,17 +330,15 @@
 
 Projects which prefer strong typing may implement the `carica.ISerializable` interface to enforce this pattern with inheritence. Carica will validate serialized objects against the `carica.PrimativeType` type alias, which is also exposed for use.
 
 ### Example
 
 *cfg.py*
 ```py
-from carica import ISerializable
-
-class MySerializableType(ISerializable):
+class MySerializableType:
     def __init__(self, myField):
         self.myField = myField
 
     def serialize(self, **kwargs):
         return {"myField": self.myField}
 
     @classmethod
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: carica Version: 1.3.3 Summary: Python module that
+Metadata-Version: 2.1 Name: carica Version: 1.3.4 Summary: Python module that
 populates variables from TOML config documents, and generates config documents
 from python variables. Home-page: https://github.com/Trimatix/carica Author:
 Jasper Law Author-email: trimatix.music@gmail.com Project-URL: Bug Tracker,
 https://github.com/Trimatix/carica/issues Keywords:
 config,cfg,python,toml,generate,auto-generate,orm Classifier: Programming
 Language :: Python :: 3.8 Classifier: License :: OSI Approved :: Apache
 Software License Classifier: Operating System :: OS Independent Requires-
@@ -124,77 +124,77 @@
 `deserialize` must be a class method, and should transform a serialized object
 representation into a new object. Carica enforces this pattern on non-primative
 types using the `SerializableType` type protocol, which allows for duck-typed
 serializable types. This protocol is exposed for use with `isinstance`.
 Projects which prefer strong typing may implement the `carica.ISerializable`
 interface to enforce this pattern with inheritence. Carica will validate
 serialized objects against the `carica.PrimativeType` type alias, which is also
-exposed for use. ### Example *cfg.py* ```py from carica import ISerializable
-class MySerializableType(ISerializable): def __init__(self, myField):
-self.myField = myField def serialize(self, **kwargs): return {"myField":
-self.myField} @classmethod def deserialize(self, data, **kwargs): return
-MySerializableClass(data["myField"]) mySerializableVar = MySerializableClass
-("hello") ``` #### Default config generation ```py >>> import cfg >>> import
-carica >>> carica.makeDefaultCfg(cfg) Created defaultCfg.toml ``` The above
-code will produce the following file: *defaultCfg.toml* ```toml
-[mySerializableVar] myField = "hello" ``` #### Config file loading
-*myConfig.toml* ```toml [mySerializableVar] myField = "some changed value" ```
-```py >>> import cfg >>> import carica >>> carica.loadCfg(cfg, "myConfig.toml")
-Config successfully loaded: myConfig.toml >>> cfg.mySerializableVar.myField
-some changed value ``` ### Premade models Carica provides serializable models
-that are ready to use (or extend) in your code. These models can be found in
-the `carica.models` package, which is imported by default. ####
-SerializableDataClass Removes the need to write boilerplate serializing
-functionality for dataclasses. This class is intended to be extended, adding
-definitions for your dataclass's fields. Extensions of `SerializableDataClass`
-**must** themselves be decorated with `@dataclasses.dataclass` in order to
-function correctly. #### SerializablePath An OS-agnostic filesystem path,
-extending `pathlib.Path`. The serializing/deserializing behaviour added by this
-class is minimal, a serialized `SerializablePath` is simply the string
-representation of the path, for readability. All other behaviour of
-`pathlib.Path` applies, for example. `SerializablePath` can be instantiated
-from a single path: `SerializablePath("my/directory/path")`, or from path
-segments: `SerializablePath("my", "file", "path.toml")`. ####
-SerializableTimedelta `datetime.datetime` is already considered a primitive
-type by TomlKit, and so no serializability needs to be added for you to use
-this class in your configs. However, `datetime.timedelta` is not serializable
-by default. `SerializableTimedelta` solves this issue as a serializable
-subclass. As a subclass, all `timedelta` behaiour applies, including the usual
-constructor. In addition, `SerializableTimedelta.fromTimedelta` is a
-convenience class method that accepts a `datetime.timedelta` and constructs a
-new `SerializableTimedelta` from it. #### Premade models example The
-recommended usage pattern for `SerializableDataClass` is to separate your
-models into a separate module/package, allowing for 'schema' definition as
-python code. This pattern is not necessary, model definition *can* be done in
-your config file. *configSchema.py* ```py from carica.models import
-SerializableDataClass from dataclasses import dataclass @dataclass class
-UserDataField(SerializableDataClass): name: str validation_regex: str ```
-*config.py* ```py from carica.models import SerializablePath,
-SerializableTimedelta from configSchema import UserDataField from datetime
-import datetime new_user_required_fields = [ UserDataField( name = "user-name"
-validation_regex = "[a-z]+" ), UserDataField( name = "password"
-validation_regex = "\\b(?!password\\b)\\w+" ) ] database_path =
-SerializablePath("default/path.csv") birthday = datetime(day=1, month=1,
-year=1500) connection_timeout = SerializableTimedelta(minutes=5) ``` ## Planned
-features - Preceeding comments: This functionality is 'complete' in that it
-functions as intended and passes all unit tests, however an issue needs to be
-worked aruond before the feature can be enabled: In order to disambiguate
-between variables and table fields, the TOML spec requires that arrays and
-tables be placed at the end of a document. Carica currently depends upon
-documents being rendered with variables appearing in the same order as they
-appear in the python config module, which is not guaranteed. This leads to
-trailing and otherwise misplaced preceeding comments. - Config mutation: Carica
-should allow for loading an existing config, changing some values, and then
-updating the TOML document with new values. This should retain all formatting
-from the original document, including variable ordering and any comments that
-are not present in the python module. ## Limitations - No support for schema
-migration - No support for asynchronous object serializing/deserializing -
-Imperfect estimation of variables defined in python modules: Listing the
-variables defined within a scope is not a known feature of python, and so
-Carica estimates this information by iterating over the tokens in your module.
-Carica does not build an AST of your python module. This means that certain
-name definition structures will result in false positives/negatives. This
-behaviour has not been extensively tested, but once such false positive has
-been identified: When invoking a callable (such as a class or function) with a
-keyword argument on a new, unindented line, the argument name will be falsely
-identified as a variable name. E.g: ```py my_variable = dict(key1=value1,
-key2=value2) ``` produces `my_variable` and `key2` as variable names.
+exposed for use. ### Example *cfg.py* ```py class MySerializableType: def
+__init__(self, myField): self.myField = myField def serialize(self, **kwargs):
+return {"myField": self.myField} @classmethod def deserialize(self, data,
+**kwargs): return MySerializableClass(data["myField"]) mySerializableVar =
+MySerializableClass("hello") ``` #### Default config generation ```py >>>
+import cfg >>> import carica >>> carica.makeDefaultCfg(cfg) Created
+defaultCfg.toml ``` The above code will produce the following file:
+*defaultCfg.toml* ```toml [mySerializableVar] myField = "hello" ``` #### Config
+file loading *myConfig.toml* ```toml [mySerializableVar] myField = "some
+changed value" ``` ```py >>> import cfg >>> import carica >>> carica.loadCfg
+(cfg, "myConfig.toml") Config successfully loaded: myConfig.toml >>>
+cfg.mySerializableVar.myField some changed value ``` ### Premade models Carica
+provides serializable models that are ready to use (or extend) in your code.
+These models can be found in the `carica.models` package, which is imported by
+default. #### SerializableDataClass Removes the need to write boilerplate
+serializing functionality for dataclasses. This class is intended to be
+extended, adding definitions for your dataclass's fields. Extensions of
+`SerializableDataClass` **must** themselves be decorated with
+`@dataclasses.dataclass` in order to function correctly. #### SerializablePath
+An OS-agnostic filesystem path, extending `pathlib.Path`. The serializing/
+deserializing behaviour added by this class is minimal, a serialized
+`SerializablePath` is simply the string representation of the path, for
+readability. All other behaviour of `pathlib.Path` applies, for example.
+`SerializablePath` can be instantiated from a single path: `SerializablePath
+("my/directory/path")`, or from path segments: `SerializablePath("my", "file",
+"path.toml")`. #### SerializableTimedelta `datetime.datetime` is already
+considered a primitive type by TomlKit, and so no serializability needs to be
+added for you to use this class in your configs. However, `datetime.timedelta`
+is not serializable by default. `SerializableTimedelta` solves this issue as a
+serializable subclass. As a subclass, all `timedelta` behaiour applies,
+including the usual constructor. In addition,
+`SerializableTimedelta.fromTimedelta` is a convenience class method that
+accepts a `datetime.timedelta` and constructs a new `SerializableTimedelta`
+from it. #### Premade models example The recommended usage pattern for
+`SerializableDataClass` is to separate your models into a separate module/
+package, allowing for 'schema' definition as python code. This pattern is not
+necessary, model definition *can* be done in your config file.
+*configSchema.py* ```py from carica.models import SerializableDataClass from
+dataclasses import dataclass @dataclass class UserDataField
+(SerializableDataClass): name: str validation_regex: str ``` *config.py* ```py
+from carica.models import SerializablePath, SerializableTimedelta from
+configSchema import UserDataField from datetime import datetime
+new_user_required_fields = [ UserDataField( name = "user-name" validation_regex
+= "[a-z]+" ), UserDataField( name = "password" validation_regex = "\\b
+(?!password\\b)\\w+" ) ] database_path = SerializablePath("default/path.csv")
+birthday = datetime(day=1, month=1, year=1500) connection_timeout =
+SerializableTimedelta(minutes=5) ``` ## Planned features - Preceeding comments:
+This functionality is 'complete' in that it functions as intended and passes
+all unit tests, however an issue needs to be worked aruond before the feature
+can be enabled: In order to disambiguate between variables and table fields,
+the TOML spec requires that arrays and tables be placed at the end of a
+document. Carica currently depends upon documents being rendered with variables
+appearing in the same order as they appear in the python config module, which
+is not guaranteed. This leads to trailing and otherwise misplaced preceeding
+comments. - Config mutation: Carica should allow for loading an existing
+config, changing some values, and then updating the TOML document with new
+values. This should retain all formatting from the original document, including
+variable ordering and any comments that are not present in the python module.
+## Limitations - No support for schema migration - No support for asynchronous
+object serializing/deserializing - Imperfect estimation of variables defined in
+python modules: Listing the variables defined within a scope is not a known
+feature of python, and so Carica estimates this information by iterating over
+the tokens in your module. Carica does not build an AST of your python module.
+This means that certain name definition structures will result in false
+positives/negatives. This behaviour has not been extensively tested, but once
+such false positive has been identified: When invoking a callable (such as a
+class or function) with a keyword argument on a new, unindented line, the
+argument name will be falsely identified as a variable name. E.g: ```py
+my_variable = dict(key1=value1, key2=value2) ``` produces `my_variable` and
+`key2` as variable names.
```

### Comparing `carica-1.3.3/src/carica.egg-info/SOURCES.txt` & `carica-1.3.4/src/carica.egg-info/SOURCES.txt`

 * *Files identical despite different names*

