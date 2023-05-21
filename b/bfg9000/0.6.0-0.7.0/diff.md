# Comparing `tmp/bfg9000-0.6.0.tar.gz` & `tmp/bfg9000-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bfg9000-0.6.0.tar", last modified: Sat Sep 12 18:54:00 2020, max compression
+gzip compressed data, was "bfg9000-0.7.0.tar", last modified: Sun May 21 01:43:10 2023, max compression
```

## Comparing `bfg9000-0.6.0.tar` & `bfg9000-0.7.0.tar`

### file list

```diff
@@ -1,130 +1,135 @@
-drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2020-09-12 18:54:00.737176 bfg9000-0.6.0/
--rw-rw-r--   0 jim       (1000) jim       (1000)       17 2020-08-05 21:44:42.000000 bfg9000-0.6.0/MANIFEST.in
--rw-rw-r--   0 jim       (1000) jim       (1000)     3766 2020-09-12 18:54:00.737176 bfg9000-0.6.0/PKG-INFO
--rw-rw-r--   0 jim       (1000) jim       (1000)     3248 2020-08-05 21:44:42.000000 bfg9000-0.6.0/README.md
-drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2020-09-12 18:54:00.713175 bfg9000-0.6.0/bfg9000/
--rw-rw-r--   0 jim       (1000) jim       (1000)        0 2020-08-05 21:44:42.000000 bfg9000-0.6.0/bfg9000/__init__.py
--rw-rw-r--   0 jim       (1000) jim       (1000)       18 2020-09-12 04:27:04.000000 bfg9000-0.6.0/bfg9000/app_version.py
-drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2020-09-12 18:54:00.717176 bfg9000-0.6.0/bfg9000/arguments/
--rw-rw-r--   0 jim       (1000) jim       (1000)        0 2020-08-05 21:44:42.000000 bfg9000-0.6.0/bfg9000/arguments/__init__.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     3476 2020-09-07 06:23:31.000000 bfg9000-0.6.0/bfg9000/arguments/parser.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     6542 2020-08-05 21:44:42.000000 bfg9000-0.6.0/bfg9000/arguments/windows.py
-drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2020-09-12 18:54:00.717176 bfg9000-0.6.0/bfg9000/backends/
--rw-rw-r--   0 jim       (1000) jim       (1000)      963 2020-08-05 21:44:42.000000 bfg9000-0.6.0/bfg9000/backends/__init__.py
-drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2020-09-12 18:54:00.717176 bfg9000-0.6.0/bfg9000/backends/make/
--rw-rw-r--   0 jim       (1000) jim       (1000)        0 2020-08-05 21:44:42.000000 bfg9000-0.6.0/bfg9000/backends/make/__init__.py
--rw-rw-r--   0 jim       (1000) jim       (1000)    14282 2020-09-07 06:23:31.000000 bfg9000-0.6.0/bfg9000/backends/make/syntax.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     3159 2020-09-10 21:05:53.000000 bfg9000-0.6.0/bfg9000/backends/make/writer.py
-drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2020-09-12 18:54:00.717176 bfg9000-0.6.0/bfg9000/backends/msbuild/
--rw-rw-r--   0 jim       (1000) jim       (1000)        0 2020-08-05 21:44:42.000000 bfg9000-0.6.0/bfg9000/backends/msbuild/__init__.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     5970 2020-09-07 06:23:31.000000 bfg9000-0.6.0/bfg9000/backends/msbuild/solution.py
--rw-rw-r--   0 jim       (1000) jim       (1000)    13467 2020-09-07 06:23:31.000000 bfg9000-0.6.0/bfg9000/backends/msbuild/syntax.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     1513 2020-09-10 21:05:53.000000 bfg9000-0.6.0/bfg9000/backends/msbuild/writer.py
-drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2020-09-12 18:54:00.721176 bfg9000-0.6.0/bfg9000/backends/ninja/
--rw-rw-r--   0 jim       (1000) jim       (1000)        0 2020-08-05 21:44:42.000000 bfg9000-0.6.0/bfg9000/backends/ninja/__init__.py
--rw-rw-r--   0 jim       (1000) jim       (1000)    11493 2020-09-07 06:23:31.000000 bfg9000-0.6.0/bfg9000/backends/ninja/syntax.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     2752 2020-09-10 21:05:53.000000 bfg9000-0.6.0/bfg9000/backends/ninja/writer.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     3363 2020-09-10 21:05:53.000000 bfg9000-0.6.0/bfg9000/build.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     2568 2020-09-07 06:23:31.000000 bfg9000-0.6.0/bfg9000/build_inputs.py
-drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2020-09-12 18:54:00.725175 bfg9000-0.6.0/bfg9000/builtins/
--rw-rw-r--   0 jim       (1000) jim       (1000)      270 2020-08-05 21:44:42.000000 bfg9000-0.6.0/bfg9000/builtins/__init__.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     1220 2020-08-05 21:44:42.000000 bfg9000-0.6.0/bfg9000/builtins/alias.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     6615 2020-08-05 21:45:09.000000 bfg9000-0.6.0/bfg9000/builtins/builtin.py
--rw-rw-r--   0 jim       (1000) jim       (1000)      250 2020-09-10 21:05:53.000000 bfg9000-0.6.0/bfg9000/builtins/clean.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     6751 2020-09-07 06:23:31.000000 bfg9000-0.6.0/bfg9000/builtins/command.py
--rw-rw-r--   0 jim       (1000) jim       (1000)    16319 2020-09-07 06:23:31.000000 bfg9000-0.6.0/bfg9000/builtins/compile.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     4919 2020-09-07 06:23:31.000000 bfg9000-0.6.0/bfg9000/builtins/copy_file.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     1097 2020-08-05 21:44:42.000000 bfg9000-0.6.0/bfg9000/builtins/core.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     2203 2020-09-07 06:23:31.000000 bfg9000-0.6.0/bfg9000/builtins/default.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     1713 2020-08-05 21:44:42.000000 bfg9000-0.6.0/bfg9000/builtins/dist.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     5903 2020-09-07 06:23:31.000000 bfg9000-0.6.0/bfg9000/builtins/file_types.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     7877 2020-09-07 06:23:31.000000 bfg9000-0.6.0/bfg9000/builtins/find.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     7068 2020-09-10 21:05:53.000000 bfg9000-0.6.0/bfg9000/builtins/install.py
--rw-rw-r--   0 jim       (1000) jim       (1000)    24124 2020-09-07 06:23:31.000000 bfg9000-0.6.0/bfg9000/builtins/link.py
--rw-rw-r--   0 jim       (1000) jim       (1000)      277 2020-08-05 21:44:42.000000 bfg9000-0.6.0/bfg9000/builtins/opts.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     5220 2020-09-10 21:05:53.000000 bfg9000-0.6.0/bfg9000/builtins/packages.py
--rw-rw-r--   0 jim       (1000) jim       (1000)      993 2020-09-07 06:23:31.000000 bfg9000-0.6.0/bfg9000/builtins/path.py
--rw-rw-r--   0 jim       (1000) jim       (1000)    18884 2020-09-07 06:23:31.000000 bfg9000-0.6.0/bfg9000/builtins/pkg_config.py
--rw-rw-r--   0 jim       (1000) jim       (1000)      988 2020-09-07 06:23:31.000000 bfg9000-0.6.0/bfg9000/builtins/project.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     1340 2020-09-10 21:05:53.000000 bfg9000-0.6.0/bfg9000/builtins/regenerate.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     4228 2020-09-07 06:23:31.000000 bfg9000-0.6.0/bfg9000/builtins/tests.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     3619 2020-09-07 06:23:31.000000 bfg9000-0.6.0/bfg9000/builtins/toolchain.py
--rw-rw-r--   0 jim       (1000) jim       (1000)      306 2020-08-05 21:44:42.000000 bfg9000-0.6.0/bfg9000/builtins/user_arguments.py
--rw-rw-r--   0 jim       (1000) jim       (1000)      791 2020-09-07 06:23:31.000000 bfg9000-0.6.0/bfg9000/builtins/version.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     3891 2020-08-05 21:44:42.000000 bfg9000-0.6.0/bfg9000/depfixer.py
--rw-rw-r--   0 jim       (1000) jim       (1000)    12697 2020-09-10 21:05:53.000000 bfg9000-0.6.0/bfg9000/driver.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     2524 2020-08-05 21:44:42.000000 bfg9000-0.6.0/bfg9000/e1m1.py
--rw-rw-r--   0 jim       (1000) jim       (1000)    10357 2020-09-10 21:05:53.000000 bfg9000-0.6.0/bfg9000/environment.py
--rw-rw-r--   0 jim       (1000) jim       (1000)      275 2020-09-07 06:23:31.000000 bfg9000-0.6.0/bfg9000/exceptions.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     9347 2020-09-07 06:23:31.000000 bfg9000-0.6.0/bfg9000/file_types.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     7131 2020-09-07 06:23:31.000000 bfg9000-0.6.0/bfg9000/glob.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     5643 2020-09-07 06:23:31.000000 bfg9000-0.6.0/bfg9000/iterutils.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     2154 2020-08-05 21:44:42.000000 bfg9000-0.6.0/bfg9000/jvmoutput.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     4685 2020-09-07 06:23:31.000000 bfg9000-0.6.0/bfg9000/languages.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     6080 2020-09-07 06:23:31.000000 bfg9000-0.6.0/bfg9000/log.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     1554 2020-08-05 21:45:09.000000 bfg9000-0.6.0/bfg9000/objutils.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     7845 2020-09-10 21:05:53.000000 bfg9000-0.6.0/bfg9000/options.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     1701 2020-09-10 21:05:53.000000 bfg9000-0.6.0/bfg9000/packages.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     2583 2020-09-07 06:23:31.000000 bfg9000-0.6.0/bfg9000/path.py
-drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2020-09-12 18:54:00.729175 bfg9000-0.6.0/bfg9000/platforms/
--rw-rw-r--   0 jim       (1000) jim       (1000)       63 2020-08-05 21:44:42.000000 bfg9000-0.6.0/bfg9000/platforms/__init__.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     9080 2020-09-07 06:23:31.000000 bfg9000-0.6.0/bfg9000/platforms/basepath.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     4552 2020-09-07 06:23:31.000000 bfg9000-0.6.0/bfg9000/platforms/core.py
--rw-rw-r--   0 jim       (1000) jim       (1000)      648 2020-09-07 06:23:31.000000 bfg9000-0.6.0/bfg9000/platforms/cygwin.py
--rw-rw-r--   0 jim       (1000) jim       (1000)      529 2020-09-10 21:05:53.000000 bfg9000-0.6.0/bfg9000/platforms/framework.py
--rw-rw-r--   0 jim       (1000) jim       (1000)      334 2020-08-05 21:44:42.000000 bfg9000-0.6.0/bfg9000/platforms/host.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     2871 2020-09-10 21:05:53.000000 bfg9000-0.6.0/bfg9000/platforms/posix.py
--rw-rw-r--   0 jim       (1000) jim       (1000)      442 2020-09-10 21:05:53.000000 bfg9000-0.6.0/bfg9000/platforms/target.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     1943 2020-09-10 21:05:53.000000 bfg9000-0.6.0/bfg9000/platforms/windows.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     1620 2020-09-07 06:23:31.000000 bfg9000-0.6.0/bfg9000/rccdep.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     6917 2020-09-07 21:57:05.000000 bfg9000-0.6.0/bfg9000/safe_str.py
-drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2020-09-12 18:54:00.729175 bfg9000-0.6.0/bfg9000/shell/
--rw-rw-r--   0 jim       (1000) jim       (1000)     3003 2020-09-07 21:57:05.000000 bfg9000-0.6.0/bfg9000/shell/__init__.py
--rw-rw-r--   0 jim       (1000) jim       (1000)      615 2020-08-05 21:44:42.000000 bfg9000-0.6.0/bfg9000/shell/list.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     3508 2020-09-07 06:23:31.000000 bfg9000-0.6.0/bfg9000/shell/posix.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     2345 2020-08-05 21:45:09.000000 bfg9000-0.6.0/bfg9000/shell/syntax.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     4469 2020-09-07 06:23:31.000000 bfg9000-0.6.0/bfg9000/shell/windows.py
-drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2020-09-12 18:54:00.733176 bfg9000-0.6.0/bfg9000/tools/
--rw-rw-r--   0 jim       (1000) jim       (1000)     1339 2020-09-07 06:23:31.000000 bfg9000-0.6.0/bfg9000/tools/__init__.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     2671 2020-09-07 06:23:31.000000 bfg9000-0.6.0/bfg9000/tools/ar.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     4274 2020-09-07 06:23:31.000000 bfg9000-0.6.0/bfg9000/tools/c_family.py
-drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2020-09-12 18:54:00.737176 bfg9000-0.6.0/bfg9000/tools/cc/
--rw-rw-r--   0 jim       (1000) jim       (1000)    10297 2020-09-10 21:05:53.000000 bfg9000-0.6.0/bfg9000/tools/cc/__init__.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     5277 2020-09-07 21:57:05.000000 bfg9000-0.6.0/bfg9000/tools/cc/compiler.py
--rw-rw-r--   0 jim       (1000) jim       (1000)      219 2020-09-07 06:23:31.000000 bfg9000-0.6.0/bfg9000/tools/cc/flags.py
--rw-rw-r--   0 jim       (1000) jim       (1000)    16778 2020-09-07 21:57:05.000000 bfg9000-0.6.0/bfg9000/tools/cc/linker.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     2557 2020-09-07 06:23:31.000000 bfg9000-0.6.0/bfg9000/tools/cc/rc.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     5830 2020-09-10 21:05:53.000000 bfg9000-0.6.0/bfg9000/tools/common.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     1547 2020-08-05 21:44:42.000000 bfg9000-0.6.0/bfg9000/tools/copy_file.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     1323 2020-09-07 06:23:31.000000 bfg9000-0.6.0/bfg9000/tools/doppel.py
--rw-rw-r--   0 jim       (1000) jim       (1000)      530 2020-09-07 06:23:31.000000 bfg9000-0.6.0/bfg9000/tools/fortran.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     1651 2020-09-07 06:23:31.000000 bfg9000-0.6.0/bfg9000/tools/install_name_tool.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     1399 2020-08-05 21:44:42.000000 bfg9000-0.6.0/bfg9000/tools/internal.py
--rw-rw-r--   0 jim       (1000) jim       (1000)      830 2020-09-07 06:23:31.000000 bfg9000-0.6.0/bfg9000/tools/java.py
--rw-rw-r--   0 jim       (1000) jim       (1000)    12536 2020-09-10 21:05:53.000000 bfg9000-0.6.0/bfg9000/tools/jvm.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     1486 2020-08-05 21:44:42.000000 bfg9000-0.6.0/bfg9000/tools/ld.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     3584 2020-09-07 06:23:31.000000 bfg9000-0.6.0/bfg9000/tools/lex.py
--rw-rw-r--   0 jim       (1000) jim       (1000)      406 2020-08-05 21:44:42.000000 bfg9000-0.6.0/bfg9000/tools/mkdir_p.py
-drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2020-09-12 18:54:00.737176 bfg9000-0.6.0/bfg9000/tools/msvc/
--rw-rw-r--   0 jim       (1000) jim       (1000)     6784 2020-09-10 21:05:53.000000 bfg9000-0.6.0/bfg9000/tools/msvc/__init__.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     7289 2020-09-07 21:57:05.000000 bfg9000-0.6.0/bfg9000/tools/msvc/compiler.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     8599 2020-09-07 21:57:05.000000 bfg9000-0.6.0/bfg9000/tools/msvc/linker.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     3116 2020-09-07 06:23:31.000000 bfg9000-0.6.0/bfg9000/tools/msvc/rc.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     2282 2020-09-07 06:23:31.000000 bfg9000-0.6.0/bfg9000/tools/patchelf.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     7145 2020-09-10 21:05:53.000000 bfg9000-0.6.0/bfg9000/tools/pkg_config.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     7220 2020-09-07 06:23:31.000000 bfg9000-0.6.0/bfg9000/tools/qt.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     1946 2020-09-07 06:23:31.000000 bfg9000-0.6.0/bfg9000/tools/rc.py
--rw-rw-r--   0 jim       (1000) jim       (1000)      455 2020-08-05 21:44:42.000000 bfg9000-0.6.0/bfg9000/tools/rm.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     1408 2020-08-05 21:44:42.000000 bfg9000-0.6.0/bfg9000/tools/scripts.py
--rw-rw-r--   0 jim       (1000) jim       (1000)      807 2020-08-05 21:44:42.000000 bfg9000-0.6.0/bfg9000/tools/setenv.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     4056 2020-09-07 06:23:31.000000 bfg9000-0.6.0/bfg9000/tools/yacc.py
--rw-rw-r--   0 jim       (1000) jim       (1000)     3310 2020-08-05 21:44:42.000000 bfg9000-0.6.0/bfg9000/versioning.py
-drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2020-09-12 18:54:00.717176 bfg9000-0.6.0/bfg9000.egg-info/
--rw-rw-r--   0 jim       (1000) jim       (1000)     3766 2020-09-12 18:54:00.000000 bfg9000-0.6.0/bfg9000.egg-info/PKG-INFO
--rw-rw-r--   0 jim       (1000) jim       (1000)     2943 2020-09-12 18:54:00.000000 bfg9000-0.6.0/bfg9000.egg-info/SOURCES.txt
--rw-rw-r--   0 jim       (1000) jim       (1000)        1 2020-09-12 18:54:00.000000 bfg9000-0.6.0/bfg9000.egg-info/dependency_links.txt
--rw-rw-r--   0 jim       (1000) jim       (1000)     1152 2020-09-12 18:54:00.000000 bfg9000-0.6.0/bfg9000.egg-info/entry_points.txt
--rw-rw-r--   0 jim       (1000) jim       (1000)      273 2020-09-12 18:54:00.000000 bfg9000-0.6.0/bfg9000.egg-info/requires.txt
--rw-rw-r--   0 jim       (1000) jim       (1000)        8 2020-09-12 18:54:00.000000 bfg9000-0.6.0/bfg9000.egg-info/top_level.txt
--rw-rw-r--   0 jim       (1000) jim       (1000)      171 2020-09-12 18:54:00.737176 bfg9000-0.6.0/setup.cfg
--rw-rw-r--   0 jim       (1000) jim       (1000)     6743 2020-09-10 21:05:53.000000 bfg9000-0.6.0/setup.py
+drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2023-05-21 01:43:10.962722 bfg9000-0.7.0/
+-rw-rw-r--   0 jim       (1000) jim       (1000)    14313 2023-05-21 01:42:08.000000 bfg9000-0.7.0/CHANGES.md
+-rw-rw-r--   0 jim       (1000) jim       (1000)     1486 2023-01-03 04:51:05.000000 bfg9000-0.7.0/LICENSE
+-rw-rw-r--   0 jim       (1000) jim       (1000)       19 2020-11-10 03:37:38.000000 bfg9000-0.7.0/MANIFEST.in
+-rw-rw-r--   0 jim       (1000) jim       (1000)     4659 2023-05-21 01:43:10.962722 bfg9000-0.7.0/PKG-INFO
+-rw-rw-r--   0 jim       (1000) jim       (1000)     3313 2023-03-25 21:38:18.000000 bfg9000-0.7.0/README.md
+drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2023-05-21 01:43:10.926722 bfg9000-0.7.0/bfg9000/
+-rw-rw-r--   0 jim       (1000) jim       (1000)        0 2020-08-05 21:44:42.000000 bfg9000-0.7.0/bfg9000/__init__.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)       18 2023-05-21 01:41:50.000000 bfg9000-0.7.0/bfg9000/app_version.py
+drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2023-05-21 01:43:10.934722 bfg9000-0.7.0/bfg9000/arguments/
+-rw-rw-r--   0 jim       (1000) jim       (1000)        0 2020-08-05 21:44:42.000000 bfg9000-0.7.0/bfg9000/arguments/__init__.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     4385 2021-09-26 20:58:29.000000 bfg9000-0.7.0/bfg9000/arguments/parser.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     6794 2021-08-04 20:26:41.000000 bfg9000-0.7.0/bfg9000/arguments/windows.py
+drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2023-05-21 01:43:10.934722 bfg9000-0.7.0/bfg9000/backends/
+-rw-rw-r--   0 jim       (1000) jim       (1000)      517 2023-04-02 06:27:55.000000 bfg9000-0.7.0/bfg9000/backends/__init__.py
+drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2023-05-21 01:43:10.934722 bfg9000-0.7.0/bfg9000/backends/compdb/
+-rw-rw-r--   0 jim       (1000) jim       (1000)        0 2021-06-27 05:36:00.000000 bfg9000-0.7.0/bfg9000/backends/compdb/__init__.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     2702 2021-06-14 02:40:53.000000 bfg9000-0.7.0/bfg9000/backends/compdb/writer.py
+drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2023-05-21 01:43:10.934722 bfg9000-0.7.0/bfg9000/backends/make/
+-rw-rw-r--   0 jim       (1000) jim       (1000)        0 2020-08-05 21:44:42.000000 bfg9000-0.7.0/bfg9000/backends/make/__init__.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)    14282 2020-09-07 06:23:31.000000 bfg9000-0.7.0/bfg9000/backends/make/syntax.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     3229 2020-12-31 22:29:46.000000 bfg9000-0.7.0/bfg9000/backends/make/writer.py
+drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2023-05-21 01:43:10.938722 bfg9000-0.7.0/bfg9000/backends/msbuild/
+-rw-rw-r--   0 jim       (1000) jim       (1000)        0 2020-08-05 21:44:42.000000 bfg9000-0.7.0/bfg9000/backends/msbuild/__init__.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     5970 2020-09-07 06:23:31.000000 bfg9000-0.7.0/bfg9000/backends/msbuild/solution.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)    14204 2022-03-02 21:04:35.000000 bfg9000-0.7.0/bfg9000/backends/msbuild/syntax.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     1589 2021-12-31 21:55:46.000000 bfg9000-0.7.0/bfg9000/backends/msbuild/writer.py
+drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2023-05-21 01:43:10.938722 bfg9000-0.7.0/bfg9000/backends/ninja/
+-rw-rw-r--   0 jim       (1000) jim       (1000)        0 2020-08-05 21:44:42.000000 bfg9000-0.7.0/bfg9000/backends/ninja/__init__.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)    11419 2020-11-10 03:37:38.000000 bfg9000-0.7.0/bfg9000/backends/ninja/syntax.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     2822 2020-12-31 22:29:46.000000 bfg9000-0.7.0/bfg9000/backends/ninja/writer.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     4005 2021-12-31 21:55:46.000000 bfg9000-0.7.0/bfg9000/build.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     2568 2020-09-07 06:23:31.000000 bfg9000-0.7.0/bfg9000/build_inputs.py
+drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2023-05-21 01:43:10.946722 bfg9000-0.7.0/bfg9000/builtins/
+-rw-rw-r--   0 jim       (1000) jim       (1000)      270 2020-11-19 04:05:52.000000 bfg9000-0.7.0/bfg9000/builtins/__init__.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     1220 2020-08-05 21:44:42.000000 bfg9000-0.7.0/bfg9000/builtins/alias.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     6615 2020-08-05 21:45:09.000000 bfg9000-0.7.0/bfg9000/builtins/builtin.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)      929 2021-02-17 02:23:34.000000 bfg9000-0.7.0/bfg9000/builtins/clean.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     7218 2021-06-14 02:40:53.000000 bfg9000-0.7.0/bfg9000/builtins/command.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)    17356 2021-07-12 23:57:44.000000 bfg9000-0.7.0/bfg9000/builtins/compile.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     7283 2021-07-12 23:57:44.000000 bfg9000-0.7.0/bfg9000/builtins/copy_file.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     1097 2020-08-05 21:44:42.000000 bfg9000-0.7.0/bfg9000/builtins/core.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     2203 2020-09-07 06:23:31.000000 bfg9000-0.7.0/bfg9000/builtins/default.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     1713 2021-02-17 02:23:34.000000 bfg9000-0.7.0/bfg9000/builtins/dist.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     5421 2021-07-12 04:00:01.000000 bfg9000-0.7.0/bfg9000/builtins/file_types.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     5986 2020-12-02 05:42:02.000000 bfg9000-0.7.0/bfg9000/builtins/find.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     7361 2021-07-12 23:57:44.000000 bfg9000-0.7.0/bfg9000/builtins/install.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)    25468 2021-11-23 05:28:03.000000 bfg9000-0.7.0/bfg9000/builtins/link.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)      277 2020-08-05 21:44:42.000000 bfg9000-0.7.0/bfg9000/builtins/opts.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     2733 2021-09-27 18:18:11.000000 bfg9000-0.7.0/bfg9000/builtins/packages.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)      993 2020-09-07 06:23:31.000000 bfg9000-0.7.0/bfg9000/builtins/path.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)    18909 2022-09-04 21:45:52.000000 bfg9000-0.7.0/bfg9000/builtins/pkg_config.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)      988 2020-09-07 06:23:31.000000 bfg9000-0.7.0/bfg9000/builtins/project.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     2313 2021-02-17 02:23:34.000000 bfg9000-0.7.0/bfg9000/builtins/regenerate.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     4222 2021-11-23 05:28:03.000000 bfg9000-0.7.0/bfg9000/builtins/tests.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     3619 2020-09-07 06:23:31.000000 bfg9000-0.7.0/bfg9000/builtins/toolchain.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)      306 2021-09-26 04:02:06.000000 bfg9000-0.7.0/bfg9000/builtins/user_arguments.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)      791 2020-09-07 06:23:31.000000 bfg9000-0.7.0/bfg9000/builtins/version.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     3891 2020-08-05 21:44:42.000000 bfg9000-0.7.0/bfg9000/depfixer.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)    16828 2023-01-14 04:23:13.000000 bfg9000-0.7.0/bfg9000/driver.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     2524 2020-08-05 21:44:42.000000 bfg9000-0.7.0/bfg9000/e1m1.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)    12905 2021-07-12 23:57:44.000000 bfg9000-0.7.0/bfg9000/environment.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)      318 2020-12-02 05:42:02.000000 bfg9000-0.7.0/bfg9000/exceptions.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     9854 2021-07-12 23:57:44.000000 bfg9000-0.7.0/bfg9000/file_types.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     6999 2020-12-02 05:42:02.000000 bfg9000-0.7.0/bfg9000/glob.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     5778 2021-02-17 02:23:34.000000 bfg9000-0.7.0/bfg9000/iterutils.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     2203 2021-02-17 02:23:34.000000 bfg9000-0.7.0/bfg9000/jvmoutput.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     4685 2020-09-07 06:23:31.000000 bfg9000-0.7.0/bfg9000/languages.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     7120 2021-12-31 21:55:46.000000 bfg9000-0.7.0/bfg9000/log.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     2228 2020-11-21 00:01:55.000000 bfg9000-0.7.0/bfg9000/objutils.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     7750 2021-02-17 02:23:34.000000 bfg9000-0.7.0/bfg9000/options.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     2420 2021-08-04 20:26:41.000000 bfg9000-0.7.0/bfg9000/packages.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     2624 2021-12-31 21:55:46.000000 bfg9000-0.7.0/bfg9000/path.py
+drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2023-05-21 01:43:10.950722 bfg9000-0.7.0/bfg9000/platforms/
+-rw-rw-r--   0 jim       (1000) jim       (1000)       75 2021-12-31 21:55:46.000000 bfg9000-0.7.0/bfg9000/platforms/__init__.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     9111 2022-09-04 21:45:52.000000 bfg9000-0.7.0/bfg9000/platforms/basepath.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     4512 2023-04-02 06:27:55.000000 bfg9000-0.7.0/bfg9000/platforms/core.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)      648 2020-09-07 06:23:31.000000 bfg9000-0.7.0/bfg9000/platforms/cygwin.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)      334 2020-08-05 21:44:42.000000 bfg9000-0.7.0/bfg9000/platforms/host.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     2779 2022-09-03 05:36:28.000000 bfg9000-0.7.0/bfg9000/platforms/posix.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)      340 2021-02-17 02:23:34.000000 bfg9000-0.7.0/bfg9000/platforms/target.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     2039 2022-09-03 05:36:35.000000 bfg9000-0.7.0/bfg9000/platforms/windows.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     1623 2021-11-23 05:28:03.000000 bfg9000-0.7.0/bfg9000/rccdep.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     6917 2020-11-10 03:37:38.000000 bfg9000-0.7.0/bfg9000/safe_str.py
+drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2023-05-21 01:43:10.950722 bfg9000-0.7.0/bfg9000/shell/
+-rw-rw-r--   0 jim       (1000) jim       (1000)     3124 2021-12-31 21:55:46.000000 bfg9000-0.7.0/bfg9000/shell/__init__.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)      615 2020-08-05 21:44:42.000000 bfg9000-0.7.0/bfg9000/shell/list.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     3835 2022-10-31 03:40:08.000000 bfg9000-0.7.0/bfg9000/shell/posix.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     2475 2022-09-04 21:45:52.000000 bfg9000-0.7.0/bfg9000/shell/syntax.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     4838 2022-10-31 03:40:08.000000 bfg9000-0.7.0/bfg9000/shell/windows.py
+drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2023-05-21 01:43:10.958722 bfg9000-0.7.0/bfg9000/tools/
+-rw-rw-r--   0 jim       (1000) jim       (1000)     1339 2020-11-19 04:05:52.000000 bfg9000-0.7.0/bfg9000/tools/__init__.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     2685 2020-11-21 00:01:55.000000 bfg9000-0.7.0/bfg9000/tools/ar.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     4635 2021-01-02 22:53:27.000000 bfg9000-0.7.0/bfg9000/tools/c_family.py
+drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2023-05-21 01:43:10.962722 bfg9000-0.7.0/bfg9000/tools/cc/
+-rw-rw-r--   0 jim       (1000) jim       (1000)     8222 2022-01-22 05:33:55.000000 bfg9000-0.7.0/bfg9000/tools/cc/__init__.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     5370 2021-09-27 18:18:11.000000 bfg9000-0.7.0/bfg9000/tools/cc/compiler.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)      219 2020-09-07 06:23:31.000000 bfg9000-0.7.0/bfg9000/tools/cc/flags.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)    16904 2021-07-12 05:24:44.000000 bfg9000-0.7.0/bfg9000/tools/cc/linker.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     2571 2021-07-12 23:57:44.000000 bfg9000-0.7.0/bfg9000/tools/cc/rc.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     6537 2021-07-12 23:57:44.000000 bfg9000-0.7.0/bfg9000/tools/common.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     1879 2021-07-12 23:57:44.000000 bfg9000-0.7.0/bfg9000/tools/copy_file.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     1452 2021-02-17 02:23:34.000000 bfg9000-0.7.0/bfg9000/tools/doppel.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)      530 2020-09-07 06:23:31.000000 bfg9000-0.7.0/bfg9000/tools/fortran.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     1651 2020-09-07 06:23:31.000000 bfg9000-0.7.0/bfg9000/tools/install_name_tool.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     1829 2021-02-17 02:23:34.000000 bfg9000-0.7.0/bfg9000/tools/internal.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)      822 2021-12-31 21:55:46.000000 bfg9000-0.7.0/bfg9000/tools/java.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)    12771 2021-09-27 18:18:11.000000 bfg9000-0.7.0/bfg9000/tools/jvm.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     1614 2021-07-12 23:57:44.000000 bfg9000-0.7.0/bfg9000/tools/ld.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     3594 2021-07-12 23:57:44.000000 bfg9000-0.7.0/bfg9000/tools/lex.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)      406 2020-08-05 21:44:42.000000 bfg9000-0.7.0/bfg9000/tools/mkdir_p.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     4739 2023-02-18 23:42:47.000000 bfg9000-0.7.0/bfg9000/tools/mopack.py
+drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2023-05-21 01:43:10.962722 bfg9000-0.7.0/bfg9000/tools/msvc/
+-rw-rw-r--   0 jim       (1000) jim       (1000)     5468 2021-12-31 21:55:46.000000 bfg9000-0.7.0/bfg9000/tools/msvc/__init__.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     7289 2020-11-19 04:05:52.000000 bfg9000-0.7.0/bfg9000/tools/msvc/compiler.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     8683 2021-08-04 20:26:41.000000 bfg9000-0.7.0/bfg9000/tools/msvc/linker.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     3125 2021-07-12 23:57:44.000000 bfg9000-0.7.0/bfg9000/tools/msvc/rc.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     2282 2020-09-07 06:23:31.000000 bfg9000-0.7.0/bfg9000/tools/patchelf.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)    10396 2021-12-31 21:55:46.000000 bfg9000-0.7.0/bfg9000/tools/pkg_config.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     7250 2021-07-12 23:57:44.000000 bfg9000-0.7.0/bfg9000/tools/qt.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     1848 2020-12-28 02:52:54.000000 bfg9000-0.7.0/bfg9000/tools/rc.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)      455 2020-08-05 21:44:42.000000 bfg9000-0.7.0/bfg9000/tools/rm.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     1408 2020-08-05 21:44:42.000000 bfg9000-0.7.0/bfg9000/tools/scripts.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)      807 2020-08-05 21:44:42.000000 bfg9000-0.7.0/bfg9000/tools/setenv.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     4065 2021-07-12 23:57:44.000000 bfg9000-0.7.0/bfg9000/tools/yacc.py
+-rw-rw-r--   0 jim       (1000) jim       (1000)     2800 2021-02-17 02:23:34.000000 bfg9000-0.7.0/bfg9000/versioning.py
+drwxrwxr-x   0 jim       (1000) jim       (1000)        0 2023-05-21 01:43:10.930722 bfg9000-0.7.0/bfg9000.egg-info/
+-rw-rw-r--   0 jim       (1000) jim       (1000)     4659 2023-05-21 01:43:10.000000 bfg9000-0.7.0/bfg9000.egg-info/PKG-INFO
+-rw-rw-r--   0 jim       (1000) jim       (1000)     3025 2023-05-21 01:43:10.000000 bfg9000-0.7.0/bfg9000.egg-info/SOURCES.txt
+-rw-rw-r--   0 jim       (1000) jim       (1000)        1 2023-05-21 01:43:10.000000 bfg9000-0.7.0/bfg9000.egg-info/dependency_links.txt
+-rw-rw-r--   0 jim       (1000) jim       (1000)     1152 2023-05-21 01:43:10.000000 bfg9000-0.7.0/bfg9000.egg-info/entry_points.txt
+-rw-rw-r--   0 jim       (1000) jim       (1000)      321 2023-05-21 01:43:10.000000 bfg9000-0.7.0/bfg9000.egg-info/requires.txt
+-rw-rw-r--   0 jim       (1000) jim       (1000)        8 2023-05-21 01:43:10.000000 bfg9000-0.7.0/bfg9000.egg-info/top_level.txt
+-rw-rw-r--   0 jim       (1000) jim       (1000)      487 2023-05-21 01:43:10.962722 bfg9000-0.7.0/setup.cfg
+-rw-rw-r--   0 jim       (1000) jim       (1000)     6838 2023-05-16 03:14:43.000000 bfg9000-0.7.0/setup.py
```

### Comparing `bfg9000-0.6.0/PKG-INFO` & `bfg9000-0.7.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,104 +1,109 @@
 Metadata-Version: 2.1
 Name: bfg9000
-Version: 0.6.0
+Version: 0.7.0
 Summary: A cross-platform build file generator
 Home-page: https://jimporter.github.io/bfg9000/
 Author: Jim Porter
 Author-email: itsjimporter@gmail.com
-License: BSD
-Description: bfg9000 - build file generator
-        ==============================
+License: BSD-3-Clause
+Description: # bfg9000 - build file generator
+        **bfg9000** is a cross-platform *build configuration system* with an emphasis on
+        making it easy to define how to build your software. It converts a Python-based
+        build script into the appropriate files for your underlying build system of
+        choice (Ninja, Make, or MSBuild).
         
-        **bfg9000** is a cross-platform *build configuration system* with an
-        emphasis on making it easy to define how to build your software. It
-        converts a Python-based build script into the appropriate files for your
-        underlying build system of choice (Ninja, Make, or MSBuild).
+        ## Why bfg9000?
         
-        Why bfg9000?
-        ------------
+        #### Familiar syntax
         
-        Familiar syntax
-        ^^^^^^^^^^^^^^^
+        `build.bfg` files are just Python scripts with some new functions added, so you
+        may already know how to write them; and when your build gets complicated, you
+        can rely on the existing Python ecosystem to get you out of trouble.
         
-        ``build.bfg`` files are just Python scripts with some new functions
-        added, so you may already know how to write them; and when your build
-        gets complicated, you can rely on the existing Python ecosystem to get
-        you out of trouble.
+        #### Fast builds
         
-        Fast builds
-        ^^^^^^^^^^^
+        bfg9000 ensures your builds are fast by relying on existing, mature build
+        systems like Make and Ninja to do the heavy lifting of building your software;
+        often, incremental builds don't need to execute bfg9000 at all!
         
-        bfg9000 ensures your builds are fast by relying on existing, mature
-        build systems like Make and Ninja to do the heavy lifting of building
-        your software; often, incremental builds don’t need to execute bfg9000
-        at all!
+        #### Stay sane
         
-        Stay sane
-        ^^^^^^^^^
+        Building your code shouldn't be the hard part of developing your project. Above
+        all else, bfg9000 strives to help you get your build right the *first* time with
+        many helpful [features][features].
         
-        Building your code shouldn’t be the hard part of developing your
-        project. Above all else, bfg9000 strives to help you get your build
-        right the *first* time with many helpful
-        `features <https://jimporter.github.io/bfg9000/latest/user/features>`__.
+        ## A brief example
         
-        A brief example
-        ---------------
+        You can't get much simpler than the simplest `build.bfg` file:
         
-        You can’t get much simpler than the simplest ``build.bfg`` file:
+        ```python
+        executable('simple', files=['simple.cpp'])
+        ```
         
-        .. code:: python
+        To build this executable, we need to create the actual build files and then
+        run them:
         
-           executable('simple', files=['simple.cpp'])
+        ```sh
+        $ cd /path/to/src/
+        $ 9k build/
+        $ cd build/
+        $ ninja
+        ```
         
-        To build this executable, we need to create the actual build files and
-        then run them:
+        From there, you can run your newly-created executable: `./simple`. Hooray!
         
-        .. code:: sh
+        For further examples, please see the [`examples/`][examples] subdirectory.
         
-           $ cd /path/to/src/
-           $ 9k build/
-           $ cd build/
-           $ ninja
+        ## Installation
         
-        From there, you can run your newly-created executable: ``./simple``.
-        Hooray!
+        bfg9000 uses [setuptools][setuptools], so installation is much the same as any
+        other Python package:
         
-        For further examples, please see the
-        ```examples/`` <https://github.com/jimporter/bfg9000/tree/master/examples>`__
-        subdirectory.
+        ```sh
+        $ pip install bfg9000
+        ```
         
-        Installation
-        ------------
+        From there, you can start using bfg to build your software! (If you're using
+        Ubuntu, you can also install bfg9000 from the following PPA:
+        [ppa:jimporter/stable][ppa]). For more information about how to install bfg9000,
+        see the [documentation][getting-started].
         
-        bfg9000 uses `setuptools <https://pythonhosted.org/setuptools/>`__, so
-        installation is much the same as any other Python package:
+        ## License
         
-        .. code:: sh
+        This project is licensed under the [BSD 3-clause license](LICENSE).
         
-           $ pip install bfg9000
+        [pypi-image]: https://img.shields.io/pypi/v/bfg9000.svg
+        [pypi-link]: https://pypi.python.org/pypi/bfg9000
+        [documentation-image]: https://img.shields.io/badge/docs-bfg9000-blue.svg
+        [documentation-link]: https://jimporter.github.io/bfg9000/
+        [gh-actions-image]: https://github.com/jimporter/bfg9000/workflows/build/badge.svg
+        [gh-actions-link]: https://github.com/jimporter/bfg9000/actions?query=branch%3Amaster+workflow%3Abuild
+        [appveyor-image]: https://ci.appveyor.com/api/projects/status/hxvbggf6exq8i2k6/branch/master?svg=true
+        [appveyor-link]: https://ci.appveyor.com/project/jimporter/bfg9000/branch/master
+        [codecov-image]: https://codecov.io/gh/jimporter/bfg9000/branch/master/graph/badge.svg
+        [codecov-link]: https://codecov.io/gh/jimporter/bfg9000
         
-        From there, you can start using bfg to build your software! (If you’re
-        using Ubuntu, you can also install bfg9000 from the following PPA:
-        `ppa:jimporter/stable <https://launchpad.net/~jimporter/+archive/ubuntu/stable>`__).
-        For more information about how to install bfg9000, see the
-        `documentation <https://jimporter.github.io/bfg9000/latest/getting-started>`__.
-        
-        License
-        -------
-        
-        This project is licensed under the `BSD 3-clause license <LICENSE>`__.
+        [features]: https://jimporter.github.io/bfg9000/latest/user/features
+        [examples]: https://github.com/jimporter/bfg9000/tree/master/examples
+        [setuptools]: https://pythonhosted.org/setuptools/
+        [ppa]: https://launchpad.net/~jimporter/+archive/ubuntu/stable
+        [getting-started]: https://jimporter.github.io/bfg9000/latest/getting-started
         
 Keywords: build file generator
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: msbuild
 Provides-Extra: test
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `bfg9000-0.6.0/README.md` & `bfg9000-0.7.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # bfg9000 - build file generator
 
 [![PyPi version][pypi-image]][pypi-link]
 [![Documentation][documentation-image]][documentation-link]
-[![Travis build status][travis-image]][travis-link]
+[![Github build status][gh-actions-image]][gh-actions-link]
 [![Appveyor build status][appveyor-image]][appveyor-link]
 [![Coverage status][codecov-image]][codecov-link]
 
 **bfg9000** is a cross-platform *build configuration system* with an emphasis on
 making it easy to define how to build your software. It converts a Python-based
 build script into the appropriate files for your underlying build system of
 choice (Ninja, Make, or MSBuild).
@@ -71,16 +71,16 @@
 
 This project is licensed under the [BSD 3-clause license](LICENSE).
 
 [pypi-image]: https://img.shields.io/pypi/v/bfg9000.svg
 [pypi-link]: https://pypi.python.org/pypi/bfg9000
 [documentation-image]: https://img.shields.io/badge/docs-bfg9000-blue.svg
 [documentation-link]: https://jimporter.github.io/bfg9000/
-[travis-image]: https://travis-ci.org/jimporter/bfg9000.svg?branch=master
-[travis-link]: https://travis-ci.org/jimporter/bfg9000
+[gh-actions-image]: https://github.com/jimporter/bfg9000/workflows/build/badge.svg
+[gh-actions-link]: https://github.com/jimporter/bfg9000/actions?query=branch%3Amaster+workflow%3Abuild
 [appveyor-image]: https://ci.appveyor.com/api/projects/status/hxvbggf6exq8i2k6/branch/master?svg=true
 [appveyor-link]: https://ci.appveyor.com/project/jimporter/bfg9000/branch/master
 [codecov-image]: https://codecov.io/gh/jimporter/bfg9000/branch/master/graph/badge.svg
 [codecov-link]: https://codecov.io/gh/jimporter/bfg9000
 
 [features]: https://jimporter.github.io/bfg9000/latest/user/features
 [examples]: https://github.com/jimporter/bfg9000/tree/master/examples
```

### Comparing `bfg9000-0.6.0/bfg9000/arguments/parser.py` & `bfg9000-0.7.0/bfg9000/arguments/parser.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,29 +1,49 @@
 import re as _re
 from argparse import *
 
 from .. import path as _path
 
 _ArgumentParser = ArgumentParser
+_Action = Action
+
+
+# Add some simple wrappers to make it easier to specify shell-completion
+# behaviors.
+
+def _add_complete(argument, complete):
+    if complete is not None:
+        argument.complete = complete
+    elif isinstance(argument.type, File):
+        argument.complete = 'file'
+    elif isinstance(argument.type, Directory):
+        argument.complete = 'directory'
+    return argument
+
+
+class Action(_Action):
+    def __init__(self, *args, complete=None, **kwargs):
+        super().__init__(*args, **kwargs)
+        _add_complete(self, complete)
 
 
 class ToggleAction(Action):
     def __init__(self, option_strings, dest, default=False, required=False,
-                 help=None):
+                 complete=None, help=None):
         if len(option_strings) == 0:
             raise ValueError('option string must begin with "--"')
 
         self.true_strings = [self._prefix(i, self._true_prefix)
                              for i in option_strings]
         self.false_strings = [self._prefix(i, self._false_prefix)
                               for i in option_strings]
 
         option_strings = self.true_strings + self.false_strings
         super().__init__(option_strings, dest=dest, nargs=0, default=default,
-                         required=required, help=help)
+                         required=required, complete=complete, help=help)
 
     def __call__(self, parser, namespace, values, option_string=None):
         value = option_string in self.true_strings
         setattr(namespace, self.dest, value)
 
     @staticmethod
     def _prefix(s, prefix):
@@ -38,30 +58,14 @@
 
 
 class WithAction(ToggleAction):
     _true_prefix = 'with-'
     _false_prefix = 'without-'
 
 
-class ArgumentParser(_ArgumentParser):
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self.register('action', 'enable', EnableAction)
-        self.register('action', 'with', WithAction)
-
-    def _get_option_tuples(self, option_string):
-        # Don't try to check prefixes for long options; this is similar to
-        # Python 3.5's `allow_abbrev=False`, except this doesn't break combined
-        # short options. See <https://bugs.python.org/issue26967>.
-        if option_string[:2] == self.prefix_chars * 2:
-            return []
-
-        return super()._get_option_tuples(option_string)
-
-
 class BaseFile:
     def __init__(self, must_exist=False):
         self.must_exist = must_exist
 
     def __call__(self, string):
         p = self._abspath(string)
         if _path.exists(p):
@@ -94,14 +98,39 @@
         return _path.abspath(p, directory=False, absdrive=False)
 
     @staticmethod
     def _check_type(p):
         return _path.isfile(p)
 
 
+class ArgumentParser(_ArgumentParser):
+    @staticmethod
+    def _wrap_complete(action):
+        def wrapper(*args, complete=None, **kwargs):
+            return _add_complete(action(*args, **kwargs), complete)
+
+        return wrapper
+
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        for k, v in self._registries['action'].items():
+            self._registries['action'][k] = self._wrap_complete(v)
+        self.register('action', 'enable', EnableAction)
+        self.register('action', 'with', WithAction)
+
+    def _get_option_tuples(self, option_string):
+        # Don't try to check prefixes for long options; this is similar to
+        # Python 3.5's `allow_abbrev=False`, except this doesn't break combined
+        # short options. See <https://bugs.python.org/issue26967>.
+        if option_string[:2] == self.prefix_chars * 2:
+            return []
+
+        return super()._get_option_tuples(option_string)
+
+
 # It'd be nice to just have a UserArgumentParser class with this method but it
 # wouldn't propagate to argument groups, so it's easier to just do it this way.
 def add_user_argument(parser, *names, **kwargs):
     if any(not i.startswith('--') for i in names):
         raise ValueError('option string must begin with "--"')
     if any(i.startswith('--x-') for i in names):
         raise ValueError('"x-" prefix is reserved')
```

### Comparing `bfg9000-0.6.0/bfg9000/arguments/windows.py` & `bfg9000-0.7.0/bfg9000/arguments/windows.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,22 +2,27 @@
 # arguments formatted for Visual Studio tools. It's used to parse user
 # arguments so they can be correctly inserted into MSBuild files.
 
 
 class ArgumentParser:
     _argument_info = {}
 
-    def __init__(self, prefix_chars='/-', value_delim=':'):
+    def __init__(self, prefix_chars='/-', value_delim=':',
+                 case_sensitive=True):
         self.prefix_chars = prefix_chars
         self.value_delim = value_delim
+        self.case_sensitive = case_sensitive
         self._options = []
         self._short_names = {}
         self._long_names = {}
         self._unnamed_dest = None
 
+    def _normcase(self, s):
+        return s if self.case_sensitive else s.lower()
+
     @classmethod
     def handler(cls, type):
         def wrapper(thing):
             cls._argument_info[type] = thing
             return thing
         return wrapper
 
@@ -33,14 +38,16 @@
                 if i in self._short_names:
                     raise ValueError('{!r} already defined'.format(i))
                 self._short_names[i] = info
             else:
                 if i[:2] in self._short_names:
                     raise ValueError('{!r} collides with {!r}'
                                      .format(i, i[:2]))
+
+                i = self._normcase(i)
                 if i in self._long_names:
                     raise ValueError('{!r} already defined'.format(i))
                 self._long_names[i] = info
 
         self._options.append(info)
         return info
 
@@ -70,14 +77,15 @@
                                 value = next(args)
                             except StopIteration:
                                 raise ValueError('expected value for option')
                     elif value:
                         raise ValueError('no value expected for option')
                 else:
                     key, colon, value = i.partition(self.value_delim)
+                    key = self._normcase(key)
                     if key in self._long_names:
                         info = self._long_names[key]
                         if not info.takes_value and colon:
                             raise ValueError('no value expected for option')
                         elif info.takes_value and not value:
                             raise ValueError('expected value for option')
             elif self._unnamed_dest:
```

### Comparing `bfg9000-0.6.0/bfg9000/backends/make/syntax.py` & `bfg9000-0.7.0/bfg9000/backends/make/syntax.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.6.0/bfg9000/backends/make/writer.py` & `bfg9000-0.7.0/bfg9000/backends/make/writer.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,19 +3,23 @@
 
 from ... import file_types, path, shell
 from .syntax import *
 from ...iterutils import listify, uniques
 from ...versioning import Version
 
 
+def executable(env=os.environ):
+    return shell.which(env.get('MAKE', ['make', 'gmake']), env)
+
+
 def version(env=os.environ):
     try:
-        make = shell.which(env.get('MAKE', ['make', 'gmake']), env)
+        make = executable(env)
         output = shell.execute(make + ['--version'], stdout=shell.Mode.pipe,
-                               stderr=shell.Mode.devnull)
+                               stderr=shell.Mode.devnull, env=env)
         m = re.match(r'GNU Make ([\d\.]+)', output)
         if m:
             return Version(m.group(1))
     except (IOError, OSError, shell.CalledProcessError):
         pass
     return None
```

### Comparing `bfg9000-0.6.0/bfg9000/backends/msbuild/solution.py` & `bfg9000-0.7.0/bfg9000/backends/msbuild/solution.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.6.0/bfg9000/backends/msbuild/syntax.py` & `bfg9000-0.7.0/bfg9000/backends/msbuild/syntax.py`

 * *Files 2% similar despite different names*

```diff
@@ -177,17 +177,23 @@
         self.mode = mode
         self.output_file = output_file
         self.files = files or []
         self.objs = objs or []
         self.compile_options = compile_options or {}
         self.link_options = link_options or {}
 
-        version = env.getvar('VCTOOLSVERSION', self.version)
+        version = env.getvar(
+            'VSCMD_ARG_VCVARS_VER',
+            env.getvar('VCTOOLSVERSION', self.version)
+        )
         self.toolset = 'v' + version.replace('.', '')[0:3]
 
+        self.windows_sdk = (env.getvar('WINDOWSSDKVERSION', '')
+                               .replace('\\', '') or None)
+
         # As above, VS 2017 remaps x86 to Win32 for C++ projects.
         if self.real_platform == 'x86':
             self.real_platform = 'Win32'
 
     def write(self, out):
         target_name = safe_str.safe_str(self.output_file).basename()
         override_props = E.PropertyGroup(
@@ -200,27 +206,33 @@
         link_opts = E.Lib() if self.mode == 'StaticLibrary' else E.Link()
         self._link_options(link_opts, self.link_options)
         sources, resources = partition(lambda i: i['name'].lang != 'rc',
                                        self.files)
 
         self._write(out, [
             E.Import(Project=r'$(VCTargetsPath)\Microsoft.Cpp.Default.props'),
-            E.PropertyGroup({'Label': 'Configuration'},
-                E.ConfigurationType(self.mode),
-                E.PlatformToolset(self.toolset)
-            ),
+            self._configuration(),
             E.Import(Project=r'$(VCTargetsPath)\Microsoft.Cpp.props'),
             override_props,
             E.ItemDefinitionGroup(compile_opts, link_opts),
             self._compiles(sources, self._cl_compile),
             self._compiles(resources, self._resource_compile),
             self._links(self.objs),
             E.Import(Project=r'$(VCTargetsPath)\Microsoft.Cpp.targets')
         ])
 
+    def _configuration(self):
+        config = E.PropertyGroup({'Label': 'Configuration'},
+            E.ConfigurationType(self.mode),
+            E.PlatformToolset(self.toolset)
+        )
+        if self.windows_sdk:
+            config.append(E.WindowsTargetPlatformVersion(self.windows_sdk))
+        return config
+
     def _compiles(self, files, func):
         def basename(path):
             return path.stripext().basename()
 
         if not files:
             return None
 
@@ -303,32 +315,38 @@
 
         self._add_bool_option(element, 'GenerateDebugInformation',
                               options.get('debug'))
 
         if options.get('import_lib'):
             element.append(E.ImportLibrary( textify(options['import_lib']) ))
 
+        self._add_list_option(element, 'AdditionalLibraryDirectories',
+                              options.get('libdirs'))
         self._add_list_option(element, 'AdditionalOptions',
                               options.get('extra'), quoted=True)
+        # We already include all the default Win32 libraries from the linker,
+        # so don't inherit from the MSBuild default here.
         self._add_list_option(element, 'AdditionalDependencies',
-                              options.get('libs'))
+                              options.get('libs'), inherit=False)
 
     def _add_bool_option(self, element, name, value):
         if value is not None:
             element.append(E(name, 'true' if value else 'false'))
 
     def _add_mapped_option(self, element, name, value, mapping):
         if value is not None:
             element.append(E(name, mapping[value]))
 
-    def _add_list_option(self, element, name, value, *, quoted=False):
+    def _add_list_option(self, element, name, value, *, quoted=False,
+                         inherit=True):
         if value:
             delim = ' ' if quoted else ';'
             element.append(E(name, delim.join(chain(
-                textify_each(value), ['%({})'.format(name)]
+                textify_each(value, quoted),
+                ['%({})'.format(name)] if inherit else []
             )) ))
 
 
 class NoopProject(Project):
     def write(self, out):
         self._write(out, [E.Target(Name='Build')])
```

### Comparing `bfg9000-0.6.0/bfg9000/backends/msbuild/writer.py` & `bfg9000-0.7.0/bfg9000/backends/msbuild/writer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 import os
 import re
 
 from ... import path
 from ... import shell
 from .solution import Solution, UuidMap
-from .syntax import *  # noqa
+from .syntax import *  # noqa: F401
 from ...versioning import Version
 
 
+def executable(env=os.environ):
+    return shell.which(env.get('MSBUILD', ['msbuild', 'xbuild']), env)
+
+
 def version(env=os.environ):
     try:
-        msbuild = shell.which(env.get('MSBUILD', ['msbuild', 'xbuild']), env)
+        msbuild = executable(env)
         output = shell.execute(msbuild + ['/version'], stdout=shell.Mode.pipe,
-                               stderr=shell.Mode.devnull)
+                               stderr=shell.Mode.devnull, env=env)
         m = re.search(r'([\d\.]+)$', output)
         if m:
             return Version(m.group(1))
     except (IOError, OSError, shell.CalledProcessError):
         pass
     return None
```

### Comparing `bfg9000-0.6.0/bfg9000/backends/ninja/syntax.py` & `bfg9000-0.7.0/bfg9000/backends/ninja/syntax.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,18 +36,16 @@
         self.shell = shell
 
     @staticmethod
     def escape_str(string, syntax):
         if '\n' in string:
             raise ValueError('illegal newline')
 
-        if syntax == Syntax.output:
+        if syntax in [Syntax.output, Syntax.input]:
             return re.sub(r'([:$ ])', r'$\1', string)
-        elif syntax == Syntax.input:
-            return re.sub(r'([$ ])', r'$\1', string)
         elif syntax in [Syntax.shell, Syntax.clean]:
             return string.replace('$', '$$')
 
         raise ValueError(
             'unknown syntax {!r}'.format(syntax)
         )  # pragma: no cover
```

### Comparing `bfg9000-0.6.0/bfg9000/backends/ninja/writer.py` & `bfg9000-0.7.0/bfg9000/backends/ninja/writer.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,19 +3,23 @@
 from ... import iterutils
 from ... import path
 from ... import shell
 from .syntax import *
 from ...versioning import Version
 
 
+def executable(env=os.environ):
+    return shell.which(env.get('NINJA', ['ninja', 'ninja-build']), env)
+
+
 def version(env=os.environ):
     try:
-        ninja = shell.which(env.get('NINJA', ['ninja', 'ninja-build']), env)
+        ninja = executable(env)
         output = shell.execute(ninja + ['--version'], stdout=shell.Mode.pipe,
-                               stderr=shell.Mode.devnull)
+                               stderr=shell.Mode.devnull, env=env)
         return Version(output.strip())
     except (IOError, OSError, shell.CalledProcessError):
         pass
     return None
 
 
 priority = 3
```

### Comparing `bfg9000-0.6.0/bfg9000/build.py` & `bfg9000-0.7.0/bfg9000/build.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import errno
 from itertools import chain
 
+from . import log
 from .arguments.parser import ArgumentParser
 from .builtins import builtin, init as builtin_init
 from .build_inputs import BuildInputs
-from .path import exists, Path, pushd, Root
 from .iterutils import listify
-from .tools import init as tools_init
+from .path import exists, Path, pushd, Root
+from .shell import Mode
+from .tools import init as tools_init, mopack
 
 bfgfile = 'build.bfg'
 optsfile = 'options.bfg'
 
 user_description = """
 These arguments are defined by the options.bfg file in the project's source
 directory. To disambiguate them from built-in arguments, you may prefix the
@@ -25,19 +27,18 @@
 
 
 def is_srcdir(path):
     return exists(path.append(bfgfile))
 
 
 def _execute_script(f, context, path, run_post=False):
-    builddir = context.env.builddir.string() if context.env.builddir else None
-    filename = path.realize({Root.srcdir: None, Root.builddir: builddir})
+    filename = path.string(context.env.base_dirs)
 
     with pushd(path.parent().string(context.env.base_dirs)), \
-         context.push_path(path) as p:  # noqa
+         context.push_path(path) as p:
         code = compile(f.read(), filename, 'exec')
         try:
             exec(code, context.builtins)
         except SystemExit as e:
             if e.code:
                 raise ScriptExitError(filename, e.code)
 
@@ -51,22 +52,21 @@
         return _execute_script(f, context, path, run_post)
 
 
 def load_toolchain(env, path, reload=False):
     builtin_init()
     tools_init()
     if reload:
-        env.init_variables()
+        env.reload()
+    else:
+        env.toolchain.path = path
 
     context = builtin.ToolchainContext(env, reload)
     execute_file(context, path, run_post=True)
 
-    if not reload:
-        env.toolchain.path = path
-
 
 def _execute_options(env, parent=None, usage='parse'):
     optspath = Path(builtin.OptionsContext.filename, Root.srcdir)
     prog = parent.prog if parent else optspath.basename()
     parser = ArgumentParser(prog=prog, parents=listify(parent), add_help=False)
 
     try:
@@ -80,14 +80,32 @@
             return parser, context.seen_paths
     except IOError as e:
         if e.errno != errno.ENOENT:
             raise
         return parser, []
 
 
+def resolve_packages(env, files, flags):
+    if env.variables.initial.get('MOPACK_NESTED_INVOCATION'):
+        return []
+
+    log.info('resolving package dependencies...')
+    mopack_files = ( [Path('.', Root.srcdir)] +
+                     listify(mopack.make_options_yml(env)) +
+                     (files or []) )
+    env.tool('mopack').run(
+        'resolve', mopack_files, directory=env.builddir, flags=flags,
+        env=env.variables.initial, stdout=Mode.normal
+    )
+    # TODO: Would it make sense to convert these paths into ones relative to
+    # the source/build directories if possible?
+    return [Path(i, Root.absolute) for i in
+            env.tool('mopack').run('list_files', directory=env.builddir)]
+
+
 def fill_user_help(env, parent):
     builtin_init()
     return _execute_options(env, parent, usage='help')[0]
 
 
 def configure_build(env):
     builtin_init()
```

### Comparing `bfg9000-0.6.0/bfg9000/build_inputs.py` & `bfg9000-0.7.0/bfg9000/build_inputs.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.6.0/bfg9000/builtins/alias.py` & `bfg9000-0.7.0/bfg9000/builtins/alias.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.6.0/bfg9000/builtins/builtin.py` & `bfg9000-0.7.0/bfg9000/builtins/builtin.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.6.0/bfg9000/builtins/command.py` & `bfg9000-0.7.0/bfg9000/builtins/command.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from itertools import chain, repeat
 
 from . import builtin
 from .. import shell
+from ..backends.compdb import writer as compdb
 from ..backends.make import writer as make
 from ..backends.ninja import writer as ninja
 from ..build_inputs import Edge
 from ..file_types import FileOrDirectory, Node, Phony
-from ..iterutils import isiterable, iterate, listify
+from ..iterutils import first, isiterable, iterate, listify
 from ..objutils import convert_each
 from ..path import Path, Root
 from ..safe_str import jbos, safe_str, safe_string
 from ..shell import posix as pshell
 
 
 class Placeholder(safe_string):
@@ -180,14 +181,25 @@
         command=shell.global_env(rule.env, rule.cmds),
         console=rule.console,
         phony=rule.phony,
         description=rule.description
     )
 
 
+@compdb.rule_handler(BuildStep)
+def compdb_copy_file(rule, build_inputs, buildfile, env):
+    # Only add this step if there's an input file; otherwise, tools consuming
+    # `compile_commands.json` won't have any use for it.
+    if len(rule.files):
+        buildfile.append(
+            arguments=shell.global_env(rule.env, rule.cmds),
+            file=rule.files[0], output=first(rule.public_output)
+        )
+
+
 try:
     from ..backends.msbuild import writer as msbuild
 
     @msbuild.rule_handler(Command, BuildStep)
     def msbuild_command(rule, build_inputs, solution, env):
         command = msbuild.CommandProject.convert_command(shell.global_env(
             rule.env, rule.cmds
```

### Comparing `bfg9000-0.6.0/bfg9000/builtins/compile.py` & `bfg9000-0.7.0/bfg9000/builtins/compile.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from collections import defaultdict
 
 from . import builtin
 from .. import options as opts
 from .path import buildpath, relname, within_directory
 from .file_types import FileList, make_file_list, static_file
+from ..backends.compdb import writer as compdb
 from ..backends.make import writer as make
 from ..backends.ninja import writer as ninja
 from ..build_inputs import build_input, Edge
 from ..file_types import *
-from ..iterutils import first, flatten, iterate
+from ..iterutils import first, flatten, iterate, unlistify
 from ..objutils import convert_each, convert_one
 from ..path import Path
 from ..shell import posix as pshell
 
 build_input('compile_options')(lambda build_inputs, env: defaultdict(list))
 
 
@@ -418,21 +419,47 @@
         rule=compiler.rule_name,
         inputs=inputs,
         implicit=implicit_deps + rule.extra_deps,
         variables=variables
     )
 
 
+@compdb.rule_handler(CompileSource, CompileHeader, GenerateSource)
+def compdb_compile(rule, build_inputs, buildfile, env):
+    compiler = rule.compiler
+    cmd_kwargs = {}
+
+    if hasattr(compiler, 'flags_var'):
+        gopts = build_inputs['compile_options'][compiler.lang]
+        cmd_kwargs['flags'] = (compiler.global_flags +
+                               compiler.flags(gopts, mode='global') +
+                               rule.flags(gopts))
+
+    if compiler.deps_flavor == 'gcc':
+        cmd_kwargs['deps'] = (first(rule.output).path.addext('.d')
+                              if compiler.deps_flavor == 'gcc' else None)
+    elif compiler.deps_flavor == 'msvc':
+        cmd_kwargs['deps'] = True
+
+    output = unlistify(rule.output if compiler.num_outputs == 'all'
+                       else rule.output[0:compiler.num_outputs])
+    buildfile.append(
+        arguments=compiler(rule.file, output, **cmd_kwargs),
+        file=rule.file, output=first(rule.public_output)
+    )
+
+
 try:
     from ..backends.msbuild import writer as msbuild
 
     @msbuild.rule_handler(CompileSource, CompileHeader)
     def msbuild_compile(rule, build_inputs, solution, env):
         # MSBuild does compilation and linking in one unit; see link.py.
         pass
 
     @msbuild.rule_handler(GenerateSource)
     def msbuild_generate_source(rule, build_inputs, solution, env):
-        raise ValueError('msbuild backend does not currently support ' +
-                         "'generated_source'")  # pragma: no cover
+        raise ValueError(
+            "msbuild backend does not currently support 'generated_source'"
+        )  # pragma: no cover
 except ImportError:  # pragma: no cover
     pass
```

### Comparing `bfg9000-0.6.0/bfg9000/builtins/copy_file.py` & `bfg9000-0.7.0/bfg9000/builtins/copy_file.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import os
 
 from . import builtin
-from .file_types import FileList, make_file_list
+from .file_types import FileList, make_file_list, static_file
 from .path import buildpath, relname, within_directory
+from ..backends.compdb import writer as compdb
 from ..backends.make import writer as make
 from ..backends.ninja import writer as ninja
 from ..build_inputs import Edge
-from ..file_types import File
+from ..file_types import File, ManPage
+from ..iterutils import first, unlistify
 from ..path import Path
 from ..versioning import SpecifierSet
 
 
 class CopyFile(Edge):
     __modes = {'copy', 'symlink', 'hardlink'}
     msbuild_output = True
@@ -40,14 +42,37 @@
                 return path
             return Path(relname(context, name))
 
         output = file.clone(pathfn)
         return output, file, kwargs
 
 
+# XXX: It might be worth generalizing this and merging it with CopyFile above,
+# e.g. if we want to allow users to easily compress any kind of file in their
+# build scripts.
+class CompressFile(Edge):
+    mode = 'gzip'
+
+    def __init__(self, context, output, file, *, extra_deps=None,
+                 description=None):
+        self.copier = context.env.tool('gzip')
+        self.file = file
+        super().__init__(context.build, output, None, extra_deps, description)
+
+    @staticmethod
+    def convert_args(context, file, kwargs):
+        file = context['auto_file'](file)
+
+        def pathfn(file):
+            return file.path.reroot().addext('.gz')
+
+        output = file.clone(pathfn)
+        return output, file, kwargs
+
+
 @builtin.function()
 @builtin.type(File, short_circuit=False, first_optional=True)
 def copy_file(context, name, file, **kwargs):
     # Note: this only handles single files. File objects with multiple
     # related files (e.g. a DLL and its import library) will only copy the
     # primary file. In practice, this shouldn't matter, as this function is
     # mostly useful for copying data files to the build directory.
@@ -57,15 +82,38 @@
 
 @builtin.function()
 @builtin.type(FileList, in_type=object)
 def copy_files(context, files, **kwargs):
     return make_file_list(context, context['copy_file'], files, **kwargs)
 
 
-@make.rule_handler(CopyFile)
+@builtin.function()
+@builtin.type(ManPage, short_circuit=False)
+def man_page(context, name, *, compress='auto', **kwargs):
+    if isinstance(name, ManPage):
+        file = name
+    else:
+        path = context['relpath'](name)
+        level = kwargs.pop('level', None)
+        if level is None:
+            ext = path.ext()
+            if not ext[1].isdigit():
+                raise ValueError('unable to guess man page level')
+            level = ext[1]
+        dist = kwargs.pop('dist', True)
+        file = static_file(context, ManPage, name, dist, [('level', level)])
+
+    if ( not compress or
+         (compress == 'auto' and not context.env.tool('gzip').found) ):
+        return file
+    output, file, kwargs = CompressFile.convert_args(context, file, kwargs)
+    return CompressFile(context, output, file, **kwargs).public_output
+
+
+@make.rule_handler(CopyFile, CompressFile)
 def make_copy_file(rule, build_inputs, buildfile, env):
     copier = rule.copier
     recipename = make.var('RULE_{}'.format(copier.rule_name.upper()))
 
     if hasattr(copier, 'transform_input'):
         input_var = make.qvar('1')
         args = [copier.transform_input(rule.file, rule.raw_output)]
@@ -80,15 +128,15 @@
         target=rule.output,
         deps=[rule.file] + rule.extra_deps,
         order_only=make.directory_deps(rule.output),
         recipe=make.Call(recipename, *args)
     )
 
 
-@ninja.rule_handler(CopyFile)
+@ninja.rule_handler(CopyFile, CompressFile)
 def ninja_copy_file(rule, build_inputs, buildfile, env):
     copier = rule.copier
 
     variables = {}
     if rule.description:
         variables['description'] = rule.description
 
@@ -113,15 +161,30 @@
         rule=copier.rule_name,
         inputs=rule.file,
         implicit=rule.extra_deps,
         variables=variables
     )
 
 
+@compdb.rule_handler(CopyFile)
+def compdb_copy_file(rule, build_inputs, buildfile, env):
+    copier = rule.copier
+
+    in_file = rule.file
+    if hasattr(copier, 'transform_input'):
+        in_file = copier.transform_input(rule.file, rule.raw_output)
+    buildfile.append(
+        arguments=copier(in_file, unlistify(rule.output)),
+        file=rule.file, output=first(rule.public_output)
+    )
+
+
 try:
+    import warnings
+
     from ..backends.msbuild import writer as msbuild
 
     @msbuild.rule_handler(CopyFile)
     def msbuild_copy_file(rule, build_inputs, solution, env):
         copier = rule.copier
         if hasattr(copier, 'transform_input'):
             input = copier.transform_input(rule.file, rule.raw_output)
@@ -141,9 +204,15 @@
             env, name=name, commands=[msbuild.CommandProject.task(
                 'Copy', SourceFiles=input, DestinationFiles=rule.raw_output,
                 **extra_attrs
             )],
             dependencies=solution.dependencies(rule.extra_deps),
         )
         solution[rule.output[0]] = project
+
+    @msbuild.rule_handler(CompressFile)
+    def msbuild_generate_source(rule, build_inputs, solution, env):
+        warnings.warn(
+            'msbuild backend does not currently support compressing files'
+        )  # pragma: no cover
 except ImportError:  # pragma: no cover
     pass
```

### Comparing `bfg9000-0.6.0/bfg9000/builtins/core.py` & `bfg9000-0.7.0/bfg9000/builtins/core.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.6.0/bfg9000/builtins/default.py` & `bfg9000-0.7.0/bfg9000/builtins/default.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.6.0/bfg9000/builtins/dist.py` & `bfg9000-0.7.0/bfg9000/builtins/dist.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     project = build_inputs['project']
     dstname = project.name
     if project.version:
         dstname += '-' + str(project.version)
 
     return doppel(
         'archive', [i.path.relpath(srcdir) for i in build_inputs.sources()],
-        Path(dstname + _exts[format]), directory=srcdir, format=format,
+        Path(dstname + _exts[format]), format=format, directory=srcdir,
         dest_prefix=dstname
     )
 
 
 @make.post_rule
 def make_dist_rule(build_inputs, buildfile, env):
     for fmt in _exts:
```

### Comparing `bfg9000-0.6.0/bfg9000/builtins/file_types.py` & `bfg9000-0.7.0/bfg9000/builtins/file_types.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import os
-import warnings
 from collections import abc
 from contextlib import contextmanager
 from itertools import chain
 
 from . import builtin
 from ..file_types import *
 from ..iterutils import iterate, listify, uniques
@@ -93,22 +92,14 @@
 @builtin.type(SourceFile)
 def source_file(context, name, lang=None, *, dist=True):
     path = context['relpath'](name)
     lang = lang or known_langs.fromext(path.ext(), 'source')
     return static_file(context, SourceFile, path, dist, [('lang', lang)])
 
 
-# TODO: remove this after 0.6 is released.
-@builtin.function()
-@builtin.type(SourceFile)
-def resource_file(context, name, lang=None, *, dist=True):  # pragma: no cover
-    warnings.warn("'resource_file' is deprecated; use 'source_file' instead")
-    return source_file(context, name, lang, dist=dist)
-
-
 @builtin.function()
 @builtin.type(HeaderFile)
 def header_file(context, name, lang=None, *, dist=True):
     path = context['relpath'](name)
     lang = lang or known_langs.fromext(path.ext(), 'header')
     return static_file(context, HeaderFile, path, dist, [('lang', lang)])
 
@@ -146,18 +137,14 @@
 # files.
 
 
 def _find(context, path, include, **kwargs):
     if not include:
         return None
 
-    # TODO: Remove this after 0.6 is released.
-    if '0.5.9' in context.build['required_version']:
-        return context['find_files'](path, include, **kwargs)
-
     patterns = [path.append(i) for i in iterate(include)]
     return context['find_files'](patterns, **kwargs)
 
 
 def _directory_path(context, thing):
     if isinstance(thing, File):
         return thing.path.parent()
```

### Comparing `bfg9000-0.6.0/bfg9000/builtins/find.py` & `bfg9000-0.7.0/bfg9000/builtins/find.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 import re
-import warnings
 from enum import Enum
 from functools import reduce
-from itertools import product
 
 from . import builtin
-from ..glob import NameGlob, NonGlobError, PathGlob
+from ..glob import NameGlob, PathGlob
 from ..iterutils import iterate, listify
 from ..backends.make import writer as make
 from ..backends.ninja import writer as ninja
 from ..backends.make.syntax import Writer, Syntax
 from ..build_inputs import build_input
-from ..path import exists, isdir, Path, Root, walk, uniquetrees
+from ..path import Path, Root, walk, uniquetrees
 from ..platforms import known_platforms
 
 build_input('find_dirs')(lambda build_inputs, env: set())
 depfile_name = '.bfg_find_deps'
 
 
 @builtin.default()
@@ -137,87 +135,39 @@
     results = []
     for path, matched in _find_files(env, file_filter):
         if matched == FindResult.include:
             results.append(path)
     return results
 
 
-def _find_files_common(context, file_filter, file_type=None, dir_type=None,
-                       dist=True, cache=True):
+@builtin.function()
+def find_files(context, pattern, *, type=None, extra=None, exclude=None,
+               filter=None, file_type=None, dir_type=None, dist=True,
+               cache=True):
     types = {'f': file_type or context['auto_file'],
              'd': dir_type or context['directory']}
     extra_types = {'f': context['generic_file'], 'd': context['directory']}
 
+    pattern = [context['relpath'](i) for i in iterate(pattern)]
+    exclude = context.build['project']['find_exclude'] + listify(exclude)
+    file_filter = FileFilter(pattern, type, extra, exclude, filter)
+
     found, seen_dirs = [], []
     for path, matched in _find_files(context.env, file_filter, seen_dirs):
         if matched == FindResult.include:
             found.append(types[_path_type(path)](path, dist=dist))
         elif matched == FindResult.not_now and dist:
             extra_types[_path_type(path)](path, dist=dist)
 
     if cache:
         context.build['find_dirs'].update(seen_dirs)
         context.build['regenerate'].depfile = depfile_name
     return found
 
 
-def _find_files_new(context, pattern, *, type=None, extra=None, exclude=None,
-                    filter=None, **kwargs):
-    pattern = [context['relpath'](i) for i in iterate(pattern)]
-    exclude = context.build['project']['find_exclude'] + listify(exclude)
-    file_filter = FileFilter(pattern, type, extra, exclude, filter)
-
-    return _find_files_common(context, file_filter, **kwargs)
-
-
-# TODO: Remove this after 0.6 is released.
-def _find_files_old(context, path='.', name='*', type='*', extra=None,
-                    exclude=['.*#', '*~', '#*#'], filter=None, flat=False,
-                    file_type=None, dir_type=None, dist=True, cache=True):
-    warnings.warn('using v0.5 compatibility mode for find_files API')
-    types = {'f': file_type or context['auto_file'],
-             'd': dir_type or context['directory']}
-
-    def make_pattern(path, name):
-        return path.append(name) if flat else path.append('**').append(name)
-
-    def make_file(path):
-        if isdir(path, context.env.base_dirs):
-            return types['d'](path, dist=dist)
-        return types['f'](path, dist=dist)
-
-    path = [context['relpath'](i) for i in iterate(path)]
-    pattern = [make_pattern(p, n) for p, n in product(path, iterate(name))]
-    try:
-        file_filter = FileFilter(pattern, type, extra, exclude, filter)
-    except NonGlobError:
-        return [make_file(i) for i in pattern
-                if exists(i, context.env.base_dirs)]
-
-    # Match against the root paths we're searching, since the old
-    # implementation did that.
-    name_glob = NameGlob(name, type)
-    found = []
-    for i in path:
-        i = i.as_directory()
-        if name_glob.match(i):
-            found.append(make_file(i))
-
-    found.extend(_find_files_common(context, file_filter, file_type, dir_type,
-                                    dist, cache))
-    return found
-
-
-@builtin.function()
-def find_files(context, *args, **kwargs):
-    if '0.5.9' in context.build['required_version']:
-        return _find_files_old(context, *args, **kwargs)
-    return _find_files_new(context, *args, **kwargs)
-
-
 @builtin.function()
 def find_paths(context, *args, **kwargs):
     return [i.path for i in context['find_files'](*args, **kwargs)]
 
 
 @make.post_rule
 def make_find_dirs(build_inputs, buildfile, env):
```

### Comparing `bfg9000-0.6.0/bfg9000/builtins/install.py` & `bfg9000-0.7.0/bfg9000/builtins/install.py`

 * *Files 4% similar despite different names*

```diff
@@ -66,24 +66,16 @@
             raise TypeError(('{!r} is not installable; specify an absolute ' +
                              'install directory?').format(type(f).__name__))
         elif directory:
             install_root = path.Path(directory, f.install_root)
         else:
             install_root = f.install_root
 
-        # Get the suffix.
-        if isinstance(f, Directory):
-            suffix = ''
-        elif f.path.root == path.Root.srcdir:
-            suffix = f.path.basename()
-        else:
-            suffix = f.path.suffix
-
         cls = cross.target_platform.Path if cross else type(f.path)
-        return cls(suffix, install_root, destdir=not cross)
+        return cls(f.install_suffix, install_root, destdir=not cross)
 
     if not isinstance(file, BaseFile):
         raise TypeError('expected a file or directory')
     return file.clone(pathfn, recursive=True)
 
 
 def can_install(env):
@@ -143,14 +135,20 @@
     def post_install(i):
         return i.post_install(install_outputs) if i.post_install else None
 
     return ([install_line(*i) for i in install_outputs.host.items()] +
             list(filter( None, (post_install(i) for i in install_outputs) )))
 
 
+def _install_mopack(env):
+    if env.mopack:
+        return [env.tool('mopack')('deploy', directory=path.Path('.'))]
+    return []
+
+
 def _uninstall_files(install_outputs, env):
     def uninstall_line(src, dst):
         if isinstance(src, Directory):
             return [dst.path.append(i.path.relpath(src.path)) for i in
                     iterate(src.files)]
         return [dst.path]
 
@@ -169,52 +167,64 @@
         buildfile.variable(buildfile.path_vars[path.DestDir.destdir],
                            env.variables.get('DESTDIR', ''),
                            buildfile.Section.path)
 
 
 @make.post_rule
 def make_install_rule(build_inputs, buildfile, env):
-    install_outputs = build_inputs['install']
-    if not can_install(env) or not install_outputs:
+    if not can_install(env):
         return
 
+    install_outputs = build_inputs['install']
     install_files = _install_files(install_outputs, buildfile, env)
     uninstall_files = _uninstall_files(install_outputs, env)
-    _add_install_paths(buildfile, env)
 
-    buildfile.rule(
-        target='install',
-        deps='all',
-        recipe=install_files,
-        phony=True
-    )
-    buildfile.rule(
-        target='uninstall',
-        recipe=uninstall_files,
-        phony=True
-    )
+    if install_files or uninstall_files:
+        _add_install_paths(buildfile, env)
+
+    install_commands = install_files + _install_mopack(env)
+
+    if install_commands:
+        buildfile.rule(
+            target='install',
+            deps='all',
+            recipe=install_commands,
+            phony=True
+        )
+    if uninstall_files:
+        buildfile.rule(
+            target='uninstall',
+            recipe=uninstall_files,
+            phony=True
+        )
 
 
 @ninja.post_rule
 def ninja_install_rule(build_inputs, buildfile, env):
-    install_outputs = build_inputs['install']
-    if not can_install(env) or not install_outputs:
+    if not can_install(env):
         return
 
+    install_outputs = build_inputs['install']
     install_files = _install_files(install_outputs, buildfile, env)
     uninstall_files = _uninstall_files(install_outputs, env)
-    _add_install_paths(buildfile, env)
 
-    ninja.command_build(
-        buildfile, env,
-        output='install',
-        inputs=['all'],
-        command=shell.join_lines(install_files),
-        console=True,
-        phony=True
-    )
-    ninja.command_build(
-        buildfile, env,
-        output='uninstall',
-        command=shell.join_lines(uninstall_files),
-        phony=True
-    )
+    if install_files or uninstall_files:
+        _add_install_paths(buildfile, env)
+
+    install_commands = install_files + _install_mopack(env)
+
+    if install_commands:
+        ninja.command_build(
+            buildfile, env,
+            output='install',
+            inputs=['all'],
+            command=shell.join_lines(install_commands),
+            console=True,
+            phony=True
+        )
+    if uninstall_files:
+        ninja.command_build(
+            buildfile, env,
+            output='uninstall',
+            command=shell.join_lines(uninstall_files),
+            phony=True
+        )
```

### Comparing `bfg9000-0.6.0/bfg9000/builtins/link.py` & `bfg9000-0.7.0/bfg9000/builtins/link.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,20 +3,22 @@
 from collections import defaultdict
 from itertools import chain
 
 from . import builtin
 from .. import options as opts
 from .file_types import static_file
 from .path import relname
+from ..backends.compdb import writer as compdb
 from ..backends.make import writer as make
 from ..backends.ninja import writer as ninja
 from ..build_inputs import build_input, Edge
 from ..exceptions import ToolNotFoundError
 from ..file_types import *
-from ..iterutils import first, flatten, iterate, listify, slice_dict, uniques
+from ..iterutils import (first, flatten, iterate, listify, slice_dict, uniques,
+                         unlistify)
 from ..languages import known_formats
 from ..objutils import convert_each, convert_one
 from ..platforms import known_native_object_formats
 from ..shell import posix as pshell
 
 build_input('link_options')(lambda build_inputs, env: {
     'dynamic': defaultdict(list), 'static': defaultdict(list)
@@ -341,16 +343,17 @@
                   ('lang', context.build['project']['lang'])]
         file_type = StaticLibrary
 
         if explicit_kind:
             if kind == 'shared':
                 file_type = SharedLibrary
             elif kind == 'dual':
-                raise ValueError("can't create dual-use libraries from an " +
-                                 "existing file")
+                raise ValueError(
+                    "can't create dual-use libraries from an existing file"
+                )
 
         # XXX: Try to detect if a string refers to a shared lib?
         return static_file(context, file_type, name, dist, params, kwargs)
 
     if kind is None:
         raise ValueError('unable to create library: both shared and static ' +
                          'modes disabled')
@@ -518,14 +521,44 @@
         inputs=rule.files,
         implicit=(rule.libs + package_build_deps + module_defs + manifest +
                   rule.extra_deps),
         variables=variables
     )
 
 
+@compdb.rule_handler(StaticLink, DynamicLink, SharedLink)
+def compdb_link(rule, build_inputs, buildfile, env):
+    linker = rule.linker
+    cmd_kwargs = {}
+
+    if hasattr(linker, 'flags_var') or hasattr(linker, 'libs_var'):
+        gopts = build_inputs['link_options'][rule.base_mode][linker.family]
+    if hasattr(linker, 'flags_var'):
+        cmd_kwargs['flags'] = (linker.global_flags +
+                               linker.flags(gopts, mode='global') +
+                               rule.flags(gopts))
+    if hasattr(linker, 'libs_var'):
+        cmd_kwargs['libs'] = (linker.global_libs +
+                              linker.lib_flags(gopts, mode='global') +
+                              rule.lib_flags(gopts))
+    if hasattr(rule, 'manifest'):
+        cmd_kwargs['manifest'] = rule.manifest
+
+    file = rule.files[0] if len(rule.files) else rule.user_libs[0]
+    in_files = rule.files
+    if hasattr(linker, 'transform_input'):
+        in_files = linker.transform_input(in_files)
+    output = unlistify(rule.output if linker.num_outputs == 'all'
+                       else rule.output[0:linker.num_outputs])
+    buildfile.append(
+        arguments=linker(in_files, output, **cmd_kwargs),
+        file=file, output=first(rule.public_output)
+    )
+
+
 try:
     from .compile import CompileHeader
     from ..backends.msbuild import writer as msbuild
 
     def _parse_compiler_cflags(compiler, global_options):
         return compiler.parse_flags(msbuild.textify_each(
             compiler.global_flags +
```

### Comparing `bfg9000-0.6.0/bfg9000/builtins/path.py` & `bfg9000-0.7.0/bfg9000/builtins/path.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.6.0/bfg9000/builtins/pkg_config.py` & `bfg9000-0.7.0/bfg9000/builtins/pkg_config.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,20 +6,20 @@
 from .file_types import make_immediate_file
 from .install import can_install
 from .. import options as opts, path
 from ..build_inputs import build_input
 from ..file_types import *
 from ..iterutils import flatten, iterate, uniques, recursive_walk
 from ..objutils import objectify, identity
-from ..packages import CommonPackage, PackageKind
+from ..packages import CommonPackage, Package
 from ..safe_str import literal, shell_literal
 from ..shell import posix as pshell
 from ..shell.syntax import Syntax, Writer
 from ..tools.install_name_tool import darwin_install_name
-from ..tools.pkg_config import PkgConfigPackage
+from ..tools.pkg_config import GeneratedPkgConfigPackage, PkgConfigPackage
 from ..versioning import simplify_specifiers, Specifier, SpecifierSet
 
 build_input('pkg_config')(lambda build_inputs, env: [])
 
 
 class Requirement:
     def __init__(self, name, version=None):
@@ -46,15 +46,15 @@
 
     def split(self, single=False):
         specs = simplify_specifiers(self.version)
         if len(specs) == 0:
             return [SimpleRequirement(self.name)]
         if single and len(specs) > 1:
             raise ValueError(
-                ("multiple specifiers ({}) used in pkg-config requirement " +
+                ('multiple specifiers ({}) used in pkg-config requirement ' +
                  "for '{}'").format(self.version, self.name)
             )
         return [SimpleRequirement(self.name, i) for i in specs]
 
     def __hash__(self):
         return hash((self.name, self.version))
 
@@ -155,24 +155,16 @@
             final_value = self.fn(obj, value) if value is not None else None
             setattr(obj, '_' + self.fn.__name__, final_value)
 
     def __init__(self, context, name=None, *, desc_name=None, desc=None,
                  url=None, version=None, requires=None, requires_private=None,
                  conflicts=None, includes=None, libs=None, libs_private=None,
                  options=None, link_options=None, link_options_private=None,
-                 lang=None, auto_fill=None):
+                 lang=None, auto_fill=False):
         self._builtins = context.builtins
-        # TODO: Remove this after 0.6 is released.
-        if auto_fill is None:  # pragma: no cover
-            if '0.5.9' in context.build['required_version']:
-                warnings.warn('auto_fill will default to False in v0.6 mode ' +
-                              '(defaulting to True this time)')
-                auto_fill = True
-            else:
-                auto_fill = False
         self.auto_fill = auto_fill
 
         self.name = name
         self.desc_name = desc_name
         self.desc = desc
         self.url = url
         self.version = version
@@ -305,24 +297,31 @@
 
     @staticmethod
     def _filter_packages(packages):
         pkg_config, system, deps = RequirementSet(), [], []
         for i in packages:
             if isinstance(i, str):
                 pkg_config.add(Requirement(i))
+                continue
             elif isinstance(i, (tuple, list)):
                 pkg_config.add(Requirement(*i))
-            elif isinstance(i, PkgConfigPackage):
-                pkg_config.add(Requirement(i.name, i.specifier))
+                continue
+            elif isinstance(i, Package):
                 if i.deps:
                     deps.append(i)
-            elif isinstance(i, CommonPackage):
-                system.append(i)
-            else:
-                raise TypeError('unsupported package type: {}'.format(type(i)))
+
+                if isinstance(i, (CommonPackage, GeneratedPkgConfigPackage)):
+                    system.append(i)
+                    continue
+                elif isinstance(i, PkgConfigPackage):
+                    pkg_config.add(Requirement(i.pcnames[0], i.specifier))
+                    pkg_config.update(Requirement(i) for i in i.pcnames[1:])
+                    continue
+
+            raise TypeError('unsupported package type: {}'.format(type(i)))
         return pkg_config, uniques(system), deps
 
 
 class PkgConfigWriter:
     directory = path.Path('pkgconfig')
 
     def __init__(self, context):
@@ -382,40 +381,41 @@
         link_options_private = opts.option_list(
             (opts.lib(installify_fn(i.all[0])) for i in data['libs_private']),
             data['link_options_private']
         )
 
         # Add the options from each of the system packages.
         for pkg in data['extra_pkgs']:
-            compile_options.extend(pkg.compile_options(compiler))
-            link_options.extend(pkg.link_options(linker))
+            compile_options.extend(pkg.compile_options(compiler, raw=True))
+            link_options.extend(pkg.link_options(linker, raw=True))
         for pkg in data['extra_pkgs_private']:
-            compile_options.extend(pkg.compile_options(compiler))
-            link_options_private.extend(pkg.link_options(linker))
+            compile_options.extend(pkg.compile_options(compiler, raw=True))
+            link_options_private.extend(pkg.link_options(linker, raw=True))
 
         cflags = compiler.flags(compile_options, mode='pkg-config')
         ldflags = (linker.flags(link_options, mode='pkg-config') +
                    linker.lib_flags(link_options, mode='pkg-config'))
         ldflags_private = (
             linker.flags(link_options_private, mode='pkg-config') +
             linker.lib_flags(link_options_private, mode='pkg-config')
         )
 
-        out = Writer(out)
+        # CMake expects POSIX-like paths in pkg-config files.
+        out = Writer(out, localize_paths=False)
 
         if installed:
             for i in path.InstallRoot:
                 if i != path.InstallRoot.bindir:
                     self._write_variable(out, i.name, env.install_dirs[i])
         else:
             self._write_variable(out, 'srcdir', env.srcdir)
             # Set the builddir to be relative to the .pc file's dir so that
             # users can move the build dir around and things still work.
             self._write_variable(out, 'builddir', path.Path('.').relpath(
-                self.directory, prefix='${pcfiledir}'
+                self.directory, prefix='${pcfiledir}', localize=False
             ))
 
         # We set absolute install_names when building mach-o libraries, but to
         # allow users to use the `-uninstalled` variant of the pkg-config file,
         # we need to let them know how to change the install_names in binaries
         # that use this package. Add an `install_names` variable that users can
         # compare between both variants that they can then pass to
@@ -463,27 +463,26 @@
     # package's libraries are fully-linked yet. However, given that this usage
     # of pkg-config files is already a corner case, it might not be worth the
     # added complexity to be smarter here.
     return context['alias']('pkg-config-' + data['name'], data['build_deps'])
 
 
 @builtin.function()
-def pkg_config(context, name=None, **kwargs):
+def pkg_config(context, name=None, *, system=False, **kwargs):
     info = PkgConfigInfo(context, name, **kwargs)
     context.build['pkg_config'].append(info)
 
     if not info.auto_fill:
         dep_alias = _write_pkg_config(context, info)
-        search_path = PkgConfigWriter.directory.string(context.env.base_dirs)
+        search_path = [PkgConfigWriter.directory.string(context.env.base_dirs)]
         try:
             return PkgConfigPackage(
-                info.name, context.env.target_platform.object_format,
-                SpecifierSet(), PackageKind.any,
-                context.env.tool('pkg_config'), dep_alias,
-                search_path=search_path
+                context.env.tool('pkg_config'), info.name,
+                format=context.env.target_platform.object_format,
+                system=system, deps=dep_alias, search_path=search_path
             )
         except FileNotFoundError:
             warnings.warn('unable to load local pkg-config package {!r}'
                           .format(info.name))
             return None
```

### Comparing `bfg9000-0.6.0/bfg9000/builtins/project.py` & `bfg9000-0.7.0/bfg9000/builtins/project.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.6.0/bfg9000/builtins/tests.py` & `bfg9000-0.7.0/bfg9000/builtins/tests.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,25 +39,27 @@
             context.build['defaults'].remove(primary)
         (driver or context.build['tests']).tests.append(self)
 
 
 class TestCase(Test):
     def __init__(self, context, cmd, environment={}, driver=None):
         if driver and environment:
-            raise TypeError("only one of 'driver' and 'environment' may be " +
-                            "specified")
+            raise TypeError(
+                "only one of 'driver' and 'environment' may be specified"
+            )
         super().__init__(context, cmd, environment, driver)
 
 
 class TestDriver(Test):
     def __init__(self, context, cmd, environment={}, parent=None,
                  wrap_children=False):
         if parent and environment:
-            raise TypeError("only one of 'parent' and 'environment' may be " +
-                            "specified")
+            raise TypeError(
+                "only one of 'parent' and 'environment' may be specified"
+            )
 
         super().__init__(context, cmd, environment, parent)
         self.tests = []
         self.wrap_children = wrap_children
 
 
 @builtin.function()
```

### Comparing `bfg9000-0.6.0/bfg9000/builtins/toolchain.py` & `bfg9000-0.7.0/bfg9000/builtins/toolchain.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.6.0/bfg9000/builtins/version.py` & `bfg9000-0.7.0/bfg9000/builtins/version.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.6.0/bfg9000/depfixer.py` & `bfg9000-0.7.0/bfg9000/depfixer.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.6.0/bfg9000/driver.py` & `bfg9000-0.7.0/bfg9000/driver.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import os
+import subprocess
 import sys
 
-from . import build
-from . import log
-from . import path
+from . import build, log, path
+from .app_version import version
 from .arguments import parser as argparse
 from .backends import list_backends
+from .backends.compdb import writer as compdb
 from .environment import Environment, EnvVersionError
 from .platforms.target import platform_info
-from .app_version import version
 
 logger = log.getLogger(__name__)
 
 description = """
 bfg9000 ("build file generator") is a cross-platform build configuration system
 with an emphasis on making it easy to define how to build your software. It
 converts a Python-based build script into the appropriate files for your
@@ -37,25 +37,35 @@
 date.
 """
 
 env_desc = """
 Print the environment variables stored by this build configuration.
 """
 
+run_desc = """
+Run an arbitrary COMMAND with the environment variables set for the current
+build.
+"""
+
 e1m1_desc = """
 You find yourself standing at Doom's gate.
 """
 
+generate_completion_desc = """
+Generate shell-completion functions for bfg9000 and write them to standard
+output. This requires the Python package `shtab`.
+"""
+
 
 def handle_reload_exception(e, suggest_rerun=False):
-    msg = 'Unable to reload environment'
+    msg = 'unable to reload environment'
     if str(e):
         msg += ': {}'.format(str(e))
     if suggest_rerun and isinstance(e, EnvVersionError):
-        msg += '\n  Please re-run bfg9000 manually'
+        msg += '\n  please re-run bfg9000 manually'
     logger.error(msg, exc_info=True)
     return e.code if isinstance(e, build.ScriptExitError) else 1
 
 
 def environment_from_args(args):
     # Get the bin directory holding bfg's executables.
     bfgdir = path.abspath(sys.argv[0]).parent()
@@ -72,14 +82,15 @@
     return env, backend
 
 
 def finalize_environment(env, args, extra_args=None):
     env.finalize(
         install_dirs={i: getattr(args, i.name) for i in path.InstallRoot},
         library_mode=(args.shared, args.static),
+        compdb=args.compdb,
         extra_args=extra_args,
     )
 
 
 def directory_pair(srcname, buildname):
     class DirectoryPair(argparse.Action):
         def __call__(self, parser, namespace, values, option_string=None):
@@ -136,47 +147,75 @@
 def add_configure_args(parser):
     backends = list_backends()
 
     parser.add_argument('-h', '--help', action=ConfigureHelp,
                         help='show this help message and exit')
 
     build = parser.add_argument_group('build arguments')
-    build.add_argument('--backend', metavar='BACKEND',
+    build.add_argument('-B', '--backend', metavar='BACKEND',
                        choices=list(backends.keys()),
                        default=list(backends.keys())[0],
                        help=('build backend (one of %(choices)s; default: ' +
                              '%(default)s)'))
     build.add_argument('--toolchain', metavar='FILE',
                        type=argparse.File(must_exist=True),
                        help=('a file defining the toolchain to use for this ' +
                              'build'))
     build.add_argument('--shared', action='enable', default=True,
                        help='build shared libraries (default: enabled)')
     build.add_argument('--static', action='enable', default=False,
                        help='build static libraries (default: disabled)')
+    build.add_argument('--compdb', action='enable', default=True,
+                       help=('generate compile_commands.json ' +
+                             '(default: enabled)'))
+
+    pkg = parser.add_argument_group('packaging arguments')
+    pkg.add_argument('-p', '--package-file', action='append', metavar='FILE',
+                     dest='package_files',
+                     help='additional package files to resolve')
+    pkg.add_argument('-P', '--package-flag', action='append',
+                     metavar='FLAG', dest='package_flags',
+                     help='additional package flags')
+    pkg.add_argument('--no-resolve-packages', action='store_true',
+                     help='skip resolution of packages')
 
     common_path_help = 'installation path for {} (default: {{}})'
     path_help = {
         'prefix': 'installation prefix (default: {})',
         'exec_prefix': ('installation prefix for architecture-dependent ' +
                         'files (default: {})'),
-        'bindir': common_path_help.format('executables'),
-        'libdir': common_path_help.format('libraries'),
+        'bindir'    : common_path_help.format('executables'),
+        'libdir'    : common_path_help.format('libraries'),
         'includedir': common_path_help.format('headers'),
+        'datadir'   : common_path_help.format('data files'),
+        'mandir'    : common_path_help.format('man pages'),
     }
 
     install_dirs = platform_info().install_dirs
     install = parser.add_argument_group('installation arguments')
     for root in path.InstallRoot:
         name = '--' + root.name.replace('_', '-')
         help = path_help[root.name].format(repr(install_dirs[root]))
         install.add_argument(name, type=argparse.Directory(), metavar='PATH',
                              help=help)
 
 
+def simple_parser():
+    parser = argparse.ArgumentParser(prog='9k', description=configure_desc,
+                                     add_help=False)
+    parser.add_argument(argparse.SUPPRESS,
+                        action=directory_pair('srcdir', 'builddir'),
+                        type=argparse.Directory(), metavar='DIRECTORY',
+                        help='source or build directory')
+    add_generic_args(parser)
+    add_configure_args(parser)
+
+    return parser
+
+
 def configure(parser, subparser, args, extra):
     if ( path.exists(args.builddir) and
          path.samefile(args.srcdir, args.builddir) ):
         subparser.error('source and build directories must be different')
     if not build.is_srcdir(args.srcdir):
         subparser.error('source directory must contain a {} file'
                         .format(build.bfgfile))
@@ -187,18 +226,25 @@
     os.makedirs(args.builddir.string(), exist_ok=True)
 
     try:
         env, backend = environment_from_args(args)
         if args.toolchain:
             build.load_toolchain(env, args.toolchain)
         finalize_environment(env, args, extra)
+
+        if not args.no_resolve_packages:
+            env.mopack = build.resolve_packages(env, args.package_files,
+                                                args.package_flags)
+
         env.save(args.builddir.string())
 
         build_inputs = build.configure_build(env)
         backend.write(env, build_inputs)
+        if env.compdb:
+            compdb.write(env, build_inputs)
     except Exception as e:
         logger.exception(e)
         return e.code if isinstance(e, build.ScriptExitError) else 1
 
 
 def refresh(parser, subparser, args, extra):
     if extra:
@@ -208,19 +254,22 @@
         subparser.error('build directory must not contain a {} file'
                         .format(build.bfgfile))
 
     try:
         env = Environment.load(args.builddir.string())
         if env.toolchain.path:
             build.load_toolchain(env, env.toolchain.path, reload=True)
+
         env.save(args.builddir.string())
 
         backend = list_backends()[env.backend]
         build_inputs = build.configure_build(env)
         backend.write(env, build_inputs)
+        if env.compdb:
+            compdb.write(env, build_inputs)
     except Exception as e:
         return handle_reload_exception(e, suggest_rerun=True)
 
 
 def env(parser, subparser, args, extra):
     if extra:
         subparser.error('unrecognized arguments: {}'.format(' '.join(extra)))
@@ -235,27 +284,62 @@
         for k, v in sorted(env.variables.items()):
             if not args.unique or os.getenv(k) != v:
                 print('{}={}'.format(k, v))
     except Exception as e:
         return handle_reload_exception(e)
 
 
+def run(parser, subparser, args, extra):
+    if extra:
+        subparser.error('unrecognized arguments: {}'.format(' '.join(extra)))
+
+    if build.is_srcdir(args.builddir):
+        subparser.error('build directory must not contain a {} file'
+                        .format(build.bfgfile))
+
+    try:
+        env = Environment.load(args.builddir.string())
+        cmd = args.command
+        if cmd and cmd[0] == '--':
+            cmd = cmd[1:]
+        if len(cmd) == 0:
+            parser.error('command required')
+
+        variables = env.variables.initial if args.initial else env.variables
+        return subprocess.run(cmd, env=variables).returncode
+    except Exception as e:
+        return handle_reload_exception(e)
+
+
 def e1m1(parser, subparser, args, extra):  # pragma: no cover
     import e1m1
     try:
         e1m1.play(args.tempo, args.long)
     except Exception as e:
         logger.exception(e)
         return 1
 
 
 def help(parser, subparser, args, extra):
     parser.parse_args(extra + ['--help'])
 
 
+def generate_completion(parser, subparser, args, extra):
+    if extra:
+        subparser.error('unrecognized arguments: {}'.format(' '.join(extra)))
+
+    try:
+        import shtab
+        p = parser if args.program == 'bfg9000' else simple_parser()
+        print(shtab.complete(p, shell=args.shell))
+    except ImportError:  # pragma: no cover
+        print('shtab not found; install via `pip install shtab`')
+        return 1
+
+
 def main():
     parser = argparse.ArgumentParser(prog='bfg9000', description=description)
     subparsers = parser.add_subparsers(metavar='COMMAND')
     subparsers.required = True
 
     add_generic_args(parser)
 
@@ -291,48 +375,67 @@
                            help='build directory')
 
     env_p = subparsers.add_parser(
         'env', description=env_desc, help='print environment'
     )
     env_p.set_defaults(func=env, parser=env_p)
     env_p.add_argument('-u', '--unique', action='store_true',
-                       help='only show variables that differ from the ' +
-                       'current environment')
+                       help=('only show variables that differ from the ' +
+                             'current environment'))
     env_p.add_argument('builddir', type=argparse.Directory(must_exist=True),
                        metavar='BUILDDIR', nargs='?', default='.',
                        help='build directory')
 
+    run_p = subparsers.add_parser(
+        'run', description=run_desc, help='run a shell command'
+    )
+    run_p.set_defaults(func=run, parser=run_p)
+    run_p.add_argument('-I', '--initial', action='store_true',
+                       help='use initial environment variable state')
+    run_p.add_argument('-B', '--builddir',
+                       type=argparse.Directory(must_exist=True),
+                       metavar='BUILDDIR', default='.', help='build directory')
+    run_p.add_argument('command', metavar='COMMAND', nargs=argparse.REMAINDER,
+                       help='command argument')
+
     e1m1_p = subparsers.add_parser('e1m1', description=e1m1_desc)
     e1m1_p.set_defaults(func=e1m1, parser=e1m1_p)
     # Windows gets glitchy if we play back too fast...
     tempo = 100 if platform_info().family == 'windows' else 120
     e1m1_p.add_argument('-t', '--tempo', metavar='BPM', type=int,
                         default=tempo,
-                        help='playback speed (default:  %(default)s)')
+                        help='playback speed (default: %(default)s)')
     e1m1_p.add_argument('-L', '--long', action='store_true',
                         help='play for longer')
 
     help_p = subparsers.add_parser(
         'help', help='show this help message and exit', add_help=False
     )
     help_p.set_defaults(func=help, parser=help_p)
 
+    completion_p = subparsers.add_parser(
+        'generate-completion', description=generate_completion_desc,
+        help='print shell completion script'
+    )
+    completion_p.set_defaults(func=generate_completion, parser=completion_p)
+    shell = (os.path.basename(os.environ['SHELL'])
+             if 'SHELL' in os.environ else None)
+    completion_p.add_argument('-p', '--program', metavar='PROG',
+                              default='bfg9000', choices=['bfg9000', '9k'],
+                              help=('program to emit completion for (one of ' +
+                                    '%(choices)s; default: %(default)s)'))
+    completion_p.add_argument('-s', '--shell', metavar='SHELL', default=shell,
+                              help='shell type (default: %(default)s)')
+
     args, extra = parser.parse_known_args()
     log.init(args.color, debug=args.debug, warn_once=args.warn_once)
 
     return args.func(parser, args.parser, args, extra)
 
 
 def simple_main():
-    parser = argparse.ArgumentParser(prog='9k', description=configure_desc,
-                                     add_help=False)
-    parser.add_argument(argparse.SUPPRESS,
-                        action=directory_pair('srcdir', 'builddir'),
-                        type=argparse.Directory(), metavar='DIRECTORY',
-                        help='source or build directory')
-    add_generic_args(parser)
-    add_configure_args(parser)
+    parser = simple_parser()
 
     args, extra = parser.parse_known_args()
     log.init(args.color, debug=args.debug, warn_once=args.warn_once)
 
     return configure(parser, parser, args, extra)
```

### Comparing `bfg9000-0.6.0/bfg9000/e1m1.py` & `bfg9000-0.7.0/bfg9000/e1m1.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.6.0/bfg9000/environment.py` & `bfg9000-0.7.0/bfg9000/environment.py`

 * *Files 20% similar despite different names*

```diff
@@ -29,19 +29,83 @@
 
 
 class EnvVersionError(RuntimeError):
     pass
 
 
 class EnvVarDict(dict):
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.initial = dict(self)
+        self._changes = {}
+
+    def to_json(self):
+        return {
+            'initial': self.initial,
+            'current': self,
+        }
+
+    @classmethod
+    def from_json(cls, data):
+        d = cls.__new__(cls)
+        super(cls, d).__init__(data['current'])
+        d.initial = data['initial']
+        return d
+
+    @property
+    def changes(self):
+        if not hasattr(self, '_changes'):
+            self._changes = {}
+            for k, v in self.items():
+                if k not in self.initial or self.initial[k] != v:
+                    self._changes[k] = v
+            for k in set(self.initial.keys()) - self.keys():
+                self._changes[k] = None
+        return self._changes
+
+    def reset(self):
+        super().clear()
+        super().update(self.initial)
+        self._changes = {}
+
     def __setitem__(self, key, value):
         if ( not isinstance(key, str) or
-             not isinstance(value, str) ):  # pragma: no cover
+             not isinstance(value, str) ):
             raise TypeError('expected a string')
         super().__setitem__(key, value)
+        self.changes[key] = value
+
+    def __delitem__(self, key):
+        super().__delitem__(key)
+        self.changes[key] = None
+
+    def clear(self):
+        for k in self:
+            self.changes[k] = None
+        super().clear()
+
+    def pop(self, key, *args, **kwargs):
+        if key in self:
+            self.changes[key] = None
+        return super().pop(key, *args, **kwargs)
+
+    def popitem(self):
+        key, value = super().popitem()
+        self.changes[key] = None
+        return key, value
+
+    def setdefault(self, key, default):
+        if key not in self:
+            self[key] = default
+            return default
+        return self[key]
+
+    def update(self, *args, **kwargs):
+        for k, v in dict(*args, **kwargs).items():
+            self[k] = v
 
     def getpaths(self, key, default=None, **kwargs):
         return [abspath(i) for i in
                 shell.split_paths(self.get(key, default), **kwargs)]
 
 
 class Toolchain:
@@ -57,15 +121,15 @@
     def from_json(cls, data):
         return cls(
             path=try_from_json(Path, data['path']),
         )
 
 
 class Environment:
-    version = 14
+    version = 17
     envfile = '.bfg_environ'
 
     Mode = shell.Mode
 
     def __new__(cls, *args, **kwargs):
         env = object.__new__(cls)
         tools.init()
@@ -81,19 +145,19 @@
         self.host_platform = platforms.host.platform_info()
         self.target_platform = platforms.target.platform_info()
 
         self.srcdir = srcdir.as_directory()
         self.builddir = try_as_directory(builddir)
         self.install_dirs = {}
         self.toolchain = Toolchain()
+        self.mopack = []
 
-        self.initial_variables = dict(os.environ)
-        self.init_variables()
+        self.variables = EnvVarDict(dict(os.environ))
 
-    def finalize(self, install_dirs, library_mode, extra_args=None):
+    def finalize(self, install_dirs, library_mode, compdb, extra_args=None):
         # Fill in any install dirs that aren't already set (e.g. by a
         # toolchain file) with defaults from the target platform, but skip
         # absolute paths if this is a cross-compilation build.
         for k, v in self.target_platform.install_dirs.items():
             if self.install_dirs.get(k):
                 continue
             elif self.is_cross and v and v.root == Root.absolute:
@@ -102,18 +166,19 @@
                 self.install_dirs[k] = try_as_directory(v)
 
         for k, v in install_dirs.items():
             if v:
                 self.install_dirs[k] = v.as_directory()
 
         self.library_mode = LibraryMode(*library_mode)
+        self.compdb = compdb
         self.extra_args = extra_args
 
-    def init_variables(self):
-        self.variables = EnvVarDict(self.initial_variables)
+    def reload(self):
+        self.variables.reset()
 
     @property
     def is_cross(self):
         return self.host_platform != self.target_platform
 
     @property
     def base_dirs(self):
@@ -204,20 +269,21 @@
                     'srcdir': self.srcdir.to_json(),
                     'builddir': self.builddir.to_json(),
                     'install_dirs': {
                         k.name: try_to_json(v)
                         for k, v in self.install_dirs.items()
                     },
                     'toolchain': self.toolchain.to_json(),
+                    'mopack': [i.to_json() for i in self.mopack],
 
                     'library_mode': self.library_mode,
+                    'compdb': self.compdb,
                     'extra_args': self.extra_args,
 
-                    'initial_variables': self.initial_variables,
-                    'variables': self.variables,
+                    'variables': self.variables.to_json(),
                 }
             }, out)
 
     @classmethod
     def load(cls, path):
         with open(os.path.join(path, cls.envfile)) as inp:
             state = json.load(inp)
@@ -237,15 +303,15 @@
         if version < 6:
             backend = list_backends()[data['backend']]
             data['backend_version'] = str(backend.version())
             data['bfgpath'] = Path(data['bfgpath']).to_json()
 
         # v7 replaces bfgpath with bfgdir.
         if version < 7:
-            bfgdir = Path.from_json(data['bfgpath'] + (False,)).parent()
+            bfgdir = Path.from_json(data['bfgpath'] + [False]).parent()
             data['bfgdir'] = bfgdir.to_json()
             del data['bfgpath']
 
         # v8 adds support for user-defined command-line arguments.
         if version < 8:
             data['extra_args'] = []
 
@@ -259,17 +325,17 @@
             for i in ('bindir', 'libdir'):
                 if data['install_dirs'][i][1] == 'prefix':
                     data['install_dirs'][i][1] = 'exec_prefix'
 
         # v11 adds $(DESTDIR) support to Path objects.
         if version < 11:
             for i in ('bfgdir', 'srcdir', 'builddir'):
-                data[i] += (False,)
+                data[i] += [False]
             for i in data['install_dirs']:
-                data['install_dirs'][i] += (False,)
+                data['install_dirs'][i] += [False]
 
         # v12 splits platform into host_platform and target_platform.
         if version < 12:
             platform_name = data.pop('platform')
             data['host_platform'] = data['target_platform'] = platform_name
 
         # v13 adds initial_variables and toolchain.
@@ -280,31 +346,52 @@
         # v14 adds architecture to platform objects.
         if version < 14:
             for i in ('host_platform', 'target_platform'):
                 genus, species = platforms.platform_tuple(data[i])
                 data[i] = {'genus': genus, 'species': species,
                            'arch': platform.machine()}
 
+        # v15 adds mopack file list and changes how variables are stored.
+        if version < 15:
+            data['mopack'] = []
+            data['variables'] = {
+                'initial': data.pop('initial_variables'),
+                'current': data.pop('variables'),
+            }
+
+        # v16 adds support for emitting compile_commands.json.
+        if version < 16:
+            data['compdb'] = True
+
+        # v17 adds datadir and mandir to install_dirs.
+        if version < 17:
+            target_plat = platforms.target.from_json(data['target_platform'])
+            for i in ('datadir', 'mandir'):
+                p = target_plat.install_dirs[InstallRoot[i]].to_json()
+                data['install_dirs'][i] = p
+
         # Now that we've upgraded, initialize the Environment object.
-        env = Environment.__new__(Environment)
+        env = cls.__new__(cls)
 
         env.host_platform = platforms.host.from_json(data['host_platform'])
         env.target_platform = platforms.target.from_json(
             data['target_platform']
         )
 
-        for i in ('backend', 'extra_args', 'initial_variables'):
+        for i in ('backend', 'extra_args'):
             setattr(env, i, data[i])
 
         for i in ('bfgdir', 'srcdir', 'builddir'):
             setattr(env, i, Path.from_json(data[i]).as_directory())
 
         env.backend_version = Version(data['backend_version'])
         env.install_dirs = {
             InstallRoot[k]: Path.from_json(v).as_directory() if v else None
             for k, v in data['install_dirs'].items()
         }
         env.toolchain = Toolchain.from_json(data['toolchain'])
-        env.variables = EnvVarDict(data['variables'])
+        env.mopack = [Path.from_json(i) for i in data['mopack']]
+        env.variables = EnvVarDict.from_json(data['variables'])
         env.library_mode = LibraryMode(*data['library_mode'])
+        env.compdb = data['compdb']
 
         return env
```

### Comparing `bfg9000-0.6.0/bfg9000/file_types.py` & `bfg9000-0.7.0/bfg9000/file_types.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
-from . import safe_str as _safe_str
+from . import path as _path, safe_str as _safe_str
 from .iterutils import listify as _listify
-from .path import InstallRoot as _InstallRoot
 
 
 def _clone_traits(exclude=set(), subfiles={}):
     def inner(cls):
         cls._clone_exclude = cls._clone_exclude | exclude
         if subfiles:
             cls._clone_subfiles = cls._clone_subfiles.copy()
@@ -96,21 +95,31 @@
 
 class File(FileOrDirectory):
     def __init__(self, path):
         if path.directory:
             raise ValueError('expected a non-directory')
         super().__init__(path)
 
+    @property
+    def install_suffix(self):
+        if self.path.root == _path.Root.srcdir:
+            return self.path.basename()
+        return self.path.suffix
+
 
 @_clone_traits(exclude={'files'})
 class Directory(FileOrDirectory):
     def __init__(self, path, files=None):
         super().__init__(path.as_directory())
         self.files = files
 
+    @property
+    def install_suffix(self):
+        return ''
+
     def _clone_args(self, pathfn, recursive):
         args = super()._clone_args(pathfn, recursive)
         if self.files is None:
             args['files'] = None
         elif recursive:
             args['files'] = [i.clone(pathfn, recursive) for i in self.files]
         else:
@@ -125,15 +134,15 @@
 
 
 class SourceFile(CodeFile):
     pass
 
 
 class HeaderFile(CodeFile):
-    install_root = _InstallRoot.includedir
+    install_root = _path.InstallRoot.includedir
 
 
 class PrecompiledHeader(HeaderFile):
     install_root = None
 
 
 @_clone_traits(subfiles={'object_file': 'object_path'})
@@ -147,28 +156,40 @@
     def _clone_args(self, pathfn, recursive):
         args = super()._clone_args(pathfn, recursive)
         args['format'] = self.object_file.format
         return args
 
 
 class HeaderDirectory(Directory):
-    install_root = _InstallRoot.includedir
+    install_root = _path.InstallRoot.includedir
 
     def __init__(self, path, files=None, system=False, langs=None):
         super().__init__(path, files)
         self.system = system
         self.langs = _listify(langs)
 
 
 class ModuleDefFile(File):
     pass
 
 
+class ManPage(File):
+    install_root = _path.InstallRoot.mandir
+
+    def __init__(self, path, level):
+        super().__init__(path)
+        self.level = level
+
+    @property
+    def install_suffix(self):
+        return 'man{}/{}'.format(self.level, self.path.basename())
+
+
 class Binary(File):
-    install_root = _InstallRoot.libdir
+    install_root = _path.InstallRoot.libdir
 
     def __init__(self, path, format, lang=None):
         super().__init__(path)
         self.format = format
         self.lang = lang
 
 
@@ -200,30 +221,30 @@
     @property
     def install_deps(self):
         return self.runtime_deps + self.linktime_deps
 
 
 class Executable(LinkedBinary):
     install_kind = 'program'
-    install_root = _InstallRoot.bindir
+    install_root = _path.InstallRoot.bindir
 
 
 @_clone_traits(exclude={'parent'})
 class Library(LinkedBinary):
     @property
     def runtime_file(self):
         return None
 
 
 # This is used for JVM binaries, which can be both executables and libraries.
 # Multiple inheritance is a sign that we should perhaps switch to a trait-based
 # system though...
 class ExecutableLibrary(Executable, Library):
     install_kind = 'program'
-    install_root = _InstallRoot.libdir
+    install_root = _path.InstallRoot.libdir
 
 
 class SharedLibrary(Library):
     install_kind = 'program'
 
     @property
     def runtime_file(self):
@@ -278,15 +299,15 @@
 # This refers specifically to DLL files that have an import library, not just
 # anything with a .dll extension (for instance, .NET DLLs are just regular
 # shared libraries). While this is a "library" in some senses, since you can't
 # link to it during building, we just consider it a LinkedBinary.
 @_clone_traits(subfiles={'import_lib': 'import_path',
                          'export_file': 'export_path'})
 class DllBinary(LinkedBinary):
-    install_root = _InstallRoot.bindir
+    install_root = _path.InstallRoot.bindir
     private = True
 
     def __init__(self, path, format, lang, import_path, export_path=None):
         super().__init__(path, format, lang)
         self.import_lib = LinkLibrary(import_path, self)
         self.export_file = ExportFile(export_path) if export_path else None
 
@@ -329,8 +350,8 @@
 
     def clone(self, *args, **kwargs):
         return DualUseLibrary(self.shared.clone(*args, **kwargs),
                               self.static.clone(*args, **kwargs))
 
 
 class PkgConfigPcFile(File):
-    install_root = _InstallRoot.libdir
+    install_root = _path.InstallRoot.libdir
```

### Comparing `bfg9000-0.6.0/bfg9000/glob.py` & `bfg9000-0.7.0/bfg9000/glob.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,19 @@
 import fnmatch
 import re
 from collections import namedtuple
-from enum import Enum
+from enum import Enum, Flag
 from itertools import zip_longest
 
-try:
-    from enum import Flag
-except ImportError:
-    from enum import IntEnum as Flag
-
+from .exceptions import NonGlobError
 from .iterutils import find_index, list_view
 from .objutils import objectify
 from .path import Path, Root
 
 
-# TODO: Remove this after 0.6 is released?
-class NonGlobError(ValueError):
-    pass
-
-
 class Glob:
     class Type(Flag):
         file = 1
         dir = 2
         any = file | dir
 
         @classmethod
```

### Comparing `bfg9000-0.6.0/bfg9000/iterutils.py` & `bfg9000-0.7.0/bfg9000/iterutils.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,16 +2,25 @@
 from functools import reduce
 
 __all__ = ['default_sentinel', 'first', 'find_index', 'flatten', 'isiterable',
            'ismapping', 'iterate', 'iterate_each', 'listify', 'list_view',
            'map_iterable', 'merge_dicts', 'merge_into_dict', 'partition',
            'recursive_walk', 'slice_dict', 'tween', 'uniques', 'unlistify']
 
+
 # This could go in a funcutils module if we ever create one...
-default_sentinel = object()
+class _DefaultType:
+    def __bool__(self):
+        return False
+
+    def __repr__(self):
+        return '<default_sentinel>'
+
+
+default_sentinel = _DefaultType()
 
 
 def isiterable(thing):
     return (isinstance(thing, Iterable) and not isinstance(thing, str) and
             not ismapping(thing))
```

### Comparing `bfg9000-0.6.0/bfg9000/jvmoutput.py` & `bfg9000-0.7.0/bfg9000/jvmoutput.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,23 +29,26 @@
     parser.add_argument('-o', type=argparse.FileType('w'), default=sys.stdout,
                         dest='output', help=('the output file to list the ' +
                                              'generated .class files'))
     parser.add_argument('command', nargs=argparse.REMAINDER, metavar='COMMAND',
                         help='the command to execute')
     args = parser.parse_args()
 
-    if len(args.command) == 0:
+    cmd = args.command
+    if cmd and cmd[0] == '--':
+        cmd = cmd[1:]
+    if len(cmd) == 0:
         parser.error('command required')
 
     try:
-        p = subprocess.Popen(args.command, universal_newlines=True,
+        p = subprocess.Popen(cmd, universal_newlines=True,
                              stderr=subprocess.PIPE)
     except OSError as e:
         if e.errno == errno.ENOENT:
-            parser.exit(66, 'command not found: {}\n'.format(args.command[0]))
+            parser.exit(66, 'command not found: {}\n'.format(cmd[0]))
         raise  # pragma: no cover
 
     for line in p.stderr:
         if line[0] != '[':
             sys.stderr.write(line)
             continue
```

### Comparing `bfg9000-0.6.0/bfg9000/languages.py` & `bfg9000-0.7.0/bfg9000/languages.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.6.0/bfg9000/log.py` & `bfg9000-0.7.0/bfg9000/log.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,52 +1,70 @@
 import colorama
 import logging
 import os
 import sys
 import traceback
 import warnings
-from logging import getLogger, CRITICAL, ERROR, WARNING, INFO, DEBUG  # noqa
+from logging import (getLogger, CRITICAL, ERROR, WARNING, INFO,  # noqa: F401
+                     DEBUG)
+from traceback import FrameSummary
 
-from .safe_str import safe_string
 from .iterutils import tween
+from .platforms.host import platform_info
+from .safe_str import safe_string
 
 
 class UserDeprecationWarning(DeprecationWarning):
     pass
 
 
-def _is_bfg_src(filename):
+def _path_within(path, parent):
     try:
-        rel = os.path.relpath(filename, os.path.dirname(__file__))
+        rel = os.path.relpath(path, parent)
     except ValueError:
         return False
     return not rel.startswith(os.pardir + os.sep)
 
 
+def _is_user_src(filename):
+    # On Windows, always treat paths within Python's exec_prefix as non-user
+    # paths. This lets us correctly identify things like runpy.py and
+    # setuptools wrappers as non-user.
+    if ( platform_info().family == 'windows' and
+         _path_within(filename, sys.exec_prefix) ):
+        return False
+    return not _path_within(filename, os.path.dirname(__file__))
+
+
 def _filter_stack(stack):
     # Find where the user's stack frames begin and end.
     gen = enumerate(stack)
     for start, line in gen:
-        if not _is_bfg_src(line[0]):
+        if _is_user_src(line[0]):
             break
     else:
         start = len(stack)
 
     for end, line in gen:
-        if _is_bfg_src(line[0]):
+        if not _is_user_src(line[0]):
             break
     else:
         end = len(stack)
 
     return stack[:start], stack[start:end], stack[end:]
 
 
-def _format_stack(stack):
+def _format_stack(stack, user=False):
     if len(stack) == 0:
         return ''
+
+    if user:
+        stack = [FrameSummary(os.path.relpath(i.filename), i.lineno, i.name,
+                              locals=i.locals, line=i.line) for i in stack]
+
     # Put the newline at the beginning, since this helps our formatting later.
     return '\n' + ''.join(traceback.format_list(stack)).rstrip()
 
 
 class StackFilter:
     def __init__(self, has_stack=True):
         self.has_stack = has_stack
@@ -82,49 +100,59 @@
     def emit(self, record):
         if record.exc_info:
             if isinstance(record.exc_info[1], SyntaxError):
                 e = record.exc_info[1]
                 record.msg = e.msg
 
                 # Figure out where to put the caret.
-                text = e.text.expandtabs()
+                text = e.text.expandtabs().rstrip()
                 dedent = len(text) - len(text.lstrip())
                 offset = 4 - dedent - 1 + e.offset
 
-                record.full_stack = [(e.filename, e.lineno, '<module>',
-                                      e.text + ' ' * offset + '^')]
+                record.full_stack = [
+                    FrameSummary(e.filename, e.lineno, '<module>',
+                                 line=e.text + '\n' + ' ' * offset + '^')
+                ]
             else:
                 if not record.msg:
                     record.msg = record.exc_info[0].__name__
                 elif self.debug:
                     record.msg = '{}: {}'.format(record.exc_info[0].__name__,
                                                  record.msg)
                 record.full_stack = traceback.extract_tb(record.exc_info[2])
             record.exc_info = None
 
         pre, stack, post = _filter_stack(record.full_stack)
 
         record.stack_pre = _format_stack(pre)
-        record.stack = _format_stack(stack)
+        record.stack = _format_stack(stack, user=True)
         record.stack_post = _format_stack(post)
 
         if len(stack):
-            record.user_pathname = stack[-1][0]
+            record.user_pathname = os.path.relpath(stack[-1][0])
             record.user_lineno = stack[-1][1]
         else:
             record.user_pathname = record.pathname
             record.user_lineno = record.lineno
 
         if len(stack) or self.debug:
             return super().emit(record)
 
         record.show_stack = False
         logging.root.handle(record)
 
 
+def _clicolor(environ):
+    if environ.get('CLICOLOR_FORCE', '0') != '0':
+        return 'always'
+    if 'CLICOLOR' in environ:
+        return 'never' if environ['CLICOLOR'] == '0' else 'auto'
+    return None
+
+
 def _init_logging(logger, debug, stream=None):
     logger.setLevel(logging.DEBUG if debug else logging.INFO)
 
     stackless = ColoredStreamHandler(stream)
     stackless.addFilter(StackFilter(has_stack=False))
 
     fmt = '%(coloredlevel)s: %(message)s'
@@ -133,24 +161,25 @@
     logger.addHandler(stackless)
 
     stackful = StackfulStreamHandler(stream, debug=debug)
     stackful.addFilter(StackFilter(has_stack=True))
 
     fmt = '%(coloredlevel)s: %(user_pathname)s:%(user_lineno)d: %(message)s'
     if debug:
-        fmt += '\033[2m%(stack_pre)s\033[0m'
+        fmt += '\033[90m%(stack_pre)s\033[0m'
     fmt += '%(stack)s'
     if debug:
-        fmt += '\033[2m%(stack_post)s\033[0m'
+        fmt += '\033[90m%(stack_post)s\033[0m'
 
     stackful.setFormatter(logging.Formatter(fmt))
     logger.addHandler(stackful)
 
 
-def init(color='auto', debug=False, warn_once=False):
+def init(color='auto', debug=False, warn_once=False, environ=os.environ):
+    color = _clicolor(environ) or color
     if color == 'always':
         colorama.init(strip=False)
     elif color == 'never':
         colorama.init(strip=True, convert=False)
     else:  # color == 'auto'
         colorama.init()
```

### Comparing `bfg9000-0.6.0/bfg9000/objutils.py` & `bfg9000-0.7.0/bfg9000/objutils.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import functools
 from itertools import chain
 
 from .iterutils import isiterable, iterate
 
 __all__ = ['convert_each', 'convert_one', 'hashify', 'identity', 'memoize',
-           'objectify']
+           'memoize_method', 'objectify']
 
 
 def identity(x):
     return x
 
 
 def objectify(thing, valid_type, creator=None, in_type=str, **kwargs):
@@ -35,15 +35,15 @@
 
 def convert_each(kwargs, key, fn, **fn_kwargs):
     kwargs[key] = [fn(i, **fn_kwargs) for i in iterate(kwargs.get(key))]
 
 
 def hashify(thing):
     if isinstance(thing, dict):
-        return frozenset((hashify(k), hashify(v)) for k, v in thing.items())
+        return tuple((hashify(k), hashify(v)) for k, v in thing.items())
     elif isiterable(thing):
         return tuple(hashify(i) for i in thing)
     return thing
 
 
 def memoize(fn):
     cache = {}
@@ -57,7 +57,34 @@
         return result
 
     def reset():
         cache.clear()
 
     wrapper._reset = reset
     return wrapper
+
+
+def memoize_method(fn):
+    cachename = '_memoize_cache_{}'.format(fn.__name__)
+
+    @functools.wraps(fn)
+    def wrapper(self, *args, **kwargs):
+        try:
+            cache = getattr(self, cachename)
+        except AttributeError:
+            cache = {}
+            setattr(self, cachename, cache)
+
+        key = (hashify(args), hashify(kwargs))
+        if key in cache:
+            return cache[key]
+        result = cache[key] = fn(self, *args, **kwargs)
+        return result
+
+    def reset(self):
+        try:
+            getattr(self, cachename).clear()
+        except AttributeError:
+            pass
+
+    wrapper._reset = reset
+    return wrapper
```

### Comparing `bfg9000-0.6.0/bfg9000/options.py` & `bfg9000-0.7.0/bfg9000/options.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,14 @@
 import enum
 from collections import namedtuple
 
-try:
-    from enum import Flag
-except ImportError:
-    from enum import IntEnum as Flag
-
 from . import path, safe_str
 from .iterutils import isiterable
 from .file_types import *
-from .platforms.framework import Framework
+from .packages import Framework
 
 
 class option_list:
     def __init__(self, *args):
         self._options = []
         self.collect(*args)
 
@@ -196,15 +191,15 @@
 
 
 class OptionEnum(enum.Enum):
     def __repr__(self):
         return self.name
 
 
-class OptionFlag(Flag):
+class OptionFlag(enum.Flag):
     def __repr__(self):
         return self.name
 
 
 def option(name, fields=[]):
     return type(name, (Option,), {'_fields': fields})
```

### Comparing `bfg9000-0.6.0/bfg9000/packages.py` & `bfg9000-0.7.0/bfg9000/packages.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,10 @@
-try:
-    from enum import EnumMeta as _EnumMeta, Flag as _Flag
-except ImportError:
-    from enum import EnumMeta as _EnumMeta, IntEnum as _Flag
+from enum import EnumMeta as _EnumMeta, Flag as _Flag
 
 from .iterutils import listify as _listify
-from .options import option_list as _option_list
-from .platforms.framework import Framework  # noqa
 
 
 class _PackageKindMeta(_EnumMeta):
     def __getitem__(cls, name):
         try:
             return _EnumMeta.__getitem__(cls, name)
         except KeyError:
@@ -24,15 +19,19 @@
     shared = 2
     any = static | shared
 
 
 class Package:
     is_package = True
 
-    def __init__(self, name, format, deps=None):
+    def __init__(self, name, submodules=None, *, format, deps=None):
+        submodules = _listify(submodules)
+        if submodules:
+            name = '{}[{}]'.format(name, ','.join(submodules))
+
         self.name = name
         self.format = format
         self.deps = _listify(deps)
 
     def __hash__(self):
         return hash(self.name)
 
@@ -46,17 +45,42 @@
     def __repr__(self):
         return '<{type} {name}>'.format(
             type=type(self).__name__, name=repr(self.name)
         )
 
 
 class CommonPackage(Package):
-    def __init__(self, name, format, compile_options=None, link_options=None):
-        super().__init__(name, format)
-        self._compile_options = compile_options or _option_list()
-        self._link_options = link_options or _option_list()
+    def __init__(self, name, submodules=None, version=None, *, format,
+                 compile_options=None, link_options=None):
+        super().__init__(name, submodules, format=format)
+        self.version = version
+
+        # Import this here to avoid circular import.
+        from .options import option_list
+        self._compile_options = compile_options or option_list()
+        self._link_options = link_options or option_list()
 
-    def compile_options(self, compiler):
+    def compile_options(self, compiler, *, raw=False):
         return self._compile_options
 
-    def link_options(self, linker):
+    def link_options(self, linker, *, raw=False):
         return self._link_options
+
+
+class Framework:
+    # A reference to a macOS framework. Can be used in place of Library objects
+    # within a Package.
+
+    def __init__(self, name, suffix=None):
+        self.name = name
+        self.suffix = suffix
+
+    @property
+    def full_name(self):
+        return self.name + ',' + self.suffix if self.suffix else self.name
+
+    def __eq__(self, rhs):
+        return (type(self) == type(rhs) and self.name == rhs.name and
+                self.suffix == rhs.suffix)
+
+    def __ne__(self, rhs):
+        return not (self == rhs)
```

### Comparing `bfg9000-0.6.0/bfg9000/path.py` & `bfg9000-0.7.0/bfg9000/path.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import functools
 import os
 from contextlib import contextmanager
 
-from .platforms.basepath import BasePath, Root, InstallRoot, DestDir  # noqa
+from .platforms.basepath import (BasePath, Root, InstallRoot,  # noqa: F401
+                                 DestDir)
 from .platforms.host import platform_info
 
 Path = platform_info().Path
 
 
 def abspath(path, type=Path, **kwargs):
     return type.abspath(path, **kwargs)
```

### Comparing `bfg9000-0.6.0/bfg9000/platforms/basepath.py` & `bfg9000-0.7.0/bfg9000/platforms/basepath.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from itertools import chain
 
 from .. import safe_str
 from ..objutils import objectify
 
 Root = Enum('Root', ['srcdir', 'builddir', 'absolute'])
 InstallRoot = Enum('InstallRoot', ['prefix', 'exec_prefix', 'bindir', 'libdir',
-                                   'includedir'])
+                                   'includedir', 'datadir', 'mandir'])
 DestDir = Enum('DestDir', ['destdir'])
 
 
 class BasePath(safe_str.safe_string):
     __slots__ = ['destdir', 'root', 'suffix']
 
     curdir = posixpath.curdir
@@ -75,20 +75,18 @@
         if strict and result.root != raw_root:
             raise ValueError('expected root of {!r}, but got {!r}'
                              .format(raw_root.name, result.root.name))
         return result
 
     @staticmethod
     def __normpath(path):
-        # A path counts as a directory if either its raw form or its normalized
-        # form ends with `\` or `/`.
         path = path.replace('\\', '/')
-        isdir = path.endswith(posixpath.sep)
+        isdir = posixpath.basename(path) in ('', posixpath.curdir,
+                                             posixpath.pardir)
         path = posixpath.normpath(path)
-        isdir = isdir or path.endswith(posixpath.sep)
         if path == posixpath.curdir:
             path = ''
         return path, isdir
 
     @classmethod
     def __normalize(cls, path, expand_user=False):
         if expand_user:
@@ -101,16 +99,16 @@
         path, isdir = cls.__normpath(path)
         return drive, path, isdir
 
     @classmethod
     def __join(cls, path1, path2):
         return cls.__normpath(posixpath.join(path1, path2))
 
-    def __localize(self, thing):
-        if isinstance(thing, str):
+    def __localize(self, thing, localize=True):
+        if localize and isinstance(thing, str):
             return self._localize_path(thing)
         return thing
 
     def cross(self, env):
         cls = env.target_platform.Path
         return cls(self.suffix, self.root, False, self.directory)
 
@@ -156,46 +154,47 @@
         return self.suffix.split(posixpath.sep) if self.suffix else []
 
     def basename(self):
         return posixpath.basename(self.suffix)
 
     def relpath(self, start, prefix='', localize=True):
         if self.root == Root.absolute:
-            return self.__localize(self.suffix) if localize else self.suffix
+            return self.__localize(self.suffix, localize)
         if self.root != start.root:
             raise ValueError('source mismatch')
 
         rel = posixpath.relpath(self.suffix or posixpath.curdir,
                                 start.suffix or posixpath.curdir)
         if prefix and rel == posixpath.curdir:
             return prefix
         result = posixpath.join(prefix, rel)
-        return self.__localize(result) if localize else result
+        return self.__localize(result, localize)
 
     def reroot(self, root=Root.builddir):
         return type(self)(self.suffix, root, self.destdir, self.directory)
 
     def to_json(self):
         suffix = self.suffix
         if self.directory and not suffix.endswith(posixpath.sep):
             if suffix:
                 suffix += posixpath.sep
             else:
                 suffix = posixpath.curdir + posixpath.sep
-        return (suffix, self.root.name, self.destdir)
+        return [suffix, self.root.name, self.destdir]
 
     @classmethod
     def from_json(cls, data):
         try:
             base = Root[data[1]]
         except KeyError:
             base = InstallRoot[data[1]]
         return cls(data[0], base, data[2])
 
-    def realize(self, variables, executable=False, variable_sep=True):
+    def realize(self, variables, executable=False, variable_sep=True,
+                localize=True):
         if self.root == Root.absolute:
             variable_sep = False
             root = None
         else:
             root = variables[self.root]
 
         if executable and root is None and posixpath.sep not in self.suffix:
@@ -203,24 +202,25 @@
 
         # Not all platforms (e.g. Windows) support $(DESTDIR), so only emit the
         # destdir variable if it's defined.
         if self.destdir and DestDir.destdir in variables:
             destdir = variables[DestDir.destdir]
             root = destdir if root is None else destdir + root
         if root is None:
-            return self.__localize(self.suffix or posixpath.curdir)
+            return self.__localize(self.suffix or posixpath.curdir, localize)
         if not self.suffix:
-            return self.__localize(root)
+            return self.__localize(root, localize)
 
         # Join the separator and the suffix first so that we don't end up with
         # unnecessarily-escaped backslashes on Windows. (It doesn't hurt
         # anything; it just looks weird.)
         suffix = (posixpath.sep + self.suffix if variable_sep else
                   self.suffix)
-        return self.__localize(root) + self.__localize(suffix)
+        return (self.__localize(root, localize) +
+                self.__localize(suffix, localize))
 
     def string(self, variables=None):
         path = self
         result = ''
 
         while True:
             real = path.realize(variables)
@@ -233,16 +233,16 @@
                 result = real + result
                 break
 
         return result
 
     def __repr__(self):
         s = self.realize(self.__repr_variables)
-        if self.directory and not s.endswith(posixpath.sep):
-            s += posixpath.sep
+        if self.directory and not s.endswith(self._localized_sep):
+            s += self._localized_sep
         return '`{}`'.format(s)
 
     def __hash__(self):
         return hash(self.suffix)
 
     def __eq__(self, rhs):
         if type(self) is not type(rhs):
```

### Comparing `bfg9000-0.6.0/bfg9000/platforms/core.py` & `bfg9000-0.7.0/bfg9000/platforms/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
+import importlib_metadata as metadata
 import platform
 import re
 import subprocess
 from collections import namedtuple
-from pkg_resources import get_entry_info
 
 from ..objutils import memoize
 from ..versioning import SpecifierSet, Version
 
 __all__ = ['known_native_object_formats', 'known_platforms', 'parse_triplet',
            'Platform', 'PlatformTriplet', 'platform_name', 'platform_tuple']
 
@@ -131,20 +131,21 @@
 
     def __ne__(self, rhs):
         return not self == rhs
 
 
 @memoize
 def _get_platform_info(kind, genus, species, arch):
-    entry_point = 'bfg9000.platforms.{}'.format(kind)
-    entry = get_entry_info('bfg9000', entry_point, genus)
-    if entry is None:
+    eps = metadata.entry_points(group='bfg9000.platforms.{}'.format(kind))
+    try:
+        entry = eps[genus]
+    except KeyError:
         # Fall back to a generic POSIX system if we don't recognize the
         # platform name.
-        entry = get_entry_info('bfg9000', entry_point, 'posix')
+        entry = eps['posix']
     return entry.load()(genus, species, arch)
 
 
 def _platform_info(kind, name=None, arch=None):
     if name is None:
         name = platform_name()
     if arch is None:
```

### Comparing `bfg9000-0.6.0/bfg9000/platforms/cygwin.py` & `bfg9000-0.7.0/bfg9000/platforms/cygwin.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.6.0/bfg9000/platforms/posix.py` & `bfg9000-0.7.0/bfg9000/platforms/posix.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 from .basepath import BasePath, Root, InstallRoot
 from .core import Platform
-from .framework import Framework
 from .host import HostPlatform
 from .target import TargetPlatform
 
 
 class PosixPath(BasePath):
+    _localized_sep = BasePath.sep
+
     def _localize_path(self, path):
         return path
 
 
 class PosixPlatform(Platform):
     Path = PosixPath
 
@@ -53,20 +54,14 @@
 
     @property
     def has_path_ext(self):
         return False
 
 
 class PosixTargetPlatform(TargetPlatform, PosixPlatform):
-    _package_map = {
-        'gl': 'GL',
-        'glu': 'GLU',
-        'zlib': 'z',
-    }
-
     @property
     def executable_ext(self):
         return ''
 
     @property
     def shared_library_ext(self):
         return '.so'
@@ -88,34 +83,30 @@
         IRoot = InstallRoot
         return {
             IRoot.prefix     : PosixPath('/usr/local/', Root.absolute),
             IRoot.exec_prefix: PosixPath('', IRoot.prefix),
             IRoot.bindir     : PosixPath('bin/', IRoot.exec_prefix),
             IRoot.libdir     : PosixPath('lib/', IRoot.exec_prefix),
             IRoot.includedir : PosixPath('include/', IRoot.prefix),
+            IRoot.datadir    : PosixPath('share/', IRoot.prefix),
+            IRoot.mandir     : PosixPath('man/', IRoot.datadir),
         }
 
 
 class DarwinPlatform(PosixPlatform):
     @property
     def object_format(self):
         return 'mach-o'
 
 
 class DarwinHostPlatform(PosixHostPlatform, DarwinPlatform):
     pass
 
 
 class DarwinTargetPlatform(PosixTargetPlatform, DarwinPlatform):
-    _package_map = {
-        'gl': Framework('OpenGL'),
-        'glu': Framework('OpenGL'),
-        'glut': Framework('GLUT'),
-    }
-
     @property
     def shared_library_ext(self):
         return '.dylib'
 
     @property
     def has_frameworks(self):
         return True
```

### Comparing `bfg9000-0.6.0/bfg9000/platforms/windows.py` & `bfg9000-0.7.0/bfg9000/platforms/windows.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 from .basepath import BasePath, InstallRoot
 from .core import Platform
 from .host import HostPlatform
 from .target import TargetPlatform
 
 
 class WindowsPath(BasePath):
+    _localized_sep = '\\'
+
     def _localize_path(self, path):
-        return path.replace('/', '\\')
+        return path.replace(self.sep, self._localized_sep)
 
 
 class WindowsPlatform(Platform):
     Path = WindowsPath
 
     @property
     def _triplet_sys_abi(self):
@@ -40,20 +42,14 @@
 
     @property
     def has_path_ext(self):
         return True
 
 
 class WindowsTargetPlatform(TargetPlatform, WindowsPlatform):
-    _package_map = {
-        'gl': 'opengl32',
-        'glu': 'glu32',
-        'glut': 'glut32',
-    }
-
     @property
     def executable_ext(self):
         return '.exe'
 
     @property
     def shared_library_ext(self):
         return '.dll'
@@ -74,8 +70,10 @@
     def install_dirs(self):
         return {
             InstallRoot.prefix     : None,
             InstallRoot.exec_prefix: WindowsPath('', InstallRoot.prefix),
             InstallRoot.bindir     : WindowsPath('', InstallRoot.exec_prefix),
             InstallRoot.libdir     : WindowsPath('', InstallRoot.exec_prefix),
             InstallRoot.includedir : WindowsPath('', InstallRoot.prefix),
+            InstallRoot.datadir    : WindowsPath('', InstallRoot.prefix),
+            InstallRoot.mandir     : WindowsPath('man/', InstallRoot.datadir),
         }
```

### Comparing `bfg9000-0.6.0/bfg9000/rccdep.py` & `bfg9000-0.7.0/bfg9000/rccdep.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,16 +21,16 @@
     return subprocess.run(subcmd + ['-o', output]).returncode
 
 
 def main():
     parser = argparse.ArgumentParser(
         prog='bfg9000-rccdep',
         usage='%(prog)s SUBCMD -o FILE -d FILE',
-        description="Write a depfile (in Makefile syntax) for Qt's rcc " +
-                    "tool, and then run rcc."
+        description=("Write a depfile (in Makefile syntax) for Qt's rcc " +
+                     'tool, and then run rcc.')
     )
     parser.add_argument('--version', action='version',
                         version='%(prog)s ' + version)
     parser.add_argument('-o', '--output', required=True, metavar='FILE',
                         help='the output file for rcc (required)')
     parser.add_argument('-d', '--depfile', required=True, metavar='FILE',
                         help='the depfile to generate (required)')
```

### Comparing `bfg9000-0.6.0/bfg9000/safe_str.py` & `bfg9000-0.7.0/bfg9000/safe_str.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.6.0/bfg9000/shell/__init__.py` & `bfg9000-0.7.0/bfg9000/shell/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,41 +1,45 @@
 import os
 import subprocess
 from enum import Enum
 
-from .list import shell_list  # noqa
-from ..iterutils import listify
+from .. import iterutils
+from .list import shell_list  # noqa: F401
 from ..path import BasePath, Path
 from ..platforms.host import platform_info
 from ..safe_str import jbos, safe_str
 
 if platform_info().family == 'windows':
-    from .windows import *  # noqa
+    from .windows import *  # noqa: F401
 else:
-    from .posix import *  # noqa
+    from .posix import *  # noqa: F401
 
 CalledProcessError = subprocess.CalledProcessError
 
 
 class Mode(Enum):
     normal = None
     pipe = subprocess.PIPE
     stdout = subprocess.STDOUT
     devnull = subprocess.DEVNULL
 
 
 def split_paths(s, sep=os.pathsep):
-    if not s:
+    if s is None:
         return []
-    return s.split(sep)
+    return [i for i in s.split(sep) if i]
+
+
+def join_paths(paths, sep=os.pathsep):
+    return sep.join(paths)
 
 
 def which(names, env=os.environ, base_dirs=None, resolve=False,
           kind='executable'):
-    names = listify(names)
+    names = iterutils.listify(names)
     if len(names) == 0:
         raise TypeError('must supply at least one name')
 
     paths = split_paths(env.get('PATH', os.defpath))
     exts = ['']
     if platform_info().has_path_ext:
         exts.extend(split_paths(env.get('PATHEXT', '')))
@@ -86,15 +90,15 @@
 
     proc = subprocess.run(
         args, universal_newlines=True, shell=shell, env=env,
         stdout=conv_mode(stdout), stderr=conv_mode(stderr)
     )
     if not (returncode == 'any' or
             (returncode == 'fail' and proc.returncode != 0) or
-            proc.returncode in listify(returncode)):
+            proc.returncode in iterutils.listify(returncode)):
         raise CalledProcessError(proc.returncode, proc.args, proc.stdout,
                                  proc.stderr)
 
     if stdout == Mode.pipe:
         if stderr == Mode.pipe:
             return proc.stdout, proc.stderr
         return proc.stdout
```

### Comparing `bfg9000-0.6.0/bfg9000/shell/list.py` & `bfg9000-0.7.0/bfg9000/shell/list.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.6.0/bfg9000/shell/posix.py` & `bfg9000-0.7.0/bfg9000/shell/posix.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 from ..safe_str import jbos, safe_str, shell_literal
 
 __all__ = ['split', 'join', 'listify', 'inner_quote', 'inner_quote_info',
            'wrap_quotes', 'quote_info', 'quote', 'force_quote', 'escape_line',
            'join_lines', 'local_env', 'global_env']
 
 _bad_chars = re.compile(r'[^\w@%+=:,./-]')
-_ends_unescaped_quote = re.compile(r"(^|[^\\])(\\\\)*'$")
 
 
 def split(s, type=list, escapes=False):
     if not isinstance(s, str):
         raise TypeError('expected a string')
     lexer = shlex(s, posix=True)
     lexer.commenters = ''
@@ -33,17 +32,23 @@
 def listify(thing, type=list):
     if isinstance(thing, str):
         return split(thing, type)
     return iterutils.listify(thing, type=type)
 
 
 def inner_quote_info(s):
-    if _bad_chars.search(s):
-        return s.replace("'", r"'\''"), True
-    return s, False
+    if isinstance(s, shell_literal):
+        return s.string, False
+    elif isinstance(s, str):
+        if s == '':
+            return '', True
+        elif _bad_chars.search(s):
+            return s.replace("'", r"'\''"), True
+        return s, False
+    raise TypeError(type(s))
 
 
 def inner_quote(s):
     return inner_quote_info(s)[0]
 
 
 def wrap_quotes(s):
@@ -52,20 +57,27 @@
 
     # Any string less than 3 characters long can't have escaped quotes.
     if len(s) < 3:
         return "'" + s + "'"
 
     start = 1 if s[0] == "'" else None
     # Thanks to `inner_quote_info` above, we can guarantee that any single-
-    # quotes are unescaped, so we can deduplicate them if they're at the end.
+    # quotes at the end are unescaped, so we can deduplicate them if so.
     end = -1 if s[-1] == "'" else None
     return q(start) + s[start:end] + q(end)
 
 
 def quote_info(s):
+    if isinstance(s, jbos):
+        result, escaped = '', False
+        for i in s.bits:
+            r, e = quote_info(i)
+            result += r
+            escaped |= e
+        return result, escaped
     s, quoted = inner_quote_info(s)
     return (wrap_quotes(s), True) if quoted else (s, False)
 
 
 def quote(s):
     return quote_info(s)[0]
```

### Comparing `bfg9000-0.6.0/bfg9000/shell/syntax.py` & `bfg9000-0.7.0/bfg9000/shell/syntax.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,16 +7,17 @@
 from .. import safe_str
 from ..shell import posix as pshell
 
 Syntax = Enum('Syntax', ['variable', 'shell'])
 
 
 class Writer:
-    def __init__(self, stream):
+    def __init__(self, stream, localize_paths=True):
         self.stream = stream
+        self.localize_paths = localize_paths
 
     def write_literal(self, string):
         self.stream.write(string)
 
     def write(self, thing, syntax, shell_quote=pshell.quote_info):
         thing = safe_str.safe_str(thing)
         shelly = syntax == Syntax.shell
@@ -30,15 +31,16 @@
                 thing, escaped = shell_quote(thing)
             self.write_literal(thing)
         elif isinstance(thing, safe_str.jbos):
             for i in thing.bits:
                 escaped |= self.write(i, syntax, shell_quote)
         elif isinstance(thing, path.BasePath):
             out = Writer(StringIO())
-            thing = thing.realize(path_vars, shelly)
+            thing = thing.realize(path_vars, shelly,
+                                  localize=self.localize_paths)
             escaped = out.write(thing, syntax, pshell.inner_quote_info)
 
             thing = out.stream.getvalue()
             if shelly and escaped:
                 thing = pshell.wrap_quotes(thing)
             self.write_literal(thing)
         else:
```

### Comparing `bfg9000-0.6.0/bfg9000/shell/windows.py` & `bfg9000-0.7.0/bfg9000/shell/windows.py`

 * *Files 11% similar despite different names*

```diff
@@ -8,17 +8,16 @@
 from ..safe_str import jbos, safe_str, shell_literal
 
 __all__ = ['split', 'join', 'listify', 'inner_quote', 'inner_quote_info',
            'wrap_quotes', 'quote_info', 'quote', 'force_quote', 'escape_line',
            'join_lines', 'global_env']
 
 # XXX: We need a way to escape cmd.exe-specific characters.
-_bad_chars = re.compile(r'(\s|"|\\$)')
+_bad_chars = re.compile(r'(\s|["&<>|]|\\$)')
 _replace = re.compile(r'(\\*)("|$)')
-_ends_unescaped_quote = re.compile(r'(^|[^\\])(\\\\)*"$')
 
 _Token = Enum('Token', ['char', 'quote', 'space'])
 _State = Enum('State', ['between', 'char', 'word', 'quoted'])
 
 
 def _tokenize(s):
     escapes = 0
@@ -76,41 +75,55 @@
 def listify(thing, type=list):
     if isinstance(thing, str):
         return split(thing, type)
     return iterutils.listify(thing, type=type)
 
 
 def inner_quote_info(s, escape_percent=False):
-    # In some contexts (mainly certain uses of the Windows shell), we want to
-    # escape percent signs. This doesn't count as "escaping" for the purposes
-    # of quoting the result though.
-    if escape_percent:
-        s = s.replace('%', '%%')
-
-    if not _bad_chars.search(s):
-        return s, False
-
-    def repl(m):
-        quote = '\\' + m.group(2) if len(m.group(2)) else ''
-        return m.group(1) * 2 + quote
-    return _replace.sub(repl, s), True
+    if isinstance(s, shell_literal):
+        return s.string, False
+    elif isinstance(s, str):
+        if s == '':
+            return '', True
+
+        # In some contexts (mainly certain uses of the Windows shell), we want
+        # to escape percent signs. This doesn't count as "escaping" for the
+        # purposes of quoting the result though.
+        if escape_percent:
+            s = s.replace('%', '%%')
+
+        if not _bad_chars.search(s):
+            return s, False
+
+        def repl(m):
+            quote = '\\' + m.group(2) if len(m.group(2)) else ''
+            return m.group(1) * 2 + quote
+        return _replace.sub(repl, s), True
+    raise TypeError(type(s))
 
 
 def inner_quote(s, escape_percent=False):
     return inner_quote_info(s, escape_percent)[0]
 
 
 def wrap_quotes(s):
     # Thanks to `inner_quote_info` above, we can guarantee that any double-
     # quotes are escaped, so we don't need to worry about duplicates if they're
     # at the end.
     return '"' + s + '"'
 
 
 def quote_info(s, escape_percent=False):
+    if isinstance(s, jbos):
+        result, escaped = '', False
+        for i in s.bits:
+            r, e = quote_info(i)
+            result += r
+            escaped |= e
+        return result, escaped
     s, quoted = inner_quote_info(s, escape_percent)
     return (wrap_quotes(s), True) if quoted else (s, False)
 
 
 def quote(s, escape_percent=False):
     return quote_info(s, escape_percent)[0]
```

### Comparing `bfg9000-0.6.0/bfg9000/tools/__init__.py` & `bfg9000-0.7.0/bfg9000/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.6.0/bfg9000/tools/ar.py` & `bfg9000-0.7.0/bfg9000/tools/ar.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import os
 from itertools import chain
 
 from .. import options as opts, safe_str, shell
 from .common import library_macro, SimpleBuildCommand
 from ..file_types import StaticLibrary
 from ..iterutils import iterate
-from ..objutils import memoize
+from ..objutils import memoize_method
 from ..path import Path
 from ..versioning import detect_version
 
 
 class ArLinker(SimpleBuildCommand):
-    @memoize
+    @memoize_method
     def _check_version(self):
         try:
             output = self.env.execute(
                 self.command + ['--version'], stdout=shell.Mode.pipe,
                 stderr=shell.Mode.devnull
             )
             if 'GNU ar' in output:
```

### Comparing `bfg9000-0.6.0/bfg9000/tools/c_family.py` & `bfg9000-0.7.0/bfg9000/tools/c_family.py`

 * *Files 10% similar despite different names*

```diff
@@ -60,15 +60,17 @@
 _windows_cmds = {
     'c'     : ['cl', 'clang-cl', 'cc', 'gcc', 'clang'],
     'c++'   : ['cl', 'clang-cl', 'c++', 'g++', 'clang++'],
     'objc'  : ['cc', 'gcc', 'clang'],
     'objc++': ['c++', 'g++', 'clang++'],
 }
 
-_builders = (cc.CcBuilder, msvc.MsvcBuilder)
+_builders = (msvc.MsvcBuilder, cc.CcBuilder)
+_fallback_posix_builder = cc.CcBuilder
+_fallback_windows_builder = msvc.MsvcBuilder
 
 
 def _guess_candidates(env, lang):
     def is_cxx_based(lang):
         return lang.endswith('c++')
 
     candidates = []
@@ -84,41 +86,48 @@
             if cmd is not None:
                 candidates.append(_guessed_info(i, sibling_cmd, cmd))
     return candidates
 
 
 @builder('c', 'c++', 'objc', 'objc++')
 def c_family_builder(env, lang):
+    if env.host_platform.family == 'windows':
+        candidates = _windows_cmds[lang]
+        fallback = _fallback_windows_builder
+    else:
+        candidates = _posix_cmds[lang]
+        fallback = _fallback_posix_builder
+
     langinfo = known_langs[lang]
     cmd = env.getvar(langinfo.var('compiler'))
     if cmd:
-        return choose_builder(env, langinfo, _builders, candidates=cmd)
+        return choose_builder(env, langinfo, _builders, candidates=cmd,
+                              fallback_builder=fallback)
 
     # We don't have an explicitly-set command from the environment, so try to
     # guess what the right command would be.
-
-    candidates = (_windows_cmds[lang] if env.host_platform.family == 'windows'
-                  else _posix_cmds[lang])
     guessed_info = _guess_candidates(env, lang)
 
     # If the last guessed command is the same as the first default command
     # candidate, remove it. This will keep us from logging a useless info
     # message that we guessed the default value for the command.
     if guessed_info and guessed_info[-1].guessed_cmd == candidates[0]:
         del guessed_info[-1]
 
     for sibling_lang, sibling_cmd, guessed_cmd in guessed_info:
         try:
             builder = choose_builder(env, langinfo, _builders,
-                                     candidates=guessed_cmd, strict=True)
+                                     candidates=guessed_cmd,
+                                     fallback_builder=fallback, strict=True)
             log.info('guessed {} compiler {!r} from {} compiler {!r}'.format(
                 lang, guessed_cmd, sibling_lang, sibling_cmd
             ))
             return builder
         except IOError:
             pass
 
     # Try all the default command candidates we haven't already tried above.
     guesses = [i.guessed_cmd for i in guessed_info]
     untried_candidates = [i for i in candidates if i not in guesses]
     return choose_builder(env, langinfo, _builders,
-                          candidates=untried_candidates)
+                          candidates=untried_candidates,
+                          fallback_builder=fallback)
```

### Comparing `bfg9000-0.6.0/bfg9000/tools/cc/__init__.py` & `bfg9000-0.7.0/bfg9000/tools/jvm.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,266 +1,369 @@
 import os
 import re
 from itertools import chain
 
-from .. import pkg_config
-from ... import log, options as opts, shell
-from .compiler import CcCompiler, CcPchCompiler
-from .linker import CcExecutableLinker, CcSharedLibraryLinker
-from .rc import CcRcBuilder  # noqa: F401
-from ..ar import ArLinker
-from ..common import Builder, check_which
-from ..ld import LdLinker
-from ...exceptions import PackageResolutionError
-from ...file_types import (HeaderDirectory, Library, LinkLibrary,
-                           SharedLibrary, StaticLibrary)
-from ...iterutils import default_sentinel, iterate, uniques
-from ...languages import known_formats
-from ...packages import CommonPackage, Framework, PackageKind
-from ...path import exists, Root
-from ...platforms import parse_triplet
-from ...versioning import detect_version
-
-
-class CcBuilder(Builder):
-    def __init__(self, env, langinfo, command, version_output):
-        brand, version, target_flags = self._parse_brand(env, command,
-                                                         version_output)
-        super().__init__(langinfo.name, brand, version)
-        self.object_format = env.target_platform.object_format
+from .common import (BuildCommand, Builder, check_which, not_buildroot,
+                     SimpleBuildCommand)
+from .. import log, options as opts, safe_str, shell
+from ..builtins.file_types import make_immediate_file
+from ..exceptions import PackageResolutionError
+from ..file_types import *
+from ..iterutils import flatten, iterate, uniques
+from ..languages import known_formats
+from ..packages import Package
+from ..path import Path, Root
+from ..versioning import detect_version
+
+_warning_flags = {
+    'java': {
+        opts.WarningValue.disable: '-nowarn',
+        opts.WarningValue.error: '-Werror',
+        opts.WarningValue.all: '-Xlint:all',
+    },
+    'scala': {
+        opts.WarningValue.disable: '-nowarn',
+        opts.WarningValue.error: '-Xfatal-errors',
+        opts.WarningValue.all: '-Xlint:_',
+    },
+}
+
+
+class JvmBuilder(Builder):
+    def __init__(self, env, langinfo, command, found, version_output):
+        # The default command name to run JVM programs is (usually) the same as
+        # the name of the language, so we'll just use that here as the default.
+        run_name = langinfo.var('runner').lower()
+        run_command, run_found = check_which(
+            env.getvar(langinfo.var('runner'), langinfo.name),
+            kind='{} runner'.format(langinfo.name)
+        )
+
+        super().__init__(langinfo.name, *self._parse_brand(
+            env, langinfo.name, version_output, run_command
+        ))
+        self.object_format = 'jvm'
 
         name = langinfo.var('compiler').lower()
-        ldinfo = known_formats['native']['dynamic']
-        arinfo = known_formats['native']['static']
+        ldinfo = known_formats['jvm']['dynamic']
 
-        # Try to infer the appropriate -fuse-ld option from the LD environment
-        # variable.
-        link_command = command[:]
-        ld_command = env.getvar(ldinfo.var('linker'))
-        if ld_command:
-            tail = os.path.splitext(ld_command)[1][1:]
-            if tail in ['bfd', 'gold']:
-                log.info('setting `-fuse-ld={}` for `{}`'
-                         .format(tail, shell.join(command)))
-                link_command.append('-fuse-ld={}'.format(tail))
-
-        cflags_name = langinfo.var('flags').lower()
-        cflags = (target_flags +
-                  shell.split(env.getvar('CPPFLAGS', '')) +
-                  shell.split(env.getvar(langinfo.var('flags'), '')))
-
-        ldflags_name = ldinfo.var('flags').lower()
-        ldflags = (target_flags +
-                   shell.split(env.getvar(ldinfo.var('flags'), '')))
-        ldlibs_name = ldinfo.var('libs').lower()
-        ldlibs = shell.split(env.getvar(ldinfo.var('libs'), ''))
-
-        ar_name = arinfo.var('linker').lower()
-        ar_command = check_which(env.getvar(arinfo.var('linker'), 'ar'),
-                                 env.variables, kind='static linker')
-        arflags_name = arinfo.var('flags').lower()
-        arflags = shell.split(env.getvar(arinfo.var('flags'), 'cr'))
-
-        # macOS's ld doesn't support --version, but we can still try it out and
-        # grab the command line.
-        ld_command = None
-        try:
-            stdout, stderr = env.execute(
-                command + ldflags + ['-v', '-Wl,--version'],
-                stdout=shell.Mode.pipe, stderr=shell.Mode.pipe,
-                returncode='any'
-            )
+        flags_name = langinfo.var('flags').lower()
+        flags = shell.split(env.getvar(langinfo.var('flags'), ''))
 
-            for line in stderr.split('\n'):
-                if '--version' in line:
-                    ld_command = shell.split(line)[0:1]
-                    if os.path.basename(ld_command[0]) != 'collect2':
-                        break
-        except (OSError, shell.CalledProcessError):
-            pass
+        jar_name = ldinfo.var('linker').lower()
+        jar_which = check_which(env.getvar(ldinfo.var('linker'), 'jar'),
+                                kind='jar builder')
+
+        jarflags_name = ldinfo.var('flags').lower()
+        jarflags = shell.split(env.getvar(ldinfo.var('flags'), 'cfm'))
+
+        self.compiler = JvmCompiler(
+            self, env, command=(name, command, found),
+            flags=(flags_name, flags)
+        )
+        self._linker = JarMaker(
+            self, env, command=(jar_name,) + jar_which,
+            flags=(jarflags_name, jarflags)
+        )
+        self.packages = JvmPackageResolver(self, env, run_command)
+        self.runner = JvmRunner(
+            self, env, command=(run_name, run_command, run_found)
+        )
 
-        compile_kwargs = {'command': (name, command),
-                          'flags': (cflags_name, cflags)}
-        self.compiler = CcCompiler(self, env, **compile_kwargs)
-        try:
-            self.pch_compiler = CcPchCompiler(self, env, **compile_kwargs)
-        except ValueError:
-            self.pch_compiler = None
-
-        link_kwargs = {'command': (name, link_command),
-                       'flags': (ldflags_name, ldflags),
-                       'libs': (ldlibs_name, ldlibs)}
-        self._linkers = {
-            'executable': CcExecutableLinker(self, env, **link_kwargs),
-            'shared_library': CcSharedLibraryLinker(self, env, **link_kwargs),
-            'static_library': ArLinker(
-                self, env, command=(ar_name, ar_command),
-                flags=(arflags_name, arflags)
-            ),
-        }
-        if ld_command:
-            self._linkers['raw'] = LdLinker(self, env, ld_command, stdout)
-
-        self.packages = CcPackageResolver(self, env, command, ldflags)
-        self.runner = None
-
-    @classmethod
-    def _parse_brand(cls, env, command, version_output):
-        target_flags = []
-        if 'Free Software Foundation' in version_output:
-            brand = 'gcc'
-            version = detect_version(version_output)
-            if env.is_cross:
-                triplet = parse_triplet(env.execute(
-                    command + ['-dumpmachine'],
-                    stdout=shell.Mode.pipe, stderr=shell.Mode.devnull
-                ).rstrip())
-                target_flags = cls._gcc_arch_flags(
-                    env.target_platform.arch, triplet.arch
+    @staticmethod
+    def _parse_brand(env, lang, version_output, run_command):
+        brand = 'unknown'
+        version = None
+        if lang == 'java':
+            try:
+                # Get the brand from the run command (rather than the compile
+                # command).
+                output = env.execute(
+                    run_command + ['-version'], stdout=shell.Mode.pipe,
+                    stderr=shell.Mode.stdout
                 )
-        elif 'clang' in version_output:
-            brand = 'clang'
+                if re.search(r'Java\(TM\) (\w+ )?Runtime Environment', output):
+                    brand = 'oracle'
+                elif 'OpenJDK Runtime Environment' in output:
+                    brand = 'openjdk'
+            except (OSError, shell.CalledProcessError):
+                pass
             version = detect_version(version_output)
-            if env.is_cross:
-                target_flags = ['-target', env.target_platform.triplet]
-        else:
-            brand = 'unknown'
-            version = None
+        elif lang == 'scala':
+            if 'EPFL' in version_output:
+                brand = 'epfl'
+                version = detect_version(version_output)
+        else:  # pragma: no cover
+            raise ValueError('unrecognized language {!r}'.format(lang))
 
-        return brand, version, target_flags
-
-    @staticmethod
-    def _gcc_arch_flags(arch, native_arch):
-        if arch == native_arch:
-            return []
-        elif arch == 'x86_64':
-            return ['-m64']
-        elif re.match(r'i.86$', arch):
-            return ['-m32'] if not re.match(r'i.86$', native_arch) else []
-        return []
+        return brand, version
 
     @staticmethod
     def check_command(env, command):
-        return env.execute(command + ['--version'], stdout=shell.Mode.pipe,
-                           stderr=shell.Mode.devnull)
+        return env.execute(command + ['-version'], stdout=shell.Mode.pipe,
+                           stderr=shell.Mode.stdout)
 
     @property
     def flavor(self):
-        return 'cc'
+        return 'jvm'
 
     @property
     def family(self):
-        return 'native'
+        return 'jvm'
 
     @property
-    def auto_link(self):
+    def can_dual_link(self):
         return False
 
+    def linker(self, mode):
+        if mode == 'static_library':
+            raise ValueError('static linking not supported with {}'.format(
+                self.brand
+            ))
+        if mode not in ('executable', 'shared_library'):
+            raise KeyError(mode)
+        return self._linker
+
+
+class JvmCompiler(SimpleBuildCommand):
     @property
-    def can_dual_link(self):
+    def deps_flavor(self):
+        return None
+
+    @property
+    def needs_libs(self):
         return True
 
-    def linker(self, mode):
-        return self._linkers[mode]
+    @property
+    def needs_package_options(self):
+        return True
+
+    @property
+    def accepts_pch(self):
+        return False
+
+    def _call(self, cmd, input, output, flags=None):
+        jvmoutput = self.env.tool('jvmoutput')
+        result = list(chain(
+            cmd, self._always_flags, iterate(flags), [input]
+        ))
+        return jvmoutput(output, result)
+
+    @property
+    def _always_flags(self):
+        return ['-verbose', '-d', '.']
+
+    def flags(self, options, global_options=None, output=None, mode='normal'):
+        flags, class_path = [], []
+        for i in options:
+            if isinstance(i, opts.lib):
+                class_path.append(i.library.path)
+            elif isinstance(i, opts.warning):
+                for j in i.value:
+                    try:
+                        flags.append(_warning_flags[self.lang][j])
+                    except KeyError:
+                        raise ValueError('unsupported warning level {!r}'
+                                         .format(j))
+            elif isinstance(i, opts.debug):
+                flags.append('-g' if self.lang == 'java' else '-g:vars')
+            elif isinstance(i, opts.optimize):
+                if ( self.lang == 'scala' and
+                     (opts.OptimizeValue.size in i.value or
+                      opts.OptimizeValue.speed in i.value) ):
+                    flags.append('-optimize')
+            elif isinstance(i, safe_str.stringy_types):
+                flags.append(i)
+            else:
+                raise TypeError('unknown option type {!r}'.format(type(i)))
 
+        if class_path:
+            flags.extend(['-cp', safe_str.join(uniques(class_path),
+                                               os.pathsep)])
+        return flags
 
-class CcPackageResolver:
-    def __init__(self, builder, env, command, ldflags):
+    def default_name(self, input, step):
+        return input.path.stripext().suffix
+
+    def output_file(self, name, step):
+        return ObjectFileList(Path(name + '.classlist'), Path(name + '.class'),
+                              self.builder.object_format, self.lang)
+
+
+class JarMaker(SimpleBuildCommand):
+    @property
+    def flavor(self):
+        return 'jar'
+
+    def can_link(self, format, langs):
+        return format == 'jvm'
+
+    @property
+    def needs_libs(self):
+        return False
+
+    @property
+    def needs_package_options(self):
+        return False
+
+    def post_output(self, context, options, output, step):
+        # Fix up paths for the Class-Path field: escape spaces and prefix
+        # Windows drive letters with '/' to disambiguate them from URLs.
+        def fix_path(p):
+            if self.env.target_platform.family == 'windows' and p[1] == ':':
+                p = '/' + p
+            return p.replace(' ', '%20')
+
+        libs = getattr(step, 'libs', []) + flatten(
+            i.libs for i in getattr(step, 'packages', [])
+        )
+        dirs = uniques(i.path for i in libs)
+        base = output.path.parent()
+
+        step.manifest = File(output.path.stripext('-manifest.txt'))
+        with make_immediate_file(context, step.manifest) as out:
+            classpath = ' '.join(fix_path(i.relpath(base, localize=False))
+                                 for i in dirs)
+            if classpath:
+                out.write('Class-Path: {}\n'.format(classpath))
+
+            entry_point = self._entry_point(options)
+            if entry_point:
+                out.write('Main-Class: {}\n'.format(entry_point))
+
+        return None
+
+    def _call(self, cmd, input, output, manifest, flags=None):
+        return list(chain(
+            cmd, iterate(flags), [output, manifest], iterate(input)
+        ))
+
+    def _entry_point(self, options):
+        filtered = options.filter(opts.entry_point) if options else None
+        if filtered:
+            return filtered[-1].value
+        return None
+
+    def transform_input(self, input):
+        return ['@' + safe_str.safe_str(i) if isinstance(i, ObjectFileList)
+                else i for i in input]
+
+    def flags(self, options, global_options=None, output=None, mode='normal'):
+        flags = []
+        for i in options:
+            if isinstance(i, safe_str.stringy_types):
+                flags.append(i)
+            elif isinstance(i, opts.debug):
+                pass
+            elif isinstance(i, opts.optimize):
+                pass
+            elif isinstance(i, opts.entry_point):
+                pass
+            elif isinstance(i, opts.gui):
+                pass
+            else:
+                raise TypeError('unknown option type {!r}'.format(type(i)))
+        return flags
+
+    def output_file(self, name, step):
+        options = getattr(step, 'options', None)
+        filetype = (ExecutableLibrary if self._entry_point(options)
+                    else Library)
+        return filetype(Path(name + '.jar'), self.builder.object_format,
+                        self.lang)
+
+
+class JvmPackage(Package):
+    def __init__(self, name, format, libs=None):
+        super().__init__(name, format=format)
+        self.libs = libs or []
+
+    def compile_options(self, compiler, *, raw=False):
+        return opts.option_list(opts.lib(i) for i in self.libs)
+
+    def link_options(self, linker, *, raw=False):
+        return opts.option_list()
+
+
+class JvmPackageResolver:
+    def __init__(self, builder, env, command):
         self.builder = builder
-        self.env = env
 
-        self.include_dirs = [i for i in uniques(chain(
-            self.builder.compiler.search_dirs(),
-            self.env.host_platform.include_dirs
-        )) if exists(i)]
+        if self.lang == 'scala':
+            extra_env = {'JAVA_OPTS': '-XshowSettings:properties'}
+            args = ['-version']
+            returncode = 1
+        else:
+            extra_env = None
+            args = ['-XshowSettings:properties', '-version']
+            returncode = 0
 
-        cc_lib_dirs = self.builder.linker('executable').search_dirs()
         try:
-            sysroot = self.builder.linker('executable').sysroot()
-            ld_lib_dirs = self.builder.linker('raw').search_dirs(sysroot, True)
-        except (KeyError, OSError, shell.CalledProcessError):
-            ld_lib_dirs = self.env.host_platform.lib_dirs
-
-        self.lib_dirs = [i for i in uniques(chain(
-            cc_lib_dirs, ld_lib_dirs, self.env.host_platform.lib_dirs
-        )) if exists(i)]
+            output = env.execute(
+                command + args, extra_env=extra_env, stdout=shell.Mode.devnull,
+                stderr=shell.Mode.pipe, returncode=returncode
+            )
+            self.ext_dirs = self._get_dirs('java.ext.dirs', output)
+            self.classpath = self._get_dirs('java.class.path', output)
+        except (OSError, shell.CalledProcessError):
+            self.ext_dirs = []
+            self.classpath = []
 
     @property
     def lang(self):
         return self.builder.lang
 
-    def header(self, name, search_dirs=None):
-        if search_dirs is None:
-            search_dirs = self.include_dirs
-
-        for base in search_dirs:
-            if base.root != Root.absolute:
-                raise ValueError('expected an absolute path')
-            if exists(base.append(name)):
-                return HeaderDirectory(base, None, system=True)
-
-        raise PackageResolutionError("unable to find header '{}'".format(name))
-
-    def library(self, name, kind=PackageKind.any, search_dirs=None):
-        if search_dirs is None:
-            search_dirs = self.lib_dirs
-
-        libnames = []
-        if kind & PackageKind.shared:
-            base = 'lib' + name + self.env.target_platform.shared_library_ext
-            if self.env.target_platform.has_import_library:
-                libnames.append((base + '.a', LinkLibrary, {}))
-            else:
-                libnames.append((base, SharedLibrary, {}))
-        if kind & PackageKind.static:
-            libnames.append(('lib' + name + '.a', StaticLibrary,
-                             {'lang': self.lang}))
-
-        # XXX: Include Cygwin here too?
-        if self.env.target_platform.family == 'windows':
-            # We don't actually know what kind of library this is. It could be
-            # a static library or an import library (which we classify as a
-            # kind of shared lib).
-            libnames.append((name + '.lib', Library, {}))
-
-        for base in search_dirs:
-            if base.root != Root.absolute:
-                raise ValueError('expected an absolute path')
-            for libname, libkind, extra_kwargs in libnames:
-                fullpath = base.append(libname)
-                if exists(fullpath):
-                    return libkind(fullpath, format=self.builder.object_format,
-                                   **extra_kwargs)
+    def _get_dirs(self, key, output):
+        ex = r'^(\s*){} = (.*(?:\n\1\s+.*)*)'.format(re.escape(key))
+        m = re.search(ex, output, re.MULTILINE)
+        if not m:
+            return []
+        return [i.strip() for i in m.group(2).split('\n')]
+
+    def _library(self, name):
+        jarname = name + '.jar'
+        for base in self.ext_dirs:
+            fullpath = os.path.join(base, jarname)
+            if os.path.exists(fullpath):
+                return Library(Path(fullpath, Root.absolute),
+                               self.builder.object_format)
+
+        for path in self.classpath:
+            if os.path.basename(path) == jarname and os.path.exists(path):
+                return Library(Path(path, Root.absolute),
+                               self.builder.object_format)
 
         raise PackageResolutionError("unable to find library '{}'"
                                      .format(name))
 
-    def resolve(self, name, version, kind, headers, lib_names):
-        format = self.builder.object_format
-        try:
-            return pkg_config.resolve(self.env, name, format, version, kind)
-        except (OSError, PackageResolutionError):
-            compile_options = opts.option_list()
-            link_options = opts.option_list()
-
-            compile_options.extend(opts.include_dir(self.header(i))
-                                   for i in iterate(headers))
-
-            lib_path = None
-            if lib_names is default_sentinel:
-                lib_names = self.env.target_platform.transform_package(name)
-            for i in iterate(lib_names):
-                if isinstance(i, Framework):
-                    link_options.append(opts.lib(i))
-                elif i == 'pthread':
-                    compile_options.append(opts.pthread())
-                    link_options.append(opts.pthread())
-                else:
-                    lib = self.library(i, kind)
-                    if not lib_path:
-                        lib_path = lib.path.parent().string()
-                    link_options.append(opts.lib(lib))
-
-            path_note = ' in {}'.format(lib_path) if lib_path else ''
-            log.info('found package {!r} via path-search{}'
-                     .format(name, path_note))
-            return CommonPackage(name, format, compile_options, link_options)
+    # TODO: Remove headers/libs from arguments after 0.7 is released.
+    def resolve(self, name, submodules, version, kind, *, headers=None,
+                libs=None, system=True):
+        lib = self._library(name)
+        pkg = JvmPackage(name, self.builder.object_format, libs=[lib])
+        log.info('found package {!r} via path-search in {!r}'
+                 .format(pkg.name, lib.path.parent().string()))
+        return pkg
+
+
+class JvmRunner(BuildCommand):
+    def __init__(self, builder, env, *, command):
+        super().__init__(builder, env, command=command)
+
+    def _call(self, cmd, file, cp=None, jar=False):
+        result = list(cmd)
+        if jar and self.lang != 'scala':
+            result.append('-jar')
+        if not_buildroot(cp):
+            result.extend(['-cp', cp])
+        result.append(file)
+        return result
+
+    def run_arguments(self, file):
+        if isinstance(file, Executable):
+            return self(file, jar=True)
+        elif isinstance(file, ObjectFileList):
+            return self.run_arguments(file.object_file)
+        elif isinstance(file, ObjectFile):
+            return self(file.path.stripext().basename(), cp=file.path.parent())
+        raise TypeError('expected an executable or object file for {} to run'
+                        .format(self.lang))
```

### Comparing `bfg9000-0.6.0/bfg9000/tools/cc/compiler.py` & `bfg9000-0.7.0/bfg9000/tools/cc/compiler.py`

 * *Files 3% similar despite different names*

```diff
@@ -44,30 +44,31 @@
             if self.brand == 'clang':
                 flags.append('-fcolor-diagnostics')
             elif (self.brand == 'gcc' and self.version and
                   self.version in SpecifierSet('>=4.9')):
                 flags.append('-fdiagnostics-color')
         return flags
 
-    def _include_dir(self, directory):
+    def _include_dir(self, directory, allow_system):
         is_default = directory.path in self.env.host_platform.include_dirs
 
         # Don't include default directories as system dirs (e.g. /usr/include).
         # Doing so would break GCC 6 when #including stdlib.h:
         # <https://gcc.gnu.org/bugzilla/show_bug.cgi?id=70129>.
-        if directory.system and not is_default:
+        if allow_system and directory.system and not is_default:
             return ['-isystem', directory.path]
         else:
             return ['-I' + directory.path]
 
     def flags(self, options, global_options=None, output=None, mode='normal'):
+        pkgconf_mode = mode == 'pkg-config'
         flags = []
         for i in options:
             if isinstance(i, opts.include_dir):
-                flags.extend(self._include_dir(i.directory))
+                flags.extend(self._include_dir(i.directory, not pkgconf_mode))
             elif isinstance(i, opts.define):
                 if i.value:
                     flags.append('-D' + i.name + '=' + i.value)
                 else:
                     flags.append('-D' + i.name)
             elif isinstance(i, opts.std):
                 flags.append('-std=' + i.value)
```

### Comparing `bfg9000-0.6.0/bfg9000/tools/cc/linker.py` & `bfg9000-0.7.0/bfg9000/tools/cc/linker.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,16 @@
 
         # Create a regular expression to extract the library name for linking
         # with -l.
         lib_formats = [r'lib(.*)\.a']
         if not self.env.target_platform.has_import_library:
             so_ext = re.escape(self.env.target_platform.shared_library_ext)
             lib_formats.append(r'lib(.*)' + so_ext)
+        if self.env.target_platform.family == 'windows':
+            lib_formats.append(r'(.*)\.lib')
         self._lib_re = re.compile('(?:' + '|'.join(lib_formats) + ')$')
 
     def _extract_lib_name(self, library):
         basename = library.path.basename()
         m = self._lib_re.match(basename)
         if not m:
             raise ValueError("'{}' is not a valid library name"
@@ -143,15 +145,15 @@
 
     def always_libs(self, primary):
         # XXX: Don't just asssume that these are the right libraries to use.
         # For instance, clang users might want to use libc++ instead.
         libs = opts.option_list()
         if self.lang in ('c++', 'objc++') and not primary:
             libs.append(opts.lib('stdc++'))
-        if self.lang in ('objc', 'objc++'):
+        if self.lang in ('objc', 'objc++') and self.brand == 'gcc':
             libs.append(opts.lib('objc'))
         if self.lang in ('f77', 'f95') and not primary:
             libs.append(opts.lib('gfortran'))
         if self.lang == 'java' and not primary:
             libs.append(opts.lib('gcj'))
         return libs
```

### Comparing `bfg9000-0.6.0/bfg9000/tools/cc/rc.py` & `bfg9000-0.7.0/bfg9000/tools/cc/rc.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 from ...iterutils import iterate
 from ...file_types import ObjectFile
 from ...path import Path
 from ...versioning import detect_version
 
 
 class CcRcBuilder(Builder):
-    def __init__(self, env, langinfo, command, version_output):
+    def __init__(self, env, langinfo, command, found, version_output):
         super().__init__(langinfo.name, *self._parse_brand(version_output))
 
         name = langinfo.var('compiler').lower()
         lflags_name = langinfo.var('flags').lower()
         lflags = shell.split(env.getvar(langinfo.var('flags'), ''))
 
         self.object_format = env.target_platform.object_format
-        self.compiler = CcRcCompiler(self, env, command=(name, command),
+        self.compiler = CcRcCompiler(self, env, command=(name, command, found),
                                      flags=(lflags_name, lflags))
 
     @staticmethod
     def _parse_brand(version_output):
         if 'Free Software Foundation' in version_output:
             return 'gcc', detect_version(version_output)
         return 'unknown', None
```

### Comparing `bfg9000-0.6.0/bfg9000/tools/common.py` & `bfg9000-0.7.0/bfg9000/tools/common.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,20 +24,26 @@
     )
 
 
 # Make a function to convert between command names for different languages in
 # the same family (e.g. # `gcc` => `g++`). If no entry in the mapping matches
 # the command, we return None to indicate that the conversion has failed.
 def make_command_converter(mapping):
-    sub = '|'.join(re.escape(i[0]) for i in mapping)
-    ex = re.compile(r'(?:^|(?<=\W))({})(?:$|(?=\W))'.format(sub))
-    d = dict(mapping)
+    def escape(i):
+        if isinstance(i, str):
+            return '({})'.format(re.escape(i))
+        if i.groups:
+            raise re.error('capturing groups not allowed')
+        return '({})'.format(i.pattern)
+
+    sub = '|'.join(escape(i[0]) for i in mapping)
+    ex = re.compile(r'(?:^|(?<=\W))(?:{})(?:$|(?=\W))'.format(sub))
 
     def fn(cmd):
-        s, n = ex.subn(lambda m: d[m.group(1)], cmd)
+        s, n = ex.subn(lambda m: mapping[m.lastindex - 1][1], cmd)
         return s if n > 0 else None
 
     return fn
 
 
 def make_command_converter_pair(mapping):
     inverse = [(v, k) for k, v in mapping]
@@ -59,15 +65,15 @@
     def __repr__(self):
         return '<{}({!r})>'.format(type(self).__name__, self.brand)
 
 
 class Command:
     def __init__(self, env, rule_name=None, *, command):
         self.env = env
-        self.command_var, self.command = command
+        self.command_var, self.command, self.found = command
         self.rule_name = rule_name or self.command_var
 
     @staticmethod
     def convert_args(args, conv):
         args = listify(args, scalar_ok=False)
         if not any(isinstance(i, Command) for i in args):
             return args
@@ -81,32 +87,33 @@
         return result
 
     def __call__(self, *args, cmd=None, **kwargs):
         cmd = listify(cmd or self)
         return self._call(cmd, *args, **kwargs)
 
     def run(self, *args, **kwargs):
-        run_kwargs = slice_dict(kwargs, ('env', 'extra_env'))
+        run_kwargs = slice_dict(kwargs, ('env', 'extra_env', 'stdout',
+                                         'stderr'))
+        run_kwargs.setdefault('stdout', shell.Mode.pipe)
+        if run_kwargs['stdout'] != shell.Mode.normal:
+            run_kwargs.setdefault('stderr', shell.Mode.devnull)
 
-        return self.env.execute(
-            self(*args, **kwargs), stdout=shell.Mode.pipe,
-            stderr=shell.Mode.devnull, **run_kwargs
-        )
+        return self.env.execute(self(*args, **kwargs), **run_kwargs)
 
     def __repr__(self):
         return '<{}({})>'.format(
             type(self).__name__, ', '.join(repr(i) for i in self.command)
         )
 
 
 class SimpleCommand(Command):
     def __init__(self, env, name, env_var, default, kind='executable'):
-        cmd = check_which(env.getvar(env_var, default), env.variables,
-                          kind=kind)
-        super().__init__(env, command=(name, cmd))
+        cmd, found = check_which(env.getvar(env_var, default),
+                                 env.variables, kind=kind)
+        super().__init__(env, command=(name, cmd, found))
 
 
 class BuildCommand(Command):
     def __init__(self, builder, env, rule_name=None, *, command, **kwargs):
         super().__init__(env, rule_name, command=command)
         self.builder = builder
 
@@ -151,46 +158,57 @@
 
 
 class SimpleBuildCommand(BuildCommand):
     def __init__(self, builder, env, *, command, flags):
         super().__init__(builder, env, command=command, flags=flags)
 
 
+def guess_command(sibling, converter):
+    for i in sibling.command:
+        guessed_cmd = converter(i)
+        if guessed_cmd is not None:
+            return guessed_cmd
+    return None
+
+
 def check_which(names, *args, **kwargs):
     names = listify(names)
     try:
-        return shell.which(names, *args, **kwargs)
+        return shell.which(names, *args, **kwargs), True
     except IOError as e:
         warnings.warn(str(e))
         # Assume the first name is the best choice.
-        return shell.listify(names[0])
+        return shell.listify(names[0]), False
 
 
 def choose_builder(env, langinfo, builders, *, candidates=None,
-                   default_candidates=None, strict=False):
+                   default_candidates=None, fallback_builder=None,
+                   strict=False):
     if candidates is None:
         candidates = env.getvar(langinfo.var('compiler'), default_candidates)
     candidates = listify(candidates)
 
     try:
         cmd = shell.which(candidates, env.variables,
                           kind='{} compiler'.format(langinfo.name))
+        found = True
     except IOError as e:
         if strict:
             raise
         warnings.warn(str(e))
         cmd = shell.listify(candidates[0])
-        builder_type = first(builders)
+        builder_type = fallback_builder or first(builders)
         output = ''
+        found = False
     else:
         for builder_type in builders:
             try:
                 output = builder_type.check_command(env, cmd)
                 break
             except Exception:
                 pass
         else:
             tried = ', '.join(repr(i) for i in iterate(candidates))
             raise IOError('no working {} compiler found; tried {}'
                           .format(langinfo.name, tried))
 
-    return builder_type(env, langinfo, cmd, output)
+    return builder_type(env, langinfo, cmd, found, output)
```

### Comparing `bfg9000-0.6.0/bfg9000/tools/copy_file.py` & `bfg9000-0.7.0/bfg9000/tools/copy_file.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from . import tool
 from .common import SimpleCommand
+from ..safe_str import shell_literal
+from ..shell import shell_list
 
 
 class LinkCommand(SimpleCommand):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
         lower_cmd = [i.lower() for i in self.command]
         self.flavor = 'mklink' if 'mklink' in lower_cmd else 'ln'
@@ -43,7 +45,16 @@
     def __init__(self, env):
         default = ('cmd /c copy' if env.host_platform.family == 'windows'
                    else 'cp -f')
         super().__init__(env, name='cp', env_var='CP', default=default)
 
     def _call(self, cmd, input, output):
         return cmd + [input, output]
+
+
+@tool('gzip')
+class Gzip(SimpleCommand):
+    def __init__(self, env):
+        super().__init__(env, name='gzip', env_var='GZIP', default='gzip')
+
+    def _call(self, cmd, input, output):
+        return shell_list(cmd + ['-c', input, shell_literal('>'), output])
```

### Comparing `bfg9000-0.6.0/bfg9000/tools/doppel.py` & `bfg9000-0.7.0/bfg9000/tools/doppel.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,31 +13,34 @@
     def kind_args(self, kind):
         if kind == 'data':
             return ['-m', '644']
         elif kind == 'program':
             return []
         raise ValueError('unknown kind {!r}'.format(kind))
 
-    def _call(self, cmd, mode, src, dst, directory=None, format=None,
-              dest_prefix=None):
-        if mode == 'onto':
-            return cmd + ['-p', src, dst]
+    def _call_onto(self, cmd, src, dst):
+        return cmd + ['-p', src, dst]
 
-        elif mode == 'into':
-            result = cmd + ['-ipN']
-            if not_buildroot(directory):
-                result.extend(['-C', directory])
-            result.extend(iterate(src))
-            result.append(dst)
-            return result
+    def _call_into(self, cmd, src, dst, *, directory=None):
+        result = cmd + ['-ipN']
+        if not_buildroot(directory):
+            result.extend(['-C', directory])
+        result.extend(iterate(src))
+        result.append(dst)
+        return result
 
-        elif mode == 'archive':
-            result = cmd + ['-ipN', '-f', format]
-            if not_buildroot(directory):
-                result.extend(['-C', directory])
-            if dest_prefix:
-                result.extend(['-P', dest_prefix])
-            result.extend(iterate(src))
-            result.append(dst)
-            return result
+    def _call_archive(self, cmd, src, dst, *, format, directory=None,
+                      dest_prefix=None):
+        result = cmd + ['-ipN', '-f', format]
+        if not_buildroot(directory):
+            result.extend(['-C', directory])
+        if dest_prefix:
+            result.extend(['-P', dest_prefix])
+        result.extend(iterate(src))
+        result.append(dst)
+        return result
 
-        raise ValueError('unknown mode {!r}'.format(mode))
+    def _call(self, cmd, mode, *args, **kwargs):
+        try:
+            return getattr(self, '_call_' + mode)(cmd, *args, **kwargs)
+        except AttributeError:
+            raise TypeError('unknown mode {!r}'.format(mode))
```

### Comparing `bfg9000-0.6.0/bfg9000/tools/fortran.py` & `bfg9000-0.7.0/bfg9000/tools/fortran.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.6.0/bfg9000/tools/install_name_tool.py` & `bfg9000-0.7.0/bfg9000/tools/install_name_tool.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.6.0/bfg9000/tools/internal.py` & `bfg9000-0.7.0/bfg9000/tools/internal.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,17 +6,29 @@
 
 @tool('bfg9000')
 class Bfg9000(SimpleCommand):
     def __init__(self, env):
         super().__init__(env, name='bfg9000', env_var='BFG9000',
                          default=env.bfgdir.append('bfg9000'))
 
-    def _call(self, cmd, builddir):
+    def _call_refresh(self, cmd, builddir):
         return cmd + ['refresh', builddir]
 
+    def _call_run(self, cmd, *, args, initial=False):
+        result = cmd + ['run']
+        if initial:
+            result.append('-I')
+        return result + ['--'] + args
+
+    def _call(self, cmd, subcmd, *args, **kwargs):
+        try:
+            return getattr(self, '_call_' + subcmd)(cmd, *args, **kwargs)
+        except AttributeError:
+            raise TypeError('unknown subcommand {!r}'.format(subcmd))
+
 
 @tool('depfixer')
 class Depfixer(SimpleCommand):
     def __init__(self, env):
         super().__init__(env, name='depfixer', env_var='DEPFIXER',
                          default=env.bfgdir.append('bfg9000-depfixer'))
 
@@ -28,15 +40,15 @@
 @tool('jvmoutput')
 class JvmOutput(SimpleCommand):
     def __init__(self, env):
         super().__init__(env, name='jvmoutput', env_var='JVMOUTPUT',
                          default=env.bfgdir.append('bfg9000-jvmoutput'))
 
     def _call(self, cmd, output, subcmd):
-        return cmd + ['-o', output] + subcmd
+        return cmd + ['-o', output, '--'] + subcmd
 
 
 @tool('rccdep')
 class RccDep(SimpleCommand):
     def __init__(self, env):
         super().__init__(env, name='rccdep', env_var='RCCDEP',
                          default=env.bfgdir.append('bfg9000-rccdep'))
```

### Comparing `bfg9000-0.6.0/bfg9000/tools/java.py` & `bfg9000-0.7.0/bfg9000/tools/java.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     x.exts(source=['.java'])
 
 with known_langs.make('scala') as x:
     x.vars(compiler='SCALAC', runner='SCALACMD', flags='SCALAFLAGS')
     x.exts(source=['.scala'])
 
 with known_formats.make('jvm', src_lang='java') as fmt, \
-     fmt.make('dynamic') as x:  # noqa
+     fmt.make('dynamic') as x:
     x.vars(linker='JAR', flags='JARFLAGS')
 
 _default_cmds = {
     'java' : ['javac', 'gcj'],
     'scala': 'scalac',
 }
```

### Comparing `bfg9000-0.6.0/bfg9000/tools/ld.py` & `bfg9000-0.7.0/bfg9000/tools/ld.py`

 * *Files 14% similar despite different names*

```diff
@@ -6,14 +6,17 @@
 
 
 class LdLinker:
     def __init__(self, builder, env, command, version_output):
         self.builder = builder
         self.env = env
         self.command = command
+        # Currently, if we're constructing this object, we know the command has
+        # been found.
+        self.found = True
 
         if 'GNU ld' in version_output:
             self.brand = 'bfd'
             self.version = detect_version(version_output)
         elif 'GNU gold' in version_output:
             self.brand = 'gold'
             self.version = detect_version(version_output, post='$',
```

### Comparing `bfg9000-0.6.0/bfg9000/tools/lex.py` & `bfg9000-0.7.0/bfg9000/tools/lex.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,23 +22,25 @@
     candidates = (_windows_cmds if env.host_platform.family == 'windows'
                   else _posix_cmds)
     return choose_builder(env, known_langs['lex'], (LexBuilder,),
                           default_candidates=candidates)
 
 
 class LexBuilder(Builder):
-    def __init__(self, env, langinfo, command, version_output):
+    def __init__(self, env, langinfo, command, found, version_output):
         super().__init__(langinfo.name, *self._parse_brand(version_output))
 
         name = langinfo.var('compiler').lower()
         lflags_name = langinfo.var('flags').lower()
         lflags = shell.split(env.getvar(langinfo.var('flags'), ''))
 
-        self.transpiler = LexCompiler(self, env, command=(name, command),
-                                      flags=(lflags_name, lflags))
+        self.transpiler = LexCompiler(
+            self, env, command=(name, command, found),
+            flags=(lflags_name, lflags)
+        )
 
     @staticmethod
     def _parse_brand(version_output):
         if 'flex' in version_output:
             return 'flex', detect_version(version_output)
         return 'unknown', None
```

### Comparing `bfg9000-0.6.0/bfg9000/tools/msvc/__init__.py` & `bfg9000-0.7.0/bfg9000/tools/msvc/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,46 +1,44 @@
 import os.path
 from itertools import chain
 
-from .. import pkg_config
-from ... import log, options as opts, shell
+from .. import mopack, pkg_config
+from ... import shell
 from .compiler import MsvcCompiler, MsvcPchCompiler
 from .linker import (MsvcExecutableLinker, MsvcSharedLibraryLinker,
                      MsvcStaticLinker)
 from .rc import MsvcRcBuilder  # noqa: F401
 from ..common import Builder, check_which
-from ...exceptions import PackageResolutionError
-from ...file_types import HeaderDirectory, Library
-from ...iterutils import default_sentinel, iterate, uniques
+from ...iterutils import uniques
 from ...languages import known_formats
-from ...packages import CommonPackage, PackageKind
-from ...path import exists, Root
+from ...path import exists
 from ...versioning import detect_version
 
 
 class MsvcBuilder(Builder):
-    def __init__(self, env, langinfo, command, version_output):
-        super().__init__(langinfo.name, *self._parse_brand(version_output))
+    def __init__(self, env, langinfo, command, found, version_output):
+        brand, version = self._parse_brand(env, command, version_output)
+        super().__init__(langinfo.name, brand, version)
         self.object_format = env.target_platform.object_format
 
         name = langinfo.var('compiler').lower()
         ldinfo = known_formats['native']['dynamic']
         arinfo = known_formats['native']['static']
 
         # Look for the last argument that looks like our compiler and use its
         # directory as the base directory to find the linkers.
         origin = ''
         for i in reversed(command):
             if os.path.basename(i) in ('cl', 'cl.exe'):
                 origin = os.path.dirname(i)
-        link_command = check_which(
+        link_which = check_which(
             env.getvar(ldinfo.var('linker'), os.path.join(origin, 'link')),
             env.variables, kind='{} dynamic linker'.format(self.lang)
         )
-        lib_command = check_which(
+        lib_which = check_which(
             env.getvar(arinfo.var('linker'), os.path.join(origin, 'lib')),
             env.variables, kind='{} static linker'.format(self.lang)
         )
 
         cflags_name = langinfo.var('flags').lower()
         cflags = (
             shell.split(env.getvar('CPPFLAGS', '')) +
@@ -53,44 +51,50 @@
         ldlibs_name = ldinfo.var('libs').lower()
         ldlibs = shell.split(env.getvar(ldinfo.var('libs'), ''))
 
         ar_name = arinfo.var('linker').lower()
         arflags_name = arinfo.var('flags').lower()
         arflags = shell.split(env.getvar(arinfo.var('flags'), ''))
 
-        compile_kwargs = {'command': (name, command),
+        compile_kwargs = {'command': (name, command, found),
                           'flags': (cflags_name, cflags)}
         self.compiler = MsvcCompiler(self, env, **compile_kwargs)
         self.pch_compiler = MsvcPchCompiler(self, env, **compile_kwargs)
 
-        link_kwargs = {'command': (ld_name, link_command),
+        link_kwargs = {'command': (ld_name,) + link_which,
                        'flags': (ldflags_name, ldflags),
                        'libs': (ldlibs_name, ldlibs)}
         self._linkers = {
             'executable': MsvcExecutableLinker(self, env, name, **link_kwargs),
             'shared_library': MsvcSharedLibraryLinker(self, env, name,
                                                       **link_kwargs),
             'static_library': MsvcStaticLinker(
-                self, env, command=(ar_name, lib_command),
+                self, env, command=(ar_name,) + lib_which,
                 flags=(arflags_name, arflags)
             ),
         }
         self.packages = MsvcPackageResolver(self, env)
         self.runner = None
 
     @staticmethod
-    def _parse_brand(version_output):
+    def _parse_brand(env, command, version_output):
         if 'Microsoft (R)' in version_output:
             return 'msvc', detect_version(version_output)
-        # XXX: Detect clang-cl.
+        elif 'clang LLVM compiler' in version_output:
+            real_version = env.execute(
+                command + ['--version'], stdout=shell.Mode.pipe,
+                stderr=shell.Mode.stdout
+            )
+            return 'clang', detect_version(real_version)
+
         return 'unknown', None
 
     @staticmethod
     def check_command(env, command):
-        return env.execute(command + ['/?'], stdout=shell.Mode.pipe,
+        return env.execute(command + ['-?'], stdout=shell.Mode.pipe,
                            stderr=shell.Mode.stdout)
 
     @property
     def flavor(self):
         return 'msvc'
 
     @property
@@ -106,14 +110,16 @@
         return False
 
     def linker(self, mode):
         return self._linkers[mode]
 
 
 class MsvcPackageResolver:
+    _lib_names = ['{}.lib']
+
     def __init__(self, builder, env):
         self.builder = builder
         self.env = env
 
         self.include_dirs = [i for i in uniques(chain(
             self.builder.compiler.search_dirs(),
             self.env.host_platform.include_dirs
@@ -124,57 +130,22 @@
             self.env.host_platform.lib_dirs
         )) if exists(i)]
 
     @property
     def lang(self):
         return self.builder.lang
 
-    def header(self, name, search_dirs=None):
-        if search_dirs is None:
-            search_dirs = self.include_dirs
-
-        for base in search_dirs:
-            if base.root != Root.absolute:
-                raise ValueError('expected an absolute path')
-            if exists(base.append(name)):
-                return HeaderDirectory(base, None, system=True)
-
-        raise PackageResolutionError("unable to find header '{}'".format(name))
-
-    def library(self, name, kind=PackageKind.any, search_dirs=None):
-        if search_dirs is None:
-            search_dirs = self.lib_dirs
-        libname = name + '.lib'
-
-        for base in search_dirs:
-            if base.root != Root.absolute:
-                raise ValueError('expected an absolute path')
-            fullpath = base.append(libname)
-            if exists(fullpath):
-                # We don't actually know what kind of library this is. It could
-                # be a static library or an import library (which we classify
-                # as a kind of shared lib).
-                return Library(fullpath, self.builder.object_format)
-        raise PackageResolutionError("unable to find library '{}'"
-                                     .format(name))
-
-    def resolve(self, name, version, kind, headers, lib_names):
+    # TODO: Remove headers/libs from arguments after 0.7 is released.
+    def resolve(self, name, submodules, version, kind, *, headers=None,
+                libs=None, system=True):
         format = self.builder.object_format
-        try:
-            return pkg_config.resolve(self.env, name, format, version, kind)
-        except (OSError, PackageResolutionError):
-            if lib_names is default_sentinel:
-                lib_names = self.env.target_platform.transform_package(name)
+        usage = mopack.get_usage(self.env, name, submodules, self.include_dirs,
+                                 self.lib_dirs, self._lib_names)
 
-            compile_options = opts.option_list(
-                opts.include_dir(self.header(i)) for i in iterate(headers)
-            )
-            link_options = opts.option_list(
-                opts.lib(self.library(i, kind)) for i in iterate(lib_names)
-            )
-
-            path_note = ' in {}'.format(
-                link_options[0].library.path.parent().string()
-            ) if link_options else ''
-            log.info('found package {!r} via path-search{}'
-                     .format(name, path_note))
-            return CommonPackage(name, format, compile_options, link_options)
+        # XXX: Add headers/libs here somehow? Add them into PkgConfigPackage
+        # directly?
+        return pkg_config.resolve(
+            self.env, name, submodules, version, usage['pcnames'],
+            format=format, kind=kind, system=system,
+            search_path=usage['pkg_config_path'],
+            generated=usage.get('generated', False)
+        )
```

### Comparing `bfg9000-0.6.0/bfg9000/tools/msvc/compiler.py` & `bfg9000-0.7.0/bfg9000/tools/msvc/compiler.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.6.0/bfg9000/tools/msvc/linker.py` & `bfg9000-0.7.0/bfg9000/tools/msvc/linker.py`

 * *Files 2% similar despite different names*

```diff
@@ -138,23 +138,24 @@
             elif isinstance(i, opts.lib_literal):
                 flags.append(i.value)
         return flags
 
     @staticmethod
     @memoize
     def __parser():
-        parser = ArgumentParser()
+        parser = ArgumentParser(case_sensitive=False)
         parser.add('/nologo')
-        parser.add('/DEBUG', dest='debug')
+        parser.add('/debug')
+        parser.add('/libpath', type=list, dest='libdirs')
         return parser
 
     @staticmethod
     @memoize
     def __lib_parser():
-        parser = ArgumentParser()
+        parser = ArgumentParser(case_sensitive=False)
         parser.add('/nologo')
         parser.add_unnamed('libs')
         return parser
 
     def parse_flags(self, flags, lib_flags):
         result, extra = self.__parser().parse_known(flags)
         libresult, libextra = self.__lib_parser().parse_known(lib_flags)
```

### Comparing `bfg9000-0.6.0/bfg9000/tools/msvc/rc.py` & `bfg9000-0.7.0/bfg9000/tools/msvc/rc.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,34 +7,36 @@
 from ...iterutils import iterate
 from ...objutils import memoize
 from ...path import Path
 from ...versioning import detect_version
 
 
 class MsvcRcBuilder(Builder):
-    def __init__(self, env, langinfo, command, version_output):
+    def __init__(self, env, langinfo, command, found, version_output):
         super().__init__(langinfo.name, *self._parse_brand(version_output))
 
         name = langinfo.var('compiler').lower()
         lflags_name = langinfo.var('flags').lower()
         lflags = shell.split(env.getvar(langinfo.var('flags'), ''))
 
         self.object_format = env.target_platform.object_format
-        self.compiler = MsvcRcCompiler(self, env, command=(name, command),
-                                       flags=(lflags_name, lflags))
+        self.compiler = MsvcRcCompiler(
+            self, env, command=(name, command, found),
+            flags=(lflags_name, lflags)
+        )
 
     @staticmethod
     def _parse_brand(version_output):
         if 'Microsoft (R)' in version_output:
             return 'msvc', detect_version(version_output)
         return 'unknown', None
 
     @staticmethod
     def check_command(env, command):
-        return env.execute(command + ['/?'], stdout=shell.Mode.pipe,
+        return env.execute(command + ['-?'], stdout=shell.Mode.pipe,
                            stderr=shell.Mode.devnull)
 
     @property
     def flavor(self):
         return 'msvc'
 
     def linker(self, kind):
```

### Comparing `bfg9000-0.6.0/bfg9000/tools/patchelf.py` & `bfg9000-0.7.0/bfg9000/tools/patchelf.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.6.0/bfg9000/tools/qt.py` & `bfg9000-0.7.0/bfg9000/tools/qt.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,23 +27,25 @@
 @builder('qtmoc')
 def moc_builder(env):
     return choose_builder(env, known_langs['qtmoc'], (MocBuilder,),
                           default_candidates=['moc'])
 
 
 class MocBuilder(Builder):
-    def __init__(self, env, langinfo, command, version_output):
+    def __init__(self, env, langinfo, command, found, version_output):
         super().__init__(langinfo.name, *self._parse_brand(version_output))
 
         name = langinfo.var('compiler').lower()
         mocflags_name = langinfo.var('flags').lower()
         mocflags = shell.split(env.getvar(langinfo.var('flags'), ''))
 
-        self.transpiler = MocCompiler(self, env, command=(name, command),
-                                      flags=(mocflags_name, mocflags))
+        self.transpiler = MocCompiler(
+            self, env, command=(name, command, found),
+            flags=(mocflags_name, mocflags)
+        )
 
     @staticmethod
     def _parse_brand(version_output):
         if 'moc' in version_output:
             return 'qt', detect_version(version_output)
         return 'unknown', None
 
@@ -101,23 +103,25 @@
 @builder('qrc')
 def qrc_builder(env):
     return choose_builder(env, known_langs['qrc'], (RccBuilder,),
                           default_candidates=['rcc'])
 
 
 class RccBuilder(Builder):
-    def __init__(self, env, langinfo, command, version_output):
+    def __init__(self, env, langinfo, command, found, version_output):
         super().__init__(langinfo.name, *self._parse_brand(version_output))
 
         name = langinfo.var('compiler').lower()
         rccflags_name = langinfo.var('flags').lower()
         rccflags = shell.split(env.getvar(langinfo.var('flags'), ''))
 
-        self.transpiler = RccCompiler(self, env, command=(name, command),
-                                      flags=(rccflags_name, rccflags))
+        self.transpiler = RccCompiler(
+            self, env, command=(name, command, found),
+            flags=(rccflags_name, rccflags)
+        )
 
     @staticmethod
     def _parse_brand(version_output):
         if 'rcc' in version_output:
             return 'qt', detect_version(version_output)
         return 'unknown', None
 
@@ -159,23 +163,25 @@
 @builder('qtui')
 def qtui_builder(env):
     return choose_builder(env, known_langs['qtui'], (UicBuilder,),
                           default_candidates=['uic'])
 
 
 class UicBuilder(Builder):
-    def __init__(self, env, langinfo, command, version_output):
+    def __init__(self, env, langinfo, command, found, version_output):
         super().__init__(langinfo.name, *self._parse_brand(version_output))
 
         name = langinfo.var('compiler').lower()
         uicflags_name = langinfo.var('flags').lower()
         uicflags = shell.split(env.getvar(langinfo.var('flags'), ''))
 
-        self.transpiler = UicCompiler(self, env, command=(name, command),
-                                      flags=(uicflags_name, uicflags))
+        self.transpiler = UicCompiler(
+            self, env, command=(name, command, found),
+            flags=(uicflags_name, uicflags)
+        )
 
     @staticmethod
     def _parse_brand(version_output):
         if 'uic' in version_output:
             return 'qt', detect_version(version_output)
         return 'unknown', None
```

### Comparing `bfg9000-0.6.0/bfg9000/tools/rc.py` & `bfg9000-0.7.0/bfg9000/tools/rc.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,20 @@
+import re
+
 from . import builder, cc, msvc
 from .. import log, shell
-from .common import choose_builder, make_command_converter
+from .common import choose_builder, guess_command, make_command_converter
 from ..languages import known_langs
 
 with known_langs.make('rc') as x:
     x.vars(compiler='RC', flags='RCFLAGS')
     x.exts(source=['.rc'])
 
 _c_to_rc = make_command_converter([
-    ('gcc-posix', 'windres'),
-    ('gcc-win32', 'windres'),
-    ('gcc', 'windres'),
+    (re.compile(r'gcc(?:-[\d.]+)?(?:-(?:posix|win32))?'), 'windres'),
 ])
 
 _posix_cmds = ['windres']
 _windows_cmds = ['rc', 'windres']
 _builders = (cc.CcRcBuilder, msvc.MsvcRcBuilder)
 
 
@@ -23,35 +23,28 @@
     langinfo = known_langs['rc']
     cmd = env.getvar(langinfo.var('compiler'))
     if cmd:
         return choose_builder(env, langinfo, _builders, candidates=cmd)
 
     # We don't have an explicitly-set command from the environment, so try to
     # guess what the right command would be based on the C compiler command.
-
     candidates = (_windows_cmds if env.host_platform.family == 'windows'
                   else _posix_cmds)
-    sibling_cmd = env.builder('c').compiler.command
-
-    for i in sibling_cmd:
-        guessed_cmd = _c_to_rc(i)
-        if guessed_cmd is not None:
-            break
-    else:
-        guessed_cmd = None
+    sibling = env.builder('c').compiler
+    guessed_cmd = guess_command(sibling, _c_to_rc)
 
     # If the guessed command is the same as the first default command
     # candidate, remove it. This will keep us from logging a useless info
     # message that we guessed the default value for the command.
     if guessed_cmd is not None and guessed_cmd != candidates[0]:
         try:
             builder = choose_builder(env, langinfo, _builders,
                                      candidates=guessed_cmd, strict=True)
             log.info('guessed windows rc compiler {!r} from c compiler {!r}'
-                     .format(guessed_cmd, shell.join(sibling_cmd)))
+                     .format(guessed_cmd, shell.join(sibling.command)))
             return builder
         except IOError:
             pass
 
     # Try the default command candidates.
     return choose_builder(env, langinfo, _builders,
                           candidates=candidates)
```

### Comparing `bfg9000-0.6.0/bfg9000/tools/scripts.py` & `bfg9000-0.7.0/bfg9000/tools/scripts.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.6.0/bfg9000/tools/setenv.py` & `bfg9000-0.7.0/bfg9000/tools/setenv.py`

 * *Files identical despite different names*

### Comparing `bfg9000-0.6.0/bfg9000/tools/yacc.py` & `bfg9000-0.7.0/bfg9000/tools/yacc.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,23 +22,25 @@
     candidates = (_windows_cmds if env.host_platform.family == 'windows'
                   else _posix_cmds)
     return choose_builder(env, known_langs['yacc'], (YaccBuilder,),
                           default_candidates=candidates)
 
 
 class YaccBuilder(Builder):
-    def __init__(self, env, langinfo, command, version_output):
+    def __init__(self, env, langinfo, command, found, version_output):
         super().__init__(langinfo.name, *self._parse_brand(version_output))
 
         name = langinfo.var('compiler').lower()
         lflags_name = langinfo.var('flags').lower()
         lflags = shell.split(env.getvar(langinfo.var('flags'), ''))
 
-        self.transpiler = YaccCompiler(self, env, command=(name, command),
-                                       flags=(lflags_name, lflags))
+        self.transpiler = YaccCompiler(
+            self, env, command=(name, command, found),
+            flags=(lflags_name, lflags)
+        )
 
     @staticmethod
     def _parse_brand(version_output):
         if 'bison' in version_output:
             return 'bison', detect_version(version_output)
         return 'unknown', None
```

### Comparing `bfg9000-0.6.0/bfg9000/versioning.py` & `bfg9000-0.7.0/bfg9000/versioning.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,27 @@
 import platform
 import re
 from itertools import chain
-from packaging.specifiers import (
-    LegacySpecifier as Specifier, Specifier as PythonSpecifier,
-    SpecifierSet as PythonSpecifierSet
-)
-from packaging.version import (
-    Version as PythonVersion, LegacyVersion as Version
-)
+from verspec.loose import Version, Specifier, SpecifierSet, InvalidSpecifier
+from verspec.python import PythonVersion, PythonSpecifier, PythonSpecifierSet
 
 from .app_version import version as bfg_version
 from .exceptions import VersionError
 from .iterutils import iterate
 
-__all__ = ['bfg_version', 'check_version', 'detect_version', 'python_version',
-           'PythonSpecifier', 'PythonSpecifierSet', 'PythonVersion',
-           'simplify_specifiers', 'Specifier', 'SpecifierSet', 'Version',
-           'VersionError']
+__all__ = ['bfg_version', 'check_version', 'detect_version',
+           'InvalidSpecifier', 'python_version', 'PythonSpecifier',
+           'PythonSpecifierSet', 'PythonVersion', 'simplify_specifiers',
+           'Specifier', 'SpecifierSet', 'Version', 'VersionError']
 
 bfg_version = PythonVersion(bfg_version)
 # Strip trailing "+" from Python version. Some versions in distros have this...
 python_version = PythonVersion(re.sub(r'\+$', '', platform.python_version()))
 
 
-# Use a LegacySpecifierSet instead once packaging.specifiers has it. See
-# <https://github.com/pypa/packaging/pull/92>.
-class SpecifierSet(PythonSpecifierSet):
-    def __init__(self, specifiers=''):
-        specifiers = [s.strip() for s in specifiers.split(',') if s.strip()]
-        parsed = set()
-        for specifier in specifiers:
-            parsed.add(Specifier(specifier))
-        self._specs = frozenset(parsed)
-        self._prereleases = None
-
-
 def simplify_specifiers(spec):
     """Try to simplify a SpecifierSet by combining redundant specifiers."""
 
     def key(s):
         return (s.version, 1 if s.operator in ['>=', '<'] else 2)
 
     def in_bounds(v, lo, hi):
```

### Comparing `bfg9000-0.6.0/bfg9000.egg-info/PKG-INFO` & `bfg9000-0.7.0/bfg9000.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,104 +1,109 @@
 Metadata-Version: 2.1
 Name: bfg9000
-Version: 0.6.0
+Version: 0.7.0
 Summary: A cross-platform build file generator
 Home-page: https://jimporter.github.io/bfg9000/
 Author: Jim Porter
 Author-email: itsjimporter@gmail.com
-License: BSD
-Description: bfg9000 - build file generator
-        ==============================
+License: BSD-3-Clause
+Description: # bfg9000 - build file generator
+        **bfg9000** is a cross-platform *build configuration system* with an emphasis on
+        making it easy to define how to build your software. It converts a Python-based
+        build script into the appropriate files for your underlying build system of
+        choice (Ninja, Make, or MSBuild).
         
-        **bfg9000** is a cross-platform *build configuration system* with an
-        emphasis on making it easy to define how to build your software. It
-        converts a Python-based build script into the appropriate files for your
-        underlying build system of choice (Ninja, Make, or MSBuild).
+        ## Why bfg9000?
         
-        Why bfg9000?
-        ------------
+        #### Familiar syntax
         
-        Familiar syntax
-        ^^^^^^^^^^^^^^^
+        `build.bfg` files are just Python scripts with some new functions added, so you
+        may already know how to write them; and when your build gets complicated, you
+        can rely on the existing Python ecosystem to get you out of trouble.
         
-        ``build.bfg`` files are just Python scripts with some new functions
-        added, so you may already know how to write them; and when your build
-        gets complicated, you can rely on the existing Python ecosystem to get
-        you out of trouble.
+        #### Fast builds
         
-        Fast builds
-        ^^^^^^^^^^^
+        bfg9000 ensures your builds are fast by relying on existing, mature build
+        systems like Make and Ninja to do the heavy lifting of building your software;
+        often, incremental builds don't need to execute bfg9000 at all!
         
-        bfg9000 ensures your builds are fast by relying on existing, mature
-        build systems like Make and Ninja to do the heavy lifting of building
-        your software; often, incremental builds don’t need to execute bfg9000
-        at all!
+        #### Stay sane
         
-        Stay sane
-        ^^^^^^^^^
+        Building your code shouldn't be the hard part of developing your project. Above
+        all else, bfg9000 strives to help you get your build right the *first* time with
+        many helpful [features][features].
         
-        Building your code shouldn’t be the hard part of developing your
-        project. Above all else, bfg9000 strives to help you get your build
-        right the *first* time with many helpful
-        `features <https://jimporter.github.io/bfg9000/latest/user/features>`__.
+        ## A brief example
         
-        A brief example
-        ---------------
+        You can't get much simpler than the simplest `build.bfg` file:
         
-        You can’t get much simpler than the simplest ``build.bfg`` file:
+        ```python
+        executable('simple', files=['simple.cpp'])
+        ```
         
-        .. code:: python
+        To build this executable, we need to create the actual build files and then
+        run them:
         
-           executable('simple', files=['simple.cpp'])
+        ```sh
+        $ cd /path/to/src/
+        $ 9k build/
+        $ cd build/
+        $ ninja
+        ```
         
-        To build this executable, we need to create the actual build files and
-        then run them:
+        From there, you can run your newly-created executable: `./simple`. Hooray!
         
-        .. code:: sh
+        For further examples, please see the [`examples/`][examples] subdirectory.
         
-           $ cd /path/to/src/
-           $ 9k build/
-           $ cd build/
-           $ ninja
+        ## Installation
         
-        From there, you can run your newly-created executable: ``./simple``.
-        Hooray!
+        bfg9000 uses [setuptools][setuptools], so installation is much the same as any
+        other Python package:
         
-        For further examples, please see the
-        ```examples/`` <https://github.com/jimporter/bfg9000/tree/master/examples>`__
-        subdirectory.
+        ```sh
+        $ pip install bfg9000
+        ```
         
-        Installation
-        ------------
+        From there, you can start using bfg to build your software! (If you're using
+        Ubuntu, you can also install bfg9000 from the following PPA:
+        [ppa:jimporter/stable][ppa]). For more information about how to install bfg9000,
+        see the [documentation][getting-started].
         
-        bfg9000 uses `setuptools <https://pythonhosted.org/setuptools/>`__, so
-        installation is much the same as any other Python package:
+        ## License
         
-        .. code:: sh
+        This project is licensed under the [BSD 3-clause license](LICENSE).
         
-           $ pip install bfg9000
+        [pypi-image]: https://img.shields.io/pypi/v/bfg9000.svg
+        [pypi-link]: https://pypi.python.org/pypi/bfg9000
+        [documentation-image]: https://img.shields.io/badge/docs-bfg9000-blue.svg
+        [documentation-link]: https://jimporter.github.io/bfg9000/
+        [gh-actions-image]: https://github.com/jimporter/bfg9000/workflows/build/badge.svg
+        [gh-actions-link]: https://github.com/jimporter/bfg9000/actions?query=branch%3Amaster+workflow%3Abuild
+        [appveyor-image]: https://ci.appveyor.com/api/projects/status/hxvbggf6exq8i2k6/branch/master?svg=true
+        [appveyor-link]: https://ci.appveyor.com/project/jimporter/bfg9000/branch/master
+        [codecov-image]: https://codecov.io/gh/jimporter/bfg9000/branch/master/graph/badge.svg
+        [codecov-link]: https://codecov.io/gh/jimporter/bfg9000
         
-        From there, you can start using bfg to build your software! (If you’re
-        using Ubuntu, you can also install bfg9000 from the following PPA:
-        `ppa:jimporter/stable <https://launchpad.net/~jimporter/+archive/ubuntu/stable>`__).
-        For more information about how to install bfg9000, see the
-        `documentation <https://jimporter.github.io/bfg9000/latest/getting-started>`__.
-        
-        License
-        -------
-        
-        This project is licensed under the `BSD 3-clause license <LICENSE>`__.
+        [features]: https://jimporter.github.io/bfg9000/latest/user/features
+        [examples]: https://github.com/jimporter/bfg9000/tree/master/examples
+        [setuptools]: https://pythonhosted.org/setuptools/
+        [ppa]: https://launchpad.net/~jimporter/+archive/ubuntu/stable
+        [getting-started]: https://jimporter.github.io/bfg9000/latest/getting-started
         
 Keywords: build file generator
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: msbuild
 Provides-Extra: test
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `bfg9000-0.6.0/bfg9000.egg-info/SOURCES.txt` & `bfg9000-0.7.0/bfg9000.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+CHANGES.md
+LICENSE
 MANIFEST.in
 README.md
 setup.cfg
 setup.py
 bfg9000/__init__.py
 bfg9000/app_version.py
 bfg9000/build.py
@@ -30,14 +32,16 @@
 bfg9000.egg-info/entry_points.txt
 bfg9000.egg-info/requires.txt
 bfg9000.egg-info/top_level.txt
 bfg9000/arguments/__init__.py
 bfg9000/arguments/parser.py
 bfg9000/arguments/windows.py
 bfg9000/backends/__init__.py
+bfg9000/backends/compdb/__init__.py
+bfg9000/backends/compdb/writer.py
 bfg9000/backends/make/__init__.py
 bfg9000/backends/make/syntax.py
 bfg9000/backends/make/writer.py
 bfg9000/backends/msbuild/__init__.py
 bfg9000/backends/msbuild/solution.py
 bfg9000/backends/msbuild/syntax.py
 bfg9000/backends/msbuild/writer.py
@@ -68,15 +72,14 @@
 bfg9000/builtins/toolchain.py
 bfg9000/builtins/user_arguments.py
 bfg9000/builtins/version.py
 bfg9000/platforms/__init__.py
 bfg9000/platforms/basepath.py
 bfg9000/platforms/core.py
 bfg9000/platforms/cygwin.py
-bfg9000/platforms/framework.py
 bfg9000/platforms/host.py
 bfg9000/platforms/posix.py
 bfg9000/platforms/target.py
 bfg9000/platforms/windows.py
 bfg9000/shell/__init__.py
 bfg9000/shell/list.py
 bfg9000/shell/posix.py
@@ -92,14 +95,15 @@
 bfg9000/tools/install_name_tool.py
 bfg9000/tools/internal.py
 bfg9000/tools/java.py
 bfg9000/tools/jvm.py
 bfg9000/tools/ld.py
 bfg9000/tools/lex.py
 bfg9000/tools/mkdir_p.py
+bfg9000/tools/mopack.py
 bfg9000/tools/patchelf.py
 bfg9000/tools/pkg_config.py
 bfg9000/tools/qt.py
 bfg9000/tools/rc.py
 bfg9000/tools/rm.py
 bfg9000/tools/scripts.py
 bfg9000/tools/setenv.py
```

### Comparing `bfg9000-0.6.0/bfg9000.egg-info/entry_points.txt` & `bfg9000-0.7.0/bfg9000.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `bfg9000-0.6.0/setup.py` & `bfg9000-0.7.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -26,33 +26,34 @@
         env = dict(os.environ)
         pythonpath = os.path.join(root_dir, 'test', 'scripts')
         if env.get('PYTHONPATH'):
             pythonpath += os.pathsep + env['PYTHONPATH']
         env.update({
             'PYTHONPATH': pythonpath,
             'COVERAGE_FILE': os.path.join(root_dir, '.coverage'),
-            'COVERAGE_PROCESS_START': os.path.join(root_dir, '.coveragerc'),
+            'COVERAGE_PROCESS_START': os.path.join(root_dir, 'setup.cfg'),
         })
 
-        subprocess.check_call(['coverage', 'erase'])
-        subprocess.check_call(
+        subprocess.run(['coverage', 'erase'], check=True)
+        subprocess.run(
             ['coverage', 'run', 'setup.py', 'test'] +
             (['-q'] if self.verbose == 0 else []) +
             (['-s', self.test_suite] if self.test_suite else []),
-            env=env
+            env=env, check=True
         )
-        subprocess.check_call(['coverage', 'combine'])
+        subprocess.run(['coverage', 'combine'], check=True,
+                       stdout=subprocess.DEVNULL)
 
 
 custom_cmds = {
     'coverage': Coverage,
 }
 
 try:
-    from packaging.version import Version
+    from verspec.python import Version
 
     class DocServe(Command):
         description = 'serve the documentation locally'
         user_options = [
             ('working', 'w', 'use the documentation in the working directory'),
             ('dev-addr=', None, 'address to host the documentation on'),
         ]
@@ -62,17 +63,17 @@
             self.dev_addr = '0.0.0.0:8000'
 
         def finalize_options(self):
             pass
 
         def run(self):
             cmd = 'mkdocs' if self.working else 'mike'
-            subprocess.check_call([
+            subprocess.run([
                 cmd, 'serve', '--dev-addr=' + self.dev_addr
-            ])
+            ], check=True)
 
     class DocDeploy(Command):
         description = 'push the documentation to GitHub'
         user_options = []
 
         def initialize_options(self):
             pass
@@ -82,99 +83,93 @@
 
         def run(self):
             v = Version(version)
             alias = 'dev' if v.is_devrelease else 'latest'
             title = '{} ({})'.format(v.base_version, alias)
             short_version = '{}.{}'.format(*v.release[:2])
 
-            info = json.loads(subprocess.check_output(
-                ['mike', 'list', '-j', alias],
-                universal_newlines=True
-            ))
-            if info['version'] != short_version:
+            try:
+                info = json.loads(subprocess.run(
+                    ['mike', 'list', '-j', alias], universal_newlines=True,
+                    check=True, stdout=subprocess.PIPE
+                ).stdout)
+            except subprocess.CalledProcessError:
+                info = None
+
+            if info and info['version'] != short_version:
                 t = re.sub(r' \({}\)$'.format(re.escape(alias)), '',
                            info['title'])
-                subprocess.check_call(['mike', 'retitle', info['version'], t])
+                subprocess.run(['mike', 'retitle', info['version'], t],
+                               check=True)
 
-            subprocess.check_call(['mike', 'deploy', '-ut', title,
-                                   short_version, alias])
+            subprocess.run(['mike', 'deploy', '-ut', title, short_version,
+                            alias], check=True)
 
     custom_cmds['doc_serve'] = DocServe
     custom_cmds['doc_deploy'] = DocDeploy
 except ImportError:
     pass
 
-try:
-    from flake8.main.setuptools_command import Flake8
-
-    class LintCommand(Flake8):
-        def distribution_files(self):
-            return ['setup.py', 'bfg9000', 'examples', 'test']
-
-    custom_cmds['lint'] = LintCommand
-except ImportError:
-    pass
-
 more_requires = []
 
 if os.getenv('STDEB_BUILD') not in ['1', 'true']:
     more_requires.extend([
         'doppel >= 0.4.0',
+        'mopack >= 0.1.0',
         'pysetenv;platform_system=="Windows"'
     ])
-    if os.getenv('NO_PATCHELF') not in ['1', 'true']:
-        more_requires.append('patchelf-wrapper;platform_system=="Linux"')
 
 with open(os.path.join(root_dir, 'README.md'), 'r') as f:
     # Read from the file and strip out the badges.
     long_desc = re.sub(r'(^# bfg9000.*)\n\n(.+\n)*', r'\1', f.read())
 
-try:
-    import pypandoc
-    long_desc = pypandoc.convert_text(long_desc, 'rst', format='md')
-except ImportError:
-    pass
-
 setup(
     name='bfg9000',
     version=version,
 
     description='A cross-platform build file generator',
     long_description=long_desc,
+    long_description_content_type='text/markdown',
     keywords='build file generator',
     url='https://jimporter.github.io/bfg9000/',
 
     author='Jim Porter',
     author_email='itsjimporter@gmail.com',
-    license='BSD',
+    license='BSD-3-Clause',
 
     classifiers=[
         'Development Status :: 3 - Alpha',
 
         'Intended Audience :: Developers',
 
         'Topic :: Software Development :: Build Tools',
         'License :: OSI Approved :: BSD License',
 
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.5',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
     ],
 
     packages=find_packages(exclude=['test', 'test.*']),
 
+    python_requires='>=3.6',
     install_requires=(
-        ['colorama', 'packaging >= 17.0', 'setuptools'] + more_requires
+        ['colorama', 'importlib_metadata', 'importlib_resources', 'pyyaml',
+         'verspec'] + more_requires
     ),
     extras_require={
-        'dev': ['coverage', 'flake8 >= 3.7', 'lxml', 'mike >= 0.3.1',
-                'mkdocs-bootswatch', 'pypandoc >= 1.4', 'stdeb'],
-        'test': ['coverage', 'flake8 >= 3.7', 'lxml'],
+        'dev': ['coverage', 'flake8 >= 3.7', 'flake8-quotes', 'lxml',
+                'mike >= 0.3.1', 'mkdocs-bootswatch-classic',
+                'mkdocs-macros-plugin', 'shtab', 'stdeb'],
+        'test': ['coverage', 'flake8 >= 3.7', 'flake8-quotes', 'lxml',
+                 'shtab'],
         'msbuild': ['lxml'],
     },
 
     entry_points={
         'console_scripts': [
             'bfg9000=bfg9000.driver:main',
             '9k=bfg9000.driver:simple_main',
```

