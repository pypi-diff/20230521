# Comparing `tmp/pytest-testinfra-8.0.0.tar.gz` & `tmp/pytest-testinfra-8.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-testinfra-8.0.0.tar", last modified: Fri May 19 08:31:51 2023, max compression
+gzip compressed data, was "pytest-testinfra-8.1.0.tar", last modified: Sun May 21 15:38:13 2023, max compression
```

## Comparing `pytest-testinfra-8.0.0.tar` & `pytest-testinfra-8.1.0.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:31:51.302628 pytest-testinfra-8.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)     1708 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11389 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-05-19 08:31:51.302628 pytest-testinfra-8.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/ansible.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/dev-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:31:51.266626 pytest-testinfra-8.0.0/doc/
--rw-r--r--   0 runner    (1001) docker     (123)     6783 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/doc/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:31:51.270626 pytest-testinfra-8.0.0/doc/source/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:31:51.270626 pytest-testinfra-8.0.0/doc/source/_static/
--rw-r--r--   0 runner    (1001) docker     (123)     9916 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/doc/source/_static/logo.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:31:51.270626 pytest-testinfra-8.0.0/doc/source/_templates/
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/doc/source/_templates/piwik.html
--rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/doc/source/api.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7205 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/doc/source/backends.rst
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/doc/source/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9497 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     5206 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/doc/source/examples.rst
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/doc/source/invocation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/doc/source/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/doc/source/support.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:31:51.254625 pytest-testinfra-8.0.0/images/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:31:51.270626 pytest-testinfra-8.0.0/images/alpine/
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/images/alpine/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:31:51.270626 pytest-testinfra-8.0.0/images/archlinux/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/images/archlinux/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:31:51.270626 pytest-testinfra-8.0.0/images/debian_bullseye/
--rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/images/debian_bullseye/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:31:51.274627 pytest-testinfra-8.0.0/images/rockylinux8/
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/images/rockylinux8/Dockerfile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:31:51.274627 pytest-testinfra-8.0.0/images/ubuntu_xenial/
--rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/images/ubuntu_xenial/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:31:51.278627 pytest-testinfra-8.0.0/pytest_testinfra.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-05-19 08:31:51.000000 pytest-testinfra-8.0.0/pytest_testinfra.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-05-19 08:31:51.000000 pytest-testinfra-8.0.0/pytest_testinfra.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-19 08:31:51.000000 pytest-testinfra-8.0.0/pytest_testinfra.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-19 08:31:51.000000 pytest-testinfra-8.0.0/pytest_testinfra.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-19 08:31:51.000000 pytest-testinfra-8.0.0/pytest_testinfra.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-19 08:31:51.000000 pytest-testinfra-8.0.0/pytest_testinfra.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-19 08:31:51.306628 pytest-testinfra-8.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:31:51.278627 pytest-testinfra-8.0.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)     8879 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/test/ssh_key
--rw-r--r--   0 runner    (1001) docker     (123)    21283 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/test/test_backends.py
--rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/test/test_invocation.py
--rw-r--r--   0 runner    (1001) docker     (123)    21843 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/test/test_modules.py
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/test-requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:31:51.282627 pytest-testinfra-8.0.0/testinfra/
--rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:31:51.290627 pytest-testinfra-8.0.0/testinfra/backend/
--rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/backend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/backend/ansible.py
--rw-r--r--   0 runner    (1001) docker     (123)     8345 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/backend/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/backend/chroot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/backend/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/backend/kubectl.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/backend/local.py
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/backend/lxc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/backend/openshift.py
--rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/backend/paramiko.py
--rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/backend/podman.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/backend/salt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/backend/ssh.py
--rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/backend/winrm.py
--rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/host.py
--rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:31:51.302628 pytest-testinfra-8.0.0/testinfra/modules/
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4739 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/modules/addr.py
--rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/modules/ansible.py
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/modules/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/modules/blockdevice.py
--rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/modules/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/modules/docker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/modules/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     8453 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/modules/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/modules/group.py
--rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/modules/interface.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/modules/iptables.py
--rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/modules/mountpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/modules/package.py
--rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/modules/pip.py
--rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/modules/podman.py
--rw-r--r--   0 runner    (1001) docker     (123)     6457 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/modules/process.py
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/modules/puppet.py
--rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/modules/salt.py
--rw-r--r--   0 runner    (1001) docker     (123)     8328 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/modules/service.py
--rw-r--r--   0 runner    (1001) docker     (123)    12724 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/modules/socket.py
--rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/modules/sudo.py
--rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/modules/supervisor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/modules/sysctl.py
--rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/modules/systeminfo.py
--rw-r--r--   0 runner    (1001) docker     (123)     6524 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/modules/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-19 08:31:51.302628 pytest-testinfra-8.0.0/testinfra/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12339 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/testinfra/utils/ansible_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-19 08:31:33.000000 pytest-testinfra-8.0.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 15:38:13.932854 pytest-testinfra-8.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11500 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10142 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-05-21 15:38:13.932854 pytest-testinfra-8.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/ansible.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 15:38:13.920854 pytest-testinfra-8.1.0/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)     6783 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/doc/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 15:38:13.920854 pytest-testinfra-8.1.0/doc/source/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 15:38:13.920854 pytest-testinfra-8.1.0/doc/source/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)     9916 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/doc/source/_static/logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 15:38:13.920854 pytest-testinfra-8.1.0/doc/source/_templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/doc/source/_templates/piwik.html
+-rw-r--r--   0 runner    (1001) docker     (123)      664 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/doc/source/api.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7205 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/doc/source/backends.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/doc/source/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9497 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5206 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/doc/source/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1859 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/doc/source/invocation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4758 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/doc/source/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/doc/source/support.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 15:38:13.916854 pytest-testinfra-8.1.0/images/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 15:38:13.920854 pytest-testinfra-8.1.0/images/alpine/
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/images/alpine/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 15:38:13.920854 pytest-testinfra-8.1.0/images/archlinux/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/images/archlinux/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 15:38:13.920854 pytest-testinfra-8.1.0/images/debian_bullseye/
+-rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/images/debian_bullseye/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 15:38:13.920854 pytest-testinfra-8.1.0/images/rockylinux8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/images/rockylinux8/Dockerfile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 15:38:13.920854 pytest-testinfra-8.1.0/images/ubuntu_xenial/
+-rw-r--r--   0 runner    (1001) docker     (123)     1222 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/images/ubuntu_xenial/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 15:38:13.924854 pytest-testinfra-8.1.0/pytest_testinfra.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3534 2023-05-21 15:38:13.000000 pytest-testinfra-8.1.0/pytest_testinfra.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-05-21 15:38:13.000000 pytest-testinfra-8.1.0/pytest_testinfra.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-21 15:38:13.000000 pytest-testinfra-8.1.0/pytest_testinfra.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-21 15:38:13.000000 pytest-testinfra-8.1.0/pytest_testinfra.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-21 15:38:13.000000 pytest-testinfra-8.1.0/pytest_testinfra.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-21 15:38:13.000000 pytest-testinfra-8.1.0/pytest_testinfra.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-21 15:38:13.932854 pytest-testinfra-8.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 15:38:13.924854 pytest-testinfra-8.1.0/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     8879 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1675 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/test/ssh_key
+-rw-r--r--   0 runner    (1001) docker     (123)    21283 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/test/test_backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/test/test_invocation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21938 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/test/test_modules.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 15:38:13.924854 pytest-testinfra-8.1.0/testinfra/
+-rw-r--r--   0 runner    (1001) docker     (123)      629 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 15:38:13.928854 pytest-testinfra-8.1.0/testinfra/backend/
+-rw-r--r--   0 runner    (1001) docker     (123)     3796 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/backend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/backend/ansible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8345 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/backend/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/backend/chroot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/backend/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/backend/kubectl.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/backend/local.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/backend/lxc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/backend/openshift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/backend/paramiko.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1212 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/backend/podman.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/backend/salt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4414 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/backend/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3135 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/backend/winrm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/host.py
+-rw-r--r--   0 runner    (1001) docker     (123)      704 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 15:38:13.932854 pytest-testinfra-8.1.0/testinfra/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4739 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/modules/addr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4185 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/modules/ansible.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/modules/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4180 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/modules/blockdevice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      854 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/modules/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3766 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/modules/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/modules/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13494 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/modules/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/modules/group.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5472 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/modules/interface.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/modules/iptables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4403 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/modules/mountpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5945 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/modules/package.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/modules/pip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2789 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/modules/podman.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6457 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/modules/process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/modules/puppet.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1707 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/modules/salt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8912 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/modules/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12724 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/modules/socket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1584 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/modules/sudo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5265 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/modules/supervisor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/modules/sysctl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/modules/systeminfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6524 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/modules/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6377 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-21 15:38:13.932854 pytest-testinfra-8.1.0/testinfra/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     1155 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12339 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/testinfra/utils/ansible_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-05-21 15:38:00.000000 pytest-testinfra-8.1.0/tox.ini
```

### Comparing `pytest-testinfra-8.0.0/.pre-commit-config.yaml` & `pytest-testinfra-8.1.0/.pre-commit-config.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -50,13 +50,12 @@
           - flake8-pep3101
           - flake8-print
   - repo: https://github.com/pre-commit/mirrors-mypy
     rev: v0.991
     hooks:
       - id: mypy
         # empty args needed in order to match mypy cli behavior
-        args: []  # [--strict]
         additional_dependencies:
           - types-paramiko
           - types-setuptools
           - setuptools-scm
           - alabaster
```

### Comparing `pytest-testinfra-8.0.0/CHANGELOG.rst` & `pytest-testinfra-8.1.0/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,17 @@
 =========
 Changelog
 =========
 
+8.1.0
+=====
+
+* [NEW] Add Windows support for File and Service modules
+* [NEW] Add File.is_executable property
+
 8.0.0
 =====
 
 * [NEW] Add Group.members attribute
 * [NEW] Add File.inode attribute
 * [NEW] Add Interface.routes() method
 * [NEW] Add Docker.is_restarting attribute
```

### Comparing `pytest-testinfra-8.0.0/CONTRIBUTING.rst` & `pytest-testinfra-8.1.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.0.0/LICENSE` & `pytest-testinfra-8.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.0.0/MANIFEST.in` & `pytest-testinfra-8.1.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.0.0/PKG-INFO` & `pytest-testinfra-8.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-testinfra
-Version: 8.0.0
+Version: 8.1.0
 Summary: Test infrastructures
 Home-page: https://github.com/pytest-dev/pytest-testinfra
 Author: Philippe Pepiot
 Author-email: phil@philpep.org
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `pytest-testinfra-8.0.0/README.rst` & `pytest-testinfra-8.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.0.0/doc/Makefile` & `pytest-testinfra-8.1.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.0.0/doc/source/_static/logo.svg` & `pytest-testinfra-8.1.0/doc/source/_static/logo.svg`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.0.0/doc/source/_templates/piwik.html` & `pytest-testinfra-8.1.0/doc/source/_templates/piwik.html`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.0.0/doc/source/api.rst` & `pytest-testinfra-8.1.0/doc/source/api.rst`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.0.0/doc/source/backends.rst` & `pytest-testinfra-8.1.0/doc/source/backends.rst`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.0.0/doc/source/conf.py` & `pytest-testinfra-8.1.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.0.0/doc/source/examples.rst` & `pytest-testinfra-8.1.0/doc/source/examples.rst`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.0.0/doc/source/invocation.rst` & `pytest-testinfra-8.1.0/doc/source/invocation.rst`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.0.0/doc/source/modules.rst` & `pytest-testinfra-8.1.0/doc/source/modules.rst`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.0.0/doc/source/support.rst` & `pytest-testinfra-8.1.0/doc/source/support.rst`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.0.0/images/alpine/Dockerfile` & `pytest-testinfra-8.1.0/images/alpine/Dockerfile`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.0.0/images/debian_bullseye/Dockerfile` & `pytest-testinfra-8.1.0/images/debian_bullseye/Dockerfile`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.0.0/images/rockylinux8/Dockerfile` & `pytest-testinfra-8.1.0/images/rockylinux8/Dockerfile`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.0.0/images/ubuntu_xenial/Dockerfile` & `pytest-testinfra-8.1.0/images/ubuntu_xenial/Dockerfile`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.0.0/pytest_testinfra.egg-info/PKG-INFO` & `pytest-testinfra-8.1.0/pytest_testinfra.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-testinfra
-Version: 8.0.0
+Version: 8.1.0
 Summary: Test infrastructures
 Home-page: https://github.com/pytest-dev/pytest-testinfra
 Author: Philippe Pepiot
 Author-email: phil@philpep.org
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
```

### Comparing `pytest-testinfra-8.0.0/pytest_testinfra.egg-info/SOURCES.txt` & `pytest-testinfra-8.1.0/pytest_testinfra.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.0.0/setup.cfg` & `pytest-testinfra-8.1.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.0.0/setup.py` & `pytest-testinfra-8.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.0.0/test/conftest.py` & `pytest-testinfra-8.1.0/test/conftest.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.0.0/test/ssh_key` & `pytest-testinfra-8.1.0/test/ssh_key`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.0.0/test/test_backends.py` & `pytest-testinfra-8.1.0/test/test_backends.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.0.0/test/test_invocation.py` & `pytest-testinfra-8.1.0/test/test_invocation.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.0.0/test/test_modules.py` & `pytest-testinfra-8.1.0/test/test_modules.py`

 * *Files 1% similar despite different names*

```diff
@@ -359,14 +359,18 @@
     assert hardlink.inode == f.inode
     assert f == host.file("/d/f")
     assert not d == f
 
     host.check_output("rm -f /d/p && mkfifo /d/p")
     assert host.file("/d/p").is_pipe
 
+    host.check_output("chmod 700 /d/f")
+    assert f.is_executable
+    assert f.mode == 0o700
+
 
 def test_ansible_unavailable(host):
     expected = "Ansible module is only available with " "ansible connection backend"
     with pytest.raises(RuntimeError) as excinfo:
         host.ansible("setup")
     assert expected in str(excinfo.value)
     with pytest.raises(RuntimeError) as excinfo:
```

### Comparing `pytest-testinfra-8.0.0/testinfra/__init__.py` & `pytest-testinfra-8.1.0/testinfra/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.0.0/testinfra/backend/__init__.py` & `pytest-testinfra-8.1.0/testinfra/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.0.0/testinfra/backend/ansible.py` & `pytest-testinfra-8.1.0/testinfra/backend/ansible.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.0.0/testinfra/backend/base.py` & `pytest-testinfra-8.1.0/testinfra/backend/base.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.0.0/testinfra/backend/chroot.py` & `pytest-testinfra-8.1.0/testinfra/backend/chroot.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.0.0/testinfra/backend/docker.py` & `pytest-testinfra-8.1.0/testinfra/backend/docker.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.0.0/testinfra/backend/kubectl.py` & `pytest-testinfra-8.1.0/testinfra/backend/kubectl.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.0.0/testinfra/backend/local.py` & `pytest-testinfra-8.1.0/testinfra/backend/local.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.0.0/testinfra/backend/lxc.py` & `pytest-testinfra-8.1.0/testinfra/backend/lxc.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.0.0/testinfra/backend/openshift.py` & `pytest-testinfra-8.1.0/testinfra/backend/openshift.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.0.0/testinfra/backend/paramiko.py` & `pytest-testinfra-8.1.0/testinfra/backend/paramiko.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.0.0/testinfra/backend/podman.py` & `pytest-testinfra-8.1.0/testinfra/backend/podman.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.0.0/testinfra/backend/salt.py` & `pytest-testinfra-8.1.0/testinfra/backend/salt.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.0.0/testinfra/backend/ssh.py` & `pytest-testinfra-8.1.0/testinfra/backend/ssh.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.0.0/testinfra/backend/winrm.py` & `pytest-testinfra-8.1.0/testinfra/backend/winrm.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.0.0/testinfra/host.py` & `pytest-testinfra-8.1.0/testinfra/host.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.0.0/testinfra/main.py` & `pytest-testinfra-8.1.0/testinfra/main.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.0.0/testinfra/modules/__init__.py` & `pytest-testinfra-8.1.0/testinfra/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.0.0/testinfra/modules/addr.py` & `pytest-testinfra-8.1.0/testinfra/modules/addr.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.0.0/testinfra/modules/ansible.py` & `pytest-testinfra-8.1.0/testinfra/modules/ansible.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.0.0/testinfra/modules/base.py` & `pytest-testinfra-8.1.0/testinfra/modules/base.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.0.0/testinfra/modules/blockdevice.py` & `pytest-testinfra-8.1.0/testinfra/modules/blockdevice.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.0.0/testinfra/modules/command.py` & `pytest-testinfra-8.1.0/testinfra/modules/command.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.0.0/testinfra/modules/docker.py` & `pytest-testinfra-8.1.0/testinfra/modules/docker.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.0.0/testinfra/modules/environment.py` & `pytest-testinfra-8.1.0/testinfra/modules/environment.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.0.0/testinfra/modules/file.py` & `pytest-testinfra-8.1.0/testinfra/modules/service.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,313 +6,296 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import datetime
-
 from testinfra.modules.base import Module
+from testinfra.utils import cached_property
 
 
-class File(Module):
-    """Test various files attributes"""
-
-    def __init__(self, path):
-        self.path = path
-        super().__init__()
-
-    @property
-    def exists(self):
-        """Test if file exists
-
-        >>> host.file("/etc/passwd").exists
-        True
-        >>> host.file("/nonexistent").exists
-        False
+class Service(Module):
+    """Test services
 
-        """
-        return self.run_test("test -e %s", self.path).rc == 0
+    Implementations:
 
-    @property
-    def is_file(self):
-        return self.run_test("test -f %s", self.path).rc == 0
+    - Linux: detect Systemd, Upstart or OpenRC, fallback to SysV
+    - FreeBSD: service(1)
+    - OpenBSD: ``/etc/rc.d/$name check`` for ``is_running``
+      ``rcctl ls on`` for ``is_enabled`` (only OpenBSD >= 5.8)
+    - NetBSD: ``/etc/rc.d/$name onestatus`` for ``is_running``
+      (``is_enabled`` is not yet implemented)
 
-    @property
-    def is_directory(self):
-        return self.run_test("test -d %s", self.path).rc == 0
+    """
 
-    @property
-    def is_pipe(self):
-        return self.run_test("test -p %s", self.path).rc == 0
-
-    @property
-    def is_socket(self):
-        return self.run_test("test -S %s", self.path).rc == 0
-
-    @property
-    def is_symlink(self):
-        return self.run_test("test -L %s", self.path).rc == 0
-
-    @property
-    def linked_to(self):
-        """Resolve symlink
-
-        >>> host.file("/var/lock").linked_to
-        '/run/lock'
-        """
-        res = self.run_expect([0, 127], "realpath %s", self.path)
-        if res.rc == 0:
-            return res.stdout.strip()
-        return self.check_output("readlink -f %s", self.path)
+    def __init__(self, name):
+        self.name = name
+        super().__init__()
 
     @property
-    def user(self):
-        """Return file owner as string
-
-        >>> host.file("/etc/passwd").user
-        'root'
-        """
+    def is_running(self):
+        """Test if service is running"""
         raise NotImplementedError
 
     @property
-    def uid(self):
-        """Return file user id as integer
-
-        >>> host.file("/etc/passwd").uid
-        0
-        """
+    def is_enabled(self):
+        """Test if service is enabled"""
         raise NotImplementedError
 
     @property
-    def group(self):
-        raise NotImplementedError
+    def is_valid(self):
+        """Test if service is valid
 
-    @property
-    def gid(self):
+        This method is only available in the systemd implementation,
+        it will raise ``NotImplementedError`` in others implementation
+        """
         raise NotImplementedError
 
     @property
-    def mode(self):
-        """Return file mode as octal integer
-
-        >>> host.file("/etc/shadow").mode
-        416  # Oo640 octal
-        >>> host.file("/etc/shadow").mode == 0o640
-        True
-        >>> oct(host.file("/etc/shadow").mode) == '0o640'
-        True
-
-        You can also utilize the file mode constants from
-        the stat_ library for testing file mode.
-
-        >>> import stat
-        >>> host.file("/etc/shadow").mode == stat.S_IRUSR | stat.S_IWUSR | stat.S_IRGRP
-        True
-
-        .. _oct(x): https://docs.python.org/3/library/functions.html#oct
-        .. _stat: https://docs.python.org/3/library/stat.html
-        """  # noqa
-        raise NotImplementedError
-
-    def contains(self, pattern):
-        """Checks content of file for pattern
+    def is_masked(self):
+        """Test if service is masked
 
-        This uses grep and thus follows the grep regex syntax.
+        This method is only available in the systemd implementation,
+        it will raise ``NotImplementedError`` in others implementations
         """
-        return self.run_test("grep -qs -- %s %s", pattern, self.path).rc == 0
-
-    @property
-    def md5sum(self):
         raise NotImplementedError
 
-    @property
-    def sha256sum(self):
-        raise NotImplementedError
+    @cached_property
+    def systemd_properties(self):
+        """Properties of the service (unit).
 
-    def _get_content(self, decode):
-        out = self.run_test("cat -- %s", self.path)
-        if out.rc != 0:
-            raise RuntimeError("Unexpected output {}".format(out))
-        if decode:
-            return out.stdout
-        return out.stdout_bytes
+        Return service properties as a `dict`,
+        empty properties are not returned.
 
-    @property
-    def content(self):
-        """Return file content as bytes
-
-        >>> host.file("/tmp/foo").content
-        b'caf\\xc3\\xa9'
-        """
-        return self._get_content(False)
-
-    @property
-    def content_string(self):
-        """Return file content as string
+        >>> ntp = host.service("ntp")
+        >>> ntp.systemd_properties["FragmentPath"]
+        '/lib/systemd/system/ntp.service'
 
-        >>> host.file("/tmp/foo").content_string
-        'café'
-        """
-        return self._get_content(True)
+        This method is only available in the systemd implementation,
+        it will raise ``NotImplementedError`` in others implementations
 
-    @property
-    def mtime(self):
-        """Return time of last modification as datetime.datetime object
+        Note: based on `systemctl show`_
 
-        >>> host.file("/etc/passwd").mtime
-        datetime.datetime(2015, 3, 15, 20, 25, 40)
+        .. _systemctl show: https://man7.org/linux/man-pages/man1/systemctl.1.html
         """
         raise NotImplementedError
 
-    @property
-    def size(self):
-        """Return size of file in bytes"""
-        raise NotImplementedError
-
-    def listdir(self):
-        """Return list of items under the directory
-
-        >>> host.file("/tmp").listdir()
-        ['foo_file', 'bar_dir']
-        """
-        out = self.run_test("ls -1 -q -- %s", self.path)
-        if out.rc != 0:
-            raise RuntimeError("Unexpected output {}".format(out))
-        return out.stdout.splitlines()
-
-    def __repr__(self):
-        return "<file {}>".format(self.path)
-
-    def __eq__(self, other):
-        if isinstance(other, File):
-            return self.path == other.path
-        if isinstance(other, str):
-            return self.path == other
-        return False
-
     @classmethod
     def get_module_class(cls, host):
         if host.system_info.type == "linux":
-            return GNUFile
+            if host.file("/run/systemd/system/").is_directory or (
+                host.exists("systemctl")
+                and "systemd" in host.file("/sbin/init").linked_to
+            ):
+                return SystemdService
+            if (
+                host.exists("initctl")
+                and host.exists("status")
+                and host.file("/etc/init").is_directory
+            ):
+                return UpstartService
+            if host.exists("rc-service"):
+                return OpenRCService
+            return SysvService
+        if host.system_info.type == "freebsd":
+            return FreeBSDService
+        if host.system_info.type == "openbsd":
+            return OpenBSDService
         if host.system_info.type == "netbsd":
-            return NetBSDFile
-        if host.system_info.type.endswith("bsd"):
-            return BSDFile
-        if host.system_info.type == "darwin":
-            return DarwinFile
+            return NetBSDService
+        if host.system_info.type == "windows":
+            return WindowsService
         raise NotImplementedError
 
+    def __repr__(self):
+        return "<service {}>".format(self.name)
 
-class GNUFile(File):
-    @property
-    def user(self):
-        return self.check_output("stat -c %%U %s", self.path)
-
-    @property
-    def uid(self):
-        return int(self.check_output("stat -c %%u %s", self.path))
-
-    @property
-    def group(self):
-        return self.check_output("stat -c %%G %s", self.path)
-
-    @property
-    def gid(self):
-        return int(self.check_output("stat -c %%g %s", self.path))
-
-    @property
-    def mode(self):
-        # Supply a base of 8 when parsing an octal integer
-        # e.g. int('644', 8) -> 420
-        return int(self.check_output("stat -c %%a %s", self.path), 8)
-
-    @property
-    def mtime(self):
-        ts = self.check_output("stat -c %%Y %s", self.path)
-        return datetime.datetime.fromtimestamp(float(ts))
 
-    @property
-    def size(self):
-        return int(self.check_output("stat -c %%s %s", self.path))
+class SysvService(Service):
+    @cached_property
+    def _service_command(self):
+        return self.find_command("service")
+
+    @property
+    def is_running(self):
+        # based on /lib/lsb/init-functions
+        # 0: program running
+        # 1: program is dead and pid file exists
+        # 3: not running and pid file does not exists
+        # 4: Unable to determine status
+        # 8: starting (alpine specific ?)
+        return (
+            self.run_expect(
+                [0, 1, 3, 8], "%s %s status", self._service_command, self.name
+            ).rc
+            == 0
+        )
 
     @property
-    def inode(self):
-        return int(self.check_output("stat -c %%i %s", self.path))
+    def is_enabled(self):
+        return bool(
+            self.check_output(
+                "find -L /etc/rc?.d/ -name %s",
+                "S??" + self.name,
+            )
+        )
 
-    @property
-    def md5sum(self):
-        return self.check_output("md5sum %s | cut -d' ' -f1", self.path)
 
+class SystemdService(SysvService):
     @property
-    def sha256sum(self):
-        return self.check_output("sha256sum %s | cut -d ' ' -f 1", self.path)
-
+    def is_running(self):
+        out = self.run_expect([0, 1, 3], "systemctl is-active %s", self.name)
+        if out.rc == 1:
+            # Failed to connect to bus: No such file or directory
+            return super().is_running
+        return out.rc == 0
+
+    @property
+    def is_enabled(self):
+        cmd = self.run_test("systemctl is-enabled %s", self.name)
+        if cmd.rc == 0:
+            return True
+        if cmd.stdout.strip() == "disabled":
+            return False
+        # Fallback on SysV
+        # https://bugs.debian.org/cgi-bin/bugreport.cgi?bug=760616
+        return super().is_enabled
+
+    @property
+    def is_valid(self):
+        # systemd-analyze requires a full path.
+        if self.name.endswith(".service"):
+            name = self.name
+        else:
+            name = self.name + ".service"
+        cmd = self.run("systemd-analyze verify %s", name)
+        # A bad unit file still returns a rc of 0, so check the
+        # stdout for anything.  Nothing means no warns/errors.
+        # Docs at https://www.freedesktop.org/software/systemd/man/systemd
+        # -analyze.html#Examples%20for%20verify
+        assert (cmd.stdout, cmd.stderr) == ("", "")
+        return True
+
+    @property
+    def is_masked(self):
+        cmd = self.run_test("systemctl is-enabled %s", self.name)
+        return cmd.stdout.strip() == "masked"
+
+    @cached_property
+    def systemd_properties(self):
+        out = self.check_output("systemctl show %s", self.name)
+        out_d = {}
+        if out:
+            # maxsplit is required because values can contain `=`
+            out_d = dict(
+                map(lambda pair: pair.split("=", maxsplit=1), out.splitlines())
+            )
+        return out_d
+
+
+class UpstartService(SysvService):
+    @property
+    def is_enabled(self):
+        if (
+            self.run(
+                "grep -q '^start on' /etc/init/%s.conf",
+                self.name,
+            ).rc
+            == 0
+            and self.run(
+                "grep -q '^manual' /etc/init/%s.override",
+                self.name,
+            ).rc
+            != 0
+        ):
+            return True
+        # Fallback on SysV
+        return super().is_enabled
+
+    @property
+    def is_running(self):
+        cmd = self.run_test("status %s", self.name)
+        if cmd.rc == 0 and len(cmd.stdout.split()) > 1:
+            return "running" in cmd.stdout.split()[1]
+        return super().is_running
+
+
+class OpenRCService(SysvService):
+    @cached_property
+    def _service_command(self):
+        return self.find_command("rc-service")
+
+    @property
+    def is_enabled(self):
+        return bool(
+            self.check_output(
+                "find /etc/runlevels/ -name %s",
+                self.name,
+            )
+        )
 
-class BSDFile(File):
-    @property
-    def user(self):
-        return self.check_output("stat -f %%Su %s", self.path)
 
+class FreeBSDService(Service):
     @property
-    def uid(self):
-        return int(self.check_output("stat -f %%u %s", self.path))
+    def is_running(self):
+        return self.run_test("service %s onestatus", self.name).rc == 0
 
     @property
-    def group(self):
-        return self.check_output("stat -f %%Sg %s", self.path)
+    def is_enabled(self):
+        # Return list of enabled services like
+        # /etc/rc.d/sshd
+        # /etc/rc.d/sendmail
+        for path in self.check_output("service -e").splitlines():
+            if path and path.rsplit("/", 1)[1] == self.name:
+                return True
+        return False
 
-    @property
-    def gid(self):
-        return int(self.check_output("stat -f %%g %s", self.path))
 
+class OpenBSDService(Service):
     @property
-    def mode(self):
-        # Supply a base of 8 when parsing an octal integer
-        # e.g. int('644', 8) -> 420
-        return int(self.check_output("stat -f %%Lp %s", self.path), 8)
+    def is_running(self):
+        return self.run_test("/etc/rc.d/%s check", self.name).rc == 0
 
     @property
-    def mtime(self):
-        ts = self.check_output("stat -f %%m %s", self.path)
-        return datetime.datetime.fromtimestamp(float(ts))
+    def is_enabled(self):
+        if self.name in self.check_output("rcctl ls on").splitlines():
+            return True
+        if self.name in self.check_output("rcctl ls off").splitlines():
+            return False
+        raise RuntimeError(
+            "Unable to determine state of {0}. Does this service exist?".format(
+                self.name
+            )
+        )
 
-    @property
-    def size(self):
-        return int(self.check_output("stat -f %%z %s", self.path))
 
+class NetBSDService(Service):
     @property
-    def md5sum(self):
-        return self.check_output("md5 < %s", self.path)
+    def is_running(self):
+        return self.run_test("/etc/rc.d/%s onestatus", self.name).rc == 0
 
     @property
-    def sha256sum(self):
-        return self.check_output("sha256 < %s", self.path)
+    def is_enabled(self):
+        raise NotImplementedError
 
 
-class DarwinFile(BSDFile):
+class WindowsService(Service):
     @property
-    def linked_to(self):
-        link_script = """
-        TARGET_FILE='{0}'
-        cd `dirname $TARGET_FILE`
-        TARGET_FILE=`basename $TARGET_FILE`
-        while [ -L "$TARGET_FILE" ]
-        do
-            TARGET_FILE=`readlink $TARGET_FILE`
-            cd `dirname $TARGET_FILE`
-            TARGET_FILE=`basename $TARGET_FILE`
-        done
-        PHYS_DIR=`pwd -P`
-        RESULT=$PHYS_DIR/$TARGET_FILE
-        echo $RESULT
-        """.format(
-            self.path
+    def is_running(self):
+        return (
+            self.check_output(
+                "Get-Service '%s' | Select -ExpandProperty Status",
+                self.name,
+            )
+            == "Running"
         )
-        return self.check_output(link_script)
 
-
-class NetBSDFile(BSDFile):
     @property
-    def sha256sum(self):
-        return self.check_output("cksum -a sha256 < %s", self.path)
+    def is_enabled(self):
+        return (
+            self.check_output(
+                "Get-Service '%s' | Select -ExpandProperty StartType",
+                self.name,
+            )
+            == "Automatic"
+        )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `pytest-testinfra-8.0.0/testinfra/modules/group.py` & `pytest-testinfra-8.1.0/testinfra/modules/group.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.0.0/testinfra/modules/interface.py` & `pytest-testinfra-8.1.0/testinfra/modules/interface.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.0.0/testinfra/modules/iptables.py` & `pytest-testinfra-8.1.0/testinfra/modules/iptables.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.0.0/testinfra/modules/mountpoint.py` & `pytest-testinfra-8.1.0/testinfra/modules/mountpoint.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.0.0/testinfra/modules/package.py` & `pytest-testinfra-8.1.0/testinfra/modules/package.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.0.0/testinfra/modules/pip.py` & `pytest-testinfra-8.1.0/testinfra/modules/pip.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.0.0/testinfra/modules/podman.py` & `pytest-testinfra-8.1.0/testinfra/modules/podman.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.0.0/testinfra/modules/process.py` & `pytest-testinfra-8.1.0/testinfra/modules/process.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.0.0/testinfra/modules/puppet.py` & `pytest-testinfra-8.1.0/testinfra/modules/puppet.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.0.0/testinfra/modules/salt.py` & `pytest-testinfra-8.1.0/testinfra/modules/salt.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.0.0/testinfra/modules/socket.py` & `pytest-testinfra-8.1.0/testinfra/modules/socket.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.0.0/testinfra/modules/sudo.py` & `pytest-testinfra-8.1.0/testinfra/modules/sudo.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.0.0/testinfra/modules/supervisor.py` & `pytest-testinfra-8.1.0/testinfra/modules/supervisor.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.0.0/testinfra/modules/sysctl.py` & `pytest-testinfra-8.1.0/testinfra/modules/sysctl.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.0.0/testinfra/modules/systeminfo.py` & `pytest-testinfra-8.1.0/testinfra/modules/systeminfo.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.0.0/testinfra/modules/user.py` & `pytest-testinfra-8.1.0/testinfra/modules/user.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.0.0/testinfra/plugin.py` & `pytest-testinfra-8.1.0/testinfra/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.0.0/testinfra/utils/__init__.py` & `pytest-testinfra-8.1.0/testinfra/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.0.0/testinfra/utils/ansible_runner.py` & `pytest-testinfra-8.1.0/testinfra/utils/ansible_runner.py`

 * *Files identical despite different names*

### Comparing `pytest-testinfra-8.0.0/tox.ini` & `pytest-testinfra-8.1.0/tox.ini`

 * *Files identical despite different names*

