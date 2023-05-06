# Comparing `tmp/samp_query-0.0.1.tar.gz` & `tmp/samp_query-0.0.2.tar.gz`

## Comparing `samp_query-0.0.1.tar` & `samp_query-0.0.2.tar`

### file list

```diff
@@ -1,162 +1,162 @@
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 samp_query-0.0.1/main.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 samp_query-0.0.1/requirements-test.txt
--rw-r--r--   0        0        0       14 2020-02-02 00:00:00.000000 samp_query-0.0.1/requirements.txt
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 samp_query-0.0.1/setup.cfg
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 samp_query-0.0.1/.github/workflows/ci.yml
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/.gitignore
--rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/@plugins_snapshot.json
--rw-r--r--   0        0        0     8487 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/__future__.data.json
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/__future__.meta.json
--rw-r--r--   0        0        0   193664 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/_ast.data.json
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/_ast.meta.json
--rw-r--r--   0        0        0    57284 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/_codecs.data.json
--rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/_codecs.meta.json
--rw-r--r--   0        0        0    19757 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/_collections_abc.data.json
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/_collections_abc.meta.json
--rw-r--r--   0        0        0     3170 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/_ctypes.data.json
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/_ctypes.meta.json
--rw-r--r--   0        0        0   186597 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/_decimal.data.json
--rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/_decimal.meta.json
--rw-r--r--   0        0        0     6656 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/_random.data.json
--rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/_random.meta.json
--rw-r--r--   0        0        0   148438 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/_socket.data.json
--rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/_socket.meta.json
--rw-r--r--   0        0        0    22352 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/abc.data.json
--rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/abc.meta.json
--rw-r--r--   0        0        0    66369 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/array.data.json
--rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/array.meta.json
--rw-r--r--   0        0        0  1141201 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/builtins.data.json
--rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/builtins.meta.json
--rw-r--r--   0        0        0   134205 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/codecs.data.json
--rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/codecs.meta.json
--rw-r--r--   0        0        0   113663 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/contextlib.data.json
--rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/contextlib.meta.json
--rw-r--r--   0        0        0    41312 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/contextvars.data.json
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/contextvars.meta.json
--rw-r--r--   0        0        0    63243 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/dataclasses.data.json
--rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/dataclasses.meta.json
--rw-r--r--   0        0        0     5291 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/decimal.data.json
--rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/decimal.meta.json
--rw-r--r--   0        0        0    66832 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/enum.data.json
--rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/enum.meta.json
--rw-r--r--   0        0        0    95774 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/fractions.data.json
--rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/fractions.meta.json
--rw-r--r--   0        0        0   131240 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/functools.data.json
--rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/functools.meta.json
--rw-r--r--   0        0        0    24392 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/genericpath.data.json
--rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/genericpath.meta.json
--rw-r--r--   0        0        0    93251 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/io.data.json
--rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/io.meta.json
--rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/main.data.json
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/main.meta.json
--rw-r--r--   0        0        0    31498 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/mmap.data.json
--rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/mmap.meta.json
--rw-r--r--   0        0        0    90192 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/mypy_extensions.data.json
--rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/mypy_extensions.meta.json
--rw-r--r--   0        0        0    86256 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/numbers.data.json
--rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/numbers.meta.json
--rw-r--r--   0        0        0    96566 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/pathlib.data.json
--rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/pathlib.meta.json
--rw-r--r--   0        0        0    48532 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/pickle.data.json
--rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/pickle.meta.json
--rw-r--r--   0        0        0    82100 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/posixpath.data.json
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/posixpath.meta.json
--rw-r--r--   0        0        0    45089 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/random.data.json
--rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/random.meta.json
--rw-r--r--   0        0        0   182913 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/re.data.json
--rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/re.meta.json
--rw-r--r--   0        0        0    23917 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/select.data.json
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/select.meta.json
--rw-r--r--   0        0        0    53813 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/signal.data.json
--rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/signal.meta.json
--rw-r--r--   0        0        0   125399 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/socket.data.json
--rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/socket.meta.json
--rw-r--r--   0        0        0    15195 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/sre_compile.data.json
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/sre_compile.meta.json
--rw-r--r--   0        0        0    30249 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/sre_constants.data.json
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/sre_constants.meta.json
--rw-r--r--   0        0        0    53699 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/sre_parse.data.json
--rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/sre_parse.meta.json
--rw-r--r--   0        0        0   204969 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/ssl.data.json
--rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/ssl.meta.json
--rw-r--r--   0        0        0    16726 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/struct.data.json
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/struct.meta.json
--rw-r--r--   0        0        0   173165 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/subprocess.data.json
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/subprocess.meta.json
--rw-r--r--   0        0        0   152142 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/sys.data.json
--rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/sys.meta.json
--rw-r--r--   0        0        0   248499 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/types.data.json
--rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/types.meta.json
--rw-r--r--   0        0        0   444944 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/typing.data.json
--rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/typing.meta.json
--rw-r--r--   0        0        0    73947 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/typing_extensions.data.json
--rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/typing_extensions.meta.json
--rw-r--r--   0        0        0    96967 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/_typeshed/__init__.data.json
--rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/_typeshed/__init__.meta.json
--rw-r--r--   0        0        0   446258 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/collections/__init__.data.json
--rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/collections/__init__.meta.json
--rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/collections/abc.data.json
--rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/collections/abc.meta.json
--rw-r--r--   0        0        0   140931 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/ctypes/__init__.data.json
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/ctypes/__init__.meta.json
--rw-r--r--   0        0        0     8118 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/email/__init__.data.json
--rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/email/__init__.meta.json
--rw-r--r--   0        0        0    13270 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/email/charset.data.json
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/email/charset.meta.json
--rw-r--r--   0        0        0     7892 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/email/contentmanager.data.json
--rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/email/contentmanager.meta.json
--rw-r--r--   0        0        0    26983 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/email/errors.data.json
--rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/email/errors.meta.json
--rw-r--r--   0        0        0     9984 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/email/header.data.json
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/email/header.meta.json
--rw-r--r--   0        0        0    86486 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/email/message.data.json
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/email/message.meta.json
--rw-r--r--   0        0        0    33569 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/email/policy.data.json
--rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/email/policy.meta.json
--rw-r--r--   0        0        0     6678 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/importlib/__init__.data.json
--rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/importlib/__init__.meta.json
--rw-r--r--   0        0        0    75523 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/importlib/abc.data.json
--rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/importlib/abc.meta.json
--rw-r--r--   0        0        0    69924 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/importlib/machinery.data.json
--rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/importlib/machinery.meta.json
--rw-r--r--   0        0        0    97890 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/importlib/metadata/__init__.data.json
--rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/importlib/metadata/__init__.meta.json
--rw-r--r--   0        0        0    12928 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/importlib/metadata/_meta.data.json
--rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/importlib/metadata/_meta.meta.json
--rw-r--r--   0        0        0   382581 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/os/__init__.data.json
--rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/os/__init__.meta.json
--rw-r--r--   0        0        0     5311 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/os/path.data.json
--rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/os/path.meta.json
--rw-r--r--   0        0        0    26165 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/outcome/__init__.data.json
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/outcome/__init__.meta.json
--rw-r--r--   0        0        0    21048 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/samp_query/__init__.data.json
--rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/samp_query/__init__.meta.json
--rw-r--r--   0        0        0   346581 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/trio/__init__.data.json
--rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/trio/__init__.meta.json
--rw-r--r--   0        0        0    58434 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/trio/abc.data.json
--rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/trio/abc.meta.json
--rw-r--r--   0        0        0    12612 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/trio/from_thread.data.json
--rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/trio/from_thread.meta.json
--rw-r--r--   0        0        0    96361 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/trio/lowlevel.data.json
--rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/trio/lowlevel.meta.json
--rw-r--r--   0        0        0    85329 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/trio/socket.data.json
--rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/trio/socket.meta.json
--rw-r--r--   0        0        0     8748 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/trio/to_thread.data.json
--rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/trio/to_thread.meta.json
--rw-r--r--   0        0        0    38045 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/trio_typing/__init__.data.json
--rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 samp_query-0.0.1/.mypy_cache/3.10/trio_typing/__init__.meta.json
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 samp_query-0.0.1/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 samp_query-0.0.1/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 samp_query-0.0.1/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 samp_query-0.0.1/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 samp_query-0.0.1/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0     3036 2020-02-02 00:00:00.000000 samp_query-0.0.1/samp_query/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 samp_query-0.0.1/test/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 samp_query-0.0.1/test/conftest.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 samp_query-0.0.1/test/test_client.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 samp_query-0.0.1/.gitignore
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 samp_query-0.0.1/LICENSE
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 samp_query-0.0.1/README.md
--rw-r--r--   0        0        0      642 2020-02-02 00:00:00.000000 samp_query-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 samp_query-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 samp_query-0.0.2/main.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 samp_query-0.0.2/requirements-test.txt
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 samp_query-0.0.2/requirements.txt
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 samp_query-0.0.2/setup.cfg
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 samp_query-0.0.2/.github/workflows/ci.yml
+-rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/.gitignore
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/@plugins_snapshot.json
+-rw-r--r--   0        0        0     8487 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/__future__.data.json
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/__future__.meta.json
+-rw-r--r--   0        0        0   193664 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/_ast.data.json
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/_ast.meta.json
+-rw-r--r--   0        0        0    57284 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/_codecs.data.json
+-rw-r--r--   0        0        0     1801 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/_codecs.meta.json
+-rw-r--r--   0        0        0    19757 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/_collections_abc.data.json
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/_collections_abc.meta.json
+-rw-r--r--   0        0        0     3170 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/_ctypes.data.json
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/_ctypes.meta.json
+-rw-r--r--   0        0        0   186597 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/_decimal.data.json
+-rw-r--r--   0        0        0     1756 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/_decimal.meta.json
+-rw-r--r--   0        0        0     6656 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/_random.data.json
+-rw-r--r--   0        0        0     1661 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/_random.meta.json
+-rw-r--r--   0        0        0   148438 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/_socket.data.json
+-rw-r--r--   0        0        0     1785 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/_socket.meta.json
+-rw-r--r--   0        0        0    22352 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/abc.data.json
+-rw-r--r--   0        0        0     1697 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/abc.meta.json
+-rw-r--r--   0        0        0    66369 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/array.data.json
+-rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/array.meta.json
+-rw-r--r--   0        0        0  1141201 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/builtins.data.json
+-rw-r--r--   0        0        0     1861 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/builtins.meta.json
+-rw-r--r--   0        0        0   134205 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/codecs.data.json
+-rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/codecs.meta.json
+-rw-r--r--   0        0        0   113663 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/contextlib.data.json
+-rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/contextlib.meta.json
+-rw-r--r--   0        0        0    41312 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/contextvars.data.json
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/contextvars.meta.json
+-rw-r--r--   0        0        0    63243 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/dataclasses.data.json
+-rw-r--r--   0        0        0     1757 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/dataclasses.meta.json
+-rw-r--r--   0        0        0     5291 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/decimal.data.json
+-rw-r--r--   0        0        0     1652 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/decimal.meta.json
+-rw-r--r--   0        0        0    66832 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/enum.data.json
+-rw-r--r--   0        0        0     1729 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/enum.meta.json
+-rw-r--r--   0        0        0    95774 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/fractions.data.json
+-rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/fractions.meta.json
+-rw-r--r--   0        0        0   131240 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/functools.data.json
+-rw-r--r--   0        0        0     1606 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/functools.meta.json
+-rw-r--r--   0        0        0    24392 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/genericpath.data.json
+-rw-r--r--   0        0        0     1726 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/genericpath.meta.json
+-rw-r--r--   0        0        0    93251 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/io.data.json
+-rw-r--r--   0        0        0     1820 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/io.meta.json
+-rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/main.data.json
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/main.meta.json
+-rw-r--r--   0        0        0    31498 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/mmap.data.json
+-rw-r--r--   0        0        0     1763 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/mmap.meta.json
+-rw-r--r--   0        0        0    90192 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/mypy_extensions.data.json
+-rw-r--r--   0        0        0     1777 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/mypy_extensions.meta.json
+-rw-r--r--   0        0        0    86256 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/numbers.data.json
+-rw-r--r--   0        0        0     1633 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/numbers.meta.json
+-rw-r--r--   0        0        0    96566 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/pathlib.data.json
+-rw-r--r--   0        0        0     1829 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/pathlib.meta.json
+-rw-r--r--   0        0        0    48532 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/pickle.data.json
+-rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/pickle.meta.json
+-rw-r--r--   0        0        0    82100 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/posixpath.data.json
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/posixpath.meta.json
+-rw-r--r--   0        0        0    45089 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/random.data.json
+-rw-r--r--   0        0        0     1745 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/random.meta.json
+-rw-r--r--   0        0        0   182913 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/re.data.json
+-rw-r--r--   0        0        0     1851 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/re.meta.json
+-rw-r--r--   0        0        0    23917 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/select.data.json
+-rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/select.meta.json
+-rw-r--r--   0        0        0    53813 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/signal.data.json
+-rw-r--r--   0        0        0     1746 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/signal.meta.json
+-rw-r--r--   0        0        0   125399 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/socket.data.json
+-rw-r--r--   0        0        0     1838 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/socket.meta.json
+-rw-r--r--   0        0        0    15195 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/sre_compile.data.json
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/sre_compile.meta.json
+-rw-r--r--   0        0        0    30249 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/sre_constants.data.json
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/sre_constants.meta.json
+-rw-r--r--   0        0        0    53699 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/sre_parse.data.json
+-rw-r--r--   0        0        0     1759 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/sre_parse.meta.json
+-rw-r--r--   0        0        0   204969 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/ssl.data.json
+-rw-r--r--   0        0        0     1840 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/ssl.meta.json
+-rw-r--r--   0        0        0    16726 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/struct.data.json
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/struct.meta.json
+-rw-r--r--   0        0        0   173165 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/subprocess.data.json
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/subprocess.meta.json
+-rw-r--r--   0        0        0   152142 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/sys.data.json
+-rw-r--r--   0        0        0     1798 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/sys.meta.json
+-rw-r--r--   0        0        0   248499 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/types.data.json
+-rw-r--r--   0        0        0     1770 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/types.meta.json
+-rw-r--r--   0        0        0   444944 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/typing.data.json
+-rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/typing.meta.json
+-rw-r--r--   0        0        0    73947 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/typing_extensions.data.json
+-rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/typing_extensions.meta.json
+-rw-r--r--   0        0        0    96967 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/_typeshed/__init__.data.json
+-rw-r--r--   0        0        0     1833 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/_typeshed/__init__.meta.json
+-rw-r--r--   0        0        0   446258 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/collections/__init__.data.json
+-rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/collections/__init__.meta.json
+-rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/collections/abc.data.json
+-rw-r--r--   0        0        0     1675 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/collections/abc.meta.json
+-rw-r--r--   0        0        0   140931 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/ctypes/__init__.data.json
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/ctypes/__init__.meta.json
+-rw-r--r--   0        0        0     8118 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/email/__init__.data.json
+-rw-r--r--   0        0        0     1736 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/email/__init__.meta.json
+-rw-r--r--   0        0        0    13270 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/email/charset.data.json
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/email/charset.meta.json
+-rw-r--r--   0        0        0     7892 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/email/contentmanager.data.json
+-rw-r--r--   0        0        0     1707 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/email/contentmanager.meta.json
+-rw-r--r--   0        0        0    26983 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/email/errors.data.json
+-rw-r--r--   0        0        0     1679 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/email/errors.meta.json
+-rw-r--r--   0        0        0     9984 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/email/header.data.json
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/email/header.meta.json
+-rw-r--r--   0        0        0    86486 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/email/message.data.json
+-rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/email/message.meta.json
+-rw-r--r--   0        0        0    33569 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/email/policy.data.json
+-rw-r--r--   0        0        0     1765 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/email/policy.meta.json
+-rw-r--r--   0        0        0     6678 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/importlib/__init__.data.json
+-rw-r--r--   0        0        0     1710 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/importlib/__init__.meta.json
+-rw-r--r--   0        0        0    75523 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/importlib/abc.data.json
+-rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/importlib/abc.meta.json
+-rw-r--r--   0        0        0    69924 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/importlib/machinery.data.json
+-rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/importlib/machinery.meta.json
+-rw-r--r--   0        0        0    97890 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/importlib/metadata/__init__.data.json
+-rw-r--r--   0        0        0     1875 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/importlib/metadata/__init__.meta.json
+-rw-r--r--   0        0        0    12928 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/importlib/metadata/_meta.data.json
+-rw-r--r--   0        0        0     1692 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/importlib/metadata/_meta.meta.json
+-rw-r--r--   0        0        0   382581 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/os/__init__.data.json
+-rw-r--r--   0        0        0     1878 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/os/__init__.meta.json
+-rw-r--r--   0        0        0     5311 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/os/path.data.json
+-rw-r--r--   0        0        0     1667 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/os/path.meta.json
+-rw-r--r--   0        0        0    26165 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/outcome/__init__.data.json
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/outcome/__init__.meta.json
+-rw-r--r--   0        0        0    21048 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/samp_query/__init__.data.json
+-rw-r--r--   0        0        0     1818 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/samp_query/__init__.meta.json
+-rw-r--r--   0        0        0   346581 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/trio/__init__.data.json
+-rw-r--r--   0        0        0     2074 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/trio/__init__.meta.json
+-rw-r--r--   0        0        0    58434 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/trio/abc.data.json
+-rw-r--r--   0        0        0     1681 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/trio/abc.meta.json
+-rw-r--r--   0        0        0    12612 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/trio/from_thread.data.json
+-rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/trio/from_thread.meta.json
+-rw-r--r--   0        0        0    96361 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/trio/lowlevel.data.json
+-rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/trio/lowlevel.meta.json
+-rw-r--r--   0        0        0    85329 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/trio/socket.data.json
+-rw-r--r--   0        0        0     1813 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/trio/socket.meta.json
+-rw-r--r--   0        0        0     8748 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/trio/to_thread.data.json
+-rw-r--r--   0        0        0     1693 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/trio/to_thread.meta.json
+-rw-r--r--   0        0        0    38045 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/trio_typing/__init__.data.json
+-rw-r--r--   0        0        0     1747 2020-02-02 00:00:00.000000 samp_query-0.0.2/.mypy_cache/3.10/trio_typing/__init__.meta.json
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 samp_query-0.0.2/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 samp_query-0.0.2/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 samp_query-0.0.2/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 samp_query-0.0.2/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 samp_query-0.0.2/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0     3036 2020-02-02 00:00:00.000000 samp_query-0.0.2/samp_query/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 samp_query-0.0.2/test/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 samp_query-0.0.2/test/conftest.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 samp_query-0.0.2/test/test_client.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 samp_query-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 samp_query-0.0.2/LICENSE
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 samp_query-0.0.2/README.md
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 samp_query-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      659 2020-02-02 00:00:00.000000 samp_query-0.0.2/PKG-INFO
```

### Comparing `samp_query-0.0.1/.github/workflows/ci.yml` & `samp_query-0.0.2/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/__future__.data.json` & `samp_query-0.0.2/.mypy_cache/3.10/__future__.data.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/__future__.meta.json` & `samp_query-0.0.2/.mypy_cache/3.10/__future__.meta.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/_ast.data.json` & `samp_query-0.0.2/.mypy_cache/3.10/_ast.data.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/_ast.meta.json` & `samp_query-0.0.2/.mypy_cache/3.10/_ast.meta.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/_codecs.data.json` & `samp_query-0.0.2/.mypy_cache/3.10/_codecs.data.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/_codecs.meta.json` & `samp_query-0.0.2/.mypy_cache/3.10/_codecs.meta.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/_collections_abc.data.json` & `samp_query-0.0.2/.mypy_cache/3.10/_collections_abc.data.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/_collections_abc.meta.json` & `samp_query-0.0.2/.mypy_cache/3.10/_collections_abc.meta.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/_ctypes.data.json` & `samp_query-0.0.2/.mypy_cache/3.10/_ctypes.data.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/_ctypes.meta.json` & `samp_query-0.0.2/.mypy_cache/3.10/_ctypes.meta.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/_decimal.data.json` & `samp_query-0.0.2/.mypy_cache/3.10/_decimal.data.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/_decimal.meta.json` & `samp_query-0.0.2/.mypy_cache/3.10/_decimal.meta.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/_random.data.json` & `samp_query-0.0.2/.mypy_cache/3.10/_random.data.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/_random.meta.json` & `samp_query-0.0.2/.mypy_cache/3.10/_random.meta.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/_socket.data.json` & `samp_query-0.0.2/.mypy_cache/3.10/_socket.data.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/_socket.meta.json` & `samp_query-0.0.2/.mypy_cache/3.10/_socket.meta.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/abc.data.json` & `samp_query-0.0.2/.mypy_cache/3.10/abc.data.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/abc.meta.json` & `samp_query-0.0.2/.mypy_cache/3.10/abc.meta.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/array.data.json` & `samp_query-0.0.2/.mypy_cache/3.10/array.data.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/array.meta.json` & `samp_query-0.0.2/.mypy_cache/3.10/array.meta.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/builtins.data.json` & `samp_query-0.0.2/.mypy_cache/3.10/builtins.data.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/builtins.meta.json` & `samp_query-0.0.2/.mypy_cache/3.10/builtins.meta.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/codecs.data.json` & `samp_query-0.0.2/.mypy_cache/3.10/codecs.data.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/codecs.meta.json` & `samp_query-0.0.2/.mypy_cache/3.10/codecs.meta.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/contextlib.data.json` & `samp_query-0.0.2/.mypy_cache/3.10/contextlib.data.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/contextlib.meta.json` & `samp_query-0.0.2/.mypy_cache/3.10/contextlib.meta.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/contextvars.data.json` & `samp_query-0.0.2/.mypy_cache/3.10/contextvars.data.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/contextvars.meta.json` & `samp_query-0.0.2/.mypy_cache/3.10/contextvars.meta.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/dataclasses.data.json` & `samp_query-0.0.2/.mypy_cache/3.10/dataclasses.data.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/dataclasses.meta.json` & `samp_query-0.0.2/.mypy_cache/3.10/dataclasses.meta.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/decimal.data.json` & `samp_query-0.0.2/.mypy_cache/3.10/decimal.data.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/decimal.meta.json` & `samp_query-0.0.2/.mypy_cache/3.10/decimal.meta.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/enum.data.json` & `samp_query-0.0.2/.mypy_cache/3.10/enum.data.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/enum.meta.json` & `samp_query-0.0.2/.mypy_cache/3.10/enum.meta.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/fractions.data.json` & `samp_query-0.0.2/.mypy_cache/3.10/fractions.data.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/fractions.meta.json` & `samp_query-0.0.2/.mypy_cache/3.10/fractions.meta.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/functools.data.json` & `samp_query-0.0.2/.mypy_cache/3.10/functools.data.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/functools.meta.json` & `samp_query-0.0.2/.mypy_cache/3.10/functools.meta.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/genericpath.data.json` & `samp_query-0.0.2/.mypy_cache/3.10/genericpath.data.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/genericpath.meta.json` & `samp_query-0.0.2/.mypy_cache/3.10/genericpath.meta.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/io.data.json` & `samp_query-0.0.2/.mypy_cache/3.10/io.data.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/io.meta.json` & `samp_query-0.0.2/.mypy_cache/3.10/io.meta.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/main.data.json` & `samp_query-0.0.2/.mypy_cache/3.10/main.data.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/main.meta.json` & `samp_query-0.0.2/.mypy_cache/3.10/main.meta.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/mmap.data.json` & `samp_query-0.0.2/.mypy_cache/3.10/mmap.data.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/mmap.meta.json` & `samp_query-0.0.2/.mypy_cache/3.10/mmap.meta.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/mypy_extensions.data.json` & `samp_query-0.0.2/.mypy_cache/3.10/mypy_extensions.data.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/mypy_extensions.meta.json` & `samp_query-0.0.2/.mypy_cache/3.10/mypy_extensions.meta.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/numbers.data.json` & `samp_query-0.0.2/.mypy_cache/3.10/numbers.data.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/numbers.meta.json` & `samp_query-0.0.2/.mypy_cache/3.10/numbers.meta.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/pathlib.data.json` & `samp_query-0.0.2/.mypy_cache/3.10/pathlib.data.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/pathlib.meta.json` & `samp_query-0.0.2/.mypy_cache/3.10/pathlib.meta.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/pickle.data.json` & `samp_query-0.0.2/.mypy_cache/3.10/pickle.data.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/pickle.meta.json` & `samp_query-0.0.2/.mypy_cache/3.10/pickle.meta.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/posixpath.data.json` & `samp_query-0.0.2/.mypy_cache/3.10/posixpath.data.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/posixpath.meta.json` & `samp_query-0.0.2/.mypy_cache/3.10/posixpath.meta.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/random.data.json` & `samp_query-0.0.2/.mypy_cache/3.10/random.data.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/random.meta.json` & `samp_query-0.0.2/.mypy_cache/3.10/random.meta.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/re.data.json` & `samp_query-0.0.2/.mypy_cache/3.10/re.data.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/re.meta.json` & `samp_query-0.0.2/.mypy_cache/3.10/re.meta.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/select.data.json` & `samp_query-0.0.2/.mypy_cache/3.10/select.data.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/select.meta.json` & `samp_query-0.0.2/.mypy_cache/3.10/select.meta.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/signal.data.json` & `samp_query-0.0.2/.mypy_cache/3.10/signal.data.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/signal.meta.json` & `samp_query-0.0.2/.mypy_cache/3.10/signal.meta.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/socket.data.json` & `samp_query-0.0.2/.mypy_cache/3.10/socket.data.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/socket.meta.json` & `samp_query-0.0.2/.mypy_cache/3.10/socket.meta.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/sre_compile.data.json` & `samp_query-0.0.2/.mypy_cache/3.10/sre_compile.data.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/sre_compile.meta.json` & `samp_query-0.0.2/.mypy_cache/3.10/sre_compile.meta.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/sre_constants.data.json` & `samp_query-0.0.2/.mypy_cache/3.10/sre_constants.data.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/sre_constants.meta.json` & `samp_query-0.0.2/.mypy_cache/3.10/sre_constants.meta.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/sre_parse.data.json` & `samp_query-0.0.2/.mypy_cache/3.10/sre_parse.data.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/sre_parse.meta.json` & `samp_query-0.0.2/.mypy_cache/3.10/sre_parse.meta.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/ssl.data.json` & `samp_query-0.0.2/.mypy_cache/3.10/ssl.data.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/ssl.meta.json` & `samp_query-0.0.2/.mypy_cache/3.10/ssl.meta.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/struct.data.json` & `samp_query-0.0.2/.mypy_cache/3.10/struct.data.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/struct.meta.json` & `samp_query-0.0.2/.mypy_cache/3.10/struct.meta.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/subprocess.data.json` & `samp_query-0.0.2/.mypy_cache/3.10/subprocess.data.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/subprocess.meta.json` & `samp_query-0.0.2/.mypy_cache/3.10/subprocess.meta.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/sys.data.json` & `samp_query-0.0.2/.mypy_cache/3.10/sys.data.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/sys.meta.json` & `samp_query-0.0.2/.mypy_cache/3.10/sys.meta.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/types.data.json` & `samp_query-0.0.2/.mypy_cache/3.10/types.data.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/types.meta.json` & `samp_query-0.0.2/.mypy_cache/3.10/types.meta.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/typing.data.json` & `samp_query-0.0.2/.mypy_cache/3.10/typing.data.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/typing.meta.json` & `samp_query-0.0.2/.mypy_cache/3.10/typing.meta.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/typing_extensions.data.json` & `samp_query-0.0.2/.mypy_cache/3.10/typing_extensions.data.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/typing_extensions.meta.json` & `samp_query-0.0.2/.mypy_cache/3.10/typing_extensions.meta.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/_typeshed/__init__.data.json` & `samp_query-0.0.2/.mypy_cache/3.10/_typeshed/__init__.data.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/_typeshed/__init__.meta.json` & `samp_query-0.0.2/.mypy_cache/3.10/_typeshed/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/collections/__init__.data.json` & `samp_query-0.0.2/.mypy_cache/3.10/collections/__init__.data.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/collections/__init__.meta.json` & `samp_query-0.0.2/.mypy_cache/3.10/collections/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/collections/abc.data.json` & `samp_query-0.0.2/.mypy_cache/3.10/collections/abc.data.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/collections/abc.meta.json` & `samp_query-0.0.2/.mypy_cache/3.10/collections/abc.meta.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/ctypes/__init__.data.json` & `samp_query-0.0.2/.mypy_cache/3.10/ctypes/__init__.data.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/ctypes/__init__.meta.json` & `samp_query-0.0.2/.mypy_cache/3.10/ctypes/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/email/__init__.data.json` & `samp_query-0.0.2/.mypy_cache/3.10/email/__init__.data.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/email/__init__.meta.json` & `samp_query-0.0.2/.mypy_cache/3.10/email/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/email/charset.data.json` & `samp_query-0.0.2/.mypy_cache/3.10/email/charset.data.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/email/charset.meta.json` & `samp_query-0.0.2/.mypy_cache/3.10/email/charset.meta.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/email/contentmanager.data.json` & `samp_query-0.0.2/.mypy_cache/3.10/email/contentmanager.data.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/email/contentmanager.meta.json` & `samp_query-0.0.2/.mypy_cache/3.10/email/contentmanager.meta.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/email/errors.data.json` & `samp_query-0.0.2/.mypy_cache/3.10/email/errors.data.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/email/errors.meta.json` & `samp_query-0.0.2/.mypy_cache/3.10/email/errors.meta.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/email/header.data.json` & `samp_query-0.0.2/.mypy_cache/3.10/email/header.data.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/email/header.meta.json` & `samp_query-0.0.2/.mypy_cache/3.10/email/header.meta.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/email/message.data.json` & `samp_query-0.0.2/.mypy_cache/3.10/email/message.data.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/email/message.meta.json` & `samp_query-0.0.2/.mypy_cache/3.10/email/message.meta.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/email/policy.data.json` & `samp_query-0.0.2/.mypy_cache/3.10/email/policy.data.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/email/policy.meta.json` & `samp_query-0.0.2/.mypy_cache/3.10/email/policy.meta.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/importlib/__init__.data.json` & `samp_query-0.0.2/.mypy_cache/3.10/importlib/__init__.data.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/importlib/__init__.meta.json` & `samp_query-0.0.2/.mypy_cache/3.10/importlib/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/importlib/abc.data.json` & `samp_query-0.0.2/.mypy_cache/3.10/importlib/abc.data.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/importlib/abc.meta.json` & `samp_query-0.0.2/.mypy_cache/3.10/importlib/abc.meta.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/importlib/machinery.data.json` & `samp_query-0.0.2/.mypy_cache/3.10/importlib/machinery.data.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/importlib/machinery.meta.json` & `samp_query-0.0.2/.mypy_cache/3.10/importlib/machinery.meta.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/importlib/metadata/__init__.data.json` & `samp_query-0.0.2/.mypy_cache/3.10/importlib/metadata/__init__.data.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/importlib/metadata/__init__.meta.json` & `samp_query-0.0.2/.mypy_cache/3.10/importlib/metadata/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/importlib/metadata/_meta.data.json` & `samp_query-0.0.2/.mypy_cache/3.10/importlib/metadata/_meta.data.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/importlib/metadata/_meta.meta.json` & `samp_query-0.0.2/.mypy_cache/3.10/importlib/metadata/_meta.meta.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/os/__init__.data.json` & `samp_query-0.0.2/.mypy_cache/3.10/os/__init__.data.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/os/__init__.meta.json` & `samp_query-0.0.2/.mypy_cache/3.10/os/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/os/path.data.json` & `samp_query-0.0.2/.mypy_cache/3.10/os/path.data.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/os/path.meta.json` & `samp_query-0.0.2/.mypy_cache/3.10/os/path.meta.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/outcome/__init__.data.json` & `samp_query-0.0.2/.mypy_cache/3.10/outcome/__init__.data.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/outcome/__init__.meta.json` & `samp_query-0.0.2/.mypy_cache/3.10/outcome/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/samp_query/__init__.data.json` & `samp_query-0.0.2/.mypy_cache/3.10/samp_query/__init__.data.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/samp_query/__init__.meta.json` & `samp_query-0.0.2/.mypy_cache/3.10/samp_query/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/trio/__init__.data.json` & `samp_query-0.0.2/.mypy_cache/3.10/trio/__init__.data.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/trio/__init__.meta.json` & `samp_query-0.0.2/.mypy_cache/3.10/trio/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/trio/abc.data.json` & `samp_query-0.0.2/.mypy_cache/3.10/trio/abc.data.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/trio/abc.meta.json` & `samp_query-0.0.2/.mypy_cache/3.10/trio/abc.meta.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/trio/from_thread.data.json` & `samp_query-0.0.2/.mypy_cache/3.10/trio/from_thread.data.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/trio/from_thread.meta.json` & `samp_query-0.0.2/.mypy_cache/3.10/trio/from_thread.meta.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/trio/lowlevel.data.json` & `samp_query-0.0.2/.mypy_cache/3.10/trio/lowlevel.data.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/trio/lowlevel.meta.json` & `samp_query-0.0.2/.mypy_cache/3.10/trio/lowlevel.meta.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/trio/socket.data.json` & `samp_query-0.0.2/.mypy_cache/3.10/trio/socket.data.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/trio/socket.meta.json` & `samp_query-0.0.2/.mypy_cache/3.10/trio/socket.meta.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/trio/to_thread.data.json` & `samp_query-0.0.2/.mypy_cache/3.10/trio/to_thread.data.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/trio/to_thread.meta.json` & `samp_query-0.0.2/.mypy_cache/3.10/trio/to_thread.meta.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/trio_typing/__init__.data.json` & `samp_query-0.0.2/.mypy_cache/3.10/trio_typing/__init__.data.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/.mypy_cache/3.10/trio_typing/__init__.meta.json` & `samp_query-0.0.2/.mypy_cache/3.10/trio_typing/__init__.meta.json`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/samp_query/__init__.py` & `samp_query-0.0.2/samp_query/__init__.py`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/LICENSE` & `samp_query-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `samp_query-0.0.1/pyproject.toml` & `samp_query-0.0.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [project]
 name = "samp_query"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="The Cheaterman", email="the.cheaterman@gmail.com" },
 ]
 description = "A SAMP query/RCON client for Python using trio."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
   "trio",
-  "cchardet",
+  "faust-cchardet",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/Cheaterman/samp-query"
 "Bug Tracker" = "https://github.com/Cheaterman/samp-query/issues"
 
 [build-system]
```

### Comparing `samp_query-0.0.1/PKG-INFO` & `samp_query-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: samp_query
-Version: 0.0.1
+Version: 0.0.2
 Summary: A SAMP query/RCON client for Python using trio.
 Project-URL: Homepage, https://github.com/Cheaterman/samp-query
 Project-URL: Bug Tracker, https://github.com/Cheaterman/samp-query/issues
 Author-email: The Cheaterman <the.cheaterman@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.10
-Requires-Dist: cchardet
+Requires-Dist: faust-cchardet
 Requires-Dist: trio
 Description-Content-Type: text/markdown
 
 samp_query
 ==========
 
 A SAMP query/RCON client for Python using trio.
```

