# Comparing `tmp/cengal-3.1.18.3.tar.gz` & `tmp/cengal-3.1.18.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cengal-3.1.18.3.tar", last modified: Sun May 21 17:04:23 2023, max compression
+gzip compressed data, was "cengal-3.1.18.4.tar", last modified: Sun May 21 17:17:46 2023, max compression
```

## Comparing `cengal-3.1.18.3.tar` & `cengal-3.1.18.4.tar`

### file list

```diff
@@ -1,1878 +1,1878 @@
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.724812 cengal-3.1.18.3/
--rw-r--r--   0 mb        (1000) mb        (1000)    11358 2023-04-22 17:28:13.000000 cengal-3.1.18.3/LICENSE.md
--rw-r--r--   0 mb        (1000) mb        (1000)      614 2023-04-22 17:37:18.000000 cengal-3.1.18.3/NOTICE
--rw-r--r--   0 mb        (1000) mb        (1000)    27217 2023-05-21 17:04:23.724812 cengal-3.1.18.3/PKG-INFO
--rw-r--r--   0 mb        (1000) mb        (1000)    22105 2023-05-21 15:53:40.000000 cengal-3.1.18.3/README.md
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.074813 cengal-3.1.18.3/cengal/
--rw-r--r--   0 mb        (1000) mb        (1000)     8228 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/RequestCache.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2761 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/ServerClock.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.084812 cengal-3.1.18.3/cengal/base/
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/base/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.084812 cengal-3.1.18.3/cengal/base/classes/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/base/classes/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.084812 cengal-3.1.18.3/cengal/base/classes/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/base/classes/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.084812 cengal-3.1.18.3/cengal/base/classes/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/base/classes/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1267 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/base/classes/versions/v_0/classes.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.084812 cengal-3.1.18.3/cengal/base/classes/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/base/classes/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/base/classes/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.084812 cengal-3.1.18.3/cengal/base/exceptions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/base/exceptions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.084812 cengal-3.1.18.3/cengal/base/exceptions/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/base/exceptions/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.094812 cengal-3.1.18.3/cengal/base/exceptions/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1233 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/base/exceptions/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1303 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/base/exceptions/versions/v_0/exceptions.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.094812 cengal-3.1.18.3/cengal/base/exceptions/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/base/exceptions/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/base/exceptions/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.094812 cengal-3.1.18.3/cengal/build_tools/
--rw-r--r--   0 mb        (1000) mb        (1000)     1210 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/build_tools/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.094812 cengal-3.1.18.3/cengal/build_tools/current_compiler/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/build_tools/current_compiler/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.094812 cengal-3.1.18.3/cengal/build_tools/current_compiler/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/build_tools/current_compiler/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.094812 cengal-3.1.18.3/cengal/build_tools/current_compiler/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1239 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/build_tools/current_compiler/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2162 2023-05-21 17:03:53.000000 cengal-3.1.18.3/cengal/build_tools/current_compiler/versions/v_0/current_compiler.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.094812 cengal-3.1.18.3/cengal/build_tools/current_compiler/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/build_tools/current_compiler/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/build_tools/current_compiler/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.094812 cengal-3.1.18.3/cengal/build_tools/prepare_cflags/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/build_tools/prepare_cflags/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.094812 cengal-3.1.18.3/cengal/build_tools/prepare_cflags/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/build_tools/prepare_cflags/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.094812 cengal-3.1.18.3/cengal/build_tools/prepare_cflags/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1237 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/build_tools/prepare_cflags/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    14704 2023-05-21 17:03:53.000000 cengal-3.1.18.3/cengal/build_tools/prepare_cflags/versions/v_0/prepare_cflags.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.094812 cengal-3.1.18.3/cengal/build_tools/prepare_cflags/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/build_tools/prepare_cflags/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/build_tools/prepare_cflags/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.094812 cengal-3.1.18.3/cengal/bulk_pip_actions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/bulk_pip_actions/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     6287 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/bulk_pip_actions/bulk_install.py
--rw-r--r--   0 mb        (1000) mb        (1000)     6023 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/bulk_pip_actions/install.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1280 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/check_is_in_pycharm.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.094812 cengal-3.1.18.3/cengal/code_flow_control/
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/code_flow_control/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.094812 cengal-3.1.18.3/cengal/code_flow_control/args_manager/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/code_flow_control/args_manager/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.094812 cengal-3.1.18.3/cengal/code_flow_control/args_manager/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/code_flow_control/args_manager/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.104812 cengal-3.1.18.3/cengal/code_flow_control/args_manager/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1235 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/code_flow_control/args_manager/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    16577 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/code_flow_control/args_manager/versions/v_0/args_manager.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.104812 cengal-3.1.18.3/cengal/code_flow_control/args_manager/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/code_flow_control/args_manager/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    17267 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/code_flow_control/args_manager/versions/v_0/tests/_manual_test__args_manager.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/code_flow_control/args_manager/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.104812 cengal-3.1.18.3/cengal/code_flow_control/call_history_reapplier/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/code_flow_control/call_history_reapplier/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.104812 cengal-3.1.18.3/cengal/code_flow_control/call_history_reapplier/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/code_flow_control/call_history_reapplier/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.104812 cengal-3.1.18.3/cengal/code_flow_control/call_history_reapplier/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1245 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/code_flow_control/call_history_reapplier/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2770 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/code_flow_control/call_history_reapplier/versions/v_0/call_history_reapplier.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.104812 cengal-3.1.18.3/cengal/code_flow_control/call_history_reapplier/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/code_flow_control/call_history_reapplier/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/code_flow_control/call_history_reapplier/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.104812 cengal-3.1.18.3/cengal/code_flow_control/chained_flow/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/code_flow_control/chained_flow/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.104812 cengal-3.1.18.3/cengal/code_flow_control/chained_flow/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/code_flow_control/chained_flow/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.104812 cengal-3.1.18.3/cengal/code_flow_control/chained_flow/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1234 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/code_flow_control/chained_flow/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    36471 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/code_flow_control/chained_flow/versions/v_0/smart_chain.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.114812 cengal-3.1.18.3/cengal/code_flow_control/chained_flow/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/code_flow_control/chained_flow/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/code_flow_control/chained_flow/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)    32962 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/code_flow_control/chained_flow/versions/v_0/tests/example_for__chained_flow.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.114812 cengal-3.1.18.3/cengal/code_flow_control/chained_flow/versions/v_1/
--rw-r--r--   0 mb        (1000) mb        (1000)     1235 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/code_flow_control/chained_flow/versions/v_1/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    35218 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/code_flow_control/chained_flow/versions/v_1/chained_flow.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.114812 cengal-3.1.18.3/cengal/code_flow_control/chained_flow/versions/v_1/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/code_flow_control/chained_flow/versions/v_1/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/code_flow_control/chained_flow/versions/v_1/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)    32962 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/code_flow_control/chained_flow/versions/v_1/tests/example_for__chained_flow.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.114812 cengal-3.1.18.3/cengal/code_flow_control/multiinterface_essence/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/code_flow_control/multiinterface_essence/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.114812 cengal-3.1.18.3/cengal/code_flow_control/multiinterface_essence/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/code_flow_control/multiinterface_essence/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.114812 cengal-3.1.18.3/cengal/code_flow_control/multiinterface_essence/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/code_flow_control/multiinterface_essence/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    23328 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/code_flow_control/multiinterface_essence/versions/v_0/essence.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.114812 cengal-3.1.18.3/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2882 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2624 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/quadrangle.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1373 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/quadrangle_test.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3467 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/square_and_rectangle.py
--rw-r--r--   0 mb        (1000) mb        (1000)     4071 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/square_and_rectangle_test.py
--rw-r--r--   0 mb        (1000) mb        (1000)     4392 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/square_and_rectangle_test_old.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.114812 cengal-3.1.18.3/cengal/code_flow_control/none_or/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/code_flow_control/none_or/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.114812 cengal-3.1.18.3/cengal/code_flow_control/none_or/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/code_flow_control/none_or/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.124812 cengal-3.1.18.3/cengal/code_flow_control/none_or/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/code_flow_control/none_or/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1487 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/code_flow_control/none_or/versions/v_0/none_or.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.124812 cengal-3.1.18.3/cengal/code_flow_control/none_or/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/code_flow_control/none_or/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/code_flow_control/none_or/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.124812 cengal-3.1.18.3/cengal/code_flow_control/python_bytecode_manipulator/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/code_flow_control/python_bytecode_manipulator/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.124812 cengal-3.1.18.3/cengal/code_flow_control/python_bytecode_manipulator/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/code_flow_control/python_bytecode_manipulator/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.124812 cengal-3.1.18.3/cengal/code_flow_control/python_bytecode_manipulator/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1250 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/code_flow_control/python_bytecode_manipulator/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    29755 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/code_flow_control/python_bytecode_manipulator/versions/v_0/python_bytecode_manipulator.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.124812 cengal-3.1.18.3/cengal/code_flow_control/python_bytecode_manipulator/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/code_flow_control/python_bytecode_manipulator/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/code_flow_control/python_bytecode_manipulator/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.124812 cengal-3.1.18.3/cengal/code_flow_control/smart_values/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/code_flow_control/smart_values/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.124812 cengal-3.1.18.3/cengal/code_flow_control/smart_values/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/code_flow_control/smart_values/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.124812 cengal-3.1.18.3/cengal/code_flow_control/smart_values/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1235 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/code_flow_control/smart_values/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2828 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/code_flow_control/smart_values/versions/v_0/result_types.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.124812 cengal-3.1.18.3/cengal/code_flow_control/smart_values/versions/v_1/
--rw-r--r--   0 mb        (1000) mb        (1000)     1235 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/code_flow_control/smart_values/versions/v_1/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2839 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/code_flow_control/smart_values/versions/v_1/smart_values.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.124812 cengal-3.1.18.3/cengal/code_flow_control/smart_values/versions/v_2/
--rw-r--r--   0 mb        (1000) mb        (1000)     1235 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/code_flow_control/smart_values/versions/v_2/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3470 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/code_flow_control/smart_values/versions/v_2/smart_values.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.134812 cengal-3.1.18.3/cengal/code_inspection/
--rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/code_inspection/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.134812 cengal-3.1.18.3/cengal/code_inspection/auto_line_tracer/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/code_inspection/auto_line_tracer/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.134812 cengal-3.1.18.3/cengal/code_inspection/auto_line_tracer/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/code_inspection/auto_line_tracer/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.134812 cengal-3.1.18.3/cengal/code_inspection/auto_line_tracer/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1239 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/code_inspection/auto_line_tracer/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     6171 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/code_inspection/auto_line_tracer/versions/v_0/auto_line_tracer.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.134812 cengal-3.1.18.3/cengal/code_inspection/auto_line_tracer/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/code_inspection/auto_line_tracer/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/code_inspection/auto_line_tracer/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.134812 cengal-3.1.18.3/cengal/code_inspection/line_profiling/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/code_inspection/line_profiling/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.134812 cengal-3.1.18.3/cengal/code_inspection/line_profiling/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/code_inspection/line_profiling/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.134812 cengal-3.1.18.3/cengal/code_inspection/line_profiling/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1237 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/code_inspection/line_profiling/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2770 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/code_inspection/line_profiling/versions/v_0/line_profiling.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.134812 cengal-3.1.18.3/cengal/code_inspection/line_profiling/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/code_inspection/line_profiling/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/code_inspection/line_profiling/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.134812 cengal-3.1.18.3/cengal/code_inspection/line_tracer/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/code_inspection/line_tracer/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.134812 cengal-3.1.18.3/cengal/code_inspection/line_tracer/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/code_inspection/line_tracer/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.134812 cengal-3.1.18.3/cengal/code_inspection/line_tracer/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1234 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/code_inspection/line_tracer/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     4305 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/code_inspection/line_tracer/versions/v_0/line_tracer.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.134812 cengal-3.1.18.3/cengal/code_inspection/line_tracer/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/code_inspection/line_tracer/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/code_inspection/line_tracer/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.134812 cengal-3.1.18.3/cengal/cross_version/
--rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/cross_version/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.134812 cengal-3.1.18.3/cengal/cross_version/console_print/
--rw-r--r--   0 mb        (1000) mb        (1000)     1243 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/cross_version/console_print/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1264 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/cross_version/console_print/python3.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1529 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/cross_version/console_print/universal.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.134812 cengal-3.1.18.3/cengal/ctypes_tools/
--rw-r--r--   0 mb        (1000) mb        (1000)     1210 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/ctypes_tools/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.134812 cengal-3.1.18.3/cengal/ctypes_tools/constants/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/ctypes_tools/constants/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.134812 cengal-3.1.18.3/cengal/ctypes_tools/constants/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/ctypes_tools/constants/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.134812 cengal-3.1.18.3/cengal/ctypes_tools/constants/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1270 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/ctypes_tools/constants/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.134812 cengal-3.1.18.3/cengal/ctypes_tools/constants/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/ctypes_tools/constants/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/ctypes_tools/constants/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)    13438 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/ctypes_tools/constants/versions/v_0/win_constants.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.144812 cengal-3.1.18.3/cengal/ctypes_tools/function_prototypes/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/ctypes_tools/function_prototypes/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.144812 cengal-3.1.18.3/cengal/ctypes_tools/function_prototypes/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/ctypes_tools/function_prototypes/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.144812 cengal-3.1.18.3/cengal/ctypes_tools/function_prototypes/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1280 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/ctypes_tools/function_prototypes/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.144812 cengal-3.1.18.3/cengal/ctypes_tools/function_prototypes/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/ctypes_tools/function_prototypes/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/ctypes_tools/function_prototypes/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)     5488 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/ctypes_tools/function_prototypes/versions/v_0/win_function_prototypes.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.144812 cengal-3.1.18.3/cengal/ctypes_tools/functions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/ctypes_tools/functions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.144812 cengal-3.1.18.3/cengal/ctypes_tools/functions/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/ctypes_tools/functions/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.144812 cengal-3.1.18.3/cengal/ctypes_tools/functions/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1296 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/ctypes_tools/functions/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1317 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/ctypes_tools/functions/versions/v_0/functions.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.144812 cengal-3.1.18.3/cengal/ctypes_tools/functions/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/ctypes_tools/functions/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/ctypes_tools/functions/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1502 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/ctypes_tools/functions/versions/v_0/win_functions.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.144812 cengal-3.1.18.3/cengal/ctypes_tools/libraries/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/ctypes_tools/libraries/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.144812 cengal-3.1.18.3/cengal/ctypes_tools/libraries/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/ctypes_tools/libraries/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.154812 cengal-3.1.18.3/cengal/ctypes_tools/libraries/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1270 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/ctypes_tools/libraries/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.154812 cengal-3.1.18.3/cengal/ctypes_tools/libraries/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/ctypes_tools/libraries/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/ctypes_tools/libraries/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1482 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/ctypes_tools/libraries/versions/v_0/win_libraries.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.154812 cengal-3.1.18.3/cengal/ctypes_tools/result_api/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/ctypes_tools/result_api/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.154812 cengal-3.1.18.3/cengal/ctypes_tools/result_api/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/ctypes_tools/result_api/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.154812 cengal-3.1.18.3/cengal/ctypes_tools/result_api/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1336 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/ctypes_tools/result_api/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1222 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/ctypes_tools/result_api/versions/v_0/result_api.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1305 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/ctypes_tools/result_api/versions/v_0/result_api_exceptions.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.154812 cengal-3.1.18.3/cengal/ctypes_tools/result_api/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/ctypes_tools/result_api/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/ctypes_tools/result_api/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2729 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/ctypes_tools/result_api/versions/v_0/win_result_api.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.154812 cengal-3.1.18.3/cengal/ctypes_tools/tools/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/ctypes_tools/tools/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.154812 cengal-3.1.18.3/cengal/ctypes_tools/tools/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/ctypes_tools/tools/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.154812 cengal-3.1.18.3/cengal/ctypes_tools/tools/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1288 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/ctypes_tools/tools/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.154812 cengal-3.1.18.3/cengal/ctypes_tools/tools/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/ctypes_tools/tools/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/ctypes_tools/tools/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1597 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/ctypes_tools/tools/versions/v_0/tools.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1601 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/ctypes_tools/tools/versions/v_0/win_tools.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.154812 cengal-3.1.18.3/cengal/ctypes_tools/types/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/ctypes_tools/types/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.154812 cengal-3.1.18.3/cengal/ctypes_tools/types/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/ctypes_tools/types/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.154812 cengal-3.1.18.3/cengal/ctypes_tools/types/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1266 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/ctypes_tools/types/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.164812 cengal-3.1.18.3/cengal/ctypes_tools/types/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/ctypes_tools/types/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/ctypes_tools/types/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)     7773 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/ctypes_tools/types/versions/v_0/win_types.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.164812 cengal-3.1.18.3/cengal/cython_tools/
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/cython_tools/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1774 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/cython_tools/cythonyser_setup_runner.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.164812 cengal-3.1.18.3/cengal/data_containers/
--rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.164812 cengal-3.1.18.3/cengal/data_containers/compound_dict_management/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/compound_dict_management/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.164812 cengal-3.1.18.3/cengal/data_containers/compound_dict_management/manager/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/compound_dict_management/manager/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.164812 cengal-3.1.18.3/cengal/data_containers/compound_dict_management/manager/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/compound_dict_management/manager/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.164812 cengal-3.1.18.3/cengal/data_containers/compound_dict_management/manager/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/compound_dict_management/manager/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2229 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/compound_dict_management/manager/versions/v_0/manager.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.164812 cengal-3.1.18.3/cengal/data_containers/compound_dict_management/manager/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/compound_dict_management/manager/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/compound_dict_management/manager/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.164812 cengal-3.1.18.3/cengal/data_containers/compound_dict_management/manager/versions/v_1/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/compound_dict_management/manager/versions/v_1/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2212 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/compound_dict_management/manager/versions/v_1/manager.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.164812 cengal-3.1.18.3/cengal/data_containers/compound_dict_management/manager/versions/v_1/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/compound_dict_management/manager/versions/v_1/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/compound_dict_management/manager/versions/v_1/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.164812 cengal-3.1.18.3/cengal/data_containers/compound_dict_management/standard_library/
--rw-r--r--   0 mb        (1000) mb        (1000)     1279 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/compound_dict_management/standard_library/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.164812 cengal-3.1.18.3/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.164812 cengal-3.1.18.3/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.164812 cengal-3.1.18.3/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1252 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1542 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/versions/v_0/key__hashable__to__value__set.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.164812 cengal-3.1.18.3/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.164812 cengal-3.1.18.3/cengal/data_containers/compound_dict_management/standard_library/key_counter/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/compound_dict_management/standard_library/key_counter/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.174812 cengal-3.1.18.3/cengal/data_containers/compound_dict_management/standard_library/key_counter/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/compound_dict_management/standard_library/key_counter/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.174812 cengal-3.1.18.3/cengal/data_containers/compound_dict_management/standard_library/key_counter/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1234 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/compound_dict_management/standard_library/key_counter/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1598 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/compound_dict_management/standard_library/key_counter/versions/v_0/key_counter.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.174812 cengal-3.1.18.3/cengal/data_containers/compound_dict_management/standard_library/key_counter/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/compound_dict_management/standard_library/key_counter/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/compound_dict_management/standard_library/key_counter/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.174812 cengal-3.1.18.3/cengal/data_containers/dynamic_list_of_pieces/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/dynamic_list_of_pieces/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.174812 cengal-3.1.18.3/cengal/data_containers/dynamic_list_of_pieces/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/dynamic_list_of_pieces/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.174812 cengal-3.1.18.3/cengal/data_containers/dynamic_list_of_pieces/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1625 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/dynamic_list_of_pieces/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    28854 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/dynamic_list_of_pieces/versions/v_0/dynamic_list_of_pieces__python.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.174812 cengal-3.1.18.3/cengal/data_containers/dynamic_list_of_pieces/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/dynamic_list_of_pieces/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/dynamic_list_of_pieces/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.174812 cengal-3.1.18.3/cengal/data_containers/dynamic_list_of_pieces/versions/v_1/
--rw-r--r--   0 mb        (1000) mb        (1000)     1625 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/dynamic_list_of_pieces/versions/v_1/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    28797 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/dynamic_list_of_pieces/versions/v_1/dynamic_list_of_pieces__python.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.174812 cengal-3.1.18.3/cengal/data_containers/dynamic_list_of_pieces/versions/v_1/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/dynamic_list_of_pieces/versions/v_1/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/dynamic_list_of_pieces/versions/v_1/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.184812 cengal-3.1.18.3/cengal/data_containers/dynamic_tag_tree/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/dynamic_tag_tree/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.184812 cengal-3.1.18.3/cengal/data_containers/dynamic_tag_tree/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/dynamic_tag_tree/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.184812 cengal-3.1.18.3/cengal/data_containers/dynamic_tag_tree/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)    39956 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/dynamic_tag_tree/versions/v_0/TagDB.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1260 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/dynamic_tag_tree/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     5405 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/dynamic_tag_tree/versions/v_0/tag_db_interface.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.184812 cengal-3.1.18.3/cengal/data_containers/dynamic_tag_tree/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/dynamic_tag_tree/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/dynamic_tag_tree/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.184812 cengal-3.1.18.3/cengal/data_containers/dynamic_tag_tree/versions/v_1/
--rw-r--r--   0 mb        (1000) mb        (1000)    41895 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/dynamic_tag_tree/versions/v_1/TagDB.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1260 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/dynamic_tag_tree/versions/v_1/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    13150 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/dynamic_tag_tree/versions/v_1/tag_db_interface.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.184812 cengal-3.1.18.3/cengal/data_containers/dynamic_tag_tree/versions/v_1/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/dynamic_tag_tree/versions/v_1/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/dynamic_tag_tree/versions/v_1/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.184812 cengal-3.1.18.3/cengal/data_containers/dynamic_tag_tree/versions/v_2/
--rw-r--r--   0 mb        (1000) mb        (1000)     1260 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/dynamic_tag_tree/versions/v_2/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     9730 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/dynamic_tag_tree/versions/v_2/dynamic_tag_tree.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.184812 cengal-3.1.18.3/cengal/data_containers/dynamic_tag_tree/versions/v_2/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/dynamic_tag_tree/versions/v_2/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/dynamic_tag_tree/versions/v_2/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.184812 cengal-3.1.18.3/cengal/data_containers/fast_fifo/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/fast_fifo/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.194812 cengal-3.1.18.3/cengal/data_containers/fast_fifo/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/fast_fifo/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.194812 cengal-3.1.18.3/cengal/data_containers/fast_fifo/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1232 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/fast_fifo/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    12328 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/fast_fifo/versions/v_0/fast_fifo.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.194812 cengal-3.1.18.3/cengal/data_containers/fast_fifo/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/fast_fifo/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/fast_fifo/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.194812 cengal-3.1.18.3/cengal/data_containers/fast_fifo/versions/v_1/
--rw-r--r--   0 mb        (1000) mb        (1000)     1232 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/fast_fifo/versions/v_1/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    12276 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/fast_fifo/versions/v_1/fast_fifo.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.194812 cengal-3.1.18.3/cengal/data_containers/fast_fifo/versions/v_1/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/fast_fifo/versions/v_1/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/fast_fifo/versions/v_1/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.194812 cengal-3.1.18.3/cengal/data_containers/limitable_dict_with_order/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/limitable_dict_with_order/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.194812 cengal-3.1.18.3/cengal/data_containers/limitable_dict_with_order/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/limitable_dict_with_order/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.194812 cengal-3.1.18.3/cengal/data_containers/limitable_dict_with_order/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/limitable_dict_with_order/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2034 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/limitable_dict_with_order/versions/v_0/limitable_dict_with_order.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.194812 cengal-3.1.18.3/cengal/data_containers/limitable_dict_with_order/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/limitable_dict_with_order/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/limitable_dict_with_order/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.194812 cengal-3.1.18.3/cengal/data_containers/limitable_dict_with_order/versions/v_1/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/limitable_dict_with_order/versions/v_1/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2465 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/limitable_dict_with_order/versions/v_1/limitable_dict_with_order.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.194812 cengal-3.1.18.3/cengal/data_containers/limitable_dict_with_order/versions/v_1/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/limitable_dict_with_order/versions/v_1/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/limitable_dict_with_order/versions/v_1/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.194812 cengal-3.1.18.3/cengal/data_containers/simple_tree/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/simple_tree/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.194812 cengal-3.1.18.3/cengal/data_containers/simple_tree/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/simple_tree/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.194812 cengal-3.1.18.3/cengal/data_containers/simple_tree/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1234 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/simple_tree/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     5001 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/simple_tree/versions/v_0/simple_tree.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.194812 cengal-3.1.18.3/cengal/data_containers/stack/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/stack/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.194812 cengal-3.1.18.3/cengal/data_containers/stack/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/stack/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.194812 cengal-3.1.18.3/cengal/data_containers/stack/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1228 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/stack/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     4660 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/stack/versions/v_0/stack.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.204812 cengal-3.1.18.3/cengal/data_containers/stack/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1234 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/stack/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3696 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_containers/stack/versions/v_0/tests/test__stack.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.204812 cengal-3.1.18.3/cengal/data_generation/
--rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_generation/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.204812 cengal-3.1.18.3/cengal/data_generation/id_generator/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_generation/id_generator/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.204812 cengal-3.1.18.3/cengal/data_generation/id_generator/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_generation/id_generator/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.204812 cengal-3.1.18.3/cengal/data_generation/id_generator/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1235 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_generation/id_generator/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2218 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_generation/id_generator/versions/v_0/id_generator.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.204812 cengal-3.1.18.3/cengal/data_generation/id_generator/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_generation/id_generator/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_generation/id_generator/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.204812 cengal-3.1.18.3/cengal/data_generation/id_generator/versions/v_1/
--rw-r--r--   0 mb        (1000) mb        (1000)     1235 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_generation/id_generator/versions/v_1/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3045 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_generation/id_generator/versions/v_1/id_generator.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.204812 cengal-3.1.18.3/cengal/data_generation/id_generator/versions/v_1/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_generation/id_generator/versions/v_1/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_generation/id_generator/versions/v_1/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.204812 cengal-3.1.18.3/cengal/data_manipulation/
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.204812 cengal-3.1.18.3/cengal/data_manipulation/conversion/
--rw-r--r--   0 mb        (1000) mb        (1000)     1210 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/conversion/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.204812 cengal-3.1.18.3/cengal/data_manipulation/conversion/bit_cast_like/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/conversion/bit_cast_like/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.204812 cengal-3.1.18.3/cengal/data_manipulation/conversion/bit_cast_like/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/conversion/bit_cast_like/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.214813 cengal-3.1.18.3/cengal/data_manipulation/conversion/bit_cast_like/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1236 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/conversion/bit_cast_like/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2012 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/conversion/bit_cast_like/versions/v_0/bit_cast_like.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.214813 cengal-3.1.18.3/cengal/data_manipulation/conversion/bit_cast_like/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/conversion/bit_cast_like/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/conversion/bit_cast_like/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.214813 cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.214813 cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.214813 cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1239 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2476 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast/versions/v_0/reinterpret_cast.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.214813 cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.214813 cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast_management/
--rw-r--r--   0 mb        (1000) mb        (1000)     1210 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast_management/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.214813 cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.214813 cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.214813 cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     8111 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/versions/v_0/manager.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.224813 cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.224813 cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/
--rw-r--r--   0 mb        (1000) mb        (1000)     1210 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.224813 cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.224813 cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.224813 cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1235 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2549 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/versions/v_0/copy_wrapper.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.224813 cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.224813 cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.224813 cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.224813 cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1240 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2565 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/versions/v_0/deep_copy_wrapper.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.224813 cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.224813 cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.224813 cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.224813 cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1239 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.224813 cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3539 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/versions/v_0/uni_copy_wrapper.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.224813 cengal-3.1.18.3/cengal/data_manipulation/front_triggerable_variable/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/front_triggerable_variable/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.224813 cengal-3.1.18.3/cengal/data_manipulation/front_triggerable_variable/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/front_triggerable_variable/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.224813 cengal-3.1.18.3/cengal/data_manipulation/front_triggerable_variable/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1249 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/front_triggerable_variable/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3917 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/front_triggerable_variable/versions/v_0/front_triggerable_variable.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.224813 cengal-3.1.18.3/cengal/data_manipulation/front_triggerable_variable/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/front_triggerable_variable/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/front_triggerable_variable/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.224813 cengal-3.1.18.3/cengal/data_manipulation/get_dict_key_with_callable_default/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/get_dict_key_with_callable_default/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.224813 cengal-3.1.18.3/cengal/data_manipulation/get_dict_key_with_callable_default/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/get_dict_key_with_callable_default/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.234813 cengal-3.1.18.3/cengal/data_manipulation/get_dict_key_with_callable_default/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1257 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/get_dict_key_with_callable_default/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1484 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/get_dict_key_with_callable_default/versions/v_0/get_dict_key_with_callable_default.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.234813 cengal-3.1.18.3/cengal/data_manipulation/get_dict_key_with_callable_default/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/get_dict_key_with_callable_default/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/get_dict_key_with_callable_default/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)     7545 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/help_tools.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.234813 cengal-3.1.18.3/cengal/data_manipulation/objects_counter/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/objects_counter/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.234813 cengal-3.1.18.3/cengal/data_manipulation/objects_counter/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/objects_counter/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.234813 cengal-3.1.18.3/cengal/data_manipulation/objects_counter/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1238 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/objects_counter/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2981 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/objects_counter/versions/v_0/objects_counter.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.234813 cengal-3.1.18.3/cengal/data_manipulation/objects_counter/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1244 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/objects_counter/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     6512 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/objects_counter/versions/v_0/tests/test__objects_counter.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.234813 cengal-3.1.18.3/cengal/data_manipulation/performant_list_operations/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/performant_list_operations/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.234813 cengal-3.1.18.3/cengal/data_manipulation/performant_list_operations/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/performant_list_operations/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.244813 cengal-3.1.18.3/cengal/data_manipulation/performant_list_operations/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1245 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/performant_list_operations/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     9311 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/performant_list_operations/versions/v_0/remove_items_from_list.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.244813 cengal-3.1.18.3/cengal/data_manipulation/performant_list_operations/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/performant_list_operations/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/performant_list_operations/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.244813 cengal-3.1.18.3/cengal/data_manipulation/serialization/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/serialization/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.244813 cengal-3.1.18.3/cengal/data_manipulation/serialization/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/serialization/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.244813 cengal-3.1.18.3/cengal/data_manipulation/serialization/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1236 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/serialization/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    27321 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/serialization/versions/v_0/serialization.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.244813 cengal-3.1.18.3/cengal/data_manipulation/serialization/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1242 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/serialization/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     4071 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/serialization/versions/v_0/tests/test__serialization.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.244813 cengal-3.1.18.3/cengal/data_manipulation/tree_traversal/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/tree_traversal/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.244813 cengal-3.1.18.3/cengal/data_manipulation/tree_traversal/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/tree_traversal/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.244813 cengal-3.1.18.3/cengal/data_manipulation/tree_traversal/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1237 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/tree_traversal/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.244813 cengal-3.1.18.3/cengal/data_manipulation/tree_traversal/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/tree_traversal/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/tree_traversal/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2652 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/tree_traversal/versions/v_0/tests/traverstal_manual_tests.py
--rw-r--r--   0 mb        (1000) mb        (1000)     8192 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/tree_traversal/versions/v_0/tree_traversal.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.244813 cengal-3.1.18.3/cengal/data_manipulation/tree_traversal/versions/v_1/
--rw-r--r--   0 mb        (1000) mb        (1000)     1237 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/tree_traversal/versions/v_1/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.244813 cengal-3.1.18.3/cengal/data_manipulation/tree_traversal/versions/v_1/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/tree_traversal/versions/v_1/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/tree_traversal/versions/v_1/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2615 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/tree_traversal/versions/v_1/tests/key_multi_value_traverstal_manual_tests.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2814 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/tree_traversal/versions/v_1/tests/key_value_traverstal_manual_tests.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2747 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/tree_traversal/versions/v_1/tests/traverstal_manual_tests.py
--rw-r--r--   0 mb        (1000) mb        (1000)    24128 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/data_manipulation/tree_traversal/versions/v_1/tree_traversal.py
--rw-r--r--   0 mb        (1000) mb        (1000)     5496 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/docten.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.244813 cengal-3.1.18.3/cengal/entities/
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/entities/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.244813 cengal-3.1.18.3/cengal/entities/bindable_to_type/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/entities/bindable_to_type/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.244813 cengal-3.1.18.3/cengal/entities/bindable_to_type/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/entities/bindable_to_type/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.244813 cengal-3.1.18.3/cengal/entities/bindable_to_type/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1239 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/entities/bindable_to_type/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     4360 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/entities/bindable_to_type/versions/v_0/bindable_to_type.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.254813 cengal-3.1.18.3/cengal/entities/bindable_to_type/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/entities/bindable_to_type/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/entities/bindable_to_type/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.254813 cengal-3.1.18.3/cengal/entities/copyable/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/entities/copyable/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.254813 cengal-3.1.18.3/cengal/entities/copyable/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/entities/copyable/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.264813 cengal-3.1.18.3/cengal/entities/copyable/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/entities/copyable/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     4450 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/entities/copyable/versions/v_0/copyable.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.264813 cengal-3.1.18.3/cengal/entities/copyable/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/entities/copyable/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/entities/copyable/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.264813 cengal-3.1.18.3/cengal/file_settings_manager/
--rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/file_settings_manager/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     7336 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/file_settings_manager/config_manager.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2248 2023-05-21 17:03:53.000000 cengal-3.1.18.3/cengal/file_settings_manager/dir_templates.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.264813 cengal-3.1.18.3/cengal/file_system/
--rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/file_system/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.264813 cengal-3.1.18.3/cengal/file_system/app_fs_structure/
--rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/file_system/app_fs_structure/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.264813 cengal-3.1.18.3/cengal/file_system/app_fs_structure/app_dir_path/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/file_system/app_fs_structure/app_dir_path/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.264813 cengal-3.1.18.3/cengal/file_system/app_fs_structure/app_dir_path/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/file_system/app_fs_structure/app_dir_path/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.264813 cengal-3.1.18.3/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1548 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1289 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/app_dir_exceptions.py
--rw-r--r--   0 mb        (1000) mb        (1000)     4302 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/app_dir_path_base.py
--rw-r--r--   0 mb        (1000) mb        (1000)     8624 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/app_dir_path_darwin.py
--rw-r--r--   0 mb        (1000) mb        (1000)     8513 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/app_dir_path_linux.py
--rw-r--r--   0 mb        (1000) mb        (1000)     7083 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/app_dir_path_win.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3825 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/app_directory_types.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.264813 cengal-3.1.18.3/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)     8151 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/file_system/directory_manager.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2529 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/file_system/file_manager.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.264813 cengal-3.1.18.3/cengal/file_system/file_patch/
--rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/file_system/file_patch/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.264813 cengal-3.1.18.3/cengal/file_system/file_patch/brackets/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/file_system/file_patch/brackets/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.264813 cengal-3.1.18.3/cengal/file_system/file_patch/brackets/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/file_system/file_patch/brackets/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.264813 cengal-3.1.18.3/cengal/file_system/file_patch/brackets/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/file_system/file_patch/brackets/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2366 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/file_system/file_patch/brackets/versions/v_0/brackets.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.264813 cengal-3.1.18.3/cengal/file_system/file_patch/brackets/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/file_system/file_patch/brackets/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/file_system/file_patch/brackets/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.264813 cengal-3.1.18.3/cengal/file_system/file_patch/generic/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/file_system/file_patch/generic/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.274813 cengal-3.1.18.3/cengal/file_system/file_patch/generic/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/file_system/file_patch/generic/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.274813 cengal-3.1.18.3/cengal/file_system/file_patch/generic/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/file_system/file_patch/generic/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2228 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/file_system/file_patch/generic/versions/v_0/generic.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.274813 cengal-3.1.18.3/cengal/file_system/file_patch/generic/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/file_system/file_patch/generic/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/file_system/file_patch/generic/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.274813 cengal-3.1.18.3/cengal/file_system/file_patch/simple/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/file_system/file_patch/simple/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.274813 cengal-3.1.18.3/cengal/file_system/file_patch/simple/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/file_system/file_patch/simple/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.274813 cengal-3.1.18.3/cengal/file_system/file_patch/simple/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1229 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/file_system/file_patch/simple/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2311 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/file_system/file_patch/simple/versions/v_0/simple.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.284813 cengal-3.1.18.3/cengal/file_system/file_patch/simple/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/file_system/file_patch/simple/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/file_system/file_patch/simple/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.284813 cengal-3.1.18.3/cengal/file_system/path_manager/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/file_system/path_manager/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.284813 cengal-3.1.18.3/cengal/file_system/path_manager/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/file_system/path_manager/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.284813 cengal-3.1.18.3/cengal/file_system/path_manager/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1235 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/file_system/path_manager/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2581 2023-05-21 17:03:53.000000 cengal-3.1.18.3/cengal/file_system/path_manager/versions/v_0/path_manager.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.284813 cengal-3.1.18.3/cengal/file_system/path_manager/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/file_system/path_manager/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/file_system/path_manager/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.284813 cengal-3.1.18.3/cengal/file_system/win_fs/
--rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/file_system/win_fs/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3114 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/file_system/win_fs/base.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1851 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/file_system/win_fs/global_install_uninstall.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1997 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/file_system/win_fs/path.py
--rw-r--r--   0 mb        (1000) mb        (1000)     5190 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/file_system/win_fs/shutil.py
--rw-r--r--   0 mb        (1000) mb        (1000)     4437 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/file_system/win_fs/shutil_readable.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.284813 cengal-3.1.18.3/cengal/hardware/
--rw-r--r--   0 mb        (1000) mb        (1000)     1210 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/hardware/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.284813 cengal-3.1.18.3/cengal/hardware/info/
--rw-r--r--   0 mb        (1000) mb        (1000)     1210 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/hardware/info/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.284813 cengal-3.1.18.3/cengal/hardware/info/cpu/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/hardware/info/cpu/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.284813 cengal-3.1.18.3/cengal/hardware/info/cpu/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/hardware/info/cpu/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.284813 cengal-3.1.18.3/cengal/hardware/info/cpu/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/hardware/info/cpu/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2282 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/hardware/info/cpu/versions/v_0/cpu.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.284813 cengal-3.1.18.3/cengal/hardware/info/cpu/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/hardware/info/cpu/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/hardware/info/cpu/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.284813 cengal-3.1.18.3/cengal/hardware/info/cpu/versions/v_1/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/hardware/info/cpu/versions/v_1/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     8748 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/hardware/info/cpu/versions/v_1/cpu.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.284813 cengal-3.1.18.3/cengal/hardware/info/cpu/versions/v_1/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/hardware/info/cpu/versions/v_1/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/hardware/info/cpu/versions/v_1/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.284813 cengal-3.1.18.3/cengal/hardware/memory/
--rw-r--r--   0 mb        (1000) mb        (1000)     1210 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/hardware/memory/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.284813 cengal-3.1.18.3/cengal/hardware/memory/barriers/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/hardware/memory/barriers/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.284813 cengal-3.1.18.3/cengal/hardware/memory/barriers/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/hardware/memory/barriers/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.284813 cengal-3.1.18.3/cengal/hardware/memory/barriers/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1235 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/hardware/memory/barriers/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.284813 cengal-3.1.18.3/cengal/hardware/memory/barriers/versions/v_0/compilable/
--rw-r--r--   0 mb        (1000) mb        (1000)     2022 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/hardware/memory/barriers/versions/v_0/compilable/__build_config.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1355 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/hardware/memory/barriers/versions/v_0/compilable/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.284813 cengal-3.1.18.3/cengal/hardware/memory/barriers/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/hardware/memory/barriers/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/hardware/memory/barriers/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.284813 cengal-3.1.18.3/cengal/hardware/memory/shared_memory/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/hardware/memory/shared_memory/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.284813 cengal-3.1.18.3/cengal/hardware/memory/shared_memory/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/hardware/memory/shared_memory/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.304813 cengal-3.1.18.3/cengal/hardware/memory/shared_memory/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1349 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/hardware/memory/shared_memory/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.304813 cengal-3.1.18.3/cengal/hardware/memory/shared_memory/versions/v_0/compilable/
--rw-r--r--   0 mb        (1000) mb        (1000)     1933 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/hardware/memory/shared_memory/versions/v_0/compilable/__build_config.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1360 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/hardware/memory/shared_memory/versions/v_0/compilable/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     4230 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/hardware/memory/shared_memory/versions/v_0/interfaces.py
--rw-r--r--   0 mb        (1000) mb        (1000)   108883 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/hardware/memory/shared_memory/versions/v_0/shared_memory.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.304813 cengal-3.1.18.3/cengal/hardware/memory/shared_memory/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/hardware/memory/shared_memory/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/hardware/memory/shared_memory/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)     8553 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/help_tools.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.304813 cengal-3.1.18.3/cengal/introspection/
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/introspection/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.304813 cengal-3.1.18.3/cengal/introspection/inspect/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/introspection/inspect/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.304813 cengal-3.1.18.3/cengal/introspection/inspect/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/introspection/inspect/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.304813 cengal-3.1.18.3/cengal/introspection/inspect/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/introspection/inspect/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    19834 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/introspection/inspect/versions/v_0/inspect.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.304813 cengal-3.1.18.3/cengal/introspection/inspect/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/introspection/inspect/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/introspection/inspect/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.304813 cengal-3.1.18.3/cengal/introspection/third_party/
--rw-r--r--   0 mb        (1000) mb        (1000)     1210 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/introspection/third_party/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.304813 cengal-3.1.18.3/cengal/introspection/third_party/ctypes/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/introspection/third_party/ctypes/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.304813 cengal-3.1.18.3/cengal/introspection/third_party/ctypes/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/introspection/third_party/ctypes/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.304813 cengal-3.1.18.3/cengal/introspection/third_party/ctypes/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1229 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/introspection/third_party/ctypes/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     5359 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/introspection/third_party/ctypes/versions/v_0/ctypes.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.304813 cengal-3.1.18.3/cengal/introspection/third_party/ctypes/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/introspection/third_party/ctypes/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/introspection/third_party/ctypes/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.304813 cengal-3.1.18.3/cengal/io/
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.304813 cengal-3.1.18.3/cengal/io/asock_io/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/asock_io/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.304813 cengal-3.1.18.3/cengal/io/asock_io/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/asock_io/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.314813 cengal-3.1.18.3/cengal/io/asock_io/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1281 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/asock_io/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     6006 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/asock_io/versions/v_0/base.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.314813 cengal-3.1.18.3/cengal/io/asock_io/versions/v_0/recv_buff_size_computer/
--rw-r--r--   0 mb        (1000) mb        (1000)     1529 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/asock_io/versions/v_0/recv_buff_size_computer/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3192 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/asock_io/versions/v_0/recv_buff_size_computer/recv_buff_size_computer__python.py
--rw-r--r--   0 mb        (1000) mb        (1000)   113359 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/asock_io/versions/v_0/tcp_app_server.py
--rw-r--r--   0 mb        (1000) mb        (1000)     5057 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/asock_io/versions/v_0/tcp_link.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.314813 cengal-3.1.18.3/cengal/io/asock_io/versions/v_1/
--rw-r--r--   0 mb        (1000) mb        (1000)     1281 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/asock_io/versions/v_1/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    18746 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/asock_io/versions/v_1/abstract.py
--rw-r--r--   0 mb        (1000) mb        (1000)   123889 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/asock_io/versions/v_1/asock_io_core.py
--rw-r--r--   0 mb        (1000) mb        (1000)    15715 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/asock_io/versions/v_1/base.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.314813 cengal-3.1.18.3/cengal/io/asock_io/versions/v_1/io_loops/
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/asock_io/versions/v_1/io_loops/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3922 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/asock_io/versions/v_1/io_loops/epoll_lt.py
--rw-r--r--   0 mb        (1000) mb        (1000)     6409 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/asock_io/versions/v_1/io_loops/select.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.314813 cengal-3.1.18.3/cengal/io/asock_io/versions/v_1/recv_buff_size_computer/
--rw-r--r--   0 mb        (1000) mb        (1000)     1476 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/asock_io/versions/v_1/recv_buff_size_computer/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3130 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/asock_io/versions/v_1/recv_buff_size_computer/recv_buff_size_computer__python.py
--rw-r--r--   0 mb        (1000) mb        (1000)     4987 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/asock_io/versions/v_1/tcp_link.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.314813 cengal-3.1.18.3/cengal/io/core/
--rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/core/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.314813 cengal-3.1.18.3/cengal/io/core/memory_management/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/core/memory_management/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.314813 cengal-3.1.18.3/cengal/io/core/memory_management/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/core/memory_management/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.324813 cengal-3.1.18.3/cengal/io/core/memory_management/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1240 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/core/memory_management/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3262 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/core/memory_management/versions/v_0/memory_management.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.324813 cengal-3.1.18.3/cengal/io/core/memory_management/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/core/memory_management/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/core/memory_management/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.324813 cengal-3.1.18.3/cengal/io/named_connections/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/named_connections/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.324813 cengal-3.1.18.3/cengal/io/named_connections/named_connections_manager/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/named_connections/named_connections_manager/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.324813 cengal-3.1.18.3/cengal/io/named_connections/named_connections_manager/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/named_connections/named_connections_manager/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.324813 cengal-3.1.18.3/cengal/io/named_connections/named_connections_manager/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/named_connections/named_connections_manager/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    10644 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/named_connections/named_connections_manager/versions/v_0/named_connections_manager.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.324813 cengal-3.1.18.3/cengal/io/named_connections/named_connections_manager/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/named_connections/named_connections_manager/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/named_connections/named_connections_manager/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.324813 cengal-3.1.18.3/cengal/io/named_connections/workers/
--rw-r--r--   0 mb        (1000) mb        (1000)     1240 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/named_connections/workers/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.324813 cengal-3.1.18.3/cengal/io/named_connections/workers/asyncio_streams/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/named_connections/workers/asyncio_streams/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.324813 cengal-3.1.18.3/cengal/io/named_connections/workers/asyncio_streams/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/named_connections/workers/asyncio_streams/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.324813 cengal-3.1.18.3/cengal/io/named_connections/workers/asyncio_streams/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1238 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/named_connections/workers/asyncio_streams/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     6610 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/named_connections/workers/asyncio_streams/versions/v_0/asyncio_streams.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.324813 cengal-3.1.18.3/cengal/io/named_connections/workers/asyncio_streams/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/named_connections/workers/asyncio_streams/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/named_connections/workers/asyncio_streams/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.324813 cengal-3.1.18.3/cengal/io/named_connections/workers/asyncio_streams_proxy/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/named_connections/workers/asyncio_streams_proxy/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.324813 cengal-3.1.18.3/cengal/io/named_connections/workers/asyncio_streams_proxy/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/named_connections/workers/asyncio_streams_proxy/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.324813 cengal-3.1.18.3/cengal/io/named_connections/workers/asyncio_streams_proxy/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1244 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/named_connections/workers/asyncio_streams_proxy/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/named_connections/workers/asyncio_streams_proxy/versions/v_0/asyncio_streams_proxy.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.324813 cengal-3.1.18.3/cengal/io/named_connections/workers/asyncio_streams_proxy/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/named_connections/workers/asyncio_streams_proxy/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/named_connections/workers/asyncio_streams_proxy/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.324813 cengal-3.1.18.3/cengal/io/net_io/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/net_io/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.334812 cengal-3.1.18.3/cengal/io/net_io/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/net_io/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.334812 cengal-3.1.18.3/cengal/io/net_io/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/net_io/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.344812 cengal-3.1.18.3/cengal/io/net_io/versions/v_0/crossplatform/
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/net_io/versions/v_0/crossplatform/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.344812 cengal-3.1.18.3/cengal/io/net_io/versions/v_0/crossplatform/exceptions_handlers/
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/net_io/versions/v_0/crossplatform/exceptions_handlers/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/net_io/versions/v_0/crossplatform/exceptions_handlers/abstract.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/net_io/versions/v_0/crossplatform/exceptions_handlers/linux.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/net_io/versions/v_0/crossplatform/exceptions_handlers/win32.py
--rw-r--r--   0 mb        (1000) mb        (1000)    11975 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/net_io/versions/v_0/net_io__linux.py
--rw-r--r--   0 mb        (1000) mb        (1000)    14773 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/net_io/versions/v_0/net_io_abstract.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3987 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/net_io/versions/v_0/net_io_method__epoll_lt.py
--rw-r--r--   0 mb        (1000) mb        (1000)     4846 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/net_io/versions/v_0/net_io_method__select.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.344812 cengal-3.1.18.3/cengal/io/recv_buff_size_computer/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/recv_buff_size_computer/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.344812 cengal-3.1.18.3/cengal/io/recv_buff_size_computer/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/recv_buff_size_computer/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.344812 cengal-3.1.18.3/cengal/io/recv_buff_size_computer/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1529 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/recv_buff_size_computer/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3192 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/recv_buff_size_computer/versions/v_0/recv_buff_size_computer__python.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.344812 cengal-3.1.18.3/cengal/io/recv_buff_size_computer/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/recv_buff_size_computer/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/recv_buff_size_computer/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.344812 cengal-3.1.18.3/cengal/io/recv_buff_size_computer/versions/v_1/
--rw-r--r--   0 mb        (1000) mb        (1000)     1476 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/recv_buff_size_computer/versions/v_1/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3130 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/recv_buff_size_computer/versions/v_1/recv_buff_size_computer__python.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.344812 cengal-3.1.18.3/cengal/io/recv_buff_size_computer/versions/v_1/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/recv_buff_size_computer/versions/v_1/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/recv_buff_size_computer/versions/v_1/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.344812 cengal-3.1.18.3/cengal/io/serve_free_ports/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/serve_free_ports/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.344812 cengal-3.1.18.3/cengal/io/serve_free_ports/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/serve_free_ports/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.344812 cengal-3.1.18.3/cengal/io/serve_free_ports/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1239 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/serve_free_ports/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     5139 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/serve_free_ports/versions/v_0/serve_free_ports.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.344812 cengal-3.1.18.3/cengal/io/serve_free_ports/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/serve_free_ports/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/serve_free_ports/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.344812 cengal-3.1.18.3/cengal/io/socket/
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/socket/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.344812 cengal-3.1.18.3/cengal/io/socket/constants/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/socket/constants/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.344812 cengal-3.1.18.3/cengal/io/socket/constants/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/socket/constants/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.344812 cengal-3.1.18.3/cengal/io/socket/constants/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1232 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/socket/constants/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1282 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/socket/constants/versions/v_0/constants.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.344812 cengal-3.1.18.3/cengal/io/socket/constants/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/socket/constants/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/socket/constants/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.344812 cengal-3.1.18.3/cengal/io/socket/errors/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/socket/errors/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.344812 cengal-3.1.18.3/cengal/io/socket/errors/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/socket/errors/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.354812 cengal-3.1.18.3/cengal/io/socket/errors/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1229 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/socket/errors/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2430 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/socket/errors/versions/v_0/errors.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.354812 cengal-3.1.18.3/cengal/io/socket/errors/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/socket/errors/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/socket/errors/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.354812 cengal-3.1.18.3/cengal/io/used_ports/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/used_ports/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.354812 cengal-3.1.18.3/cengal/io/used_ports/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/used_ports/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.354812 cengal-3.1.18.3/cengal/io/used_ports/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1233 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/used_ports/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.354812 cengal-3.1.18.3/cengal/io/used_ports/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/used_ports/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3133 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/used_ports/versions/v_0/tests/_test__used_ports.py
--rw-r--r--   0 mb        (1000) mb        (1000)     8979 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/io/used_ports/versions/v_0/used_ports.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.354812 cengal-3.1.18.3/cengal/math/
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/math/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.354812 cengal-3.1.18.3/cengal/math/algebra/
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/math/algebra/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.354812 cengal-3.1.18.3/cengal/math/algebra/fast_algorithms/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/math/algebra/fast_algorithms/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.354812 cengal-3.1.18.3/cengal/math/algebra/fast_algorithms/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/math/algebra/fast_algorithms/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.364812 cengal-3.1.18.3/cengal/math/algebra/fast_algorithms/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1238 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/math/algebra/fast_algorithms/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1784 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/math/algebra/fast_algorithms/versions/v_0/fast_algorithms.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.364812 cengal-3.1.18.3/cengal/math/algebra/fast_algorithms/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/math/algebra/fast_algorithms/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/math/algebra/fast_algorithms/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.364812 cengal-3.1.18.3/cengal/math/geometry/
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/math/geometry/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.364812 cengal-3.1.18.3/cengal/math/geometry/ellipse/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/math/geometry/ellipse/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.364812 cengal-3.1.18.3/cengal/math/geometry/ellipse/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/math/geometry/ellipse/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.364812 cengal-3.1.18.3/cengal/math/geometry/ellipse/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/math/geometry/ellipse/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     4989 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/math/geometry/ellipse/versions/v_0/ellipse.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.364812 cengal-3.1.18.3/cengal/math/geometry/ellipse/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/math/geometry/ellipse/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/math/geometry/ellipse/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2714 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/math/geometry/ellipse/versions/v_0/tests/informal_tests.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.364812 cengal-3.1.18.3/cengal/math/geometry/point/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/math/geometry/point/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.364812 cengal-3.1.18.3/cengal/math/geometry/point/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/math/geometry/point/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.364812 cengal-3.1.18.3/cengal/math/geometry/point/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1228 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/math/geometry/point/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    16020 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/math/geometry/point/versions/v_0/point.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.364812 cengal-3.1.18.3/cengal/math/geometry/point/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/math/geometry/point/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/math/geometry/point/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.364812 cengal-3.1.18.3/cengal/math/geometry/vector/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/math/geometry/vector/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.364812 cengal-3.1.18.3/cengal/math/geometry/vector/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/math/geometry/vector/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.364812 cengal-3.1.18.3/cengal/math/geometry/vector/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1229 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/math/geometry/vector/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.364812 cengal-3.1.18.3/cengal/math/geometry/vector/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/math/geometry/vector/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/math/geometry/vector/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)    46033 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/math/geometry/vector/versions/v_0/vector.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.364812 cengal-3.1.18.3/cengal/math/numbers/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/math/numbers/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.364812 cengal-3.1.18.3/cengal/math/numbers/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/math/numbers/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.364812 cengal-3.1.18.3/cengal/math/numbers/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/math/numbers/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1347 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/math/numbers/versions/v_0/numbers.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.364812 cengal-3.1.18.3/cengal/math/numbers/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/math/numbers/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/math/numbers/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.364812 cengal-3.1.18.3/cengal/modules_management/
--rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/modules_management/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1570 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/modules_management/alternative_import.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.364812 cengal-3.1.18.3/cengal/modules_management/ignore_in_build_mode/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/modules_management/ignore_in_build_mode/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.364812 cengal-3.1.18.3/cengal/modules_management/ignore_in_build_mode/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/modules_management/ignore_in_build_mode/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.364812 cengal-3.1.18.3/cengal/modules_management/ignore_in_build_mode/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1243 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/modules_management/ignore_in_build_mode/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1512 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/modules_management/ignore_in_build_mode/versions/v_0/ignore_in_build_mode.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.364812 cengal-3.1.18.3/cengal/modules_management/ignore_in_build_mode/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/modules_management/ignore_in_build_mode/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/modules_management/ignore_in_build_mode/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2183 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/modules_management/reload_module.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.364812 cengal-3.1.18.3/cengal/os/
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/os/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1349 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/os/help_tools.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.374812 cengal-3.1.18.3/cengal/parallel_execution/
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.374812 cengal-3.1.18.3/cengal/parallel_execution/asyncio/
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/asyncio/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.374812 cengal-3.1.18.3/cengal/parallel_execution/asyncio/atasks/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/asyncio/atasks/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.374812 cengal-3.1.18.3/cengal/parallel_execution/asyncio/atasks/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/asyncio/atasks/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.374812 cengal-3.1.18.3/cengal/parallel_execution/asyncio/atasks/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1229 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/asyncio/atasks/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1848 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/asyncio/atasks/versions/v_0/atasks.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.374812 cengal-3.1.18.3/cengal/parallel_execution/asyncio/atasks/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/asyncio/atasks/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/asyncio/atasks/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.374812 cengal-3.1.18.3/cengal/parallel_execution/asyncio/efficient_streams/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/asyncio/efficient_streams/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.374812 cengal-3.1.18.3/cengal/parallel_execution/asyncio/efficient_streams/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/asyncio/efficient_streams/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.374812 cengal-3.1.18.3/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1361 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    12105 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/efficient_streams_abstract.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2468 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/efficient_streams_base.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1990 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/efficient_streams_base_internal.py
--rw-r--r--   0 mb        (1000) mb        (1000)    51582 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/tcp_efficient_streams.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.384812 cengal-3.1.18.3/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3773 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/tests/asyncio_streams_client.py
--rw-r--r--   0 mb        (1000) mb        (1000)     6498 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/tests/asyncio_streams_server.py
--rw-r--r--   0 mb        (1000) mb        (1000)    35910 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/udp_efficient_streams.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.384812 cengal-3.1.18.3/cengal/parallel_execution/asyncio/init_loop/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/asyncio/init_loop/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.384812 cengal-3.1.18.3/cengal/parallel_execution/asyncio/init_loop/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/asyncio/init_loop/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.384812 cengal-3.1.18.3/cengal/parallel_execution/asyncio/init_loop/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1232 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/asyncio/init_loop/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1393 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/asyncio/init_loop/versions/v_0/init_loop.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.384812 cengal-3.1.18.3/cengal/parallel_execution/asyncio/init_loop/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/asyncio/init_loop/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/asyncio/init_loop/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.384812 cengal-3.1.18.3/cengal/parallel_execution/asyncio/run_in_process_pool/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/asyncio/run_in_process_pool/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.384812 cengal-3.1.18.3/cengal/parallel_execution/asyncio/run_in_process_pool/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/asyncio/run_in_process_pool/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.384812 cengal-3.1.18.3/cengal/parallel_execution/asyncio/run_in_process_pool/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1242 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/asyncio/run_in_process_pool/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     9440 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/asyncio/run_in_process_pool/versions/v_0/run_in_process_pool.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.384812 cengal-3.1.18.3/cengal/parallel_execution/asyncio/run_in_process_pool/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/asyncio/run_in_process_pool/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/asyncio/run_in_process_pool/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.384812 cengal-3.1.18.3/cengal/parallel_execution/asyncio/run_loop/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/asyncio/run_loop/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.384812 cengal-3.1.18.3/cengal/parallel_execution/asyncio/run_loop/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/asyncio/run_loop/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.384812 cengal-3.1.18.3/cengal/parallel_execution/asyncio/run_loop/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/asyncio/run_loop/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3527 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/asyncio/run_loop/versions/v_0/run_loop.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.384812 cengal-3.1.18.3/cengal/parallel_execution/asyncio/run_loop/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/asyncio/run_loop/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/asyncio/run_loop/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.384812 cengal-3.1.18.3/cengal/parallel_execution/asyncio/timed_yield/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/asyncio/timed_yield/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.384812 cengal-3.1.18.3/cengal/parallel_execution/asyncio/timed_yield/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/asyncio/timed_yield/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.384812 cengal-3.1.18.3/cengal/parallel_execution/asyncio/timed_yield/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1234 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/asyncio/timed_yield/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.384812 cengal-3.1.18.3/cengal/parallel_execution/asyncio/timed_yield/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/asyncio/timed_yield/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/asyncio/timed_yield/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1642 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/asyncio/timed_yield/versions/v_0/timed_yield.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.384812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/
--rw-r--r--   0 mb        (1000) mb        (1000)     1301 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.384812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_scheduler/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_scheduler/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.384812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_scheduler/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_scheduler/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.384812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_scheduler/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1237 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_scheduler/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)   126514 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_scheduler/versions/v_0/coro_scheduler.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.384812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_scheduler/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_scheduler/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_scheduler/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.384812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/
--rw-r--r--   0 mb        (1000) mb        (1000)     1453 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.384812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.384812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.394812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1238 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    11265 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/versions/v_0/async_event_bus.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.394812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.394812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.394812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.394812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1235 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    20728 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/versions/v_0/asyncio_loop.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.394812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.394812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/communication/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/communication/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.394812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/communication/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/communication/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.394812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/communication/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1236 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/communication/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     6566 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/communication/versions/v_0/communication.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.404812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/communication/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/communication/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/communication/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.404812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.404812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.454812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     4174 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/versions/v_0/cpu_tick_count_per_second.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.454812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.454812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/db/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/db/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.454812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/db/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/db/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.454812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/db/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/db/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    55878 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/db/versions/v_0/db.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.454812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/db/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/db/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/db/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.454812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.454812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.454812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1232 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     7707 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/versions/v_0/event_bus.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.454812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.454812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.454812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.464812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1238 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     7638 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/versions/v_0/fast_aggregator.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.464812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.464812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/instance/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/instance/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.464812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/instance/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/instance/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.464812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/instance/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/instance/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     9089 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/instance/versions/v_0/instance.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.464812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/instance/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/instance/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/instance/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.464812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.464812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.464812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1232 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     5522 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/versions/v_0/kill_coro.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.464812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.464812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.464812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.474813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1237 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     7537 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/versions/v_0/kill_coro_list.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.484813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.484813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.484813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.494813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1233 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3908 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/versions/v_0/lazy_print.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.494813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.494813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.494813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.494813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1227 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    21255 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/versions/v_0/lmdb.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.494813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.494813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/log/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/log/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.494813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/log/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/log/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.494813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/log/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/log/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    13686 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/log/versions/v_0/log.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.494813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/log/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/log/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/log/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.494813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.494813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.494813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1265 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     5971 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/v_0/bytecode_patcher.py
--rw-r--r--   0 mb        (1000) mb        (1000)    27436 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/v_0/loop_yield.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.494813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.494813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.494813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.494813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    22657 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/versions/v_0/put_coro.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.494813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.494813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.494813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.494813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1236 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     6168 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/versions/v_0/put_coro_list.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.494813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.494813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.494813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.504813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1240 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    25204 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/versions/v_0/read_write_locker.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.514813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.514813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.514813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.514813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1235 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     4956 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/class_info.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3827 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/commands.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1399 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/exceptions.py
--rw-r--r--   0 mb        (1000) mb        (1000)     5316 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/remote_node.py
--rw-r--r--   0 mb        (1000) mb        (1000)    21055 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/remote_nodes.py
--rw-r--r--   0 mb        (1000) mb        (1000)     6044 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/request_class_info.py
--rw-r--r--   0 mb        (1000) mb        (1000)     5877 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/serializers.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.514813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.514813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.514813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.514813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3465 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/versions/v_0/run_coro.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.524813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.524813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.524813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.524813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1236 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1748 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/versions/v_0/shutdown_loop.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.524813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.524813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.524813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.524813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1253 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2897 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/versions/v_0/shutdown_on_keyboard_interrupt.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.524813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.524813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.524813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.524813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1235 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1652 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/versions/v_0/simple_yield.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.534813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.534813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/sleep/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/sleep/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.534813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/sleep/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/sleep/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.544813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/sleep/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1232 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/sleep/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2901 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/sleep/versions/v_0/sleep.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.544813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/sleep/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/sleep/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/sleep/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.544813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.544813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.544813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1235 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1725 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/versions/v_0/some_printer.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.564813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.564813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.564813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.564813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1233 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.564813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)     6825 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/versions/v_0/throw_coro.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.564813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.564813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.564813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1238 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.564813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)     7154 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/versions/v_0/throw_coro_list.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.564813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.564813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.564813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1240 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.564813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)    11822 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/versions/v_0/timer_coro_runner.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.564813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.564813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.564813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1240 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.564813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)    11053 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/versions/v_0/timer_func_runner.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.564813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.564813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.564813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.564813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)    28117 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/v_0/tkinter.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.564813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.564813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.564813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1232 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.564813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)    18947 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/versions/v_0/wait_coro.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.564813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/
--rw-r--r--   0 mb        (1000) mb        (1000)     1210 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.564813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.564813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.574813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/versions/v_0/general.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.574813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.574813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.574813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.574813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1252 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     5687 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/versions/v_0/service_with_a_direct_request.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.574813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.574813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/
--rw-r--r--   0 mb        (1000) mb        (1000)     1233 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.574813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/await_coro/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/await_coro/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.574813 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/await_coro/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/await_coro/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.584812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/await_coro/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1233 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/await_coro/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    14142 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/await_coro/versions/v_0/await_coro.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.584812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/await_coro/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/await_coro/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/await_coro/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.584812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.584812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.584812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1240 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     5186 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/versions/v_0/coro_flow_control.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.584812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.584812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/low_latency/
--rw-r--r--   0 mb        (1000) mb        (1000)     1227 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/low_latency/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.584812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.584812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.584812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3175 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/v_0/ajson.py
--rw-r--r--   0 mb        (1000) mb        (1000)     5182 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/v_0/json.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.584812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.584812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.584812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.584812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1235 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     5979 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/versions/v_0/prepare_loop.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.584812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.584812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.584812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.594812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1234 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     8391 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/v_0/run_in_loop.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.594812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.594812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/wait_coro/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/wait_coro/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.594812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/wait_coro/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/wait_coro/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.594812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/wait_coro/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1232 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/wait_coro/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.594812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/wait_coro/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/wait_coro/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/wait_coro/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)     7876 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/wait_coro/versions/v_0/wait_coro.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.594812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/
--rw-r--r--   0 mb        (1000) mb        (1000)     1210 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.594812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/customtkinter/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/customtkinter/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.604812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/customtkinter/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/customtkinter/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.604812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/customtkinter/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1236 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/customtkinter/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1829 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/customtkinter/versions/v_0/customtkinter.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.604812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/customtkinter/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/customtkinter/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/customtkinter/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.604812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/nicegui/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/nicegui/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.604812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/nicegui/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/nicegui/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.604812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/nicegui/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/nicegui/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    19201 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/nicegui/versions/v_0/nicegui.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.604812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/nicegui/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/nicegui/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/nicegui/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.604812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/pytermgui/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/pytermgui/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.604812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.604812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1232 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     4691 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/v_0/pytermgui.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.604812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.604812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/qt/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/qt/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.604812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/qt/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/qt/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.604812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/qt/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/qt/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    13310 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/qt/versions/v_0/qt.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.604812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/qt/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/qt/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/qt/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.604812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/uvicorn/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/uvicorn/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.604812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/uvicorn/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/uvicorn/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.604812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/uvicorn/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/uvicorn/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.604812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/uvicorn/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/uvicorn/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/uvicorn/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)     5547 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/uvicorn/versions/v_0/uvicorn.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.604812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/uvloop/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/uvloop/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.604812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/uvloop/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/uvloop/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.604812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/uvloop/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1229 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/uvloop/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.604812 cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/uvloop/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/uvloop/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/uvloop/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1530 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/uvloop/versions/v_0/uvloop.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.614812 cengal-3.1.18.3/cengal/parallel_execution/green_threads_tools/
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/green_threads_tools/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3707 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/green_threads_tools/task_management.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.614812 cengal-3.1.18.3/cengal/parallel_execution/multiprocess/
--rw-r--r--   0 mb        (1000) mb        (1000)     1251 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/multiprocess/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2840 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/multiprocess/multiprocess_testing.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3086 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/multiprocess/multiprocessing_task_pool.py
--rw-r--r--   0 mb        (1000) mb        (1000)    24843 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/multiprocess/multiprocessing_task_runner.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.624812 cengal-3.1.18.3/cengal/parallel_execution/multithreading/
--rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/multithreading/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     7151 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/parallel_execution/multithreading/thread_workers_pool.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.624812 cengal-3.1.18.3/cengal/performance_test_lib/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/performance_test_lib/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.624812 cengal-3.1.18.3/cengal/performance_test_lib/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/performance_test_lib/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.624812 cengal-3.1.18.3/cengal/performance_test_lib/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1243 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/performance_test_lib/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     8268 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/performance_test_lib/versions/v_0/performance_test_lib.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.624812 cengal-3.1.18.3/cengal/performance_test_lib/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1249 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/performance_test_lib/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2241 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/performance_test_lib/versions/v_0/tests/test__performance_test_lib.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.624812 cengal-3.1.18.3/cengal/performance_test_lib/versions/v_1/
--rw-r--r--   0 mb        (1000) mb        (1000)     1243 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/performance_test_lib/versions/v_1/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     9291 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/performance_test_lib/versions/v_1/performance_test_lib.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.624812 cengal-3.1.18.3/cengal/performance_test_lib/versions/v_1/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1249 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/performance_test_lib/versions/v_1/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2241 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/performance_test_lib/versions/v_1/tests/test__performance_test_lib.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.624812 cengal-3.1.18.3/cengal/shared_memory/
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/shared_memory/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.624812 cengal-3.1.18.3/cengal/shared_memory/versions/
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.624812 cengal-3.1.18.3/cengal/shared_memory/versions/1/
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/shared_memory/versions/1/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1502 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/shared_memory/versions/1/mmap.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/shared_memory/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.624812 cengal-3.1.18.3/cengal/statistics/
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/statistics/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.624812 cengal-3.1.18.3/cengal/statistics/normal_distribution/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/statistics/normal_distribution/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.624812 cengal-3.1.18.3/cengal/statistics/normal_distribution/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/statistics/normal_distribution/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.624812 cengal-3.1.18.3/cengal/statistics/normal_distribution/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1242 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/statistics/normal_distribution/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     4157 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/statistics/normal_distribution/versions/v_0/normal_distribution.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.624812 cengal-3.1.18.3/cengal/statistics/normal_distribution/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/statistics/normal_distribution/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/statistics/normal_distribution/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3262 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/system.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.624812 cengal-3.1.18.3/cengal/testing_lib/
--rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/testing_lib/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3057 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/testing_lib/tests_list_runner.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.624812 cengal-3.1.18.3/cengal/text_processing/
--rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/text_processing/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.624812 cengal-3.1.18.3/cengal/text_processing/brackets_processing/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/text_processing/brackets_processing/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.624812 cengal-3.1.18.3/cengal/text_processing/brackets_processing/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/text_processing/brackets_processing/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.624812 cengal-3.1.18.3/cengal/text_processing/brackets_processing/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1290 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/text_processing/brackets_processing/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2345 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/text_processing/brackets_processing/versions/v_0/brackets.py
--rw-r--r--   0 mb        (1000) mb        (1000)     6468 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/text_processing/brackets_processing/versions/v_0/processing.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3780 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/text_processing/brackets_processing/versions/v_0/standard_brackets.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.624812 cengal-3.1.18.3/cengal/text_processing/brackets_processing/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/text_processing/brackets_processing/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/text_processing/brackets_processing/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.624812 cengal-3.1.18.3/cengal/text_processing/encoding_detection/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/text_processing/encoding_detection/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.624812 cengal-3.1.18.3/cengal/text_processing/encoding_detection/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/text_processing/encoding_detection/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.634812 cengal-3.1.18.3/cengal/text_processing/encoding_detection/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1241 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/text_processing/encoding_detection/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2465 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/text_processing/encoding_detection/versions/v_0/encoding_detection.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.644812 cengal-3.1.18.3/cengal/text_processing/encoding_detection/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/text_processing/encoding_detection/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/text_processing/encoding_detection/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)    11969 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/text_processing/help_tools.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.644812 cengal-3.1.18.3/cengal/text_processing/optional_formatter/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/text_processing/optional_formatter/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.644812 cengal-3.1.18.3/cengal/text_processing/optional_formatter/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/text_processing/optional_formatter/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.644812 cengal-3.1.18.3/cengal/text_processing/optional_formatter/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1241 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/text_processing/optional_formatter/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     4275 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/text_processing/optional_formatter/versions/v_0/optional_formatter.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.644812 cengal-3.1.18.3/cengal/text_processing/optional_formatter/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/text_processing/optional_formatter/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/text_processing/optional_formatter/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.644812 cengal-3.1.18.3/cengal/text_processing/simple_config_file_processor/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/text_processing/simple_config_file_processor/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.644812 cengal-3.1.18.3/cengal/text_processing/simple_config_file_processor/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/text_processing/simple_config_file_processor/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.644812 cengal-3.1.18.3/cengal/text_processing/simple_config_file_processor/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1251 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/text_processing/simple_config_file_processor/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/text_processing/simple_config_file_processor/versions/v_0/simple_config_file_processor.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.644812 cengal-3.1.18.3/cengal/text_processing/simple_config_file_processor/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/text_processing/simple_config_file_processor/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/text_processing/simple_config_file_processor/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.644812 cengal-3.1.18.3/cengal/text_processing/text_patch/
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/text_processing/text_patch/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.644812 cengal-3.1.18.3/cengal/text_processing/text_patch/brackets/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/text_processing/text_patch/brackets/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.644812 cengal-3.1.18.3/cengal/text_processing/text_patch/brackets/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/text_processing/text_patch/brackets/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.644812 cengal-3.1.18.3/cengal/text_processing/text_patch/brackets/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/text_processing/text_patch/brackets/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2010 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/text_processing/text_patch/brackets/versions/v_0/brackets.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.644812 cengal-3.1.18.3/cengal/text_processing/text_patch/brackets/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/text_processing/text_patch/brackets/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/text_processing/text_patch/brackets/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.644812 cengal-3.1.18.3/cengal/text_processing/text_patch/simple/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/text_processing/text_patch/simple/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.644812 cengal-3.1.18.3/cengal/text_processing/text_patch/simple/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/text_processing/text_patch/simple/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.644812 cengal-3.1.18.3/cengal/text_processing/text_patch/simple/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1229 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/text_processing/text_patch/simple/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1830 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/text_processing/text_patch/simple/versions/v_0/simple.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.644812 cengal-3.1.18.3/cengal/text_processing/text_patch/simple/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/text_processing/text_patch/simple/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/text_processing/text_patch/simple/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.654812 cengal-3.1.18.3/cengal/text_processing/text_processing/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/text_processing/text_processing/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.654812 cengal-3.1.18.3/cengal/text_processing/text_processing/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/text_processing/text_processing/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.654812 cengal-3.1.18.3/cengal/text_processing/text_processing/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1233 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/text_processing/text_processing/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     6282 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/text_processing/text_processing/versions/v_0/processing.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.654812 cengal-3.1.18.3/cengal/text_processing/text_processing/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/text_processing/text_processing/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/text_processing/text_processing/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.654812 cengal-3.1.18.3/cengal/text_processing/text_translator/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/text_processing/text_translator/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.664812 cengal-3.1.18.3/cengal/text_processing/text_translator/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/text_processing/text_translator/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.664812 cengal-3.1.18.3/cengal/text_processing/text_translator/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1238 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/text_processing/text_translator/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.664812 cengal-3.1.18.3/cengal/text_processing/text_translator/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/text_processing/text_translator/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/text_processing/text_translator/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)    12696 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/text_processing/text_translator/versions/v_0/text_translator.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.664812 cengal-3.1.18.3/cengal/text_processing/utf_bom_processing/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/text_processing/utf_bom_processing/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.664812 cengal-3.1.18.3/cengal/text_processing/utf_bom_processing/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/text_processing/utf_bom_processing/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.664812 cengal-3.1.18.3/cengal/text_processing/utf_bom_processing/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1241 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/text_processing/utf_bom_processing/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.664812 cengal-3.1.18.3/cengal/text_processing/utf_bom_processing/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/text_processing/utf_bom_processing/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/text_processing/utf_bom_processing/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2994 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/text_processing/utf_bom_processing/versions/v_0/utf_bom_processing.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.664812 cengal-3.1.18.3/cengal/time_management/
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/time_management/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.664812 cengal-3.1.18.3/cengal/time_management/cpu_clock/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/time_management/cpu_clock/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.664812 cengal-3.1.18.3/cengal/time_management/cpu_clock/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/time_management/cpu_clock/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.664812 cengal-3.1.18.3/cengal/time_management/cpu_clock/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1232 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/time_management/cpu_clock/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.664812 cengal-3.1.18.3/cengal/time_management/cpu_clock/versions/v_0/compilable/
--rw-r--r--   0 mb        (1000) mb        (1000)     1357 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/time_management/cpu_clock/versions/v_0/compilable/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1930 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/time_management/cpu_clock/versions/v_0/compilable/__x__build_config.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1640 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/time_management/cpu_clock/versions/v_0/cpu_clock.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.664812 cengal-3.1.18.3/cengal/time_management/cpu_clock/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/time_management/cpu_clock/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/time_management/cpu_clock/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.664812 cengal-3.1.18.3/cengal/time_management/cpu_clock_cycles/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/time_management/cpu_clock_cycles/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.664812 cengal-3.1.18.3/cengal/time_management/cpu_clock_cycles/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/time_management/cpu_clock_cycles/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.664812 cengal-3.1.18.3/cengal/time_management/cpu_clock_cycles/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1233 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/time_management/cpu_clock_cycles/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.664812 cengal-3.1.18.3/cengal/time_management/cpu_clock_cycles/versions/v_0/compilable/
--rw-r--r--   0 mb        (1000) mb        (1000)     1936 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/time_management/cpu_clock_cycles/versions/v_0/compilable/__build_config.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1412 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/time_management/cpu_clock_cycles/versions/v_0/compilable/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.664812 cengal-3.1.18.3/cengal/time_management/cpu_clock_cycles/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/time_management/cpu_clock_cycles/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/time_management/cpu_clock_cycles/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.664812 cengal-3.1.18.3/cengal/time_management/high_precision_sync_sleep/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/time_management/high_precision_sync_sleep/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.664812 cengal-3.1.18.3/cengal/time_management/high_precision_sync_sleep/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/time_management/high_precision_sync_sleep/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.664812 cengal-3.1.18.3/cengal/time_management/high_precision_sync_sleep/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1369 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/time_management/high_precision_sync_sleep/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.664812 cengal-3.1.18.3/cengal/time_management/high_precision_sync_sleep/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/time_management/high_precision_sync_sleep/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/time_management/high_precision_sync_sleep/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.664812 cengal-3.1.18.3/cengal/time_management/load_best_timer/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/time_management/load_best_timer/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.664812 cengal-3.1.18.3/cengal/time_management/load_best_timer/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/time_management/load_best_timer/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.664812 cengal-3.1.18.3/cengal/time_management/load_best_timer/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1238 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/time_management/load_best_timer/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1446 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/time_management/load_best_timer/versions/v_0/load_best_timer.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.664812 cengal-3.1.18.3/cengal/time_management/relative_time/
--rw-r--r--   0 mb        (1000) mb        (1000)     1366 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/time_management/relative_time/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.664812 cengal-3.1.18.3/cengal/time_management/relative_time/approximate_representation/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/time_management/relative_time/approximate_representation/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.664812 cengal-3.1.18.3/cengal/time_management/relative_time/approximate_representation/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/time_management/relative_time/approximate_representation/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.684812 cengal-3.1.18.3/cengal/time_management/relative_time/approximate_representation/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1249 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/time_management/relative_time/approximate_representation/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     8715 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/time_management/relative_time/approximate_representation/versions/v_0/approximate_representation.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.684812 cengal-3.1.18.3/cengal/time_management/relative_time/bysiness_relativedelta/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/time_management/relative_time/bysiness_relativedelta/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.684812 cengal-3.1.18.3/cengal/time_management/relative_time/bysiness_relativedelta/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/time_management/relative_time/bysiness_relativedelta/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.684812 cengal-3.1.18.3/cengal/time_management/relative_time/bysiness_relativedelta/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1245 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/time_management/relative_time/bysiness_relativedelta/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1490 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/time_management/relative_time/bysiness_relativedelta/versions/v_0/bysiness_relativedelta.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.684812 cengal-3.1.18.3/cengal/time_management/relative_time/constants/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/time_management/relative_time/constants/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.684812 cengal-3.1.18.3/cengal/time_management/relative_time/constants/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/time_management/relative_time/constants/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.684812 cengal-3.1.18.3/cengal/time_management/relative_time/constants/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1232 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/time_management/relative_time/constants/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1419 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/time_management/relative_time/constants/versions/v_0/constants.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.684812 cengal-3.1.18.3/cengal/time_management/relative_time/relativedelta/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/time_management/relative_time/relativedelta/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.684812 cengal-3.1.18.3/cengal/time_management/relative_time/relativedelta/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/time_management/relative_time/relativedelta/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.684812 cengal-3.1.18.3/cengal/time_management/relative_time/relativedelta/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1236 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/time_management/relative_time/relativedelta/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1860 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/time_management/relative_time/relativedelta/versions/v_0/relativedelta.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.684812 cengal-3.1.18.3/cengal/time_management/relative_time/timedelta/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/time_management/relative_time/timedelta/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.684812 cengal-3.1.18.3/cengal/time_management/relative_time/timedelta/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/time_management/relative_time/timedelta/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.684812 cengal-3.1.18.3/cengal/time_management/relative_time/timedelta/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1232 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/time_management/relative_time/timedelta/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1633 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/time_management/relative_time/timedelta/versions/v_0/timedelta.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.684812 cengal-3.1.18.3/cengal/time_management/repeat_for_a_time/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/time_management/repeat_for_a_time/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.684812 cengal-3.1.18.3/cengal/time_management/repeat_for_a_time/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/time_management/repeat_for_a_time/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.684812 cengal-3.1.18.3/cengal/time_management/repeat_for_a_time/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1457 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/time_management/repeat_for_a_time/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    13454 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/time_management/repeat_for_a_time/versions/v_0/repeat_for_a_time__python.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.684812 cengal-3.1.18.3/cengal/time_management/repeat_for_a_time/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/time_management/repeat_for_a_time/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/time_management/repeat_for_a_time/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)    16609 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/time_management/repeat_for_a_time/versions/v_0/tests/example_for__repeat_for_a_time.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.684812 cengal-3.1.18.3/cengal/time_management/sleep_tools/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/time_management/sleep_tools/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.684812 cengal-3.1.18.3/cengal/time_management/sleep_tools/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/time_management/sleep_tools/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.684812 cengal-3.1.18.3/cengal/time_management/sleep_tools/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1234 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/time_management/sleep_tools/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     4701 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/time_management/sleep_tools/versions/v_0/sleep_tools.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.684812 cengal-3.1.18.3/cengal/time_management/sleep_tools/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/time_management/sleep_tools/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/time_management/sleep_tools/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.684812 cengal-3.1.18.3/cengal/time_management/timer/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/time_management/timer/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.684812 cengal-3.1.18.3/cengal/time_management/timer/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/time_management/timer/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.684812 cengal-3.1.18.3/cengal/time_management/timer/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1228 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/time_management/timer/versions/v_0/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.684812 cengal-3.1.18.3/cengal/time_management/timer/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/time_management/timer/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/time_management/timer/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)     4568 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/time_management/timer/versions/v_0/timer.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.684812 cengal-3.1.18.3/cengal/time_management/timer/versions/v_1/
--rw-r--r--   0 mb        (1000) mb        (1000)     1228 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/time_management/timer/versions/v_1/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.684812 cengal-3.1.18.3/cengal/time_management/timer/versions/v_1/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/time_management/timer/versions/v_1/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/time_management/timer/versions/v_1/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)     6792 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/time_management/timer/versions/v_1/timer.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.684812 cengal-3.1.18.3/cengal/time_management/timer_precision/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/time_management/timer_precision/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.684812 cengal-3.1.18.3/cengal/time_management/timer_precision/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/time_management/timer_precision/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.684812 cengal-3.1.18.3/cengal/time_management/timer_precision/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1243 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/time_management/timer_precision/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1867 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/time_management/timer_precision/versions/v_0/test_timer_precision.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.694812 cengal-3.1.18.3/cengal/time_management/timer_precision/versions/v_1/
--rw-r--r--   0 mb        (1000) mb        (1000)     1238 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/time_management/timer_precision/versions/v_1/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     4328 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/time_management/timer_precision/versions/v_1/timer_precision.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.694812 cengal-3.1.18.3/cengal/unittest/
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/unittest/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.694812 cengal-3.1.18.3/cengal/unittest/behavior_stabilizer/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/unittest/behavior_stabilizer/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.704812 cengal-3.1.18.3/cengal/unittest/behavior_stabilizer/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/unittest/behavior_stabilizer/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.704812 cengal-3.1.18.3/cengal/unittest/behavior_stabilizer/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1242 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/unittest/behavior_stabilizer/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2033 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/unittest/behavior_stabilizer/versions/v_0/behavior_stabilizer.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.704812 cengal-3.1.18.3/cengal/unittest/behavior_stabilizer/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/unittest/behavior_stabilizer/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/unittest/behavior_stabilizer/versions/v_0/tests/_test__behavior_stabilizer.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.704812 cengal-3.1.18.3/cengal/unittest/patcher/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/unittest/patcher/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.704812 cengal-3.1.18.3/cengal/unittest/patcher/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/unittest/patcher/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.704812 cengal-3.1.18.3/cengal/unittest/patcher/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/unittest/patcher/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3085 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/unittest/patcher/versions/v_0/patcher.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.704812 cengal-3.1.18.3/cengal/unittest/patcher/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/unittest/patcher/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/unittest/patcher/versions/v_0/tests/_test__patcher.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.704812 cengal-3.1.18.3/cengal/universal_parser/
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/universal_parser/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1208 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/universal_parser/help_tools.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1378 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/universal_parser/idioms.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1229 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/universal_parser/parser.py
--rw-r--r--   0 mb        (1000) mb        (1000)     8668 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/universal_parser/test.py
--rw-r--r--   0 mb        (1000) mb        (1000)    75710 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/universal_parser/types.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.704812 cengal-3.1.18.3/cengal/upk_helping_tools/
--rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/upk_helping_tools/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2300 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/upk_helping_tools/upk_api.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1822 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/upk_helping_tools/upk_constants.py
--rw-r--r--   0 mb        (1000) mb        (1000)     6519 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/upk_helping_tools/upk_utils_api.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.704812 cengal-3.1.18.3/cengal/user_interface/
--rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/user_interface/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.704812 cengal-3.1.18.3/cengal/user_interface/console/
--rw-r--r--   0 mb        (1000) mb        (1000)     1325 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/user_interface/console/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3505 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/user_interface/console/chooser.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1550 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/user_interface/console/colorama_helpers.py
--rw-r--r--   0 mb        (1000) mb        (1000)    11361 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/user_interface/console/encoding_changer.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.704812 cengal-3.1.18.3/cengal/user_interface/console/progress_meter/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/user_interface/console/progress_meter/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.704812 cengal-3.1.18.3/cengal/user_interface/console/progress_meter/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/user_interface/console/progress_meter/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.704812 cengal-3.1.18.3/cengal/user_interface/console/progress_meter/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1365 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/user_interface/console/progress_meter/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     4876 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/user_interface/console/progress_meter/versions/v_0/progress_meter.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1275 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/user_interface/console/progress_meter/versions/v_0/progress_meter_python2.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.704812 cengal-3.1.18.3/cengal/user_interface/gui/
--rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/user_interface/gui/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.704812 cengal-3.1.18.3/cengal/user_interface/gui/nt/
--rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/user_interface/gui/nt/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.704812 cengal-3.1.18.3/cengal/user_interface/gui/nt/blur_behind/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/user_interface/gui/nt/blur_behind/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.704812 cengal-3.1.18.3/cengal/user_interface/gui/nt/blur_behind/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/user_interface/gui/nt/blur_behind/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.704812 cengal-3.1.18.3/cengal/user_interface/gui/nt/blur_behind/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1234 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/user_interface/gui/nt/blur_behind/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3162 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/user_interface/gui/nt/blur_behind/versions/v_0/blur_behind.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.724812 cengal-3.1.18.3/cengal/user_interface/gui/nt/blur_behind/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/user_interface/gui/nt/blur_behind/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/user_interface/gui/nt/blur_behind/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.724812 cengal-3.1.18.3/cengal/user_interface/gui/nt/dpi_awareness/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/user_interface/gui/nt/dpi_awareness/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.724812 cengal-3.1.18.3/cengal/user_interface/gui/nt/dpi_awareness/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/user_interface/gui/nt/dpi_awareness/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.724812 cengal-3.1.18.3/cengal/user_interface/gui/nt/dpi_awareness/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1236 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/user_interface/gui/nt/dpi_awareness/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     3687 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/user_interface/gui/nt/dpi_awareness/versions/v_0/dpi_awareness.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.724812 cengal-3.1.18.3/cengal/user_interface/gui/nt/dpi_awareness/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/user_interface/gui/nt/dpi_awareness/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/user_interface/gui/nt/dpi_awareness/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.724812 cengal-3.1.18.3/cengal/user_interface/plot/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/user_interface/plot/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.724812 cengal-3.1.18.3/cengal/user_interface/plot/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/user_interface/plot/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.724812 cengal-3.1.18.3/cengal/user_interface/plot/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1227 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/user_interface/plot/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1878 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/user_interface/plot/versions/v_0/plot.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.724812 cengal-3.1.18.3/cengal/user_interface/plot/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/user_interface/plot/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.3/cengal/user_interface/plot/versions/v_0/tests/_test__template_submodule.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.724812 cengal-3.1.18.3/cengal/web_tools/
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/web_tools/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.724812 cengal-3.1.18.3/cengal/web_tools/detect_browsers_host_device_type/
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/web_tools/detect_browsers_host_device_type/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.724812 cengal-3.1.18.3/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/
--rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.724812 cengal-3.1.18.3/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/
--rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/__init__.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.724812 cengal-3.1.18.3/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/v_0/
--rw-r--r--   0 mb        (1000) mb        (1000)     1241 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/v_0/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     4333 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/v_0/by_http_user_agent.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.724812 cengal-3.1.18.3/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/v_0/tests/
--rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/v_0/tests/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/v_0/tests/_test__template_submodule.py
--rw-r--r--   0 mb        (1000) mb        (1000)    12870 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal/web_tools/help_tools.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.084812 cengal-3.1.18.3/cengal.egg-info/
--rw-r--r--   0 mb        (1000) mb        (1000)    27217 2023-05-21 17:04:22.000000 cengal-3.1.18.3/cengal.egg-info/PKG-INFO
--rw-r--r--   0 mb        (1000) mb        (1000)    86285 2023-05-21 17:04:22.000000 cengal-3.1.18.3/cengal.egg-info/SOURCES.txt
--rw-r--r--   0 mb        (1000) mb        (1000)        1 2023-05-21 17:04:22.000000 cengal-3.1.18.3/cengal.egg-info/dependency_links.txt
--rw-r--r--   0 mb        (1000) mb        (1000)      211 2023-05-21 17:04:22.000000 cengal-3.1.18.3/cengal.egg-info/requires.txt
--rw-r--r--   0 mb        (1000) mb        (1000)       28 2023-05-21 17:04:22.000000 cengal-3.1.18.3/cengal.egg-info/top_level.txt
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.724812 cengal-3.1.18.3/cengal_setup_scripts/
--rw-r--r--   0 mb        (1000) mb        (1000)     1251 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal_setup_scripts/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     2429 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal_setup_scripts/compile_all_cython_modules.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.724812 cengal-3.1.18.3/cengal_setup_scripts/find_and_prepare_cython_modules/
--rw-r--r--   0 mb        (1000) mb        (1000)     1254 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal_setup_scripts/find_and_prepare_cython_modules/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)     8107 2023-05-21 17:03:53.000000 cengal-3.1.18.3/cengal_setup_scripts/find_and_prepare_cython_modules/find_and_prepare_cython_modules.py
-drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:04:23.724812 cengal-3.1.18.3/cengal_setup_scripts/install_required_packages/
--rw-r--r--   0 mb        (1000) mb        (1000)     1239 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal_setup_scripts/install_required_packages/__init__.py
--rw-r--r--   0 mb        (1000) mb        (1000)    10416 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal_setup_scripts/install_required_packages/install_packages.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1784 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal_setup_scripts/install_required_packages/set_environment_variables.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1501 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal_setup_scripts/setup__dynamic_list_of_pieces.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1498 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal_setup_scripts/setup__recv_buff_size_computer.py
--rw-r--r--   0 mb        (1000) mb        (1000)     1499 2023-05-19 10:11:50.000000 cengal-3.1.18.3/cengal_setup_scripts/setup__repeat_for_a_time.py
--rw-r--r--   0 mb        (1000) mb        (1000)      156 2023-04-22 17:37:18.000000 cengal-3.1.18.3/pyproject.toml
--rw-r--r--   0 mb        (1000) mb        (1000)       38 2023-05-21 17:04:23.724812 cengal-3.1.18.3/setup.cfg
--rw-r--r--   0 mb        (1000) mb        (1000)     8531 2023-05-21 17:04:16.000000 cengal-3.1.18.3/setup.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.704813 cengal-3.1.18.4/
+-rw-r--r--   0 mb        (1000) mb        (1000)    11358 2023-04-22 17:28:13.000000 cengal-3.1.18.4/LICENSE.md
+-rw-r--r--   0 mb        (1000) mb        (1000)      614 2023-04-22 17:37:18.000000 cengal-3.1.18.4/NOTICE
+-rw-r--r--   0 mb        (1000) mb        (1000)    27225 2023-05-21 17:17:46.704813 cengal-3.1.18.4/PKG-INFO
+-rw-r--r--   0 mb        (1000) mb        (1000)    22113 2023-05-21 17:15:01.000000 cengal-3.1.18.4/README.md
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.904813 cengal-3.1.18.4/cengal/
+-rw-r--r--   0 mb        (1000) mb        (1000)     8228 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/RequestCache.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2761 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/ServerClock.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.904813 cengal-3.1.18.4/cengal/_cengal_setup_scripts/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1251 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/_cengal_setup_scripts/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2429 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/_cengal_setup_scripts/compile_all_cython_modules.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.904813 cengal-3.1.18.4/cengal/_cengal_setup_scripts/find_and_prepare_cython_modules/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1254 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/_cengal_setup_scripts/find_and_prepare_cython_modules/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     8107 2023-05-21 17:03:53.000000 cengal-3.1.18.4/cengal/_cengal_setup_scripts/find_and_prepare_cython_modules/find_and_prepare_cython_modules.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.914813 cengal-3.1.18.4/cengal/_cengal_setup_scripts/install_required_packages/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1239 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/_cengal_setup_scripts/install_required_packages/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    10416 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/_cengal_setup_scripts/install_required_packages/install_packages.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1784 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/_cengal_setup_scripts/install_required_packages/set_environment_variables.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1501 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/_cengal_setup_scripts/setup__dynamic_list_of_pieces.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1498 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/_cengal_setup_scripts/setup__recv_buff_size_computer.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1499 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/_cengal_setup_scripts/setup__repeat_for_a_time.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.914813 cengal-3.1.18.4/cengal/base/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/base/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.914813 cengal-3.1.18.4/cengal/base/classes/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/base/classes/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.914813 cengal-3.1.18.4/cengal/base/classes/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/base/classes/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.914813 cengal-3.1.18.4/cengal/base/classes/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/base/classes/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1267 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/base/classes/versions/v_0/classes.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.914813 cengal-3.1.18.4/cengal/base/classes/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/base/classes/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/base/classes/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.914813 cengal-3.1.18.4/cengal/base/exceptions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/base/exceptions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.914813 cengal-3.1.18.4/cengal/base/exceptions/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/base/exceptions/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.914813 cengal-3.1.18.4/cengal/base/exceptions/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1233 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/base/exceptions/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1303 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/base/exceptions/versions/v_0/exceptions.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.914813 cengal-3.1.18.4/cengal/base/exceptions/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/base/exceptions/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/base/exceptions/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.914813 cengal-3.1.18.4/cengal/build_tools/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1210 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/build_tools/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.914813 cengal-3.1.18.4/cengal/build_tools/current_compiler/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/build_tools/current_compiler/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.914813 cengal-3.1.18.4/cengal/build_tools/current_compiler/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/build_tools/current_compiler/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.914813 cengal-3.1.18.4/cengal/build_tools/current_compiler/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1239 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/build_tools/current_compiler/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2162 2023-05-21 17:03:53.000000 cengal-3.1.18.4/cengal/build_tools/current_compiler/versions/v_0/current_compiler.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.914813 cengal-3.1.18.4/cengal/build_tools/current_compiler/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/build_tools/current_compiler/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/build_tools/current_compiler/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.914813 cengal-3.1.18.4/cengal/build_tools/prepare_cflags/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/build_tools/prepare_cflags/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.924813 cengal-3.1.18.4/cengal/build_tools/prepare_cflags/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/build_tools/prepare_cflags/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.924813 cengal-3.1.18.4/cengal/build_tools/prepare_cflags/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1237 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/build_tools/prepare_cflags/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    14704 2023-05-21 17:03:53.000000 cengal-3.1.18.4/cengal/build_tools/prepare_cflags/versions/v_0/prepare_cflags.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.924813 cengal-3.1.18.4/cengal/build_tools/prepare_cflags/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/build_tools/prepare_cflags/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/build_tools/prepare_cflags/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.924813 cengal-3.1.18.4/cengal/bulk_pip_actions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/bulk_pip_actions/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     6287 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/bulk_pip_actions/bulk_install.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     6023 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/bulk_pip_actions/install.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1280 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/check_is_in_pycharm.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.924813 cengal-3.1.18.4/cengal/code_flow_control/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/code_flow_control/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.924813 cengal-3.1.18.4/cengal/code_flow_control/args_manager/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/code_flow_control/args_manager/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.924813 cengal-3.1.18.4/cengal/code_flow_control/args_manager/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/code_flow_control/args_manager/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.924813 cengal-3.1.18.4/cengal/code_flow_control/args_manager/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1235 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/code_flow_control/args_manager/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    16577 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/code_flow_control/args_manager/versions/v_0/args_manager.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.934813 cengal-3.1.18.4/cengal/code_flow_control/args_manager/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/code_flow_control/args_manager/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    17267 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/code_flow_control/args_manager/versions/v_0/tests/_manual_test__args_manager.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/code_flow_control/args_manager/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.934813 cengal-3.1.18.4/cengal/code_flow_control/call_history_reapplier/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/code_flow_control/call_history_reapplier/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.934813 cengal-3.1.18.4/cengal/code_flow_control/call_history_reapplier/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/code_flow_control/call_history_reapplier/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.934813 cengal-3.1.18.4/cengal/code_flow_control/call_history_reapplier/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1245 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/code_flow_control/call_history_reapplier/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2770 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/code_flow_control/call_history_reapplier/versions/v_0/call_history_reapplier.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.934813 cengal-3.1.18.4/cengal/code_flow_control/call_history_reapplier/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/code_flow_control/call_history_reapplier/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/code_flow_control/call_history_reapplier/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.934813 cengal-3.1.18.4/cengal/code_flow_control/chained_flow/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/code_flow_control/chained_flow/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.934813 cengal-3.1.18.4/cengal/code_flow_control/chained_flow/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/code_flow_control/chained_flow/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.934813 cengal-3.1.18.4/cengal/code_flow_control/chained_flow/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1234 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/code_flow_control/chained_flow/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    36471 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/code_flow_control/chained_flow/versions/v_0/smart_chain.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.934813 cengal-3.1.18.4/cengal/code_flow_control/chained_flow/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/code_flow_control/chained_flow/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/code_flow_control/chained_flow/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    32962 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/code_flow_control/chained_flow/versions/v_0/tests/example_for__chained_flow.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.934813 cengal-3.1.18.4/cengal/code_flow_control/chained_flow/versions/v_1/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1235 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/code_flow_control/chained_flow/versions/v_1/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    35218 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/code_flow_control/chained_flow/versions/v_1/chained_flow.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.934813 cengal-3.1.18.4/cengal/code_flow_control/chained_flow/versions/v_1/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/code_flow_control/chained_flow/versions/v_1/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/code_flow_control/chained_flow/versions/v_1/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    32962 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/code_flow_control/chained_flow/versions/v_1/tests/example_for__chained_flow.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.934813 cengal-3.1.18.4/cengal/code_flow_control/multiinterface_essence/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/code_flow_control/multiinterface_essence/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.934813 cengal-3.1.18.4/cengal/code_flow_control/multiinterface_essence/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/code_flow_control/multiinterface_essence/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.934813 cengal-3.1.18.4/cengal/code_flow_control/multiinterface_essence/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/code_flow_control/multiinterface_essence/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    23328 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/code_flow_control/multiinterface_essence/versions/v_0/essence.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.954813 cengal-3.1.18.4/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2882 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2624 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/quadrangle.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1373 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/quadrangle_test.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3467 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/square_and_rectangle.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     4071 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/square_and_rectangle_test.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     4392 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/square_and_rectangle_test_old.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.954813 cengal-3.1.18.4/cengal/code_flow_control/none_or/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/code_flow_control/none_or/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.954813 cengal-3.1.18.4/cengal/code_flow_control/none_or/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/code_flow_control/none_or/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.954813 cengal-3.1.18.4/cengal/code_flow_control/none_or/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/code_flow_control/none_or/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1487 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/code_flow_control/none_or/versions/v_0/none_or.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.954813 cengal-3.1.18.4/cengal/code_flow_control/none_or/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/code_flow_control/none_or/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/code_flow_control/none_or/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.954813 cengal-3.1.18.4/cengal/code_flow_control/python_bytecode_manipulator/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/code_flow_control/python_bytecode_manipulator/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.954813 cengal-3.1.18.4/cengal/code_flow_control/python_bytecode_manipulator/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/code_flow_control/python_bytecode_manipulator/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.954813 cengal-3.1.18.4/cengal/code_flow_control/python_bytecode_manipulator/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1250 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/code_flow_control/python_bytecode_manipulator/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    29755 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/code_flow_control/python_bytecode_manipulator/versions/v_0/python_bytecode_manipulator.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.954813 cengal-3.1.18.4/cengal/code_flow_control/python_bytecode_manipulator/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/code_flow_control/python_bytecode_manipulator/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/code_flow_control/python_bytecode_manipulator/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.954813 cengal-3.1.18.4/cengal/code_flow_control/smart_values/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/code_flow_control/smart_values/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.954813 cengal-3.1.18.4/cengal/code_flow_control/smart_values/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/code_flow_control/smart_values/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.954813 cengal-3.1.18.4/cengal/code_flow_control/smart_values/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1235 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/code_flow_control/smart_values/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2828 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/code_flow_control/smart_values/versions/v_0/result_types.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.964813 cengal-3.1.18.4/cengal/code_flow_control/smart_values/versions/v_1/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1235 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/code_flow_control/smart_values/versions/v_1/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2839 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/code_flow_control/smart_values/versions/v_1/smart_values.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.964813 cengal-3.1.18.4/cengal/code_flow_control/smart_values/versions/v_2/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1235 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/code_flow_control/smart_values/versions/v_2/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3470 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/code_flow_control/smart_values/versions/v_2/smart_values.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.964813 cengal-3.1.18.4/cengal/code_inspection/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/code_inspection/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.964813 cengal-3.1.18.4/cengal/code_inspection/auto_line_tracer/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/code_inspection/auto_line_tracer/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.964813 cengal-3.1.18.4/cengal/code_inspection/auto_line_tracer/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/code_inspection/auto_line_tracer/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.964813 cengal-3.1.18.4/cengal/code_inspection/auto_line_tracer/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1239 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/code_inspection/auto_line_tracer/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     6171 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/code_inspection/auto_line_tracer/versions/v_0/auto_line_tracer.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.964813 cengal-3.1.18.4/cengal/code_inspection/auto_line_tracer/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/code_inspection/auto_line_tracer/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/code_inspection/auto_line_tracer/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.964813 cengal-3.1.18.4/cengal/code_inspection/line_profiling/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/code_inspection/line_profiling/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.964813 cengal-3.1.18.4/cengal/code_inspection/line_profiling/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/code_inspection/line_profiling/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.964813 cengal-3.1.18.4/cengal/code_inspection/line_profiling/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1237 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/code_inspection/line_profiling/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2770 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/code_inspection/line_profiling/versions/v_0/line_profiling.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.964813 cengal-3.1.18.4/cengal/code_inspection/line_profiling/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/code_inspection/line_profiling/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/code_inspection/line_profiling/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.964813 cengal-3.1.18.4/cengal/code_inspection/line_tracer/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/code_inspection/line_tracer/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.964813 cengal-3.1.18.4/cengal/code_inspection/line_tracer/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/code_inspection/line_tracer/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.964813 cengal-3.1.18.4/cengal/code_inspection/line_tracer/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1234 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/code_inspection/line_tracer/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     4305 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/code_inspection/line_tracer/versions/v_0/line_tracer.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.964813 cengal-3.1.18.4/cengal/code_inspection/line_tracer/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/code_inspection/line_tracer/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/code_inspection/line_tracer/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.984813 cengal-3.1.18.4/cengal/cross_version/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/cross_version/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.984813 cengal-3.1.18.4/cengal/cross_version/console_print/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1243 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/cross_version/console_print/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1264 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/cross_version/console_print/python3.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1529 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/cross_version/console_print/universal.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.984813 cengal-3.1.18.4/cengal/ctypes_tools/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1210 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/ctypes_tools/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.984813 cengal-3.1.18.4/cengal/ctypes_tools/constants/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/ctypes_tools/constants/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.984813 cengal-3.1.18.4/cengal/ctypes_tools/constants/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/ctypes_tools/constants/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.984813 cengal-3.1.18.4/cengal/ctypes_tools/constants/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1270 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/ctypes_tools/constants/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.984813 cengal-3.1.18.4/cengal/ctypes_tools/constants/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/ctypes_tools/constants/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/ctypes_tools/constants/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    13438 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/ctypes_tools/constants/versions/v_0/win_constants.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.984813 cengal-3.1.18.4/cengal/ctypes_tools/function_prototypes/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/ctypes_tools/function_prototypes/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.984813 cengal-3.1.18.4/cengal/ctypes_tools/function_prototypes/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/ctypes_tools/function_prototypes/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.984813 cengal-3.1.18.4/cengal/ctypes_tools/function_prototypes/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1280 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/ctypes_tools/function_prototypes/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.984813 cengal-3.1.18.4/cengal/ctypes_tools/function_prototypes/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/ctypes_tools/function_prototypes/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/ctypes_tools/function_prototypes/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     5488 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/ctypes_tools/function_prototypes/versions/v_0/win_function_prototypes.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.984813 cengal-3.1.18.4/cengal/ctypes_tools/functions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/ctypes_tools/functions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.984813 cengal-3.1.18.4/cengal/ctypes_tools/functions/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/ctypes_tools/functions/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.984813 cengal-3.1.18.4/cengal/ctypes_tools/functions/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1296 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/ctypes_tools/functions/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1317 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/ctypes_tools/functions/versions/v_0/functions.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.994813 cengal-3.1.18.4/cengal/ctypes_tools/functions/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/ctypes_tools/functions/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/ctypes_tools/functions/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1502 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/ctypes_tools/functions/versions/v_0/win_functions.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.994813 cengal-3.1.18.4/cengal/ctypes_tools/libraries/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/ctypes_tools/libraries/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.994813 cengal-3.1.18.4/cengal/ctypes_tools/libraries/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/ctypes_tools/libraries/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.994813 cengal-3.1.18.4/cengal/ctypes_tools/libraries/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1270 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/ctypes_tools/libraries/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.994813 cengal-3.1.18.4/cengal/ctypes_tools/libraries/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/ctypes_tools/libraries/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/ctypes_tools/libraries/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1482 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/ctypes_tools/libraries/versions/v_0/win_libraries.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.994813 cengal-3.1.18.4/cengal/ctypes_tools/result_api/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/ctypes_tools/result_api/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.994813 cengal-3.1.18.4/cengal/ctypes_tools/result_api/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/ctypes_tools/result_api/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.994813 cengal-3.1.18.4/cengal/ctypes_tools/result_api/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1336 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/ctypes_tools/result_api/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1222 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/ctypes_tools/result_api/versions/v_0/result_api.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1305 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/ctypes_tools/result_api/versions/v_0/result_api_exceptions.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.994813 cengal-3.1.18.4/cengal/ctypes_tools/result_api/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/ctypes_tools/result_api/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/ctypes_tools/result_api/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2729 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/ctypes_tools/result_api/versions/v_0/win_result_api.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.994813 cengal-3.1.18.4/cengal/ctypes_tools/tools/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/ctypes_tools/tools/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.994813 cengal-3.1.18.4/cengal/ctypes_tools/tools/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/ctypes_tools/tools/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.994813 cengal-3.1.18.4/cengal/ctypes_tools/tools/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1288 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/ctypes_tools/tools/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.014813 cengal-3.1.18.4/cengal/ctypes_tools/tools/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/ctypes_tools/tools/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/ctypes_tools/tools/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1597 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/ctypes_tools/tools/versions/v_0/tools.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1601 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/ctypes_tools/tools/versions/v_0/win_tools.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.014813 cengal-3.1.18.4/cengal/ctypes_tools/types/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/ctypes_tools/types/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.014813 cengal-3.1.18.4/cengal/ctypes_tools/types/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/ctypes_tools/types/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.014813 cengal-3.1.18.4/cengal/ctypes_tools/types/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1266 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/ctypes_tools/types/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.014813 cengal-3.1.18.4/cengal/ctypes_tools/types/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/ctypes_tools/types/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/ctypes_tools/types/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     7773 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/ctypes_tools/types/versions/v_0/win_types.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.014813 cengal-3.1.18.4/cengal/cython_tools/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/cython_tools/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1774 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/cython_tools/cythonyser_setup_runner.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.014813 cengal-3.1.18.4/cengal/data_containers/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.014813 cengal-3.1.18.4/cengal/data_containers/compound_dict_management/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/compound_dict_management/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.014813 cengal-3.1.18.4/cengal/data_containers/compound_dict_management/manager/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/compound_dict_management/manager/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.014813 cengal-3.1.18.4/cengal/data_containers/compound_dict_management/manager/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/compound_dict_management/manager/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.014813 cengal-3.1.18.4/cengal/data_containers/compound_dict_management/manager/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/compound_dict_management/manager/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2229 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/compound_dict_management/manager/versions/v_0/manager.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.034813 cengal-3.1.18.4/cengal/data_containers/compound_dict_management/manager/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/compound_dict_management/manager/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/compound_dict_management/manager/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.034813 cengal-3.1.18.4/cengal/data_containers/compound_dict_management/manager/versions/v_1/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/compound_dict_management/manager/versions/v_1/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2212 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/compound_dict_management/manager/versions/v_1/manager.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.034813 cengal-3.1.18.4/cengal/data_containers/compound_dict_management/manager/versions/v_1/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/compound_dict_management/manager/versions/v_1/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/compound_dict_management/manager/versions/v_1/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.034813 cengal-3.1.18.4/cengal/data_containers/compound_dict_management/standard_library/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1279 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/compound_dict_management/standard_library/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.034813 cengal-3.1.18.4/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.034813 cengal-3.1.18.4/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.034813 cengal-3.1.18.4/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1252 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1542 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/versions/v_0/key__hashable__to__value__set.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.034813 cengal-3.1.18.4/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.034813 cengal-3.1.18.4/cengal/data_containers/compound_dict_management/standard_library/key_counter/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/compound_dict_management/standard_library/key_counter/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.034813 cengal-3.1.18.4/cengal/data_containers/compound_dict_management/standard_library/key_counter/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/compound_dict_management/standard_library/key_counter/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.034813 cengal-3.1.18.4/cengal/data_containers/compound_dict_management/standard_library/key_counter/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1234 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/compound_dict_management/standard_library/key_counter/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1598 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/compound_dict_management/standard_library/key_counter/versions/v_0/key_counter.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.034813 cengal-3.1.18.4/cengal/data_containers/compound_dict_management/standard_library/key_counter/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/compound_dict_management/standard_library/key_counter/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/compound_dict_management/standard_library/key_counter/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.034813 cengal-3.1.18.4/cengal/data_containers/dynamic_list_of_pieces/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/dynamic_list_of_pieces/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.034813 cengal-3.1.18.4/cengal/data_containers/dynamic_list_of_pieces/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/dynamic_list_of_pieces/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.034813 cengal-3.1.18.4/cengal/data_containers/dynamic_list_of_pieces/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1625 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/dynamic_list_of_pieces/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    28854 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/dynamic_list_of_pieces/versions/v_0/dynamic_list_of_pieces__python.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.034813 cengal-3.1.18.4/cengal/data_containers/dynamic_list_of_pieces/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/dynamic_list_of_pieces/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/dynamic_list_of_pieces/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.034813 cengal-3.1.18.4/cengal/data_containers/dynamic_list_of_pieces/versions/v_1/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1625 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/dynamic_list_of_pieces/versions/v_1/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    28797 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/dynamic_list_of_pieces/versions/v_1/dynamic_list_of_pieces__python.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.034813 cengal-3.1.18.4/cengal/data_containers/dynamic_list_of_pieces/versions/v_1/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/dynamic_list_of_pieces/versions/v_1/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/dynamic_list_of_pieces/versions/v_1/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.034813 cengal-3.1.18.4/cengal/data_containers/dynamic_tag_tree/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/dynamic_tag_tree/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.034813 cengal-3.1.18.4/cengal/data_containers/dynamic_tag_tree/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/dynamic_tag_tree/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.034813 cengal-3.1.18.4/cengal/data_containers/dynamic_tag_tree/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)    39956 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/dynamic_tag_tree/versions/v_0/TagDB.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1260 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/dynamic_tag_tree/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     5405 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/dynamic_tag_tree/versions/v_0/tag_db_interface.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.034813 cengal-3.1.18.4/cengal/data_containers/dynamic_tag_tree/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/dynamic_tag_tree/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/dynamic_tag_tree/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.034813 cengal-3.1.18.4/cengal/data_containers/dynamic_tag_tree/versions/v_1/
+-rw-r--r--   0 mb        (1000) mb        (1000)    41895 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/dynamic_tag_tree/versions/v_1/TagDB.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1260 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/dynamic_tag_tree/versions/v_1/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    13150 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/dynamic_tag_tree/versions/v_1/tag_db_interface.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.034813 cengal-3.1.18.4/cengal/data_containers/dynamic_tag_tree/versions/v_1/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/dynamic_tag_tree/versions/v_1/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/dynamic_tag_tree/versions/v_1/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.044813 cengal-3.1.18.4/cengal/data_containers/dynamic_tag_tree/versions/v_2/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1260 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/dynamic_tag_tree/versions/v_2/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     9730 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/dynamic_tag_tree/versions/v_2/dynamic_tag_tree.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.044813 cengal-3.1.18.4/cengal/data_containers/dynamic_tag_tree/versions/v_2/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/dynamic_tag_tree/versions/v_2/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/dynamic_tag_tree/versions/v_2/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.044813 cengal-3.1.18.4/cengal/data_containers/fast_fifo/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/fast_fifo/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.044813 cengal-3.1.18.4/cengal/data_containers/fast_fifo/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/fast_fifo/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.044813 cengal-3.1.18.4/cengal/data_containers/fast_fifo/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1232 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/fast_fifo/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    12328 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/fast_fifo/versions/v_0/fast_fifo.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.044813 cengal-3.1.18.4/cengal/data_containers/fast_fifo/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/fast_fifo/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/fast_fifo/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.044813 cengal-3.1.18.4/cengal/data_containers/fast_fifo/versions/v_1/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1232 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/fast_fifo/versions/v_1/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    12276 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/fast_fifo/versions/v_1/fast_fifo.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.054813 cengal-3.1.18.4/cengal/data_containers/fast_fifo/versions/v_1/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/fast_fifo/versions/v_1/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/fast_fifo/versions/v_1/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.054813 cengal-3.1.18.4/cengal/data_containers/limitable_dict_with_order/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/limitable_dict_with_order/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.054813 cengal-3.1.18.4/cengal/data_containers/limitable_dict_with_order/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/limitable_dict_with_order/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.054813 cengal-3.1.18.4/cengal/data_containers/limitable_dict_with_order/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/limitable_dict_with_order/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2034 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/limitable_dict_with_order/versions/v_0/limitable_dict_with_order.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.054813 cengal-3.1.18.4/cengal/data_containers/limitable_dict_with_order/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/limitable_dict_with_order/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/limitable_dict_with_order/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.054813 cengal-3.1.18.4/cengal/data_containers/limitable_dict_with_order/versions/v_1/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/limitable_dict_with_order/versions/v_1/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2465 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/limitable_dict_with_order/versions/v_1/limitable_dict_with_order.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.054813 cengal-3.1.18.4/cengal/data_containers/limitable_dict_with_order/versions/v_1/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/limitable_dict_with_order/versions/v_1/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/limitable_dict_with_order/versions/v_1/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.054813 cengal-3.1.18.4/cengal/data_containers/simple_tree/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/simple_tree/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.054813 cengal-3.1.18.4/cengal/data_containers/simple_tree/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/simple_tree/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.054813 cengal-3.1.18.4/cengal/data_containers/simple_tree/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1234 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/simple_tree/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     5001 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/simple_tree/versions/v_0/simple_tree.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.054813 cengal-3.1.18.4/cengal/data_containers/stack/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/stack/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.054813 cengal-3.1.18.4/cengal/data_containers/stack/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/stack/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.054813 cengal-3.1.18.4/cengal/data_containers/stack/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1228 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/stack/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     4660 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/stack/versions/v_0/stack.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.054813 cengal-3.1.18.4/cengal/data_containers/stack/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1234 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/stack/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3696 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_containers/stack/versions/v_0/tests/test__stack.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.054813 cengal-3.1.18.4/cengal/data_generation/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_generation/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.054813 cengal-3.1.18.4/cengal/data_generation/id_generator/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_generation/id_generator/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.054813 cengal-3.1.18.4/cengal/data_generation/id_generator/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_generation/id_generator/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.054813 cengal-3.1.18.4/cengal/data_generation/id_generator/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1235 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_generation/id_generator/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2218 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_generation/id_generator/versions/v_0/id_generator.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.054813 cengal-3.1.18.4/cengal/data_generation/id_generator/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_generation/id_generator/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_generation/id_generator/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.054813 cengal-3.1.18.4/cengal/data_generation/id_generator/versions/v_1/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1235 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_generation/id_generator/versions/v_1/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3045 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_generation/id_generator/versions/v_1/id_generator.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.074813 cengal-3.1.18.4/cengal/data_generation/id_generator/versions/v_1/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_generation/id_generator/versions/v_1/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_generation/id_generator/versions/v_1/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.074813 cengal-3.1.18.4/cengal/data_manipulation/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.074813 cengal-3.1.18.4/cengal/data_manipulation/conversion/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1210 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/conversion/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.074813 cengal-3.1.18.4/cengal/data_manipulation/conversion/bit_cast_like/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/conversion/bit_cast_like/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.074813 cengal-3.1.18.4/cengal/data_manipulation/conversion/bit_cast_like/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/conversion/bit_cast_like/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.074813 cengal-3.1.18.4/cengal/data_manipulation/conversion/bit_cast_like/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1236 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/conversion/bit_cast_like/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2012 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/conversion/bit_cast_like/versions/v_0/bit_cast_like.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.074813 cengal-3.1.18.4/cengal/data_manipulation/conversion/bit_cast_like/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/conversion/bit_cast_like/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/conversion/bit_cast_like/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.074813 cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.074813 cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.074813 cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1239 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2476 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast/versions/v_0/reinterpret_cast.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.074813 cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.074813 cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast_management/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1210 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast_management/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.074813 cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.074813 cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.074813 cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     8111 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/versions/v_0/manager.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.074813 cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.074813 cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1210 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.074813 cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.074813 cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.074813 cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1235 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2549 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/versions/v_0/copy_wrapper.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.074813 cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.074813 cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.074813 cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.074813 cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1240 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2565 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/versions/v_0/deep_copy_wrapper.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.074813 cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.074813 cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.074813 cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.074813 cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1239 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.074813 cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3539 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/versions/v_0/uni_copy_wrapper.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.074813 cengal-3.1.18.4/cengal/data_manipulation/front_triggerable_variable/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/front_triggerable_variable/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.084813 cengal-3.1.18.4/cengal/data_manipulation/front_triggerable_variable/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/front_triggerable_variable/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.094813 cengal-3.1.18.4/cengal/data_manipulation/front_triggerable_variable/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1249 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/front_triggerable_variable/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3917 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/front_triggerable_variable/versions/v_0/front_triggerable_variable.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.094813 cengal-3.1.18.4/cengal/data_manipulation/front_triggerable_variable/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/front_triggerable_variable/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/front_triggerable_variable/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.094813 cengal-3.1.18.4/cengal/data_manipulation/get_dict_key_with_callable_default/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/get_dict_key_with_callable_default/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.094813 cengal-3.1.18.4/cengal/data_manipulation/get_dict_key_with_callable_default/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/get_dict_key_with_callable_default/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.094813 cengal-3.1.18.4/cengal/data_manipulation/get_dict_key_with_callable_default/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1257 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/get_dict_key_with_callable_default/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1484 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/get_dict_key_with_callable_default/versions/v_0/get_dict_key_with_callable_default.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.094813 cengal-3.1.18.4/cengal/data_manipulation/get_dict_key_with_callable_default/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/get_dict_key_with_callable_default/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/get_dict_key_with_callable_default/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     7545 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/help_tools.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.094813 cengal-3.1.18.4/cengal/data_manipulation/objects_counter/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/objects_counter/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.094813 cengal-3.1.18.4/cengal/data_manipulation/objects_counter/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/objects_counter/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.094813 cengal-3.1.18.4/cengal/data_manipulation/objects_counter/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1238 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/objects_counter/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2981 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/objects_counter/versions/v_0/objects_counter.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.094813 cengal-3.1.18.4/cengal/data_manipulation/objects_counter/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1244 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/objects_counter/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     6512 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/objects_counter/versions/v_0/tests/test__objects_counter.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.094813 cengal-3.1.18.4/cengal/data_manipulation/performant_list_operations/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/performant_list_operations/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.094813 cengal-3.1.18.4/cengal/data_manipulation/performant_list_operations/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/performant_list_operations/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.094813 cengal-3.1.18.4/cengal/data_manipulation/performant_list_operations/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1245 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/performant_list_operations/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     9311 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/performant_list_operations/versions/v_0/remove_items_from_list.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.094813 cengal-3.1.18.4/cengal/data_manipulation/performant_list_operations/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/performant_list_operations/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/performant_list_operations/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.094813 cengal-3.1.18.4/cengal/data_manipulation/serialization/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/serialization/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.094813 cengal-3.1.18.4/cengal/data_manipulation/serialization/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/serialization/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.094813 cengal-3.1.18.4/cengal/data_manipulation/serialization/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1236 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/serialization/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    27321 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/serialization/versions/v_0/serialization.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.094813 cengal-3.1.18.4/cengal/data_manipulation/serialization/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1242 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/serialization/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     4071 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/serialization/versions/v_0/tests/test__serialization.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.094813 cengal-3.1.18.4/cengal/data_manipulation/tree_traversal/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/tree_traversal/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.094813 cengal-3.1.18.4/cengal/data_manipulation/tree_traversal/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/tree_traversal/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.094813 cengal-3.1.18.4/cengal/data_manipulation/tree_traversal/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1237 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/tree_traversal/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.094813 cengal-3.1.18.4/cengal/data_manipulation/tree_traversal/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/tree_traversal/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/tree_traversal/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2652 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/tree_traversal/versions/v_0/tests/traverstal_manual_tests.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     8192 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/tree_traversal/versions/v_0/tree_traversal.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.094813 cengal-3.1.18.4/cengal/data_manipulation/tree_traversal/versions/v_1/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1237 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/tree_traversal/versions/v_1/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.094813 cengal-3.1.18.4/cengal/data_manipulation/tree_traversal/versions/v_1/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/tree_traversal/versions/v_1/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/tree_traversal/versions/v_1/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2615 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/tree_traversal/versions/v_1/tests/key_multi_value_traverstal_manual_tests.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2814 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/tree_traversal/versions/v_1/tests/key_value_traverstal_manual_tests.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2747 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/tree_traversal/versions/v_1/tests/traverstal_manual_tests.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    24128 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/data_manipulation/tree_traversal/versions/v_1/tree_traversal.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     5496 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/docten.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.114813 cengal-3.1.18.4/cengal/entities/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/entities/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.114813 cengal-3.1.18.4/cengal/entities/bindable_to_type/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/entities/bindable_to_type/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.114813 cengal-3.1.18.4/cengal/entities/bindable_to_type/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/entities/bindable_to_type/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.114813 cengal-3.1.18.4/cengal/entities/bindable_to_type/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1239 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/entities/bindable_to_type/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     4360 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/entities/bindable_to_type/versions/v_0/bindable_to_type.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.114813 cengal-3.1.18.4/cengal/entities/bindable_to_type/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/entities/bindable_to_type/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/entities/bindable_to_type/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.114813 cengal-3.1.18.4/cengal/entities/copyable/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/entities/copyable/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.114813 cengal-3.1.18.4/cengal/entities/copyable/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/entities/copyable/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.114813 cengal-3.1.18.4/cengal/entities/copyable/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/entities/copyable/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     4450 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/entities/copyable/versions/v_0/copyable.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.114813 cengal-3.1.18.4/cengal/entities/copyable/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/entities/copyable/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/entities/copyable/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.114813 cengal-3.1.18.4/cengal/file_settings_manager/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/file_settings_manager/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     7336 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/file_settings_manager/config_manager.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2248 2023-05-21 17:03:53.000000 cengal-3.1.18.4/cengal/file_settings_manager/dir_templates.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.114813 cengal-3.1.18.4/cengal/file_system/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/file_system/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.114813 cengal-3.1.18.4/cengal/file_system/app_fs_structure/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/file_system/app_fs_structure/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.114813 cengal-3.1.18.4/cengal/file_system/app_fs_structure/app_dir_path/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/file_system/app_fs_structure/app_dir_path/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.114813 cengal-3.1.18.4/cengal/file_system/app_fs_structure/app_dir_path/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/file_system/app_fs_structure/app_dir_path/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.114813 cengal-3.1.18.4/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1548 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1289 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/app_dir_exceptions.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     4302 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/app_dir_path_base.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     8624 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/app_dir_path_darwin.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     8513 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/app_dir_path_linux.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     7083 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/app_dir_path_win.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3825 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/app_directory_types.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.114813 cengal-3.1.18.4/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     8151 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/file_system/directory_manager.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2529 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/file_system/file_manager.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.114813 cengal-3.1.18.4/cengal/file_system/file_patch/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/file_system/file_patch/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.114813 cengal-3.1.18.4/cengal/file_system/file_patch/brackets/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/file_system/file_patch/brackets/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.114813 cengal-3.1.18.4/cengal/file_system/file_patch/brackets/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/file_system/file_patch/brackets/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.114813 cengal-3.1.18.4/cengal/file_system/file_patch/brackets/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/file_system/file_patch/brackets/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2366 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/file_system/file_patch/brackets/versions/v_0/brackets.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.114813 cengal-3.1.18.4/cengal/file_system/file_patch/brackets/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/file_system/file_patch/brackets/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/file_system/file_patch/brackets/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.114813 cengal-3.1.18.4/cengal/file_system/file_patch/generic/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/file_system/file_patch/generic/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.114813 cengal-3.1.18.4/cengal/file_system/file_patch/generic/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/file_system/file_patch/generic/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.114813 cengal-3.1.18.4/cengal/file_system/file_patch/generic/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/file_system/file_patch/generic/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2228 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/file_system/file_patch/generic/versions/v_0/generic.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.134813 cengal-3.1.18.4/cengal/file_system/file_patch/generic/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/file_system/file_patch/generic/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/file_system/file_patch/generic/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.134813 cengal-3.1.18.4/cengal/file_system/file_patch/simple/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/file_system/file_patch/simple/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.134813 cengal-3.1.18.4/cengal/file_system/file_patch/simple/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/file_system/file_patch/simple/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.134813 cengal-3.1.18.4/cengal/file_system/file_patch/simple/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1229 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/file_system/file_patch/simple/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2311 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/file_system/file_patch/simple/versions/v_0/simple.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.134813 cengal-3.1.18.4/cengal/file_system/file_patch/simple/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/file_system/file_patch/simple/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/file_system/file_patch/simple/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.134813 cengal-3.1.18.4/cengal/file_system/path_manager/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/file_system/path_manager/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.134813 cengal-3.1.18.4/cengal/file_system/path_manager/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/file_system/path_manager/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.134813 cengal-3.1.18.4/cengal/file_system/path_manager/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1235 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/file_system/path_manager/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2581 2023-05-21 17:03:53.000000 cengal-3.1.18.4/cengal/file_system/path_manager/versions/v_0/path_manager.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.134813 cengal-3.1.18.4/cengal/file_system/path_manager/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/file_system/path_manager/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/file_system/path_manager/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.134813 cengal-3.1.18.4/cengal/file_system/win_fs/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/file_system/win_fs/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3114 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/file_system/win_fs/base.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1851 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/file_system/win_fs/global_install_uninstall.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1997 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/file_system/win_fs/path.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     5190 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/file_system/win_fs/shutil.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     4437 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/file_system/win_fs/shutil_readable.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.134813 cengal-3.1.18.4/cengal/hardware/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1210 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/hardware/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.134813 cengal-3.1.18.4/cengal/hardware/info/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1210 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/hardware/info/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.134813 cengal-3.1.18.4/cengal/hardware/info/cpu/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/hardware/info/cpu/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.144813 cengal-3.1.18.4/cengal/hardware/info/cpu/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/hardware/info/cpu/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.144813 cengal-3.1.18.4/cengal/hardware/info/cpu/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/hardware/info/cpu/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2282 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/hardware/info/cpu/versions/v_0/cpu.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.144813 cengal-3.1.18.4/cengal/hardware/info/cpu/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/hardware/info/cpu/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/hardware/info/cpu/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.144813 cengal-3.1.18.4/cengal/hardware/info/cpu/versions/v_1/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/hardware/info/cpu/versions/v_1/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     8748 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/hardware/info/cpu/versions/v_1/cpu.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.144813 cengal-3.1.18.4/cengal/hardware/info/cpu/versions/v_1/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/hardware/info/cpu/versions/v_1/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/hardware/info/cpu/versions/v_1/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.144813 cengal-3.1.18.4/cengal/hardware/memory/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1210 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/hardware/memory/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.144813 cengal-3.1.18.4/cengal/hardware/memory/barriers/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/hardware/memory/barriers/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.144813 cengal-3.1.18.4/cengal/hardware/memory/barriers/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/hardware/memory/barriers/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.144813 cengal-3.1.18.4/cengal/hardware/memory/barriers/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1235 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/hardware/memory/barriers/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.154813 cengal-3.1.18.4/cengal/hardware/memory/barriers/versions/v_0/compilable/
+-rw-r--r--   0 mb        (1000) mb        (1000)     2022 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/hardware/memory/barriers/versions/v_0/compilable/__build_config.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1355 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/hardware/memory/barriers/versions/v_0/compilable/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.154813 cengal-3.1.18.4/cengal/hardware/memory/barriers/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/hardware/memory/barriers/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/hardware/memory/barriers/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.154813 cengal-3.1.18.4/cengal/hardware/memory/shared_memory/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/hardware/memory/shared_memory/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.154813 cengal-3.1.18.4/cengal/hardware/memory/shared_memory/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/hardware/memory/shared_memory/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.154813 cengal-3.1.18.4/cengal/hardware/memory/shared_memory/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1349 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/hardware/memory/shared_memory/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.154813 cengal-3.1.18.4/cengal/hardware/memory/shared_memory/versions/v_0/compilable/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1933 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/hardware/memory/shared_memory/versions/v_0/compilable/__build_config.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1360 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/hardware/memory/shared_memory/versions/v_0/compilable/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     4230 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/hardware/memory/shared_memory/versions/v_0/interfaces.py
+-rw-r--r--   0 mb        (1000) mb        (1000)   108883 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/hardware/memory/shared_memory/versions/v_0/shared_memory.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.154813 cengal-3.1.18.4/cengal/hardware/memory/shared_memory/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/hardware/memory/shared_memory/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/hardware/memory/shared_memory/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     8553 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/help_tools.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.154813 cengal-3.1.18.4/cengal/introspection/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/introspection/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.154813 cengal-3.1.18.4/cengal/introspection/inspect/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/introspection/inspect/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.154813 cengal-3.1.18.4/cengal/introspection/inspect/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/introspection/inspect/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.154813 cengal-3.1.18.4/cengal/introspection/inspect/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/introspection/inspect/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    19834 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/introspection/inspect/versions/v_0/inspect.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.154813 cengal-3.1.18.4/cengal/introspection/inspect/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/introspection/inspect/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/introspection/inspect/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.154813 cengal-3.1.18.4/cengal/introspection/third_party/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1210 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/introspection/third_party/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.154813 cengal-3.1.18.4/cengal/introspection/third_party/ctypes/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/introspection/third_party/ctypes/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.154813 cengal-3.1.18.4/cengal/introspection/third_party/ctypes/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/introspection/third_party/ctypes/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.184813 cengal-3.1.18.4/cengal/introspection/third_party/ctypes/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1229 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/introspection/third_party/ctypes/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     5359 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/introspection/third_party/ctypes/versions/v_0/ctypes.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.184813 cengal-3.1.18.4/cengal/introspection/third_party/ctypes/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/introspection/third_party/ctypes/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/introspection/third_party/ctypes/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.184813 cengal-3.1.18.4/cengal/io/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.184813 cengal-3.1.18.4/cengal/io/asock_io/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/asock_io/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.184813 cengal-3.1.18.4/cengal/io/asock_io/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/asock_io/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.184813 cengal-3.1.18.4/cengal/io/asock_io/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1281 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/asock_io/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     6006 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/asock_io/versions/v_0/base.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.184813 cengal-3.1.18.4/cengal/io/asock_io/versions/v_0/recv_buff_size_computer/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1529 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/asock_io/versions/v_0/recv_buff_size_computer/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3192 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/asock_io/versions/v_0/recv_buff_size_computer/recv_buff_size_computer__python.py
+-rw-r--r--   0 mb        (1000) mb        (1000)   113359 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/asock_io/versions/v_0/tcp_app_server.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     5057 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/asock_io/versions/v_0/tcp_link.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.184813 cengal-3.1.18.4/cengal/io/asock_io/versions/v_1/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1281 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/asock_io/versions/v_1/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    18746 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/asock_io/versions/v_1/abstract.py
+-rw-r--r--   0 mb        (1000) mb        (1000)   123889 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/asock_io/versions/v_1/asock_io_core.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    15715 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/asock_io/versions/v_1/base.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.184813 cengal-3.1.18.4/cengal/io/asock_io/versions/v_1/io_loops/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/asock_io/versions/v_1/io_loops/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3922 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/asock_io/versions/v_1/io_loops/epoll_lt.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     6409 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/asock_io/versions/v_1/io_loops/select.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.194813 cengal-3.1.18.4/cengal/io/asock_io/versions/v_1/recv_buff_size_computer/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1476 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/asock_io/versions/v_1/recv_buff_size_computer/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3130 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/asock_io/versions/v_1/recv_buff_size_computer/recv_buff_size_computer__python.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     4987 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/asock_io/versions/v_1/tcp_link.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.194813 cengal-3.1.18.4/cengal/io/core/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/core/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.194813 cengal-3.1.18.4/cengal/io/core/memory_management/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/core/memory_management/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.194813 cengal-3.1.18.4/cengal/io/core/memory_management/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/core/memory_management/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.194813 cengal-3.1.18.4/cengal/io/core/memory_management/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1240 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/core/memory_management/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3262 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/core/memory_management/versions/v_0/memory_management.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.194813 cengal-3.1.18.4/cengal/io/core/memory_management/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/core/memory_management/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/core/memory_management/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.194813 cengal-3.1.18.4/cengal/io/named_connections/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/named_connections/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.194813 cengal-3.1.18.4/cengal/io/named_connections/named_connections_manager/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/named_connections/named_connections_manager/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.194813 cengal-3.1.18.4/cengal/io/named_connections/named_connections_manager/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/named_connections/named_connections_manager/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.194813 cengal-3.1.18.4/cengal/io/named_connections/named_connections_manager/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/named_connections/named_connections_manager/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    10644 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/named_connections/named_connections_manager/versions/v_0/named_connections_manager.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.194813 cengal-3.1.18.4/cengal/io/named_connections/named_connections_manager/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/named_connections/named_connections_manager/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/named_connections/named_connections_manager/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.194813 cengal-3.1.18.4/cengal/io/named_connections/workers/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1240 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/named_connections/workers/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.194813 cengal-3.1.18.4/cengal/io/named_connections/workers/asyncio_streams/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/named_connections/workers/asyncio_streams/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.194813 cengal-3.1.18.4/cengal/io/named_connections/workers/asyncio_streams/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/named_connections/workers/asyncio_streams/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.194813 cengal-3.1.18.4/cengal/io/named_connections/workers/asyncio_streams/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1238 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/named_connections/workers/asyncio_streams/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     6610 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/named_connections/workers/asyncio_streams/versions/v_0/asyncio_streams.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.194813 cengal-3.1.18.4/cengal/io/named_connections/workers/asyncio_streams/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/named_connections/workers/asyncio_streams/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/named_connections/workers/asyncio_streams/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.214813 cengal-3.1.18.4/cengal/io/named_connections/workers/asyncio_streams_proxy/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/named_connections/workers/asyncio_streams_proxy/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.214813 cengal-3.1.18.4/cengal/io/named_connections/workers/asyncio_streams_proxy/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/named_connections/workers/asyncio_streams_proxy/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.214813 cengal-3.1.18.4/cengal/io/named_connections/workers/asyncio_streams_proxy/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1244 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/named_connections/workers/asyncio_streams_proxy/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/named_connections/workers/asyncio_streams_proxy/versions/v_0/asyncio_streams_proxy.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.214813 cengal-3.1.18.4/cengal/io/named_connections/workers/asyncio_streams_proxy/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/named_connections/workers/asyncio_streams_proxy/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/named_connections/workers/asyncio_streams_proxy/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.214813 cengal-3.1.18.4/cengal/io/net_io/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/net_io/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.214813 cengal-3.1.18.4/cengal/io/net_io/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/net_io/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.214813 cengal-3.1.18.4/cengal/io/net_io/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/net_io/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.214813 cengal-3.1.18.4/cengal/io/net_io/versions/v_0/crossplatform/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/net_io/versions/v_0/crossplatform/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.214813 cengal-3.1.18.4/cengal/io/net_io/versions/v_0/crossplatform/exceptions_handlers/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/net_io/versions/v_0/crossplatform/exceptions_handlers/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/net_io/versions/v_0/crossplatform/exceptions_handlers/abstract.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/net_io/versions/v_0/crossplatform/exceptions_handlers/linux.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/net_io/versions/v_0/crossplatform/exceptions_handlers/win32.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    11975 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/net_io/versions/v_0/net_io__linux.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    14773 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/net_io/versions/v_0/net_io_abstract.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3987 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/net_io/versions/v_0/net_io_method__epoll_lt.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     4846 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/net_io/versions/v_0/net_io_method__select.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.214813 cengal-3.1.18.4/cengal/io/recv_buff_size_computer/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/recv_buff_size_computer/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.214813 cengal-3.1.18.4/cengal/io/recv_buff_size_computer/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/recv_buff_size_computer/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.214813 cengal-3.1.18.4/cengal/io/recv_buff_size_computer/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1529 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/recv_buff_size_computer/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3192 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/recv_buff_size_computer/versions/v_0/recv_buff_size_computer__python.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.214813 cengal-3.1.18.4/cengal/io/recv_buff_size_computer/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/recv_buff_size_computer/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/recv_buff_size_computer/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.214813 cengal-3.1.18.4/cengal/io/recv_buff_size_computer/versions/v_1/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1476 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/recv_buff_size_computer/versions/v_1/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3130 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/recv_buff_size_computer/versions/v_1/recv_buff_size_computer__python.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.214813 cengal-3.1.18.4/cengal/io/recv_buff_size_computer/versions/v_1/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/recv_buff_size_computer/versions/v_1/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/recv_buff_size_computer/versions/v_1/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.214813 cengal-3.1.18.4/cengal/io/serve_free_ports/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/serve_free_ports/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.214813 cengal-3.1.18.4/cengal/io/serve_free_ports/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/serve_free_ports/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.214813 cengal-3.1.18.4/cengal/io/serve_free_ports/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1239 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/serve_free_ports/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     5139 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/serve_free_ports/versions/v_0/serve_free_ports.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.214813 cengal-3.1.18.4/cengal/io/serve_free_ports/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/serve_free_ports/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/serve_free_ports/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.214813 cengal-3.1.18.4/cengal/io/socket/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/socket/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.224813 cengal-3.1.18.4/cengal/io/socket/constants/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/socket/constants/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.224813 cengal-3.1.18.4/cengal/io/socket/constants/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/socket/constants/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.224813 cengal-3.1.18.4/cengal/io/socket/constants/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1232 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/socket/constants/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1282 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/socket/constants/versions/v_0/constants.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.224813 cengal-3.1.18.4/cengal/io/socket/constants/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/socket/constants/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/socket/constants/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.234813 cengal-3.1.18.4/cengal/io/socket/errors/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/socket/errors/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.234813 cengal-3.1.18.4/cengal/io/socket/errors/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/socket/errors/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.234813 cengal-3.1.18.4/cengal/io/socket/errors/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1229 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/socket/errors/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2430 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/socket/errors/versions/v_0/errors.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.234813 cengal-3.1.18.4/cengal/io/socket/errors/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/socket/errors/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/socket/errors/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.234813 cengal-3.1.18.4/cengal/io/used_ports/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/used_ports/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.234813 cengal-3.1.18.4/cengal/io/used_ports/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/used_ports/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.234813 cengal-3.1.18.4/cengal/io/used_ports/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1233 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/used_ports/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.234813 cengal-3.1.18.4/cengal/io/used_ports/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/used_ports/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3133 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/used_ports/versions/v_0/tests/_test__used_ports.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     8979 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/io/used_ports/versions/v_0/used_ports.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.234813 cengal-3.1.18.4/cengal/math/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/math/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.234813 cengal-3.1.18.4/cengal/math/algebra/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/math/algebra/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.234813 cengal-3.1.18.4/cengal/math/algebra/fast_algorithms/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/math/algebra/fast_algorithms/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.234813 cengal-3.1.18.4/cengal/math/algebra/fast_algorithms/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/math/algebra/fast_algorithms/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.234813 cengal-3.1.18.4/cengal/math/algebra/fast_algorithms/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1238 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/math/algebra/fast_algorithms/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1784 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/math/algebra/fast_algorithms/versions/v_0/fast_algorithms.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.234813 cengal-3.1.18.4/cengal/math/algebra/fast_algorithms/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/math/algebra/fast_algorithms/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/math/algebra/fast_algorithms/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.234813 cengal-3.1.18.4/cengal/math/geometry/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/math/geometry/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.234813 cengal-3.1.18.4/cengal/math/geometry/ellipse/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/math/geometry/ellipse/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.234813 cengal-3.1.18.4/cengal/math/geometry/ellipse/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/math/geometry/ellipse/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.234813 cengal-3.1.18.4/cengal/math/geometry/ellipse/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/math/geometry/ellipse/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     4989 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/math/geometry/ellipse/versions/v_0/ellipse.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.234813 cengal-3.1.18.4/cengal/math/geometry/ellipse/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/math/geometry/ellipse/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/math/geometry/ellipse/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2714 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/math/geometry/ellipse/versions/v_0/tests/informal_tests.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.234813 cengal-3.1.18.4/cengal/math/geometry/point/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/math/geometry/point/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.244813 cengal-3.1.18.4/cengal/math/geometry/point/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/math/geometry/point/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.244813 cengal-3.1.18.4/cengal/math/geometry/point/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1228 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/math/geometry/point/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    16020 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/math/geometry/point/versions/v_0/point.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.244813 cengal-3.1.18.4/cengal/math/geometry/point/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/math/geometry/point/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/math/geometry/point/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.244813 cengal-3.1.18.4/cengal/math/geometry/vector/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/math/geometry/vector/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.244813 cengal-3.1.18.4/cengal/math/geometry/vector/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/math/geometry/vector/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.244813 cengal-3.1.18.4/cengal/math/geometry/vector/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1229 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/math/geometry/vector/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.244813 cengal-3.1.18.4/cengal/math/geometry/vector/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/math/geometry/vector/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/math/geometry/vector/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    46033 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/math/geometry/vector/versions/v_0/vector.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.244813 cengal-3.1.18.4/cengal/math/numbers/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/math/numbers/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.244813 cengal-3.1.18.4/cengal/math/numbers/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/math/numbers/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.254813 cengal-3.1.18.4/cengal/math/numbers/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/math/numbers/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1347 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/math/numbers/versions/v_0/numbers.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.254813 cengal-3.1.18.4/cengal/math/numbers/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/math/numbers/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/math/numbers/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.254813 cengal-3.1.18.4/cengal/modules_management/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/modules_management/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1570 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/modules_management/alternative_import.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.254813 cengal-3.1.18.4/cengal/modules_management/ignore_in_build_mode/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/modules_management/ignore_in_build_mode/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.254813 cengal-3.1.18.4/cengal/modules_management/ignore_in_build_mode/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/modules_management/ignore_in_build_mode/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.254813 cengal-3.1.18.4/cengal/modules_management/ignore_in_build_mode/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1243 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/modules_management/ignore_in_build_mode/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1512 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/modules_management/ignore_in_build_mode/versions/v_0/ignore_in_build_mode.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.254813 cengal-3.1.18.4/cengal/modules_management/ignore_in_build_mode/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/modules_management/ignore_in_build_mode/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/modules_management/ignore_in_build_mode/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2183 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/modules_management/reload_module.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.254813 cengal-3.1.18.4/cengal/os/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/os/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1349 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/os/help_tools.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.254813 cengal-3.1.18.4/cengal/parallel_execution/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.254813 cengal-3.1.18.4/cengal/parallel_execution/asyncio/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/asyncio/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.254813 cengal-3.1.18.4/cengal/parallel_execution/asyncio/atasks/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/asyncio/atasks/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.254813 cengal-3.1.18.4/cengal/parallel_execution/asyncio/atasks/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/asyncio/atasks/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.254813 cengal-3.1.18.4/cengal/parallel_execution/asyncio/atasks/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1229 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/asyncio/atasks/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1848 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/asyncio/atasks/versions/v_0/atasks.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.254813 cengal-3.1.18.4/cengal/parallel_execution/asyncio/atasks/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/asyncio/atasks/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/asyncio/atasks/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.264813 cengal-3.1.18.4/cengal/parallel_execution/asyncio/efficient_streams/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/asyncio/efficient_streams/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.274813 cengal-3.1.18.4/cengal/parallel_execution/asyncio/efficient_streams/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/asyncio/efficient_streams/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.274813 cengal-3.1.18.4/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1361 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    12105 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/efficient_streams_abstract.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2468 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/efficient_streams_base.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1990 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/efficient_streams_base_internal.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    51582 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/tcp_efficient_streams.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.274813 cengal-3.1.18.4/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3773 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/tests/asyncio_streams_client.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     6498 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/tests/asyncio_streams_server.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    35910 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/udp_efficient_streams.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.274813 cengal-3.1.18.4/cengal/parallel_execution/asyncio/init_loop/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/asyncio/init_loop/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.274813 cengal-3.1.18.4/cengal/parallel_execution/asyncio/init_loop/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/asyncio/init_loop/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.274813 cengal-3.1.18.4/cengal/parallel_execution/asyncio/init_loop/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1232 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/asyncio/init_loop/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1393 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/asyncio/init_loop/versions/v_0/init_loop.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.274813 cengal-3.1.18.4/cengal/parallel_execution/asyncio/init_loop/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/asyncio/init_loop/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/asyncio/init_loop/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.274813 cengal-3.1.18.4/cengal/parallel_execution/asyncio/run_in_process_pool/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/asyncio/run_in_process_pool/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.274813 cengal-3.1.18.4/cengal/parallel_execution/asyncio/run_in_process_pool/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/asyncio/run_in_process_pool/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.274813 cengal-3.1.18.4/cengal/parallel_execution/asyncio/run_in_process_pool/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1242 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/asyncio/run_in_process_pool/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     9440 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/asyncio/run_in_process_pool/versions/v_0/run_in_process_pool.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.274813 cengal-3.1.18.4/cengal/parallel_execution/asyncio/run_in_process_pool/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/asyncio/run_in_process_pool/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/asyncio/run_in_process_pool/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.274813 cengal-3.1.18.4/cengal/parallel_execution/asyncio/run_loop/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/asyncio/run_loop/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.274813 cengal-3.1.18.4/cengal/parallel_execution/asyncio/run_loop/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/asyncio/run_loop/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.274813 cengal-3.1.18.4/cengal/parallel_execution/asyncio/run_loop/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/asyncio/run_loop/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3527 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/asyncio/run_loop/versions/v_0/run_loop.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.284813 cengal-3.1.18.4/cengal/parallel_execution/asyncio/run_loop/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/asyncio/run_loop/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/asyncio/run_loop/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.284813 cengal-3.1.18.4/cengal/parallel_execution/asyncio/timed_yield/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/asyncio/timed_yield/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.284813 cengal-3.1.18.4/cengal/parallel_execution/asyncio/timed_yield/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/asyncio/timed_yield/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.284813 cengal-3.1.18.4/cengal/parallel_execution/asyncio/timed_yield/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1234 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/asyncio/timed_yield/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.284813 cengal-3.1.18.4/cengal/parallel_execution/asyncio/timed_yield/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/asyncio/timed_yield/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/asyncio/timed_yield/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1642 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/asyncio/timed_yield/versions/v_0/timed_yield.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.284813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1301 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.284813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_scheduler/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_scheduler/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.284813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_scheduler/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_scheduler/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.284813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_scheduler/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1237 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_scheduler/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)   126514 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_scheduler/versions/v_0/coro_scheduler.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.294813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_scheduler/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_scheduler/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_scheduler/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.294813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1453 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.294813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.294813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.294813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1238 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    11265 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/versions/v_0/async_event_bus.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.294813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.294813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.294813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.294813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1235 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    20728 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/versions/v_0/asyncio_loop.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.294813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.294813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/communication/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/communication/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.294813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/communication/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/communication/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.294813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/communication/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1236 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/communication/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     6566 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/communication/versions/v_0/communication.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.294813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/communication/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/communication/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/communication/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.294813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.294813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.304813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     4174 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/versions/v_0/cpu_tick_count_per_second.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.304813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.304813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/db/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/db/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.304813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/db/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/db/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.304813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/db/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/db/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    55878 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/db/versions/v_0/db.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.304813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/db/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/db/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/db/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.304813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.304813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.314813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1232 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     7707 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/versions/v_0/event_bus.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.314813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.314813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.314813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.314813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1238 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     7638 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/versions/v_0/fast_aggregator.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.314813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.314813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/instance/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/instance/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.314813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/instance/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/instance/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.314813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/instance/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/instance/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     9089 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/instance/versions/v_0/instance.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.314813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/instance/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/instance/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/instance/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.314813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.314813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.314813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1232 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     5522 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/versions/v_0/kill_coro.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.314813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.314813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.324813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.324813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1237 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     7537 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/versions/v_0/kill_coro_list.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.324813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.324813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.324813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.324813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1233 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3908 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/versions/v_0/lazy_print.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.324813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.324813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.324813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.324813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1227 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    21255 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/versions/v_0/lmdb.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.324813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.324813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/log/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/log/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.334813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/log/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/log/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.334813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/log/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/log/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    13686 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/log/versions/v_0/log.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.334813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/log/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/log/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/log/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.334813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.334813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.334813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1265 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     5971 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/v_0/bytecode_patcher.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    27436 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/v_0/loop_yield.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.334813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.334813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.334813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.334813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    22657 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/versions/v_0/put_coro.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.334813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.334813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.334813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.334813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1236 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     6168 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/versions/v_0/put_coro_list.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.334813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.334813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.334813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.334813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1240 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    25204 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/versions/v_0/read_write_locker.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.334813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.334813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.334813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.344813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1235 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     4956 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/class_info.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3827 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/commands.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1399 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/exceptions.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     5316 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/remote_node.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    21055 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/remote_nodes.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     6044 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/request_class_info.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     5877 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/serializers.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.344813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.344813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.344813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.344813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3465 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/versions/v_0/run_coro.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.344813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.344813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.344813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.344813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1236 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1748 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/versions/v_0/shutdown_loop.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.344813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.344813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.344813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.354813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1253 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2897 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/versions/v_0/shutdown_on_keyboard_interrupt.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.354813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.354813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.434813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.454813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1235 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1652 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/versions/v_0/simple_yield.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.454813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.454813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/sleep/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/sleep/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.454813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/sleep/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/sleep/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.454813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/sleep/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1232 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/sleep/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2901 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/sleep/versions/v_0/sleep.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.454813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/sleep/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/sleep/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/sleep/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.454813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.454813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.454813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1235 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1725 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/versions/v_0/some_printer.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.454813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.454813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.454813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.454813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1233 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.454813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     6825 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/versions/v_0/throw_coro.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.454813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.454813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.454813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1238 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.454813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     7154 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/versions/v_0/throw_coro_list.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.454813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.454813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.454813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1240 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.464813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    11822 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/versions/v_0/timer_coro_runner.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.464813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.464813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.464813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1240 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.464813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    11053 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/versions/v_0/timer_func_runner.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.464813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.464813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.464813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.464813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    28117 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/v_0/tkinter.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.464813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.464813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.474813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1232 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.474813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    18947 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/versions/v_0/wait_coro.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.474813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1210 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.474813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.474813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.474813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/versions/v_0/general.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.474813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.474813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.474813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.474813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1252 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     5687 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/versions/v_0/service_with_a_direct_request.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.474813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.474813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1233 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.474813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/await_coro/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/await_coro/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.474813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/await_coro/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/await_coro/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.474813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/await_coro/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1233 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/await_coro/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    14142 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/await_coro/versions/v_0/await_coro.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.494813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/await_coro/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/await_coro/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/await_coro/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.494813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.494813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.494813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1240 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     5186 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/versions/v_0/coro_flow_control.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.494813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.494813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/low_latency/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1227 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/low_latency/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.494813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.494813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.494813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3175 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/v_0/ajson.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     5182 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/v_0/json.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.494813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.494813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.494813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.504813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1235 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     5979 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/versions/v_0/prepare_loop.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.504813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.504813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.504813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.504813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1234 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     8391 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/v_0/run_in_loop.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.504813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.504813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/wait_coro/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/wait_coro/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.504813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/wait_coro/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/wait_coro/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.504813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/wait_coro/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1232 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/wait_coro/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.514813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/wait_coro/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/wait_coro/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/wait_coro/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     7876 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/wait_coro/versions/v_0/wait_coro.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.514813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1210 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.514813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/customtkinter/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/customtkinter/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.534813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/customtkinter/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/customtkinter/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.534813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/customtkinter/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1236 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/customtkinter/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1829 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/customtkinter/versions/v_0/customtkinter.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.534813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/customtkinter/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/customtkinter/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/customtkinter/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.534813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/nicegui/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/nicegui/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.534813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/nicegui/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/nicegui/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.534813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/nicegui/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/nicegui/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    19201 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/nicegui/versions/v_0/nicegui.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.534813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/nicegui/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/nicegui/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/nicegui/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.534813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/pytermgui/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/pytermgui/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.534813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.534813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1232 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     4691 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/v_0/pytermgui.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.534813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.534813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/qt/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/qt/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.534813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/qt/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/qt/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.534813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/qt/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1225 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/qt/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    13310 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/qt/versions/v_0/qt.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.534813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/qt/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/qt/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/qt/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.534813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/uvicorn/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/uvicorn/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.534813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/uvicorn/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/uvicorn/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.554813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/uvicorn/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/uvicorn/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.554813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/uvicorn/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/uvicorn/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/uvicorn/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     5547 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/uvicorn/versions/v_0/uvicorn.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.554813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/uvloop/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/uvloop/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.554813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/uvloop/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/uvloop/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.554813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/uvloop/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1229 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/uvloop/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.554813 cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/uvloop/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/uvloop/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/uvloop/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1530 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/uvloop/versions/v_0/uvloop.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.554813 cengal-3.1.18.4/cengal/parallel_execution/green_threads_tools/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/green_threads_tools/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3707 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/green_threads_tools/task_management.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.554813 cengal-3.1.18.4/cengal/parallel_execution/multiprocess/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1251 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/multiprocess/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2840 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/multiprocess/multiprocess_testing.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3086 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/multiprocess/multiprocessing_task_pool.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    24843 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/multiprocess/multiprocessing_task_runner.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.554813 cengal-3.1.18.4/cengal/parallel_execution/multithreading/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/multithreading/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     7151 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/parallel_execution/multithreading/thread_workers_pool.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.554813 cengal-3.1.18.4/cengal/performance_test_lib/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/performance_test_lib/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.554813 cengal-3.1.18.4/cengal/performance_test_lib/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/performance_test_lib/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.554813 cengal-3.1.18.4/cengal/performance_test_lib/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1243 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/performance_test_lib/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     8268 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/performance_test_lib/versions/v_0/performance_test_lib.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.554813 cengal-3.1.18.4/cengal/performance_test_lib/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1249 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/performance_test_lib/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2241 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/performance_test_lib/versions/v_0/tests/test__performance_test_lib.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.564813 cengal-3.1.18.4/cengal/performance_test_lib/versions/v_1/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1243 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/performance_test_lib/versions/v_1/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     9291 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/performance_test_lib/versions/v_1/performance_test_lib.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.564813 cengal-3.1.18.4/cengal/performance_test_lib/versions/v_1/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1249 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/performance_test_lib/versions/v_1/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2241 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/performance_test_lib/versions/v_1/tests/test__performance_test_lib.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.564813 cengal-3.1.18.4/cengal/shared_memory/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/shared_memory/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.564813 cengal-3.1.18.4/cengal/shared_memory/versions/
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.564813 cengal-3.1.18.4/cengal/shared_memory/versions/1/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/shared_memory/versions/1/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1502 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/shared_memory/versions/1/mmap.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/shared_memory/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.564813 cengal-3.1.18.4/cengal/statistics/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/statistics/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.564813 cengal-3.1.18.4/cengal/statistics/normal_distribution/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/statistics/normal_distribution/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.564813 cengal-3.1.18.4/cengal/statistics/normal_distribution/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/statistics/normal_distribution/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.564813 cengal-3.1.18.4/cengal/statistics/normal_distribution/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1242 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/statistics/normal_distribution/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     4157 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/statistics/normal_distribution/versions/v_0/normal_distribution.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.564813 cengal-3.1.18.4/cengal/statistics/normal_distribution/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/statistics/normal_distribution/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/statistics/normal_distribution/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3262 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/system.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.564813 cengal-3.1.18.4/cengal/testing_lib/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/testing_lib/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3057 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/testing_lib/tests_list_runner.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.574813 cengal-3.1.18.4/cengal/text_processing/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/text_processing/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.574813 cengal-3.1.18.4/cengal/text_processing/brackets_processing/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/text_processing/brackets_processing/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.574813 cengal-3.1.18.4/cengal/text_processing/brackets_processing/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/text_processing/brackets_processing/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.584813 cengal-3.1.18.4/cengal/text_processing/brackets_processing/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1290 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/text_processing/brackets_processing/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2345 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/text_processing/brackets_processing/versions/v_0/brackets.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     6468 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/text_processing/brackets_processing/versions/v_0/processing.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3780 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/text_processing/brackets_processing/versions/v_0/standard_brackets.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.584813 cengal-3.1.18.4/cengal/text_processing/brackets_processing/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/text_processing/brackets_processing/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/text_processing/brackets_processing/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.584813 cengal-3.1.18.4/cengal/text_processing/encoding_detection/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/text_processing/encoding_detection/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.584813 cengal-3.1.18.4/cengal/text_processing/encoding_detection/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/text_processing/encoding_detection/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.584813 cengal-3.1.18.4/cengal/text_processing/encoding_detection/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1241 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/text_processing/encoding_detection/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2465 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/text_processing/encoding_detection/versions/v_0/encoding_detection.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.584813 cengal-3.1.18.4/cengal/text_processing/encoding_detection/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/text_processing/encoding_detection/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/text_processing/encoding_detection/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    11969 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/text_processing/help_tools.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.584813 cengal-3.1.18.4/cengal/text_processing/optional_formatter/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/text_processing/optional_formatter/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.584813 cengal-3.1.18.4/cengal/text_processing/optional_formatter/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/text_processing/optional_formatter/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.584813 cengal-3.1.18.4/cengal/text_processing/optional_formatter/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1241 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/text_processing/optional_formatter/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     4275 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/text_processing/optional_formatter/versions/v_0/optional_formatter.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.584813 cengal-3.1.18.4/cengal/text_processing/optional_formatter/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/text_processing/optional_formatter/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/text_processing/optional_formatter/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.584813 cengal-3.1.18.4/cengal/text_processing/simple_config_file_processor/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/text_processing/simple_config_file_processor/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.584813 cengal-3.1.18.4/cengal/text_processing/simple_config_file_processor/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/text_processing/simple_config_file_processor/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.584813 cengal-3.1.18.4/cengal/text_processing/simple_config_file_processor/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1251 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/text_processing/simple_config_file_processor/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/text_processing/simple_config_file_processor/versions/v_0/simple_config_file_processor.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.594813 cengal-3.1.18.4/cengal/text_processing/simple_config_file_processor/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/text_processing/simple_config_file_processor/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/text_processing/simple_config_file_processor/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.594813 cengal-3.1.18.4/cengal/text_processing/text_patch/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/text_processing/text_patch/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.594813 cengal-3.1.18.4/cengal/text_processing/text_patch/brackets/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/text_processing/text_patch/brackets/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.594813 cengal-3.1.18.4/cengal/text_processing/text_patch/brackets/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/text_processing/text_patch/brackets/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.604813 cengal-3.1.18.4/cengal/text_processing/text_patch/brackets/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/text_processing/text_patch/brackets/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2010 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/text_processing/text_patch/brackets/versions/v_0/brackets.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.604813 cengal-3.1.18.4/cengal/text_processing/text_patch/brackets/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/text_processing/text_patch/brackets/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/text_processing/text_patch/brackets/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.604813 cengal-3.1.18.4/cengal/text_processing/text_patch/simple/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/text_processing/text_patch/simple/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.604813 cengal-3.1.18.4/cengal/text_processing/text_patch/simple/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/text_processing/text_patch/simple/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.604813 cengal-3.1.18.4/cengal/text_processing/text_patch/simple/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1229 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/text_processing/text_patch/simple/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1830 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/text_processing/text_patch/simple/versions/v_0/simple.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.604813 cengal-3.1.18.4/cengal/text_processing/text_patch/simple/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/text_processing/text_patch/simple/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/text_processing/text_patch/simple/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.614813 cengal-3.1.18.4/cengal/text_processing/text_processing/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/text_processing/text_processing/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.614813 cengal-3.1.18.4/cengal/text_processing/text_processing/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/text_processing/text_processing/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.614813 cengal-3.1.18.4/cengal/text_processing/text_processing/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1233 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/text_processing/text_processing/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     6282 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/text_processing/text_processing/versions/v_0/processing.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.614813 cengal-3.1.18.4/cengal/text_processing/text_processing/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/text_processing/text_processing/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/text_processing/text_processing/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.614813 cengal-3.1.18.4/cengal/text_processing/text_translator/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/text_processing/text_translator/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.614813 cengal-3.1.18.4/cengal/text_processing/text_translator/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/text_processing/text_translator/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.614813 cengal-3.1.18.4/cengal/text_processing/text_translator/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1238 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/text_processing/text_translator/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.624813 cengal-3.1.18.4/cengal/text_processing/text_translator/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/text_processing/text_translator/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/text_processing/text_translator/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    12696 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/text_processing/text_translator/versions/v_0/text_translator.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.624813 cengal-3.1.18.4/cengal/text_processing/utf_bom_processing/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/text_processing/utf_bom_processing/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.624813 cengal-3.1.18.4/cengal/text_processing/utf_bom_processing/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/text_processing/utf_bom_processing/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.624813 cengal-3.1.18.4/cengal/text_processing/utf_bom_processing/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1241 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/text_processing/utf_bom_processing/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.624813 cengal-3.1.18.4/cengal/text_processing/utf_bom_processing/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/text_processing/utf_bom_processing/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/text_processing/utf_bom_processing/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2994 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/text_processing/utf_bom_processing/versions/v_0/utf_bom_processing.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.624813 cengal-3.1.18.4/cengal/time_management/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/time_management/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.624813 cengal-3.1.18.4/cengal/time_management/cpu_clock/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/time_management/cpu_clock/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.624813 cengal-3.1.18.4/cengal/time_management/cpu_clock/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/time_management/cpu_clock/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.624813 cengal-3.1.18.4/cengal/time_management/cpu_clock/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1232 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/time_management/cpu_clock/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.624813 cengal-3.1.18.4/cengal/time_management/cpu_clock/versions/v_0/compilable/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1357 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/time_management/cpu_clock/versions/v_0/compilable/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1930 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/time_management/cpu_clock/versions/v_0/compilable/__x__build_config.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1640 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/time_management/cpu_clock/versions/v_0/cpu_clock.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.624813 cengal-3.1.18.4/cengal/time_management/cpu_clock/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/time_management/cpu_clock/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/time_management/cpu_clock/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.624813 cengal-3.1.18.4/cengal/time_management/cpu_clock_cycles/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/time_management/cpu_clock_cycles/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.624813 cengal-3.1.18.4/cengal/time_management/cpu_clock_cycles/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/time_management/cpu_clock_cycles/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.624813 cengal-3.1.18.4/cengal/time_management/cpu_clock_cycles/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1233 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/time_management/cpu_clock_cycles/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.624813 cengal-3.1.18.4/cengal/time_management/cpu_clock_cycles/versions/v_0/compilable/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1936 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/time_management/cpu_clock_cycles/versions/v_0/compilable/__build_config.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1412 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/time_management/cpu_clock_cycles/versions/v_0/compilable/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.624813 cengal-3.1.18.4/cengal/time_management/cpu_clock_cycles/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/time_management/cpu_clock_cycles/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/time_management/cpu_clock_cycles/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.624813 cengal-3.1.18.4/cengal/time_management/high_precision_sync_sleep/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/time_management/high_precision_sync_sleep/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.624813 cengal-3.1.18.4/cengal/time_management/high_precision_sync_sleep/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/time_management/high_precision_sync_sleep/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.624813 cengal-3.1.18.4/cengal/time_management/high_precision_sync_sleep/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1369 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/time_management/high_precision_sync_sleep/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.624813 cengal-3.1.18.4/cengal/time_management/high_precision_sync_sleep/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/time_management/high_precision_sync_sleep/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/time_management/high_precision_sync_sleep/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.644813 cengal-3.1.18.4/cengal/time_management/load_best_timer/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/time_management/load_best_timer/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.644813 cengal-3.1.18.4/cengal/time_management/load_best_timer/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/time_management/load_best_timer/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.644813 cengal-3.1.18.4/cengal/time_management/load_best_timer/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1238 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/time_management/load_best_timer/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1446 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/time_management/load_best_timer/versions/v_0/load_best_timer.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.644813 cengal-3.1.18.4/cengal/time_management/relative_time/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1366 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/time_management/relative_time/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.644813 cengal-3.1.18.4/cengal/time_management/relative_time/approximate_representation/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/time_management/relative_time/approximate_representation/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.644813 cengal-3.1.18.4/cengal/time_management/relative_time/approximate_representation/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/time_management/relative_time/approximate_representation/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.644813 cengal-3.1.18.4/cengal/time_management/relative_time/approximate_representation/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1249 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/time_management/relative_time/approximate_representation/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     8715 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/time_management/relative_time/approximate_representation/versions/v_0/approximate_representation.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.644813 cengal-3.1.18.4/cengal/time_management/relative_time/bysiness_relativedelta/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/time_management/relative_time/bysiness_relativedelta/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.644813 cengal-3.1.18.4/cengal/time_management/relative_time/bysiness_relativedelta/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/time_management/relative_time/bysiness_relativedelta/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.644813 cengal-3.1.18.4/cengal/time_management/relative_time/bysiness_relativedelta/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1245 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/time_management/relative_time/bysiness_relativedelta/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1490 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/time_management/relative_time/bysiness_relativedelta/versions/v_0/bysiness_relativedelta.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.644813 cengal-3.1.18.4/cengal/time_management/relative_time/constants/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/time_management/relative_time/constants/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.644813 cengal-3.1.18.4/cengal/time_management/relative_time/constants/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/time_management/relative_time/constants/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.644813 cengal-3.1.18.4/cengal/time_management/relative_time/constants/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1232 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/time_management/relative_time/constants/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1419 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/time_management/relative_time/constants/versions/v_0/constants.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.644813 cengal-3.1.18.4/cengal/time_management/relative_time/relativedelta/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/time_management/relative_time/relativedelta/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.644813 cengal-3.1.18.4/cengal/time_management/relative_time/relativedelta/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/time_management/relative_time/relativedelta/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.644813 cengal-3.1.18.4/cengal/time_management/relative_time/relativedelta/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1236 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/time_management/relative_time/relativedelta/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1860 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/time_management/relative_time/relativedelta/versions/v_0/relativedelta.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.644813 cengal-3.1.18.4/cengal/time_management/relative_time/timedelta/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/time_management/relative_time/timedelta/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.644813 cengal-3.1.18.4/cengal/time_management/relative_time/timedelta/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/time_management/relative_time/timedelta/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.644813 cengal-3.1.18.4/cengal/time_management/relative_time/timedelta/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1232 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/time_management/relative_time/timedelta/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1633 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/time_management/relative_time/timedelta/versions/v_0/timedelta.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.644813 cengal-3.1.18.4/cengal/time_management/repeat_for_a_time/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/time_management/repeat_for_a_time/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.644813 cengal-3.1.18.4/cengal/time_management/repeat_for_a_time/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/time_management/repeat_for_a_time/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.644813 cengal-3.1.18.4/cengal/time_management/repeat_for_a_time/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1457 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/time_management/repeat_for_a_time/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    13454 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/time_management/repeat_for_a_time/versions/v_0/repeat_for_a_time__python.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.644813 cengal-3.1.18.4/cengal/time_management/repeat_for_a_time/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/time_management/repeat_for_a_time/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/time_management/repeat_for_a_time/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    16609 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/time_management/repeat_for_a_time/versions/v_0/tests/example_for__repeat_for_a_time.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.644813 cengal-3.1.18.4/cengal/time_management/sleep_tools/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/time_management/sleep_tools/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.644813 cengal-3.1.18.4/cengal/time_management/sleep_tools/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/time_management/sleep_tools/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.654813 cengal-3.1.18.4/cengal/time_management/sleep_tools/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1234 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/time_management/sleep_tools/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     4701 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/time_management/sleep_tools/versions/v_0/sleep_tools.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.664813 cengal-3.1.18.4/cengal/time_management/sleep_tools/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/time_management/sleep_tools/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/time_management/sleep_tools/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.664813 cengal-3.1.18.4/cengal/time_management/timer/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/time_management/timer/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.664813 cengal-3.1.18.4/cengal/time_management/timer/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/time_management/timer/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.664813 cengal-3.1.18.4/cengal/time_management/timer/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1228 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/time_management/timer/versions/v_0/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.664813 cengal-3.1.18.4/cengal/time_management/timer/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/time_management/timer/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/time_management/timer/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     4568 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/time_management/timer/versions/v_0/timer.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.664813 cengal-3.1.18.4/cengal/time_management/timer/versions/v_1/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1228 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/time_management/timer/versions/v_1/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.664813 cengal-3.1.18.4/cengal/time_management/timer/versions/v_1/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/time_management/timer/versions/v_1/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/time_management/timer/versions/v_1/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     6792 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/time_management/timer/versions/v_1/timer.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.664813 cengal-3.1.18.4/cengal/time_management/timer_precision/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/time_management/timer_precision/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.664813 cengal-3.1.18.4/cengal/time_management/timer_precision/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/time_management/timer_precision/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.664813 cengal-3.1.18.4/cengal/time_management/timer_precision/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1243 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/time_management/timer_precision/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1867 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/time_management/timer_precision/versions/v_0/test_timer_precision.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.674813 cengal-3.1.18.4/cengal/time_management/timer_precision/versions/v_1/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1238 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/time_management/timer_precision/versions/v_1/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     4328 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/time_management/timer_precision/versions/v_1/timer_precision.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.674813 cengal-3.1.18.4/cengal/unittest/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/unittest/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.674813 cengal-3.1.18.4/cengal/unittest/behavior_stabilizer/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/unittest/behavior_stabilizer/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.674813 cengal-3.1.18.4/cengal/unittest/behavior_stabilizer/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/unittest/behavior_stabilizer/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.674813 cengal-3.1.18.4/cengal/unittest/behavior_stabilizer/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1242 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/unittest/behavior_stabilizer/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2033 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/unittest/behavior_stabilizer/versions/v_0/behavior_stabilizer.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.674813 cengal-3.1.18.4/cengal/unittest/behavior_stabilizer/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/unittest/behavior_stabilizer/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/unittest/behavior_stabilizer/versions/v_0/tests/_test__behavior_stabilizer.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.674813 cengal-3.1.18.4/cengal/unittest/patcher/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/unittest/patcher/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.674813 cengal-3.1.18.4/cengal/unittest/patcher/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/unittest/patcher/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.674813 cengal-3.1.18.4/cengal/unittest/patcher/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1230 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/unittest/patcher/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3085 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/unittest/patcher/versions/v_0/patcher.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.674813 cengal-3.1.18.4/cengal/unittest/patcher/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/unittest/patcher/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/unittest/patcher/versions/v_0/tests/_test__patcher.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.684813 cengal-3.1.18.4/cengal/universal_parser/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/universal_parser/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1208 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/universal_parser/help_tools.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1378 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/universal_parser/idioms.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1229 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/universal_parser/parser.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     8668 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/universal_parser/test.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    75710 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/universal_parser/types.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.684813 cengal-3.1.18.4/cengal/upk_helping_tools/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/upk_helping_tools/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     2300 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/upk_helping_tools/upk_api.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1822 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/upk_helping_tools/upk_constants.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     6519 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/upk_helping_tools/upk_utils_api.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.684813 cengal-3.1.18.4/cengal/user_interface/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/user_interface/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.684813 cengal-3.1.18.4/cengal/user_interface/console/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1325 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/user_interface/console/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3505 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/user_interface/console/chooser.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1550 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/user_interface/console/colorama_helpers.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    11361 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/user_interface/console/encoding_changer.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.684813 cengal-3.1.18.4/cengal/user_interface/console/progress_meter/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/user_interface/console/progress_meter/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.684813 cengal-3.1.18.4/cengal/user_interface/console/progress_meter/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/user_interface/console/progress_meter/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.684813 cengal-3.1.18.4/cengal/user_interface/console/progress_meter/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1365 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/user_interface/console/progress_meter/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     4876 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/user_interface/console/progress_meter/versions/v_0/progress_meter.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1275 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/user_interface/console/progress_meter/versions/v_0/progress_meter_python2.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.684813 cengal-3.1.18.4/cengal/user_interface/gui/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/user_interface/gui/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.684813 cengal-3.1.18.4/cengal/user_interface/gui/nt/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1207 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/user_interface/gui/nt/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.684813 cengal-3.1.18.4/cengal/user_interface/gui/nt/blur_behind/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/user_interface/gui/nt/blur_behind/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.684813 cengal-3.1.18.4/cengal/user_interface/gui/nt/blur_behind/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/user_interface/gui/nt/blur_behind/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.694813 cengal-3.1.18.4/cengal/user_interface/gui/nt/blur_behind/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1234 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/user_interface/gui/nt/blur_behind/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3162 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/user_interface/gui/nt/blur_behind/versions/v_0/blur_behind.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.704813 cengal-3.1.18.4/cengal/user_interface/gui/nt/blur_behind/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/user_interface/gui/nt/blur_behind/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/user_interface/gui/nt/blur_behind/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.704813 cengal-3.1.18.4/cengal/user_interface/gui/nt/dpi_awareness/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/user_interface/gui/nt/dpi_awareness/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.704813 cengal-3.1.18.4/cengal/user_interface/gui/nt/dpi_awareness/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/user_interface/gui/nt/dpi_awareness/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.704813 cengal-3.1.18.4/cengal/user_interface/gui/nt/dpi_awareness/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1236 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/user_interface/gui/nt/dpi_awareness/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     3687 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/user_interface/gui/nt/dpi_awareness/versions/v_0/dpi_awareness.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.704813 cengal-3.1.18.4/cengal/user_interface/gui/nt/dpi_awareness/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/user_interface/gui/nt/dpi_awareness/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/user_interface/gui/nt/dpi_awareness/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.704813 cengal-3.1.18.4/cengal/user_interface/plot/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/user_interface/plot/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.704813 cengal-3.1.18.4/cengal/user_interface/plot/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/user_interface/plot/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.704813 cengal-3.1.18.4/cengal/user_interface/plot/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1227 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/user_interface/plot/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1878 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/user_interface/plot/versions/v_0/plot.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.704813 cengal-3.1.18.4/cengal/user_interface/plot/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/user_interface/plot/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:51.000000 cengal-3.1.18.4/cengal/user_interface/plot/versions/v_0/tests/_test__template_submodule.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.704813 cengal-3.1.18.4/cengal/web_tools/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/web_tools/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.704813 cengal-3.1.18.4/cengal/web_tools/detect_browsers_host_device_type/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/web_tools/detect_browsers_host_device_type/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.704813 cengal-3.1.18.4/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1231 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.704813 cengal-3.1.18.4/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1226 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/__init__.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.704813 cengal-3.1.18.4/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/v_0/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1241 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/v_0/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     4333 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/v_0/by_http_user_agent.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:46.704813 cengal-3.1.18.4/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/v_0/tests/
+-rw-r--r--   0 mb        (1000) mb        (1000)     1248 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/v_0/tests/__init__.py
+-rw-r--r--   0 mb        (1000) mb        (1000)     1206 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/v_0/tests/_test__template_submodule.py
+-rw-r--r--   0 mb        (1000) mb        (1000)    12870 2023-05-19 10:11:50.000000 cengal-3.1.18.4/cengal/web_tools/help_tools.py
+drwxr-xr-x   0 mb        (1000) mb        (1000)        0 2023-05-21 17:17:45.904813 cengal-3.1.18.4/cengal.egg-info/
+-rw-r--r--   0 mb        (1000) mb        (1000)    27225 2023-05-21 17:17:45.000000 cengal-3.1.18.4/cengal.egg-info/PKG-INFO
+-rw-r--r--   0 mb        (1000) mb        (1000)    86365 2023-05-21 17:17:45.000000 cengal-3.1.18.4/cengal.egg-info/SOURCES.txt
+-rw-r--r--   0 mb        (1000) mb        (1000)        1 2023-05-21 17:17:45.000000 cengal-3.1.18.4/cengal.egg-info/dependency_links.txt
+-rw-r--r--   0 mb        (1000) mb        (1000)      211 2023-05-21 17:17:45.000000 cengal-3.1.18.4/cengal.egg-info/requires.txt
+-rw-r--r--   0 mb        (1000) mb        (1000)        7 2023-05-21 17:17:45.000000 cengal-3.1.18.4/cengal.egg-info/top_level.txt
+-rw-r--r--   0 mb        (1000) mb        (1000)      156 2023-04-22 17:37:18.000000 cengal-3.1.18.4/pyproject.toml
+-rw-r--r--   0 mb        (1000) mb        (1000)       38 2023-05-21 17:17:46.704813 cengal-3.1.18.4/setup.cfg
+-rw-r--r--   0 mb        (1000) mb        (1000)     8547 2023-05-21 17:17:19.000000 cengal-3.1.18.4/setup.py
```

### Comparing `cengal-3.1.18.3/LICENSE.md` & `cengal-3.1.18.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/NOTICE` & `cengal-3.1.18.4/NOTICE`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/PKG-INFO` & `cengal-3.1.18.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cengal
-Version: 3.1.18.3
+Version: 3.1.18.4
 Summary: General purpose library
 Home-page: https://github.com/FI-Mihej/Cengal
 Author: ButenkoMS
 Author-email: gtalk@butenkoms.space
 License: Apache License, Version 2.0
 Keywords: async loop,coroutine,async Qt,async Tkinter,bytecode manipulation,introspection,text parsing
 Classifier: Programming Language :: Python :: 3
@@ -396,15 +396,15 @@
 
 * [General idea, greenlet main Cengal.coro](https://github.com/FI-Mihej/Cengal/blob/master/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/v_0/development/main.py)
 * [General idea, async main Cengal.coro](https://github.com/FI-Mihej/Cengal/blob/master/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/v_0/development/amain.py)
 * [Transparent interconnection between Cengal.coroutines and asyncio](https://github.com/FI-Mihej/Cengal/blob/master/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/v_0/development/asyncio_interconnection.py)
 
 ### Text processing example
 
-[Ensures and updates copyright (with dates) in each Cengal's source file](https://github.com/FI-Mihej/Cengal/blob/master/cengal_setup_scripts/ensure_copyright/ensure_copyright.py)
+[Ensures and updates copyright (with dates) in each Cengal's source file](https://github.com/FI-Mihej/Cengal/blob/master/cengal._cengal_setup_scripts/ensure_copyright/ensure_copyright.py)
 
 ## Projects using Cengal
 
 * [flet_async](https://github.com/FI-Mihej/flet_async) - wrapper which makes [Flet](https://github.com/flet-dev/flet) async and brings booth Cengal.coroutines and asyncio to Flet (Flutter based UI)
 * [justpy_containers](https://github.com/FI-Mihej/justpy_containers) - wrapper around [JustPy](https://github.com/justpy-org/justpy) in order to bring more security and more production-needed features to JustPy (VueJS based UI)
 * [Bensbach](https://github.com/FI-Mihej/Bensbach) - decompiler from Unreal Engine 3 bytecode to a Lisp-like script and compiler back to Unreal Engine 3 bytecode. Made for a game modding purposes
 * [Realistic-Damage-Model-mod-for-Long-War](https://github.com/FI-Mihej/Realistic-Damage-Model-mod-for-Long-War) - Mod for both the original XCOM:EW and the mod Long War. Was made with a Bensbach, which was made with Cengal
```

### Comparing `cengal-3.1.18.3/README.md` & `cengal-3.1.18.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -291,15 +291,15 @@
 
 * [General idea, greenlet main Cengal.coro](https://github.com/FI-Mihej/Cengal/blob/master/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/v_0/development/main.py)
 * [General idea, async main Cengal.coro](https://github.com/FI-Mihej/Cengal/blob/master/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/v_0/development/amain.py)
 * [Transparent interconnection between Cengal.coroutines and asyncio](https://github.com/FI-Mihej/Cengal/blob/master/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/v_0/development/asyncio_interconnection.py)
 
 ### Text processing example
 
-[Ensures and updates copyright (with dates) in each Cengal's source file](https://github.com/FI-Mihej/Cengal/blob/master/cengal_setup_scripts/ensure_copyright/ensure_copyright.py)
+[Ensures and updates copyright (with dates) in each Cengal's source file](https://github.com/FI-Mihej/Cengal/blob/master/cengal._cengal_setup_scripts/ensure_copyright/ensure_copyright.py)
 
 ## Projects using Cengal
 
 * [flet_async](https://github.com/FI-Mihej/flet_async) - wrapper which makes [Flet](https://github.com/flet-dev/flet) async and brings booth Cengal.coroutines and asyncio to Flet (Flutter based UI)
 * [justpy_containers](https://github.com/FI-Mihej/justpy_containers) - wrapper around [JustPy](https://github.com/justpy-org/justpy) in order to bring more security and more production-needed features to JustPy (VueJS based UI)
 * [Bensbach](https://github.com/FI-Mihej/Bensbach) - decompiler from Unreal Engine 3 bytecode to a Lisp-like script and compiler back to Unreal Engine 3 bytecode. Made for a game modding purposes
 * [Realistic-Damage-Model-mod-for-Long-War](https://github.com/FI-Mihej/Realistic-Damage-Model-mod-for-Long-War) - Mod for both the original XCOM:EW and the mod Long War. Was made with a Bensbach, which was made with Cengal
```

### Comparing `cengal-3.1.18.3/cengal/RequestCache.py` & `cengal-3.1.18.4/cengal/RequestCache.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/ServerClock.py` & `cengal-3.1.18.4/cengal/ServerClock.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/__init__.py` & `cengal-3.1.18.4/cengal/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/base/__init__.py` & `cengal-3.1.18.4/cengal/base/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/base/classes/__init__.py` & `cengal-3.1.18.4/cengal/base/classes/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/base/classes/versions/__init__.py` & `cengal-3.1.18.4/cengal/base/classes/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/base/classes/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/base/classes/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/base/classes/versions/v_0/classes.py` & `cengal-3.1.18.4/cengal/base/classes/versions/v_0/classes.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/base/classes/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/base/classes/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/base/classes/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/base/classes/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/base/exceptions/__init__.py` & `cengal-3.1.18.4/cengal/base/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/base/exceptions/versions/__init__.py` & `cengal-3.1.18.4/cengal/base/exceptions/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/base/exceptions/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/base/exceptions/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/base/exceptions/versions/v_0/exceptions.py` & `cengal-3.1.18.4/cengal/base/exceptions/versions/v_0/exceptions.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/base/exceptions/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/base/exceptions/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/base/exceptions/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/base/exceptions/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/build_tools/__init__.py` & `cengal-3.1.18.4/cengal/build_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/build_tools/current_compiler/__init__.py` & `cengal-3.1.18.4/cengal/build_tools/current_compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/build_tools/current_compiler/versions/__init__.py` & `cengal-3.1.18.4/cengal/build_tools/current_compiler/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/build_tools/current_compiler/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/build_tools/current_compiler/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/build_tools/current_compiler/versions/v_0/current_compiler.py` & `cengal-3.1.18.4/cengal/build_tools/current_compiler/versions/v_0/current_compiler.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/build_tools/current_compiler/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/build_tools/current_compiler/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/build_tools/current_compiler/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/build_tools/current_compiler/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/build_tools/prepare_cflags/__init__.py` & `cengal-3.1.18.4/cengal/build_tools/prepare_cflags/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/build_tools/prepare_cflags/versions/__init__.py` & `cengal-3.1.18.4/cengal/build_tools/prepare_cflags/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/build_tools/prepare_cflags/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/build_tools/prepare_cflags/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/build_tools/prepare_cflags/versions/v_0/prepare_cflags.py` & `cengal-3.1.18.4/cengal/build_tools/prepare_cflags/versions/v_0/prepare_cflags.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/build_tools/prepare_cflags/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/build_tools/prepare_cflags/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/build_tools/prepare_cflags/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/build_tools/prepare_cflags/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/bulk_pip_actions/__init__.py` & `cengal-3.1.18.4/cengal/bulk_pip_actions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/bulk_pip_actions/bulk_install.py` & `cengal-3.1.18.4/cengal/bulk_pip_actions/bulk_install.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/bulk_pip_actions/install.py` & `cengal-3.1.18.4/cengal/bulk_pip_actions/install.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/check_is_in_pycharm.py` & `cengal-3.1.18.4/cengal/check_is_in_pycharm.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/code_flow_control/__init__.py` & `cengal-3.1.18.4/cengal/code_flow_control/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/code_flow_control/args_manager/__init__.py` & `cengal-3.1.18.4/cengal/code_flow_control/args_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/code_flow_control/args_manager/versions/__init__.py` & `cengal-3.1.18.4/cengal/code_flow_control/args_manager/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/code_flow_control/args_manager/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/code_flow_control/args_manager/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/code_flow_control/args_manager/versions/v_0/args_manager.py` & `cengal-3.1.18.4/cengal/code_flow_control/args_manager/versions/v_0/args_manager.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/code_flow_control/args_manager/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/code_flow_control/args_manager/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/code_flow_control/args_manager/versions/v_0/tests/_manual_test__args_manager.py` & `cengal-3.1.18.4/cengal/code_flow_control/args_manager/versions/v_0/tests/_manual_test__args_manager.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/code_flow_control/args_manager/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/code_flow_control/args_manager/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/code_flow_control/call_history_reapplier/__init__.py` & `cengal-3.1.18.4/cengal/code_flow_control/call_history_reapplier/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/code_flow_control/call_history_reapplier/versions/__init__.py` & `cengal-3.1.18.4/cengal/code_flow_control/call_history_reapplier/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/code_flow_control/call_history_reapplier/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/code_flow_control/call_history_reapplier/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/code_flow_control/call_history_reapplier/versions/v_0/call_history_reapplier.py` & `cengal-3.1.18.4/cengal/code_flow_control/call_history_reapplier/versions/v_0/call_history_reapplier.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/code_flow_control/call_history_reapplier/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/code_flow_control/call_history_reapplier/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/code_flow_control/call_history_reapplier/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/code_flow_control/call_history_reapplier/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/code_flow_control/chained_flow/__init__.py` & `cengal-3.1.18.4/cengal/code_flow_control/chained_flow/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/code_flow_control/chained_flow/versions/__init__.py` & `cengal-3.1.18.4/cengal/code_flow_control/chained_flow/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/code_flow_control/chained_flow/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/code_flow_control/chained_flow/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/code_flow_control/chained_flow/versions/v_0/smart_chain.py` & `cengal-3.1.18.4/cengal/code_flow_control/chained_flow/versions/v_0/smart_chain.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/code_flow_control/chained_flow/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/code_flow_control/chained_flow/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/code_flow_control/chained_flow/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/code_flow_control/chained_flow/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/code_flow_control/chained_flow/versions/v_0/tests/example_for__chained_flow.py` & `cengal-3.1.18.4/cengal/code_flow_control/chained_flow/versions/v_0/tests/example_for__chained_flow.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/code_flow_control/chained_flow/versions/v_1/__init__.py` & `cengal-3.1.18.4/cengal/code_flow_control/chained_flow/versions/v_1/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/code_flow_control/chained_flow/versions/v_1/chained_flow.py` & `cengal-3.1.18.4/cengal/code_flow_control/chained_flow/versions/v_1/chained_flow.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/code_flow_control/chained_flow/versions/v_1/tests/__init__.py` & `cengal-3.1.18.4/cengal/code_flow_control/chained_flow/versions/v_1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/code_flow_control/chained_flow/versions/v_1/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/code_flow_control/chained_flow/versions/v_1/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/code_flow_control/chained_flow/versions/v_1/tests/example_for__chained_flow.py` & `cengal-3.1.18.4/cengal/code_flow_control/chained_flow/versions/v_1/tests/example_for__chained_flow.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/code_flow_control/multiinterface_essence/__init__.py` & `cengal-3.1.18.4/cengal/code_flow_control/multiinterface_essence/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/code_flow_control/multiinterface_essence/versions/__init__.py` & `cengal-3.1.18.4/cengal/code_flow_control/multiinterface_essence/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/code_flow_control/multiinterface_essence/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/code_flow_control/multiinterface_essence/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/code_flow_control/multiinterface_essence/versions/v_0/essence.py` & `cengal-3.1.18.4/cengal/code_flow_control/multiinterface_essence/versions/v_0/essence.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/quadrangle.py` & `cengal-3.1.18.4/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/quadrangle.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/quadrangle_test.py` & `cengal-3.1.18.4/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/quadrangle_test.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/square_and_rectangle.py` & `cengal-3.1.18.4/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/square_and_rectangle.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/square_and_rectangle_test.py` & `cengal-3.1.18.4/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/square_and_rectangle_test.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/square_and_rectangle_test_old.py` & `cengal-3.1.18.4/cengal/code_flow_control/multiinterface_essence/versions/v_0/tests/square_and_rectangle_test_old.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/code_flow_control/none_or/__init__.py` & `cengal-3.1.18.4/cengal/code_flow_control/none_or/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/code_flow_control/none_or/versions/__init__.py` & `cengal-3.1.18.4/cengal/code_flow_control/none_or/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/code_flow_control/none_or/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/code_flow_control/none_or/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/code_flow_control/none_or/versions/v_0/none_or.py` & `cengal-3.1.18.4/cengal/code_flow_control/none_or/versions/v_0/none_or.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/code_flow_control/none_or/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/code_flow_control/none_or/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/code_flow_control/none_or/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/code_flow_control/none_or/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/code_flow_control/python_bytecode_manipulator/__init__.py` & `cengal-3.1.18.4/cengal/code_flow_control/python_bytecode_manipulator/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/code_flow_control/python_bytecode_manipulator/versions/__init__.py` & `cengal-3.1.18.4/cengal/code_flow_control/python_bytecode_manipulator/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/code_flow_control/python_bytecode_manipulator/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/code_flow_control/python_bytecode_manipulator/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/code_flow_control/python_bytecode_manipulator/versions/v_0/python_bytecode_manipulator.py` & `cengal-3.1.18.4/cengal/code_flow_control/python_bytecode_manipulator/versions/v_0/python_bytecode_manipulator.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/code_flow_control/python_bytecode_manipulator/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/code_flow_control/python_bytecode_manipulator/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/code_flow_control/python_bytecode_manipulator/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/code_flow_control/python_bytecode_manipulator/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/code_flow_control/smart_values/__init__.py` & `cengal-3.1.18.4/cengal/code_flow_control/smart_values/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/code_flow_control/smart_values/versions/__init__.py` & `cengal-3.1.18.4/cengal/code_flow_control/smart_values/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/code_flow_control/smart_values/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/code_flow_control/smart_values/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/code_flow_control/smart_values/versions/v_0/result_types.py` & `cengal-3.1.18.4/cengal/code_flow_control/smart_values/versions/v_0/result_types.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/code_flow_control/smart_values/versions/v_1/__init__.py` & `cengal-3.1.18.4/cengal/code_flow_control/smart_values/versions/v_1/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/code_flow_control/smart_values/versions/v_1/smart_values.py` & `cengal-3.1.18.4/cengal/code_flow_control/smart_values/versions/v_1/smart_values.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/code_flow_control/smart_values/versions/v_2/__init__.py` & `cengal-3.1.18.4/cengal/code_flow_control/smart_values/versions/v_2/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/code_flow_control/smart_values/versions/v_2/smart_values.py` & `cengal-3.1.18.4/cengal/code_flow_control/smart_values/versions/v_2/smart_values.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/code_inspection/__init__.py` & `cengal-3.1.18.4/cengal/code_inspection/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/code_inspection/auto_line_tracer/__init__.py` & `cengal-3.1.18.4/cengal/code_inspection/auto_line_tracer/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/code_inspection/auto_line_tracer/versions/__init__.py` & `cengal-3.1.18.4/cengal/code_inspection/auto_line_tracer/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/code_inspection/auto_line_tracer/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/code_inspection/auto_line_tracer/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/code_inspection/auto_line_tracer/versions/v_0/auto_line_tracer.py` & `cengal-3.1.18.4/cengal/code_inspection/auto_line_tracer/versions/v_0/auto_line_tracer.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/code_inspection/auto_line_tracer/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/code_inspection/auto_line_tracer/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/code_inspection/auto_line_tracer/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/code_inspection/auto_line_tracer/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/code_inspection/line_profiling/__init__.py` & `cengal-3.1.18.4/cengal/code_inspection/line_profiling/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/code_inspection/line_profiling/versions/__init__.py` & `cengal-3.1.18.4/cengal/code_inspection/line_profiling/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/code_inspection/line_profiling/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/code_inspection/line_profiling/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/code_inspection/line_profiling/versions/v_0/line_profiling.py` & `cengal-3.1.18.4/cengal/code_inspection/line_profiling/versions/v_0/line_profiling.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/code_inspection/line_profiling/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/code_inspection/line_profiling/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/code_inspection/line_profiling/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/code_inspection/line_profiling/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/code_inspection/line_tracer/__init__.py` & `cengal-3.1.18.4/cengal/code_inspection/line_tracer/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/code_inspection/line_tracer/versions/__init__.py` & `cengal-3.1.18.4/cengal/code_inspection/line_tracer/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/code_inspection/line_tracer/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/code_inspection/line_tracer/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/code_inspection/line_tracer/versions/v_0/line_tracer.py` & `cengal-3.1.18.4/cengal/code_inspection/line_tracer/versions/v_0/line_tracer.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/code_inspection/line_tracer/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/code_inspection/line_tracer/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/code_inspection/line_tracer/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/code_inspection/line_tracer/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/cross_version/__init__.py` & `cengal-3.1.18.4/cengal/cross_version/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/cross_version/console_print/__init__.py` & `cengal-3.1.18.4/cengal/cross_version/console_print/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/cross_version/console_print/python3.py` & `cengal-3.1.18.4/cengal/cross_version/console_print/python3.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/cross_version/console_print/universal.py` & `cengal-3.1.18.4/cengal/cross_version/console_print/universal.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/ctypes_tools/__init__.py` & `cengal-3.1.18.4/cengal/ctypes_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/ctypes_tools/constants/__init__.py` & `cengal-3.1.18.4/cengal/ctypes_tools/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/ctypes_tools/constants/versions/__init__.py` & `cengal-3.1.18.4/cengal/ctypes_tools/constants/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/ctypes_tools/constants/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/ctypes_tools/constants/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/ctypes_tools/constants/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/ctypes_tools/constants/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/ctypes_tools/constants/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/ctypes_tools/constants/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/ctypes_tools/constants/versions/v_0/win_constants.py` & `cengal-3.1.18.4/cengal/ctypes_tools/constants/versions/v_0/win_constants.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/ctypes_tools/function_prototypes/__init__.py` & `cengal-3.1.18.4/cengal/ctypes_tools/function_prototypes/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/ctypes_tools/function_prototypes/versions/__init__.py` & `cengal-3.1.18.4/cengal/ctypes_tools/function_prototypes/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/ctypes_tools/function_prototypes/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/ctypes_tools/function_prototypes/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/ctypes_tools/function_prototypes/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/ctypes_tools/function_prototypes/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/ctypes_tools/function_prototypes/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/ctypes_tools/function_prototypes/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/ctypes_tools/function_prototypes/versions/v_0/win_function_prototypes.py` & `cengal-3.1.18.4/cengal/ctypes_tools/function_prototypes/versions/v_0/win_function_prototypes.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/ctypes_tools/functions/__init__.py` & `cengal-3.1.18.4/cengal/ctypes_tools/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/ctypes_tools/functions/versions/__init__.py` & `cengal-3.1.18.4/cengal/ctypes_tools/functions/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/ctypes_tools/functions/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/ctypes_tools/functions/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/ctypes_tools/functions/versions/v_0/functions.py` & `cengal-3.1.18.4/cengal/ctypes_tools/functions/versions/v_0/functions.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/ctypes_tools/functions/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/ctypes_tools/functions/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/ctypes_tools/functions/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/ctypes_tools/functions/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/ctypes_tools/functions/versions/v_0/win_functions.py` & `cengal-3.1.18.4/cengal/ctypes_tools/functions/versions/v_0/win_functions.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/ctypes_tools/libraries/__init__.py` & `cengal-3.1.18.4/cengal/ctypes_tools/libraries/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/ctypes_tools/libraries/versions/__init__.py` & `cengal-3.1.18.4/cengal/ctypes_tools/libraries/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/ctypes_tools/libraries/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/ctypes_tools/libraries/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/ctypes_tools/libraries/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/ctypes_tools/libraries/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/ctypes_tools/libraries/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/ctypes_tools/libraries/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/ctypes_tools/libraries/versions/v_0/win_libraries.py` & `cengal-3.1.18.4/cengal/ctypes_tools/libraries/versions/v_0/win_libraries.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/ctypes_tools/result_api/__init__.py` & `cengal-3.1.18.4/cengal/ctypes_tools/result_api/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/ctypes_tools/result_api/versions/__init__.py` & `cengal-3.1.18.4/cengal/ctypes_tools/result_api/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/ctypes_tools/result_api/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/ctypes_tools/result_api/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/ctypes_tools/result_api/versions/v_0/result_api.py` & `cengal-3.1.18.4/cengal/ctypes_tools/result_api/versions/v_0/result_api.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/ctypes_tools/result_api/versions/v_0/result_api_exceptions.py` & `cengal-3.1.18.4/cengal/ctypes_tools/result_api/versions/v_0/result_api_exceptions.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/ctypes_tools/result_api/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/ctypes_tools/result_api/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/ctypes_tools/result_api/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/ctypes_tools/result_api/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/ctypes_tools/result_api/versions/v_0/win_result_api.py` & `cengal-3.1.18.4/cengal/ctypes_tools/result_api/versions/v_0/win_result_api.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/ctypes_tools/tools/__init__.py` & `cengal-3.1.18.4/cengal/ctypes_tools/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/ctypes_tools/tools/versions/__init__.py` & `cengal-3.1.18.4/cengal/ctypes_tools/tools/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/ctypes_tools/tools/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/ctypes_tools/tools/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/ctypes_tools/tools/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/ctypes_tools/tools/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/ctypes_tools/tools/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/ctypes_tools/tools/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/ctypes_tools/tools/versions/v_0/tools.py` & `cengal-3.1.18.4/cengal/ctypes_tools/tools/versions/v_0/tools.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/ctypes_tools/tools/versions/v_0/win_tools.py` & `cengal-3.1.18.4/cengal/ctypes_tools/tools/versions/v_0/win_tools.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/ctypes_tools/types/__init__.py` & `cengal-3.1.18.4/cengal/ctypes_tools/types/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/ctypes_tools/types/versions/__init__.py` & `cengal-3.1.18.4/cengal/ctypes_tools/types/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/ctypes_tools/types/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/ctypes_tools/types/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/ctypes_tools/types/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/ctypes_tools/types/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/ctypes_tools/types/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/ctypes_tools/types/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/ctypes_tools/types/versions/v_0/win_types.py` & `cengal-3.1.18.4/cengal/ctypes_tools/types/versions/v_0/win_types.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/cython_tools/__init__.py` & `cengal-3.1.18.4/cengal/cython_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/cython_tools/cythonyser_setup_runner.py` & `cengal-3.1.18.4/cengal/cython_tools/cythonyser_setup_runner.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/__init__.py` & `cengal-3.1.18.4/cengal/data_containers/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/compound_dict_management/__init__.py` & `cengal-3.1.18.4/cengal/data_containers/compound_dict_management/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/compound_dict_management/manager/__init__.py` & `cengal-3.1.18.4/cengal/data_containers/compound_dict_management/manager/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/compound_dict_management/manager/versions/__init__.py` & `cengal-3.1.18.4/cengal/data_containers/compound_dict_management/manager/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/compound_dict_management/manager/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/data_containers/compound_dict_management/manager/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/compound_dict_management/manager/versions/v_0/manager.py` & `cengal-3.1.18.4/cengal/data_containers/compound_dict_management/manager/versions/v_0/manager.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/compound_dict_management/manager/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/data_containers/compound_dict_management/manager/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/compound_dict_management/manager/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/data_containers/compound_dict_management/manager/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/compound_dict_management/manager/versions/v_1/__init__.py` & `cengal-3.1.18.4/cengal/data_containers/compound_dict_management/manager/versions/v_1/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/compound_dict_management/manager/versions/v_1/manager.py` & `cengal-3.1.18.4/cengal/data_containers/compound_dict_management/manager/versions/v_1/manager.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/compound_dict_management/manager/versions/v_1/tests/__init__.py` & `cengal-3.1.18.4/cengal/data_containers/compound_dict_management/manager/versions/v_1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/compound_dict_management/manager/versions/v_1/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/data_containers/compound_dict_management/manager/versions/v_1/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/compound_dict_management/standard_library/__init__.py` & `cengal-3.1.18.4/cengal/data_containers/compound_dict_management/standard_library/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/__init__.py` & `cengal-3.1.18.4/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/versions/__init__.py` & `cengal-3.1.18.4/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/versions/v_0/key__hashable__to__value__set.py` & `cengal-3.1.18.4/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/versions/v_0/key__hashable__to__value__set.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/data_containers/compound_dict_management/standard_library/key__hashable__to__value__set/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/compound_dict_management/standard_library/key_counter/__init__.py` & `cengal-3.1.18.4/cengal/data_containers/compound_dict_management/standard_library/key_counter/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/compound_dict_management/standard_library/key_counter/versions/__init__.py` & `cengal-3.1.18.4/cengal/data_containers/compound_dict_management/standard_library/key_counter/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/compound_dict_management/standard_library/key_counter/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/data_containers/compound_dict_management/standard_library/key_counter/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/compound_dict_management/standard_library/key_counter/versions/v_0/key_counter.py` & `cengal-3.1.18.4/cengal/data_containers/compound_dict_management/standard_library/key_counter/versions/v_0/key_counter.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/compound_dict_management/standard_library/key_counter/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/data_containers/compound_dict_management/standard_library/key_counter/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/compound_dict_management/standard_library/key_counter/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/data_containers/compound_dict_management/standard_library/key_counter/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/dynamic_list_of_pieces/__init__.py` & `cengal-3.1.18.4/cengal/data_containers/dynamic_list_of_pieces/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/dynamic_list_of_pieces/versions/__init__.py` & `cengal-3.1.18.4/cengal/data_containers/dynamic_list_of_pieces/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/dynamic_list_of_pieces/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/data_containers/dynamic_list_of_pieces/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/dynamic_list_of_pieces/versions/v_0/dynamic_list_of_pieces__python.py` & `cengal-3.1.18.4/cengal/data_containers/dynamic_list_of_pieces/versions/v_0/dynamic_list_of_pieces__python.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/dynamic_list_of_pieces/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/data_containers/dynamic_list_of_pieces/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/dynamic_list_of_pieces/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/data_containers/dynamic_list_of_pieces/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/dynamic_list_of_pieces/versions/v_1/__init__.py` & `cengal-3.1.18.4/cengal/data_containers/dynamic_list_of_pieces/versions/v_1/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/dynamic_list_of_pieces/versions/v_1/dynamic_list_of_pieces__python.py` & `cengal-3.1.18.4/cengal/data_containers/dynamic_list_of_pieces/versions/v_1/dynamic_list_of_pieces__python.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/dynamic_list_of_pieces/versions/v_1/tests/__init__.py` & `cengal-3.1.18.4/cengal/data_containers/dynamic_list_of_pieces/versions/v_1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/dynamic_list_of_pieces/versions/v_1/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/data_containers/dynamic_list_of_pieces/versions/v_1/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/dynamic_tag_tree/__init__.py` & `cengal-3.1.18.4/cengal/data_containers/dynamic_tag_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/dynamic_tag_tree/versions/__init__.py` & `cengal-3.1.18.4/cengal/data_containers/dynamic_tag_tree/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/dynamic_tag_tree/versions/v_0/TagDB.py` & `cengal-3.1.18.4/cengal/data_containers/dynamic_tag_tree/versions/v_0/TagDB.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/dynamic_tag_tree/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/data_containers/dynamic_tag_tree/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/dynamic_tag_tree/versions/v_0/tag_db_interface.py` & `cengal-3.1.18.4/cengal/data_containers/dynamic_tag_tree/versions/v_0/tag_db_interface.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/dynamic_tag_tree/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/data_containers/dynamic_tag_tree/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/dynamic_tag_tree/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/data_containers/dynamic_tag_tree/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/dynamic_tag_tree/versions/v_1/TagDB.py` & `cengal-3.1.18.4/cengal/data_containers/dynamic_tag_tree/versions/v_1/TagDB.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/dynamic_tag_tree/versions/v_1/__init__.py` & `cengal-3.1.18.4/cengal/data_containers/dynamic_tag_tree/versions/v_1/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/dynamic_tag_tree/versions/v_1/tag_db_interface.py` & `cengal-3.1.18.4/cengal/data_containers/dynamic_tag_tree/versions/v_1/tag_db_interface.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/dynamic_tag_tree/versions/v_1/tests/__init__.py` & `cengal-3.1.18.4/cengal/data_containers/dynamic_tag_tree/versions/v_1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/dynamic_tag_tree/versions/v_1/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/data_containers/dynamic_tag_tree/versions/v_1/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/dynamic_tag_tree/versions/v_2/__init__.py` & `cengal-3.1.18.4/cengal/data_containers/dynamic_tag_tree/versions/v_2/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/dynamic_tag_tree/versions/v_2/dynamic_tag_tree.py` & `cengal-3.1.18.4/cengal/data_containers/dynamic_tag_tree/versions/v_2/dynamic_tag_tree.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/dynamic_tag_tree/versions/v_2/tests/__init__.py` & `cengal-3.1.18.4/cengal/data_containers/dynamic_tag_tree/versions/v_2/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/dynamic_tag_tree/versions/v_2/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/data_containers/dynamic_tag_tree/versions/v_2/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/fast_fifo/__init__.py` & `cengal-3.1.18.4/cengal/data_containers/fast_fifo/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/fast_fifo/versions/__init__.py` & `cengal-3.1.18.4/cengal/data_containers/fast_fifo/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/fast_fifo/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/data_containers/fast_fifo/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/fast_fifo/versions/v_0/fast_fifo.py` & `cengal-3.1.18.4/cengal/data_containers/fast_fifo/versions/v_0/fast_fifo.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/fast_fifo/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/data_containers/fast_fifo/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/fast_fifo/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/data_containers/fast_fifo/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/fast_fifo/versions/v_1/__init__.py` & `cengal-3.1.18.4/cengal/data_containers/fast_fifo/versions/v_1/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/fast_fifo/versions/v_1/fast_fifo.py` & `cengal-3.1.18.4/cengal/data_containers/fast_fifo/versions/v_1/fast_fifo.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/fast_fifo/versions/v_1/tests/__init__.py` & `cengal-3.1.18.4/cengal/data_containers/fast_fifo/versions/v_1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/fast_fifo/versions/v_1/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/data_containers/fast_fifo/versions/v_1/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/limitable_dict_with_order/__init__.py` & `cengal-3.1.18.4/cengal/data_containers/limitable_dict_with_order/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/limitable_dict_with_order/versions/__init__.py` & `cengal-3.1.18.4/cengal/data_containers/limitable_dict_with_order/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/limitable_dict_with_order/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/data_containers/limitable_dict_with_order/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/limitable_dict_with_order/versions/v_0/limitable_dict_with_order.py` & `cengal-3.1.18.4/cengal/data_containers/limitable_dict_with_order/versions/v_0/limitable_dict_with_order.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/limitable_dict_with_order/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/data_containers/limitable_dict_with_order/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/limitable_dict_with_order/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/data_containers/limitable_dict_with_order/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/limitable_dict_with_order/versions/v_1/__init__.py` & `cengal-3.1.18.4/cengal/data_containers/limitable_dict_with_order/versions/v_1/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/limitable_dict_with_order/versions/v_1/limitable_dict_with_order.py` & `cengal-3.1.18.4/cengal/data_containers/limitable_dict_with_order/versions/v_1/limitable_dict_with_order.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/limitable_dict_with_order/versions/v_1/tests/__init__.py` & `cengal-3.1.18.4/cengal/data_containers/limitable_dict_with_order/versions/v_1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/limitable_dict_with_order/versions/v_1/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/data_containers/limitable_dict_with_order/versions/v_1/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/simple_tree/__init__.py` & `cengal-3.1.18.4/cengal/data_containers/simple_tree/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/simple_tree/versions/__init__.py` & `cengal-3.1.18.4/cengal/data_containers/simple_tree/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/simple_tree/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/data_containers/simple_tree/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/simple_tree/versions/v_0/simple_tree.py` & `cengal-3.1.18.4/cengal/data_containers/simple_tree/versions/v_0/simple_tree.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/stack/__init__.py` & `cengal-3.1.18.4/cengal/data_containers/stack/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/stack/versions/__init__.py` & `cengal-3.1.18.4/cengal/data_containers/stack/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/stack/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/data_containers/stack/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/stack/versions/v_0/stack.py` & `cengal-3.1.18.4/cengal/data_containers/stack/versions/v_0/stack.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/stack/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/data_containers/stack/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_containers/stack/versions/v_0/tests/test__stack.py` & `cengal-3.1.18.4/cengal/data_containers/stack/versions/v_0/tests/test__stack.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_generation/__init__.py` & `cengal-3.1.18.4/cengal/data_generation/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_generation/id_generator/__init__.py` & `cengal-3.1.18.4/cengal/data_generation/id_generator/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_generation/id_generator/versions/__init__.py` & `cengal-3.1.18.4/cengal/data_generation/id_generator/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_generation/id_generator/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/data_generation/id_generator/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_generation/id_generator/versions/v_0/id_generator.py` & `cengal-3.1.18.4/cengal/data_generation/id_generator/versions/v_0/id_generator.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_generation/id_generator/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/data_generation/id_generator/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_generation/id_generator/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/data_generation/id_generator/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_generation/id_generator/versions/v_1/__init__.py` & `cengal-3.1.18.4/cengal/data_generation/id_generator/versions/v_1/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_generation/id_generator/versions/v_1/id_generator.py` & `cengal-3.1.18.4/cengal/data_generation/id_generator/versions/v_1/id_generator.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_generation/id_generator/versions/v_1/tests/__init__.py` & `cengal-3.1.18.4/cengal/data_generation/id_generator/versions/v_1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_generation/id_generator/versions/v_1/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/data_generation/id_generator/versions/v_1/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/__init__.py` & `cengal-3.1.18.4/cengal/data_manipulation/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/conversion/__init__.py` & `cengal-3.1.18.4/cengal/data_manipulation/conversion/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/conversion/bit_cast_like/__init__.py` & `cengal-3.1.18.4/cengal/data_manipulation/conversion/bit_cast_like/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/conversion/bit_cast_like/versions/__init__.py` & `cengal-3.1.18.4/cengal/data_manipulation/conversion/bit_cast_like/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/conversion/bit_cast_like/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/data_manipulation/conversion/bit_cast_like/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/conversion/bit_cast_like/versions/v_0/bit_cast_like.py` & `cengal-3.1.18.4/cengal/data_manipulation/conversion/bit_cast_like/versions/v_0/bit_cast_like.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/conversion/bit_cast_like/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/data_manipulation/conversion/bit_cast_like/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/conversion/bit_cast_like/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/data_manipulation/conversion/bit_cast_like/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast/__init__.py` & `cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast/versions/__init__.py` & `cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast/versions/v_0/reinterpret_cast.py` & `cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast/versions/v_0/reinterpret_cast.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast_management/__init__.py` & `cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast_management/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/__init__.py` & `cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/versions/__init__.py` & `cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/versions/v_0/manager.py` & `cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/versions/v_0/manager.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast_management/manager/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/__init__.py` & `cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/__init__.py` & `cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/versions/__init__.py` & `cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/versions/v_0/copy_wrapper.py` & `cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/versions/v_0/copy_wrapper.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/copy_wrapper/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/__init__.py` & `cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/versions/__init__.py` & `cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/versions/v_0/deep_copy_wrapper.py` & `cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/versions/v_0/deep_copy_wrapper.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/deep_copy_wrapper/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/__init__.py` & `cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/versions/__init__.py` & `cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/versions/v_0/uni_copy_wrapper.py` & `cengal-3.1.18.4/cengal/data_manipulation/conversion/reinterpret_cast_management/standard_library/uni_copy_wrapper/versions/v_0/uni_copy_wrapper.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/front_triggerable_variable/__init__.py` & `cengal-3.1.18.4/cengal/data_manipulation/front_triggerable_variable/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/front_triggerable_variable/versions/__init__.py` & `cengal-3.1.18.4/cengal/data_manipulation/front_triggerable_variable/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/front_triggerable_variable/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/data_manipulation/front_triggerable_variable/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/front_triggerable_variable/versions/v_0/front_triggerable_variable.py` & `cengal-3.1.18.4/cengal/data_manipulation/front_triggerable_variable/versions/v_0/front_triggerable_variable.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/front_triggerable_variable/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/data_manipulation/front_triggerable_variable/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/front_triggerable_variable/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/data_manipulation/front_triggerable_variable/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/get_dict_key_with_callable_default/__init__.py` & `cengal-3.1.18.4/cengal/data_manipulation/get_dict_key_with_callable_default/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/get_dict_key_with_callable_default/versions/__init__.py` & `cengal-3.1.18.4/cengal/data_manipulation/get_dict_key_with_callable_default/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/get_dict_key_with_callable_default/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/data_manipulation/get_dict_key_with_callable_default/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/get_dict_key_with_callable_default/versions/v_0/get_dict_key_with_callable_default.py` & `cengal-3.1.18.4/cengal/data_manipulation/get_dict_key_with_callable_default/versions/v_0/get_dict_key_with_callable_default.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/get_dict_key_with_callable_default/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/data_manipulation/get_dict_key_with_callable_default/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/get_dict_key_with_callable_default/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/data_manipulation/get_dict_key_with_callable_default/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/help_tools.py` & `cengal-3.1.18.4/cengal/data_manipulation/help_tools.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/objects_counter/__init__.py` & `cengal-3.1.18.4/cengal/data_manipulation/objects_counter/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/objects_counter/versions/__init__.py` & `cengal-3.1.18.4/cengal/data_manipulation/objects_counter/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/objects_counter/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/data_manipulation/objects_counter/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/objects_counter/versions/v_0/objects_counter.py` & `cengal-3.1.18.4/cengal/data_manipulation/objects_counter/versions/v_0/objects_counter.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/objects_counter/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/data_manipulation/objects_counter/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/objects_counter/versions/v_0/tests/test__objects_counter.py` & `cengal-3.1.18.4/cengal/data_manipulation/objects_counter/versions/v_0/tests/test__objects_counter.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/performant_list_operations/__init__.py` & `cengal-3.1.18.4/cengal/data_manipulation/performant_list_operations/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/performant_list_operations/versions/__init__.py` & `cengal-3.1.18.4/cengal/data_manipulation/performant_list_operations/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/performant_list_operations/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/data_manipulation/performant_list_operations/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/performant_list_operations/versions/v_0/remove_items_from_list.py` & `cengal-3.1.18.4/cengal/data_manipulation/performant_list_operations/versions/v_0/remove_items_from_list.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/performant_list_operations/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/data_manipulation/performant_list_operations/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/performant_list_operations/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/data_manipulation/performant_list_operations/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/serialization/__init__.py` & `cengal-3.1.18.4/cengal/data_manipulation/serialization/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/serialization/versions/__init__.py` & `cengal-3.1.18.4/cengal/data_manipulation/serialization/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/serialization/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/data_manipulation/serialization/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/serialization/versions/v_0/serialization.py` & `cengal-3.1.18.4/cengal/data_manipulation/serialization/versions/v_0/serialization.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/serialization/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/data_manipulation/serialization/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/serialization/versions/v_0/tests/test__serialization.py` & `cengal-3.1.18.4/cengal/data_manipulation/serialization/versions/v_0/tests/test__serialization.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/tree_traversal/__init__.py` & `cengal-3.1.18.4/cengal/data_manipulation/tree_traversal/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/tree_traversal/versions/__init__.py` & `cengal-3.1.18.4/cengal/data_manipulation/tree_traversal/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/tree_traversal/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/data_manipulation/tree_traversal/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/tree_traversal/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/data_manipulation/tree_traversal/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/tree_traversal/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/data_manipulation/tree_traversal/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/tree_traversal/versions/v_0/tests/traverstal_manual_tests.py` & `cengal-3.1.18.4/cengal/data_manipulation/tree_traversal/versions/v_0/tests/traverstal_manual_tests.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/tree_traversal/versions/v_0/tree_traversal.py` & `cengal-3.1.18.4/cengal/data_manipulation/tree_traversal/versions/v_0/tree_traversal.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/tree_traversal/versions/v_1/__init__.py` & `cengal-3.1.18.4/cengal/data_manipulation/tree_traversal/versions/v_1/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/tree_traversal/versions/v_1/tests/__init__.py` & `cengal-3.1.18.4/cengal/data_manipulation/tree_traversal/versions/v_1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/tree_traversal/versions/v_1/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/data_manipulation/tree_traversal/versions/v_1/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/tree_traversal/versions/v_1/tests/key_multi_value_traverstal_manual_tests.py` & `cengal-3.1.18.4/cengal/data_manipulation/tree_traversal/versions/v_1/tests/key_multi_value_traverstal_manual_tests.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/tree_traversal/versions/v_1/tests/key_value_traverstal_manual_tests.py` & `cengal-3.1.18.4/cengal/data_manipulation/tree_traversal/versions/v_1/tests/key_value_traverstal_manual_tests.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/tree_traversal/versions/v_1/tests/traverstal_manual_tests.py` & `cengal-3.1.18.4/cengal/data_manipulation/tree_traversal/versions/v_1/tests/traverstal_manual_tests.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/data_manipulation/tree_traversal/versions/v_1/tree_traversal.py` & `cengal-3.1.18.4/cengal/data_manipulation/tree_traversal/versions/v_1/tree_traversal.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/docten.py` & `cengal-3.1.18.4/cengal/docten.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/entities/__init__.py` & `cengal-3.1.18.4/cengal/entities/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/entities/bindable_to_type/__init__.py` & `cengal-3.1.18.4/cengal/entities/bindable_to_type/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/entities/bindable_to_type/versions/__init__.py` & `cengal-3.1.18.4/cengal/entities/bindable_to_type/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/entities/bindable_to_type/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/entities/bindable_to_type/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/entities/bindable_to_type/versions/v_0/bindable_to_type.py` & `cengal-3.1.18.4/cengal/entities/bindable_to_type/versions/v_0/bindable_to_type.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/entities/bindable_to_type/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/entities/bindable_to_type/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/entities/bindable_to_type/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/entities/bindable_to_type/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/entities/copyable/__init__.py` & `cengal-3.1.18.4/cengal/entities/copyable/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/entities/copyable/versions/__init__.py` & `cengal-3.1.18.4/cengal/entities/copyable/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/entities/copyable/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/entities/copyable/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/entities/copyable/versions/v_0/copyable.py` & `cengal-3.1.18.4/cengal/entities/copyable/versions/v_0/copyable.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/entities/copyable/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/entities/copyable/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/entities/copyable/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/entities/copyable/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/file_settings_manager/__init__.py` & `cengal-3.1.18.4/cengal/file_settings_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/file_settings_manager/config_manager.py` & `cengal-3.1.18.4/cengal/file_settings_manager/config_manager.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/file_settings_manager/dir_templates.py` & `cengal-3.1.18.4/cengal/file_settings_manager/dir_templates.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/file_system/__init__.py` & `cengal-3.1.18.4/cengal/file_system/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/file_system/app_fs_structure/__init__.py` & `cengal-3.1.18.4/cengal/file_system/app_fs_structure/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/file_system/app_fs_structure/app_dir_path/__init__.py` & `cengal-3.1.18.4/cengal/file_system/app_fs_structure/app_dir_path/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/file_system/app_fs_structure/app_dir_path/versions/__init__.py` & `cengal-3.1.18.4/cengal/file_system/app_fs_structure/app_dir_path/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/app_dir_exceptions.py` & `cengal-3.1.18.4/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/app_dir_exceptions.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/app_dir_path_base.py` & `cengal-3.1.18.4/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/app_dir_path_base.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/app_dir_path_darwin.py` & `cengal-3.1.18.4/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/app_dir_path_darwin.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/app_dir_path_linux.py` & `cengal-3.1.18.4/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/app_dir_path_linux.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/app_dir_path_win.py` & `cengal-3.1.18.4/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/app_dir_path_win.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/app_directory_types.py` & `cengal-3.1.18.4/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/app_directory_types.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/file_system/app_fs_structure/app_dir_path/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/file_system/directory_manager.py` & `cengal-3.1.18.4/cengal/file_system/directory_manager.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/file_system/file_manager.py` & `cengal-3.1.18.4/cengal/file_system/file_manager.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/file_system/file_patch/__init__.py` & `cengal-3.1.18.4/cengal/file_system/file_patch/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/file_system/file_patch/brackets/__init__.py` & `cengal-3.1.18.4/cengal/file_system/file_patch/brackets/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/file_system/file_patch/brackets/versions/__init__.py` & `cengal-3.1.18.4/cengal/file_system/file_patch/brackets/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/file_system/file_patch/brackets/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/file_system/file_patch/brackets/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/file_system/file_patch/brackets/versions/v_0/brackets.py` & `cengal-3.1.18.4/cengal/file_system/file_patch/brackets/versions/v_0/brackets.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/file_system/file_patch/brackets/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/file_system/file_patch/brackets/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/file_system/file_patch/brackets/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/file_system/file_patch/brackets/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/file_system/file_patch/generic/__init__.py` & `cengal-3.1.18.4/cengal/file_system/file_patch/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/file_system/file_patch/generic/versions/__init__.py` & `cengal-3.1.18.4/cengal/file_system/file_patch/generic/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/file_system/file_patch/generic/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/file_system/file_patch/generic/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/file_system/file_patch/generic/versions/v_0/generic.py` & `cengal-3.1.18.4/cengal/file_system/file_patch/generic/versions/v_0/generic.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/file_system/file_patch/generic/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/file_system/file_patch/generic/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/file_system/file_patch/generic/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/file_system/file_patch/generic/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/file_system/file_patch/simple/__init__.py` & `cengal-3.1.18.4/cengal/file_system/file_patch/simple/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/file_system/file_patch/simple/versions/__init__.py` & `cengal-3.1.18.4/cengal/file_system/file_patch/simple/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/file_system/file_patch/simple/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/file_system/file_patch/simple/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/file_system/file_patch/simple/versions/v_0/simple.py` & `cengal-3.1.18.4/cengal/file_system/file_patch/simple/versions/v_0/simple.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/file_system/file_patch/simple/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/file_system/file_patch/simple/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/file_system/file_patch/simple/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/file_system/file_patch/simple/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/file_system/path_manager/__init__.py` & `cengal-3.1.18.4/cengal/file_system/path_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/file_system/path_manager/versions/__init__.py` & `cengal-3.1.18.4/cengal/file_system/path_manager/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/file_system/path_manager/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/file_system/path_manager/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/file_system/path_manager/versions/v_0/path_manager.py` & `cengal-3.1.18.4/cengal/file_system/path_manager/versions/v_0/path_manager.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/file_system/path_manager/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/file_system/path_manager/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/file_system/path_manager/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/file_system/path_manager/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/file_system/win_fs/__init__.py` & `cengal-3.1.18.4/cengal/file_system/win_fs/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/file_system/win_fs/base.py` & `cengal-3.1.18.4/cengal/file_system/win_fs/base.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/file_system/win_fs/global_install_uninstall.py` & `cengal-3.1.18.4/cengal/file_system/win_fs/global_install_uninstall.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/file_system/win_fs/path.py` & `cengal-3.1.18.4/cengal/file_system/win_fs/path.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/file_system/win_fs/shutil.py` & `cengal-3.1.18.4/cengal/file_system/win_fs/shutil.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/file_system/win_fs/shutil_readable.py` & `cengal-3.1.18.4/cengal/file_system/win_fs/shutil_readable.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/hardware/__init__.py` & `cengal-3.1.18.4/cengal/hardware/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/hardware/info/__init__.py` & `cengal-3.1.18.4/cengal/hardware/info/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/hardware/info/cpu/__init__.py` & `cengal-3.1.18.4/cengal/hardware/info/cpu/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/hardware/info/cpu/versions/__init__.py` & `cengal-3.1.18.4/cengal/hardware/info/cpu/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/hardware/info/cpu/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/hardware/info/cpu/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/hardware/info/cpu/versions/v_0/cpu.py` & `cengal-3.1.18.4/cengal/hardware/info/cpu/versions/v_0/cpu.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/hardware/info/cpu/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/hardware/info/cpu/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/hardware/info/cpu/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/hardware/info/cpu/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/hardware/info/cpu/versions/v_1/__init__.py` & `cengal-3.1.18.4/cengal/hardware/info/cpu/versions/v_1/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/hardware/info/cpu/versions/v_1/cpu.py` & `cengal-3.1.18.4/cengal/hardware/info/cpu/versions/v_1/cpu.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/hardware/info/cpu/versions/v_1/tests/__init__.py` & `cengal-3.1.18.4/cengal/hardware/info/cpu/versions/v_1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/hardware/info/cpu/versions/v_1/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/hardware/info/cpu/versions/v_1/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/hardware/memory/__init__.py` & `cengal-3.1.18.4/cengal/hardware/memory/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/hardware/memory/barriers/__init__.py` & `cengal-3.1.18.4/cengal/hardware/memory/barriers/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/hardware/memory/barriers/versions/__init__.py` & `cengal-3.1.18.4/cengal/hardware/memory/barriers/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/hardware/memory/barriers/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/hardware/memory/barriers/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/hardware/memory/barriers/versions/v_0/compilable/__build_config.py` & `cengal-3.1.18.4/cengal/hardware/memory/barriers/versions/v_0/compilable/__build_config.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/hardware/memory/barriers/versions/v_0/compilable/__init__.py` & `cengal-3.1.18.4/cengal/hardware/memory/barriers/versions/v_0/compilable/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/hardware/memory/barriers/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/hardware/memory/barriers/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/hardware/memory/barriers/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/hardware/memory/barriers/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/hardware/memory/shared_memory/__init__.py` & `cengal-3.1.18.4/cengal/hardware/memory/shared_memory/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/hardware/memory/shared_memory/versions/__init__.py` & `cengal-3.1.18.4/cengal/hardware/memory/shared_memory/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/hardware/memory/shared_memory/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/hardware/memory/shared_memory/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/hardware/memory/shared_memory/versions/v_0/compilable/__build_config.py` & `cengal-3.1.18.4/cengal/hardware/memory/shared_memory/versions/v_0/compilable/__build_config.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/hardware/memory/shared_memory/versions/v_0/compilable/__init__.py` & `cengal-3.1.18.4/cengal/hardware/memory/shared_memory/versions/v_0/compilable/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/hardware/memory/shared_memory/versions/v_0/interfaces.py` & `cengal-3.1.18.4/cengal/hardware/memory/shared_memory/versions/v_0/interfaces.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/hardware/memory/shared_memory/versions/v_0/shared_memory.py` & `cengal-3.1.18.4/cengal/hardware/memory/shared_memory/versions/v_0/shared_memory.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/hardware/memory/shared_memory/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/hardware/memory/shared_memory/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/hardware/memory/shared_memory/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/hardware/memory/shared_memory/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/help_tools.py` & `cengal-3.1.18.4/cengal/help_tools.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/introspection/__init__.py` & `cengal-3.1.18.4/cengal/introspection/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/introspection/inspect/__init__.py` & `cengal-3.1.18.4/cengal/introspection/inspect/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/introspection/inspect/versions/__init__.py` & `cengal-3.1.18.4/cengal/introspection/inspect/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/introspection/inspect/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/introspection/inspect/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/introspection/inspect/versions/v_0/inspect.py` & `cengal-3.1.18.4/cengal/introspection/inspect/versions/v_0/inspect.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/introspection/inspect/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/introspection/inspect/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/introspection/inspect/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/introspection/inspect/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/introspection/third_party/__init__.py` & `cengal-3.1.18.4/cengal/introspection/third_party/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/introspection/third_party/ctypes/__init__.py` & `cengal-3.1.18.4/cengal/introspection/third_party/ctypes/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/introspection/third_party/ctypes/versions/__init__.py` & `cengal-3.1.18.4/cengal/introspection/third_party/ctypes/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/introspection/third_party/ctypes/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/introspection/third_party/ctypes/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/introspection/third_party/ctypes/versions/v_0/ctypes.py` & `cengal-3.1.18.4/cengal/introspection/third_party/ctypes/versions/v_0/ctypes.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/introspection/third_party/ctypes/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/introspection/third_party/ctypes/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/introspection/third_party/ctypes/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/introspection/third_party/ctypes/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/__init__.py` & `cengal-3.1.18.4/cengal/io/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/asock_io/__init__.py` & `cengal-3.1.18.4/cengal/io/asock_io/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/asock_io/versions/__init__.py` & `cengal-3.1.18.4/cengal/io/asock_io/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/asock_io/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/io/asock_io/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/asock_io/versions/v_0/base.py` & `cengal-3.1.18.4/cengal/io/asock_io/versions/v_0/base.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/asock_io/versions/v_0/recv_buff_size_computer/__init__.py` & `cengal-3.1.18.4/cengal/io/asock_io/versions/v_0/recv_buff_size_computer/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/asock_io/versions/v_0/recv_buff_size_computer/recv_buff_size_computer__python.py` & `cengal-3.1.18.4/cengal/io/asock_io/versions/v_0/recv_buff_size_computer/recv_buff_size_computer__python.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/asock_io/versions/v_0/tcp_app_server.py` & `cengal-3.1.18.4/cengal/io/asock_io/versions/v_0/tcp_app_server.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/asock_io/versions/v_0/tcp_link.py` & `cengal-3.1.18.4/cengal/io/asock_io/versions/v_0/tcp_link.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/asock_io/versions/v_1/__init__.py` & `cengal-3.1.18.4/cengal/io/asock_io/versions/v_1/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/asock_io/versions/v_1/abstract.py` & `cengal-3.1.18.4/cengal/io/asock_io/versions/v_1/abstract.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/asock_io/versions/v_1/asock_io_core.py` & `cengal-3.1.18.4/cengal/io/asock_io/versions/v_1/asock_io_core.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/asock_io/versions/v_1/base.py` & `cengal-3.1.18.4/cengal/io/asock_io/versions/v_1/base.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/asock_io/versions/v_1/io_loops/__init__.py` & `cengal-3.1.18.4/cengal/io/asock_io/versions/v_1/io_loops/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/asock_io/versions/v_1/io_loops/epoll_lt.py` & `cengal-3.1.18.4/cengal/io/asock_io/versions/v_1/io_loops/epoll_lt.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/asock_io/versions/v_1/io_loops/select.py` & `cengal-3.1.18.4/cengal/io/asock_io/versions/v_1/io_loops/select.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/asock_io/versions/v_1/recv_buff_size_computer/__init__.py` & `cengal-3.1.18.4/cengal/io/asock_io/versions/v_1/recv_buff_size_computer/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/asock_io/versions/v_1/recv_buff_size_computer/recv_buff_size_computer__python.py` & `cengal-3.1.18.4/cengal/io/asock_io/versions/v_1/recv_buff_size_computer/recv_buff_size_computer__python.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/asock_io/versions/v_1/tcp_link.py` & `cengal-3.1.18.4/cengal/io/asock_io/versions/v_1/tcp_link.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/core/__init__.py` & `cengal-3.1.18.4/cengal/io/core/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/core/memory_management/__init__.py` & `cengal-3.1.18.4/cengal/io/core/memory_management/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/core/memory_management/versions/__init__.py` & `cengal-3.1.18.4/cengal/io/core/memory_management/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/core/memory_management/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/io/core/memory_management/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/core/memory_management/versions/v_0/memory_management.py` & `cengal-3.1.18.4/cengal/io/core/memory_management/versions/v_0/memory_management.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/core/memory_management/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/io/core/memory_management/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/core/memory_management/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/io/core/memory_management/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/named_connections/__init__.py` & `cengal-3.1.18.4/cengal/io/named_connections/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/named_connections/named_connections_manager/__init__.py` & `cengal-3.1.18.4/cengal/io/named_connections/named_connections_manager/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/named_connections/named_connections_manager/versions/__init__.py` & `cengal-3.1.18.4/cengal/io/named_connections/named_connections_manager/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/named_connections/named_connections_manager/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/io/named_connections/named_connections_manager/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/named_connections/named_connections_manager/versions/v_0/named_connections_manager.py` & `cengal-3.1.18.4/cengal/io/named_connections/named_connections_manager/versions/v_0/named_connections_manager.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/named_connections/named_connections_manager/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/io/named_connections/named_connections_manager/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/named_connections/named_connections_manager/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/io/named_connections/named_connections_manager/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/named_connections/workers/__init__.py` & `cengal-3.1.18.4/cengal/io/named_connections/workers/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/named_connections/workers/asyncio_streams/__init__.py` & `cengal-3.1.18.4/cengal/io/named_connections/workers/asyncio_streams/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/named_connections/workers/asyncio_streams/versions/__init__.py` & `cengal-3.1.18.4/cengal/io/named_connections/workers/asyncio_streams/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/named_connections/workers/asyncio_streams/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/io/named_connections/workers/asyncio_streams/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/named_connections/workers/asyncio_streams/versions/v_0/asyncio_streams.py` & `cengal-3.1.18.4/cengal/io/named_connections/workers/asyncio_streams/versions/v_0/asyncio_streams.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/named_connections/workers/asyncio_streams/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/io/named_connections/workers/asyncio_streams/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/named_connections/workers/asyncio_streams/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/io/named_connections/workers/asyncio_streams/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/named_connections/workers/asyncio_streams_proxy/__init__.py` & `cengal-3.1.18.4/cengal/io/named_connections/workers/asyncio_streams_proxy/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/named_connections/workers/asyncio_streams_proxy/versions/__init__.py` & `cengal-3.1.18.4/cengal/io/named_connections/workers/asyncio_streams_proxy/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/named_connections/workers/asyncio_streams_proxy/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/io/named_connections/workers/asyncio_streams_proxy/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/named_connections/workers/asyncio_streams_proxy/versions/v_0/asyncio_streams_proxy.py` & `cengal-3.1.18.4/cengal/io/named_connections/workers/asyncio_streams_proxy/versions/v_0/asyncio_streams_proxy.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/named_connections/workers/asyncio_streams_proxy/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/io/named_connections/workers/asyncio_streams_proxy/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/named_connections/workers/asyncio_streams_proxy/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/io/named_connections/workers/asyncio_streams_proxy/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/net_io/__init__.py` & `cengal-3.1.18.4/cengal/io/net_io/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/net_io/versions/__init__.py` & `cengal-3.1.18.4/cengal/io/net_io/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/net_io/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/io/net_io/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/net_io/versions/v_0/crossplatform/__init__.py` & `cengal-3.1.18.4/cengal/io/net_io/versions/v_0/crossplatform/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/net_io/versions/v_0/crossplatform/exceptions_handlers/__init__.py` & `cengal-3.1.18.4/cengal/io/net_io/versions/v_0/crossplatform/exceptions_handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/net_io/versions/v_0/crossplatform/exceptions_handlers/abstract.py` & `cengal-3.1.18.4/cengal/io/net_io/versions/v_0/crossplatform/exceptions_handlers/abstract.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/net_io/versions/v_0/crossplatform/exceptions_handlers/linux.py` & `cengal-3.1.18.4/cengal/io/net_io/versions/v_0/crossplatform/exceptions_handlers/linux.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/net_io/versions/v_0/crossplatform/exceptions_handlers/win32.py` & `cengal-3.1.18.4/cengal/io/net_io/versions/v_0/crossplatform/exceptions_handlers/win32.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/net_io/versions/v_0/net_io__linux.py` & `cengal-3.1.18.4/cengal/io/net_io/versions/v_0/net_io__linux.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/net_io/versions/v_0/net_io_abstract.py` & `cengal-3.1.18.4/cengal/io/net_io/versions/v_0/net_io_abstract.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/net_io/versions/v_0/net_io_method__epoll_lt.py` & `cengal-3.1.18.4/cengal/io/net_io/versions/v_0/net_io_method__epoll_lt.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/net_io/versions/v_0/net_io_method__select.py` & `cengal-3.1.18.4/cengal/io/net_io/versions/v_0/net_io_method__select.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/recv_buff_size_computer/__init__.py` & `cengal-3.1.18.4/cengal/io/recv_buff_size_computer/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/recv_buff_size_computer/versions/__init__.py` & `cengal-3.1.18.4/cengal/io/recv_buff_size_computer/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/recv_buff_size_computer/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/io/recv_buff_size_computer/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/recv_buff_size_computer/versions/v_0/recv_buff_size_computer__python.py` & `cengal-3.1.18.4/cengal/io/recv_buff_size_computer/versions/v_0/recv_buff_size_computer__python.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/recv_buff_size_computer/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/io/recv_buff_size_computer/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/recv_buff_size_computer/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/io/recv_buff_size_computer/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/recv_buff_size_computer/versions/v_1/__init__.py` & `cengal-3.1.18.4/cengal/io/recv_buff_size_computer/versions/v_1/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/recv_buff_size_computer/versions/v_1/recv_buff_size_computer__python.py` & `cengal-3.1.18.4/cengal/io/recv_buff_size_computer/versions/v_1/recv_buff_size_computer__python.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/recv_buff_size_computer/versions/v_1/tests/__init__.py` & `cengal-3.1.18.4/cengal/io/recv_buff_size_computer/versions/v_1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/recv_buff_size_computer/versions/v_1/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/io/recv_buff_size_computer/versions/v_1/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/serve_free_ports/__init__.py` & `cengal-3.1.18.4/cengal/io/serve_free_ports/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/serve_free_ports/versions/__init__.py` & `cengal-3.1.18.4/cengal/io/serve_free_ports/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/serve_free_ports/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/io/serve_free_ports/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/serve_free_ports/versions/v_0/serve_free_ports.py` & `cengal-3.1.18.4/cengal/io/serve_free_ports/versions/v_0/serve_free_ports.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/serve_free_ports/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/io/serve_free_ports/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/serve_free_ports/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/io/serve_free_ports/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/socket/__init__.py` & `cengal-3.1.18.4/cengal/io/socket/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/socket/constants/__init__.py` & `cengal-3.1.18.4/cengal/io/socket/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/socket/constants/versions/__init__.py` & `cengal-3.1.18.4/cengal/io/socket/constants/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/socket/constants/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/io/socket/constants/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/socket/constants/versions/v_0/constants.py` & `cengal-3.1.18.4/cengal/io/socket/constants/versions/v_0/constants.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/socket/constants/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/io/socket/constants/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/socket/constants/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/io/socket/constants/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/socket/errors/__init__.py` & `cengal-3.1.18.4/cengal/io/socket/errors/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/socket/errors/versions/__init__.py` & `cengal-3.1.18.4/cengal/io/socket/errors/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/socket/errors/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/io/socket/errors/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/socket/errors/versions/v_0/errors.py` & `cengal-3.1.18.4/cengal/io/socket/errors/versions/v_0/errors.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/socket/errors/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/io/socket/errors/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/socket/errors/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/io/socket/errors/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/used_ports/__init__.py` & `cengal-3.1.18.4/cengal/io/used_ports/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/used_ports/versions/__init__.py` & `cengal-3.1.18.4/cengal/io/used_ports/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/used_ports/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/io/used_ports/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/used_ports/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/io/used_ports/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/used_ports/versions/v_0/tests/_test__used_ports.py` & `cengal-3.1.18.4/cengal/io/used_ports/versions/v_0/tests/_test__used_ports.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/io/used_ports/versions/v_0/used_ports.py` & `cengal-3.1.18.4/cengal/io/used_ports/versions/v_0/used_ports.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/math/__init__.py` & `cengal-3.1.18.4/cengal/math/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/math/algebra/__init__.py` & `cengal-3.1.18.4/cengal/math/algebra/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/math/algebra/fast_algorithms/__init__.py` & `cengal-3.1.18.4/cengal/math/algebra/fast_algorithms/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/math/algebra/fast_algorithms/versions/__init__.py` & `cengal-3.1.18.4/cengal/math/algebra/fast_algorithms/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/math/algebra/fast_algorithms/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/math/algebra/fast_algorithms/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/math/algebra/fast_algorithms/versions/v_0/fast_algorithms.py` & `cengal-3.1.18.4/cengal/math/algebra/fast_algorithms/versions/v_0/fast_algorithms.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/math/algebra/fast_algorithms/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/math/algebra/fast_algorithms/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/math/algebra/fast_algorithms/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/math/algebra/fast_algorithms/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/math/geometry/__init__.py` & `cengal-3.1.18.4/cengal/math/geometry/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/math/geometry/ellipse/__init__.py` & `cengal-3.1.18.4/cengal/math/geometry/ellipse/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/math/geometry/ellipse/versions/__init__.py` & `cengal-3.1.18.4/cengal/math/geometry/ellipse/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/math/geometry/ellipse/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/math/geometry/ellipse/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/math/geometry/ellipse/versions/v_0/ellipse.py` & `cengal-3.1.18.4/cengal/math/geometry/ellipse/versions/v_0/ellipse.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/math/geometry/ellipse/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/math/geometry/ellipse/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/math/geometry/ellipse/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/math/geometry/ellipse/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/math/geometry/ellipse/versions/v_0/tests/informal_tests.py` & `cengal-3.1.18.4/cengal/math/geometry/ellipse/versions/v_0/tests/informal_tests.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/math/geometry/point/__init__.py` & `cengal-3.1.18.4/cengal/math/geometry/point/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/math/geometry/point/versions/__init__.py` & `cengal-3.1.18.4/cengal/math/geometry/point/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/math/geometry/point/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/math/geometry/point/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/math/geometry/point/versions/v_0/point.py` & `cengal-3.1.18.4/cengal/math/geometry/point/versions/v_0/point.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/math/geometry/point/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/math/geometry/point/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/math/geometry/point/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/math/geometry/point/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/math/geometry/vector/__init__.py` & `cengal-3.1.18.4/cengal/math/geometry/vector/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/math/geometry/vector/versions/__init__.py` & `cengal-3.1.18.4/cengal/math/geometry/vector/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/math/geometry/vector/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/math/geometry/vector/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/math/geometry/vector/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/math/geometry/vector/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/math/geometry/vector/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/math/geometry/vector/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/math/geometry/vector/versions/v_0/vector.py` & `cengal-3.1.18.4/cengal/math/geometry/vector/versions/v_0/vector.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/math/numbers/__init__.py` & `cengal-3.1.18.4/cengal/math/numbers/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/math/numbers/versions/__init__.py` & `cengal-3.1.18.4/cengal/math/numbers/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/math/numbers/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/math/numbers/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/math/numbers/versions/v_0/numbers.py` & `cengal-3.1.18.4/cengal/math/numbers/versions/v_0/numbers.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/math/numbers/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/math/numbers/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/math/numbers/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/math/numbers/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/modules_management/__init__.py` & `cengal-3.1.18.4/cengal/modules_management/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/modules_management/alternative_import.py` & `cengal-3.1.18.4/cengal/modules_management/alternative_import.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/modules_management/ignore_in_build_mode/__init__.py` & `cengal-3.1.18.4/cengal/modules_management/ignore_in_build_mode/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/modules_management/ignore_in_build_mode/versions/__init__.py` & `cengal-3.1.18.4/cengal/modules_management/ignore_in_build_mode/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/modules_management/ignore_in_build_mode/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/modules_management/ignore_in_build_mode/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/modules_management/ignore_in_build_mode/versions/v_0/ignore_in_build_mode.py` & `cengal-3.1.18.4/cengal/modules_management/ignore_in_build_mode/versions/v_0/ignore_in_build_mode.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/modules_management/ignore_in_build_mode/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/modules_management/ignore_in_build_mode/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/modules_management/ignore_in_build_mode/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/modules_management/ignore_in_build_mode/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/modules_management/reload_module.py` & `cengal-3.1.18.4/cengal/modules_management/reload_module.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/os/__init__.py` & `cengal-3.1.18.4/cengal/os/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/os/help_tools.py` & `cengal-3.1.18.4/cengal/os/help_tools.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/asyncio/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/asyncio/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/asyncio/atasks/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/asyncio/atasks/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/asyncio/atasks/versions/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/asyncio/atasks/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/asyncio/atasks/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/asyncio/atasks/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/asyncio/atasks/versions/v_0/atasks.py` & `cengal-3.1.18.4/cengal/parallel_execution/asyncio/atasks/versions/v_0/atasks.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/asyncio/atasks/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/asyncio/atasks/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/asyncio/atasks/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/parallel_execution/asyncio/atasks/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/asyncio/efficient_streams/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/asyncio/efficient_streams/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/asyncio/efficient_streams/versions/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/asyncio/efficient_streams/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/efficient_streams_abstract.py` & `cengal-3.1.18.4/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/efficient_streams_abstract.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/efficient_streams_base.py` & `cengal-3.1.18.4/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/efficient_streams_base.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/efficient_streams_base_internal.py` & `cengal-3.1.18.4/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/efficient_streams_base_internal.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/tcp_efficient_streams.py` & `cengal-3.1.18.4/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/tcp_efficient_streams.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/tests/asyncio_streams_client.py` & `cengal-3.1.18.4/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/tests/asyncio_streams_client.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/tests/asyncio_streams_server.py` & `cengal-3.1.18.4/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/tests/asyncio_streams_server.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/udp_efficient_streams.py` & `cengal-3.1.18.4/cengal/parallel_execution/asyncio/efficient_streams/versions/v_0/udp_efficient_streams.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/asyncio/init_loop/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/asyncio/init_loop/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/asyncio/init_loop/versions/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/asyncio/init_loop/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/asyncio/init_loop/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/asyncio/init_loop/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/asyncio/init_loop/versions/v_0/init_loop.py` & `cengal-3.1.18.4/cengal/parallel_execution/asyncio/init_loop/versions/v_0/init_loop.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/asyncio/init_loop/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/asyncio/init_loop/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/asyncio/init_loop/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/parallel_execution/asyncio/init_loop/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/asyncio/run_in_process_pool/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/asyncio/run_in_process_pool/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/asyncio/run_in_process_pool/versions/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/asyncio/run_in_process_pool/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/asyncio/run_in_process_pool/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/asyncio/run_in_process_pool/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/asyncio/run_in_process_pool/versions/v_0/run_in_process_pool.py` & `cengal-3.1.18.4/cengal/parallel_execution/asyncio/run_in_process_pool/versions/v_0/run_in_process_pool.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/asyncio/run_in_process_pool/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/asyncio/run_in_process_pool/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/asyncio/run_in_process_pool/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/parallel_execution/asyncio/run_in_process_pool/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/asyncio/run_loop/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/asyncio/run_loop/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/asyncio/run_loop/versions/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/asyncio/run_loop/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/asyncio/run_loop/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/asyncio/run_loop/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/asyncio/run_loop/versions/v_0/run_loop.py` & `cengal-3.1.18.4/cengal/parallel_execution/asyncio/run_loop/versions/v_0/run_loop.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/asyncio/run_loop/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/asyncio/run_loop/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/asyncio/run_loop/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/parallel_execution/asyncio/run_loop/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/asyncio/timed_yield/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/asyncio/timed_yield/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/asyncio/timed_yield/versions/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/asyncio/timed_yield/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/asyncio/timed_yield/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/asyncio/timed_yield/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/asyncio/timed_yield/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/asyncio/timed_yield/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/asyncio/timed_yield/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/parallel_execution/asyncio/timed_yield/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/asyncio/timed_yield/versions/v_0/timed_yield.py` & `cengal-3.1.18.4/cengal/parallel_execution/asyncio/timed_yield/versions/v_0/timed_yield.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_scheduler/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_scheduler/versions/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_scheduler/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_scheduler/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_scheduler/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_scheduler/versions/v_0/coro_scheduler.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_scheduler/versions/v_0/coro_scheduler.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_scheduler/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_scheduler/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_scheduler/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_scheduler/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/versions/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/versions/v_0/async_event_bus.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/versions/v_0/async_event_bus.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/async_event_bus/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/versions/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/versions/v_0/asyncio_loop.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/versions/v_0/asyncio_loop.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/asyncio_loop/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/communication/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/communication/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/communication/versions/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/communication/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/communication/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/communication/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/communication/versions/v_0/communication.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/communication/versions/v_0/communication.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/communication/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/communication/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/communication/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/communication/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/versions/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/versions/v_0/cpu_tick_count_per_second.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/versions/v_0/cpu_tick_count_per_second.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/cpu_tick_count_per_second/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/db/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/db/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/db/versions/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/db/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/db/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/db/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/db/versions/v_0/db.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/db/versions/v_0/db.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/db/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/db/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/db/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/db/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/versions/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/versions/v_0/event_bus.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/versions/v_0/event_bus.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/event_bus/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/versions/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/versions/v_0/fast_aggregator.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/versions/v_0/fast_aggregator.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/fast_aggregator/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/instance/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/instance/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/instance/versions/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/instance/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/instance/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/instance/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/instance/versions/v_0/instance.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/instance/versions/v_0/instance.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/instance/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/instance/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/instance/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/instance/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/versions/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/versions/v_0/kill_coro.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/versions/v_0/kill_coro.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/versions/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/versions/v_0/kill_coro_list.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/versions/v_0/kill_coro_list.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/kill_coro_list/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/versions/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/versions/v_0/lazy_print.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/versions/v_0/lazy_print.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/lazy_print/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/versions/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/versions/v_0/lmdb.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/versions/v_0/lmdb.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/lmdb/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/log/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/log/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/log/versions/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/log/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/log/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/log/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/log/versions/v_0/log.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/log/versions/v_0/log.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/log/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/log/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/log/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/log/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/v_0/bytecode_patcher.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/v_0/bytecode_patcher.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/v_0/loop_yield.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/v_0/loop_yield.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/loop_yield/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/versions/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/versions/v_0/put_coro.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/versions/v_0/put_coro.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/put_coro/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/versions/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/versions/v_0/put_coro_list.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/versions/v_0/put_coro_list.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/put_coro_list/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/versions/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/versions/v_0/read_write_locker.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/versions/v_0/read_write_locker.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/read_write_locker/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/class_info.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/class_info.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/commands.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/commands.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/exceptions.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/exceptions.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/remote_node.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/remote_node.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/remote_nodes.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/remote_nodes.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/request_class_info.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/request_class_info.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/serializers.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/serializers.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/remote_nodes/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/versions/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/versions/v_0/run_coro.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/versions/v_0/run_coro.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/run_coro/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/versions/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/versions/v_0/shutdown_loop.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/versions/v_0/shutdown_loop.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_loop/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/versions/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/versions/v_0/shutdown_on_keyboard_interrupt.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/versions/v_0/shutdown_on_keyboard_interrupt.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/shutdown_on_keyboard_interrupt/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/versions/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/versions/v_0/simple_yield.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/versions/v_0/simple_yield.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/simple_yield/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/sleep/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/sleep/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/sleep/versions/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/sleep/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/sleep/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/sleep/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/sleep/versions/v_0/sleep.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/sleep/versions/v_0/sleep.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/sleep/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/sleep/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/sleep/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/sleep/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/versions/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/versions/v_0/some_printer.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/versions/v_0/some_printer.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/some_printer/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/versions/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/versions/v_0/throw_coro.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro/versions/v_0/throw_coro.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/versions/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/versions/v_0/throw_coro_list.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/throw_coro_list/versions/v_0/throw_coro_list.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/versions/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/versions/v_0/timer_coro_runner.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/timer_coro_runner/versions/v_0/timer_coro_runner.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/versions/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/versions/v_0/timer_func_runner.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/timer_func_runner/versions/v_0/timer_func_runner.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/v_0/tkinter.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/tkinter/versions/v_0/tkinter.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/versions/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/versions/v_0/wait_coro.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services/wait_coro/versions/v_0/wait_coro.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/versions/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/versions/v_0/general.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/versions/v_0/general.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/general/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/versions/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/versions/v_0/service_with_a_direct_request.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/versions/v_0/service_with_a_direct_request.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_standard_services_internal_lib/service_with_a_direct_request/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/await_coro/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/await_coro/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/await_coro/versions/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/await_coro/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/await_coro/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/await_coro/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/await_coro/versions/v_0/await_coro.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/await_coro/versions/v_0/await_coro.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/await_coro/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/await_coro/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/await_coro/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/await_coro/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/versions/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/versions/v_0/coro_flow_control.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/versions/v_0/coro_flow_control.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/coro_flow_control/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/low_latency/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/low_latency/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/v_0/ajson.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/v_0/ajson.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/v_0/json.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/v_0/json.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/low_latency/json/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/versions/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/versions/v_0/prepare_loop.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/versions/v_0/prepare_loop.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/prepare_loop/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/v_0/run_in_loop.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/v_0/run_in_loop.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/wait_coro/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/wait_coro/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/wait_coro/versions/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/wait_coro/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/wait_coro/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/wait_coro/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/wait_coro/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/wait_coro/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/wait_coro/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/wait_coro/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/coro_tools/wait_coro/versions/v_0/wait_coro.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/coro_tools/wait_coro/versions/v_0/wait_coro.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/customtkinter/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/customtkinter/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/customtkinter/versions/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/customtkinter/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/customtkinter/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/customtkinter/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/customtkinter/versions/v_0/customtkinter.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/customtkinter/versions/v_0/customtkinter.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/customtkinter/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/customtkinter/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/customtkinter/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/customtkinter/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/nicegui/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/nicegui/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/nicegui/versions/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/nicegui/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/nicegui/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/nicegui/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/nicegui/versions/v_0/nicegui.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/nicegui/versions/v_0/nicegui.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/nicegui/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/nicegui/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/nicegui/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/nicegui/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/pytermgui/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/pytermgui/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/v_0/pytermgui.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/v_0/pytermgui.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/pytermgui/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/qt/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/qt/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/qt/versions/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/qt/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/qt/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/qt/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/qt/versions/v_0/qt.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/qt/versions/v_0/qt.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/qt/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/qt/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/qt/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/qt/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/uvicorn/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/uvicorn/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/uvicorn/versions/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/uvicorn/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/uvicorn/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/uvicorn/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/uvicorn/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/uvicorn/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/uvicorn/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/uvicorn/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/uvicorn/versions/v_0/uvicorn.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/uvicorn/versions/v_0/uvicorn.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/uvloop/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/uvloop/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/uvloop/versions/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/uvloop/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/uvloop/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/uvloop/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/uvloop/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/uvloop/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/uvloop/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/uvloop/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/coroutines/integrations/uvloop/versions/v_0/uvloop.py` & `cengal-3.1.18.4/cengal/parallel_execution/coroutines/integrations/uvloop/versions/v_0/uvloop.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/green_threads_tools/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/green_threads_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/green_threads_tools/task_management.py` & `cengal-3.1.18.4/cengal/parallel_execution/green_threads_tools/task_management.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/multiprocess/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/multiprocess/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/multiprocess/multiprocess_testing.py` & `cengal-3.1.18.4/cengal/parallel_execution/multiprocess/multiprocess_testing.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/multiprocess/multiprocessing_task_pool.py` & `cengal-3.1.18.4/cengal/parallel_execution/multiprocess/multiprocessing_task_pool.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/multiprocess/multiprocessing_task_runner.py` & `cengal-3.1.18.4/cengal/parallel_execution/multiprocess/multiprocessing_task_runner.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/multithreading/__init__.py` & `cengal-3.1.18.4/cengal/parallel_execution/multithreading/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/parallel_execution/multithreading/thread_workers_pool.py` & `cengal-3.1.18.4/cengal/parallel_execution/multithreading/thread_workers_pool.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/performance_test_lib/__init__.py` & `cengal-3.1.18.4/cengal/performance_test_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/performance_test_lib/versions/__init__.py` & `cengal-3.1.18.4/cengal/performance_test_lib/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/performance_test_lib/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/performance_test_lib/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/performance_test_lib/versions/v_0/performance_test_lib.py` & `cengal-3.1.18.4/cengal/performance_test_lib/versions/v_0/performance_test_lib.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/performance_test_lib/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/performance_test_lib/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/performance_test_lib/versions/v_0/tests/test__performance_test_lib.py` & `cengal-3.1.18.4/cengal/performance_test_lib/versions/v_0/tests/test__performance_test_lib.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/performance_test_lib/versions/v_1/__init__.py` & `cengal-3.1.18.4/cengal/performance_test_lib/versions/v_1/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/performance_test_lib/versions/v_1/performance_test_lib.py` & `cengal-3.1.18.4/cengal/performance_test_lib/versions/v_1/performance_test_lib.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/performance_test_lib/versions/v_1/tests/__init__.py` & `cengal-3.1.18.4/cengal/performance_test_lib/versions/v_1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/performance_test_lib/versions/v_1/tests/test__performance_test_lib.py` & `cengal-3.1.18.4/cengal/performance_test_lib/versions/v_1/tests/test__performance_test_lib.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/shared_memory/__init__.py` & `cengal-3.1.18.4/cengal/shared_memory/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/shared_memory/versions/1/__init__.py` & `cengal-3.1.18.4/cengal/shared_memory/versions/1/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/shared_memory/versions/1/mmap.py` & `cengal-3.1.18.4/cengal/shared_memory/versions/1/mmap.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/shared_memory/versions/__init__.py` & `cengal-3.1.18.4/cengal/shared_memory/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/statistics/__init__.py` & `cengal-3.1.18.4/cengal/statistics/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/statistics/normal_distribution/__init__.py` & `cengal-3.1.18.4/cengal/statistics/normal_distribution/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/statistics/normal_distribution/versions/__init__.py` & `cengal-3.1.18.4/cengal/statistics/normal_distribution/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/statistics/normal_distribution/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/statistics/normal_distribution/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/statistics/normal_distribution/versions/v_0/normal_distribution.py` & `cengal-3.1.18.4/cengal/statistics/normal_distribution/versions/v_0/normal_distribution.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/statistics/normal_distribution/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/statistics/normal_distribution/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/statistics/normal_distribution/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/statistics/normal_distribution/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/system.py` & `cengal-3.1.18.4/cengal/system.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/testing_lib/__init__.py` & `cengal-3.1.18.4/cengal/testing_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/testing_lib/tests_list_runner.py` & `cengal-3.1.18.4/cengal/testing_lib/tests_list_runner.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/text_processing/__init__.py` & `cengal-3.1.18.4/cengal/text_processing/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/text_processing/brackets_processing/__init__.py` & `cengal-3.1.18.4/cengal/text_processing/brackets_processing/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/text_processing/brackets_processing/versions/__init__.py` & `cengal-3.1.18.4/cengal/text_processing/brackets_processing/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/text_processing/brackets_processing/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/text_processing/brackets_processing/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/text_processing/brackets_processing/versions/v_0/brackets.py` & `cengal-3.1.18.4/cengal/text_processing/brackets_processing/versions/v_0/brackets.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/text_processing/brackets_processing/versions/v_0/processing.py` & `cengal-3.1.18.4/cengal/text_processing/brackets_processing/versions/v_0/processing.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/text_processing/brackets_processing/versions/v_0/standard_brackets.py` & `cengal-3.1.18.4/cengal/text_processing/brackets_processing/versions/v_0/standard_brackets.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/text_processing/brackets_processing/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/text_processing/brackets_processing/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/text_processing/brackets_processing/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/text_processing/brackets_processing/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/text_processing/encoding_detection/__init__.py` & `cengal-3.1.18.4/cengal/text_processing/encoding_detection/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/text_processing/encoding_detection/versions/__init__.py` & `cengal-3.1.18.4/cengal/text_processing/encoding_detection/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/text_processing/encoding_detection/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/text_processing/encoding_detection/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/text_processing/encoding_detection/versions/v_0/encoding_detection.py` & `cengal-3.1.18.4/cengal/text_processing/encoding_detection/versions/v_0/encoding_detection.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/text_processing/encoding_detection/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/text_processing/encoding_detection/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/text_processing/encoding_detection/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/text_processing/encoding_detection/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/text_processing/help_tools.py` & `cengal-3.1.18.4/cengal/text_processing/help_tools.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/text_processing/optional_formatter/__init__.py` & `cengal-3.1.18.4/cengal/text_processing/optional_formatter/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/text_processing/optional_formatter/versions/__init__.py` & `cengal-3.1.18.4/cengal/text_processing/optional_formatter/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/text_processing/optional_formatter/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/text_processing/optional_formatter/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/text_processing/optional_formatter/versions/v_0/optional_formatter.py` & `cengal-3.1.18.4/cengal/text_processing/optional_formatter/versions/v_0/optional_formatter.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/text_processing/optional_formatter/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/text_processing/optional_formatter/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/text_processing/optional_formatter/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/text_processing/optional_formatter/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/text_processing/simple_config_file_processor/__init__.py` & `cengal-3.1.18.4/cengal/text_processing/simple_config_file_processor/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/text_processing/simple_config_file_processor/versions/__init__.py` & `cengal-3.1.18.4/cengal/text_processing/simple_config_file_processor/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/text_processing/simple_config_file_processor/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/text_processing/simple_config_file_processor/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/text_processing/simple_config_file_processor/versions/v_0/simple_config_file_processor.py` & `cengal-3.1.18.4/cengal/text_processing/simple_config_file_processor/versions/v_0/simple_config_file_processor.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/text_processing/simple_config_file_processor/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/text_processing/simple_config_file_processor/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/text_processing/simple_config_file_processor/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/text_processing/simple_config_file_processor/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/text_processing/text_patch/__init__.py` & `cengal-3.1.18.4/cengal/text_processing/text_patch/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/text_processing/text_patch/brackets/__init__.py` & `cengal-3.1.18.4/cengal/text_processing/text_patch/brackets/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/text_processing/text_patch/brackets/versions/__init__.py` & `cengal-3.1.18.4/cengal/text_processing/text_patch/brackets/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/text_processing/text_patch/brackets/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/text_processing/text_patch/brackets/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/text_processing/text_patch/brackets/versions/v_0/brackets.py` & `cengal-3.1.18.4/cengal/text_processing/text_patch/brackets/versions/v_0/brackets.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/text_processing/text_patch/brackets/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/text_processing/text_patch/brackets/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/text_processing/text_patch/brackets/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/text_processing/text_patch/brackets/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/text_processing/text_patch/simple/__init__.py` & `cengal-3.1.18.4/cengal/text_processing/text_patch/simple/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/text_processing/text_patch/simple/versions/__init__.py` & `cengal-3.1.18.4/cengal/text_processing/text_patch/simple/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/text_processing/text_patch/simple/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/text_processing/text_patch/simple/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/text_processing/text_patch/simple/versions/v_0/simple.py` & `cengal-3.1.18.4/cengal/text_processing/text_patch/simple/versions/v_0/simple.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/text_processing/text_patch/simple/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/text_processing/text_patch/simple/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/text_processing/text_patch/simple/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/text_processing/text_patch/simple/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/text_processing/text_processing/__init__.py` & `cengal-3.1.18.4/cengal/text_processing/text_processing/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/text_processing/text_processing/versions/__init__.py` & `cengal-3.1.18.4/cengal/text_processing/text_processing/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/text_processing/text_processing/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/text_processing/text_processing/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/text_processing/text_processing/versions/v_0/processing.py` & `cengal-3.1.18.4/cengal/text_processing/text_processing/versions/v_0/processing.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/text_processing/text_processing/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/text_processing/text_processing/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/text_processing/text_processing/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/text_processing/text_processing/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/text_processing/text_translator/__init__.py` & `cengal-3.1.18.4/cengal/text_processing/text_translator/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/text_processing/text_translator/versions/__init__.py` & `cengal-3.1.18.4/cengal/text_processing/text_translator/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/text_processing/text_translator/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/text_processing/text_translator/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/text_processing/text_translator/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/text_processing/text_translator/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/text_processing/text_translator/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/text_processing/text_translator/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/text_processing/text_translator/versions/v_0/text_translator.py` & `cengal-3.1.18.4/cengal/text_processing/text_translator/versions/v_0/text_translator.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/text_processing/utf_bom_processing/__init__.py` & `cengal-3.1.18.4/cengal/text_processing/utf_bom_processing/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/text_processing/utf_bom_processing/versions/__init__.py` & `cengal-3.1.18.4/cengal/text_processing/utf_bom_processing/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/text_processing/utf_bom_processing/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/text_processing/utf_bom_processing/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/text_processing/utf_bom_processing/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/text_processing/utf_bom_processing/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/text_processing/utf_bom_processing/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/text_processing/utf_bom_processing/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/text_processing/utf_bom_processing/versions/v_0/utf_bom_processing.py` & `cengal-3.1.18.4/cengal/text_processing/utf_bom_processing/versions/v_0/utf_bom_processing.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/time_management/__init__.py` & `cengal-3.1.18.4/cengal/time_management/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/time_management/cpu_clock/__init__.py` & `cengal-3.1.18.4/cengal/time_management/cpu_clock/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/time_management/cpu_clock/versions/__init__.py` & `cengal-3.1.18.4/cengal/time_management/cpu_clock/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/time_management/cpu_clock/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/time_management/cpu_clock/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/time_management/cpu_clock/versions/v_0/compilable/__init__.py` & `cengal-3.1.18.4/cengal/time_management/cpu_clock/versions/v_0/compilable/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/time_management/cpu_clock/versions/v_0/compilable/__x__build_config.py` & `cengal-3.1.18.4/cengal/time_management/cpu_clock/versions/v_0/compilable/__x__build_config.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/time_management/cpu_clock/versions/v_0/cpu_clock.py` & `cengal-3.1.18.4/cengal/time_management/cpu_clock/versions/v_0/cpu_clock.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/time_management/cpu_clock/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/time_management/cpu_clock/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/time_management/cpu_clock/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/time_management/cpu_clock/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/time_management/cpu_clock_cycles/__init__.py` & `cengal-3.1.18.4/cengal/time_management/cpu_clock_cycles/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/time_management/cpu_clock_cycles/versions/__init__.py` & `cengal-3.1.18.4/cengal/time_management/cpu_clock_cycles/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/time_management/cpu_clock_cycles/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/time_management/cpu_clock_cycles/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/time_management/cpu_clock_cycles/versions/v_0/compilable/__build_config.py` & `cengal-3.1.18.4/cengal/time_management/cpu_clock_cycles/versions/v_0/compilable/__build_config.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/time_management/cpu_clock_cycles/versions/v_0/compilable/__init__.py` & `cengal-3.1.18.4/cengal/time_management/cpu_clock_cycles/versions/v_0/compilable/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/time_management/cpu_clock_cycles/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/time_management/cpu_clock_cycles/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/time_management/cpu_clock_cycles/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/time_management/cpu_clock_cycles/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/time_management/high_precision_sync_sleep/__init__.py` & `cengal-3.1.18.4/cengal/time_management/high_precision_sync_sleep/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/time_management/high_precision_sync_sleep/versions/__init__.py` & `cengal-3.1.18.4/cengal/time_management/high_precision_sync_sleep/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/time_management/high_precision_sync_sleep/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/time_management/high_precision_sync_sleep/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/time_management/high_precision_sync_sleep/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/time_management/high_precision_sync_sleep/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/time_management/high_precision_sync_sleep/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/time_management/high_precision_sync_sleep/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/time_management/load_best_timer/__init__.py` & `cengal-3.1.18.4/cengal/time_management/load_best_timer/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/time_management/load_best_timer/versions/__init__.py` & `cengal-3.1.18.4/cengal/time_management/load_best_timer/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/time_management/load_best_timer/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/time_management/load_best_timer/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/time_management/load_best_timer/versions/v_0/load_best_timer.py` & `cengal-3.1.18.4/cengal/time_management/load_best_timer/versions/v_0/load_best_timer.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/time_management/relative_time/__init__.py` & `cengal-3.1.18.4/cengal/time_management/relative_time/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/time_management/relative_time/approximate_representation/__init__.py` & `cengal-3.1.18.4/cengal/time_management/relative_time/approximate_representation/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/time_management/relative_time/approximate_representation/versions/__init__.py` & `cengal-3.1.18.4/cengal/time_management/relative_time/approximate_representation/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/time_management/relative_time/approximate_representation/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/time_management/relative_time/approximate_representation/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/time_management/relative_time/approximate_representation/versions/v_0/approximate_representation.py` & `cengal-3.1.18.4/cengal/time_management/relative_time/approximate_representation/versions/v_0/approximate_representation.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/time_management/relative_time/bysiness_relativedelta/__init__.py` & `cengal-3.1.18.4/cengal/time_management/relative_time/bysiness_relativedelta/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/time_management/relative_time/bysiness_relativedelta/versions/__init__.py` & `cengal-3.1.18.4/cengal/time_management/relative_time/bysiness_relativedelta/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/time_management/relative_time/bysiness_relativedelta/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/time_management/relative_time/bysiness_relativedelta/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/time_management/relative_time/bysiness_relativedelta/versions/v_0/bysiness_relativedelta.py` & `cengal-3.1.18.4/cengal/time_management/relative_time/bysiness_relativedelta/versions/v_0/bysiness_relativedelta.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/time_management/relative_time/constants/__init__.py` & `cengal-3.1.18.4/cengal/time_management/relative_time/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/time_management/relative_time/constants/versions/__init__.py` & `cengal-3.1.18.4/cengal/time_management/relative_time/constants/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/time_management/relative_time/constants/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/time_management/relative_time/constants/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/time_management/relative_time/constants/versions/v_0/constants.py` & `cengal-3.1.18.4/cengal/time_management/relative_time/constants/versions/v_0/constants.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/time_management/relative_time/relativedelta/__init__.py` & `cengal-3.1.18.4/cengal/time_management/relative_time/relativedelta/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/time_management/relative_time/relativedelta/versions/__init__.py` & `cengal-3.1.18.4/cengal/time_management/relative_time/relativedelta/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/time_management/relative_time/relativedelta/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/time_management/relative_time/relativedelta/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/time_management/relative_time/relativedelta/versions/v_0/relativedelta.py` & `cengal-3.1.18.4/cengal/time_management/relative_time/relativedelta/versions/v_0/relativedelta.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/time_management/relative_time/timedelta/__init__.py` & `cengal-3.1.18.4/cengal/time_management/relative_time/timedelta/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/time_management/relative_time/timedelta/versions/__init__.py` & `cengal-3.1.18.4/cengal/time_management/relative_time/timedelta/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/time_management/relative_time/timedelta/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/time_management/relative_time/timedelta/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/time_management/relative_time/timedelta/versions/v_0/timedelta.py` & `cengal-3.1.18.4/cengal/time_management/relative_time/timedelta/versions/v_0/timedelta.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/time_management/repeat_for_a_time/__init__.py` & `cengal-3.1.18.4/cengal/time_management/repeat_for_a_time/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/time_management/repeat_for_a_time/versions/__init__.py` & `cengal-3.1.18.4/cengal/time_management/repeat_for_a_time/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/time_management/repeat_for_a_time/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/time_management/repeat_for_a_time/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/time_management/repeat_for_a_time/versions/v_0/repeat_for_a_time__python.py` & `cengal-3.1.18.4/cengal/time_management/repeat_for_a_time/versions/v_0/repeat_for_a_time__python.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/time_management/repeat_for_a_time/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/time_management/repeat_for_a_time/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/time_management/repeat_for_a_time/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/time_management/repeat_for_a_time/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/time_management/repeat_for_a_time/versions/v_0/tests/example_for__repeat_for_a_time.py` & `cengal-3.1.18.4/cengal/time_management/repeat_for_a_time/versions/v_0/tests/example_for__repeat_for_a_time.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/time_management/sleep_tools/__init__.py` & `cengal-3.1.18.4/cengal/time_management/sleep_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/time_management/sleep_tools/versions/__init__.py` & `cengal-3.1.18.4/cengal/time_management/sleep_tools/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/time_management/sleep_tools/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/time_management/sleep_tools/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/time_management/sleep_tools/versions/v_0/sleep_tools.py` & `cengal-3.1.18.4/cengal/time_management/sleep_tools/versions/v_0/sleep_tools.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/time_management/sleep_tools/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/time_management/sleep_tools/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/time_management/sleep_tools/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/time_management/sleep_tools/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/time_management/timer/__init__.py` & `cengal-3.1.18.4/cengal/time_management/timer/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/time_management/timer/versions/__init__.py` & `cengal-3.1.18.4/cengal/time_management/timer/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/time_management/timer/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/time_management/timer/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/time_management/timer/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/time_management/timer/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/time_management/timer/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/time_management/timer/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/time_management/timer/versions/v_0/timer.py` & `cengal-3.1.18.4/cengal/time_management/timer/versions/v_0/timer.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/time_management/timer/versions/v_1/__init__.py` & `cengal-3.1.18.4/cengal/time_management/timer/versions/v_1/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/time_management/timer/versions/v_1/tests/__init__.py` & `cengal-3.1.18.4/cengal/time_management/timer/versions/v_1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/time_management/timer/versions/v_1/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/time_management/timer/versions/v_1/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/time_management/timer/versions/v_1/timer.py` & `cengal-3.1.18.4/cengal/time_management/timer/versions/v_1/timer.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/time_management/timer_precision/__init__.py` & `cengal-3.1.18.4/cengal/time_management/timer_precision/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/time_management/timer_precision/versions/__init__.py` & `cengal-3.1.18.4/cengal/time_management/timer_precision/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/time_management/timer_precision/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/time_management/timer_precision/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/time_management/timer_precision/versions/v_0/test_timer_precision.py` & `cengal-3.1.18.4/cengal/time_management/timer_precision/versions/v_0/test_timer_precision.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/time_management/timer_precision/versions/v_1/__init__.py` & `cengal-3.1.18.4/cengal/time_management/timer_precision/versions/v_1/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/time_management/timer_precision/versions/v_1/timer_precision.py` & `cengal-3.1.18.4/cengal/time_management/timer_precision/versions/v_1/timer_precision.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/unittest/__init__.py` & `cengal-3.1.18.4/cengal/unittest/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/unittest/behavior_stabilizer/__init__.py` & `cengal-3.1.18.4/cengal/unittest/behavior_stabilizer/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/unittest/behavior_stabilizer/versions/__init__.py` & `cengal-3.1.18.4/cengal/unittest/behavior_stabilizer/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/unittest/behavior_stabilizer/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/unittest/behavior_stabilizer/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/unittest/behavior_stabilizer/versions/v_0/behavior_stabilizer.py` & `cengal-3.1.18.4/cengal/unittest/behavior_stabilizer/versions/v_0/behavior_stabilizer.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/unittest/behavior_stabilizer/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/unittest/behavior_stabilizer/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/unittest/behavior_stabilizer/versions/v_0/tests/_test__behavior_stabilizer.py` & `cengal-3.1.18.4/cengal/unittest/behavior_stabilizer/versions/v_0/tests/_test__behavior_stabilizer.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/unittest/patcher/__init__.py` & `cengal-3.1.18.4/cengal/unittest/patcher/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/unittest/patcher/versions/__init__.py` & `cengal-3.1.18.4/cengal/unittest/patcher/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/unittest/patcher/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/unittest/patcher/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/unittest/patcher/versions/v_0/patcher.py` & `cengal-3.1.18.4/cengal/unittest/patcher/versions/v_0/patcher.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/unittest/patcher/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/unittest/patcher/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/unittest/patcher/versions/v_0/tests/_test__patcher.py` & `cengal-3.1.18.4/cengal/unittest/patcher/versions/v_0/tests/_test__patcher.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/universal_parser/__init__.py` & `cengal-3.1.18.4/cengal/universal_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/universal_parser/help_tools.py` & `cengal-3.1.18.4/cengal/universal_parser/help_tools.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/universal_parser/idioms.py` & `cengal-3.1.18.4/cengal/universal_parser/idioms.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/universal_parser/parser.py` & `cengal-3.1.18.4/cengal/universal_parser/parser.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/universal_parser/test.py` & `cengal-3.1.18.4/cengal/universal_parser/test.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/universal_parser/types.py` & `cengal-3.1.18.4/cengal/universal_parser/types.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/upk_helping_tools/__init__.py` & `cengal-3.1.18.4/cengal/upk_helping_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/upk_helping_tools/upk_api.py` & `cengal-3.1.18.4/cengal/upk_helping_tools/upk_api.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/upk_helping_tools/upk_constants.py` & `cengal-3.1.18.4/cengal/upk_helping_tools/upk_constants.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/upk_helping_tools/upk_utils_api.py` & `cengal-3.1.18.4/cengal/upk_helping_tools/upk_utils_api.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/user_interface/__init__.py` & `cengal-3.1.18.4/cengal/user_interface/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/user_interface/console/__init__.py` & `cengal-3.1.18.4/cengal/user_interface/console/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/user_interface/console/chooser.py` & `cengal-3.1.18.4/cengal/user_interface/console/chooser.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/user_interface/console/colorama_helpers.py` & `cengal-3.1.18.4/cengal/user_interface/console/colorama_helpers.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/user_interface/console/encoding_changer.py` & `cengal-3.1.18.4/cengal/user_interface/console/encoding_changer.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/user_interface/console/progress_meter/__init__.py` & `cengal-3.1.18.4/cengal/user_interface/console/progress_meter/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/user_interface/console/progress_meter/versions/__init__.py` & `cengal-3.1.18.4/cengal/user_interface/console/progress_meter/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/user_interface/console/progress_meter/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/user_interface/console/progress_meter/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/user_interface/console/progress_meter/versions/v_0/progress_meter.py` & `cengal-3.1.18.4/cengal/user_interface/console/progress_meter/versions/v_0/progress_meter.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/user_interface/console/progress_meter/versions/v_0/progress_meter_python2.py` & `cengal-3.1.18.4/cengal/user_interface/console/progress_meter/versions/v_0/progress_meter_python2.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/user_interface/gui/__init__.py` & `cengal-3.1.18.4/cengal/user_interface/gui/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/user_interface/gui/nt/__init__.py` & `cengal-3.1.18.4/cengal/user_interface/gui/nt/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/user_interface/gui/nt/blur_behind/__init__.py` & `cengal-3.1.18.4/cengal/user_interface/gui/nt/blur_behind/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/user_interface/gui/nt/blur_behind/versions/__init__.py` & `cengal-3.1.18.4/cengal/user_interface/gui/nt/blur_behind/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/user_interface/gui/nt/blur_behind/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/user_interface/gui/nt/blur_behind/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/user_interface/gui/nt/blur_behind/versions/v_0/blur_behind.py` & `cengal-3.1.18.4/cengal/user_interface/gui/nt/blur_behind/versions/v_0/blur_behind.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/user_interface/gui/nt/blur_behind/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/user_interface/gui/nt/blur_behind/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/user_interface/gui/nt/blur_behind/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/user_interface/gui/nt/blur_behind/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/user_interface/gui/nt/dpi_awareness/__init__.py` & `cengal-3.1.18.4/cengal/user_interface/gui/nt/dpi_awareness/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/user_interface/gui/nt/dpi_awareness/versions/__init__.py` & `cengal-3.1.18.4/cengal/user_interface/gui/nt/dpi_awareness/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/user_interface/gui/nt/dpi_awareness/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/user_interface/gui/nt/dpi_awareness/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/user_interface/gui/nt/dpi_awareness/versions/v_0/dpi_awareness.py` & `cengal-3.1.18.4/cengal/user_interface/gui/nt/dpi_awareness/versions/v_0/dpi_awareness.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/user_interface/gui/nt/dpi_awareness/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/user_interface/gui/nt/dpi_awareness/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/user_interface/gui/nt/dpi_awareness/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/user_interface/gui/nt/dpi_awareness/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/user_interface/plot/__init__.py` & `cengal-3.1.18.4/cengal/user_interface/plot/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/user_interface/plot/versions/__init__.py` & `cengal-3.1.18.4/cengal/user_interface/plot/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/user_interface/plot/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/user_interface/plot/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/user_interface/plot/versions/v_0/plot.py` & `cengal-3.1.18.4/cengal/user_interface/plot/versions/v_0/plot.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/user_interface/plot/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/user_interface/plot/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/user_interface/plot/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/user_interface/plot/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/web_tools/__init__.py` & `cengal-3.1.18.4/cengal/web_tools/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/web_tools/detect_browsers_host_device_type/__init__.py` & `cengal-3.1.18.4/cengal/web_tools/detect_browsers_host_device_type/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/__init__.py` & `cengal-3.1.18.4/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/__init__.py` & `cengal-3.1.18.4/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/v_0/__init__.py` & `cengal-3.1.18.4/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/v_0/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/v_0/by_http_user_agent.py` & `cengal-3.1.18.4/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/v_0/by_http_user_agent.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/v_0/tests/__init__.py` & `cengal-3.1.18.4/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/v_0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/v_0/tests/_test__template_submodule.py` & `cengal-3.1.18.4/cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/v_0/tests/_test__template_submodule.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal/web_tools/help_tools.py` & `cengal-3.1.18.4/cengal/web_tools/help_tools.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal.egg-info/PKG-INFO` & `cengal-3.1.18.4/cengal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cengal
-Version: 3.1.18.3
+Version: 3.1.18.4
 Summary: General purpose library
 Home-page: https://github.com/FI-Mihej/Cengal
 Author: ButenkoMS
 Author-email: gtalk@butenkoms.space
 License: Apache License, Version 2.0
 Keywords: async loop,coroutine,async Qt,async Tkinter,bytecode manipulation,introspection,text parsing
 Classifier: Programming Language :: Python :: 3
@@ -396,15 +396,15 @@
 
 * [General idea, greenlet main Cengal.coro](https://github.com/FI-Mihej/Cengal/blob/master/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/v_0/development/main.py)
 * [General idea, async main Cengal.coro](https://github.com/FI-Mihej/Cengal/blob/master/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/v_0/development/amain.py)
 * [Transparent interconnection between Cengal.coroutines and asyncio](https://github.com/FI-Mihej/Cengal/blob/master/cengal/parallel_execution/coroutines/coro_tools/run_in_loop/versions/v_0/development/asyncio_interconnection.py)
 
 ### Text processing example
 
-[Ensures and updates copyright (with dates) in each Cengal's source file](https://github.com/FI-Mihej/Cengal/blob/master/cengal_setup_scripts/ensure_copyright/ensure_copyright.py)
+[Ensures and updates copyright (with dates) in each Cengal's source file](https://github.com/FI-Mihej/Cengal/blob/master/cengal._cengal_setup_scripts/ensure_copyright/ensure_copyright.py)
 
 ## Projects using Cengal
 
 * [flet_async](https://github.com/FI-Mihej/flet_async) - wrapper which makes [Flet](https://github.com/flet-dev/flet) async and brings booth Cengal.coroutines and asyncio to Flet (Flutter based UI)
 * [justpy_containers](https://github.com/FI-Mihej/justpy_containers) - wrapper around [JustPy](https://github.com/justpy-org/justpy) in order to bring more security and more production-needed features to JustPy (VueJS based UI)
 * [Bensbach](https://github.com/FI-Mihej/Bensbach) - decompiler from Unreal Engine 3 bytecode to a Lisp-like script and compiler back to Unreal Engine 3 bytecode. Made for a game modding purposes
 * [Realistic-Damage-Model-mod-for-Long-War](https://github.com/FI-Mihej/Realistic-Damage-Model-mod-for-Long-War) - Mod for both the original XCOM:EW and the mod Long War. Was made with a Bensbach, which was made with Cengal
```

### Comparing `cengal-3.1.18.3/cengal.egg-info/SOURCES.txt` & `cengal-3.1.18.4/cengal.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -24,14 +24,24 @@
 cengal/help_tools.py
 cengal/system.py
 cengal.egg-info/PKG-INFO
 cengal.egg-info/SOURCES.txt
 cengal.egg-info/dependency_links.txt
 cengal.egg-info/requires.txt
 cengal.egg-info/top_level.txt
+cengal/_cengal_setup_scripts/__init__.py
+cengal/_cengal_setup_scripts/compile_all_cython_modules.py
+cengal/_cengal_setup_scripts/setup__dynamic_list_of_pieces.py
+cengal/_cengal_setup_scripts/setup__recv_buff_size_computer.py
+cengal/_cengal_setup_scripts/setup__repeat_for_a_time.py
+cengal/_cengal_setup_scripts/find_and_prepare_cython_modules/__init__.py
+cengal/_cengal_setup_scripts/find_and_prepare_cython_modules/find_and_prepare_cython_modules.py
+cengal/_cengal_setup_scripts/install_required_packages/__init__.py
+cengal/_cengal_setup_scripts/install_required_packages/install_packages.py
+cengal/_cengal_setup_scripts/install_required_packages/set_environment_variables.py
 cengal/base/__init__.py
 cengal/base/classes/__init__.py
 cengal/base/classes/versions/__init__.py
 cengal/base/classes/versions/v_0/__init__.py
 cengal/base/classes/versions/v_0/classes.py
 cengal/base/classes/versions/v_0/tests/__init__.py
 cengal/base/classes/versions/v_0/tests/_test__template_submodule.py
@@ -1156,18 +1166,8 @@
 cengal/web_tools/help_tools.py
 cengal/web_tools/detect_browsers_host_device_type/__init__.py
 cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/__init__.py
 cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/__init__.py
 cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/v_0/__init__.py
 cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/v_0/by_http_user_agent.py
 cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/v_0/tests/__init__.py
-cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/v_0/tests/_test__template_submodule.py
-cengal_setup_scripts/__init__.py
-cengal_setup_scripts/compile_all_cython_modules.py
-cengal_setup_scripts/setup__dynamic_list_of_pieces.py
-cengal_setup_scripts/setup__recv_buff_size_computer.py
-cengal_setup_scripts/setup__repeat_for_a_time.py
-cengal_setup_scripts/find_and_prepare_cython_modules/__init__.py
-cengal_setup_scripts/find_and_prepare_cython_modules/find_and_prepare_cython_modules.py
-cengal_setup_scripts/install_required_packages/__init__.py
-cengal_setup_scripts/install_required_packages/install_packages.py
-cengal_setup_scripts/install_required_packages/set_environment_variables.py
+cengal/web_tools/detect_browsers_host_device_type/by_http_user_agent/versions/v_0/tests/_test__template_submodule.py
```

### Comparing `cengal-3.1.18.3/cengal_setup_scripts/__init__.py` & `cengal-3.1.18.4/cengal/_cengal_setup_scripts/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal_setup_scripts/compile_all_cython_modules.py` & `cengal-3.1.18.4/cengal/_cengal_setup_scripts/compile_all_cython_modules.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal_setup_scripts/find_and_prepare_cython_modules/__init__.py` & `cengal-3.1.18.4/cengal/_cengal_setup_scripts/find_and_prepare_cython_modules/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal_setup_scripts/find_and_prepare_cython_modules/find_and_prepare_cython_modules.py` & `cengal-3.1.18.4/cengal/_cengal_setup_scripts/find_and_prepare_cython_modules/find_and_prepare_cython_modules.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal_setup_scripts/install_required_packages/__init__.py` & `cengal-3.1.18.4/cengal/_cengal_setup_scripts/install_required_packages/__init__.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal_setup_scripts/install_required_packages/install_packages.py` & `cengal-3.1.18.4/cengal/_cengal_setup_scripts/install_required_packages/install_packages.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal_setup_scripts/install_required_packages/set_environment_variables.py` & `cengal-3.1.18.4/cengal/_cengal_setup_scripts/install_required_packages/set_environment_variables.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal_setup_scripts/setup__dynamic_list_of_pieces.py` & `cengal-3.1.18.4/cengal/_cengal_setup_scripts/setup__dynamic_list_of_pieces.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal_setup_scripts/setup__recv_buff_size_computer.py` & `cengal-3.1.18.4/cengal/_cengal_setup_scripts/setup__recv_buff_size_computer.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/cengal_setup_scripts/setup__repeat_for_a_time.py` & `cengal-3.1.18.4/cengal/_cengal_setup_scripts/setup__repeat_for_a_time.py`

 * *Files identical despite different names*

### Comparing `cengal-3.1.18.3/setup.py` & `cengal-3.1.18.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 Docstrings: http://www.python.org/dev/peps/pep-0257/
 """
 
 __author__ = "ButenkoMS <gtalk@butenkoms.space>"
 __copyright__ = "Copyright © 2012-2023 ButenkoMS. All rights reserved. Contacts: <gtalk@butenkoms.space>"
 __credits__ = ["ButenkoMS <gtalk@butenkoms.space>", ]
 __license__ = "Apache License, Version 2.0"
-__version__ = "3.1.18.3"
+__version__ = "3.1.18.4"
 __maintainer__ = "ButenkoMS <gtalk@butenkoms.space>"
 __email__ = "gtalk@butenkoms.space"
 # __status__ = "Prototype"
 __status__ = "Development"
 # __status__ = "Production"
 
 from os import environ
@@ -68,17 +68,17 @@
 
     return good_packages
 
 
 setuptools._install_setup_requires({'setup_requires': ['py-cpuinfo', 'Cython']})
 
 
-from cengal_setup_scripts.install_required_packages.install_packages import install_bundled, get_pypi_requirements_list, get_remote_requirements_list
+from cengal._cengal_setup_scripts.install_required_packages.install_packages import install_bundled, get_pypi_requirements_list, get_remote_requirements_list
 install_bundled()
-from cengal_setup_scripts.find_and_prepare_cython_modules import find_and_prepare_cython_modules
+from cengal._cengal_setup_scripts.find_and_prepare_cython_modules import find_and_prepare_cython_modules
 from cengal.file_system.path_manager import path_relative_to_src
 from Cython.Build import cythonize
 
 
 with open(path_relative_to_src('README.md'), 'r') as fh:
     long_description = fh.read()
```

