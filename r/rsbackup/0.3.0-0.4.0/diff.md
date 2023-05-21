# Comparing `tmp/rsbackup-0.3.0.tar.gz` & `tmp/rsbackup-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rsbackup-0.3.0.tar", last modified: Sat Mar 25 14:15:25 2023, max compression
+gzip compressed data, was "rsbackup-0.4.0.tar", last modified: Sun May 21 16:22:53 2023, max compression
```

## Comparing `rsbackup-0.3.0.tar` & `rsbackup-0.4.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-03-25 14:15:25.491934 rsbackup-0.3.0/
--rw-r--r--   0 alex       (501) staff       (20)    11357 2023-03-23 08:40:01.000000 rsbackup-0.3.0/LICENSE
--rw-r--r--   0 alex       (501) staff       (20)     5488 2023-03-25 14:15:25.492120 rsbackup-0.3.0/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)     4709 2023-03-25 07:53:54.000000 rsbackup-0.3.0/README.md
--rw-r--r--   0 alex       (501) staff       (20)      107 2023-03-23 08:40:01.000000 rsbackup-0.3.0/pyproject.toml
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-03-25 14:15:25.469627 rsbackup-0.3.0/rsbackup/
--rw-r--r--   0 alex       (501) staff       (20)     8978 2023-03-25 14:11:28.000000 rsbackup-0.3.0/rsbackup/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     5688 2023-03-25 07:53:54.000000 rsbackup-0.3.0/rsbackup/__main__.py
--rw-r--r--   0 alex       (501) staff       (20)      812 2023-03-23 08:40:01.000000 rsbackup-0.3.0/rsbackup/main_test.py
--rw-r--r--   0 alex       (501) staff       (20)     3167 2023-03-23 14:37:13.000000 rsbackup-0.3.0/rsbackup/rsbackup_test.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-03-25 14:15:25.488478 rsbackup-0.3.0/rsbackup.egg-info/
--rw-r--r--   0 alex       (501) staff       (20)     5488 2023-03-25 14:15:25.000000 rsbackup-0.3.0/rsbackup.egg-info/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)      353 2023-03-25 14:15:25.000000 rsbackup-0.3.0/rsbackup.egg-info/SOURCES.txt
--rw-r--r--   0 alex       (501) staff       (20)        1 2023-03-25 14:15:25.000000 rsbackup-0.3.0/rsbackup.egg-info/dependency_links.txt
--rw-r--r--   0 alex       (501) staff       (20)       52 2023-03-25 14:15:25.000000 rsbackup-0.3.0/rsbackup.egg-info/entry_points.txt
--rw-r--r--   0 alex       (501) staff       (20)       30 2023-03-25 14:15:25.000000 rsbackup-0.3.0/rsbackup.egg-info/requires.txt
--rw-r--r--   0 alex       (501) staff       (20)        9 2023-03-25 14:15:25.000000 rsbackup-0.3.0/rsbackup.egg-info/top_level.txt
--rw-r--r--   0 alex       (501) staff       (20)        1 2023-03-25 14:15:25.000000 rsbackup-0.3.0/rsbackup.egg-info/zip-safe
--rw-r--r--   0 alex       (501) staff       (20)      961 2023-03-25 14:15:25.492864 rsbackup-0.3.0/setup.cfg
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-05-21 16:22:53.573100 rsbackup-0.4.0/
+-rw-r--r--   0 alex       (501) staff       (20)    11357 2023-03-16 08:29:09.000000 rsbackup-0.4.0/LICENSE
+-rw-r--r--   0 alex       (501) staff       (20)     5501 2023-05-21 16:22:53.573181 rsbackup-0.4.0/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)     4721 2023-05-21 16:19:13.000000 rsbackup-0.4.0/README.md
+-rw-r--r--   0 alex       (501) staff       (20)      107 2023-03-16 08:29:09.000000 rsbackup-0.4.0/pyproject.toml
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-05-21 16:22:53.572040 rsbackup-0.4.0/rsbackup/
+-rw-r--r--   0 alex       (501) staff       (20)     9066 2023-05-21 16:18:45.000000 rsbackup-0.4.0/rsbackup/__init__.py
+-rw-r--r--   0 alex       (501) staff       (20)     5644 2023-05-21 16:17:59.000000 rsbackup-0.4.0/rsbackup/__main__.py
+-rw-r--r--   0 alex       (501) staff       (20)      824 2023-05-21 16:17:59.000000 rsbackup-0.4.0/rsbackup/main_test.py
+-rw-r--r--   0 alex       (501) staff       (20)     4662 2023-05-21 16:17:59.000000 rsbackup-0.4.0/rsbackup/rsbackup_test.py
+drwxr-xr-x   0 alex       (501) staff       (20)        0 2023-05-21 16:22:53.572993 rsbackup-0.4.0/rsbackup.egg-info/
+-rw-r--r--   0 alex       (501) staff       (20)     5501 2023-05-21 16:22:53.000000 rsbackup-0.4.0/rsbackup.egg-info/PKG-INFO
+-rw-r--r--   0 alex       (501) staff       (20)      353 2023-05-21 16:22:53.000000 rsbackup-0.4.0/rsbackup.egg-info/SOURCES.txt
+-rw-r--r--   0 alex       (501) staff       (20)        1 2023-05-21 16:22:53.000000 rsbackup-0.4.0/rsbackup.egg-info/dependency_links.txt
+-rw-r--r--   0 alex       (501) staff       (20)       52 2023-05-21 16:22:53.000000 rsbackup-0.4.0/rsbackup.egg-info/entry_points.txt
+-rw-r--r--   0 alex       (501) staff       (20)       30 2023-05-21 16:22:53.000000 rsbackup-0.4.0/rsbackup.egg-info/requires.txt
+-rw-r--r--   0 alex       (501) staff       (20)        9 2023-05-21 16:22:53.000000 rsbackup-0.4.0/rsbackup.egg-info/top_level.txt
+-rw-r--r--   0 alex       (501) staff       (20)        1 2023-05-21 16:22:53.000000 rsbackup-0.4.0/rsbackup.egg-info/zip-safe
+-rw-r--r--   0 alex       (501) staff       (20)      962 2023-05-21 16:22:53.573447 rsbackup-0.4.0/setup.cfg
```

### Comparing `rsbackup-0.3.0/LICENSE` & `rsbackup-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rsbackup-0.3.0/PKG-INFO` & `rsbackup-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: rsbackup
-Version: 0.3.0
+Version: 0.4.0
 Summary: Backup for unix-like systems using rsync.
 Home-page: https://github.com/halimath/rsbackup
 Author: Alexander Metzner
 Author-email: alexander.metzner@gmail.com
 License: Apache
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Archiving :: Backup
 Classifier: Topic :: Utilities
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # rsbackup
@@ -69,15 +69,15 @@
 shell escaping.
 
 Each table contains the following keys:
 
 Key | Type | Optional | Description
 -- | -- | -- | --
 `description` | string | yes | contains an optional description.
-`source` | string | no | lists the source directory to create a backup of
+`sources` | array of string | no | lists the source directories to create a backup of
 `target` | string | no | contains a target directory which will eventualy contain multiple backups
 `excludes` | array of strings | yes | lists patterns to be excluded from the backup. See the `rsync` documentation for a description of the pattern format.
 
 You can use
 
 ```shell
 rsbackup list
```

### Comparing `rsbackup-0.3.0/README.md` & `rsbackup-0.4.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 shell escaping.
 
 Each table contains the following keys:
 
 Key | Type | Optional | Description
 -- | -- | -- | --
 `description` | string | yes | contains an optional description.
-`source` | string | no | lists the source directory to create a backup of
+`sources` | array of string | no | lists the source directories to create a backup of
 `target` | string | no | contains a target directory which will eventualy contain multiple backups
 `excludes` | array of strings | yes | lists patterns to be excluded from the backup. See the `rsync` documentation for a description of the pattern format.
 
 You can use
 
 ```shell
 rsbackup list
```

### Comparing `rsbackup-0.3.0/rsbackup/__init__.py` & `rsbackup-0.4.0/rsbackup/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import os
 import shutil
 import typing
 
 import aiofiles
 import aiofiles.os
 
-__version__ = '0.3.0'
+__version__ = '0.4.0'
 __author__ = 'Alexander Metzner'
 
 _LATEST = '_latest'
 
 
 class LoggingProtocol(typing.Protocol):
     """
@@ -52,35 +52,35 @@
 
 class Backup:
     """A class that represents a single backup definition.
 
     A Backup can be exectued which will produce a new backup generation. 
     """
 
-    def __init__(self, source: str, target: str,
+    def __init__(self, sources: typing.Sequence[str], target: str,
                  description: typing.Optional[str] = None,
                  excludes: typing.Optional[typing.Iterable[str]] = None):
         """Initializes the Backup instance to use.
 
-        `source` is the source path to create a backup from.
+        `sources` is the sequence of source paths to create a backup from.
 
         `target` is the target path containing the backup generations.
 
         `description` is an optional human readable description.
 
         `excludes` is an optional list of exclude patterns as defined by
         rsync.
         """
-        self.source = source
+        self.sources = sources
         self.target = target
         self.description = description
         self.excludes = list(excludes or [])
 
     def __eq__(self, other):
-        return self.source == other.source and\
+        return self.sources == other.sources and\
             self.target == other.target and\
             self.description == other.description and\
             self.excludes == other.excludes
 
     async def run(self, logger: typing.Optional[LoggingProtocol] = None,
                   dry_mode: bool = False, skip_latest: bool = False):
         """Creates a new generation for this backup.
@@ -99,26 +99,26 @@
         """
         start = datetime.datetime.now()
         target = os.path.join(self.target, start.isoformat(
             sep='_', timespec='seconds').replace(':', '-'))
         latest = os.path.join(self.target, _LATEST)
         log_file = os.path.join(target, '.log')
 
-        await logger.info(f"Creating new backup generation for '{self.source}'")
+        await logger.info(f"Creating new backup generation for '{', '.join(self.sources)}'")
 
         await logger.details(f"Creating backup at {target}")
 
         prev = None
 
         if not skip_latest and os.path.exists(latest):
             prev = os.readlink(latest)
             await logger.info(
                 f"Found previous backup generation at {prev}")
 
-        rs = RSync(self.source, target, excludes=self.excludes, link_dest=prev)
+        rs = RSync(self.sources, target, excludes=self.excludes, link_dest=prev)
 
         if dry_mode:
             await logger.warn(
                 'dry_mode is set to True; not going to touch any files.')
             await logger.details(f"mkdir -p {target}")
             await logger.details(' '.join(rs.command))
 
@@ -153,24 +153,24 @@
                 await aiofiles.os.remove(latest)
 
             # TODO: Make this asynchronous
             os.symlink(target, latest)
 
         end = datetime.datetime.now()
 
-        await logger.success(f"Backup of '{self.source}' finished at '{start}'")
+        await logger.success(f"Backup of {self.sources!r} finished at '{start}'")
         await logger.details(f"Took {end - start}")
 
 
 class RSync:
     """A class to execute rsync as a subprocess. The constructor provides 
     keyword args to set different options which are passed to rsync as command
     line args.
 
-    `source` defines the source file or directory.
+    `sources` defines the source files or directories.
 
     `target` defines the target directory.
 
     If `archive` is set to True (the default) rsync is run in archive mode.
 
     If `verbose` is set to True (the default) rsync will output additional log.
 
@@ -187,20 +187,21 @@
     syntax supported by exclude.
 
     If `binary` is not `None` it will be used as the binary to execute rsync,
     i.e. `/usr/bin/rsync`. If `None`, binary will be determined from the `PATH`
     environment variable.
     """
 
-    def __init__(self, source: str, target: str, archive: bool = True,
+    def __init__(self, sources: typing.Sequence[str], target: str, 
+                 archive: bool = True,
                  verbose: bool = True, delete: bool = True,
                  link_dest: str = None,
                  excludes: typing.Optional[typing.Iterable[str]] = None,
                  binary: typing.Optional[str] = None):
-        self.source = source
+        self.sources = sources
         self.target = target
         self.archive = archive
         self.verbose = verbose
         self.delete = delete
         self.link_dest = link_dest
         self.excludes = excludes
         self.binary = binary or shutil.which('rsync')
@@ -250,15 +251,15 @@
 
         if self.delete:
             args.append('--delete')
 
         if dry_run:
             args.append('--dry-run')
 
-        args.append(self.source)
+        args += self.sources
 
         if self.link_dest:
             args.append('--link-dest')
             args.append(self.link_dest)
 
         if self.excludes:
             for exclude in self.excludes:
```

### Comparing `rsbackup-0.3.0/rsbackup/__main__.py` & `rsbackup-0.4.0/rsbackup/__main__.py`

 * *Files 5% similar despite different names*

```diff
@@ -101,18 +101,15 @@
     Backup values.
 
     `s` must be valid TOML configuration.
     """
     data = tomli.loads(s)
 
     return {key: Backup(
-        source=os.path.abspath(
-            os.path.normpath(data[key]['source'] if os.path.isabs(
-                data[key]['source']) else os.path.join(basedir,
-                                                       data[key]['source']))),
+        sources=[os.path.abspath(os.path.normpath(p)) if os.path.isabs(p) else os.path.join(basedir, p) for p in data[key]['sources']],
         target=os.path.abspath(
             os.path.normpath(data[key]['target'] if os.path.isabs(
                 data[key]['target']) else os.path.join(basedir,
                                                        data[key]['target']))),
         description=data[key].get('description'),
         excludes=data[key].get('excludes') or [],
     ) for key in data}
@@ -160,21 +157,22 @@
         async with app.apply_styles(BOLD, FG_CYAN):
             await app.write(name)
         if c.description:
             await app.write(f" - {c.description}")
 
         await app.write_line()
         
-        await app.write('  Source: ')
+        await app.write_line('  Sources:')
         async with app.apply_styles(FG_CYAN):
-            await app.write_line(c.source)
+            for src in c.sources:
+                await app.write_line(f"    - {src}")
 
-        await app.write('  Target: ')
+        await app.write_line('  Target:')
         async with app.apply_styles(FG_CYAN):
-            await app.write_line(c.target)
+            await app.write_line(f"    {c.target}")
 
         await app.write_line('  Excludes:')
         for e in c.excludes:
             await app.write_line(f'    - {e}')
         await app.write_line()
     return 0
```

### Comparing `rsbackup-0.3.0/rsbackup.egg-info/PKG-INFO` & `rsbackup-0.4.0/rsbackup.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: rsbackup
-Version: 0.3.0
+Version: 0.4.0
 Summary: Backup for unix-like systems using rsync.
 Home-page: https://github.com/halimath/rsbackup
 Author: Alexander Metzner
 Author-email: alexander.metzner@gmail.com
 License: Apache
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Natural Language :: English
 Classifier: Operating System :: POSIX
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: System :: Archiving :: Backup
 Classifier: Topic :: Utilities
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # rsbackup
@@ -69,15 +69,15 @@
 shell escaping.
 
 Each table contains the following keys:
 
 Key | Type | Optional | Description
 -- | -- | -- | --
 `description` | string | yes | contains an optional description.
-`source` | string | no | lists the source directory to create a backup of
+`sources` | array of string | no | lists the source directories to create a backup of
 `target` | string | no | contains a target directory which will eventualy contain multiple backups
 `excludes` | array of strings | yes | lists patterns to be excluded from the backup. See the `rsync` documentation for a description of the pattern format.
 
 You can use
 
 ```shell
 rsbackup list
```

### Comparing `rsbackup-0.3.0/setup.cfg` & `rsbackup-0.4.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -11,16 +11,16 @@
 classifiers = 
 	Development Status :: 4 - Beta
 	Environment :: Console
 	Intended Audience :: System Administrators
 	License :: OSI Approved :: Apache Software License
 	Natural Language :: English
 	Operating System :: POSIX
-	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Topic :: System :: Archiving :: Backup
 	Topic :: Utilities
 
 [options]
 zip_safe = True
 packages = rsbackup
 python_requires = >=3.10
```

