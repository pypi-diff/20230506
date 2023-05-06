# Comparing `tmp/libvsapm-python-20230430.tar.gz` & `tmp/libvsapm-python-20230506.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libvsapm-python-20230430.tar", last modified: Thu May  4 04:54:14 2023, max compression
+gzip compressed data, was "libvsapm-python-20230506.tar", last modified: Sat May  6 10:54:01 2023, max compression
```

## Comparing `libvsapm-python-20230430.tar` & `libvsapm-python-20230506.tar`

### file list

```diff
@@ -1,706 +1,708 @@
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:54:14.000000 libvsapm-20230430/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2712 2023-05-04 04:31:09.000000 libvsapm-20230430/libvsapm.spec
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:54:13.000000 libvsapm-20230430/libfcache/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2023-05-04 04:30:38.000000 libvsapm-20230430/libfcache/libfcache_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1619 2023-05-04 04:30:38.000000 libvsapm-20230430/libfcache/libfcache_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3806 2023-05-04 04:30:38.000000 libvsapm-20230430/libfcache/libfcache_cache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2023-05-04 04:30:38.000000 libvsapm-20230430/libfcache/libfcache_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1178 2023-05-04 04:30:38.000000 libvsapm-20230430/libfcache/libfcache_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      845 2023-05-04 04:30:38.000000 libvsapm-20230430/libfcache/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2023-05-04 04:30:38.000000 libvsapm-20230430/libfcache/libfcache_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2023-05-04 04:30:38.000000 libvsapm-20230430/libfcache/libfcache_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2023-05-04 04:30:38.000000 libvsapm-20230430/libfcache/libfcache_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1680 2023-05-04 04:30:38.000000 libvsapm-20230430/libfcache/libfcache_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3161 2023-05-04 04:30:38.000000 libvsapm-20230430/libfcache/libfcache_cache_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12461 2023-05-04 04:30:38.000000 libvsapm-20230430/libfcache/libfcache_cache_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29202 2023-05-04 04:30:56.000000 libvsapm-20230430/libfcache/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2023-05-04 04:30:38.000000 libvsapm-20230430/libfcache/libfcache_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2259 2023-05-04 04:30:38.000000 libvsapm-20230430/libfcache/libfcache_date_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26186 2023-05-04 04:30:38.000000 libvsapm-20230430/libfcache/libfcache_cache.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2023-05-04 04:30:38.000000 libvsapm-20230430/libfcache/libfcache_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2023-05-04 04:30:38.000000 libvsapm-20230430/libfcache/libfcache_date_time.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:54:12.000000 libvsapm-20230430/common/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2023-04-30 04:23:08.000000 libvsapm-20230430/common/config_msc.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2023-04-30 04:23:08.000000 libvsapm-20230430/common/byte_stream.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2023-04-30 04:23:08.000000 libvsapm-20230430/common/common.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2023-04-30 04:23:08.000000 libvsapm-20230430/common/system_string.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      378 2023-04-30 04:23:04.000000 libvsapm-20230430/common/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7374 2023-05-04 04:31:09.000000 libvsapm-20230430/common/types.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2023-04-30 04:23:08.000000 libvsapm-20230430/common/types.h.in
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2023-04-30 04:23:08.000000 libvsapm-20230430/common/config_winapi.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2023-04-30 04:23:08.000000 libvsapm-20230430/common/memory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16351 2023-05-04 04:31:09.000000 libvsapm-20230430/common/config.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2023-04-30 04:23:08.000000 libvsapm-20230430/common/narrow_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23773 2023-05-04 04:30:55.000000 libvsapm-20230430/common/Makefile.in
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2023-04-30 04:23:08.000000 libvsapm-20230430/common/file_stream.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      957 2023-04-30 04:23:08.000000 libvsapm-20230430/common/config_borlandc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15432 2023-05-04 04:30:55.000000 libvsapm-20230430/common/config.h.in
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2023-04-30 04:23:08.000000 libvsapm-20230430/common/wide_string.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:54:14.000000 libvsapm-20230430/tests/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1702 2023-04-30 04:23:09.000000 libvsapm-20230430/tests/vsapm_test_memory.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3853 2023-04-30 04:58:04.000000 libvsapm-20230430/tests/test_library.sh
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5004 2023-04-30 04:23:09.000000 libvsapm-20230430/tests/pyvsapm_test_volume.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1462 2023-04-30 04:23:09.000000 libvsapm-20230430/tests/vsapm_test_libcnotify.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1558 2023-04-30 04:23:09.000000 libvsapm-20230430/tests/pyvsapm_test_support.py
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)     3427 2023-04-30 04:23:09.000000 libvsapm-20230430/tests/test_python_module.sh
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      981 2023-04-30 04:23:09.000000 libvsapm-20230430/tests/vsapm_test_libvsapm.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5880 2023-04-30 04:57:52.000000 libvsapm-20230430/tests/Makefile.am
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5634 2023-04-30 04:23:09.000000 libvsapm-20230430/tests/vsapm_test_tools_info_handle.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4535 2023-04-30 04:23:09.000000 libvsapm-20230430/tests/vsapm_test_getopt.c
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)     2168 2023-04-30 04:23:09.000000 libvsapm-20230430/tests/test_vsapminfo.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16671 2023-04-30 04:23:55.000000 libvsapm-20230430/tests/vsapm_test_partition_map_entry.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3139 2023-04-30 04:23:09.000000 libvsapm-20230430/tests/vsapm_test_error.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1813 2023-04-30 04:23:09.000000 libvsapm-20230430/tests/vsapm_test_getopt.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     8056 2023-04-30 04:23:09.000000 libvsapm-20230430/tests/vsapm_test_io_handle.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3802 2023-04-30 04:25:55.000000 libvsapm-20230430/tests/test_tools.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6608 2023-04-30 04:23:55.000000 libvsapm-20230430/tests/vsapm_test_rwlock.c
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)     1653 2023-04-30 04:23:09.000000 libvsapm-20230430/tests/test_manpage.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    60028 2023-04-30 04:23:55.000000 libvsapm-20230430/tests/vsapm_test_partition.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2447 2023-04-30 04:23:09.000000 libvsapm-20230430/tests/vsapm_test_tools_output.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2023-04-30 04:23:09.000000 libvsapm-20230430/tests/vsapm_test_unused.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    37792 2023-04-30 04:23:30.000000 libvsapm-20230430/tests/test_runner.sh
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    13259 2023-04-30 04:23:09.000000 libvsapm-20230430/tests/vsapm_test_functions.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     8574 2023-04-30 04:23:09.000000 libvsapm-20230430/tests/vsapm_test_macros.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4169 2023-04-30 04:23:09.000000 libvsapm-20230430/tests/vsapm_test_tools_signal.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4700 2023-04-30 04:23:09.000000 libvsapm-20230430/tests/vsapm_test_memory.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4323 2023-04-30 04:23:09.000000 libvsapm-20230430/tests/vsapm_test_notify.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1700 2023-04-30 04:23:09.000000 libvsapm-20230430/tests/vsapm_test_rwlock.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1444 2023-04-30 04:23:09.000000 libvsapm-20230430/tests/vsapm_test_libcerror.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1812 2023-04-30 04:23:09.000000 libvsapm-20230430/tests/vsapm_test_functions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    57765 2023-05-04 04:30:56.000000 libvsapm-20230430/tests/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9606 2023-04-30 04:23:55.000000 libvsapm-20230430/tests/vsapm_test_sector_data.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31131 2023-04-30 04:23:55.000000 libvsapm-20230430/tests/vsapm_test_volume.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1742 2023-04-30 04:23:09.000000 libvsapm-20230430/tests/vsapm_test_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9016 2023-04-30 04:23:54.000000 libvsapm-20230430/tests/pyvsapm_test_partition.py
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1709 2023-04-30 04:23:09.000000 libvsapm-20230430/tests/vsapm_test_libbfio.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    14431 2023-04-30 04:23:09.000000 libvsapm-20230430/tests/vsapm_test_support.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1465 2023-04-30 04:23:09.000000 libvsapm-20230430/tests/vsapm_test_libclocale.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:54:12.000000 libvsapm-20230430/libclocale/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2023-05-04 04:30:31.000000 libvsapm-20230430/libclocale/libclocale_wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3094 2023-05-04 04:30:31.000000 libvsapm-20230430/libclocale/libclocale_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1717 2023-05-04 04:30:31.000000 libvsapm-20230430/libclocale/libclocale_locale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      744 2023-05-04 04:30:31.000000 libvsapm-20230430/libclocale/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10671 2023-05-04 04:30:31.000000 libvsapm-20230430/libclocale/libclocale_locale.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2023-05-04 04:30:31.000000 libvsapm-20230430/libclocale/libclocale_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2023-05-04 04:30:31.000000 libvsapm-20230430/libclocale/libclocale_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2023-05-04 04:30:31.000000 libvsapm-20230430/libclocale/libclocale_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3412 2023-05-04 04:30:31.000000 libvsapm-20230430/libclocale/libclocale_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2023-05-04 04:30:31.000000 libvsapm-20230430/libclocale/libclocale_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21033 2023-05-04 04:30:31.000000 libvsapm-20230430/libclocale/libclocale_codepage.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28729 2023-05-04 04:30:56.000000 libvsapm-20230430/libclocale/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1969 2023-05-04 04:30:31.000000 libvsapm-20230430/libclocale/libclocale_wide_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2023-05-04 04:30:31.000000 libvsapm-20230430/libclocale/libclocale_libcerror.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2023-05-04 04:30:55.000000 libvsapm-20230430/missing
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3176 2021-06-10 04:17:04.000000 libvsapm-20230430/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    55932 2023-05-04 04:30:52.000000 libvsapm-20230430/aclocal.m4
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:54:13.000000 libvsapm-20230430/libbfio/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8883 2023-05-04 04:30:25.000000 libvsapm-20230430/libbfio/libbfio_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2023-05-04 04:30:25.000000 libvsapm-20230430/libbfio/libbfio_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    64816 2023-05-04 04:30:25.000000 libvsapm-20230430/libbfio/libbfio_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2023-05-04 04:30:25.000000 libvsapm-20230430/libbfio/libbfio_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2708 2023-05-04 04:30:25.000000 libvsapm-20230430/libbfio/libbfio_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2023-05-04 04:30:25.000000 libvsapm-20230430/libbfio/libbfio_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2023-05-04 04:30:25.000000 libvsapm-20230430/libbfio/libbfio_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2023-05-04 04:30:25.000000 libvsapm-20230430/libbfio/libbfio_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2023-05-04 04:30:25.000000 libvsapm-20230430/libbfio/libbfio_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12186 2023-05-04 04:30:25.000000 libvsapm-20230430/libbfio/libbfio_file_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27543 2023-05-04 04:30:25.000000 libvsapm-20230430/libbfio/libbfio_file_range_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2023-05-04 04:30:25.000000 libvsapm-20230430/libbfio/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10798 2023-05-04 04:30:25.000000 libvsapm-20230430/libbfio/libbfio_file_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10899 2023-05-04 04:30:25.000000 libvsapm-20230430/libbfio/libbfio_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6841 2023-05-04 04:30:25.000000 libvsapm-20230430/libbfio/libbfio_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2630 2023-05-04 04:30:25.000000 libvsapm-20230430/libbfio/libbfio_file_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2814 2023-05-04 04:30:25.000000 libvsapm-20230430/libbfio/libbfio_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4085 2023-05-04 04:30:25.000000 libvsapm-20230430/libbfio/libbfio_file_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21082 2023-05-04 04:30:25.000000 libvsapm-20230430/libbfio/libbfio_memory_range_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2234 2023-05-04 04:30:25.000000 libvsapm-20230430/libbfio/libbfio_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2324 2023-05-04 04:30:25.000000 libvsapm-20230430/libbfio/libbfio_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2077 2023-05-04 04:30:25.000000 libvsapm-20230430/libbfio/libbfio_file_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3835 2023-05-04 04:30:25.000000 libvsapm-20230430/libbfio/libbfio_memory_range_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2023-05-04 04:30:25.000000 libvsapm-20230430/libbfio/libbfio_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1918 2023-05-04 04:30:25.000000 libvsapm-20230430/libbfio/libbfio_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25540 2023-05-04 04:30:25.000000 libvsapm-20230430/libbfio/libbfio_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2023-05-04 04:30:25.000000 libvsapm-20230430/libbfio/libbfio_memory_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4806 2023-05-04 04:30:25.000000 libvsapm-20230430/libbfio/libbfio_file_range_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5821 2023-05-04 04:30:25.000000 libvsapm-20230430/libbfio/libbfio_memory_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32235 2023-05-04 04:30:55.000000 libvsapm-20230430/libbfio/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    81879 2023-05-04 04:30:25.000000 libvsapm-20230430/libbfio/libbfio_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2023-05-04 04:30:25.000000 libvsapm-20230430/libbfio/libbfio_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1362 2023-05-04 04:30:25.000000 libvsapm-20230430/libbfio/libbfio_libcpath.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1420 2023-05-04 04:30:25.000000 libvsapm-20230430/libbfio/libbfio_libcfile.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2023-05-04 04:30:25.000000 libvsapm-20230430/libbfio/libbfio_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26845 2023-05-04 04:30:25.000000 libvsapm-20230430/libbfio/libbfio_file_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2023-05-04 04:30:25.000000 libvsapm-20230430/libbfio/libbfio_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1572 2023-05-04 04:30:25.000000 libvsapm-20230430/libbfio/libbfio_types.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2023-04-30 04:23:04.000000 libvsapm-20230430/COPYING
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      403 2023-04-30 04:24:08.000000 libvsapm-20230430/README
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      660 2023-04-30 04:23:04.000000 libvsapm-20230430/libvsapm.pc.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:54:12.000000 libvsapm-20230430/include/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      494 2023-04-30 04:23:04.000000 libvsapm-20230430/include/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11476 2023-05-04 04:31:09.000000 libvsapm-20230430/include/libvsapm.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11476 2023-04-30 04:23:08.000000 libvsapm-20230430/include/libvsapm.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26774 2023-05-04 04:30:55.000000 libvsapm-20230430/include/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:54:12.000000 libvsapm-20230430/include/libvsapm/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1799 2023-04-30 04:23:08.000000 libvsapm-20230430/include/libvsapm/definitions.h.in
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2023-04-30 04:23:08.000000 libvsapm-20230430/include/libvsapm/extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4852 2023-05-04 04:31:09.000000 libvsapm-20230430/include/libvsapm/types.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2023-04-30 04:23:08.000000 libvsapm-20230430/include/libvsapm/features.h.in
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4983 2023-04-30 04:23:08.000000 libvsapm-20230430/include/libvsapm/types.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1487 2023-05-04 04:31:09.000000 libvsapm-20230430/include/libvsapm/features.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1797 2023-05-04 04:31:09.000000 libvsapm-20230430/include/libvsapm/definitions.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5306 2023-04-30 04:23:08.000000 libvsapm-20230430/include/libvsapm/codepage.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     6758 2023-04-30 04:23:08.000000 libvsapm-20230430/include/libvsapm/error.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2023-05-04 04:30:55.000000 libvsapm-20230430/install-sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2023-05-04 04:30:55.000000 libvsapm-20230430/INSTALL
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:54:11.000000 libvsapm-20230430/dpkg/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      121 2023-04-30 04:23:04.000000 libvsapm-20230430/dpkg/changelog.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      140 2023-05-04 04:31:09.000000 libvsapm-20230430/dpkg/changelog
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1026 2023-04-30 04:23:09.000000 libvsapm-20230430/dpkg/copyright
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       22 2023-04-30 04:23:04.000000 libvsapm-20230430/dpkg/libvsapm.install
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       96 2023-04-30 04:23:04.000000 libvsapm-20230430/dpkg/libvsapm-dev.install
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:54:11.000000 libvsapm-20230430/dpkg/source/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       12 2023-04-30 04:23:04.000000 libvsapm-20230430/dpkg/source/format
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      770 2023-04-30 04:23:04.000000 libvsapm-20230430/dpkg/rules
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        3 2023-04-30 04:23:04.000000 libvsapm-20230430/dpkg/compat
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2194 2023-04-30 04:23:04.000000 libvsapm-20230430/dpkg/control
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:54:13.000000 libvsapm-20230430/pyvsapm-python2/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1646 2023-04-30 04:23:06.000000 libvsapm-20230430/pyvsapm-python2/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41580 2023-05-04 04:30:56.000000 libvsapm-20230430/pyvsapm-python2/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:54:12.000000 libvsapm-20230430/libcfile/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   105597 2023-05-04 04:30:29.000000 libvsapm-20230430/libcfile/libcfile_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2023-05-04 04:30:29.000000 libvsapm-20230430/libcfile/libcfile_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25753 2023-05-04 04:30:29.000000 libvsapm-20230430/libcfile/libcfile_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2389 2023-05-04 04:30:29.000000 libvsapm-20230430/libcfile/libcfile_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2023-05-04 04:30:29.000000 libvsapm-20230430/libcfile/libcfile_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18388 2023-05-04 04:30:29.000000 libvsapm-20230430/libcfile/libcfile_winapi.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      907 2023-05-04 04:30:30.000000 libvsapm-20230430/libcfile/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2023-05-04 04:30:29.000000 libvsapm-20230430/libcfile/libcfile_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2023-05-04 04:30:29.000000 libvsapm-20230430/libcfile/libcfile_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3107 2023-05-04 04:30:29.000000 libvsapm-20230430/libcfile/libcfile_winapi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1497 2023-05-04 04:30:29.000000 libvsapm-20230430/libcfile/libcfile_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2023-05-04 04:30:29.000000 libvsapm-20230430/libcfile/libcfile_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2023-05-04 04:30:29.000000 libvsapm-20230430/libcfile/libcfile_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2879 2023-05-04 04:30:30.000000 libvsapm-20230430/libcfile/libcfile_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6452 2023-05-04 04:30:29.000000 libvsapm-20230430/libcfile/libcfile_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2023-05-04 04:30:29.000000 libvsapm-20230430/libcfile/libcfile_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2023-05-04 04:30:29.000000 libvsapm-20230430/libcfile/libcfile_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29493 2023-05-04 04:30:55.000000 libvsapm-20230430/libcfile/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2023-05-04 04:30:29.000000 libvsapm-20230430/libcfile/libcfile_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2023-05-04 04:30:29.000000 libvsapm-20230430/libcfile/libcfile_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2023-05-04 04:30:29.000000 libvsapm-20230430/libcfile/libcfile_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2023-05-04 04:30:29.000000 libvsapm-20230430/libcfile/libcfile_notify.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3468 2023-04-30 04:23:04.000000 libvsapm-20230430/libvsapm.spec.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:54:12.000000 libvsapm-20230430/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2023-05-04 04:30:36.000000 libvsapm-20230430/libcthreads/libcthreads_thread_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2023-05-04 04:30:36.000000 libvsapm-20230430/libcthreads/libcthreads_thread_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2023-05-04 04:30:36.000000 libvsapm-20230430/libcthreads/libcthreads_repeating_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2023-05-04 04:30:36.000000 libvsapm-20230430/libcthreads/libcthreads_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1136 2023-05-04 04:30:36.000000 libvsapm-20230430/libcthreads/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2023-05-04 04:30:36.000000 libvsapm-20230430/libcthreads/libcthreads_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2023-05-04 04:30:36.000000 libvsapm-20230430/libcthreads/libcthreads_condition.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2023-05-04 04:30:36.000000 libvsapm-20230430/libcthreads/libcthreads_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2023-05-04 04:30:36.000000 libvsapm-20230430/libcthreads/libcthreads_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2023-05-04 04:30:36.000000 libvsapm-20230430/libcthreads/libcthreads_repeating_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2023-05-04 04:30:36.000000 libvsapm-20230430/libcthreads/libcthreads_read_write_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2023-05-04 04:30:36.000000 libvsapm-20230430/libcthreads/libcthreads_mutex.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2023-05-04 04:30:36.000000 libvsapm-20230430/libcthreads/libcthreads_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2023-05-04 04:30:36.000000 libvsapm-20230430/libcthreads/libcthreads_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2023-05-04 04:30:36.000000 libvsapm-20230430/libcthreads/libcthreads_mutex.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2023-05-04 04:30:36.000000 libvsapm-20230430/libcthreads/libcthreads_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2023-05-04 04:30:36.000000 libvsapm-20230430/libcthreads/libcthreads_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2023-05-04 04:30:36.000000 libvsapm-20230430/libcthreads/libcthreads_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2023-05-04 04:30:36.000000 libvsapm-20230430/libcthreads/libcthreads_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2023-05-04 04:30:36.000000 libvsapm-20230430/libcthreads/libcthreads_queue.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2023-05-04 04:30:36.000000 libvsapm-20230430/libcthreads/libcthreads_condition.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31583 2023-05-04 04:30:56.000000 libvsapm-20230430/libcthreads/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2023-05-04 04:30:36.000000 libvsapm-20230430/libcthreads/libcthreads_thread_attributes.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2023-05-04 04:30:36.000000 libvsapm-20230430/libcthreads/libcthreads_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2023-05-04 04:30:36.000000 libvsapm-20230430/libcthreads/libcthreads_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2023-05-04 04:30:36.000000 libvsapm-20230430/libcthreads/libcthreads_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2023-05-04 04:30:36.000000 libvsapm-20230430/libcthreads/libcthreads_read_write_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2023-05-04 04:30:36.000000 libvsapm-20230430/libcthreads/libcthreads_thread_attributes.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2023-05-04 04:30:36.000000 libvsapm-20230430/libcthreads/libcthreads_queue.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       92 2023-04-30 04:23:08.000000 libvsapm-20230430/AUTHORS
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35409 2023-05-04 04:30:55.000000 libvsapm-20230430/config.sub
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:54:13.000000 libvsapm-20230430/libcpath/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2023-05-04 04:30:33.000000 libvsapm-20230430/libcpath/libcpath_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2336 2023-05-04 04:30:33.000000 libvsapm-20230430/libcpath/libcpath_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2023-05-04 04:30:33.000000 libvsapm-20230430/libcpath/libcpath_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      807 2023-05-04 04:30:33.000000 libvsapm-20230430/libcpath/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2023-05-04 04:30:33.000000 libvsapm-20230430/libcpath/libcpath_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2023-05-04 04:30:33.000000 libvsapm-20230430/libcpath/libcpath_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2023-05-04 04:30:33.000000 libvsapm-20230430/libcpath/libcpath_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2023-05-04 04:30:33.000000 libvsapm-20230430/libcpath/libcpath_libcsplit.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7170 2023-05-04 04:30:33.000000 libvsapm-20230430/libcpath/libcpath_path.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28771 2023-05-04 04:30:56.000000 libvsapm-20230430/libcpath/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1990 2023-05-04 04:30:33.000000 libvsapm-20230430/libcpath/libcpath_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2023-05-04 04:30:33.000000 libvsapm-20230430/libcpath/libcpath_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2023-05-04 04:30:33.000000 libvsapm-20230430/libcpath/libcpath_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   176165 2023-05-04 04:30:33.000000 libvsapm-20230430/libcpath/libcpath_path.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2023-05-04 04:30:33.000000 libvsapm-20230430/libcpath/libcpath_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1461 2023-05-04 04:30:33.000000 libvsapm-20230430/libcpath/libcpath_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2023-05-04 04:30:33.000000 libvsapm-20230430/libcpath/libcpath_libuna.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:54:13.000000 libvsapm-20230430/manuals/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      162 2021-05-09 05:40:12.000000 libvsapm-20230430/manuals/Makefile.am
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1777 2023-04-30 04:23:09.000000 libvsapm-20230430/manuals/vsapminfo.1
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25735 2023-05-04 04:30:56.000000 libvsapm-20230430/manuals/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5698 2023-04-30 04:23:09.000000 libvsapm-20230430/manuals/libvsapm.3
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2022-07-15 04:19:38.000000 libvsapm-20230430/ABOUT-NLS
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:54:14.000000 libvsapm-20230430/msvscpp/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:54:14.000000 libvsapm-20230430/msvscpp/vsapm_test_volume/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6497 2023-04-30 04:58:11.000000 libvsapm-20230430/msvscpp/vsapm_test_volume/vsapm_test_volume.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:54:14.000000 libvsapm-20230430/msvscpp/vsapm_test_partition/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6173 2023-04-30 04:58:11.000000 libvsapm-20230430/msvscpp/vsapm_test_partition/vsapm_test_partition.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:54:14.000000 libvsapm-20230430/msvscpp/libfcache/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5237 2023-04-30 04:58:11.000000 libvsapm-20230430/msvscpp/libfcache/libfcache.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:54:14.000000 libvsapm-20230430/msvscpp/vsapm_test_io_handle/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5681 2023-04-30 04:58:11.000000 libvsapm-20230430/msvscpp/vsapm_test_io_handle/vsapm_test_io_handle.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:54:14.000000 libvsapm-20230430/msvscpp/vsapm_test_tools_info_handle/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5782 2023-04-30 04:58:11.000000 libvsapm-20230430/msvscpp/vsapm_test_tools_info_handle/vsapm_test_tools_info_handle.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:54:14.000000 libvsapm-20230430/msvscpp/libclocale/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4778 2023-04-30 04:58:11.000000 libvsapm-20230430/msvscpp/libclocale/libclocale.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1179 2023-04-30 04:58:11.000000 libvsapm-20230430/msvscpp/Makefile.am
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:54:14.000000 libvsapm-20230430/msvscpp/libbfio/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7306 2023-04-30 04:58:11.000000 libvsapm-20230430/msvscpp/libbfio/libbfio.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25042 2023-04-30 04:58:11.000000 libvsapm-20230430/msvscpp/libvsapm.sln
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:54:14.000000 libvsapm-20230430/msvscpp/libcfile/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5597 2023-04-30 04:58:11.000000 libvsapm-20230430/msvscpp/libcfile/libcfile.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:54:14.000000 libvsapm-20230430/msvscpp/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2023-04-30 04:58:11.000000 libvsapm-20230430/msvscpp/libcthreads/libcthreads.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:54:14.000000 libvsapm-20230430/msvscpp/vsapm_test_error/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5423 2023-04-30 04:58:11.000000 libvsapm-20230430/msvscpp/vsapm_test_error/vsapm_test_error.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:54:14.000000 libvsapm-20230430/msvscpp/libcpath/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5183 2023-04-30 04:58:11.000000 libvsapm-20230430/msvscpp/libcpath/libcpath.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:54:14.000000 libvsapm-20230430/msvscpp/vsapm_test_sector_data/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5937 2023-04-30 04:58:11.000000 libvsapm-20230430/msvscpp/vsapm_test_sector_data/vsapm_test_sector_data.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:54:14.000000 libvsapm-20230430/msvscpp/vsapminfo/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6312 2023-04-30 04:58:11.000000 libvsapm-20230430/msvscpp/vsapminfo/vsapminfo.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:54:14.000000 libvsapm-20230430/msvscpp/libuna/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15387 2023-04-30 04:58:11.000000 libvsapm-20230430/msvscpp/libuna/libuna.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21908 2023-05-04 04:30:56.000000 libvsapm-20230430/msvscpp/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:54:14.000000 libvsapm-20230430/msvscpp/libvsapm/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7752 2023-04-30 04:58:11.000000 libvsapm-20230430/msvscpp/libvsapm/libvsapm.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:54:14.000000 libvsapm-20230430/msvscpp/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2023-04-30 04:58:11.000000 libvsapm-20230430/msvscpp/libcerror/libcerror.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:54:14.000000 libvsapm-20230430/msvscpp/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2023-04-30 04:58:11.000000 libvsapm-20230430/msvscpp/libcnotify/libcnotify.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:54:14.000000 libvsapm-20230430/msvscpp/vsapm_test_notify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5510 2023-04-30 04:58:11.000000 libvsapm-20230430/msvscpp/vsapm_test_notify/vsapm_test_notify.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:54:14.000000 libvsapm-20230430/msvscpp/vsapm_test_tools_output/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5617 2023-04-30 04:58:11.000000 libvsapm-20230430/msvscpp/vsapm_test_tools_output/vsapm_test_tools_output.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:54:14.000000 libvsapm-20230430/msvscpp/vsapm_test_support/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6338 2023-04-30 04:58:11.000000 libvsapm-20230430/msvscpp/vsapm_test_support/vsapm_test_support.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:54:14.000000 libvsapm-20230430/msvscpp/libfdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6858 2023-04-30 04:58:11.000000 libvsapm-20230430/msvscpp/libfdata/libfdata.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:54:14.000000 libvsapm-20230430/msvscpp/libcdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6172 2023-04-30 04:58:11.000000 libvsapm-20230430/msvscpp/libcdata/libcdata.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:54:14.000000 libvsapm-20230430/msvscpp/vsapm_test_tools_signal/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5617 2023-04-30 04:58:11.000000 libvsapm-20230430/msvscpp/vsapm_test_tools_signal/vsapm_test_tools_signal.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:54:14.000000 libvsapm-20230430/msvscpp/pyvsapm/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6415 2023-04-30 04:58:11.000000 libvsapm-20230430/msvscpp/pyvsapm/pyvsapm.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:54:14.000000 libvsapm-20230430/msvscpp/libcsplit/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5225 2023-04-30 04:58:11.000000 libvsapm-20230430/msvscpp/libcsplit/libcsplit.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:54:14.000000 libvsapm-20230430/msvscpp/vsapm_test_partition_map_entry/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5961 2023-04-30 04:58:11.000000 libvsapm-20230430/msvscpp/vsapm_test_partition_map_entry/vsapm_test_partition_map_entry.vcproj
--rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)    11497 2023-04-30 04:23:30.000000 libvsapm-20230430/setup.py
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49797 2023-05-04 04:30:55.000000 libvsapm-20230430/config.guess
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        0 2023-04-30 04:23:04.000000 libvsapm-20230430/NEWS
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:54:14.000000 libvsapm-20230430/ossfuzz/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2021-05-09 07:25:01.000000 libvsapm-20230430/ossfuzz/Makefile.am
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2700 2023-04-30 04:23:08.000000 libvsapm-20230430/ossfuzz/partition_fuzzer.cc
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2239 2023-04-30 04:23:08.000000 libvsapm-20230430/ossfuzz/volume_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32986 2023-05-04 04:30:56.000000 libvsapm-20230430/ossfuzz/Makefile.in
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      972 2023-04-30 04:23:08.000000 libvsapm-20230430/ossfuzz/ossfuzz_libvsapm.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2023-04-30 04:23:08.000000 libvsapm-20230430/ossfuzz/ossfuzz_libbfio.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2023-05-04 04:30:56.000000 libvsapm-20230430/test-driver
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)  1617768 2023-05-04 04:30:54.000000 libvsapm-20230430/configure
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:54:12.000000 libvsapm-20230430/libuna/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15532 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_url_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1801 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_mac_symbol.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1259 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_scsu.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2738 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_iso_8859_5.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3610 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_iso_8859_2.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8602 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_windows_1253.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_koi8_u.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7189 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_windows_1252.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19794 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_utf32_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_windows_1257.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9125 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_mac_cyrillic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9435 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_mac_thai.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    95123 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_utf32_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_mac_thai.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8050 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_windows_874.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1628 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_windows_1251.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   484762 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_windows_949.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_iso_8859_6.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_windows_1256.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_mac_greek.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_mac_russian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_mac_ukrainian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2540 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_iso_8859_6.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_windows_874.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8811 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_windows_1251.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10005 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_windows_1256.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2623 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_base16_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_iso_8859_2.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4162 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9076 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_windows_1257.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_windows_1254.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9211 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_windows_1255.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_windows_1253.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5908 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_unicode_character.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_mac_dingbats.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3181 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_scsu.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15485 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_byte_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_mac_celtic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_mac_croatian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_iso_8859_3.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1346 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_iso_8859_15.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9745 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_mac_roman.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_utf32_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9542 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_koi8_r.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_mac_icelandic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_windows_936.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3679 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_base64_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9871 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_mac_celtic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   360710 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_windows_950.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9666 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_utf8_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   430461 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_windows_936.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   129163 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_unicode_character.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   101951 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_utf8_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82226 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_base32_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_windows_950.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_windows_932.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_mac_turkish.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18019 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_utf8_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9088 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_mac_ukrainian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_koi8_r.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39461 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_base16_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_windows_1250.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1783 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_iso_8859_16.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_mac_croatian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10379 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_mac_gaelic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_utf16_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_iso_8859_10.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9394 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_mac_centraleurroman.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   286239 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_windows_932.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2993 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_utf8_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1929 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_url_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11002 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_mac_farsi.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_windows_949.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_mac_romanian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_mac_gaelic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2629 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_iso_8859_8.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10389 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_mac_arabic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1644 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_windows_1252.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_windows_1250.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_mac_russian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    98825 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_utf16_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_iso_8859_5.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_iso_8859_4.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2921 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_mac_roman.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_utf16_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3561 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_iso_8859_4.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3225 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_iso_8859_10.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_mac_icelandic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    52295 2023-05-04 04:30:56.000000 libvsapm-20230430/libuna/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_utf7_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14020 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_mac_symbol.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3704 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_base32_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9844 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_mac_turkish.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10880 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_mac_inuit.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19595 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_utf16_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15691 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_utf7_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_utf32_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3335 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_iso_8859_3.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9078 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_mac_greek.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16696 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_windows_1255.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2823 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_iso_8859_14.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3664 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_iso_8859_13.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_mac_centraleurroman.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_iso_8859_8.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2053 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_iso_8859_9.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_windows_1254.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_mac_cyrillic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_mac_arabic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9116 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_windows_1258.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_mac_farsi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_iso_8859_15.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2873 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_iso_8859_7.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10134 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_mac_dingbats.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1340 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_iso_8859_9.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1630 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_windows_1258.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    74767 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_base64_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9953 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_mac_romanian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9984 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_koi8_u.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1455 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_iso_8859_13.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_iso_8859_7.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_iso_8859_14.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_mac_inuit.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3296 2023-05-04 04:30:42.000000 libvsapm-20230430/libuna/libuna_codepage_iso_8859_16.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40544 2023-05-04 04:30:55.000000 libvsapm-20230430/Makefile.in
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      404 2021-06-11 04:43:51.000000 libvsapm-20230430/ChangeLog
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:54:13.000000 libvsapm-20230430/libvsapm/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2023-04-30 04:23:08.000000 libvsapm-20230430/libvsapm/libvsapm_libcnotify.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2023-04-30 04:23:08.000000 libvsapm-20230430/libvsapm/libvsapm_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1099 2023-05-04 04:31:09.000000 libvsapm-20230430/libvsapm/libvsapm.rc
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     8802 2023-04-30 04:23:08.000000 libvsapm-20230430/libvsapm/libvsapm_sector_data.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2023-04-30 04:23:08.000000 libvsapm-20230430/libvsapm/libvsapm_error.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2822 2023-04-30 04:23:08.000000 libvsapm-20230430/libvsapm/vsapm_partition_map_entry.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2023-04-30 04:23:08.000000 libvsapm-20230430/libvsapm/libvsapm_libclocale.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1897 2023-04-30 04:57:27.000000 libvsapm-20230430/libvsapm/Makefile.am
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1703 2023-04-30 04:23:08.000000 libvsapm-20230430/libvsapm/libvsapm_libbfio.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2179 2023-04-30 04:23:08.000000 libvsapm-20230430/libvsapm/libvsapm_support.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2023-04-30 04:23:08.000000 libvsapm-20230430/libvsapm/libvsapm_libfdata.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    29630 2023-04-30 04:23:08.000000 libvsapm-20230430/libvsapm/libvsapm_partition.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2023-04-30 04:23:08.000000 libvsapm-20230430/libvsapm/libvsapm_notify.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1380 2023-04-30 04:23:08.000000 libvsapm-20230430/libvsapm/libvsapm_debug.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2023-04-30 04:23:08.000000 libvsapm-20230430/libvsapm/libvsapm_unused.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3696 2023-04-30 04:23:08.000000 libvsapm-20230430/libvsapm/libvsapm_io_handle.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2175 2023-04-30 05:02:37.000000 libvsapm-20230430/libvsapm/libvsapm_definitions.h.in
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2023-04-30 04:23:08.000000 libvsapm-20230430/libvsapm/libvsapm_extern.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1101 2023-04-30 04:23:08.000000 libvsapm-20230430/libvsapm/libvsapm.rc.in
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4179 2023-04-30 04:23:08.000000 libvsapm-20230430/libvsapm/libvsapm_debug.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     9852 2023-05-03 04:14:22.000000 libvsapm-20230430/libvsapm/libvsapm_support.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3247 2023-04-30 04:23:08.000000 libvsapm-20230430/libvsapm/libvsapm_partition_map_entry.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2173 2023-05-04 04:31:09.000000 libvsapm-20230430/libvsapm/libvsapm_definitions.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4385 2023-04-30 04:23:08.000000 libvsapm-20230430/libvsapm/libvsapm_partition.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2023-04-30 04:23:08.000000 libvsapm-20230430/libvsapm/libvsapm_libfcache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33074 2023-05-04 04:30:56.000000 libvsapm-20230430/libvsapm/Makefile.in
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2023-04-30 04:23:08.000000 libvsapm-20230430/libvsapm/libvsapm_libcerror.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1682 2023-04-30 04:23:08.000000 libvsapm-20230430/libvsapm/libvsapm_io_handle.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3995 2023-04-30 04:23:08.000000 libvsapm-20230430/libvsapm/libvsapm_volume.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2023-04-30 04:23:08.000000 libvsapm-20230430/libvsapm/libvsapm_notify.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2023-04-30 04:23:08.000000 libvsapm-20230430/libvsapm/libvsapm_error.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1844 2023-04-30 04:23:08.000000 libvsapm-20230430/libvsapm/libvsapm.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1601 2023-04-30 04:23:08.000000 libvsapm-20230430/libvsapm/libvsapm_types.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2023-04-30 04:23:08.000000 libvsapm-20230430/libvsapm/libvsapm_libcdata.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2151 2023-04-30 04:23:08.000000 libvsapm-20230430/libvsapm/libvsapm_sector_data.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    34820 2023-04-30 05:06:51.000000 libvsapm-20230430/libvsapm/libvsapm_volume.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    17794 2023-04-30 04:23:08.000000 libvsapm-20230430/libvsapm/libvsapm_partition_map_entry.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:54:11.000000 libvsapm-20230430/m4/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    23765 2021-09-11 08:08:59.000000 libvsapm-20230430/m4/libuna.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2022-07-15 04:19:38.000000 libvsapm-20230430/m4/gettext.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      756 2021-05-09 05:40:12.000000 libvsapm-20230430/m4/tests.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2022-07-15 04:19:38.000000 libvsapm-20230430/m4/lib-prefix.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2023-05-04 04:30:49.000000 libvsapm-20230430/m4/ltoptions.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     9379 2021-05-09 05:40:12.000000 libvsapm-20230430/m4/libcpath.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2022-07-15 04:19:38.000000 libvsapm-20230430/m4/lib-ld.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11112 2021-05-09 05:40:12.000000 libvsapm-20230430/m4/libcthreads.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2022-07-15 04:19:38.000000 libvsapm-20230430/m4/lib-link.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    17674 2021-12-23 13:41:17.000000 libvsapm-20230430/m4/python.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2023-05-04 04:30:49.000000 libvsapm-20230430/m4/libtool.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2022-07-15 04:19:38.000000 libvsapm-20230430/m4/nls.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     8230 2021-05-09 05:40:12.000000 libvsapm-20230430/m4/libclocale.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    15545 2023-03-20 05:48:50.000000 libvsapm-20230430/m4/libfdata.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2021-05-09 05:08:54.000000 libvsapm-20230430/m4/host-cpu-c-abi.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5638 2021-05-09 05:40:12.000000 libvsapm-20230430/m4/libcnotify.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2023-05-04 04:30:49.000000 libvsapm-20230430/m4/ltversion.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    17147 2023-02-11 06:41:16.000000 libvsapm-20230430/m4/libcdata.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2022-07-15 04:19:38.000000 libvsapm-20230430/m4/progtest.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2023-05-04 04:30:49.000000 libvsapm-20230430/m4/lt~obsolete.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11498 2021-05-09 05:40:12.000000 libvsapm-20230430/m4/libcfile.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2022-07-15 04:19:38.000000 libvsapm-20230430/m4/po.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3852 2021-05-09 05:40:12.000000 libvsapm-20230430/m4/pthread.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    14115 2021-05-09 05:40:12.000000 libvsapm-20230430/m4/common.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     6260 2021-05-09 05:40:12.000000 libvsapm-20230430/m4/libcerror.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2022-07-15 04:19:38.000000 libvsapm-20230430/m4/iconv.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2023-05-04 04:30:49.000000 libvsapm-20230430/m4/ltsugar.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     7325 2023-02-11 06:41:17.000000 libvsapm-20230430/m4/libfcache.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     7384 2021-05-09 05:40:12.000000 libvsapm-20230430/m4/libcsplit.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2022-07-15 04:19:38.000000 libvsapm-20230430/m4/intlmacosx.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2021-05-09 05:40:12.000000 libvsapm-20230430/m4/types.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11692 2021-05-09 05:40:12.000000 libvsapm-20230430/m4/libbfio.m4
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2023-04-30 04:23:04.000000 libvsapm-20230430/COPYING.LESSER
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:54:12.000000 libvsapm-20230430/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2023-05-04 04:30:28.000000 libvsapm-20230430/libcerror/libcerror_system.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2023-05-04 04:30:28.000000 libvsapm-20230430/libcerror/libcerror_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2023-05-04 04:30:28.000000 libvsapm-20230430/libcerror/libcerror_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      605 2023-05-04 04:30:28.000000 libvsapm-20230430/libcerror/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2023-05-04 04:30:28.000000 libvsapm-20230430/libcerror/libcerror_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2023-05-04 04:30:28.000000 libvsapm-20230430/libcerror/libcerror_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2023-05-04 04:30:28.000000 libvsapm-20230430/libcerror/libcerror_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2023-05-04 04:30:28.000000 libvsapm-20230430/libcerror/libcerror_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2023-05-04 04:30:28.000000 libvsapm-20230430/libcerror/libcerror_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28118 2023-05-04 04:30:55.000000 libvsapm-20230430/libcerror/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2023-05-04 04:30:28.000000 libvsapm-20230430/libcerror/libcerror_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2023-05-04 04:30:28.000000 libvsapm-20230430/libcerror/libcerror_system.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:54:13.000000 libvsapm-20230430/pyvsapm-python3/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1646 2023-04-30 04:23:06.000000 libvsapm-20230430/pyvsapm-python3/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41580 2023-05-04 04:30:56.000000 libvsapm-20230430/pyvsapm-python3/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:54:12.000000 libvsapm-20230430/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2023-05-04 04:30:32.000000 libvsapm-20230430/libcnotify/libcnotify_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2023-05-04 04:30:32.000000 libvsapm-20230430/libcnotify/libcnotify_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2023-05-04 04:30:32.000000 libvsapm-20230430/libcnotify/libcnotify_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2023-05-04 04:30:32.000000 libvsapm-20230430/libcnotify/libcnotify_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      693 2023-05-04 04:30:32.000000 libvsapm-20230430/libcnotify/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2023-05-04 04:30:32.000000 libvsapm-20230430/libcnotify/libcnotify_print.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2023-05-04 04:30:32.000000 libvsapm-20230430/libcnotify/libcnotify_verbose.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2023-05-04 04:30:32.000000 libvsapm-20230430/libcnotify/libcnotify_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2023-05-04 04:30:32.000000 libvsapm-20230430/libcnotify/libcnotify_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2023-05-04 04:30:32.000000 libvsapm-20230430/libcnotify/libcnotify_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28605 2023-05-04 04:30:56.000000 libvsapm-20230430/libcnotify/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2023-05-04 04:30:32.000000 libvsapm-20230430/libcnotify/libcnotify_print.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2023-05-04 04:30:32.000000 libvsapm-20230430/libcnotify/libcnotify_verbose.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2023-05-04 04:30:32.000000 libvsapm-20230430/libcnotify/libcnotify_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2023-05-04 04:30:49.000000 libvsapm-20230430/ltmain.sh
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2023-05-04 04:30:55.000000 libvsapm-20230430/compile
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:54:13.000000 libvsapm-20230430/vsapmtools/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17817 2023-04-30 04:23:55.000000 libvsapm-20230430/vsapmtools/info_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6883 2023-05-03 04:13:12.000000 libvsapm-20230430/vsapmtools/vsapminfo.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1748 2023-04-30 04:23:09.000000 libvsapm-20230430/vsapmtools/vsapmtools_libbfio.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1130 2021-05-09 05:40:12.000000 libvsapm-20230430/vsapmtools/Makefile.am
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5707 2023-04-30 04:23:09.000000 libvsapm-20230430/vsapmtools/vsapmtools_signal.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4535 2023-04-30 04:23:09.000000 libvsapm-20230430/vsapmtools/vsapmtools_getopt.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1483 2023-04-30 04:23:09.000000 libvsapm-20230430/vsapmtools/vsapmtools_libcerror.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2023-04-30 04:23:09.000000 libvsapm-20230430/vsapmtools/vsapmtools_unused.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1761 2023-04-30 04:23:09.000000 libvsapm-20230430/vsapmtools/vsapmtools_signal.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1501 2023-04-30 04:23:09.000000 libvsapm-20230430/vsapmtools/vsapmtools_libcnotify.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1781 2023-04-30 04:23:09.000000 libvsapm-20230430/vsapmtools/vsapmtools_libuna.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      981 2023-04-30 04:23:09.000000 libvsapm-20230430/vsapmtools/vsapmtools_libvsapm.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2647 2023-04-30 04:23:55.000000 libvsapm-20230430/vsapmtools/info_handle.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1472 2023-04-30 04:23:09.000000 libvsapm-20230430/vsapmtools/vsapmtools_output.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30141 2023-05-04 04:30:56.000000 libvsapm-20230430/vsapmtools/Makefile.in
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1504 2023-04-30 04:23:09.000000 libvsapm-20230430/vsapmtools/vsapmtools_libclocale.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1213 2023-04-30 04:23:09.000000 libvsapm-20230430/vsapmtools/vsapmtools_i18n.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1813 2023-04-30 04:23:09.000000 libvsapm-20230430/vsapmtools/vsapmtools_getopt.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3451 2023-04-30 04:23:09.000000 libvsapm-20230430/vsapmtools/vsapmtools_output.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2022-07-15 04:19:38.000000 libvsapm-20230430/config.rpath
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2023-05-04 04:30:56.000000 libvsapm-20230430/depcomp
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:54:13.000000 libvsapm-20230430/po/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2022-07-15 04:19:38.000000 libvsapm-20230430/po/en@quot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2022-07-15 04:19:38.000000 libvsapm-20230430/po/Rules-quot
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       59 2021-05-09 05:40:12.000000 libvsapm-20230430/po/POTFILES.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2022-07-15 04:19:38.000000 libvsapm-20230430/po/remove-potcdate.sin
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1808 2021-05-09 05:40:12.000000 libvsapm-20230430/po/Makevars.in
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       50 2021-05-09 05:40:12.000000 libvsapm-20230430/po/ChangeLog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2022-07-15 04:19:38.000000 libvsapm-20230430/po/en@boldquot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2021-05-09 05:09:30.000000 libvsapm-20230430/po/quot.sed
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1810 2023-05-04 04:31:09.000000 libvsapm-20230430/po/Makevars
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2022-07-15 04:19:38.000000 libvsapm-20230430/po/insert-header.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2022-07-15 04:19:38.000000 libvsapm-20230430/po/Makefile.in.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2021-05-09 05:09:30.000000 libvsapm-20230430/po/boldquot.sed
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:54:13.000000 libvsapm-20230430/libfdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2804 2023-05-04 04:30:39.000000 libvsapm-20230430/libfdata/libfdata_segments_array.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2023-05-04 04:30:39.000000 libvsapm-20230430/libfdata/libfdata_cache.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1172 2023-05-04 04:30:39.000000 libvsapm-20230430/libfdata/libfdata_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19329 2023-05-04 04:30:39.000000 libvsapm-20230430/libfdata/libfdata_list_element.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1995 2023-05-04 04:30:39.000000 libvsapm-20230430/libfdata/libfdata_mapped_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2023-05-04 04:30:39.000000 libvsapm-20230430/libfdata/libfdata_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   107689 2023-05-04 04:30:39.000000 libvsapm-20230430/libfdata/libfdata_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2023-05-04 04:30:39.000000 libvsapm-20230430/libfdata/libfdata_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2023-05-04 04:30:39.000000 libvsapm-20230430/libfdata/libfdata_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6013 2023-05-04 04:30:39.000000 libvsapm-20230430/libfdata/libfdata_range_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1256 2023-05-04 04:30:39.000000 libvsapm-20230430/libfdata/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2023-05-04 04:30:39.000000 libvsapm-20230430/libfdata/libfdata_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12090 2023-05-04 04:30:39.000000 libvsapm-20230430/libfdata/libfdata_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7327 2023-05-04 04:30:39.000000 libvsapm-20230430/libfdata/libfdata_area.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2054 2023-05-04 04:30:39.000000 libvsapm-20230430/libfdata/libfdata_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37893 2023-05-04 04:30:39.000000 libvsapm-20230430/libfdata/libfdata_area.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2092 2023-05-04 04:30:39.000000 libvsapm-20230430/libfdata/libfdata_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49670 2023-05-04 04:30:39.000000 libvsapm-20230430/libfdata/libfdata_vector.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9700 2023-05-04 04:30:39.000000 libvsapm-20230430/libfdata/libfdata_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7810 2023-05-04 04:30:39.000000 libvsapm-20230430/libfdata/libfdata_vector.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2023-05-04 04:30:39.000000 libvsapm-20230430/libfdata/libfdata_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2023-05-04 04:30:39.000000 libvsapm-20230430/libfdata/libfdata_libfcache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2023-05-04 04:30:39.000000 libvsapm-20230430/libfdata/libfdata_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30931 2023-05-04 04:30:39.000000 libvsapm-20230430/libfdata/libfdata_range_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2023-05-04 04:30:39.000000 libvsapm-20230430/libfdata/libfdata_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2023-05-04 04:30:39.000000 libvsapm-20230430/libfdata/libfdata_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3999 2023-05-04 04:30:39.000000 libvsapm-20230430/libfdata/libfdata_list_element.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2023-05-04 04:30:39.000000 libvsapm-20230430/libfdata/libfdata_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2023-05-04 04:30:39.000000 libvsapm-20230430/libfdata/libfdata_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31958 2023-05-04 04:30:56.000000 libvsapm-20230430/libfdata/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1491 2023-05-04 04:30:39.000000 libvsapm-20230430/libfdata/libfdata_cache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    66203 2023-05-04 04:30:39.000000 libvsapm-20230430/libfdata/libfdata_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21271 2023-05-04 04:30:39.000000 libvsapm-20230430/libfdata/libfdata_segments_array.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6826 2023-05-04 04:30:39.000000 libvsapm-20230430/libfdata/libfdata_mapped_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6533 2023-05-04 04:30:39.000000 libvsapm-20230430/libfdata/libfdata_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7149 2023-05-04 04:30:39.000000 libvsapm-20230430/libfdata/libfdata_range.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:54:12.000000 libvsapm-20230430/libcdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49968 2023-05-04 04:30:26.000000 libvsapm-20230430/libcdata/libcdata_array.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37549 2023-05-04 04:30:26.000000 libvsapm-20230430/libcdata/libcdata_btree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100501 2023-05-04 04:30:26.000000 libvsapm-20230430/libcdata/libcdata_tree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2023-05-04 04:30:26.000000 libvsapm-20230430/libcdata/libcdata_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2789 2023-05-04 04:30:26.000000 libvsapm-20230430/libcdata/libcdata_range_list_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2023-05-04 04:30:26.000000 libvsapm-20230430/libcdata/libcdata_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12295 2023-05-04 04:30:26.000000 libvsapm-20230430/libcdata/libcdata_range_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1092 2023-05-04 04:30:26.000000 libvsapm-20230430/libcdata/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   122285 2023-05-04 04:30:26.000000 libvsapm-20230430/libcdata/libcdata_range_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2023-05-04 04:30:26.000000 libvsapm-20230430/libcdata/libcdata_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2023-05-04 04:30:26.000000 libvsapm-20230430/libcdata/libcdata_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3871 2023-05-04 04:30:26.000000 libvsapm-20230430/libcdata/libcdata_list_element.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5251 2023-05-04 04:30:26.000000 libvsapm-20230430/libcdata/libcdata_btree_values_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10647 2023-05-04 04:30:26.000000 libvsapm-20230430/libcdata/libcdata_range_list_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2023-05-04 04:30:26.000000 libvsapm-20230430/libcdata/libcdata_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2023-05-04 04:30:26.000000 libvsapm-20230430/libcdata/libcdata_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2023-05-04 04:30:26.000000 libvsapm-20230430/libcdata/libcdata_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2023-05-04 04:30:26.000000 libvsapm-20230430/libcdata/libcdata_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2960 2023-05-04 04:30:26.000000 libvsapm-20230430/libcdata/libcdata_btree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69515 2023-05-04 04:30:26.000000 libvsapm-20230430/libcdata/libcdata_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8365 2023-05-04 04:30:26.000000 libvsapm-20230430/libcdata/libcdata_tree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6448 2023-05-04 04:30:26.000000 libvsapm-20230430/libcdata/libcdata_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2023-05-04 04:30:26.000000 libvsapm-20230430/libcdata/libcdata_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23846 2023-05-04 04:30:26.000000 libvsapm-20230430/libcdata/libcdata_list_element.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31177 2023-05-04 04:30:55.000000 libvsapm-20230430/libcdata/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2023-05-04 04:30:26.000000 libvsapm-20230430/libcdata/libcdata_btree_values_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5231 2023-05-04 04:30:26.000000 libvsapm-20230430/libcdata/libcdata_array.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3790 2023-05-04 04:30:26.000000 libvsapm-20230430/libcdata/libcdata_btree.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2023-05-04 04:30:26.000000 libvsapm-20230430/libcdata/libcdata_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22358 2023-05-04 04:30:26.000000 libvsapm-20230430/libcdata/libcdata_btree.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:54:13.000000 libvsapm-20230430/pyvsapm/
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1544 2023-04-30 04:23:08.000000 libvsapm-20230430/pyvsapm/pyvsapm_integer.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2023-04-30 04:23:08.000000 libvsapm-20230430/pyvsapm/pyvsapm_unused.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2023-04-30 04:23:08.000000 libvsapm-20230430/pyvsapm/pyvsapm_libcerror.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4118 2023-04-30 04:23:08.000000 libvsapm-20230430/pyvsapm/pyvsapm_file_object_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25879 2023-04-30 04:23:54.000000 libvsapm-20230430/pyvsapm/pyvsapm_partition.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2033 2023-04-30 04:23:08.000000 libvsapm-20230430/pyvsapm/pyvsapm_python.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     8876 2023-04-30 04:23:08.000000 libvsapm-20230430/pyvsapm/pyvsapm_integer.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1172 2021-06-10 04:17:11.000000 libvsapm-20230430/pyvsapm/Makefile.am
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      973 2023-04-30 04:23:08.000000 libvsapm-20230430/pyvsapm/pyvsapm_libvsapm.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3031 2023-04-30 04:23:08.000000 libvsapm-20230430/pyvsapm/pyvsapm_partition.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1868 2023-04-30 04:23:08.000000 libvsapm-20230430/pyvsapm/pyvsapm.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1525 2023-04-30 04:23:08.000000 libvsapm-20230430/pyvsapm/pyvsapm_libbfio.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    14846 2023-04-30 04:23:08.000000 libvsapm-20230430/pyvsapm/pyvsapm.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2445 2023-04-30 04:23:08.000000 libvsapm-20230430/pyvsapm/pyvsapm_partitions.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2023-04-30 04:23:08.000000 libvsapm-20230430/pyvsapm/pyvsapm_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2825 2023-04-30 04:23:54.000000 libvsapm-20230430/pyvsapm/pyvsapm_volume.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     9546 2023-04-30 04:23:08.000000 libvsapm-20230430/pyvsapm/pyvsapm_error.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1540 2023-04-30 04:23:08.000000 libvsapm-20230430/pyvsapm/pyvsapm_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41205 2023-05-04 04:30:56.000000 libvsapm-20230430/pyvsapm/Makefile.in
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    33875 2023-04-30 04:23:08.000000 libvsapm-20230430/pyvsapm/pyvsapm_file_object_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22133 2023-04-30 04:23:54.000000 libvsapm-20230430/pyvsapm/pyvsapm_volume.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     9329 2023-04-30 04:23:08.000000 libvsapm-20230430/pyvsapm/pyvsapm_partitions.c
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1208 2023-04-30 04:23:04.000000 libvsapm-20230430/acinclude.m4
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:54:12.000000 libvsapm-20230430/libcsplit/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1679 2023-05-04 04:30:35.000000 libvsapm-20230430/libcsplit/libcsplit_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1471 2023-05-04 04:30:35.000000 libvsapm-20230430/libcsplit/libcsplit_wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2023-05-04 04:30:35.000000 libvsapm-20230430/libcsplit/libcsplit_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2023-05-04 04:30:35.000000 libvsapm-20230430/libcsplit/libcsplit_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13912 2023-05-04 04:30:35.000000 libvsapm-20230430/libcsplit/libcsplit_narrow_split_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2849 2023-05-04 04:30:35.000000 libvsapm-20230430/libcsplit/libcsplit_narrow_split_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      849 2023-05-04 04:30:35.000000 libvsapm-20230430/libcsplit/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13944 2023-05-04 04:30:35.000000 libvsapm-20230430/libcsplit/libcsplit_wide_split_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1386 2023-05-04 04:30:35.000000 libvsapm-20230430/libcsplit/libcsplit_narrow_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2023-05-04 04:30:35.000000 libvsapm-20230430/libcsplit/libcsplit_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6206 2023-05-04 04:30:35.000000 libvsapm-20230430/libcsplit/libcsplit_wide_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6125 2023-05-04 04:30:35.000000 libvsapm-20230430/libcsplit/libcsplit_narrow_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29551 2023-05-04 04:30:56.000000 libvsapm-20230430/libcsplit/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2920 2023-05-04 04:30:35.000000 libvsapm-20230430/libcsplit/libcsplit_wide_split_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1360 2023-05-04 04:30:35.000000 libvsapm-20230430/libcsplit/libcsplit_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2023-05-04 04:30:35.000000 libvsapm-20230430/libcsplit/libcsplit_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2023-05-04 04:30:35.000000 libvsapm-20230430/libcsplit/libcsplit_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2023-05-04 04:30:35.000000 libvsapm-20230430/libcsplit/libcsplit_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2023-05-04 04:30:35.000000 libvsapm-20230430/libcsplit/libcsplit_extern.h
--rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     7083 2023-04-30 04:23:04.000000 libvsapm-20230430/configure.ac
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      351 2023-05-04 04:54:14.858953 libvsapm-20230430/PKG-INFO
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 10:54:00.000000 libvsapm-20230506/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2712 2023-05-06 10:39:22.000000 libvsapm-20230506/libvsapm.spec
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 10:53:59.000000 libvsapm-20230506/libfcache/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2023-05-06 10:38:57.000000 libvsapm-20230506/libfcache/libfcache_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1619 2023-05-06 10:38:57.000000 libvsapm-20230506/libfcache/libfcache_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3806 2023-05-06 10:38:57.000000 libvsapm-20230506/libfcache/libfcache_cache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2023-05-06 10:38:57.000000 libvsapm-20230506/libfcache/libfcache_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1178 2023-05-06 10:38:57.000000 libvsapm-20230506/libfcache/libfcache_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      845 2023-05-06 10:38:57.000000 libvsapm-20230506/libfcache/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2023-05-06 10:38:57.000000 libvsapm-20230506/libfcache/libfcache_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2023-05-06 10:38:57.000000 libvsapm-20230506/libfcache/libfcache_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2023-05-06 10:38:57.000000 libvsapm-20230506/libfcache/libfcache_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1680 2023-05-06 10:38:57.000000 libvsapm-20230506/libfcache/libfcache_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3161 2023-05-06 10:38:57.000000 libvsapm-20230506/libfcache/libfcache_cache_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12461 2023-05-06 10:38:57.000000 libvsapm-20230506/libfcache/libfcache_cache_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29202 2023-05-06 10:39:12.000000 libvsapm-20230506/libfcache/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2023-05-06 10:38:57.000000 libvsapm-20230506/libfcache/libfcache_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2259 2023-05-06 10:38:57.000000 libvsapm-20230506/libfcache/libfcache_date_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26186 2023-05-06 10:38:57.000000 libvsapm-20230506/libfcache/libfcache_cache.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2023-05-06 10:38:57.000000 libvsapm-20230506/libfcache/libfcache_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2023-05-06 10:38:57.000000 libvsapm-20230506/libfcache/libfcache_date_time.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 10:53:57.000000 libvsapm-20230506/common/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1157 2023-05-06 09:06:27.000000 libvsapm-20230506/common/config_msc.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    10437 2023-05-06 09:06:27.000000 libvsapm-20230506/common/byte_stream.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2023-05-06 09:06:27.000000 libvsapm-20230506/common/common.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4611 2023-05-06 09:06:27.000000 libvsapm-20230506/common/system_string.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      378 2023-05-06 09:06:25.000000 libvsapm-20230506/common/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7374 2023-05-06 10:39:22.000000 libvsapm-20230506/common/types.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     7375 2023-05-06 09:06:27.000000 libvsapm-20230506/common/types.h.in
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2382 2023-05-06 09:06:27.000000 libvsapm-20230506/common/config_winapi.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3259 2023-05-06 09:06:27.000000 libvsapm-20230506/common/memory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16351 2023-05-06 10:39:22.000000 libvsapm-20230506/common/config.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5419 2023-05-06 09:06:27.000000 libvsapm-20230506/common/narrow_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23773 2023-05-06 10:39:12.000000 libvsapm-20230506/common/Makefile.in
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3878 2023-05-06 09:06:27.000000 libvsapm-20230506/common/file_stream.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      957 2023-05-06 09:06:27.000000 libvsapm-20230506/common/config_borlandc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15432 2023-05-06 10:39:11.000000 libvsapm-20230506/common/config.h.in
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5064 2023-05-06 09:06:27.000000 libvsapm-20230506/common/wide_string.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 10:54:00.000000 libvsapm-20230506/tests/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1702 2023-05-06 09:06:28.000000 libvsapm-20230506/tests/vsapm_test_memory.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3853 2023-05-06 09:07:22.000000 libvsapm-20230506/tests/test_library.sh
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5004 2023-05-06 09:06:28.000000 libvsapm-20230506/tests/pyvsapm_test_volume.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1462 2023-05-06 09:06:28.000000 libvsapm-20230506/tests/vsapm_test_libcnotify.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1558 2023-05-06 09:06:28.000000 libvsapm-20230506/tests/pyvsapm_test_support.py
+-rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)     3427 2023-05-06 09:06:28.000000 libvsapm-20230506/tests/test_python_module.sh
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      981 2023-05-06 09:06:28.000000 libvsapm-20230506/tests/vsapm_test_libvsapm.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5880 2023-05-06 09:07:22.000000 libvsapm-20230506/tests/Makefile.am
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5634 2023-05-06 09:06:28.000000 libvsapm-20230506/tests/vsapm_test_tools_info_handle.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4535 2023-05-06 09:06:28.000000 libvsapm-20230506/tests/vsapm_test_getopt.c
+-rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)     2168 2023-05-06 09:06:28.000000 libvsapm-20230506/tests/test_vsapminfo.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16671 2023-05-06 09:07:22.000000 libvsapm-20230506/tests/vsapm_test_partition_map_entry.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3139 2023-05-06 09:06:28.000000 libvsapm-20230506/tests/vsapm_test_error.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1813 2023-05-06 09:06:28.000000 libvsapm-20230506/tests/vsapm_test_getopt.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     8056 2023-05-06 09:06:28.000000 libvsapm-20230506/tests/vsapm_test_io_handle.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3802 2023-05-06 09:07:22.000000 libvsapm-20230506/tests/test_tools.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6608 2023-05-06 09:07:22.000000 libvsapm-20230506/tests/vsapm_test_rwlock.c
+-rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)     1653 2023-05-06 09:06:28.000000 libvsapm-20230506/tests/test_manpage.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    60028 2023-05-06 09:07:22.000000 libvsapm-20230506/tests/vsapm_test_partition.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2447 2023-05-06 09:06:28.000000 libvsapm-20230506/tests/vsapm_test_tools_output.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2023-05-06 09:06:28.000000 libvsapm-20230506/tests/vsapm_test_unused.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    37792 2023-05-06 09:06:28.000000 libvsapm-20230506/tests/test_runner.sh
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    13259 2023-05-06 09:06:28.000000 libvsapm-20230506/tests/vsapm_test_functions.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     8574 2023-05-06 09:06:28.000000 libvsapm-20230506/tests/vsapm_test_macros.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4169 2023-05-06 09:06:28.000000 libvsapm-20230506/tests/vsapm_test_tools_signal.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4700 2023-05-06 09:06:28.000000 libvsapm-20230506/tests/vsapm_test_memory.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4323 2023-05-06 09:06:28.000000 libvsapm-20230506/tests/vsapm_test_notify.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1700 2023-05-06 09:06:28.000000 libvsapm-20230506/tests/vsapm_test_rwlock.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1444 2023-05-06 09:06:28.000000 libvsapm-20230506/tests/vsapm_test_libcerror.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1812 2023-05-06 09:06:28.000000 libvsapm-20230506/tests/vsapm_test_functions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    57765 2023-05-06 10:39:13.000000 libvsapm-20230506/tests/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9606 2023-05-06 09:07:22.000000 libvsapm-20230506/tests/vsapm_test_sector_data.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31131 2023-05-06 09:07:22.000000 libvsapm-20230506/tests/vsapm_test_volume.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1742 2023-05-06 09:06:28.000000 libvsapm-20230506/tests/vsapm_test_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9016 2023-05-06 09:07:22.000000 libvsapm-20230506/tests/pyvsapm_test_partition.py
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1709 2023-05-06 09:06:28.000000 libvsapm-20230506/tests/vsapm_test_libbfio.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    14431 2023-05-06 09:06:28.000000 libvsapm-20230506/tests/vsapm_test_support.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1465 2023-05-06 09:06:28.000000 libvsapm-20230506/tests/vsapm_test_libclocale.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 10:53:58.000000 libvsapm-20230506/libclocale/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2023-05-06 10:38:50.000000 libvsapm-20230506/libclocale/libclocale_wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3094 2023-05-06 10:38:50.000000 libvsapm-20230506/libclocale/libclocale_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1717 2023-05-06 10:38:50.000000 libvsapm-20230506/libclocale/libclocale_locale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      744 2023-05-06 10:38:50.000000 libvsapm-20230506/libclocale/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10671 2023-05-06 10:38:50.000000 libvsapm-20230506/libclocale/libclocale_locale.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2023-05-06 10:38:50.000000 libvsapm-20230506/libclocale/libclocale_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2023-05-06 10:38:50.000000 libvsapm-20230506/libclocale/libclocale_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2023-05-06 10:38:50.000000 libvsapm-20230506/libclocale/libclocale_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3412 2023-05-06 10:38:50.000000 libvsapm-20230506/libclocale/libclocale_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2023-05-06 10:38:50.000000 libvsapm-20230506/libclocale/libclocale_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21033 2023-05-06 10:38:50.000000 libvsapm-20230506/libclocale/libclocale_codepage.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28729 2023-05-06 10:39:12.000000 libvsapm-20230506/libclocale/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1969 2023-05-06 10:38:50.000000 libvsapm-20230506/libclocale/libclocale_wide_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2023-05-06 10:38:50.000000 libvsapm-20230506/libclocale/libclocale_libcerror.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2023-05-06 10:39:12.000000 libvsapm-20230506/missing
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3240 2023-05-06 07:39:55.000000 libvsapm-20230506/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    55932 2023-05-06 10:39:09.000000 libvsapm-20230506/aclocal.m4
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 10:53:58.000000 libvsapm-20230506/libbfio/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8883 2023-05-06 10:38:44.000000 libvsapm-20230506/libbfio/libbfio_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2023-05-06 10:38:44.000000 libvsapm-20230506/libbfio/libbfio_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    64816 2023-05-06 10:38:44.000000 libvsapm-20230506/libbfio/libbfio_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2023-05-06 10:38:44.000000 libvsapm-20230506/libbfio/libbfio_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2708 2023-05-06 10:38:44.000000 libvsapm-20230506/libbfio/libbfio_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2023-05-06 10:38:44.000000 libvsapm-20230506/libbfio/libbfio_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2023-05-06 10:38:44.000000 libvsapm-20230506/libbfio/libbfio_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2023-05-06 10:38:44.000000 libvsapm-20230506/libbfio/libbfio_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2023-05-06 10:38:44.000000 libvsapm-20230506/libbfio/libbfio_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12186 2023-05-06 10:38:44.000000 libvsapm-20230506/libbfio/libbfio_file_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27543 2023-05-06 10:38:44.000000 libvsapm-20230506/libbfio/libbfio_file_range_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2023-05-06 10:38:44.000000 libvsapm-20230506/libbfio/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10798 2023-05-06 10:38:44.000000 libvsapm-20230506/libbfio/libbfio_file_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10899 2023-05-06 10:38:44.000000 libvsapm-20230506/libbfio/libbfio_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6841 2023-05-06 10:38:44.000000 libvsapm-20230506/libbfio/libbfio_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2630 2023-05-06 10:38:44.000000 libvsapm-20230506/libbfio/libbfio_file_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2814 2023-05-06 10:38:44.000000 libvsapm-20230506/libbfio/libbfio_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4085 2023-05-06 10:38:44.000000 libvsapm-20230506/libbfio/libbfio_file_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21082 2023-05-06 10:38:44.000000 libvsapm-20230506/libbfio/libbfio_memory_range_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2234 2023-05-06 10:38:44.000000 libvsapm-20230506/libbfio/libbfio_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2324 2023-05-06 10:38:44.000000 libvsapm-20230506/libbfio/libbfio_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2077 2023-05-06 10:38:44.000000 libvsapm-20230506/libbfio/libbfio_file_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3835 2023-05-06 10:38:44.000000 libvsapm-20230506/libbfio/libbfio_memory_range_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2023-05-06 10:38:44.000000 libvsapm-20230506/libbfio/libbfio_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1918 2023-05-06 10:38:44.000000 libvsapm-20230506/libbfio/libbfio_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25540 2023-05-06 10:38:44.000000 libvsapm-20230506/libbfio/libbfio_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2023-05-06 10:38:44.000000 libvsapm-20230506/libbfio/libbfio_memory_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4806 2023-05-06 10:38:44.000000 libvsapm-20230506/libbfio/libbfio_file_range_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5821 2023-05-06 10:38:44.000000 libvsapm-20230506/libbfio/libbfio_memory_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32235 2023-05-06 10:39:12.000000 libvsapm-20230506/libbfio/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    81879 2023-05-06 10:38:44.000000 libvsapm-20230506/libbfio/libbfio_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2023-05-06 10:38:44.000000 libvsapm-20230506/libbfio/libbfio_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1362 2023-05-06 10:38:44.000000 libvsapm-20230506/libbfio/libbfio_libcpath.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1420 2023-05-06 10:38:44.000000 libvsapm-20230506/libbfio/libbfio_libcfile.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2023-05-06 10:38:44.000000 libvsapm-20230506/libbfio/libbfio_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26845 2023-05-06 10:38:44.000000 libvsapm-20230506/libbfio/libbfio_file_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2023-05-06 10:38:44.000000 libvsapm-20230506/libbfio/libbfio_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1572 2023-05-06 10:38:44.000000 libvsapm-20230506/libbfio/libbfio_types.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2023-05-06 09:06:25.000000 libvsapm-20230506/COPYING
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      325 2023-05-06 09:06:25.000000 libvsapm-20230506/README
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      660 2023-05-06 09:06:25.000000 libvsapm-20230506/libvsapm.pc.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 10:53:57.000000 libvsapm-20230506/include/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      494 2023-05-06 09:06:25.000000 libvsapm-20230506/include/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11476 2023-05-06 10:39:22.000000 libvsapm-20230506/include/libvsapm.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11476 2023-05-06 09:48:57.000000 libvsapm-20230506/include/libvsapm.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26774 2023-05-06 10:39:12.000000 libvsapm-20230506/include/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 10:53:57.000000 libvsapm-20230506/include/libvsapm/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1799 2023-05-06 09:06:27.000000 libvsapm-20230506/include/libvsapm/definitions.h.in
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2023-05-06 09:06:27.000000 libvsapm-20230506/include/libvsapm/extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4852 2023-05-06 10:39:22.000000 libvsapm-20230506/include/libvsapm/types.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2023-05-06 09:06:27.000000 libvsapm-20230506/include/libvsapm/features.h.in
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4983 2023-05-06 09:06:27.000000 libvsapm-20230506/include/libvsapm/types.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1487 2023-05-06 10:39:22.000000 libvsapm-20230506/include/libvsapm/features.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1797 2023-05-06 10:39:22.000000 libvsapm-20230506/include/libvsapm/definitions.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5306 2023-05-06 09:06:27.000000 libvsapm-20230506/include/libvsapm/codepage.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     6758 2023-05-06 09:06:27.000000 libvsapm-20230506/include/libvsapm/error.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2023-05-06 10:39:12.000000 libvsapm-20230506/install-sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2023-05-06 10:39:12.000000 libvsapm-20230506/INSTALL
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 10:53:57.000000 libvsapm-20230506/dpkg/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       27 2023-05-06 09:06:25.000000 libvsapm-20230506/dpkg/libvsapm-tools.install
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      121 2023-05-06 09:06:25.000000 libvsapm-20230506/dpkg/changelog.in
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       18 2023-05-06 09:06:25.000000 libvsapm-20230506/dpkg/libvsapm-python3.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      140 2023-05-06 10:39:22.000000 libvsapm-20230506/dpkg/changelog
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1026 2023-05-06 09:06:28.000000 libvsapm-20230506/dpkg/copyright
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       22 2023-05-06 09:06:25.000000 libvsapm-20230506/dpkg/libvsapm.install
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       96 2023-05-06 09:06:25.000000 libvsapm-20230506/dpkg/libvsapm-dev.install
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 10:53:57.000000 libvsapm-20230506/dpkg/source/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       12 2023-05-06 09:06:25.000000 libvsapm-20230506/dpkg/source/format
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      770 2023-05-06 09:06:25.000000 libvsapm-20230506/dpkg/rules
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        3 2023-05-06 09:06:25.000000 libvsapm-20230506/dpkg/compat
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2194 2023-05-06 09:06:25.000000 libvsapm-20230506/dpkg/control
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 10:53:59.000000 libvsapm-20230506/pyvsapm-python2/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1646 2023-05-06 09:06:26.000000 libvsapm-20230506/pyvsapm-python2/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41580 2023-05-06 10:39:13.000000 libvsapm-20230506/pyvsapm-python2/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 10:53:58.000000 libvsapm-20230506/libcfile/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   105597 2023-05-06 10:38:49.000000 libvsapm-20230506/libcfile/libcfile_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2023-05-06 10:38:49.000000 libvsapm-20230506/libcfile/libcfile_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25753 2023-05-06 10:38:49.000000 libvsapm-20230506/libcfile/libcfile_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2389 2023-05-06 10:38:49.000000 libvsapm-20230506/libcfile/libcfile_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2023-05-06 10:38:49.000000 libvsapm-20230506/libcfile/libcfile_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18388 2023-05-06 10:38:49.000000 libvsapm-20230506/libcfile/libcfile_winapi.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      907 2023-05-06 10:38:49.000000 libvsapm-20230506/libcfile/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2023-05-06 10:38:49.000000 libvsapm-20230506/libcfile/libcfile_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2023-05-06 10:38:49.000000 libvsapm-20230506/libcfile/libcfile_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3107 2023-05-06 10:38:49.000000 libvsapm-20230506/libcfile/libcfile_winapi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1497 2023-05-06 10:38:49.000000 libvsapm-20230506/libcfile/libcfile_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2023-05-06 10:38:49.000000 libvsapm-20230506/libcfile/libcfile_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2023-05-06 10:38:49.000000 libvsapm-20230506/libcfile/libcfile_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2879 2023-05-06 10:38:49.000000 libvsapm-20230506/libcfile/libcfile_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6452 2023-05-06 10:38:49.000000 libvsapm-20230506/libcfile/libcfile_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2023-05-06 10:38:49.000000 libvsapm-20230506/libcfile/libcfile_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2023-05-06 10:38:49.000000 libvsapm-20230506/libcfile/libcfile_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29493 2023-05-06 10:39:12.000000 libvsapm-20230506/libcfile/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2023-05-06 10:38:49.000000 libvsapm-20230506/libcfile/libcfile_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2023-05-06 10:38:49.000000 libvsapm-20230506/libcfile/libcfile_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2023-05-06 10:38:49.000000 libvsapm-20230506/libcfile/libcfile_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2023-05-06 10:38:49.000000 libvsapm-20230506/libcfile/libcfile_notify.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3468 2023-05-06 09:06:25.000000 libvsapm-20230506/libvsapm.spec.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 10:53:58.000000 libvsapm-20230506/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2023-05-06 10:38:56.000000 libvsapm-20230506/libcthreads/libcthreads_thread_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2023-05-06 10:38:56.000000 libvsapm-20230506/libcthreads/libcthreads_thread_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2023-05-06 10:38:56.000000 libvsapm-20230506/libcthreads/libcthreads_repeating_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2023-05-06 10:38:56.000000 libvsapm-20230506/libcthreads/libcthreads_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1136 2023-05-06 10:38:56.000000 libvsapm-20230506/libcthreads/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2023-05-06 10:38:56.000000 libvsapm-20230506/libcthreads/libcthreads_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2023-05-06 10:38:56.000000 libvsapm-20230506/libcthreads/libcthreads_condition.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2023-05-06 10:38:56.000000 libvsapm-20230506/libcthreads/libcthreads_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2023-05-06 10:38:56.000000 libvsapm-20230506/libcthreads/libcthreads_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2023-05-06 10:38:56.000000 libvsapm-20230506/libcthreads/libcthreads_repeating_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2023-05-06 10:38:56.000000 libvsapm-20230506/libcthreads/libcthreads_read_write_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2023-05-06 10:38:56.000000 libvsapm-20230506/libcthreads/libcthreads_mutex.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2023-05-06 10:38:56.000000 libvsapm-20230506/libcthreads/libcthreads_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2023-05-06 10:38:56.000000 libvsapm-20230506/libcthreads/libcthreads_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2023-05-06 10:38:56.000000 libvsapm-20230506/libcthreads/libcthreads_mutex.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2023-05-06 10:38:56.000000 libvsapm-20230506/libcthreads/libcthreads_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2023-05-06 10:38:56.000000 libvsapm-20230506/libcthreads/libcthreads_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2023-05-06 10:38:56.000000 libvsapm-20230506/libcthreads/libcthreads_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2023-05-06 10:38:56.000000 libvsapm-20230506/libcthreads/libcthreads_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2023-05-06 10:38:56.000000 libvsapm-20230506/libcthreads/libcthreads_queue.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2023-05-06 10:38:56.000000 libvsapm-20230506/libcthreads/libcthreads_condition.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31583 2023-05-06 10:39:12.000000 libvsapm-20230506/libcthreads/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2023-05-06 10:38:56.000000 libvsapm-20230506/libcthreads/libcthreads_thread_attributes.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2023-05-06 10:38:56.000000 libvsapm-20230506/libcthreads/libcthreads_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2023-05-06 10:38:56.000000 libvsapm-20230506/libcthreads/libcthreads_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2023-05-06 10:38:56.000000 libvsapm-20230506/libcthreads/libcthreads_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2023-05-06 10:38:56.000000 libvsapm-20230506/libcthreads/libcthreads_read_write_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2023-05-06 10:38:56.000000 libvsapm-20230506/libcthreads/libcthreads_thread_attributes.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2023-05-06 10:38:56.000000 libvsapm-20230506/libcthreads/libcthreads_queue.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       92 2023-05-06 09:06:27.000000 libvsapm-20230506/AUTHORS
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35409 2023-05-06 10:39:12.000000 libvsapm-20230506/config.sub
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 10:53:58.000000 libvsapm-20230506/libcpath/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2023-05-06 10:38:53.000000 libvsapm-20230506/libcpath/libcpath_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2336 2023-05-06 10:38:53.000000 libvsapm-20230506/libcpath/libcpath_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2023-05-06 10:38:53.000000 libvsapm-20230506/libcpath/libcpath_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      807 2023-05-06 10:38:53.000000 libvsapm-20230506/libcpath/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2023-05-06 10:38:53.000000 libvsapm-20230506/libcpath/libcpath_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2023-05-06 10:38:53.000000 libvsapm-20230506/libcpath/libcpath_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2023-05-06 10:38:53.000000 libvsapm-20230506/libcpath/libcpath_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2023-05-06 10:38:53.000000 libvsapm-20230506/libcpath/libcpath_libcsplit.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7170 2023-05-06 10:38:53.000000 libvsapm-20230506/libcpath/libcpath_path.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28771 2023-05-06 10:39:12.000000 libvsapm-20230506/libcpath/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1990 2023-05-06 10:38:53.000000 libvsapm-20230506/libcpath/libcpath_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2023-05-06 10:38:53.000000 libvsapm-20230506/libcpath/libcpath_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2023-05-06 10:38:53.000000 libvsapm-20230506/libcpath/libcpath_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   176165 2023-05-06 10:38:53.000000 libvsapm-20230506/libcpath/libcpath_path.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2023-05-06 10:38:53.000000 libvsapm-20230506/libcpath/libcpath_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1461 2023-05-06 10:38:53.000000 libvsapm-20230506/libcpath/libcpath_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2023-05-06 10:38:53.000000 libvsapm-20230506/libcpath/libcpath_libuna.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 10:54:00.000000 libvsapm-20230506/manuals/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      162 2021-05-09 05:40:12.000000 libvsapm-20230506/manuals/Makefile.am
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1777 2023-05-06 09:06:28.000000 libvsapm-20230506/manuals/vsapminfo.1
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25735 2023-05-06 10:39:13.000000 libvsapm-20230506/manuals/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5698 2023-05-06 09:48:57.000000 libvsapm-20230506/manuals/libvsapm.3
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2022-07-15 04:19:38.000000 libvsapm-20230506/ABOUT-NLS
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 10:54:00.000000 libvsapm-20230506/msvscpp/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 10:54:00.000000 libvsapm-20230506/msvscpp/vsapm_test_volume/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6497 2023-05-06 09:07:22.000000 libvsapm-20230506/msvscpp/vsapm_test_volume/vsapm_test_volume.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 10:54:00.000000 libvsapm-20230506/msvscpp/vsapm_test_partition/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6173 2023-05-06 09:07:22.000000 libvsapm-20230506/msvscpp/vsapm_test_partition/vsapm_test_partition.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 10:54:00.000000 libvsapm-20230506/msvscpp/libfcache/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5237 2023-05-06 09:06:48.000000 libvsapm-20230506/msvscpp/libfcache/libfcache.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 10:54:00.000000 libvsapm-20230506/msvscpp/vsapm_test_io_handle/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5681 2023-05-06 09:06:48.000000 libvsapm-20230506/msvscpp/vsapm_test_io_handle/vsapm_test_io_handle.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 10:54:00.000000 libvsapm-20230506/msvscpp/vsapm_test_tools_info_handle/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5782 2023-05-06 09:06:48.000000 libvsapm-20230506/msvscpp/vsapm_test_tools_info_handle/vsapm_test_tools_info_handle.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 10:54:00.000000 libvsapm-20230506/msvscpp/libclocale/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4778 2023-05-06 09:06:48.000000 libvsapm-20230506/msvscpp/libclocale/libclocale.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1179 2023-05-06 09:06:48.000000 libvsapm-20230506/msvscpp/Makefile.am
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 10:54:00.000000 libvsapm-20230506/msvscpp/libbfio/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7306 2023-05-06 09:06:48.000000 libvsapm-20230506/msvscpp/libbfio/libbfio.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25042 2023-05-06 09:07:22.000000 libvsapm-20230506/msvscpp/libvsapm.sln
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 10:54:00.000000 libvsapm-20230506/msvscpp/libcfile/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5597 2023-05-06 09:06:48.000000 libvsapm-20230506/msvscpp/libcfile/libcfile.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 10:54:00.000000 libvsapm-20230506/msvscpp/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2023-05-06 09:06:48.000000 libvsapm-20230506/msvscpp/libcthreads/libcthreads.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 10:54:00.000000 libvsapm-20230506/msvscpp/vsapm_test_error/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5423 2023-05-06 09:06:48.000000 libvsapm-20230506/msvscpp/vsapm_test_error/vsapm_test_error.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 10:54:00.000000 libvsapm-20230506/msvscpp/libcpath/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5183 2023-05-06 09:06:48.000000 libvsapm-20230506/msvscpp/libcpath/libcpath.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 10:54:00.000000 libvsapm-20230506/msvscpp/vsapm_test_sector_data/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5937 2023-05-06 09:06:48.000000 libvsapm-20230506/msvscpp/vsapm_test_sector_data/vsapm_test_sector_data.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 10:54:00.000000 libvsapm-20230506/msvscpp/vsapminfo/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6312 2023-05-06 09:06:48.000000 libvsapm-20230506/msvscpp/vsapminfo/vsapminfo.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 10:54:00.000000 libvsapm-20230506/msvscpp/libuna/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15387 2023-05-06 09:06:48.000000 libvsapm-20230506/msvscpp/libuna/libuna.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21908 2023-05-06 10:39:13.000000 libvsapm-20230506/msvscpp/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 10:54:00.000000 libvsapm-20230506/msvscpp/libvsapm/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7752 2023-05-06 09:06:48.000000 libvsapm-20230506/msvscpp/libvsapm/libvsapm.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 10:54:00.000000 libvsapm-20230506/msvscpp/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2023-05-06 09:06:48.000000 libvsapm-20230506/msvscpp/libcerror/libcerror.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 10:54:00.000000 libvsapm-20230506/msvscpp/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2023-05-06 09:06:48.000000 libvsapm-20230506/msvscpp/libcnotify/libcnotify.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 10:54:00.000000 libvsapm-20230506/msvscpp/vsapm_test_notify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5510 2023-05-06 09:06:48.000000 libvsapm-20230506/msvscpp/vsapm_test_notify/vsapm_test_notify.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 10:54:00.000000 libvsapm-20230506/msvscpp/vsapm_test_tools_output/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5617 2023-05-06 09:06:48.000000 libvsapm-20230506/msvscpp/vsapm_test_tools_output/vsapm_test_tools_output.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 10:54:00.000000 libvsapm-20230506/msvscpp/vsapm_test_support/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6338 2023-05-06 09:06:48.000000 libvsapm-20230506/msvscpp/vsapm_test_support/vsapm_test_support.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 10:54:00.000000 libvsapm-20230506/msvscpp/libfdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6858 2023-05-06 09:06:48.000000 libvsapm-20230506/msvscpp/libfdata/libfdata.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 10:54:00.000000 libvsapm-20230506/msvscpp/libcdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6172 2023-05-06 09:06:48.000000 libvsapm-20230506/msvscpp/libcdata/libcdata.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 10:54:00.000000 libvsapm-20230506/msvscpp/vsapm_test_tools_signal/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5617 2023-05-06 09:06:48.000000 libvsapm-20230506/msvscpp/vsapm_test_tools_signal/vsapm_test_tools_signal.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 10:54:00.000000 libvsapm-20230506/msvscpp/pyvsapm/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6415 2023-05-06 09:06:48.000000 libvsapm-20230506/msvscpp/pyvsapm/pyvsapm.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 10:54:00.000000 libvsapm-20230506/msvscpp/libcsplit/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5225 2023-05-06 09:06:48.000000 libvsapm-20230506/msvscpp/libcsplit/libcsplit.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 10:54:00.000000 libvsapm-20230506/msvscpp/vsapm_test_partition_map_entry/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5961 2023-05-06 09:06:48.000000 libvsapm-20230506/msvscpp/vsapm_test_partition_map_entry/vsapm_test_partition_map_entry.vcproj
+-rwxrwxr-x   0 lordyesta  (1000) lordyesta  (1000)    11497 2023-05-06 09:06:48.000000 libvsapm-20230506/setup.py
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49797 2023-05-06 10:39:12.000000 libvsapm-20230506/config.guess
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 09:06:25.000000 libvsapm-20230506/NEWS
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 10:54:00.000000 libvsapm-20230506/ossfuzz/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2021-05-09 07:25:01.000000 libvsapm-20230506/ossfuzz/Makefile.am
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2700 2023-05-06 09:06:27.000000 libvsapm-20230506/ossfuzz/partition_fuzzer.cc
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2239 2023-05-06 09:06:27.000000 libvsapm-20230506/ossfuzz/volume_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32986 2023-05-06 10:39:13.000000 libvsapm-20230506/ossfuzz/Makefile.in
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      972 2023-05-06 09:06:27.000000 libvsapm-20230506/ossfuzz/ossfuzz_libvsapm.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2023-05-06 09:06:27.000000 libvsapm-20230506/ossfuzz/ossfuzz_libbfio.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2023-05-06 10:39:13.000000 libvsapm-20230506/test-driver
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)  1617768 2023-05-06 10:39:10.000000 libvsapm-20230506/configure
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 10:53:58.000000 libvsapm-20230506/libuna/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15532 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_url_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1801 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_mac_symbol.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1259 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_scsu.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2738 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_iso_8859_5.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3610 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_iso_8859_2.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8602 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_windows_1253.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_koi8_u.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7189 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_windows_1252.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19794 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_utf32_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_windows_1257.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9125 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_mac_cyrillic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9435 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_mac_thai.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    95123 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_utf32_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_mac_thai.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8050 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_windows_874.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1628 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_windows_1251.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   484762 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_windows_949.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_iso_8859_6.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_windows_1256.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_mac_greek.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_mac_russian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_mac_ukrainian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2540 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_iso_8859_6.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_windows_874.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8811 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_windows_1251.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10005 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_windows_1256.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2623 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_base16_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_iso_8859_2.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4162 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9076 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_windows_1257.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_windows_1254.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9211 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_windows_1255.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_windows_1253.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5908 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_unicode_character.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_mac_dingbats.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3181 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_scsu.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15485 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_byte_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_mac_celtic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_mac_croatian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_iso_8859_3.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1346 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_iso_8859_15.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9745 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_mac_roman.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_utf32_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9542 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_koi8_r.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_mac_icelandic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_windows_936.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3679 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_base64_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9871 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_mac_celtic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   360710 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_windows_950.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9666 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_utf8_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   430461 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_windows_936.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   129163 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_unicode_character.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   101951 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_utf8_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82226 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_base32_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_windows_950.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_windows_932.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_mac_turkish.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18019 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_utf8_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9088 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_mac_ukrainian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_koi8_r.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39461 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_base16_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_windows_1250.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1783 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_iso_8859_16.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_mac_croatian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10379 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_mac_gaelic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_utf16_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_iso_8859_10.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9394 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_mac_centraleurroman.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   286239 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_windows_932.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2993 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_utf8_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1929 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_url_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11002 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_mac_farsi.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_windows_949.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_mac_romanian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_mac_gaelic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2629 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_iso_8859_8.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10389 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_mac_arabic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1644 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_windows_1252.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_windows_1250.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_mac_russian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    98825 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_utf16_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_iso_8859_5.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_iso_8859_4.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2921 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_mac_roman.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_utf16_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3561 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_iso_8859_4.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3225 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_iso_8859_10.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_mac_icelandic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    52295 2023-05-06 10:39:13.000000 libvsapm-20230506/libuna/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_utf7_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14020 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_mac_symbol.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3704 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_base32_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9844 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_mac_turkish.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10880 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_mac_inuit.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19595 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_utf16_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15691 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_utf7_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_utf32_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3335 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_iso_8859_3.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9078 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_mac_greek.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16696 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_windows_1255.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2823 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_iso_8859_14.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3664 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_iso_8859_13.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_mac_centraleurroman.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_iso_8859_8.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2053 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_iso_8859_9.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_windows_1254.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_mac_cyrillic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_mac_arabic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9116 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_windows_1258.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_mac_farsi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_iso_8859_15.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2873 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_iso_8859_7.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10134 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_mac_dingbats.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1340 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_iso_8859_9.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1630 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_windows_1258.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    74767 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_base64_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9953 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_mac_romanian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9984 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_koi8_u.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1455 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_iso_8859_13.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_iso_8859_7.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_iso_8859_14.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_mac_inuit.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3296 2023-05-06 10:39:01.000000 libvsapm-20230506/libuna/libuna_codepage_iso_8859_16.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40608 2023-05-06 10:39:12.000000 libvsapm-20230506/Makefile.in
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      404 2021-06-11 04:43:51.000000 libvsapm-20230506/ChangeLog
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 10:53:59.000000 libvsapm-20230506/libvsapm/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2023-05-06 09:06:27.000000 libvsapm-20230506/libvsapm/libvsapm_libcnotify.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2023-05-06 09:06:27.000000 libvsapm-20230506/libvsapm/libvsapm_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1099 2023-05-06 10:39:22.000000 libvsapm-20230506/libvsapm/libvsapm.rc
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     8802 2023-05-06 09:06:27.000000 libvsapm-20230506/libvsapm/libvsapm_sector_data.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2023-05-06 09:06:27.000000 libvsapm-20230506/libvsapm/libvsapm_error.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2822 2023-05-06 09:06:27.000000 libvsapm-20230506/libvsapm/vsapm_partition_map_entry.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2023-05-06 09:06:27.000000 libvsapm-20230506/libvsapm/libvsapm_libclocale.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1897 2023-04-30 04:57:27.000000 libvsapm-20230506/libvsapm/Makefile.am
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1703 2023-05-06 09:06:27.000000 libvsapm-20230506/libvsapm/libvsapm_libbfio.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2179 2023-05-06 09:06:27.000000 libvsapm-20230506/libvsapm/libvsapm_support.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2023-05-06 09:06:27.000000 libvsapm-20230506/libvsapm/libvsapm_libfdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29630 2023-05-06 09:48:57.000000 libvsapm-20230506/libvsapm/libvsapm_partition.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2023-05-06 09:06:27.000000 libvsapm-20230506/libvsapm/libvsapm_notify.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1380 2023-05-06 09:06:27.000000 libvsapm-20230506/libvsapm/libvsapm_debug.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2023-05-06 09:06:27.000000 libvsapm-20230506/libvsapm/libvsapm_unused.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3696 2023-05-06 09:06:27.000000 libvsapm-20230506/libvsapm/libvsapm_io_handle.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2175 2023-05-06 09:06:27.000000 libvsapm-20230506/libvsapm/libvsapm_definitions.h.in
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2023-05-06 09:06:27.000000 libvsapm-20230506/libvsapm/libvsapm_extern.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1101 2023-05-06 09:06:27.000000 libvsapm-20230506/libvsapm/libvsapm.rc.in
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4179 2023-05-06 09:06:27.000000 libvsapm-20230506/libvsapm/libvsapm_debug.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     9852 2023-05-06 09:06:27.000000 libvsapm-20230506/libvsapm/libvsapm_support.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3247 2023-05-06 09:06:27.000000 libvsapm-20230506/libvsapm/libvsapm_partition_map_entry.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2173 2023-05-06 10:39:22.000000 libvsapm-20230506/libvsapm/libvsapm_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4385 2023-05-06 09:48:57.000000 libvsapm-20230506/libvsapm/libvsapm_partition.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2023-05-06 09:06:27.000000 libvsapm-20230506/libvsapm/libvsapm_libfcache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33074 2023-05-06 10:39:13.000000 libvsapm-20230506/libvsapm/Makefile.in
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2023-05-06 09:06:27.000000 libvsapm-20230506/libvsapm/libvsapm_libcerror.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1682 2023-05-06 09:06:27.000000 libvsapm-20230506/libvsapm/libvsapm_io_handle.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3995 2023-05-06 09:06:27.000000 libvsapm-20230506/libvsapm/libvsapm_volume.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2023-05-06 09:06:27.000000 libvsapm-20230506/libvsapm/libvsapm_notify.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2023-05-06 09:06:27.000000 libvsapm-20230506/libvsapm/libvsapm_error.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1844 2023-05-06 09:06:27.000000 libvsapm-20230506/libvsapm/libvsapm.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1601 2023-05-06 09:06:27.000000 libvsapm-20230506/libvsapm/libvsapm_types.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2023-05-06 09:06:27.000000 libvsapm-20230506/libvsapm/libvsapm_libcdata.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2151 2023-05-06 09:06:27.000000 libvsapm-20230506/libvsapm/libvsapm_sector_data.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    34820 2023-05-06 09:06:27.000000 libvsapm-20230506/libvsapm/libvsapm_volume.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    17794 2023-05-06 09:06:27.000000 libvsapm-20230506/libvsapm/libvsapm_partition_map_entry.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 10:53:57.000000 libvsapm-20230506/m4/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    23765 2021-09-11 08:08:59.000000 libvsapm-20230506/m4/libuna.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2022-07-15 04:19:38.000000 libvsapm-20230506/m4/gettext.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      756 2021-05-09 05:40:12.000000 libvsapm-20230506/m4/tests.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2022-07-15 04:19:38.000000 libvsapm-20230506/m4/lib-prefix.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2023-05-06 10:39:06.000000 libvsapm-20230506/m4/ltoptions.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     9379 2021-05-09 05:40:12.000000 libvsapm-20230506/m4/libcpath.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2022-07-15 04:19:38.000000 libvsapm-20230506/m4/lib-ld.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11112 2021-05-09 05:40:12.000000 libvsapm-20230506/m4/libcthreads.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2022-07-15 04:19:38.000000 libvsapm-20230506/m4/lib-link.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    17674 2021-12-23 13:41:17.000000 libvsapm-20230506/m4/python.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2023-05-06 10:39:06.000000 libvsapm-20230506/m4/libtool.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2022-07-15 04:19:38.000000 libvsapm-20230506/m4/nls.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     8230 2021-05-09 05:40:12.000000 libvsapm-20230506/m4/libclocale.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    15545 2023-03-20 05:48:50.000000 libvsapm-20230506/m4/libfdata.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2021-05-09 05:08:54.000000 libvsapm-20230506/m4/host-cpu-c-abi.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5638 2021-05-09 05:40:12.000000 libvsapm-20230506/m4/libcnotify.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2023-05-06 10:39:06.000000 libvsapm-20230506/m4/ltversion.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    17147 2023-02-11 06:41:16.000000 libvsapm-20230506/m4/libcdata.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2022-07-15 04:19:38.000000 libvsapm-20230506/m4/progtest.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2023-05-06 10:39:06.000000 libvsapm-20230506/m4/lt~obsolete.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11498 2021-05-09 05:40:12.000000 libvsapm-20230506/m4/libcfile.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2022-07-15 04:19:38.000000 libvsapm-20230506/m4/po.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3852 2021-05-09 05:40:12.000000 libvsapm-20230506/m4/pthread.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    14115 2021-05-09 05:40:12.000000 libvsapm-20230506/m4/common.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     6260 2021-05-09 05:40:12.000000 libvsapm-20230506/m4/libcerror.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2022-07-15 04:19:38.000000 libvsapm-20230506/m4/iconv.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2023-05-06 10:39:06.000000 libvsapm-20230506/m4/ltsugar.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     7325 2023-02-11 06:41:17.000000 libvsapm-20230506/m4/libfcache.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     7384 2021-05-09 05:40:12.000000 libvsapm-20230506/m4/libcsplit.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2022-07-15 04:19:38.000000 libvsapm-20230506/m4/intlmacosx.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2021-05-09 05:40:12.000000 libvsapm-20230506/m4/types.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    11692 2021-05-09 05:40:12.000000 libvsapm-20230506/m4/libbfio.m4
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2023-05-06 09:06:25.000000 libvsapm-20230506/COPYING.LESSER
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 10:53:58.000000 libvsapm-20230506/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2023-05-06 10:38:47.000000 libvsapm-20230506/libcerror/libcerror_system.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2023-05-06 10:38:47.000000 libvsapm-20230506/libcerror/libcerror_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2023-05-06 10:38:47.000000 libvsapm-20230506/libcerror/libcerror_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      605 2023-05-06 10:38:47.000000 libvsapm-20230506/libcerror/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2023-05-06 10:38:47.000000 libvsapm-20230506/libcerror/libcerror_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2023-05-06 10:38:47.000000 libvsapm-20230506/libcerror/libcerror_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2023-05-06 10:38:47.000000 libvsapm-20230506/libcerror/libcerror_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2023-05-06 10:38:47.000000 libvsapm-20230506/libcerror/libcerror_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2023-05-06 10:38:47.000000 libvsapm-20230506/libcerror/libcerror_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28118 2023-05-06 10:39:12.000000 libvsapm-20230506/libcerror/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2023-05-06 10:38:47.000000 libvsapm-20230506/libcerror/libcerror_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2023-05-06 10:38:47.000000 libvsapm-20230506/libcerror/libcerror_system.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 10:53:59.000000 libvsapm-20230506/pyvsapm-python3/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1646 2023-05-06 09:06:26.000000 libvsapm-20230506/pyvsapm-python3/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41580 2023-05-06 10:39:13.000000 libvsapm-20230506/pyvsapm-python3/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 10:53:58.000000 libvsapm-20230506/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2023-05-06 10:38:51.000000 libvsapm-20230506/libcnotify/libcnotify_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2023-05-06 10:38:51.000000 libvsapm-20230506/libcnotify/libcnotify_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2023-05-06 10:38:51.000000 libvsapm-20230506/libcnotify/libcnotify_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2023-05-06 10:38:51.000000 libvsapm-20230506/libcnotify/libcnotify_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      693 2023-05-06 10:38:51.000000 libvsapm-20230506/libcnotify/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2023-05-06 10:38:51.000000 libvsapm-20230506/libcnotify/libcnotify_print.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2023-05-06 10:38:51.000000 libvsapm-20230506/libcnotify/libcnotify_verbose.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2023-05-06 10:38:51.000000 libvsapm-20230506/libcnotify/libcnotify_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2023-05-06 10:38:51.000000 libvsapm-20230506/libcnotify/libcnotify_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2023-05-06 10:38:51.000000 libvsapm-20230506/libcnotify/libcnotify_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28605 2023-05-06 10:39:12.000000 libvsapm-20230506/libcnotify/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2023-05-06 10:38:51.000000 libvsapm-20230506/libcnotify/libcnotify_print.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2023-05-06 10:38:51.000000 libvsapm-20230506/libcnotify/libcnotify_verbose.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2023-05-06 10:38:51.000000 libvsapm-20230506/libcnotify/libcnotify_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2023-05-06 10:39:06.000000 libvsapm-20230506/ltmain.sh
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2023-05-06 10:39:12.000000 libvsapm-20230506/compile
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 10:53:59.000000 libvsapm-20230506/vsapmtools/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17817 2023-05-06 09:07:22.000000 libvsapm-20230506/vsapmtools/info_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6883 2023-05-06 09:07:22.000000 libvsapm-20230506/vsapmtools/vsapminfo.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1748 2023-05-06 09:06:28.000000 libvsapm-20230506/vsapmtools/vsapmtools_libbfio.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1130 2021-05-09 05:40:12.000000 libvsapm-20230506/vsapmtools/Makefile.am
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     5707 2023-05-06 09:06:28.000000 libvsapm-20230506/vsapmtools/vsapmtools_signal.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4535 2023-05-06 09:06:28.000000 libvsapm-20230506/vsapmtools/vsapmtools_getopt.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1483 2023-05-06 09:06:28.000000 libvsapm-20230506/vsapmtools/vsapmtools_libcerror.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2023-05-06 09:06:28.000000 libvsapm-20230506/vsapmtools/vsapmtools_unused.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1761 2023-05-06 09:06:28.000000 libvsapm-20230506/vsapmtools/vsapmtools_signal.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1501 2023-05-06 09:06:28.000000 libvsapm-20230506/vsapmtools/vsapmtools_libcnotify.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1781 2023-05-06 09:06:28.000000 libvsapm-20230506/vsapmtools/vsapmtools_libuna.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      981 2023-05-06 09:06:28.000000 libvsapm-20230506/vsapmtools/vsapmtools_libvsapm.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2647 2023-05-06 09:07:22.000000 libvsapm-20230506/vsapmtools/info_handle.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1472 2023-05-06 09:06:28.000000 libvsapm-20230506/vsapmtools/vsapmtools_output.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30141 2023-05-06 10:39:13.000000 libvsapm-20230506/vsapmtools/Makefile.in
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1504 2023-05-06 09:06:28.000000 libvsapm-20230506/vsapmtools/vsapmtools_libclocale.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1213 2023-05-06 09:06:28.000000 libvsapm-20230506/vsapmtools/vsapmtools_i18n.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1813 2023-05-06 09:06:28.000000 libvsapm-20230506/vsapmtools/vsapmtools_getopt.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     3451 2023-05-06 09:06:28.000000 libvsapm-20230506/vsapmtools/vsapmtools_output.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2022-07-15 04:19:38.000000 libvsapm-20230506/config.rpath
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2023-05-06 10:39:13.000000 libvsapm-20230506/depcomp
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 10:54:00.000000 libvsapm-20230506/po/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2022-07-15 04:19:38.000000 libvsapm-20230506/po/en@quot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2022-07-15 04:19:38.000000 libvsapm-20230506/po/Rules-quot
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       59 2021-05-09 05:40:12.000000 libvsapm-20230506/po/POTFILES.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2022-07-15 04:19:38.000000 libvsapm-20230506/po/remove-potcdate.sin
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1808 2021-05-09 05:40:12.000000 libvsapm-20230506/po/Makevars.in
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)       50 2021-05-09 05:40:12.000000 libvsapm-20230506/po/ChangeLog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2022-07-15 04:19:38.000000 libvsapm-20230506/po/en@boldquot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2021-05-09 05:09:30.000000 libvsapm-20230506/po/quot.sed
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1810 2023-05-06 10:39:22.000000 libvsapm-20230506/po/Makevars
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2022-07-15 04:19:38.000000 libvsapm-20230506/po/insert-header.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2022-07-15 04:19:38.000000 libvsapm-20230506/po/Makefile.in.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2021-05-09 05:09:30.000000 libvsapm-20230506/po/boldquot.sed
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 10:53:59.000000 libvsapm-20230506/libfdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2804 2023-05-06 10:38:59.000000 libvsapm-20230506/libfdata/libfdata_segments_array.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2023-05-06 10:38:59.000000 libvsapm-20230506/libfdata/libfdata_cache.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1172 2023-05-06 10:38:59.000000 libvsapm-20230506/libfdata/libfdata_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19329 2023-05-06 10:38:59.000000 libvsapm-20230506/libfdata/libfdata_list_element.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1995 2023-05-06 10:38:59.000000 libvsapm-20230506/libfdata/libfdata_mapped_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2023-05-06 10:38:59.000000 libvsapm-20230506/libfdata/libfdata_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   107689 2023-05-06 10:38:59.000000 libvsapm-20230506/libfdata/libfdata_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2023-05-06 10:38:59.000000 libvsapm-20230506/libfdata/libfdata_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2023-05-06 10:38:59.000000 libvsapm-20230506/libfdata/libfdata_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6013 2023-05-06 10:38:59.000000 libvsapm-20230506/libfdata/libfdata_range_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1256 2023-05-06 10:38:59.000000 libvsapm-20230506/libfdata/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2023-05-06 10:38:59.000000 libvsapm-20230506/libfdata/libfdata_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12090 2023-05-06 10:38:59.000000 libvsapm-20230506/libfdata/libfdata_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7327 2023-05-06 10:38:59.000000 libvsapm-20230506/libfdata/libfdata_area.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2054 2023-05-06 10:38:59.000000 libvsapm-20230506/libfdata/libfdata_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37893 2023-05-06 10:38:59.000000 libvsapm-20230506/libfdata/libfdata_area.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2092 2023-05-06 10:38:59.000000 libvsapm-20230506/libfdata/libfdata_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49670 2023-05-06 10:38:59.000000 libvsapm-20230506/libfdata/libfdata_vector.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9700 2023-05-06 10:38:59.000000 libvsapm-20230506/libfdata/libfdata_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7810 2023-05-06 10:38:59.000000 libvsapm-20230506/libfdata/libfdata_vector.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2023-05-06 10:38:59.000000 libvsapm-20230506/libfdata/libfdata_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2023-05-06 10:38:59.000000 libvsapm-20230506/libfdata/libfdata_libfcache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2023-05-06 10:38:59.000000 libvsapm-20230506/libfdata/libfdata_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30931 2023-05-06 10:38:59.000000 libvsapm-20230506/libfdata/libfdata_range_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2023-05-06 10:38:59.000000 libvsapm-20230506/libfdata/libfdata_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2023-05-06 10:38:59.000000 libvsapm-20230506/libfdata/libfdata_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3999 2023-05-06 10:38:59.000000 libvsapm-20230506/libfdata/libfdata_list_element.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2023-05-06 10:38:59.000000 libvsapm-20230506/libfdata/libfdata_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2023-05-06 10:38:59.000000 libvsapm-20230506/libfdata/libfdata_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31958 2023-05-06 10:39:12.000000 libvsapm-20230506/libfdata/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1491 2023-05-06 10:38:59.000000 libvsapm-20230506/libfdata/libfdata_cache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    66203 2023-05-06 10:38:59.000000 libvsapm-20230506/libfdata/libfdata_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21271 2023-05-06 10:38:59.000000 libvsapm-20230506/libfdata/libfdata_segments_array.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6826 2023-05-06 10:38:59.000000 libvsapm-20230506/libfdata/libfdata_mapped_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6533 2023-05-06 10:38:59.000000 libvsapm-20230506/libfdata/libfdata_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7149 2023-05-06 10:38:59.000000 libvsapm-20230506/libfdata/libfdata_range.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 10:53:58.000000 libvsapm-20230506/libcdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49968 2023-05-06 10:38:45.000000 libvsapm-20230506/libcdata/libcdata_array.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37549 2023-05-06 10:38:45.000000 libvsapm-20230506/libcdata/libcdata_btree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100501 2023-05-06 10:38:45.000000 libvsapm-20230506/libcdata/libcdata_tree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2023-05-06 10:38:45.000000 libvsapm-20230506/libcdata/libcdata_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2789 2023-05-06 10:38:45.000000 libvsapm-20230506/libcdata/libcdata_range_list_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2023-05-06 10:38:45.000000 libvsapm-20230506/libcdata/libcdata_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12295 2023-05-06 10:38:45.000000 libvsapm-20230506/libcdata/libcdata_range_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1092 2023-05-06 10:38:46.000000 libvsapm-20230506/libcdata/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   122285 2023-05-06 10:38:45.000000 libvsapm-20230506/libcdata/libcdata_range_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2023-05-06 10:38:45.000000 libvsapm-20230506/libcdata/libcdata_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2023-05-06 10:38:45.000000 libvsapm-20230506/libcdata/libcdata_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3871 2023-05-06 10:38:45.000000 libvsapm-20230506/libcdata/libcdata_list_element.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5251 2023-05-06 10:38:45.000000 libvsapm-20230506/libcdata/libcdata_btree_values_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10647 2023-05-06 10:38:45.000000 libvsapm-20230506/libcdata/libcdata_range_list_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2023-05-06 10:38:45.000000 libvsapm-20230506/libcdata/libcdata_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2023-05-06 10:38:45.000000 libvsapm-20230506/libcdata/libcdata_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2023-05-06 10:38:45.000000 libvsapm-20230506/libcdata/libcdata_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2023-05-06 10:38:45.000000 libvsapm-20230506/libcdata/libcdata_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2960 2023-05-06 10:38:45.000000 libvsapm-20230506/libcdata/libcdata_btree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69515 2023-05-06 10:38:45.000000 libvsapm-20230506/libcdata/libcdata_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8365 2023-05-06 10:38:45.000000 libvsapm-20230506/libcdata/libcdata_tree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6448 2023-05-06 10:38:45.000000 libvsapm-20230506/libcdata/libcdata_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2023-05-06 10:38:45.000000 libvsapm-20230506/libcdata/libcdata_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23846 2023-05-06 10:38:45.000000 libvsapm-20230506/libcdata/libcdata_list_element.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31177 2023-05-06 10:39:12.000000 libvsapm-20230506/libcdata/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2023-05-06 10:38:45.000000 libvsapm-20230506/libcdata/libcdata_btree_values_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5231 2023-05-06 10:38:45.000000 libvsapm-20230506/libcdata/libcdata_array.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3790 2023-05-06 10:38:45.000000 libvsapm-20230506/libcdata/libcdata_btree.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2023-05-06 10:38:46.000000 libvsapm-20230506/libcdata/libcdata_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22358 2023-05-06 10:38:45.000000 libvsapm-20230506/libcdata/libcdata_btree.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 10:53:59.000000 libvsapm-20230506/pyvsapm/
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1544 2023-05-06 09:06:28.000000 libvsapm-20230506/pyvsapm/pyvsapm_integer.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2023-05-06 09:06:28.000000 libvsapm-20230506/pyvsapm/pyvsapm_unused.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2023-05-06 09:06:28.000000 libvsapm-20230506/pyvsapm/pyvsapm_libcerror.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     4118 2023-05-06 09:06:28.000000 libvsapm-20230506/pyvsapm/pyvsapm_file_object_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25879 2023-05-06 09:48:57.000000 libvsapm-20230506/pyvsapm/pyvsapm_partition.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2033 2023-05-06 09:06:28.000000 libvsapm-20230506/pyvsapm/pyvsapm_python.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     8876 2023-05-06 09:06:28.000000 libvsapm-20230506/pyvsapm/pyvsapm_integer.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1172 2021-06-10 04:17:11.000000 libvsapm-20230506/pyvsapm/Makefile.am
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)      973 2023-05-06 09:06:28.000000 libvsapm-20230506/pyvsapm/pyvsapm_libvsapm.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3031 2023-05-06 09:48:57.000000 libvsapm-20230506/pyvsapm/pyvsapm_partition.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1868 2023-05-06 09:06:28.000000 libvsapm-20230506/pyvsapm/pyvsapm.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1525 2023-05-06 09:06:28.000000 libvsapm-20230506/pyvsapm/pyvsapm_libbfio.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    14846 2023-05-06 09:06:28.000000 libvsapm-20230506/pyvsapm/pyvsapm.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     2445 2023-05-06 09:06:28.000000 libvsapm-20230506/pyvsapm/pyvsapm_partitions.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2023-05-06 09:06:28.000000 libvsapm-20230506/pyvsapm/pyvsapm_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2825 2023-05-06 09:07:22.000000 libvsapm-20230506/pyvsapm/pyvsapm_volume.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     9546 2023-05-06 09:06:28.000000 libvsapm-20230506/pyvsapm/pyvsapm_error.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1540 2023-05-06 09:06:28.000000 libvsapm-20230506/pyvsapm/pyvsapm_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41205 2023-05-06 10:39:13.000000 libvsapm-20230506/pyvsapm/Makefile.in
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)    33875 2023-05-06 09:06:28.000000 libvsapm-20230506/pyvsapm/pyvsapm_file_object_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22133 2023-05-06 09:07:22.000000 libvsapm-20230506/pyvsapm/pyvsapm_volume.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     9329 2023-05-06 09:06:28.000000 libvsapm-20230506/pyvsapm/pyvsapm_partitions.c
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     1208 2023-05-06 09:06:25.000000 libvsapm-20230506/acinclude.m4
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 10:53:58.000000 libvsapm-20230506/libcsplit/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1679 2023-05-06 10:38:54.000000 libvsapm-20230506/libcsplit/libcsplit_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1471 2023-05-06 10:38:54.000000 libvsapm-20230506/libcsplit/libcsplit_wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2023-05-06 10:38:54.000000 libvsapm-20230506/libcsplit/libcsplit_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2023-05-06 10:38:54.000000 libvsapm-20230506/libcsplit/libcsplit_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13912 2023-05-06 10:38:54.000000 libvsapm-20230506/libcsplit/libcsplit_narrow_split_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2849 2023-05-06 10:38:54.000000 libvsapm-20230506/libcsplit/libcsplit_narrow_split_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      849 2023-05-06 10:38:54.000000 libvsapm-20230506/libcsplit/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13944 2023-05-06 10:38:54.000000 libvsapm-20230506/libcsplit/libcsplit_wide_split_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1386 2023-05-06 10:38:54.000000 libvsapm-20230506/libcsplit/libcsplit_narrow_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2023-05-06 10:38:54.000000 libvsapm-20230506/libcsplit/libcsplit_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6206 2023-05-06 10:38:54.000000 libvsapm-20230506/libcsplit/libcsplit_wide_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6125 2023-05-06 10:38:54.000000 libvsapm-20230506/libcsplit/libcsplit_narrow_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29551 2023-05-06 10:39:12.000000 libvsapm-20230506/libcsplit/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2920 2023-05-06 10:38:54.000000 libvsapm-20230506/libcsplit/libcsplit_wide_split_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1360 2023-05-06 10:38:54.000000 libvsapm-20230506/libcsplit/libcsplit_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2023-05-06 10:38:54.000000 libvsapm-20230506/libcsplit/libcsplit_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2023-05-06 10:38:54.000000 libvsapm-20230506/libcsplit/libcsplit_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2023-05-06 10:38:54.000000 libvsapm-20230506/libcsplit/libcsplit_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2023-05-06 10:38:54.000000 libvsapm-20230506/libcsplit/libcsplit_extern.h
+-rw-rw-r--   0 lordyesta  (1000) lordyesta  (1000)     7083 2023-05-06 09:06:25.000000 libvsapm-20230506/configure.ac
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      351 2023-05-06 10:54:01.421168 libvsapm-20230506/PKG-INFO
```

### Comparing `libvsapm-20230430/libvsapm.spec` & `libvsapm-20230506/libvsapm.spec`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 Name: libvsapm
-Version: 20230430
+Version: 20230506
 Release: 1
 Summary: Library to access the Apple Partition Map (APM) volume system format
 Group: System Environment/Libraries
 License: LGPLv3+
 Source: %{name}-%{version}.tar.gz
 URL: https://github.com/libyal/libvsapm
 BuildRoot: %{_tmppath}/%{name}-%{version}-%{release}-root-%(%{__id_u} -n)
@@ -96,10 +96,10 @@
 %defattr(644,root,root,755)
 %license COPYING COPYING.LESSER
 %doc AUTHORS README
 %attr(755,root,root) %{_bindir}/*
 %{_mandir}/man1/*
 
 %changelog
-* Thu May  4 2023 Joachim Metz <joachim.metz@gmail.com> 20230430-1
+* Sat May  6 2023 Joachim Metz <joachim.metz@gmail.com> 20230506-1
 - Auto-generated
```

### Comparing `libvsapm-20230430/libfcache/libfcache_extern.h` & `libvsapm-20230506/libfcache/libfcache_extern.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libfcache/libfcache_types.h` & `libvsapm-20230506/libfcache/libfcache_types.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libfcache/libfcache_cache.h` & `libvsapm-20230506/libfcache/libfcache_cache.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libfcache/libfcache_support.h` & `libvsapm-20230506/libfcache/libfcache_support.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libfcache/libfcache_support.c` & `libvsapm-20230506/libfcache/libfcache_support.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libfcache/Makefile.am` & `libvsapm-20230506/libfcache/Makefile.am`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libfcache/libfcache_libcdata.h` & `libvsapm-20230506/libfcache/libfcache_libcdata.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libfcache/libfcache_unused.h` & `libvsapm-20230506/libfcache/libfcache_unused.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libfcache/libfcache_libcerror.h` & `libvsapm-20230506/libfcache/libfcache_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libfcache/libfcache_definitions.h` & `libvsapm-20230506/libfcache/libfcache_definitions.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libfcache/libfcache_cache_value.h` & `libvsapm-20230506/libfcache/libfcache_cache_value.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libfcache/libfcache_cache_value.c` & `libvsapm-20230506/libfcache/libfcache_cache_value.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libfcache/Makefile.in` & `libvsapm-20230506/libfcache/Makefile.in`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libfcache/libfcache_error.c` & `libvsapm-20230506/libfcache/libfcache_error.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libfcache/libfcache_date_time.c` & `libvsapm-20230506/libfcache/libfcache_date_time.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libfcache/libfcache_cache.c` & `libvsapm-20230506/libfcache/libfcache_cache.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libfcache/libfcache_error.h` & `libvsapm-20230506/libfcache/libfcache_error.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libfcache/libfcache_date_time.h` & `libvsapm-20230506/libfcache/libfcache_date_time.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/common/config_msc.h` & `libvsapm-20230506/common/config_msc.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/common/byte_stream.h` & `libvsapm-20230506/common/byte_stream.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/common/common.h` & `libvsapm-20230506/common/common.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/common/system_string.h` & `libvsapm-20230506/common/system_string.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/common/types.h` & `libvsapm-20230506/common/types.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/common/types.h.in` & `libvsapm-20230506/common/types.h.in`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/common/config_winapi.h` & `libvsapm-20230506/common/config_winapi.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/common/memory.h` & `libvsapm-20230506/common/memory.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/common/config.h` & `libvsapm-20230506/common/config.h`

 * *Files 1% similar despite different names*

```diff
@@ -505,24 +505,24 @@
 /* Define to the address where bug reports for this package should be sent. */
 #define PACKAGE_BUGREPORT "joachim.metz@gmail.com"
 
 /* Define to the full name of this package. */
 #define PACKAGE_NAME "libvsapm"
 
 /* Define to the full name and version of this package. */
-#define PACKAGE_STRING "libvsapm 20230430"
+#define PACKAGE_STRING "libvsapm 20230506"
 
 /* Define to the one symbol short name of this package. */
 #define PACKAGE_TARNAME "libvsapm"
 
 /* Define to the home page for this package. */
 #define PACKAGE_URL ""
 
 /* Define to the version of this package. */
-#define PACKAGE_VERSION "20230430"
+#define PACKAGE_VERSION "20230506"
 
 /* The size of `int', as computed by sizeof. */
 #define SIZEOF_INT 4
 
 /* The size of `long', as computed by sizeof. */
 #define SIZEOF_LONG 8
 
@@ -543,15 +543,15 @@
 /* Define to 1 if strerror_r returns char *. */
 /* #undef STRERROR_R_CHAR_P */
 
 /* Define to 1 if your <sys/time.h> declares `struct tm'. */
 /* #undef TM_IN_SYS_TIME */
 
 /* Version number of package */
-#define VERSION "20230430"
+#define VERSION "20230506"
 
 /* Number of bits in a file offset, on hosts where this is settable. */
 /* #undef _FILE_OFFSET_BITS */
 
 /* Define for large files, on AIX-style hosts. */
 /* #undef _LARGE_FILES */
```

### Comparing `libvsapm-20230430/common/narrow_string.h` & `libvsapm-20230506/common/narrow_string.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/common/Makefile.in` & `libvsapm-20230506/common/Makefile.in`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/common/file_stream.h` & `libvsapm-20230506/common/file_stream.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/common/config_borlandc.h` & `libvsapm-20230506/common/config_borlandc.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/common/config.h.in` & `libvsapm-20230506/common/config.h.in`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/common/wide_string.h` & `libvsapm-20230506/common/wide_string.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/tests/vsapm_test_memory.h` & `libvsapm-20230506/tests/vsapm_test_memory.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/tests/test_library.sh` & `libvsapm-20230506/tests/test_library.sh`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/tests/pyvsapm_test_volume.py` & `libvsapm-20230506/tests/pyvsapm_test_volume.py`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/tests/vsapm_test_libcnotify.h` & `libvsapm-20230506/tests/vsapm_test_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/tests/pyvsapm_test_support.py` & `libvsapm-20230506/tests/pyvsapm_test_support.py`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/tests/test_python_module.sh` & `libvsapm-20230506/tests/test_python_module.sh`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/tests/vsapm_test_libvsapm.h` & `libvsapm-20230506/tests/vsapm_test_libvsapm.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/tests/Makefile.am` & `libvsapm-20230506/tests/Makefile.am`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/tests/vsapm_test_tools_info_handle.c` & `libvsapm-20230506/tests/vsapm_test_tools_info_handle.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/tests/vsapm_test_getopt.c` & `libvsapm-20230506/tests/vsapm_test_getopt.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/tests/test_vsapminfo.sh` & `libvsapm-20230506/tests/test_vsapminfo.sh`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/tests/vsapm_test_partition_map_entry.c` & `libvsapm-20230506/tests/vsapm_test_partition_map_entry.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/tests/vsapm_test_error.c` & `libvsapm-20230506/tests/vsapm_test_error.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/tests/vsapm_test_getopt.h` & `libvsapm-20230506/tests/vsapm_test_getopt.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/tests/vsapm_test_io_handle.c` & `libvsapm-20230506/tests/vsapm_test_io_handle.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/tests/test_tools.sh` & `libvsapm-20230506/tests/test_tools.sh`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/tests/vsapm_test_rwlock.c` & `libvsapm-20230506/tests/vsapm_test_rwlock.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/tests/test_manpage.sh` & `libvsapm-20230506/tests/test_manpage.sh`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/tests/vsapm_test_partition.c` & `libvsapm-20230506/tests/vsapm_test_partition.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/tests/vsapm_test_tools_output.c` & `libvsapm-20230506/tests/vsapm_test_tools_output.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/tests/vsapm_test_unused.h` & `libvsapm-20230506/tests/vsapm_test_unused.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/tests/test_runner.sh` & `libvsapm-20230506/tests/test_runner.sh`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/tests/vsapm_test_functions.c` & `libvsapm-20230506/tests/vsapm_test_functions.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/tests/vsapm_test_macros.h` & `libvsapm-20230506/tests/vsapm_test_macros.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/tests/vsapm_test_tools_signal.c` & `libvsapm-20230506/tests/vsapm_test_tools_signal.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/tests/vsapm_test_memory.c` & `libvsapm-20230506/tests/vsapm_test_memory.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/tests/vsapm_test_notify.c` & `libvsapm-20230506/tests/vsapm_test_notify.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/tests/vsapm_test_rwlock.h` & `libvsapm-20230506/tests/vsapm_test_rwlock.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/tests/vsapm_test_libcerror.h` & `libvsapm-20230506/tests/vsapm_test_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/tests/vsapm_test_functions.h` & `libvsapm-20230506/tests/vsapm_test_functions.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/tests/Makefile.in` & `libvsapm-20230506/tests/Makefile.in`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/tests/vsapm_test_sector_data.c` & `libvsapm-20230506/tests/vsapm_test_sector_data.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/tests/vsapm_test_volume.c` & `libvsapm-20230506/tests/vsapm_test_volume.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/tests/vsapm_test_libuna.h` & `libvsapm-20230506/tests/vsapm_test_libuna.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/tests/pyvsapm_test_partition.py` & `libvsapm-20230506/tests/pyvsapm_test_partition.py`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/tests/vsapm_test_libbfio.h` & `libvsapm-20230506/tests/vsapm_test_libbfio.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/tests/vsapm_test_support.c` & `libvsapm-20230506/tests/vsapm_test_support.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/tests/vsapm_test_libclocale.h` & `libvsapm-20230506/tests/vsapm_test_libclocale.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libclocale/libclocale_wide_string.h` & `libvsapm-20230506/libclocale/libclocale_wide_string.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libclocale/libclocale_support.c` & `libvsapm-20230506/libclocale/libclocale_support.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libclocale/libclocale_locale.h` & `libvsapm-20230506/libclocale/libclocale_locale.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libclocale/Makefile.am` & `libvsapm-20230506/libclocale/Makefile.am`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libclocale/libclocale_locale.c` & `libvsapm-20230506/libclocale/libclocale_locale.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libclocale/libclocale_extern.h` & `libvsapm-20230506/libclocale/libclocale_extern.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libclocale/libclocale_unused.h` & `libvsapm-20230506/libclocale/libclocale_unused.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libclocale/libclocale_support.h` & `libvsapm-20230506/libclocale/libclocale_support.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libclocale/libclocale_definitions.h` & `libvsapm-20230506/libclocale/libclocale_definitions.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libclocale/libclocale_codepage.h` & `libvsapm-20230506/libclocale/libclocale_codepage.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libclocale/libclocale_codepage.c` & `libvsapm-20230506/libclocale/libclocale_codepage.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libclocale/Makefile.in` & `libvsapm-20230506/libclocale/Makefile.in`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libclocale/libclocale_wide_string.c` & `libvsapm-20230506/libclocale/libclocale_wide_string.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libclocale/libclocale_libcerror.h` & `libvsapm-20230506/libclocale/libclocale_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/missing` & `libvsapm-20230506/missing`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/Makefile.am` & `libvsapm-20230506/Makefile.am`

 * *Files 8% similar despite different names*

```diff
@@ -29,16 +29,18 @@
 DPKG_FILES = \
 	dpkg/changelog \
 	dpkg/changelog.in \
 	dpkg/compat \
 	dpkg/control \
 	dpkg/copyright \
 	dpkg/rules \
-	dpkg/libvsapm-dev.install \
 	dpkg/libvsapm.install \
+	dpkg/libvsapm-dev.install \
+	dpkg/libvsapm-python3.install \
+	dpkg/libvsapm-tools.install \
 	dpkg/source/format
 
 GETTEXT_FILES = \
 	config.rpath \
 	po/Makevars.in
 
 PKGCONFIG_FILES = \
```

### Comparing `libvsapm-20230430/aclocal.m4` & `libvsapm-20230506/aclocal.m4`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libbfio/libbfio_handle.h` & `libvsapm-20230506/libbfio/libbfio_handle.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libbfio/libbfio_libcerror.h` & `libvsapm-20230506/libbfio/libbfio_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libbfio/libbfio_handle.c` & `libvsapm-20230506/libbfio/libbfio_handle.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libbfio/libbfio_libuna.h` & `libvsapm-20230506/libbfio/libbfio_libuna.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libbfio/libbfio_definitions.h` & `libvsapm-20230506/libbfio/libbfio_definitions.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libbfio/libbfio_libclocale.h` & `libvsapm-20230506/libbfio/libbfio_libclocale.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libbfio/libbfio_codepage.h` & `libvsapm-20230506/libbfio/libbfio_codepage.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libbfio/libbfio_libcdata.h` & `libvsapm-20230506/libbfio/libbfio_libcdata.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libbfio/libbfio_extern.h` & `libvsapm-20230506/libbfio/libbfio_extern.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libbfio/libbfio_file_range.c` & `libvsapm-20230506/libbfio/libbfio_file_range.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libbfio/libbfio_file_range_io_handle.c` & `libvsapm-20230506/libbfio/libbfio_file_range_io_handle.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libbfio/Makefile.am` & `libvsapm-20230506/libbfio/Makefile.am`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libbfio/libbfio_file_pool.c` & `libvsapm-20230506/libbfio/libbfio_file_pool.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libbfio/libbfio_file.c` & `libvsapm-20230506/libbfio/libbfio_file.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libbfio/libbfio_pool.h` & `libvsapm-20230506/libbfio/libbfio_pool.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libbfio/libbfio_file_range.h` & `libvsapm-20230506/libbfio/libbfio_file_range.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libbfio/libbfio_system_string.h` & `libvsapm-20230506/libbfio/libbfio_system_string.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libbfio/libbfio_file_io_handle.h` & `libvsapm-20230506/libbfio/libbfio_file_io_handle.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libbfio/libbfio_memory_range_io_handle.c` & `libvsapm-20230506/libbfio/libbfio_memory_range_io_handle.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libbfio/libbfio_file.h` & `libvsapm-20230506/libbfio/libbfio_file.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libbfio/libbfio_support.c` & `libvsapm-20230506/libbfio/libbfio_support.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libbfio/libbfio_file_pool.h` & `libvsapm-20230506/libbfio/libbfio_file_pool.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libbfio/libbfio_memory_range_io_handle.h` & `libvsapm-20230506/libbfio/libbfio_memory_range_io_handle.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libbfio/libbfio_error.h` & `libvsapm-20230506/libbfio/libbfio_error.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libbfio/libbfio_libcthreads.h` & `libvsapm-20230506/libbfio/libbfio_libcthreads.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libbfio/libbfio_system_string.c` & `libvsapm-20230506/libbfio/libbfio_system_string.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libbfio/libbfio_memory_range.h` & `libvsapm-20230506/libbfio/libbfio_memory_range.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libbfio/libbfio_file_range_io_handle.h` & `libvsapm-20230506/libbfio/libbfio_file_range_io_handle.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libbfio/libbfio_memory_range.c` & `libvsapm-20230506/libbfio/libbfio_memory_range.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libbfio/Makefile.in` & `libvsapm-20230506/libbfio/Makefile.in`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libbfio/libbfio_pool.c` & `libvsapm-20230506/libbfio/libbfio_pool.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libbfio/libbfio_unused.h` & `libvsapm-20230506/libbfio/libbfio_unused.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libbfio/libbfio_libcpath.h` & `libvsapm-20230506/libbfio/libbfio_libcpath.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libbfio/libbfio_libcfile.h` & `libvsapm-20230506/libbfio/libbfio_libcfile.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libbfio/libbfio_support.h` & `libvsapm-20230506/libbfio/libbfio_support.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libbfio/libbfio_file_io_handle.c` & `libvsapm-20230506/libbfio/libbfio_file_io_handle.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libbfio/libbfio_error.c` & `libvsapm-20230506/libbfio/libbfio_error.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libbfio/libbfio_types.h` & `libvsapm-20230506/libbfio/libbfio_types.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/COPYING` & `libvsapm-20230506/COPYING`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libvsapm.pc.in` & `libvsapm-20230506/libvsapm.pc.in`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/include/libvsapm.h` & `libvsapm-20230506/include/libvsapm.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/include/libvsapm.h.in` & `libvsapm-20230506/include/libvsapm.h.in`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/include/Makefile.in` & `libvsapm-20230506/include/Makefile.in`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/include/libvsapm/definitions.h.in` & `libvsapm-20230506/include/libvsapm/definitions.h.in`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/include/libvsapm/extern.h` & `libvsapm-20230506/include/libvsapm/extern.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/include/libvsapm/types.h` & `libvsapm-20230506/include/libvsapm/types.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/include/libvsapm/features.h.in` & `libvsapm-20230506/include/libvsapm/features.h.in`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/include/libvsapm/types.h.in` & `libvsapm-20230506/include/libvsapm/types.h.in`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/include/libvsapm/features.h` & `libvsapm-20230506/include/libvsapm/features.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/include/libvsapm/definitions.h` & `libvsapm-20230506/include/libvsapm/definitions.h`

 * *Files 8% similar despite different names*

```diff
@@ -20,19 +20,19 @@
  */
 
 #if !defined( _LIBVSAPM_DEFINITIONS_H )
 #define _LIBVSAPM_DEFINITIONS_H
 
 #include <libvsapm/types.h>
 
-#define LIBVSAPM_VERSION		20230430
+#define LIBVSAPM_VERSION		20230506
 
 /* The version string
  */
-#define LIBVSAPM_VERSION_STRING		"20230430"
+#define LIBVSAPM_VERSION_STRING		"20230506"
 
 /* The byte order definitions
  */
 enum LIBVSAPM_ENDIAN
 {
 	LIBVSAPM_ENDIAN_BIG		= (int) 'b',
 	LIBVSAPM_ENDIAN_LITTLE		= (int) 'l',
```

### Comparing `libvsapm-20230430/include/libvsapm/codepage.h` & `libvsapm-20230506/include/libvsapm/codepage.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/include/libvsapm/error.h` & `libvsapm-20230506/include/libvsapm/error.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/install-sh` & `libvsapm-20230506/install-sh`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/INSTALL` & `libvsapm-20230506/INSTALL`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/dpkg/copyright` & `libvsapm-20230506/dpkg/copyright`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/dpkg/rules` & `libvsapm-20230506/dpkg/rules`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/dpkg/control` & `libvsapm-20230506/dpkg/control`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/pyvsapm-python2/Makefile.am` & `libvsapm-20230506/pyvsapm-python2/Makefile.am`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/pyvsapm-python2/Makefile.in` & `libvsapm-20230506/pyvsapm-python2/Makefile.in`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcfile/libcfile_file.c` & `libvsapm-20230506/libcfile/libcfile_file.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcfile/libcfile_libclocale.h` & `libvsapm-20230506/libcfile/libcfile_libclocale.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcfile/libcfile_support.c` & `libvsapm-20230506/libcfile/libcfile_support.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcfile/libcfile_support.h` & `libvsapm-20230506/libcfile/libcfile_support.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcfile/libcfile_error.c` & `libvsapm-20230506/libcfile/libcfile_error.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcfile/libcfile_winapi.c` & `libvsapm-20230506/libcfile/libcfile_winapi.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcfile/Makefile.am` & `libvsapm-20230506/libcfile/Makefile.am`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcfile/libcfile_libcerror.h` & `libvsapm-20230506/libcfile/libcfile_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcfile/libcfile_unused.h` & `libvsapm-20230506/libcfile/libcfile_unused.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcfile/libcfile_winapi.h` & `libvsapm-20230506/libcfile/libcfile_winapi.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcfile/libcfile_types.h` & `libvsapm-20230506/libcfile/libcfile_types.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcfile/libcfile_extern.h` & `libvsapm-20230506/libcfile/libcfile_extern.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcfile/libcfile_notify.h` & `libvsapm-20230506/libcfile/libcfile_notify.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcfile/libcfile_definitions.h` & `libvsapm-20230506/libcfile/libcfile_definitions.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcfile/libcfile_file.h` & `libvsapm-20230506/libcfile/libcfile_file.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcfile/libcfile_error.h` & `libvsapm-20230506/libcfile/libcfile_error.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcfile/libcfile_system_string.c` & `libvsapm-20230506/libcfile/libcfile_system_string.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcfile/Makefile.in` & `libvsapm-20230506/libcfile/Makefile.in`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcfile/libcfile_system_string.h` & `libvsapm-20230506/libcfile/libcfile_system_string.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcfile/libcfile_libcnotify.h` & `libvsapm-20230506/libcfile/libcfile_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcfile/libcfile_libuna.h` & `libvsapm-20230506/libcfile/libcfile_libuna.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcfile/libcfile_notify.c` & `libvsapm-20230506/libcfile/libcfile_notify.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libvsapm.spec.in` & `libvsapm-20230506/libvsapm.spec.in`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcthreads/libcthreads_thread_pool.h` & `libvsapm-20230506/libcthreads/libcthreads_thread_pool.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcthreads/libcthreads_thread_pool.c` & `libvsapm-20230506/libcthreads/libcthreads_thread_pool.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcthreads/libcthreads_repeating_thread.c` & `libvsapm-20230506/libcthreads/libcthreads_repeating_thread.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcthreads/libcthreads_error.c` & `libvsapm-20230506/libcthreads/libcthreads_error.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcthreads/Makefile.am` & `libvsapm-20230506/libcthreads/Makefile.am`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcthreads/libcthreads_unused.h` & `libvsapm-20230506/libcthreads/libcthreads_unused.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcthreads/libcthreads_condition.h` & `libvsapm-20230506/libcthreads/libcthreads_condition.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcthreads/libcthreads_definitions.h` & `libvsapm-20230506/libcthreads/libcthreads_definitions.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcthreads/libcthreads_thread.h` & `libvsapm-20230506/libcthreads/libcthreads_thread.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcthreads/libcthreads_repeating_thread.h` & `libvsapm-20230506/libcthreads/libcthreads_repeating_thread.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcthreads/libcthreads_read_write_lock.c` & `libvsapm-20230506/libcthreads/libcthreads_read_write_lock.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcthreads/libcthreads_mutex.h` & `libvsapm-20230506/libcthreads/libcthreads_mutex.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcthreads/libcthreads_support.h` & `libvsapm-20230506/libcthreads/libcthreads_support.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcthreads/libcthreads_thread.c` & `libvsapm-20230506/libcthreads/libcthreads_thread.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcthreads/libcthreads_mutex.c` & `libvsapm-20230506/libcthreads/libcthreads_mutex.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcthreads/libcthreads_types.h` & `libvsapm-20230506/libcthreads/libcthreads_types.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcthreads/libcthreads_lock.h` & `libvsapm-20230506/libcthreads/libcthreads_lock.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcthreads/libcthreads_extern.h` & `libvsapm-20230506/libcthreads/libcthreads_extern.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcthreads/libcthreads_error.h` & `libvsapm-20230506/libcthreads/libcthreads_error.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcthreads/libcthreads_queue.c` & `libvsapm-20230506/libcthreads/libcthreads_queue.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcthreads/libcthreads_condition.c` & `libvsapm-20230506/libcthreads/libcthreads_condition.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcthreads/Makefile.in` & `libvsapm-20230506/libcthreads/Makefile.in`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcthreads/libcthreads_thread_attributes.c` & `libvsapm-20230506/libcthreads/libcthreads_thread_attributes.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcthreads/libcthreads_libcerror.h` & `libvsapm-20230506/libcthreads/libcthreads_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcthreads/libcthreads_lock.c` & `libvsapm-20230506/libcthreads/libcthreads_lock.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcthreads/libcthreads_support.c` & `libvsapm-20230506/libcthreads/libcthreads_support.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcthreads/libcthreads_read_write_lock.h` & `libvsapm-20230506/libcthreads/libcthreads_read_write_lock.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcthreads/libcthreads_thread_attributes.h` & `libvsapm-20230506/libcthreads/libcthreads_thread_attributes.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcthreads/libcthreads_queue.h` & `libvsapm-20230506/libcthreads/libcthreads_queue.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/config.sub` & `libvsapm-20230506/config.sub`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcpath/libcpath_unused.h` & `libvsapm-20230506/libcpath/libcpath_unused.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcpath/libcpath_support.c` & `libvsapm-20230506/libcpath/libcpath_support.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcpath/libcpath_libclocale.h` & `libvsapm-20230506/libcpath/libcpath_libclocale.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcpath/Makefile.am` & `libvsapm-20230506/libcpath/Makefile.am`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcpath/libcpath_error.h` & `libvsapm-20230506/libcpath/libcpath_error.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcpath/libcpath_system_string.h` & `libvsapm-20230506/libcpath/libcpath_system_string.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcpath/libcpath_error.c` & `libvsapm-20230506/libcpath/libcpath_error.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcpath/libcpath_libcsplit.h` & `libvsapm-20230506/libcpath/libcpath_libcsplit.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcpath/libcpath_path.h` & `libvsapm-20230506/libcpath/libcpath_path.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcpath/Makefile.in` & `libvsapm-20230506/libcpath/Makefile.in`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcpath/libcpath_definitions.h` & `libvsapm-20230506/libcpath/libcpath_definitions.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcpath/libcpath_libcerror.h` & `libvsapm-20230506/libcpath/libcpath_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcpath/libcpath_extern.h` & `libvsapm-20230506/libcpath/libcpath_extern.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcpath/libcpath_path.c` & `libvsapm-20230506/libcpath/libcpath_path.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcpath/libcpath_system_string.c` & `libvsapm-20230506/libcpath/libcpath_system_string.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcpath/libcpath_support.h` & `libvsapm-20230506/libcpath/libcpath_support.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcpath/libcpath_libuna.h` & `libvsapm-20230506/libcpath/libcpath_libuna.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/manuals/vsapminfo.1` & `libvsapm-20230506/manuals/vsapminfo.1`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/manuals/Makefile.in` & `libvsapm-20230506/manuals/Makefile.in`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/manuals/libvsapm.3` & `libvsapm-20230506/manuals/libvsapm.3`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/msvscpp/vsapm_test_volume/vsapm_test_volume.vcproj` & `libvsapm-20230506/msvscpp/vsapm_test_volume/vsapm_test_volume.vcproj`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/msvscpp/vsapm_test_partition/vsapm_test_partition.vcproj` & `libvsapm-20230506/msvscpp/vsapm_test_partition/vsapm_test_partition.vcproj`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/msvscpp/libfcache/libfcache.vcproj` & `libvsapm-20230506/msvscpp/libfcache/libfcache.vcproj`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/msvscpp/vsapm_test_io_handle/vsapm_test_io_handle.vcproj` & `libvsapm-20230506/msvscpp/vsapm_test_io_handle/vsapm_test_io_handle.vcproj`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/msvscpp/vsapm_test_tools_info_handle/vsapm_test_tools_info_handle.vcproj` & `libvsapm-20230506/msvscpp/vsapm_test_tools_info_handle/vsapm_test_tools_info_handle.vcproj`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/msvscpp/libclocale/libclocale.vcproj` & `libvsapm-20230506/msvscpp/libclocale/libclocale.vcproj`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/msvscpp/Makefile.am` & `libvsapm-20230506/msvscpp/Makefile.am`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/msvscpp/libbfio/libbfio.vcproj` & `libvsapm-20230506/msvscpp/libbfio/libbfio.vcproj`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/msvscpp/libvsapm.sln` & `libvsapm-20230506/msvscpp/libvsapm.sln`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/msvscpp/libcfile/libcfile.vcproj` & `libvsapm-20230506/msvscpp/libcfile/libcfile.vcproj`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/msvscpp/libcthreads/libcthreads.vcproj` & `libvsapm-20230506/msvscpp/libcthreads/libcthreads.vcproj`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/msvscpp/vsapm_test_error/vsapm_test_error.vcproj` & `libvsapm-20230506/msvscpp/vsapm_test_error/vsapm_test_error.vcproj`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/msvscpp/libcpath/libcpath.vcproj` & `libvsapm-20230506/msvscpp/libcpath/libcpath.vcproj`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/msvscpp/vsapm_test_sector_data/vsapm_test_sector_data.vcproj` & `libvsapm-20230506/msvscpp/vsapm_test_sector_data/vsapm_test_sector_data.vcproj`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/msvscpp/vsapminfo/vsapminfo.vcproj` & `libvsapm-20230506/msvscpp/vsapminfo/vsapminfo.vcproj`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/msvscpp/libuna/libuna.vcproj` & `libvsapm-20230506/msvscpp/libuna/libuna.vcproj`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/msvscpp/Makefile.in` & `libvsapm-20230506/msvscpp/Makefile.in`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/msvscpp/libvsapm/libvsapm.vcproj` & `libvsapm-20230506/msvscpp/libvsapm/libvsapm.vcproj`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/msvscpp/libcerror/libcerror.vcproj` & `libvsapm-20230506/msvscpp/libcerror/libcerror.vcproj`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/msvscpp/libcnotify/libcnotify.vcproj` & `libvsapm-20230506/msvscpp/libcnotify/libcnotify.vcproj`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/msvscpp/vsapm_test_notify/vsapm_test_notify.vcproj` & `libvsapm-20230506/msvscpp/vsapm_test_notify/vsapm_test_notify.vcproj`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/msvscpp/vsapm_test_tools_output/vsapm_test_tools_output.vcproj` & `libvsapm-20230506/msvscpp/vsapm_test_tools_output/vsapm_test_tools_output.vcproj`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/msvscpp/vsapm_test_support/vsapm_test_support.vcproj` & `libvsapm-20230506/msvscpp/vsapm_test_support/vsapm_test_support.vcproj`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/msvscpp/libfdata/libfdata.vcproj` & `libvsapm-20230506/msvscpp/libfdata/libfdata.vcproj`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/msvscpp/libcdata/libcdata.vcproj` & `libvsapm-20230506/msvscpp/libcdata/libcdata.vcproj`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/msvscpp/vsapm_test_tools_signal/vsapm_test_tools_signal.vcproj` & `libvsapm-20230506/msvscpp/vsapm_test_tools_signal/vsapm_test_tools_signal.vcproj`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/msvscpp/pyvsapm/pyvsapm.vcproj` & `libvsapm-20230506/msvscpp/pyvsapm/pyvsapm.vcproj`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/msvscpp/libcsplit/libcsplit.vcproj` & `libvsapm-20230506/msvscpp/libcsplit/libcsplit.vcproj`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/msvscpp/vsapm_test_partition_map_entry/vsapm_test_partition_map_entry.vcproj` & `libvsapm-20230506/msvscpp/vsapm_test_partition_map_entry/vsapm_test_partition_map_entry.vcproj`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/setup.py` & `libvsapm-20230506/setup.py`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/config.guess` & `libvsapm-20230506/config.guess`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/ossfuzz/Makefile.am` & `libvsapm-20230506/ossfuzz/Makefile.am`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/ossfuzz/partition_fuzzer.cc` & `libvsapm-20230506/ossfuzz/partition_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/ossfuzz/volume_fuzzer.cc` & `libvsapm-20230506/ossfuzz/volume_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/ossfuzz/Makefile.in` & `libvsapm-20230506/ossfuzz/Makefile.in`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/ossfuzz/ossfuzz_libvsapm.h` & `libvsapm-20230506/ossfuzz/ossfuzz_libvsapm.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/ossfuzz/ossfuzz_libbfio.h` & `libvsapm-20230506/ossfuzz/ossfuzz_libbfio.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/test-driver` & `libvsapm-20230506/test-driver`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/configure` & `libvsapm-20230506/configure`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #! /bin/sh
 # Guess values for system-dependent variables and create Makefiles.
-# Generated by GNU Autoconf 2.71 for libvsapm 20230430.
+# Generated by GNU Autoconf 2.71 for libvsapm 20230506.
 #
 # Report bugs to <joachim.metz@gmail.com>.
 #
 #
 # Copyright (C) 1992-1996, 1998-2017, 2020-2021 Free Software Foundation,
 # Inc.
 #
@@ -617,16 +617,16 @@
 subdirs=
 MFLAGS=
 MAKEFLAGS=
 
 # Identity of this package.
 PACKAGE_NAME='libvsapm'
 PACKAGE_TARNAME='libvsapm'
-PACKAGE_VERSION='20230430'
-PACKAGE_STRING='libvsapm 20230430'
+PACKAGE_VERSION='20230506'
+PACKAGE_STRING='libvsapm 20230506'
 PACKAGE_BUGREPORT='joachim.metz@gmail.com'
 PACKAGE_URL=''
 
 ac_unique_file="include/libvsapm.h.in"
 # Factoring default headers for most tests.
 ac_includes_default="\
 #include <stddef.h>
@@ -1643,15 +1643,15 @@
 #
 # Report the --help message.
 #
 if test "$ac_init_help" = "long"; then
   # Omit some internal or obsolete options to make the list less imposing.
   # This message is too long to be a string in the A/UX 3.1 sh.
   cat <<_ACEOF
-\`configure' configures libvsapm 20230430 to adapt to many kinds of systems.
+\`configure' configures libvsapm 20230506 to adapt to many kinds of systems.
 
 Usage: $0 [OPTION]... [VAR=VALUE]...
 
 To assign environment variables (e.g., CC, CFLAGS...), specify them as
 VAR=VALUE.  See below for descriptions of some of the useful variables.
 
 Defaults for the options are specified in brackets.
@@ -1714,15 +1714,15 @@
   --build=BUILD     configure for building on BUILD [guessed]
   --host=HOST       cross-compile to build programs to run on HOST [BUILD]
 _ACEOF
 fi
 
 if test -n "$ac_init_help"; then
   case $ac_init_help in
-     short | recursive ) echo "Configuration of libvsapm 20230430:";;
+     short | recursive ) echo "Configuration of libvsapm 20230506:";;
    esac
   cat <<\_ACEOF
 
 Optional Features:
   --disable-option-checking  ignore unrecognized --enable/--with options
   --disable-FEATURE       do not include FEATURE (same as --enable-FEATURE=no)
   --enable-FEATURE[=ARG]  include FEATURE [ARG=yes]
@@ -1950,15 +1950,15 @@
     cd "$ac_pwd" || { ac_status=$?; break; }
   done
 fi
 
 test -n "$ac_init_help" && exit $ac_status
 if $ac_init_version; then
   cat <<\_ACEOF
-libvsapm configure 20230430
+libvsapm configure 20230506
 generated by GNU Autoconf 2.71
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This configure script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it.
 _ACEOF
   exit
@@ -2671,15 +2671,15 @@
     ac_configure_args_raw=`      printf "%s\n" "$ac_configure_args_raw" | sed "$ac_safe_unquote"`;;
 esac
 
 cat >config.log <<_ACEOF
 This file contains any messages produced by compilers while
 running configure, to aid debugging if configure makes a mistake.
 
-It was created by libvsapm $as_me 20230430, which was
+It was created by libvsapm $as_me 20230506, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   $ $0$ac_configure_args_raw
 
 _ACEOF
 exec 5>>config.log
 {
@@ -4160,15 +4160,15 @@
     CYGPATH_W=echo
   fi
 fi
 
 
 # Define the identity of the package.
  PACKAGE='libvsapm'
- VERSION='20230430'
+ VERSION='20230506'
 
 
 printf "%s\n" "#define PACKAGE \"$PACKAGE\"" >>confdefs.h
 
 
 printf "%s\n" "#define VERSION \"$VERSION\"" >>confdefs.h
 
@@ -49954,15 +49954,15 @@
 test $as_write_fail = 0 && chmod +x $CONFIG_STATUS || ac_write_fail=1
 
 cat >>$CONFIG_STATUS <<\_ACEOF || ac_write_fail=1
 # Save the log message, to keep $0 and so on meaningful, and to
 # report actual input values of CONFIG_FILES etc. instead of their
 # values after options handling.
 ac_log="
-This file was extended by libvsapm $as_me 20230430, which was
+This file was extended by libvsapm $as_me 20230506, which was
 generated by GNU Autoconf 2.71.  Invocation command line was
 
   CONFIG_FILES    = $CONFIG_FILES
   CONFIG_HEADERS  = $CONFIG_HEADERS
   CONFIG_LINKS    = $CONFIG_LINKS
   CONFIG_COMMANDS = $CONFIG_COMMANDS
   $ $0 $@
@@ -50022,15 +50022,15 @@
 
 _ACEOF
 ac_cs_config=`printf "%s\n" "$ac_configure_args" | sed "$ac_safe_unquote"`
 ac_cs_config_escaped=`printf "%s\n" "$ac_cs_config" | sed "s/^ //; s/'/'\\\\\\\\''/g"`
 cat >>$CONFIG_STATUS <<_ACEOF || ac_write_fail=1
 ac_cs_config='$ac_cs_config_escaped'
 ac_cs_version="\\
-libvsapm config.status 20230430
+libvsapm config.status 20230506
 configured by $0, generated by GNU Autoconf 2.71,
   with options \\"\$ac_cs_config\\"
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This config.status script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it."
```

### Comparing `libvsapm-20230430/libuna/libuna_url_stream.c` & `libvsapm-20230506/libuna/libuna_url_stream.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_mac_symbol.h` & `libvsapm-20230506/libuna/libuna_codepage_mac_symbol.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_support.c` & `libvsapm-20230506/libuna/libuna_support.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_scsu.h` & `libvsapm-20230506/libuna/libuna_scsu.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_iso_8859_5.c` & `libvsapm-20230506/libuna/libuna_codepage_iso_8859_5.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_iso_8859_2.c` & `libvsapm-20230506/libuna/libuna_codepage_iso_8859_2.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_windows_1253.c` & `libvsapm-20230506/libuna/libuna_codepage_windows_1253.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_koi8_u.h` & `libvsapm-20230506/libuna/libuna_codepage_koi8_u.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_windows_1252.c` & `libvsapm-20230506/libuna/libuna_codepage_windows_1252.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_utf32_stream.c` & `libvsapm-20230506/libuna/libuna_utf32_stream.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_windows_1257.h` & `libvsapm-20230506/libuna/libuna_codepage_windows_1257.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_mac_cyrillic.c` & `libvsapm-20230506/libuna/libuna_codepage_mac_cyrillic.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_mac_thai.c` & `libvsapm-20230506/libuna/libuna_codepage_mac_thai.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_utf32_string.c` & `libvsapm-20230506/libuna/libuna_utf32_string.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_mac_thai.h` & `libvsapm-20230506/libuna/libuna_codepage_mac_thai.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_windows_874.c` & `libvsapm-20230506/libuna/libuna_codepage_windows_874.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_windows_1251.h` & `libvsapm-20230506/libuna/libuna_codepage_windows_1251.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_libcerror.h` & `libvsapm-20230506/libuna/libuna_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_windows_949.c` & `libvsapm-20230506/libuna/libuna_codepage_windows_949.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_iso_8859_6.h` & `libvsapm-20230506/libuna/libuna_codepage_iso_8859_6.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_windows_1256.h` & `libvsapm-20230506/libuna/libuna_codepage_windows_1256.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_mac_greek.h` & `libvsapm-20230506/libuna/libuna_codepage_mac_greek.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_mac_russian.h` & `libvsapm-20230506/libuna/libuna_codepage_mac_russian.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_mac_ukrainian.h` & `libvsapm-20230506/libuna/libuna_codepage_mac_ukrainian.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_iso_8859_6.c` & `libvsapm-20230506/libuna/libuna_codepage_iso_8859_6.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_windows_874.h` & `libvsapm-20230506/libuna/libuna_codepage_windows_874.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_windows_1251.c` & `libvsapm-20230506/libuna/libuna_codepage_windows_1251.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_windows_1256.c` & `libvsapm-20230506/libuna/libuna_codepage_windows_1256.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_base16_stream.h` & `libvsapm-20230506/libuna/libuna_base16_stream.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_iso_8859_2.h` & `libvsapm-20230506/libuna/libuna_codepage_iso_8859_2.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/Makefile.am` & `libvsapm-20230506/libuna/Makefile.am`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_windows_1257.c` & `libvsapm-20230506/libuna/libuna_codepage_windows_1257.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_windows_1254.h` & `libvsapm-20230506/libuna/libuna_codepage_windows_1254.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_windows_1255.c` & `libvsapm-20230506/libuna/libuna_codepage_windows_1255.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_unused.h` & `libvsapm-20230506/libuna/libuna_unused.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_windows_1253.h` & `libvsapm-20230506/libuna/libuna_codepage_windows_1253.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_unicode_character.h` & `libvsapm-20230506/libuna/libuna_unicode_character.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_mac_dingbats.h` & `libvsapm-20230506/libuna/libuna_codepage_mac_dingbats.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_scsu.c` & `libvsapm-20230506/libuna/libuna_scsu.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_byte_stream.c` & `libvsapm-20230506/libuna/libuna_byte_stream.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_mac_celtic.h` & `libvsapm-20230506/libuna/libuna_codepage_mac_celtic.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_mac_croatian.c` & `libvsapm-20230506/libuna/libuna_codepage_mac_croatian.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_iso_8859_3.h` & `libvsapm-20230506/libuna/libuna_codepage_iso_8859_3.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_iso_8859_15.h` & `libvsapm-20230506/libuna/libuna_codepage_iso_8859_15.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_mac_roman.c` & `libvsapm-20230506/libuna/libuna_codepage_mac_roman.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_utf32_string.h` & `libvsapm-20230506/libuna/libuna_utf32_string.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_koi8_r.c` & `libvsapm-20230506/libuna/libuna_codepage_koi8_r.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_mac_icelandic.c` & `libvsapm-20230506/libuna/libuna_codepage_mac_icelandic.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_windows_936.h` & `libvsapm-20230506/libuna/libuna_codepage_windows_936.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_base64_stream.h` & `libvsapm-20230506/libuna/libuna_base64_stream.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_mac_celtic.c` & `libvsapm-20230506/libuna/libuna_codepage_mac_celtic.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_windows_950.c` & `libvsapm-20230506/libuna/libuna_codepage_windows_950.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_utf8_string.h` & `libvsapm-20230506/libuna/libuna_utf8_string.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_windows_936.c` & `libvsapm-20230506/libuna/libuna_codepage_windows_936.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_unicode_character.c` & `libvsapm-20230506/libuna/libuna_unicode_character.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_utf8_string.c` & `libvsapm-20230506/libuna/libuna_utf8_string.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_base32_stream.c` & `libvsapm-20230506/libuna/libuna_base32_stream.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_windows_950.h` & `libvsapm-20230506/libuna/libuna_codepage_windows_950.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_error.h` & `libvsapm-20230506/libuna/libuna_error.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_windows_932.h` & `libvsapm-20230506/libuna/libuna_codepage_windows_932.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_mac_turkish.h` & `libvsapm-20230506/libuna/libuna_codepage_mac_turkish.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_utf8_stream.c` & `libvsapm-20230506/libuna/libuna_utf8_stream.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_mac_ukrainian.c` & `libvsapm-20230506/libuna/libuna_codepage_mac_ukrainian.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_koi8_r.h` & `libvsapm-20230506/libuna/libuna_codepage_koi8_r.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_base16_stream.c` & `libvsapm-20230506/libuna/libuna_base16_stream.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_windows_1250.h` & `libvsapm-20230506/libuna/libuna_codepage_windows_1250.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_iso_8859_16.h` & `libvsapm-20230506/libuna/libuna_codepage_iso_8859_16.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_mac_croatian.h` & `libvsapm-20230506/libuna/libuna_codepage_mac_croatian.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_mac_gaelic.c` & `libvsapm-20230506/libuna/libuna_codepage_mac_gaelic.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_utf16_stream.h` & `libvsapm-20230506/libuna/libuna_utf16_stream.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_iso_8859_10.h` & `libvsapm-20230506/libuna/libuna_codepage_iso_8859_10.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_mac_centraleurroman.c` & `libvsapm-20230506/libuna/libuna_codepage_mac_centraleurroman.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_windows_932.c` & `libvsapm-20230506/libuna/libuna_codepage_windows_932.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_utf8_stream.h` & `libvsapm-20230506/libuna/libuna_utf8_stream.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_url_stream.h` & `libvsapm-20230506/libuna/libuna_url_stream.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_mac_farsi.c` & `libvsapm-20230506/libuna/libuna_codepage_mac_farsi.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_windows_949.h` & `libvsapm-20230506/libuna/libuna_codepage_windows_949.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_mac_romanian.h` & `libvsapm-20230506/libuna/libuna_codepage_mac_romanian.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_mac_gaelic.h` & `libvsapm-20230506/libuna/libuna_codepage_mac_gaelic.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_iso_8859_8.c` & `libvsapm-20230506/libuna/libuna_codepage_iso_8859_8.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_types.h` & `libvsapm-20230506/libuna/libuna_types.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_mac_arabic.c` & `libvsapm-20230506/libuna/libuna_codepage_mac_arabic.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_windows_1252.h` & `libvsapm-20230506/libuna/libuna_codepage_windows_1252.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_windows_1250.c` & `libvsapm-20230506/libuna/libuna_codepage_windows_1250.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_mac_russian.c` & `libvsapm-20230506/libuna/libuna_codepage_mac_russian.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_utf16_string.c` & `libvsapm-20230506/libuna/libuna_utf16_string.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_iso_8859_5.h` & `libvsapm-20230506/libuna/libuna_codepage_iso_8859_5.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_extern.h` & `libvsapm-20230506/libuna/libuna_extern.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_iso_8859_4.h` & `libvsapm-20230506/libuna/libuna_codepage_iso_8859_4.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_byte_stream.h` & `libvsapm-20230506/libuna/libuna_byte_stream.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_mac_roman.h` & `libvsapm-20230506/libuna/libuna_codepage_mac_roman.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_utf16_string.h` & `libvsapm-20230506/libuna/libuna_utf16_string.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_iso_8859_4.c` & `libvsapm-20230506/libuna/libuna_codepage_iso_8859_4.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_iso_8859_10.c` & `libvsapm-20230506/libuna/libuna_codepage_iso_8859_10.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_mac_icelandic.h` & `libvsapm-20230506/libuna/libuna_codepage_mac_icelandic.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/Makefile.in` & `libvsapm-20230506/libuna/Makefile.in`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_utf7_stream.h` & `libvsapm-20230506/libuna/libuna_utf7_stream.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_mac_symbol.c` & `libvsapm-20230506/libuna/libuna_codepage_mac_symbol.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_base32_stream.h` & `libvsapm-20230506/libuna/libuna_base32_stream.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_mac_turkish.c` & `libvsapm-20230506/libuna/libuna_codepage_mac_turkish.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_mac_inuit.c` & `libvsapm-20230506/libuna/libuna_codepage_mac_inuit.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_utf16_stream.c` & `libvsapm-20230506/libuna/libuna_utf16_stream.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_utf7_stream.c` & `libvsapm-20230506/libuna/libuna_utf7_stream.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_support.h` & `libvsapm-20230506/libuna/libuna_support.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_utf32_stream.h` & `libvsapm-20230506/libuna/libuna_utf32_stream.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_iso_8859_3.c` & `libvsapm-20230506/libuna/libuna_codepage_iso_8859_3.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_mac_greek.c` & `libvsapm-20230506/libuna/libuna_codepage_mac_greek.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_definitions.h` & `libvsapm-20230506/libuna/libuna_definitions.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_windows_1255.h` & `libvsapm-20230506/libuna/libuna_codepage_windows_1255.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_iso_8859_14.c` & `libvsapm-20230506/libuna/libuna_codepage_iso_8859_14.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_iso_8859_13.c` & `libvsapm-20230506/libuna/libuna_codepage_iso_8859_13.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_mac_centraleurroman.h` & `libvsapm-20230506/libuna/libuna_codepage_mac_centraleurroman.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_iso_8859_8.h` & `libvsapm-20230506/libuna/libuna_codepage_iso_8859_8.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_iso_8859_9.c` & `libvsapm-20230506/libuna/libuna_codepage_iso_8859_9.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_windows_1254.c` & `libvsapm-20230506/libuna/libuna_codepage_windows_1254.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_mac_cyrillic.h` & `libvsapm-20230506/libuna/libuna_codepage_mac_cyrillic.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_mac_arabic.h` & `libvsapm-20230506/libuna/libuna_codepage_mac_arabic.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_windows_1258.c` & `libvsapm-20230506/libuna/libuna_codepage_windows_1258.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_mac_farsi.h` & `libvsapm-20230506/libuna/libuna_codepage_mac_farsi.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_iso_8859_15.c` & `libvsapm-20230506/libuna/libuna_codepage_iso_8859_15.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_iso_8859_7.c` & `libvsapm-20230506/libuna/libuna_codepage_iso_8859_7.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_mac_dingbats.c` & `libvsapm-20230506/libuna/libuna_codepage_mac_dingbats.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_iso_8859_9.h` & `libvsapm-20230506/libuna/libuna_codepage_iso_8859_9.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_windows_1258.h` & `libvsapm-20230506/libuna/libuna_codepage_windows_1258.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_base64_stream.c` & `libvsapm-20230506/libuna/libuna_base64_stream.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_mac_romanian.c` & `libvsapm-20230506/libuna/libuna_codepage_mac_romanian.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_error.c` & `libvsapm-20230506/libuna/libuna_error.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_koi8_u.c` & `libvsapm-20230506/libuna/libuna_codepage_koi8_u.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_iso_8859_13.h` & `libvsapm-20230506/libuna/libuna_codepage_iso_8859_13.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_iso_8859_7.h` & `libvsapm-20230506/libuna/libuna_codepage_iso_8859_7.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_iso_8859_14.h` & `libvsapm-20230506/libuna/libuna_codepage_iso_8859_14.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_mac_inuit.h` & `libvsapm-20230506/libuna/libuna_codepage_mac_inuit.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libuna/libuna_codepage_iso_8859_16.c` & `libvsapm-20230506/libuna/libuna_codepage_iso_8859_16.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/Makefile.in` & `libvsapm-20230506/Makefile.in`

 * *Files 1% similar despite different names*

```diff
@@ -598,16 +598,18 @@
 DPKG_FILES = \
 	dpkg/changelog \
 	dpkg/changelog.in \
 	dpkg/compat \
 	dpkg/control \
 	dpkg/copyright \
 	dpkg/rules \
-	dpkg/libvsapm-dev.install \
 	dpkg/libvsapm.install \
+	dpkg/libvsapm-dev.install \
+	dpkg/libvsapm-python3.install \
+	dpkg/libvsapm-tools.install \
 	dpkg/source/format
 
 GETTEXT_FILES = \
 	config.rpath \
 	po/Makevars.in
 
 PKGCONFIG_FILES = \
```

### Comparing `libvsapm-20230430/libvsapm/libvsapm_libcnotify.h` & `libvsapm-20230506/libvsapm/libvsapm_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libvsapm/libvsapm_libcthreads.h` & `libvsapm-20230506/libvsapm/libvsapm_libcthreads.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libvsapm/libvsapm.rc` & `libvsapm-20230506/libvsapm/libvsapm.rc`

 * *Files 10% similar despite different names*

```diff
@@ -18,20 +18,20 @@
   FILESUBTYPE				0x0L
 BEGIN
   BLOCK "StringFileInfo"
   BEGIN
     BLOCK "040904E4"
     BEGIN
       VALUE "FileDescription",		"Library to access the Apple Partition Map (APM) volume system format\0"
-      VALUE "FileVersion",		"20230430" "\0"
+      VALUE "FileVersion",		"20230506" "\0"
       VALUE "InternalName",		"libvsapm.dll\0"
       VALUE "LegalCopyright",		"(C) 2009-2023, Joachim Metz <joachim.metz@gmail.com>\0"
       VALUE "OriginalFilename",		"libvsapm.dll\0"
       VALUE "ProductName",		"libvsapm\0"
-      VALUE "ProductVersion",		"20230430" "\0"
+      VALUE "ProductVersion",		"20230506" "\0"
       VALUE "Comments",			"For more information visit https://github.com/libyal/libvsapm/\0"
     END
   END
   BLOCK "VarFileInfo"
   BEGIN
     VALUE "Translation", 0x0409, 1200
   END
```

### Comparing `libvsapm-20230430/libvsapm/libvsapm_sector_data.c` & `libvsapm-20230506/libvsapm/libvsapm_sector_data.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libvsapm/libvsapm_error.h` & `libvsapm-20230506/libvsapm/libvsapm_error.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libvsapm/vsapm_partition_map_entry.h` & `libvsapm-20230506/libvsapm/vsapm_partition_map_entry.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libvsapm/libvsapm_libclocale.h` & `libvsapm-20230506/libvsapm/libvsapm_libclocale.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libvsapm/Makefile.am` & `libvsapm-20230506/libvsapm/Makefile.am`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libvsapm/libvsapm_libbfio.h` & `libvsapm-20230506/libvsapm/libvsapm_libbfio.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libvsapm/libvsapm_support.h` & `libvsapm-20230506/libvsapm/libvsapm_support.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libvsapm/libvsapm_libfdata.h` & `libvsapm-20230506/libvsapm/libvsapm_libfdata.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libvsapm/libvsapm_partition.c` & `libvsapm-20230506/libvsapm/libvsapm_partition.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libvsapm/libvsapm_notify.c` & `libvsapm-20230506/libvsapm/libvsapm_notify.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libvsapm/libvsapm_debug.h` & `libvsapm-20230506/libvsapm/libvsapm_debug.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libvsapm/libvsapm_unused.h` & `libvsapm-20230506/libvsapm/libvsapm_unused.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libvsapm/libvsapm_io_handle.c` & `libvsapm-20230506/libvsapm/libvsapm_io_handle.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libvsapm/libvsapm_definitions.h.in` & `libvsapm-20230506/libvsapm/libvsapm_definitions.h.in`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libvsapm/libvsapm_extern.h` & `libvsapm-20230506/libvsapm/libvsapm_extern.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libvsapm/libvsapm.rc.in` & `libvsapm-20230506/libvsapm/libvsapm.rc.in`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libvsapm/libvsapm_debug.c` & `libvsapm-20230506/libvsapm/libvsapm_debug.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libvsapm/libvsapm_support.c` & `libvsapm-20230506/libvsapm/libvsapm_support.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libvsapm/libvsapm_partition_map_entry.h` & `libvsapm-20230506/libvsapm/libvsapm_partition_map_entry.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libvsapm/libvsapm_definitions.h` & `libvsapm-20230506/libvsapm/libvsapm_definitions.h`

 * *Files 4% similar despite different names*

```diff
@@ -29,19 +29,19 @@
 #if !defined( HAVE_LOCAL_LIBVSAPM )
 #include <libvsapm/definitions.h>
 
 /* The definitions in <libvsapm/definitions.h> are copied here
  * for local use of libvsapm
  */
 #else
-#define LIBVSAPM_VERSION			20230430
+#define LIBVSAPM_VERSION			20230506
 
 /* The libvsapm version string
  */
-#define LIBVSAPM_VERSION_STRING			"20230430"
+#define LIBVSAPM_VERSION_STRING			"20230506"
 
 /* The endian definitions
  */
 #define LIBVSAPM_ENDIAN_BIG			_BYTE_STREAM_ENDIAN_BIG
 #define LIBVSAPM_ENDIAN_LITTLE			_BYTE_STREAM_ENDIAN_LITTLE
 
 /* The access flags definitions
```

### Comparing `libvsapm-20230430/libvsapm/libvsapm_partition.h` & `libvsapm-20230506/libvsapm/libvsapm_partition.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libvsapm/libvsapm_libfcache.h` & `libvsapm-20230506/libvsapm/libvsapm_libfcache.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libvsapm/Makefile.in` & `libvsapm-20230506/libvsapm/Makefile.in`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libvsapm/libvsapm_libcerror.h` & `libvsapm-20230506/libvsapm/libvsapm_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libvsapm/libvsapm_io_handle.h` & `libvsapm-20230506/libvsapm/libvsapm_io_handle.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libvsapm/libvsapm_volume.h` & `libvsapm-20230506/libvsapm/libvsapm_volume.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libvsapm/libvsapm_notify.h` & `libvsapm-20230506/libvsapm/libvsapm_notify.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libvsapm/libvsapm_error.c` & `libvsapm-20230506/libvsapm/libvsapm_error.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libvsapm/libvsapm.c` & `libvsapm-20230506/libvsapm/libvsapm.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libvsapm/libvsapm_types.h` & `libvsapm-20230506/libvsapm/libvsapm_types.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libvsapm/libvsapm_libcdata.h` & `libvsapm-20230506/libvsapm/libvsapm_libcdata.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libvsapm/libvsapm_sector_data.h` & `libvsapm-20230506/libvsapm/libvsapm_sector_data.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libvsapm/libvsapm_volume.c` & `libvsapm-20230506/libvsapm/libvsapm_volume.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libvsapm/libvsapm_partition_map_entry.c` & `libvsapm-20230506/libvsapm/libvsapm_partition_map_entry.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/m4/libuna.m4` & `libvsapm-20230506/m4/libuna.m4`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/m4/gettext.m4` & `libvsapm-20230506/m4/gettext.m4`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/m4/tests.m4` & `libvsapm-20230506/m4/tests.m4`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/m4/lib-prefix.m4` & `libvsapm-20230506/m4/lib-prefix.m4`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/m4/ltoptions.m4` & `libvsapm-20230506/m4/ltoptions.m4`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/m4/libcpath.m4` & `libvsapm-20230506/m4/libcpath.m4`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/m4/lib-ld.m4` & `libvsapm-20230506/m4/lib-ld.m4`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/m4/libcthreads.m4` & `libvsapm-20230506/m4/libcthreads.m4`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/m4/lib-link.m4` & `libvsapm-20230506/m4/lib-link.m4`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/m4/python.m4` & `libvsapm-20230506/m4/python.m4`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/m4/libtool.m4` & `libvsapm-20230506/m4/libtool.m4`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/m4/nls.m4` & `libvsapm-20230506/m4/nls.m4`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/m4/libclocale.m4` & `libvsapm-20230506/m4/libclocale.m4`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/m4/libfdata.m4` & `libvsapm-20230506/m4/libfdata.m4`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/m4/host-cpu-c-abi.m4` & `libvsapm-20230506/m4/host-cpu-c-abi.m4`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/m4/libcnotify.m4` & `libvsapm-20230506/m4/libcnotify.m4`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/m4/ltversion.m4` & `libvsapm-20230506/m4/ltversion.m4`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/m4/libcdata.m4` & `libvsapm-20230506/m4/libcdata.m4`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/m4/progtest.m4` & `libvsapm-20230506/m4/progtest.m4`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/m4/lt~obsolete.m4` & `libvsapm-20230506/m4/lt~obsolete.m4`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/m4/libcfile.m4` & `libvsapm-20230506/m4/libcfile.m4`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/m4/po.m4` & `libvsapm-20230506/m4/po.m4`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/m4/pthread.m4` & `libvsapm-20230506/m4/pthread.m4`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/m4/common.m4` & `libvsapm-20230506/m4/common.m4`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/m4/libcerror.m4` & `libvsapm-20230506/m4/libcerror.m4`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/m4/iconv.m4` & `libvsapm-20230506/m4/iconv.m4`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/m4/ltsugar.m4` & `libvsapm-20230506/m4/ltsugar.m4`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/m4/libfcache.m4` & `libvsapm-20230506/m4/libfcache.m4`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/m4/libcsplit.m4` & `libvsapm-20230506/m4/libcsplit.m4`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/m4/intlmacosx.m4` & `libvsapm-20230506/m4/intlmacosx.m4`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/m4/types.m4` & `libvsapm-20230506/m4/types.m4`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/m4/libbfio.m4` & `libvsapm-20230506/m4/libbfio.m4`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/COPYING.LESSER` & `libvsapm-20230506/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcerror/libcerror_system.c` & `libvsapm-20230506/libcerror/libcerror_system.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcerror/libcerror_error.c` & `libvsapm-20230506/libcerror/libcerror_error.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcerror/libcerror_extern.h` & `libvsapm-20230506/libcerror/libcerror_extern.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcerror/Makefile.am` & `libvsapm-20230506/libcerror/Makefile.am`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcerror/libcerror_error.h` & `libvsapm-20230506/libcerror/libcerror_error.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcerror/libcerror_support.h` & `libvsapm-20230506/libcerror/libcerror_support.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcerror/libcerror_types.h` & `libvsapm-20230506/libcerror/libcerror_types.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcerror/libcerror_definitions.h` & `libvsapm-20230506/libcerror/libcerror_definitions.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcerror/libcerror_unused.h` & `libvsapm-20230506/libcerror/libcerror_unused.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcerror/Makefile.in` & `libvsapm-20230506/libcerror/Makefile.in`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcerror/libcerror_support.c` & `libvsapm-20230506/libcerror/libcerror_support.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcerror/libcerror_system.h` & `libvsapm-20230506/libcerror/libcerror_system.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/pyvsapm-python3/Makefile.am` & `libvsapm-20230506/pyvsapm-python3/Makefile.am`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/pyvsapm-python3/Makefile.in` & `libvsapm-20230506/pyvsapm-python3/Makefile.in`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcnotify/libcnotify_libcerror.h` & `libvsapm-20230506/libcnotify/libcnotify_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcnotify/libcnotify_unused.h` & `libvsapm-20230506/libcnotify/libcnotify_unused.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcnotify/libcnotify_support.h` & `libvsapm-20230506/libcnotify/libcnotify_support.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcnotify/libcnotify_support.c` & `libvsapm-20230506/libcnotify/libcnotify_support.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcnotify/Makefile.am` & `libvsapm-20230506/libcnotify/Makefile.am`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcnotify/libcnotify_print.c` & `libvsapm-20230506/libcnotify/libcnotify_print.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcnotify/libcnotify_verbose.c` & `libvsapm-20230506/libcnotify/libcnotify_verbose.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcnotify/libcnotify_stream.h` & `libvsapm-20230506/libcnotify/libcnotify_stream.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcnotify/libcnotify_extern.h` & `libvsapm-20230506/libcnotify/libcnotify_extern.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcnotify/libcnotify_stream.c` & `libvsapm-20230506/libcnotify/libcnotify_stream.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcnotify/Makefile.in` & `libvsapm-20230506/libcnotify/Makefile.in`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcnotify/libcnotify_print.h` & `libvsapm-20230506/libcnotify/libcnotify_print.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcnotify/libcnotify_verbose.h` & `libvsapm-20230506/libcnotify/libcnotify_verbose.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcnotify/libcnotify_definitions.h` & `libvsapm-20230506/libcnotify/libcnotify_definitions.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/ltmain.sh` & `libvsapm-20230506/ltmain.sh`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/compile` & `libvsapm-20230506/compile`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/vsapmtools/info_handle.c` & `libvsapm-20230506/vsapmtools/info_handle.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/vsapmtools/vsapminfo.c` & `libvsapm-20230506/vsapmtools/vsapminfo.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/vsapmtools/vsapmtools_libbfio.h` & `libvsapm-20230506/vsapmtools/vsapmtools_libbfio.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/vsapmtools/Makefile.am` & `libvsapm-20230506/vsapmtools/Makefile.am`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/vsapmtools/vsapmtools_signal.c` & `libvsapm-20230506/vsapmtools/vsapmtools_signal.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/vsapmtools/vsapmtools_getopt.c` & `libvsapm-20230506/vsapmtools/vsapmtools_getopt.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/vsapmtools/vsapmtools_libcerror.h` & `libvsapm-20230506/vsapmtools/vsapmtools_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/vsapmtools/vsapmtools_unused.h` & `libvsapm-20230506/vsapmtools/vsapmtools_unused.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/vsapmtools/vsapmtools_signal.h` & `libvsapm-20230506/vsapmtools/vsapmtools_signal.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/vsapmtools/vsapmtools_libcnotify.h` & `libvsapm-20230506/vsapmtools/vsapmtools_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/vsapmtools/vsapmtools_libuna.h` & `libvsapm-20230506/vsapmtools/vsapmtools_libuna.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/vsapmtools/vsapmtools_libvsapm.h` & `libvsapm-20230506/vsapmtools/vsapmtools_libvsapm.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/vsapmtools/info_handle.h` & `libvsapm-20230506/vsapmtools/info_handle.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/vsapmtools/vsapmtools_output.h` & `libvsapm-20230506/vsapmtools/vsapmtools_output.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/vsapmtools/Makefile.in` & `libvsapm-20230506/vsapmtools/Makefile.in`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/vsapmtools/vsapmtools_libclocale.h` & `libvsapm-20230506/vsapmtools/vsapmtools_libclocale.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/vsapmtools/vsapmtools_i18n.h` & `libvsapm-20230506/vsapmtools/vsapmtools_i18n.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/vsapmtools/vsapmtools_getopt.h` & `libvsapm-20230506/vsapmtools/vsapmtools_getopt.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/vsapmtools/vsapmtools_output.c` & `libvsapm-20230506/vsapmtools/vsapmtools_output.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/config.rpath` & `libvsapm-20230506/config.rpath`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/depcomp` & `libvsapm-20230506/depcomp`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/po/en@quot.header` & `libvsapm-20230506/po/en@quot.header`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/po/Rules-quot` & `libvsapm-20230506/po/Rules-quot`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/po/remove-potcdate.sin` & `libvsapm-20230506/po/remove-potcdate.sin`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/po/Makevars.in` & `libvsapm-20230506/po/Makevars.in`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/po/en@boldquot.header` & `libvsapm-20230506/po/en@boldquot.header`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/po/Makevars` & `libvsapm-20230506/po/Makevars`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/po/insert-header.sin` & `libvsapm-20230506/po/insert-header.sin`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/po/Makefile.in.in` & `libvsapm-20230506/po/Makefile.in.in`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libfdata/libfdata_segments_array.h` & `libvsapm-20230506/libfdata/libfdata_segments_array.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libfdata/libfdata_cache.c` & `libvsapm-20230506/libfdata/libfdata_cache.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libfdata/libfdata_support.c` & `libvsapm-20230506/libfdata/libfdata_support.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libfdata/libfdata_list_element.c` & `libvsapm-20230506/libfdata/libfdata_list_element.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libfdata/libfdata_mapped_range.h` & `libvsapm-20230506/libfdata/libfdata_mapped_range.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libfdata/libfdata_extern.h` & `libvsapm-20230506/libfdata/libfdata_extern.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libfdata/libfdata_list.c` & `libvsapm-20230506/libfdata/libfdata_list.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libfdata/libfdata_libcdata.h` & `libvsapm-20230506/libfdata/libfdata_libcdata.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libfdata/libfdata_notify.h` & `libvsapm-20230506/libfdata/libfdata_notify.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libfdata/libfdata_range_list.h` & `libvsapm-20230506/libfdata/libfdata_range_list.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libfdata/Makefile.am` & `libvsapm-20230506/libfdata/Makefile.am`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libfdata/libfdata_error.c` & `libvsapm-20230506/libfdata/libfdata_error.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libfdata/libfdata_list.h` & `libvsapm-20230506/libfdata/libfdata_list.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libfdata/libfdata_area.h` & `libvsapm-20230506/libfdata/libfdata_area.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libfdata/libfdata_types.h` & `libvsapm-20230506/libfdata/libfdata_types.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libfdata/libfdata_area.c` & `libvsapm-20230506/libfdata/libfdata_area.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libfdata/libfdata_range.h` & `libvsapm-20230506/libfdata/libfdata_range.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libfdata/libfdata_vector.c` & `libvsapm-20230506/libfdata/libfdata_vector.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libfdata/libfdata_stream.h` & `libvsapm-20230506/libfdata/libfdata_stream.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libfdata/libfdata_vector.h` & `libvsapm-20230506/libfdata/libfdata_vector.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libfdata/libfdata_support.h` & `libvsapm-20230506/libfdata/libfdata_support.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libfdata/libfdata_libfcache.h` & `libvsapm-20230506/libfdata/libfdata_libfcache.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libfdata/libfdata_libcerror.h` & `libvsapm-20230506/libfdata/libfdata_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libfdata/libfdata_range_list.c` & `libvsapm-20230506/libfdata/libfdata_range_list.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libfdata/libfdata_libcnotify.h` & `libvsapm-20230506/libfdata/libfdata_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libfdata/libfdata_notify.c` & `libvsapm-20230506/libfdata/libfdata_notify.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libfdata/libfdata_list_element.h` & `libvsapm-20230506/libfdata/libfdata_list_element.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libfdata/libfdata_unused.h` & `libvsapm-20230506/libfdata/libfdata_unused.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libfdata/libfdata_error.h` & `libvsapm-20230506/libfdata/libfdata_error.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libfdata/Makefile.in` & `libvsapm-20230506/libfdata/Makefile.in`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libfdata/libfdata_cache.h` & `libvsapm-20230506/libfdata/libfdata_cache.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libfdata/libfdata_stream.c` & `libvsapm-20230506/libfdata/libfdata_stream.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libfdata/libfdata_segments_array.c` & `libvsapm-20230506/libfdata/libfdata_segments_array.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libfdata/libfdata_mapped_range.c` & `libvsapm-20230506/libfdata/libfdata_mapped_range.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libfdata/libfdata_definitions.h` & `libvsapm-20230506/libfdata/libfdata_definitions.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libfdata/libfdata_range.c` & `libvsapm-20230506/libfdata/libfdata_range.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcdata/libcdata_array.c` & `libvsapm-20230506/libcdata/libcdata_array.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcdata/libcdata_btree_node.c` & `libvsapm-20230506/libcdata/libcdata_btree_node.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcdata/libcdata_tree_node.c` & `libvsapm-20230506/libcdata/libcdata_tree_node.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcdata/libcdata_libcthreads.h` & `libvsapm-20230506/libcdata/libcdata_libcthreads.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcdata/libcdata_range_list_value.h` & `libvsapm-20230506/libcdata/libcdata_range_list_value.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcdata/libcdata_unused.h` & `libvsapm-20230506/libcdata/libcdata_unused.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcdata/libcdata_range_list.h` & `libvsapm-20230506/libcdata/libcdata_range_list.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcdata/Makefile.am` & `libvsapm-20230506/libcdata/Makefile.am`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcdata/libcdata_range_list.c` & `libvsapm-20230506/libcdata/libcdata_range_list.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcdata/libcdata_extern.h` & `libvsapm-20230506/libcdata/libcdata_extern.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcdata/libcdata_support.c` & `libvsapm-20230506/libcdata/libcdata_support.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcdata/libcdata_list_element.h` & `libvsapm-20230506/libcdata/libcdata_list_element.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcdata/libcdata_btree_values_list.c` & `libvsapm-20230506/libcdata/libcdata_btree_values_list.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcdata/libcdata_range_list_value.c` & `libvsapm-20230506/libcdata/libcdata_range_list_value.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcdata/libcdata_libcerror.h` & `libvsapm-20230506/libcdata/libcdata_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcdata/libcdata_error.c` & `libvsapm-20230506/libcdata/libcdata_error.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcdata/libcdata_error.h` & `libvsapm-20230506/libcdata/libcdata_error.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcdata/libcdata_support.h` & `libvsapm-20230506/libcdata/libcdata_support.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcdata/libcdata_btree_node.h` & `libvsapm-20230506/libcdata/libcdata_btree_node.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcdata/libcdata_list.c` & `libvsapm-20230506/libcdata/libcdata_list.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcdata/libcdata_tree_node.h` & `libvsapm-20230506/libcdata/libcdata_tree_node.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcdata/libcdata_list.h` & `libvsapm-20230506/libcdata/libcdata_list.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcdata/libcdata_types.h` & `libvsapm-20230506/libcdata/libcdata_types.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcdata/libcdata_list_element.c` & `libvsapm-20230506/libcdata/libcdata_list_element.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcdata/Makefile.in` & `libvsapm-20230506/libcdata/Makefile.in`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcdata/libcdata_btree_values_list.h` & `libvsapm-20230506/libcdata/libcdata_btree_values_list.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcdata/libcdata_array.h` & `libvsapm-20230506/libcdata/libcdata_array.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcdata/libcdata_btree.h` & `libvsapm-20230506/libcdata/libcdata_btree.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcdata/libcdata_definitions.h` & `libvsapm-20230506/libcdata/libcdata_definitions.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcdata/libcdata_btree.c` & `libvsapm-20230506/libcdata/libcdata_btree.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/pyvsapm/pyvsapm_integer.h` & `libvsapm-20230506/pyvsapm/pyvsapm_integer.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/pyvsapm/pyvsapm_unused.h` & `libvsapm-20230506/pyvsapm/pyvsapm_unused.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/pyvsapm/pyvsapm_libcerror.h` & `libvsapm-20230506/pyvsapm/pyvsapm_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/pyvsapm/pyvsapm_file_object_io_handle.h` & `libvsapm-20230506/pyvsapm/pyvsapm_file_object_io_handle.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/pyvsapm/pyvsapm_partition.c` & `libvsapm-20230506/pyvsapm/pyvsapm_partition.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/pyvsapm/pyvsapm_python.h` & `libvsapm-20230506/pyvsapm/pyvsapm_python.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/pyvsapm/pyvsapm_integer.c` & `libvsapm-20230506/pyvsapm/pyvsapm_integer.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/pyvsapm/Makefile.am` & `libvsapm-20230506/pyvsapm/Makefile.am`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/pyvsapm/pyvsapm_libvsapm.h` & `libvsapm-20230506/pyvsapm/pyvsapm_libvsapm.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/pyvsapm/pyvsapm_partition.h` & `libvsapm-20230506/pyvsapm/pyvsapm_partition.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/pyvsapm/pyvsapm.h` & `libvsapm-20230506/pyvsapm/pyvsapm.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/pyvsapm/pyvsapm_libbfio.h` & `libvsapm-20230506/pyvsapm/pyvsapm_libbfio.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/pyvsapm/pyvsapm.c` & `libvsapm-20230506/pyvsapm/pyvsapm.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/pyvsapm/pyvsapm_partitions.h` & `libvsapm-20230506/pyvsapm/pyvsapm_partitions.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/pyvsapm/pyvsapm_libclocale.h` & `libvsapm-20230506/pyvsapm/pyvsapm_libclocale.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/pyvsapm/pyvsapm_volume.h` & `libvsapm-20230506/pyvsapm/pyvsapm_volume.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/pyvsapm/pyvsapm_error.c` & `libvsapm-20230506/pyvsapm/pyvsapm_error.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/pyvsapm/pyvsapm_error.h` & `libvsapm-20230506/pyvsapm/pyvsapm_error.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/pyvsapm/Makefile.in` & `libvsapm-20230506/pyvsapm/Makefile.in`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/pyvsapm/pyvsapm_file_object_io_handle.c` & `libvsapm-20230506/pyvsapm/pyvsapm_file_object_io_handle.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/pyvsapm/pyvsapm_volume.c` & `libvsapm-20230506/pyvsapm/pyvsapm_volume.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/pyvsapm/pyvsapm_partitions.c` & `libvsapm-20230506/pyvsapm/pyvsapm_partitions.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/acinclude.m4` & `libvsapm-20230506/acinclude.m4`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcsplit/libcsplit_types.h` & `libvsapm-20230506/libcsplit/libcsplit_types.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcsplit/libcsplit_wide_string.h` & `libvsapm-20230506/libcsplit/libcsplit_wide_string.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcsplit/libcsplit_error.h` & `libvsapm-20230506/libcsplit/libcsplit_error.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcsplit/libcsplit_support.h` & `libvsapm-20230506/libcsplit/libcsplit_support.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcsplit/libcsplit_narrow_split_string.c` & `libvsapm-20230506/libcsplit/libcsplit_narrow_split_string.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcsplit/libcsplit_narrow_split_string.h` & `libvsapm-20230506/libcsplit/libcsplit_narrow_split_string.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcsplit/Makefile.am` & `libvsapm-20230506/libcsplit/Makefile.am`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcsplit/libcsplit_wide_split_string.c` & `libvsapm-20230506/libcsplit/libcsplit_wide_split_string.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcsplit/libcsplit_narrow_string.h` & `libvsapm-20230506/libcsplit/libcsplit_narrow_string.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcsplit/libcsplit_unused.h` & `libvsapm-20230506/libcsplit/libcsplit_unused.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcsplit/libcsplit_wide_string.c` & `libvsapm-20230506/libcsplit/libcsplit_wide_string.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcsplit/libcsplit_narrow_string.c` & `libvsapm-20230506/libcsplit/libcsplit_narrow_string.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcsplit/Makefile.in` & `libvsapm-20230506/libcsplit/Makefile.in`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcsplit/libcsplit_wide_split_string.h` & `libvsapm-20230506/libcsplit/libcsplit_wide_split_string.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcsplit/libcsplit_definitions.h` & `libvsapm-20230506/libcsplit/libcsplit_definitions.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcsplit/libcsplit_error.c` & `libvsapm-20230506/libcsplit/libcsplit_error.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcsplit/libcsplit_support.c` & `libvsapm-20230506/libcsplit/libcsplit_support.c`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcsplit/libcsplit_libcerror.h` & `libvsapm-20230506/libcsplit/libcsplit_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/libcsplit/libcsplit_extern.h` & `libvsapm-20230506/libcsplit/libcsplit_extern.h`

 * *Files identical despite different names*

### Comparing `libvsapm-20230430/configure.ac` & `libvsapm-20230506/configure.ac`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 AC_PREREQ([2.71])
 
 AC_INIT(
  [libvsapm],
- [20230430],
+ [20230506],
  [joachim.metz@gmail.com])
 
 AC_CONFIG_SRCDIR(
  [include/libvsapm.h.in])
 
 AM_INIT_AUTOMAKE([gnu 1.6 tar-ustar])
```

