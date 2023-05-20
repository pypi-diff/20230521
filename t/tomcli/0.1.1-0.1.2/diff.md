# Comparing `tmp/tomcli-0.1.1.tar.gz` & `tmp/tomcli-0.1.2.tar.gz`

## Comparing `tomcli-0.1.1.tar` & `tomcli-0.1.2.tar`

### file list

```diff
@@ -1,467 +1,492 @@
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 tomcli-0.1.1/CONTRIBUTING.md
--rw-r--r--   0        0        0      666 2020-02-02 00:00:00.000000 tomcli-0.1.1/NEWS.md
--rw-r--r--   0        0        0     9035 2020-02-02 00:00:00.000000 tomcli-0.1.1/noxfile.py
--rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 tomcli-0.1.1/ruff.toml
--rw-r--r--   0        0        0     2417 2020-02-02 00:00:00.000000 tomcli-0.1.1/tomcli.spec
--rw-r--r--   0        0        0      356 2020-02-02 00:00:00.000000 tomcli-0.1.1/.builds/nox-lint.yml
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 tomcli-0.1.1/.builds/nox-mockbuild-36.yml
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 tomcli-0.1.1/.builds/nox-mockbuild.yml
--rw-r--r--   0        0        0      542 2020-02-02 00:00:00.000000 tomcli-0.1.1/.builds/nox.yml
--rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 tomcli-0.1.1/.copr/Makefile
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/.gitignore
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/@plugins_snapshot.json
--rw-r--r--   0        0        0     7860 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/__future__.data.json
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/__future__.meta.json
--rw-r--r--   0        0        0   180407 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/_ast.data.json
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/_ast.meta.json
--rw-r--r--   0        0        0    52439 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/_codecs.data.json
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/_codecs.meta.json
--rw-r--r--   0        0        0    18266 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/_collections_abc.data.json
--rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/_collections_abc.meta.json
--rw-r--r--   0        0        0     3164 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/_ctypes.data.json
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/_ctypes.meta.json
--rw-r--r--   0        0        0   171970 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/_decimal.data.json
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/_decimal.meta.json
--rw-r--r--   0        0        0   113968 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/_operator.data.json
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/_operator.meta.json
--rw-r--r--   0        0        0     6134 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/_random.data.json
--rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/_random.meta.json
--rw-r--r--   0        0        0    19742 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/_stat.data.json
--rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/_stat.meta.json
--rw-r--r--   0        0        0    23900 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/_thread.data.json
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/_thread.meta.json
--rw-r--r--   0        0        0    13117 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/_warnings.data.json
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/_warnings.meta.json
--rw-r--r--   0        0        0    27348 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/_weakref.data.json
--rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/_weakref.meta.json
--rw-r--r--   0        0        0    50468 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/_weakrefset.data.json
--rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/_weakrefset.meta.json
--rw-r--r--   0        0        0    23375 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/abc.data.json
--rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/abc.meta.json
--rw-r--r--   0        0        0    60715 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/array.data.json
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/array.meta.json
--rw-r--r--   0        0        0  1130451 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/builtins.data.json
--rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/builtins.meta.json
--rw-r--r--   0        0        0   123356 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/codecs.data.json
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/codecs.meta.json
--rw-r--r--   0        0        0   109243 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/contextlib.data.json
--rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/contextlib.meta.json
--rw-r--r--   0        0        0     5448 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/copy.data.json
--rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/copy.meta.json
--rw-r--r--   0        0        0    57784 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/dataclasses.data.json
--rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/dataclasses.meta.json
--rw-r--r--   0        0        0   141567 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/datetime.data.json
--rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/datetime.meta.json
--rw-r--r--   0        0        0     4950 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/decimal.data.json
--rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/decimal.meta.json
--rw-r--r--   0        0        0    58330 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/difflib.data.json
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/difflib.meta.json
--rw-r--r--   0        0        0    62945 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/dis.data.json
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/dis.meta.json
--rw-r--r--   0        0        0    90162 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/enum.data.json
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/enum.meta.json
--rw-r--r--   0        0        0    27315 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/errno.data.json
--rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/errno.meta.json
--rw-r--r--   0        0        0    88816 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/fractions.data.json
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/fractions.meta.json
--rw-r--r--   0        0        0   130394 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/functools.data.json
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/functools.meta.json
--rw-r--r--   0        0        0    22427 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/genericpath.data.json
--rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/genericpath.meta.json
--rw-r--r--   0        0        0     3778 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/getpass.data.json
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/getpass.meta.json
--rw-r--r--   0        0        0    46229 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/gettext.data.json
--rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/gettext.meta.json
--rw-r--r--   0        0        0     9543 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/glob.data.json
--rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/glob.meta.json
--rw-r--r--   0        0        0   322714 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/inspect.data.json
--rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/inspect.meta.json
--rw-r--r--   0        0        0    85376 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/io.data.json
--rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/io.meta.json
--rw-r--r--   0        0        0   266348 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/itertools.data.json
--rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/itertools.meta.json
--rw-r--r--   0        0        0    52550 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/math.data.json
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/math.meta.json
--rw-r--r--   0        0        0    28806 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/mmap.data.json
--rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/mmap.meta.json
--rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/msvcrt.data.json
--rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/msvcrt.meta.json
--rw-r--r--   0        0        0    79021 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/numbers.data.json
--rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/numbers.meta.json
--rw-r--r--   0        0        0     6133 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/opcode.data.json
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/opcode.meta.json
--rw-r--r--   0        0        0    49237 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/operator.data.json
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/operator.meta.json
--rw-r--r--   0        0        0    87503 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/pathlib.data.json
--rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/pathlib.meta.json
--rw-r--r--   0        0        0    44432 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/pickle.data.json
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/pickle.meta.json
--rw-r--r--   0        0        0    75236 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/posixpath.data.json
--rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/posixpath.meta.json
--rw-r--r--   0        0        0    40067 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/random.data.json
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/random.meta.json
--rw-r--r--   0        0        0   167584 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/re.data.json
--rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/re.meta.json
--rw-r--r--   0        0        0    16322 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/shlex.data.json
--rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/shlex.meta.json
--rw-r--r--   0        0        0    71151 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/shutil.data.json
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/shutil.meta.json
--rw-r--r--   0        0        0    14412 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/sre_compile.data.json
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/sre_compile.meta.json
--rw-r--r--   0        0        0    28519 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/sre_constants.data.json
--rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/sre_constants.meta.json
--rw-r--r--   0        0        0    49780 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/sre_parse.data.json
--rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/sre_parse.meta.json
--rw-r--r--   0        0        0     6569 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/stat.data.json
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/stat.meta.json
--rw-r--r--   0        0        0    27787 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/string.data.json
--rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/string.meta.json
--rw-r--r--   0        0        0   162203 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/subprocess.data.json
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/subprocess.meta.json
--rw-r--r--   0        0        0   142491 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/sys.data.json
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/sys.meta.json
--rw-r--r--   0        0        0   140364 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tempfile.data.json
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tempfile.meta.json
--rw-r--r--   0        0        0    49134 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/termios.data.json
--rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/termios.meta.json
--rw-r--r--   0        0        0    19592 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/textwrap.data.json
--rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/textwrap.meta.json
--rw-r--r--   0        0        0    64754 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/threading.data.json
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/threading.meta.json
--rw-r--r--   0        0        0    43644 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/time.data.json
--rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/time.meta.json
--rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomllib.data.json
--rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomllib.meta.json
--rw-r--r--   0        0        0    57057 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/traceback.data.json
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/traceback.meta.json
--rw-r--r--   0        0        0     4865 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tty.data.json
--rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tty.meta.json
--rw-r--r--   0        0        0   239671 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/types.data.json
--rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/types.meta.json
--rw-r--r--   0        0        0   432441 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/typing.data.json
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/typing.meta.json
--rw-r--r--   0        0        0    57905 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/typing_extensions.data.json
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/typing_extensions.meta.json
--rw-r--r--   0        0        0    33625 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/uuid.data.json
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/uuid.meta.json
--rw-r--r--   0        0        0    23828 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/warnings.data.json
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/warnings.meta.json
--rw-r--r--   0        0        0   142967 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/weakref.data.json
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/weakref.meta.json
--rw-r--r--   0        0        0    24308 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/webbrowser.data.json
--rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/webbrowser.meta.json
--rw-r--r--   0        0        0    89093 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/_typeshed/__init__.data.json
--rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/_typeshed/__init__.meta.json
--rw-r--r--   0        0        0     7789 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/click/__init__.data.json
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/click/__init__.meta.json
--rw-r--r--   0        0        0    47214 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/click/_compat.data.json
--rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/click/_compat.meta.json
--rw-r--r--   0        0        0    44790 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/click/_termui_impl.data.json
--rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/click/_termui_impl.meta.json
--rw-r--r--   0        0        0     5382 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/click/_textwrap.data.json
--rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/click/_textwrap.meta.json
--rw-r--r--   0        0        0   180689 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/click/core.data.json
--rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/click/core.meta.json
--rw-r--r--   0        0        0    55966 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/click/decorators.data.json
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/click/decorators.meta.json
--rw-r--r--   0        0        0    27677 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/click/exceptions.data.json
--rw-r--r--   0        0        0     1683 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/click/exceptions.meta.json
--rw-r--r--   0        0        0    17583 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/click/formatting.data.json
--rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/click/formatting.meta.json
--rw-r--r--   0        0        0     7084 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/click/globals.data.json
--rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/click/globals.meta.json
--rw-r--r--   0        0        0    28715 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/click/parser.data.json
--rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/click/parser.meta.json
--rw-r--r--   0        0        0    33794 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/click/shell_completion.data.json
--rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/click/shell_completion.meta.json
--rw-r--r--   0        0        0    23327 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/click/termui.data.json
--rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/click/termui.meta.json
--rw-r--r--   0        0        0    81136 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/click/types.data.json
--rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/click/types.meta.json
--rw-r--r--   0        0        0    32015 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/click/utils.data.json
--rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/click/utils.meta.json
--rw-r--r--   0        0        0   408027 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/collections/__init__.data.json
--rw-r--r--   0        0        0     1698 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/collections/__init__.meta.json
--rw-r--r--   0        0        0     3770 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/collections/abc.data.json
--rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/collections/abc.meta.json
--rw-r--r--   0        0        0   129022 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/ctypes/__init__.data.json
--rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/ctypes/__init__.meta.json
--rw-r--r--   0        0        0     7477 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/email/__init__.data.json
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/email/__init__.meta.json
--rw-r--r--   0        0        0    12239 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/email/charset.data.json
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/email/charset.meta.json
--rw-r--r--   0        0        0     7288 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/email/contentmanager.data.json
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/email/contentmanager.meta.json
--rw-r--r--   0        0        0    25112 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/email/errors.data.json
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/email/errors.meta.json
--rw-r--r--   0        0        0     9193 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/email/header.data.json
--rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/email/header.meta.json
--rw-r--r--   0        0        0    79309 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/email/message.data.json
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/email/message.meta.json
--rw-r--r--   0        0        0    30896 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/email/policy.data.json
--rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/email/policy.meta.json
--rw-r--r--   0        0        0     6164 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/importlib/__init__.data.json
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/importlib/__init__.meta.json
--rw-r--r--   0        0        0    70618 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/importlib/abc.data.json
--rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/importlib/abc.meta.json
--rw-r--r--   0        0        0    64610 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/importlib/machinery.data.json
--rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/importlib/machinery.meta.json
--rw-r--r--   0        0        0    91158 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/importlib/metadata/__init__.data.json
--rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/importlib/metadata/__init__.meta.json
--rw-r--r--   0        0        0    11974 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/importlib/metadata/_meta.data.json
--rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/importlib/metadata/_meta.meta.json
--rw-r--r--   0        0        0   350782 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/os/__init__.data.json
--rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/os/__init__.meta.json
--rw-r--r--   0        0        0     4947 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/os/path.data.json
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/os/path.meta.json
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomcli/__init__.data.json
--rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomcli/__init__.meta.json
--rw-r--r--   0        0        0    12001 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomcli/toml.data.json
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomcli/toml.meta.json
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomcli/cli/__init__.data.json
--rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomcli/cli/__init__.meta.json
--rw-r--r--   0        0        0     4368 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomcli/cli/_util.data.json
--rw-r--r--   0        0        0     1596 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomcli/cli/_util.meta.json
--rw-r--r--   0        0        0     5006 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomcli/cli/get.data.json
--rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomcli/cli/get.meta.json
--rw-r--r--   0        0        0    26419 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomcli/cli/set.data.json
--rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomcli/cli/set.meta.json
--rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomli_w/__init__.data.json
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomli_w/__init__.meta.json
--rw-r--r--   0        0        0    30762 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomli_w/_writer.data.json
--rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomli_w/_writer.meta.json
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomlkit/__init__.data.json
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomlkit/__init__.meta.json
--rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomlkit/_compat.data.json
--rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomlkit/_compat.meta.json
--rw-r--r--   0        0        0     7831 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomlkit/_utils.data.json
--rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomlkit/_utils.meta.json
--rw-r--r--   0        0        0    18634 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomlkit/api.data.json
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomlkit/api.meta.json
--rw-r--r--   0        0        0    47564 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomlkit/container.data.json
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomlkit/container.meta.json
--rw-r--r--   0        0        0    32954 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomlkit/exceptions.data.json
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomlkit/exceptions.meta.json
--rw-r--r--   0        0        0   220449 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomlkit/items.data.json
--rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomlkit/items.meta.json
--rw-r--r--   0        0        0    33483 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomlkit/parser.data.json
--rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomlkit/parser.meta.json
--rw-r--r--   0        0        0    22675 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomlkit/source.data.json
--rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomlkit/source.meta.json
--rw-r--r--   0        0        0     7653 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomlkit/toml_char.data.json
--rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomlkit/toml_char.meta.json
--rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomlkit/toml_document.data.json
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/tomlkit/toml_document.meta.json
--rw-r--r--   0        0        0     4723 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/typer/__init__.data.json
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/typer/__init__.meta.json
--rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/typer/_compat_utils.data.json
--rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/typer/_compat_utils.meta.json
--rw-r--r--   0        0        0     7176 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/typer/_completion_click7.data.json
--rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/typer/_completion_click7.meta.json
--rw-r--r--   0        0        0    20998 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/typer/_completion_click8.data.json
--rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/typer/_completion_click8.meta.json
--rw-r--r--   0        0        0    11493 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/typer/_completion_shared.data.json
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/typer/_completion_shared.meta.json
--rw-r--r--   0        0        0    34961 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/typer/_typing.data.json
--rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/typer/_typing.meta.json
--rw-r--r--   0        0        0     4880 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/typer/colors.data.json
--rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/typer/colors.meta.json
--rw-r--r--   0        0        0     8933 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/typer/completion.data.json
--rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/typer/completion.meta.json
--rw-r--r--   0        0        0    47747 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/typer/core.data.json
--rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/typer/core.meta.json
--rw-r--r--   0        0        0    55896 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/typer/main.data.json
--rw-r--r--   0        0        0     2057 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/typer/main.meta.json
--rw-r--r--   0        0        0    68398 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/typer/models.data.json
--rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/typer/models.meta.json
--rw-r--r--   0        0        0    56992 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/typer/params.data.json
--rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/typer/params.meta.json
--rw-r--r--   0        0        0    36082 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/typer/rich_utils.data.json
--rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/typer/rich_utils.meta.json
--rw-r--r--   0        0        0    17477 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/typer/utils.data.json
--rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/typer/utils.meta.json
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/urllib/__init__.data.json
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/urllib/__init__.meta.json
--rw-r--r--   0        0        0   182183 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/urllib/parse.data.json
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 tomcli-0.1.1/.mypy_cache/3.11/urllib/parse.meta.json
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 tomcli-0.1.1/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 tomcli-0.1.1/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 tomcli-0.1.1/.pytest_cache/README.md
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 tomcli-0.1.1/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0     3658 2020-02-02 00:00:00.000000 tomcli-0.1.1/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 tomcli-0.1.1/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/102ae904ce423ecb
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/12dc023d4eeb0e37
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/132a3334bcb697d4
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/138cd2ffd9a72fa1
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/16cf683684086e42
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/17032b34c3539c33
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/182adab4e5a8e026
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/191bd3e667e65878
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/195fac077159fecb
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/1cae0246f47a51e6
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/1ed1e9bc14a8e947
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/21b095e72d064d0b
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/228428ef6c55f9b4
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/242872c45603caf
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/25f3447aeaf90609
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/26fd5f1a8357f894
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/2b63439cd5af3054
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/2b7341a8921547bd
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/2ff578dfeee119ca
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/33669fbc3402d0a1
--rw-r--r--   0        0        0     2427 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/343c17d86941be6d
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/346d839a0caccf20
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/34e1ab478d40a9f3
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/3622d24d03165106
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/3bd00a94f33fcfb6
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/3c9f99f371b068bd
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/3f58ceb8ff490785
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/4053dc61d6f25547
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/41414cb33223f426
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/4308237c7c08ba51
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/4553072f09555c43
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/46998819e6ff077f
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/47990969b0816c19
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/4888e119c62fc817
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/4a7642a70dda40d5
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/4cd0cccf6ffbd37f
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/4d0ebeb74dea6e4b
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/4dbd6c78c25046fa
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/4ee7b8cdcbae7088
--rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/50fbcc50cbc6963e
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/51d60f70e1c125ab
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/52052331ac998de4
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/53b770c79f3eb823
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/550a149458063685
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/558db8308279fc8
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/567b69da99e997a2
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/597c305794afb3f8
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/59e5ebb72bd3ba47
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/5c0560476bf0f9ad
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/60cd4b8318ff3584
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/657ba086a2498dbf
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/6746594f55461582
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/674c74015bfddf43
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/6786b37a5221b5ca
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/68c3bf3fc39850ae
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/69bb70c63199ed7e
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/6b2cd9174eb27a0b
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/6b3a3867f95ee3d2
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/6c2e1ccb7af019ae
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/6ca2f2fc9012834d
--rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/6e1805a0b2587263
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/6e75d02f45e0b6fb
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/6e8ccc9f8483820
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/6fe881ef0238e47f
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/72b1b7c696d63174
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/7504488c70d0af41
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/76586ca86e26121c
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/774d1d87720a5875
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/78d76edde2035610
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/7a8936c6cc6300fc
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/7c61d90fd1d2157e
--rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/7daa321bf9a53c19
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/868e7acfe2fb4ddd
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/8a402591edeaa7cd
--rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/8c07c91f8542951d
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/8cbb3cc218d2ac4e
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/8ee62ebec18533c6
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/8f65f16675aa2609
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/9077c3459649e893
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/9121b1d341614163
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/92cc94298f42a9ca
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/92dba4109cb7630e
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/92ef05225680b6d9
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/937b28c1e8bec5db
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/997ed1b7b1b436bc
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/99c02b984716f598
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/99d43425a9401b4
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/9a95a18da5948a17
--rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/9d5dbdd0a8f1e60
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/9fb39b3a808d7699
--rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/a27d76782310c1d1
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/a29416463f58d4c8
--rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/a443eb5443fdca85
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/a86f2775c1a8a107
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/a893c04545a27cb5
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/ac3bb96a02e8e6e
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/ae8098d6ad3ba72c
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/b0498287d2c842b7
--rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/b3930246cf024275
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/b5d7fd139b8e8a0e
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/b92653f4ad1ae939
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/bab378b835e02eca
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/bb5da1dd2b74eb4a
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/bbbc901adcc3cdce
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/bca2376011140193
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/c5e9cf82f769cc55
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/c95bdd44d51da69b
--rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/cf0c578ec805a96d
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/d16f80d852d45e0f
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/d3122b9270693438
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/d605b54ed8ac564b
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/db1c6b1a34a124cf
--rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/db3b51a62df336a
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/dc0a1dabe7469cc9
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/dc597330036fdb6b
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/dca3ff05fc9331c1
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/dccc2bf75292b03c
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/de5d7f1c9f277e6e
--rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/de7a47327060d771
--rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/defb66c7533f1af0
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/e0d6034af33a507f
--rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/e41759e40bb12348
--rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/e4f9058a88b51681
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/e86563f1db503e0a
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/e9947e79394d7105
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/e9a66483d5236f84
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/ebc4eaabfb6b1a87
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/ebc90afe0dc2f9c9
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/ee43000363d5572
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/ee5eab6a18e8f319
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/ef2b9c6d0e28e698
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/f03dc93d3317a16d
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/f14acfbd1d4b990e
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/f24f2f95e29bfcd4
--rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/f4fbc527411366a3
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/f7743eea7895cd9a
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/f7ab763b6cbfb8c
--rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/f91fb7119f181aad
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/fc383bcf580fd858
--rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 tomcli-0.1.1/.ruff_cache/content/fcc03fa280ebd898
--rwxr-xr-x   0        0        0      912 2020-02-02 00:00:00.000000 tomcli-0.1.1/contrib/fedoraify.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 tomcli-0.1.1/htmlcov/.gitignore
--rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 tomcli-0.1.1/htmlcov/coverage_html.js
--rw-r--r--   0        0        0     6246 2020-02-02 00:00:00.000000 tomcli-0.1.1/htmlcov/d_0cdc8f8d5ab5d777___init___py.html
--rw-r--r--   0        0        0    57283 2020-02-02 00:00:00.000000 tomcli-0.1.1/htmlcov/d_0cdc8f8d5ab5d777_toml_py.html
--rw-r--r--   0        0        0     5037 2020-02-02 00:00:00.000000 tomcli-0.1.1/htmlcov/d_1f8b6c189908f960___init___py.html
--rw-r--r--   0        0        0     8827 2020-02-02 00:00:00.000000 tomcli-0.1.1/htmlcov/d_1f8b6c189908f960__util_py.html
--rw-r--r--   0        0        0    19997 2020-02-02 00:00:00.000000 tomcli-0.1.1/htmlcov/d_1f8b6c189908f960_get_py.html
--rw-r--r--   0        0        0    34226 2020-02-02 00:00:00.000000 tomcli-0.1.1/htmlcov/d_1f8b6c189908f960_set_py.html
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 tomcli-0.1.1/htmlcov/favicon_32.png
--rw-r--r--   0        0        0     5421 2020-02-02 00:00:00.000000 tomcli-0.1.1/htmlcov/index.html
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 tomcli-0.1.1/htmlcov/keybd_closed.png
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 tomcli-0.1.1/htmlcov/keybd_open.png
--rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 tomcli-0.1.1/htmlcov/status.json
--rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 tomcli-0.1.1/htmlcov/style.css
--rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 tomcli-0.1.1/src/tomcli/__init__.py
--rw-r--r--   0        0        0     6585 2020-02-02 00:00:00.000000 tomcli-0.1.1/src/tomcli/toml.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 tomcli-0.1.1/src/tomcli/cli/__init__.py
--rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 tomcli-0.1.1/src/tomcli/cli/_util.py
--rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 tomcli-0.1.1/src/tomcli/cli/get.py
--rw-r--r--   0        0        0     8127 2020-02-02 00:00:00.000000 tomcli-0.1.1/src/tomcli/cli/set.py
--rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 tomcli-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 tomcli-0.1.1/tests/conftest.py
--rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 tomcli-0.1.1/tests/test_tomcli_get.py
--rw-r--r--   0        0        0     1992 2020-02-02 00:00:00.000000 tomcli-0.1.1/tests/test_tomcli_set.py
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 tomcli-0.1.1/tests/test_data/pyproject.toml
--rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 tomcli-0.1.1/tests/test_data/test1.toml
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 tomcli-0.1.1/.gitignore
--rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 tomcli-0.1.1/README.md
--rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 tomcli-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 tomcli-0.1.1/LICENSES/MIT.txt
--rw-r--r--   0        0        0     3240 2020-02-02 00:00:00.000000 tomcli-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 tomcli-0.1.2/CONTRIBUTING.md
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 tomcli-0.1.2/NEWS.md
+-rw-r--r--   0        0        0     9085 2020-02-02 00:00:00.000000 tomcli-0.1.2/noxfile.py
+-rw-r--r--   0        0        0      723 2020-02-02 00:00:00.000000 tomcli-0.1.2/ruff.toml
+-rw-r--r--   0        0        0     2502 2020-02-02 00:00:00.000000 tomcli-0.1.2/tomcli.spec
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 tomcli-0.1.2/.builds/nox-mockbuild-36.yml
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 tomcli-0.1.2/.builds/nox-mockbuild-epel9.yml
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 tomcli-0.1.2/.builds/nox-mockbuild.yml
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 tomcli-0.1.2/.builds/nox.yml
+-rw-r--r--   0        0        0      253 2020-02-02 00:00:00.000000 tomcli-0.1.2/.copr/Makefile
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/.gitignore
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/@plugins_snapshot.json
+-rw-r--r--   0        0        0     7860 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/__future__.data.json
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/__future__.meta.json
+-rw-r--r--   0        0        0   180407 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/_ast.data.json
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/_ast.meta.json
+-rw-r--r--   0        0        0    52439 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/_codecs.data.json
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/_codecs.meta.json
+-rw-r--r--   0        0        0    18266 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/_collections_abc.data.json
+-rw-r--r--   0        0        0     1637 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/_collections_abc.meta.json
+-rw-r--r--   0        0        0     3164 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/_ctypes.data.json
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/_ctypes.meta.json
+-rw-r--r--   0        0        0   171970 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/_decimal.data.json
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/_decimal.meta.json
+-rw-r--r--   0        0        0   113968 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/_operator.data.json
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/_operator.meta.json
+-rw-r--r--   0        0        0     6134 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/_random.data.json
+-rw-r--r--   0        0        0     1595 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/_random.meta.json
+-rw-r--r--   0        0        0    19742 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/_stat.data.json
+-rw-r--r--   0        0        0     1603 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/_stat.meta.json
+-rw-r--r--   0        0        0    23900 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/_thread.data.json
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/_thread.meta.json
+-rw-r--r--   0        0        0    13117 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/_warnings.data.json
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/_warnings.meta.json
+-rw-r--r--   0        0        0    27348 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/_weakref.data.json
+-rw-r--r--   0        0        0     1659 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/_weakref.meta.json
+-rw-r--r--   0        0        0    50468 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/_weakrefset.data.json
+-rw-r--r--   0        0        0     1665 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/_weakrefset.meta.json
+-rw-r--r--   0        0        0    23375 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/abc.data.json
+-rw-r--r--   0        0        0     1625 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/abc.meta.json
+-rw-r--r--   0        0        0    60715 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/array.data.json
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/array.meta.json
+-rw-r--r--   0        0        0  1130451 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/builtins.data.json
+-rw-r--r--   0        0        0     1762 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/builtins.meta.json
+-rw-r--r--   0        0        0   123356 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/codecs.data.json
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/codecs.meta.json
+-rw-r--r--   0        0        0   109243 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/contextlib.data.json
+-rw-r--r--   0        0        0     1671 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/contextlib.meta.json
+-rw-r--r--   0        0        0     5448 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/copy.data.json
+-rw-r--r--   0        0        0     1564 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/copy.meta.json
+-rw-r--r--   0        0        0    57784 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/dataclasses.data.json
+-rw-r--r--   0        0        0     1676 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/dataclasses.meta.json
+-rw-r--r--   0        0        0   142247 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/datetime.data.json
+-rw-r--r--   0        0        0     1636 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/datetime.meta.json
+-rw-r--r--   0        0        0     4950 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/decimal.data.json
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/decimal.meta.json
+-rw-r--r--   0        0        0    58330 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/difflib.data.json
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/difflib.meta.json
+-rw-r--r--   0        0        0    62945 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/dis.data.json
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/dis.meta.json
+-rw-r--r--   0        0        0    90162 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/enum.data.json
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/enum.meta.json
+-rw-r--r--   0        0        0    27315 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/errno.data.json
+-rw-r--r--   0        0        0     1601 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/errno.meta.json
+-rw-r--r--   0        0        0    88816 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/fractions.data.json
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/fractions.meta.json
+-rw-r--r--   0        0        0   132106 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/functools.data.json
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/functools.meta.json
+-rw-r--r--   0        0        0    22427 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/genericpath.data.json
+-rw-r--r--   0        0        0     1651 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/genericpath.meta.json
+-rw-r--r--   0        0        0     3778 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/getpass.data.json
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/getpass.meta.json
+-rw-r--r--   0        0        0    46229 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/gettext.data.json
+-rw-r--r--   0        0        0     1654 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/gettext.meta.json
+-rw-r--r--   0        0        0     9543 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/glob.data.json
+-rw-r--r--   0        0        0     1614 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/glob.meta.json
+-rw-r--r--   0        0        0   330927 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/inspect.data.json
+-rw-r--r--   0        0        0     1701 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/inspect.meta.json
+-rw-r--r--   0        0        0    85376 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/io.data.json
+-rw-r--r--   0        0        0     1724 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/io.meta.json
+-rw-r--r--   0        0        0   266348 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/itertools.data.json
+-rw-r--r--   0        0        0     1662 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/itertools.meta.json
+-rw-r--r--   0        0        0    52550 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/math.data.json
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/math.meta.json
+-rw-r--r--   0        0        0    28806 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/mmap.data.json
+-rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/mmap.meta.json
+-rw-r--r--   0        0        0     1545 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/msvcrt.data.json
+-rw-r--r--   0        0        0     1604 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/msvcrt.meta.json
+-rw-r--r--   0        0        0    79021 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/numbers.data.json
+-rw-r--r--   0        0        0     1570 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/numbers.meta.json
+-rw-r--r--   0        0        0     6133 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/opcode.data.json
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/opcode.meta.json
+-rw-r--r--   0        0        0    49237 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/operator.data.json
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/operator.meta.json
+-rw-r--r--   0        0        0    87527 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/pathlib.data.json
+-rw-r--r--   0        0        0     1733 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/pathlib.meta.json
+-rw-r--r--   0        0        0    44432 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/pickle.data.json
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/pickle.meta.json
+-rw-r--r--   0        0        0    75236 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/posixpath.data.json
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/posixpath.meta.json
+-rw-r--r--   0        0        0    40046 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/random.data.json
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/random.meta.json
+-rw-r--r--   0        0        0   167584 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/re.data.json
+-rw-r--r--   0        0        0     1752 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/re.meta.json
+-rw-r--r--   0        0        0    16535 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/shlex.data.json
+-rw-r--r--   0        0        0     1641 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/shlex.meta.json
+-rw-r--r--   0        0        0    71151 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/shutil.data.json
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/shutil.meta.json
+-rw-r--r--   0        0        0    14412 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/sre_compile.data.json
+-rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/sre_compile.meta.json
+-rw-r--r--   0        0        0    28519 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/sre_constants.data.json
+-rw-r--r--   0        0        0     1635 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/sre_constants.meta.json
+-rw-r--r--   0        0        0    49780 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/sre_parse.data.json
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/sre_parse.meta.json
+-rw-r--r--   0        0        0     6569 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/stat.data.json
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/stat.meta.json
+-rw-r--r--   0        0        0    27787 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/string.data.json
+-rw-r--r--   0        0        0     1663 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/string.meta.json
+-rw-r--r--   0        0        0   162203 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/subprocess.data.json
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/subprocess.meta.json
+-rw-r--r--   0        0        0   148693 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/sys.data.json
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/sys.meta.json
+-rw-r--r--   0        0        0   140364 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/tempfile.data.json
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/tempfile.meta.json
+-rw-r--r--   0        0        0    49134 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/termios.data.json
+-rw-r--r--   0        0        0     1622 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/termios.meta.json
+-rw-r--r--   0        0        0    19592 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/textwrap.data.json
+-rw-r--r--   0        0        0     1605 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/textwrap.meta.json
+-rw-r--r--   0        0        0    64754 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/threading.data.json
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/threading.meta.json
+-rw-r--r--   0        0        0    43644 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/time.data.json
+-rw-r--r--   0        0        0     1616 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/time.meta.json
+-rw-r--r--   0        0        0     5279 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/tomllib.data.json
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/tomllib.meta.json
+-rw-r--r--   0        0        0    57057 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/traceback.data.json
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/traceback.meta.json
+-rw-r--r--   0        0        0     4865 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/tty.data.json
+-rw-r--r--   0        0        0     1597 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/tty.meta.json
+-rw-r--r--   0        0        0   239671 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/types.data.json
+-rw-r--r--   0        0        0     1689 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/types.meta.json
+-rw-r--r--   0        0        0   432273 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/typing.data.json
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/typing.meta.json
+-rw-r--r--   0        0        0    57884 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/typing_extensions.data.json
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/typing_extensions.meta.json
+-rw-r--r--   0        0        0    33625 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/uuid.data.json
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/uuid.meta.json
+-rw-r--r--   0        0        0    23828 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/warnings.data.json
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/warnings.meta.json
+-rw-r--r--   0        0        0   142967 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/weakref.data.json
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/weakref.meta.json
+-rw-r--r--   0        0        0    24308 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/webbrowser.data.json
+-rw-r--r--   0        0        0     1634 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/webbrowser.meta.json
+-rw-r--r--   0        0        0    89093 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/_typeshed/__init__.data.json
+-rw-r--r--   0        0        0     1740 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/_typeshed/__init__.meta.json
+-rw-r--r--   0        0        0     7789 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/click/__init__.data.json
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/click/__init__.meta.json
+-rw-r--r--   0        0        0    47214 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/click/_compat.data.json
+-rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/click/_compat.meta.json
+-rw-r--r--   0        0        0    44790 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/click/_termui_impl.data.json
+-rw-r--r--   0        0        0     2059 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/click/_termui_impl.meta.json
+-rw-r--r--   0        0        0     5382 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/click/_textwrap.data.json
+-rw-r--r--   0        0        0     1639 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/click/_textwrap.meta.json
+-rw-r--r--   0        0        0   180689 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/click/core.data.json
+-rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/click/core.meta.json
+-rw-r--r--   0        0        0    55966 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/click/decorators.data.json
+-rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/click/decorators.meta.json
+-rw-r--r--   0        0        0    27677 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/click/exceptions.data.json
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/click/exceptions.meta.json
+-rw-r--r--   0        0        0    17583 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/click/formatting.data.json
+-rw-r--r--   0        0        0     1768 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/click/formatting.meta.json
+-rw-r--r--   0        0        0     7084 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/click/globals.data.json
+-rw-r--r--   0        0        0     1619 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/click/globals.meta.json
+-rw-r--r--   0        0        0    28715 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/click/parser.data.json
+-rw-r--r--   0        0        0     1778 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/click/parser.meta.json
+-rw-r--r--   0        0        0    33794 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/click/shell_completion.data.json
+-rw-r--r--   0        0        0     1828 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/click/shell_completion.meta.json
+-rw-r--r--   0        0        0    23327 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/click/termui.data.json
+-rw-r--r--   0        0        0     1926 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/click/termui.meta.json
+-rw-r--r--   0        0        0    81136 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/click/types.data.json
+-rw-r--r--   0        0        0     1945 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/click/types.meta.json
+-rw-r--r--   0        0        0    32015 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/click/utils.data.json
+-rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/click/utils.meta.json
+-rw-r--r--   0        0        0   408027 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/collections/__init__.data.json
+-rw-r--r--   0        0        0     1751 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/collections/__init__.meta.json
+-rw-r--r--   0        0        0     3770 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/collections/abc.data.json
+-rw-r--r--   0        0        0     1609 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/collections/abc.meta.json
+-rw-r--r--   0        0        0   129022 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/ctypes/__init__.data.json
+-rw-r--r--   0        0        0     1717 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/ctypes/__init__.meta.json
+-rw-r--r--   0        0        0     7477 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/email/__init__.data.json
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/email/__init__.meta.json
+-rw-r--r--   0        0        0    12239 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/email/charset.data.json
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/email/charset.meta.json
+-rw-r--r--   0        0        0     7288 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/email/contentmanager.data.json
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/email/contentmanager.meta.json
+-rw-r--r--   0        0        0    25112 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/email/errors.data.json
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/email/errors.meta.json
+-rw-r--r--   0        0        0     9193 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/email/header.data.json
+-rw-r--r--   0        0        0     1623 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/email/header.meta.json
+-rw-r--r--   0        0        0    79309 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/email/message.data.json
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/email/message.meta.json
+-rw-r--r--   0        0        0    30896 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/email/policy.data.json
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/email/policy.meta.json
+-rw-r--r--   0        0        0     6164 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/importlib/__init__.data.json
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/importlib/__init__.meta.json
+-rw-r--r--   0        0        0    70618 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/importlib/abc.data.json
+-rw-r--r--   0        0        0     1784 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/importlib/abc.meta.json
+-rw-r--r--   0        0        0    64610 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/importlib/machinery.data.json
+-rw-r--r--   0        0        0     1773 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/importlib/machinery.meta.json
+-rw-r--r--   0        0        0    91158 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/importlib/metadata/__init__.data.json
+-rw-r--r--   0        0        0     1782 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/importlib/metadata/__init__.meta.json
+-rw-r--r--   0        0        0    11974 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/importlib/metadata/_meta.data.json
+-rw-r--r--   0        0        0     1626 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/importlib/metadata/_meta.meta.json
+-rw-r--r--   0        0        0   350782 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/os/__init__.data.json
+-rw-r--r--   0        0        0     1776 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/os/__init__.meta.json
+-rw-r--r--   0        0        0     4947 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/os/path.data.json
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/os/path.meta.json
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/tomcli/__init__.data.json
+-rw-r--r--   0        0        0     1474 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/tomcli/__init__.meta.json
+-rw-r--r--   0        0        0    12001 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/tomcli/toml.data.json
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/tomcli/toml.meta.json
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/tomcli/cli/__init__.data.json
+-rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/tomcli/cli/__init__.meta.json
+-rw-r--r--   0        0        0     4368 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/tomcli/cli/_util.data.json
+-rw-r--r--   0        0        0     1586 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/tomcli/cli/_util.meta.json
+-rw-r--r--   0        0        0     5006 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/tomcli/cli/get.data.json
+-rw-r--r--   0        0        0     1793 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/tomcli/cli/get.meta.json
+-rw-r--r--   0        0        0    26419 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/tomcli/cli/set.data.json
+-rw-r--r--   0        0        0     1903 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/tomcli/cli/set.meta.json
+-rw-r--r--   0        0        0     2495 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/tomli_w/__init__.data.json
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/tomli_w/__init__.meta.json
+-rw-r--r--   0        0        0    30762 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/tomli_w/_writer.data.json
+-rw-r--r--   0        0        0     1792 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/tomli_w/_writer.meta.json
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/tomlkit/__init__.data.json
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/tomlkit/__init__.meta.json
+-rw-r--r--   0        0        0     2726 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/tomlkit/_compat.data.json
+-rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/tomlkit/_compat.meta.json
+-rw-r--r--   0        0        0     7831 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/tomlkit/_utils.data.json
+-rw-r--r--   0        0        0     1781 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/tomlkit/_utils.meta.json
+-rw-r--r--   0        0        0    18634 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/tomlkit/api.data.json
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/tomlkit/api.meta.json
+-rw-r--r--   0        0        0    47564 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/tomlkit/container.data.json
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/tomlkit/container.meta.json
+-rw-r--r--   0        0        0    32954 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/tomlkit/exceptions.data.json
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/tomlkit/exceptions.meta.json
+-rw-r--r--   0        0        0   220449 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/tomlkit/items.data.json
+-rw-r--r--   0        0        0     1907 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/tomlkit/items.meta.json
+-rw-r--r--   0        0        0    33483 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/tomlkit/parser.data.json
+-rw-r--r--   0        0        0     1931 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/tomlkit/parser.meta.json
+-rw-r--r--   0        0        0    22675 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/tomlkit/source.data.json
+-rw-r--r--   0        0        0     1680 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/tomlkit/source.meta.json
+-rw-r--r--   0        0        0     7653 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/tomlkit/toml_char.data.json
+-rw-r--r--   0        0        0     1582 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/tomlkit/toml_char.meta.json
+-rw-r--r--   0        0        0     2356 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/tomlkit/toml_document.data.json
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/tomlkit/toml_document.meta.json
+-rw-r--r--   0        0        0     4723 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/typer/__init__.data.json
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/typer/__init__.meta.json
+-rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/typer/_compat_utils.data.json
+-rw-r--r--   0        0        0     1678 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/typer/_compat_utils.meta.json
+-rw-r--r--   0        0        0     7176 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/typer/_completion_click7.data.json
+-rw-r--r--   0        0        0     1887 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/typer/_completion_click7.meta.json
+-rw-r--r--   0        0        0    20998 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/typer/_completion_click8.data.json
+-rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/typer/_completion_click8.meta.json
+-rw-r--r--   0        0        0    11493 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/typer/_completion_shared.data.json
+-rw-r--r--   0        0        0     1870 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/typer/_completion_shared.meta.json
+-rw-r--r--   0        0        0    34961 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/typer/_typing.data.json
+-rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/typer/_typing.meta.json
+-rw-r--r--   0        0        0     4880 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/typer/colors.data.json
+-rw-r--r--   0        0        0     1557 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/typer/colors.meta.json
+-rw-r--r--   0        0        0     8933 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/typer/completion.data.json
+-rw-r--r--   0        0        0     2051 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/typer/completion.meta.json
+-rw-r--r--   0        0        0    47747 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/typer/core.data.json
+-rw-r--r--   0        0        0     2102 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/typer/core.meta.json
+-rw-r--r--   0        0        0    55896 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/typer/main.data.json
+-rw-r--r--   0        0        0     2095 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/typer/main.meta.json
+-rw-r--r--   0        0        0    68398 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/typer/models.data.json
+-rw-r--r--   0        0        0     1742 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/typer/models.meta.json
+-rw-r--r--   0        0        0    56992 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/typer/params.data.json
+-rw-r--r--   0        0        0     1657 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/typer/params.meta.json
+-rw-r--r--   0        0        0    36082 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/typer/rich_utils.data.json
+-rw-r--r--   0        0        0     2098 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/typer/rich_utils.meta.json
+-rw-r--r--   0        0        0    17477 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/typer/utils.data.json
+-rw-r--r--   0        0        0     1737 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/typer/utils.meta.json
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/urllib/__init__.data.json
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/urllib/__init__.meta.json
+-rw-r--r--   0        0        0   175351 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/urllib/parse.data.json
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 tomcli-0.1.2/.mypy_cache/3.11/urllib/parse.meta.json
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 tomcli-0.1.2/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 tomcli-0.1.2/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 tomcli-0.1.2/.pytest_cache/README.md
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 tomcli-0.1.2/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0     3930 2020-02-02 00:00:00.000000 tomcli-0.1.2/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 tomcli-0.1.2/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/102ae904ce423ecb
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/122ee1fc81581912
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/12dc023d4eeb0e37
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/132a3334bcb697d4
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/138cd2ffd9a72fa1
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/16cf683684086e42
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/17032b34c3539c33
+-rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/182adab4e5a8e026
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/191bd3e667e65878
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/192747c3e751c52b
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/195fac077159fecb
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/197f44b46efda2dd
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/1c02530f140d338
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/1cae0246f47a51e6
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/1ed1e9bc14a8e947
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/21b095e72d064d0b
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/228428ef6c55f9b4
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/242872c45603caf
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/24aa5788af5686ac
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/25f3447aeaf90609
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/26541aae610902df
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/26fd5f1a8357f894
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/2b63439cd5af3054
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/2b7341a8921547bd
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/2ff578dfeee119ca
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/33669fbc3402d0a1
+-rw-r--r--   0        0        0     2427 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/343c17d86941be6d
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/3445408793eb7659
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/346d839a0caccf20
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/34e1ab478d40a9f3
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/3622d24d03165106
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/3bd00a94f33fcfb6
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/3c9f99f371b068bd
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/3f58ceb8ff490785
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/4053dc61d6f25547
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/41414cb33223f426
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/4308237c7c08ba51
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/4553072f09555c43
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/46998819e6ff077f
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/47990969b0816c19
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/4888e119c62fc817
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/48ce03c3d88dc7f2
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/4a7642a70dda40d5
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/4cd0cccf6ffbd37f
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/4d0ebeb74dea6e4b
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/4dbd6c78c25046fa
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/4ee7b8cdcbae7088
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/50fbcc50cbc6963e
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/51d60f70e1c125ab
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/52052331ac998de4
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/53b770c79f3eb823
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/547484e47a5bcf4f
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/550a149458063685
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/558db8308279fc8
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/56105254aa1f3365
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/567b69da99e997a2
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/597c305794afb3f8
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/59e5ebb72bd3ba47
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/5c0560476bf0f9ad
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/60cd4b8318ff3584
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/657ba086a2498dbf
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/6746594f55461582
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/674c74015bfddf43
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/6786b37a5221b5ca
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/68c3bf3fc39850ae
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/69bb70c63199ed7e
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/6b2cd9174eb27a0b
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/6b3a3867f95ee3d2
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/6c2e1ccb7af019ae
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/6ca2f2fc9012834d
+-rw-r--r--   0        0        0      281 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/6e1805a0b2587263
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/6e75d02f45e0b6fb
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/6e8ccc9f8483820
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/6fe881ef0238e47f
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/72b1b7c696d63174
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/7504488c70d0af41
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/76586ca86e26121c
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/774d1d87720a5875
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/78d76edde2035610
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/7a8936c6cc6300fc
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/7c61d90fd1d2157e
+-rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/7daa321bf9a53c19
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/7e9d830e6d834048
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/85899bca0851049b
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/868e7acfe2fb4ddd
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/8a402591edeaa7cd
+-rw-r--r--   0        0        0      293 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/8c07c91f8542951d
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/8cbb3cc218d2ac4e
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/8ee62ebec18533c6
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/8f65f16675aa2609
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/8f731058df9bc427
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/9077c3459649e893
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/9121b1d341614163
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/92cc94298f42a9ca
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/92dba4109cb7630e
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/92ef05225680b6d9
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/937b28c1e8bec5db
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/94b5413d0944b661
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/9672ea10694796b
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/997ed1b7b1b436bc
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/99c02b984716f598
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/99d43425a9401b4
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/9a95a18da5948a17
+-rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/9d5dbdd0a8f1e60
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/9fb39b3a808d7699
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/a272f240a36e1fb3
+-rw-r--r--   0        0        0      959 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/a27d76782310c1d1
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/a29416463f58d4c8
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/a443eb5443fdca85
+-rw-r--r--   0        0        0      211 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/a54531389912a2fe
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/a86f2775c1a8a107
+-rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/a893c04545a27cb5
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/ac3bb96a02e8e6e
+-rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/ae8098d6ad3ba72c
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/b0498287d2c842b7
+-rw-r--r--   0        0        0      915 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/b3930246cf024275
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/b5d7fd139b8e8a0e
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/b92653f4ad1ae939
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/bab378b835e02eca
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/bb5da1dd2b74eb4a
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/bbbc901adcc3cdce
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/bca2376011140193
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/c5e9cf82f769cc55
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/c95bdd44d51da69b
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/cd2ce9836068d44c
+-rw-r--r--   0        0        0     1195 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/cf0c578ec805a96d
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/d16f80d852d45e0f
+-rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/d3122b9270693438
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/d37c3fd0c1ba2ef9
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/d3df8ba475437184
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/d605b54ed8ac564b
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/db1c6b1a34a124cf
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/db3b51a62df336a
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/dc0a1dabe7469cc9
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/dc597330036fdb6b
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/dca3ff05fc9331c1
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/dccc2bf75292b03c
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/de5d7f1c9f277e6e
+-rw-r--r--   0        0        0      315 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/de7a47327060d771
+-rw-r--r--   0        0        0      612 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/defb66c7533f1af0
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/e0d6034af33a507f
+-rw-r--r--   0        0        0       16 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/e41759e40bb12348
+-rw-r--r--   0        0        0      258 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/e4f9058a88b51681
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/e86563f1db503e0a
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/e9947e79394d7105
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/e9a66483d5236f84
+-rw-r--r--   0        0        0      768 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/ebbce3e5bf8a9484
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/ebc4eaabfb6b1a87
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/ebc90afe0dc2f9c9
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/ee43000363d5572
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/ee5eab6a18e8f319
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/ef2b9c6d0e28e698
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/f03dc93d3317a16d
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/f14acfbd1d4b990e
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/f24f2f95e29bfcd4
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/f251486086601a09
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/f27310c1e68a17a0
+-rw-r--r--   0        0        0      400 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/f4fbc527411366a3
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/f65719427aac5229
+-rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/f7743eea7895cd9a
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/f7ab763b6cbfb8c
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/f7e78f9b3172429e
+-rw-r--r--   0        0        0      636 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/f91fb7119f181aad
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/fc383bcf580fd858
+-rw-r--r--   0        0        0     2072 2020-02-02 00:00:00.000000 tomcli-0.1.2/.ruff_cache/content/fcc03fa280ebd898
+-rwxr-xr-x   0        0        0      912 2020-02-02 00:00:00.000000 tomcli-0.1.2/contrib/fedoraify.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 tomcli-0.1.2/htmlcov/.gitignore
+-rw-r--r--   0        0        0    21359 2020-02-02 00:00:00.000000 tomcli-0.1.2/htmlcov/coverage_html.js
+-rw-r--r--   0        0        0     6246 2020-02-02 00:00:00.000000 tomcli-0.1.2/htmlcov/d_0cdc8f8d5ab5d777___init___py.html
+-rw-r--r--   0        0        0    57283 2020-02-02 00:00:00.000000 tomcli-0.1.2/htmlcov/d_0cdc8f8d5ab5d777_toml_py.html
+-rw-r--r--   0        0        0     5037 2020-02-02 00:00:00.000000 tomcli-0.1.2/htmlcov/d_1f8b6c189908f960___init___py.html
+-rw-r--r--   0        0        0     8827 2020-02-02 00:00:00.000000 tomcli-0.1.2/htmlcov/d_1f8b6c189908f960__util_py.html
+-rw-r--r--   0        0        0    19997 2020-02-02 00:00:00.000000 tomcli-0.1.2/htmlcov/d_1f8b6c189908f960_get_py.html
+-rw-r--r--   0        0        0    34226 2020-02-02 00:00:00.000000 tomcli-0.1.2/htmlcov/d_1f8b6c189908f960_set_py.html
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 tomcli-0.1.2/htmlcov/favicon_32.png
+-rw-r--r--   0        0        0     5421 2020-02-02 00:00:00.000000 tomcli-0.1.2/htmlcov/index.html
+-rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 tomcli-0.1.2/htmlcov/keybd_closed.png
+-rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 tomcli-0.1.2/htmlcov/keybd_open.png
+-rw-r--r--   0        0        0     1322 2020-02-02 00:00:00.000000 tomcli-0.1.2/htmlcov/status.json
+-rw-r--r--   0        0        0    12387 2020-02-02 00:00:00.000000 tomcli-0.1.2/htmlcov/style.css
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 tomcli-0.1.2/src/tomcli/__init__.py
+-rw-r--r--   0        0        0     6585 2020-02-02 00:00:00.000000 tomcli-0.1.2/src/tomcli/toml.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 tomcli-0.1.2/src/tomcli/cli/__init__.py
+-rw-r--r--   0        0        0      468 2020-02-02 00:00:00.000000 tomcli-0.1.2/src/tomcli/cli/_util.py
+-rw-r--r--   0        0        0     1544 2020-02-02 00:00:00.000000 tomcli-0.1.2/src/tomcli/cli/get.py
+-rw-r--r--   0        0        0     8125 2020-02-02 00:00:00.000000 tomcli-0.1.2/src/tomcli/cli/set.py
+-rw-r--r--   0        0        0      117 2020-02-02 00:00:00.000000 tomcli-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0      602 2020-02-02 00:00:00.000000 tomcli-0.1.2/tests/conftest.py
+-rw-r--r--   0        0        0     1688 2020-02-02 00:00:00.000000 tomcli-0.1.2/tests/test_tomcli_get.py
+-rw-r--r--   0        0        0     2625 2020-02-02 00:00:00.000000 tomcli-0.1.2/tests/test_tomcli_set.py
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 tomcli-0.1.2/tests/test_data/pyproject.toml
+-rw-r--r--   0        0        0      123 2020-02-02 00:00:00.000000 tomcli-0.1.2/tests/test_data/test1.toml
+-rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 tomcli-0.1.2/.gitignore
+-rw-r--r--   0        0        0     1350 2020-02-02 00:00:00.000000 tomcli-0.1.2/README.md
+-rw-r--r--   0        0        0     1731 2020-02-02 00:00:00.000000 tomcli-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 tomcli-0.1.2/LICENSES/MIT.txt
+-rw-r--r--   0        0        0     3240 2020-02-02 00:00:00.000000 tomcli-0.1.2/PKG-INFO
```

### Comparing `tomcli-0.1.1/CONTRIBUTING.md` & `tomcli-0.1.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/noxfile.py` & `tomcli-0.1.2/noxfile.py`

 * *Files 2% similar despite different names*

```diff
@@ -201,22 +201,25 @@
 @nox.session
 def publish(session: nox.Session):
     # Setup
     ensure_clean(session)
     install(session, "hatch")
     session.run("hatch", "publish", *session.posargs)
 
-    # Copr build
-    copr_release.func(session)
-
     # Push to git
-    if session.interactive and input("Push to Sourcehut (Y/n)").lower() != "n":
+    if (
+        not session.interactive
+        or input("Push to Sourcehut and copr build (Y/n)").lower() != "n"
+    ):
         git(session, "push", "--follow-tags")
         srht_artifacts.func(session)
 
+        # Copr build
+        copr_release.func(session)
+
     # Post-release bump
     session.run("hatch", "version", "post")
     git(session, "add", f"src/{PROJECT}/__init__.py")
     git(session, "commit", "-S", "-m", "Post release version bump")
 
 
 @nox.session
```

### Comparing `tomcli-0.1.1/ruff.toml` & `tomcli-0.1.2/ruff.toml`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/tomcli.spec` & `tomcli-0.1.2/tomcli.spec`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # This specfile is licensed under:
 #
 # Copyright (C) 2023 Maxwell G <maxwell@gtmx.me>
 # SPDX-License-Identifier: MIT
 # License text: https://spdx.org/licenses/MIT.html
 
 Name:           tomcli
-Version:        0.1.1
+Version:        0.1.2
 Release:        1%{?dist}
 Summary:        CLI for working with TOML files. Pronounced "tom clee."
 
 License:        MIT
 URL:            https://sr.ht/~gotmax23/tomcli
 %global furl    https://git.sr.ht/~gotmax23/tomcli
 Source0:        %{furl}/refs/download/v%{version}/tomcli-%{version}.tar.gz
@@ -32,15 +32,15 @@
 
 
 %prep
 %autosetup -p1
 
 
 %generate_buildrequires
-%pyproject_buildrequires -x all,tomlkit,tomli,test
+%pyproject_buildrequires -x all,tomlkit,tomli,test %{?el9:-w}
 
 
 %build
 %pyproject_wheel
 
 
 %install
@@ -79,14 +79,17 @@
 %{_bindir}/tomcli*
 %{bash_completions_dir}/tomcli*
 %{fish_completions_dir}/tomcli*.fish
 %{zsh_completions_dir}/_tomcli*
 
 
 %changelog
+* Sat May 20 2023 Maxwell G <maxwell@gtmx.me> - 0.1.2-1
+- Release 0.1.2.
+
 * Wed May 03 2023 Maxwell G <maxwell@gtmx.me> - 0.1.1-1
 - Release 0.1.1.
 
 * Fri Apr 14 2023 Maxwell G <maxwell@gtmx.me> - 0.1.0-1
 - Release 0.1.0.
 
 * Thu Apr 13 2023 Maxwell G <maxwell@gtmx.me> - 0.0.0-1
```

### Comparing `tomcli-0.1.1/.builds/nox-mockbuild-36.yml` & `tomcli-0.1.2/.builds/nox-mockbuild-36.yml`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.builds/nox-mockbuild.yml` & `tomcli-0.1.2/.builds/nox-mockbuild.yml`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.builds/nox.yml` & `tomcli-0.1.2/.builds/nox.yml`

 * *Files 14% similar despite different names*

```diff
@@ -20,7 +20,10 @@
       pipx install nox
   - copr_webhook: |
       cd tomcli
       nox -e copr_webhook -- ~/.copr-dev-hook -b origin/main --skip-if-missing
   - nox-test: |
       cd tomcli
       nox -v -e test
+  - nox-lint: |
+      cd tomcli
+      nox -v -e lint
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/__future__.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/__future__.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/__future__.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/__future__.meta.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'data_mtime'": '1683843440', "'mtime'": '1684623296', "'version_id'": "'1.3.0'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843440,
     "dep_lines": [
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
@@ -18,15 +18,15 @@
         "abc",
         "typing"
     ],
     "hash": "a88c160e68dac375c28ae94a628281401fde2632f1c1e7ac50ac017699204245",
     "id": "__future__",
     "ignore_all": true,
     "interface_hash": "3192f5d3ead66040ac58e4c62fafd7eebab0d4f98c6c77abb0590e1f06299032",
-    "mtime": 1683082840,
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -64,9 +64,9 @@
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
     "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/__future__.pyi",
     "plugin_data": null,
     "size": 915,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/_ast.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/_ast.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/_ast.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/itertools.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.701851851851852%*

 * *Differences: {"'data_mtime'": '1683843440',*

 * * "'dep_lines'": '{insert: [(1, 1), (3, 4), (4, 7)], delete: [0]}',*

 * * "'dep_prios'": '{insert: [(0, 5), (2, 5)]}',*

 * * "'dependencies'": "{insert: [(0, 'collections.abc'), (4, 'types')]}",*

 * * "'hash'": "'8d452d6d11a70ac8cf92f7f8ca2f0ec391f06ffd520b0a5e9c6083b3efe75b5d'",*

 * * "'id'": "'itertools'",*

 * * "'interface_hash'": "'f44c52f578278b7de5867c5634921ea0a2a1c43a005a6874f20464d46cd5ebd3'",*

 * * "'mtime'": '1684623296',*

 * * "'path'": "'/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/. […]*

```diff
@@ -1,38 +1,44 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843440,
     "dep_lines": [
-        1,
         2,
+        1,
         3,
+        4,
+        7,
         1,
         1,
         1
     ],
     "dep_prios": [
+        5,
         10,
         5,
         5,
         5,
+        5,
         30,
         30
     ],
     "dependencies": [
+        "collections.abc",
         "sys",
         "typing",
         "typing_extensions",
+        "types",
         "builtins",
         "_typeshed",
         "abc"
     ],
-    "hash": "189ca9e5f979d2fafddf0fde549a04c4da5840422b279c427ac3b84df670b646",
-    "id": "_ast",
+    "hash": "8d452d6d11a70ac8cf92f7f8ca2f0ec391f06ffd520b0a5e9c6083b3efe75b5d",
+    "id": "itertools",
     "ignore_all": true,
-    "interface_hash": "a313ff97b5329396c2ba6b232b465b36bc665df2453493f09065b6b911d9c1d4",
-    "mtime": 1683082840,
+    "interface_hash": "f44c52f578278b7de5867c5634921ea0a2a1c43a005a6874f20464d46cd5ebd3",
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -66,13 +72,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/_ast.pyi",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/itertools.pyi",
     "plugin_data": null,
-    "size": 14752,
+    "size": 10908,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/_codecs.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/_codecs.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/_codecs.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/_random.meta.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6632478632478632%*

 * *Differences: {"'data_mtime'": '1683843440',*

 * * "'dep_lines'": '{delete: [7, 6, 5, 4, 3, 2, 1, 0]}',*

 * * "'dep_prios'": '{delete: [9, 8, 7, 4, 3, 2, 1, 0]}',*

 * * "'dependencies'": "{insert: [(3, 'typing')], delete: [11, 10, 9, 8, 4, 3, 2, 1, 0]}",*

 * * "'hash'": "'fdcf346a4f5cf1e59ed16298d1a44114f183d1641e67553a52691ba2bd17c788'",*

 * * "'id'": "'_random'",*

 * * "'interface_hash'": "'d23b07d1261fda7351f064e4c6f5f3814028e6dd5f7a0c9481f754b58f051b14'",*

 * * "'mtime'": '1684623296',*

 * * "'path'": "'/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev […]*

```diff
@@ -1,56 +1,32 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843440,
     "dep_lines": [
-        4,
-        1,
-        2,
-        3,
-        5,
-        6,
-        1,
-        1,
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
-        10,
-        10,
-        5,
         5,
-        5,
-        5,
-        30,
-        30,
-        30,
         30,
         30
     ],
     "dependencies": [
-        "collections.abc",
-        "codecs",
-        "sys",
-        "_typeshed",
-        "typing",
         "typing_extensions",
         "builtins",
         "abc",
-        "array",
-        "ctypes",
-        "mmap",
-        "pickle"
+        "typing"
     ],
-    "hash": "70e3defc1875bd08c24cbe869d9c14280401dc8b591637db091aad6a71684e1d",
-    "id": "_codecs",
+    "hash": "fdcf346a4f5cf1e59ed16298d1a44114f183d1641e67553a52691ba2bd17c788",
+    "id": "_random",
     "ignore_all": true,
-    "interface_hash": "9f0ae4ebfc6b4ad5b744bba8fd125716016d5c00b34dfc96e52aceb26dcfe0c0",
-    "mtime": 1683082840,
+    "interface_hash": "d23b07d1261fda7351f064e4c6f5f3814028e6dd5f7a0c9481f754b58f051b14",
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -84,13 +60,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/_codecs.pyi",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/_random.pyi",
     "plugin_data": null,
-    "size": 7280,
+    "size": 405,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/_collections_abc.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/_collections_abc.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/_collections_abc.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/getpass.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6833333333333333%*

 * *Differences: {"'data_mtime'": '1683843440',*

 * * "'dep_lines'": '{delete: [3, 2, 1]}',*

 * * "'dep_prios'": '{delete: [2, 1, 0]}',*

 * * "'dependencies'": '{delete: [3, 1, 0]}',*

 * * "'hash'": "'1c755308b5f630e123566d4785ff25d521e2d12de4014056713d1d1f2dbbc19f'",*

 * * "'id'": "'getpass'",*

 * * "'interface_hash'": "'85322b1aed39fd71f882f1d766b67bb023d447f2f4543632110184b47c9d4ce3'",*

 * * "'mtime'": '1684623296',*

 * * "'path'": "'/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/get […]*

```diff
@@ -1,38 +1,29 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843440,
     "dep_lines": [
         1,
-        2,
-        3,
-        32,
         1,
         1
     ],
     "dep_prios": [
-        10,
-        5,
-        5,
         5,
         5,
         30
     ],
     "dependencies": [
-        "sys",
-        "types",
         "typing",
-        "typing_extensions",
         "builtins",
         "abc"
     ],
-    "hash": "a1242071aa8e060f1cb055c8d542467362f026499a9139fbcf15943f854ffcf5",
-    "id": "_collections_abc",
+    "hash": "1c755308b5f630e123566d4785ff25d521e2d12de4014056713d1d1f2dbbc19f",
+    "id": "getpass",
     "ignore_all": true,
-    "interface_hash": "8462eba7ef0c128e18111644a04ba39f65ff94458e18e0fb602331c9f0f2c666",
-    "mtime": 1683082840,
+    "interface_hash": "85322b1aed39fd71f882f1d766b67bb023d447f2f4543632110184b47c9d4ce3",
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -66,13 +57,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/_collections_abc.pyi",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/getpass.pyi",
     "plugin_data": null,
-    "size": 2123,
+    "size": 227,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/_ctypes.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/_ctypes.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/_ctypes.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/_ctypes.meta.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'data_mtime'": '1683843440', "'mtime'": '1684623296', "'version_id'": "'1.3.0'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843440,
     "dep_lines": [
         1,
         2,
         3,
         1,
         1,
         1,
@@ -27,15 +27,15 @@
         "abc",
         "typing"
     ],
     "hash": "f3f569576a38ac44f7351d80826ca0da2673c3895b9278a10d671615e6388fc9",
     "id": "_ctypes",
     "ignore_all": true,
     "interface_hash": "509814b22fb0a46ff46bdb95534b870d91bbf4c781f142324fcbc9a63abbfe57",
-    "mtime": 1683082840,
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -73,9 +73,9 @@
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
     "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/_ctypes.pyi",
     "plugin_data": null,
     "size": 829,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/_decimal.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/_decimal.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/_decimal.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/_decimal.meta.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'data_mtime'": '1683843440', "'mtime'": '1684623296', "'version_id'": "'1.3.0'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843440,
     "dep_lines": [
         3,
         1,
         2,
         4,
         5,
         6,
@@ -33,15 +33,15 @@
         "_typeshed",
         "abc"
     ],
     "hash": "48f8deddc79e8ef4fb7dfd0456d1de03d7cd794ec47739eea4b21ccef910976c",
     "id": "_decimal",
     "ignore_all": true,
     "interface_hash": "4aefdf6ad733646f3c4bd30ecc4fcd954023c14046971d5850286c9b9f884219",
-    "mtime": 1683082840,
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -79,9 +79,9 @@
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
     "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/_decimal.pyi",
     "plugin_data": null,
     "size": 13741,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/_operator.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/_operator.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/_operator.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/math.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6966666666666667%*

 * *Differences: {"'data_mtime'": '1683843440',*

 * * "'dep_lines'": '{insert: [(1, 1), (2, 3), (4, 1)], delete: [4, 1, 0]}',*

 * * "'dep_prios'": '{insert: [(5, 30)], delete: [2]}',*

 * * "'dependencies'": "{insert: [(5, '_typeshed')], delete: [2]}",*

 * * "'hash'": "'7383fb2c7e3a74ef80504a0d82a06ed95c4c7754272c54e89a64f1319ab87732'",*

 * * "'id'": "'math'",*

 * * "'interface_hash'": "'97da52b3476c6652bbedd6e0becfa77cc03d1db9c6f3ac24e112b7acebd5aa9a'",*

 * * "'mtime'": '1684623296',*

 * * "'path'": "'/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/. […]*

```diff
@@ -1,41 +1,41 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843440,
     "dep_lines": [
-        3,
-        1,
         2,
+        1,
+        3,
         4,
-        5,
+        1,
         1,
         1
     ],
     "dep_prios": [
         5,
         10,
         5,
         5,
         5,
-        5,
+        30,
         30
     ],
     "dependencies": [
         "collections.abc",
         "sys",
-        "_typeshed",
         "typing",
         "typing_extensions",
         "builtins",
+        "_typeshed",
         "abc"
     ],
-    "hash": "6af6cdd45bab26f05bd668e6a9adf75595caa87cbfb531af9addb4e0dd18636a",
-    "id": "_operator",
+    "hash": "7383fb2c7e3a74ef80504a0d82a06ed95c4c7754272c54e89a64f1319ab87732",
+    "id": "math",
     "ignore_all": true,
-    "interface_hash": "67cc042377da6a0902fae8d0822025f9497774d7bf8608bbdf579a9263d0be11",
-    "mtime": 1683082840,
+    "interface_hash": "97da52b3476c6652bbedd6e0becfa77cc03d1db9c6f3ac24e112b7acebd5aa9a",
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -69,13 +69,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/_operator.pyi",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/math.pyi",
     "plugin_data": null,
-    "size": 6585,
+    "size": 5025,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/_random.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/_random.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/_random.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/msvcrt.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7133333333333334%*

 * *Differences: {"'data_mtime'": '1683843440',*

 * * "'dep_lines'": '{insert: [(1, 2)]}',*

 * * "'dep_prios'": '{insert: [(0, 10)]}',*

 * * "'dependencies'": "{insert: [(0, 'sys')]}",*

 * * "'hash'": "'d4a762dc87ddb7286da0abdb399dec04efb82a19579a4ef11af621851da7b598'",*

 * * "'id'": "'msvcrt'",*

 * * "'interface_hash'": "'71abd058cd942a211c31935f165761a99d332719aaa55402e1adc032384a33d2'",*

 * * "'mtime'": '1684623296',*

 * * "'path'": "'/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/ms […]*

```diff
@@ -1,32 +1,35 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843440,
     "dep_lines": [
         1,
+        2,
         1,
         1,
         1
     ],
     "dep_prios": [
+        10,
         5,
         5,
         30,
         30
     ],
     "dependencies": [
+        "sys",
         "typing_extensions",
         "builtins",
         "abc",
         "typing"
     ],
-    "hash": "fdcf346a4f5cf1e59ed16298d1a44114f183d1641e67553a52691ba2bd17c788",
-    "id": "_random",
+    "hash": "d4a762dc87ddb7286da0abdb399dec04efb82a19579a4ef11af621851da7b598",
+    "id": "msvcrt",
     "ignore_all": true,
-    "interface_hash": "d23b07d1261fda7351f064e4c6f5f3814028e6dd5f7a0c9481f754b58f051b14",
-    "mtime": 1683082840,
+    "interface_hash": "71abd058cd942a211c31935f165761a99d332719aaa55402e1adc032384a33d2",
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -60,13 +63,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/_random.pyi",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/msvcrt.pyi",
     "plugin_data": null,
-    "size": 405,
+    "size": 995,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/_stat.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/_stat.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/_stat.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/_stat.meta.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'data_mtime'": '1683843440', "'mtime'": '1684623296', "'version_id'": "'1.3.0'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843440,
     "dep_lines": [
         1,
         2,
         1,
         1,
         1
     ],
@@ -21,15 +21,15 @@
         "abc",
         "typing"
     ],
     "hash": "4545d9f4011bbe91db363d9537e5d852b7ba1d7bb73b7bda9b540122a7cac958",
     "id": "_stat",
     "ignore_all": true,
     "interface_hash": "d84067f0430367a33a4ee859f861d5b7a8e65b06b082a26e9fd78bed12c88f68",
-    "mtime": 1683082840,
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -67,9 +67,9 @@
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
     "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/_stat.pyi",
     "plugin_data": null,
     "size": 2944,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/_thread.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/_thread.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/_thread.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/_thread.meta.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'data_mtime'": '1683843440', "'mtime'": '1684623296', "'version_id'": "'1.3.0'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843440,
     "dep_lines": [
         3,
         1,
         2,
         4,
         5,
         6,
@@ -33,15 +33,15 @@
         "builtins",
         "abc"
     ],
     "hash": "1dd9af47a90f2cba023502a65ef81a3126f4c5a0299b3b749b8a738dab49754f",
     "id": "_thread",
     "ignore_all": true,
     "interface_hash": "95f43ac86f8a7078f149d2f5fef1e0c0e147c6c84f674df6cad61e2589056369",
-    "mtime": 1683082840,
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -79,9 +79,9 @@
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
     "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/_thread.pyi",
     "plugin_data": null,
     "size": 1646,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/_warnings.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/_warnings.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/_warnings.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/_warnings.meta.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'data_mtime'": '1683843440', "'mtime'": '1684623296', "'version_id'": "'1.3.0'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843440,
     "dep_lines": [
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
@@ -15,15 +15,15 @@
         "builtins",
         "abc"
     ],
     "hash": "12ca327a8db64a2d4a7ce3e48dec89640981b34dbc8f6485f78899f6bd7625bc",
     "id": "_warnings",
     "ignore_all": true,
     "interface_hash": "250924390e6d933b3ffc635b59de8b3c4374c7eeabb61cfb01e29fdc315e0fe9",
-    "mtime": 1683082840,
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -61,9 +61,9 @@
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
     "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/_warnings.pyi",
     "plugin_data": null,
     "size": 1026,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/_weakref.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/_weakref.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/_weakref.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/_weakref.meta.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'data_mtime'": '1683843440', "'mtime'": '1684623296', "'version_id'": "'1.3.0'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843440,
     "dep_lines": [
         2,
         1,
         3,
         4,
         7,
         1,
@@ -30,15 +30,15 @@
         "_typeshed",
         "abc"
     ],
     "hash": "bc440d5501e9ede6acdd4bab5144475ec983f6eecd62e3dc9f71b0c29506a02e",
     "id": "_weakref",
     "ignore_all": true,
     "interface_hash": "0350b65b760e16ce17a716220dcb47693d6db13cbf205f59b96174a733213ca3",
-    "mtime": 1683082840,
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -76,9 +76,9 @@
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
     "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/_weakref.pyi",
     "plugin_data": null,
     "size": 1238,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/_weakrefset.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/_weakrefset.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/_weakrefset.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/_weakrefset.meta.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'data_mtime'": '1683843440', "'mtime'": '1684623296', "'version_id'": "'1.3.0'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843440,
     "dep_lines": [
         2,
         1,
         3,
         4,
         7,
         1,
@@ -30,15 +30,15 @@
         "_typeshed",
         "abc"
     ],
     "hash": "a95feb712aa1ad0440aa1c3ff081329b8a7a976bf976c7cdcd39b1c5d227ea57",
     "id": "_weakrefset",
     "ignore_all": true,
     "interface_hash": "c7f574698c9fcfa33290f1df203a21a874d4b812b7c70d1b41a34ffaacd7dcde",
-    "mtime": 1683082840,
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -76,9 +76,9 @@
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
     "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/_weakrefset.pyi",
     "plugin_data": null,
     "size": 2383,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/abc.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/abc.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/abc.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/abc.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'data_mtime'": '1683843440', "'mtime'": '1684623296', "'version_id'": "'1.3.0'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843440,
     "dep_lines": [
         4,
         1,
         2,
         5,
         6,
         1
@@ -24,15 +24,15 @@
         "typing_extensions",
         "builtins"
     ],
     "hash": "ceadae3f72efc214373499b073a01a7026c2fbec852c488327ec4bad5cb23b67",
     "id": "abc",
     "ignore_all": true,
     "interface_hash": "8e250d1a17f08e7d8ccec54c0cf2b35b3b719c66b3d361d756997fa20769d341",
-    "mtime": 1683082840,
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -70,9 +70,9 @@
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
     "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/abc.pyi",
     "plugin_data": null,
     "size": 1773,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/array.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/array.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/array.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/collections/__init__.meta.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.699198717948718%*

 * *Differences: {"'data_mtime'": '1683843440',*

 * * "'dep_lines'": '{insert: [(0, 11), (3, 3), (4, 4), (5, 5), (6, 8), (7, 1)], delete: [4, 3, 0]}',*

 * * "'dep_prios'": '{insert: [(2, 5), (3, 5), (8, 30)]}',*

 * * "'dependencies'": "{insert: [(2, '_collections_abc'), (6, 'types'), (9, 'array')]}",*

 * * "'hash'": "'f5e16c9ed8790956c54a074ea675d0ce3404db9e0e83a2d254e706d06290b724'",*

 * * "'id'": "'collections'",*

 * * "'interface_hash'": "'9b370fdc1a826574f79bc27163dfa6a4600f8373a80e29c07fa76a47b7e51a6a'",*

 * * "'mtime'": '1684623296',*

 * * "'path'": "'/home […]*

```diff
@@ -1,50 +1,59 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843440,
     "dep_lines": [
-        3,
+        11,
         1,
         2,
-        6,
-        7,
+        3,
+        4,
+        5,
+        8,
+        1,
         1,
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
         10,
         5,
         5,
         5,
         5,
+        5,
+        5,
+        30,
         30,
         30,
         30,
         30
     ],
     "dependencies": [
         "collections.abc",
         "sys",
+        "_collections_abc",
         "_typeshed",
         "typing",
         "typing_extensions",
+        "types",
         "builtins",
         "abc",
+        "array",
         "ctypes",
         "mmap",
         "pickle"
     ],
-    "hash": "857e937ecf94979d69f776505b3837900fb0898aee25681aec6aecea918cecf7",
-    "id": "array",
+    "hash": "f5e16c9ed8790956c54a074ea675d0ce3404db9e0e83a2d254e706d06290b724",
+    "id": "collections",
     "ignore_all": true,
-    "interface_hash": "e8051443f355ce5f520aaf1fab03d18570975779253fb4496a84f9f3f6a8c99d",
-    "mtime": 1683082840,
+    "interface_hash": "9b370fdc1a826574f79bc27163dfa6a4600f8373a80e29c07fa76a47b7e51a6a",
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -78,13 +87,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/array.pyi",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/collections/__init__.pyi",
     "plugin_data": null,
-    "size": 3717,
+    "size": 20830,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/builtins.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/builtins.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/builtins.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/builtins.meta.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8333333333333334%*

 * *Differences: {"'data_mtime'": '1683843440',*

 * * "'hash'": "'c40d372b9738999cc202708777b2205bbb3a183ed81fd5bb2814e1527ca6bbe1'",*

 * * "'mtime'": '1684623296',*

 * * "'size'": '82961',*

 * * "'version_id'": "'1.3.0'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843440,
     "dep_lines": [
         30,
         1,
         2,
         3,
         4,
         5,
@@ -47,19 +47,19 @@
         "abc",
         "array",
         "ctypes",
         "importlib",
         "mmap",
         "pickle"
     ],
-    "hash": "5ec9abe957eda59f9620e08145d6f4b1de55df8e6f46aabcb6098c6d3b2be3ad",
+    "hash": "c40d372b9738999cc202708777b2205bbb3a183ed81fd5bb2814e1527ca6bbe1",
     "id": "builtins",
     "ignore_all": true,
     "interface_hash": "deff0e488aac5f99076ba57eac14fe019849953fe2f0c33e27fedd49c04fe2f7",
-    "mtime": 1683082840,
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -95,11 +95,11 @@
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
     "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/builtins.pyi",
     "plugin_data": null,
-    "size": 82962,
+    "size": 82961,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/codecs.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/codecs.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/codecs.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/mmap.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7018315018315018%*

 * *Differences: {"'data_mtime'": '1683843440',*

 * * "'dep_lines'": '{insert: [(0, 3)], delete: [7, 6, 3, 0]}',*

 * * "'dep_prios'": '{delete: [4, 3, 1]}',*

 * * "'dependencies'": "{insert: [(6, 'abc')], delete: [11, 5, 3, 2]}",*

 * * "'hash'": "'d9e78f0946bc6297002b245e9d85b5be1bcfe36b9a503843f57923c1574200ea'",*

 * * "'id'": "'mmap'",*

 * * "'interface_hash'": "'50e1b41dc66c18ca281b637d2fc764f5c44a55824c90ed2c0e3bacd97b1f67d2'",*

 * * "'mtime'": '1684623296',*

 * * "'path'": "'/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/pytho […]*

```diff
@@ -1,59 +1,50 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843440,
     "dep_lines": [
-        6,
+        3,
         1,
         2,
-        3,
         4,
         5,
-        7,
-        8,
         1,
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
         10,
-        10,
-        5,
-        5,
         5,
         5,
         5,
         5,
         30,
         30,
         30,
         30
     ],
     "dependencies": [
         "collections.abc",
         "sys",
-        "types",
-        "_codecs",
         "_typeshed",
-        "abc",
         "typing",
         "typing_extensions",
         "builtins",
+        "abc",
         "array",
         "ctypes",
-        "mmap",
         "pickle"
     ],
-    "hash": "abcdbf8e98a1d1dcc78b663b26b2c59e461cc46b1fc60fda37f079266e35df68",
-    "id": "codecs",
+    "hash": "d9e78f0946bc6297002b245e9d85b5be1bcfe36b9a503843f57923c1574200ea",
+    "id": "mmap",
     "ignore_all": true,
-    "interface_hash": "0fdf421732626f3c5bf22599d383a7f8eaafb8be02a4922f990ddf72739abf68",
-    "mtime": 1683082840,
+    "interface_hash": "50e1b41dc66c18ca281b637d2fc764f5c44a55824c90ed2c0e3bacd97b1f67d2",
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -87,13 +78,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/codecs.pyi",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/mmap.pyi",
     "plugin_data": null,
-    "size": 11984,
+    "size": 4009,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/contextlib.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/contextlib.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/contextlib.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/threading.meta.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6940326340326342%*

 * *Differences: {"'data_mtime'": '1683843440',*

 * * "'dep_lines'": '{insert: [(0, 3), (3, 4), (4, 5), (6, 51)], delete: [6, 5, 3, 0]}',*

 * * "'dep_prios'": '{insert: [(2, 5)], delete: [0]}',*

 * * "'dependencies'": "{insert: [(6, '_thread'), (8, 'abc')], delete: [8, 1]}",*

 * * "'hash'": "'f2c4bdcb0b9cbdadb0c49fa600420d90019d83e6854d3a5a5aafd988fe3cd378'",*

 * * "'id'": "'threading'",*

 * * "'interface_hash'": "'2a22c41a46eb4d669992a32e118c0cd74d215c10d295d5b535b5fcbe4e403add'",*

 * * "'mtime'": '1684623296',*

 * * "'path'": "'/home/gotmax/Sync/git-repos/packa […]*

```diff
@@ -1,47 +1,47 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843440,
     "dep_lines": [
-        5,
+        3,
         1,
         2,
-        3,
+        4,
+        5,
         6,
-        7,
-        8,
+        51,
         1,
         1
     ],
     "dep_prios": [
         5,
-        5,
         10,
         5,
         5,
         5,
         5,
         5,
+        5,
         30
     ],
     "dependencies": [
         "collections.abc",
-        "abc",
         "sys",
         "_typeshed",
         "types",
         "typing",
         "typing_extensions",
+        "_thread",
         "builtins",
-        "os"
+        "abc"
     ],
-    "hash": "c4656ab0b855c3aed90b09036223336af2d28ce8f7b002882c0cd4971d758511",
-    "id": "contextlib",
+    "hash": "f2c4bdcb0b9cbdadb0c49fa600420d90019d83e6854d3a5a5aafd988fe3cd378",
+    "id": "threading",
     "ignore_all": true,
-    "interface_hash": "e9cddaa2c20280182f6e8dcabfab2c2c1f918d97d5d8881b401ded361f638fad",
-    "mtime": 1683082840,
+    "interface_hash": "2a22c41a46eb4d669992a32e118c0cd74d215c10d295d5b535b5fcbe4e403add",
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -75,13 +75,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/contextlib.pyi",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/threading.pyi",
     "plugin_data": null,
-    "size": 8986,
+    "size": 6028,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/copy.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/copy.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/copy.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/tomlkit/toml_char.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.685%*

 * *Differences: {"'data_mtime'": '1683843440',*

 * * "'dep_lines'": '{insert: [(0, 1)]}',*

 * * "'dep_prios'": '{insert: [(0, 10), (2, 30)], delete: [0]}',*

 * * "'dependencies'": "{insert: [(0, 'string'), (3, 'typing')], delete: [0]}",*

 * * "'hash'": "'c37b10674768959d6a8d9d91c63fecbef96944d34607f7e37c17180f48059c3b'",*

 * * "'id'": "'tomlkit.toml_char'",*

 * * "'interface_hash'": "'0f6e6b41ade4473ef928872c918cc6ba9fe19aad46409e3d07e03bf4e517215a'",*

 * * "'mtime'": '1684623295',*

 * * "'path'": "'/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.n […]*

```diff
@@ -1,29 +1,32 @@
 {
-    "data_mtime": 1681571246,
+    "data_mtime": 1683843440,
     "dep_lines": [
         1,
         1,
+        1,
         1
     ],
     "dep_prios": [
+        10,
         5,
-        5,
+        30,
         30
     ],
     "dependencies": [
-        "typing",
+        "string",
         "builtins",
-        "abc"
+        "abc",
+        "typing"
     ],
-    "hash": "3c11d8d56380cc077c98b9380ef9b6305e8e75db60052fed0260650e15ad1673",
-    "id": "copy",
+    "hash": "c37b10674768959d6a8d9d91c63fecbef96944d34607f7e37c17180f48059c3b",
+    "id": "tomlkit.toml_char",
     "ignore_all": true,
-    "interface_hash": "022ac223f551840f8f85eef00a862d50292bd030555b9d2559f0faabfbcac6dc",
-    "mtime": 1683082840,
+    "interface_hash": "0f6e6b41ade4473ef928872c918cc6ba9fe19aad46409e3d07e03bf4e517215a",
+    "mtime": 1684623295,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -57,13 +60,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/copy.pyi",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib/python3.11/site-packages/tomlkit/toml_char.py",
     "plugin_data": null,
-    "size": 351,
+    "size": 1291,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/dataclasses.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/dataclasses.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/dataclasses.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/warnings.meta.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6894871794871794%*

 * *Differences: {"'data_mtime'": '1683843440',*

 * * "'dep_lines'": '{insert: [(0, 3), (5, 6), (6, 1), (7, 1)], delete: [7, 6, 3, 0]}',*

 * * "'dep_prios'": '{insert: [(7, 30)], delete: [1]}',*

 * * "'dependencies'": "{insert: [(2, '_warnings'), (6, 'builtins'), (7, '_typeshed')], delete: [5, 4, "*

 * *                   '1]}',*

 * * "'hash'": "'9a991da6c7cb550f45efd87385ec22f61a45c69511ab3af2594b6d1ce0487343'",*

 * * "'id'": "'warnings'",*

 * * "'interface_hash'": "'6213d76a67fb20859c74dfa0275499ced0d593f9f03d850e7b0aae112d04c31a'",*

 * * "'mtime'": '1684623296 […]*

```diff
@@ -1,47 +1,47 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843440,
     "dep_lines": [
-        6,
+        3,
         1,
         2,
-        3,
         4,
         5,
-        7,
-        8,
+        6,
+        1,
+        1,
         1
     ],
     "dep_prios": [
         5,
         10,
-        10,
         5,
         5,
         5,
         5,
         5,
+        30,
         30
     ],
     "dependencies": [
         "collections.abc",
-        "enum",
         "sys",
+        "_warnings",
         "types",
-        "_typeshed",
-        "builtins",
         "typing",
         "typing_extensions",
+        "builtins",
+        "_typeshed",
         "abc"
     ],
-    "hash": "415285e494916aa82324cfae93a3f9395ef48cf6d5689d07880f15e2d93eb034",
-    "id": "dataclasses",
+    "hash": "9a991da6c7cb550f45efd87385ec22f61a45c69511ab3af2594b6d1ce0487343",
+    "id": "warnings",
     "ignore_all": true,
-    "interface_hash": "3399190451b5b1f097620ff9bd964e8b7695d0aba902eaa09793a66e0e34707c",
-    "mtime": 1683082840,
+    "interface_hash": "6213d76a67fb20859c74dfa0275499ced0d593f9f03d850e7b0aae112d04c31a",
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -75,13 +75,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/dataclasses.pyi",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/warnings.pyi",
     "plugin_data": null,
-    "size": 8790,
+    "size": 3682,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/datetime.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/datetime.data.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.997899159558343%*

 * *Differences: {"'names'": "{'date': {'node': {'names': {'__new__': {'node': {'type': {'arg_types': {insert: [(1, "*

 * *            "'typing_extensions.SupportsIndex'), (2, 'typing_extensions.SupportsIndex'), (3, "*

 * *            "'typing_extensions.SupportsIndex')], delete: [3, 2, 1]}}}}, 'replace': {'node': "*

 * *            "{'type': {'arg_types': {insert: [(1, 'typing_extensions.SupportsIndex'), (2, "*

 * *            "'typing_extensions.SupportsIndex'), (3, 'typing_extensions.SupportsIndex')], delete: "*

 * *            "[3, 2, 1]}}}}}}} […]*

```diff
@@ -71,14 +71,21 @@
         "Self": {
             ".class": "SymbolTableNode",
             "cross_ref": "typing.Self",
             "kind": "Gdef",
             "module_hidden": true,
             "module_public": false
         },
+        "SupportsIndex": {
+            ".class": "SymbolTableNode",
+            "cross_ref": "typing_extensions.SupportsIndex",
+            "kind": "Gdef",
+            "module_hidden": true,
+            "module_public": false
+        },
         "TypeAlias": {
             ".class": "SymbolTableNode",
             "cross_ref": "typing.TypeAlias",
             "kind": "Gdef",
             "module_hidden": true,
             "module_public": false
         },
@@ -1703,17 +1710,17 @@
                                             "name": "Self",
                                             "namespace": "",
                                             "upper_bound": "datetime.date",
                                             "values": [],
                                             "variance": 0
                                         }
                                     },
-                                    "builtins.int",
-                                    "builtins.int",
-                                    "builtins.int"
+                                    "typing_extensions.SupportsIndex",
+                                    "typing_extensions.SupportsIndex",
+                                    "typing_extensions.SupportsIndex"
                                 ],
                                 "bound_args": [],
                                 "def_extras": {
                                     "first_arg": "cls"
                                 },
                                 "fallback": "builtins.function",
                                 "from_concatenate": false,
@@ -3296,17 +3303,17 @@
                                         "id": 0,
                                         "name": "Self",
                                         "namespace": "",
                                         "upper_bound": "datetime.date",
                                         "values": [],
                                         "variance": 0
                                     },
-                                    "builtins.int",
-                                    "builtins.int",
-                                    "builtins.int"
+                                    "typing_extensions.SupportsIndex",
+                                    "typing_extensions.SupportsIndex",
+                                    "typing_extensions.SupportsIndex"
                                 ],
                                 "bound_args": [],
                                 "def_extras": {
                                     "first_arg": "self"
                                 },
                                 "fallback": "builtins.function",
                                 "from_concatenate": false,
@@ -4084,21 +4091,21 @@
                                             "name": "Self",
                                             "namespace": "",
                                             "upper_bound": "datetime.datetime",
                                             "values": [],
                                             "variance": 0
                                         }
                                     },
-                                    "builtins.int",
-                                    "builtins.int",
-                                    "builtins.int",
-                                    "builtins.int",
-                                    "builtins.int",
-                                    "builtins.int",
-                                    "builtins.int",
+                                    "typing_extensions.SupportsIndex",
+                                    "typing_extensions.SupportsIndex",
+                                    "typing_extensions.SupportsIndex",
+                                    "typing_extensions.SupportsIndex",
+                                    "typing_extensions.SupportsIndex",
+                                    "typing_extensions.SupportsIndex",
+                                    "typing_extensions.SupportsIndex",
                                     {
                                         ".class": "UnionType",
                                         "items": [
                                             "datetime.tzinfo",
                                             {
                                                 ".class": "NoneType"
                                             }
@@ -5670,21 +5677,21 @@
                                         "id": 0,
                                         "name": "Self",
                                         "namespace": "",
                                         "upper_bound": "datetime.datetime",
                                         "values": [],
                                         "variance": 0
                                     },
-                                    "builtins.int",
-                                    "builtins.int",
-                                    "builtins.int",
-                                    "builtins.int",
-                                    "builtins.int",
-                                    "builtins.int",
-                                    "builtins.int",
+                                    "typing_extensions.SupportsIndex",
+                                    "typing_extensions.SupportsIndex",
+                                    "typing_extensions.SupportsIndex",
+                                    "typing_extensions.SupportsIndex",
+                                    "typing_extensions.SupportsIndex",
+                                    "typing_extensions.SupportsIndex",
+                                    "typing_extensions.SupportsIndex",
                                     {
                                         ".class": "UnionType",
                                         "items": [
                                             "datetime.tzinfo",
                                             {
                                                 ".class": "NoneType"
                                             }
@@ -7043,18 +7050,18 @@
                                             "name": "Self",
                                             "namespace": "",
                                             "upper_bound": "datetime.time",
                                             "values": [],
                                             "variance": 0
                                         }
                                     },
-                                    "builtins.int",
-                                    "builtins.int",
-                                    "builtins.int",
-                                    "builtins.int",
+                                    "typing_extensions.SupportsIndex",
+                                    "typing_extensions.SupportsIndex",
+                                    "typing_extensions.SupportsIndex",
+                                    "typing_extensions.SupportsIndex",
                                     {
                                         ".class": "UnionType",
                                         "items": [
                                             "datetime.tzinfo",
                                             {
                                                 ".class": "NoneType"
                                             }
@@ -7784,18 +7791,18 @@
                                         "id": 0,
                                         "name": "Self",
                                         "namespace": "",
                                         "upper_bound": "datetime.time",
                                         "values": [],
                                         "variance": 0
                                     },
-                                    "builtins.int",
-                                    "builtins.int",
-                                    "builtins.int",
-                                    "builtins.int",
+                                    "typing_extensions.SupportsIndex",
+                                    "typing_extensions.SupportsIndex",
+                                    "typing_extensions.SupportsIndex",
+                                    "typing_extensions.SupportsIndex",
                                     {
                                         ".class": "UnionType",
                                         "items": [
                                             "datetime.tzinfo",
                                             {
                                                 ".class": "NoneType"
                                             }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/datetime.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/array.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.672027972027972%*

 * *Differences: {"'data_mtime'": '1683843440',*

 * * "'dep_lines'": '{insert: [(0, 3), (3, 6), (4, 7), (5, 1), (6, 1), (7, 1)], delete: [4, 3, 2]}',*

 * * "'dep_prios'": '{insert: [(1, 10), (6, 30), (7, 30), (8, 30)], delete: [0]}',*

 * * "'dependencies'": "{insert: [(0, 'collections.abc'), (2, '_typeshed'), (6, 'abc'), (7, 'ctypes'), "*

 * *                   "(8, 'mmap'), (9, 'pickle')], delete: [6, 2, 1]}",*

 * * "'hash'": "'857e937ecf94979d69f776505b3837900fb0898aee25681aec6aecea918cecf7'",*

 * * "'id'": "'array'",*

 * * "'interface_hash'": "'e8051443f3 […]*

```diff
@@ -1,41 +1,50 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843440,
     "dep_lines": [
+        3,
         1,
         2,
-        3,
-        4,
-        5,
+        6,
+        7,
+        1,
+        1,
+        1,
         1,
         1
     ],
     "dep_prios": [
-        10,
         5,
+        10,
         5,
         5,
         5,
         5,
+        30,
+        30,
+        30,
         30
     ],
     "dependencies": [
+        "collections.abc",
         "sys",
-        "abc",
-        "time",
+        "_typeshed",
         "typing",
         "typing_extensions",
         "builtins",
-        "_typeshed"
+        "abc",
+        "ctypes",
+        "mmap",
+        "pickle"
     ],
-    "hash": "9e8cf0eee6a7657ab4fb2593655f19adf87b42531d2ec86e59a6425090906307",
-    "id": "datetime",
+    "hash": "857e937ecf94979d69f776505b3837900fb0898aee25681aec6aecea918cecf7",
+    "id": "array",
     "ignore_all": true,
-    "interface_hash": "c9e5e09c95f98a45da00c25b441df8d49b76c091a223028f4ec32ba4f21301bc",
-    "mtime": 1683082840,
+    "interface_hash": "e8051443f355ce5f520aaf1fab03d18570975779253fb4496a84f9f3f6a8c99d",
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -69,13 +78,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/datetime.pyi",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/array.pyi",
     "plugin_data": null,
-    "size": 11239,
+    "size": 3717,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/decimal.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/decimal.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/decimal.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/difflib.meta.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6788359788359788%*

 * *Differences: {"'data_mtime'": '1683843440',*

 * * "'dep_lines'": '{insert: [(0, 2), (2, 3), (3, 6)]}',*

 * * "'dep_prios'": '{insert: [(0, 5), (1, 10), (2, 5)]}',*

 * * "'dependencies'": "{insert: [(0, 'collections.abc'), (1, 'sys'), (2, 'typing'), (3, 'types'), (5, "*

 * *                   "'_typeshed')], delete: [3, 0]}",*

 * * "'hash'": "'5d9e951886d13fa0360b66b47c9ecbe97aa42d246e795301f9926abf344bc305'",*

 * * "'id'": "'difflib'",*

 * * "'interface_hash'": "'3987deac92f18d4d9ae603d9a5b9d8cd6640cc726a2a8b13567989fb34ebee28'",*

 * * "'mtime'": '1684623296' […]*

```diff
@@ -1,32 +1,41 @@
 {
-    "data_mtime": 1681571164,
+    "data_mtime": 1683843440,
     "dep_lines": [
+        2,
         1,
+        3,
+        6,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
+        10,
+        5,
+        5,
         5,
         30,
         30
     ],
     "dependencies": [
-        "_decimal",
+        "collections.abc",
+        "sys",
+        "typing",
+        "types",
         "builtins",
-        "abc",
-        "typing"
+        "_typeshed",
+        "abc"
     ],
-    "hash": "3af726e9b7292d9cb1396aeb99d9d991d615541e03459cf2265298543cb29e69",
-    "id": "decimal",
+    "hash": "5d9e951886d13fa0360b66b47c9ecbe97aa42d246e795301f9926abf344bc305",
+    "id": "difflib",
     "ignore_all": true,
-    "interface_hash": "cea9a17314c38f7e8dbdf2b25979492ee7a7df56056d180bb80a3a1c4cbffd57",
-    "mtime": 1683082840,
+    "interface_hash": "3987deac92f18d4d9ae603d9a5b9d8cd6640cc726a2a8b13567989fb34ebee28",
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -60,13 +69,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/decimal.pyi",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/difflib.pyi",
     "plugin_data": null,
-    "size": 117,
+    "size": 4504,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/difflib.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/difflib.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/difflib.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/webbrowser.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6867195767195767%*

 * *Differences: {"'data_mtime'": '1683843440',*

 * * "'dep_lines'": '{insert: [(2, 2), (3, 4)], delete: [3, 1, 0]}',*

 * * "'dep_prios'": '{delete: [5]}',*

 * * "'dependencies'": "{insert: [(3, 'typing_extensions'), (4, 'builtins'), (5, 'typing')], delete: "*

 * *                   '[5, 4, 3, 2]}',*

 * * "'hash'": "'5eafef06c53dd8b7d5ef6d7ece9ac1448f3f153c6061af7e9701fdf92f9e307c'",*

 * * "'id'": "'webbrowser'",*

 * * "'interface_hash'": "'796e455516416541b15a08d8bc8461efcc8d9a0bd7820fe08ee46ae7b4bcdf5c'",*

 * * "'mtime'": '1684623296',*

 * * "'path'": "'/home/gotmax […]*

```diff
@@ -1,41 +1,38 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843440,
     "dep_lines": [
-        2,
-        1,
         3,
-        6,
         1,
+        2,
+        4,
         1,
         1
     ],
     "dep_prios": [
         5,
         10,
         5,
         5,
         5,
-        30,
         30
     ],
     "dependencies": [
         "collections.abc",
         "sys",
-        "typing",
-        "types",
+        "abc",
+        "typing_extensions",
         "builtins",
-        "_typeshed",
-        "abc"
+        "typing"
     ],
-    "hash": "5d9e951886d13fa0360b66b47c9ecbe97aa42d246e795301f9926abf344bc305",
-    "id": "difflib",
+    "hash": "5eafef06c53dd8b7d5ef6d7ece9ac1448f3f153c6061af7e9701fdf92f9e307c",
+    "id": "webbrowser",
     "ignore_all": true,
-    "interface_hash": "3987deac92f18d4d9ae603d9a5b9d8cd6640cc726a2a8b13567989fb34ebee28",
-    "mtime": 1683082840,
+    "interface_hash": "796e455516416541b15a08d8bc8461efcc8d9a0bd7820fe08ee46ae7b4bcdf5c",
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -69,13 +66,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/difflib.pyi",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/webbrowser.pyi",
     "plugin_data": null,
-    "size": 4504,
+    "size": 2527,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/dis.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/dis.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/dis.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/contextlib.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.684032634032634%*

 * *Differences: {"'data_mtime'": '1683843440',*

 * * "'dep_lines'": '{insert: [(0, 5), (3, 3), (5, 7), (6, 8)], delete: [6, 4, 3, 0]}',*

 * * "'dep_prios'": '{insert: [(1, 5), (7, 5)], delete: [7, 1]}',*

 * * "'dependencies'": "{insert: [(1, 'abc'), (3, '_typeshed'), (8, 'os')], delete: [8, 7, 3]}",*

 * * "'hash'": "'c4656ab0b855c3aed90b09036223336af2d28ce8f7b002882c0cd4971d758511'",*

 * * "'id'": "'contextlib'",*

 * * "'interface_hash'": "'e9cddaa2c20280182f6e8dcabfab2c2c1f918d97d5d8881b401ded361f638fad'",*

 * * "'mtime'": '1684623296',*

 * * "'path'": "'/home/ […]*

```diff
@@ -1,47 +1,47 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843440,
     "dep_lines": [
-        3,
+        5,
         1,
         2,
-        4,
-        5,
+        3,
         6,
-        1,
+        7,
+        8,
         1,
         1
     ],
     "dep_prios": [
         5,
+        5,
         10,
-        10,
         5,
         5,
         5,
         5,
-        30,
+        5,
         30
     ],
     "dependencies": [
         "collections.abc",
+        "abc",
         "sys",
+        "_typeshed",
         "types",
-        "opcode",
         "typing",
         "typing_extensions",
         "builtins",
-        "_typeshed",
-        "abc"
+        "os"
     ],
-    "hash": "0752728fe06a3c30c30280311b749ec46eee32ec08b5ec9221c552757dd04ca7",
-    "id": "dis",
+    "hash": "c4656ab0b855c3aed90b09036223336af2d28ce8f7b002882c0cd4971d758511",
+    "id": "contextlib",
     "ignore_all": true,
-    "interface_hash": "549c8473c8ca310f5f94ab3adb5facd61785d1e89865622c4a97cf625bc847ed",
-    "mtime": 1683082840,
+    "interface_hash": "e9cddaa2c20280182f6e8dcabfab2c2c1f918d97d5d8881b401ded361f638fad",
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -75,13 +75,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/dis.pyi",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/contextlib.pyi",
     "plugin_data": null,
-    "size": 4403,
+    "size": 8986,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/enum.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/enum.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/enum.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/enum.meta.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'data_mtime'": '1683843440', "'mtime'": '1684623296', "'version_id'": "'1.3.0'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843440,
     "dep_lines": [
         7,
         1,
         2,
         3,
         5,
         6,
@@ -30,15 +30,15 @@
         "typing",
         "typing_extensions"
     ],
     "hash": "ed43c787e02aed02cae5cca660012347f2c99e5ea96f4fd79d96d060f4aa5685",
     "id": "enum",
     "ignore_all": true,
     "interface_hash": "f6ca2a77baf46b68cd385f1e1b085c20ea997b35bab747dde9eba390400eda8d",
-    "mtime": 1683082840,
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -76,9 +76,9 @@
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
     "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/enum.pyi",
     "plugin_data": null,
     "size": 10374,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/errno.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/errno.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/errno.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/decimal.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7033333333333334%*

 * *Differences: {"'data_mtime'": '1683843440',*

 * * "'dep_lines'": '{delete: [0]}',*

 * * "'dep_prios'": '{delete: [1]}',*

 * * "'dependencies'": "{insert: [(0, '_decimal')], delete: [1, 0]}",*

 * * "'hash'": "'3af726e9b7292d9cb1396aeb99d9d991d615541e03459cf2265298543cb29e69'",*

 * * "'id'": "'decimal'",*

 * * "'interface_hash'": "'cea9a17314c38f7e8dbdf2b25979492ee7a7df56056d180bb80a3a1c4cbffd57'",*

 * * "'mtime'": '1684623296',*

 * * "'path'": "'/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshe […]*

```diff
@@ -1,35 +1,32 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843440,
     "dep_lines": [
-        2,
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
-        10,
         5,
         30,
         30
     ],
     "dependencies": [
-        "collections.abc",
-        "sys",
+        "_decimal",
         "builtins",
         "abc",
         "typing"
     ],
-    "hash": "bd0401f598c4a64b36aec1483018fe5d595ea6c95bdead83dc5e75db0925a27c",
-    "id": "errno",
+    "hash": "3af726e9b7292d9cb1396aeb99d9d991d615541e03459cf2265298543cb29e69",
+    "id": "decimal",
     "ignore_all": true,
-    "interface_hash": "03b1dd20dd89d01a2a439bbf48f8d1ef52d84cbf0f05ee4e433fda2734cb8842",
-    "mtime": 1683082840,
+    "interface_hash": "cea9a17314c38f7e8dbdf2b25979492ee7a7df56056d180bb80a3a1c4cbffd57",
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -63,13 +60,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/errno.pyi",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/decimal.pyi",
     "plugin_data": null,
-    "size": 3911,
+    "size": 117,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/fractions.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/fractions.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/fractions.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/errno.meta.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6747474747474748%*

 * *Differences: {"'data_mtime'": '1683843440',*

 * * "'dep_lines'": '{delete: [6, 5, 4, 3, 2, 1]}',*

 * * "'dep_prios'": '{delete: [8, 7, 5, 4, 3, 2]}',*

 * * "'dependencies'": "{insert: [(4, 'typing')], delete: [9, 8, 7, 5, 4, 3, 2]}",*

 * * "'hash'": "'bd0401f598c4a64b36aec1483018fe5d595ea6c95bdead83dc5e75db0925a27c'",*

 * * "'id'": "'errno'",*

 * * "'interface_hash'": "'03b1dd20dd89d01a2a439bbf48f8d1ef52d84cbf0f05ee4e433fda2734cb8842'",*

 * * "'mtime'": '1684623296',*

 * * "'path'": "'/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/li […]*

```diff
@@ -1,53 +1,35 @@
 {
-    "data_mtime": 1681571164,
+    "data_mtime": 1683843440,
     "dep_lines": [
         2,
         1,
-        3,
-        4,
-        5,
-        6,
-        1,
-        1,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
         10,
         5,
-        5,
-        5,
-        5,
-        5,
-        30,
-        30,
         30,
         30
     ],
     "dependencies": [
         "collections.abc",
         "sys",
-        "decimal",
-        "numbers",
-        "typing",
-        "typing_extensions",
         "builtins",
-        "_decimal",
-        "_operator",
-        "_typeshed",
-        "abc"
+        "abc",
+        "typing"
     ],
-    "hash": "8920640aa1ef26e4093747df64e273af50a65c28cef9cb693e6feaff46bdfe88",
-    "id": "fractions",
+    "hash": "bd0401f598c4a64b36aec1483018fe5d595ea6c95bdead83dc5e75db0925a27c",
+    "id": "errno",
     "ignore_all": true,
-    "interface_hash": "22a8033e0f019548b33352a9f733c7e5810adac15da15f82803a06b46f30f94a",
-    "mtime": 1683082840,
+    "interface_hash": "03b1dd20dd89d01a2a439bbf48f8d1ef52d84cbf0f05ee4e433fda2734cb8842",
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -81,13 +63,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/fractions.pyi",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/errno.pyi",
     "plugin_data": null,
-    "size": 5584,
+    "size": 3911,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/functools.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/functools.data.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999991544890157%*

 * *Differences: {"'names'": "{'_Descriptor': {'node': {'line': 97}}, 'cached_property': {'node': {'names': "*

 * *            "{'__get__': {'node': {'items': {0: {'func': {'type': {'arg_types': {0: {'.class': "*

 * *            "'TypeVarType', 'fullname': 'functools.cached_property.Self', 'id': 0, 'name': 'Self', "*

 * *            "'namespace': '', 'upper_bound': OrderedDict([('.class', 'Instance'), ('args', "*

 * *            "[OrderedDict([('.class', 'TypeVarType'), ('fullname', 'functools._T'), ('id', 1), "*

 * *            "('name', '_T'), (' […]*

```diff
@@ -1621,15 +1621,15 @@
             "kind": "Gdef",
             "module_public": false,
             "node": {
                 ".class": "TypeAlias",
                 "alias_tvars": [],
                 "column": 0,
                 "fullname": "functools._Descriptor",
-                "line": 88,
+                "line": 97,
                 "no_args": false,
                 "normalized": false,
                 "target": {
                     ".class": "AnyType",
                     "missing_import_name": null,
                     "source_any": null,
                     "type_of_any": 6
@@ -4035,28 +4035,37 @@
                                             "arg_names": [
                                                 "self",
                                                 "instance",
                                                 "owner"
                                             ],
                                             "arg_types": [
                                                 {
-                                                    ".class": "Instance",
-                                                    "args": [
-                                                        {
-                                                            ".class": "TypeVarType",
-                                                            "fullname": "functools._T",
-                                                            "id": 1,
-                                                            "name": "_T",
-                                                            "namespace": "functools.cached_property",
-                                                            "upper_bound": "builtins.object",
-                                                            "values": [],
-                                                            "variance": 0
-                                                        }
-                                                    ],
-                                                    "type_ref": "functools.cached_property"
+                                                    ".class": "TypeVarType",
+                                                    "fullname": "functools.cached_property.Self",
+                                                    "id": 0,
+                                                    "name": "Self",
+                                                    "namespace": "",
+                                                    "upper_bound": {
+                                                        ".class": "Instance",
+                                                        "args": [
+                                                            {
+                                                                ".class": "TypeVarType",
+                                                                "fullname": "functools._T",
+                                                                "id": 1,
+                                                                "name": "_T",
+                                                                "namespace": "functools.cached_property",
+                                                                "upper_bound": "builtins.object",
+                                                                "values": [],
+                                                                "variance": 0
+                                                            }
+                                                        ],
+                                                        "type_ref": "functools.cached_property"
+                                                    },
+                                                    "values": [],
+                                                    "variance": 0
                                                 },
                                                 {
                                                     ".class": "NoneType"
                                                 },
                                                 {
                                                     ".class": "UnionType",
                                                     "items": [
@@ -4081,32 +4090,67 @@
                                             },
                                             "fallback": "builtins.function",
                                             "from_concatenate": false,
                                             "implicit": false,
                                             "is_ellipsis_args": false,
                                             "name": "__get__ of cached_property",
                                             "ret_type": {
-                                                ".class": "Instance",
-                                                "args": [
-                                                    {
-                                                        ".class": "TypeVarType",
-                                                        "fullname": "functools._T",
-                                                        "id": 1,
-                                                        "name": "_T",
-                                                        "namespace": "functools.cached_property",
-                                                        "upper_bound": "builtins.object",
-                                                        "values": [],
-                                                        "variance": 0
-                                                    }
-                                                ],
-                                                "type_ref": "functools.cached_property"
+                                                ".class": "TypeVarType",
+                                                "fullname": "functools.cached_property.Self",
+                                                "id": 0,
+                                                "name": "Self",
+                                                "namespace": "",
+                                                "upper_bound": {
+                                                    ".class": "Instance",
+                                                    "args": [
+                                                        {
+                                                            ".class": "TypeVarType",
+                                                            "fullname": "functools._T",
+                                                            "id": 1,
+                                                            "name": "_T",
+                                                            "namespace": "functools.cached_property",
+                                                            "upper_bound": "builtins.object",
+                                                            "values": [],
+                                                            "variance": 0
+                                                        }
+                                                    ],
+                                                    "type_ref": "functools.cached_property"
+                                                },
+                                                "values": [],
+                                                "variance": 0
                                             },
                                             "type_guard": null,
                                             "unpack_kwargs": false,
-                                            "variables": []
+                                            "variables": [
+                                                {
+                                                    ".class": "TypeVarType",
+                                                    "fullname": "functools.cached_property.Self",
+                                                    "id": 0,
+                                                    "name": "Self",
+                                                    "namespace": "",
+                                                    "upper_bound": {
+                                                        ".class": "Instance",
+                                                        "args": [
+                                                            {
+                                                                ".class": "TypeVarType",
+                                                                "fullname": "functools._T",
+                                                                "id": 1,
+                                                                "name": "_T",
+                                                                "namespace": "functools.cached_property",
+                                                                "upper_bound": "builtins.object",
+                                                                "values": [],
+                                                                "variance": 0
+                                                            }
+                                                        ],
+                                                        "type_ref": "functools.cached_property"
+                                                    },
+                                                    "values": [],
+                                                    "variance": 0
+                                                }
+                                            ]
                                         }
                                     },
                                     "is_overload": true,
                                     "var": {
                                         ".class": "Var",
                                         "flags": [
                                             "is_inferred"
@@ -4235,28 +4279,37 @@
                                         "arg_names": [
                                             "self",
                                             "instance",
                                             "owner"
                                         ],
                                         "arg_types": [
                                             {
-                                                ".class": "Instance",
-                                                "args": [
-                                                    {
-                                                        ".class": "TypeVarType",
-                                                        "fullname": "functools._T",
-                                                        "id": 1,
-                                                        "name": "_T",
-                                                        "namespace": "functools.cached_property",
-                                                        "upper_bound": "builtins.object",
-                                                        "values": [],
-                                                        "variance": 0
-                                                    }
-                                                ],
-                                                "type_ref": "functools.cached_property"
+                                                ".class": "TypeVarType",
+                                                "fullname": "functools.cached_property.Self",
+                                                "id": 0,
+                                                "name": "Self",
+                                                "namespace": "",
+                                                "upper_bound": {
+                                                    ".class": "Instance",
+                                                    "args": [
+                                                        {
+                                                            ".class": "TypeVarType",
+                                                            "fullname": "functools._T",
+                                                            "id": 1,
+                                                            "name": "_T",
+                                                            "namespace": "functools.cached_property",
+                                                            "upper_bound": "builtins.object",
+                                                            "values": [],
+                                                            "variance": 0
+                                                        }
+                                                    ],
+                                                    "type_ref": "functools.cached_property"
+                                                },
+                                                "values": [],
+                                                "variance": 0
                                             },
                                             {
                                                 ".class": "NoneType"
                                             },
                                             {
                                                 ".class": "UnionType",
                                                 "items": [
@@ -4281,32 +4334,67 @@
                                         },
                                         "fallback": "builtins.function",
                                         "from_concatenate": false,
                                         "implicit": false,
                                         "is_ellipsis_args": false,
                                         "name": "__get__ of cached_property",
                                         "ret_type": {
-                                            ".class": "Instance",
-                                            "args": [
-                                                {
-                                                    ".class": "TypeVarType",
-                                                    "fullname": "functools._T",
-                                                    "id": 1,
-                                                    "name": "_T",
-                                                    "namespace": "functools.cached_property",
-                                                    "upper_bound": "builtins.object",
-                                                    "values": [],
-                                                    "variance": 0
-                                                }
-                                            ],
-                                            "type_ref": "functools.cached_property"
+                                            ".class": "TypeVarType",
+                                            "fullname": "functools.cached_property.Self",
+                                            "id": 0,
+                                            "name": "Self",
+                                            "namespace": "",
+                                            "upper_bound": {
+                                                ".class": "Instance",
+                                                "args": [
+                                                    {
+                                                        ".class": "TypeVarType",
+                                                        "fullname": "functools._T",
+                                                        "id": 1,
+                                                        "name": "_T",
+                                                        "namespace": "functools.cached_property",
+                                                        "upper_bound": "builtins.object",
+                                                        "values": [],
+                                                        "variance": 0
+                                                    }
+                                                ],
+                                                "type_ref": "functools.cached_property"
+                                            },
+                                            "values": [],
+                                            "variance": 0
                                         },
                                         "type_guard": null,
                                         "unpack_kwargs": false,
-                                        "variables": []
+                                        "variables": [
+                                            {
+                                                ".class": "TypeVarType",
+                                                "fullname": "functools.cached_property.Self",
+                                                "id": 0,
+                                                "name": "Self",
+                                                "namespace": "",
+                                                "upper_bound": {
+                                                    ".class": "Instance",
+                                                    "args": [
+                                                        {
+                                                            ".class": "TypeVarType",
+                                                            "fullname": "functools._T",
+                                                            "id": 1,
+                                                            "name": "_T",
+                                                            "namespace": "functools.cached_property",
+                                                            "upper_bound": "builtins.object",
+                                                            "values": [],
+                                                            "variance": 0
+                                                        }
+                                                    ],
+                                                    "type_ref": "functools.cached_property"
+                                                },
+                                                "values": [],
+                                                "variance": 0
+                                            }
+                                        ]
                                     },
                                     {
                                         ".class": "CallableType",
                                         "arg_kinds": [
                                             0,
                                             0,
                                             1
@@ -4706,15 +4794,39 @@
                                 "type_guard": null,
                                 "unpack_kwargs": false,
                                 "variables": []
                             }
                         }
                     }
                 },
-                "self_type": null,
+                "self_type": {
+                    ".class": "TypeVarType",
+                    "fullname": "functools.cached_property.Self",
+                    "id": 0,
+                    "name": "Self",
+                    "namespace": "",
+                    "upper_bound": {
+                        ".class": "Instance",
+                        "args": [
+                            {
+                                ".class": "TypeVarType",
+                                "fullname": "functools._T",
+                                "id": 1,
+                                "name": "_T",
+                                "namespace": "functools.cached_property",
+                                "upper_bound": "builtins.object",
+                                "values": [],
+                                "variance": 0
+                            }
+                        ],
+                        "type_ref": "functools.cached_property"
+                    },
+                    "values": [],
+                    "variance": 0
+                },
                 "slots": null,
                 "tuple_type": null,
                 "type_vars": [
                     "_T"
                 ],
                 "typeddict_type": null
             }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/functools.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/dataclasses.meta.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7001851851851851%*

 * *Differences: {"'data_mtime'": '1683843440',*

 * * "'dep_lines'": '{insert: [(0, 6), (4, 4), (6, 7), (7, 8)], delete: [6, 5, 0]}',*

 * * "'dep_prios'": '{insert: [(1, 10)]}',*

 * * "'dependencies'": "{insert: [(1, 'enum'), (5, 'builtins')], delete: [6]}",*

 * * "'hash'": "'3c60aa626a823ecffdf68a8e1856506b8ebdd4c073cff06364b4f619e489b5a9'",*

 * * "'id'": "'dataclasses'",*

 * * "'interface_hash'": "'3399190451b5b1f097620ff9bd964e8b7695d0aba902eaa09793a66e0e34707c'",*

 * * "'mtime'": '1684623296',*

 * * "'path'": "'/home/gotmax/Sync/git-repos/packaging/fedora_rpm […]*

```diff
@@ -1,44 +1,47 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843440,
     "dep_lines": [
-        4,
+        6,
         1,
         2,
         3,
+        4,
         5,
-        6,
-        1,
+        7,
+        8,
         1
     ],
     "dep_prios": [
         5,
         10,
+        10,
         5,
         5,
         5,
         5,
         5,
         30
     ],
     "dependencies": [
         "collections.abc",
+        "enum",
         "sys",
         "types",
         "_typeshed",
+        "builtins",
         "typing",
         "typing_extensions",
-        "builtins",
         "abc"
     ],
-    "hash": "91ac2c9281c81c7eaee95c89dc17b8b7fb0f2ba04514a897c736d475d41f5870",
-    "id": "functools",
+    "hash": "3c60aa626a823ecffdf68a8e1856506b8ebdd4c073cff06364b4f619e489b5a9",
+    "id": "dataclasses",
     "ignore_all": true,
-    "interface_hash": "6ebeb04d43784b6a1c1c1df84e41afa5018a493f941bb6dc09b63355637f45e0",
-    "mtime": 1683082840,
+    "interface_hash": "3399190451b5b1f097620ff9bd964e8b7695d0aba902eaa09793a66e0e34707c",
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -72,13 +75,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/functools.pyi",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/dataclasses.pyi",
     "plugin_data": null,
-    "size": 6535,
+    "size": 9397,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/genericpath.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/genericpath.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/genericpath.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/genericpath.meta.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'data_mtime'": '1683843440', "'mtime'": '1684623296', "'version_id'": "'1.3.0'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843440,
     "dep_lines": [
         3,
         1,
         2,
         4,
         5,
         1,
@@ -27,15 +27,15 @@
         "builtins",
         "abc"
     ],
     "hash": "50d45ab3fd6f6adc2a69a00ae4885e0c123e9e773ee3d3366768e99b9e6e8fbd",
     "id": "genericpath",
     "ignore_all": true,
     "interface_hash": "a3c3e7abc4b8536cdb81c011fd195ce552fa9690945d00c7473b472c091baea0",
-    "mtime": 1683082840,
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -73,9 +73,9 @@
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
     "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/genericpath.pyi",
     "plugin_data": null,
     "size": 1756,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/getpass.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/getpass.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/getpass.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/tomllib.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6933333333333332%*

 * *Differences: {"'data_mtime'": '1683843440',*

 * * "'dep_lines'": '{insert: [(0, 2), (2, 3)]}',*

 * * "'dep_prios'": '{insert: [(0, 5), (1, 5)]}',*

 * * "'dependencies'": "{insert: [(0, 'collections.abc'), (1, '_typeshed')]}",*

 * * "'hash'": "'f0faf1b61c8a37d2a2dc1cfd5cfd21097c2b5dfbcd2275bf8b025007a94a56f1'",*

 * * "'id'": "'tomllib'",*

 * * "'interface_hash'": "'0dbff1dc077a42ad9993c43115582bd792aaa05efc3634a4c9447a3bb2a83551'",*

 * * "'mtime'": '1684623296',*

 * * "'path'": "'/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/py […]*

```diff
@@ -1,29 +1,35 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843440,
     "dep_lines": [
+        2,
         1,
+        3,
         1,
         1
     ],
     "dep_prios": [
         5,
         5,
+        5,
+        5,
         30
     ],
     "dependencies": [
+        "collections.abc",
+        "_typeshed",
         "typing",
         "builtins",
         "abc"
     ],
-    "hash": "1c755308b5f630e123566d4785ff25d521e2d12de4014056713d1d1f2dbbc19f",
-    "id": "getpass",
+    "hash": "f0faf1b61c8a37d2a2dc1cfd5cfd21097c2b5dfbcd2275bf8b025007a94a56f1",
+    "id": "tomllib",
     "ignore_all": true,
-    "interface_hash": "85322b1aed39fd71f882f1d766b67bb023d447f2f4543632110184b47c9d4ce3",
-    "mtime": 1683082840,
+    "interface_hash": "0dbff1dc077a42ad9993c43115582bd792aaa05efc3634a4c9447a3bb2a83551",
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -57,13 +63,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/getpass.pyi",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/tomllib.pyi",
     "plugin_data": null,
-    "size": 227,
+    "size": 374,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/gettext.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/gettext.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/gettext.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/sre_constants.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6888888888888888%*

 * *Differences: {"'data_mtime'": '1683843439',*

 * * "'dep_lines'": '{insert: [(3, 1)], delete: [5, 4, 0]}',*

 * * "'dep_prios'": '{insert: [(4, 30)], delete: [3, 1, 0]}',*

 * * "'dependencies'": "{insert: [(4, '_typeshed')], delete: [3, 1, 0]}",*

 * * "'hash'": "'cfb8327ad6d1f82090949665027111e9f4f54c3e1dc0b5baec0b377845590a5c'",*

 * * "'id'": "'sre_constants'",*

 * * "'interface_hash'": "'fc1c739257bfb8151b2188ae01d06d69f8ba90f3c9a8a68ad5fa93062826d8db'",*

 * * "'mtime'": '1684623296',*

 * * "'path'": "'/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tom […]*

```diff
@@ -1,44 +1,38 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843439,
     "dep_lines": [
-        4,
         1,
         2,
         3,
-        5,
-        6,
+        1,
         1,
         1
     ],
     "dep_prios": [
-        5,
-        10,
         10,
         5,
         5,
         5,
-        5,
+        30,
         30
     ],
     "dependencies": [
-        "collections.abc",
-        "io",
         "sys",
-        "_typeshed",
         "typing",
         "typing_extensions",
         "builtins",
+        "_typeshed",
         "abc"
     ],
-    "hash": "05bcfbfe3e5ba3e16560a69ffaeba02e1e3b810e78532bd08cc44617306fc579",
-    "id": "gettext",
+    "hash": "cfb8327ad6d1f82090949665027111e9f4f54c3e1dc0b5baec0b377845590a5c",
+    "id": "sre_constants",
     "ignore_all": true,
-    "interface_hash": "1188a81fd724794ad25bb1216f2375f068fb732d6cfed257da7c28778c9a0fe0",
-    "mtime": 1683082840,
+    "interface_hash": "fc1c739257bfb8151b2188ae01d06d69f8ba90f3c9a8a68ad5fa93062826d8db",
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -72,13 +66,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/gettext.pyi",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/sre_constants.pyi",
     "plugin_data": null,
-    "size": 6274,
+    "size": 3986,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/glob.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/glob.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/glob.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/functools.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6966666666666667%*

 * *Differences: {"'data_mtime'": '1683843440',*

 * * "'dep_lines'": '{insert: [(0, 4), (3, 3), (4, 5), (5, 6)], delete: [3, 0]}',*

 * * "'dep_prios'": '{insert: [(2, 5), (3, 5)]}',*

 * * "'dependencies'": "{insert: [(2, 'types'), (5, 'typing_extensions')]}",*

 * * "'hash'": "'a55fc5249be5a8cc7802223683191b924150d000994f1beac88c3134361db0ee'",*

 * * "'id'": "'functools'",*

 * * "'interface_hash'": "'1dccc641c5682f5b9187e57c7b2e4fe7334a961a5faa7ea2e38ed22cba36b4c1'",*

 * * "'mtime'": '1684623296',*

 * * "'path'": "'/home/gotmax/Sync/git-repos/packaging/fedora_rpms […]*

```diff
@@ -1,38 +1,44 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843440,
     "dep_lines": [
-        3,
+        4,
         1,
         2,
-        4,
+        3,
+        5,
+        6,
         1,
         1
     ],
     "dep_prios": [
         5,
         10,
         5,
         5,
         5,
+        5,
+        5,
         30
     ],
     "dependencies": [
         "collections.abc",
         "sys",
+        "types",
         "_typeshed",
         "typing",
+        "typing_extensions",
         "builtins",
         "abc"
     ],
-    "hash": "b23877cf7cc743ec86f6a87b449a4cc1a92ad72e573a19c7a17a82c3fc3507a2",
-    "id": "glob",
+    "hash": "a55fc5249be5a8cc7802223683191b924150d000994f1beac88c3134361db0ee",
+    "id": "functools",
     "ignore_all": true,
-    "interface_hash": "266e5d53c08178ba44335144c11737885af67ee5e9dc75a2aebc95df4df21509",
-    "mtime": 1683082840,
+    "interface_hash": "1dccc641c5682f5b9187e57c7b2e4fe7334a961a5faa7ea2e38ed22cba36b4c1",
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -66,13 +72,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/glob.pyi",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/functools.pyi",
     "plugin_data": null,
-    "size": 1421,
+    "size": 6712,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/inspect.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/inspect.data.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9990677235937335%*

 * *Differences: {"'names'": "{'_GetMembersPredicate': {'node': {'line': 165}}, '_GetMembersReturn': {'node': "*

 * *            "{'line': 167}}, '_IntrospectableCallable': {'node': {'line': 291}}, '_Object': "*

 * *            "{'node': {'line': 589}}, '_SourceObjectType': {'node': {'line': 274}}, 'getmembers': "*

 * *            "{'node': {'.class': 'OverloadedFuncDef', 'type': {'.class': 'Overloaded', 'items': "*

 * *            "[OrderedDict([('.class', 'CallableType'), ('arg_kinds', [0, 0]), ('arg_names', "*

 * *            "['object', 'predic […]*

```diff
@@ -16252,15 +16252,15 @@
             "kind": "Gdef",
             "module_public": false,
             "node": {
                 ".class": "TypeAlias",
                 "alias_tvars": [],
                 "column": 0,
                 "fullname": "inspect._GetMembersPredicate",
-                "line": 164,
+                "line": 165,
                 "no_args": false,
                 "normalized": false,
                 "target": {
                     ".class": "CallableType",
                     "arg_kinds": [
                         0
                     ],
@@ -16285,24 +16285,86 @@
                     "ret_type": "builtins.bool",
                     "type_guard": null,
                     "unpack_kwargs": false,
                     "variables": []
                 }
             }
         },
+        "_GetMembersPredicateTypeGuard": {
+            ".class": "SymbolTableNode",
+            "kind": "Gdef",
+            "module_public": false,
+            "node": {
+                ".class": "TypeAlias",
+                "alias_tvars": [
+                    {
+                        ".class": "TypeVarType",
+                        "fullname": "inspect._T",
+                        "id": 1,
+                        "name": "_T",
+                        "namespace": "inspect._GetMembersPredicateTypeGuard",
+                        "upper_bound": "builtins.object",
+                        "values": [],
+                        "variance": 0
+                    }
+                ],
+                "column": 0,
+                "fullname": "inspect._GetMembersPredicateTypeGuard",
+                "line": 164,
+                "no_args": false,
+                "normalized": false,
+                "target": {
+                    ".class": "CallableType",
+                    "arg_kinds": [
+                        0
+                    ],
+                    "arg_names": [
+                        null
+                    ],
+                    "arg_types": [
+                        {
+                            ".class": "AnyType",
+                            "missing_import_name": null,
+                            "source_any": null,
+                            "type_of_any": 6
+                        }
+                    ],
+                    "bound_args": [],
+                    "def_extras": {},
+                    "fallback": "builtins.function",
+                    "from_concatenate": false,
+                    "implicit": false,
+                    "is_ellipsis_args": false,
+                    "name": null,
+                    "ret_type": "builtins.bool",
+                    "type_guard": {
+                        ".class": "TypeVarType",
+                        "fullname": "inspect._T",
+                        "id": 1,
+                        "name": "_T",
+                        "namespace": "inspect._GetMembersPredicateTypeGuard",
+                        "upper_bound": "builtins.object",
+                        "values": [],
+                        "variance": 0
+                    },
+                    "unpack_kwargs": false,
+                    "variables": []
+                }
+            }
+        },
         "_GetMembersReturn": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "module_public": false,
             "node": {
                 ".class": "TypeAlias",
                 "alias_tvars": [],
                 "column": 0,
                 "fullname": "inspect._GetMembersReturn",
-                "line": 165,
+                "line": 167,
                 "no_args": false,
                 "normalized": false,
                 "target": {
                     ".class": "Instance",
                     "args": [
                         {
                             ".class": "TupleType",
@@ -16330,24 +16392,84 @@
                             }
                         }
                     ],
                     "type_ref": "builtins.list"
                 }
             }
         },
+        "_GetMembersReturnTypeGuard": {
+            ".class": "SymbolTableNode",
+            "kind": "Gdef",
+            "module_public": false,
+            "node": {
+                ".class": "TypeAlias",
+                "alias_tvars": [
+                    {
+                        ".class": "TypeVarType",
+                        "fullname": "inspect._T",
+                        "id": 1,
+                        "name": "_T",
+                        "namespace": "inspect._GetMembersReturnTypeGuard",
+                        "upper_bound": "builtins.object",
+                        "values": [],
+                        "variance": 0
+                    }
+                ],
+                "column": 0,
+                "fullname": "inspect._GetMembersReturnTypeGuard",
+                "line": 166,
+                "no_args": false,
+                "normalized": false,
+                "target": {
+                    ".class": "Instance",
+                    "args": [
+                        {
+                            ".class": "TupleType",
+                            "implicit": false,
+                            "items": [
+                                "builtins.str",
+                                {
+                                    ".class": "TypeVarType",
+                                    "fullname": "inspect._T",
+                                    "id": 1,
+                                    "name": "_T",
+                                    "namespace": "inspect._GetMembersReturnTypeGuard",
+                                    "upper_bound": "builtins.object",
+                                    "values": [],
+                                    "variance": 0
+                                }
+                            ],
+                            "partial_fallback": {
+                                ".class": "Instance",
+                                "args": [
+                                    {
+                                        ".class": "AnyType",
+                                        "missing_import_name": null,
+                                        "source_any": null,
+                                        "type_of_any": 6
+                                    }
+                                ],
+                                "type_ref": "builtins.tuple"
+                            }
+                        }
+                    ],
+                    "type_ref": "builtins.list"
+                }
+            }
+        },
         "_IntrospectableCallable": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "module_public": false,
             "node": {
                 ".class": "TypeAlias",
                 "alias_tvars": [],
                 "column": 0,
                 "fullname": "inspect._IntrospectableCallable",
-                "line": 283,
+                "line": 291,
                 "no_args": false,
                 "normalized": false,
                 "target": {
                     ".class": "CallableType",
                     "arg_kinds": [
                         2,
                         4
@@ -16394,15 +16516,15 @@
             "kind": "Gdef",
             "module_public": false,
             "node": {
                 ".class": "TypeAlias",
                 "alias_tvars": [],
                 "column": 0,
                 "fullname": "inspect._Object",
-                "line": 581,
+                "line": 589,
                 "no_args": true,
                 "normalized": false,
                 "target": "builtins.object"
             }
         },
         "_P": {
             ".class": "SymbolTableNode",
@@ -16624,15 +16746,15 @@
             "kind": "Gdef",
             "module_public": false,
             "node": {
                 ".class": "TypeAlias",
                 "alias_tvars": [],
                 "column": 0,
                 "fullname": "inspect._SourceObjectType",
-                "line": 266,
+                "line": 274,
                 "no_args": false,
                 "normalized": false,
                 "target": {
                     ".class": "UnionType",
                     "items": [
                         "types.ModuleType",
                         {
@@ -20782,135 +20904,621 @@
                 }
             }
         },
         "getmembers": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
-                ".class": "FuncDef",
-                "abstract_status": 0,
-                "arg_kinds": [
-                    0,
-                    1
-                ],
-                "arg_names": [
-                    "object",
-                    "predicate"
-                ],
-                "dataclass_transform_spec": null,
+                ".class": "OverloadedFuncDef",
                 "flags": [],
                 "fullname": "inspect.getmembers",
-                "name": "getmembers",
+                "impl": null,
+                "items": [
+                    {
+                        ".class": "Decorator",
+                        "func": {
+                            ".class": "FuncDef",
+                            "abstract_status": 0,
+                            "arg_kinds": [
+                                0,
+                                0
+                            ],
+                            "arg_names": [
+                                "object",
+                                "predicate"
+                            ],
+                            "dataclass_transform_spec": null,
+                            "flags": [
+                                "is_overload",
+                                "is_decorated"
+                            ],
+                            "fullname": "inspect.getmembers",
+                            "name": "getmembers",
+                            "type": {
+                                ".class": "CallableType",
+                                "arg_kinds": [
+                                    0,
+                                    0
+                                ],
+                                "arg_names": [
+                                    "object",
+                                    "predicate"
+                                ],
+                                "arg_types": [
+                                    "builtins.object",
+                                    {
+                                        ".class": "TypeAliasType",
+                                        "args": [
+                                            {
+                                                ".class": "TypeVarType",
+                                                "fullname": "inspect._T",
+                                                "id": -1,
+                                                "name": "_T",
+                                                "namespace": "",
+                                                "upper_bound": "builtins.object",
+                                                "values": [],
+                                                "variance": 0
+                                            }
+                                        ],
+                                        "type_ref": "inspect._GetMembersPredicateTypeGuard"
+                                    }
+                                ],
+                                "bound_args": [],
+                                "def_extras": {
+                                    "first_arg": null
+                                },
+                                "fallback": "builtins.function",
+                                "from_concatenate": false,
+                                "implicit": false,
+                                "is_ellipsis_args": false,
+                                "name": "getmembers",
+                                "ret_type": {
+                                    ".class": "TypeAliasType",
+                                    "args": [
+                                        {
+                                            ".class": "TypeVarType",
+                                            "fullname": "inspect._T",
+                                            "id": -1,
+                                            "name": "_T",
+                                            "namespace": "",
+                                            "upper_bound": "builtins.object",
+                                            "values": [],
+                                            "variance": 0
+                                        }
+                                    ],
+                                    "type_ref": "inspect._GetMembersReturnTypeGuard"
+                                },
+                                "type_guard": null,
+                                "unpack_kwargs": false,
+                                "variables": [
+                                    {
+                                        ".class": "TypeVarType",
+                                        "fullname": "inspect._T",
+                                        "id": -1,
+                                        "name": "_T",
+                                        "namespace": "",
+                                        "upper_bound": "builtins.object",
+                                        "values": [],
+                                        "variance": 0
+                                    }
+                                ]
+                            }
+                        },
+                        "is_overload": true,
+                        "var": {
+                            ".class": "Var",
+                            "flags": [
+                                "is_inferred"
+                            ],
+                            "fullname": "inspect.getmembers",
+                            "name": "getmembers",
+                            "type": null
+                        }
+                    },
+                    {
+                        ".class": "Decorator",
+                        "func": {
+                            ".class": "FuncDef",
+                            "abstract_status": 0,
+                            "arg_kinds": [
+                                0,
+                                1
+                            ],
+                            "arg_names": [
+                                "object",
+                                "predicate"
+                            ],
+                            "dataclass_transform_spec": null,
+                            "flags": [
+                                "is_overload",
+                                "is_decorated"
+                            ],
+                            "fullname": "inspect.getmembers",
+                            "name": "getmembers",
+                            "type": {
+                                ".class": "CallableType",
+                                "arg_kinds": [
+                                    0,
+                                    1
+                                ],
+                                "arg_names": [
+                                    "object",
+                                    "predicate"
+                                ],
+                                "arg_types": [
+                                    "builtins.object",
+                                    {
+                                        ".class": "UnionType",
+                                        "items": [
+                                            {
+                                                ".class": "TypeAliasType",
+                                                "args": [],
+                                                "type_ref": "inspect._GetMembersPredicate"
+                                            },
+                                            {
+                                                ".class": "NoneType"
+                                            }
+                                        ]
+                                    }
+                                ],
+                                "bound_args": [],
+                                "def_extras": {
+                                    "first_arg": null
+                                },
+                                "fallback": "builtins.function",
+                                "from_concatenate": false,
+                                "implicit": false,
+                                "is_ellipsis_args": false,
+                                "name": "getmembers",
+                                "ret_type": {
+                                    ".class": "TypeAliasType",
+                                    "args": [],
+                                    "type_ref": "inspect._GetMembersReturn"
+                                },
+                                "type_guard": null,
+                                "unpack_kwargs": false,
+                                "variables": []
+                            }
+                        },
+                        "is_overload": true,
+                        "var": {
+                            ".class": "Var",
+                            "flags": [
+                                "is_inferred"
+                            ],
+                            "fullname": "inspect.getmembers",
+                            "name": "getmembers",
+                            "type": null
+                        }
+                    }
+                ],
                 "type": {
-                    ".class": "CallableType",
-                    "arg_kinds": [
-                        0,
-                        1
-                    ],
-                    "arg_names": [
-                        "object",
-                        "predicate"
-                    ],
-                    "arg_types": [
-                        "builtins.object",
+                    ".class": "Overloaded",
+                    "items": [
                         {
-                            ".class": "UnionType",
-                            "items": [
+                            ".class": "CallableType",
+                            "arg_kinds": [
+                                0,
+                                0
+                            ],
+                            "arg_names": [
+                                "object",
+                                "predicate"
+                            ],
+                            "arg_types": [
+                                "builtins.object",
                                 {
                                     ".class": "TypeAliasType",
-                                    "args": [],
-                                    "type_ref": "inspect._GetMembersPredicate"
-                                },
+                                    "args": [
+                                        {
+                                            ".class": "TypeVarType",
+                                            "fullname": "inspect._T",
+                                            "id": -1,
+                                            "name": "_T",
+                                            "namespace": "",
+                                            "upper_bound": "builtins.object",
+                                            "values": [],
+                                            "variance": 0
+                                        }
+                                    ],
+                                    "type_ref": "inspect._GetMembersPredicateTypeGuard"
+                                }
+                            ],
+                            "bound_args": [],
+                            "def_extras": {
+                                "first_arg": null
+                            },
+                            "fallback": "builtins.function",
+                            "from_concatenate": false,
+                            "implicit": false,
+                            "is_ellipsis_args": false,
+                            "name": "getmembers",
+                            "ret_type": {
+                                ".class": "TypeAliasType",
+                                "args": [
+                                    {
+                                        ".class": "TypeVarType",
+                                        "fullname": "inspect._T",
+                                        "id": -1,
+                                        "name": "_T",
+                                        "namespace": "",
+                                        "upper_bound": "builtins.object",
+                                        "values": [],
+                                        "variance": 0
+                                    }
+                                ],
+                                "type_ref": "inspect._GetMembersReturnTypeGuard"
+                            },
+                            "type_guard": null,
+                            "unpack_kwargs": false,
+                            "variables": [
                                 {
-                                    ".class": "NoneType"
+                                    ".class": "TypeVarType",
+                                    "fullname": "inspect._T",
+                                    "id": -1,
+                                    "name": "_T",
+                                    "namespace": "",
+                                    "upper_bound": "builtins.object",
+                                    "values": [],
+                                    "variance": 0
                                 }
                             ]
+                        },
+                        {
+                            ".class": "CallableType",
+                            "arg_kinds": [
+                                0,
+                                1
+                            ],
+                            "arg_names": [
+                                "object",
+                                "predicate"
+                            ],
+                            "arg_types": [
+                                "builtins.object",
+                                {
+                                    ".class": "UnionType",
+                                    "items": [
+                                        {
+                                            ".class": "TypeAliasType",
+                                            "args": [],
+                                            "type_ref": "inspect._GetMembersPredicate"
+                                        },
+                                        {
+                                            ".class": "NoneType"
+                                        }
+                                    ]
+                                }
+                            ],
+                            "bound_args": [],
+                            "def_extras": {
+                                "first_arg": null
+                            },
+                            "fallback": "builtins.function",
+                            "from_concatenate": false,
+                            "implicit": false,
+                            "is_ellipsis_args": false,
+                            "name": "getmembers",
+                            "ret_type": {
+                                ".class": "TypeAliasType",
+                                "args": [],
+                                "type_ref": "inspect._GetMembersReturn"
+                            },
+                            "type_guard": null,
+                            "unpack_kwargs": false,
+                            "variables": []
                         }
-                    ],
-                    "bound_args": [],
-                    "def_extras": {
-                        "first_arg": null
-                    },
-                    "fallback": "builtins.function",
-                    "from_concatenate": false,
-                    "implicit": false,
-                    "is_ellipsis_args": false,
-                    "name": "getmembers",
-                    "ret_type": {
-                        ".class": "TypeAliasType",
-                        "args": [],
-                        "type_ref": "inspect._GetMembersReturn"
-                    },
-                    "type_guard": null,
-                    "unpack_kwargs": false,
-                    "variables": []
+                    ]
                 }
             }
         },
         "getmembers_static": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
-                ".class": "FuncDef",
-                "abstract_status": 0,
-                "arg_kinds": [
-                    0,
-                    1
-                ],
-                "arg_names": [
-                    "object",
-                    "predicate"
-                ],
-                "dataclass_transform_spec": null,
+                ".class": "OverloadedFuncDef",
                 "flags": [],
                 "fullname": "inspect.getmembers_static",
-                "name": "getmembers_static",
+                "impl": null,
+                "items": [
+                    {
+                        ".class": "Decorator",
+                        "func": {
+                            ".class": "FuncDef",
+                            "abstract_status": 0,
+                            "arg_kinds": [
+                                0,
+                                0
+                            ],
+                            "arg_names": [
+                                "object",
+                                "predicate"
+                            ],
+                            "dataclass_transform_spec": null,
+                            "flags": [
+                                "is_overload",
+                                "is_decorated"
+                            ],
+                            "fullname": "inspect.getmembers_static",
+                            "name": "getmembers_static",
+                            "type": {
+                                ".class": "CallableType",
+                                "arg_kinds": [
+                                    0,
+                                    0
+                                ],
+                                "arg_names": [
+                                    "object",
+                                    "predicate"
+                                ],
+                                "arg_types": [
+                                    "builtins.object",
+                                    {
+                                        ".class": "TypeAliasType",
+                                        "args": [
+                                            {
+                                                ".class": "TypeVarType",
+                                                "fullname": "inspect._T",
+                                                "id": -1,
+                                                "name": "_T",
+                                                "namespace": "",
+                                                "upper_bound": "builtins.object",
+                                                "values": [],
+                                                "variance": 0
+                                            }
+                                        ],
+                                        "type_ref": "inspect._GetMembersPredicateTypeGuard"
+                                    }
+                                ],
+                                "bound_args": [],
+                                "def_extras": {
+                                    "first_arg": null
+                                },
+                                "fallback": "builtins.function",
+                                "from_concatenate": false,
+                                "implicit": false,
+                                "is_ellipsis_args": false,
+                                "name": "getmembers_static",
+                                "ret_type": {
+                                    ".class": "TypeAliasType",
+                                    "args": [
+                                        {
+                                            ".class": "TypeVarType",
+                                            "fullname": "inspect._T",
+                                            "id": -1,
+                                            "name": "_T",
+                                            "namespace": "",
+                                            "upper_bound": "builtins.object",
+                                            "values": [],
+                                            "variance": 0
+                                        }
+                                    ],
+                                    "type_ref": "inspect._GetMembersReturnTypeGuard"
+                                },
+                                "type_guard": null,
+                                "unpack_kwargs": false,
+                                "variables": [
+                                    {
+                                        ".class": "TypeVarType",
+                                        "fullname": "inspect._T",
+                                        "id": -1,
+                                        "name": "_T",
+                                        "namespace": "",
+                                        "upper_bound": "builtins.object",
+                                        "values": [],
+                                        "variance": 0
+                                    }
+                                ]
+                            }
+                        },
+                        "is_overload": true,
+                        "var": {
+                            ".class": "Var",
+                            "flags": [
+                                "is_inferred"
+                            ],
+                            "fullname": "inspect.getmembers_static",
+                            "name": "getmembers_static",
+                            "type": null
+                        }
+                    },
+                    {
+                        ".class": "Decorator",
+                        "func": {
+                            ".class": "FuncDef",
+                            "abstract_status": 0,
+                            "arg_kinds": [
+                                0,
+                                1
+                            ],
+                            "arg_names": [
+                                "object",
+                                "predicate"
+                            ],
+                            "dataclass_transform_spec": null,
+                            "flags": [
+                                "is_overload",
+                                "is_decorated"
+                            ],
+                            "fullname": "inspect.getmembers_static",
+                            "name": "getmembers_static",
+                            "type": {
+                                ".class": "CallableType",
+                                "arg_kinds": [
+                                    0,
+                                    1
+                                ],
+                                "arg_names": [
+                                    "object",
+                                    "predicate"
+                                ],
+                                "arg_types": [
+                                    "builtins.object",
+                                    {
+                                        ".class": "UnionType",
+                                        "items": [
+                                            {
+                                                ".class": "TypeAliasType",
+                                                "args": [],
+                                                "type_ref": "inspect._GetMembersPredicate"
+                                            },
+                                            {
+                                                ".class": "NoneType"
+                                            }
+                                        ]
+                                    }
+                                ],
+                                "bound_args": [],
+                                "def_extras": {
+                                    "first_arg": null
+                                },
+                                "fallback": "builtins.function",
+                                "from_concatenate": false,
+                                "implicit": false,
+                                "is_ellipsis_args": false,
+                                "name": "getmembers_static",
+                                "ret_type": {
+                                    ".class": "TypeAliasType",
+                                    "args": [],
+                                    "type_ref": "inspect._GetMembersReturn"
+                                },
+                                "type_guard": null,
+                                "unpack_kwargs": false,
+                                "variables": []
+                            }
+                        },
+                        "is_overload": true,
+                        "var": {
+                            ".class": "Var",
+                            "flags": [
+                                "is_inferred"
+                            ],
+                            "fullname": "inspect.getmembers_static",
+                            "name": "getmembers_static",
+                            "type": null
+                        }
+                    }
+                ],
                 "type": {
-                    ".class": "CallableType",
-                    "arg_kinds": [
-                        0,
-                        1
-                    ],
-                    "arg_names": [
-                        "object",
-                        "predicate"
-                    ],
-                    "arg_types": [
-                        "builtins.object",
+                    ".class": "Overloaded",
+                    "items": [
                         {
-                            ".class": "UnionType",
-                            "items": [
+                            ".class": "CallableType",
+                            "arg_kinds": [
+                                0,
+                                0
+                            ],
+                            "arg_names": [
+                                "object",
+                                "predicate"
+                            ],
+                            "arg_types": [
+                                "builtins.object",
                                 {
                                     ".class": "TypeAliasType",
-                                    "args": [],
-                                    "type_ref": "inspect._GetMembersPredicate"
-                                },
+                                    "args": [
+                                        {
+                                            ".class": "TypeVarType",
+                                            "fullname": "inspect._T",
+                                            "id": -1,
+                                            "name": "_T",
+                                            "namespace": "",
+                                            "upper_bound": "builtins.object",
+                                            "values": [],
+                                            "variance": 0
+                                        }
+                                    ],
+                                    "type_ref": "inspect._GetMembersPredicateTypeGuard"
+                                }
+                            ],
+                            "bound_args": [],
+                            "def_extras": {
+                                "first_arg": null
+                            },
+                            "fallback": "builtins.function",
+                            "from_concatenate": false,
+                            "implicit": false,
+                            "is_ellipsis_args": false,
+                            "name": "getmembers_static",
+                            "ret_type": {
+                                ".class": "TypeAliasType",
+                                "args": [
+                                    {
+                                        ".class": "TypeVarType",
+                                        "fullname": "inspect._T",
+                                        "id": -1,
+                                        "name": "_T",
+                                        "namespace": "",
+                                        "upper_bound": "builtins.object",
+                                        "values": [],
+                                        "variance": 0
+                                    }
+                                ],
+                                "type_ref": "inspect._GetMembersReturnTypeGuard"
+                            },
+                            "type_guard": null,
+                            "unpack_kwargs": false,
+                            "variables": [
                                 {
-                                    ".class": "NoneType"
+                                    ".class": "TypeVarType",
+                                    "fullname": "inspect._T",
+                                    "id": -1,
+                                    "name": "_T",
+                                    "namespace": "",
+                                    "upper_bound": "builtins.object",
+                                    "values": [],
+                                    "variance": 0
                                 }
                             ]
+                        },
+                        {
+                            ".class": "CallableType",
+                            "arg_kinds": [
+                                0,
+                                1
+                            ],
+                            "arg_names": [
+                                "object",
+                                "predicate"
+                            ],
+                            "arg_types": [
+                                "builtins.object",
+                                {
+                                    ".class": "UnionType",
+                                    "items": [
+                                        {
+                                            ".class": "TypeAliasType",
+                                            "args": [],
+                                            "type_ref": "inspect._GetMembersPredicate"
+                                        },
+                                        {
+                                            ".class": "NoneType"
+                                        }
+                                    ]
+                                }
+                            ],
+                            "bound_args": [],
+                            "def_extras": {
+                                "first_arg": null
+                            },
+                            "fallback": "builtins.function",
+                            "from_concatenate": false,
+                            "implicit": false,
+                            "is_ellipsis_args": false,
+                            "name": "getmembers_static",
+                            "ret_type": {
+                                ".class": "TypeAliasType",
+                                "args": [],
+                                "type_ref": "inspect._GetMembersReturn"
+                            },
+                            "type_guard": null,
+                            "unpack_kwargs": false,
+                            "variables": []
                         }
-                    ],
-                    "bound_args": [],
-                    "def_extras": {
-                        "first_arg": null
-                    },
-                    "fallback": "builtins.function",
-                    "from_concatenate": false,
-                    "implicit": false,
-                    "is_ellipsis_args": false,
-                    "name": "getmembers_static",
-                    "ret_type": {
-                        ".class": "TypeAliasType",
-                        "args": [],
-                        "type_ref": "inspect._GetMembersReturn"
-                    },
-                    "type_guard": null,
-                    "unpack_kwargs": false,
-                    "variables": []
+                    ]
                 }
             }
         },
         "getmodule": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/inspect.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/sre_parse.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6928404928404928%*

 * *Differences: {"'data_mtime'": '1683843439',*

 * * "'dep_lines'": '{insert: [(1, 1), (4, 6), (5, 7)], delete: [7, 6, 5, 1, 0]}',*

 * * "'dep_prios'": '{delete: [2, 1]}',*

 * * "'dependencies'": "{insert: [(2, 're'), (3, 'sre_constants')], delete: [5, 4, 2, 1]}",*

 * * "'hash'": "'38b6a819e544b584ec71b7040293fae6a77f2447fc14e9bc70e752ec237c8022'",*

 * * "'id'": "'sre_parse'",*

 * * "'interface_hash'": "'f5b5305584ba71c58843130ee41dcb142383ee5c147b1f177f4029bfd99b1751'",*

 * * "'mtime'": '1684623296',*

 * * "'path'": "'/home/gotmax/Sync/git-repos/packaging/fedor […]*

```diff
@@ -1,53 +1,47 @@
 {
-    "data_mtime": 1681571164,
+    "data_mtime": 1683843439,
     "dep_lines": [
-        6,
-        1,
         2,
+        1,
         3,
         4,
-        5,
-        27,
-        28,
+        6,
+        7,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
         10,
-        10,
-        10,
         5,
         5,
         5,
         5,
         5,
         30,
         30
     ],
     "dependencies": [
         "collections.abc",
-        "dis",
-        "enum",
         "sys",
-        "types",
-        "collections",
+        "re",
+        "sre_constants",
         "typing",
         "typing_extensions",
         "builtins",
         "_typeshed",
         "abc"
     ],
-    "hash": "7fbbe4f5f1d1280df9c32c8924d222b540e433476cf280205ba60f3f335ed250",
-    "id": "inspect",
+    "hash": "38b6a819e544b584ec71b7040293fae6a77f2447fc14e9bc70e752ec237c8022",
+    "id": "sre_parse",
     "ignore_all": true,
-    "interface_hash": "dfdb109fce48041fa301c8d50697d94cbd390bfc9ff3735b285929067edd087d",
-    "mtime": 1683082840,
+    "interface_hash": "f5b5305584ba71c58843130ee41dcb142383ee5c147b1f177f4029bfd99b1751",
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -81,13 +75,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/inspect.pyi",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/sre_parse.pyi",
     "plugin_data": null,
-    "size": 19505,
+    "size": 4069,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/io.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/io.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/io.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/codecs.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7033333333333334%*

 * *Differences: {"'data_mtime'": '1683843440',*

 * * "'dep_lines'": '{insert: [(8, 1)], delete: [9, 8]}',*

 * * "'dep_prios'": '{insert: [(3, 5)], delete: [2, 1]}',*

 * * "'dependencies'": "{insert: [(3, '_codecs'), (4, '_typeshed'), (5, 'abc'), (8, 'builtins')], "*

 * *                   'delete: [6, 5, 3, 2, 1]}',*

 * * "'hash'": "'abcdbf8e98a1d1dcc78b663b26b2c59e461cc46b1fc60fda37f079266e35df68'",*

 * * "'id'": "'codecs'",*

 * * "'interface_hash'": "'0fdf421732626f3c5bf22599d383a7f8eaafb8be02a4922f990ddf72739abf68'",*

 * * "'mtime'": '1684623296',*

 * * "'path'":  […]*

```diff
@@ -1,62 +1,59 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843440,
     "dep_lines": [
         6,
         1,
         2,
         3,
         4,
         5,
         7,
         8,
-        9,
-        10,
+        1,
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
         10,
         10,
-        10,
-        10,
+        5,
         5,
         5,
         5,
         5,
         5,
         30,
         30,
         30,
         30
     ],
     "dependencies": [
         "collections.abc",
-        "abc",
-        "builtins",
-        "codecs",
         "sys",
-        "_typeshed",
-        "os",
         "types",
+        "_codecs",
+        "_typeshed",
+        "abc",
         "typing",
         "typing_extensions",
+        "builtins",
         "array",
         "ctypes",
         "mmap",
         "pickle"
     ],
-    "hash": "0b41ad24faa49ac20e0c8c0d0bf223ff7de8ce8ea44fe01e3a4a2cb1f363054d",
-    "id": "io",
+    "hash": "abcdbf8e98a1d1dcc78b663b26b2c59e461cc46b1fc60fda37f079266e35df68",
+    "id": "codecs",
     "ignore_all": true,
-    "interface_hash": "d56edaef4812437216957ff6b311c183e73e734608323734beeea8c56b340db8",
-    "mtime": 1683082840,
+    "interface_hash": "0fdf421732626f3c5bf22599d383a7f8eaafb8be02a4922f990ddf72739abf68",
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -90,13 +87,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/io.pyi",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/codecs.pyi",
     "plugin_data": null,
-    "size": 7875,
+    "size": 11984,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/itertools.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/itertools.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/itertools.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/importlib/metadata/_meta.meta.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6777777777777778%*

 * *Differences: {"'data_mtime'": '1683843440',*

 * * "'dep_lines'": '{insert: [(1, 2)], delete: [4, 3, 2, 1, 0]}',*

 * * "'dep_prios'": '{delete: [6, 2, 1, 0]}',*

 * * "'dependencies'": '{delete: [6, 4, 3, 1]}',*

 * * "'hash'": "'2be6b67f68a873ae65d787d3f698fdaf7871860828243a5e6d747d1305c5ffa4'",*

 * * "'id'": "'importlib.metadata._meta'",*

 * * "'interface_hash'": "'1db704b0286cfe333cd9435e9f98ea264d93b92ffc6067f47c05700759a0233d'",*

 * * "'mtime'": '1684623296',*

 * * "'path'": "'/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/py […]*

```diff
@@ -1,44 +1,32 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843440,
     "dep_lines": [
-        2,
-        1,
-        3,
-        4,
-        7,
         1,
+        2,
         1,
         1
     ],
     "dep_prios": [
         5,
-        10,
-        5,
-        5,
         5,
         5,
-        30,
         30
     ],
     "dependencies": [
         "collections.abc",
-        "sys",
         "typing",
-        "typing_extensions",
-        "types",
         "builtins",
-        "_typeshed",
         "abc"
     ],
-    "hash": "8d452d6d11a70ac8cf92f7f8ca2f0ec391f06ffd520b0a5e9c6083b3efe75b5d",
-    "id": "itertools",
+    "hash": "2be6b67f68a873ae65d787d3f698fdaf7871860828243a5e6d747d1305c5ffa4",
+    "id": "importlib.metadata._meta",
     "ignore_all": true,
-    "interface_hash": "f44c52f578278b7de5867c5634921ea0a2a1c43a005a6874f20464d46cd5ebd3",
-    "mtime": 1683082840,
+    "interface_hash": "1db704b0286cfe333cd9435e9f98ea264d93b92ffc6067f47c05700759a0233d",
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -72,13 +60,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/itertools.pyi",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/importlib/metadata/_meta.pyi",
     "plugin_data": null,
-    "size": 10908,
+    "size": 842,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/math.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/math.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/math.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/inspect.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6924242424242425%*

 * *Differences: {"'data_mtime'": '1683843440',*

 * * "'dep_lines'": '{insert: [(0, 6), (2, 2), (5, 5), (6, 27), (7, 28)], delete: [0]}',*

 * * "'dep_prios'": '{insert: [(1, 10), (2, 10), (4, 5), (5, 5)]}',*

 * * "'dependencies'": "{insert: [(1, 'dis'), (2, 'enum'), (4, 'types'), (5, 'collections')]}",*

 * * "'hash'": "'9b9bc26634b9323492d1abe333418ad1bb84b2bd41bf161b538d0202abb34d8f'",*

 * * "'id'": "'inspect'",*

 * * "'interface_hash'": "'2d65050e11afcc6331e0513e0c37216d1a7cf73c9de70864cc174fcbce7aaa22'",*

 * * "'mtime'": '1684623296',*

 * * "'path'": "'/home/g […]*

```diff
@@ -1,41 +1,53 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843440,
     "dep_lines": [
-        2,
+        6,
         1,
+        2,
         3,
         4,
+        5,
+        27,
+        28,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
         10,
+        10,
+        10,
+        5,
+        5,
         5,
         5,
         5,
         30,
         30
     ],
     "dependencies": [
         "collections.abc",
+        "dis",
+        "enum",
         "sys",
+        "types",
+        "collections",
         "typing",
         "typing_extensions",
         "builtins",
         "_typeshed",
         "abc"
     ],
-    "hash": "7383fb2c7e3a74ef80504a0d82a06ed95c4c7754272c54e89a64f1319ab87732",
-    "id": "math",
+    "hash": "9b9bc26634b9323492d1abe333418ad1bb84b2bd41bf161b538d0202abb34d8f",
+    "id": "inspect",
     "ignore_all": true,
-    "interface_hash": "97da52b3476c6652bbedd6e0becfa77cc03d1db9c6f3ac24e112b7acebd5aa9a",
-    "mtime": 1683082840,
+    "interface_hash": "2d65050e11afcc6331e0513e0c37216d1a7cf73c9de70864cc174fcbce7aaa22",
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -69,13 +81,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/math.pyi",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/inspect.pyi",
     "plugin_data": null,
-    "size": 5025,
+    "size": 19928,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/mmap.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/mmap.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/mmap.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/glob.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6933333333333332%*

 * *Differences: {"'data_mtime'": '1683843440',*

 * * "'dep_lines'": '{delete: [7, 6, 5, 4]}',*

 * * "'dep_prios'": '{delete: [8, 7, 6, 2]}',*

 * * "'dependencies'": '{delete: [9, 8, 7, 4]}',*

 * * "'hash'": "'b23877cf7cc743ec86f6a87b449a4cc1a92ad72e573a19c7a17a82c3fc3507a2'",*

 * * "'id'": "'glob'",*

 * * "'interface_hash'": "'266e5d53c08178ba44335144c11737885af67ee5e9dc75a2aebc95df4df21509'",*

 * * "'mtime'": '1684623296',*

 * * "'path'": "'/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdl […]*

```diff
@@ -1,50 +1,38 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843440,
     "dep_lines": [
         3,
         1,
         2,
         4,
-        5,
-        1,
-        1,
-        1,
         1,
         1
     ],
     "dep_prios": [
         5,
         10,
         5,
         5,
         5,
-        5,
-        30,
-        30,
-        30,
         30
     ],
     "dependencies": [
         "collections.abc",
         "sys",
         "_typeshed",
         "typing",
-        "typing_extensions",
         "builtins",
-        "abc",
-        "array",
-        "ctypes",
-        "pickle"
+        "abc"
     ],
-    "hash": "d9e78f0946bc6297002b245e9d85b5be1bcfe36b9a503843f57923c1574200ea",
-    "id": "mmap",
+    "hash": "b23877cf7cc743ec86f6a87b449a4cc1a92ad72e573a19c7a17a82c3fc3507a2",
+    "id": "glob",
     "ignore_all": true,
-    "interface_hash": "50e1b41dc66c18ca281b637d2fc764f5c44a55824c90ed2c0e3bacd97b1f67d2",
-    "mtime": 1683082840,
+    "interface_hash": "266e5d53c08178ba44335144c11737885af67ee5e9dc75a2aebc95df4df21509",
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -78,13 +66,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/mmap.pyi",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/glob.pyi",
     "plugin_data": null,
-    "size": 4009,
+    "size": 1421,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/msvcrt.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/msvcrt.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/msvcrt.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/tty.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7%*

 * *Differences: {"'data_mtime'": '1683843440',*

 * * "'dep_lines'": '{insert: [(2, 3)], delete: [2]}',*

 * * "'dep_prios'": '{insert: [(3, 5)], delete: [3]}',*

 * * "'dependencies'": "{insert: [(1, 'typing')], delete: [4]}",*

 * * "'hash'": "'93eadd2f4010b8e595f7f4af4efc698bd6d7a8fe571bfad7e90078f8fdaf26f8'",*

 * * "'id'": "'tty'",*

 * * "'interface_hash'": "'27ec90732677bd7784fffab768dfef3cbd0c62398fce4a10dcde646616f7bd42'",*

 * * "'mtime'": '1684623296',*

 * * "'path'": "'/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11 […]*

```diff
@@ -1,35 +1,35 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843440,
     "dep_lines": [
         1,
         2,
-        1,
+        3,
         1,
         1
     ],
     "dep_prios": [
         10,
         5,
         5,
-        30,
+        5,
         30
     ],
     "dependencies": [
         "sys",
+        "typing",
         "typing_extensions",
         "builtins",
-        "abc",
-        "typing"
+        "abc"
     ],
-    "hash": "d4a762dc87ddb7286da0abdb399dec04efb82a19579a4ef11af621851da7b598",
-    "id": "msvcrt",
+    "hash": "93eadd2f4010b8e595f7f4af4efc698bd6d7a8fe571bfad7e90078f8fdaf26f8",
+    "id": "tty",
     "ignore_all": true,
-    "interface_hash": "71abd058cd942a211c31935f165761a99d332719aaa55402e1adc032384a33d2",
-    "mtime": 1683082840,
+    "interface_hash": "27ec90732677bd7784fffab768dfef3cbd0c62398fce4a10dcde646616f7bd42",
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -63,13 +63,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/msvcrt.pyi",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/tty.pyi",
     "plugin_data": null,
-    "size": 995,
+    "size": 430,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/numbers.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/numbers.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/numbers.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/numbers.meta.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'data_mtime'": '1683843440', "'mtime'": '1684623296', "'version_id'": "'1.3.0'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843440,
     "dep_lines": [
         4,
         5,
         1
     ],
     "dep_prios": [
         5,
@@ -15,15 +15,15 @@
         "typing",
         "builtins"
     ],
     "hash": "aa29ea52bc87c75f589211fa38294e2cc1bc735c97f4fa331ebaff28e5f2cb84",
     "id": "numbers",
     "ignore_all": true,
     "interface_hash": "a2f34266cc1748dd3c1c47d9e60f3115834146c69acd372559a6cb5cc500fb1c",
-    "mtime": 1683082840,
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -61,9 +61,9 @@
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
     "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/numbers.pyi",
     "plugin_data": null,
     "size": 3914,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/opcode.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/opcode.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/opcode.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/opcode.meta.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'data_mtime'": '1683843440', "'mtime'": '1684623296', "'version_id'": "'1.3.0'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843440,
     "dep_lines": [
         1,
         2,
         1,
         1,
         1,
         1
@@ -24,15 +24,15 @@
         "abc",
         "typing"
     ],
     "hash": "59c0a8b72408537be5d42d12987309aac4a2d17dc740d1d3c2d88732320749e1",
     "id": "opcode",
     "ignore_all": true,
     "interface_hash": "8d01b9e08cec8de32da3ca4e41d16a9fd8aae89f2b8a0b907ccf63cc69bd7bb0",
-    "mtime": 1683082840,
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -70,9 +70,9 @@
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
     "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/opcode.pyi",
     "plugin_data": null,
     "size": 1231,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/operator.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/operator.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/operator.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/operator.meta.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'data_mtime'": '1683843440', "'mtime'": '1684623296', "'version_id'": "'1.3.0'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843440,
     "dep_lines": [
         1,
         2,
         1,
         1,
         1,
         1,
@@ -27,15 +27,15 @@
         "typing",
         "typing_extensions"
     ],
     "hash": "b5874dad84073d6251c60f2da6aded0683c8cf18d7369e3f606cd1787d383625",
     "id": "operator",
     "ignore_all": true,
     "interface_hash": "190d35158dfbd6595108293705a83748397719085e646d5ecf89dba96354f927",
-    "mtime": 1683082840,
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -73,9 +73,9 @@
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
     "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/operator.pyi",
     "plugin_data": null,
     "size": 1644,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/pathlib.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/pathlib.data.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999999999913655%*

 * *Differences: {"'names'": "{'Path': {'node': {'names': {'hardlink_to': {'node': {'type': {'arg_types': {1: "*

 * *            "{'.class': 'TypeAliasType', 'args': [], 'type_ref': '_typeshed.StrOrBytesPath', "*

 * *            "delete: ['items']}}}}}, 'symlink_to': {'node': {'type': {'arg_types': {1: {'.class': "*

 * *            "'TypeAliasType', 'args': [], 'type_ref': '_typeshed.StrOrBytesPath', delete: "*

 * *            "['items']}}}}}}}}}"}*

```diff
@@ -963,19 +963,17 @@
                                 "arg_names": [
                                     "self",
                                     "target"
                                 ],
                                 "arg_types": [
                                     "pathlib.Path",
                                     {
-                                        ".class": "UnionType",
-                                        "items": [
-                                            "builtins.str",
-                                            "pathlib.Path"
-                                        ]
+                                        ".class": "TypeAliasType",
+                                        "args": [],
+                                        "type_ref": "_typeshed.StrOrBytesPath"
                                     }
                                 ],
                                 "bound_args": [],
                                 "def_extras": {
                                     "first_arg": "self"
                                 },
                                 "fallback": "builtins.function",
@@ -3695,19 +3693,17 @@
                                     "self",
                                     "target",
                                     "target_is_directory"
                                 ],
                                 "arg_types": [
                                     "pathlib.Path",
                                     {
-                                        ".class": "UnionType",
-                                        "items": [
-                                            "builtins.str",
-                                            "pathlib.Path"
-                                        ]
+                                        ".class": "TypeAliasType",
+                                        "args": [],
+                                        "type_ref": "_typeshed.StrOrBytesPath"
                                     },
                                     "builtins.bool"
                                 ],
                                 "bound_args": [],
                                 "def_extras": {
                                     "first_arg": "self"
                                 },
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/pathlib.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/io.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6855614973262032%*

 * *Differences: {"'data_mtime'": '1683843440',*

 * * "'dep_lines'": '{insert: [(0, 6), (3, 3), (4, 4), (5, 5), (6, 7), (7, 8), (8, 9), (9, 10)], '*

 * *                'delete: [9, 8, 7, 6, 5, 4, 3, 0]}',*

 * * "'dep_prios'": '{insert: [(2, 10), (3, 10), (4, 10)], delete: [9, 3, 2]}',*

 * * "'dependencies'": "{insert: [(1, 'abc'), (2, 'builtins'), (3, 'codecs')], delete: [9, 8, 3]}",*

 * * "'hash'": "'0b41ad24faa49ac20e0c8c0d0bf223ff7de8ce8ea44fe01e3a4a2cb1f363054d'",*

 * * "'id'": "'io'",*

 * * "'interface_hash'": "'d56edaef4812437216957ff6b311c183e73e7346 […]*

```diff
@@ -1,62 +1,62 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843440,
     "dep_lines": [
-        12,
+        6,
         1,
         2,
-        13,
-        14,
-        15,
-        16,
-        17,
-        1,
-        1,
+        3,
+        4,
+        5,
+        7,
+        8,
+        9,
+        10,
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
         10,
-        5,
-        5,
+        10,
+        10,
+        10,
         5,
         5,
         5,
         5,
         5,
         30,
         30,
         30,
-        30,
         30
     ],
     "dependencies": [
         "collections.abc",
+        "abc",
+        "builtins",
+        "codecs",
         "sys",
         "_typeshed",
-        "io",
         "os",
         "types",
         "typing",
         "typing_extensions",
-        "builtins",
-        "abc",
         "array",
         "ctypes",
         "mmap",
         "pickle"
     ],
-    "hash": "04a9e436986cd9b24089af97b33a4ce12d691429398e3de21b63d203baa68ccf",
-    "id": "pathlib",
+    "hash": "0b41ad24faa49ac20e0c8c0d0bf223ff7de8ce8ea44fe01e3a4a2cb1f363054d",
+    "id": "io",
     "ignore_all": true,
-    "interface_hash": "c19b5166a41fd36d275b1fd3e461934c6838b8aabff55b137464e78ab7bda865",
-    "mtime": 1683082840,
+    "interface_hash": "d56edaef4812437216957ff6b311c183e73e734608323734beeea8c56b340db8",
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -90,13 +90,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/pathlib.pyi",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/io.pyi",
     "plugin_data": null,
-    "size": 7941,
+    "size": 7875,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/pickle.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/pickle.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/pickle.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/time.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6884848484848486%*

 * *Differences: {"'data_mtime'": '1683843440',*

 * * "'dep_lines'": '{insert: [(2, 3)], delete: [7, 6, 5, 4, 0]}',*

 * * "'dep_prios'": '{delete: [8, 7, 6, 0]}',*

 * * "'dependencies'": '{delete: [9, 8, 7, 0]}',*

 * * "'hash'": "'81ee1e52c98cc1cd26d7a6aa6d5a9c23d100b4e14cdd725b405a720187e41f8c'",*

 * * "'id'": "'time'",*

 * * "'interface_hash'": "'1cbf1127c399d86b63dab8b6f2658b55c520340ebda63950277141e8cdddc99e'",*

 * * "'mtime'": '1684623296',*

 * * "'path'": "'/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packag […]*

```diff
@@ -1,50 +1,38 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843440,
     "dep_lines": [
-        3,
         1,
         2,
+        3,
         4,
-        5,
-        1,
-        1,
-        1,
         1,
         1
     ],
     "dep_prios": [
-        5,
         10,
         5,
         5,
         5,
         5,
-        30,
-        30,
-        30,
         30
     ],
     "dependencies": [
-        "collections.abc",
         "sys",
         "_typeshed",
         "typing",
         "typing_extensions",
         "builtins",
-        "abc",
-        "array",
-        "ctypes",
-        "mmap"
+        "abc"
     ],
-    "hash": "6fded61e7405957711fd339ce4f5b97a3204216f1028cc18fed5ade352fa755d",
-    "id": "pickle",
+    "hash": "81ee1e52c98cc1cd26d7a6aa6d5a9c23d100b4e14cdd725b405a720187e41f8c",
+    "id": "time",
     "ignore_all": true,
-    "interface_hash": "46f362cf2b7503f02d7928b6b9a37e40f1d22ab9d8eef01a9038db8667ca7609",
-    "mtime": 1683082840,
+    "interface_hash": "1cbf1127c399d86b63dab8b6f2658b55c520340ebda63950277141e8cdddc99e",
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -78,13 +66,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/pickle.pyi",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/time.pyi",
     "plugin_data": null,
-    "size": 6766,
+    "size": 3663,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/posixpath.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/posixpath.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/posixpath.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/posixpath.meta.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'data_mtime'": '1683843439', "'mtime'": '1684623296', "'version_id'": "'1.3.0'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843439,
     "dep_lines": [
         3,
         1,
         2,
         4,
         17,
         18,
@@ -33,15 +33,15 @@
         "builtins",
         "abc"
     ],
     "hash": "e29af0b8d907ad14fb6a1be8ff951377d80ecca2f14c39f13e7d9b0b5727e530",
     "id": "posixpath",
     "ignore_all": true,
     "interface_hash": "b2433e2b9b3d24b7e5e5275fdeb002d7520c2b8614f794b3fc9d2e4bf3f4f950",
-    "mtime": 1683082840,
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -79,9 +79,9 @@
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
     "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/posixpath.pyi",
     "plugin_data": null,
     "size": 4270,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/random.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/random.data.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999951294636994%*

 * *Differences: {"'names'": "{'_inst': {'node': {'flags': {delete: [1]}}}, 'choice': {'node': {'type': "*

 * *            "{'arg_types': {0: {'args': {0: {'id': 748}}}}, 'ret_type': {'id': 748}, 'variables': "*

 * *            "{0: {'id': 748}}}}}, 'choices': {'node': {'type': {'arg_types': {0: {'args': {0: "*

 * *            "{'id': 750}}}}, 'ret_type': {'args': {0: {'id': 750}}}, 'variables': {0: {'id': "*

 * *            "750}}}}}, 'sample': {'node': {'type': {'arg_types': {0: {'args': {0: {'id': 749}}}}, "*

 * *            "'ret_type': {'args' […]*

```diff
@@ -1871,16 +1871,15 @@
         "_inst": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "module_public": false,
             "node": {
                 ".class": "Var",
                 "flags": [
-                    "is_ready",
-                    "has_explicit_value"
+                    "is_ready"
                 ],
                 "fullname": "random._inst",
                 "name": "_inst",
                 "type": "random.Random"
             }
         },
         "_random": {
@@ -1955,15 +1954,15 @@
                     "arg_types": [
                         {
                             ".class": "Instance",
                             "args": [
                                 {
                                     ".class": "TypeVarType",
                                     "fullname": "random._T",
-                                    "id": 237,
+                                    "id": 748,
                                     "name": "_T",
                                     "namespace": "",
                                     "upper_bound": "builtins.object",
                                     "values": [],
                                     "variance": 0
                                 }
                             ],
@@ -1980,28 +1979,28 @@
                     "from_concatenate": false,
                     "implicit": false,
                     "is_ellipsis_args": false,
                     "name": null,
                     "ret_type": {
                         ".class": "TypeVarType",
                         "fullname": "random._T",
-                        "id": 237,
+                        "id": 748,
                         "name": "_T",
                         "namespace": "",
                         "upper_bound": "builtins.object",
                         "values": [],
                         "variance": 0
                     },
                     "type_guard": null,
                     "unpack_kwargs": false,
                     "variables": [
                         {
                             ".class": "TypeVarType",
                             "fullname": "random._T",
-                            "id": 237,
+                            "id": 748,
                             "name": "_T",
                             "namespace": "",
                             "upper_bound": "builtins.object",
                             "values": [],
                             "variance": 0
                         }
                     ]
@@ -2036,15 +2035,15 @@
                     "arg_types": [
                         {
                             ".class": "Instance",
                             "args": [
                                 {
                                     ".class": "TypeVarType",
                                     "fullname": "random._T",
-                                    "id": 239,
+                                    "id": 750,
                                     "name": "_T",
                                     "namespace": "",
                                     "upper_bound": "builtins.object",
                                     "values": [],
                                     "variance": 0
                                 }
                             ],
@@ -2107,15 +2106,15 @@
                     "name": null,
                     "ret_type": {
                         ".class": "Instance",
                         "args": [
                             {
                                 ".class": "TypeVarType",
                                 "fullname": "random._T",
-                                "id": 239,
+                                "id": 750,
                                 "name": "_T",
                                 "namespace": "",
                                 "upper_bound": "builtins.object",
                                 "values": [],
                                 "variance": 0
                             }
                         ],
@@ -2123,15 +2122,15 @@
                     },
                     "type_guard": null,
                     "unpack_kwargs": false,
                     "variables": [
                         {
                             ".class": "TypeVarType",
                             "fullname": "random._T",
-                            "id": 239,
+                            "id": 750,
                             "name": "_T",
                             "namespace": "",
                             "upper_bound": "builtins.object",
                             "values": [],
                             "variance": 0
                         }
                     ]
@@ -2672,15 +2671,15 @@
                     "arg_types": [
                         {
                             ".class": "Instance",
                             "args": [
                                 {
                                     ".class": "TypeVarType",
                                     "fullname": "random._T",
-                                    "id": 238,
+                                    "id": 749,
                                     "name": "_T",
                                     "namespace": "",
                                     "upper_bound": "builtins.object",
                                     "values": [],
                                     "variance": 0
                                 }
                             ],
@@ -2716,15 +2715,15 @@
                     "name": null,
                     "ret_type": {
                         ".class": "Instance",
                         "args": [
                             {
                                 ".class": "TypeVarType",
                                 "fullname": "random._T",
-                                "id": 238,
+                                "id": 749,
                                 "name": "_T",
                                 "namespace": "",
                                 "upper_bound": "builtins.object",
                                 "values": [],
                                 "variance": 0
                             }
                         ],
@@ -2732,15 +2731,15 @@
                     },
                     "type_guard": null,
                     "unpack_kwargs": false,
                     "variables": [
                         {
                             ".class": "TypeVarType",
                             "fullname": "random._T",
-                            "id": 238,
+                            "id": 749,
                             "name": "_T",
                             "namespace": "",
                             "upper_bound": "builtins.object",
                             "values": [],
                             "variance": 0
                         }
                     ]
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/random.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/stat.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6690235690235691%*

 * *Differences: {"'data_mtime'": '1683843440',*

 * * "'dep_lines'": '{delete: [5, 4, 3, 2, 0]}',*

 * * "'dep_prios'": '{delete: [4, 3, 2, 1, 0]}',*

 * * "'dependencies'": "{insert: [(0, '_stat'), (3, 'typing')], delete: [8, 5, 4, 3, 2, 1, 0]}",*

 * * "'hash'": "'1fd817ee6e4326df5c4f9878c64dc9c080c05437734adfdc1dfa1e546fc1d8aa'",*

 * * "'id'": "'stat'",*

 * * "'interface_hash'": "'1b3706b64ab100789d464059bc54ddbff999417b9d38e3a3e6f62cd0eee4c0a9'",*

 * * "'mtime'": '1684623296',*

 * * "'path'": "'/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/ty […]*

```diff
@@ -1,47 +1,32 @@
 {
-    "data_mtime": 1681571164,
+    "data_mtime": 1683843440,
     "dep_lines": [
-        4,
         1,
-        2,
-        3,
-        5,
-        6,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
-        10,
-        10,
-        5,
-        5,
-        5,
         5,
         30,
         30
     ],
     "dependencies": [
-        "collections.abc",
-        "_random",
-        "sys",
-        "_typeshed",
-        "fractions",
-        "typing",
+        "_stat",
         "builtins",
         "abc",
-        "numbers"
+        "typing"
     ],
-    "hash": "4150f6064948349145e44742cf86b1d00ced19d7ca150ea07a18496afbec1f48",
-    "id": "random",
+    "hash": "1fd817ee6e4326df5c4f9878c64dc9c080c05437734adfdc1dfa1e546fc1d8aa",
+    "id": "stat",
     "ignore_all": true,
-    "interface_hash": "9756fcdcb85c76b37ee6eedee06c88b5992fa6b9aabd8682f0c8cfac7d90194c",
-    "mtime": 1683082840,
+    "interface_hash": "1b3706b64ab100789d464059bc54ddbff999417b9d38e3a3e6f62cd0eee4c0a9",
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -75,13 +60,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/random.pyi",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/stat.pyi",
     "plugin_data": null,
-    "size": 4686,
+    "size": 20,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/re.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/re.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/re.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/re.meta.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'data_mtime'": '1683843439', "'mtime'": '1684623296', "'version_id'": "'1.3.0'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843439,
     "dep_lines": [
         5,
         1,
         2,
         3,
         4,
         6,
@@ -51,15 +51,15 @@
         "mmap",
         "pickle"
     ],
     "hash": "6628a0287263a0a91b274aea7dce328361b557f6249454c8f92f79af56500fbe",
     "id": "re",
     "ignore_all": true,
     "interface_hash": "8a0a850cb0ecc643a8090101b75d81e2e7801fb41785da41e29c93dcef04e110",
-    "mtime": 1683082840,
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -97,9 +97,9 @@
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
     "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/re.pyi",
     "plugin_data": null,
     "size": 11135,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/shlex.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/shlex.data.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999999969086341%*

 * *Differences: {"'names'": "{'shlex': {'node': {'names': {'eof': {'node': {'type': {replace: "*

 * *            "OrderedDict([('.class', 'UnionType'), ('items', ['builtins.str', "*

 * *            "OrderedDict([('.class', 'NoneType')])])])}}}, 'error_leader': {'node': {'type': "*

 * *            "{'ret_type': 'builtins.str'}}}, 'get_token': {'node': {'type': {'ret_type': {replace: "*

 * *            "OrderedDict([('.class', 'UnionType'), ('items', ['builtins.str', "*

 * *            "OrderedDict([('.class', 'NoneType')])])])}}}}, 'read_token': {' […]*

```diff
@@ -499,15 +499,23 @@
                             ".class": "Var",
                             "flags": [
                                 "is_initialized_in_class",
                                 "is_ready"
                             ],
                             "fullname": "shlex.shlex.eof",
                             "name": "eof",
-                            "type": "builtins.str"
+                            "type": {
+                                ".class": "UnionType",
+                                "items": [
+                                    "builtins.str",
+                                    {
+                                        ".class": "NoneType"
+                                    }
+                                ]
+                            }
                         }
                     },
                     "error_leader": {
                         ".class": "SymbolTableNode",
                         "kind": "Mdef",
                         "node": {
                             ".class": "FuncDef",
@@ -564,17 +572,15 @@
                                     "first_arg": "self"
                                 },
                                 "fallback": "builtins.function",
                                 "from_concatenate": false,
                                 "implicit": false,
                                 "is_ellipsis_args": false,
                                 "name": "error_leader of shlex",
-                                "ret_type": {
-                                    ".class": "NoneType"
-                                },
+                                "ret_type": "builtins.str",
                                 "type_guard": null,
                                 "unpack_kwargs": false,
                                 "variables": []
                             }
                         }
                     },
                     "escape": {
@@ -637,15 +643,23 @@
                                     "first_arg": "self"
                                 },
                                 "fallback": "builtins.function",
                                 "from_concatenate": false,
                                 "implicit": false,
                                 "is_ellipsis_args": false,
                                 "name": "get_token of shlex",
-                                "ret_type": "builtins.str",
+                                "ret_type": {
+                                    ".class": "UnionType",
+                                    "items": [
+                                        "builtins.str",
+                                        {
+                                            ".class": "NoneType"
+                                        }
+                                    ]
+                                },
                                 "type_guard": null,
                                 "unpack_kwargs": false,
                                 "variables": []
                             }
                         }
                     },
                     "infile": {
@@ -994,15 +1008,23 @@
                                     "first_arg": "self"
                                 },
                                 "fallback": "builtins.function",
                                 "from_concatenate": false,
                                 "implicit": false,
                                 "is_ellipsis_args": false,
                                 "name": "read_token of shlex",
-                                "ret_type": "builtins.str",
+                                "ret_type": {
+                                    ".class": "UnionType",
+                                    "items": [
+                                        "builtins.str",
+                                        {
+                                            ".class": "NoneType"
+                                        }
+                                    ]
+                                },
                                 "type_guard": null,
                                 "unpack_kwargs": false,
                                 "variables": []
                             }
                         }
                     },
                     "source": {
@@ -1057,32 +1079,40 @@
                                 },
                                 "fallback": "builtins.function",
                                 "from_concatenate": false,
                                 "implicit": false,
                                 "is_ellipsis_args": false,
                                 "name": "sourcehook of shlex",
                                 "ret_type": {
-                                    ".class": "TupleType",
-                                    "implicit": false,
+                                    ".class": "UnionType",
                                     "items": [
-                                        "builtins.str",
-                                        "typing.TextIO"
-                                    ],
-                                    "partial_fallback": {
-                                        ".class": "Instance",
-                                        "args": [
-                                            {
-                                                ".class": "AnyType",
-                                                "missing_import_name": null,
-                                                "source_any": null,
-                                                "type_of_any": 6
+                                        {
+                                            ".class": "TupleType",
+                                            "implicit": false,
+                                            "items": [
+                                                "builtins.str",
+                                                "typing.TextIO"
+                                            ],
+                                            "partial_fallback": {
+                                                ".class": "Instance",
+                                                "args": [
+                                                    {
+                                                        ".class": "AnyType",
+                                                        "missing_import_name": null,
+                                                        "source_any": null,
+                                                        "type_of_any": 6
+                                                    }
+                                                ],
+                                                "type_ref": "builtins.tuple"
                                             }
-                                        ],
-                                        "type_ref": "builtins.tuple"
-                                    }
+                                        },
+                                        {
+                                            ".class": "NoneType"
+                                        }
+                                    ]
                                 },
                                 "type_guard": null,
                                 "unpack_kwargs": false,
                                 "variables": []
                             }
                         }
                     },
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/shlex.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/shlex.meta.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8%*

 * *Differences: {"'data_mtime'": '1683843440',*

 * * "'hash'": "'b6068708c447c5be5cab55e6b0d9ea628424eac94864658817eaff5f659ce914'",*

 * * "'interface_hash'": "'a26a6eed061dc3ebee7ec3f00654f4c6750d77cbae9a9bfbd1f9211bf1848d84'",*

 * * "'mtime'": '1684623296',*

 * * "'size'": '1502',*

 * * "'version_id'": "'1.3.0'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843440,
     "dep_lines": [
         2,
         1,
         3,
         4,
         1,
         1,
@@ -23,19 +23,19 @@
         "sys",
         "typing",
         "typing_extensions",
         "builtins",
         "_typeshed",
         "abc"
     ],
-    "hash": "a7171f9693df2f4c3af37e86f05adf69eaab9b999b5e3d1cf9ad0190a9701963",
+    "hash": "b6068708c447c5be5cab55e6b0d9ea628424eac94864658817eaff5f659ce914",
     "id": "shlex",
     "ignore_all": true,
-    "interface_hash": "73be19d5bc49365ce75985ba5ae02de2ee25f9d1a19c58f2d3b26ba60a65e985",
-    "mtime": 1683082840,
+    "interface_hash": "a26a6eed061dc3ebee7ec3f00654f4c6750d77cbae9a9bfbd1f9211bf1848d84",
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -71,11 +71,11 @@
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
     "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/shlex.pyi",
     "plugin_data": null,
-    "size": 1475,
+    "size": 1502,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/shutil.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/shutil.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/shutil.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/_ast.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6717948717948717%*

 * *Differences: {"'data_mtime'": '1683843440',*

 * * "'dep_lines'": '{insert: [(3, 1), (4, 1), (5, 1), (6, 1), (7, 1)], delete: [5, 4, 0]}',*

 * * "'dep_prios'": '{insert: [(4, 30), (5, 30), (6, 30), (7, 30), (8, 30)], delete: [3, 1, 0]}',*

 * * "'dependencies'": "{insert: [(4, '_typeshed'), (6, 'array'), (7, 'ctypes'), (8, 'mmap'), (9, "*

 * *                   "'pickle')], delete: [3, 1, 0]}",*

 * * "'hash'": "'189ca9e5f979d2fafddf0fde549a04c4da5840422b279c427ac3b84df670b646'",*

 * * "'id'": "'_ast'",*

 * * "'interface_hash'": "'a313ff97b5329396c2ba6b232b […]*

```diff
@@ -1,44 +1,50 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843440,
     "dep_lines": [
-        4,
         1,
         2,
         3,
-        5,
-        6,
+        1,
+        1,
+        1,
+        1,
+        1,
         1,
         1
     ],
     "dep_prios": [
-        5,
-        10,
         10,
         5,
         5,
         5,
-        5,
+        30,
+        30,
+        30,
+        30,
+        30,
         30
     ],
     "dependencies": [
-        "collections.abc",
-        "os",
         "sys",
-        "_typeshed",
         "typing",
         "typing_extensions",
         "builtins",
-        "abc"
+        "_typeshed",
+        "abc",
+        "array",
+        "ctypes",
+        "mmap",
+        "pickle"
     ],
-    "hash": "7d62792364f18e7e491b842042c2abffbf0331c6f9e3b9871fdb48ef5ef0e8ca",
-    "id": "shutil",
+    "hash": "189ca9e5f979d2fafddf0fde549a04c4da5840422b279c427ac3b84df670b646",
+    "id": "_ast",
     "ignore_all": true,
-    "interface_hash": "c31bb8365bf9434dd242575270735882df910b7c55b39b8e312be0961ea06831",
-    "mtime": 1683082840,
+    "interface_hash": "a313ff97b5329396c2ba6b232b465b36bc665df2453493f09065b6b911d9c1d4",
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -72,13 +78,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/shutil.pyi",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/_ast.pyi",
     "plugin_data": null,
-    "size": 6653,
+    "size": 14752,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/sre_compile.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/sre_compile.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/sre_compile.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/email/contentmanager.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6926587301587301%*

 * *Differences: {"'data_mtime'": '1683843440',*

 * * "'dep_lines'": '{insert: [(2, 3)], delete: [3, 2]}',*

 * * "'dep_prios'": '{delete: [0]}',*

 * * "'dependencies'": "{insert: [(0, 'collections.abc'), (1, 'email.message')], delete: [2, 1, 0]}",*

 * * "'hash'": "'53099e51c46e4530831d75440f30c0481378944b551b503d0689cd68c9afd1bf'",*

 * * "'id'": "'email.contentmanager'",*

 * * "'interface_hash'": "'e8be1394995719c9a2c021f56688ad6fb187cb5c81ab78e43653093ad9b27fd0'",*

 * * "'mtime'": '1684623296',*

 * * "'path'": "'/home/gotmax/Sync/git-repos/packaging/fedora_rpms/ […]*

```diff
@@ -1,38 +1,35 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843440,
     "dep_lines": [
         1,
         2,
-        4,
-        5,
+        3,
         1,
         1
     ],
     "dep_prios": [
         5,
         5,
         5,
         5,
-        5,
         30
     ],
     "dependencies": [
-        "re",
-        "sre_constants",
-        "sre_parse",
+        "collections.abc",
+        "email.message",
         "typing",
         "builtins",
         "abc"
     ],
-    "hash": "c9cd67b263730096df01415a2933288a4f7d800e1380fc31f76bb1e39af65440",
-    "id": "sre_compile",
+    "hash": "53099e51c46e4530831d75440f30c0481378944b551b503d0689cd68c9afd1bf",
+    "id": "email.contentmanager",
     "ignore_all": true,
-    "interface_hash": "3128a45ec285be40db17b279b171fb09c4c5a67948ec05ca7a4f65007ae945a0",
-    "mtime": 1683082840,
+    "interface_hash": "e8be1394995719c9a2c021f56688ad6fb187cb5c81ab78e43653093ad9b27fd0",
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -66,13 +63,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/sre_compile.pyi",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/email/contentmanager.pyi",
     "plugin_data": null,
-    "size": 332,
+    "size": 480,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/sre_constants.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/sre_constants.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/sre_constants.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/click/globals.meta.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6833333333333333%*

 * *Differences: {"'data_mtime'": '1683843441',*

 * * "'dep_lines'": '{insert: [(0, 6), (3, 5)], delete: [3, 2]}',*

 * * "'dep_prios'": '{insert: [(0, 25), (3, 25)], delete: [4, 1]}',*

 * * "'dependencies'": "{insert: [(0, 'click.core'), (2, 'threading')], delete: [4, 0]}",*

 * * "'hash'": "'4cffaa33cf124f373b7f5dbb877e530ffbfddb41607ce0f6130cea034a04f175'",*

 * * "'id'": "'click.globals'",*

 * * "'interface_hash'": "'ae61ea35093262c5c00b99651085c8dac525ebd30575b9c101234bc83a3c55bf'",*

 * * "'mtime'": '1684623295',*

 * * "'path'": "'/home/gotmax/Sync/git-repos/pa […]*

```diff
@@ -1,38 +1,38 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843441,
     "dep_lines": [
+        6,
         1,
         2,
-        3,
-        1,
+        5,
         1,
         1
     ],
     "dep_prios": [
+        25,
         10,
         5,
+        25,
         5,
-        5,
-        30,
         30
     ],
     "dependencies": [
-        "sys",
+        "click.core",
         "typing",
+        "threading",
         "typing_extensions",
         "builtins",
-        "_typeshed",
         "abc"
     ],
-    "hash": "cfb8327ad6d1f82090949665027111e9f4f54c3e1dc0b5baec0b377845590a5c",
-    "id": "sre_constants",
+    "hash": "4cffaa33cf124f373b7f5dbb877e530ffbfddb41607ce0f6130cea034a04f175",
+    "id": "click.globals",
     "ignore_all": true,
-    "interface_hash": "fc1c739257bfb8151b2188ae01d06d69f8ba90f3c9a8a68ad5fa93062826d8db",
-    "mtime": 1683082840,
+    "interface_hash": "ae61ea35093262c5c00b99651085c8dac525ebd30575b9c101234bc83a3c55bf",
+    "mtime": 1684623295,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -66,13 +66,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/sre_constants.pyi",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib/python3.11/site-packages/click/globals.py",
     "plugin_data": null,
-    "size": 3986,
+    "size": 1961,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/sre_parse.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/sre_parse.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/sre_parse.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/string.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7045454545454546%*

 * *Differences: {"'data_mtime'": '1683843440',*

 * * "'dep_lines'": '{insert: [(1, 1), (2, 2), (4, 5)], delete: [5, 1, 0]}',*

 * * "'dependencies'": "{insert: [(2, '_typeshed'), (8, 'enum')], delete: [7, 3]}",*

 * * "'hash'": "'cc44bbe664dd2094229250b9499117bb258740f154f72d04a08d32edb54ad646'",*

 * * "'id'": "'string'",*

 * * "'interface_hash'": "'989dc335797bf2f421e98de64ee179f5970c6e7534a955751f97f88a2d1c6ec0'",*

 * * "'mtime'": '1684623296',*

 * * "'path'": "'/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-p […]*

```diff
@@ -1,16 +1,16 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843440,
     "dep_lines": [
-        2,
-        1,
         3,
+        1,
+        2,
         4,
+        5,
         6,
-        7,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
         10,
@@ -21,27 +21,27 @@
         5,
         30,
         30
     ],
     "dependencies": [
         "collections.abc",
         "sys",
+        "_typeshed",
         "re",
-        "sre_constants",
         "typing",
         "typing_extensions",
         "builtins",
-        "_typeshed",
-        "abc"
+        "abc",
+        "enum"
     ],
-    "hash": "38b6a819e544b584ec71b7040293fae6a77f2447fc14e9bc70e752ec237c8022",
-    "id": "sre_parse",
+    "hash": "cc44bbe664dd2094229250b9499117bb258740f154f72d04a08d32edb54ad646",
+    "id": "string",
     "ignore_all": true,
-    "interface_hash": "f5b5305584ba71c58843130ee41dcb142383ee5c147b1f177f4029bfd99b1751",
-    "mtime": 1683082840,
+    "interface_hash": "989dc335797bf2f421e98de64ee179f5970c6e7534a955751f97f88a2d1c6ec0",
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -75,13 +75,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/sre_parse.pyi",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/string.pyi",
     "plugin_data": null,
-    "size": 4069,
+    "size": 3097,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/stat.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/stat.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/stat.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/copy.meta.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6966666666666667%*

 * *Differences: {"'data_mtime'": '1683843440',*

 * * "'dep_lines'": '{delete: [0]}',*

 * * "'dep_prios'": '{delete: [2]}',*

 * * "'dependencies'": "{insert: [(0, 'typing')], delete: [3, 0]}",*

 * * "'hash'": "'891dbbc4965fc233e2f13e2c8f79729c2bfce84a3f6f841f77ab43efd675ee7d'",*

 * * "'id'": "'copy'",*

 * * "'interface_hash'": "'022ac223f551840f8f85eef00a862d50292bd030555b9d2559f0faabfbcac6dc'",*

 * * "'mtime'": '1684623296',*

 * * "'path'": "'/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/std […]*

```diff
@@ -1,32 +1,29 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843440,
     "dep_lines": [
         1,
         1,
-        1,
         1
     ],
     "dep_prios": [
         5,
         5,
-        30,
         30
     ],
     "dependencies": [
-        "_stat",
+        "typing",
         "builtins",
-        "abc",
-        "typing"
+        "abc"
     ],
-    "hash": "1fd817ee6e4326df5c4f9878c64dc9c080c05437734adfdc1dfa1e546fc1d8aa",
-    "id": "stat",
+    "hash": "891dbbc4965fc233e2f13e2c8f79729c2bfce84a3f6f841f77ab43efd675ee7d",
+    "id": "copy",
     "ignore_all": true,
-    "interface_hash": "1b3706b64ab100789d464059bc54ddbff999417b9d38e3a3e6f62cd0eee4c0a9",
-    "mtime": 1683082840,
+    "interface_hash": "022ac223f551840f8f85eef00a862d50292bd030555b9d2559f0faabfbcac6dc",
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -60,13 +57,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/stat.pyi",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/copy.pyi",
     "plugin_data": null,
-    "size": 20,
+    "size": 350,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/string.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/string.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/string.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/fractions.meta.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6928404928404928%*

 * *Differences: {"'data_mtime'": '1683843440',*

 * * "'dep_lines'": '{insert: [(1, 1), (2, 3), (6, 1), (7, 1)], delete: [1, 0]}',*

 * * "'dep_prios'": '{insert: [(7, 30), (8, 30)]}',*

 * * "'dependencies'": "{insert: [(2, 'decimal'), (3, 'numbers'), (7, '_decimal'), (8, '_operator'), "*

 * *                   "(9, '_typeshed')], delete: [8, 3, 2]}",*

 * * "'hash'": "'8920640aa1ef26e4093747df64e273af50a65c28cef9cb693e6feaff46bdfe88'",*

 * * "'id'": "'fractions'",*

 * * "'interface_hash'": "'22a8033e0f019548b33352a9f733c7e5810adac15da15f82803a06b46f30f94a'",*

 * * […]*

```diff
@@ -1,47 +1,53 @@
 {
-    "data_mtime": 1681571246,
+    "data_mtime": 1683843440,
     "dep_lines": [
-        3,
-        1,
         2,
+        1,
+        3,
         4,
         5,
         6,
         1,
         1,
+        1,
+        1,
         1
     ],
     "dep_prios": [
         5,
         10,
         5,
         5,
         5,
         5,
         5,
         30,
+        30,
+        30,
         30
     ],
     "dependencies": [
         "collections.abc",
         "sys",
-        "_typeshed",
-        "re",
+        "decimal",
+        "numbers",
         "typing",
         "typing_extensions",
         "builtins",
-        "abc",
-        "enum"
+        "_decimal",
+        "_operator",
+        "_typeshed",
+        "abc"
     ],
-    "hash": "1975bf6d1701cdae908af3479e5af21981f03650faed23c04fdcbdd9cf56ba4f",
-    "id": "string",
+    "hash": "8920640aa1ef26e4093747df64e273af50a65c28cef9cb693e6feaff46bdfe88",
+    "id": "fractions",
     "ignore_all": true,
-    "interface_hash": "989dc335797bf2f421e98de64ee179f5970c6e7534a955751f97f88a2d1c6ec0",
-    "mtime": 1683082840,
+    "interface_hash": "22a8033e0f019548b33352a9f733c7e5810adac15da15f82803a06b46f30f94a",
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -75,13 +81,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/string.pyi",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/fractions.pyi",
     "plugin_data": null,
-    "size": 3099,
+    "size": 5584,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/subprocess.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/subprocess.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/subprocess.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/os/__init__.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6773993558776167%*

 * *Differences: {"'data_mtime'": '1683843440',*

 * * "'dep_lines'": '{insert: [(0, 23), (1, 30), (4, 21), (5, 22), (6, 24), (7, 25), (8, 26), (9, 27), '*

 * *                '(10, 28), (11, 33)], delete: [8, 7, 6, 5, 4, 3, 0]}',*

 * * "'dep_prios'": '{insert: [(1, 10), (8, 5), (9, 5), (10, 5), (11, 5)], delete: [8, 7]}',*

 * * "'dependencies'": "{insert: [(1, 'os.path'), (4, 'abc'), (5, 'builtins'), (6, 'contextlib'), (7, "*

 * *                   "'io'), (8, 'subprocess'), (11, 'types')], delete: [11, 7, 6, 3]}",*

 * * "'hash'": "'43f0abc8936c573dfefd […]*

```diff
@@ -1,59 +1,68 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843440,
     "dep_lines": [
-        3,
+        23,
+        30,
         1,
         2,
-        4,
-        5,
-        6,
-        1,
-        1,
-        1,
+        21,
+        22,
+        24,
+        25,
+        26,
+        27,
+        28,
+        33,
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
         10,
+        10,
+        5,
+        5,
+        5,
+        5,
         5,
         5,
         5,
         5,
         5,
-        30,
-        30,
         30,
         30,
         30,
         30
     ],
     "dependencies": [
         "collections.abc",
+        "os.path",
         "sys",
         "_typeshed",
-        "types",
+        "abc",
+        "builtins",
+        "contextlib",
+        "io",
+        "subprocess",
         "typing",
         "typing_extensions",
-        "builtins",
-        "abc",
+        "types",
         "array",
         "ctypes",
         "mmap",
-        "os",
         "pickle"
     ],
-    "hash": "e6dad7d21be099bd7eb941b53a17631fd100aeeec7d943ff981298f8363e5d59",
-    "id": "subprocess",
+    "hash": "43f0abc8936c573dfefd04ae185e74a6fc8eac1be65a0daaaf327303d8dc486e",
+    "id": "os",
     "ignore_all": true,
-    "interface_hash": "1a69c378047966f5989ec904cd1b1d993251601f6a9eae741e5a0e04af9ae035",
-    "mtime": 1683082840,
+    "interface_hash": "c472e678239a2b046b7a9b8db5b5d3650e4d7aa2b07ee3c6d26a03316a587b2a",
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -87,13 +96,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/subprocess.pyi",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/os/__init__.pyi",
     "plugin_data": null,
-    "size": 91115,
+    "size": 36995,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/sys.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/sys.data.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9974337912752141%*

 * *Differences: {"'names'": "{'_AsyncgenHook': {'node': {'line': 324}}, 'getsizeof': {'node': {'.class': "*

 * *            "'FuncDef', 'type': {'.class': 'CallableType', 'arg_kinds': [0, 1], 'arg_names': "*

 * *            "['obj', 'default'], 'arg_types': ['builtins.object', 'builtins.int'], 'bound_args': "*

 * *            "[], 'def_extras': OrderedDict([('first_arg', None)]), 'fallback': "*

 * *            "'builtins.function', 'from_concatenate': False, 'implicit': False, "*

 * *            "'is_ellipsis_args': False, 'name': 'getsizeof', 're […]*

```diff
@@ -294,15 +294,15 @@
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "TypeAlias",
                 "alias_tvars": [],
                 "column": 0,
                 "fullname": "sys._AsyncgenHook",
-                "line": 313,
+                "line": 324,
                 "no_args": false,
                 "normalized": false,
                 "target": {
                     ".class": "UnionType",
                     "items": [
                         {
                             ".class": "CallableType",
@@ -579,14 +579,83 @@
                 "fullname": "sys._T",
                 "name": "_T",
                 "upper_bound": "builtins.object",
                 "values": [],
                 "variance": 0
             }
         },
+        "_ThreadInfoLock": {
+            ".class": "SymbolTableNode",
+            "kind": "Gdef",
+            "node": {
+                ".class": "TypeAlias",
+                "alias_tvars": [],
+                "column": 0,
+                "fullname": "sys._ThreadInfoLock",
+                "line": 205,
+                "no_args": false,
+                "normalized": false,
+                "target": {
+                    ".class": "UnionType",
+                    "items": [
+                        {
+                            ".class": "LiteralType",
+                            "fallback": "builtins.str",
+                            "value": "semaphore"
+                        },
+                        {
+                            ".class": "LiteralType",
+                            "fallback": "builtins.str",
+                            "value": "mutex+cond"
+                        },
+                        {
+                            ".class": "NoneType"
+                        }
+                    ]
+                }
+            }
+        },
+        "_ThreadInfoName": {
+            ".class": "SymbolTableNode",
+            "kind": "Gdef",
+            "node": {
+                ".class": "TypeAlias",
+                "alias_tvars": [],
+                "column": 0,
+                "fullname": "sys._ThreadInfoName",
+                "line": 204,
+                "no_args": false,
+                "normalized": false,
+                "target": {
+                    ".class": "UnionType",
+                    "items": [
+                        {
+                            ".class": "LiteralType",
+                            "fallback": "builtins.str",
+                            "value": "nt"
+                        },
+                        {
+                            ".class": "LiteralType",
+                            "fallback": "builtins.str",
+                            "value": "pthread"
+                        },
+                        {
+                            ".class": "LiteralType",
+                            "fallback": "builtins.str",
+                            "value": "pthread-stubs"
+                        },
+                        {
+                            ".class": "LiteralType",
+                            "fallback": "builtins.str",
+                            "value": "solaris"
+                        }
+                    ]
+                }
+            }
+        },
         "_UninstantiableStructseq": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "TypeAlias",
                 "alias_tvars": [],
                 "column": 0,
@@ -7039,14 +7108,552 @@
         "_object": {
             ".class": "SymbolTableNode",
             "cross_ref": "builtins.object",
             "kind": "Gdef",
             "module_hidden": true,
             "module_public": false
         },
+        "_thread_info": {
+            ".class": "SymbolTableNode",
+            "kind": "Gdef",
+            "node": {
+                ".class": "TypeInfo",
+                "_promote": [],
+                "abstract_attributes": [],
+                "alt_promote": null,
+                "bases": [
+                    {
+                        ".class": "Instance",
+                        "args": [
+                            {
+                                ".class": "AnyType",
+                                "missing_import_name": null,
+                                "source_any": null,
+                                "type_of_any": 6
+                            }
+                        ],
+                        "type_ref": "_typeshed.structseq"
+                    },
+                    {
+                        ".class": "Instance",
+                        "args": [
+                            "builtins.str"
+                        ],
+                        "type_ref": "builtins.tuple"
+                    }
+                ],
+                "dataclass_transform_spec": null,
+                "declared_metaclass": null,
+                "defn": {
+                    ".class": "ClassDef",
+                    "fullname": "sys._thread_info",
+                    "name": "_thread_info",
+                    "type_vars": []
+                },
+                "deletable_attributes": [],
+                "flags": [
+                    "is_final"
+                ],
+                "fullname": "sys._thread_info",
+                "has_param_spec_type": false,
+                "metaclass_type": "abc.ABCMeta",
+                "metadata": {},
+                "module_name": "sys",
+                "mro": [
+                    "sys._thread_info",
+                    "_typeshed.structseq",
+                    "builtins.tuple",
+                    "typing.Sequence",
+                    "typing.Collection",
+                    "typing.Reversible",
+                    "typing.Iterable",
+                    "typing.Container",
+                    "builtins.object"
+                ],
+                "names": {
+                    ".class": "SymbolTable",
+                    "lock": {
+                        ".class": "SymbolTableNode",
+                        "kind": "Mdef",
+                        "node": {
+                            ".class": "Decorator",
+                            "func": {
+                                ".class": "FuncDef",
+                                "abstract_status": 0,
+                                "arg_kinds": [
+                                    0
+                                ],
+                                "arg_names": [
+                                    "self"
+                                ],
+                                "dataclass_transform_spec": null,
+                                "flags": [
+                                    "is_property",
+                                    "is_decorated"
+                                ],
+                                "fullname": "sys._thread_info.lock",
+                                "name": "lock",
+                                "type": {
+                                    ".class": "CallableType",
+                                    "arg_kinds": [
+                                        0
+                                    ],
+                                    "arg_names": [
+                                        "self"
+                                    ],
+                                    "arg_types": [
+                                        {
+                                            ".class": "TupleType",
+                                            "implicit": false,
+                                            "items": [
+                                                {
+                                                    ".class": "TypeAliasType",
+                                                    "args": [],
+                                                    "type_ref": "sys._ThreadInfoName"
+                                                },
+                                                {
+                                                    ".class": "TypeAliasType",
+                                                    "args": [],
+                                                    "type_ref": "sys._ThreadInfoLock"
+                                                },
+                                                {
+                                                    ".class": "UnionType",
+                                                    "items": [
+                                                        "builtins.str",
+                                                        {
+                                                            ".class": "NoneType"
+                                                        }
+                                                    ]
+                                                }
+                                            ],
+                                            "partial_fallback": "sys._thread_info"
+                                        }
+                                    ],
+                                    "bound_args": [],
+                                    "def_extras": {
+                                        "first_arg": "self"
+                                    },
+                                    "fallback": "builtins.function",
+                                    "from_concatenate": false,
+                                    "implicit": false,
+                                    "is_ellipsis_args": false,
+                                    "name": "lock of _thread_info",
+                                    "ret_type": {
+                                        ".class": "TypeAliasType",
+                                        "args": [],
+                                        "type_ref": "sys._ThreadInfoLock"
+                                    },
+                                    "type_guard": null,
+                                    "unpack_kwargs": false,
+                                    "variables": []
+                                }
+                            },
+                            "is_overload": false,
+                            "var": {
+                                ".class": "Var",
+                                "flags": [
+                                    "is_initialized_in_class",
+                                    "is_property",
+                                    "is_ready",
+                                    "is_inferred"
+                                ],
+                                "fullname": "sys._thread_info.lock",
+                                "name": "lock",
+                                "type": {
+                                    ".class": "CallableType",
+                                    "arg_kinds": [
+                                        0
+                                    ],
+                                    "arg_names": [
+                                        "self"
+                                    ],
+                                    "arg_types": [
+                                        {
+                                            ".class": "TupleType",
+                                            "implicit": false,
+                                            "items": [
+                                                {
+                                                    ".class": "TypeAliasType",
+                                                    "args": [],
+                                                    "type_ref": "sys._ThreadInfoName"
+                                                },
+                                                {
+                                                    ".class": "TypeAliasType",
+                                                    "args": [],
+                                                    "type_ref": "sys._ThreadInfoLock"
+                                                },
+                                                {
+                                                    ".class": "UnionType",
+                                                    "items": [
+                                                        "builtins.str",
+                                                        {
+                                                            ".class": "NoneType"
+                                                        }
+                                                    ]
+                                                }
+                                            ],
+                                            "partial_fallback": "sys._thread_info"
+                                        }
+                                    ],
+                                    "bound_args": [],
+                                    "def_extras": {
+                                        "first_arg": "self"
+                                    },
+                                    "fallback": "builtins.function",
+                                    "from_concatenate": false,
+                                    "implicit": false,
+                                    "is_ellipsis_args": false,
+                                    "name": "lock of _thread_info",
+                                    "ret_type": {
+                                        ".class": "TypeAliasType",
+                                        "args": [],
+                                        "type_ref": "sys._ThreadInfoLock"
+                                    },
+                                    "type_guard": null,
+                                    "unpack_kwargs": false,
+                                    "variables": []
+                                }
+                            }
+                        }
+                    },
+                    "name": {
+                        ".class": "SymbolTableNode",
+                        "kind": "Mdef",
+                        "node": {
+                            ".class": "Decorator",
+                            "func": {
+                                ".class": "FuncDef",
+                                "abstract_status": 0,
+                                "arg_kinds": [
+                                    0
+                                ],
+                                "arg_names": [
+                                    "self"
+                                ],
+                                "dataclass_transform_spec": null,
+                                "flags": [
+                                    "is_property",
+                                    "is_decorated"
+                                ],
+                                "fullname": "sys._thread_info.name",
+                                "name": "name",
+                                "type": {
+                                    ".class": "CallableType",
+                                    "arg_kinds": [
+                                        0
+                                    ],
+                                    "arg_names": [
+                                        "self"
+                                    ],
+                                    "arg_types": [
+                                        {
+                                            ".class": "TupleType",
+                                            "implicit": false,
+                                            "items": [
+                                                {
+                                                    ".class": "TypeAliasType",
+                                                    "args": [],
+                                                    "type_ref": "sys._ThreadInfoName"
+                                                },
+                                                {
+                                                    ".class": "TypeAliasType",
+                                                    "args": [],
+                                                    "type_ref": "sys._ThreadInfoLock"
+                                                },
+                                                {
+                                                    ".class": "UnionType",
+                                                    "items": [
+                                                        "builtins.str",
+                                                        {
+                                                            ".class": "NoneType"
+                                                        }
+                                                    ]
+                                                }
+                                            ],
+                                            "partial_fallback": "sys._thread_info"
+                                        }
+                                    ],
+                                    "bound_args": [],
+                                    "def_extras": {
+                                        "first_arg": "self"
+                                    },
+                                    "fallback": "builtins.function",
+                                    "from_concatenate": false,
+                                    "implicit": false,
+                                    "is_ellipsis_args": false,
+                                    "name": "name of _thread_info",
+                                    "ret_type": {
+                                        ".class": "TypeAliasType",
+                                        "args": [],
+                                        "type_ref": "sys._ThreadInfoName"
+                                    },
+                                    "type_guard": null,
+                                    "unpack_kwargs": false,
+                                    "variables": []
+                                }
+                            },
+                            "is_overload": false,
+                            "var": {
+                                ".class": "Var",
+                                "flags": [
+                                    "is_initialized_in_class",
+                                    "is_property",
+                                    "is_ready",
+                                    "is_inferred"
+                                ],
+                                "fullname": "sys._thread_info.name",
+                                "name": "name",
+                                "type": {
+                                    ".class": "CallableType",
+                                    "arg_kinds": [
+                                        0
+                                    ],
+                                    "arg_names": [
+                                        "self"
+                                    ],
+                                    "arg_types": [
+                                        {
+                                            ".class": "TupleType",
+                                            "implicit": false,
+                                            "items": [
+                                                {
+                                                    ".class": "TypeAliasType",
+                                                    "args": [],
+                                                    "type_ref": "sys._ThreadInfoName"
+                                                },
+                                                {
+                                                    ".class": "TypeAliasType",
+                                                    "args": [],
+                                                    "type_ref": "sys._ThreadInfoLock"
+                                                },
+                                                {
+                                                    ".class": "UnionType",
+                                                    "items": [
+                                                        "builtins.str",
+                                                        {
+                                                            ".class": "NoneType"
+                                                        }
+                                                    ]
+                                                }
+                                            ],
+                                            "partial_fallback": "sys._thread_info"
+                                        }
+                                    ],
+                                    "bound_args": [],
+                                    "def_extras": {
+                                        "first_arg": "self"
+                                    },
+                                    "fallback": "builtins.function",
+                                    "from_concatenate": false,
+                                    "implicit": false,
+                                    "is_ellipsis_args": false,
+                                    "name": "name of _thread_info",
+                                    "ret_type": {
+                                        ".class": "TypeAliasType",
+                                        "args": [],
+                                        "type_ref": "sys._ThreadInfoName"
+                                    },
+                                    "type_guard": null,
+                                    "unpack_kwargs": false,
+                                    "variables": []
+                                }
+                            }
+                        }
+                    },
+                    "version": {
+                        ".class": "SymbolTableNode",
+                        "kind": "Mdef",
+                        "node": {
+                            ".class": "Decorator",
+                            "func": {
+                                ".class": "FuncDef",
+                                "abstract_status": 0,
+                                "arg_kinds": [
+                                    0
+                                ],
+                                "arg_names": [
+                                    "self"
+                                ],
+                                "dataclass_transform_spec": null,
+                                "flags": [
+                                    "is_property",
+                                    "is_decorated"
+                                ],
+                                "fullname": "sys._thread_info.version",
+                                "name": "version",
+                                "type": {
+                                    ".class": "CallableType",
+                                    "arg_kinds": [
+                                        0
+                                    ],
+                                    "arg_names": [
+                                        "self"
+                                    ],
+                                    "arg_types": [
+                                        {
+                                            ".class": "TupleType",
+                                            "implicit": false,
+                                            "items": [
+                                                {
+                                                    ".class": "TypeAliasType",
+                                                    "args": [],
+                                                    "type_ref": "sys._ThreadInfoName"
+                                                },
+                                                {
+                                                    ".class": "TypeAliasType",
+                                                    "args": [],
+                                                    "type_ref": "sys._ThreadInfoLock"
+                                                },
+                                                {
+                                                    ".class": "UnionType",
+                                                    "items": [
+                                                        "builtins.str",
+                                                        {
+                                                            ".class": "NoneType"
+                                                        }
+                                                    ]
+                                                }
+                                            ],
+                                            "partial_fallback": "sys._thread_info"
+                                        }
+                                    ],
+                                    "bound_args": [],
+                                    "def_extras": {
+                                        "first_arg": "self"
+                                    },
+                                    "fallback": "builtins.function",
+                                    "from_concatenate": false,
+                                    "implicit": false,
+                                    "is_ellipsis_args": false,
+                                    "name": "version of _thread_info",
+                                    "ret_type": {
+                                        ".class": "UnionType",
+                                        "items": [
+                                            "builtins.str",
+                                            {
+                                                ".class": "NoneType"
+                                            }
+                                        ]
+                                    },
+                                    "type_guard": null,
+                                    "unpack_kwargs": false,
+                                    "variables": []
+                                }
+                            },
+                            "is_overload": false,
+                            "var": {
+                                ".class": "Var",
+                                "flags": [
+                                    "is_initialized_in_class",
+                                    "is_property",
+                                    "is_ready",
+                                    "is_inferred"
+                                ],
+                                "fullname": "sys._thread_info.version",
+                                "name": "version",
+                                "type": {
+                                    ".class": "CallableType",
+                                    "arg_kinds": [
+                                        0
+                                    ],
+                                    "arg_names": [
+                                        "self"
+                                    ],
+                                    "arg_types": [
+                                        {
+                                            ".class": "TupleType",
+                                            "implicit": false,
+                                            "items": [
+                                                {
+                                                    ".class": "TypeAliasType",
+                                                    "args": [],
+                                                    "type_ref": "sys._ThreadInfoName"
+                                                },
+                                                {
+                                                    ".class": "TypeAliasType",
+                                                    "args": [],
+                                                    "type_ref": "sys._ThreadInfoLock"
+                                                },
+                                                {
+                                                    ".class": "UnionType",
+                                                    "items": [
+                                                        "builtins.str",
+                                                        {
+                                                            ".class": "NoneType"
+                                                        }
+                                                    ]
+                                                }
+                                            ],
+                                            "partial_fallback": "sys._thread_info"
+                                        }
+                                    ],
+                                    "bound_args": [],
+                                    "def_extras": {
+                                        "first_arg": "self"
+                                    },
+                                    "fallback": "builtins.function",
+                                    "from_concatenate": false,
+                                    "implicit": false,
+                                    "is_ellipsis_args": false,
+                                    "name": "version of _thread_info",
+                                    "ret_type": {
+                                        ".class": "UnionType",
+                                        "items": [
+                                            "builtins.str",
+                                            {
+                                                ".class": "NoneType"
+                                            }
+                                        ]
+                                    },
+                                    "type_guard": null,
+                                    "unpack_kwargs": false,
+                                    "variables": []
+                                }
+                            }
+                        }
+                    }
+                },
+                "self_type": null,
+                "slots": null,
+                "tuple_type": {
+                    ".class": "TupleType",
+                    "implicit": false,
+                    "items": [
+                        {
+                            ".class": "TypeAliasType",
+                            "args": [],
+                            "type_ref": "sys._ThreadInfoName"
+                        },
+                        {
+                            ".class": "TypeAliasType",
+                            "args": [],
+                            "type_ref": "sys._ThreadInfoLock"
+                        },
+                        {
+                            ".class": "UnionType",
+                            "items": [
+                                "builtins.str",
+                                {
+                                    ".class": "NoneType"
+                                }
+                            ]
+                        }
+                    ],
+                    "partial_fallback": {
+                        ".class": "Instance",
+                        "args": [
+                            "builtins.str"
+                        ],
+                        "type_ref": "builtins.tuple"
+                    }
+                },
+                "type_vars": [],
+                "typeddict_type": null
+            }
+        },
         "_version_info": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "TypeInfo",
                 "_promote": [],
                 "abstract_attributes": [],
@@ -8874,192 +9481,55 @@
                 }
             }
         },
         "getsizeof": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
-                ".class": "OverloadedFuncDef",
+                ".class": "FuncDef",
+                "abstract_status": 0,
+                "arg_kinds": [
+                    0,
+                    1
+                ],
+                "arg_names": [
+                    "obj",
+                    "default"
+                ],
+                "dataclass_transform_spec": null,
                 "flags": [],
                 "fullname": "sys.getsizeof",
-                "impl": null,
-                "items": [
-                    {
-                        ".class": "Decorator",
-                        "func": {
-                            ".class": "FuncDef",
-                            "abstract_status": 0,
-                            "arg_kinds": [
-                                0
-                            ],
-                            "arg_names": [
-                                "obj"
-                            ],
-                            "dataclass_transform_spec": null,
-                            "flags": [
-                                "is_overload",
-                                "is_decorated"
-                            ],
-                            "fullname": "sys.getsizeof",
-                            "name": "getsizeof",
-                            "type": {
-                                ".class": "CallableType",
-                                "arg_kinds": [
-                                    0
-                                ],
-                                "arg_names": [
-                                    "obj"
-                                ],
-                                "arg_types": [
-                                    "builtins.object"
-                                ],
-                                "bound_args": [],
-                                "def_extras": {
-                                    "first_arg": null
-                                },
-                                "fallback": "builtins.function",
-                                "from_concatenate": false,
-                                "implicit": false,
-                                "is_ellipsis_args": false,
-                                "name": "getsizeof",
-                                "ret_type": "builtins.int",
-                                "type_guard": null,
-                                "unpack_kwargs": false,
-                                "variables": []
-                            }
-                        },
-                        "is_overload": true,
-                        "var": {
-                            ".class": "Var",
-                            "flags": [
-                                "is_inferred"
-                            ],
-                            "fullname": "sys.getsizeof",
-                            "name": "getsizeof",
-                            "type": null
-                        }
-                    },
-                    {
-                        ".class": "Decorator",
-                        "func": {
-                            ".class": "FuncDef",
-                            "abstract_status": 0,
-                            "arg_kinds": [
-                                0,
-                                0
-                            ],
-                            "arg_names": [
-                                "obj",
-                                "default"
-                            ],
-                            "dataclass_transform_spec": null,
-                            "flags": [
-                                "is_overload",
-                                "is_decorated"
-                            ],
-                            "fullname": "sys.getsizeof",
-                            "name": "getsizeof",
-                            "type": {
-                                ".class": "CallableType",
-                                "arg_kinds": [
-                                    0,
-                                    0
-                                ],
-                                "arg_names": [
-                                    "obj",
-                                    "default"
-                                ],
-                                "arg_types": [
-                                    "builtins.object",
-                                    "builtins.int"
-                                ],
-                                "bound_args": [],
-                                "def_extras": {
-                                    "first_arg": null
-                                },
-                                "fallback": "builtins.function",
-                                "from_concatenate": false,
-                                "implicit": false,
-                                "is_ellipsis_args": false,
-                                "name": "getsizeof",
-                                "ret_type": "builtins.int",
-                                "type_guard": null,
-                                "unpack_kwargs": false,
-                                "variables": []
-                            }
-                        },
-                        "is_overload": true,
-                        "var": {
-                            ".class": "Var",
-                            "flags": [
-                                "is_inferred"
-                            ],
-                            "fullname": "sys.getsizeof",
-                            "name": "getsizeof",
-                            "type": null
-                        }
-                    }
-                ],
+                "name": "getsizeof",
                 "type": {
-                    ".class": "Overloaded",
-                    "items": [
-                        {
-                            ".class": "CallableType",
-                            "arg_kinds": [
-                                0
-                            ],
-                            "arg_names": [
-                                "obj"
-                            ],
-                            "arg_types": [
-                                "builtins.object"
-                            ],
-                            "bound_args": [],
-                            "def_extras": {
-                                "first_arg": null
-                            },
-                            "fallback": "builtins.function",
-                            "from_concatenate": false,
-                            "implicit": false,
-                            "is_ellipsis_args": false,
-                            "name": "getsizeof",
-                            "ret_type": "builtins.int",
-                            "type_guard": null,
-                            "unpack_kwargs": false,
-                            "variables": []
-                        },
-                        {
-                            ".class": "CallableType",
-                            "arg_kinds": [
-                                0,
-                                0
-                            ],
-                            "arg_names": [
-                                "obj",
-                                "default"
-                            ],
-                            "arg_types": [
-                                "builtins.object",
-                                "builtins.int"
-                            ],
-                            "bound_args": [],
-                            "def_extras": {
-                                "first_arg": null
-                            },
-                            "fallback": "builtins.function",
-                            "from_concatenate": false,
-                            "implicit": false,
-                            "is_ellipsis_args": false,
-                            "name": "getsizeof",
-                            "ret_type": "builtins.int",
-                            "type_guard": null,
-                            "unpack_kwargs": false,
-                            "variables": []
-                        }
-                    ]
+                    ".class": "CallableType",
+                    "arg_kinds": [
+                        0,
+                        1
+                    ],
+                    "arg_names": [
+                        "obj",
+                        "default"
+                    ],
+                    "arg_types": [
+                        "builtins.object",
+                        "builtins.int"
+                    ],
+                    "bound_args": [],
+                    "def_extras": {
+                        "first_arg": null
+                    },
+                    "fallback": "builtins.function",
+                    "from_concatenate": false,
+                    "implicit": false,
+                    "is_ellipsis_args": false,
+                    "name": "getsizeof",
+                    "ret_type": "builtins.int",
+                    "type_guard": null,
+                    "unpack_kwargs": false,
+                    "variables": []
                 }
             }
         },
         "getswitchinterval": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
@@ -9452,21 +9922,14 @@
                     "args": [
                         "builtins.str"
                     ],
                     "type_ref": "builtins.list"
                 }
             }
         },
-        "overload": {
-            ".class": "SymbolTableNode",
-            "cross_ref": "typing.overload",
-            "kind": "Gdef",
-            "module_hidden": true,
-            "module_public": false
-        },
         "path": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "Var",
                 "flags": [
                     "is_ready"
@@ -10102,14 +10565,31 @@
         "sys": {
             ".class": "SymbolTableNode",
             "cross_ref": "sys",
             "kind": "Gdef",
             "module_hidden": true,
             "module_public": false
         },
+        "thread_info": {
+            ".class": "SymbolTableNode",
+            "kind": "Gdef",
+            "node": {
+                ".class": "Var",
+                "flags": [
+                    "is_ready"
+                ],
+                "fullname": "sys.thread_info",
+                "name": "thread_info",
+                "type": {
+                    ".class": "TypeAliasType",
+                    "args": [],
+                    "type_ref": "sys._thread_info"
+                }
+            }
+        },
         "tracebacklimit": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "Var",
                 "flags": [
                     "is_ready"
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/sys.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/datetime.meta.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6636904761904762%*

 * *Differences: {"'data_mtime'": '1683843440',*

 * * "'dep_lines'": '{insert: [(0, 1), (3, 4), (4, 5)], delete: [8, 7, 6, 5, 2, 1, 0]}',*

 * * "'dep_prios'": '{insert: [(0, 10)], delete: [9, 3, 2, 1, 0]}',*

 * * "'dependencies'": "{insert: [(0, 'sys'), (1, 'abc'), (2, 'time'), (5, 'builtins'), (6, "*

 * *                   "'_typeshed')], delete: [10, 9, 6, 5, 4, 3, 2, 1, 0]}",*

 * * "'hash'": "'0c60f43831b1f7d0abcfb453bf4fcc2d42dc7a37ad8ffe0d7344f047a6ecb87e'",*

 * * "'id'": "'datetime'",*

 * * "'interface_hash'": "'e02d883bc71712722a561b862d984894c2f838d8 […]*

```diff
@@ -1,53 +1,41 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843440,
     "dep_lines": [
-        4,
-        5,
-        6,
+        1,
         2,
         3,
-        7,
-        8,
-        9,
-        10,
+        4,
+        5,
         1,
         1
     ],
     "dep_prios": [
+        10,
         5,
         5,
         5,
         5,
         5,
-        5,
-        5,
-        5,
-        5,
-        30,
         30
     ],
     "dependencies": [
-        "collections.abc",
-        "importlib.abc",
-        "importlib.machinery",
-        "_typeshed",
-        "builtins",
-        "io",
-        "types",
+        "sys",
+        "abc",
+        "time",
         "typing",
         "typing_extensions",
-        "abc",
-        "importlib"
+        "builtins",
+        "_typeshed"
     ],
-    "hash": "793d3a1ebb273506c6ac569ed50a9159bf0e77f70b743fcfe89d4c0607a84030",
-    "id": "sys",
+    "hash": "0c60f43831b1f7d0abcfb453bf4fcc2d42dc7a37ad8ffe0d7344f047a6ecb87e",
+    "id": "datetime",
     "ignore_all": true,
-    "interface_hash": "b34fd9fcefa6bff5210041da0351a2d5d37aeca5e2b022e8cd67336d43299232",
-    "mtime": 1683082840,
+    "interface_hash": "e02d883bc71712722a561b862d984894c2f838d8d8a4591f6baf4fe14010cbee",
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -81,13 +69,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/sys.pyi",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/datetime.pyi",
     "plugin_data": null,
-    "size": 11287,
+    "size": 11534,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/tempfile.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/tempfile.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/tempfile.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/tempfile.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'data_mtime'": '1683843440', "'mtime'": '1684623296', "'version_id'": "'1.3.0'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843440,
     "dep_lines": [
         4,
         1,
         2,
         3,
         5,
         6,
@@ -48,15 +48,15 @@
         "os",
         "pickle"
     ],
     "hash": "7907cc70476aaeb3c54da28bb94a0ee3b8183cedae5975862c489f6c4a25678b",
     "id": "tempfile",
     "ignore_all": true,
     "interface_hash": "101c918da4c27f06805c0a3b828ba299a4745d047b674221b4ff9751ce8c5e1a",
-    "mtime": 1683082840,
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -94,9 +94,9 @@
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
     "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/tempfile.pyi",
     "plugin_data": null,
     "size": 17269,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/termios.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/termios.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/termios.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/tomlkit/source.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.675%*

 * *Differences: {"'data_mtime'": '1683843440',*

 * * "'dep_lines'": '{insert: [(0, 6), (1, 8), (5, 1), (6, 1)], delete: [1]}',*

 * * "'dep_prios'": '{insert: [(0, 5), (1, 5), (6, 30), (7, 30)], delete: [0]}',*

 * * "'dependencies'": "{insert: [(0, 'tomlkit.exceptions'), (1, 'tomlkit.toml_char'), (2, "*

 * *                   "'__future__'), (3, 'copy'), (6, '_typeshed'), (8, 'typing_extensions')], "*

 * *                   'delete: [3, 1, 0]}',*

 * * "'hash'": "'9f046b014909d82c830ca16ce23a3da3446934c35a34da0b0c58b0a3864d6533'",*

 * * "'id'": "'tomlkit.sour […]*

```diff
@@ -1,38 +1,47 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843440,
     "dep_lines": [
+        6,
+        8,
         1,
-        2,
         3,
         4,
         1,
+        1,
+        1,
         1
     ],
     "dep_prios": [
-        10,
         5,
         5,
         5,
         5,
+        5,
+        5,
+        30,
+        30,
         30
     ],
     "dependencies": [
-        "sys",
-        "_typeshed",
+        "tomlkit.exceptions",
+        "tomlkit.toml_char",
+        "__future__",
+        "copy",
         "typing",
-        "typing_extensions",
         "builtins",
-        "abc"
+        "_typeshed",
+        "abc",
+        "typing_extensions"
     ],
-    "hash": "2f0f08844c903b2aa786d04a8a488242c21b5912f570b5db810e5afc7ec29ba9",
-    "id": "termios",
+    "hash": "9f046b014909d82c830ca16ce23a3da3446934c35a34da0b0c58b0a3864d6533",
+    "id": "tomlkit.source",
     "ignore_all": true,
-    "interface_hash": "4e4e4b86f862323bacb98d5169dacc01fe5d7021516565360bd9180ab9c9983e",
-    "mtime": 1683082840,
+    "interface_hash": "2aa600a17b944e8001cbf04116c4a852d2c953e4becdd6571bd32609d8ee4153",
+    "mtime": 1684623295,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -66,13 +75,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/termios.pyi",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib/python3.11/site-packages/tomlkit/source.py",
     "plugin_data": null,
-    "size": 5095,
+    "size": 4823,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/textwrap.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/textwrap.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/textwrap.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/textwrap.meta.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'data_mtime'": '1683843440', "'mtime'": '1684623296', "'version_id'": "'1.3.0'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843440,
     "dep_lines": [
         1,
         2,
         1,
         1,
         1
     ],
@@ -21,15 +21,15 @@
         "abc",
         "typing"
     ],
     "hash": "e9e1065949260d153ff9f03e68e2165ac7bdfb5188abc4fcf52e1569ff5a27b6",
     "id": "textwrap",
     "ignore_all": true,
     "interface_hash": "d149208645051d4a730ca44b2f48f3f85059a7da0f35ca71c93c6bb7f6bec037",
-    "mtime": 1683082840,
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -67,9 +67,9 @@
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
     "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/textwrap.pyi",
     "plugin_data": null,
     "size": 3233,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/threading.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/threading.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/threading.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/typing.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6727119883040935%*

 * *Differences: {"'data_mtime'": '1683843439',*

 * * "'dep_lines'": '{insert: [(2, 3), (6, 7), (7, 8), (8, 9), (9, 1), (10, 1), (11, 1)], delete: [6, '*

 * *                '0]}',*

 * * "'dep_prios'": '{insert: [(0, 10), (2, 5), (3, 5), (10, 30), (11, 30), (12, 30)], delete: [0]}',*

 * * "'dependencies'": "{insert: [(0, 'collections'), (2, 'typing_extensions'), (3, "*

 * *                   "'_collections_abc'), (5, 'abc'), (6, 'contextlib'), (7, 're'), (10, 'array'), "*

 * *                   "(11, 'ctypes'), (12, 'mmap'), (13, 'pickle')], delete: [8, […]*

```diff
@@ -1,47 +1,62 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843439,
     "dep_lines": [
-        3,
         1,
         2,
+        3,
         4,
         5,
         6,
-        51,
+        7,
+        8,
+        9,
+        1,
+        1,
+        1,
         1,
         1
     ],
     "dep_prios": [
-        5,
         10,
+        10,
+        5,
+        5,
         5,
         5,
         5,
         5,
         5,
         5,
+        30,
+        30,
+        30,
         30
     ],
     "dependencies": [
-        "collections.abc",
+        "collections",
         "sys",
+        "typing_extensions",
+        "_collections_abc",
         "_typeshed",
+        "abc",
+        "contextlib",
+        "re",
         "types",
-        "typing",
-        "typing_extensions",
-        "_thread",
         "builtins",
-        "abc"
+        "array",
+        "ctypes",
+        "mmap",
+        "pickle"
     ],
-    "hash": "7af8d48540c0d86831059b650b1b0b697aa113be33d60df61fa5eeef1699dcd1",
-    "id": "threading",
+    "hash": "78c5d7fda12b38e4f9c30cdbdfbb1dec5e28302fca1d3e1b86d0f48b9cecbb0f",
+    "id": "typing",
     "ignore_all": true,
-    "interface_hash": "2a22c41a46eb4d669992a32e118c0cd74d215c10d295d5b535b5fcbe4e403add",
-    "mtime": 1683082840,
+    "interface_hash": "f5c1fd25973831f458378cc4a43ba97837e94e077191cf2cdf76c3918a4e40c6",
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -75,13 +90,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/threading.pyi",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/typing.pyi",
     "plugin_data": null,
-    "size": 6029,
+    "size": 30303,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/time.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/time.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/time.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/pickle.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6884848484848486%*

 * *Differences: {"'data_mtime'": '1683843439',*

 * * "'dep_lines'": '{insert: [(0, 3), (4, 5), (5, 1), (6, 1), (7, 1)], delete: [2]}',*

 * * "'dep_prios'": '{insert: [(0, 5), (6, 30), (7, 30), (8, 30)]}',*

 * * "'dependencies'": "{insert: [(0, 'collections.abc'), (7, 'array'), (8, 'ctypes'), (9, 'mmap')]}",*

 * * "'hash'": "'01215def75497e54bbe02f50a7b531a9884a9939582b42a2ddf2348b7c8e9d94'",*

 * * "'id'": "'pickle'",*

 * * "'interface_hash'": "'46f362cf2b7503f02d7928b6b9a37e40f1d22ab9d8eef01a9038db8667ca7609'",*

 * * "'mtime'": '1684623296',*

 * * "'path'": "'/h […]*

```diff
@@ -1,38 +1,50 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843439,
     "dep_lines": [
+        3,
         1,
         2,
-        3,
         4,
+        5,
+        1,
+        1,
+        1,
         1,
         1
     ],
     "dep_prios": [
+        5,
         10,
         5,
         5,
         5,
         5,
+        30,
+        30,
+        30,
         30
     ],
     "dependencies": [
+        "collections.abc",
         "sys",
         "_typeshed",
         "typing",
         "typing_extensions",
         "builtins",
-        "abc"
+        "abc",
+        "array",
+        "ctypes",
+        "mmap"
     ],
-    "hash": "81ee1e52c98cc1cd26d7a6aa6d5a9c23d100b4e14cdd725b405a720187e41f8c",
-    "id": "time",
+    "hash": "01215def75497e54bbe02f50a7b531a9884a9939582b42a2ddf2348b7c8e9d94",
+    "id": "pickle",
     "ignore_all": true,
-    "interface_hash": "1cbf1127c399d86b63dab8b6f2658b55c520340ebda63950277141e8cdddc99e",
-    "mtime": 1683082840,
+    "interface_hash": "46f362cf2b7503f02d7928b6b9a37e40f1d22ab9d8eef01a9038db8667ca7609",
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -66,13 +78,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/time.pyi",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/pickle.pyi",
     "plugin_data": null,
-    "size": 3663,
+    "size": 6764,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/tomllib.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/tomllib.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/tomllib.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/termios.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6992063492063492%*

 * *Differences: {"'data_mtime'": '1683843440',*

 * * "'dep_lines'": '{insert: [(1, 2), (3, 4)], delete: [0]}',*

 * * "'dep_prios'": '{insert: [(0, 10)]}',*

 * * "'dependencies'": "{insert: [(0, 'sys'), (3, 'typing_extensions')], delete: [0]}",*

 * * "'hash'": "'2f0f08844c903b2aa786d04a8a488242c21b5912f570b5db810e5afc7ec29ba9'",*

 * * "'id'": "'termios'",*

 * * "'interface_hash'": "'4e4e4b86f862323bacb98d5169dacc01fe5d7021516565360bd9180ab9c9983e'",*

 * * "'mtime'": '1684623296',*

 * * "'path'": "'/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/ […]*

```diff
@@ -1,35 +1,38 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843440,
     "dep_lines": [
-        2,
         1,
+        2,
         3,
+        4,
         1,
         1
     ],
     "dep_prios": [
+        10,
         5,
         5,
         5,
         5,
         30
     ],
     "dependencies": [
-        "collections.abc",
+        "sys",
         "_typeshed",
         "typing",
+        "typing_extensions",
         "builtins",
         "abc"
     ],
-    "hash": "f0faf1b61c8a37d2a2dc1cfd5cfd21097c2b5dfbcd2275bf8b025007a94a56f1",
-    "id": "tomllib",
+    "hash": "2f0f08844c903b2aa786d04a8a488242c21b5912f570b5db810e5afc7ec29ba9",
+    "id": "termios",
     "ignore_all": true,
-    "interface_hash": "0dbff1dc077a42ad9993c43115582bd792aaa05efc3634a4c9447a3bb2a83551",
-    "mtime": 1683082840,
+    "interface_hash": "4e4e4b86f862323bacb98d5169dacc01fe5d7021516565360bd9180ab9c9983e",
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -63,13 +66,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/tomllib.pyi",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/termios.pyi",
     "plugin_data": null,
-    "size": 374,
+    "size": 5095,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/traceback.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/traceback.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/traceback.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/traceback.meta.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'data_mtime'": '1683843440', "'mtime'": '1684623296', "'version_id'": "'1.3.0'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843440,
     "dep_lines": [
         3,
         1,
         2,
         4,
         5,
         6,
@@ -30,15 +30,15 @@
         "builtins",
         "abc"
     ],
     "hash": "2497208e6ba2109935f781184e0161660605078966bace07775dd17c03e462aa",
     "id": "traceback",
     "ignore_all": true,
     "interface_hash": "38f752411b7a39110ec2a5feabe400c4ccc44329cecd6d646f1c38ac8cef8010",
-    "mtime": 1683082840,
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -76,9 +76,9 @@
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
     "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/traceback.pyi",
     "plugin_data": null,
     "size": 8906,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/tty.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/tty.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/tty.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/gettext.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6958333333333333%*

 * *Differences: {"'data_mtime'": '1683843440',*

 * * "'dep_lines'": '{insert: [(0, 4), (4, 5), (5, 6)]}',*

 * * "'dep_prios'": '{insert: [(0, 5), (1, 10), (3, 5)]}',*

 * * "'dependencies'": "{insert: [(0, 'collections.abc'), (1, 'io'), (3, '_typeshed')]}",*

 * * "'hash'": "'05bcfbfe3e5ba3e16560a69ffaeba02e1e3b810e78532bd08cc44617306fc579'",*

 * * "'id'": "'gettext'",*

 * * "'interface_hash'": "'1188a81fd724794ad25bb1216f2375f068fb732d6cfed257da7c28778c9a0fe0'",*

 * * "'mtime'": '1684623296',*

 * * "'path'": "'/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev […]*

```diff
@@ -1,35 +1,44 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843440,
     "dep_lines": [
+        4,
         1,
         2,
         3,
+        5,
+        6,
         1,
         1
     ],
     "dep_prios": [
+        5,
         10,
+        10,
+        5,
         5,
         5,
         5,
         30
     ],
     "dependencies": [
+        "collections.abc",
+        "io",
         "sys",
+        "_typeshed",
         "typing",
         "typing_extensions",
         "builtins",
         "abc"
     ],
-    "hash": "93eadd2f4010b8e595f7f4af4efc698bd6d7a8fe571bfad7e90078f8fdaf26f8",
-    "id": "tty",
+    "hash": "05bcfbfe3e5ba3e16560a69ffaeba02e1e3b810e78532bd08cc44617306fc579",
+    "id": "gettext",
     "ignore_all": true,
-    "interface_hash": "27ec90732677bd7784fffab768dfef3cbd0c62398fce4a10dcde646616f7bd42",
-    "mtime": 1683082840,
+    "interface_hash": "1188a81fd724794ad25bb1216f2375f068fb732d6cfed257da7c28778c9a0fe0",
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -63,13 +72,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/tty.pyi",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/gettext.pyi",
     "plugin_data": null,
-    "size": 430,
+    "size": 6274,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/types.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/types.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/types.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/urllib/__init__.meta.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6622222222222223%*

 * *Differences: {"'data_mtime'": '1683843440',*

 * * "'dep_lines'": '{delete: [6, 5, 4, 3, 1, 0]}',*

 * * "'dep_prios'": '{delete: [5, 4, 3, 2, 1, 0]}',*

 * * "'dependencies'": "{insert: [(2, 'typing')], delete: [8, 5, 4, 3, 2, 1, 0]}",*

 * * "'hash'": "'e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855'",*

 * * "'id'": "'urllib'",*

 * * "'interface_hash'": "'334334ce667cfc17887b547ff7b4339c3fdd4fd11bf5707924d50b6be582668c'",*

 * * "'mtime'": '1684623296',*

 * * "'path'": "'/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/l […]*

```diff
@@ -1,47 +1,29 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843440,
     "dep_lines": [
-        3,
-        16,
         1,
-        2,
-        19,
-        20,
-        607,
         1,
         1
     ],
     "dep_prios": [
         5,
-        5,
-        10,
-        5,
-        5,
-        5,
-        5,
         30,
         30
     ],
     "dependencies": [
-        "collections.abc",
-        "importlib.machinery",
-        "sys",
-        "_typeshed",
-        "typing",
-        "typing_extensions",
         "builtins",
         "abc",
-        "importlib"
+        "typing"
     ],
-    "hash": "705708bbcdf5b70f1ff8d31e9608013c734980d284bf795349dced225c2d046b",
-    "id": "types",
+    "hash": "e3b0c44298fc1c149afbf4c8996fb92427ae41e4649b934ca495991b7852b855",
+    "id": "urllib",
     "ignore_all": true,
-    "interface_hash": "d837e1814d54b77a49618bbb00979340d14c37e5d61c6843e08957a9c2fe5c38",
-    "mtime": 1683082840,
+    "interface_hash": "334334ce667cfc17887b547ff7b4339c3fdd4fd11bf5707924d50b6be582668c",
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -75,13 +57,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/types.pyi",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/urllib/__init__.pyi",
     "plugin_data": null,
-    "size": 20811,
+    "size": 0,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/typing.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/typing.data.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999803117269634%*

 * *Differences: {"'names'": "{'Callable': {'node': {'flags': {delete: [1]}}}, 'ClassVar': {'node': {'flags': "*

 * *            "{delete: [1]}}}, 'Generic': {'node': {'flags': {delete: [1]}}}, 'Never': {'node': "*

 * *            "{'flags': {delete: [1]}}}, 'NoReturn': {'node': {'flags': {delete: [1]}}}, "*

 * *            "'Protocol': {'node': {'flags': {delete: [1]}}}, 'Text': {'node': {'line': 640}}, "*

 * *            "'Type': {'node': {'flags': {delete: [1]}}}, 'Union': {'node': {'flags': {delete: "*

 * *            "[1]}}}, '_get_type_hints_ […]*

```diff
@@ -3745,16 +3745,15 @@
         },
         "Callable": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "Var",
                 "flags": [
-                    "is_ready",
-                    "has_explicit_value"
+                    "is_ready"
                 ],
                 "fullname": "typing.Callable",
                 "name": "Callable",
                 "type": "typing._SpecialForm"
             }
         },
         "ChainMap": {
@@ -3790,16 +3789,15 @@
         },
         "ClassVar": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "Var",
                 "flags": [
-                    "is_ready",
-                    "has_explicit_value"
+                    "is_ready"
                 ],
                 "fullname": "typing.ClassVar",
                 "name": "ClassVar",
                 "type": "typing._SpecialForm"
             }
         },
         "CodeType": {
@@ -8250,16 +8248,15 @@
         },
         "Generic": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "Var",
                 "flags": [
-                    "is_ready",
-                    "has_explicit_value"
+                    "is_ready"
                 ],
                 "fullname": "typing.Generic",
                 "name": "Generic",
                 "type": "typing._SpecialForm"
             }
         },
         "GenericAlias": {
@@ -22609,16 +22606,15 @@
         },
         "Never": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "Var",
                 "flags": [
-                    "is_ready",
-                    "has_explicit_value"
+                    "is_ready"
                 ],
                 "fullname": "typing.Never",
                 "name": "Never",
                 "type": "typing._SpecialForm"
             }
         },
         "NewType": {
@@ -22920,16 +22916,15 @@
         },
         "NoReturn": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "Var",
                 "flags": [
-                    "is_ready",
-                    "has_explicit_value"
+                    "is_ready"
                 ],
                 "fullname": "typing.NoReturn",
                 "name": "NoReturn",
                 "type": "typing._SpecialForm"
             }
         },
         "NotRequired": {
@@ -23790,16 +23785,15 @@
         },
         "Protocol": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "Var",
                 "flags": [
-                    "is_ready",
-                    "has_explicit_value"
+                    "is_ready"
                 ],
                 "fullname": "typing.Protocol",
                 "name": "Protocol",
                 "type": "typing._SpecialForm"
             }
         },
         "ReadableBuffer": {
@@ -26182,15 +26176,15 @@
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "TypeAlias",
                 "alias_tvars": [],
                 "column": 0,
                 "fullname": "typing.Text",
-                "line": 646,
+                "line": 640,
                 "no_args": true,
                 "normalized": false,
                 "target": "builtins.str"
             }
         },
         "TextIO": {
             ".class": "SymbolTableNode",
@@ -26882,16 +26876,15 @@
         },
         "Type": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "Var",
                 "flags": [
-                    "is_ready",
-                    "has_explicit_value"
+                    "is_ready"
                 ],
                 "fullname": "typing.Type",
                 "name": "Type",
                 "type": "typing._SpecialForm"
             }
         },
         "TypeAlias": {
@@ -27592,16 +27585,15 @@
         },
         "Union": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "Var",
                 "flags": [
-                    "is_ready",
-                    "has_explicit_value"
+                    "is_ready"
                 ],
                 "fullname": "typing.Union",
                 "name": "Union",
                 "type": "typing._SpecialForm"
             }
         },
         "UnionType": {
@@ -29462,15 +29454,15 @@
             "kind": "Gdef",
             "module_public": false,
             "node": {
                 ".class": "TypeAlias",
                 "alias_tvars": [],
                 "column": 0,
                 "fullname": "typing._get_type_hints_obj_allowed_types",
-                "line": 741,
+                "line": 735,
                 "no_args": false,
                 "normalized": false,
                 "target": {
                     ".class": "UnionType",
                     "items": [
                         "builtins.object",
                         {
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/typing.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/click/parser.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6659090909090909%*

 * *Differences: {"'data_mtime'": '1683843441',*

 * * "'dep_lines'": '{insert: [(0, 29), (1, 36), (2, 24), (3, 25), (4, 26), (5, 35), (6, 140), (7, '*

 * *                '395), (9, 1), (10, 1)], delete: [8, 7, 6, 5, 4, 3, 2, 1]}',*

 * * "'dep_prios'": '{insert: [(1, 25), (2, 10), (5, 25), (6, 20), (7, 20), (9, 30), (10, 30), (11, '*

 * *                '30)], delete: [5, 4, 3, 2, 1, 0]}',*

 * * "'dependencies'": "{insert: [(0, 'click.exceptions'), (1, 'click.core'), (2, 'typing'), (4, "*

 * *                   "'gettext'), (6, 'shlex'), (7, 'difflib'), […]*

```diff
@@ -1,62 +1,68 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843441,
     "dep_lines": [
+        29,
+        36,
+        24,
+        25,
+        26,
+        35,
+        140,
+        395,
+        1,
+        1,
         1,
-        2,
-        3,
-        4,
-        5,
-        6,
-        7,
-        8,
-        9,
         1,
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
-        10,
-        10,
-        5,
-        5,
-        5,
-        5,
         5,
+        25,
+        10,
         5,
         5,
+        25,
+        20,
+        20,
         5,
         30,
         30,
         30,
+        30,
+        30,
+        30,
         30
     ],
     "dependencies": [
+        "click.exceptions",
+        "click.core",
+        "typing",
         "collections",
-        "sys",
+        "gettext",
         "typing_extensions",
-        "_collections_abc",
+        "shlex",
+        "difflib",
+        "builtins",
         "_typeshed",
         "abc",
-        "contextlib",
-        "re",
-        "types",
-        "builtins",
         "array",
         "ctypes",
         "mmap",
-        "pickle"
+        "pickle",
+        "types"
     ],
-    "hash": "c1fca6577e709cdeb3e8511b94e06063867af2623ea098b52441dfd559f76a6f",
-    "id": "typing",
+    "hash": "70012dd6e411f20ab7f92f72b2a6d553e7dd01936f8a5c70e11789fd3d4e40c9",
+    "id": "click.parser",
     "ignore_all": true,
-    "interface_hash": "068487c61589cc618c89dfef723b16a49e6a2f2cc4b4b15335eaa4aa2b88829a",
-    "mtime": 1683082840,
+    "interface_hash": "fce531f96966c28a3fd4a137c86130b3972e1d4153d0aadd4146bf0e87250381",
+    "mtime": 1684623295,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -90,13 +96,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/typing.pyi",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib/python3.11/site-packages/click/parser.py",
     "plugin_data": null,
-    "size": 30735,
+    "size": 19044,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/typing_extensions.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/typing_extensions.data.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999965790914066%*

 * *Differences: {"'names'": "{'Protocol': {'node': {'flags': {delete: [1]}}}}"}*

```diff
@@ -698,16 +698,15 @@
         },
         "Protocol": {
             ".class": "SymbolTableNode",
             "kind": "Gdef",
             "node": {
                 ".class": "Var",
                 "flags": [
-                    "is_ready",
-                    "has_explicit_value"
+                    "is_ready"
                 ],
                 "fullname": "typing_extensions.Protocol",
                 "name": "Protocol",
                 "type": "typing_extensions._SpecialForm"
             }
         },
         "Required": {
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/typing_extensions.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/_codecs.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6711764705882353%*

 * *Differences: {"'data_mtime'": '1683843440',*

 * * "'dep_lines'": '{insert: [(0, 4), (6, 1), (7, 1), (8, 1), (9, 1), (10, 1)], delete: [7, 4, 0]}',*

 * * "'dep_prios'": '{insert: [(7, 30), (8, 30), (9, 30), (10, 30), (11, 30)], delete: [4, 1]}',*

 * * "'dependencies'": "{insert: [(1, 'codecs'), (4, 'typing'), (5, 'typing_extensions'), (7, 'abc'), "*

 * *                   "(8, 'array'), (9, 'ctypes'), (10, 'mmap'), (11, 'pickle')], delete: [7, 5, 4, "*

 * *                   '2, 1]}',*

 * * "'hash'": "'70e3defc1875bd08c24cbe869d9c14280401dc8b591637db […]*

```diff
@@ -1,47 +1,56 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843440,
     "dep_lines": [
-        7,
+        4,
         1,
         2,
         3,
-        4,
         5,
         6,
-        36,
+        1,
+        1,
+        1,
+        1,
+        1,
         1
     ],
     "dep_prios": [
         5,
         10,
         10,
-        10,
         5,
         5,
         5,
         5,
-        5
+        30,
+        30,
+        30,
+        30,
+        30
     ],
     "dependencies": [
         "collections.abc",
-        "abc",
-        "collections",
+        "codecs",
         "sys",
-        "typing",
-        "_collections_abc",
         "_typeshed",
-        "types",
-        "builtins"
+        "typing",
+        "typing_extensions",
+        "builtins",
+        "abc",
+        "array",
+        "ctypes",
+        "mmap",
+        "pickle"
     ],
-    "hash": "cc94cf062e3157caad2767a45b964b3433d2e1010668a682781afbf902a0999e",
-    "id": "typing_extensions",
+    "hash": "70e3defc1875bd08c24cbe869d9c14280401dc8b591637db091aad6a71684e1d",
+    "id": "_codecs",
     "ignore_all": true,
-    "interface_hash": "202b4532a42427d53474bf85e4bfeb05eacccba2cdc647f44302f00719a2e961",
-    "mtime": 1683082840,
+    "interface_hash": "9f0ae4ebfc6b4ad5b744bba8fd125716016d5c00b34dfc96e52aceb26dcfe0c0",
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -75,13 +84,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/typing_extensions.pyi",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/_codecs.pyi",
     "plugin_data": null,
-    "size": 9856,
+    "size": 7280,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/uuid.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/uuid.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/uuid.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/email/charset.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6659090909090909%*

 * *Differences: {"'data_mtime'": '1683843440',*

 * * "'dep_lines'": '{delete: [6, 5, 4, 3, 2, 1, 0]}',*

 * * "'dep_prios'": '{delete: [8, 7, 6, 5, 2, 1, 0]}',*

 * * "'dependencies'": "{insert: [(0, 'collections.abc')], delete: [9, 8, 7, 6, 3, 2, 1, 0]}",*

 * * "'hash'": "'7eb946e66f91d483704797cfcbe5603351fd555cb7655a0e5444e653fcd491d7'",*

 * * "'id'": "'email.charset'",*

 * * "'interface_hash'": "'f87f2e3130de71b46db48f0b4c53f1a3a30d08e4024f0c757230f1b312dcfc2a'",*

 * * "'mtime'": '1684623296',*

 * * "'path'": "'/home/gotmax/Sync/git-repos/packaging/fedora_rpms […]*

```diff
@@ -1,53 +1,32 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843440,
     "dep_lines": [
         1,
-        2,
-        3,
-        4,
-        1,
-        1,
-        1,
-        1,
         1,
         1,
         1
     ],
     "dep_prios": [
-        10,
-        5,
         5,
         5,
-        5,
-        30,
-        30,
-        30,
-        30,
         30,
         30
     ],
     "dependencies": [
-        "sys",
-        "_typeshed",
-        "enum",
-        "typing_extensions",
+        "collections.abc",
         "builtins",
         "abc",
-        "array",
-        "ctypes",
-        "mmap",
-        "pickle",
         "typing"
     ],
-    "hash": "3dc073e65788f3027a8839ccc311cefc9291141fc8818035bb976a007346b615",
-    "id": "uuid",
+    "hash": "7eb946e66f91d483704797cfcbe5603351fd555cb7655a0e5444e653fcd491d7",
+    "id": "email.charset",
     "ignore_all": true,
-    "interface_hash": "5184910ef79cb98c9c1c17ad419e263fc62447917ee959d42c10922c84c3c15d",
-    "mtime": 1683082840,
+    "interface_hash": "f87f2e3130de71b46db48f0b4c53f1a3a30d08e4024f0c757230f1b312dcfc2a",
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -81,13 +60,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/uuid.pyi",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/email/charset.pyi",
     "plugin_data": null,
-    "size": 2343,
+    "size": 1077,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/warnings.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/warnings.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/warnings.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/importlib/abc.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6731359649122807%*

 * *Differences: {"'data_mtime'": '1683843440',*

 * * "'dep_lines'": '{insert: [(0, 14), (1, 15), (4, 3), (6, 13), (7, 16), (8, 17), (9, 18), (10, 1), '*

 * *                '(11, 1), (12, 1)], delete: [5, 4, 0]}',*

 * * "'dep_prios'": '{insert: [(0, 5), (2, 10), (3, 10), (5, 5), (11, 30), (12, 30), (13, 30)]}',*

 * * "'dependencies'": "{insert: [(1, 'importlib.machinery'), (2, '_ast'), (5, '_typeshed'), (6, "*

 * *                   "'abc'), (7, 'io'), (11, 'array'), (12, 'ctypes'), (13, 'mmap'), (14, 'os'), "*

 * *                   "(15, 'pickle')],  […]*

```diff
@@ -1,47 +1,68 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843440,
     "dep_lines": [
-        3,
+        14,
+        15,
         1,
         2,
+        3,
         4,
-        5,
-        6,
+        13,
+        16,
+        17,
+        18,
+        1,
+        1,
+        1,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
+        5,
+        10,
         10,
+        10,
+        5,
         5,
         5,
         5,
         5,
         5,
         30,
+        30,
+        30,
+        30,
         30
     ],
     "dependencies": [
         "collections.abc",
+        "importlib.machinery",
+        "_ast",
         "sys",
-        "_warnings",
         "types",
+        "_typeshed",
+        "abc",
+        "io",
         "typing",
         "typing_extensions",
         "builtins",
-        "_typeshed",
-        "abc"
+        "array",
+        "ctypes",
+        "mmap",
+        "os",
+        "pickle"
     ],
-    "hash": "9a991da6c7cb550f45efd87385ec22f61a45c69511ab3af2594b6d1ce0487343",
-    "id": "warnings",
+    "hash": "2ef3e7cd4f57d7730ef462502b680809572a49eb21b9555784a5744ab4e70c3f",
+    "id": "importlib.abc",
     "ignore_all": true,
-    "interface_hash": "6213d76a67fb20859c74dfa0275499ced0d593f9f03d850e7b0aae112d04c31a",
-    "mtime": 1683082840,
+    "interface_hash": "27fdc7881cd5848e3fd5c8b1552d0e9e76bf0628ec4c7d0fccea76cdfa697ff6",
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -75,13 +96,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/warnings.pyi",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/importlib/abc.pyi",
     "plugin_data": null,
-    "size": 3682,
+    "size": 7380,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/weakref.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/weakref.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/weakref.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/weakref.meta.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8333333333333334%*

 * *Differences: {"'data_mtime'": '1683843440',*

 * * "'hash'": "'2f4d35940e2c4b0c2eb1bf2a5ba693d7594eb77431269f2de4e9683bb3f3d9e2'",*

 * * "'mtime'": '1684623296',*

 * * "'size'": '6020',*

 * * "'version_id'": "'1.3.0'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843440,
     "dep_lines": [
         13,
         1,
         2,
         3,
         12,
         14,
@@ -29,19 +29,19 @@
         "_weakref",
         "_weakrefset",
         "typing",
         "typing_extensions",
         "builtins",
         "abc"
     ],
-    "hash": "463ba4740adbdd75450c7c4fea5012ec60e4f42b6aa431183dae531fdfc97e7e",
+    "hash": "2f4d35940e2c4b0c2eb1bf2a5ba693d7594eb77431269f2de4e9683bb3f3d9e2",
     "id": "weakref",
     "ignore_all": true,
     "interface_hash": "644f7bc5689ba412a14ab886293856443d34872d281e2b3802fbe74558d84a62",
-    "mtime": 1683082840,
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -77,11 +77,11 @@
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
     "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/weakref.pyi",
     "plugin_data": null,
-    "size": 6021,
+    "size": 6020,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/webbrowser.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/webbrowser.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/webbrowser.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/typer/__init__.meta.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6631024531024531%*

 * *Differences: {"'data_mtime'": '1683843441',*

 * * "'dep_lines'": '{insert: [(0, 7), (1, 10), (2, 22), (3, 29), (4, 30), (5, 32), (6, 38), (7, 5)], '*

 * *                'delete: [3, 2, 0]}',*

 * * "'dep_prios'": '{insert: [(0, 5), (1, 5), (4, 5), (5, 5), (9, 30)]}',*

 * * "'dependencies'": "{insert: [(0, 'click.exceptions'), (1, 'click.termui'), (2, 'click.utils'), "*

 * *                   "(3, 'typer.colors'), (4, 'typer.main'), (5, 'typer.models'), (6, "*

 * *                   "'typer.params'), (7, 'shutil'), (9, 'abc')], delete: [3, 2, 1, 0]}" […]*

```diff
@@ -1,38 +1,53 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843441,
     "dep_lines": [
-        3,
+        7,
+        10,
+        22,
+        29,
+        30,
+        32,
+        38,
+        5,
         1,
-        2,
-        4,
         1,
         1
     ],
     "dep_prios": [
         5,
+        5,
+        5,
         10,
         5,
         5,
         5,
+        5,
+        5,
+        30,
         30
     ],
     "dependencies": [
-        "collections.abc",
-        "sys",
-        "abc",
-        "typing_extensions",
+        "click.exceptions",
+        "click.termui",
+        "click.utils",
+        "typer.colors",
+        "typer.main",
+        "typer.models",
+        "typer.params",
+        "shutil",
         "builtins",
+        "abc",
         "typing"
     ],
-    "hash": "5eafef06c53dd8b7d5ef6d7ece9ac1448f3f153c6061af7e9701fdf92f9e307c",
-    "id": "webbrowser",
+    "hash": "c5ff549135bc942c56bd006b25e9430d11aca40c240e6d2f7762a28e11ea3f28",
+    "id": "typer",
     "ignore_all": true,
-    "interface_hash": "796e455516416541b15a08d8bc8461efcc8d9a0bd7820fe08ee46ae7b4bcdf5c",
-    "mtime": 1683082840,
+    "interface_hash": "67656c94cc4fb27dcc533749f8b383284f1fe2ca9d49490955bd0df882a8877e",
+    "mtime": 1684623295,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -66,13 +81,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/webbrowser.pyi",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib/python3.11/site-packages/typer/__init__.py",
     "plugin_data": null,
-    "size": 2527,
+    "size": 1602,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/_typeshed/__init__.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/_typeshed/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/_typeshed/__init__.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/_typeshed/__init__.meta.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'data_mtime'": '1683843440', "'mtime'": '1684623296', "'version_id'": "'1.3.0'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843440,
     "dep_lines": [
         10,
         5,
         6,
         7,
         8,
         9,
@@ -45,15 +45,15 @@
         "builtins",
         "abc"
     ],
     "hash": "b51d2b79a156278383c840da565bf3312ef8e715015d3a44096c0c5eac13393d",
     "id": "_typeshed",
     "ignore_all": true,
     "interface_hash": "fb51381900accaaa64efe44910a327f5b9f0cbf3692ea7d1689793a9921939ac",
-    "mtime": 1683082840,
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -91,9 +91,9 @@
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
     "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/_typeshed/__init__.pyi",
     "plugin_data": null,
     "size": 11016,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/click/__init__.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/click/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/click/__init__.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/click/__init__.meta.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'data_mtime'": '1683843441', "'mtime'": '1684623295', "'version_id'": "'1.3.0'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681571164,
+    "data_mtime": 1683843441,
     "dep_lines": [
         7,
         16,
         27,
         36,
         38,
         39,
@@ -42,15 +42,15 @@
         "abc",
         "typing"
     ],
     "hash": "ad004bbadaa0fb3ea6f273b38af21f8a00e7fde9a28c1fdd2aff4167614d8b9b",
     "id": "click",
     "ignore_all": true,
     "interface_hash": "8c899cf720ce6b8fe72c27ca3df02b68e28fd5b6f5f9aea405af3b5e24199de1",
-    "mtime": 1683082839,
+    "mtime": 1684623295,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -88,9 +88,9 @@
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
     "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib/python3.11/site-packages/click/__init__.py",
     "plugin_data": null,
     "size": 3138,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/click/_compat.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/click/_compat.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/click/_compat.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/click/_compat.meta.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'data_mtime'": '1683843440', "'mtime'": '1684623295', "'version_id'": "'1.3.0'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681571164,
+    "data_mtime": 1683843440,
     "dep_lines": [
         1,
         2,
         3,
         4,
         5,
         6,
@@ -69,15 +69,15 @@
         "types",
         "typing_extensions"
     ],
     "hash": "2481cb62cec9cf3e0a4fdb7e76ce28e230732e39f00a22502aababfb98b008a2",
     "id": "click._compat",
     "ignore_all": true,
     "interface_hash": "072f2de468d08716c62e3f5f42e335158eb60e9a0e995ff0aa12d403f60c7ee0",
-    "mtime": 1683082839,
+    "mtime": 1684623295,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -115,9 +115,9 @@
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
     "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib/python3.11/site-packages/click/_compat.py",
     "plugin_data": null,
     "size": 18810,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/click/_termui_impl.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/click/_termui_impl.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/click/_termui_impl.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/click/_termui_impl.meta.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'data_mtime'": '1683843441', "'mtime'": '1684623295', "'version_id'": "'1.3.0'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681571164,
+    "data_mtime": 1683843441,
     "dep_lines": [
         14,
         22,
         23,
         555,
         6,
         7,
@@ -105,15 +105,15 @@
         "typing_extensions",
         "urllib"
     ],
     "hash": "a8ae827f2e26445c6fc44f1dc9af110612e9482f078c5fa5bc173a68dacf7708",
     "id": "click._termui_impl",
     "ignore_all": true,
     "interface_hash": "b3be6628d7c55103da2cc2c339678504d8ce42ac8f08feb31602c7b39f0dac25",
-    "mtime": 1683082839,
+    "mtime": 1684623295,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -151,9 +151,9 @@
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
     "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib/python3.11/site-packages/click/_termui_impl.py",
     "plugin_data": null,
     "size": 23451,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/click/_textwrap.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/click/_textwrap.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/click/_textwrap.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/email/errors.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.692063492063492%*

 * *Differences: {"'data_mtime'": '1683843440',*

 * * "'dep_lines'": '{delete: [2, 1]}',*

 * * "'dep_prios'": '{delete: [2, 0]}',*

 * * "'dependencies'": "{insert: [(0, 'sys'), (4, 'typing')], delete: [6, 2, 1, 0]}",*

 * * "'hash'": "'ca7498bfe12fcf0148a719c9bfa9f40ff037ddb6e1308f6101d338a8b9a859b9'",*

 * * "'id'": "'email.errors'",*

 * * "'interface_hash'": "'392541fc8423d0fcd6bd24011421b115260845ea897f4b51074fd079ea362025'",*

 * * "'mtime'": '1684623296',*

 * * "'path'": "'/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11 […]*

```diff
@@ -1,41 +1,35 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843440,
     "dep_lines": [
         1,
-        2,
-        3,
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
         10,
-        10,
-        5,
         5,
         30,
         30,
         30
     ],
     "dependencies": [
-        "textwrap",
-        "typing",
-        "contextlib",
+        "sys",
         "builtins",
         "_typeshed",
         "abc",
-        "typing_extensions"
+        "typing"
     ],
-    "hash": "d747d0eb839c05432e2bb985be1f37eb7feea0ec4f95122d64198acd12438286",
-    "id": "click._textwrap",
+    "hash": "ca7498bfe12fcf0148a719c9bfa9f40ff037ddb6e1308f6101d338a8b9a859b9",
+    "id": "email.errors",
     "ignore_all": true,
-    "interface_hash": "7434e38ac65160d707a6362d23cee3aab3b4085cebbe903a6fb6b9b9c2b45038",
-    "mtime": 1683082839,
+    "interface_hash": "392541fc8423d0fcd6bd24011421b115260845ea897f4b51074fd079ea362025",
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -69,13 +63,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib/python3.11/site-packages/click/_textwrap.py",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/email/errors.pyi",
     "plugin_data": null,
-    "size": 1353,
+    "size": 1533,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/click/core.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/click/core.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/click/core.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/click/termui.meta.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6818986131037781%*

 * *Differences: {"'data_mtime'": '1683843441',*

 * * "'dep_lines'": '{insert: [(0, 9), (1, 12), (2, 14), (3, 15), (4, 18), (5, 22), (13, 53), (14, 1), '*

 * *                '(15, 1)], delete: [22, 21, 20, 19, 18, 17, 9, 8, 7, 6, 5, 4, 3, 2, 1, 0]}',*

 * * "'dep_prios'": '{insert: [(15, 30), (16, 30)], delete: [22, 19, 18, 17, 16, 8, 2, 1, 0]}',*

 * * "'dependencies'": "{insert: [(0, 'click._compat'), (3, 'click.types'), (5, 'click._termui_impl'), "*

 * *                   "(7, 'io'), (8, 'itertools'), (13, 'getpass'), (18, 'click.core'), (19, "*

 * *  […]*

```diff
@@ -1,116 +1,95 @@
 {
-    "data_mtime": 1681571164,
+    "data_mtime": 1683843441,
     "dep_lines": [
-        7,
-        16,
-        17,
-        23,
-        25,
-        27,
-        30,
-        33,
-        42,
-        1839,
+        9,
+        12,
+        14,
+        15,
+        18,
+        22,
         1,
         2,
         3,
         4,
         5,
         6,
         7,
-        8,
-        10,
-        12,
-        14,
-        16,
-        41,
+        53,
+        1,
+        1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
-        10,
-        10,
-        5,
         5,
         5,
         5,
         5,
         5,
         20,
-        20,
         10,
         10,
         10,
         10,
         10,
         10,
-        20,
-        5,
-        5,
-        5,
         5,
         20,
-        25,
         5,
         30,
         30,
         30,
         30,
         30,
         30,
         30,
+        30,
+        30,
         30
     ],
     "dependencies": [
-        "collections.abc",
-        "click.types",
+        "click._compat",
         "click.exceptions",
-        "click.formatting",
         "click.globals",
-        "click.parser",
-        "click.termui",
+        "click.types",
         "click.utils",
-        "click.shell_completion",
-        "click.decorators",
-        "enum",
-        "errno",
+        "click._termui_impl",
         "inspect",
+        "io",
+        "itertools",
         "os",
         "sys",
         "typing",
-        "collections",
-        "contextlib",
-        "functools",
         "gettext",
-        "itertools",
-        "click",
-        "typing_extensions",
+        "getpass",
         "builtins",
-        "_collections_abc",
         "_typeshed",
         "abc",
         "array",
+        "click.core",
+        "contextlib",
         "ctypes",
         "mmap",
         "pickle",
-        "types"
+        "types",
+        "typing_extensions"
     ],
-    "hash": "9b3f3b6d810acc8a0d6046b9e8114088e267bedd58d0bfa2ef00f8fd979c89e1",
-    "id": "click.core",
+    "hash": "00205054ebc50934aab43e5544478201d46d94777e22695af8bb5ee3049f3230",
+    "id": "click.termui",
     "ignore_all": true,
-    "interface_hash": "69e4ba6a6af7fc096a0fe1e35ebd83c7d4ed8cf17d452e3c214023b6d6d16a0b",
-    "mtime": 1683082840,
+    "interface_hash": "9cc7785b6d19ee5cf6aafb9bbbfb1a9e634723918a98bd089ddb2be9d5abe167",
+    "mtime": 1684623295,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -144,13 +123,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib/python3.11/site-packages/click/core.py",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib/python3.11/site-packages/click/termui.py",
     "plugin_data": null,
-    "size": 112782,
+    "size": 28355,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/click/decorators.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/click/decorators.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/click/decorators.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/click/decorators.meta.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'data_mtime'": '1683843441', "'mtime'": '1684623295', "'version_id'": "'1.3.0'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681571164,
+    "data_mtime": 1683843441,
     "dep_lines": [
         7,
         13,
         14,
         433,
         1,
         2,
@@ -53,15 +53,15 @@
         "click.types",
         "typing_extensions"
     ],
     "hash": "ca8df3bf38149b9abb8790978f257aab787f3c902251a7a6d7bf335f07565052",
     "id": "click.decorators",
     "ignore_all": true,
     "interface_hash": "1a606dded10ebabc3518288a37620499d18dc1166a8090b6a685e896dc4f7eef",
-    "mtime": 1683082840,
+    "mtime": 1684623295,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -101,9 +101,9 @@
     },
     "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib/python3.11/site-packages/click/decorators.py",
     "plugin_data": null,
     "size": 16350,
     "suppressed": [
         "importlib_metadata"
     ],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/click/exceptions.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/click/exceptions.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/click/exceptions.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/typer/models.meta.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6763627819548872%*

 * *Differences: {"'data_mtime'": '1683843441',*

 * * "'dep_lines'": '{insert: [(0, 18), (1, 22), (2, 24), (3, 25), (7, 16), (8, 1)], delete: [2, 1, '*

 * *                '0]}',*

 * * "'dep_prios'": '{insert: [(1, 25), (2, 25), (7, 10), (9, 30)], delete: [0]}',*

 * * "'dependencies'": "{insert: [(0, 'typer._compat_utils'), (1, 'click.shell_completion'), (2, "*

 * *                   "'typer.core'), (3, 'typer.main'), (4, 'inspect'), (5, 'io'), (7, 'click'), "*

 * *                   "(10, 'click.core'), (12, 'enum')], delete: [7, 5, 3, 2, 1, 0]}",*

 * * "'h […]*

```diff
@@ -1,50 +1,59 @@
 {
-    "data_mtime": 1681571164,
+    "data_mtime": 1683843441,
     "dep_lines": [
-        6,
-        7,
-        10,
+        18,
+        22,
+        24,
+        25,
         1,
         2,
         3,
+        16,
+        1,
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
-        5,
+        25,
+        25,
         25,
         10,
         10,
         5,
+        10,
         5,
         30,
         30,
+        30,
         30
     ],
     "dependencies": [
-        "click._compat",
-        "click.utils",
-        "click.core",
-        "os",
+        "typer._compat_utils",
+        "click.shell_completion",
+        "typer.core",
+        "typer.main",
+        "inspect",
+        "io",
         "typing",
-        "gettext",
+        "click",
         "builtins",
-        "_typeshed",
         "abc",
-        "click.types"
+        "click.core",
+        "click.types",
+        "enum"
     ],
-    "hash": "ee00da2c6b8564178237063d11132c176f99dd1f45bead3d65ce886522a3b1ea",
-    "id": "click.exceptions",
+    "hash": "0d625201001a209a45048efff3154017d132f4d3479b8755ea29f6b81ecdeca9",
+    "id": "typer.models",
     "ignore_all": true,
-    "interface_hash": "f24b97a0246f7b5bf481f49537df8452800f697851e761591030da46680acef9",
-    "mtime": 1683082840,
+    "interface_hash": "db492461bb763161350ae9740b2d8fde7036d8a2b37090afef47e1d08451eebe",
+    "mtime": 1684623295,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -78,13 +87,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib/python3.11/site-packages/click/exceptions.py",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib/python3.11/site-packages/typer/models.py",
     "plugin_data": null,
-    "size": 9167,
+    "size": 15981,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/click/formatting.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/click/formatting.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/click/formatting.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/click/formatting.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'data_mtime'": '1683843441', "'mtime'": '1684623295', "'version_id'": "'1.3.0'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681571164,
+    "data_mtime": 1683843441,
     "dep_lines": [
         5,
         6,
         54,
         1,
         2,
         3,
@@ -48,15 +48,15 @@
         "textwrap",
         "typing_extensions"
     ],
     "hash": "16b7f4fb95b7dfe968c98fe2f6aaf05d1f3e4939d6de6e60bf2c4b554772c729",
     "id": "click.formatting",
     "ignore_all": true,
     "interface_hash": "dc5adce89ec5b3723e65b36217bdce3880282f03b619511e345da40d0a80355d",
-    "mtime": 1683082840,
+    "mtime": 1684623295,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -94,9 +94,9 @@
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
     "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib/python3.11/site-packages/click/formatting.py",
     "plugin_data": null,
     "size": 9706,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/click/globals.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/click/globals.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/click/globals.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/typing_extensions.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6589160839160839%*

 * *Differences: {"'data_mtime'": '1683843439',*

 * * "'dep_lines'": '{insert: [(0, 7), (3, 3), (4, 4), (6, 6), (7, 36)], delete: [4, 0]}',*

 * * "'dep_prios'": '{insert: [(0, 5), (1, 10), (2, 10), (6, 5), (7, 5), (8, 5)], delete: [5, 3, 0]}',*

 * * "'dependencies'": "{insert: [(0, 'collections.abc'), (1, 'abc'), (2, 'collections'), (3, 'sys'), "*

 * *                   "(5, '_collections_abc'), (6, '_typeshed'), (7, 'types')], delete: [5, 3, 2, "*

 * *                   '0]}',*

 * * "'hash'": "'44b4201aff73a621deda9aa2be5ee1f0260fb30c6bda0dbefc887a3c65 […]*

```diff
@@ -1,38 +1,47 @@
 {
-    "data_mtime": 1681571164,
+    "data_mtime": 1683843439,
     "dep_lines": [
-        6,
+        7,
         1,
         2,
+        3,
+        4,
         5,
-        1,
+        6,
+        36,
         1
     ],
     "dep_prios": [
-        25,
+        5,
         10,
+        10,
+        10,
+        5,
+        5,
         5,
-        25,
         5,
-        30
+        5
     ],
     "dependencies": [
-        "click.core",
+        "collections.abc",
+        "abc",
+        "collections",
+        "sys",
         "typing",
-        "threading",
-        "typing_extensions",
-        "builtins",
-        "abc"
+        "_collections_abc",
+        "_typeshed",
+        "types",
+        "builtins"
     ],
-    "hash": "4cffaa33cf124f373b7f5dbb877e530ffbfddb41607ce0f6130cea034a04f175",
-    "id": "click.globals",
+    "hash": "44b4201aff73a621deda9aa2be5ee1f0260fb30c6bda0dbefc887a3c65a04119",
+    "id": "typing_extensions",
     "ignore_all": true,
-    "interface_hash": "ae61ea35093262c5c00b99651085c8dac525ebd30575b9c101234bc83a3c55bf",
-    "mtime": 1683082840,
+    "interface_hash": "9c6e256eefd545477b69e1392c452cb23b7a68be78408344893cad567b833008",
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -66,13 +75,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib/python3.11/site-packages/click/globals.py",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/typing_extensions.pyi",
     "plugin_data": null,
-    "size": 1961,
+    "size": 9843,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/click/parser.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/click/parser.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/click/parser.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/importlib/metadata/__init__.meta.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6498974709501025%*

 * *Differences: {"'data_mtime'": '1683843440',*

 * * "'dep_lines'": '{insert: [(0, 31), (1, 5), (2, 6), (3, 7), (5, 2), (6, 3), (7, 4), (8, 8), (9, '*

 * *                '10), (10, 11), (11, 12)], delete: [8, 7, 6, 5, 4, 3, 2, 1, 0]}',*

 * * "'dep_prios'": '{insert: [(1, 5), (2, 5), (3, 5), (6, 10), (9, 5), (10, 5), (11, 5), (12, 5)], '*

 * *                'delete: [10, 9, 7, 6, 5, 1]}',*

 * * "'dependencies'": "{insert: [(0, 'importlib.metadata._meta'), (1, 'collections.abc'), (2, "*

 * *                   "'email.message'), (3, 'importlib.abc'), (4 […]*

```diff
@@ -1,53 +1,59 @@
 {
-    "data_mtime": 1681571164,
+    "data_mtime": 1683843440,
     "dep_lines": [
-        29,
-        36,
-        24,
-        25,
-        26,
-        35,
-        140,
-        395,
-        1,
+        31,
+        5,
+        6,
+        7,
         1,
+        2,
+        3,
+        4,
+        8,
+        10,
+        11,
+        12,
         1
     ],
     "dep_prios": [
         5,
-        25,
+        5,
+        5,
+        5,
         10,
         5,
+        10,
+        5,
+        5,
         5,
-        25,
-        20,
-        20,
         5,
-        30,
-        30
+        5,
+        5
     ],
     "dependencies": [
-        "click.exceptions",
-        "click.core",
+        "importlib.metadata._meta",
+        "collections.abc",
+        "email.message",
+        "importlib.abc",
+        "abc",
+        "pathlib",
+        "sys",
+        "_typeshed",
+        "os",
+        "re",
         "typing",
-        "collections",
-        "gettext",
         "typing_extensions",
-        "shlex",
-        "difflib",
-        "builtins",
-        "_typeshed",
-        "abc"
+        "builtins"
     ],
-    "hash": "70012dd6e411f20ab7f92f72b2a6d553e7dd01936f8a5c70e11789fd3d4e40c9",
-    "id": "click.parser",
+    "hash": "ae422af81eff03dc03edf2ef5f854e32c69b6b23ebb6d7415e1165121041a540",
+    "id": "importlib.metadata",
     "ignore_all": true,
-    "interface_hash": "fce531f96966c28a3fd4a137c86130b3972e1d4153d0aadd4146bf0e87250381",
-    "mtime": 1683082840,
+    "interface_hash": "a9774322780c6a1b91d5929f056cf14807f1f2799e2af15510a91677d9523c1c",
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -81,13 +87,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib/python3.11/site-packages/click/parser.py",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/importlib/metadata/__init__.pyi",
     "plugin_data": null,
-    "size": 19044,
+    "size": 6736,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/click/shell_completion.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/click/shell_completion.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/click/shell_completion.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/click/shell_completion.meta.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8947368421052632%*

 * *Differences: {"'data_mtime'": '1683843441',*

 * * "'dep_lines'": '{insert: [(8, 1)]}',*

 * * "'dep_prios'": '{insert: [(9, 30)]}',*

 * * "'dependencies'": "{insert: [(17, 'types')]}",*

 * * "'mtime'": '1684623295',*

 * * "'version_id'": "'1.3.0'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681571164,
+    "data_mtime": 1683843441,
     "dep_lines": [
         6,
         13,
         14,
         1,
         2,
         3,
@@ -14,14 +14,15 @@
         1,
         1,
         1,
         1,
         1,
         1,
         1,
+        1,
         1
     ],
     "dep_prios": [
         5,
         5,
         5,
         10,
@@ -34,14 +35,15 @@
         30,
         30,
         30,
         30,
         30,
         30,
         30,
+        30,
         30
     ],
     "dependencies": [
         "click.core",
         "click.parser",
         "click.utils",
         "os",
@@ -54,21 +56,22 @@
         "abc",
         "array",
         "click.types",
         "ctypes",
         "enum",
         "mmap",
         "pickle",
+        "types",
         "typing_extensions"
     ],
     "hash": "a8ea7f05e0bd7ac10e4992b2bb91bb448c4451a2ec5d45fe9936fb841d6be106",
     "id": "click.shell_completion",
     "ignore_all": true,
     "interface_hash": "78563bcc5ed48407a7bc9d1b232f6fa059cb118020a6a9f0fc30538e356e168c",
-    "mtime": 1683082840,
+    "mtime": 1684623295,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -106,9 +109,9 @@
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
     "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib/python3.11/site-packages/click/shell_completion.py",
     "plugin_data": null,
     "size": 18018,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/click/termui.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/click/termui.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/click/termui.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/typer/rich_utils.meta.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.63745763280647%*

 * *Differences: {"'data_mtime'": '1683843441',*

 * * "'dep_lines'": '{insert: [(0, 240), (6, 9), (7, 1), (8, 1), (9, 1), (21, 11), (22, 12), (23, 13), '*

 * *                '(24, 14), (25, 15), (26, 16), (27, 17), (28, 18), (29, 19), (30, 20), (31, 21), '*

 * *                '(32, 10)], delete: [13, 7, 6, 5, 4, 3, 2, 1, 0]}',*

 * * "'dep_prios'": '{insert: [(4, 5), (5, 5), (6, 10), (8, 30), (9, 30), (10, 30), (21, 5), (22, 5), '*

 * *                '(23, 5), (24, 5), (25, 5), (26, 5), (27, 5), (28, 5), (29, 5), (30, 5), (31, 5), '*

 * *              […]*

```diff
@@ -1,95 +1,107 @@
 {
-    "data_mtime": 1681571164,
+    "data_mtime": 1683843441,
     "dep_lines": [
-        9,
-        12,
-        14,
-        15,
-        18,
-        22,
-        1,
-        2,
+        240,
         3,
         4,
         5,
         6,
         7,
-        53,
+        9,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
-        1
+        1,
+        1,
+        1,
+        1,
+        11,
+        12,
+        13,
+        14,
+        15,
+        16,
+        17,
+        18,
+        19,
+        20,
+        21,
+        10
     ],
     "dep_prios": [
-        5,
-        5,
-        5,
-        5,
-        5,
         20,
         10,
         10,
-        10,
-        10,
-        10,
-        10,
         5,
-        20,
         5,
+        5,
+        10,
+        5,
+        30,
+        30,
+        30,
+        30,
         30,
         30,
         30,
         30,
         30,
         30,
         30,
         30,
         30,
-        30
+        5,
+        5,
+        5,
+        5,
+        5,
+        5,
+        5,
+        5,
+        5,
+        5,
+        5,
+        5
     ],
     "dependencies": [
-        "click._compat",
-        "click.exceptions",
-        "click.globals",
-        "click.types",
-        "click.utils",
-        "click._termui_impl",
+        "typer.core",
         "inspect",
-        "io",
-        "itertools",
-        "os",
         "sys",
+        "collections",
+        "os",
         "typing",
-        "gettext",
-        "getpass",
+        "click",
         "builtins",
+        "_collections_abc",
         "_typeshed",
         "abc",
         "array",
         "click.core",
-        "contextlib",
+        "click.exceptions",
+        "click.shell_completion",
+        "click.types",
         "ctypes",
         "mmap",
         "pickle",
         "types",
         "typing_extensions"
     ],
-    "hash": "00205054ebc50934aab43e5544478201d46d94777e22695af8bb5ee3049f3230",
-    "id": "click.termui",
+    "hash": "73518e6d145375bea4e7298a3c057f534091fd529c975c4f775c2376751839c7",
+    "id": "typer.rich_utils",
     "ignore_all": true,
-    "interface_hash": "9cc7785b6d19ee5cf6aafb9bbbfb1a9e634723918a98bd089ddb2be9d5abe167",
-    "mtime": 1683082840,
+    "interface_hash": "2d0be71701ac8ef7a29ed1bfebcebe484ca8756ef35fe0cffeb055e7c22f6b4c",
+    "mtime": 1684623295,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -123,13 +135,26 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib/python3.11/site-packages/click/termui.py",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib/python3.11/site-packages/typer/rich_utils.py",
     "plugin_data": null,
-    "size": 28355,
-    "suppressed": [],
-    "version_id": "1.2.0"
+    "size": 23654,
+    "suppressed": [
+        "rich.align",
+        "rich.columns",
+        "rich.console",
+        "rich.emoji",
+        "rich.highlighter",
+        "rich.markdown",
+        "rich.padding",
+        "rich.panel",
+        "rich.table",
+        "rich.text",
+        "rich.theme",
+        "rich"
+    ],
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/click/types.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/click/types.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/click/types.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/click/types.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'data_mtime'": '1683843441', "'mtime'": '1684623295', "'version_id'": "'1.3.0'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681571164,
+    "data_mtime": 1683843441,
     "dep_lines": [
         8,
         11,
         12,
         17,
         19,
         1,
@@ -84,15 +84,15 @@
         "pickle",
         "types"
     ],
     "hash": "ac46f56994902aaddc8823268e91b652f6bdbe4e3df1744bed386b70ad8646cb",
     "id": "click.types",
     "ignore_all": true,
     "interface_hash": "9d62e11dee29135d2ec2685637004ef37729a31d7e5f0b47557ef25e6c5a178a",
-    "mtime": 1683082840,
+    "mtime": 1684623295,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -130,9 +130,9 @@
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
     "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib/python3.11/site-packages/click/types.py",
     "plugin_data": null,
     "size": 35805,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/click/utils.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/click/utils.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/click/utils.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/click/utils.meta.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'data_mtime'": '1683843441', "'mtime'": '1684623295', "'version_id'": "'1.3.0'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681571164,
+    "data_mtime": 1683843441,
     "dep_lines": [
         8,
         19,
         156,
         1,
         2,
         3,
@@ -75,15 +75,15 @@
         "posixpath",
         "sre_constants"
     ],
     "hash": "df70fa13ba681ff9eb281fb1afe5320c45e7c4e702890ab1b912edaea795bfaa",
     "id": "click.utils",
     "ignore_all": true,
     "interface_hash": "db613fdf4fc2174a1f92a63f3e781834c08286b26687300b9535cd7db6f3e632",
-    "mtime": 1683082840,
+    "mtime": 1684623295,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -121,9 +121,9 @@
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
     "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib/python3.11/site-packages/click/utils.py",
     "plugin_data": null,
     "size": 18682,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/collections/__init__.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/collections/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/collections/__init__.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/tomlkit/__init__.meta.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6593939393939394%*

 * *Differences: {"'data_mtime'": '1683843440',*

 * * "'dep_lines'": '{insert: [(1, 1)], delete: [6, 5, 4, 3, 2, 0]}',*

 * * "'dep_prios'": '{insert: [(2, 30)], delete: [5, 4, 3, 2, 1, 0]}',*

 * * "'dependencies'": "{insert: [(0, 'tomlkit.api'), (3, 'typing')], delete: [6, 5, 4, 3, 2, 1, 0]}",*

 * * "'hash'": "'feee93b1ddf737d85ff86840869aa3eadd2ca0d9d33b92cfdae31d5b05fdc46d'",*

 * * "'id'": "'tomlkit'",*

 * * "'interface_hash'": "'6b8614dd81fc21aadca9be9da93595eacfb2c9151bba35c2d55e64eef4bbd2dd'",*

 * * "'mtime'": '1684623295',*

 * * "'path'": "'/home/gotmax/Syn […]*

```diff
@@ -1,47 +1,32 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843440,
     "dep_lines": [
-        11,
         1,
-        2,
-        3,
-        4,
-        5,
-        8,
+        1,
         1,
         1
     ],
     "dep_prios": [
         5,
-        10,
-        5,
-        5,
-        5,
-        5,
-        5,
         5,
+        30,
         30
     ],
     "dependencies": [
-        "collections.abc",
-        "sys",
-        "_collections_abc",
-        "_typeshed",
-        "typing",
-        "typing_extensions",
-        "types",
+        "tomlkit.api",
         "builtins",
-        "abc"
+        "abc",
+        "typing"
     ],
-    "hash": "f5e16c9ed8790956c54a074ea675d0ce3404db9e0e83a2d254e706d06290b724",
-    "id": "collections",
+    "hash": "feee93b1ddf737d85ff86840869aa3eadd2ca0d9d33b92cfdae31d5b05fdc46d",
+    "id": "tomlkit",
     "ignore_all": true,
-    "interface_hash": "9b370fdc1a826574f79bc27163dfa6a4600f8373a80e29c07fa76a47b7e51a6a",
-    "mtime": 1683082840,
+    "interface_hash": "6b8614dd81fc21aadca9be9da93595eacfb2c9151bba35c2d55e64eef4bbd2dd",
+    "mtime": 1684623295,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -75,13 +60,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/collections/__init__.pyi",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib/python3.11/site-packages/tomlkit/__init__.py",
     "plugin_data": null,
-    "size": 20830,
+    "size": 1148,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/collections/abc.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/collections/abc.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/collections/abc.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/collections/abc.meta.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'data_mtime'": '1683843440', "'mtime'": '1684623296', "'version_id'": "'1.3.0'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843440,
     "dep_lines": [
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
@@ -18,15 +18,15 @@
         "abc",
         "typing"
     ],
     "hash": "90189900dd153dff2aa642276e3a8a65145ed0f5eb67b8f1366086b38a3950e7",
     "id": "collections.abc",
     "ignore_all": true,
     "interface_hash": "a49383ff92c6a48f17d7aa16dc078d05f10677511eb84852bcba4bf3cd24b57d",
-    "mtime": 1683082840,
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -64,9 +64,9 @@
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
     "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/collections/abc.pyi",
     "plugin_data": null,
     "size": 79,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/ctypes/__init__.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/ctypes/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/ctypes/__init__.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/ctypes/__init__.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'data_mtime'": '1683843440', "'mtime'": '1684623296', "'version_id'": "'1.3.0'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843440,
     "dep_lines": [
         5,
         1,
         2,
         3,
         4,
         6,
@@ -42,15 +42,15 @@
         "mmap",
         "pickle"
     ],
     "hash": "4e07f95e28e46e9d4c5eda8e3a693994b25ddc9e70955e59f569acc5472d3284",
     "id": "ctypes",
     "ignore_all": true,
     "interface_hash": "27824822e37ab201113f9c436765dd4f8faefe70d1b0c64290d077adb40cbbf9",
-    "mtime": 1683082840,
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -88,9 +88,9 @@
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
     "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/ctypes/__init__.pyi",
     "plugin_data": null,
     "size": 11646,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/email/__init__.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/email/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/email/__init__.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/email/__init__.meta.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'data_mtime'": '1683843440', "'mtime'": '1684623296', "'version_id'": "'1.3.0'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843440,
     "dep_lines": [
         1,
         2,
         3,
         4,
         5,
         1,
@@ -27,15 +27,15 @@
         "builtins",
         "abc"
     ],
     "hash": "6bef9c70cfca2efd38e18849f547603c1578043aabfa6e9ac44b019e9e2c323b",
     "id": "email",
     "ignore_all": true,
     "interface_hash": "a1f468baca09b46c3650dd75a62d029bf78402e94ec41aed896e6b9310488c57",
-    "mtime": 1683082840,
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -73,9 +73,9 @@
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
     "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/email/__init__.pyi",
     "plugin_data": null,
     "size": 1054,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/email/charset.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/email/charset.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/email/charset.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/typer/colors.meta.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7083333333333334%*

 * *Differences: {"'data_mtime'": '1683843440',*

 * * "'dep_lines'": '{delete: [0]}',*

 * * "'dep_prios'": '{delete: [0]}',*

 * * "'dependencies'": '{delete: [0]}',*

 * * "'hash'": "'7b8da3f2e079db484ba57e42ff47e247738ea0814c6e13b700366fbfa865015f'",*

 * * "'id'": "'typer.colors'",*

 * * "'interface_hash'": "'b8723b40b62875262b3f7214a0af15e5a533172dfd03f9929ebf8a731ea8c105'",*

 * * "'mtime'": '1684623295',*

 * * "'path'": "'/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib/python3.11/site-packages/typer/colors.py'",*

 * * "'size'": '430',*

 * * " […]*

```diff
@@ -1,32 +1,29 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843440,
     "dep_lines": [
         1,
         1,
-        1,
         1
     ],
     "dep_prios": [
         5,
-        5,
         30,
         30
     ],
     "dependencies": [
-        "collections.abc",
         "builtins",
         "abc",
         "typing"
     ],
-    "hash": "7eb946e66f91d483704797cfcbe5603351fd555cb7655a0e5444e653fcd491d7",
-    "id": "email.charset",
+    "hash": "7b8da3f2e079db484ba57e42ff47e247738ea0814c6e13b700366fbfa865015f",
+    "id": "typer.colors",
     "ignore_all": true,
-    "interface_hash": "f87f2e3130de71b46db48f0b4c53f1a3a30d08e4024f0c757230f1b312dcfc2a",
-    "mtime": 1683082840,
+    "interface_hash": "b8723b40b62875262b3f7214a0af15e5a533172dfd03f9929ebf8a731ea8c105",
+    "mtime": 1684623295,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -60,13 +57,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/email/charset.pyi",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib/python3.11/site-packages/typer/colors.py",
     "plugin_data": null,
-    "size": 1077,
+    "size": 430,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/email/contentmanager.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/email/contentmanager.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/email/contentmanager.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/tomli_w/__init__.meta.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6761904761904761%*

 * *Differences: {"'data_mtime'": '1683843440',*

 * * "'dep_lines'": '{insert: [(0, 4)], delete: [2, 1]}',*

 * * "'dep_prios'": '{insert: [(2, 30)], delete: [1, 0]}',*

 * * "'dependencies'": "{insert: [(0, 'tomli_w._writer'), (3, 'typing')], delete: [2, 1, 0]}",*

 * * "'hash'": "'c3cdef9f865651a478788c5258258e5643d8f2a18943ebae5699c8b5dce69245'",*

 * * "'id'": "'tomli_w'",*

 * * "'interface_hash'": "'cbfc201f42bbd11842b55dd5f80ad2f898a253e0d2952c0953f374e19058fc76'",*

 * * "'mtime'": '1684623295',*

 * * "'path'": "'/home/gotmax/Sync/git-repos/packaging/fedora_rpm […]*

```diff
@@ -1,35 +1,32 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843440,
     "dep_lines": [
+        4,
         1,
-        2,
-        3,
         1,
         1
     ],
     "dep_prios": [
         5,
         5,
-        5,
-        5,
+        30,
         30
     ],
     "dependencies": [
-        "collections.abc",
-        "email.message",
-        "typing",
+        "tomli_w._writer",
         "builtins",
-        "abc"
+        "abc",
+        "typing"
     ],
-    "hash": "53099e51c46e4530831d75440f30c0481378944b551b503d0689cd68c9afd1bf",
-    "id": "email.contentmanager",
+    "hash": "c3cdef9f865651a478788c5258258e5643d8f2a18943ebae5699c8b5dce69245",
+    "id": "tomli_w",
     "ignore_all": true,
-    "interface_hash": "e8be1394995719c9a2c021f56688ad6fb187cb5c81ab78e43653093ad9b27fd0",
-    "mtime": 1683082840,
+    "interface_hash": "cbfc201f42bbd11842b55dd5f80ad2f898a253e0d2952c0953f374e19058fc76",
+    "mtime": 1684623295,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -63,13 +60,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/email/contentmanager.pyi",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib/python3.11/site-packages/tomli_w/__init__.py",
     "plugin_data": null,
-    "size": 480,
+    "size": 157,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/email/errors.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/email/errors.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/email/errors.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/email/policy.meta.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6482323232323232%*

 * *Differences: {"'data_mtime'": '1683843440',*

 * * "'dep_lines'": '{insert: [(0, 2), (1, 3), (2, 4), (3, 5), (4, 6), (6, 7)], delete: [2, 1, 0]}',*

 * * "'dep_prios'": '{insert: [(1, 5), (2, 5), (3, 5), (4, 5), (5, 5), (6, 5), (7, 5)], delete: [4, 3, '*

 * *                '2, 0]}',*

 * * "'dependencies'": "{insert: [(0, 'collections.abc'), (1, 'email.contentmanager'), (2, "*

 * *                   "'email.errors'), (3, 'email.header'), (4, 'email.message'), (7, 'builtins')], "*

 * *                   'delete: [2, 1, 0]}',*

 * * "'hash'": "'2122e2c085231b […]*

```diff
@@ -1,35 +1,44 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843440,
     "dep_lines": [
+        2,
+        3,
+        4,
+        5,
+        6,
         1,
-        1,
-        1,
-        1,
+        7,
         1
     ],
     "dep_prios": [
-        10,
         5,
-        30,
-        30,
-        30
+        5,
+        5,
+        5,
+        5,
+        5,
+        5,
+        5
     ],
     "dependencies": [
-        "sys",
-        "builtins",
-        "_typeshed",
+        "collections.abc",
+        "email.contentmanager",
+        "email.errors",
+        "email.header",
+        "email.message",
         "abc",
-        "typing"
+        "typing",
+        "builtins"
     ],
-    "hash": "ca7498bfe12fcf0148a719c9bfa9f40ff037ddb6e1308f6101d338a8b9a859b9",
-    "id": "email.errors",
+    "hash": "2122e2c085231b4505c48fb54f55b2fb36ead76660699bc3d800fffbd4f0c6f4",
+    "id": "email.policy",
     "ignore_all": true,
-    "interface_hash": "392541fc8423d0fcd6bd24011421b115260845ea897f4b51074fd079ea362025",
-    "mtime": 1683082840,
+    "interface_hash": "3b053f392752efc7ea1ae9fc534e0ecdbb69fbcca710c4bc8fc3cf0ee77b0a36",
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -63,13 +72,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/email/errors.pyi",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/email/policy.pyi",
     "plugin_data": null,
-    "size": 1533,
+    "size": 3055,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/email/header.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/email/header.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/email/header.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/email/header.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'data_mtime'": '1683843440', "'mtime'": '1684623296', "'version_id'": "'1.3.0'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843440,
     "dep_lines": [
         1,
         2,
         3,
         1,
         1
     ],
@@ -21,15 +21,15 @@
         "builtins",
         "abc"
     ],
     "hash": "d98ef62919eee52c902ba572fe572fc3a54622a5e630532cf09aa7f12374562d",
     "id": "email.header",
     "ignore_all": true,
     "interface_hash": "d6694eacb53203b17f13cad23440f78f35aa4206fc911546b697d44f4ffd9ac7",
-    "mtime": 1683082840,
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -67,9 +67,9 @@
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
     "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/email/header.pyi",
     "plugin_data": null,
     "size": 1264,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/email/message.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/email/message.data.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999999999948684%*

 * *Differences: {"'names'": "{'Message': {'node': {'names': {'get_charsets': {'node': {'items': {0: {'func': "*

 * *            "{'type': {'ret_type': {'.class': 'Instance', 'args': [OrderedDict([('.class', "*

 * *            "'UnionType'), ('items', ['builtins.str', OrderedDict([('.class', 'NoneType')])])])], "*

 * *            "'type_ref': 'builtins.list', delete: ['items']}}}}, 1: {'func': {'type': {'ret_type': "*

 * *            "{'.class': 'Instance', 'args': [OrderedDict([('.class', 'UnionType'), ('items', "*

 * *            "['builtins.str' […]*

```diff
@@ -2921,27 +2921,27 @@
                                             },
                                             "fallback": "builtins.function",
                                             "from_concatenate": false,
                                             "implicit": false,
                                             "is_ellipsis_args": false,
                                             "name": "get_charsets of Message",
                                             "ret_type": {
-                                                ".class": "UnionType",
-                                                "items": [
+                                                ".class": "Instance",
+                                                "args": [
                                                     {
-                                                        ".class": "Instance",
-                                                        "args": [
-                                                            "builtins.str"
-                                                        ],
-                                                        "type_ref": "builtins.list"
-                                                    },
-                                                    {
-                                                        ".class": "NoneType"
+                                                        ".class": "UnionType",
+                                                        "items": [
+                                                            "builtins.str",
+                                                            {
+                                                                ".class": "NoneType"
+                                                            }
+                                                        ]
                                                     }
-                                                ]
+                                                ],
+                                                "type_ref": "builtins.list"
                                             },
                                             "type_guard": null,
                                             "unpack_kwargs": false,
                                             "variables": []
                                         }
                                     },
                                     "is_overload": true,
@@ -3004,34 +3004,34 @@
                                             },
                                             "fallback": "builtins.function",
                                             "from_concatenate": false,
                                             "implicit": false,
                                             "is_ellipsis_args": false,
                                             "name": "get_charsets of Message",
                                             "ret_type": {
-                                                ".class": "UnionType",
-                                                "items": [
-                                                    {
-                                                        ".class": "Instance",
-                                                        "args": [
-                                                            "builtins.str"
-                                                        ],
-                                                        "type_ref": "builtins.list"
-                                                    },
+                                                ".class": "Instance",
+                                                "args": [
                                                     {
-                                                        ".class": "TypeVarType",
-                                                        "fullname": "email.message._T",
-                                                        "id": -1,
-                                                        "name": "_T",
-                                                        "namespace": "",
-                                                        "upper_bound": "builtins.object",
-                                                        "values": [],
-                                                        "variance": 0
+                                                        ".class": "UnionType",
+                                                        "items": [
+                                                            "builtins.str",
+                                                            {
+                                                                ".class": "TypeVarType",
+                                                                "fullname": "email.message._T",
+                                                                "id": -1,
+                                                                "name": "_T",
+                                                                "namespace": "",
+                                                                "upper_bound": "builtins.object",
+                                                                "values": [],
+                                                                "variance": 0
+                                                            }
+                                                        ]
                                                     }
-                                                ]
+                                                ],
+                                                "type_ref": "builtins.list"
                                             },
                                             "type_guard": null,
                                             "unpack_kwargs": false,
                                             "variables": [
                                                 {
                                                     ".class": "TypeVarType",
                                                     "fullname": "email.message._T",
@@ -3082,27 +3082,27 @@
                                         },
                                         "fallback": "builtins.function",
                                         "from_concatenate": false,
                                         "implicit": false,
                                         "is_ellipsis_args": false,
                                         "name": "get_charsets of Message",
                                         "ret_type": {
-                                            ".class": "UnionType",
-                                            "items": [
+                                            ".class": "Instance",
+                                            "args": [
                                                 {
-                                                    ".class": "Instance",
-                                                    "args": [
-                                                        "builtins.str"
-                                                    ],
-                                                    "type_ref": "builtins.list"
-                                                },
-                                                {
-                                                    ".class": "NoneType"
+                                                    ".class": "UnionType",
+                                                    "items": [
+                                                        "builtins.str",
+                                                        {
+                                                            ".class": "NoneType"
+                                                        }
+                                                    ]
                                                 }
-                                            ]
+                                            ],
+                                            "type_ref": "builtins.list"
                                         },
                                         "type_guard": null,
                                         "unpack_kwargs": false,
                                         "variables": []
                                     },
                                     {
                                         ".class": "CallableType",
@@ -3133,34 +3133,34 @@
                                         },
                                         "fallback": "builtins.function",
                                         "from_concatenate": false,
                                         "implicit": false,
                                         "is_ellipsis_args": false,
                                         "name": "get_charsets of Message",
                                         "ret_type": {
-                                            ".class": "UnionType",
-                                            "items": [
-                                                {
-                                                    ".class": "Instance",
-                                                    "args": [
-                                                        "builtins.str"
-                                                    ],
-                                                    "type_ref": "builtins.list"
-                                                },
+                                            ".class": "Instance",
+                                            "args": [
                                                 {
-                                                    ".class": "TypeVarType",
-                                                    "fullname": "email.message._T",
-                                                    "id": -1,
-                                                    "name": "_T",
-                                                    "namespace": "",
-                                                    "upper_bound": "builtins.object",
-                                                    "values": [],
-                                                    "variance": 0
+                                                    ".class": "UnionType",
+                                                    "items": [
+                                                        "builtins.str",
+                                                        {
+                                                            ".class": "TypeVarType",
+                                                            "fullname": "email.message._T",
+                                                            "id": -1,
+                                                            "name": "_T",
+                                                            "namespace": "",
+                                                            "upper_bound": "builtins.object",
+                                                            "values": [],
+                                                            "variance": 0
+                                                        }
+                                                    ]
                                                 }
-                                            ]
+                                            ],
+                                            "type_ref": "builtins.list"
                                         },
                                         "type_guard": null,
                                         "unpack_kwargs": false,
                                         "variables": [
                                             {
                                                 ".class": "TypeVarType",
                                                 "fullname": "email.message._T",
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/email/message.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/typer/params.meta.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.659047619047619%*

 * *Differences: {"'data_mtime'": '1683843441',*

 * * "'dep_lines'": '{insert: [(2, 1), (3, 3), (4, 1), (5, 1)], delete: [6, 5, 4, 2, 1, 0]}',*

 * * "'dep_prios'": '{insert: [(1, 25), (3, 10), (5, 30), (6, 30)], delete: [5, 4, 3, 2, 1, 0]}',*

 * * "'dependencies'": "{insert: [(0, 'typer.models'), (1, 'click.shell_completion'), (3, 'click'), "*

 * *                   "(6, 'click.core'), (7, 'click.types')], delete: [7, 5, 4, 3, 2, 1, 0]}",*

 * * "'hash'": "'fcf07893bfc8bf4aa53628a147a0b9383364d9146d16d97b31bf5d993a818c4c'",*

 * * "'id'": "'typer.params'" […]*

```diff
@@ -1,50 +1,44 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843441,
     "dep_lines": [
-        1,
-        3,
-        4,
         5,
-        6,
-        2,
-        7,
         8,
         1,
+        3,
+        1,
+        1,
+        1,
         1
     ],
     "dep_prios": [
         5,
+        25,
         5,
+        10,
         5,
-        5,
-        5,
-        5,
-        5,
-        5,
-        5,
+        30,
+        30,
         30
     ],
     "dependencies": [
-        "collections.abc",
-        "email.charset",
-        "email.contentmanager",
-        "email.errors",
-        "email.policy",
-        "email",
+        "typer.models",
+        "click.shell_completion",
         "typing",
-        "typing_extensions",
+        "click",
         "builtins",
-        "abc"
+        "abc",
+        "click.core",
+        "click.types"
     ],
-    "hash": "6e0993b354bdf6bbe105b3598646b27a62851aead468c8a871eb4c4baef5ed2f",
-    "id": "email.message",
+    "hash": "fcf07893bfc8bf4aa53628a147a0b9383364d9146d16d97b31bf5d993a818c4c",
+    "id": "typer.params",
     "ignore_all": true,
-    "interface_hash": "e8f2bdc4254aca1700f2062ead8cd156b137fdaa47eb7506f0edf2a1e0b5710c",
-    "mtime": 1683082840,
+    "interface_hash": "9f3ba03f753769f82325ea23db014f845f69308f332d7cc50cc11cbecd346913",
+    "mtime": 1684623295,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -78,13 +72,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/email/message.pyi",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib/python3.11/site-packages/typer/params.py",
     "plugin_data": null,
-    "size": 6091,
+    "size": 13401,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/email/policy.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/email/policy.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/email/policy.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/sre_compile.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6759259259259259%*

 * *Differences: {"'data_mtime'": '1683843439',*

 * * "'dep_lines'": '{insert: [(0, 1)], delete: [6, 4, 1]}',*

 * * "'dep_prios'": '{insert: [(5, 30)], delete: [2, 1, 0]}',*

 * * "'dependencies'": "{insert: [(0, 're'), (1, 'sre_constants'), (2, 'sre_parse'), (5, 'abc')], "*

 * *                   'delete: [5, 4, 3, 2, 1, 0]}',*

 * * "'hash'": "'c9cd67b263730096df01415a2933288a4f7d800e1380fc31f76bb1e39af65440'",*

 * * "'id'": "'sre_compile'",*

 * * "'interface_hash'": "'3128a45ec285be40db17b279b171fb09c4c5a67948ec05ca7a4f65007ae945a0'",*

 * * "'mtime'": '168462329 […]*

```diff
@@ -1,44 +1,38 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843439,
     "dep_lines": [
+        1,
         2,
-        3,
         4,
         5,
-        6,
         1,
-        7,
         1
     ],
     "dep_prios": [
         5,
         5,
         5,
         5,
         5,
-        5,
-        5,
-        5
+        30
     ],
     "dependencies": [
-        "collections.abc",
-        "email.contentmanager",
-        "email.errors",
-        "email.header",
-        "email.message",
-        "abc",
+        "re",
+        "sre_constants",
+        "sre_parse",
         "typing",
-        "builtins"
+        "builtins",
+        "abc"
     ],
-    "hash": "2122e2c085231b4505c48fb54f55b2fb36ead76660699bc3d800fffbd4f0c6f4",
-    "id": "email.policy",
+    "hash": "c9cd67b263730096df01415a2933288a4f7d800e1380fc31f76bb1e39af65440",
+    "id": "sre_compile",
     "ignore_all": true,
-    "interface_hash": "3b053f392752efc7ea1ae9fc534e0ecdbb69fbcca710c4bc8fc3cf0ee77b0a36",
-    "mtime": 1683082840,
+    "interface_hash": "3128a45ec285be40db17b279b171fb09c4c5a67948ec05ca7a4f65007ae945a0",
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -72,13 +66,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/email/policy.pyi",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/sre_compile.pyi",
     "plugin_data": null,
-    "size": 3055,
+    "size": 332,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/importlib/__init__.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/importlib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/importlib/__init__.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/dis.meta.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6843434343434344%*

 * *Differences: {"'data_mtime'": '1683843440',*

 * * "'dep_lines'": '{insert: [(0, 3), (3, 4), (4, 5), (5, 6)], delete: [2]}',*

 * * "'dep_prios'": '{insert: [(0, 5), (1, 10), (2, 10)]}',*

 * * "'dependencies'": "{insert: [(1, 'sys'), (3, 'opcode'), (4, 'typing'), (5, 'typing_extensions'), "*

 * *                   "(7, '_typeshed')], delete: [5, 1]}",*

 * * "'hash'": "'d29f5fee5fb560e7554e8bdc2cc65a05992e94838554fa808ee3838971c37085'",*

 * * "'id'": "'dis'",*

 * * "'interface_hash'": "'549c8473c8ca310f5f94ab3adb5facd61785d1e89865622c4a97cf625bc847ed'",*

 * * "' […]*

```diff
@@ -1,38 +1,47 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843440,
     "dep_lines": [
+        3,
         1,
         2,
-        3,
+        4,
+        5,
+        6,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
+        10,
+        10,
+        5,
         5,
         5,
         5,
         30,
         30
     ],
     "dependencies": [
         "collections.abc",
-        "importlib.abc",
+        "sys",
         "types",
+        "opcode",
+        "typing",
+        "typing_extensions",
         "builtins",
-        "abc",
-        "typing"
+        "_typeshed",
+        "abc"
     ],
-    "hash": "a8c6ba5a31a05b67b94b6b2d122f04c1046a7dd19c5db581ee299b3a3f0a2761",
-    "id": "importlib",
+    "hash": "d29f5fee5fb560e7554e8bdc2cc65a05992e94838554fa808ee3838971c37085",
+    "id": "dis",
     "ignore_all": true,
-    "interface_hash": "b80a4994b195a25dcb726ee5d3ab6f304ddccbc43699e382291f1aeabe66a601",
-    "mtime": 1683082840,
+    "interface_hash": "549c8473c8ca310f5f94ab3adb5facd61785d1e89865622c4a97cf625bc847ed",
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -66,13 +75,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/importlib/__init__.pyi",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/dis.pyi",
     "plugin_data": null,
-    "size": 802,
+    "size": 4408,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/importlib/abc.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/importlib/abc.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/importlib/abc.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/tomlkit/_utils.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6712380952380953%*

 * *Differences: {"'data_mtime'": '1683843440',*

 * * "'dep_lines'": '{insert: [(0, 5), (1, 13), (4, 6), (5, 11), (6, 1), (7, 1), (8, 1), (9, 1)], '*

 * *                'delete: [9, 8, 7, 6, 5, 3, 1, 0]}',*

 * * "'dep_prios'": '{insert: [(3, 10), (7, 30), (8, 30), (9, 30), (10, 30)], delete: [4, 3, 2, 1, 0]}',*

 * * "'dependencies'": "{insert: [(1, 'tomlkit._compat'), (2, '__future__'), (3, 're'), (4, "*

 * *                   "'datetime'), (7, '_collections_abc'), (8, '_typeshed'), (9, 'abc'), (14, "*

 * *                   "'types'), (15, 'typing_ext […]*

```diff
@@ -1,68 +1,68 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843440,
     "dep_lines": [
-        14,
-        15,
+        5,
+        13,
         1,
-        2,
         3,
-        4,
-        13,
-        16,
-        17,
-        18,
+        6,
+        11,
+        1,
+        1,
+        1,
+        1,
         1,
         1,
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
         5,
-        10,
-        10,
-        10,
-        5,
-        5,
         5,
+        10,
         5,
         5,
         5,
         30,
         30,
         30,
         30,
+        30,
+        30,
+        30,
+        30,
         30
     ],
     "dependencies": [
         "collections.abc",
-        "importlib.machinery",
-        "_ast",
-        "sys",
-        "types",
-        "_typeshed",
-        "abc",
-        "io",
+        "tomlkit._compat",
+        "__future__",
+        "re",
+        "datetime",
         "typing",
-        "typing_extensions",
         "builtins",
+        "_collections_abc",
+        "_typeshed",
+        "abc",
         "array",
         "ctypes",
         "mmap",
-        "os",
-        "pickle"
+        "pickle",
+        "types",
+        "typing_extensions"
     ],
-    "hash": "2ef3e7cd4f57d7730ef462502b680809572a49eb21b9555784a5744ab4e70c3f",
-    "id": "importlib.abc",
+    "hash": "7d7d67edba028bbfdb05505e99acb09347b2c6a8536276563e10991c980166ff",
+    "id": "tomlkit._utils",
     "ignore_all": true,
-    "interface_hash": "27fdc7881cd5848e3fd5c8b1552d0e9e76bf0628ec4c7d0fccea76cdfa697ff6",
-    "mtime": 1683082840,
+    "interface_hash": "d9614e97cc2e07d645f1684d67fc9de46360e633a9fff2bbe1957f090b668f2d",
+    "mtime": 1684623295,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -96,13 +96,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/importlib/abc.pyi",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib/python3.11/site-packages/tomlkit/_utils.py",
     "plugin_data": null,
-    "size": 7380,
+    "size": 4021,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/importlib/machinery.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/importlib/machinery.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/importlib/machinery.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/importlib/machinery.meta.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'data_mtime'": '1683843440', "'mtime'": '1684623296', "'version_id'": "'1.3.0'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843440,
     "dep_lines": [
         1,
         5,
         9,
         1,
         2,
         3,
@@ -48,15 +48,15 @@
         "mmap",
         "pickle"
     ],
     "hash": "d8d65c367ab0b794c41c101e2200e4171d0d147dfa49385be91cdd958db6fc1d",
     "id": "importlib.machinery",
     "ignore_all": true,
     "interface_hash": "b3172b298c17e5a5eff0b769b759ba09730f82b101504615c5b6e15ac7c4e8e0",
-    "mtime": 1683082840,
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -94,9 +94,9 @@
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
     "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/importlib/machinery.pyi",
     "plugin_data": null,
     "size": 5621,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/importlib/metadata/__init__.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/importlib/metadata/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/importlib/metadata/__init__.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/random.meta.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6661002178649238%*

 * *Differences: {"'data_mtime'": '1683843440',*

 * * "'dep_lines'": '{insert: [(0, 4), (4, 5), (5, 6), (6, 1), (7, 1)], delete: [11, 10, 9, 8, 7, 3, '*

 * *                '2, 1, 0]}',*

 * * "'dep_prios'": '{insert: [(7, 30), (8, 30)], delete: [8, 7, 5, 2, 1, 0]}',*

 * * "'dependencies'": "{insert: [(1, '_random'), (4, 'fractions'), (7, 'abc'), (8, 'numbers')], "*

 * *                   'delete: [11, 9, 8, 5, 4, 3, 2, 0]}',*

 * * "'hash'": "'cd0376273b30c0297134c77768237d572ecd19d309a415d628265d2a817b39e8'",*

 * * "'id'": "'random'",*

 * * "'interface_hash'": "' […]*

```diff
@@ -1,59 +1,47 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843440,
     "dep_lines": [
-        31,
-        5,
-        6,
-        7,
+        4,
         1,
         2,
         3,
-        4,
-        8,
-        10,
-        11,
-        12,
+        5,
+        6,
+        1,
+        1,
         1
     ],
     "dep_prios": [
         5,
-        5,
-        5,
-        5,
         10,
-        5,
         10,
         5,
         5,
         5,
         5,
-        5,
-        5
+        30,
+        30
     ],
     "dependencies": [
-        "importlib.metadata._meta",
         "collections.abc",
-        "email.message",
-        "importlib.abc",
-        "abc",
-        "pathlib",
+        "_random",
         "sys",
         "_typeshed",
-        "os",
-        "re",
+        "fractions",
         "typing",
-        "typing_extensions",
-        "builtins"
+        "builtins",
+        "abc",
+        "numbers"
     ],
-    "hash": "ae422af81eff03dc03edf2ef5f854e32c69b6b23ebb6d7415e1165121041a540",
-    "id": "importlib.metadata",
+    "hash": "cd0376273b30c0297134c77768237d572ecd19d309a415d628265d2a817b39e8",
+    "id": "random",
     "ignore_all": true,
-    "interface_hash": "a9774322780c6a1b91d5929f056cf14807f1f2799e2af15510a91677d9523c1c",
-    "mtime": 1683082840,
+    "interface_hash": "bf5c4ab5938e9edadc255d6af3e00c2ac3568dd9b5df5bd729229373f845638a",
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -87,13 +75,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/importlib/metadata/__init__.pyi",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/random.pyi",
     "plugin_data": null,
-    "size": 6736,
+    "size": 4643,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/importlib/metadata/_meta.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/importlib/metadata/_meta.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/importlib/metadata/_meta.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/tomcli/__init__.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6511111111111111%*

 * *Differences: {"'data_mtime'": '1683843440',*

 * * "'dep_lines'": '{insert: [(0, 8)], delete: [1]}',*

 * * "'dep_prios'": '{insert: [(2, 30)], delete: [0]}',*

 * * "'dependencies'": "{insert: [(0, '__future__'), (3, 'typing')], delete: [1, 0]}",*

 * * "'hash'": "'d054c9b4e8da0003db105ae76371260894a808cf2bd348576ad5aebec27c993c'",*

 * * "'id'": "'tomcli'",*

 * * "'ignore_all'": 'False',*

 * * "'interface_hash'": "'f4f562dc0c67b2b3c3636bd765b2e9a944987d80b207a04cfcc750c7d2477770'",*

 * * "'mtime'": '1683085458',*

 * * "'path'": "'src/tomcli/__init__.py'",*

 * * "'size'":  […]*

```diff
@@ -1,32 +1,32 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843440,
     "dep_lines": [
+        8,
         1,
-        2,
         1,
         1
     ],
     "dep_prios": [
         5,
         5,
-        5,
+        30,
         30
     ],
     "dependencies": [
-        "collections.abc",
-        "typing",
+        "__future__",
         "builtins",
-        "abc"
+        "abc",
+        "typing"
     ],
-    "hash": "2be6b67f68a873ae65d787d3f698fdaf7871860828243a5e6d747d1305c5ffa4",
-    "id": "importlib.metadata._meta",
-    "ignore_all": true,
-    "interface_hash": "1db704b0286cfe333cd9435e9f98ea264d93b92ffc6067f47c05700759a0233d",
-    "mtime": 1683082840,
+    "hash": "d054c9b4e8da0003db105ae76371260894a808cf2bd348576ad5aebec27c993c",
+    "id": "tomcli",
+    "ignore_all": false,
+    "interface_hash": "f4f562dc0c67b2b3c3636bd765b2e9a944987d80b207a04cfcc750c7d2477770",
+    "mtime": 1683085458,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -60,13 +60,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/importlib/metadata/_meta.pyi",
+    "path": "src/tomcli/__init__.py",
     "plugin_data": null,
-    "size": 842,
+    "size": 212,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/os/__init__.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/os/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/os/__init__.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/tomlkit/_compat.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6658838383838384%*

 * *Differences: {"'data_mtime'": '1683843440',*

 * * "'dep_lines'": '{insert: [(1, 3), (2, 4), (3, 6), (4, 1), (5, 1), (6, 1), (7, 1), (8, 1)], '*

 * *                'delete: [11, 10, 9, 8, 7, 6, 5, 4, 3, 1, 0]}',*

 * * "'dep_prios'": '{insert: [(5, 30), (6, 30), (7, 30), (8, 30)], delete: [9, 8, 7, 6, 5, 4, 3]}',*

 * * "'dependencies'": "{insert: [(0, '__future__'), (1, 'contextlib'), (3, 'typing'), (4, "*

 * *                   "'builtins'), (11, 'types'), (12, 'typing_extensions')], delete: [11, 10, 9, 8, "*

 * *                   '7, 6, 5, 1, 0]}' […]*

```diff
@@ -1,68 +1,59 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843440,
     "dep_lines": [
-        23,
-        30,
         1,
-        2,
-        21,
-        22,
-        24,
-        25,
-        26,
-        27,
-        28,
-        33,
+        3,
+        4,
+        6,
+        1,
+        1,
+        1,
+        1,
+        1,
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
         10,
         10,
         5,
         5,
-        5,
-        5,
-        5,
-        5,
-        5,
-        5,
-        5,
+        30,
+        30,
+        30,
+        30,
         30,
         30,
         30,
         30
     ],
     "dependencies": [
-        "collections.abc",
-        "os.path",
+        "__future__",
+        "contextlib",
         "sys",
+        "typing",
+        "builtins",
         "_typeshed",
         "abc",
-        "builtins",
-        "contextlib",
-        "io",
-        "subprocess",
-        "typing",
-        "typing_extensions",
-        "types",
         "array",
         "ctypes",
         "mmap",
-        "pickle"
+        "pickle",
+        "types",
+        "typing_extensions"
     ],
-    "hash": "43f0abc8936c573dfefd04ae185e74a6fc8eac1be65a0daaaf327303d8dc486e",
-    "id": "os",
+    "hash": "829ecfeea361d32635760d30ca38820db570153754a3ba744308d5e13dc5ba7b",
+    "id": "tomlkit._compat",
     "ignore_all": true,
-    "interface_hash": "c472e678239a2b046b7a9b8db5b5d3650e4d7aa2b07ee3c6d26a03316a587b2a",
-    "mtime": 1683082840,
+    "interface_hash": "356684536ba841ed5c7bd895e38f54f1f73b9181d3ffae4621694b620a223762",
+    "mtime": 1684623295,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -96,13 +87,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/os/__init__.pyi",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib/python3.11/site-packages/tomlkit/_compat.py",
     "plugin_data": null,
-    "size": 36995,
+    "size": 513,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/os/path.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/os/path.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/os/path.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/os/path.meta.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'data_mtime'": '1683843439', "'mtime'": '1684623296', "'version_id'": "'1.3.0'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843439,
     "dep_lines": [
         1,
         7,
         1,
         1,
         1
     ],
@@ -21,15 +21,15 @@
         "abc",
         "typing"
     ],
     "hash": "1bbead25bbe51b5fe4cc577c8270aa4b8321b7780fce50b58a1201ab3babc433",
     "id": "os.path",
     "ignore_all": true,
     "interface_hash": "be0df37ce66c7656498a847d168a4a73878352808c77e6f66e821de6819346a1",
-    "mtime": 1683082840,
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -67,9 +67,9 @@
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
     "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/os/path.pyi",
     "plugin_data": null,
     "size": 186,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/tomcli/__init__.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/tomcli/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/tomcli/__init__.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/tomcli/cli/_util.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6659090909090909%*

 * *Differences: {"'data_mtime'": '1683843440',*

 * * "'dep_lines'": '{insert: [(0, 6), (1, 4), (2, 7), (4, 1), (5, 1), (6, 1), (7, 1)]}',*

 * * "'dep_prios'": '{insert: [(0, 5), (1, 5), (2, 5), (5, 30), (6, 30), (7, 30), (8, 30)]}',*

 * * "'dependencies'": "{insert: [(0, 'collections.abc'), (2, 'contextlib'), (3, 'typing'), (6, "*

 * *                   "'array'), (7, 'ctypes'), (8, 'io'), (9, 'mmap'), (10, 'pickle')], delete: [3]}",*

 * * "'hash'": "'51f25d636074a960e9eb2bf88b9b96bdcbc17d4bf7d3897fec0bd3af11f1815e'",*

 * * "'id'": "'tomcli.cli._util'" […]*

```diff
@@ -1,32 +1,53 @@
 {
-    "data_mtime": 1681571164,
+    "data_mtime": 1683843440,
     "dep_lines": [
+        6,
+        4,
+        7,
         8,
         1,
         1,
+        1,
+        1,
+        1,
+        1,
         1
     ],
     "dep_prios": [
         5,
         5,
+        5,
+        5,
+        5,
+        30,
+        30,
+        30,
+        30,
         30,
         30
     ],
     "dependencies": [
+        "collections.abc",
         "__future__",
+        "contextlib",
+        "typing",
         "builtins",
         "abc",
-        "typing"
+        "array",
+        "ctypes",
+        "io",
+        "mmap",
+        "pickle"
     ],
-    "hash": "abcb243a5436410702c15923274d33029deadd8139ce5a7eadd2397c5e1e90c0",
-    "id": "tomcli",
+    "hash": "51f25d636074a960e9eb2bf88b9b96bdcbc17d4bf7d3897fec0bd3af11f1815e",
+    "id": "tomcli.cli._util",
     "ignore_all": false,
-    "interface_hash": "f4f562dc0c67b2b3c3636bd765b2e9a944987d80b207a04cfcc750c7d2477770",
-    "mtime": 1681492086,
+    "interface_hash": "f3687283861f779915f03712bb0bf09d1665cea4400b3083611262b57f4eb8e6",
+    "mtime": 1681573706,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -60,13 +81,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "src/tomcli/__init__.py",
+    "path": "src/tomcli/cli/_util.py",
     "plugin_data": null,
-    "size": 212,
+    "size": 468,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/tomcli/toml.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/tomcli/toml.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/tomcli/toml.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/tomcli/toml.meta.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9333333333333333%*

 * *Differences: {"'data_mtime'": '1683843440', "'version_id'": "'1.3.0'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681573228,
+    "data_mtime": 1683843440,
     "dep_lines": [
         10,
         5,
         7,
         8,
         9,
         11,
@@ -109,9 +109,9 @@
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
     "path": "src/tomcli/toml.py",
     "plugin_data": null,
     "size": 6585,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/tomcli/cli/__init__.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/tomcli/cli/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/tomcli/cli/__init__.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/tomcli/cli/__init__.meta.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9333333333333333%*

 * *Differences: {"'data_mtime'": '1683843440', "'version_id'": "'1.3.0'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843440,
     "dep_lines": [
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
@@ -61,9 +61,9 @@
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
     "path": "src/tomcli/cli/__init__.py",
     "plugin_data": null,
     "size": 82,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/tomcli/cli/_util.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/tomcli/cli/_util.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/tomcli/cli/_util.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/tomlkit/toml_document.meta.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.626984126984127%*

 * *Differences: {"'data_mtime'": '1683843440',*

 * * "'dep_lines'": '{delete: [7, 6, 5, 4, 3, 2, 1, 0]}',*

 * * "'dep_prios'": '{delete: [9, 8, 7, 6, 5, 2, 1, 0]}',*

 * * "'dependencies'": "{insert: [(0, 'tomlkit.container'), (3, 'typing')], delete: [11, 10, 9, 8, 7, "*

 * *                   '6, 3, 2, 1, 0]}',*

 * * "'hash'": "'3824e45977773f9f04653e120fcfdd75cd58a6431aaad952e7fb2d1d306630e2'",*

 * * "'id'": "'tomlkit.toml_document'",*

 * * "'ignore_all'": 'True',*

 * * "'interface_hash'": "'41d90e6ed171badd184c00b285e764b8b5790aa519d60e8d3aca13cf9c1ecf45'",*

 * * " […]*

```diff
@@ -1,56 +1,32 @@
 {
-    "data_mtime": 1681573243,
+    "data_mtime": 1683843440,
     "dep_lines": [
-        6,
-        4,
-        7,
-        8,
-        1,
-        1,
-        1,
-        1,
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
         5,
-        5,
-        5,
-        5,
-        30,
-        30,
-        30,
-        30,
-        30,
         30,
         30
     ],
     "dependencies": [
-        "collections.abc",
-        "__future__",
-        "contextlib",
-        "typing",
+        "tomlkit.container",
         "builtins",
         "abc",
-        "array",
-        "ctypes",
-        "io",
-        "mmap",
-        "os",
-        "pickle"
+        "typing"
     ],
-    "hash": "51f25d636074a960e9eb2bf88b9b96bdcbc17d4bf7d3897fec0bd3af11f1815e",
-    "id": "tomcli.cli._util",
-    "ignore_all": false,
-    "interface_hash": "f3687283861f779915f03712bb0bf09d1665cea4400b3083611262b57f4eb8e6",
-    "mtime": 1681573706,
+    "hash": "3824e45977773f9f04653e120fcfdd75cd58a6431aaad952e7fb2d1d306630e2",
+    "id": "tomlkit.toml_document",
+    "ignore_all": true,
+    "interface_hash": "41d90e6ed171badd184c00b285e764b8b5790aa519d60e8d3aca13cf9c1ecf45",
+    "mtime": 1684623295,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -84,13 +60,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "src/tomcli/cli/_util.py",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib/python3.11/site-packages/tomlkit/toml_document.py",
     "plugin_data": null,
-    "size": 468,
+    "size": 110,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/tomcli/cli/get.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/tomcli/cli/get.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/tomcli/cli/get.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/tomcli/cli/get.meta.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9303030303030303%*

 * *Differences: {"'data_mtime'": '1683843441',*

 * * "'dependencies'": "{insert: [(13, 'click.types')], delete: [20]}",*

 * * "'version_id'": "'1.3.0'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681573243,
+    "data_mtime": 1683843441,
     "dep_lines": [
         15,
         10,
         16,
         7,
         9,
         11,
@@ -56,22 +56,22 @@
         "typer",
         "builtins",
         "_typeshed",
         "abc",
         "click",
         "click.core",
         "click.shell_completion",
+        "click.types",
         "contextlib",
         "enum",
         "typer.core",
         "typer.main",
         "typer.params",
         "types",
-        "typing_extensions",
-        "click.types"
+        "typing_extensions"
     ],
     "hash": "8ed3a29a8b2ff83517974290a306644f665ad9639b3ebd9570acbee5535e7fae",
     "id": "tomcli.cli.get",
     "ignore_all": false,
     "interface_hash": "dd1f13834936238fc17e0f0ff15c6730e2d06f9d24ef23e2c68be75805c882e5",
     "mtime": 1681591974,
     "options": {
@@ -115,9 +115,9 @@
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
     "path": "src/tomcli/cli/get.py",
     "plugin_data": null,
     "size": 1544,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/tomcli/cli/set.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/tomcli/cli/set.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/tomcli/cli/set.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/tomcli/cli/set.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8310344827586207%*

 * *Differences: {"'data_mtime'": '1683843441',*

 * * "'dependencies'": "{insert: [(17, 'click.types')], delete: [27]}",*

 * * "'hash'": "'6937123ce2868fec15ecb25920fd4354af17391b025a44dab2293b7040e49650'",*

 * * "'mtime'": '1684623469',*

 * * "'size'": '8125',*

 * * "'version_id'": "'1.3.0'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681591852,
+    "data_mtime": 1683843441,
     "dep_lines": [
         22,
         12,
         23,
         7,
         9,
         10,
@@ -74,31 +74,31 @@
         "builtins",
         "_typeshed",
         "abc",
         "array",
         "click",
         "click.core",
         "click.shell_completion",
+        "click.types",
         "contextlib",
         "ctypes",
         "enum",
         "mmap",
         "pickle",
         "typer.core",
         "typer.main",
         "typer.models",
         "typer.params",
-        "typing_extensions",
-        "click.types"
+        "typing_extensions"
     ],
-    "hash": "0d615cd7d3805fe56f43dd3fffee17828b98498e744484d5c41d3d0a42e43348",
+    "hash": "6937123ce2868fec15ecb25920fd4354af17391b025a44dab2293b7040e49650",
     "id": "tomcli.cli.set",
     "ignore_all": false,
     "interface_hash": "a7e63f4692b8e2c5697eb5fdabb1f1734b447326a0c04d931bb53f48604c61ad",
-    "mtime": 1681573771,
+    "mtime": 1684623469,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -134,11 +134,11 @@
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
     "path": "src/tomcli/cli/set.py",
     "plugin_data": null,
-    "size": 8127,
+    "size": 8125,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/tomli_w/__init__.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/tomli_w/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/tomli_w/__init__.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/pathlib.meta.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6536904761904762%*

 * *Differences: {"'data_mtime'": '1683843439',*

 * * "'dep_lines'": '{insert: [(0, 12), (1, 1), (2, 2), (3, 13), (4, 14), (5, 15), (6, 16), (7, 17), '*

 * *                '(8, 1), (9, 1), (10, 1)], delete: [0]}',*

 * * "'dep_prios'": '{insert: [(0, 5), (1, 10), (2, 5), (3, 5), (4, 5), (5, 5), (6, 5), (9, 30), (10, '*

 * *                '30), (11, 30)]}',*

 * * "'dependencies'": "{insert: [(0, 'collections.abc'), (1, 'sys'), (2, '_typeshed'), (3, 'io'), (4, "*

 * *                   "'os'), (5, 'types'), (6, 'typing'), (7, 'typing_extensions'), (10, ' […]*

```diff
@@ -1,32 +1,62 @@
 {
-    "data_mtime": 1681571247,
+    "data_mtime": 1683843439,
     "dep_lines": [
-        4,
+        12,
+        1,
+        2,
+        13,
+        14,
+        15,
+        16,
+        17,
+        1,
+        1,
+        1,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
+        10,
+        5,
+        5,
+        5,
         5,
+        5,
+        5,
+        5,
+        30,
+        30,
+        30,
         30,
         30
     ],
     "dependencies": [
-        "tomli_w._writer",
+        "collections.abc",
+        "sys",
+        "_typeshed",
+        "io",
+        "os",
+        "types",
+        "typing",
+        "typing_extensions",
         "builtins",
         "abc",
-        "typing"
+        "array",
+        "ctypes",
+        "mmap",
+        "pickle"
     ],
-    "hash": "c3cdef9f865651a478788c5258258e5643d8f2a18943ebae5699c8b5dce69245",
-    "id": "tomli_w",
+    "hash": "af5d9944e5c7afe3dd4c99f5d83d4950e1d88bbcaba5db66ac57f946b5d10f41",
+    "id": "pathlib",
     "ignore_all": true,
-    "interface_hash": "cbfc201f42bbd11842b55dd5f80ad2f898a253e0d2952c0953f374e19058fc76",
-    "mtime": 1683082839,
+    "interface_hash": "a451d0ad4441309cae277e964031839c4ee01143f05a8ea778e13c2b5f179b86",
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -60,13 +90,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib/python3.11/site-packages/tomli_w/__init__.py",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/pathlib.pyi",
     "plugin_data": null,
-    "size": 157,
+    "size": 7949,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/tomli_w/_writer.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/tomli_w/_writer.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/tomli_w/_writer.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/tomli_w/_writer.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'data_mtime'": '1683843440', "'mtime'": '1684623295', "'version_id'": "'1.3.0'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681571247,
+    "data_mtime": 1683843440,
     "dep_lines": [
         3,
         1,
         4,
         5,
         6,
         7,
@@ -57,15 +57,15 @@
         "pickle",
         "typing_extensions"
     ],
     "hash": "9ffe972f0c70ca65c7c5e2695163fed5ff71d04c45ec4170fa64ffb21ce61a0b",
     "id": "tomli_w._writer",
     "ignore_all": true,
     "interface_hash": "01963175ccbf04b974516a502c2ae32a5f9c0f73ff326f20cb9505dc9323b8ae",
-    "mtime": 1683082839,
+    "mtime": 1684623295,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -103,9 +103,9 @@
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
     "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib/python3.11/site-packages/tomli_w/_writer.py",
     "plugin_data": null,
     "size": 6132,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/tomlkit/__init__.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/tomlkit/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/tomlkit/__init__.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/urllib/parse.meta.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6733333333333333%*

 * *Differences: {"'data_mtime'": '1683843440',*

 * * "'dep_lines'": '{insert: [(0, 2), (2, 3), (3, 4), (4, 7)]}',*

 * * "'dep_prios'": '{insert: [(0, 5), (1, 10), (2, 5), (3, 5)]}',*

 * * "'dependencies'": "{insert: [(0, 'collections.abc'), (1, 'sys'), (2, 'typing'), (3, "*

 * *                   "'typing_extensions'), (4, 'types'), (6, '_typeshed')], delete: [3, 0]}",*

 * * "'hash'": "'9287a7f222fba8bc2687913f39901a13c2ea5f00638158f8f20397227702b7d1'",*

 * * "'id'": "'urllib.parse'",*

 * * "'interface_hash'": "'f0749d9a12ff32a39b87a6a3fc1ecca2ebcd738be268d […]*

```diff
@@ -1,32 +1,44 @@
 {
-    "data_mtime": 1681571247,
+    "data_mtime": 1683843440,
     "dep_lines": [
+        2,
         1,
+        3,
+        4,
+        7,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
+        10,
+        5,
+        5,
+        5,
         5,
         30,
         30
     ],
     "dependencies": [
-        "tomlkit.api",
+        "collections.abc",
+        "sys",
+        "typing",
+        "typing_extensions",
+        "types",
         "builtins",
-        "abc",
-        "typing"
+        "_typeshed",
+        "abc"
     ],
-    "hash": "feee93b1ddf737d85ff86840869aa3eadd2ca0d9d33b92cfdae31d5b05fdc46d",
-    "id": "tomlkit",
+    "hash": "9287a7f222fba8bc2687913f39901a13c2ea5f00638158f8f20397227702b7d1",
+    "id": "urllib.parse",
     "ignore_all": true,
-    "interface_hash": "6b8614dd81fc21aadca9be9da93595eacfb2c9151bba35c2d55e64eef4bbd2dd",
-    "mtime": 1683082839,
+    "interface_hash": "f0749d9a12ff32a39b87a6a3fc1ecca2ebcd738be268dde5a88c9236882f7339",
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -60,13 +72,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib/python3.11/site-packages/tomlkit/__init__.py",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/urllib/parse.pyi",
     "plugin_data": null,
-    "size": 1148,
+    "size": 6532,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/tomlkit/_compat.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/tomlkit/_compat.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/tomlkit/_compat.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/subprocess.meta.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6898148148148148%*

 * *Differences: {"'data_mtime'": '1683843439',*

 * * "'dep_lines'": '{insert: [(1, 1), (2, 2), (4, 5)], delete: [5, 4, 0]}',*

 * * "'dep_prios'": '{insert: [(4, 5), (5, 5), (6, 5)], delete: [6, 5, 1]}',*

 * * "'dependencies'": "{insert: [(0, 'collections.abc'), (2, '_typeshed'), (3, 'types'), (5, "*

 * *                   "'typing_extensions'), (11, 'os')], delete: [12, 11, 5, 1, 0]}",*

 * * "'hash'": "'d4ba0d25f732153c8003c650e12155f803326ed0fac4281b27d871f56a50cd34'",*

 * * "'id'": "'subprocess'",*

 * * "'interface_hash'": "'1a69c378047966f5989ec904cd1b1d […]*

```diff
@@ -1,59 +1,59 @@
 {
-    "data_mtime": 1683082842,
+    "data_mtime": 1683843439,
     "dep_lines": [
-        1,
         3,
+        1,
+        2,
         4,
+        5,
         6,
         1,
         1,
         1,
         1,
         1,
         1,
-        1,
-        1,
         1
     ],
     "dep_prios": [
         5,
         10,
-        10,
         5,
         5,
-        30,
-        30,
+        5,
+        5,
+        5,
         30,
         30,
         30,
         30,
         30,
         30
     ],
     "dependencies": [
-        "__future__",
-        "contextlib",
+        "collections.abc",
         "sys",
+        "_typeshed",
+        "types",
         "typing",
+        "typing_extensions",
         "builtins",
-        "_typeshed",
         "abc",
         "array",
         "ctypes",
         "mmap",
-        "pickle",
-        "types",
-        "typing_extensions"
+        "os",
+        "pickle"
     ],
-    "hash": "829ecfeea361d32635760d30ca38820db570153754a3ba744308d5e13dc5ba7b",
-    "id": "tomlkit._compat",
+    "hash": "d4ba0d25f732153c8003c650e12155f803326ed0fac4281b27d871f56a50cd34",
+    "id": "subprocess",
     "ignore_all": true,
-    "interface_hash": "356684536ba841ed5c7bd895e38f54f1f73b9181d3ffae4621694b620a223762",
-    "mtime": 1683082839,
+    "interface_hash": "1a69c378047966f5989ec904cd1b1d993251601f6a9eae741e5a0e04af9ae035",
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -87,13 +87,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib/python3.11/site-packages/tomlkit/_compat.py",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/subprocess.pyi",
     "plugin_data": null,
-    "size": 513,
+    "size": 91091,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/tomlkit/_utils.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/tomlkit/_utils.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/tomlkit/_utils.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/_operator.meta.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6577777777777778%*

 * *Differences: {"'data_mtime'": '1683843440',*

 * * "'dep_lines'": '{insert: [(2, 2), (3, 4), (4, 5)], delete: [13, 12, 11, 10, 9, 8, 7, 6, 5, 4, 2, '*

 * *                '1, 0]}',*

 * * "'dep_prios'": '{insert: [(5, 5)], delete: [15, 14, 13, 12, 11, 10, 9, 8, 7, 1, 0]}',*

 * * "'dependencies'": "{insert: [(1, 'sys'), (2, '_typeshed'), (4, 'typing_extensions')], delete: "*

 * *                   '[16, 15, 14, 13, 12, 11, 10, 8, 7, 4, 3, 2, 1]}',*

 * * "'hash'": "'6af6cdd45bab26f05bd668e6a9adf75595caa87cbfb531af9addb4e0dd18636a'",*

 * * "'id'": "'_operator […]*

```diff
@@ -1,71 +1,41 @@
 {
-    "data_mtime": 1683082842,
+    "data_mtime": 1683843440,
     "dep_lines": [
-        5,
-        13,
-        1,
         3,
-        6,
-        11,
-        1,
-        1,
-        1,
-        1,
-        1,
-        1,
-        1,
-        1,
         1,
+        2,
+        4,
+        5,
         1,
         1
     ],
     "dep_prios": [
         5,
-        5,
-        5,
         10,
         5,
         5,
         5,
-        30,
-        30,
-        30,
-        30,
-        30,
-        30,
-        30,
-        30,
-        30,
+        5,
         30
     ],
     "dependencies": [
         "collections.abc",
-        "tomlkit._compat",
-        "__future__",
-        "re",
-        "datetime",
+        "sys",
+        "_typeshed",
         "typing",
+        "typing_extensions",
         "builtins",
-        "_collections_abc",
-        "_typeshed",
-        "abc",
-        "array",
-        "ctypes",
-        "enum",
-        "mmap",
-        "pickle",
-        "types",
-        "typing_extensions"
+        "abc"
     ],
-    "hash": "7d7d67edba028bbfdb05505e99acb09347b2c6a8536276563e10991c980166ff",
-    "id": "tomlkit._utils",
+    "hash": "6af6cdd45bab26f05bd668e6a9adf75595caa87cbfb531af9addb4e0dd18636a",
+    "id": "_operator",
     "ignore_all": true,
-    "interface_hash": "d9614e97cc2e07d645f1684d67fc9de46360e633a9fff2bbe1957f090b668f2d",
-    "mtime": 1683082839,
+    "interface_hash": "67cc042377da6a0902fae8d0822025f9497774d7bf8608bbdf579a9263d0be11",
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -99,13 +69,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib/python3.11/site-packages/tomlkit/_utils.py",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/_operator.pyi",
     "plugin_data": null,
-    "size": 4021,
+    "size": 6585,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/tomlkit/api.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/tomlkit/api.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/tomlkit/api.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/tomlkit/api.meta.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'data_mtime'": '1683843440', "'mtime'": '1684623295', "'version_id'": "'1.3.0'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1683082842,
+    "data_mtime": 1683843440,
     "dep_lines": [
         5,
         9,
         10,
         11,
         12,
         32,
@@ -66,15 +66,15 @@
         "types",
         "typing_extensions"
     ],
     "hash": "0e721dab30328b916909c4411b35fb59ed30a9d0630988a17b44da191d180381",
     "id": "tomlkit.api",
     "ignore_all": true,
     "interface_hash": "ba5cf3e9dca20ee08d854fb8dc509e39bfd8a377070a5ff1db2ae980f5e39c48",
-    "mtime": 1683082839,
+    "mtime": 1684623295,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -112,9 +112,9 @@
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
     "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib/python3.11/site-packages/tomlkit/api.py",
     "plugin_data": null,
     "size": 7065,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/tomlkit/container.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/tomlkit/container.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/tomlkit/container.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/tomlkit/container.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'data_mtime'": '1683843440', "'mtime'": '1684623295', "'version_id'": "'1.3.0'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1683082842,
+    "data_mtime": 1683843440,
     "dep_lines": [
         8,
         9,
         10,
         13,
         1,
         3,
@@ -63,15 +63,15 @@
         "types",
         "typing_extensions"
     ],
     "hash": "9c77ac86c1677bbecb6be2ea3b13132a4f71cae174f87af07cc952c2980fee1b",
     "id": "tomlkit.container",
     "ignore_all": true,
     "interface_hash": "7ca78f942d8ff23a3c293517c7336eee209ad6c4975151452d96a9160f2f24fd",
-    "mtime": 1683082839,
+    "mtime": 1684623295,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -109,9 +109,9 @@
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
     "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib/python3.11/site-packages/tomlkit/container.py",
     "plugin_data": null,
     "size": 28192,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/tomlkit/exceptions.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/tomlkit/exceptions.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/tomlkit/exceptions.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/tomlkit/exceptions.meta.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'data_mtime'": '1683843440', "'mtime'": '1684623295', "'version_id'": "'1.3.0'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1683082842,
+    "data_mtime": 1683843440,
     "dep_lines": [
         1,
         3,
         1,
         1,
         1
     ],
@@ -21,15 +21,15 @@
         "abc",
         "typing_extensions"
     ],
     "hash": "4dd787cbd7bdca25c8f28491f9e0b1aad40e5819721609fbb538efa42580a93c",
     "id": "tomlkit.exceptions",
     "ignore_all": true,
     "interface_hash": "2ad4cff74c96bfb909f7d7f7fa61ab14d93785531805898408641c4f0a3ba828",
-    "mtime": 1683082839,
+    "mtime": 1684623295,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -67,9 +67,9 @@
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
     "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib/python3.11/site-packages/tomlkit/exceptions.py",
     "plugin_data": null,
     "size": 5487,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/tomlkit/items.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/tomlkit/items.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/tomlkit/items.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/tomlkit/items.meta.json`

 * *Files 7% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'data_mtime'": '1683843440', "'mtime'": '1684623295', "'version_id'": "'1.3.0'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1683082842,
+    "data_mtime": 1683843440,
     "dep_lines": [
         24,
         26,
         28,
         47,
         1,
         3,
@@ -75,15 +75,15 @@
         "types",
         "typing_extensions"
     ],
     "hash": "a90d23cb34b1d1aa652baa9da4853eee31060b96c7a384ccbba6cfc67918f93b",
     "id": "tomlkit.items",
     "ignore_all": true,
     "interface_hash": "cc8fbe4656b54f25c0aaadad8664e3f64f5c29d8d59d0d4c9276eee43b73a81a",
-    "mtime": 1683082839,
+    "mtime": 1684623295,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -121,9 +121,9 @@
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
     "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib/python3.11/site-packages/tomlkit/items.py",
     "plugin_data": null,
     "size": 51695,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/tomlkit/parser.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/tomlkit/parser.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/tomlkit/parser.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/tomlkit/parser.meta.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'data_mtime'": '1683843440', "'mtime'": '1684623295', "'version_id'": "'1.3.0'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1683082842,
+    "data_mtime": 1683843440,
     "dep_lines": [
         7,
         8,
         11,
         12,
         25,
         46,
@@ -75,15 +75,15 @@
         "typing",
         "typing_extensions"
     ],
     "hash": "701b82f53dd9aef295b70ccad0f144a39ae826aaeeec0d1c5cc1612a571bfcb5",
     "id": "tomlkit.parser",
     "ignore_all": true,
     "interface_hash": "01100aba0ae5f3022be815cec951fcc5530591ee0f448be293585e96c4ebdbd9",
-    "mtime": 1683082839,
+    "mtime": 1684623295,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -121,9 +121,9 @@
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
     "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib/python3.11/site-packages/tomlkit/parser.py",
     "plugin_data": null,
     "size": 37839,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/tomlkit/source.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/tomlkit/source.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/tomlkit/source.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/click/_textwrap.meta.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6836363636363636%*

 * *Differences: {"'data_mtime'": '1683843440',*

 * * "'dep_lines'": '{insert: [(1, 2)], delete: [4, 1, 0]}',*

 * * "'dep_prios'": '{insert: [(0, 10), (1, 10)], delete: [3, 2, 1, 0]}',*

 * * "'dependencies'": "{insert: [(0, 'textwrap'), (2, 'contextlib')], delete: [3, 2, 1, 0]}",*

 * * "'hash'": "'d747d0eb839c05432e2bb985be1f37eb7feea0ec4f95122d64198acd12438286'",*

 * * "'id'": "'click._textwrap'",*

 * * "'interface_hash'": "'7434e38ac65160d707a6362d23cee3aab3b4085cebbe903a6fb6b9b9c2b45038'",*

 * * "'mtime'": '1684623295',*

 * * "'path'": "'/home/gotmax/Sync/git- […]*

```diff
@@ -1,47 +1,41 @@
 {
-    "data_mtime": 1683082842,
+    "data_mtime": 1683843440,
     "dep_lines": [
-        6,
-        8,
         1,
+        2,
         3,
-        4,
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
-        5,
-        5,
-        5,
-        5,
+        10,
+        10,
         5,
         5,
         30,
         30,
         30
     ],
     "dependencies": [
-        "tomlkit.exceptions",
-        "tomlkit.toml_char",
-        "__future__",
-        "copy",
+        "textwrap",
         "typing",
+        "contextlib",
         "builtins",
         "_typeshed",
         "abc",
         "typing_extensions"
     ],
-    "hash": "9f046b014909d82c830ca16ce23a3da3446934c35a34da0b0c58b0a3864d6533",
-    "id": "tomlkit.source",
+    "hash": "d747d0eb839c05432e2bb985be1f37eb7feea0ec4f95122d64198acd12438286",
+    "id": "click._textwrap",
     "ignore_all": true,
-    "interface_hash": "2aa600a17b944e8001cbf04116c4a852d2c953e4becdd6571bd32609d8ee4153",
-    "mtime": 1683082839,
+    "interface_hash": "7434e38ac65160d707a6362d23cee3aab3b4085cebbe903a6fb6b9b9c2b45038",
+    "mtime": 1684623295,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -75,13 +69,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib/python3.11/site-packages/tomlkit/source.py",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib/python3.11/site-packages/click/_textwrap.py",
     "plugin_data": null,
-    "size": 4823,
+    "size": 1353,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/tomlkit/toml_char.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/tomlkit/toml_char.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/tomlkit/toml_char.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/sys.meta.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6519230769230769%*

 * *Differences: {"'data_mtime'": '1683843439',*

 * * "'dep_lines'": '{insert: [(0, 4), (1, 5), (2, 6), (3, 2), (4, 3), (5, 7), (6, 8), (7, 9), (8, '*

 * *                '10)], delete: [1, 0]}',*

 * * "'dep_prios'": '{insert: [(0, 5), (1, 5), (2, 5), (3, 5), (4, 5), (5, 5), (6, 5), (7, 5)], '*

 * *                'delete: [0]}',*

 * * "'dependencies'": "{insert: [(0, 'collections.abc'), (1, 'importlib.abc'), (2, "*

 * *                   "'importlib.machinery'), (3, '_typeshed'), (5, 'io'), (6, 'types'), (8, "*

 * *                   "'typing_extensions'),  […]*

```diff
@@ -1,32 +1,53 @@
 {
-    "data_mtime": 1681571246,
+    "data_mtime": 1683843439,
     "dep_lines": [
-        1,
-        1,
+        4,
+        5,
+        6,
+        2,
+        3,
+        7,
+        8,
+        9,
+        10,
         1,
         1
     ],
     "dep_prios": [
-        10,
+        5,
+        5,
+        5,
+        5,
+        5,
+        5,
+        5,
+        5,
         5,
         30,
         30
     ],
     "dependencies": [
-        "string",
+        "collections.abc",
+        "importlib.abc",
+        "importlib.machinery",
+        "_typeshed",
         "builtins",
+        "io",
+        "types",
+        "typing",
+        "typing_extensions",
         "abc",
-        "typing"
+        "importlib"
     ],
-    "hash": "c37b10674768959d6a8d9d91c63fecbef96944d34607f7e37c17180f48059c3b",
-    "id": "tomlkit.toml_char",
+    "hash": "bb33fcc38a16497298549aa7d67ceac363fdf6c670ea0baeed5f44f5a24e2b3b",
+    "id": "sys",
     "ignore_all": true,
-    "interface_hash": "0f6e6b41ade4473ef928872c918cc6ba9fe19aad46409e3d07e03bf4e517215a",
-    "mtime": 1683082839,
+    "interface_hash": "f63a10e5fbbc430a7e77ee851a0a39543928178e2d28437e79f555e4a40dbf64",
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -60,13 +81,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib/python3.11/site-packages/tomlkit/toml_char.py",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/sys.pyi",
     "plugin_data": null,
-    "size": 1291,
+    "size": 11681,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/tomlkit/toml_document.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/tomlkit/toml_document.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/tomlkit/toml_document.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/types.meta.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6642087542087542%*

 * *Differences: {"'data_mtime'": '1683843439',*

 * * "'dep_lines'": '{insert: [(0, 3), (1, 16), (3, 2), (4, 19), (5, 20), (6, 607)], delete: [0]}',*

 * * "'dep_prios'": '{insert: [(0, 5), (1, 5), (2, 10), (3, 5), (4, 5)]}',*

 * * "'dependencies'": "{insert: [(0, 'collections.abc'), (1, 'importlib.machinery'), (2, 'sys'), (3, "*

 * *                   "'_typeshed'), (4, 'typing'), (5, 'typing_extensions'), (8, 'importlib')], "*

 * *                   'delete: [3, 0]}',*

 * * "'hash'": "'bb1594589ec5ca09736286838e17153b5f7c33e7eaa783ab884856ab9bbd8f04'", […]*

```diff
@@ -1,32 +1,47 @@
 {
-    "data_mtime": 1681571247,
+    "data_mtime": 1683843439,
     "dep_lines": [
+        3,
+        16,
         1,
-        1,
+        2,
+        19,
+        20,
+        607,
         1,
         1
     ],
     "dep_prios": [
         5,
         5,
+        10,
+        5,
+        5,
+        5,
+        5,
         30,
         30
     ],
     "dependencies": [
-        "tomlkit.container",
+        "collections.abc",
+        "importlib.machinery",
+        "sys",
+        "_typeshed",
+        "typing",
+        "typing_extensions",
         "builtins",
         "abc",
-        "typing"
+        "importlib"
     ],
-    "hash": "3824e45977773f9f04653e120fcfdd75cd58a6431aaad952e7fb2d1d306630e2",
-    "id": "tomlkit.toml_document",
+    "hash": "bb1594589ec5ca09736286838e17153b5f7c33e7eaa783ab884856ab9bbd8f04",
+    "id": "types",
     "ignore_all": true,
-    "interface_hash": "41d90e6ed171badd184c00b285e764b8b5790aa519d60e8d3aca13cf9c1ecf45",
-    "mtime": 1683082839,
+    "interface_hash": "d837e1814d54b77a49618bbb00979340d14c37e5d61c6843e08957a9c2fe5c38",
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -60,13 +75,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib/python3.11/site-packages/tomlkit/toml_document.py",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/types.pyi",
     "plugin_data": null,
-    "size": 110,
+    "size": 20809,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/typer/__init__.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/typer/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/typer/__init__.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/typer/_typing.meta.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6616946778711484%*

 * *Differences: {"'data_mtime'": '1683843441',*

 * * "'dep_lines'": '{insert: [(0, 101), (1, 491), (2, 5), (3, 6), (6, 43), (7, 1), (8, 1), (9, 1), '*

 * *                '(10, 1), (11, 1)], delete: [7, 6, 5, 4, 2, 1]}',*

 * * "'dep_prios'": '{insert: [(1, 20), (8, 30), (9, 30), (10, 30), (11, 30), (12, 30)], delete: [1, '*

 * *                '0]}',*

 * * "'dependencies'": "{insert: [(0, 'collections.abc'), (1, 'typer.utils'), (2, 'sys'), (3, 'os'), "*

 * *                   "(4, 'typing'), (5, 'typing_extensions'), (6, 'types'), (8, "*

 * *                […]*

```diff
@@ -1,53 +1,65 @@
 {
-    "data_mtime": 1681571164,
+    "data_mtime": 1683843441,
     "dep_lines": [
+        101,
+        491,
+        5,
+        6,
         7,
-        10,
-        22,
         29,
-        30,
-        32,
-        38,
-        5,
+        43,
+        1,
+        1,
+        1,
+        1,
+        1,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
-        5,
-        5,
+        20,
         10,
         5,
         5,
         5,
         5,
         5,
         30,
+        30,
+        30,
+        30,
+        30,
+        30,
         30
     ],
     "dependencies": [
-        "click.exceptions",
-        "click.termui",
-        "click.utils",
-        "typer.colors",
-        "typer.main",
-        "typer.models",
-        "typer.params",
-        "shutil",
+        "collections.abc",
+        "typer.utils",
+        "sys",
+        "os",
+        "typing",
+        "typing_extensions",
+        "types",
         "builtins",
+        "_collections_abc",
+        "_typeshed",
         "abc",
-        "typing"
+        "array",
+        "ctypes",
+        "mmap",
+        "pickle"
     ],
-    "hash": "c5ff549135bc942c56bd006b25e9430d11aca40c240e6d2f7762a28e11ea3f28",
-    "id": "typer",
+    "hash": "1211bc8ebacfc892f46d646cc389f5e3793aa03da83de623e2c65f2b52adc389",
+    "id": "typer._typing",
     "ignore_all": true,
-    "interface_hash": "67656c94cc4fb27dcc533749f8b383284f1fe2ca9d49490955bd0df882a8877e",
-    "mtime": 1683082840,
+    "interface_hash": "ee04d26abd812e1a22b73e94fed69d4fb3bc2557408832322b942acc9dd662f1",
+    "mtime": 1684623295,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -81,13 +93,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib/python3.11/site-packages/typer/__init__.py",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib/python3.11/site-packages/typer/_typing.py",
     "plugin_data": null,
-    "size": 1602,
+    "size": 19743,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/typer/_compat_utils.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/typer/_compat_utils.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/typer/_compat_utils.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/typer/_compat_utils.meta.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9%*

 * *Differences: {"'data_mtime'": '1683843441', "'mtime'": '1684623295', "'version_id'": "'1.3.0'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681571164,
+    "data_mtime": 1683843441,
     "dep_lines": [
         1,
         1,
         1,
         1,
         1,
         1,
@@ -36,15 +36,15 @@
         "typing",
         "typing_extensions"
     ],
     "hash": "929e3d1ab540c6f3dc505b64c2941ffa96e066ce970270984765790ded7a5a9a",
     "id": "typer._compat_utils",
     "ignore_all": true,
     "interface_hash": "7f36b6ed07717cffdd326cef1e14ad4ec7a2c96065b0a424803ed22860b704a9",
-    "mtime": 1683082840,
+    "mtime": 1684623295,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -82,9 +82,9 @@
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
     "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib/python3.11/site-packages/typer/_compat_utils.py",
     "plugin_data": null,
     "size": 94,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/typer/_completion_click7.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/typer/_completion_click7.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/typer/_completion_click7.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/typer/_completion_click8.meta.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6797338603425561%*

 * *Differences: {"'data_mtime'": '1683843441',*

 * * "'dep_lines'": '{insert: [(0, 7), (2, 10), (6, 4), (7, 6), (18, 19)], delete: [19, 18, 7, 6, 5, '*

 * *                '4]}',*

 * * "'dep_prios'": '{insert: [(0, 10), (1, 10), (6, 5)], delete: [18, 8, 7, 6]}',*

 * * "'dependencies'": "{insert: [(0, 'click.parser'), (1, 'click.shell_completion'), (6, 'typing'), "*

 * *                   "(14, 'enum')], delete: [16, 15, 11, 10]}",*

 * * "'hash'": "'d267196e0547f701e7f4e0e0d2032b91a7da14a817eafbb690a5c74dc9e10f4b'",*

 * * "'id'": "'typer._completion_click8'" […]*

```diff
@@ -1,78 +1,76 @@
 {
-    "data_mtime": 1681571164,
+    "data_mtime": 1683843441,
     "dep_lines": [
+        7,
         8,
+        10,
         1,
         2,
         3,
-        5,
-        1,
-        1,
-        1,
+        4,
+        6,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
-        6,
-        11
+        19
     ],
     "dep_prios": [
+        10,
+        10,
         5,
         10,
         10,
         10,
+        5,
         10,
         5,
         30,
         30,
         30,
         30,
         30,
         30,
         30,
         30,
         30,
-        30,
-        30,
-        30,
-        10,
         10
     ],
     "dependencies": [
+        "click.parser",
+        "click.shell_completion",
         "typer._completion_shared",
         "os",
         "re",
         "sys",
+        "typing",
         "click",
         "builtins",
         "_typeshed",
         "abc",
         "array",
         "click.core",
-        "click.parser",
-        "click.utils",
         "ctypes",
+        "enum",
         "mmap",
         "pickle",
-        "typer._completion_click8",
-        "typing",
         "typing_extensions"
     ],
-    "hash": "b7c4968f29b29d503c7340461b8e37a8a77649ae7b7a207f2c54dd44313db777",
-    "id": "typer._completion_click7",
+    "hash": "d267196e0547f701e7f4e0e0d2032b91a7da14a817eafbb690a5c74dc9e10f4b",
+    "id": "typer._completion_click8",
     "ignore_all": true,
-    "interface_hash": "f0b8c293ac0032d12c7d09207dbed717231333e23385716ee4454fa383d860c4",
-    "mtime": 1683082840,
+    "interface_hash": "2c3d80fe3b41fdd144262698bef94a44546de91fd821df25636f31eafc3c7ab1",
+    "mtime": 1684623295,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -106,16 +104,15 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib/python3.11/site-packages/typer/_completion_click7.py",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib/python3.11/site-packages/typer/_completion_click8.py",
     "plugin_data": null,
-    "size": 4957,
+    "size": 6688,
     "suppressed": [
-        "click._bashcomplete",
         "shellingham"
     ],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/typer/_completion_click8.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/typer/_completion_click8.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/typer/_completion_click8.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/click/exceptions.meta.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6564682539682539%*

 * *Differences: {"'data_mtime'": '1683843441',*

 * * "'dep_lines'": '{insert: [(0, 6)], delete: [18, 8, 7, 6, 1]}',*

 * * "'dep_prios'": '{insert: [(1, 5), (2, 25)], delete: [18, 9, 7, 3, 1, 0]}',*

 * * "'dependencies'": "{insert: [(0, 'click._compat'), (1, 'click.utils'), (2, 'click.core'), (5, "*

 * *                   "'gettext'), (10, 'click.types'), (14, 'types')], delete: [17, 14, 12, 7, 5, 4, "*

 * *                   '2, 1, 0]}',*

 * * "'hash'": "'ee00da2c6b8564178237063d11132c176f99dd1f45bead3d65ce886522a3b1ea'",*

 * * "'id'": "'click.exceptions'", […]*

```diff
@@ -1,76 +1,65 @@
 {
-    "data_mtime": 1681571164,
+    "data_mtime": 1683843441,
     "dep_lines": [
+        6,
         7,
-        8,
         10,
         1,
         2,
         3,
-        4,
-        6,
-        1,
-        1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
-        19
+        1
     ],
     "dep_prios": [
-        10,
-        10,
         5,
-        10,
+        5,
+        25,
         10,
         10,
         5,
-        10,
         5,
         30,
         30,
         30,
         30,
         30,
         30,
         30,
-        30,
-        30,
-        10
+        30
     ],
     "dependencies": [
-        "click.parser",
-        "click.shell_completion",
-        "typer._completion_shared",
+        "click._compat",
+        "click.utils",
+        "click.core",
         "os",
-        "re",
-        "sys",
         "typing",
-        "click",
+        "gettext",
         "builtins",
         "_typeshed",
         "abc",
         "array",
-        "click.core",
+        "click.types",
         "ctypes",
-        "enum",
         "mmap",
         "pickle",
-        "typing_extensions"
+        "types"
     ],
-    "hash": "d267196e0547f701e7f4e0e0d2032b91a7da14a817eafbb690a5c74dc9e10f4b",
-    "id": "typer._completion_click8",
+    "hash": "ee00da2c6b8564178237063d11132c176f99dd1f45bead3d65ce886522a3b1ea",
+    "id": "click.exceptions",
     "ignore_all": true,
-    "interface_hash": "2c3d80fe3b41fdd144262698bef94a44546de91fd821df25636f31eafc3c7ab1",
-    "mtime": 1683082840,
+    "interface_hash": "f24b97a0246f7b5bf481f49537df8452800f697851e761591030da46680acef9",
+    "mtime": 1684623295,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -104,15 +93,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib/python3.11/site-packages/typer/_completion_click8.py",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib/python3.11/site-packages/click/exceptions.py",
     "plugin_data": null,
-    "size": 6688,
-    "suppressed": [
-        "shellingham"
-    ],
-    "version_id": "1.2.0"
+    "size": 9167,
+    "suppressed": [],
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/typer/_completion_shared.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/typer/_completion_shared.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/typer/_completion_shared.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/typer/_completion_shared.meta.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8953823953823953%*

 * *Differences: {"'data_mtime'": '1683843441',*

 * * "'dep_lines'": '{insert: [(8, 1)]}',*

 * * "'dep_prios'": '{insert: [(9, 30)]}',*

 * * "'dependencies'": "{insert: [(19, 'types')]}",*

 * * "'mtime'": '1684623295',*

 * * "'version_id'": "'1.3.0'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681571164,
+    "data_mtime": 1683843441,
     "dep_lines": [
         1,
         2,
         3,
         4,
         5,
         6,
@@ -17,14 +17,15 @@
         1,
         1,
         1,
         1,
         1,
         1,
         1,
+        1,
         12
     ],
     "dep_prios": [
         10,
         10,
         10,
         10,
@@ -40,14 +41,15 @@
         30,
         30,
         30,
         30,
         30,
         30,
         30,
+        30,
         10
     ],
     "dependencies": [
         "os",
         "re",
         "subprocess",
         "sys",
@@ -62,21 +64,22 @@
         "click.exceptions",
         "click.globals",
         "click.utils",
         "ctypes",
         "io",
         "mmap",
         "pickle",
+        "types",
         "typing_extensions"
     ],
     "hash": "07d57ab9af0bc9668092450a3be34d73bbc19793d036b5b9a1366b0434c02eb8",
     "id": "typer._completion_shared",
     "ignore_all": true,
     "interface_hash": "8498eb771d2aea5d8570bba9290f4503c1ddcdf8924e38670f1819b42ccd07d8",
-    "mtime": 1683082840,
+    "mtime": 1684623295,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -116,9 +119,9 @@
     },
     "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib/python3.11/site-packages/typer/_completion_shared.py",
     "plugin_data": null,
     "size": 8541,
     "suppressed": [
         "shellingham"
     ],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/typer/_typing.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/typer/_typing.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/typer/_typing.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/uuid.meta.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6874074074074075%*

 * *Differences: {"'data_mtime'": '1683843440',*

 * * "'dep_lines'": '{insert: [(1, 2), (2, 3), (3, 4)], delete: [6, 5, 4, 3, 2, 1, 0]}',*

 * * "'dep_prios'": '{delete: [8, 3, 1, 0]}',*

 * * "'dependencies'": "{insert: [(1, '_typeshed'), (2, 'enum'), (10, 'typing')], delete: [9, 8, 6, 4, "*

 * *                   '3, 1, 0]}',*

 * * "'hash'": "'8c28006bde3a41ef255422bf6626035a62a8e9edaf430622e7f05e329a3c422e'",*

 * * "'id'": "'uuid'",*

 * * "'interface_hash'": "'5184910ef79cb98c9c1c17ad419e263fc62447917ee959d42c10922c84c3c15d'",*

 * * "'mtime'": '1684623296',*

 * * "'p […]*

```diff
@@ -1,65 +1,53 @@
 {
-    "data_mtime": 1683082842,
+    "data_mtime": 1683843440,
     "dep_lines": [
-        101,
-        491,
-        5,
-        6,
-        7,
-        29,
-        43,
         1,
+        2,
+        3,
+        4,
         1,
         1,
         1,
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
-        5,
-        20,
         10,
         5,
         5,
         5,
         5,
-        5,
-        30,
         30,
         30,
         30,
         30,
         30,
         30
     ],
     "dependencies": [
-        "collections.abc",
-        "typer.utils",
         "sys",
-        "os",
-        "typing",
+        "_typeshed",
+        "enum",
         "typing_extensions",
-        "types",
         "builtins",
-        "_collections_abc",
-        "_typeshed",
         "abc",
         "array",
         "ctypes",
         "mmap",
-        "pickle"
+        "pickle",
+        "typing"
     ],
-    "hash": "1211bc8ebacfc892f46d646cc389f5e3793aa03da83de623e2c65f2b52adc389",
-    "id": "typer._typing",
+    "hash": "8c28006bde3a41ef255422bf6626035a62a8e9edaf430622e7f05e329a3c422e",
+    "id": "uuid",
     "ignore_all": true,
-    "interface_hash": "ee04d26abd812e1a22b73e94fed69d4fb3bc2557408832322b942acc9dd662f1",
-    "mtime": 1683082840,
+    "interface_hash": "5184910ef79cb98c9c1c17ad419e263fc62447917ee959d42c10922c84c3c15d",
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -93,13 +81,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib/python3.11/site-packages/typer/_typing.py",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/uuid.pyi",
     "plugin_data": null,
-    "size": 19743,
+    "size": 2558,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/typer/colors.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/typer/colors.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/typer/colors.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/_collections_abc.meta.json`

 * *Files 19% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.669047619047619%*

 * *Differences: {"'data_mtime'": '1683843440',*

 * * "'dep_lines'": '{insert: [(1, 2), (2, 3), (3, 32)]}',*

 * * "'dep_prios'": '{insert: [(0, 10), (2, 5), (3, 5), (4, 5)], delete: [1]}',*

 * * "'dependencies'": "{insert: [(0, 'sys'), (1, 'types'), (2, 'typing'), (3, 'typing_extensions')], "*

 * *                   'delete: [2]}',*

 * * "'hash'": "'a1242071aa8e060f1cb055c8d542467362f026499a9139fbcf15943f854ffcf5'",*

 * * "'id'": "'_collections_abc'",*

 * * "'interface_hash'": "'8462eba7ef0c128e18111644a04ba39f65ff94458e18e0fb602331c9f0f2c666'",*

 * * "'mtime'":  […]*

```diff
@@ -1,29 +1,38 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843440,
     "dep_lines": [
         1,
+        2,
+        3,
+        32,
         1,
         1
     ],
     "dep_prios": [
+        10,
+        5,
+        5,
+        5,
         5,
-        30,
         30
     ],
     "dependencies": [
+        "sys",
+        "types",
+        "typing",
+        "typing_extensions",
         "builtins",
-        "abc",
-        "typing"
+        "abc"
     ],
-    "hash": "7b8da3f2e079db484ba57e42ff47e247738ea0814c6e13b700366fbfa865015f",
-    "id": "typer.colors",
+    "hash": "a1242071aa8e060f1cb055c8d542467362f026499a9139fbcf15943f854ffcf5",
+    "id": "_collections_abc",
     "ignore_all": true,
-    "interface_hash": "b8723b40b62875262b3f7214a0af15e5a533172dfd03f9929ebf8a731ea8c105",
-    "mtime": 1683082840,
+    "interface_hash": "8462eba7ef0c128e18111644a04ba39f65ff94458e18e0fb602331c9f0f2c666",
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -57,13 +66,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib/python3.11/site-packages/typer/colors.py",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/_collections_abc.pyi",
     "plugin_data": null,
-    "size": 430,
+    "size": 2123,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/typer/completion.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/typer/completion.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/typer/completion.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/typer/completion.meta.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8895833333333333%*

 * *Differences: {"'data_mtime'": '1683843441',*

 * * "'dependencies'": "{insert: [(15, 'array'), (19, 'click.utils'), (21, 'enum'), (23, 'pathlib'), "*

 * *                   "(26, 'typing_extensions')], delete: [21, 20, 19, 18, 17]}",*

 * * "'mtime'": '1684623295',*

 * * "'version_id'": "'1.3.0'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681571164,
+    "data_mtime": 1683843441,
     "dep_lines": [
         7,
         8,
         9,
         10,
         11,
         107,
@@ -72,32 +72,32 @@
         "os",
         "sys",
         "typing",
         "click",
         "builtins",
         "_collections_abc",
         "abc",
+        "array",
         "click.core",
         "click.termui",
-        "click.utils",
-        "enum",
-        "pathlib",
-        "typing_extensions",
-        "array",
         "click.types",
+        "click.utils",
         "ctypes",
+        "enum",
         "mmap",
+        "pathlib",
         "pickle",
-        "types"
+        "types",
+        "typing_extensions"
     ],
     "hash": "655da34a812d7b0b0ea4df6b2e4111dc604bb1c3da18129a9d93ae11b0ba136f",
     "id": "typer.completion",
     "ignore_all": true,
     "interface_hash": "1671f04f46cd13c1e2f4d5ecd4415eaa27f86f1e53c85ec99d39c15d76e853d8",
-    "mtime": 1683082840,
+    "mtime": 1684623295,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -137,9 +137,9 @@
     },
     "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib/python3.11/site-packages/typer/completion.py",
     "plugin_data": null,
     "size": 4979,
     "suppressed": [
         "shellingham"
     ],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/typer/core.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/typer/core.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/typer/core.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/typer/core.meta.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8925925925925926%*

 * *Differences: {"'data_mtime'": '1683843441',*

 * * "'dependencies'": "{insert: [(22, 'array'), (25, 'ctypes'), (26, 'mmap'), (27, 'pickle')], "*

 * *                   'delete: [31, 30, 29, 28]}',*

 * * "'mtime'": '1684623295',*

 * * "'version_id'": "'1.3.0'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681571164,
+    "data_mtime": 1683843441,
     "dep_lines": [
         21,
         22,
         23,
         24,
         25,
         26,
@@ -89,30 +89,30 @@
         "click",
         "typer",
         "warnings",
         "builtins",
         "_typeshed",
         "_warnings",
         "abc",
+        "array",
         "click.exceptions",
         "contextlib",
+        "ctypes",
+        "mmap",
+        "pickle",
         "posixpath",
         "typer._completion_click8",
         "types",
-        "typing_extensions",
-        "array",
-        "ctypes",
-        "mmap",
-        "pickle"
+        "typing_extensions"
     ],
     "hash": "4e854e1f3b38cac177e4a25af37050960cc2cdc54d10c257791d45283ac3a5a9",
     "id": "typer.core",
     "ignore_all": true,
     "interface_hash": "c200efef894f610a0339e97424caff46e2b25ad43fa067883c5ab60d79d95dd0",
-    "mtime": 1683082840,
+    "mtime": 1684623295,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -152,9 +152,9 @@
     },
     "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib/python3.11/site-packages/typer/core.py",
     "plugin_data": null,
     "size": 26545,
     "suppressed": [
         "rich"
     ],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/typer/main.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/typer/main.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/typer/main.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/typer/main.meta.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8941071428571429%*

 * *Differences: {"'data_mtime'": '1683843441',*

 * * "'dep_lines'": '{insert: [(16, 1), (17, 1)]}',*

 * * "'dep_prios'": '{insert: [(17, 30), (18, 30)]}',*

 * * "'dependencies'": "{insert: [(23, 'click.globals'), (30, 'posixpath')]}",*

 * * "'mtime'": '1684623295',*

 * * "'version_id'": "'1.3.0'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "data_mtime": 1681571164,
+    "data_mtime": 1683843441,
     "dep_lines": [
         16,
         17,
         18,
         37,
         1,
         2,
@@ -27,14 +27,16 @@
         1,
         1,
         1,
         1,
         1,
         1,
         1,
+        1,
+        1,
         41,
         42,
         40
     ],
     "dep_prios": [
         5,
         5,
@@ -62,14 +64,16 @@
         30,
         30,
         30,
         30,
         30,
         30,
         30,
+        30,
+        30,
         5,
         5,
         10
     ],
     "dependencies": [
         "typer.completion",
         "typer.core",
@@ -90,27 +94,29 @@
         "builtins",
         "_collections_abc",
         "_typeshed",
         "abc",
         "array",
         "click.core",
         "click.exceptions",
+        "click.globals",
         "click.shell_completion",
         "click.types",
         "ctypes",
         "io",
         "mmap",
         "pickle",
+        "posixpath",
         "typing_extensions"
     ],
     "hash": "84a1b3cda07cad9e7f4498ccfe456a2792be53551831289a8eeaf066e204f851",
     "id": "typer.main",
     "ignore_all": true,
     "interface_hash": "bfdc79e51c9095a483471cfee27010e6d21be52c1d155572e3a3d0ed9fde00cb",
-    "mtime": 1683082840,
+    "mtime": 1684623295,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -152,9 +158,9 @@
     "plugin_data": null,
     "size": 39310,
     "suppressed": [
         "rich.console",
         "rich.traceback",
         "rich"
     ],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/typer/models.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/typer/models.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/typer/models.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/typer/utils.meta.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.672962962962963%*

 * *Differences: {"'data_mtime'": '1683843441',*

 * * "'dep_lines'": '{insert: [(0, 7), (1, 8), (5, 5), (6, 1), (7, 1)], delete: [7, 3, 2, 1, 0]}',*

 * * "'dep_prios'": '{insert: [(3, 5), (4, 5), (5, 5), (7, 30), (8, 30)], delete: [5, 4, 3, 2, 1]}',*

 * * "'dependencies'": "{insert: [(0, 'typer._typing'), (1, 'typer.models'), (3, 'copy'), (5, "*

 * *                   "'typing_extensions'), (8, 'click'), (10, 'click.shell_completion'), (12, "*

 * *                   "'types')], delete: [12, 7, 5, 3, 2, 1, 0]}",*

 * * "'hash'": "'2eac497a8186c33e8f50339a […]*

```diff
@@ -1,59 +1,59 @@
 {
-    "data_mtime": 1683082842,
+    "data_mtime": 1683843441,
     "dep_lines": [
-        18,
-        22,
-        24,
-        25,
+        7,
+        8,
         1,
         2,
         3,
-        16,
+        5,
+        1,
+        1,
         1,
         1,
         1,
         1,
         1
     ],
     "dep_prios": [
         5,
-        25,
-        25,
-        25,
-        10,
-        10,
         5,
         10,
         5,
+        5,
+        5,
+        5,
+        30,
+        30,
         30,
         30,
         30,
         30
     ],
     "dependencies": [
-        "typer._compat_utils",
-        "click.shell_completion",
-        "typer.core",
-        "typer.main",
+        "typer._typing",
+        "typer.models",
         "inspect",
-        "io",
+        "copy",
         "typing",
-        "click",
+        "typing_extensions",
         "builtins",
         "abc",
+        "click",
         "click.core",
+        "click.shell_completion",
         "click.types",
-        "enum"
+        "types"
     ],
-    "hash": "0d625201001a209a45048efff3154017d132f4d3479b8755ea29f6b81ecdeca9",
-    "id": "typer.models",
+    "hash": "2eac497a8186c33e8f50339adabeba874b14695217c4faeef2ad1b8fcee7fd4e",
+    "id": "typer.utils",
     "ignore_all": true,
-    "interface_hash": "db492461bb763161350ae9740b2d8fde7036d8a2b37090afef47e1d08451eebe",
-    "mtime": 1683082840,
+    "interface_hash": "da04e072a72c41f7d69e1a60105be13b0fa676d7d978db357cb866c4db5a93ca",
+    "mtime": 1684623295,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -87,13 +87,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib/python3.11/site-packages/typer/models.py",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib/python3.11/site-packages/typer/utils.py",
     "plugin_data": null,
-    "size": 15981,
+    "size": 7293,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/typer/params.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/typer/params.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/typer/params.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/importlib/__init__.meta.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6759259259259259%*

 * *Differences: {"'data_mtime'": '1683843440',*

 * * "'dep_lines'": '{insert: [(1, 2)], delete: [4, 1, 0]}',*

 * * "'dep_prios'": '{insert: [(3, 5)], delete: [5, 3, 1]}',*

 * * "'dependencies'": "{insert: [(0, 'collections.abc'), (1, 'importlib.abc'), (2, 'types'), (5, "*

 * *                   "'typing')], delete: [7, 6, 3, 2, 1, 0]}",*

 * * "'hash'": "'93eead5bbc091781ea2b4c431442dde9de8d5f668e14b0d2779ed5bd7a1e1914'",*

 * * "'id'": "'importlib'",*

 * * "'interface_hash'": "'b80a4994b195a25dcb726ee5d3ab6f304ddccbc43699e382291f1aeabe66a601'",*

 * * "'mtime'": ' […]*

```diff
@@ -1,44 +1,38 @@
 {
-    "data_mtime": 1683082842,
+    "data_mtime": 1683843440,
     "dep_lines": [
-        5,
-        8,
         1,
+        2,
         3,
         1,
         1,
-        1,
         1
     ],
     "dep_prios": [
         5,
-        25,
         5,
-        10,
         5,
-        30,
+        5,
         30,
         30
     ],
     "dependencies": [
-        "typer.models",
-        "click.shell_completion",
-        "typing",
-        "click",
+        "collections.abc",
+        "importlib.abc",
+        "types",
         "builtins",
         "abc",
-        "click.core",
-        "click.types"
+        "typing"
     ],
-    "hash": "fcf07893bfc8bf4aa53628a147a0b9383364d9146d16d97b31bf5d993a818c4c",
-    "id": "typer.params",
+    "hash": "93eead5bbc091781ea2b4c431442dde9de8d5f668e14b0d2779ed5bd7a1e1914",
+    "id": "importlib",
     "ignore_all": true,
-    "interface_hash": "9f3ba03f753769f82325ea23db014f845f69308f332d7cc50cc11cbecd346913",
-    "mtime": 1683082840,
+    "interface_hash": "b80a4994b195a25dcb726ee5d3ab6f304ddccbc43699e382291f1aeabe66a601",
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -72,13 +66,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib/python3.11/site-packages/typer/params.py",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/importlib/__init__.pyi",
     "plugin_data": null,
-    "size": 13401,
+    "size": 801,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/typer/rich_utils.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/typer/rich_utils.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/typer/rich_utils.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/click/core.meta.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6299836601307189%*

 * *Differences: {"'data_mtime'": '1683843441',*

 * * "'dep_lines'": '{insert: [(0, 7), (1, 16), (2, 17), (3, 23), (4, 25), (5, 27), (6, 30), (7, 33), '*

 * *                '(8, 42), (9, 1839), (10, 1), (11, 2), (17, 8), (18, 10), (19, 12), (20, 14), (21, '*

 * *                '16), (22, 41)], delete: [32, 31, 30, 29, 28, 27, 26, 25, 24, 23, 22, 21, 11, 10, '*

 * *                '9, 8, 7, 6, 0]}',*

 * * "'dep_prios'": '{insert: [(2, 5), (3, 5), (4, 5), (8, 20), (9, 20), (10, 10), (11, 10), (12, 10), '*

 * *                '(13, 10), (14, 10), (16, 20 […]*

```diff
@@ -1,107 +1,116 @@
 {
-    "data_mtime": 1681571164,
+    "data_mtime": 1683843441,
     "dep_lines": [
-        240,
+        7,
+        16,
+        17,
+        23,
+        25,
+        27,
+        30,
+        33,
+        42,
+        1839,
+        1,
+        2,
         3,
         4,
         5,
         6,
         7,
-        9,
-        1,
-        1,
-        1,
-        1,
-        1,
-        1,
+        8,
+        10,
+        12,
+        14,
+        16,
+        41,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
         1,
-        11,
-        12,
-        13,
-        14,
-        15,
-        16,
-        17,
-        18,
-        19,
-        20,
-        21,
-        10
+        1
     ],
     "dep_prios": [
-        20,
         10,
         10,
         5,
         5,
         5,
+        5,
+        5,
+        5,
+        20,
+        20,
+        10,
+        10,
+        10,
         10,
+        10,
+        10,
+        20,
+        5,
+        5,
+        5,
+        5,
+        20,
+        25,
         5,
         30,
         30,
         30,
         30,
         30,
         30,
         30,
-        30,
-        30,
-        30,
-        30,
-        30,
-        30,
-        5,
-        5,
-        5,
-        5,
-        5,
-        5,
-        5,
-        5,
-        5,
-        5,
-        5,
-        5
+        30
     ],
     "dependencies": [
-        "typer.core",
+        "collections.abc",
+        "click.types",
+        "click.exceptions",
+        "click.formatting",
+        "click.globals",
+        "click.parser",
+        "click.termui",
+        "click.utils",
+        "click.shell_completion",
+        "click.decorators",
+        "enum",
+        "errno",
         "inspect",
-        "sys",
-        "collections",
         "os",
+        "sys",
         "typing",
+        "collections",
+        "contextlib",
+        "functools",
+        "gettext",
+        "itertools",
         "click",
+        "typing_extensions",
         "builtins",
         "_collections_abc",
         "_typeshed",
         "abc",
         "array",
-        "click.core",
-        "click.exceptions",
-        "click.shell_completion",
-        "click.types",
         "ctypes",
         "mmap",
         "pickle",
-        "types",
-        "typing_extensions"
+        "types"
     ],
-    "hash": "73518e6d145375bea4e7298a3c057f534091fd529c975c4f775c2376751839c7",
-    "id": "typer.rich_utils",
+    "hash": "9b3f3b6d810acc8a0d6046b9e8114088e267bedd58d0bfa2ef00f8fd979c89e1",
+    "id": "click.core",
     "ignore_all": true,
-    "interface_hash": "2d0be71701ac8ef7a29ed1bfebcebe484ca8756ef35fe0cffeb055e7c22f6b4c",
-    "mtime": 1683082840,
+    "interface_hash": "69e4ba6a6af7fc096a0fe1e35ebd83c7d4ed8cf17d452e3c214023b6d6d16a0b",
+    "mtime": 1684623295,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -135,26 +144,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib/python3.11/site-packages/typer/rich_utils.py",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib/python3.11/site-packages/click/core.py",
     "plugin_data": null,
-    "size": 23654,
-    "suppressed": [
-        "rich.align",
-        "rich.columns",
-        "rich.console",
-        "rich.emoji",
-        "rich.highlighter",
-        "rich.markdown",
-        "rich.padding",
-        "rich.panel",
-        "rich.table",
-        "rich.text",
-        "rich.theme",
-        "rich"
-    ],
-    "version_id": "1.2.0"
+    "size": 112782,
+    "suppressed": [],
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/typer/utils.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/typer/utils.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/typer/utils.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/shutil.meta.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6711764705882353%*

 * *Differences: {"'data_mtime'": '1683843440',*

 * * "'dep_lines'": '{insert: [(0, 4), (5, 6)], delete: [10, 9, 8, 7, 6, 1, 0]}',*

 * * "'dep_prios'": '{insert: [(1, 10)], delete: [11, 10, 9, 8, 7, 0]}',*

 * * "'dependencies'": "{insert: [(0, 'collections.abc'), (1, 'os'), (2, 'sys'), (3, '_typeshed')], "*

 * *                   'delete: [12, 11, 10, 9, 8, 3, 2, 1, 0]}',*

 * * "'hash'": "'14a2bb451d6170f6e211ac293eed7182c2d925a35b3c28b0bb5509c21bf1a000'",*

 * * "'id'": "'shutil'",*

 * * "'interface_hash'": "'c31bb8365bf9434dd242575270735882df910b7c55b39b8e3 […]*

```diff
@@ -1,59 +1,44 @@
 {
-    "data_mtime": 1683082842,
+    "data_mtime": 1683843440,
     "dep_lines": [
-        7,
-        8,
+        4,
         1,
         2,
         3,
         5,
-        1,
-        1,
-        1,
-        1,
-        1,
+        6,
         1,
         1
     ],
     "dep_prios": [
         5,
-        5,
+        10,
         10,
         5,
         5,
         5,
         5,
-        30,
-        30,
-        30,
-        30,
-        30,
         30
     ],
     "dependencies": [
-        "typer._typing",
-        "typer.models",
-        "inspect",
-        "copy",
+        "collections.abc",
+        "os",
+        "sys",
+        "_typeshed",
         "typing",
         "typing_extensions",
         "builtins",
-        "abc",
-        "click",
-        "click.core",
-        "click.shell_completion",
-        "click.types",
-        "types"
+        "abc"
     ],
-    "hash": "2eac497a8186c33e8f50339adabeba874b14695217c4faeef2ad1b8fcee7fd4e",
-    "id": "typer.utils",
+    "hash": "14a2bb451d6170f6e211ac293eed7182c2d925a35b3c28b0bb5509c21bf1a000",
+    "id": "shutil",
     "ignore_all": true,
-    "interface_hash": "da04e072a72c41f7d69e1a60105be13b0fa676d7d978db357cb866c4db5a93ca",
-    "mtime": 1683082840,
+    "interface_hash": "c31bb8365bf9434dd242575270735882df910b7c55b39b8e312be0961ea06831",
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -87,13 +72,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib/python3.11/site-packages/typer/utils.py",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/shutil.pyi",
     "plugin_data": null,
-    "size": 7293,
+    "size": 6658,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/urllib/__init__.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/urllib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/urllib/parse.data.json` & `tomcli-0.1.2/.mypy_cache/3.11/urllib/parse.data.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999997852187643%*

 * *Differences: {"'names'": "{'urlunparse': {'node': {'items': {0: {'func': {'type': {'arg_types': {0: {'.class': "*

 * *            "'Instance', 'args': [OrderedDict([('.class', 'NoneType')])], 'type_ref': "*

 * *            "'typing.Iterable', delete: ['implicit', 'items', 'partial_fallback']}}, 'ret_type': "*

 * *            "{'.class': 'LiteralType', 'fallback': 'builtins.bytes', 'value': '', delete: "*

 * *            "['fullname', 'id', 'name', 'namespace', 'upper_bound', 'values', 'variance']}, "*

 * *            "'variables': []}}}, 1: {'f […]*

```diff
@@ -11913,197 +11913,40 @@
                                     0
                                 ],
                                 "arg_names": [
                                     "components"
                                 ],
                                 "arg_types": [
                                     {
-                                        ".class": "TupleType",
-                                        "implicit": false,
-                                        "items": [
-                                            {
-                                                ".class": "UnionType",
-                                                "items": [
-                                                    {
-                                                        ".class": "TypeVarType",
-                                                        "fullname": "typing.AnyStr",
-                                                        "id": -1,
-                                                        "name": "AnyStr",
-                                                        "namespace": "",
-                                                        "upper_bound": "builtins.object",
-                                                        "values": [
-                                                            "builtins.str",
-                                                            "builtins.bytes"
-                                                        ],
-                                                        "variance": 0
-                                                    },
-                                                    {
-                                                        ".class": "NoneType"
-                                                    }
-                                                ]
-                                            },
-                                            {
-                                                ".class": "UnionType",
-                                                "items": [
-                                                    {
-                                                        ".class": "TypeVarType",
-                                                        "fullname": "typing.AnyStr",
-                                                        "id": -1,
-                                                        "name": "AnyStr",
-                                                        "namespace": "",
-                                                        "upper_bound": "builtins.object",
-                                                        "values": [
-                                                            "builtins.str",
-                                                            "builtins.bytes"
-                                                        ],
-                                                        "variance": 0
-                                                    },
-                                                    {
-                                                        ".class": "NoneType"
-                                                    }
-                                                ]
-                                            },
-                                            {
-                                                ".class": "UnionType",
-                                                "items": [
-                                                    {
-                                                        ".class": "TypeVarType",
-                                                        "fullname": "typing.AnyStr",
-                                                        "id": -1,
-                                                        "name": "AnyStr",
-                                                        "namespace": "",
-                                                        "upper_bound": "builtins.object",
-                                                        "values": [
-                                                            "builtins.str",
-                                                            "builtins.bytes"
-                                                        ],
-                                                        "variance": 0
-                                                    },
-                                                    {
-                                                        ".class": "NoneType"
-                                                    }
-                                                ]
-                                            },
-                                            {
-                                                ".class": "UnionType",
-                                                "items": [
-                                                    {
-                                                        ".class": "TypeVarType",
-                                                        "fullname": "typing.AnyStr",
-                                                        "id": -1,
-                                                        "name": "AnyStr",
-                                                        "namespace": "",
-                                                        "upper_bound": "builtins.object",
-                                                        "values": [
-                                                            "builtins.str",
-                                                            "builtins.bytes"
-                                                        ],
-                                                        "variance": 0
-                                                    },
-                                                    {
-                                                        ".class": "NoneType"
-                                                    }
-                                                ]
-                                            },
-                                            {
-                                                ".class": "UnionType",
-                                                "items": [
-                                                    {
-                                                        ".class": "TypeVarType",
-                                                        "fullname": "typing.AnyStr",
-                                                        "id": -1,
-                                                        "name": "AnyStr",
-                                                        "namespace": "",
-                                                        "upper_bound": "builtins.object",
-                                                        "values": [
-                                                            "builtins.str",
-                                                            "builtins.bytes"
-                                                        ],
-                                                        "variance": 0
-                                                    },
-                                                    {
-                                                        ".class": "NoneType"
-                                                    }
-                                                ]
-                                            },
+                                        ".class": "Instance",
+                                        "args": [
                                             {
-                                                ".class": "UnionType",
-                                                "items": [
-                                                    {
-                                                        ".class": "TypeVarType",
-                                                        "fullname": "typing.AnyStr",
-                                                        "id": -1,
-                                                        "name": "AnyStr",
-                                                        "namespace": "",
-                                                        "upper_bound": "builtins.object",
-                                                        "values": [
-                                                            "builtins.str",
-                                                            "builtins.bytes"
-                                                        ],
-                                                        "variance": 0
-                                                    },
-                                                    {
-                                                        ".class": "NoneType"
-                                                    }
-                                                ]
+                                                ".class": "NoneType"
                                             }
                                         ],
-                                        "partial_fallback": {
-                                            ".class": "Instance",
-                                            "args": [
-                                                {
-                                                    ".class": "AnyType",
-                                                    "missing_import_name": null,
-                                                    "source_any": null,
-                                                    "type_of_any": 6
-                                                }
-                                            ],
-                                            "type_ref": "builtins.tuple"
-                                        }
+                                        "type_ref": "typing.Iterable"
                                     }
                                 ],
                                 "bound_args": [],
                                 "def_extras": {
                                     "first_arg": null
                                 },
                                 "fallback": "builtins.function",
                                 "from_concatenate": false,
                                 "implicit": false,
                                 "is_ellipsis_args": false,
                                 "name": "urlunparse",
                                 "ret_type": {
-                                    ".class": "TypeVarType",
-                                    "fullname": "typing.AnyStr",
-                                    "id": -1,
-                                    "name": "AnyStr",
-                                    "namespace": "",
-                                    "upper_bound": "builtins.object",
-                                    "values": [
-                                        "builtins.str",
-                                        "builtins.bytes"
-                                    ],
-                                    "variance": 0
+                                    ".class": "LiteralType",
+                                    "fallback": "builtins.bytes",
+                                    "value": ""
                                 },
                                 "type_guard": null,
                                 "unpack_kwargs": false,
-                                "variables": [
-                                    {
-                                        ".class": "TypeVarType",
-                                        "fullname": "typing.AnyStr",
-                                        "id": -1,
-                                        "name": "AnyStr",
-                                        "namespace": "",
-                                        "upper_bound": "builtins.object",
-                                        "values": [
-                                            "builtins.str",
-                                            "builtins.bytes"
-                                        ],
-                                        "variance": 0
-                                    }
-                                ]
+                                "variables": []
                             }
                         },
                         "is_overload": true,
                         "var": {
                             ".class": "Var",
                             "flags": [
                                 "is_inferred"
@@ -12161,15 +12004,15 @@
                                                     },
                                                     {
                                                         ".class": "NoneType"
                                                     }
                                                 ]
                                             }
                                         ],
-                                        "type_ref": "typing.Sequence"
+                                        "type_ref": "typing.Iterable"
                                     }
                                 ],
                                 "bound_args": [],
                                 "def_extras": {
                                     "first_arg": null
                                 },
                                 "fallback": "builtins.function",
@@ -12230,197 +12073,40 @@
                                 0
                             ],
                             "arg_names": [
                                 "components"
                             ],
                             "arg_types": [
                                 {
-                                    ".class": "TupleType",
-                                    "implicit": false,
-                                    "items": [
-                                        {
-                                            ".class": "UnionType",
-                                            "items": [
-                                                {
-                                                    ".class": "TypeVarType",
-                                                    "fullname": "typing.AnyStr",
-                                                    "id": -1,
-                                                    "name": "AnyStr",
-                                                    "namespace": "",
-                                                    "upper_bound": "builtins.object",
-                                                    "values": [
-                                                        "builtins.str",
-                                                        "builtins.bytes"
-                                                    ],
-                                                    "variance": 0
-                                                },
-                                                {
-                                                    ".class": "NoneType"
-                                                }
-                                            ]
-                                        },
-                                        {
-                                            ".class": "UnionType",
-                                            "items": [
-                                                {
-                                                    ".class": "TypeVarType",
-                                                    "fullname": "typing.AnyStr",
-                                                    "id": -1,
-                                                    "name": "AnyStr",
-                                                    "namespace": "",
-                                                    "upper_bound": "builtins.object",
-                                                    "values": [
-                                                        "builtins.str",
-                                                        "builtins.bytes"
-                                                    ],
-                                                    "variance": 0
-                                                },
-                                                {
-                                                    ".class": "NoneType"
-                                                }
-                                            ]
-                                        },
-                                        {
-                                            ".class": "UnionType",
-                                            "items": [
-                                                {
-                                                    ".class": "TypeVarType",
-                                                    "fullname": "typing.AnyStr",
-                                                    "id": -1,
-                                                    "name": "AnyStr",
-                                                    "namespace": "",
-                                                    "upper_bound": "builtins.object",
-                                                    "values": [
-                                                        "builtins.str",
-                                                        "builtins.bytes"
-                                                    ],
-                                                    "variance": 0
-                                                },
-                                                {
-                                                    ".class": "NoneType"
-                                                }
-                                            ]
-                                        },
-                                        {
-                                            ".class": "UnionType",
-                                            "items": [
-                                                {
-                                                    ".class": "TypeVarType",
-                                                    "fullname": "typing.AnyStr",
-                                                    "id": -1,
-                                                    "name": "AnyStr",
-                                                    "namespace": "",
-                                                    "upper_bound": "builtins.object",
-                                                    "values": [
-                                                        "builtins.str",
-                                                        "builtins.bytes"
-                                                    ],
-                                                    "variance": 0
-                                                },
-                                                {
-                                                    ".class": "NoneType"
-                                                }
-                                            ]
-                                        },
-                                        {
-                                            ".class": "UnionType",
-                                            "items": [
-                                                {
-                                                    ".class": "TypeVarType",
-                                                    "fullname": "typing.AnyStr",
-                                                    "id": -1,
-                                                    "name": "AnyStr",
-                                                    "namespace": "",
-                                                    "upper_bound": "builtins.object",
-                                                    "values": [
-                                                        "builtins.str",
-                                                        "builtins.bytes"
-                                                    ],
-                                                    "variance": 0
-                                                },
-                                                {
-                                                    ".class": "NoneType"
-                                                }
-                                            ]
-                                        },
+                                    ".class": "Instance",
+                                    "args": [
                                         {
-                                            ".class": "UnionType",
-                                            "items": [
-                                                {
-                                                    ".class": "TypeVarType",
-                                                    "fullname": "typing.AnyStr",
-                                                    "id": -1,
-                                                    "name": "AnyStr",
-                                                    "namespace": "",
-                                                    "upper_bound": "builtins.object",
-                                                    "values": [
-                                                        "builtins.str",
-                                                        "builtins.bytes"
-                                                    ],
-                                                    "variance": 0
-                                                },
-                                                {
-                                                    ".class": "NoneType"
-                                                }
-                                            ]
+                                            ".class": "NoneType"
                                         }
                                     ],
-                                    "partial_fallback": {
-                                        ".class": "Instance",
-                                        "args": [
-                                            {
-                                                ".class": "AnyType",
-                                                "missing_import_name": null,
-                                                "source_any": null,
-                                                "type_of_any": 6
-                                            }
-                                        ],
-                                        "type_ref": "builtins.tuple"
-                                    }
+                                    "type_ref": "typing.Iterable"
                                 }
                             ],
                             "bound_args": [],
                             "def_extras": {
                                 "first_arg": null
                             },
                             "fallback": "builtins.function",
                             "from_concatenate": false,
                             "implicit": false,
                             "is_ellipsis_args": false,
                             "name": "urlunparse",
                             "ret_type": {
-                                ".class": "TypeVarType",
-                                "fullname": "typing.AnyStr",
-                                "id": -1,
-                                "name": "AnyStr",
-                                "namespace": "",
-                                "upper_bound": "builtins.object",
-                                "values": [
-                                    "builtins.str",
-                                    "builtins.bytes"
-                                ],
-                                "variance": 0
+                                ".class": "LiteralType",
+                                "fallback": "builtins.bytes",
+                                "value": ""
                             },
                             "type_guard": null,
                             "unpack_kwargs": false,
-                            "variables": [
-                                {
-                                    ".class": "TypeVarType",
-                                    "fullname": "typing.AnyStr",
-                                    "id": -1,
-                                    "name": "AnyStr",
-                                    "namespace": "",
-                                    "upper_bound": "builtins.object",
-                                    "values": [
-                                        "builtins.str",
-                                        "builtins.bytes"
-                                    ],
-                                    "variance": 0
-                                }
-                            ]
+                            "variables": []
                         },
                         {
                             ".class": "CallableType",
                             "arg_kinds": [
                                 0
                             ],
                             "arg_names": [
@@ -12448,15 +12134,15 @@
                                                 },
                                                 {
                                                     ".class": "NoneType"
                                                 }
                                             ]
                                         }
                                     ],
-                                    "type_ref": "typing.Sequence"
+                                    "type_ref": "typing.Iterable"
                                 }
                             ],
                             "bound_args": [],
                             "def_extras": {
                                 "first_arg": null
                             },
                             "fallback": "builtins.function",
@@ -12532,176 +12218,40 @@
                                     0
                                 ],
                                 "arg_names": [
                                     "components"
                                 ],
                                 "arg_types": [
                                     {
-                                        ".class": "TupleType",
-                                        "implicit": false,
-                                        "items": [
-                                            {
-                                                ".class": "UnionType",
-                                                "items": [
-                                                    {
-                                                        ".class": "TypeVarType",
-                                                        "fullname": "typing.AnyStr",
-                                                        "id": -1,
-                                                        "name": "AnyStr",
-                                                        "namespace": "",
-                                                        "upper_bound": "builtins.object",
-                                                        "values": [
-                                                            "builtins.str",
-                                                            "builtins.bytes"
-                                                        ],
-                                                        "variance": 0
-                                                    },
-                                                    {
-                                                        ".class": "NoneType"
-                                                    }
-                                                ]
-                                            },
-                                            {
-                                                ".class": "UnionType",
-                                                "items": [
-                                                    {
-                                                        ".class": "TypeVarType",
-                                                        "fullname": "typing.AnyStr",
-                                                        "id": -1,
-                                                        "name": "AnyStr",
-                                                        "namespace": "",
-                                                        "upper_bound": "builtins.object",
-                                                        "values": [
-                                                            "builtins.str",
-                                                            "builtins.bytes"
-                                                        ],
-                                                        "variance": 0
-                                                    },
-                                                    {
-                                                        ".class": "NoneType"
-                                                    }
-                                                ]
-                                            },
-                                            {
-                                                ".class": "UnionType",
-                                                "items": [
-                                                    {
-                                                        ".class": "TypeVarType",
-                                                        "fullname": "typing.AnyStr",
-                                                        "id": -1,
-                                                        "name": "AnyStr",
-                                                        "namespace": "",
-                                                        "upper_bound": "builtins.object",
-                                                        "values": [
-                                                            "builtins.str",
-                                                            "builtins.bytes"
-                                                        ],
-                                                        "variance": 0
-                                                    },
-                                                    {
-                                                        ".class": "NoneType"
-                                                    }
-                                                ]
-                                            },
-                                            {
-                                                ".class": "UnionType",
-                                                "items": [
-                                                    {
-                                                        ".class": "TypeVarType",
-                                                        "fullname": "typing.AnyStr",
-                                                        "id": -1,
-                                                        "name": "AnyStr",
-                                                        "namespace": "",
-                                                        "upper_bound": "builtins.object",
-                                                        "values": [
-                                                            "builtins.str",
-                                                            "builtins.bytes"
-                                                        ],
-                                                        "variance": 0
-                                                    },
-                                                    {
-                                                        ".class": "NoneType"
-                                                    }
-                                                ]
-                                            },
+                                        ".class": "Instance",
+                                        "args": [
                                             {
-                                                ".class": "UnionType",
-                                                "items": [
-                                                    {
-                                                        ".class": "TypeVarType",
-                                                        "fullname": "typing.AnyStr",
-                                                        "id": -1,
-                                                        "name": "AnyStr",
-                                                        "namespace": "",
-                                                        "upper_bound": "builtins.object",
-                                                        "values": [
-                                                            "builtins.str",
-                                                            "builtins.bytes"
-                                                        ],
-                                                        "variance": 0
-                                                    },
-                                                    {
-                                                        ".class": "NoneType"
-                                                    }
-                                                ]
+                                                ".class": "NoneType"
                                             }
                                         ],
-                                        "partial_fallback": {
-                                            ".class": "Instance",
-                                            "args": [
-                                                {
-                                                    ".class": "AnyType",
-                                                    "missing_import_name": null,
-                                                    "source_any": null,
-                                                    "type_of_any": 6
-                                                }
-                                            ],
-                                            "type_ref": "builtins.tuple"
-                                        }
+                                        "type_ref": "typing.Iterable"
                                     }
                                 ],
                                 "bound_args": [],
                                 "def_extras": {
                                     "first_arg": null
                                 },
                                 "fallback": "builtins.function",
                                 "from_concatenate": false,
                                 "implicit": false,
                                 "is_ellipsis_args": false,
                                 "name": "urlunsplit",
                                 "ret_type": {
-                                    ".class": "TypeVarType",
-                                    "fullname": "typing.AnyStr",
-                                    "id": -1,
-                                    "name": "AnyStr",
-                                    "namespace": "",
-                                    "upper_bound": "builtins.object",
-                                    "values": [
-                                        "builtins.str",
-                                        "builtins.bytes"
-                                    ],
-                                    "variance": 0
+                                    ".class": "LiteralType",
+                                    "fallback": "builtins.bytes",
+                                    "value": ""
                                 },
                                 "type_guard": null,
                                 "unpack_kwargs": false,
-                                "variables": [
-                                    {
-                                        ".class": "TypeVarType",
-                                        "fullname": "typing.AnyStr",
-                                        "id": -1,
-                                        "name": "AnyStr",
-                                        "namespace": "",
-                                        "upper_bound": "builtins.object",
-                                        "values": [
-                                            "builtins.str",
-                                            "builtins.bytes"
-                                        ],
-                                        "variance": 0
-                                    }
-                                ]
+                                "variables": []
                             }
                         },
                         "is_overload": true,
                         "var": {
                             ".class": "Var",
                             "flags": [
                                 "is_inferred"
@@ -12759,15 +12309,15 @@
                                                     },
                                                     {
                                                         ".class": "NoneType"
                                                     }
                                                 ]
                                             }
                                         ],
-                                        "type_ref": "typing.Sequence"
+                                        "type_ref": "typing.Iterable"
                                     }
                                 ],
                                 "bound_args": [],
                                 "def_extras": {
                                     "first_arg": null
                                 },
                                 "fallback": "builtins.function",
@@ -12828,176 +12378,40 @@
                                 0
                             ],
                             "arg_names": [
                                 "components"
                             ],
                             "arg_types": [
                                 {
-                                    ".class": "TupleType",
-                                    "implicit": false,
-                                    "items": [
-                                        {
-                                            ".class": "UnionType",
-                                            "items": [
-                                                {
-                                                    ".class": "TypeVarType",
-                                                    "fullname": "typing.AnyStr",
-                                                    "id": -1,
-                                                    "name": "AnyStr",
-                                                    "namespace": "",
-                                                    "upper_bound": "builtins.object",
-                                                    "values": [
-                                                        "builtins.str",
-                                                        "builtins.bytes"
-                                                    ],
-                                                    "variance": 0
-                                                },
-                                                {
-                                                    ".class": "NoneType"
-                                                }
-                                            ]
-                                        },
-                                        {
-                                            ".class": "UnionType",
-                                            "items": [
-                                                {
-                                                    ".class": "TypeVarType",
-                                                    "fullname": "typing.AnyStr",
-                                                    "id": -1,
-                                                    "name": "AnyStr",
-                                                    "namespace": "",
-                                                    "upper_bound": "builtins.object",
-                                                    "values": [
-                                                        "builtins.str",
-                                                        "builtins.bytes"
-                                                    ],
-                                                    "variance": 0
-                                                },
-                                                {
-                                                    ".class": "NoneType"
-                                                }
-                                            ]
-                                        },
-                                        {
-                                            ".class": "UnionType",
-                                            "items": [
-                                                {
-                                                    ".class": "TypeVarType",
-                                                    "fullname": "typing.AnyStr",
-                                                    "id": -1,
-                                                    "name": "AnyStr",
-                                                    "namespace": "",
-                                                    "upper_bound": "builtins.object",
-                                                    "values": [
-                                                        "builtins.str",
-                                                        "builtins.bytes"
-                                                    ],
-                                                    "variance": 0
-                                                },
-                                                {
-                                                    ".class": "NoneType"
-                                                }
-                                            ]
-                                        },
-                                        {
-                                            ".class": "UnionType",
-                                            "items": [
-                                                {
-                                                    ".class": "TypeVarType",
-                                                    "fullname": "typing.AnyStr",
-                                                    "id": -1,
-                                                    "name": "AnyStr",
-                                                    "namespace": "",
-                                                    "upper_bound": "builtins.object",
-                                                    "values": [
-                                                        "builtins.str",
-                                                        "builtins.bytes"
-                                                    ],
-                                                    "variance": 0
-                                                },
-                                                {
-                                                    ".class": "NoneType"
-                                                }
-                                            ]
-                                        },
+                                    ".class": "Instance",
+                                    "args": [
                                         {
-                                            ".class": "UnionType",
-                                            "items": [
-                                                {
-                                                    ".class": "TypeVarType",
-                                                    "fullname": "typing.AnyStr",
-                                                    "id": -1,
-                                                    "name": "AnyStr",
-                                                    "namespace": "",
-                                                    "upper_bound": "builtins.object",
-                                                    "values": [
-                                                        "builtins.str",
-                                                        "builtins.bytes"
-                                                    ],
-                                                    "variance": 0
-                                                },
-                                                {
-                                                    ".class": "NoneType"
-                                                }
-                                            ]
+                                            ".class": "NoneType"
                                         }
                                     ],
-                                    "partial_fallback": {
-                                        ".class": "Instance",
-                                        "args": [
-                                            {
-                                                ".class": "AnyType",
-                                                "missing_import_name": null,
-                                                "source_any": null,
-                                                "type_of_any": 6
-                                            }
-                                        ],
-                                        "type_ref": "builtins.tuple"
-                                    }
+                                    "type_ref": "typing.Iterable"
                                 }
                             ],
                             "bound_args": [],
                             "def_extras": {
                                 "first_arg": null
                             },
                             "fallback": "builtins.function",
                             "from_concatenate": false,
                             "implicit": false,
                             "is_ellipsis_args": false,
                             "name": "urlunsplit",
                             "ret_type": {
-                                ".class": "TypeVarType",
-                                "fullname": "typing.AnyStr",
-                                "id": -1,
-                                "name": "AnyStr",
-                                "namespace": "",
-                                "upper_bound": "builtins.object",
-                                "values": [
-                                    "builtins.str",
-                                    "builtins.bytes"
-                                ],
-                                "variance": 0
+                                ".class": "LiteralType",
+                                "fallback": "builtins.bytes",
+                                "value": ""
                             },
                             "type_guard": null,
                             "unpack_kwargs": false,
-                            "variables": [
-                                {
-                                    ".class": "TypeVarType",
-                                    "fullname": "typing.AnyStr",
-                                    "id": -1,
-                                    "name": "AnyStr",
-                                    "namespace": "",
-                                    "upper_bound": "builtins.object",
-                                    "values": [
-                                        "builtins.str",
-                                        "builtins.bytes"
-                                    ],
-                                    "variance": 0
-                                }
-                            ]
+                            "variables": []
                         },
                         {
                             ".class": "CallableType",
                             "arg_kinds": [
                                 0
                             ],
                             "arg_names": [
@@ -13025,15 +12439,15 @@
                                                 },
                                                 {
                                                     ".class": "NoneType"
                                                 }
                                             ]
                                         }
                                     ],
-                                    "type_ref": "typing.Sequence"
+                                    "type_ref": "typing.Iterable"
                                 }
                             ],
                             "bound_args": [],
                             "def_extras": {
                                 "first_arg": null
                             },
                             "fallback": "builtins.function",
```

### Comparing `tomcli-0.1.1/.mypy_cache/3.11/urllib/parse.meta.json` & `tomcli-0.1.2/.mypy_cache/3.11/email/message.meta.json`

 * *Files 17% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.6794871794871795%*

 * *Differences: {"'data_mtime'": '1683843440',*

 * * "'dep_lines'": '{insert: [(3, 5), (4, 6), (5, 2), (7, 8)], delete: [5, 0]}',*

 * * "'dep_prios'": '{insert: [(5, 5), (6, 5), (7, 5), (8, 5)], delete: [6, 1]}',*

 * * "'dependencies'": "{insert: [(1, 'email.charset'), (2, 'email.contentmanager'), (3, "*

 * *                   "'email.errors'), (4, 'email.policy'), (5, 'email')], delete: [6, 4, 1]}",*

 * * "'hash'": "'762e166d09e139961a402ba13a8aaabb0c5cbd010af7cd6f562150d86b3d6f4f'",*

 * * "'id'": "'email.message'",*

 * * "'interface_hash'": "'6d0eb6ed3922 […]*

```diff
@@ -1,44 +1,50 @@
 {
-    "data_mtime": 1681571163,
+    "data_mtime": 1683843440,
     "dep_lines": [
-        2,
         1,
         3,
         4,
+        5,
+        6,
+        2,
         7,
-        1,
+        8,
         1,
         1
     ],
     "dep_prios": [
         5,
-        10,
         5,
         5,
         5,
         5,
-        30,
+        5,
+        5,
+        5,
+        5,
         30
     ],
     "dependencies": [
         "collections.abc",
-        "sys",
+        "email.charset",
+        "email.contentmanager",
+        "email.errors",
+        "email.policy",
+        "email",
         "typing",
         "typing_extensions",
-        "types",
         "builtins",
-        "_typeshed",
         "abc"
     ],
-    "hash": "7cee4f12e177703c3fa882c95efa8800dbcdf149911cffaf1758f0ff8e439bcd",
-    "id": "urllib.parse",
+    "hash": "762e166d09e139961a402ba13a8aaabb0c5cbd010af7cd6f562150d86b3d6f4f",
+    "id": "email.message",
     "ignore_all": true,
-    "interface_hash": "b2d03ae12937bc45055436192bbf91567b3b1e763fc42233449a888eb8f245eb",
-    "mtime": 1683082840,
+    "interface_hash": "6d0eb6ed3922fabc9003d4507ada8810a45a32bd2717f4b802d2f22b62ec64ba",
+    "mtime": 1684623296,
     "options": {
         "allow_redefinition": false,
         "allow_untyped_globals": false,
         "always_false": [],
         "always_true": [],
         "bazel": false,
         "check_untyped_defs": false,
@@ -72,13 +78,13 @@
         "strict_equality": false,
         "strict_optional": true,
         "warn_no_return": true,
         "warn_return_any": false,
         "warn_unreachable": false,
         "warn_unused_ignores": false
     },
-    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/urllib/parse.pyi",
+    "path": "/home/gotmax/Sync/git-repos/packaging/fedora_rpms/dev/tomcli/.nox/typing/lib64/python3.11/site-packages/mypy/typeshed/stdlib/email/message.pyi",
     "plugin_data": null,
-    "size": 6602,
+    "size": 6116,
     "suppressed": [],
-    "version_id": "1.2.0"
+    "version_id": "1.3.0"
 }
```

### Comparing `tomcli-0.1.1/.pytest_cache/v/cache/nodeids` & `tomcli-0.1.2/.pytest_cache/v/cache/nodeids`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9310344827586207%*

 * *Differences: {'insert': "[(54, 'tests/test_tomcli_set.py::test_set_multilevel[tomlkit-tomli_w]'), (55, "*

 * *           "'tests/test_tomcli_set.py::test_set_multilevel[tomlkit-tomlkit]'), (56, "*

 * *           "'tests/test_tomcli_set.py::test_set_multilevel[tomllib-tomli_w]'), (57, "*

 * *           "'tests/test_tomcli_set.py::test_set_multilevel[tomllib-tomlkit]')]"}*

```diff
@@ -48,9 +48,13 @@
     "tests/test_tomcli_set.py::test_set_del[tomlkit-tomli_w]",
     "tests/test_tomcli_set.py::test_set_del[tomlkit-tomlkit]",
     "tests/test_tomcli_set.py::test_set_del[tomllib-tomli_w]",
     "tests/test_tomcli_set.py::test_set_del[tomllib-tomlkit]",
     "tests/test_tomcli_set.py::test_set_del_inplace[tomlkit-tomli_w]",
     "tests/test_tomcli_set.py::test_set_del_inplace[tomlkit-tomlkit]",
     "tests/test_tomcli_set.py::test_set_del_inplace[tomllib-tomli_w]",
-    "tests/test_tomcli_set.py::test_set_del_inplace[tomllib-tomlkit]"
+    "tests/test_tomcli_set.py::test_set_del_inplace[tomllib-tomlkit]",
+    "tests/test_tomcli_set.py::test_set_multilevel[tomlkit-tomli_w]",
+    "tests/test_tomcli_set.py::test_set_multilevel[tomlkit-tomlkit]",
+    "tests/test_tomcli_set.py::test_set_multilevel[tomllib-tomli_w]",
+    "tests/test_tomcli_set.py::test_set_multilevel[tomllib-tomlkit]"
 ]
```

### Comparing `tomcli-0.1.1/.ruff_cache/content/12dc023d4eeb0e37` & `tomcli-0.1.2/.ruff_cache/content/12dc023d4eeb0e37`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.ruff_cache/content/17032b34c3539c33` & `tomcli-0.1.2/.ruff_cache/content/17032b34c3539c33`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.ruff_cache/content/182adab4e5a8e026` & `tomcli-0.1.2/.ruff_cache/content/182adab4e5a8e026`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.ruff_cache/content/191bd3e667e65878` & `tomcli-0.1.2/.ruff_cache/content/191bd3e667e65878`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.ruff_cache/content/195fac077159fecb` & `tomcli-0.1.2/.ruff_cache/content/195fac077159fecb`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.ruff_cache/content/1ed1e9bc14a8e947` & `tomcli-0.1.2/.ruff_cache/content/1ed1e9bc14a8e947`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.ruff_cache/content/242872c45603caf` & `tomcli-0.1.2/.ruff_cache/content/242872c45603caf`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.ruff_cache/content/26fd5f1a8357f894` & `tomcli-0.1.2/.ruff_cache/content/26fd5f1a8357f894`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.ruff_cache/content/2b63439cd5af3054` & `tomcli-0.1.2/.ruff_cache/content/2b63439cd5af3054`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.ruff_cache/content/2ff578dfeee119ca` & `tomcli-0.1.2/.ruff_cache/content/2ff578dfeee119ca`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.ruff_cache/content/343c17d86941be6d` & `tomcli-0.1.2/.ruff_cache/content/343c17d86941be6d`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.ruff_cache/content/41414cb33223f426` & `tomcli-0.1.2/.ruff_cache/content/41414cb33223f426`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.ruff_cache/content/4a7642a70dda40d5` & `tomcli-0.1.2/.ruff_cache/content/4a7642a70dda40d5`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.ruff_cache/content/4dbd6c78c25046fa` & `tomcli-0.1.2/.ruff_cache/content/4dbd6c78c25046fa`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.ruff_cache/content/50fbcc50cbc6963e` & `tomcli-0.1.2/.ruff_cache/content/50fbcc50cbc6963e`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.ruff_cache/content/567b69da99e997a2` & `tomcli-0.1.2/.ruff_cache/content/567b69da99e997a2`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.ruff_cache/content/6786b37a5221b5ca` & `tomcli-0.1.2/.ruff_cache/content/6786b37a5221b5ca`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.ruff_cache/content/68c3bf3fc39850ae` & `tomcli-0.1.2/.ruff_cache/content/68c3bf3fc39850ae`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.ruff_cache/content/6ca2f2fc9012834d` & `tomcli-0.1.2/.ruff_cache/content/6ca2f2fc9012834d`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.ruff_cache/content/6e75d02f45e0b6fb` & `tomcli-0.1.2/.ruff_cache/content/6e75d02f45e0b6fb`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.ruff_cache/content/78d76edde2035610` & `tomcli-0.1.2/.ruff_cache/content/78d76edde2035610`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.ruff_cache/content/7c61d90fd1d2157e` & `tomcli-0.1.2/.ruff_cache/content/7c61d90fd1d2157e`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.ruff_cache/content/7daa321bf9a53c19` & `tomcli-0.1.2/.ruff_cache/content/7daa321bf9a53c19`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.ruff_cache/content/8ee62ebec18533c6` & `tomcli-0.1.2/.ruff_cache/content/8ee62ebec18533c6`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.ruff_cache/content/937b28c1e8bec5db` & `tomcli-0.1.2/.ruff_cache/content/937b28c1e8bec5db`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.ruff_cache/content/99c02b984716f598` & `tomcli-0.1.2/.ruff_cache/content/99c02b984716f598`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.ruff_cache/content/99d43425a9401b4` & `tomcli-0.1.2/.ruff_cache/content/99d43425a9401b4`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.ruff_cache/content/9a95a18da5948a17` & `tomcli-0.1.2/.ruff_cache/content/9a95a18da5948a17`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.ruff_cache/content/9d5dbdd0a8f1e60` & `tomcli-0.1.2/.ruff_cache/content/9d5dbdd0a8f1e60`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.ruff_cache/content/a27d76782310c1d1` & `tomcli-0.1.2/.ruff_cache/content/a27d76782310c1d1`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.ruff_cache/content/a86f2775c1a8a107` & `tomcli-0.1.2/.ruff_cache/content/a86f2775c1a8a107`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.ruff_cache/content/a893c04545a27cb5` & `tomcli-0.1.2/.ruff_cache/content/a893c04545a27cb5`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.ruff_cache/content/ae8098d6ad3ba72c` & `tomcli-0.1.2/.ruff_cache/content/ae8098d6ad3ba72c`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.ruff_cache/content/b3930246cf024275` & `tomcli-0.1.2/.ruff_cache/content/b3930246cf024275`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.ruff_cache/content/bab378b835e02eca` & `tomcli-0.1.2/.ruff_cache/content/bab378b835e02eca`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.ruff_cache/content/cf0c578ec805a96d` & `tomcli-0.1.2/.ruff_cache/content/cf0c578ec805a96d`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.ruff_cache/content/db3b51a62df336a` & `tomcli-0.1.2/.ruff_cache/content/192747c3e751c52b`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.ruff_cache/content/defb66c7533f1af0` & `tomcli-0.1.2/.ruff_cache/content/defb66c7533f1af0`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.ruff_cache/content/ee5eab6a18e8f319` & `tomcli-0.1.2/.ruff_cache/content/ee5eab6a18e8f319`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.ruff_cache/content/f03dc93d3317a16d` & `tomcli-0.1.2/.ruff_cache/content/f03dc93d3317a16d`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.ruff_cache/content/f7743eea7895cd9a` & `tomcli-0.1.2/.ruff_cache/content/f7743eea7895cd9a`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.ruff_cache/content/f91fb7119f181aad` & `tomcli-0.1.2/.ruff_cache/content/f91fb7119f181aad`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/.ruff_cache/content/fcc03fa280ebd898` & `tomcli-0.1.2/.ruff_cache/content/fcc03fa280ebd898`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/contrib/fedoraify.py` & `tomcli-0.1.2/contrib/fedoraify.py`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/htmlcov/coverage_html.js` & `tomcli-0.1.2/htmlcov/coverage_html.js`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/htmlcov/d_0cdc8f8d5ab5d777___init___py.html` & `tomcli-0.1.2/htmlcov/d_0cdc8f8d5ab5d777___init___py.html`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/htmlcov/d_0cdc8f8d5ab5d777_toml_py.html` & `tomcli-0.1.2/htmlcov/d_0cdc8f8d5ab5d777_toml_py.html`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/htmlcov/d_1f8b6c189908f960___init___py.html` & `tomcli-0.1.2/htmlcov/d_1f8b6c189908f960___init___py.html`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/htmlcov/d_1f8b6c189908f960__util_py.html` & `tomcli-0.1.2/htmlcov/d_1f8b6c189908f960__util_py.html`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/htmlcov/d_1f8b6c189908f960_get_py.html` & `tomcli-0.1.2/htmlcov/d_1f8b6c189908f960_get_py.html`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/htmlcov/d_1f8b6c189908f960_set_py.html` & `tomcli-0.1.2/htmlcov/d_1f8b6c189908f960_set_py.html`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/htmlcov/favicon_32.png` & `tomcli-0.1.2/htmlcov/favicon_32.png`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/htmlcov/index.html` & `tomcli-0.1.2/htmlcov/index.html`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/htmlcov/keybd_closed.png` & `tomcli-0.1.2/htmlcov/keybd_closed.png`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/htmlcov/keybd_open.png` & `tomcli-0.1.2/htmlcov/keybd_open.png`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/htmlcov/status.json` & `tomcli-0.1.2/htmlcov/status.json`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/htmlcov/style.css` & `tomcli-0.1.2/htmlcov/style.css`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/src/tomcli/toml.py` & `tomcli-0.1.2/src/tomcli/toml.py`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/src/tomcli/cli/get.py` & `tomcli-0.1.2/src/tomcli/cli/get.py`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/src/tomcli/cli/set.py` & `tomcli-0.1.2/src/tomcli/cli/set.py`

 * *Files 1% similar despite different names*

```diff
@@ -149,15 +149,15 @@
 
 @app.command(name="float")
 def float_(ctx: Context, selector: str = Argument(...), value: float = Argument(...)):
     """
     Set a float value in a TOML file
     """
     fun_msg = (
-        "I'll be very sad if you replace the whole TOML file with a string."
+        "I'll be very sad if you replace the whole TOML file with a float."
         " Computers have feelings too, ya know."
     )
     modder: ModderCtx = ctx.ensure_object(ModderCtx)
     modder.set_default_rw(Reader.TOMLKIT, Writer.TOMLKIT)
     return set_type(
         typ=float,
         default=dict,
@@ -217,15 +217,15 @@
         )
     lst.extend(value)
 
 
 T = TypeVar("T")
 
 
-def set_type(
+def set_type(  # noqa: PLR0913
     *,
     typ: Callable[[Any], T] = lambda x: x,
     callback: Callable[[MutableMapping[str, Any], str, T], Any]
     | Callable[[MutableMapping[str, Any], str], Any] = operator.setitem,
     default: Callable[[], Any] | EllipsisType = ...,
     fun_msg: str | None = "Invalid selector: '.'",
     modder: ModderCtx,
@@ -273,16 +273,15 @@
             parts = ["data"]
     idx = 0
     for idx, part in enumerate(parts):
         if idx + 1 == len(parts):
             break
         if part not in cur and default is not ...:
             cur[part] = default()
-        else:
-            cur = cur[part]
+        cur = cur[part]
     if value is ...:
         callback(cur, part)  # type: ignore[call-arg]
     else:
         callback(cur, part, typ(value))  # type: ignore[call-arg]
     if selector == ".":
         data = data["data"]
     modder.dump(data)
```

### Comparing `tomcli-0.1.1/tests/conftest.py` & `tomcli-0.1.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/tests/test_tomcli_get.py` & `tomcli-0.1.2/tests/test_tomcli_get.py`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/tests/test_tomcli_set.py` & `tomcli-0.1.2/tests/test_tomcli_set.py`

 * *Files 22% similar despite different names*

```diff
@@ -69,7 +69,23 @@
     data.update(expected)
 
     args = [*rwargs, "-o", "-", str(path), typ, "data", "3.14"]
     ran = CliRunner().invoke(app, args, catch_exceptions=False)
     print(ran.stdout)
     assert ran.exit_code == 0
     assert loads(ran.stdout) == data
+
+
+def test_set_multilevel(reader: str, writer: str, tmp_path: Path):
+    path = tmp_path / "pyproject.toml"
+    copy2(TEST_DATA / "pyproject.toml", path)
+    with open(path, "rb") as fp:
+        data = load(fp)
+    # Replace project.license string with dict
+    data["project"]["license"] = {"text": "MIT"}
+
+    for cmd in (("del", "project.license"), ("str", "project.license.text", "MIT")):
+        args = ["--reader", reader, "--writer", writer, str(path), *cmd]
+        ran = CliRunner().invoke(app, args, catch_exceptions=False)
+        assert ran.exit_code == 0
+    with open(path, "rb") as fp:
+        assert data == load(fp)
```

### Comparing `tomcli-0.1.1/tests/test_data/pyproject.toml` & `tomcli-0.1.2/tests/test_data/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/README.md` & `tomcli-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/pyproject.toml` & `tomcli-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/LICENSES/MIT.txt` & `tomcli-0.1.2/LICENSES/MIT.txt`

 * *Files identical despite different names*

### Comparing `tomcli-0.1.1/PKG-INFO` & `tomcli-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tomcli
-Version: 0.1.1
+Version: 0.1.2
 Summary: CLI for working with TOML files. Pronounced "tom clee."
 Project-URL: Source code, https://git.sr.ht/~gotmax23/tomcli
 Project-URL: Mailing list, https://lists.sr.ht/~gotmax23/tomcli
 Author-email: Maxwell G <maxwell@gtmx.me>
 License-Expression: MIT
 License-File: LICENSES/MIT.txt
 Classifier: Development Status :: 3 - Alpha
```

