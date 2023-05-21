# Comparing `tmp/allianceauth-tax-tools-0.0.1b1.tar.gz` & `tmp/allianceauth-tax-tools-0.0.1b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "allianceauth-tax-tools-0.0.1b1.tar", last modified: Thu Jan 12 08:31:16 2023, max compression
+gzip compressed data, was "allianceauth-tax-tools-0.0.1b6.tar", last modified: Sun May 21 01:52:43 2023, max compression
```

## Comparing `allianceauth-tax-tools-0.0.1b1.tar` & `allianceauth-tax-tools-0.0.1b6.tar`

### file list

```diff
@@ -1,68 +1,69 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 08:31:16.363594 allianceauth-tax-tools-0.0.1b1/
--rw-r--r--   0 runner    (1001) docker     (123)    18365 2023-01-12 08:30:46.000000 allianceauth-tax-tools-0.0.1b1/LICENCE
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-01-12 08:30:46.000000 allianceauth-tax-tools-0.0.1b1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-01-12 08:31:16.363594 allianceauth-tax-tools-0.0.1b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-01-12 08:30:46.000000 allianceauth-tax-tools-0.0.1b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 08:31:16.359594 allianceauth-tax-tools-0.0.1b1/allianceauth_tax_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-01-12 08:31:16.000000 allianceauth-tax-tools-0.0.1b1/allianceauth_tax_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2410 2023-01-12 08:31:16.000000 allianceauth-tax-tools-0.0.1b1/allianceauth_tax_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-12 08:31:16.000000 allianceauth-tax-tools-0.0.1b1/allianceauth_tax_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-01-12 08:31:16.000000 allianceauth-tax-tools-0.0.1b1/allianceauth_tax_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-01-12 08:31:16.000000 allianceauth-tax-tools-0.0.1b1/allianceauth_tax_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-12 08:31:16.363594 allianceauth-tax-tools-0.0.1b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-01-12 08:30:46.000000 allianceauth-tax-tools-0.0.1b1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 08:31:16.359594 allianceauth-tax-tools-0.0.1b1/taxtools/
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-01-12 08:30:46.000000 allianceauth-tax-tools-0.0.1b1/taxtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2418 2023-01-12 08:30:46.000000 allianceauth-tax-tools-0.0.1b1/taxtools/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-01-12 08:30:46.000000 allianceauth-tax-tools-0.0.1b1/taxtools/api.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-01-12 08:30:46.000000 allianceauth-tax-tools-0.0.1b1/taxtools/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-01-12 08:30:46.000000 allianceauth-tax-tools-0.0.1b1/taxtools/auth_hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 08:31:16.359594 allianceauth-tax-tools-0.0.1b1/taxtools/management/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 08:31:16.359594 allianceauth-tax-tools-0.0.1b1/taxtools/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 08:30:46.000000 allianceauth-tax-tools-0.0.1b1/taxtools/management/commands/__init.py
--rw-r--r--   0 runner    (1001) docker     (123)     5698 2023-01-12 08:30:46.000000 allianceauth-tax-tools-0.0.1b1/taxtools/management/commands/tax_defaults.py
--rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-01-12 08:30:46.000000 allianceauth-tax-tools-0.0.1b1/taxtools/management/commands/tax_explain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 08:31:16.363594 allianceauth-tax-tools-0.0.1b1/taxtools/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-01-12 08:30:46.000000 allianceauth-tax-tools-0.0.1b1/taxtools/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-01-12 08:30:46.000000 allianceauth-tax-tools-0.0.1b1/taxtools/migrations/0002_alter_corppayouttaxconfiguration_corporation_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-01-12 08:30:46.000000 allianceauth-tax-tools-0.0.1b1/taxtools/migrations/0003_corppayouttaxconfiguration_tax.py
--rw-r--r--   0 runner    (1001) docker     (123)      915 2023-01-12 08:30:46.000000 allianceauth-tax-tools-0.0.1b1/taxtools/migrations/0004_corptaxhistory.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-01-12 08:30:46.000000 allianceauth-tax-tools-0.0.1b1/taxtools/migrations/0005_rename_entry_corptaxhistory_corp.py
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-01-12 08:30:46.000000 allianceauth-tax-tools-0.0.1b1/taxtools/migrations/0006_alter_corptaxhistory_unique_together.py
--rw-r--r--   0 runner    (1001) docker     (123)      594 2023-01-12 08:30:46.000000 allianceauth-tax-tools-0.0.1b1/taxtools/migrations/0007_rename_corppayouttaxconfiguration_characterpayouttaxconfiguration_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-01-12 08:30:46.000000 allianceauth-tax-tools-0.0.1b1/taxtools/migrations/0008_rename_corppayouttaxhistory_characterpayouttaxhistory_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-01-12 08:30:46.000000 allianceauth-tax-tools-0.0.1b1/taxtools/migrations/0009_alter_characterpayouttaxrecord_entry_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-01-12 08:30:46.000000 allianceauth-tax-tools-0.0.1b1/taxtools/migrations/0010_corptaxpermembertaxconfiguration.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-01-12 08:30:46.000000 allianceauth-tax-tools-0.0.1b1/taxtools/migrations/0011_corptaxperservicemoduleconfiguration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-01-12 08:30:46.000000 allianceauth-tax-tools-0.0.1b1/taxtools/migrations/0012_corptaxconfiguration_corptaxrecord_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-01-12 08:30:46.000000 allianceauth-tax-tools-0.0.1b1/taxtools/migrations/0013_alter_corptaxconfiguration_charactertaxesincluded_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-01-12 08:30:46.000000 allianceauth-tax-tools-0.0.1b1/taxtools/migrations/0014_remove_corptaxperservicemoduleconfiguration_region_filter_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-01-12 08:30:46.000000 allianceauth-tax-tools-0.0.1b1/taxtools/migrations/0015_corptaxconfiguration_exemptedcorps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-01-12 08:30:46.000000 allianceauth-tax-tools-0.0.1b1/taxtools/migrations/0016_rename_charactertaxesincluded_corptaxconfiguration_character_taxes_included_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-01-12 08:30:46.000000 allianceauth-tax-tools-0.0.1b1/taxtools/migrations/0017_corptaxrecord_end_date_corptaxrecord_start_date.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-01-12 08:30:46.000000 allianceauth-tax-tools-0.0.1b1/taxtools/migrations/0018_rename_name_corptaxrecord_name.py
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-01-12 08:30:46.000000 allianceauth-tax-tools-0.0.1b1/taxtools/migrations/0019_characterpayouttaxrecord_record_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-01-12 08:30:46.000000 allianceauth-tax-tools-0.0.1b1/taxtools/migrations/0020_alter_characterpayouttaxconfiguration_options_and_more.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-01-12 08:30:46.000000 allianceauth-tax-tools-0.0.1b1/taxtools/migrations/0021_corptaxconfiguration_character_ratting_included.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 08:30:46.000000 allianceauth-tax-tools-0.0.1b1/taxtools/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    39261 2023-01-12 08:30:46.000000 allianceauth-tax-tools-0.0.1b1/taxtools/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 08:31:16.359594 allianceauth-tax-tools-0.0.1b1/taxtools/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 08:31:16.363594 allianceauth-tax-tools-0.0.1b1/taxtools/static/taxtools/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 08:30:46.000000 allianceauth-tax-tools-0.0.1b1/taxtools/static/taxtools/asset-manifest.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 08:30:46.000000 allianceauth-tax-tools-0.0.1b1/taxtools/static/taxtools/static
--rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-01-12 08:30:46.000000 allianceauth-tax-tools-0.0.1b1/taxtools/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-01-12 08:30:46.000000 allianceauth-tax-tools-0.0.1b1/taxtools/tax_cog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 08:31:16.359594 allianceauth-tax-tools-0.0.1b1/taxtools/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 08:31:16.363594 allianceauth-tax-tools-0.0.1b1/taxtools/templates/ghosttools/
--rw-r--r--   0 runner    (1001) docker     (123)     6945 2023-01-12 08:30:46.000000 allianceauth-tax-tools-0.0.1b1/taxtools/templates/ghosttools/react_base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 08:31:16.363594 allianceauth-tax-tools-0.0.1b1/taxtools/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-12 08:30:46.000000 allianceauth-tax-tools-0.0.1b1/taxtools/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-01-12 08:30:46.000000 allianceauth-tax-tools-0.0.1b1/taxtools/tests/test_tax.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-01-12 08:30:46.000000 allianceauth-tax-tools-0.0.1b1/taxtools/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-01-12 08:30:46.000000 allianceauth-tax-tools-0.0.1b1/taxtools/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-12 08:31:16.363594 allianceauth-tax-tools-0.0.1b1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-01-12 08:30:46.000000 allianceauth-tax-tools-0.0.1b1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      627 2023-01-12 08:30:46.000000 allianceauth-tax-tools-0.0.1b1/tests/celery.py
--rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-01-12 08:30:46.000000 allianceauth-tax-tools-0.0.1b1/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-01-12 08:30:46.000000 allianceauth-tax-tools-0.0.1b1/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-01-12 08:30:46.000000 allianceauth-tax-tools-0.0.1b1/tests/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 01:52:43.652150 allianceauth-tax-tools-0.0.1b6/
+-rw-r--r--   0 runner    (1001) docker     (123)    18365 2023-05-21 01:52:14.000000 allianceauth-tax-tools-0.0.1b6/LICENCE
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-21 01:52:14.000000 allianceauth-tax-tools-0.0.1b6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-21 01:52:43.648150 allianceauth-tax-tools-0.0.1b6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-21 01:52:14.000000 allianceauth-tax-tools-0.0.1b6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 01:52:43.648150 allianceauth-tax-tools-0.0.1b6/allianceauth_tax_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-21 01:52:43.000000 allianceauth-tax-tools-0.0.1b6/allianceauth_tax_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-05-21 01:52:43.000000 allianceauth-tax-tools-0.0.1b6/allianceauth_tax_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 01:52:43.000000 allianceauth-tax-tools-0.0.1b6/allianceauth_tax_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-21 01:52:43.000000 allianceauth-tax-tools-0.0.1b6/allianceauth_tax_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-21 01:52:43.000000 allianceauth-tax-tools-0.0.1b6/allianceauth_tax_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-21 01:52:43.652150 allianceauth-tax-tools-0.0.1b6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1296 2023-05-21 01:52:14.000000 allianceauth-tax-tools-0.0.1b6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 01:52:43.648150 allianceauth-tax-tools-0.0.1b6/taxtools/
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-21 01:52:14.000000 allianceauth-tax-tools-0.0.1b6/taxtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-05-21 01:52:14.000000 allianceauth-tax-tools-0.0.1b6/taxtools/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6607 2023-05-21 01:52:14.000000 allianceauth-tax-tools-0.0.1b6/taxtools/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-21 01:52:14.000000 allianceauth-tax-tools-0.0.1b6/taxtools/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-21 01:52:14.000000 allianceauth-tax-tools-0.0.1b6/taxtools/auth_hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 01:52:43.644150 allianceauth-tax-tools-0.0.1b6/taxtools/management/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 01:52:43.648150 allianceauth-tax-tools-0.0.1b6/taxtools/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 01:52:14.000000 allianceauth-tax-tools-0.0.1b6/taxtools/management/commands/__init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5698 2023-05-21 01:52:14.000000 allianceauth-tax-tools-0.0.1b6/taxtools/management/commands/tax_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2558 2023-05-21 01:52:14.000000 allianceauth-tax-tools-0.0.1b6/taxtools/management/commands/tax_explain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 01:52:43.648150 allianceauth-tax-tools-0.0.1b6/taxtools/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1371 2023-05-21 01:52:14.000000 allianceauth-tax-tools-0.0.1b6/taxtools/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1446 2023-05-21 01:52:14.000000 allianceauth-tax-tools-0.0.1b6/taxtools/migrations/0002_alter_corppayouttaxconfiguration_corporation_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-21 01:52:14.000000 allianceauth-tax-tools-0.0.1b6/taxtools/migrations/0003_corppayouttaxconfiguration_tax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      915 2023-05-21 01:52:14.000000 allianceauth-tax-tools-0.0.1b6/taxtools/migrations/0004_corptaxhistory.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-05-21 01:52:14.000000 allianceauth-tax-tools-0.0.1b6/taxtools/migrations/0005_rename_entry_corptaxhistory_corp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-21 01:52:14.000000 allianceauth-tax-tools-0.0.1b6/taxtools/migrations/0006_alter_corptaxhistory_unique_together.py
+-rw-r--r--   0 runner    (1001) docker     (123)      594 2023-05-21 01:52:14.000000 allianceauth-tax-tools-0.0.1b6/taxtools/migrations/0007_rename_corppayouttaxconfiguration_characterpayouttaxconfiguration_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-05-21 01:52:14.000000 allianceauth-tax-tools-0.0.1b6/taxtools/migrations/0008_rename_corppayouttaxhistory_characterpayouttaxhistory_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-21 01:52:14.000000 allianceauth-tax-tools-0.0.1b6/taxtools/migrations/0009_alter_characterpayouttaxrecord_entry_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-21 01:52:14.000000 allianceauth-tax-tools-0.0.1b6/taxtools/migrations/0010_corptaxpermembertaxconfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-21 01:52:14.000000 allianceauth-tax-tools-0.0.1b6/taxtools/migrations/0011_corptaxperservicemoduleconfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3820 2023-05-21 01:52:14.000000 allianceauth-tax-tools-0.0.1b6/taxtools/migrations/0012_corptaxconfiguration_corptaxrecord_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1274 2023-05-21 01:52:14.000000 allianceauth-tax-tools-0.0.1b6/taxtools/migrations/0013_alter_corptaxconfiguration_charactertaxesincluded_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      727 2023-05-21 01:52:14.000000 allianceauth-tax-tools-0.0.1b6/taxtools/migrations/0014_remove_corptaxperservicemoduleconfiguration_region_filter_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-21 01:52:14.000000 allianceauth-tax-tools-0.0.1b6/taxtools/migrations/0015_corptaxconfiguration_exemptedcorps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-05-21 01:52:14.000000 allianceauth-tax-tools-0.0.1b6/taxtools/migrations/0016_rename_charactertaxesincluded_corptaxconfiguration_character_taxes_included_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-21 01:52:14.000000 allianceauth-tax-tools-0.0.1b6/taxtools/migrations/0017_corptaxrecord_end_date_corptaxrecord_start_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-21 01:52:14.000000 allianceauth-tax-tools-0.0.1b6/taxtools/migrations/0018_rename_name_corptaxrecord_name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-21 01:52:14.000000 allianceauth-tax-tools-0.0.1b6/taxtools/migrations/0019_characterpayouttaxrecord_record_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5067 2023-05-21 01:52:14.000000 allianceauth-tax-tools-0.0.1b6/taxtools/migrations/0020_alter_characterpayouttaxconfiguration_options_and_more.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-21 01:52:14.000000 allianceauth-tax-tools-0.0.1b6/taxtools/migrations/0021_corptaxconfiguration_character_ratting_included.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-21 01:52:14.000000 allianceauth-tax-tools-0.0.1b6/taxtools/migrations/0022_corptaxconfiguration_included_alliances.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 01:52:14.000000 allianceauth-tax-tools-0.0.1b6/taxtools/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40604 2023-05-21 01:52:14.000000 allianceauth-tax-tools-0.0.1b6/taxtools/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 01:52:43.644150 allianceauth-tax-tools-0.0.1b6/taxtools/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 01:52:43.648150 allianceauth-tax-tools-0.0.1b6/taxtools/static/taxtools/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 01:52:14.000000 allianceauth-tax-tools-0.0.1b6/taxtools/static/taxtools/asset-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 01:52:14.000000 allianceauth-tax-tools-0.0.1b6/taxtools/static/taxtools/static
+-rw-r--r--   0 runner    (1001) docker     (123)     2627 2023-05-21 01:52:14.000000 allianceauth-tax-tools-0.0.1b6/taxtools/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-05-21 01:52:14.000000 allianceauth-tax-tools-0.0.1b6/taxtools/tax_cog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 01:52:43.644150 allianceauth-tax-tools-0.0.1b6/taxtools/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 01:52:43.648150 allianceauth-tax-tools-0.0.1b6/taxtools/templates/ghosttools/
+-rw-r--r--   0 runner    (1001) docker     (123)     6945 2023-05-21 01:52:14.000000 allianceauth-tax-tools-0.0.1b6/taxtools/templates/ghosttools/react_base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 01:52:43.648150 allianceauth-tax-tools-0.0.1b6/taxtools/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-21 01:52:14.000000 allianceauth-tax-tools-0.0.1b6/taxtools/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2432 2023-05-21 01:52:14.000000 allianceauth-tax-tools-0.0.1b6/taxtools/tests/test_tax.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-21 01:52:14.000000 allianceauth-tax-tools-0.0.1b6/taxtools/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-21 01:52:14.000000 allianceauth-tax-tools-0.0.1b6/taxtools/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 01:52:43.648150 allianceauth-tax-tools-0.0.1b6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-21 01:52:14.000000 allianceauth-tax-tools-0.0.1b6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-21 01:52:14.000000 allianceauth-tax-tools-0.0.1b6/tests/celery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-21 01:52:14.000000 allianceauth-tax-tools-0.0.1b6/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-21 01:52:14.000000 allianceauth-tax-tools-0.0.1b6/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-21 01:52:14.000000 allianceauth-tax-tools-0.0.1b6/tests/views.py
```

### Comparing `allianceauth-tax-tools-0.0.1b1/LICENCE` & `allianceauth-tax-tools-0.0.1b6/LICENCE`

 * *Files identical despite different names*

### Comparing `allianceauth-tax-tools-0.0.1b1/PKG-INFO` & `allianceauth-tax-tools-0.0.1b6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: allianceauth-tax-tools
-Version: 0.0.1b1
+Version: 0.0.1b6
 Summary: Alliance Auth Plugin
 Home-page: https://github.com/pvyParts/allianceauth-corp-tools-tax-tools
 Author: AaronKable
 Author-email: aaronkable@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `allianceauth-tax-tools-0.0.1b1/allianceauth_tax_tools.egg-info/PKG-INFO` & `allianceauth-tax-tools-0.0.1b6/allianceauth_tax_tools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: allianceauth-tax-tools
-Version: 0.0.1b1
+Version: 0.0.1b6
 Summary: Alliance Auth Plugin
 Home-page: https://github.com/pvyParts/allianceauth-corp-tools-tax-tools
 Author: AaronKable
 Author-email: aaronkable@gmail.com
 License: GNU General Public License v3 (GPLv3)
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `allianceauth-tax-tools-0.0.1b1/allianceauth_tax_tools.egg-info/SOURCES.txt` & `allianceauth-tax-tools-0.0.1b6/allianceauth_tax_tools.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -37,14 +37,15 @@
 taxtools/migrations/0015_corptaxconfiguration_exemptedcorps.py
 taxtools/migrations/0016_rename_charactertaxesincluded_corptaxconfiguration_character_taxes_included_and_more.py
 taxtools/migrations/0017_corptaxrecord_end_date_corptaxrecord_start_date.py
 taxtools/migrations/0018_rename_name_corptaxrecord_name.py
 taxtools/migrations/0019_characterpayouttaxrecord_record_and_more.py
 taxtools/migrations/0020_alter_characterpayouttaxconfiguration_options_and_more.py
 taxtools/migrations/0021_corptaxconfiguration_character_ratting_included.py
+taxtools/migrations/0022_corptaxconfiguration_included_alliances.py
 taxtools/migrations/__init__.py
 taxtools/static/taxtools/asset-manifest.json
 taxtools/static/taxtools/static
 taxtools/templates/ghosttools/react_base.html
 taxtools/tests/__init__.py
 taxtools/tests/test_tax.py
 tests/__init__.py
```

### Comparing `allianceauth-tax-tools-0.0.1b1/setup.py` & `allianceauth-tax-tools-0.0.1b6/setup.py`

 * *Files identical despite different names*

### Comparing `allianceauth-tax-tools-0.0.1b1/taxtools/admin.py` & `allianceauth-tax-tools-0.0.1b6/taxtools/admin.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     list_display = ['state', 'isk_per_main']
 
 
 @admin.register(models.CorpTaxConfiguration)
 class CorpTaxConfigurationAdmin(admin.ModelAdmin):
     filter_horizontal = ["character_taxes_included", "corporate_taxes_included",
                          "corporate_member_tax_included", "corporate_structure_tax_included",
-                         "exempted_corps", "character_ratting_included"]
+                         "exempted_corps", "character_ratting_included", "included_alliances"]
 
 
 @admin.register(models.CorpTaxPerServiceModuleConfiguration)
 class CorpTaxPerServiceModuleConfigurationAdmin(admin.ModelAdmin):
     filter_horizontal = ["region_filter"]
```

### Comparing `allianceauth-tax-tools-0.0.1b1/taxtools/api.py` & `allianceauth-tax-tools-0.0.1b6/taxtools/api.py`

 * *Files identical despite different names*

### Comparing `allianceauth-tax-tools-0.0.1b1/taxtools/management/commands/tax_defaults.py` & `allianceauth-tax-tools-0.0.1b6/taxtools/management/commands/tax_defaults.py`

 * *Files identical despite different names*

### Comparing `allianceauth-tax-tools-0.0.1b1/taxtools/management/commands/tax_explain.py` & `allianceauth-tax-tools-0.0.1b6/taxtools/management/commands/tax_explain.py`

 * *Files identical despite different names*

### Comparing `allianceauth-tax-tools-0.0.1b1/taxtools/migrations/0001_initial.py` & `allianceauth-tax-tools-0.0.1b6/taxtools/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `allianceauth-tax-tools-0.0.1b1/taxtools/migrations/0002_alter_corppayouttaxconfiguration_corporation_and_more.py` & `allianceauth-tax-tools-0.0.1b6/taxtools/migrations/0002_alter_corppayouttaxconfiguration_corporation_and_more.py`

 * *Files identical despite different names*

### Comparing `allianceauth-tax-tools-0.0.1b1/taxtools/migrations/0004_corptaxhistory.py` & `allianceauth-tax-tools-0.0.1b6/taxtools/migrations/0004_corptaxhistory.py`

 * *Files identical despite different names*

### Comparing `allianceauth-tax-tools-0.0.1b1/taxtools/migrations/0007_rename_corppayouttaxconfiguration_characterpayouttaxconfiguration_and_more.py` & `allianceauth-tax-tools-0.0.1b6/taxtools/migrations/0007_rename_corppayouttaxconfiguration_characterpayouttaxconfiguration_and_more.py`

 * *Files identical despite different names*

### Comparing `allianceauth-tax-tools-0.0.1b1/taxtools/migrations/0008_rename_corppayouttaxhistory_characterpayouttaxhistory_and_more.py` & `allianceauth-tax-tools-0.0.1b6/taxtools/migrations/0008_rename_corppayouttaxhistory_characterpayouttaxhistory_and_more.py`

 * *Files identical despite different names*

### Comparing `allianceauth-tax-tools-0.0.1b1/taxtools/migrations/0009_alter_characterpayouttaxrecord_entry_and_more.py` & `allianceauth-tax-tools-0.0.1b6/taxtools/migrations/0009_alter_characterpayouttaxrecord_entry_and_more.py`

 * *Files identical despite different names*

### Comparing `allianceauth-tax-tools-0.0.1b1/taxtools/migrations/0010_corptaxpermembertaxconfiguration.py` & `allianceauth-tax-tools-0.0.1b6/taxtools/migrations/0010_corptaxpermembertaxconfiguration.py`

 * *Files identical despite different names*

### Comparing `allianceauth-tax-tools-0.0.1b1/taxtools/migrations/0011_corptaxperservicemoduleconfiguration.py` & `allianceauth-tax-tools-0.0.1b6/taxtools/migrations/0011_corptaxperservicemoduleconfiguration.py`

 * *Files identical despite different names*

### Comparing `allianceauth-tax-tools-0.0.1b1/taxtools/migrations/0012_corptaxconfiguration_corptaxrecord_and_more.py` & `allianceauth-tax-tools-0.0.1b6/taxtools/migrations/0012_corptaxconfiguration_corptaxrecord_and_more.py`

 * *Files identical despite different names*

### Comparing `allianceauth-tax-tools-0.0.1b1/taxtools/migrations/0013_alter_corptaxconfiguration_charactertaxesincluded_and_more.py` & `allianceauth-tax-tools-0.0.1b6/taxtools/migrations/0013_alter_corptaxconfiguration_charactertaxesincluded_and_more.py`

 * *Files identical despite different names*

### Comparing `allianceauth-tax-tools-0.0.1b1/taxtools/migrations/0014_remove_corptaxperservicemoduleconfiguration_region_filter_and_more.py` & `allianceauth-tax-tools-0.0.1b6/taxtools/migrations/0014_remove_corptaxperservicemoduleconfiguration_region_filter_and_more.py`

 * *Files identical despite different names*

### Comparing `allianceauth-tax-tools-0.0.1b1/taxtools/migrations/0015_corptaxconfiguration_exemptedcorps.py` & `allianceauth-tax-tools-0.0.1b6/taxtools/migrations/0015_corptaxconfiguration_exemptedcorps.py`

 * *Files identical despite different names*

### Comparing `allianceauth-tax-tools-0.0.1b1/taxtools/migrations/0016_rename_charactertaxesincluded_corptaxconfiguration_character_taxes_included_and_more.py` & `allianceauth-tax-tools-0.0.1b6/taxtools/migrations/0016_rename_charactertaxesincluded_corptaxconfiguration_character_taxes_included_and_more.py`

 * *Files identical despite different names*

### Comparing `allianceauth-tax-tools-0.0.1b1/taxtools/migrations/0017_corptaxrecord_end_date_corptaxrecord_start_date.py` & `allianceauth-tax-tools-0.0.1b6/taxtools/migrations/0017_corptaxrecord_end_date_corptaxrecord_start_date.py`

 * *Files identical despite different names*

### Comparing `allianceauth-tax-tools-0.0.1b1/taxtools/migrations/0019_characterpayouttaxrecord_record_and_more.py` & `allianceauth-tax-tools-0.0.1b6/taxtools/migrations/0019_characterpayouttaxrecord_record_and_more.py`

 * *Files identical despite different names*

### Comparing `allianceauth-tax-tools-0.0.1b1/taxtools/migrations/0020_alter_characterpayouttaxconfiguration_options_and_more.py` & `allianceauth-tax-tools-0.0.1b6/taxtools/migrations/0020_alter_characterpayouttaxconfiguration_options_and_more.py`

 * *Files identical despite different names*

### Comparing `allianceauth-tax-tools-0.0.1b1/taxtools/migrations/0021_corptaxconfiguration_character_ratting_included.py` & `allianceauth-tax-tools-0.0.1b6/taxtools/migrations/0021_corptaxconfiguration_character_ratting_included.py`

 * *Files identical despite different names*

### Comparing `allianceauth-tax-tools-0.0.1b1/taxtools/models.py` & `allianceauth-tax-tools-0.0.1b6/taxtools/models.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 import logging
 from datetime import datetime, timedelta, timezone
 from decimal import Decimal
 from math import floor, log
 
 import yaml
 from allianceauth.authentication.models import State
-from allianceauth.eveonline.models import EveCharacter, EveCorporationInfo
+from allianceauth.eveonline.models import (EveAllianceInfo, EveCharacter,
+                                           EveCorporationInfo)
+from allianceauth.eveonline.providers import Corporation
 from corptools.models import (CharacterWalletJournalEntry, CorporationAudit,
                               CorporationWalletJournalEntry, EveName,
                               MapRegion, MapSystem, Notification, Structure,
                               StructureService)
 from corptools.providers import esi
 from django.contrib.auth.models import User
 from django.core.exceptions import ObjectDoesNotExist
@@ -65,15 +67,15 @@
     def get_payment_data(self, start_date=MIN_DATE, end_date=MAX_DATE, alliance_filter=None):
         query = CharacterWalletJournalEntry.objects.filter(
             date__gte=start_date,
             date__lte=end_date,
             ref_type__in=["bounty_prizes"])
         if alliance_filter:
             query = query.filter(
-                character__character__character_ownership__user__profile__main_character__alliance_id=alliance_filter)
+                character__character__character_ownership__user__profile__main_character__alliance_id__in=alliance_filter)
         if self.region_filter.all().count():
             query = query.filter(
                 context_id__in=MapSystem.objects.filter(
                     constellation__region__in=self.region_filter.all())
             )
         return query.exclude(taxed__processed=True)
 
@@ -150,14 +152,16 @@
                 if d['date'] > output[cid]["end"]:
                     output[cid]["end"] = d['date']
 
         # print(bad_transactions)
         return output
 
     def get_character_aggregates_corp_level(self, start_date=MIN_DATE, end_date=MAX_DATE, full=True, alliance_filter=None):
+        logger.debug(
+            f"TAXTOOLS: Started get_character_aggregates_corp_level {self.__str_discord__()}")
         data = self.get_character_aggregates(
             start_date, end_date, alliance_filter)
         output = {}
         for id, t in data.items():
             cid = t['corp']
             if cid not in output:
                 output[cid] = {
@@ -229,18 +233,20 @@
             date__gte=start_date,
             date__lte=end_date,
             ref_type__in=ref_types)
         if self.corporation_id:
             query = query.filter(first_party_name_id=self.corporation_id)
         if alliance_filter:
             query = query.filter(
-                character__character__character_ownership__user__profile__main_character__alliance_id=alliance_filter)
+                character__character__character_ownership__user__profile__main_character__alliance_id__in=alliance_filter)
         return query.exclude(taxed__processed=True)
 
     def get_character_aggregates(self, start_date=MIN_DATE, end_date=MAX_DATE, alliance_filter=None):
+        logger.debug(
+            f"TAXTOOLS: Started get_character_aggregates {self.__str_discord__()}")
         data = self.get_payment_data(start_date, end_date, alliance_filter).values(
             'amount',
             'entry_id',
             'date',
             'tax',
             char=F('character__character__character_id'),
             corp=F('character__character__corporation_id'),
@@ -321,14 +327,16 @@
                 if d['date'] > output[cid]["end"]:
                     output[cid]["end"] = d['date']
 
         # print(bad_transactions)
         return output
 
     def get_character_aggregates_corp_level(self, start_date=MIN_DATE, end_date=MAX_DATE, full=True, alliance_filter=None):
+        logger.debug(
+            f"TAXTOOLS: Started get_character_aggregates_corp_level {self.__str_discord__()}")
         data = self.get_character_aggregates(
             start_date, end_date, alliance_filter)
         output = {}
         for id, t in data.items():
             cid = t['corp']
             if cid not in output:
                 output[cid] = {
@@ -589,14 +597,16 @@
             Count("character_id"),
             corp_name=F(
                 "character_ownership__user__profile__main_character__corporation_name")
         )
         return characters
 
     def get_invoice_data(self):
+        logger.debug(
+            f"TAXTOOLS: Started get_invoice_data {self.__str_discord__()}")
         corp_list = self.get_main_counts()
         corp_info = {}
         output = {}
         corps = EveCorporationInfo.objects.filter(corporation_id__in=corp_list.values_list(
             "character_ownership__user__profile__main_character__corporation_id"))
 
         for c in corps:
@@ -674,14 +684,16 @@
 
         structures = structures.values(corp=F("corporation__corporation__corporation_id")).distinct().annotate(
             total_structures=Count("structure_id"),
         )
         return structures
 
     def get_invoice_data(self):  # TODO update
+        logger.debug(
+            f"TAXTOOLS: Started get_invoice_data {self.__str_discord__()}")
         corp_list = self.get_service_counts()
         output = {}
 
         for corp in corp_list:
             cid = corp['corp']
             output[cid] = {
                 "services_count": corp['total_structures'],
@@ -742,14 +754,16 @@
     corporate_member_tax_included = models.ManyToManyField(
         CorpTaxPerMemberTaxConfiguration, blank=True)
     corporate_structure_tax_included = models.ManyToManyField(
         CorpTaxPerServiceModuleConfiguration, blank=True)
 
     exempted_corps = models.ManyToManyField(EveCorporationInfo, blank=True)
 
+    included_alliances = models.ManyToManyField(EveAllianceInfo, blank=True)
+
     def __str__(self) -> str:
         return F"{self.Name}"
 
     class Meta:
         verbose_name = "Config: Corporate"
         verbose_name_plural = "Config: Corporate"
 
@@ -757,26 +771,27 @@
     def get_last_invoice_date(cls):
         try:
             return CorpTaxRecord.objects.all().order_by('-end_date').first().end_date
         except (ObjectDoesNotExist, AttributeError) as e:
             return datetime.min + timedelta(days=5)
 
     @classmethod
-    def generate_corp_ref(cls, corporation, date):
-        return f"{corporation.corporation_ticker}-{date.strftime('%Y%m%d')}"
+    def generate_corp_ref(cls, corporation: Corporation, date):
+        return f"{corporation.ticker}-{date.strftime('%Y%m%d')}"
 
     @staticmethod
     def human_format(number):
 
         units = ['', 'K', 'M', 'B', 'T']
         k = 1000.0
         magnitude = int(floor(log(number, k)))
         return '%.2f%s' % (float(number) / k**magnitude, units[magnitude])
 
     def calculate_tax(self, start_date=datetime.min, end_date=datetime.max, alliance_filter=None):
+        logger.debug("TAXTOOLS: Starting calculate_tax")
         excluded_cids = self.exempted_corps.all().values_list("corporation_id", flat=True)
         tax_invoices = {}
         char_trans_ids = []
         corp_trans_ids = []
         output = {
             "char_tax": [],
             "corp_tax": [],
@@ -786,14 +801,15 @@
             "char": 0,
             "corp": 0,
             "member": 0,
             "structure": 0,
             "total_tax": 0
         }
 
+        logger.debug("TAXTOOLS: Starting character_ratting_included")
         for tax in self.character_ratting_included.all():
             _taxes = tax.get_character_aggregates_corp_level(
                 start_date=start_date, end_date=end_date, alliance_filter=alliance_filter)
             output["char_tax"].append(_taxes)
             for cid, data in _taxes.items():
                 if cid not in excluded_cids:
                     amount = round(data['tax_to_pay'], -6)
@@ -806,14 +822,15 @@
                         tax_invoices[cid]['total_tax'] += amount
                         output['total_tax'] += amount
                         output['ratting'] += amount
                         tax_invoices[cid]['messages'].append(
                             f"{tax.name}: {self.human_format(amount)} ({tax.tax:,.1f}% of Total Earnings)")
                     char_trans_ids += data['trans_ids']
 
+        logger.debug("TAXTOOLS: Starting character_taxes_included")
         for tax in self.character_taxes_included.all():
             _taxes = tax.get_character_aggregates_corp_level(
                 start_date=start_date, end_date=end_date, alliance_filter=alliance_filter)
             output["char_tax"].append(_taxes)
             for cid, data in _taxes.items():
                 if cid not in excluded_cids:
                     amount = round(data['tax_to_pay'], -6)
@@ -826,14 +843,15 @@
                         tax_invoices[cid]['total_tax'] += amount
                         output['total_tax'] += amount
                         output['char'] += amount
                         tax_invoices[cid]['messages'].append(
                             f"{tax.name}: {self.human_format(amount)} ({tax.tax:,.1f}% of Total Earnings)")
                     char_trans_ids += data['trans_ids']
 
+        logger.debug("TAXTOOLS: Starting corporate_taxes_included")
         for tax in self.corporate_taxes_included.all():
             _taxes = tax.get_aggregates(
                 start_date=start_date, end_date=end_date, alliance_filter=alliance_filter)
             output["corp_tax"].append(_taxes)
             for cid, data in _taxes.items():
                 if cid not in excluded_cids:
                     amount = round(data['tax_to_pay'], -6)
@@ -846,14 +864,15 @@
                         tax_invoices[cid]['total_tax'] += amount
                         output['total_tax'] += amount
                         output['corp'] += amount
                         tax_invoices[cid]['messages'].append(
                             f"{tax.name}: {self.human_format(amount)} ({tax.tax:,.1f}% of Total Earnings)")
                     corp_trans_ids += data['trans_ids']
 
+        logger.debug("TAXTOOLS: Starting corporate_member_tax_included")
         for tax in self.corporate_member_tax_included.all():
             _taxes = tax.get_invoice_data()
             output["corp_member_tax"].append(_taxes)
             for cid, data in _taxes.items():
                 if cid not in excluded_cids:
                     amount = round(data['tax_to_pay'], -6)
                     if amount > 1000000:
@@ -864,15 +883,15 @@
                             }
 
                         tax_invoices[cid]['total_tax'] += amount
                         output['total_tax'] += amount
                         output['member'] += amount
                         tax_invoices[cid]['messages'].append(
                             f"Main Character Tax: ${self.human_format(amount)} ({tax.state.name}: {data['main_count']} Mains @ {self.human_format(tax.isk_per_main)} Per)")
-
+        logger.debug("TAXTOOLS: Starting corporate_structure_tax_included")
         for tax in self.corporate_structure_tax_included.all():
             _taxes = tax.get_invoice_data()
             output["corp_structure_tax"].append(_taxes)
             for cid, data in _taxes.items():
                 if cid not in excluded_cids:
                     amount = round(data['tax_to_pay'], -6)
                     if amount > 1000000:
@@ -883,15 +902,15 @@
                             }
                         tax_invoices[cid]['total_tax'] += amount
                         output['total_tax'] += amount
                         output['structure'] += amount
 
                         tax_invoices[cid]['messages'].append(
                             f"Industry Structures Tax: ${self.human_format(amount)} ({data['services_count']} Structure @ {self.human_format(tax.isk_per_service)} Per)")
-
+        logger.debug("TAXTOOLS: Done corporate_structure_tax_included")
         return {"taxes": tax_invoices, "raw": output, "char_trans_ids": char_trans_ids, "corp_trans_ids": corp_trans_ids}
 
     @classmethod
     def sanitize_date(cls, date):
         return datetime(year=date.year,
                         month=date.month,
                         day=date.day,
@@ -900,33 +919,35 @@
                         minute=0,
                         second=0)
 
     @classmethod
     def generate_invoice_for_ceo(cls, corp_id, ref, amount, message):
         # generate an invoice and return it
         due = tzone.now() + timedelta(days=14)
-        corp = EveCorporationInfo.objects.get(corporation_id=corp_id)
+        corp = EveCorporationInfo.provider.get_corporation(corp_id)
         character = EveCharacter.objects.get_character_by_id(corp.ceo_id)
         if not character:
-            if not corp.ceo_id:
-                corp.update_corporation()
             character = EveCharacter.objects.create_character(corp.ceo_id)
         return Invoice(character=character,
                        amount=amount,
                        invoice_ref=cls.generate_corp_ref(corp, tzone.now()),
                        note=message,
                        due_date=due)
 
     def get_invoice_data(self):
         start_date = self.sanitize_date(
             # allow for esi delays in the wallets
             self.get_last_invoice_date() - timedelta(days=2)
         )
         end_date = self.sanitize_date(tzone.now())
-        return start_date, end_date, self.calculate_tax(start_date=start_date, end_date=end_date)
+        alliances = None
+        if self.included_alliances.all().count():
+            alliances = self.included_alliances.all().values_list("alliance_id", flat=True)
+
+        return start_date, end_date, self.calculate_tax(start_date=start_date, end_date=end_date, alliance_filter=alliances)
 
     def send_invoices(self):
         start_date, end_date, taxes = self.get_invoice_data()
         total_tax = 0
         for id, tax in taxes['taxes'].items():
             msg = "\n".join(tax['messages'])
             invoice = self.generate_invoice_for_ceo(
```

### Comparing `allianceauth-tax-tools-0.0.1b1/taxtools/tasks.py` & `allianceauth-tax-tools-0.0.1b6/taxtools/tasks.py`

 * *Files identical despite different names*

### Comparing `allianceauth-tax-tools-0.0.1b1/taxtools/tax_cog.py` & `allianceauth-tax-tools-0.0.1b6/taxtools/tax_cog.py`

 * *Files identical despite different names*

### Comparing `allianceauth-tax-tools-0.0.1b1/taxtools/templates/ghosttools/react_base.html` & `allianceauth-tax-tools-0.0.1b6/taxtools/templates/ghosttools/react_base.html`

 * *Files identical despite different names*

### Comparing `allianceauth-tax-tools-0.0.1b1/taxtools/tests/test_tax.py` & `allianceauth-tax-tools-0.0.1b6/taxtools/tests/test_tax.py`

 * *Files identical despite different names*

### Comparing `allianceauth-tax-tools-0.0.1b1/tests/celery.py` & `allianceauth-tax-tools-0.0.1b6/tests/celery.py`

 * *Files identical despite different names*

### Comparing `allianceauth-tax-tools-0.0.1b1/tests/test_settings.py` & `allianceauth-tax-tools-0.0.1b6/tests/test_settings.py`

 * *Files identical despite different names*

