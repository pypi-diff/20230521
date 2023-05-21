# Comparing `tmp/seaport-0.8.0.tar.gz` & `tmp/seaport-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seaport-0.8.0.tar", max compression
+gzip compressed data, was "seaport-0.9.0.tar", max compression
```

## Comparing `seaport-0.8.0.tar` & `seaport-0.9.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1498 2022-08-03 17:26:21.773443 seaport-0.8.0/LICENSE
--rw-r--r--   0        0        0     5265 2023-02-07 18:34:29.437125 seaport-0.8.0/README.rst
--rw-r--r--   0        0        0     1887 2023-02-07 18:39:47.314339 seaport-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     1710 2023-02-07 18:40:02.709645 seaport-0.8.0/seaport/__init__.py
--rw-r--r--   0        0        0      677 2022-09-22 18:30:57.942372 seaport-0.8.0/seaport/_autocomplete/seaport.bash
--rw-r--r--   0        0        0      674 2022-09-22 18:31:01.181942 seaport-0.8.0/seaport/_autocomplete/seaport.fish
--rw-r--r--   0        0        0      973 2022-09-22 18:31:03.886008 seaport-0.8.0/seaport/_autocomplete/seaport.zsh
--rw-r--r--   0        0        0     4428 2022-09-23 14:07:21.208851 seaport-0.8.0/seaport/_click_functions.py
--rw-r--r--   0        0        0     1626 2022-08-03 17:26:21.770736 seaport-0.8.0/seaport/_clipboard/__init__.py
--rw-r--r--   0        0        0     4780 2022-08-05 10:59:17.960706 seaport-0.8.0/seaport/_clipboard/additional.py
--rw-r--r--   0        0        0     3352 2022-08-05 13:28:24.524585 seaport-0.8.0/seaport/_clipboard/checks.py
--rw-r--r--   0        0        0     6080 2023-02-07 18:11:51.487995 seaport-0.8.0/seaport/_clipboard/clipboard.py
--rw-r--r--   0        0        0     2174 2022-08-03 17:26:21.770905 seaport-0.8.0/seaport/_clipboard/format.py
--rw-r--r--   0        0        0     1622 2022-08-03 17:26:21.770304 seaport-0.8.0/seaport/_clipboard/portfile/__init__.py
--rw-r--r--   0        0        0     5651 2022-08-03 17:26:21.770520 seaport-0.8.0/seaport/_clipboard/portfile/checksums.py
--rw-r--r--   0        0        0     6174 2022-09-22 17:40:30.543073 seaport-0.8.0/seaport/_clipboard/portfile/portfile_numbers.py
--rw-r--r--   0        0        0     3597 2022-08-03 17:26:21.767942 seaport-0.8.0/seaport/_clipboard/user.py
--rw-r--r--   0        0        0     2225 2022-08-03 17:26:21.771386 seaport-0.8.0/seaport/_init.py
--rw-r--r--   0        0        0     1635 2022-08-03 17:26:21.771779 seaport-0.8.0/seaport/_pull_request/__init__.py
--rw-r--r--   0        0        0     3400 2022-08-03 17:26:21.772139 seaport-0.8.0/seaport/_pull_request/clone.py
--rw-r--r--   0        0        0     2683 2022-08-03 17:26:21.771975 seaport-0.8.0/seaport/_pull_request/portfile.py
--rw-r--r--   0        0        0     7322 2022-08-06 14:46:13.991368 seaport-0.8.0/seaport/_pull_request/pull_request.py
--rw-r--r--   0        0        0    11111 2022-08-05 18:04:46.741300 seaport-0.8.0/seaport/portfile.py
--rw-r--r--   0        0        0     1606 2022-08-03 17:26:21.772818 seaport-0.8.0/seaport/py.typed
--rw-r--r--   0        0        0     6325 1970-01-01 00:00:00.000000 seaport-0.8.0/setup.py
--rw-r--r--   0        0        0     6414 1970-01-01 00:00:00.000000 seaport-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1498 2023-02-11 13:51:14.217693 seaport-0.9.0/LICENSE
+-rw-r--r--   0        0        0     5265 2023-02-07 18:34:29.437125 seaport-0.9.0/README.rst
+-rw-r--r--   0        0        0     1954 2023-02-12 11:20:44.255818 seaport-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     1710 2023-02-12 11:20:44.242386 seaport-0.9.0/seaport/__init__.py
+-rw-r--r--   0        0        0      677 2022-09-22 18:30:57.942372 seaport-0.9.0/seaport/_autocomplete/seaport.bash
+-rw-r--r--   0        0        0      674 2022-09-22 18:31:01.181942 seaport-0.9.0/seaport/_autocomplete/seaport.fish
+-rw-r--r--   0        0        0      973 2022-09-22 18:31:03.886008 seaport-0.9.0/seaport/_autocomplete/seaport.zsh
+-rw-r--r--   0        0        0     4428 2023-02-11 13:51:14.217007 seaport-0.9.0/seaport/_click_functions.py
+-rw-r--r--   0        0        0     1626 2023-02-11 13:51:14.213237 seaport-0.9.0/seaport/_clipboard/__init__.py
+-rw-r--r--   0        0        0     4780 2023-02-11 13:51:14.211141 seaport-0.9.0/seaport/_clipboard/additional.py
+-rw-r--r--   0        0        0     3352 2023-02-11 13:51:14.210476 seaport-0.9.0/seaport/_clipboard/checks.py
+-rw-r--r--   0        0        0     5828 2023-02-11 13:51:14.213796 seaport-0.9.0/seaport/_clipboard/clipboard.py
+-rw-r--r--   0        0        0     2174 2023-02-11 13:51:14.213449 seaport-0.9.0/seaport/_clipboard/format.py
+-rw-r--r--   0        0        0     1622 2023-02-11 13:51:14.212418 seaport-0.9.0/seaport/_clipboard/portfile/__init__.py
+-rw-r--r--   0        0        0     5705 2023-02-11 13:51:14.212963 seaport-0.9.0/seaport/_clipboard/portfile/checksums.py
+-rw-r--r--   0        0        0     6243 2023-02-11 16:34:42.701680 seaport-0.9.0/seaport/_clipboard/portfile/portfile_numbers.py
+-rw-r--r--   0        0        0     3880 2023-02-11 13:51:14.209885 seaport-0.9.0/seaport/_clipboard/user.py
+-rw-r--r--   0        0        0     2225 2023-02-11 13:51:14.214171 seaport-0.9.0/seaport/_init.py
+-rw-r--r--   0        0        0     1635 2023-02-11 13:51:14.215243 seaport-0.9.0/seaport/_pull_request/__init__.py
+-rw-r--r--   0        0        0     3400 2023-02-11 13:51:14.215774 seaport-0.9.0/seaport/_pull_request/clone.py
+-rw-r--r--   0        0        0     2683 2023-02-11 13:51:14.215534 seaport-0.9.0/seaport/_pull_request/portfile.py
+-rw-r--r--   0        0        0     7322 2023-02-11 13:51:14.214696 seaport-0.9.0/seaport/_pull_request/pull_request.py
+-rw-r--r--   0        0        0    11695 2023-02-11 16:38:52.068251 seaport-0.9.0/seaport/portfile.py
+-rw-r--r--   0        0        0     1606 2023-02-11 13:51:14.216777 seaport-0.9.0/seaport/py.typed
+-rw-r--r--   0        0        0     6446 1970-01-01 00:00:00.000000 seaport-0.9.0/setup.py
+-rw-r--r--   0        0        0     6487 1970-01-01 00:00:00.000000 seaport-0.9.0/PKG-INFO
```

### Comparing `seaport-0.8.0/LICENSE` & `seaport-0.9.0/LICENSE`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2022, harens
+Copyright (c) 2023, harens
 
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without modification,
 are permitted provided that the following conditions are met:
 
     * Redistributions of source code must retain the above copyright notice,
```

### Comparing `seaport-0.8.0/README.rst` & `seaport-0.9.0/README.rst`

 * *Files identical despite different names*

### Comparing `seaport-0.8.0/pyproject.toml` & `seaport-0.9.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "seaport"
-version = "0.8.0"
+version = "0.9.0"
 description = "The modern MacPorts portfile updater"
 authors = ["harens <harensdeveloper@gmail.com>"]
 maintainers = ["harens <harensdeveloper@gmail.com>"]
 readme = "README.rst"
 license = "BSD-3-Clause"
 include = ["seaport/py.typed"]
 keywords = ["MacPorts", "Port", "Bump", "Checksums"]
@@ -22,19 +22,20 @@
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/harens/seaport/issues"
 
 [tool.poetry.dependencies]
 python = ">=3.7,<4.0"
 click = "^8.1.3"
 beartype = "^0.12.0"
+typing-extensions = { version = ">=4.0.0, <5.0", python = "<3.9" }
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.2.1"
 black = "^23.1.0"
-isort = "5.11.4"
+isort = "5.11.5"
 mypy = "^1.0.0"
 pytest-subprocess = "^1.5.0"
 pytest-mock = "^3.10.0"
 pytest-cov = "^4.0.0"
 coverage = "^7.1.0"
 pydocstyle = "^6.3.0"
 pre-commit = "2.21.0"
@@ -63,18 +64,18 @@
 [tool.pylint.messages_control]
 disable = "C0330, C0326"
 
 [tool.pylint.format]
 max-line-length = "88"
 
 [tool.black]
-target-version = ["py38"]
+target-version = ["py37"]
 
 [tool.commitizen]
-version = "0.7.1"
+version = "0.9.0"
 tag_format = "v$version"
 version_files = [
   "pyproject.toml:version",
   "seaport/__init__.py",
 ]
 
 [build-system]
```

### Comparing `seaport-0.8.0/seaport/__init__.py` & `seaport-0.9.0/seaport/_clipboard/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-# Copyright (c) 2022, harens
+# Copyright (c) 2023, harens
 #
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without modification,
 # are permitted provided that the following conditions are met:
 #
 #     * Redistributions of source code must retain the above copyright notice,
@@ -24,14 +24,8 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR
 # PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-"""The modern MacPorts portfile updater.
-
-Find out more at https://seaport.rtfd.io/
-"""
-
-__version__ = "0.8.0"
-__all__ = ["portfile"]
+"""Functions related to commands/clipboard.py."""
```

### Comparing `seaport-0.8.0/seaport/_autocomplete/seaport.bash` & `seaport-0.9.0/seaport/_autocomplete/seaport.bash`

 * *Files identical despite different names*

### Comparing `seaport-0.8.0/seaport/_autocomplete/seaport.fish` & `seaport-0.9.0/seaport/_autocomplete/seaport.fish`

 * *Files identical despite different names*

### Comparing `seaport-0.8.0/seaport/_autocomplete/seaport.zsh` & `seaport-0.9.0/seaport/_autocomplete/seaport.zsh`

 * *Files identical despite different names*

### Comparing `seaport-0.8.0/seaport/_click_functions.py` & `seaport-0.9.0/seaport/_click_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-# Copyright (c) 2022, harens
+# Copyright (c) 2023, harens
 #
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without modification,
 # are permitted provided that the following conditions are met:
 #
 #     * Redistributions of source code must retain the above copyright notice,
```

### Comparing `seaport-0.8.0/seaport/_clipboard/__init__.py` & `seaport-0.9.0/seaport/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-# Copyright (c) 2022, harens
+# Copyright (c) 2023, harens
 #
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without modification,
 # are permitted provided that the following conditions are met:
 #
 #     * Redistributions of source code must retain the above copyright notice,
@@ -24,8 +24,14 @@
 # EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO,
 # PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR
 # PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
-"""Functions related to commands/clipboard.py."""
+"""The modern MacPorts portfile updater.
+
+Find out more at https://seaport.rtfd.io/
+"""
+
+__version__ = "0.9.0"
+__all__ = ["portfile"]
```

### Comparing `seaport-0.8.0/seaport/_clipboard/additional.py` & `seaport-0.9.0/seaport/_clipboard/additional.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-# Copyright (c) 2022, harens
+# Copyright (c) 2023, harens
 #
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without modification,
 # are permitted provided that the following conditions are met:
 #
 #     * Redistributions of source code must retain the above copyright notice,
```

### Comparing `seaport-0.8.0/seaport/_clipboard/checks.py` & `seaport-0.9.0/seaport/_clipboard/checks.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-# Copyright (c) 2022, harens
+# Copyright (c) 2023, harens
 #
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without modification,
 # are permitted provided that the following conditions are met:
 #
 #     * Redistributions of source code must retain the above copyright notice,
```

### Comparing `seaport-0.8.0/seaport/_clipboard/clipboard.py` & `seaport-0.9.0/seaport/_clipboard/clipboard.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-# Copyright (c) 2022, harens
+# Copyright (c) 2023, harens
 #
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without modification,
 # are permitted provided that the following conditions are met:
 #
 #     * Redistributions of source code must retain the above copyright notice,
@@ -64,30 +64,21 @@
     location: Optional[str] = None,
     new: bool = False,
 ) -> None:
     """Bumps the version number and checksum of NAME.
 
     It then copies the result to your clipboard.
     """
-    # Tasks that require sudo
-    sudo = test or lint or install or write
+    # Tasks that definitely require sudo
+    sudo = test or install
 
     port = Port(name)
 
     old_checks = port.checksums()
 
-    if not port._index():
-        # Likely something's gone wrong with port --index info
-        # Probably lots of writing to portfiles
-        click.secho(
-            f"😬 `port --index info {port.name}` doesn't match `port info {port.name}`",
-            fg="yellow",
-        )
-        click.echo("🐌 Going into slow but careful mode...")
-
     # Determine new version
     bump = new_version(port, bump)
 
     click.secho(f"👍 New version is {bump}", fg="green")
 
     # Allows pr function to get the version number and category
     # new_version checks if bump is none and deals with it there
@@ -121,52 +112,56 @@
 
     new_contents = replace_checksums(
         original,
         (old_checks[0], old_checks[1], old_checks[2], port.version),
         (new_rmd160, new_sha256, new_size, bump),
     )
 
-    if sudo:
+    if sudo or write or lint:
         # Temporary files created to get around sudo write problem
         tmp_version = tempfile.NamedTemporaryFile(mode="w")
         tmp_version.write(new_contents)
         tmp_version.seek(0)
 
-        click.secho("💾 Editing local portfile repo, sudo required", fg="cyan")
+        click.secho("💾 Editing local portfile repo", fg="cyan")
         if not write:
             # Changes only reverted if the user doesn't use the --write flag
-            click.echo("Changes will be reverted after completion")
+            click.secho("📝 Changes will be reverted after completion", fg="cyan")
+
         subprocess.run(
-            [f"{user_path()}/sudo", "cp", tmp_version.name, file_location], check=True
+            ([] if os.access(file_location, os.W_OK) else [f"{user_path()}/sudo"])
+            + ["cp", tmp_version.name, file_location],
+            check=True,
         )
 
         if write:
             click.secho(
                 "📝 The portfile's contents have been updated",
                 fg="cyan",
             )
 
+        if lint:
+            # If the lint is not successful
+            if not perform_lint(name):
+                clean(original, file_location, name)
+                sys.exit(1)
+
         if test:
             subport = port.subports()
             if subport is not None:
                 result = perform_test(name, subport[-1])
             else:
                 result = perform_test(name)
             # If the tests fail
             if not result:
                 clean(original, file_location, name)
                 sys.exit(1)
-        if lint:
-            # If the lint is not successful
-            if not perform_lint(name):
-                clean(original, file_location, name)
-                sys.exit(1)
 
         if install:
             perform_install(name)
 
-        clean(original, file_location, name, write)
+        clean(original, file_location, name, write, sudo)
 
     # Clipboard functions at the very end
     # to reduce the chance of user's clipboard being changed
     # after adding contents
     user_clipboard(new_contents)
```

### Comparing `seaport-0.8.0/seaport/_clipboard/format.py` & `seaport-0.9.0/seaport/_clipboard/format.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-# Copyright (c) 2022, harens
+# Copyright (c) 2023, harens
 #
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without modification,
 # are permitted provided that the following conditions are met:
 #
 #     * Redistributions of source code must retain the above copyright notice,
```

### Comparing `seaport-0.8.0/seaport/_clipboard/portfile/__init__.py` & `seaport-0.9.0/seaport/_clipboard/portfile/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-# Copyright (c) 2022, harens
+# Copyright (c) 2023, harens
 #
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without modification,
 # are permitted provided that the following conditions are met:
 #
 #     * Redistributions of source code must retain the above copyright notice,
```

### Comparing `seaport-0.8.0/seaport/_clipboard/portfile/checksums.py` & `seaport-0.9.0/seaport/_clipboard/portfile/checksums.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-# Copyright (c) 2022, harens
+# Copyright (c) 2023, harens
 #
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without modification,
 # are permitted provided that the following conditions are met:
 #
 #     * Redistributions of source code must retain the above copyright notice,
@@ -26,31 +26,39 @@
 # PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 """Functions related to determining the current and new checksums."""
 
+import hashlib
 import shutil
 import sys
 import tempfile
 import urllib.request
 from pathlib import Path
 
 import click
 from beartype import beartype
 from beartype.typing import Tuple
+from beartype.vale import Is
 
-from seaport._clipboard.checks import user_path
-from seaport._clipboard.format import format_subprocess
 from seaport._clipboard.portfile.portfile_numbers import undo_revision
 
+# Don't count code coverage since different python versions
+# won't run different parts of code
+if sys.version_info >= (3, 9):  # pragma: no cover
+    from typing import Annotated
+else:  # pragma: no cover
+    from typing_extensions import Annotated
 
-@beartype
-def new_checksums(website: str) -> Tuple[str, str, str]:
+
+def new_checksums(
+    website: Annotated[str, Is[lambda text: text[:4] == "http"]]
+) -> Tuple[str, str, str]:
     """Generate checksums of file downloaded from website.
 
     Args:
         website: Where to download the new file from
 
     Examples:
         >>> from seaport._clipboard.portfile.checksums import new_checksums
@@ -61,15 +69,16 @@
         ...     new_checksums("I_don't_exist_and_so_will_fail")
         ... except SystemExit:
         ...     pass
         🔻 Downloading from I_don't_exist_and_so_will_fail
         Couldn't determine the new url. Modify the url above and use the --url flag to set it manually
 
     Returns:
-        Tuple[str, str, str]: A tuple of strings representing the new checksums
+        Tuple[str, str, str]: A tuple of strings representing the new checksums in the order sha256,
+            rmd160 and size.
     """
     download_dir = tempfile.TemporaryDirectory()
     download_location = f"{download_dir.name}/download"
 
     # Download the file from `url` and save it locally under `file_name`:
     # Originally urllib.request.urlretrieve(website, download_location), but this is depreciated
     # Credit https://stackoverflow.com/a/7244263
@@ -82,25 +91,21 @@
     except (urllib.error.HTTPError, urllib.error.URLError, ValueError):
         click.secho(
             "Couldn't determine the new url. Modify the url above and use the --url flag to set it manually",
             fg="red",
         )
         sys.exit(1)
 
-    # sha256 flag added even though it's the default
-    # Otherwise sometimes doesn't return sha256
-    # TODO: Repalce the subprocess with native python functions
-    sha256 = format_subprocess(
-        [f"{user_path()}/openssl", "dgst", "-sha256", download_location]
-    ).split(" ")[-1]
-    rmd160 = format_subprocess(
-        [f"{user_path()}/openssl", "dgst", "-rmd160", download_location]
-    ).split(" ")[-1]
     size = str(Path(download_location).stat().st_size)
 
+    with open(download_location, "rb") as file:
+        data = file.read()
+        sha256 = hashlib.sha256(data).hexdigest()
+        rmd160 = hashlib.new("ripemd160", data).hexdigest()
+
     download_dir.cleanup()
 
     return sha256, rmd160, size
 
 
 @beartype
 def replace_checksums(
```

### Comparing `seaport-0.8.0/seaport/_clipboard/portfile/portfile_numbers.py` & `seaport-0.9.0/seaport/_clipboard/portfile/portfile_numbers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-# Copyright (c) 2022, harens
+# Copyright (c) 2023, harens
 #
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without modification,
 # are permitted provided that the following conditions are met:
 #
 #     * Redistributions of source code must retain the above copyright notice,
@@ -128,15 +128,16 @@
         str: Either the latest version number or the user's custom one.
 
     """
     # TODO: This will need some serious refactoring at some point
     # If it's a new port, essentially ignore version checks
     # Returns the current version from the portfile
     if new:
-        return port.version
+        # N.B. str seems to be required for py3.7 type checking
+        return str(port.version)
 
     # Determines new version number if none manually specified
     if stated is None:  # None used rather than "is not" to make mypy happy
         stated = port.livecheck()
 
     if stated == port.version:
         click.secho(
```

### Comparing `seaport-0.8.0/seaport/_clipboard/user.py` & `seaport-0.9.0/seaport/_clipboard/user.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-# Copyright (c) 2022, harens
+# Copyright (c) 2023, harens
 #
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without modification,
 # are permitted provided that the following conditions are met:
 #
 #     * Redistributions of source code must retain the above copyright notice,
@@ -26,53 +26,68 @@
 # PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF
 # LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 """Functions for modifying the user's system, such as the _clipboard."""
 
+import os
 import subprocess
 import tempfile
 
 import click
 from beartype import beartype
 
 from seaport._clipboard.checks import user_path
 
 
 @beartype
 def clean(
-    original_text: str, location: str, port_name: str, write: bool = False
+    original_text: str,
+    location: str,
+    port_name: str,
+    write: bool = False,
+    sudo: bool = False,
 ) -> None:
     """Returns the user's local portfile repo to the original state.
 
     Args:
         original_text: What the contents of the portfile originally was
         location: Where the portfile is located
         port_name: The name of the portfile
         write: Whether to keep the updated portfile contents
+        sudo: Whether any testing or building was done.
 
     """
     click.secho("🧽 Cleanup", fg="cyan")
 
     # Only revert the portfile contents if the user doesn't use --write
     if not write:
         # Change contents of local portfile back to original
         tmp_original = tempfile.NamedTemporaryFile(mode="w")
         tmp_original.write(original_text)
         tmp_original.seek(0)
         subprocess.run(
-            [f"{user_path()}/sudo", "cp", tmp_original.name, location], check=True
+            ([] if os.access(location, os.W_OK) else [f"{user_path()}/sudo"])
+            + ["cp", tmp_original.name, location],
+            check=True,
         )
         tmp_original.close()
 
-    subprocess.run(
-        [f"{user_path()}/sudo", f"{user_path(True)}/port", "clean", "--all", port_name],
-        check=True,
-    )
+    if sudo:
+        subprocess.run(
+            [
+                f"{user_path()}/sudo",
+                f"{user_path(True)}/port",
+                "clean",
+                "--all",
+                port_name,
+            ],
+            check=True,
+        )
 
 
 @beartype
 def user_clipboard(new_contents: str) -> None:
     """Copies the new contents of the portfile to the _clipboard.
 
     Examples:
@@ -84,15 +99,15 @@
         'hello there'
 
     Args:
         new_contents: What to copy the clipboard
     """
     subprocess.run(
         f"{user_path()}/pbcopy",
-        universal_newlines=True,
+        text=True,
         input=new_contents,
         check=True,
     )
 
     click.secho(
         "📋 The contents of the portfile have been copied to your clipboard!",
         fg="cyan",
```

### Comparing `seaport-0.8.0/seaport/_init.py` & `seaport-0.9.0/seaport/_init.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-# Copyright (c) 2022, harens
+# Copyright (c) 2023, harens
 #
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without modification,
 # are permitted provided that the following conditions are met:
 #
 #     * Redistributions of source code must retain the above copyright notice,
```

### Comparing `seaport-0.8.0/seaport/_pull_request/__init__.py` & `seaport-0.9.0/seaport/_pull_request/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-# Copyright (c) 2022, harens
+# Copyright (c) 2023, harens
 #
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without modification,
 # are permitted provided that the following conditions are met:
 #
 #     * Redistributions of source code must retain the above copyright notice,
```

### Comparing `seaport-0.8.0/seaport/_pull_request/clone.py` & `seaport-0.9.0/seaport/_pull_request/clone.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-# Copyright (c) 2022, harens
+# Copyright (c) 2023, harens
 #
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without modification,
 # are permitted provided that the following conditions are met:
 #
 #     * Redistributions of source code must retain the above copyright notice,
```

### Comparing `seaport-0.8.0/seaport/_pull_request/portfile.py` & `seaport-0.9.0/seaport/_pull_request/portfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-# Copyright (c) 2022, harens
+# Copyright (c) 2023, harens
 #
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without modification,
 # are permitted provided that the following conditions are met:
 #
 #     * Redistributions of source code must retain the above copyright notice,
```

### Comparing `seaport-0.8.0/seaport/_pull_request/pull_request.py` & `seaport-0.9.0/seaport/_pull_request/pull_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-# Copyright (c) 2022, harens
+# Copyright (c) 2023, harens
 #
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without modification,
 # are permitted provided that the following conditions are met:
 #
 #     * Redistributions of source code must retain the above copyright notice,
```

### Comparing `seaport-0.8.0/seaport/portfile.py` & `seaport-0.9.0/seaport/portfile.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python3
 
-# Copyright (c) 2022, harens
+# Copyright (c) 2023, harens
 #
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without modification,
 # are permitted provided that the following conditions are met:
 #
 #     * Redistributions of source code must retain the above copyright notice,
@@ -28,124 +28,125 @@
 # NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS
 # SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
 
 """Python API for MacPorts portfiles."""
 
 import re
 import subprocess
+import sys
 from typing import Optional
 
 from beartype import beartype
 from beartype.typing import List, Tuple
 
 from seaport._clipboard.format import format_subprocess
 
-# TODO: Set no output (especially for errors)
+# Don't count code coverage since different python versions
+# won't run different parts of code
+if sys.version_info >= (3, 8):  # pragma: no cover
+    from beartype.typing import Final
+else:  # pragma: no cover
+    from typing_extensions import Final
 
 
+# TODO: Set no output (especially for errors)
 class Port:
     """Scrapes portfile info for usage in Python modules.
 
     Examples:
         >>> from seaport.portfile import Port
         >>> port = Port("py-base91")
         >>> port.version
         '1.0.1'
 
         >>> from seaport.portfile import Port
+        >>> port = Port("py-base91")
+        >>> port.revision
+        0
+
+        >>> from seaport.portfile import Port
         >>> try:
         ...     port = Port("non-existent-port")
         ... except Exception:
         ...     pass
         >>> # This raises an exception
 
     Attributes:
         name (str): The name of the port e.g. gping
     """
 
-    # This makes mypy and pytype happy
-    # See https://google.github.io/pytype/errors.html#attribute-error
-    name: str
-    version: str
-
     @beartype
     def __init__(self, name: str) -> None:
         """Set optional attributes and check if port exists."""
         # TODO: Figure out how to find path without subprocess
         # TODO: Refactor this
         # TODO: This also kind of defeats the purpose of that bandit error, so find a better way to determine the path
         # no forward slash at end for Bandit B607
-        self.name = name
-        self._path = format_subprocess(["/usr/bin/which", "port"]).replace("/port", "")
+        self.name: Final[str] = name
+        self._path: Final[str] = format_subprocess(["/usr/bin/which", "port"]).replace(
+            "/port", ""
+        )
 
-        # TODO: We're calling port info twice (here and in _index()). Maybe find a way to only do it once.
         try:
-            if self._index():
-                # Caches port info for later
-                # --index provides big speed boost, but doesn't always work
-                self._info = format_subprocess(
-                    [f"{self._path}/port", "info", "--index", self.name]
-                )
-            else:
-                self._info = format_subprocess(
-                    [f"{self._path}/port", "info", self.name]
-                )
+            self._info: Final[str] = format_subprocess(
+                [f"{self._path}/port", "info", self.name]
+            )
         except subprocess.CalledProcessError:
             # TODO: Set a more specific exception
             raise Exception(f"{self.name} doesn't exist, run portindex if port is new")
 
-        self.version = self.__current()
+        self._parsedInfo: Final[List[str]] = self._info[
+            self._info.find("@") + 1 :
+        ].split()
+        versionParse: Final[List[str]] = self._parsedInfo[0].split("_")
 
-    @beartype
-    def _index(self) -> bool:
-        """Whether to use the --index flag with port or not.
+        # Parse saved port info, falling back to calling the explicit function
+        # As a quick sanity check, see that the first digit of the version number is indeed a digit
 
-        --index provides a speed boost, but can be wrong if the port has been edited recently.
-        """
-        return format_subprocess(
-            [f"{self._path}/port", "info", self.name]
-        ) == format_subprocess([f"{self._path}/port", "info", "--index", self.name])
+        self.version: Final[str] = (
+            format_subprocess(
+                [f"{self._path}/port", "info", "--version", self.name]
+            ).split(" ")[1]
+            if len(versionParse) not in (1, 2) or not versionParse[0][0].isdigit()
+            else versionParse[0]
+        )
+
+        self.revision: Final[int] = (
+            int(
+                format_subprocess(
+                    [f"{self._path}/port", "info", "--revision", self.name]
+                ).split(" ")[1]
+            )
+            if len(versionParse) not in (1, 2) or not versionParse[0][0].isdigit()
+            else 0
+            if len(versionParse) == 1
+            else int(versionParse[1])
+        )
 
     @beartype
     def __str__(self) -> str:
         """Outputs the name and version of the port.
 
         Examples:
             >>> from seaport.portfile import Port
             >>> print(Port("py-base91"))
             py-base91 1.0.1
         """
         return f"{self.name} {self.version}"
 
     @beartype
-    def __len__(self) -> int:
-        """Returns the size of the downloaded file.
+    def __repr__(self) -> str:
+        """Outputs the attributes that a port was defined with.
 
         Examples:
             >>> from seaport.portfile import Port
-            >>> len(Port("py-base91"))
-            2331
+            >>> Port("py-base91")
+            Port(name=py-base91)
         """
-        return int(self.checksums()[2])
-
-    @beartype
-    def __current(self) -> str:
-        """Determines the current version of the portfile."""
-        # TODO: Uses self._info to determine current version (since it's already saved)
-        # Be careful of revision numbers e.g. 1.2.3_1
-        # Credit to https://stackoverflow.com/a/29836831/10763533
-        # return self._info[self._info.find("@") + 1 :].split()[0]
-        if self._index():
-            return format_subprocess(
-                [f"{self._path}/port", "info", "--version", "--index", self.name]
-            ).split(" ")[1]
-        else:
-            return format_subprocess(
-                [f"{self._path}/port", "info", "--version", self.name]
-            ).split(" ")[1]
+        return f"Port(name={self.name})"
 
     # TODO: These livecheck tests will fail when I least expect it
     @beartype
     def livecheck(self) -> str:
         """Runs port livecheck to check for any new versions.
 
         If no livecheck is available or the portfile is already the latest version, the current version is outputted.
@@ -169,23 +170,25 @@
         update = format_subprocess(
             [f"{self._path}/port", "livecheck", self.name]
         ).split(" ")[-1][:-1]
 
         # If there's no livecheck output, fallback to subport
         # Convoluted if statement to make mypy happy
         if update == "":
+            # Makes mypy happy since a function could theoretically change to be None
             subports = self.subports()
             if subports is not None:
                 update = format_subprocess(
                     [f"{self._path}/port", "livecheck", subports[-1]]
                 ).split(" ")[-1][:-1]
 
         # If there's no livecheck output again, fallback to current version
         # Implies no livecheck available or already up-to-date
-        return update if update != "" else self.version
+        # N.B. str is required for py 3.7 type checking
+        return update if update != "" else str(self.version)
 
     @beartype
     def subports(self) -> Optional[List[str]]:
         """Determines a list of subports of a port.
 
         If there are no subports available, None is outputted.
 
@@ -201,25 +204,31 @@
             >>> port = Port("folderify")
             >>> print(port.subports())
             None
 
         Returns:
             A list representing all the subports of the port.
         """
-        if "Sub-ports" not in self._info:
-            return None
-
         # Split subport section by colon and comma
         # This needs to be made more efficient
-        subport_list = re.split(
-            "[:,]", " ".join([s for s in self._info.splitlines() if "Sub-ports" in s])
+        # TODO: Refactor so that as soon as a line containing sub-ports is found, don't bother
+        # with other iterations in for list comprehension
+        return (
+            None
+            if "Sub-ports" not in self._info
+            else [
+                i.replace(" ", "")
+                for i in re.split(
+                    "[:,]",
+                    " ".join([s for s in self._info.splitlines() if "Sub-ports" in s]),
+                )
+                if i != "Sub-ports"
+            ]
         )
 
-        return [i.replace(" ", "") for i in subport_list if i != "Sub-ports"]
-
     @beartype
     def checksums(self, _name: Optional[str] = None) -> Tuple[str, str, str, str]:
         """Determines the current checksums of a portfile.
 
         For python ports, their pyXY- subport is used to determine the checksums.
         Note that this method only works for ports with the standard rmd/sha/size setup (not the older format), and it can also be
         quite slow since it's scraping `port distfiles NAME`
@@ -241,25 +250,27 @@
             format_subprocess([f"{self._path}/port", "distfiles", _name])
             .replace("\n ", "")
             .split(" ")
         )
         try:
             # We're only interested in the first result
             # Credit to https://stackoverflow.com/a/9868665/10763533
-            website = next(s for s in distfiles if "http://" in s or "https://" in s)
+            website: Final[str] = next(
+                s for s in distfiles if "http://" in s or "https://" in s
+            )
         except StopIteration:
             # Tries to determine the subport
             # This is since the distfiles cmd only works for subports
             subports = self.subports()
             if subports is None:
                 raise Exception(f"port distfiles {_name} provides no output")
             # Repeat the process with the subport
             return self.checksums(subports[-1])
 
-        website_index = distfiles.index(website)
+        website_index: Final[int] = distfiles.index(website)
 
         # rmd, sha, size, download website
         # TODO: This will not work for the old format
         return (
             distfiles[website_index - 3][:-7],
             distfiles[website_index - 2][:-5],
             distfiles[website_index - 1],
@@ -277,17 +288,25 @@
             >>> port = Port("gping")
             >>> port.primary_category()
             'net'
 
         Returns:
             The category of the port e.g. sysutils.
         """
-        if self._index():
-            category_list = format_subprocess(
-                [f"{self._path}/port", "info", "--index", "--category", self.name]
-            ).split(" ")
-        else:
-            category_list = format_subprocess(
+        # Remove leftmost bracket and rightmost comma (if multiple categories) or bracket (if only one)
+        if self._parsedInfo[1][0] != "(" or self._parsedInfo[1][-1] not in (
+            ")",
+            ",",
+        ):
+            category_list: Final[List[str]] = format_subprocess(
                 [f"{self._path}/port", "info", "--category", self.name]
             ).split(" ")
-        # Remove comma, and only take the first category
-        return category_list[1][:-1] if len(category_list) > 2 else category_list[1]
+            # Remove comma, and only take the first category
+            # N.B. str seems to be required for py37 type checking
+            return (
+                str(category_list[1][:-1])
+                if len(category_list) > 2
+                else str(category_list[1])
+            )
+        else:
+            # N.B. str is required for python type checking
+            return str(self._parsedInfo[1][1:-1])
```

### Comparing `seaport-0.8.0/seaport/py.typed` & `seaport-0.9.0/seaport/py.typed`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright (c) 2022, harens
+# Copyright (c) 2023, harens
 #
 # All rights reserved.
 #
 # Redistribution and use in source and binary forms, with or without modification,
 # are permitted provided that the following conditions are met:
 #
 #     * Redistributions of source code must retain the above copyright notice,
```

### Comparing `seaport-0.8.0/setup.py` & `seaport-0.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,29 +9,33 @@
 
 package_data = \
 {'': ['*'], 'seaport': ['_autocomplete/*']}
 
 install_requires = \
 ['beartype>=0.12.0,<0.13.0', 'click>=8.1.3,<9.0.0']
 
+extras_require = \
+{':python_version < "3.9"': ['typing-extensions>=4.0.0,<5.0']}
+
 entry_points = \
 {'console_scripts': ['seaport = seaport._init:seaport']}
 
 setup_kwargs = {
     'name': 'seaport',
-    'version': '0.8.0',
+    'version': '0.9.0',
     'description': 'The modern MacPorts portfile updater',
     'long_description': '🌊 seaport\n==========\n\n|ci-badge| |rtd-badge| |cov-badge|\n\nThe modern `MacPorts <https://www.macports.org>`_ portfile updater.\n\n.. code-block::\n\n    > seaport clip gping\n    🌊 Starting seaport...\n    👍 New version is 1.2.0-post\n    🔻 Downloading from https://github.com/orf/gping/tarball/v1.2.0-post/gping-1.2.0-post.tar.gz\n    🔎 Checksums:\n    Old rmd160: 8b274132c8389ec560f213007368c7f521fdf682\n    New rmd160: 4a614e35d4e1e496871ee2b270ba8836f84650c6\n    Old sha256: 1879b37f811c09e43d3759ccd97d9c8b432f06c75a27025cfa09404abdeda8f5\n    New sha256: 1008306e8293e7c59125de02e2baa6a17bc1c10de1daba2247bfc789eaf34ff5\n    Old size: 853432\n    New size: 853450\n    ⏪️ Changing revision numbers\n    No changes necessary\n    📋 The contents of the portfile have been copied to your clipboard!\n\nInstallation\n------------\n\nMacPorts 🍎\n************\n\n.. code-block::\n\n    sudo port install seaport\n\nPyPi 🐍\n********\n\n.. code-block::\n\n    pip3 install seaport\n    # Optionally, install GitHub CLI to send PRs\n    sudo port install gh\n\n⚡️ Features\n--------------\n\n🖥 `Command Line Tool <https://seaport.readthedocs.io/en/stable/overview.html>`_\n*********************************************************************************\n\n* ⏩ **Automatically determines new version numbers and checksums** for MacPorts portfiles.\n* 📋 **Copies the changes to your clipboard**, and optionally **sends a PR to update them**.\n* 🔎 Contains **additional checking functionality**, such as running tests, linting and installing the updated program.\n\n🐍 `Python API <https://seaport.readthedocs.io/en/stable/reference.html>`_\n****************************************************************************\n\n* 📚 Library for convenient access to portfile information. Easily import as a Python module for your project.\n* ⌨️ `PEP 561 compatible <https://www.python.org/dev/peps/pep-0561>`_, with built in support for type checking.\n*  📦 Works out of the box with all `supported Python versions <https://endoflife.date/python>`_ (3.7-3.11).\n\nTo find out more, please read the `Documentation <https://seaport.rtfd.io/>`_.\n\n🤔 How to use seaport\n----------------------\n\nFor simple ports with straightforward updates, use :code:`seaport pr example_port`.\nThis sends a PR with the updated portfile and automatically fills in the PR template for you.\n\nFor ports that require some manual changes, use :code:`seaport clip example_port`.\nThis updates the version number and checksums so you don\'t have to. 😎\n\nBe sure to check out the `flags overview <https://seaport.readthedocs.io/en/stable/overview.html>`_ for information on additional features.\n\n🔥 seaport vs port bump\n-------------------------\n\n.. list-table::\n   :widths: 25 25 25\n   :header-rows: 1\n\n   * - Features\n     - 🌊 seaport\n     - 🛼 port bump\n   * - 🔒 Updates checksums\n     - ✅\n     - ✅\n   * - 📚 Updates the revision number\n     - ✅\n     - ✅\n   * - 📝 Can write changes to the original file\n     - ✅\n     - ✅\n   * - ⏮ Can update portfile to a specific version\n     - ✅\n     - ✅\n   * - 🔮 Updates the version number via livecheck\n     - ✅\n     - ❌\n   * - 🚀 Can send a pull request (both for updated and new ports)\n     - ✅\n     - ❌\n   * - 🧪 Can lint/test/install the port to check if the update works\n     - ✅\n     - ❌\n   * - 📋 Copies changes to clipboard\n     - ✅\n     - ❌\n   * - 🌎 Can both manually and automatically set the url to download from\n     - ✅\n     - ❌\n\n🔨 Contributing\n---------------\n\n- Issue Tracker: `<https://github.com/harens/seaport/issues>`_\n- Source Code: `<https://github.com/harens/seaport>`_\n\nAny change, big or small, that you think can help improve this project is more than welcome 🎉.\n\nAs well as this, feel free to open an issue with any new suggestions or bug reports. Every contribution is appreciated.\n\nFor more information, please read our `contributing page <https://seaport.readthedocs.io/en/latest/contributing.html>`_ on how to get started.\n\n©️ License\n----------\n\nSimilar to other MacPorts-based projects, seaport is licensed under the `BSD 3-Clause "New" or "Revised" License <https://github.com/harens/seaport/blob/master/LICENSE>`_.\n\n📒 Notice of Non-Affiliation and Disclaimer\n-------------------------------------------\n\nThis project is not affiliated, associated, authorized, endorsed by, or in any way officially connected with the MacPorts Project, or any of its subsidiaries or its affiliates. The official MacPorts Project website can be found at `<https://www.macports.org>`_.\n\nThe name MacPorts as well as related names, marks, emblems and images are registered trademarks of their respective owners.\n\n.. |ci-badge| image:: https://img.shields.io/github/actions/workflow/status/harens/seaport/test.yml?logo=github&style=flat-square\n   :target: https://github.com/harens/seaport/actions\n   :alt: GitHub Workflow Status\n.. |rtd-badge| image:: https://img.shields.io/readthedocs/seaport?logo=read%20the%20docs&style=flat-square\n   :target: https://seaport.rtfd.io/\n   :alt: Read the Docs\n.. |cov-badge| image:: https://img.shields.io/codecov/c/github/harens/seaport?logo=codecov&style=flat-square\n   :target: https://codecov.io/gh/harens/seaport\n   :alt: Codecov\n',
     'author': 'harens',
     'author_email': 'harensdeveloper@gmail.com',
     'maintainer': 'harens',
     'maintainer_email': 'harensdeveloper@gmail.com',
     'url': 'https://seaport.rtfd.io/',
     'packages': packages,
     'package_data': package_data,
     'install_requires': install_requires,
+    'extras_require': extras_require,
     'entry_points': entry_points,
     'python_requires': '>=3.7,<4.0',
 }
 
 
 setup(**setup_kwargs)
```

### Comparing `seaport-0.8.0/PKG-INFO` & `seaport-0.9.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seaport
-Version: 0.8.0
+Version: 0.9.0
 Summary: The modern MacPorts portfile updater
 Home-page: https://seaport.rtfd.io/
 License: BSD-3-Clause
 Keywords: MacPorts,Port,Bump,Checksums
 Author: harens
 Author-email: harensdeveloper@gmail.com
 Maintainer: harens
@@ -19,14 +19,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Requires-Dist: beartype (>=0.12.0,<0.13.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
+Requires-Dist: typing-extensions (>=4.0.0,<5.0) ; python_version < "3.9"
 Project-URL: Bug Tracker, https://github.com/harens/seaport/issues
 Project-URL: Documentation, https://seaport.rtfd.io/
 Project-URL: Repository, https://github.com/harens/seaport
 Description-Content-Type: text/x-rst
 
 🌊 seaport
 ==========
```

