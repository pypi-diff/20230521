# Comparing `tmp/irails-1.3.19.tar.gz` & `tmp/irails-1.3.20.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irails-1.3.19.tar", last modified: Sat May 20 12:05:31 2023, max compression
+gzip compressed data, was "irails-1.3.20.tar", last modified: Sun May 21 08:56:37 2023, max compression
```

## Comparing `irails-1.3.19.tar` & `irails-1.3.20.tar`

### file list

```diff
@@ -1,103 +1,104 @@
-drwxrwxrwx   0        0        0        0 2023-05-20 12:05:31.120375 irails-1.3.19/
--rw-rw-rw-   0        0        0       83 2023-05-04 04:10:30.000000 irails-1.3.19/MANIFEST.in
--rw-rw-rw-   0        0        0     6172 2023-05-20 12:05:31.119084 irails-1.3.19/PKG-INFO
--rw-rw-rw-   0        0        0     5388 2023-05-18 08:26:27.000000 irails-1.3.19/README.md
-drwxrwxrwx   0        0        0        0 2023-05-20 12:05:31.034384 irails-1.3.19/irails/
--rw-rw-rw-   0        0        0      307 2023-05-20 12:05:11.000000 irails-1.3.19/irails/__init__.py
--rw-rw-rw-   0        0        0     3948 2023-05-18 07:35:56.000000 irails-1.3.19/irails/_i18n.py
--rw-rw-rw-   0        0        0     2875 2023-05-19 11:46:57.000000 irails-1.3.19/irails/_loader.py
--rw-rw-rw-   0        0        0     5073 2023-05-19 15:28:59.000000 irails-1.3.19/irails/_utils.py
--rw-rw-rw-   0        0        0    12042 2023-05-20 06:44:17.000000 irails-1.3.19/irails/auth.py
--rw-rw-rw-   0        0        0    12705 2023-05-18 07:46:03.000000 irails-1.3.19/irails/base_controller.py
-drwxrwxrwx   0        0        0        0 2023-05-20 12:05:31.043361 irails-1.3.19/irails/casbin_adapters/
-drwxrwxrwx   0        0        0        0 2023-05-20 12:05:31.044363 irails-1.3.19/irails/casbin_adapters/__pycache__/
--rw-rw-rw-   0        0        0    17834 2023-04-30 14:29:09.000000 irails-1.3.19/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc
--rw-rw-rw-   0        0        0    10589 2023-05-13 05:03:07.000000 irails-1.3.19/irails/casbin_adapters/sqlalchemy_adapter.py
--rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 irails-1.3.19/irails/cbv.py
--rw-rw-rw-   0        0        0     6174 2023-05-19 07:06:13.000000 irails-1.3.19/irails/config.py
--rw-rw-rw-   0        0        0    12478 2023-05-12 05:56:24.000000 irails-1.3.19/irails/controller_utils.py
--rw-rw-rw-   0        0        0    24918 2023-05-19 11:59:51.000000 irails-1.3.19/irails/core.py
--rw-rw-rw-   0        0        0    13243 2023-05-20 11:48:25.000000 irails-1.3.19/irails/database.py
--rw-rw-rw-   0        0        0     1459 2023-05-11 15:27:11.000000 irails-1.3.19/irails/log.py
--rw-rw-rw-   0        0        0     8672 2023-05-13 15:15:01.000000 irails-1.3.19/irails/midware.py
--rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 irails-1.3.19/irails/midware_casbin.py
--rw-rw-rw-   0        0        0     9103 2023-05-16 08:16:43.000000 irails-1.3.19/irails/midware_session.py
--rw-rw-rw-   0        0        0     4208 2023-05-16 08:12:27.000000 irails-1.3.19/irails/mvc_router.py
-drwxrwxrwx   0        0        0        0 2023-05-20 12:05:31.056327 irails-1.3.19/irails/scripts/
--rw-rw-rw-   0        0        0        0 2023-04-26 07:44:41.000000 irails-1.3.19/irails/scripts/__init__.py
--rw-rw-rw-   0        0        0     7862 2023-05-13 15:04:27.000000 irails-1.3.19/irails/scripts/_app.py
--rw-rw-rw-   0        0        0     6892 2023-05-19 07:21:20.000000 irails-1.3.19/irails/scripts/_controller.py
--rw-rw-rw-   0        0        0     7755 2023-05-13 05:57:18.000000 irails-1.3.19/irails/scripts/_i18n.py
--rw-rw-rw-   0        0        0     3774 2023-05-14 13:34:33.000000 irails-1.3.19/irails/scripts/_model.py
--rw-rw-rw-   0        0        0     2301 2023-05-03 14:35:33.000000 irails-1.3.19/irails/scripts/_project.py
--rw-rw-rw-   0        0        0     1600 2023-05-11 15:45:21.000000 irails-1.3.19/irails/scripts/_run.py
--rw-rw-rw-   0        0        0     2288 2023-05-11 14:15:32.000000 irails-1.3.19/irails/scripts/_shell.py
--rw-rw-rw-   0        0        0     4130 2023-05-20 08:45:35.000000 irails-1.3.19/irails/scripts/_test.py
--rw-rw-rw-   0        0        0     2431 2023-05-20 09:01:43.000000 irails-1.3.19/irails/scripts/main.py
-drwxrwxrwx   0        0        0        0 2023-05-20 12:05:30.999179 irails-1.3.19/irails/scripts/tpls/
-drwxrwxrwx   0        0        0        0 2023-05-20 12:05:31.068294 irails-1.3.19/irails/scripts/tpls/app/
--rw-rw-rw-   0        0        0      223 2023-05-09 15:18:47.000000 irails-1.3.19/irails/scripts/tpls/app/controller.tpl
--rw-rw-rw-   0        0        0        0 2023-04-28 06:03:05.000000 irails-1.3.19/irails/scripts/tpls/app/css.tpl
--rw-rw-rw-   0        0        0      791 2023-04-25 10:42:10.000000 irails-1.3.19/irails/scripts/tpls/app/home.css.tpl
--rw-rw-rw-   0        0        0     1293 2023-05-05 10:16:42.000000 irails-1.3.19/irails/scripts/tpls/app/home.tpl
--rw-rw-rw-   0        0        0     1023 2023-05-19 12:27:03.000000 irails-1.3.19/irails/scripts/tpls/app/model.jinja
--rw-rw-rw-   0        0        0      658 2023-05-20 10:49:39.000000 irails-1.3.19/irails/scripts/tpls/app/service.jinja
--rw-rw-rw-   0        0        0      237 2023-05-13 13:54:20.000000 irails-1.3.19/irails/scripts/tpls/app/test_controller.jinja
--rw-rw-rw-   0        0        0      893 2023-05-14 14:08:50.000000 irails-1.3.19/irails/scripts/tpls/app/test_service.jinja
--rw-rw-rw-   0        0        0       18 2023-05-02 08:56:04.000000 irails-1.3.19/irails/scripts/tpls/app/view.tpl
-drwxrwxrwx   0        0        0        0 2023-05-20 12:05:31.070289 irails-1.3.19/irails/scripts/tpls/project/
--rw-rw-rw-   0        0        0      139 2023-04-23 09:46:24.000000 irails-1.3.19/irails/scripts/tpls/project/.gitignore
-drwxrwxrwx   0        0        0        0 2023-05-20 12:05:31.071286 irails-1.3.19/irails/scripts/tpls/project/apps/
--rw-rw-rw-   0        0        0        0 2023-04-26 09:58:51.000000 irails-1.3.19/irails/scripts/tpls/project/apps/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-20 12:05:31.082257 irails-1.3.19/irails/scripts/tpls/project/configs/
--rw-rw-rw-   0        0        0      746 2023-05-09 06:45:34.000000 irails-1.3.19/irails/scripts/tpls/project/configs/alembic.ini
--rw-rw-rw-   0        0        0      179 2023-05-13 09:22:15.000000 irails-1.3.19/irails/scripts/tpls/project/configs/authencation.yaml
--rw-rw-rw-   0        0        0        0 2023-03-06 08:27:07.000000 irails-1.3.19/irails/scripts/tpls/project/configs/cache.yaml
--rw-rw-rw-   0        0        0      104 2023-05-04 05:06:32.000000 irails-1.3.19/irails/scripts/tpls/project/configs/casbin-adapter.csv
--rw-rw-rw-   0        0        0      302 2023-05-04 05:24:51.000000 irails-1.3.19/irails/scripts/tpls/project/configs/casbin-model.conf
-drwxrwxrwx   0        0        0        0 2023-05-20 12:05:31.097216 irails-1.3.19/irails/scripts/tpls/project/configs/casbin_templates/
--rw-rw-rw-   0        0        0      204 2023-05-18 07:46:03.000000 irails-1.3.19/irails/scripts/tpls/project/configs/casbin_templates/ALC.conf
--rw-rw-rw-   0        0        0       37 2023-05-18 07:46:03.000000 irails-1.3.19/irails/scripts/tpls/project/configs/casbin_templates/ALC.csv
--rw-rw-rw-   0        0        0      236 2023-05-18 07:46:03.000000 irails-1.3.19/irails/scripts/tpls/project/configs/casbin_templates/RBAC.conf
--rw-rw-rw-   0        0        0      125 2023-05-18 07:46:03.000000 irails-1.3.19/irails/scripts/tpls/project/configs/casbin_templates/RBAC.csv
--rw-rw-rw-   0        0        0      249 2023-05-18 07:46:03.000000 irails-1.3.19/irails/scripts/tpls/project/configs/casbin_templates/RBACR.conf
--rw-rw-rw-   0        0        0      159 2023-05-18 07:46:03.000000 irails-1.3.19/irails/scripts/tpls/project/configs/casbin_templates/RBACR.csv
--rw-rw-rw-   0        0        0      274 2023-05-18 07:46:03.000000 irails-1.3.19/irails/scripts/tpls/project/configs/casbin_templates/RBACT.conf
--rw-rw-rw-   0        0        0      178 2023-05-18 07:46:03.000000 irails-1.3.19/irails/scripts/tpls/project/configs/casbin_templates/RBACT.csv
--rw-rw-rw-   0        0        0      222 2023-05-18 07:46:03.000000 irails-1.3.19/irails/scripts/tpls/project/configs/casbin_templates/RESTFUL.conf
--rw-rw-rw-   0        0        0      152 2023-05-18 07:46:03.000000 irails-1.3.19/irails/scripts/tpls/project/configs/casbin_templates/RESTFUL.csv
--rw-rw-rw-   0        0        0      817 2023-05-10 10:45:36.000000 irails-1.3.19/irails/scripts/tpls/project/configs/database.yaml
--rw-rw-rw-   0        0        0      748 2023-05-11 05:35:06.000000 irails-1.3.19/irails/scripts/tpls/project/configs/general.yaml
--rw-rw-rw-   0        0        0      337 2023-04-22 10:54:12.000000 irails-1.3.19/irails/scripts/tpls/project/configs/session.yaml
--rw-rw-rw-   0        0        0      272 2023-05-09 06:44:59.000000 irails-1.3.19/irails/scripts/tpls/project/configs/upload.yaml
-drwxrwxrwx   0        0        0        0 2023-05-20 12:05:31.004584 irails-1.3.19/irails/scripts/tpls/project/data/
-drwxrwxrwx   0        0        0        0 2023-05-20 12:05:31.100208 irails-1.3.19/irails/scripts/tpls/project/data/alembic/
--rw-rw-rw-   0        0        0       38 2023-04-09 12:01:20.000000 irails-1.3.19/irails/scripts/tpls/project/data/alembic/README
--rw-rw-rw-   0        0        0     2144 2023-04-30 09:03:04.000000 irails-1.3.19/irails/scripts/tpls/project/data/alembic/env.py
--rw-rw-rw-   0        0        0      510 2023-04-09 12:01:20.000000 irails-1.3.19/irails/scripts/tpls/project/data/alembic/script.py.mako
--rw-rw-rw-   0        0        0      231 2023-05-11 15:42:13.000000 irails-1.3.19/irails/scripts/tpls/project/main.py
-drwxrwxrwx   0        0        0        0 2023-05-20 12:05:31.104198 irails-1.3.19/irails/scripts/tpls/project/public/
--rw-rw-rw-   0        0        0     1233 2023-05-02 08:46:22.000000 irails-1.3.19/irails/scripts/tpls/project/public/error_404.html
--rw-rw-rw-   0        0        0     1083 2023-05-02 08:46:46.000000 irails-1.3.19/irails/scripts/tpls/project/public/error_500.html
-drwxrwxrwx   0        0        0        0 2023-05-20 12:05:31.107116 irails-1.3.19/irails/scripts/tpls/project/public/libs/
-drwxrwxrwx   0        0        0        0 2023-05-20 12:05:31.008129 irails-1.3.19/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/
-drwxrwxrwx   0        0        0        0 2023-05-20 12:05:31.109110 irails-1.3.19/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/
--rw-rw-rw-   0        0        0  1970121 2023-04-23 08:02:36.000000 irails-1.3.19/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js
-drwxrwxrwx   0        0        0        0 2023-05-20 12:05:31.114099 irails-1.3.19/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/
--rw-rw-rw-   0        0        0   323666 2023-04-23 08:04:13.000000 irails-1.3.19/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css
--rw-rw-rw-   0        0        0      725 2023-04-21 12:39:53.000000 irails-1.3.19/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js
--rw-rw-rw-   0        0        0  1441055 2023-04-21 07:36:37.000000 irails-1.3.19/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js
-drwxrwxrwx   0        0        0        0 2023-05-20 12:05:31.009126 irails-1.3.19/irails/scripts/tpls/project/public/vue@3.2.36/
-drwxrwxrwx   0        0        0        0 2023-05-20 12:05:31.117092 irails-1.3.19/irails/scripts/tpls/project/public/vue@3.2.36/dist/
--rw-rw-rw-   0        0        0   640610 2023-04-21 07:36:07.000000 irails-1.3.19/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js
--rw-rw-rw-   0        0        0      866 2023-05-14 13:44:31.000000 irails-1.3.19/irails/unit_test.py
--rw-rw-rw-   0        0        0     3034 2023-05-16 08:15:25.000000 irails-1.3.19/irails/view.py
-drwxrwxrwx   0        0        0        0 2023-05-20 12:05:31.040368 irails-1.3.19/irails.egg-info/
--rw-rw-rw-   0        0        0     6172 2023-05-20 12:05:30.000000 irails-1.3.19/irails.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3088 2023-05-20 12:05:30.000000 irails-1.3.19/irails.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-20 12:05:30.000000 irails-1.3.19/irails.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-05-20 12:05:30.000000 irails-1.3.19/irails.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      360 2023-05-20 12:05:30.000000 irails-1.3.19/irails.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-20 12:05:30.000000 irails-1.3.19/irails.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-20 12:05:31.120375 irails-1.3.19/setup.cfg
--rw-rw-rw-   0        0        0     2551 2023-05-09 11:27:27.000000 irails-1.3.19/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-21 08:56:37.689959 irails-1.3.20/
+-rw-rw-rw-   0        0        0       83 2023-05-04 04:10:30.000000 irails-1.3.20/MANIFEST.in
+-rw-rw-rw-   0        0        0     6224 2023-05-21 08:56:37.688146 irails-1.3.20/PKG-INFO
+-rw-rw-rw-   0        0        0     5440 2023-05-21 08:50:53.000000 irails-1.3.20/README.md
+drwxrwxrwx   0        0        0        0 2023-05-21 08:56:37.599198 irails-1.3.20/irails/
+-rw-rw-rw-   0        0        0      307 2023-05-21 08:56:13.000000 irails-1.3.20/irails/__init__.py
+-rw-rw-rw-   0        0        0     3948 2023-05-18 07:35:56.000000 irails-1.3.20/irails/_i18n.py
+-rw-rw-rw-   0        0        0     2878 2023-05-21 08:27:23.000000 irails-1.3.20/irails/_loader.py
+-rw-rw-rw-   0        0        0     5253 2023-05-20 14:13:50.000000 irails-1.3.20/irails/_utils.py
+-rw-rw-rw-   0        0        0    12042 2023-05-20 06:44:17.000000 irails-1.3.20/irails/auth.py
+-rw-rw-rw-   0        0        0    12705 2023-05-18 07:46:03.000000 irails-1.3.20/irails/base_controller.py
+drwxrwxrwx   0        0        0        0 2023-05-21 08:56:37.609171 irails-1.3.20/irails/casbin_adapters/
+drwxrwxrwx   0        0        0        0 2023-05-21 08:56:37.611167 irails-1.3.20/irails/casbin_adapters/__pycache__/
+-rw-rw-rw-   0        0        0    17834 2023-04-30 14:29:09.000000 irails-1.3.20/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc
+-rw-rw-rw-   0        0        0    10589 2023-05-13 05:03:07.000000 irails-1.3.20/irails/casbin_adapters/sqlalchemy_adapter.py
+-rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 irails-1.3.20/irails/cbv.py
+-rw-rw-rw-   0        0        0     6174 2023-05-19 07:06:13.000000 irails-1.3.20/irails/config.py
+-rw-rw-rw-   0        0        0    12478 2023-05-12 05:56:24.000000 irails-1.3.20/irails/controller_utils.py
+-rw-rw-rw-   0        0        0    24918 2023-05-19 11:59:51.000000 irails-1.3.20/irails/core.py
+-rw-rw-rw-   0        0        0    14266 2023-05-21 08:48:41.000000 irails-1.3.20/irails/database.py
+-rw-rw-rw-   0        0        0     1459 2023-05-11 15:27:11.000000 irails-1.3.20/irails/log.py
+-rw-rw-rw-   0        0        0     8672 2023-05-13 15:15:01.000000 irails-1.3.20/irails/midware.py
+-rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 irails-1.3.20/irails/midware_casbin.py
+-rw-rw-rw-   0        0        0     9103 2023-05-16 08:16:43.000000 irails-1.3.20/irails/midware_session.py
+-rw-rw-rw-   0        0        0     4208 2023-05-16 08:12:27.000000 irails-1.3.20/irails/mvc_router.py
+drwxrwxrwx   0        0        0        0 2023-05-21 08:56:37.623039 irails-1.3.20/irails/scripts/
+-rw-rw-rw-   0        0        0        0 2023-04-26 07:44:41.000000 irails-1.3.20/irails/scripts/__init__.py
+-rw-rw-rw-   0        0        0     7862 2023-05-13 15:04:27.000000 irails-1.3.20/irails/scripts/_app.py
+-rw-rw-rw-   0        0        0     6892 2023-05-19 07:21:20.000000 irails-1.3.20/irails/scripts/_controller.py
+-rw-rw-rw-   0        0        0     7755 2023-05-13 05:57:18.000000 irails-1.3.20/irails/scripts/_i18n.py
+-rw-rw-rw-   0        0        0     1332 2023-05-21 08:39:33.000000 irails-1.3.20/irails/scripts/_migrate.py
+-rw-rw-rw-   0        0        0     3774 2023-05-14 13:34:33.000000 irails-1.3.20/irails/scripts/_model.py
+-rw-rw-rw-   0        0        0     2301 2023-05-03 14:35:33.000000 irails-1.3.20/irails/scripts/_project.py
+-rw-rw-rw-   0        0        0     1600 2023-05-11 15:45:21.000000 irails-1.3.20/irails/scripts/_run.py
+-rw-rw-rw-   0        0        0     2288 2023-05-11 14:15:32.000000 irails-1.3.20/irails/scripts/_shell.py
+-rw-rw-rw-   0        0        0     4130 2023-05-20 08:45:35.000000 irails-1.3.20/irails/scripts/_test.py
+-rw-rw-rw-   0        0        0     2900 2023-05-21 08:16:21.000000 irails-1.3.20/irails/scripts/main.py
+drwxrwxrwx   0        0        0        0 2023-05-21 08:56:37.556843 irails-1.3.20/irails/scripts/tpls/
+drwxrwxrwx   0        0        0        0 2023-05-21 08:56:37.636317 irails-1.3.20/irails/scripts/tpls/app/
+-rw-rw-rw-   0        0        0      223 2023-05-09 15:18:47.000000 irails-1.3.20/irails/scripts/tpls/app/controller.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-28 06:03:05.000000 irails-1.3.20/irails/scripts/tpls/app/css.tpl
+-rw-rw-rw-   0        0        0      791 2023-04-25 10:42:10.000000 irails-1.3.20/irails/scripts/tpls/app/home.css.tpl
+-rw-rw-rw-   0        0        0     1293 2023-05-05 10:16:42.000000 irails-1.3.20/irails/scripts/tpls/app/home.tpl
+-rw-rw-rw-   0        0        0     1023 2023-05-19 12:27:03.000000 irails-1.3.20/irails/scripts/tpls/app/model.jinja
+-rw-rw-rw-   0        0        0     1300 2023-05-20 14:09:55.000000 irails-1.3.20/irails/scripts/tpls/app/service.jinja
+-rw-rw-rw-   0        0        0      237 2023-05-13 13:54:20.000000 irails-1.3.20/irails/scripts/tpls/app/test_controller.jinja
+-rw-rw-rw-   0        0        0      893 2023-05-14 14:08:50.000000 irails-1.3.20/irails/scripts/tpls/app/test_service.jinja
+-rw-rw-rw-   0        0        0       18 2023-05-02 08:56:04.000000 irails-1.3.20/irails/scripts/tpls/app/view.tpl
+drwxrwxrwx   0        0        0        0 2023-05-21 08:56:37.638312 irails-1.3.20/irails/scripts/tpls/project/
+-rw-rw-rw-   0        0        0      139 2023-04-23 09:46:24.000000 irails-1.3.20/irails/scripts/tpls/project/.gitignore
+drwxrwxrwx   0        0        0        0 2023-05-21 08:56:37.639968 irails-1.3.20/irails/scripts/tpls/project/apps/
+-rw-rw-rw-   0        0        0        0 2023-04-26 09:58:51.000000 irails-1.3.20/irails/scripts/tpls/project/apps/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-21 08:56:37.653239 irails-1.3.20/irails/scripts/tpls/project/configs/
+-rw-rw-rw-   0        0        0      746 2023-05-09 06:45:34.000000 irails-1.3.20/irails/scripts/tpls/project/configs/alembic.ini
+-rw-rw-rw-   0        0        0      179 2023-05-13 09:22:15.000000 irails-1.3.20/irails/scripts/tpls/project/configs/authencation.yaml
+-rw-rw-rw-   0        0        0        0 2023-03-06 08:27:07.000000 irails-1.3.20/irails/scripts/tpls/project/configs/cache.yaml
+-rw-rw-rw-   0        0        0      104 2023-05-04 05:06:32.000000 irails-1.3.20/irails/scripts/tpls/project/configs/casbin-adapter.csv
+-rw-rw-rw-   0        0        0      302 2023-05-04 05:24:51.000000 irails-1.3.20/irails/scripts/tpls/project/configs/casbin-model.conf
+drwxrwxrwx   0        0        0        0 2023-05-21 08:56:37.668199 irails-1.3.20/irails/scripts/tpls/project/configs/casbin_templates/
+-rw-rw-rw-   0        0        0      204 2023-05-18 07:46:03.000000 irails-1.3.20/irails/scripts/tpls/project/configs/casbin_templates/ALC.conf
+-rw-rw-rw-   0        0        0       37 2023-05-18 07:46:03.000000 irails-1.3.20/irails/scripts/tpls/project/configs/casbin_templates/ALC.csv
+-rw-rw-rw-   0        0        0      236 2023-05-18 07:46:03.000000 irails-1.3.20/irails/scripts/tpls/project/configs/casbin_templates/RBAC.conf
+-rw-rw-rw-   0        0        0      125 2023-05-18 07:46:03.000000 irails-1.3.20/irails/scripts/tpls/project/configs/casbin_templates/RBAC.csv
+-rw-rw-rw-   0        0        0      249 2023-05-18 07:46:03.000000 irails-1.3.20/irails/scripts/tpls/project/configs/casbin_templates/RBACR.conf
+-rw-rw-rw-   0        0        0      159 2023-05-18 07:46:03.000000 irails-1.3.20/irails/scripts/tpls/project/configs/casbin_templates/RBACR.csv
+-rw-rw-rw-   0        0        0      274 2023-05-18 07:46:03.000000 irails-1.3.20/irails/scripts/tpls/project/configs/casbin_templates/RBACT.conf
+-rw-rw-rw-   0        0        0      178 2023-05-18 07:46:03.000000 irails-1.3.20/irails/scripts/tpls/project/configs/casbin_templates/RBACT.csv
+-rw-rw-rw-   0        0        0      222 2023-05-18 07:46:03.000000 irails-1.3.20/irails/scripts/tpls/project/configs/casbin_templates/RESTFUL.conf
+-rw-rw-rw-   0        0        0      152 2023-05-18 07:46:03.000000 irails-1.3.20/irails/scripts/tpls/project/configs/casbin_templates/RESTFUL.csv
+-rw-rw-rw-   0        0        0      817 2023-05-10 10:45:36.000000 irails-1.3.20/irails/scripts/tpls/project/configs/database.yaml
+-rw-rw-rw-   0        0        0      748 2023-05-11 05:35:06.000000 irails-1.3.20/irails/scripts/tpls/project/configs/general.yaml
+-rw-rw-rw-   0        0        0      337 2023-04-22 10:54:12.000000 irails-1.3.20/irails/scripts/tpls/project/configs/session.yaml
+-rw-rw-rw-   0        0        0      272 2023-05-09 06:44:59.000000 irails-1.3.20/irails/scripts/tpls/project/configs/upload.yaml
+drwxrwxrwx   0        0        0        0 2023-05-21 08:56:37.561829 irails-1.3.20/irails/scripts/tpls/project/data/
+drwxrwxrwx   0        0        0        0 2023-05-21 08:56:37.672190 irails-1.3.20/irails/scripts/tpls/project/data/alembic/
+-rw-rw-rw-   0        0        0       38 2023-04-09 12:01:20.000000 irails-1.3.20/irails/scripts/tpls/project/data/alembic/README
+-rw-rw-rw-   0        0        0     2144 2023-04-30 09:03:04.000000 irails-1.3.20/irails/scripts/tpls/project/data/alembic/env.py
+-rw-rw-rw-   0        0        0      510 2023-04-09 12:01:20.000000 irails-1.3.20/irails/scripts/tpls/project/data/alembic/script.py.mako
+-rw-rw-rw-   0        0        0      231 2023-05-11 15:42:13.000000 irails-1.3.20/irails/scripts/tpls/project/main.py
+drwxrwxrwx   0        0        0        0 2023-05-21 08:56:37.674187 irails-1.3.20/irails/scripts/tpls/project/public/
+-rw-rw-rw-   0        0        0     1233 2023-05-02 08:46:22.000000 irails-1.3.20/irails/scripts/tpls/project/public/error_404.html
+-rw-rw-rw-   0        0        0     1083 2023-05-02 08:46:46.000000 irails-1.3.20/irails/scripts/tpls/project/public/error_500.html
+drwxrwxrwx   0        0        0        0 2023-05-21 08:56:37.678175 irails-1.3.20/irails/scripts/tpls/project/public/libs/
+drwxrwxrwx   0        0        0        0 2023-05-21 08:56:37.565819 irails-1.3.20/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/
+drwxrwxrwx   0        0        0        0 2023-05-21 08:56:37.681164 irails-1.3.20/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/
+-rw-rw-rw-   0        0        0  1970121 2023-04-23 08:02:36.000000 irails-1.3.20/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js
+drwxrwxrwx   0        0        0        0 2023-05-21 08:56:37.685154 irails-1.3.20/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/
+-rw-rw-rw-   0        0        0   323666 2023-04-23 08:04:13.000000 irails-1.3.20/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css
+-rw-rw-rw-   0        0        0      725 2023-04-21 12:39:53.000000 irails-1.3.20/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js
+-rw-rw-rw-   0        0        0  1441055 2023-04-21 07:36:37.000000 irails-1.3.20/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js
+drwxrwxrwx   0        0        0        0 2023-05-21 08:56:37.567819 irails-1.3.20/irails/scripts/tpls/project/public/vue@3.2.36/
+drwxrwxrwx   0        0        0        0 2023-05-21 08:56:37.686151 irails-1.3.20/irails/scripts/tpls/project/public/vue@3.2.36/dist/
+-rw-rw-rw-   0        0        0   640610 2023-04-21 07:36:07.000000 irails-1.3.20/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js
+-rw-rw-rw-   0        0        0      866 2023-05-14 13:44:31.000000 irails-1.3.20/irails/unit_test.py
+-rw-rw-rw-   0        0        0     3034 2023-05-16 08:15:25.000000 irails-1.3.20/irails/view.py
+drwxrwxrwx   0        0        0        0 2023-05-21 08:56:37.606180 irails-1.3.20/irails.egg-info/
+-rw-rw-rw-   0        0        0     6224 2023-05-21 08:56:37.000000 irails-1.3.20/irails.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3115 2023-05-21 08:56:37.000000 irails-1.3.20/irails.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-21 08:56:37.000000 irails-1.3.20/irails.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-05-21 08:56:37.000000 irails-1.3.20/irails.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      360 2023-05-21 08:56:37.000000 irails-1.3.20/irails.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-21 08:56:37.000000 irails-1.3.20/irails.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-21 08:56:37.689959 irails-1.3.20/setup.cfg
+-rw-rw-rw-   0        0        0     2551 2023-05-09 11:27:27.000000 irails-1.3.20/setup.py
```

### Comparing `irails-1.3.19/PKG-INFO` & `irails-1.3.20/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irails
-Version: 1.3.19
+Version: 1.3.20
 Summary: Simple and elegant use of FastApi in MVC mode
 Home-page: https://github.com/smjkzsl/irails
 Author: Bruce chou
 Author-email: smjkzsl@gmail.com
 License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework
 Classifier: License :: OSI Approved :: Apache Software License
@@ -81,14 +81,15 @@
     |
     +---uploads                             ## Others dir(if your need or not)
 ```
 ## Extras commands
 * `irails i18n gettext`  --generate i18n in irails app dir
 * `irails shell`         --run python interpreter with buildin support contexts 
 * `irails test`          --run project tests 
+* `irails migrate`       --run database migrations
 
 ## Take a look configure file `general.yaml`
  
 ``` 
     app:
         appdir:
         - apps
```

### Comparing `irails-1.3.19/README.md` & `irails-1.3.20/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,15 @@
     |
     +---uploads                             ## Others dir(if your need or not)
 ```
 ## Extras commands
 * `irails i18n gettext`  --generate i18n in irails app dir
 * `irails shell`         --run python interpreter with buildin support contexts 
 * `irails test`          --run project tests 
+* `irails migrate`       --run database migrations
 
 ## Take a look configure file `general.yaml`
  
 ``` 
     app:
         appdir:
         - apps
```

### Comparing `irails-1.3.19/irails/_i18n.py` & `irails-1.3.20/irails/_i18n.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.19/irails/_loader.py` & `irails-1.3.20/irails/_loader.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         _log.info(_('Loading module:%s')%module_name)
         try:
             importlib.import_module(module_name) 
             if m=='controllers':
                 cnt += 1
         except ImportError as e:
             if m:#=='controllers':
-                _log.error(_("load app %s failed")%app_dir)
+                _log.error(_("load app %s failed")%module_name)
                 _log.error(e.args)
                 cnt -= 1
             else:
                 pass
     return cnt
 def _load_apps(debug=False,do_load:bool=True):
     global app_dirs,app_enabled
@@ -66,15 +66,15 @@
         app_list =  __list_directories(abs_app_dir)
         for app in app_list:
             if __check_if_enabled(app):  
                 if do_load:
                     #_dir = os.path.join(app_dir,app)
                     _abs_app_path =  abs_app_dir
                     if _abs_app_path not in sys.path:
-                        sys.path.insert(-1,_abs_app_path)
+                        sys.path.insert(0,_abs_app_path)
                     debug and print('load app:'+app)
                     n = _load_app(app)
                     if n:
                         loaded = loaded + 1
                     else:
                         unloaded = unloaded + 1
                 else:
```

### Comparing `irails-1.3.19/irails/_utils.py` & `irails-1.3.20/irails/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,36 +77,41 @@
     illegal_chars = set('/\\?%*:|"<>')
     if any(char in illegal_chars for char in filename):
         return False
     if ' ' in filename:
         return False
     return True
 
-def ensure_line(filepath, line_to_add):
+def ensure_line(filepath, line_to_add,create_if_not_exists=True):
     found = False
     lines = []
     if os.path.exists(filepath):
         # Read in the file
         with open(filepath, 'r') as file:
             lines = file.readlines()
 
             # Check if the line is already in the file
             for line in lines:
                 if line.strip() == line_to_add.strip():
                     found = True
                     break
+            if not found:# If the line is not in the file, add it
+                lines.append('\n' + line_to_add.strip() + '\n')
+                with open(filepath, 'w') as file:
+                    file.writelines(lines)
+                return True
     else:
-        with open(filepath,'w') as file:
-            file.write(line_to_add)
-        return True              
-    # If the line is not in the file, add it
-    if not found:
-        lines.append('\n' + line_to_add.strip() + '\n')
-        with open(filepath, 'w') as file:
-            file.writelines(lines)
+        if create_if_not_exists:
+            with open(filepath,'w') as file:
+                file.write(line_to_add)
+            return True  
+        else:
+            return False            
+    
+    
 _datetime_regex = re.compile(
 r'^\d{4}-\d{2}-\d{2}(T\d{2}:\d{2}:\d{2}(\.\d+)?(Z|[+-]\d{2}:\d{2})?)?$'
 )
 
 _date_regex = re.compile(r'^\d{4}-\d{2}-\d{2}$')
 
 _time_regex = re.compile(r'^\d{2}:\d{2}:\d{2}$')
```

### Comparing `irails-1.3.19/irails/auth.py` & `irails-1.3.20/irails/auth.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.19/irails/base_controller.py` & `irails-1.3.20/irails/base_controller.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.19/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc` & `irails-1.3.20/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `irails-1.3.19/irails/casbin_adapters/sqlalchemy_adapter.py` & `irails-1.3.20/irails/casbin_adapters/sqlalchemy_adapter.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.19/irails/cbv.py` & `irails-1.3.20/irails/cbv.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.19/irails/config.py` & `irails-1.3.20/irails/config.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.19/irails/controller_utils.py` & `irails-1.3.20/irails/controller_utils.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.19/irails/core.py` & `irails-1.3.20/irails/core.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.19/irails/database.py` & `irails-1.3.20/irails/database.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from contextlib import contextmanager
 from sqlalchemy import DateTime, Integer, String, create_engine,Engine,MetaData, Table, Column, ForeignKey, func,select,join,TableClause,update
-from sqlalchemy.orm import DeclarativeBase,Session,sessionmaker,relationship
+from sqlalchemy.orm import DeclarativeBase,Session,sessionmaker,relationship,Query
 from sqlalchemy import text,TextClause,Table
 from sqlalchemy.ext.automap import automap_base
 
 from ._utils import camelize_classname,pluralize_collection
  
 from alembic import command
 from alembic.config import Config
 import configparser
 import re,os,sys
 from typing import Dict, List, Type, Union
 from .log import _log
 from ._i18n import _,load_app_translations
-from .config import config
+from .config import config,ROOT_PATH
 from ._utils import get_plural_name,get_singularize_name
 
 DataMap = None
 mapped_base = None
 engine:Engine=None 
 table_prefix=""
 cfg = config.get("database")
@@ -114,14 +114,15 @@
             session_local = getattr(self,'_session_local')
         else:
             session_local =  sessionmaker(bind=engine)
             setattr(self,"_session_local", session_local) #cache sessionmaker object
         session = session_local()
         setattr(self,"_session",session)
         return session
+ 
     @classmethod
     def get(self,model:Base,id:int)->Base:
         return self.session().get(model,id)
     @classmethod
     def add(self,model:Union[Type,Base],**kwargs)->Base:
         if isinstance(model,Base):
             m=model
@@ -138,15 +139,21 @@
     @classmethod
     def list(self,model:Base,**kwargs)->List[Base]:
         session = self.session()  
         query = session.query(model) 
         if kwargs:
             query = query.filter_by(**kwargs) 
         return query.all()
-          
+    @classmethod
+    def query(self,model:Base)->Query:
+        session = self.session()  
+        query = session.query(model) 
+         
+        return query
+    
     @classmethod
     def delete(self,model:Base,**kwargs)->int:
         session = self.session()  
         if kwargs:
             cnt = session.query(model).filter_by(**kwargs).delete()
         else:
             cnt = session.query(model).delete()
@@ -248,43 +255,61 @@
 def sanitize_path(path):
     # 匹配非法字符
     illegal_chars = r'[\\/:\*\?"<>\|]'
     # 将非法字符替换为下划线
     sanitized_path = re.sub(illegal_chars, '_', path)
     return sanitized_path
 
-def check_migration(engine:Engine,uri,alembic_ini): 
+def check_migration(engine:Engine,uri,alembic_ini,upgrade=None): 
+    alembic_ini = os.path.abspath(os.path.join(ROOT_PATH,alembic_ini))
     def _update_uri_to_ini(): 
         #auto update alembic.ini sqlalchemy.url section 
+        
         config = configparser.ConfigParser() 
         # read ini config
         config.read(alembic_ini)
         config.set('alembic','sqlalchemy.url',uri)
+        script_location = config.get('alembic','script_location')
+        script_location= os.path.abspath(os.path.join(ROOT_PATH,script_location))
+        config.set("alembic",'script_location',script_location)
         # save modified ini file
         with open(alembic_ini, 'w') as f:
             config.write(f)
         #makesure the migrations directory exists
-        reversions_dir = config.get("alembic",'script_location')
-        reversions_dir = os.path.join(reversions_dir,"versions")
+        reversions_dir =  os.path.join(script_location,"versions")
         if not os.path.exists(reversions_dir):
             os.makedirs(reversions_dir,exist_ok=True)
     try:
         Base.metadata.create_all(bind=engine)
     except Exception as e:
         raise InitDbError(e.args)
     _update_uri_to_ini()
     #  
     alembic_cfg = Config(alembic_ini)    
     try:
         command.check(config=alembic_cfg)
     except Exception as e: 
         msg = sanitize_path(str(e.args)) 
-        command.revision(alembic_cfg, autogenerate=True, message=msg) 
+        msg = msg.replace('_New upgrade operations detected_','').replace("None","").replace(table_prefix,"")
+        if 'Target database is not up to date' in msg:
+            #check is check,the database version is not matched alembic
+            _log.warn(_('Target database is not up to date'))
+        else:
+            if isinstance(upgrade,bool):
+                #call by script ,igonred it
+                pass
+            else:
+                #create revision file
+                command.revision(alembic_cfg, autogenerate=True, message=msg) 
         # upgrade the db
-        command.upgrade(alembic_cfg, "head") 
+    to_revision = 'head'
+    if  upgrade is None or upgrade==True: 
+        command.upgrade(alembic_cfg, to_revision)    
+    else:
+        command.downgrade(alembic_cfg,"-1")
 def _test_connection():
     #test connect
     try:
         with engine.connect() as conn:
             _log.disabled = False
             _log.debug(_('database connection successed:') + str(conn))
 
@@ -310,15 +335,15 @@
     global DataMap, mapped_base, engine, table_prefix
      # Get the database encoding and decoding configurations
     dbencode = cfg.get('dbencode')
     dbdecode = cfg.get('dbdecode')
     
      # Check if the database is sqlite and create the directory
     if uri.startswith('sqlite'):
-        from .config import ROOT_PATH
+        
         part = uri.split(':///')
         db_directory  = os.path.dirname(part[1])
         db_directory = os.path.abspath(os.path.join(ROOT_PATH, db_directory))
         db_file = os.path.join(db_directory,os.path.basename(part[1]))
         cfg['uri'] = uri = f"sqlite:///{db_file}"
         os.makedirs(db_directory, exist_ok=True) 
      # Get the maptables and dbfirst configurations
```

### Comparing `irails-1.3.19/irails/log.py` & `irails-1.3.20/irails/log.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.19/irails/midware.py` & `irails-1.3.20/irails/midware.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.19/irails/midware_casbin.py` & `irails-1.3.20/irails/midware_casbin.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.19/irails/midware_session.py` & `irails-1.3.20/irails/midware_session.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.19/irails/mvc_router.py` & `irails-1.3.20/irails/mvc_router.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.19/irails/scripts/_app.py` & `irails-1.3.20/irails/scripts/_app.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.19/irails/scripts/_controller.py` & `irails-1.3.20/irails/scripts/_controller.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.19/irails/scripts/_i18n.py` & `irails-1.3.20/irails/scripts/_i18n.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.19/irails/scripts/_model.py` & `irails-1.3.20/irails/scripts/_model.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.19/irails/scripts/_project.py` & `irails-1.3.20/irails/scripts/_project.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.19/irails/scripts/_run.py` & `irails-1.3.20/irails/scripts/_run.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.19/irails/scripts/_shell.py` & `irails-1.3.20/irails/scripts/_shell.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.19/irails/scripts/_test.py` & `irails-1.3.20/irails/scripts/_test.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.19/irails/scripts/main.py` & `irails-1.3.20/irails/scripts/main.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,27 +6,40 @@
 import os
 import re
 def _ensure_cli():
     executable = os.path.basename(sys.argv[0])
     if not executable.startswith('irails'):
         sys.argv[0] = 'irails'
 _ensure_cli()
+def is_in_irails(directory):
+    """
+    check exists configs dir,   main.py and configs/general.yaml 
+    """ 
+    configs_dir = os.path.join(directory, 'configs') 
+
+    if not os.path.exists(configs_dir):  # or not os.path.exists(main_file):
+        return False
+    general_file = os.path.join(configs_dir, 'general.yaml') 
+    if not os.path.exists(general_file):
+        return False
 
+    return True
 def is_dev_mode(path):
     dev_mode = True
     irails_srcs = ['__init__.py','_i18n.py','_loader.py','_utils.py','auth.py','base_controller.py','cbv.py']
     for src in irails_srcs:
         p = os.path.join(path,src)
         if not os.path.exists(p):
             dev_mode = False
     return dev_mode
 curdir = os.path.abspath(os.curdir)
-project_root = os.path.abspath(os.path.join(curdir,"../.."))
-if is_dev_mode(os.path.join(project_root,'irails')): 
-    
+project_root = curdir
+if not is_in_irails(curdir):
+    project_root = os.path.abspath(os.path.join(curdir,"../.."))
+if is_dev_mode(os.path.join(project_root,'irails')):  
     sys.path.insert(0, project_root)
     
 sys.path.insert(-1,os.path.abspath(os.curdir))
 from irails import __version__
 def collect_features():
     """
     return files in current dir start with '_' no sub dir
```

### Comparing `irails-1.3.19/irails/scripts/tpls/app/home.css.tpl` & `irails-1.3.20/irails/scripts/tpls/app/home.css.tpl`

 * *Files identical despite different names*

### Comparing `irails-1.3.19/irails/scripts/tpls/app/home.tpl` & `irails-1.3.20/irails/scripts/tpls/app/home.tpl`

 * *Files identical despite different names*

### Comparing `irails-1.3.19/irails/scripts/tpls/app/model.jinja` & `irails-1.3.20/irails/scripts/tpls/app/model.jinja`

 * *Files identical despite different names*

### Comparing `irails-1.3.19/irails/scripts/tpls/app/test_service.jinja` & `irails-1.3.20/irails/scripts/tpls/app/test_service.jinja`

 * *Files identical despite different names*

### Comparing `irails-1.3.19/irails/scripts/tpls/project/configs/alembic.ini` & `irails-1.3.20/irails/scripts/tpls/project/configs/alembic.ini`

 * *Files identical despite different names*

### Comparing `irails-1.3.19/irails/scripts/tpls/project/configs/database.yaml` & `irails-1.3.20/irails/scripts/tpls/project/configs/database.yaml`

 * *Files identical despite different names*

### Comparing `irails-1.3.19/irails/scripts/tpls/project/configs/general.yaml` & `irails-1.3.20/irails/scripts/tpls/project/configs/general.yaml`

 * *Files identical despite different names*

### Comparing `irails-1.3.19/irails/scripts/tpls/project/data/alembic/env.py` & `irails-1.3.20/irails/scripts/tpls/project/data/alembic/env.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.19/irails/scripts/tpls/project/public/error_404.html` & `irails-1.3.20/irails/scripts/tpls/project/public/error_404.html`

 * *Files identical despite different names*

### Comparing `irails-1.3.19/irails/scripts/tpls/project/public/error_500.html` & `irails-1.3.20/irails/scripts/tpls/project/public/error_500.html`

 * *Files identical despite different names*

### Comparing `irails-1.3.19/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js` & `irails-1.3.20/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.19/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css` & `irails-1.3.20/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css`

 * *Files identical despite different names*

### Comparing `irails-1.3.19/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js` & `irails-1.3.20/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.19/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js` & `irails-1.3.20/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.19/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js` & `irails-1.3.20/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.19/irails/unit_test.py` & `irails-1.3.20/irails/unit_test.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.19/irails/view.py` & `irails-1.3.20/irails/view.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.19/irails.egg-info/PKG-INFO` & `irails-1.3.20/irails.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irails
-Version: 1.3.19
+Version: 1.3.20
 Summary: Simple and elegant use of FastApi in MVC mode
 Home-page: https://github.com/smjkzsl/irails
 Author: Bruce chou
 Author-email: smjkzsl@gmail.com
 License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework
 Classifier: License :: OSI Approved :: Apache Software License
@@ -81,14 +81,15 @@
     |
     +---uploads                             ## Others dir(if your need or not)
 ```
 ## Extras commands
 * `irails i18n gettext`  --generate i18n in irails app dir
 * `irails shell`         --run python interpreter with buildin support contexts 
 * `irails test`          --run project tests 
+* `irails migrate`       --run database migrations
 
 ## Take a look configure file `general.yaml`
  
 ``` 
     app:
         appdir:
         - apps
```

### Comparing `irails-1.3.19/irails.egg-info/SOURCES.txt` & `irails-1.3.20/irails.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 irails/scripts/main.py
 irails/casbin_adapters/sqlalchemy_adapter.py
 irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc
 irails/scripts/__init__.py
 irails/scripts/_app.py
 irails/scripts/_controller.py
 irails/scripts/_i18n.py
+irails/scripts/_migrate.py
 irails/scripts/_model.py
 irails/scripts/_project.py
 irails/scripts/_run.py
 irails/scripts/_shell.py
 irails/scripts/_test.py
 irails/scripts/main.py
 irails/scripts/tpls/app/controller.tpl
```

### Comparing `irails-1.3.19/setup.py` & `irails-1.3.20/setup.py`

 * *Files identical despite different names*

