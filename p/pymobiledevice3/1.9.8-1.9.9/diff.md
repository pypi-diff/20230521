# Comparing `tmp/pymobiledevice3-1.9.8.tar.gz` & `tmp/pymobiledevice3-1.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymobiledevice3-1.9.8.tar", last modified: Mon Jul 19 08:39:16 2021, max compression
+gzip compressed data, was "pymobiledevice3-1.9.9.tar", last modified: Mon Aug  9 09:47:42 2021, max compression
```

## Comparing `pymobiledevice3-1.9.8.tar` & `pymobiledevice3-1.9.9.tar`

### file list

```diff
@@ -1,101 +1,114 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-19 08:39:16.132397 pymobiledevice3-1.9.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1065 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    16354 2021-07-19 08:39:16.132397 pymobiledevice3-1.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    13244 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-19 08:39:16.124397 pymobiledevice3-1.9.8/pymobiledevice3/
--rwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/pymobiledevice3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1646 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/pymobiledevice3/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     5315 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/pymobiledevice3/ca.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-19 08:39:16.124397 pymobiledevice3-1.9.8/pymobiledevice3/cli/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/pymobiledevice3/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1972 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/pymobiledevice3/cli/afc.py
--rw-r--r--   0 runner    (1001) docker     (121)     1571 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/pymobiledevice3/cli/apps.py
--rw-r--r--   0 runner    (1001) docker     (121)     1272 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/pymobiledevice3/cli/cli_common.py
--rw-r--r--   0 runner    (1001) docker     (121)     1395 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/pymobiledevice3/cli/crash.py
--rw-r--r--   0 runner    (1001) docker     (121)    27492 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/pymobiledevice3/cli/developer.py
--rw-r--r--   0 runner    (1001) docker     (121)     2683 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/pymobiledevice3/cli/diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (121)      679 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/pymobiledevice3/cli/list_devices.py
--rw-r--r--   0 runner    (1001) docker     (121)     1626 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/pymobiledevice3/cli/lockdown.py
--rw-r--r--   0 runner    (1001) docker     (121)     3820 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/pymobiledevice3/cli/mounter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1416 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/pymobiledevice3/cli/notification.py
--rw-r--r--   0 runner    (1001) docker     (121)     1695 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/pymobiledevice3/cli/pcap.py
--rw-r--r--   0 runner    (1001) docker     (121)      719 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/pymobiledevice3/cli/power_assertion.py
--rw-r--r--   0 runner    (1001) docker     (121)      998 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/pymobiledevice3/cli/processes.py
--rw-r--r--   0 runner    (1001) docker     (121)     1074 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/pymobiledevice3/cli/profile.py
--rw-r--r--   0 runner    (1001) docker     (121)     1755 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/pymobiledevice3/cli/springboard.py
--rw-r--r--   0 runner    (1001) docker     (121)     4663 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/pymobiledevice3/cli/syslog.py
--rw-r--r--   0 runner    (1001) docker     (121)     1565 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/pymobiledevice3/exceptions.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    11166 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/pymobiledevice3/lockdown.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-19 08:39:16.128397 pymobiledevice3-1.9.8/pymobiledevice3/resources/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/pymobiledevice3/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)  1023280 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/pymobiledevice3/resources/dsc_uuid_map.json
--rw-r--r--   0 runner    (1001) docker     (121)     2520 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/pymobiledevice3/resources/dsc_uuid_map.py
--rw-r--r--   0 runner    (1001) docker     (121)     1794 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/pymobiledevice3/resources/firmware_notifications.py
--rw-r--r--   0 runner    (1001) docker     (121)    20970 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/pymobiledevice3/resources/notifications.txt
--rwxr-xr-x   0 runner    (1001) docker     (121)     3905 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/pymobiledevice3/service_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-19 08:39:16.128397 pymobiledevice3-1.9.8/pymobiledevice3/services/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/pymobiledevice3/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5807 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/pymobiledevice3/services/accessibilityaudit.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    20357 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/pymobiledevice3/services/afc.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      593 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/pymobiledevice3/services/debugserver_applist.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     5608 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/pymobiledevice3/services/diagnostics.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1433 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/pymobiledevice3/services/dtfetchsymbols.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-19 08:39:16.128397 pymobiledevice3-1.9.8/pymobiledevice3/services/dvt/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/pymobiledevice3/services/dvt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      744 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/pymobiledevice3/services/dvt/dvt_secure_socket_proxy.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-19 08:39:16.132397 pymobiledevice3-1.9.8/pymobiledevice3/services/dvt/instruments/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/pymobiledevice3/services/dvt/instruments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8570 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/pymobiledevice3/services/dvt/instruments/activity_trace_tap.py
--rw-r--r--   0 runner    (1001) docker     (121)      666 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/pymobiledevice3/services/dvt/instruments/application_listing.py
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/pymobiledevice3/services/dvt/instruments/condition_inducer.py
--rw-r--r--   0 runner    (1001) docker     (121)    26146 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/pymobiledevice3/services/dvt/instruments/core_profile_session_tap.py
--rw-r--r--   0 runner    (1001) docker     (121)     2124 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/pymobiledevice3/services/dvt/instruments/device_info.py
--rw-r--r--   0 runner    (1001) docker     (121)      892 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/pymobiledevice3/services/dvt/instruments/energy_monitor.py
--rw-r--r--   0 runner    (1001) docker     (121)      588 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/pymobiledevice3/services/dvt/instruments/graphics.py
--rw-r--r--   0 runner    (1001) docker     (121)     2547 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/pymobiledevice3/services/dvt/instruments/network_monitor.py
--rw-r--r--   0 runner    (1001) docker     (121)      829 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/pymobiledevice3/services/dvt/instruments/notifications.py
--rw-r--r--   0 runner    (1001) docker     (121)     1406 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/pymobiledevice3/services/dvt/instruments/process_control.py
--rw-r--r--   0 runner    (1001) docker     (121)     1575 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/pymobiledevice3/services/dvt/instruments/sysmontap.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1406 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/pymobiledevice3/services/file_relay.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      985 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/pymobiledevice3/services/house_arrest.py
--rw-r--r--   0 runner    (1001) docker     (121)     6130 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/pymobiledevice3/services/installation_proxy.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1809 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/pymobiledevice3/services/mobile_config.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2895 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/pymobiledevice3/services/mobile_image_mounter.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1263 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/pymobiledevice3/services/notification_proxy.py
--rw-r--r--   0 runner    (1001) docker     (121)     3624 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/pymobiledevice3/services/os_trace.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     8856 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/pymobiledevice3/services/pcapd.py
--rwxr-xr-x   0 runner    (1001) docker     (121)      819 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/pymobiledevice3/services/power_assertion.py
--rw-r--r--   0 runner    (1001) docker     (121)    12701 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/pymobiledevice3/services/remote_server.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1317 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/pymobiledevice3/services/screenshot.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     1732 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/pymobiledevice3/services/simulate_location.py
--rw-r--r--   0 runner    (1001) docker     (121)     1551 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/pymobiledevice3/services/springboard.py
--rw-r--r--   0 runner    (1001) docker     (121)     1153 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/pymobiledevice3/services/syslog.py
--rw-r--r--   0 runner    (1001) docker     (121)     4138 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/pymobiledevice3/tcp_forwarder.py
--rw-r--r--   0 runner    (1001) docker     (121)     8747 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/pymobiledevice3/usbmux.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-19 08:39:16.124397 pymobiledevice3-1.9.8/pymobiledevice3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    16354 2021-07-19 08:39:15.000000 pymobiledevice3-1.9.8/pymobiledevice3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3363 2021-07-19 08:39:15.000000 pymobiledevice3-1.9.8/pymobiledevice3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-07-19 08:39:15.000000 pymobiledevice3-1.9.8/pymobiledevice3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       66 2021-07-19 08:39:15.000000 pymobiledevice3-1.9.8/pymobiledevice3.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      138 2021-07-19 08:39:15.000000 pymobiledevice3-1.9.8/pymobiledevice3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       22 2021-07-19 08:39:15.000000 pymobiledevice3-1.9.8/pymobiledevice3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      138 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-07-19 08:39:16.132397 pymobiledevice3-1.9.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1636 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-19 08:39:16.132397 pymobiledevice3-1.9.8/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-19 08:39:16.132397 pymobiledevice3-1.9.8/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/tests/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      358 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/tests/cli/test_mounter.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-19 08:39:16.132397 pymobiledevice3-1.9.8/tests/services/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/tests/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      212 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/tests/services/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-07-19 08:39:16.132397 pymobiledevice3-1.9.8/tests/services/instruments/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/tests/services/instruments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      777 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/tests/services/instruments/test_core_profile_session.py
--rw-r--r--   0 runner    (1001) docker     (121)      664 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/tests/services/test_afc.py
--rw-r--r--   0 runner    (1001) docker     (121)     4321 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/tests/services/test_dvt_secure_socket_proxy.py
--rw-r--r--   0 runner    (1001) docker     (121)      645 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/tests/services/test_pcapd.py
--rw-r--r--   0 runner    (1001) docker     (121)      440 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/tests/services/test_screenshotr_relay.py
--rw-r--r--   0 runner    (1001) docker     (121)      480 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/tests/services/test_springboard_services_relay.py
--rw-r--r--   0 runner    (1001) docker     (121)      979 2021-07-19 08:39:04.000000 pymobiledevice3-1.9.8/tests/services/test_syslog_relay.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-09 09:47:42.795218 pymobiledevice3-1.9.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1065 2021-08-09 09:47:32.000000 pymobiledevice3-1.9.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)    16368 2021-08-09 09:47:42.791217 pymobiledevice3-1.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    13258 2021-08-09 09:47:32.000000 pymobiledevice3-1.9.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-09 09:47:42.779218 pymobiledevice3-1.9.9/pymobiledevice3/
+-rwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1872 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     5315 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/ca.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-09 09:47:42.783218 pymobiledevice3-1.9.9/pymobiledevice3/cli/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1972 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/cli/afc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1571 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/cli/apps.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4874 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/cli/backup.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1272 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/cli/cli_common.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1395 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/cli/crash.py
+-rw-r--r--   0 runner    (1001) docker     (121)    27492 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/cli/developer.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2683 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/cli/diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (121)      679 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/cli/list_devices.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1857 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/cli/lockdown.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3820 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/cli/mounter.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1416 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/cli/notification.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1695 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/cli/pcap.py
+-rw-r--r--   0 runner    (1001) docker     (121)      719 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/cli/power_assertion.py
+-rw-r--r--   0 runner    (1001) docker     (121)      998 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/cli/processes.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1074 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/cli/profile.py
+-rw-r--r--   0 runner    (1001) docker     (121)      998 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/cli/provision.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2295 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/cli/restore.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1755 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/cli/springboard.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4661 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/cli/syslog.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1678 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3223 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/irecv.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    11356 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/lockdown.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-09 09:47:42.783218 pymobiledevice3-1.9.9/pymobiledevice3/resources/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)  1023280 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/resources/dsc_uuid_map.json
+-rw-r--r--   0 runner    (1001) docker     (121)     2520 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/resources/dsc_uuid_map.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1794 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/resources/firmware_notifications.py
+-rw-r--r--   0 runner    (1001) docker     (121)    20970 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/resources/notifications.txt
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-09 09:47:42.787217 pymobiledevice3-1.9.9/pymobiledevice3/restore/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/restore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2979 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/restore/img4.py
+-rw-r--r--   0 runner    (1001) docker     (121)    16208 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/restore/restore.py
+-rw-r--r--   0 runner    (1001) docker     (121)     9471 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/restore/tss.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     3905 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/service_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-09 09:47:42.787217 pymobiledevice3-1.9.9/pymobiledevice3/services/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5807 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/services/accessibilityaudit.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    20621 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/services/afc.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      593 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/services/debugserver_applist.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7341 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/services/device_link.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     5608 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/services/diagnostics.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1433 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/services/dtfetchsymbols.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-09 09:47:42.787217 pymobiledevice3-1.9.9/pymobiledevice3/services/dvt/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/services/dvt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      744 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/services/dvt/dvt_secure_socket_proxy.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-09 09:47:42.791217 pymobiledevice3-1.9.9/pymobiledevice3/services/dvt/instruments/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/services/dvt/instruments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8570 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/services/dvt/instruments/activity_trace_tap.py
+-rw-r--r--   0 runner    (1001) docker     (121)      666 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/services/dvt/instruments/application_listing.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1069 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/services/dvt/instruments/condition_inducer.py
+-rw-r--r--   0 runner    (1001) docker     (121)    26146 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/services/dvt/instruments/core_profile_session_tap.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2124 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/services/dvt/instruments/device_info.py
+-rw-r--r--   0 runner    (1001) docker     (121)      892 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/services/dvt/instruments/energy_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (121)      588 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/services/dvt/instruments/graphics.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2547 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/services/dvt/instruments/network_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (121)      829 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/services/dvt/instruments/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1406 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/services/dvt/instruments/process_control.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1575 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/services/dvt/instruments/sysmontap.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1406 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/services/file_relay.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      985 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/services/house_arrest.py
+-rw-r--r--   0 runner    (1001) docker     (121)     6130 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/services/installation_proxy.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1483 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/services/misagent.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1809 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/services/mobile_config.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     2895 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/services/mobile_image_mounter.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)    12675 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/services/mobilebackup2.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      977 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/services/notification_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4011 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/services/os_trace.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     8856 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/services/pcapd.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)      819 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/services/power_assertion.py
+-rw-r--r--   0 runner    (1001) docker     (121)      629 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/services/preboard.py
+-rw-r--r--   0 runner    (1001) docker     (121)    12701 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/services/remote_server.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1317 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/services/screenshot.py
+-rwxr-xr-x   0 runner    (1001) docker     (121)     1732 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/services/simulate_location.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1551 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/services/springboard.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1153 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/services/syslog.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4148 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/tcp_forwarder.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8865 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/pymobiledevice3/usbmux.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-09 09:47:42.783218 pymobiledevice3-1.9.9/pymobiledevice3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    16368 2021-08-09 09:47:42.000000 pymobiledevice3-1.9.9/pymobiledevice3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3772 2021-08-09 09:47:42.000000 pymobiledevice3-1.9.9/pymobiledevice3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-08-09 09:47:42.000000 pymobiledevice3-1.9.9/pymobiledevice3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       66 2021-08-09 09:47:42.000000 pymobiledevice3-1.9.9/pymobiledevice3.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      149 2021-08-09 09:47:42.000000 pymobiledevice3-1.9.9/pymobiledevice3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       22 2021-08-09 09:47:42.000000 pymobiledevice3-1.9.9/pymobiledevice3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      149 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2021-08-09 09:47:42.795218 pymobiledevice3-1.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1636 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-09 09:47:42.791217 pymobiledevice3-1.9.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-09 09:47:42.791217 pymobiledevice3-1.9.9/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/tests/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      358 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/tests/cli/test_mounter.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-09 09:47:42.791217 pymobiledevice3-1.9.9/tests/services/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/tests/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      212 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/tests/services/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-08-09 09:47:42.791217 pymobiledevice3-1.9.9/tests/services/instruments/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/tests/services/instruments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      777 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/tests/services/instruments/test_core_profile_session.py
+-rw-r--r--   0 runner    (1001) docker     (121)      664 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/tests/services/test_afc.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4321 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/tests/services/test_dvt_secure_socket_proxy.py
+-rw-r--r--   0 runner    (1001) docker     (121)      645 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/tests/services/test_pcapd.py
+-rw-r--r--   0 runner    (1001) docker     (121)      440 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/tests/services/test_screenshotr_relay.py
+-rw-r--r--   0 runner    (1001) docker     (121)      480 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/tests/services/test_springboard_services_relay.py
+-rw-r--r--   0 runner    (1001) docker     (121)      979 2021-08-09 09:47:33.000000 pymobiledevice3-1.9.9/tests/services/test_syslog_relay.py
```

### Comparing `pymobiledevice3-1.9.8/LICENSE` & `pymobiledevice3-1.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-1.9.8/PKG-INFO` & `pymobiledevice3-1.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymobiledevice3
-Version: 1.9.8
+Version: 1.9.9
 Summary: python implementation for libimobiledevice library
 Home-page: https://github.com/doronz88/pymobiledevice3
 Author: DoronZ
 License: UNKNOWN
 Project-URL: pymobiledevice3, https://github.com/doronz88/pymobiledevice3
 Description: [![Python application](https://github.com/doronz88/pymobiledevice3/workflows/Python%20application/badge.svg)](https://github.com/doronz88/pymobiledevice3/actions/workflows/python-app.yml "Python application action")
         [![Pypi version](https://img.shields.io/pypi/v/pymobiledevice3.svg)](https://pypi.org/project/pymobiledevice3/ "PyPi package")
@@ -152,29 +152,29 @@
         DONE | `com.apple.pcapd` | Sniff device's network traffic
         DONE | `com.apple.syslog_relay` | Just streams syslog lines as raw strings
         DONE | `com.apple.os_trace_relay` | More extensive syslog monitoring
         DONE | `com.apple.mobile.diagnostics_relay` | General diagnostic tools
         DONE | `com.apple.mobile.notification_proxy` | API wrapper for `notify_post()` & `notify_register_dispatch()`
         DONE | `com.apple.crashreportmover` | Just trigger `crash_mover` to move all crash reports into crash directory
         DONE | `com.apple.mobile.MCInstall` | Profile management
+        DONE | `com.apple.misagent` | Provisioning Profiles management
         DONE | `com.apple.mobile.assertion_agent` | Create power assertion to prevent different kinds of sleep
         DONE | `com.apple.springboardservices` | Icon related
         DONE | `com.apple.mobile.mobile_image_mounter` | Image mounter service (used for DeveloperDiskImage mounting)
         DONE | `com.apple.mobile.house_arrest` | Get AFC utils (file management per application bundle)
         DONE | `com.apple.mobile.installation_proxy`|  Application management
         DONE | `com.apple.instruments.remoteserver` | Developer instrumentation service, iOS<14  (DeveloperDiskImage)
         DONE | `com.apple.instruments.remoteserver.DVTSecureSocketProxy` | Developer instrumentation service, iOS>=14  (DeveloperDiskImage)
         DONE | `com.apple.mobile.screenshotr` | Take screenshot into a PNG format (DeveloperDiskImage)
         DONE | `com.apple.accessibility.axAuditDaemon.remoteserver` | Accessibility features (DeveloperDiskImage)
         DONE | `com.apple.dt.simulatelocation` | Allows to simulate locations (DeveloperDiskImage)
         DONE | `com.apple.dt.fetchsymbols` | Allows fetching of `dyld` and dyld shared cache files (DeveloperDiskImage)
         Not yet | `com.apple.idamd` | Allows settings the IDAM configuration (whatever that means...)
         Not yet | `com.apple.atc` | AirTraffic related
         Not yet | `com.apple.ait.aitd` | AirTraffic related
-        Not yet | `com.apple.misagent` | Profile related
         Not yet | `com.apple.mobile.file_relay` | File access for iOS <= 8
         Not yet | `com.apple.mobile.heartbeat` | Just a ping to `lockdownd` service
         Not yet | `com.apple.mobile.insecure_notification_proxy` | API wrapper for `notify_post()` & `notify_register_dispatch()` from whitelist
         Not yet | `com.apple.mobilebackup` |
         Not yet | `com.apple.mobilebackup2` |
         Not yet | `com.apple.mobilesync` |
         Not yet | `com.apple.purpletestr` |
```

### Comparing `pymobiledevice3-1.9.8/README.md` & `pymobiledevice3-1.9.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -144,29 +144,29 @@
 DONE | `com.apple.pcapd` | Sniff device's network traffic
 DONE | `com.apple.syslog_relay` | Just streams syslog lines as raw strings
 DONE | `com.apple.os_trace_relay` | More extensive syslog monitoring
 DONE | `com.apple.mobile.diagnostics_relay` | General diagnostic tools
 DONE | `com.apple.mobile.notification_proxy` | API wrapper for `notify_post()` & `notify_register_dispatch()`
 DONE | `com.apple.crashreportmover` | Just trigger `crash_mover` to move all crash reports into crash directory
 DONE | `com.apple.mobile.MCInstall` | Profile management
+DONE | `com.apple.misagent` | Provisioning Profiles management
 DONE | `com.apple.mobile.assertion_agent` | Create power assertion to prevent different kinds of sleep
 DONE | `com.apple.springboardservices` | Icon related
 DONE | `com.apple.mobile.mobile_image_mounter` | Image mounter service (used for DeveloperDiskImage mounting)
 DONE | `com.apple.mobile.house_arrest` | Get AFC utils (file management per application bundle)
 DONE | `com.apple.mobile.installation_proxy`|  Application management
 DONE | `com.apple.instruments.remoteserver` | Developer instrumentation service, iOS<14  (DeveloperDiskImage)
 DONE | `com.apple.instruments.remoteserver.DVTSecureSocketProxy` | Developer instrumentation service, iOS>=14  (DeveloperDiskImage)
 DONE | `com.apple.mobile.screenshotr` | Take screenshot into a PNG format (DeveloperDiskImage)
 DONE | `com.apple.accessibility.axAuditDaemon.remoteserver` | Accessibility features (DeveloperDiskImage)
 DONE | `com.apple.dt.simulatelocation` | Allows to simulate locations (DeveloperDiskImage)
 DONE | `com.apple.dt.fetchsymbols` | Allows fetching of `dyld` and dyld shared cache files (DeveloperDiskImage)
 Not yet | `com.apple.idamd` | Allows settings the IDAM configuration (whatever that means...)
 Not yet | `com.apple.atc` | AirTraffic related
 Not yet | `com.apple.ait.aitd` | AirTraffic related
-Not yet | `com.apple.misagent` | Profile related
 Not yet | `com.apple.mobile.file_relay` | File access for iOS <= 8
 Not yet | `com.apple.mobile.heartbeat` | Just a ping to `lockdownd` service
 Not yet | `com.apple.mobile.insecure_notification_proxy` | API wrapper for `notify_post()` & `notify_register_dispatch()` from whitelist
 Not yet | `com.apple.mobilebackup` |
 Not yet | `com.apple.mobilebackup2` |
 Not yet | `com.apple.mobilesync` |
 Not yet | `com.apple.purpletestr` |
```

### Comparing `pymobiledevice3-1.9.8/pymobiledevice3/__main__.py` & `pymobiledevice3-1.9.9/pymobiledevice3/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,45 @@
 #!/usr/bin/env python3
 import logging
 
 import click
 import coloredlogs
 
-from pymobiledevice3.cli.developer import cli as developer_cli
-from pymobiledevice3.cli.mounter import cli as mounter_cli
+from pymobiledevice3.cli.afc import cli as afc_cli
 from pymobiledevice3.cli.apps import cli as apps_cli
-from pymobiledevice3.cli.profile import cli as profile_cli
-from pymobiledevice3.cli.lockdown import cli as lockdown_cli
-from pymobiledevice3.cli.diagnostics import cli as diagnostics_cli
-from pymobiledevice3.cli.syslog import cli as syslog_cli
-from pymobiledevice3.cli.pcap import cli as pcap_cli
+from pymobiledevice3.cli.backup import cli as backup_cli
 from pymobiledevice3.cli.crash import cli as crash_cli
-from pymobiledevice3.cli.afc import cli as afc_cli
-from pymobiledevice3.cli.processes import cli as ps_cli
-from pymobiledevice3.cli.notification import cli as notification_cli
+from pymobiledevice3.cli.developer import cli as developer_cli
+from pymobiledevice3.cli.diagnostics import cli as diagnostics_cli
 from pymobiledevice3.cli.list_devices import cli as list_devices_cli
+from pymobiledevice3.cli.lockdown import cli as lockdown_cli
+from pymobiledevice3.cli.mounter import cli as mounter_cli
+from pymobiledevice3.cli.notification import cli as notification_cli
+from pymobiledevice3.cli.pcap import cli as pcap_cli
 from pymobiledevice3.cli.power_assertion import cli as power_assertion_cli
+from pymobiledevice3.cli.processes import cli as ps_cli
+from pymobiledevice3.cli.profile import cli as profile_cli
+from pymobiledevice3.cli.provision import cli as provision_cli
+from pymobiledevice3.cli.restore import cli as restore_cli
 from pymobiledevice3.cli.springboard import cli as springboard_cli
+from pymobiledevice3.cli.syslog import cli as syslog_cli
 
 coloredlogs.install(level=logging.DEBUG)
 
 logging.getLogger('asyncio').disabled = True
 logging.getLogger('parso.cache').disabled = True
 logging.getLogger('parso.cache.pickle').disabled = True
 logging.getLogger('parso.python.diff').disabled = True
 logging.getLogger('humanfriendly.prompts').disabled = True
 
 
 def cli():
     cli_commands = click.CommandCollection(sources=[
         developer_cli, mounter_cli, apps_cli, profile_cli, lockdown_cli, diagnostics_cli, syslog_cli, pcap_cli,
         crash_cli, afc_cli, ps_cli, notification_cli, list_devices_cli, power_assertion_cli, springboard_cli,
+        provision_cli, backup_cli, restore_cli
     ])
     cli_commands()
 
 
 if __name__ == '__main__':
     cli()
```

### Comparing `pymobiledevice3-1.9.8/pymobiledevice3/ca.py` & `pymobiledevice3-1.9.9/pymobiledevice3/ca.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-1.9.8/pymobiledevice3/cli/afc.py` & `pymobiledevice3-1.9.9/pymobiledevice3/cli/afc.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-1.9.8/pymobiledevice3/cli/apps.py` & `pymobiledevice3-1.9.9/pymobiledevice3/cli/apps.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-1.9.8/pymobiledevice3/cli/cli_common.py` & `pymobiledevice3-1.9.9/pymobiledevice3/cli/cli_common.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-1.9.8/pymobiledevice3/cli/crash.py` & `pymobiledevice3-1.9.9/pymobiledevice3/cli/crash.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-1.9.8/pymobiledevice3/cli/developer.py` & `pymobiledevice3-1.9.9/pymobiledevice3/cli/developer.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-1.9.8/pymobiledevice3/cli/diagnostics.py` & `pymobiledevice3-1.9.9/pymobiledevice3/cli/diagnostics.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-1.9.8/pymobiledevice3/cli/list_devices.py` & `pymobiledevice3-1.9.9/pymobiledevice3/cli/list_devices.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-1.9.8/pymobiledevice3/cli/lockdown.py` & `pymobiledevice3-1.9.9/pymobiledevice3/cli/lockdown.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import tempfile
 from pprint import pprint
 
 import click
 
-from pymobiledevice3.cli.cli_common import Command
+from pymobiledevice3.cli.cli_common import Command, print_json
 from pymobiledevice3.tcp_forwarder import TcpForwarder
 
 
 @click.group()
 def cli():
     """ apps cli """
     pass
@@ -50,10 +50,17 @@
 @click.argument('service_name')
 def lockdown_service(lockdown, service_name):
     """ send-receive raw service messages """
     lockdown.start_service(service_name).shell()
 
 
 @lockdown_group.command('info', cls=Command)
-def lockdown_info(lockdown):
+@click.option('--color/--no-color', default=True)
+def lockdown_info(lockdown, color):
     """ query all lockdown values """
-    pprint(lockdown.all_values)
+    print_json(lockdown.all_values, colored=color)
+
+
+@lockdown_group.command('unpair', cls=Command)
+def lockdown_unpair(lockdown):
+    """ unpair from connected device """
+    lockdown.unpair()
```

### Comparing `pymobiledevice3-1.9.8/pymobiledevice3/cli/mounter.py` & `pymobiledevice3-1.9.9/pymobiledevice3/cli/mounter.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-1.9.8/pymobiledevice3/cli/notification.py` & `pymobiledevice3-1.9.9/pymobiledevice3/cli/notification.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-1.9.8/pymobiledevice3/cli/pcap.py` & `pymobiledevice3-1.9.9/pymobiledevice3/cli/pcap.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-1.9.8/pymobiledevice3/cli/power_assertion.py` & `pymobiledevice3-1.9.9/pymobiledevice3/cli/power_assertion.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-1.9.8/pymobiledevice3/cli/processes.py` & `pymobiledevice3-1.9.9/pymobiledevice3/cli/processes.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-1.9.8/pymobiledevice3/cli/profile.py` & `pymobiledevice3-1.9.9/pymobiledevice3/cli/profile.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-1.9.8/pymobiledevice3/cli/springboard.py` & `pymobiledevice3-1.9.9/pymobiledevice3/cli/springboard.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-1.9.8/pymobiledevice3/cli/syslog.py` & `pymobiledevice3-1.9.9/pymobiledevice3/cli/syslog.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
     process_name = os.path.basename(filename)
     label = ''
 
     if (pid != -1) and (syslog_pid != pid):
         return None
 
     if syslog_entry.label is not None:
-        label = f'[{syslog_entry.label.bundle_id}][{syslog_entry.label.identifier}]'
+        label = f'[{syslog_entry.label.subsystem}][{syslog_entry.label.category}]'
 
     if color:
         timestamp = colored(str(timestamp), 'green')
         process_name = colored(process_name, 'magenta')
         if len(image_name) > 0:
             image_name = colored(image_name, 'magenta')
         syslog_pid = colored(syslog_entry['pid'], 'cyan')
```

### Comparing `pymobiledevice3-1.9.8/pymobiledevice3/exceptions.py` & `pymobiledevice3-1.9.9/pymobiledevice3/exceptions.py`

 * *Files 14% similar despite different names*

```diff
@@ -59,15 +59,17 @@
 
 
 class ArgumentError(PyMobileDevice3Exception):
     pass
 
 
 class AfcException(PyMobileDevice3Exception):
-    pass
+    def __init__(self, message, status):
+        super(AfcException, self).__init__(message)
+        self.status = status
 
 
 class AfcFileNotFoundError(AfcException):
     pass
 
 
 class DvtException(PyMobileDevice3Exception):
```

### Comparing `pymobiledevice3-1.9.8/pymobiledevice3/lockdown.py` & `pymobiledevice3-1.9.9/pymobiledevice3/lockdown.py`

 * *Files 1% similar despite different names*

```diff
@@ -221,14 +221,19 @@
             self.service.close()
             raise NotTrustedError()
         else:
             self.logger.error(pair.get('Error'))
             self.service.close()
             raise PairingError()
 
+    def unpair(self):
+        req = {'Label': self.label, 'Request': 'Unpair', 'PairRecord': self.pair_record}
+        self.service.send_plist(req)
+        return self.service.recv_plist()
+
     def get_value(self, domain=None, key=None):
         if isinstance(key, str) and hasattr(self, 'record') and hasattr(self.pair_record, key):
             return self.pair_record[key]
 
         req = {'Request': 'GetValue', 'Label': self.label}
 
         if domain:
```

### Comparing `pymobiledevice3-1.9.8/pymobiledevice3/resources/dsc_uuid_map.json` & `pymobiledevice3-1.9.9/pymobiledevice3/resources/dsc_uuid_map.json`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-1.9.8/pymobiledevice3/resources/dsc_uuid_map.py` & `pymobiledevice3-1.9.9/pymobiledevice3/resources/dsc_uuid_map.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-1.9.8/pymobiledevice3/resources/firmware_notifications.py` & `pymobiledevice3-1.9.9/pymobiledevice3/resources/firmware_notifications.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-1.9.8/pymobiledevice3/resources/notifications.txt` & `pymobiledevice3-1.9.9/pymobiledevice3/resources/notifications.txt`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-1.9.8/pymobiledevice3/service_connection.py` & `pymobiledevice3-1.9.9/pymobiledevice3/service_connection.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-1.9.8/pymobiledevice3/services/accessibilityaudit.py` & `pymobiledevice3-1.9.9/pymobiledevice3/services/accessibilityaudit.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-1.9.8/pymobiledevice3/services/afc.py` & `pymobiledevice3-1.9.9/pymobiledevice3/services/afc.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,14 +169,19 @@
 )
 
 afc_fread_req_t = Struct(
     'handle' / Int64ul,
     'size' / Int64ul,
 )
 
+afc_lock_t = Struct(
+    'handle' / Int64ul,
+    'op' / Int64ul,
+)
+
 
 def list_to_dict(d):
     d = d.decode('utf-8')
     t = d.split('\x00')
     t = t[:-1]
 
     assert len(t) % 2 == 0
@@ -327,15 +332,15 @@
             if sz > MAXIMUM_READ_SIZE:
                 to_read = MAXIMUM_READ_SIZE
             else:
                 to_read = sz
             self._dispatch_packet(afc_opcode_t.READ, afc_fread_req_t.build({'handle': handle, 'size': to_read}))
             status, chunk = self._receive_data()
             if status != afc_error_t.SUCCESS:
-                raise AfcException('fread error')
+                raise AfcException('fread error', status)
             sz -= to_read
             data += chunk
         return data
 
     def fwrite(self, handle, data, chunk_size=MAXIMUM_WRITE_SIZE):
         file_handle = struct.pack('<Q', handle)
         chunks_count = len(data) // chunk_size
@@ -366,15 +371,15 @@
     def get_file_contents(self, filename):
         info = self.stat(filename)
         if info:
             if info['st_ifmt'] == 'S_IFLNK':
                 filename = info['LinkTarget']
 
             if info['st_ifmt'] == 'S_IFDIR':
-                raise AfcException(f'{filename} is a directory')
+                raise AfcException(f'{filename} is a directory', afc_error_t.OBJECT_IS_DIR)
 
             h = self.fopen(filename)
             if not h:
                 return
             d = self.fread(h, int(info['st_size']))
             self.fclose(h)
             return d
@@ -400,14 +405,17 @@
         yield dirname, dirs, files
 
         if dirs:
             for d in dirs:
                 for walk_result in self.walk(posixpath.join(dirname, d)):
                     yield walk_result
 
+    def lock(self, handle, operation):
+        return self._do_operation(afc_opcode_t.FILE_LOCK, afc_lock_t.build({'handle': handle, 'op': operation}))
+
     def _dispatch_packet(self, operation, data, this_length=0):
         afcpack = Container(magic=AFCMAGIC,
                             entire_length=afc_header_t.sizeof() + len(data),
                             this_length=afc_header_t.sizeof() + len(data),
                             packet_num=self.packet_num,
                             operation=operation)
         if this_length:
@@ -438,15 +446,15 @@
         status, data = self._receive_data()
 
         exception = AfcException
         if status != afc_error_t.SUCCESS:
             if status == afc_error_t.OBJECT_NOT_FOUND:
                 exception = AfcFileNotFoundError
 
-            raise exception(f'opcode: {opcode} failed with status: {status}')
+            raise exception(f'opcode: {opcode} failed with status: {status}', status)
 
         return data
 
 
 def safe_cmd(f):
     def safe_f(self, *args, **kwargs):
         try:
```

### Comparing `pymobiledevice3-1.9.8/pymobiledevice3/services/debugserver_applist.py` & `pymobiledevice3-1.9.9/pymobiledevice3/services/debugserver_applist.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-1.9.8/pymobiledevice3/services/diagnostics.py` & `pymobiledevice3-1.9.9/pymobiledevice3/services/diagnostics.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-1.9.8/pymobiledevice3/services/dtfetchsymbols.py` & `pymobiledevice3-1.9.9/pymobiledevice3/services/dtfetchsymbols.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-1.9.8/pymobiledevice3/services/dvt/dvt_secure_socket_proxy.py` & `pymobiledevice3-1.9.9/pymobiledevice3/services/dvt/dvt_secure_socket_proxy.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-1.9.8/pymobiledevice3/services/dvt/instruments/activity_trace_tap.py` & `pymobiledevice3-1.9.9/pymobiledevice3/services/dvt/instruments/activity_trace_tap.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-1.9.8/pymobiledevice3/services/dvt/instruments/application_listing.py` & `pymobiledevice3-1.9.9/pymobiledevice3/services/dvt/instruments/application_listing.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-1.9.8/pymobiledevice3/services/dvt/instruments/condition_inducer.py` & `pymobiledevice3-1.9.9/pymobiledevice3/services/dvt/instruments/condition_inducer.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-1.9.8/pymobiledevice3/services/dvt/instruments/core_profile_session_tap.py` & `pymobiledevice3-1.9.9/pymobiledevice3/services/dvt/instruments/core_profile_session_tap.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-1.9.8/pymobiledevice3/services/dvt/instruments/device_info.py` & `pymobiledevice3-1.9.9/pymobiledevice3/services/dvt/instruments/device_info.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-1.9.8/pymobiledevice3/services/dvt/instruments/energy_monitor.py` & `pymobiledevice3-1.9.9/pymobiledevice3/services/dvt/instruments/energy_monitor.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-1.9.8/pymobiledevice3/services/dvt/instruments/graphics.py` & `pymobiledevice3-1.9.9/pymobiledevice3/services/dvt/instruments/graphics.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-1.9.8/pymobiledevice3/services/dvt/instruments/network_monitor.py` & `pymobiledevice3-1.9.9/pymobiledevice3/services/dvt/instruments/network_monitor.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-1.9.8/pymobiledevice3/services/dvt/instruments/notifications.py` & `pymobiledevice3-1.9.9/pymobiledevice3/services/dvt/instruments/notifications.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-1.9.8/pymobiledevice3/services/dvt/instruments/process_control.py` & `pymobiledevice3-1.9.9/pymobiledevice3/services/dvt/instruments/process_control.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-1.9.8/pymobiledevice3/services/dvt/instruments/sysmontap.py` & `pymobiledevice3-1.9.9/pymobiledevice3/services/dvt/instruments/sysmontap.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-1.9.8/pymobiledevice3/services/file_relay.py` & `pymobiledevice3-1.9.9/pymobiledevice3/services/file_relay.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-1.9.8/pymobiledevice3/services/house_arrest.py` & `pymobiledevice3-1.9.9/pymobiledevice3/services/house_arrest.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-1.9.8/pymobiledevice3/services/installation_proxy.py` & `pymobiledevice3-1.9.9/pymobiledevice3/services/installation_proxy.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-1.9.8/pymobiledevice3/services/mobile_config.py` & `pymobiledevice3-1.9.9/pymobiledevice3/services/mobile_config.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-1.9.8/pymobiledevice3/services/mobile_image_mounter.py` & `pymobiledevice3-1.9.9/pymobiledevice3/services/mobile_image_mounter.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-1.9.8/pymobiledevice3/services/notification_proxy.py` & `pymobiledevice3-1.9.9/pymobiledevice3/services/notification_proxy.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import logging
 
-from pymobiledevice3.exceptions import PyMobileDevice3Exception
 from pymobiledevice3.lockdown import LockdownClient
 
 
 class NotificationProxyService(object):
     SERVICE_NAME = 'com.apple.mobile.notification_proxy'
 
     def __init__(self, lockdown: LockdownClient):
@@ -13,19 +12,14 @@
         self.service = self.lockdown.start_service(self.SERVICE_NAME)
 
     def notify_post(self, name):
         """ Send notification to the device's notification_proxy. """
         self.service.send_plist({'Command': 'PostNotification',
                                  'Name': name})
 
-        self.service.send_plist({'Command': 'Shutdown'})
-        res = self.service.recv_plist()
-        if res.get('Command', None) != 'ProxyDeath':
-            raise PyMobileDevice3Exception(f'invalid response: {res}')
-
     def notify_register_dispatch(self, name):
         """ Tells the device to send a notification on the specified event. """
         self.logger.info('Observing %s', name)
         self.service.send_plist({'Command': 'ObserveNotification',
                                  'Name': name})
 
     def receive_notification(self):
```

### Comparing `pymobiledevice3-1.9.8/pymobiledevice3/services/os_trace.py` & `pymobiledevice3-1.9.9/pymobiledevice3/services/os_trace.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,16 @@
 import plistlib
 import struct
 import tempfile
 from datetime import datetime
 from io import BytesIO
 from tarfile import TarFile
 
-from construct import Struct, Bytes, Int32ul, CString, Optional, Enum, Byte, Adapter, Int16ul, this, Computed
+from construct import Struct, Bytes, Int32ul, Optional, Enum, Byte, Adapter, Int16ul, this, Computed, \
+    RepeatUntil
 from pymobiledevice3.exceptions import PyMobileDevice3Exception
 from pymobiledevice3.lockdown import LockdownClient
 
 CHUNK_SIZE = 4096
 TIME_FORMAT = '%H:%M:%S'
 SYSLOG_LINE_SPLITTER = '\n\x00'
 
@@ -44,23 +45,29 @@
     Bytes(42),
     'timestamp' / TimestampAdapter(timestamp_t),
     Bytes(1),
     'level' / Enum(Byte, Notice=0, Info=0x01, Debug=0x02, Error=0x10, Fault=0x11),
     Bytes(38),
     'image_name_size' / Int16ul,
     'message_size' / Int16ul,
-    Bytes(19),
-    'filename' / CString('utf8'),
+    Bytes(6),
+    '_subsystem_size' / Int32ul,
+    '_category_size' / Int32ul,
+    Bytes(4),
+    '_filename' / RepeatUntil(lambda x, lst, ctx: lst[-1] == 0, Byte),
+    'filename' / Computed(lambda ctx: try_decode(bytearray(ctx._filename[:-1]))),
     '_image_name' / Bytes(this.image_name_size),
     'image_name' / Computed(lambda ctx: try_decode(ctx._image_name[:-1])),
     '_message' / Bytes(this.message_size),
     'message' / Computed(lambda ctx: try_decode(ctx._message[:-1])),
     'label' / Optional(Struct(
-        'bundle_id' / CString('utf8'),
-        'identifier' / CString('utf8')
+        '_subsystem' / Bytes(this._._subsystem_size),
+        'subsystem' / Computed(lambda ctx: try_decode(ctx._subsystem[:-1])),
+        '_category' / Bytes(this._._category_size),
+        'category' / Computed(lambda ctx: try_decode(ctx._category[:-1])),
     )),
 )
 
 
 class OsTraceService(object):
     SERVICE_NAME = 'com.apple.os_trace_relay'
```

### Comparing `pymobiledevice3-1.9.8/pymobiledevice3/services/pcapd.py` & `pymobiledevice3-1.9.9/pymobiledevice3/services/pcapd.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-1.9.8/pymobiledevice3/services/power_assertion.py` & `pymobiledevice3-1.9.9/pymobiledevice3/services/power_assertion.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-1.9.8/pymobiledevice3/services/remote_server.py` & `pymobiledevice3-1.9.9/pymobiledevice3/services/remote_server.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-1.9.8/pymobiledevice3/services/screenshot.py` & `pymobiledevice3-1.9.9/pymobiledevice3/services/screenshot.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-1.9.8/pymobiledevice3/services/simulate_location.py` & `pymobiledevice3-1.9.9/pymobiledevice3/services/simulate_location.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-1.9.8/pymobiledevice3/services/springboard.py` & `pymobiledevice3-1.9.9/pymobiledevice3/services/springboard.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-1.9.8/pymobiledevice3/services/syslog.py` & `pymobiledevice3-1.9.9/pymobiledevice3/services/syslog.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-1.9.8/pymobiledevice3/tcp_forwarder.py` & `pymobiledevice3-1.9.9/pymobiledevice3/tcp_forwarder.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 
     def _handle_server_connection(self):
         """ accept the connection from local machine and attempt to connect at remote """
         local_connection, client_address = self.server_socket.accept()
         local_connection.setblocking(False)
 
         try:
-            service_connection = ServiceConnection.create(self.lockdown.udid, self.dst_port)
+            service_connection = ServiceConnection.create_from_udid(self.lockdown.udid, self.dst_port)
 
             if self.enable_ssl:
                 service_connection.ssl_start(self.lockdown.ssl_file, self.lockdown.ssl_file)
 
             remote_connection = service_connection.socket
         except ConnectionFailedError:
             self.logger.error(f'failed to connect to port: {self.dst_port}')
```

### Comparing `pymobiledevice3-1.9.8/pymobiledevice3/usbmux.py` & `pymobiledevice3-1.9.9/pymobiledevice3/usbmux.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import plistlib
 import select
 import socket
 import struct
 import time
 import sys
 
-from pymobiledevice3.exceptions import MuxException, MuxVersionError
+from pymobiledevice3.exceptions import MuxException, MuxVersionError, NotPairedError
 
 MuxDevice = namedtuple('MuxDevice', 'devid usbprod serial location')
 
 
 class SafeStreamSocket:
     def __init__(self, address, family):
         self.sock = socket.socket(family, socket.SOCK_STREAM)
@@ -238,10 +238,12 @@
         tag = self.pkttag
         self.pkttag += 1
         payload = {'PairRecordID': udid}
         self.proto.send_packet('ReadPairRecord', tag, payload)
         _, recvtag, data = self.proto.get_packet()
         if recvtag != tag:
             raise MuxException('Reply tag mismatch: expected %d, got %d' % (tag, recvtag))
-        pair_record = data['PairRecordData']
+        pair_record = data.get('PairRecordData')
+        if pair_record is None:
+            raise NotPairedError('device should be paired first')
         pair_record = plistlib.loads(pair_record)
         return pair_record
```

### Comparing `pymobiledevice3-1.9.8/pymobiledevice3.egg-info/PKG-INFO` & `pymobiledevice3-1.9.9/pymobiledevice3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymobiledevice3
-Version: 1.9.8
+Version: 1.9.9
 Summary: python implementation for libimobiledevice library
 Home-page: https://github.com/doronz88/pymobiledevice3
 Author: DoronZ
 License: UNKNOWN
 Project-URL: pymobiledevice3, https://github.com/doronz88/pymobiledevice3
 Description: [![Python application](https://github.com/doronz88/pymobiledevice3/workflows/Python%20application/badge.svg)](https://github.com/doronz88/pymobiledevice3/actions/workflows/python-app.yml "Python application action")
         [![Pypi version](https://img.shields.io/pypi/v/pymobiledevice3.svg)](https://pypi.org/project/pymobiledevice3/ "PyPi package")
@@ -152,29 +152,29 @@
         DONE | `com.apple.pcapd` | Sniff device's network traffic
         DONE | `com.apple.syslog_relay` | Just streams syslog lines as raw strings
         DONE | `com.apple.os_trace_relay` | More extensive syslog monitoring
         DONE | `com.apple.mobile.diagnostics_relay` | General diagnostic tools
         DONE | `com.apple.mobile.notification_proxy` | API wrapper for `notify_post()` & `notify_register_dispatch()`
         DONE | `com.apple.crashreportmover` | Just trigger `crash_mover` to move all crash reports into crash directory
         DONE | `com.apple.mobile.MCInstall` | Profile management
+        DONE | `com.apple.misagent` | Provisioning Profiles management
         DONE | `com.apple.mobile.assertion_agent` | Create power assertion to prevent different kinds of sleep
         DONE | `com.apple.springboardservices` | Icon related
         DONE | `com.apple.mobile.mobile_image_mounter` | Image mounter service (used for DeveloperDiskImage mounting)
         DONE | `com.apple.mobile.house_arrest` | Get AFC utils (file management per application bundle)
         DONE | `com.apple.mobile.installation_proxy`|  Application management
         DONE | `com.apple.instruments.remoteserver` | Developer instrumentation service, iOS<14  (DeveloperDiskImage)
         DONE | `com.apple.instruments.remoteserver.DVTSecureSocketProxy` | Developer instrumentation service, iOS>=14  (DeveloperDiskImage)
         DONE | `com.apple.mobile.screenshotr` | Take screenshot into a PNG format (DeveloperDiskImage)
         DONE | `com.apple.accessibility.axAuditDaemon.remoteserver` | Accessibility features (DeveloperDiskImage)
         DONE | `com.apple.dt.simulatelocation` | Allows to simulate locations (DeveloperDiskImage)
         DONE | `com.apple.dt.fetchsymbols` | Allows fetching of `dyld` and dyld shared cache files (DeveloperDiskImage)
         Not yet | `com.apple.idamd` | Allows settings the IDAM configuration (whatever that means...)
         Not yet | `com.apple.atc` | AirTraffic related
         Not yet | `com.apple.ait.aitd` | AirTraffic related
-        Not yet | `com.apple.misagent` | Profile related
         Not yet | `com.apple.mobile.file_relay` | File access for iOS <= 8
         Not yet | `com.apple.mobile.heartbeat` | Just a ping to `lockdownd` service
         Not yet | `com.apple.mobile.insecure_notification_proxy` | API wrapper for `notify_post()` & `notify_register_dispatch()` from whitelist
         Not yet | `com.apple.mobilebackup` |
         Not yet | `com.apple.mobilebackup2` |
         Not yet | `com.apple.mobilesync` |
         Not yet | `com.apple.purpletestr` |
```

### Comparing `pymobiledevice3-1.9.8/pymobiledevice3.egg-info/SOURCES.txt` & `pymobiledevice3-1.9.9/pymobiledevice3.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -2,61 +2,73 @@
 README.md
 requirements.txt
 setup.py
 pymobiledevice3/__init__.py
 pymobiledevice3/__main__.py
 pymobiledevice3/ca.py
 pymobiledevice3/exceptions.py
+pymobiledevice3/irecv.py
 pymobiledevice3/lockdown.py
 pymobiledevice3/service_connection.py
 pymobiledevice3/tcp_forwarder.py
 pymobiledevice3/usbmux.py
 pymobiledevice3.egg-info/PKG-INFO
 pymobiledevice3.egg-info/SOURCES.txt
 pymobiledevice3.egg-info/dependency_links.txt
 pymobiledevice3.egg-info/entry_points.txt
 pymobiledevice3.egg-info/requires.txt
 pymobiledevice3.egg-info/top_level.txt
 pymobiledevice3/cli/__init__.py
 pymobiledevice3/cli/afc.py
 pymobiledevice3/cli/apps.py
+pymobiledevice3/cli/backup.py
 pymobiledevice3/cli/cli_common.py
 pymobiledevice3/cli/crash.py
 pymobiledevice3/cli/developer.py
 pymobiledevice3/cli/diagnostics.py
 pymobiledevice3/cli/list_devices.py
 pymobiledevice3/cli/lockdown.py
 pymobiledevice3/cli/mounter.py
 pymobiledevice3/cli/notification.py
 pymobiledevice3/cli/pcap.py
 pymobiledevice3/cli/power_assertion.py
 pymobiledevice3/cli/processes.py
 pymobiledevice3/cli/profile.py
+pymobiledevice3/cli/provision.py
+pymobiledevice3/cli/restore.py
 pymobiledevice3/cli/springboard.py
 pymobiledevice3/cli/syslog.py
 pymobiledevice3/resources/__init__.py
 pymobiledevice3/resources/dsc_uuid_map.json
 pymobiledevice3/resources/dsc_uuid_map.py
 pymobiledevice3/resources/firmware_notifications.py
 pymobiledevice3/resources/notifications.txt
+pymobiledevice3/restore/__init__.py
+pymobiledevice3/restore/img4.py
+pymobiledevice3/restore/restore.py
+pymobiledevice3/restore/tss.py
 pymobiledevice3/services/__init__.py
 pymobiledevice3/services/accessibilityaudit.py
 pymobiledevice3/services/afc.py
 pymobiledevice3/services/debugserver_applist.py
+pymobiledevice3/services/device_link.py
 pymobiledevice3/services/diagnostics.py
 pymobiledevice3/services/dtfetchsymbols.py
 pymobiledevice3/services/file_relay.py
 pymobiledevice3/services/house_arrest.py
 pymobiledevice3/services/installation_proxy.py
+pymobiledevice3/services/misagent.py
 pymobiledevice3/services/mobile_config.py
 pymobiledevice3/services/mobile_image_mounter.py
+pymobiledevice3/services/mobilebackup2.py
 pymobiledevice3/services/notification_proxy.py
 pymobiledevice3/services/os_trace.py
 pymobiledevice3/services/pcapd.py
 pymobiledevice3/services/power_assertion.py
+pymobiledevice3/services/preboard.py
 pymobiledevice3/services/remote_server.py
 pymobiledevice3/services/screenshot.py
 pymobiledevice3/services/simulate_location.py
 pymobiledevice3/services/springboard.py
 pymobiledevice3/services/syslog.py
 pymobiledevice3/services/dvt/__init__.py
 pymobiledevice3/services/dvt/dvt_secure_socket_proxy.py
```

### Comparing `pymobiledevice3-1.9.8/setup.py` & `pymobiledevice3-1.9.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 import os
 
 BASE_DIR = os.path.realpath(os.path.dirname(__file__))
-VERSION = '1.9.8'
+VERSION = '1.9.9'
 
 
 def parse_requirements():
     reqs = []
     if os.path.isfile(os.path.join(BASE_DIR, 'requirements.txt')):
         with open(os.path.join(BASE_DIR, 'requirements.txt'), 'r') as fd:
             for line in fd.readlines():
```

### Comparing `pymobiledevice3-1.9.8/tests/services/instruments/test_core_profile_session.py` & `pymobiledevice3-1.9.9/tests/services/instruments/test_core_profile_session.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-1.9.8/tests/services/test_afc.py` & `pymobiledevice3-1.9.9/tests/services/test_afc.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-1.9.8/tests/services/test_dvt_secure_socket_proxy.py` & `pymobiledevice3-1.9.9/tests/services/test_dvt_secure_socket_proxy.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-1.9.8/tests/services/test_pcapd.py` & `pymobiledevice3-1.9.9/tests/services/test_pcapd.py`

 * *Files identical despite different names*

### Comparing `pymobiledevice3-1.9.8/tests/services/test_syslog_relay.py` & `pymobiledevice3-1.9.9/tests/services/test_syslog_relay.py`

 * *Files identical despite different names*

