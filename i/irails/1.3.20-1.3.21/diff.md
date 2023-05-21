# Comparing `tmp/irails-1.3.20.tar.gz` & `tmp/irails-1.3.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irails-1.3.20.tar", last modified: Sun May 21 08:56:37 2023, max compression
+gzip compressed data, was "irails-1.3.21.tar", last modified: Sun May 21 14:43:30 2023, max compression
```

## Comparing `irails-1.3.20.tar` & `irails-1.3.21.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxrwxrwx   0        0        0        0 2023-05-21 08:56:37.689959 irails-1.3.20/
--rw-rw-rw-   0        0        0       83 2023-05-04 04:10:30.000000 irails-1.3.20/MANIFEST.in
--rw-rw-rw-   0        0        0     6224 2023-05-21 08:56:37.688146 irails-1.3.20/PKG-INFO
--rw-rw-rw-   0        0        0     5440 2023-05-21 08:50:53.000000 irails-1.3.20/README.md
-drwxrwxrwx   0        0        0        0 2023-05-21 08:56:37.599198 irails-1.3.20/irails/
--rw-rw-rw-   0        0        0      307 2023-05-21 08:56:13.000000 irails-1.3.20/irails/__init__.py
--rw-rw-rw-   0        0        0     3948 2023-05-18 07:35:56.000000 irails-1.3.20/irails/_i18n.py
--rw-rw-rw-   0        0        0     2878 2023-05-21 08:27:23.000000 irails-1.3.20/irails/_loader.py
--rw-rw-rw-   0        0        0     5253 2023-05-20 14:13:50.000000 irails-1.3.20/irails/_utils.py
--rw-rw-rw-   0        0        0    12042 2023-05-20 06:44:17.000000 irails-1.3.20/irails/auth.py
--rw-rw-rw-   0        0        0    12705 2023-05-18 07:46:03.000000 irails-1.3.20/irails/base_controller.py
-drwxrwxrwx   0        0        0        0 2023-05-21 08:56:37.609171 irails-1.3.20/irails/casbin_adapters/
-drwxrwxrwx   0        0        0        0 2023-05-21 08:56:37.611167 irails-1.3.20/irails/casbin_adapters/__pycache__/
--rw-rw-rw-   0        0        0    17834 2023-04-30 14:29:09.000000 irails-1.3.20/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc
--rw-rw-rw-   0        0        0    10589 2023-05-13 05:03:07.000000 irails-1.3.20/irails/casbin_adapters/sqlalchemy_adapter.py
--rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 irails-1.3.20/irails/cbv.py
--rw-rw-rw-   0        0        0     6174 2023-05-19 07:06:13.000000 irails-1.3.20/irails/config.py
--rw-rw-rw-   0        0        0    12478 2023-05-12 05:56:24.000000 irails-1.3.20/irails/controller_utils.py
--rw-rw-rw-   0        0        0    24918 2023-05-19 11:59:51.000000 irails-1.3.20/irails/core.py
--rw-rw-rw-   0        0        0    14266 2023-05-21 08:48:41.000000 irails-1.3.20/irails/database.py
--rw-rw-rw-   0        0        0     1459 2023-05-11 15:27:11.000000 irails-1.3.20/irails/log.py
--rw-rw-rw-   0        0        0     8672 2023-05-13 15:15:01.000000 irails-1.3.20/irails/midware.py
--rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 irails-1.3.20/irails/midware_casbin.py
--rw-rw-rw-   0        0        0     9103 2023-05-16 08:16:43.000000 irails-1.3.20/irails/midware_session.py
--rw-rw-rw-   0        0        0     4208 2023-05-16 08:12:27.000000 irails-1.3.20/irails/mvc_router.py
-drwxrwxrwx   0        0        0        0 2023-05-21 08:56:37.623039 irails-1.3.20/irails/scripts/
--rw-rw-rw-   0        0        0        0 2023-04-26 07:44:41.000000 irails-1.3.20/irails/scripts/__init__.py
--rw-rw-rw-   0        0        0     7862 2023-05-13 15:04:27.000000 irails-1.3.20/irails/scripts/_app.py
--rw-rw-rw-   0        0        0     6892 2023-05-19 07:21:20.000000 irails-1.3.20/irails/scripts/_controller.py
--rw-rw-rw-   0        0        0     7755 2023-05-13 05:57:18.000000 irails-1.3.20/irails/scripts/_i18n.py
--rw-rw-rw-   0        0        0     1332 2023-05-21 08:39:33.000000 irails-1.3.20/irails/scripts/_migrate.py
--rw-rw-rw-   0        0        0     3774 2023-05-14 13:34:33.000000 irails-1.3.20/irails/scripts/_model.py
--rw-rw-rw-   0        0        0     2301 2023-05-03 14:35:33.000000 irails-1.3.20/irails/scripts/_project.py
--rw-rw-rw-   0        0        0     1600 2023-05-11 15:45:21.000000 irails-1.3.20/irails/scripts/_run.py
--rw-rw-rw-   0        0        0     2288 2023-05-11 14:15:32.000000 irails-1.3.20/irails/scripts/_shell.py
--rw-rw-rw-   0        0        0     4130 2023-05-20 08:45:35.000000 irails-1.3.20/irails/scripts/_test.py
--rw-rw-rw-   0        0        0     2900 2023-05-21 08:16:21.000000 irails-1.3.20/irails/scripts/main.py
-drwxrwxrwx   0        0        0        0 2023-05-21 08:56:37.556843 irails-1.3.20/irails/scripts/tpls/
-drwxrwxrwx   0        0        0        0 2023-05-21 08:56:37.636317 irails-1.3.20/irails/scripts/tpls/app/
--rw-rw-rw-   0        0        0      223 2023-05-09 15:18:47.000000 irails-1.3.20/irails/scripts/tpls/app/controller.tpl
--rw-rw-rw-   0        0        0        0 2023-04-28 06:03:05.000000 irails-1.3.20/irails/scripts/tpls/app/css.tpl
--rw-rw-rw-   0        0        0      791 2023-04-25 10:42:10.000000 irails-1.3.20/irails/scripts/tpls/app/home.css.tpl
--rw-rw-rw-   0        0        0     1293 2023-05-05 10:16:42.000000 irails-1.3.20/irails/scripts/tpls/app/home.tpl
--rw-rw-rw-   0        0        0     1023 2023-05-19 12:27:03.000000 irails-1.3.20/irails/scripts/tpls/app/model.jinja
--rw-rw-rw-   0        0        0     1300 2023-05-20 14:09:55.000000 irails-1.3.20/irails/scripts/tpls/app/service.jinja
--rw-rw-rw-   0        0        0      237 2023-05-13 13:54:20.000000 irails-1.3.20/irails/scripts/tpls/app/test_controller.jinja
--rw-rw-rw-   0        0        0      893 2023-05-14 14:08:50.000000 irails-1.3.20/irails/scripts/tpls/app/test_service.jinja
--rw-rw-rw-   0        0        0       18 2023-05-02 08:56:04.000000 irails-1.3.20/irails/scripts/tpls/app/view.tpl
-drwxrwxrwx   0        0        0        0 2023-05-21 08:56:37.638312 irails-1.3.20/irails/scripts/tpls/project/
--rw-rw-rw-   0        0        0      139 2023-04-23 09:46:24.000000 irails-1.3.20/irails/scripts/tpls/project/.gitignore
-drwxrwxrwx   0        0        0        0 2023-05-21 08:56:37.639968 irails-1.3.20/irails/scripts/tpls/project/apps/
--rw-rw-rw-   0        0        0        0 2023-04-26 09:58:51.000000 irails-1.3.20/irails/scripts/tpls/project/apps/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-21 08:56:37.653239 irails-1.3.20/irails/scripts/tpls/project/configs/
--rw-rw-rw-   0        0        0      746 2023-05-09 06:45:34.000000 irails-1.3.20/irails/scripts/tpls/project/configs/alembic.ini
--rw-rw-rw-   0        0        0      179 2023-05-13 09:22:15.000000 irails-1.3.20/irails/scripts/tpls/project/configs/authencation.yaml
--rw-rw-rw-   0        0        0        0 2023-03-06 08:27:07.000000 irails-1.3.20/irails/scripts/tpls/project/configs/cache.yaml
--rw-rw-rw-   0        0        0      104 2023-05-04 05:06:32.000000 irails-1.3.20/irails/scripts/tpls/project/configs/casbin-adapter.csv
--rw-rw-rw-   0        0        0      302 2023-05-04 05:24:51.000000 irails-1.3.20/irails/scripts/tpls/project/configs/casbin-model.conf
-drwxrwxrwx   0        0        0        0 2023-05-21 08:56:37.668199 irails-1.3.20/irails/scripts/tpls/project/configs/casbin_templates/
--rw-rw-rw-   0        0        0      204 2023-05-18 07:46:03.000000 irails-1.3.20/irails/scripts/tpls/project/configs/casbin_templates/ALC.conf
--rw-rw-rw-   0        0        0       37 2023-05-18 07:46:03.000000 irails-1.3.20/irails/scripts/tpls/project/configs/casbin_templates/ALC.csv
--rw-rw-rw-   0        0        0      236 2023-05-18 07:46:03.000000 irails-1.3.20/irails/scripts/tpls/project/configs/casbin_templates/RBAC.conf
--rw-rw-rw-   0        0        0      125 2023-05-18 07:46:03.000000 irails-1.3.20/irails/scripts/tpls/project/configs/casbin_templates/RBAC.csv
--rw-rw-rw-   0        0        0      249 2023-05-18 07:46:03.000000 irails-1.3.20/irails/scripts/tpls/project/configs/casbin_templates/RBACR.conf
--rw-rw-rw-   0        0        0      159 2023-05-18 07:46:03.000000 irails-1.3.20/irails/scripts/tpls/project/configs/casbin_templates/RBACR.csv
--rw-rw-rw-   0        0        0      274 2023-05-18 07:46:03.000000 irails-1.3.20/irails/scripts/tpls/project/configs/casbin_templates/RBACT.conf
--rw-rw-rw-   0        0        0      178 2023-05-18 07:46:03.000000 irails-1.3.20/irails/scripts/tpls/project/configs/casbin_templates/RBACT.csv
--rw-rw-rw-   0        0        0      222 2023-05-18 07:46:03.000000 irails-1.3.20/irails/scripts/tpls/project/configs/casbin_templates/RESTFUL.conf
--rw-rw-rw-   0        0        0      152 2023-05-18 07:46:03.000000 irails-1.3.20/irails/scripts/tpls/project/configs/casbin_templates/RESTFUL.csv
--rw-rw-rw-   0        0        0      817 2023-05-10 10:45:36.000000 irails-1.3.20/irails/scripts/tpls/project/configs/database.yaml
--rw-rw-rw-   0        0        0      748 2023-05-11 05:35:06.000000 irails-1.3.20/irails/scripts/tpls/project/configs/general.yaml
--rw-rw-rw-   0        0        0      337 2023-04-22 10:54:12.000000 irails-1.3.20/irails/scripts/tpls/project/configs/session.yaml
--rw-rw-rw-   0        0        0      272 2023-05-09 06:44:59.000000 irails-1.3.20/irails/scripts/tpls/project/configs/upload.yaml
-drwxrwxrwx   0        0        0        0 2023-05-21 08:56:37.561829 irails-1.3.20/irails/scripts/tpls/project/data/
-drwxrwxrwx   0        0        0        0 2023-05-21 08:56:37.672190 irails-1.3.20/irails/scripts/tpls/project/data/alembic/
--rw-rw-rw-   0        0        0       38 2023-04-09 12:01:20.000000 irails-1.3.20/irails/scripts/tpls/project/data/alembic/README
--rw-rw-rw-   0        0        0     2144 2023-04-30 09:03:04.000000 irails-1.3.20/irails/scripts/tpls/project/data/alembic/env.py
--rw-rw-rw-   0        0        0      510 2023-04-09 12:01:20.000000 irails-1.3.20/irails/scripts/tpls/project/data/alembic/script.py.mako
--rw-rw-rw-   0        0        0      231 2023-05-11 15:42:13.000000 irails-1.3.20/irails/scripts/tpls/project/main.py
-drwxrwxrwx   0        0        0        0 2023-05-21 08:56:37.674187 irails-1.3.20/irails/scripts/tpls/project/public/
--rw-rw-rw-   0        0        0     1233 2023-05-02 08:46:22.000000 irails-1.3.20/irails/scripts/tpls/project/public/error_404.html
--rw-rw-rw-   0        0        0     1083 2023-05-02 08:46:46.000000 irails-1.3.20/irails/scripts/tpls/project/public/error_500.html
-drwxrwxrwx   0        0        0        0 2023-05-21 08:56:37.678175 irails-1.3.20/irails/scripts/tpls/project/public/libs/
-drwxrwxrwx   0        0        0        0 2023-05-21 08:56:37.565819 irails-1.3.20/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/
-drwxrwxrwx   0        0        0        0 2023-05-21 08:56:37.681164 irails-1.3.20/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/
--rw-rw-rw-   0        0        0  1970121 2023-04-23 08:02:36.000000 irails-1.3.20/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js
-drwxrwxrwx   0        0        0        0 2023-05-21 08:56:37.685154 irails-1.3.20/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/
--rw-rw-rw-   0        0        0   323666 2023-04-23 08:04:13.000000 irails-1.3.20/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css
--rw-rw-rw-   0        0        0      725 2023-04-21 12:39:53.000000 irails-1.3.20/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js
--rw-rw-rw-   0        0        0  1441055 2023-04-21 07:36:37.000000 irails-1.3.20/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js
-drwxrwxrwx   0        0        0        0 2023-05-21 08:56:37.567819 irails-1.3.20/irails/scripts/tpls/project/public/vue@3.2.36/
-drwxrwxrwx   0        0        0        0 2023-05-21 08:56:37.686151 irails-1.3.20/irails/scripts/tpls/project/public/vue@3.2.36/dist/
--rw-rw-rw-   0        0        0   640610 2023-04-21 07:36:07.000000 irails-1.3.20/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js
--rw-rw-rw-   0        0        0      866 2023-05-14 13:44:31.000000 irails-1.3.20/irails/unit_test.py
--rw-rw-rw-   0        0        0     3034 2023-05-16 08:15:25.000000 irails-1.3.20/irails/view.py
-drwxrwxrwx   0        0        0        0 2023-05-21 08:56:37.606180 irails-1.3.20/irails.egg-info/
--rw-rw-rw-   0        0        0     6224 2023-05-21 08:56:37.000000 irails-1.3.20/irails.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3115 2023-05-21 08:56:37.000000 irails-1.3.20/irails.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-21 08:56:37.000000 irails-1.3.20/irails.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-05-21 08:56:37.000000 irails-1.3.20/irails.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      360 2023-05-21 08:56:37.000000 irails-1.3.20/irails.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-21 08:56:37.000000 irails-1.3.20/irails.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-21 08:56:37.689959 irails-1.3.20/setup.cfg
--rw-rw-rw-   0        0        0     2551 2023-05-09 11:27:27.000000 irails-1.3.20/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-21 14:43:30.252108 irails-1.3.21/
+-rw-rw-rw-   0        0        0       83 2023-05-04 04:10:30.000000 irails-1.3.21/MANIFEST.in
+-rw-rw-rw-   0        0        0     6224 2023-05-21 14:43:30.251109 irails-1.3.21/PKG-INFO
+-rw-rw-rw-   0        0        0     5440 2023-05-21 08:50:53.000000 irails-1.3.21/README.md
+drwxrwxrwx   0        0        0        0 2023-05-21 14:43:30.159736 irails-1.3.21/irails/
+-rw-rw-rw-   0        0        0      307 2023-05-21 14:43:14.000000 irails-1.3.21/irails/__init__.py
+-rw-rw-rw-   0        0        0     4887 2023-05-21 14:33:24.000000 irails-1.3.21/irails/_i18n.py
+-rw-rw-rw-   0        0        0     2878 2023-05-21 08:27:23.000000 irails-1.3.21/irails/_loader.py
+-rw-rw-rw-   0        0        0     5253 2023-05-20 14:13:50.000000 irails-1.3.21/irails/_utils.py
+-rw-rw-rw-   0        0        0    12042 2023-05-20 06:44:17.000000 irails-1.3.21/irails/auth.py
+-rw-rw-rw-   0        0        0    12705 2023-05-18 07:46:03.000000 irails-1.3.21/irails/base_controller.py
+drwxrwxrwx   0        0        0        0 2023-05-21 14:43:30.168036 irails-1.3.21/irails/casbin_adapters/
+drwxrwxrwx   0        0        0        0 2023-05-21 14:43:30.169034 irails-1.3.21/irails/casbin_adapters/__pycache__/
+-rw-rw-rw-   0        0        0    17834 2023-04-30 14:29:09.000000 irails-1.3.21/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc
+-rw-rw-rw-   0        0        0    10589 2023-05-13 05:03:07.000000 irails-1.3.21/irails/casbin_adapters/sqlalchemy_adapter.py
+-rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 irails-1.3.21/irails/cbv.py
+-rw-rw-rw-   0        0        0     6174 2023-05-19 07:06:13.000000 irails-1.3.21/irails/config.py
+-rw-rw-rw-   0        0        0    12478 2023-05-12 05:56:24.000000 irails-1.3.21/irails/controller_utils.py
+-rw-rw-rw-   0        0        0    24918 2023-05-19 11:59:51.000000 irails-1.3.21/irails/core.py
+-rw-rw-rw-   0        0        0    14606 2023-05-21 14:41:11.000000 irails-1.3.21/irails/database.py
+-rw-rw-rw-   0        0        0     1459 2023-05-11 15:27:11.000000 irails-1.3.21/irails/log.py
+-rw-rw-rw-   0        0        0     8736 2023-05-21 14:38:31.000000 irails-1.3.21/irails/midware.py
+-rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 irails-1.3.21/irails/midware_casbin.py
+-rw-rw-rw-   0        0        0     9103 2023-05-16 08:16:43.000000 irails-1.3.21/irails/midware_session.py
+-rw-rw-rw-   0        0        0     4208 2023-05-16 08:12:27.000000 irails-1.3.21/irails/mvc_router.py
+drwxrwxrwx   0        0        0        0 2023-05-21 14:43:30.185989 irails-1.3.21/irails/scripts/
+-rw-rw-rw-   0        0        0        0 2023-04-26 07:44:41.000000 irails-1.3.21/irails/scripts/__init__.py
+-rw-rw-rw-   0        0        0     7862 2023-05-13 15:04:27.000000 irails-1.3.21/irails/scripts/_app.py
+-rw-rw-rw-   0        0        0     6892 2023-05-19 07:21:20.000000 irails-1.3.21/irails/scripts/_controller.py
+-rw-rw-rw-   0        0        0     7763 2023-05-21 13:57:03.000000 irails-1.3.21/irails/scripts/_i18n.py
+-rw-rw-rw-   0        0        0     1332 2023-05-21 08:39:33.000000 irails-1.3.21/irails/scripts/_migrate.py
+-rw-rw-rw-   0        0        0     3774 2023-05-14 13:34:33.000000 irails-1.3.21/irails/scripts/_model.py
+-rw-rw-rw-   0        0        0     2301 2023-05-03 14:35:33.000000 irails-1.3.21/irails/scripts/_project.py
+-rw-rw-rw-   0        0        0     1600 2023-05-11 15:45:21.000000 irails-1.3.21/irails/scripts/_run.py
+-rw-rw-rw-   0        0        0     2288 2023-05-11 14:15:32.000000 irails-1.3.21/irails/scripts/_shell.py
+-rw-rw-rw-   0        0        0     4930 2023-05-21 14:27:15.000000 irails-1.3.21/irails/scripts/_test.py
+-rw-rw-rw-   0        0        0     2900 2023-05-21 08:16:21.000000 irails-1.3.21/irails/scripts/main.py
+drwxrwxrwx   0        0        0        0 2023-05-21 14:43:30.125070 irails-1.3.21/irails/scripts/tpls/
+drwxrwxrwx   0        0        0        0 2023-05-21 14:43:30.199379 irails-1.3.21/irails/scripts/tpls/app/
+-rw-rw-rw-   0        0        0      223 2023-05-09 15:18:47.000000 irails-1.3.21/irails/scripts/tpls/app/controller.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-28 06:03:05.000000 irails-1.3.21/irails/scripts/tpls/app/css.tpl
+-rw-rw-rw-   0        0        0      791 2023-04-25 10:42:10.000000 irails-1.3.21/irails/scripts/tpls/app/home.css.tpl
+-rw-rw-rw-   0        0        0     1293 2023-05-05 10:16:42.000000 irails-1.3.21/irails/scripts/tpls/app/home.tpl
+-rw-rw-rw-   0        0        0     1023 2023-05-19 12:27:03.000000 irails-1.3.21/irails/scripts/tpls/app/model.jinja
+-rw-rw-rw-   0        0        0     1300 2023-05-20 14:09:55.000000 irails-1.3.21/irails/scripts/tpls/app/service.jinja
+-rw-rw-rw-   0        0        0      237 2023-05-13 13:54:20.000000 irails-1.3.21/irails/scripts/tpls/app/test_controller.jinja
+-rw-rw-rw-   0        0        0      893 2023-05-14 14:08:50.000000 irails-1.3.21/irails/scripts/tpls/app/test_service.jinja
+-rw-rw-rw-   0        0        0       18 2023-05-02 08:56:04.000000 irails-1.3.21/irails/scripts/tpls/app/view.tpl
+drwxrwxrwx   0        0        0        0 2023-05-21 14:43:30.201375 irails-1.3.21/irails/scripts/tpls/project/
+-rw-rw-rw-   0        0        0      139 2023-04-23 09:46:24.000000 irails-1.3.21/irails/scripts/tpls/project/.gitignore
+drwxrwxrwx   0        0        0        0 2023-05-21 14:43:30.203383 irails-1.3.21/irails/scripts/tpls/project/apps/
+-rw-rw-rw-   0        0        0        0 2023-04-26 09:58:51.000000 irails-1.3.21/irails/scripts/tpls/project/apps/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-21 14:43:30.215096 irails-1.3.21/irails/scripts/tpls/project/configs/
+-rw-rw-rw-   0        0        0      746 2023-05-09 06:45:34.000000 irails-1.3.21/irails/scripts/tpls/project/configs/alembic.ini
+-rw-rw-rw-   0        0        0      179 2023-05-13 09:22:15.000000 irails-1.3.21/irails/scripts/tpls/project/configs/authencation.yaml
+-rw-rw-rw-   0        0        0        0 2023-03-06 08:27:07.000000 irails-1.3.21/irails/scripts/tpls/project/configs/cache.yaml
+-rw-rw-rw-   0        0        0      104 2023-05-04 05:06:32.000000 irails-1.3.21/irails/scripts/tpls/project/configs/casbin-adapter.csv
+-rw-rw-rw-   0        0        0      302 2023-05-04 05:24:51.000000 irails-1.3.21/irails/scripts/tpls/project/configs/casbin-model.conf
+drwxrwxrwx   0        0        0        0 2023-05-21 14:43:30.229169 irails-1.3.21/irails/scripts/tpls/project/configs/casbin_templates/
+-rw-rw-rw-   0        0        0      204 2023-05-18 07:46:03.000000 irails-1.3.21/irails/scripts/tpls/project/configs/casbin_templates/ALC.conf
+-rw-rw-rw-   0        0        0       37 2023-05-18 07:46:03.000000 irails-1.3.21/irails/scripts/tpls/project/configs/casbin_templates/ALC.csv
+-rw-rw-rw-   0        0        0      236 2023-05-18 07:46:03.000000 irails-1.3.21/irails/scripts/tpls/project/configs/casbin_templates/RBAC.conf
+-rw-rw-rw-   0        0        0      125 2023-05-18 07:46:03.000000 irails-1.3.21/irails/scripts/tpls/project/configs/casbin_templates/RBAC.csv
+-rw-rw-rw-   0        0        0      249 2023-05-18 07:46:03.000000 irails-1.3.21/irails/scripts/tpls/project/configs/casbin_templates/RBACR.conf
+-rw-rw-rw-   0        0        0      159 2023-05-18 07:46:03.000000 irails-1.3.21/irails/scripts/tpls/project/configs/casbin_templates/RBACR.csv
+-rw-rw-rw-   0        0        0      274 2023-05-18 07:46:03.000000 irails-1.3.21/irails/scripts/tpls/project/configs/casbin_templates/RBACT.conf
+-rw-rw-rw-   0        0        0      178 2023-05-18 07:46:03.000000 irails-1.3.21/irails/scripts/tpls/project/configs/casbin_templates/RBACT.csv
+-rw-rw-rw-   0        0        0      222 2023-05-18 07:46:03.000000 irails-1.3.21/irails/scripts/tpls/project/configs/casbin_templates/RESTFUL.conf
+-rw-rw-rw-   0        0        0      152 2023-05-18 07:46:03.000000 irails-1.3.21/irails/scripts/tpls/project/configs/casbin_templates/RESTFUL.csv
+-rw-rw-rw-   0        0        0      817 2023-05-10 10:45:36.000000 irails-1.3.21/irails/scripts/tpls/project/configs/database.yaml
+-rw-rw-rw-   0        0        0      748 2023-05-11 05:35:06.000000 irails-1.3.21/irails/scripts/tpls/project/configs/general.yaml
+-rw-rw-rw-   0        0        0      337 2023-04-22 10:54:12.000000 irails-1.3.21/irails/scripts/tpls/project/configs/session.yaml
+-rw-rw-rw-   0        0        0      272 2023-05-09 06:44:59.000000 irails-1.3.21/irails/scripts/tpls/project/configs/upload.yaml
+drwxrwxrwx   0        0        0        0 2023-05-21 14:43:30.128058 irails-1.3.21/irails/scripts/tpls/project/data/
+drwxrwxrwx   0        0        0        0 2023-05-21 14:43:30.233158 irails-1.3.21/irails/scripts/tpls/project/data/alembic/
+-rw-rw-rw-   0        0        0       38 2023-04-09 12:01:20.000000 irails-1.3.21/irails/scripts/tpls/project/data/alembic/README
+-rw-rw-rw-   0        0        0     2144 2023-04-30 09:03:04.000000 irails-1.3.21/irails/scripts/tpls/project/data/alembic/env.py
+-rw-rw-rw-   0        0        0      510 2023-04-09 12:01:20.000000 irails-1.3.21/irails/scripts/tpls/project/data/alembic/script.py.mako
+-rw-rw-rw-   0        0        0      231 2023-05-11 15:42:13.000000 irails-1.3.21/irails/scripts/tpls/project/main.py
+drwxrwxrwx   0        0        0        0 2023-05-21 14:43:30.237148 irails-1.3.21/irails/scripts/tpls/project/public/
+-rw-rw-rw-   0        0        0     1233 2023-05-02 08:46:22.000000 irails-1.3.21/irails/scripts/tpls/project/public/error_404.html
+-rw-rw-rw-   0        0        0     1083 2023-05-02 08:46:46.000000 irails-1.3.21/irails/scripts/tpls/project/public/error_500.html
+drwxrwxrwx   0        0        0        0 2023-05-21 14:43:30.239142 irails-1.3.21/irails/scripts/tpls/project/public/libs/
+drwxrwxrwx   0        0        0        0 2023-05-21 14:43:30.131049 irails-1.3.21/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/
+drwxrwxrwx   0        0        0        0 2023-05-21 14:43:30.244129 irails-1.3.21/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/
+-rw-rw-rw-   0        0        0  1970121 2023-04-23 08:02:36.000000 irails-1.3.21/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js
+drwxrwxrwx   0        0        0        0 2023-05-21 14:43:30.247126 irails-1.3.21/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/
+-rw-rw-rw-   0        0        0   323666 2023-04-23 08:04:13.000000 irails-1.3.21/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css
+-rw-rw-rw-   0        0        0      725 2023-04-21 12:39:53.000000 irails-1.3.21/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js
+-rw-rw-rw-   0        0        0  1441055 2023-04-21 07:36:37.000000 irails-1.3.21/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js
+drwxrwxrwx   0        0        0        0 2023-05-21 14:43:30.132049 irails-1.3.21/irails/scripts/tpls/project/public/vue@3.2.36/
+drwxrwxrwx   0        0        0        0 2023-05-21 14:43:30.249115 irails-1.3.21/irails/scripts/tpls/project/public/vue@3.2.36/dist/
+-rw-rw-rw-   0        0        0   640610 2023-04-21 07:36:07.000000 irails-1.3.21/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js
+-rw-rw-rw-   0        0        0     1052 2023-05-21 13:45:32.000000 irails-1.3.21/irails/unit_test.py
+-rw-rw-rw-   0        0        0     3034 2023-05-16 08:15:25.000000 irails-1.3.21/irails/view.py
+drwxrwxrwx   0        0        0        0 2023-05-21 14:43:30.166038 irails-1.3.21/irails.egg-info/
+-rw-rw-rw-   0        0        0     6224 2023-05-21 14:43:29.000000 irails-1.3.21/irails.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3115 2023-05-21 14:43:29.000000 irails-1.3.21/irails.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-21 14:43:29.000000 irails-1.3.21/irails.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-05-21 14:43:29.000000 irails-1.3.21/irails.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      360 2023-05-21 14:43:29.000000 irails-1.3.21/irails.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-21 14:43:29.000000 irails-1.3.21/irails.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-21 14:43:30.253105 irails-1.3.21/setup.cfg
+-rw-rw-rw-   0        0        0     2551 2023-05-09 11:27:27.000000 irails-1.3.21/setup.py
```

### Comparing `irails-1.3.20/PKG-INFO` & `irails-1.3.21/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irails
-Version: 1.3.20
+Version: 1.3.21
 Summary: Simple and elegant use of FastApi in MVC mode
 Home-page: https://github.com/smjkzsl/irails
 Author: Bruce chou
 Author-email: smjkzsl@gmail.com
 License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `irails-1.3.20/README.md` & `irails-1.3.21/README.md`

 * *Files identical despite different names*

### Comparing `irails-1.3.20/irails/_i18n.py` & `irails-1.3.21/irails/_i18n.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import datetime
 import gettext
 import importlib  
 
 import os,sys
 import gettext
 from typing import Union
+
 _default_localedir = os.path.join(sys.base_prefix, 'share', 'locale')
 _old_find = gettext.find
 
 
 def load_module(module_name:str,module_path:str):
     if os.path.exists(module_path):
         spec = importlib.util.spec_from_file_location(module_name, module_path)
@@ -37,14 +38,37 @@
         if pod_time>mod_time: 
             do_mfgmft()
 # 获取当前模块的 ModuleSpec 实例
 # module_spec = importlib.util.find_spec(__name__)
 
 __all_trans = {}          
 default_langs = ['en','zh'] 
+
+def set_module_i18n(obj, module_name ):
+     
+    module = sys.modules[module_name]
+    module_package = module.__package__ 
+      
+    if module_package:
+        if module_package in sys.modules:
+            package_module = sys.modules[module_package]
+        
+            service_package_path =  package_module.__path__[0]
+            app_dirs = service_package_path.split(os.sep)
+        else: #test  mode
+            app_dirs = module_package.split(".")
+            service_package_path = os.path.dirname(module.__file__)
+        if len(app_dirs)>=2:
+            app_dirs = app_dirs[-2:]
+            setattr(obj,"__appdir__",".".join(app_dirs))
+            app_dir = os.path.dirname(service_package_path)
+            # auto set the i18n locales to the `app_name/locales`
+            t = load_app_translations(app_dir)
+            # setattr(obj,"_",t) #modify object
+            setattr(module,'_',t.gettext)
 def load_app_translations(module_dir,lan=None) -> gettext.GNUTranslations: 
     global __all_trans
     
     if  not lan:
         from .config import config
         cfg = config.get('i18n')
         if not cfg:
```

### Comparing `irails-1.3.20/irails/_loader.py` & `irails-1.3.21/irails/_loader.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.20/irails/_utils.py` & `irails-1.3.21/irails/_utils.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.20/irails/auth.py` & `irails-1.3.21/irails/auth.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.20/irails/base_controller.py` & `irails-1.3.21/irails/base_controller.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.20/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc` & `irails-1.3.21/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `irails-1.3.20/irails/casbin_adapters/sqlalchemy_adapter.py` & `irails-1.3.21/irails/casbin_adapters/sqlalchemy_adapter.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.20/irails/cbv.py` & `irails-1.3.21/irails/cbv.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.20/irails/config.py` & `irails-1.3.21/irails/config.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.20/irails/controller_utils.py` & `irails-1.3.21/irails/controller_utils.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.20/irails/core.py` & `irails-1.3.21/irails/core.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.20/irails/database.py` & `irails-1.3.21/irails/database.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,36 +1,75 @@
-from contextlib import contextmanager
-from sqlalchemy import DateTime, Integer, String, create_engine,Engine,MetaData, Table, Column, ForeignKey, func,select,join,TableClause,update
-from sqlalchemy.orm import DeclarativeBase,Session,sessionmaker,relationship,Query
-from sqlalchemy import text,TextClause,Table
-from sqlalchemy.ext.automap import automap_base
-
-from ._utils import camelize_classname,pluralize_collection
- 
-from alembic import command
-from alembic.config import Config
 import configparser
 import re,os,sys
-from typing import Dict, List, Type, Union
+from typing import Any, Dict, List, Type, Union
+from contextlib import contextmanager
+from sqlalchemy import (DateTime, Integer, 
+                        String, Text, 
+                        create_engine,
+                        Engine,
+                        MetaData, 
+                        Table, 
+                        Column, 
+                        ForeignKey, 
+                        func,
+                        select,join,
+                        TableClause,
+                        update,
+                        event,text,TextClause,Table)
+from sqlalchemy.orm import DeclarativeBase,Session,sessionmaker,relationship,Query 
+from sqlalchemy.ext.automap import automap_base 
+from ._utils import camelize_classname,pluralize_collection 
+from alembic import command
+from alembic.config import Config 
 from .log import _log
-from ._i18n import _,load_app_translations
+from ._i18n import _,set_module_i18n
 from .config import config,ROOT_PATH
 from ._utils import get_plural_name,get_singularize_name
+ 
+events={
+'before_insert', 
+'after_insert', 
+'before_update', 
+'after_update',
+'before_delete',
+'after_delete', 
+'before_attach',
+'after_attach', 
+'before_commit',
+'after_commit',
+'before_rollback',
+'after_rollback',
+'after_soft_delete',
+'after_bulk_update', 
+'after_bulk_delete',
+'before_flush', 
+'after_flush',
+}
 
+ 
 DataMap = None
 mapped_base = None
 engine:Engine=None 
 table_prefix=""
 cfg = config.get("database")
 if cfg:
     table_prefix = cfg.get("table_prefix","")
-class Base(DeclarativeBase):
+
+ 
+class Base( DeclarativeBase ):
     __abstract__ = True
     update_at = Column(DateTime(timezone=True), server_default=func.now(), onupdate=func.now())
     create_at = Column(DateTime(timezone=True), server_default=func.now())
+    i18n_json_data = Column(Text,server_default='{}',info={'json':True})
+    def __init_subclass__(cls,*args,**kwargs) -> None: 
+        for e in events:
+            if hasattr(cls,e):
+                event.listen(cls, e, getattr(cls,e)) 
+        set_module_i18n(cls,cls.__module__)
+        super().__init_subclass__(*args,**kwargs)
 class Relations():
     __all = {}
     @classmethod
     def M2M(self,Tb1:Base,Tb2:Base):
         '''
         set many to many relationship on :Tb1 and :Tb2\n
         :Tb1 will added attribute tb2_tablename(if it's not setted)\n
@@ -78,31 +117,17 @@
     pass
 
 
 
  
 class _serviceMeta(type):
     def __new__(cls, name, bases, attrs):
-        module_name = attrs['__module__']
-        module = sys.modules[module_name]
-        module_package = module.__package__ 
-                
-        # print(f"Creating class {name} in module {module_name}")
         obj = super().__new__(cls, name, bases, attrs)
-        if module_package:
-            package_module = sys.modules[module_package]
-            service_package_path =  package_module.__path__[0]
-            app_dirs = service_package_path.split(os.sep)
-            if len(app_dirs)>2:
-                app_dirs = app_dirs[-2:]
-                setattr(obj,"__appdir__",".".join(app_dirs))
-                app_dir = os.path.dirname(service_package_path)
-                # auto set the i18n locales to the `app_name/locales`
-                t = load_app_translations(app_dir)
-                setattr(obj,"_",t) #modify object
+        if obj.__name__!="Service":
+            set_module_i18n(obj=obj,module_name=attrs['__module__'])
         return obj
 
 class Service(metaclass=_serviceMeta):
     __all_generated = {}
     engine:Engine = engine
     _ = _ #the i18n traslation object ,it's will auto redirect the `app_name/locales` dir i18n configure
     
@@ -338,15 +363,16 @@
     dbdecode = cfg.get('dbdecode')
     
      # Check if the database is sqlite and create the directory
     if uri.startswith('sqlite'):
         
         part = uri.split(':///')
         db_directory  = os.path.dirname(part[1])
-        db_directory = os.path.abspath(os.path.join(ROOT_PATH, db_directory))
+        if not os.path.isabs(db_directory):
+            db_directory = os.path.abspath(os.path.join(ROOT_PATH, db_directory))
         db_file = os.path.join(db_directory,os.path.basename(part[1]))
         cfg['uri'] = uri = f"sqlite:///{db_file}"
         os.makedirs(db_directory, exist_ok=True) 
      # Get the maptables and dbfirst configurations
     dbfirst = cfg.get("dbfirst") 
     maptables = cfg.get("maptables") #if configured, only the listed tables will be mapped
```

### Comparing `irails-1.3.20/irails/log.py` & `irails-1.3.21/irails/log.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.20/irails/midware.py` & `irails-1.3.21/irails/midware.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     request_validation_exception_handler,
 )
 from fastapi.exceptions import RequestValidationError
 from starlette.exceptions import HTTPException as StarletteHTTPException
 import traceback
 
 from starlette.staticfiles import PathLike
-from .config import config
+from .config import config,ROOT_PATH
 from .log import _log
 from .midware_session import (SessionMiddleware,FileStorage,MemoryStorage,RedisStorage,SessionStorage,_SESSION_STORAGES)
 from fastapi.middleware.cors import CORSMiddleware
 from starlette.types import   Scope 
 from .view import _View,env_configs,static_format
 from .config import config,ROOT_PATH
 
@@ -88,15 +88,16 @@
         else:
             if not _url.endswith("/"):_url+="/"
             _url = _url.lower()
             if debug:
                 _log.info(f"StaticDir:{_dir} mounted: {_url}")
             app.mount(_url,MvcStaticFiles(directory=_dir),name=_dir)       
     #mount public resources
-    public_dir =  os.path.abspath(config.get("public_dir"))
+    public_dir =  config.get("public_dir") 
+    public_dir = os.path.abspath(os.path.join(ROOT_PATH,public_dir))
     if not os.path.exists(public_dir):
         os.makedirs(public_dir) 
     app.mount('/public/',  MvcStaticFiles(directory=public_dir), name='public') 
     
     if config.get("upload"):
             updir = config.get("upload")['dir'] or "uploads"
     else:
```

### Comparing `irails-1.3.20/irails/midware_casbin.py` & `irails-1.3.21/irails/midware_casbin.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.20/irails/midware_session.py` & `irails-1.3.21/irails/midware_session.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.20/irails/mvc_router.py` & `irails-1.3.21/irails/mvc_router.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.20/irails/scripts/_app.py` & `irails-1.3.21/irails/scripts/_app.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.20/irails/scripts/_controller.py` & `irails-1.3.21/irails/scripts/_controller.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.20/irails/scripts/_i18n.py` & `irails-1.3.21/irails/scripts/_i18n.py`

 * *Files 2% similar despite different names*

```diff
@@ -183,15 +183,15 @@
         
         if not os.path.exists(locales_path):
             os.makedirs(locales_path,exist_ok=True)
         if len(sys.argv)<2:
             if dev_mode:
                 sys.argv.append(cur_dir)
             else:
-                for d in ['controllers','services','models']:
+                for d in ['controllers','services','models','tests']:
                     sys.argv.append(d)
 
         if not '-o' in sys.argv:
             sys.argv.insert(1,'-o') 
             sys.argv.insert(2,f'{locales_path}{os.sep}messages.pot')
```

### Comparing `irails-1.3.20/irails/scripts/_migrate.py` & `irails-1.3.21/irails/scripts/_migrate.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.20/irails/scripts/_model.py` & `irails-1.3.21/irails/scripts/_model.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.20/irails/scripts/_project.py` & `irails-1.3.21/irails/scripts/_project.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.20/irails/scripts/_run.py` & `irails-1.3.21/irails/scripts/_run.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.20/irails/scripts/_shell.py` & `irails-1.3.21/irails/scripts/_shell.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.20/irails/scripts/_test.py` & `irails-1.3.21/irails/scripts/_test.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,79 +1,100 @@
+import argparse
 import importlib
 import unittest
 import os,sys
 from irails.config import is_in_app,is_in_irails,config
+from irails._i18n import set_module_i18n
 curdir = os.path.abspath(os.curdir)
 
 def load_module(module_name:str,module_path:str):
     if os.path.exists(module_path):
         spec = importlib.util.spec_from_file_location(module_name, module_path)
         module = importlib.util.module_from_spec(spec)
+        sys.modules[module_name] = module
         spec.loader.exec_module(module)
         return module
     return None
 def _get_tests(_root_path):
     all_files = {}
     for root, dirs, files in os.walk(os.path.join(_root_path,'tests')):
         for file in files:
             name,ext = os.path.splitext(file)
             file_path = os.path.join(root, file)
             if file.endswith('.py') and file.startswith('test_'):
                 all_files[name] = file_path
     return all_files
-def do_test_app(app_dir, print_out):
+def do_test_app(app_dir, print_out=None):
     
     test_files = _get_tests(app_dir)
+    app_package = os.path.basename(app_dir)
+    app_package_dir = os.path.dirname(app_dir)
+    if not app_package_dir in sys.path:
+        sys.path.insert(0,app_package_dir)
     for name in test_files:
         print(f"Starting test {test_files[name]}")
-        module = load_module(name,test_files[name])
+        module = load_module(f"{app_package}.tests.{name}",test_files[name])
+        
         if module:
+            
+            set_module_i18n(module,f"{app_package}.tests.{name}")
             sys.argv = [test_files[name]]
-            unittest.main(module=module,exit=False,buffer=print_out )
-    
+            kwargs = {'module':module,'exit':False}
+            if print_out:
+                kwargs['buffer']=print_out
+            unittest.main(**kwargs)
     
+    sys.path.remove(app_package_dir)
 def get_all_enabled_apps():
     from irails._loader import _load_apps
     apps = _load_apps(do_load=False)
     return apps
-def do_test_project(print_out): 
-    _old_stdout = sys.stdout
-    _old_stderr = sys.stderr
-    sys.stdout = sys.__stdout__
-    sys.stderr = sys.__stderr__
+def do_test_project(print_out=None): 
+     
     response = input("Do you want to continue to test all apps? (y/n)")
     if response.lower() == "y":
-        sys.stdout = _old_stdout
-        sys.stderr = _old_stderr
+         
         apps = get_all_enabled_apps() 
         for app in apps:
             dirs = app.split('.')
             if len(dirs)==2:
                 app_dir = os.path.join(curdir,dirs[0],dirs[1])
                 do_test_app(app_dir=app_dir, print_out=print_out)
          
     elif response.lower() == "n":
         print("User chose to cancel.")
     else:
         print("Invalid input.")
-    sys.stdout = _old_stdout
-    sys.stderr = _old_stderr
+     
 def main():
+    self_file = os.path.basename(__file__).lstrip("_").replace(".py",'')
+    parser = argparse.ArgumentParser(
+        usage=f"{sys.argv[0]} {self_file} [-h] [--verbose]",
+          description='run project or app tests')
+    parser.add_argument('-v','--verbose',action='store_true', help="full verbose with testing")  
+    args = parser.parse_args()  
     import io
-    print_out = io.StringIO() 
-    sys.stdout = print_out
-    sys.stderr = print_out
+    print_out = io.StringIO() if not args.verbose else None
+    if print_out:
+        sys.stdout = print_out
+        sys.stderr = print_out
+    if args.verbose:
+        sys.argv.pop()
     try:
         if is_in_app(curdir):
             do_test_app(curdir,print_out)
         elif is_in_irails(curdir):
             do_test_project(print_out)
     except Exception as e:
         raise
-    if print_out:
+    sys.stdout = sys.__stdout__
+    sys.stderr = sys.__stderr__
+    if not print_out: 
+        return 0
+    else:
         import re
         pattern_starting = r"^Starting test .*$"
         pattern = r"Ran \d+ test in [\d\.]+s$" 
         result:str = print_out.getvalue()
         tested_line = []
         lines = result.split("\n")
         lnt = 0
@@ -102,13 +123,12 @@
             elif re.match(pattern=r"^FAIL:.*$", string=line) or re.match(pattern=r"^ERROR:",string=line)  :
                 if not matched_fail:
                     fail+=1
                 matched_fail=True
             elif  matched_fail:
                 tested_line.append(line) 
             lnt += 1
-    sys.stdout = sys.__stdout__
-    sys.stderr = sys.__stderr__
+    
     print("\n\ntest finished ,results:")
     print("====================================================")
     print("\n".join(tested_line))
     print(f"=========OK:{ok}====Fail:{fail}======================")
```

### Comparing `irails-1.3.20/irails/scripts/main.py` & `irails-1.3.21/irails/scripts/main.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.20/irails/scripts/tpls/app/home.css.tpl` & `irails-1.3.21/irails/scripts/tpls/app/home.css.tpl`

 * *Files identical despite different names*

### Comparing `irails-1.3.20/irails/scripts/tpls/app/home.tpl` & `irails-1.3.21/irails/scripts/tpls/app/home.tpl`

 * *Files identical despite different names*

### Comparing `irails-1.3.20/irails/scripts/tpls/app/model.jinja` & `irails-1.3.21/irails/scripts/tpls/app/model.jinja`

 * *Files identical despite different names*

### Comparing `irails-1.3.20/irails/scripts/tpls/app/service.jinja` & `irails-1.3.21/irails/scripts/tpls/app/service.jinja`

 * *Files identical despite different names*

### Comparing `irails-1.3.20/irails/scripts/tpls/app/test_service.jinja` & `irails-1.3.21/irails/scripts/tpls/app/test_service.jinja`

 * *Files identical despite different names*

### Comparing `irails-1.3.20/irails/scripts/tpls/project/configs/alembic.ini` & `irails-1.3.21/irails/scripts/tpls/project/configs/alembic.ini`

 * *Files identical despite different names*

### Comparing `irails-1.3.20/irails/scripts/tpls/project/configs/database.yaml` & `irails-1.3.21/irails/scripts/tpls/project/configs/database.yaml`

 * *Files identical despite different names*

### Comparing `irails-1.3.20/irails/scripts/tpls/project/configs/general.yaml` & `irails-1.3.21/irails/scripts/tpls/project/configs/general.yaml`

 * *Files identical despite different names*

### Comparing `irails-1.3.20/irails/scripts/tpls/project/data/alembic/env.py` & `irails-1.3.21/irails/scripts/tpls/project/data/alembic/env.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.20/irails/scripts/tpls/project/public/error_404.html` & `irails-1.3.21/irails/scripts/tpls/project/public/error_404.html`

 * *Files identical despite different names*

### Comparing `irails-1.3.20/irails/scripts/tpls/project/public/error_500.html` & `irails-1.3.21/irails/scripts/tpls/project/public/error_500.html`

 * *Files identical despite different names*

### Comparing `irails-1.3.20/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js` & `irails-1.3.21/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.20/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css` & `irails-1.3.21/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css`

 * *Files identical despite different names*

### Comparing `irails-1.3.20/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js` & `irails-1.3.21/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.20/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js` & `irails-1.3.21/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.20/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js` & `irails-1.3.21/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.20/irails/unit_test.py` & `irails-1.3.21/irails/unit_test.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,19 @@
 
 import unittest
 from .core import generate_mvc_app
+from ._i18n import set_module_i18n
+
 class _BaseUnitTest(unittest.TestCase):
     application = generate_mvc_app()
     def __init__(self,*args,**kwargv) -> None:
         super().__init__(*args,**kwargv)
-        
+    def __init_subclass__(cls,*args,**kwargs) -> None:  
+        set_module_i18n(cls,cls.__module__)
+        super().__init_subclass__(*args,**kwargs)    
 class ControllerTest(_BaseUnitTest):
     def __init__(self,*args,**kwargv) -> None:
         super().__init__(*args,**kwargv)
         from fastapi.testclient import TestClient 
         self.client = TestClient(app=self.application)
         
     pass
```

### Comparing `irails-1.3.20/irails/view.py` & `irails-1.3.21/irails/view.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.20/irails.egg-info/PKG-INFO` & `irails-1.3.21/irails.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irails
-Version: 1.3.20
+Version: 1.3.21
 Summary: Simple and elegant use of FastApi in MVC mode
 Home-page: https://github.com/smjkzsl/irails
 Author: Bruce chou
 Author-email: smjkzsl@gmail.com
 License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `irails-1.3.20/irails.egg-info/SOURCES.txt` & `irails-1.3.21/irails.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `irails-1.3.20/setup.py` & `irails-1.3.21/setup.py`

 * *Files identical despite different names*

