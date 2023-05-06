# Comparing `tmp/libvsbsdl-python-20230502.tar.gz` & `tmp/libvsbsdl-python-20230506.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libvsbsdl-python-20230502.tar", last modified: Thu May  4 04:14:37 2023, max compression
+gzip compressed data, was "libvsbsdl-python-20230506.tar", last modified: Sat May  6 06:05:37 2023, max compression
```

## Comparing `libvsbsdl-python-20230502.tar` & `libvsbsdl-python-20230506.tar`

### file list

```diff
@@ -1,712 +1,712 @@
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:14:36.000000 libvsbsdl-20230502/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:14:34.000000 libvsbsdl-20230502/libfcache/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2023-05-04 03:55:41.000000 libvsbsdl-20230502/libfcache/libfcache_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1619 2023-05-04 03:55:41.000000 libvsbsdl-20230502/libfcache/libfcache_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3806 2023-05-04 03:55:41.000000 libvsbsdl-20230502/libfcache/libfcache_cache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2023-05-04 03:55:41.000000 libvsbsdl-20230502/libfcache/libfcache_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1178 2023-05-04 03:55:41.000000 libvsbsdl-20230502/libfcache/libfcache_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      845 2023-05-04 03:55:41.000000 libvsbsdl-20230502/libfcache/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2023-05-04 03:55:41.000000 libvsbsdl-20230502/libfcache/libfcache_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2023-05-04 03:55:41.000000 libvsbsdl-20230502/libfcache/libfcache_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2023-05-04 03:55:41.000000 libvsbsdl-20230502/libfcache/libfcache_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1680 2023-05-04 03:55:41.000000 libvsbsdl-20230502/libfcache/libfcache_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3161 2023-05-04 03:55:41.000000 libvsbsdl-20230502/libfcache/libfcache_cache_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12461 2023-05-04 03:55:41.000000 libvsbsdl-20230502/libfcache/libfcache_cache_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29208 2023-05-04 03:55:57.000000 libvsbsdl-20230502/libfcache/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2023-05-04 03:55:41.000000 libvsbsdl-20230502/libfcache/libfcache_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2259 2023-05-04 03:55:41.000000 libvsbsdl-20230502/libfcache/libfcache_date_time.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26186 2023-05-04 03:55:41.000000 libvsbsdl-20230502/libfcache/libfcache_cache.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2023-05-04 03:55:41.000000 libvsbsdl-20230502/libfcache/libfcache_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2023-05-04 03:55:41.000000 libvsbsdl-20230502/libfcache/libfcache_date_time.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:14:29.000000 libvsbsdl-20230502/common/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2023-05-02 04:08:32.000000 libvsbsdl-20230502/common/config_msc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10432 2023-05-02 04:08:32.000000 libvsbsdl-20230502/common/byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1245 2023-05-02 04:08:32.000000 libvsbsdl-20230502/common/common.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4606 2023-05-02 04:08:32.000000 libvsbsdl-20230502/common/system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      378 2023-05-02 04:08:31.000000 libvsbsdl-20230502/common/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7370 2023-05-04 03:56:12.000000 libvsbsdl-20230502/common/types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7370 2023-05-02 04:08:32.000000 libvsbsdl-20230502/common/types.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2377 2023-05-02 04:08:32.000000 libvsbsdl-20230502/common/config_winapi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3254 2023-05-02 04:08:32.000000 libvsbsdl-20230502/common/memory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16355 2023-05-03 15:41:32.000000 libvsbsdl-20230502/common/config.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5414 2023-05-02 04:08:32.000000 libvsbsdl-20230502/common/narrow_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23779 2023-05-04 03:55:56.000000 libvsbsdl-20230502/common/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3873 2023-05-02 04:08:32.000000 libvsbsdl-20230502/common/file_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      952 2023-05-02 04:08:32.000000 libvsbsdl-20230502/common/config_borlandc.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15432 2023-05-04 03:55:56.000000 libvsbsdl-20230502/common/config.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5059 2023-05-02 04:08:32.000000 libvsbsdl-20230502/common/wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      650 2023-05-02 04:08:31.000000 libvsbsdl-20230502/libvsbsdl.pc.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:14:36.000000 libvsbsdl-20230502/tests/
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3862 2023-05-02 04:10:55.000000 libvsbsdl-20230502/tests/test_library.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5044 2023-05-02 04:08:34.000000 libvsbsdl-20230502/tests/pyvsbsdl_test_volume.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      984 2023-05-02 04:08:34.000000 libvsbsdl-20230502/tests/vsbsdl_test_libvsbsdl.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9434 2023-05-02 04:09:34.000000 libvsbsdl-20230502/tests/vsbsdl_test_partition_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4742 2023-05-02 04:08:34.000000 libvsbsdl-20230502/tests/vsbsdl_test_memory.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1709 2023-05-02 04:08:34.000000 libvsbsdl-20230502/tests/vsbsdl_test_rwlock.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3430 2023-05-02 04:08:34.000000 libvsbsdl-20230502/tests/test_python_module.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6652 2023-05-02 04:09:34.000000 libvsbsdl-20230502/tests/vsbsdl_test_rwlock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6502 2023-05-02 04:52:35.000000 libvsbsdl-20230502/tests/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3174 2023-05-02 04:08:34.000000 libvsbsdl-20230502/tests/vsbsdl_test_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1707 2023-05-02 04:08:34.000000 libvsbsdl-20230502/tests/vsbsdl_test_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13266 2023-05-02 04:08:34.000000 libvsbsdl-20230502/tests/vsbsdl_test_functions.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23239 2023-05-02 04:09:34.000000 libvsbsdl-20230502/tests/vsbsdl_test_disklabel.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1460 2023-05-02 04:08:34.000000 libvsbsdl-20230502/tests/vsbsdl_test_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1813 2023-05-02 04:08:34.000000 libvsbsdl-20230502/tests/vsbsdl_test_getopt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4534 2023-05-02 04:08:34.000000 libvsbsdl-20230502/tests/vsbsdl_test_getopt.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2464 2023-05-02 04:08:34.000000 libvsbsdl-20230502/tests/vsbsdl_test_tools_output.c
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3805 2023-05-02 04:10:55.000000 libvsbsdl-20230502/tests/test_tools.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8604 2023-05-02 04:08:34.000000 libvsbsdl-20230502/tests/vsbsdl_test_macros.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31469 2023-05-02 04:09:34.000000 libvsbsdl-20230502/tests/vsbsdl_test_volume.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1442 2023-05-02 04:08:34.000000 libvsbsdl-20230502/tests/vsbsdl_test_libcerror.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     1653 2023-05-02 04:08:34.000000 libvsbsdl-20230502/tests/test_manpage.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1463 2023-05-02 04:08:34.000000 libvsbsdl-20230502/tests/vsbsdl_test_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    57176 2023-05-02 04:09:34.000000 libvsbsdl-20230502/tests/vsbsdl_test_partition.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4210 2023-05-02 04:08:34.000000 libvsbsdl-20230502/tests/vsbsdl_test_tools_signal.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9091 2023-05-02 04:09:34.000000 libvsbsdl-20230502/tests/pyvsbsdl_test_partition.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37792 2023-05-02 04:08:34.000000 libvsbsdl-20230502/tests/test_runner.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1555 2023-05-02 04:08:34.000000 libvsbsdl-20230502/tests/pyvsbsdl_test_support.py
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1549 2023-05-02 04:08:34.000000 libvsbsdl-20230502/tests/vsbsdl_test_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    59388 2023-05-04 03:55:58.000000 libvsbsdl-20230502/tests/Makefile.in
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     2174 2023-05-02 04:08:34.000000 libvsbsdl-20230502/tests/test_vsbsdlinfo.sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9709 2023-05-02 04:09:34.000000 libvsbsdl-20230502/tests/vsbsdl_test_sector_data.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1708 2023-05-02 04:08:34.000000 libvsbsdl-20230502/tests/vsbsdl_test_memory.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8150 2023-05-02 04:09:34.000000 libvsbsdl-20230502/tests/vsbsdl_test_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5673 2023-05-02 04:08:34.000000 libvsbsdl-20230502/tests/vsbsdl_test_tools_info_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14574 2023-05-02 04:08:34.000000 libvsbsdl-20230502/tests/vsbsdl_test_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4365 2023-05-02 04:08:34.000000 libvsbsdl-20230502/tests/vsbsdl_test_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1740 2023-05-02 04:08:34.000000 libvsbsdl-20230502/tests/vsbsdl_test_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1816 2023-05-02 04:08:34.000000 libvsbsdl-20230502/tests/vsbsdl_test_functions.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:14:31.000000 libvsbsdl-20230502/libclocale/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2023-05-04 03:55:33.000000 libvsbsdl-20230502/libclocale/libclocale_wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3094 2023-05-04 03:55:33.000000 libvsbsdl-20230502/libclocale/libclocale_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1717 2023-05-04 03:55:33.000000 libvsbsdl-20230502/libclocale/libclocale_locale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      744 2023-05-04 03:55:33.000000 libvsbsdl-20230502/libclocale/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10671 2023-05-04 03:55:33.000000 libvsbsdl-20230502/libclocale/libclocale_locale.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2023-05-04 03:55:33.000000 libvsbsdl-20230502/libclocale/libclocale_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2023-05-04 03:55:33.000000 libvsbsdl-20230502/libclocale/libclocale_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2023-05-04 03:55:33.000000 libvsbsdl-20230502/libclocale/libclocale_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3412 2023-05-04 03:55:33.000000 libvsbsdl-20230502/libclocale/libclocale_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2023-05-04 03:55:33.000000 libvsbsdl-20230502/libclocale/libclocale_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21033 2023-05-04 03:55:33.000000 libvsbsdl-20230502/libclocale/libclocale_codepage.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28735 2023-05-04 03:55:57.000000 libvsbsdl-20230502/libclocale/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1969 2023-05-04 03:55:33.000000 libvsbsdl-20230502/libclocale/libclocale_wide_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2023-05-04 03:55:33.000000 libvsbsdl-20230502/libclocale/libclocale_libcerror.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2023-05-04 03:55:56.000000 libvsbsdl-20230502/missing
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3193 2023-04-29 13:19:51.000000 libvsbsdl-20230502/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    55932 2023-05-04 03:55:53.000000 libvsbsdl-20230502/aclocal.m4
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:14:34.000000 libvsbsdl-20230502/libbfio/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8883 2023-05-04 03:55:26.000000 libvsbsdl-20230502/libbfio/libbfio_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2023-05-04 03:55:26.000000 libvsbsdl-20230502/libbfio/libbfio_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    64816 2023-05-04 03:55:26.000000 libvsbsdl-20230502/libbfio/libbfio_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2023-05-04 03:55:26.000000 libvsbsdl-20230502/libbfio/libbfio_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2708 2023-05-04 03:55:27.000000 libvsbsdl-20230502/libbfio/libbfio_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2023-05-04 03:55:26.000000 libvsbsdl-20230502/libbfio/libbfio_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2023-05-04 03:55:26.000000 libvsbsdl-20230502/libbfio/libbfio_codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2023-05-04 03:55:26.000000 libvsbsdl-20230502/libbfio/libbfio_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2023-05-04 03:55:26.000000 libvsbsdl-20230502/libbfio/libbfio_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12186 2023-05-04 03:55:26.000000 libvsbsdl-20230502/libbfio/libbfio_file_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27543 2023-05-04 03:55:26.000000 libvsbsdl-20230502/libbfio/libbfio_file_range_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2023-05-04 03:55:26.000000 libvsbsdl-20230502/libbfio/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10798 2023-05-04 03:55:26.000000 libvsbsdl-20230502/libbfio/libbfio_file_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10899 2023-05-04 03:55:26.000000 libvsbsdl-20230502/libbfio/libbfio_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6841 2023-05-04 03:55:26.000000 libvsbsdl-20230502/libbfio/libbfio_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2630 2023-05-04 03:55:26.000000 libvsbsdl-20230502/libbfio/libbfio_file_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2814 2023-05-04 03:55:26.000000 libvsbsdl-20230502/libbfio/libbfio_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4085 2023-05-04 03:55:26.000000 libvsbsdl-20230502/libbfio/libbfio_file_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21082 2023-05-04 03:55:26.000000 libvsbsdl-20230502/libbfio/libbfio_memory_range_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2234 2023-05-04 03:55:26.000000 libvsbsdl-20230502/libbfio/libbfio_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2324 2023-05-04 03:55:26.000000 libvsbsdl-20230502/libbfio/libbfio_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2077 2023-05-04 03:55:26.000000 libvsbsdl-20230502/libbfio/libbfio_file_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3835 2023-05-04 03:55:26.000000 libvsbsdl-20230502/libbfio/libbfio_memory_range_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2023-05-04 03:55:26.000000 libvsbsdl-20230502/libbfio/libbfio_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1918 2023-05-04 03:55:26.000000 libvsbsdl-20230502/libbfio/libbfio_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25540 2023-05-04 03:55:26.000000 libvsbsdl-20230502/libbfio/libbfio_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2023-05-04 03:55:26.000000 libvsbsdl-20230502/libbfio/libbfio_memory_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4806 2023-05-04 03:55:26.000000 libvsbsdl-20230502/libbfio/libbfio_file_range_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5821 2023-05-04 03:55:26.000000 libvsbsdl-20230502/libbfio/libbfio_memory_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32241 2023-05-04 03:55:57.000000 libvsbsdl-20230502/libbfio/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    81879 2023-05-04 03:55:26.000000 libvsbsdl-20230502/libbfio/libbfio_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2023-05-04 03:55:26.000000 libvsbsdl-20230502/libbfio/libbfio_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1362 2023-05-04 03:55:26.000000 libvsbsdl-20230502/libbfio/libbfio_libcpath.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1420 2023-05-04 03:55:26.000000 libvsbsdl-20230502/libbfio/libbfio_libcfile.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2023-05-04 03:55:26.000000 libvsbsdl-20230502/libbfio/libbfio_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26845 2023-05-04 03:55:26.000000 libvsbsdl-20230502/libbfio/libbfio_file_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2023-05-04 03:55:26.000000 libvsbsdl-20230502/libbfio/libbfio_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1572 2023-05-04 03:55:26.000000 libvsbsdl-20230502/libbfio/libbfio_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2023-05-02 04:08:31.000000 libvsbsdl-20230502/COPYING
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      394 2023-05-02 04:09:44.000000 libvsbsdl-20230502/README
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:14:29.000000 libvsbsdl-20230502/include/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      509 2023-05-02 04:08:31.000000 libvsbsdl-20230502/include/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11038 2023-05-04 03:56:12.000000 libvsbsdl-20230502/include/libvsbsdl.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26799 2023-05-04 03:55:56.000000 libvsbsdl-20230502/include/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11038 2023-05-03 04:14:47.000000 libvsbsdl-20230502/include/libvsbsdl.h.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:14:29.000000 libvsbsdl-20230502/include/libvsbsdl/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1813 2023-05-02 04:08:32.000000 libvsbsdl-20230502/include/libvsbsdl/definitions.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1431 2023-05-02 04:08:32.000000 libvsbsdl-20230502/include/libvsbsdl/extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4857 2023-05-04 03:56:12.000000 libvsbsdl-20230502/include/libvsbsdl/types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1558 2023-05-02 04:08:32.000000 libvsbsdl-20230502/include/libvsbsdl/features.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4988 2023-05-02 04:08:32.000000 libvsbsdl-20230502/include/libvsbsdl/types.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1494 2023-05-04 03:56:12.000000 libvsbsdl-20230502/include/libvsbsdl/features.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1811 2023-05-04 03:56:12.000000 libvsbsdl-20230502/include/libvsbsdl/definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5417 2023-05-02 04:08:32.000000 libvsbsdl-20230502/include/libvsbsdl/codepage.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6821 2023-05-02 04:08:32.000000 libvsbsdl-20230502/include/libvsbsdl/error.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2023-05-04 03:55:56.000000 libvsbsdl-20230502/install-sh
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2023-05-04 03:55:56.000000 libvsbsdl-20230502/INSTALL
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:14:29.000000 libvsbsdl-20230502/dpkg/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      122 2023-05-02 04:08:31.000000 libvsbsdl-20230502/dpkg/changelog.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      141 2023-05-04 03:56:12.000000 libvsbsdl-20230502/dpkg/changelog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1023 2023-05-02 04:08:34.000000 libvsbsdl-20230502/dpkg/copyright
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       96 2023-05-02 04:08:31.000000 libvsbsdl-20230502/dpkg/libvsbsdl-dev.install
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:14:29.000000 libvsbsdl-20230502/dpkg/source/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2023-05-02 04:08:31.000000 libvsbsdl-20230502/dpkg/source/format
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       22 2023-05-02 04:08:31.000000 libvsbsdl-20230502/dpkg/libvsbsdl.install
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      778 2023-05-02 04:08:31.000000 libvsbsdl-20230502/dpkg/rules
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        3 2023-05-02 04:08:31.000000 libvsbsdl-20230502/dpkg/compat
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2181 2023-05-02 04:08:31.000000 libvsbsdl-20230502/dpkg/control
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:14:35.000000 libvsbsdl-20230502/pyvsbsdl/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2023-05-02 04:08:33.000000 libvsbsdl-20230502/pyvsbsdl/pyvsbsdl_integer.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      976 2023-05-02 04:08:33.000000 libvsbsdl-20230502/pyvsbsdl/pyvsbsdl_libvsbsdl.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8889 2023-05-02 04:08:33.000000 libvsbsdl-20230502/pyvsbsdl/pyvsbsdl_integer.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1201 2023-04-29 13:19:51.000000 libvsbsdl-20230502/pyvsbsdl/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9366 2023-05-02 04:08:33.000000 libvsbsdl-20230502/pyvsbsdl/pyvsbsdl_partitions.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2940 2023-05-03 04:27:03.000000 libvsbsdl-20230502/pyvsbsdl/pyvsbsdl_partition.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1523 2023-05-02 04:08:33.000000 libvsbsdl-20230502/pyvsbsdl/pyvsbsdl_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9561 2023-05-02 04:08:33.000000 libvsbsdl-20230502/pyvsbsdl/pyvsbsdl_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33959 2023-05-02 04:08:33.000000 libvsbsdl-20230502/pyvsbsdl/pyvsbsdl_file_object_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1544 2023-05-02 04:08:33.000000 libvsbsdl-20230502/pyvsbsdl/pyvsbsdl_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2463 2023-05-02 04:08:33.000000 libvsbsdl-20230502/pyvsbsdl/pyvsbsdl_partitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1403 2023-05-02 04:08:33.000000 libvsbsdl-20230502/pyvsbsdl/pyvsbsdl_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22303 2023-05-02 04:09:34.000000 libvsbsdl-20230502/pyvsbsdl/pyvsbsdl_volume.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1876 2023-05-02 04:08:33.000000 libvsbsdl-20230502/pyvsbsdl/pyvsbsdl.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41530 2023-05-04 03:55:58.000000 libvsbsdl-20230502/pyvsbsdl/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14918 2023-05-02 04:08:33.000000 libvsbsdl-20230502/pyvsbsdl/pyvsbsdl.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1433 2023-05-02 04:08:33.000000 libvsbsdl-20230502/pyvsbsdl/pyvsbsdl_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2031 2023-05-02 04:08:33.000000 libvsbsdl-20230502/pyvsbsdl/pyvsbsdl_python.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1454 2023-05-02 04:08:33.000000 libvsbsdl-20230502/pyvsbsdl/pyvsbsdl_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4151 2023-05-02 04:08:33.000000 libvsbsdl-20230502/pyvsbsdl/pyvsbsdl_file_object_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2867 2023-05-02 04:08:33.000000 libvsbsdl-20230502/pyvsbsdl/pyvsbsdl_volume.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24351 2023-05-03 15:51:01.000000 libvsbsdl-20230502/pyvsbsdl/pyvsbsdl_partition.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:14:34.000000 libvsbsdl-20230502/libcfile/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   105597 2023-05-04 03:55:31.000000 libvsbsdl-20230502/libcfile/libcfile_file.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2023-05-04 03:55:31.000000 libvsbsdl-20230502/libcfile/libcfile_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25753 2023-05-04 03:55:31.000000 libvsbsdl-20230502/libcfile/libcfile_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2389 2023-05-04 03:55:31.000000 libvsbsdl-20230502/libcfile/libcfile_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2023-05-04 03:55:31.000000 libvsbsdl-20230502/libcfile/libcfile_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18388 2023-05-04 03:55:31.000000 libvsbsdl-20230502/libcfile/libcfile_winapi.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      907 2023-05-04 03:55:31.000000 libvsbsdl-20230502/libcfile/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2023-05-04 03:55:31.000000 libvsbsdl-20230502/libcfile/libcfile_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2023-05-04 03:55:31.000000 libvsbsdl-20230502/libcfile/libcfile_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3107 2023-05-04 03:55:31.000000 libvsbsdl-20230502/libcfile/libcfile_winapi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1497 2023-05-04 03:55:31.000000 libvsbsdl-20230502/libcfile/libcfile_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2023-05-04 03:55:31.000000 libvsbsdl-20230502/libcfile/libcfile_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2023-05-04 03:55:31.000000 libvsbsdl-20230502/libcfile/libcfile_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2879 2023-05-04 03:55:31.000000 libvsbsdl-20230502/libcfile/libcfile_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6452 2023-05-04 03:55:31.000000 libvsbsdl-20230502/libcfile/libcfile_file.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2023-05-04 03:55:31.000000 libvsbsdl-20230502/libcfile/libcfile_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2023-05-04 03:55:31.000000 libvsbsdl-20230502/libcfile/libcfile_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29499 2023-05-04 03:55:57.000000 libvsbsdl-20230502/libcfile/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2023-05-04 03:55:31.000000 libvsbsdl-20230502/libcfile/libcfile_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2023-05-04 03:55:31.000000 libvsbsdl-20230502/libcfile/libcfile_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2023-05-04 03:55:31.000000 libvsbsdl-20230502/libcfile/libcfile_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2023-05-04 03:55:31.000000 libvsbsdl-20230502/libcfile/libcfile_notify.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:14:30.000000 libvsbsdl-20230502/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2023-05-04 03:55:39.000000 libvsbsdl-20230502/libcthreads/libcthreads_thread_pool.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2023-05-04 03:55:39.000000 libvsbsdl-20230502/libcthreads/libcthreads_thread_pool.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2023-05-04 03:55:39.000000 libvsbsdl-20230502/libcthreads/libcthreads_repeating_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2023-05-04 03:55:39.000000 libvsbsdl-20230502/libcthreads/libcthreads_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1136 2023-05-04 03:55:39.000000 libvsbsdl-20230502/libcthreads/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2023-05-04 03:55:39.000000 libvsbsdl-20230502/libcthreads/libcthreads_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2023-05-04 03:55:39.000000 libvsbsdl-20230502/libcthreads/libcthreads_condition.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2023-05-04 03:55:39.000000 libvsbsdl-20230502/libcthreads/libcthreads_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2023-05-04 03:55:39.000000 libvsbsdl-20230502/libcthreads/libcthreads_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2023-05-04 03:55:39.000000 libvsbsdl-20230502/libcthreads/libcthreads_repeating_thread.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2023-05-04 03:55:39.000000 libvsbsdl-20230502/libcthreads/libcthreads_read_write_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2023-05-04 03:55:39.000000 libvsbsdl-20230502/libcthreads/libcthreads_mutex.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2023-05-04 03:55:39.000000 libvsbsdl-20230502/libcthreads/libcthreads_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2023-05-04 03:55:39.000000 libvsbsdl-20230502/libcthreads/libcthreads_thread.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2023-05-04 03:55:39.000000 libvsbsdl-20230502/libcthreads/libcthreads_mutex.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2023-05-04 03:55:39.000000 libvsbsdl-20230502/libcthreads/libcthreads_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2023-05-04 03:55:39.000000 libvsbsdl-20230502/libcthreads/libcthreads_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2023-05-04 03:55:39.000000 libvsbsdl-20230502/libcthreads/libcthreads_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2023-05-04 03:55:39.000000 libvsbsdl-20230502/libcthreads/libcthreads_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2023-05-04 03:55:39.000000 libvsbsdl-20230502/libcthreads/libcthreads_queue.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2023-05-04 03:55:39.000000 libvsbsdl-20230502/libcthreads/libcthreads_condition.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31589 2023-05-04 03:55:57.000000 libvsbsdl-20230502/libcthreads/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2023-05-04 03:55:39.000000 libvsbsdl-20230502/libcthreads/libcthreads_thread_attributes.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2023-05-04 03:55:39.000000 libvsbsdl-20230502/libcthreads/libcthreads_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2023-05-04 03:55:39.000000 libvsbsdl-20230502/libcthreads/libcthreads_lock.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2023-05-04 03:55:39.000000 libvsbsdl-20230502/libcthreads/libcthreads_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2023-05-04 03:55:39.000000 libvsbsdl-20230502/libcthreads/libcthreads_read_write_lock.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2023-05-04 03:55:39.000000 libvsbsdl-20230502/libcthreads/libcthreads_thread_attributes.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2023-05-04 03:55:39.000000 libvsbsdl-20230502/libcthreads/libcthreads_queue.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       88 2023-05-02 04:08:32.000000 libvsbsdl-20230502/AUTHORS
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35409 2023-05-04 03:55:56.000000 libvsbsdl-20230502/config.sub
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:14:34.000000 libvsbsdl-20230502/libcpath/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2023-05-04 03:55:36.000000 libvsbsdl-20230502/libcpath/libcpath_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2336 2023-05-04 03:55:36.000000 libvsbsdl-20230502/libcpath/libcpath_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2023-05-04 03:55:36.000000 libvsbsdl-20230502/libcpath/libcpath_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      807 2023-05-04 03:55:36.000000 libvsbsdl-20230502/libcpath/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2023-05-04 03:55:36.000000 libvsbsdl-20230502/libcpath/libcpath_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2023-05-04 03:55:36.000000 libvsbsdl-20230502/libcpath/libcpath_system_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2023-05-04 03:55:36.000000 libvsbsdl-20230502/libcpath/libcpath_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2023-05-04 03:55:36.000000 libvsbsdl-20230502/libcpath/libcpath_libcsplit.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7170 2023-05-04 03:55:36.000000 libvsbsdl-20230502/libcpath/libcpath_path.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28777 2023-05-04 03:55:57.000000 libvsbsdl-20230502/libcpath/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1990 2023-05-04 03:55:36.000000 libvsbsdl-20230502/libcpath/libcpath_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2023-05-04 03:55:36.000000 libvsbsdl-20230502/libcpath/libcpath_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2023-05-04 03:55:36.000000 libvsbsdl-20230502/libcpath/libcpath_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   176165 2023-05-04 03:55:36.000000 libvsbsdl-20230502/libcpath/libcpath_path.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2023-05-04 03:55:36.000000 libvsbsdl-20230502/libcpath/libcpath_system_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1461 2023-05-04 03:55:36.000000 libvsbsdl-20230502/libcpath/libcpath_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2023-05-04 03:55:36.000000 libvsbsdl-20230502/libcpath/libcpath_libuna.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:14:35.000000 libvsbsdl-20230502/vsbsdltools/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17552 2023-05-03 04:25:19.000000 libvsbsdl-20230502/vsbsdltools/info_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1549 2023-05-02 04:08:33.000000 libvsbsdl-20230502/vsbsdltools/vsbsdltools_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1305 2023-05-02 04:32:50.000000 libvsbsdl-20230502/vsbsdltools/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1211 2023-05-02 04:08:33.000000 libvsbsdl-20230502/vsbsdltools/vsbsdltools_i18n.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1746 2023-05-02 04:08:33.000000 libvsbsdl-20230502/vsbsdltools/vsbsdltools_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4534 2023-05-02 04:08:33.000000 libvsbsdl-20230502/vsbsdltools/vsbsdltools_getopt.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1779 2023-05-02 04:08:33.000000 libvsbsdl-20230502/vsbsdltools/vsbsdltools_libuna.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6634 2023-05-03 04:13:36.000000 libvsbsdl-20230502/vsbsdltools/vsbsdlinfo.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1813 2023-05-02 04:08:33.000000 libvsbsdl-20230502/vsbsdltools/vsbsdltools_getopt.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2639 2023-05-02 04:09:34.000000 libvsbsdl-20230502/vsbsdltools/info_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1476 2023-05-02 04:08:33.000000 libvsbsdl-20230502/vsbsdltools/vsbsdltools_output.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30356 2023-05-04 03:55:58.000000 libvsbsdl-20230502/vsbsdltools/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      984 2023-05-02 04:08:33.000000 libvsbsdl-20230502/vsbsdltools/vsbsdltools_libvsbsdl.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1768 2023-05-02 04:08:33.000000 libvsbsdl-20230502/vsbsdltools/vsbsdltools_signal.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1481 2023-05-02 04:08:33.000000 libvsbsdl-20230502/vsbsdltools/vsbsdltools_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5726 2023-05-02 04:08:33.000000 libvsbsdl-20230502/vsbsdltools/vsbsdltools_signal.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3458 2023-05-02 04:08:33.000000 libvsbsdl-20230502/vsbsdltools/vsbsdltools_output.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1499 2023-05-02 04:08:33.000000 libvsbsdl-20230502/vsbsdltools/vsbsdltools_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1502 2023-05-02 04:08:33.000000 libvsbsdl-20230502/vsbsdltools/vsbsdltools_libclocale.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:14:36.000000 libvsbsdl-20230502/manuals/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1777 2023-05-02 04:08:34.000000 libvsbsdl-20230502/manuals/vsbsdlinfo.1
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5501 2023-05-03 04:15:23.000000 libvsbsdl-20230502/manuals/libvsbsdl.3
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      166 2023-04-29 13:19:51.000000 libvsbsdl-20230502/manuals/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25745 2023-05-04 03:55:57.000000 libvsbsdl-20230502/manuals/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2023-04-29 13:20:19.000000 libvsbsdl-20230502/ABOUT-NLS
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:14:36.000000 libvsbsdl-20230502/msvscpp/
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:14:36.000000 libvsbsdl-20230502/msvscpp/vsbsdl_test_support/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6358 2023-05-02 04:52:41.000000 libvsbsdl-20230502/msvscpp/vsbsdl_test_support/vsbsdl_test_support.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:14:36.000000 libvsbsdl-20230502/msvscpp/vsbsdl_test_io_handle/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5693 2023-05-02 04:52:41.000000 libvsbsdl-20230502/msvscpp/vsbsdl_test_io_handle/vsbsdl_test_io_handle.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:14:36.000000 libvsbsdl-20230502/msvscpp/libfcache/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5237 2023-05-02 04:52:41.000000 libvsbsdl-20230502/msvscpp/libfcache/libfcache.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:14:36.000000 libvsbsdl-20230502/msvscpp/vsbsdl_test_volume/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6519 2023-05-02 04:52:41.000000 libvsbsdl-20230502/msvscpp/vsbsdl_test_volume/vsbsdl_test_volume.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:14:36.000000 libvsbsdl-20230502/msvscpp/libclocale/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4778 2023-05-02 04:52:41.000000 libvsbsdl-20230502/msvscpp/libclocale/libclocale.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:14:36.000000 libvsbsdl-20230502/msvscpp/vsbsdl_test_sector_data/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5952 2023-05-02 04:52:41.000000 libvsbsdl-20230502/msvscpp/vsbsdl_test_sector_data/vsbsdl_test_sector_data.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2023-05-02 04:52:41.000000 libvsbsdl-20230502/msvscpp/Makefile.am
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:14:36.000000 libvsbsdl-20230502/msvscpp/libbfio/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7306 2023-05-02 04:52:41.000000 libvsbsdl-20230502/msvscpp/libbfio/libbfio.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:14:36.000000 libvsbsdl-20230502/msvscpp/vsbsdl_test_error/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5432 2023-05-02 04:52:41.000000 libvsbsdl-20230502/msvscpp/vsbsdl_test_error/vsbsdl_test_error.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26981 2023-05-02 04:52:41.000000 libvsbsdl-20230502/msvscpp/libvsbsdl.sln
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:14:36.000000 libvsbsdl-20230502/msvscpp/pyvsbsdl/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6460 2023-05-02 04:52:41.000000 libvsbsdl-20230502/msvscpp/pyvsbsdl/pyvsbsdl.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:14:36.000000 libvsbsdl-20230502/msvscpp/libcfile/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5597 2023-05-02 04:52:41.000000 libvsbsdl-20230502/msvscpp/libcfile/libcfile.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:14:36.000000 libvsbsdl-20230502/msvscpp/vsbsdl_test_partition/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6192 2023-05-02 04:52:41.000000 libvsbsdl-20230502/msvscpp/vsbsdl_test_partition/vsbsdl_test_partition.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:14:36.000000 libvsbsdl-20230502/msvscpp/libcthreads/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2023-05-02 04:52:41.000000 libvsbsdl-20230502/msvscpp/libcthreads/libcthreads.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:14:36.000000 libvsbsdl-20230502/msvscpp/libcpath/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5183 2023-05-02 04:52:41.000000 libvsbsdl-20230502/msvscpp/libcpath/libcpath.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:14:36.000000 libvsbsdl-20230502/msvscpp/vsbsdlinfo/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6349 2023-05-02 04:52:41.000000 libvsbsdl-20230502/msvscpp/vsbsdlinfo/vsbsdlinfo.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:14:36.000000 libvsbsdl-20230502/msvscpp/libuna/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15387 2023-05-02 04:52:41.000000 libvsbsdl-20230502/msvscpp/libuna/libuna.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:14:36.000000 libvsbsdl-20230502/msvscpp/vsbsdl_test_tools_info_handle/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5794 2023-05-02 04:52:41.000000 libvsbsdl-20230502/msvscpp/vsbsdl_test_tools_info_handle/vsbsdl_test_tools_info_handle.vcproj
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21989 2023-05-04 03:55:57.000000 libvsbsdl-20230502/msvscpp/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:14:36.000000 libvsbsdl-20230502/msvscpp/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2023-05-02 04:52:41.000000 libvsbsdl-20230502/msvscpp/libcerror/libcerror.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:14:36.000000 libvsbsdl-20230502/msvscpp/vsbsdl_test_disklabel/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5946 2023-05-02 04:52:41.000000 libvsbsdl-20230502/msvscpp/vsbsdl_test_disklabel/vsbsdl_test_disklabel.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:14:36.000000 libvsbsdl-20230502/msvscpp/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2023-05-02 04:52:41.000000 libvsbsdl-20230502/msvscpp/libcnotify/libcnotify.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:14:36.000000 libvsbsdl-20230502/msvscpp/vsbsdl_test_partition_entry/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5711 2023-05-02 04:52:41.000000 libvsbsdl-20230502/msvscpp/vsbsdl_test_partition_entry/vsbsdl_test_partition_entry.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:14:36.000000 libvsbsdl-20230502/msvscpp/vsbsdl_test_tools_output/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5629 2023-05-02 04:52:41.000000 libvsbsdl-20230502/msvscpp/vsbsdl_test_tools_output/vsbsdl_test_tools_output.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:14:36.000000 libvsbsdl-20230502/msvscpp/vsbsdl_test_tools_signal/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5629 2023-05-02 04:52:41.000000 libvsbsdl-20230502/msvscpp/vsbsdl_test_tools_signal/vsbsdl_test_tools_signal.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:14:36.000000 libvsbsdl-20230502/msvscpp/libvsbsdl/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8068 2023-05-02 04:52:41.000000 libvsbsdl-20230502/msvscpp/libvsbsdl/libvsbsdl.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:14:36.000000 libvsbsdl-20230502/msvscpp/libfdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6858 2023-05-02 04:52:41.000000 libvsbsdl-20230502/msvscpp/libfdata/libfdata.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:14:36.000000 libvsbsdl-20230502/msvscpp/libcdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6172 2023-05-02 04:52:41.000000 libvsbsdl-20230502/msvscpp/libcdata/libcdata.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:14:36.000000 libvsbsdl-20230502/msvscpp/vsbsdl_test_notify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5520 2023-05-02 04:52:41.000000 libvsbsdl-20230502/msvscpp/vsbsdl_test_notify/vsbsdl_test_notify.vcproj
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:14:36.000000 libvsbsdl-20230502/msvscpp/libcsplit/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5225 2023-05-02 04:52:41.000000 libvsbsdl-20230502/msvscpp/libcsplit/libcsplit.vcproj
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    11497 2023-05-02 04:50:00.000000 libvsbsdl-20230502/setup.py
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49797 2023-05-04 03:55:56.000000 libvsbsdl-20230502/config.guess
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3435 2023-05-02 04:08:31.000000 libvsbsdl-20230502/libvsbsdl.spec.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-02 04:08:31.000000 libvsbsdl-20230502/NEWS
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:14:36.000000 libvsbsdl-20230502/ossfuzz/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2023-04-29 13:19:51.000000 libvsbsdl-20230502/ossfuzz/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2716 2023-05-02 04:08:33.000000 libvsbsdl-20230502/ossfuzz/partition_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2250 2023-05-02 04:08:33.000000 libvsbsdl-20230502/ossfuzz/volume_fuzzer.cc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      977 2023-05-02 04:08:33.000000 libvsbsdl-20230502/ossfuzz/ossfuzz_libvsbsdl.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33004 2023-05-04 03:55:57.000000 libvsbsdl-20230502/ossfuzz/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2023-05-02 04:08:33.000000 libvsbsdl-20230502/ossfuzz/ossfuzz_libbfio.h
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2023-05-04 03:55:58.000000 libvsbsdl-20230502/test-driver
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)  1617870 2023-05-04 03:55:55.000000 libvsbsdl-20230502/configure
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:14:34.000000 libvsbsdl-20230502/libuna/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15532 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_url_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1801 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_mac_symbol.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1259 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_scsu.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2738 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_iso_8859_5.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3610 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_iso_8859_2.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8602 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_windows_1253.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_koi8_u.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7189 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_windows_1252.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19794 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_utf32_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_windows_1257.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9125 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_mac_cyrillic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9435 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_mac_thai.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    95123 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_utf32_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_mac_thai.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8050 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_windows_874.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1628 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_windows_1251.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   484762 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_windows_949.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_iso_8859_6.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_windows_1256.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_mac_greek.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_mac_russian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_mac_ukrainian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2540 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_iso_8859_6.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_windows_874.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8811 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_windows_1251.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10005 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_windows_1256.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2623 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_base16_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_iso_8859_2.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4162 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9076 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_windows_1257.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_windows_1254.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9211 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_windows_1255.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_windows_1253.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5908 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_unicode_character.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_mac_dingbats.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3181 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_scsu.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15485 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_byte_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_mac_celtic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_mac_croatian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_iso_8859_3.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1346 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_iso_8859_15.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9745 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_mac_roman.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_utf32_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9542 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_koi8_r.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_mac_icelandic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_windows_936.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3679 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_base64_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9871 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_mac_celtic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   360710 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_windows_950.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9666 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_utf8_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   430461 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_windows_936.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   129163 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_unicode_character.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   101951 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_utf8_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82226 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_base32_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_windows_950.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_windows_932.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_mac_turkish.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18019 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_utf8_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9088 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_mac_ukrainian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_koi8_r.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39461 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_base16_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_windows_1250.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1783 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_iso_8859_16.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_mac_croatian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10379 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_mac_gaelic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_utf16_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_iso_8859_10.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9394 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_mac_centraleurroman.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   286239 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_windows_932.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2993 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_utf8_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1929 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_url_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11002 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_mac_farsi.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_windows_949.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_mac_romanian.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_mac_gaelic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2629 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_iso_8859_8.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10389 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_mac_arabic.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1644 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_windows_1252.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_windows_1250.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_mac_russian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    98825 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_utf16_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_iso_8859_5.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_iso_8859_4.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2921 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_byte_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_mac_roman.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_utf16_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3561 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_iso_8859_4.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3225 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_iso_8859_10.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_mac_icelandic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    52301 2023-05-04 03:55:57.000000 libvsbsdl-20230502/libuna/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_utf7_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14020 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_mac_symbol.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3704 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_base32_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9844 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_mac_turkish.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10880 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_mac_inuit.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19595 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_utf16_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15691 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_utf7_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_utf32_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3335 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_iso_8859_3.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9078 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_mac_greek.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16696 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_windows_1255.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2823 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_iso_8859_14.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3664 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_iso_8859_13.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_mac_centraleurroman.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_iso_8859_8.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2053 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_iso_8859_9.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_windows_1254.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_mac_cyrillic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_mac_arabic.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9116 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_windows_1258.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_mac_farsi.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_iso_8859_15.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2873 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_iso_8859_7.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10134 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_mac_dingbats.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1340 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_iso_8859_9.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1630 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_windows_1258.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    74767 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_base64_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9953 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_mac_romanian.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9984 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_koi8_u.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1455 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_iso_8859_13.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_iso_8859_7.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_iso_8859_14.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_mac_inuit.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3296 2023-05-04 03:55:45.000000 libvsbsdl-20230502/libuna/libuna_codepage_iso_8859_16.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40587 2023-05-04 03:55:56.000000 libvsbsdl-20230502/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       53 2023-04-28 17:14:35.000000 libvsbsdl-20230502/ChangeLog
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:14:28.000000 libvsbsdl-20230502/m4/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23765 2023-04-29 13:19:51.000000 libvsbsdl-20230502/m4/libuna.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2023-04-29 13:20:19.000000 libvsbsdl-20230502/m4/gettext.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      756 2023-04-29 13:19:51.000000 libvsbsdl-20230502/m4/tests.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2023-04-29 13:20:19.000000 libvsbsdl-20230502/m4/lib-prefix.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2023-05-04 03:55:50.000000 libvsbsdl-20230502/m4/ltoptions.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9379 2023-04-29 13:19:51.000000 libvsbsdl-20230502/m4/libcpath.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2023-04-29 13:20:19.000000 libvsbsdl-20230502/m4/lib-ld.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11112 2023-04-29 13:19:51.000000 libvsbsdl-20230502/m4/libcthreads.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2023-04-29 13:20:19.000000 libvsbsdl-20230502/m4/lib-link.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17674 2023-04-29 13:19:51.000000 libvsbsdl-20230502/m4/python.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2023-05-04 03:55:50.000000 libvsbsdl-20230502/m4/libtool.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-04-29 13:20:19.000000 libvsbsdl-20230502/m4/nls.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8230 2023-04-29 13:19:51.000000 libvsbsdl-20230502/m4/libclocale.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15545 2023-04-29 13:19:51.000000 libvsbsdl-20230502/m4/libfdata.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2023-04-29 13:20:19.000000 libvsbsdl-20230502/m4/host-cpu-c-abi.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5638 2023-04-29 13:19:51.000000 libvsbsdl-20230502/m4/libcnotify.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2023-05-04 03:55:50.000000 libvsbsdl-20230502/m4/ltversion.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17147 2023-04-29 13:19:51.000000 libvsbsdl-20230502/m4/libcdata.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2023-04-29 13:20:19.000000 libvsbsdl-20230502/m4/progtest.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2023-05-04 03:55:50.000000 libvsbsdl-20230502/m4/lt~obsolete.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11498 2023-04-29 13:19:51.000000 libvsbsdl-20230502/m4/libcfile.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2023-04-29 13:20:19.000000 libvsbsdl-20230502/m4/po.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3852 2023-04-29 13:19:51.000000 libvsbsdl-20230502/m4/pthread.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14115 2023-04-29 13:19:51.000000 libvsbsdl-20230502/m4/common.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6260 2023-04-29 13:19:51.000000 libvsbsdl-20230502/m4/libcerror.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2023-04-29 13:20:19.000000 libvsbsdl-20230502/m4/iconv.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2023-05-04 03:55:50.000000 libvsbsdl-20230502/m4/ltsugar.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7325 2023-04-29 13:19:51.000000 libvsbsdl-20230502/m4/libfcache.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7384 2023-04-29 13:19:51.000000 libvsbsdl-20230502/m4/libcsplit.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2023-04-29 13:20:19.000000 libvsbsdl-20230502/m4/intlmacosx.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2023-04-29 13:19:51.000000 libvsbsdl-20230502/m4/types.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11692 2023-04-29 13:19:51.000000 libvsbsdl-20230502/m4/libbfio.m4
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2023-05-02 04:08:31.000000 libvsbsdl-20230502/COPYING.LESSER
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:14:35.000000 libvsbsdl-20230502/pyvsbsdl-python3/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1678 2023-05-02 04:08:31.000000 libvsbsdl-20230502/pyvsbsdl-python3/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41885 2023-05-04 03:55:57.000000 libvsbsdl-20230502/pyvsbsdl-python3/Makefile.in
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:14:30.000000 libvsbsdl-20230502/libcerror/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2023-05-04 03:55:29.000000 libvsbsdl-20230502/libcerror/libcerror_system.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2023-05-04 03:55:29.000000 libvsbsdl-20230502/libcerror/libcerror_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2023-05-04 03:55:29.000000 libvsbsdl-20230502/libcerror/libcerror_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      605 2023-05-04 03:55:29.000000 libvsbsdl-20230502/libcerror/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2023-05-04 03:55:29.000000 libvsbsdl-20230502/libcerror/libcerror_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2023-05-04 03:55:29.000000 libvsbsdl-20230502/libcerror/libcerror_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2023-05-04 03:55:29.000000 libvsbsdl-20230502/libcerror/libcerror_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2023-05-04 03:55:29.000000 libvsbsdl-20230502/libcerror/libcerror_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2023-05-04 03:55:29.000000 libvsbsdl-20230502/libcerror/libcerror_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28124 2023-05-04 03:55:57.000000 libvsbsdl-20230502/libcerror/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2023-05-04 03:55:29.000000 libvsbsdl-20230502/libcerror/libcerror_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2023-05-04 03:55:29.000000 libvsbsdl-20230502/libcerror/libcerror_system.h
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:14:32.000000 libvsbsdl-20230502/libcnotify/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2023-05-04 03:55:35.000000 libvsbsdl-20230502/libcnotify/libcnotify_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2023-05-04 03:55:35.000000 libvsbsdl-20230502/libcnotify/libcnotify_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2023-05-04 03:55:35.000000 libvsbsdl-20230502/libcnotify/libcnotify_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2023-05-04 03:55:35.000000 libvsbsdl-20230502/libcnotify/libcnotify_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      693 2023-05-04 03:55:35.000000 libvsbsdl-20230502/libcnotify/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2023-05-04 03:55:35.000000 libvsbsdl-20230502/libcnotify/libcnotify_print.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2023-05-04 03:55:35.000000 libvsbsdl-20230502/libcnotify/libcnotify_verbose.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2023-05-04 03:55:35.000000 libvsbsdl-20230502/libcnotify/libcnotify_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2023-05-04 03:55:35.000000 libvsbsdl-20230502/libcnotify/libcnotify_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2023-05-04 03:55:35.000000 libvsbsdl-20230502/libcnotify/libcnotify_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28611 2023-05-04 03:55:57.000000 libvsbsdl-20230502/libcnotify/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2023-05-04 03:55:35.000000 libvsbsdl-20230502/libcnotify/libcnotify_print.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2023-05-04 03:55:35.000000 libvsbsdl-20230502/libcnotify/libcnotify_verbose.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2023-05-04 03:55:35.000000 libvsbsdl-20230502/libcnotify/libcnotify_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2023-05-04 03:55:50.000000 libvsbsdl-20230502/ltmain.sh
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2023-05-04 03:55:56.000000 libvsbsdl-20230502/compile
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2023-04-29 13:20:19.000000 libvsbsdl-20230502/config.rpath
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:14:35.000000 libvsbsdl-20230502/libvsbsdl/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2193 2023-05-04 03:56:12.000000 libvsbsdl-20230502/libvsbsdl/libvsbsdl_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19674 2023-05-02 04:08:33.000000 libvsbsdl-20230502/libvsbsdl/libvsbsdl_disklabel.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1813 2023-05-02 04:08:33.000000 libvsbsdl-20230502/libvsbsdl/libvsbsdl_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1457 2023-05-02 04:08:33.000000 libvsbsdl-20230502/libvsbsdl/libvsbsdl_libclocale.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4181 2023-05-02 04:08:33.000000 libvsbsdl-20230502/libvsbsdl/libvsbsdl_debug.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2200 2023-05-02 04:08:33.000000 libvsbsdl-20230502/libvsbsdl/libvsbsdl_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2023-05-02 04:08:33.000000 libvsbsdl-20230502/libvsbsdl/libvsbsdl_libfcache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2162 2023-05-02 04:08:33.000000 libvsbsdl-20230502/libvsbsdl/libvsbsdl_sector_data.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2328 2023-05-02 04:08:33.000000 libvsbsdl-20230502/libvsbsdl/libvsbsdl_partition_entry.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2517 2023-05-02 04:08:33.000000 libvsbsdl-20230502/libvsbsdl/libvsbsdl_disklabel.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28412 2023-05-03 04:18:59.000000 libvsbsdl-20230502/libvsbsdl/libvsbsdl_partition.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30229 2023-05-02 04:08:33.000000 libvsbsdl-20230502/libvsbsdl/libvsbsdl_volume.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3705 2023-05-02 04:08:33.000000 libvsbsdl-20230502/libvsbsdl/libvsbsdl_io_handle.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1603 2023-05-02 04:08:33.000000 libvsbsdl-20230502/libvsbsdl/libvsbsdl_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8423 2023-05-02 04:08:33.000000 libvsbsdl-20230502/libvsbsdl/libvsbsdl_partition_entry.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1998 2023-04-30 05:39:27.000000 libvsbsdl-20230502/libvsbsdl/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1543 2023-05-02 04:08:33.000000 libvsbsdl-20230502/libvsbsdl/libvsbsdl_libfdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1611 2023-05-02 04:08:33.000000 libvsbsdl-20230502/libvsbsdl/libvsbsdl_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1694 2023-05-02 04:08:33.000000 libvsbsdl-20230502/libvsbsdl/libvsbsdl_io_handle.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1086 2023-05-04 03:56:12.000000 libvsbsdl-20230502/libvsbsdl/libvsbsdl.rc
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1701 2023-05-02 04:08:33.000000 libvsbsdl-20230502/libvsbsdl/libvsbsdl_libbfio.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1698 2023-05-02 04:08:33.000000 libvsbsdl-20230502/libvsbsdl/vsbsdl_partition_entry.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1834 2023-05-02 04:08:33.000000 libvsbsdl-20230502/libvsbsdl/libvsbsdl.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2195 2023-05-02 04:08:33.000000 libvsbsdl-20230502/libvsbsdl/libvsbsdl_definitions.h.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1397 2023-05-02 04:08:33.000000 libvsbsdl-20230502/libvsbsdl/libvsbsdl_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3580 2023-05-02 04:08:33.000000 libvsbsdl-20230502/libvsbsdl/vsbsdl_disklabel.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1436 2023-05-02 04:08:33.000000 libvsbsdl-20230502/libvsbsdl/libvsbsdl_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1454 2023-05-02 04:08:33.000000 libvsbsdl-20230502/libvsbsdl/libvsbsdl_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1546 2023-05-02 04:08:33.000000 libvsbsdl-20230502/libvsbsdl/libvsbsdl_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1382 2023-05-02 04:08:33.000000 libvsbsdl-20230502/libvsbsdl/libvsbsdl_debug.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3800 2023-05-02 04:08:33.000000 libvsbsdl-20230502/libvsbsdl/libvsbsdl_volume.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2919 2023-05-02 04:08:33.000000 libvsbsdl-20230502/libvsbsdl/libvsbsdl_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1411 2023-05-02 04:08:33.000000 libvsbsdl-20230502/libvsbsdl/libvsbsdl_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33451 2023-05-04 03:55:57.000000 libvsbsdl-20230502/libvsbsdl/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1927 2023-05-02 04:08:33.000000 libvsbsdl-20230502/libvsbsdl/libvsbsdl_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8830 2023-05-02 04:08:33.000000 libvsbsdl-20230502/libvsbsdl/libvsbsdl_sector_data.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9800 2023-05-03 04:13:57.000000 libvsbsdl-20230502/libvsbsdl/libvsbsdl_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4230 2023-05-03 04:16:12.000000 libvsbsdl-20230502/libvsbsdl/libvsbsdl_partition.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2761 2023-05-02 04:08:33.000000 libvsbsdl-20230502/libvsbsdl/libvsbsdl_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1088 2023-05-02 04:08:33.000000 libvsbsdl-20230502/libvsbsdl/libvsbsdl.rc.in
--rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2023-05-04 03:55:58.000000 libvsbsdl-20230502/depcomp
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:14:36.000000 libvsbsdl-20230502/po/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2023-04-29 13:20:19.000000 libvsbsdl-20230502/po/en@quot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2023-04-29 13:20:19.000000 libvsbsdl-20230502/po/Rules-quot
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2023-04-29 13:19:51.000000 libvsbsdl-20230502/po/POTFILES.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2023-04-29 13:20:19.000000 libvsbsdl-20230502/po/remove-potcdate.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1808 2023-04-29 13:19:51.000000 libvsbsdl-20230502/po/Makevars.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       50 2023-04-29 13:19:51.000000 libvsbsdl-20230502/po/ChangeLog
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2023-04-29 13:20:19.000000 libvsbsdl-20230502/po/en@boldquot.header
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2023-04-29 13:20:19.000000 libvsbsdl-20230502/po/quot.sed
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1811 2023-05-04 03:56:12.000000 libvsbsdl-20230502/po/Makevars
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2023-04-29 13:20:19.000000 libvsbsdl-20230502/po/insert-header.sin
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2023-04-29 13:20:19.000000 libvsbsdl-20230502/po/Makefile.in.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2023-04-29 13:20:19.000000 libvsbsdl-20230502/po/boldquot.sed
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2678 2023-05-04 03:56:12.000000 libvsbsdl-20230502/libvsbsdl.spec
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:14:34.000000 libvsbsdl-20230502/libfdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2804 2023-05-04 03:55:42.000000 libvsbsdl-20230502/libfdata/libfdata_segments_array.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2023-05-04 03:55:42.000000 libvsbsdl-20230502/libfdata/libfdata_cache.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1172 2023-05-04 03:55:42.000000 libvsbsdl-20230502/libfdata/libfdata_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19329 2023-05-04 03:55:42.000000 libvsbsdl-20230502/libfdata/libfdata_list_element.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1995 2023-05-04 03:55:42.000000 libvsbsdl-20230502/libfdata/libfdata_mapped_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2023-05-04 03:55:42.000000 libvsbsdl-20230502/libfdata/libfdata_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   107689 2023-05-04 03:55:42.000000 libvsbsdl-20230502/libfdata/libfdata_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2023-05-04 03:55:42.000000 libvsbsdl-20230502/libfdata/libfdata_libcdata.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2023-05-04 03:55:42.000000 libvsbsdl-20230502/libfdata/libfdata_notify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6013 2023-05-04 03:55:42.000000 libvsbsdl-20230502/libfdata/libfdata_range_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1256 2023-05-04 03:55:42.000000 libvsbsdl-20230502/libfdata/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2023-05-04 03:55:42.000000 libvsbsdl-20230502/libfdata/libfdata_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12090 2023-05-04 03:55:42.000000 libvsbsdl-20230502/libfdata/libfdata_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7327 2023-05-04 03:55:42.000000 libvsbsdl-20230502/libfdata/libfdata_area.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2054 2023-05-04 03:55:42.000000 libvsbsdl-20230502/libfdata/libfdata_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37893 2023-05-04 03:55:42.000000 libvsbsdl-20230502/libfdata/libfdata_area.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2092 2023-05-04 03:55:42.000000 libvsbsdl-20230502/libfdata/libfdata_range.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49670 2023-05-04 03:55:42.000000 libvsbsdl-20230502/libfdata/libfdata_vector.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9700 2023-05-04 03:55:42.000000 libvsbsdl-20230502/libfdata/libfdata_stream.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7810 2023-05-04 03:55:42.000000 libvsbsdl-20230502/libfdata/libfdata_vector.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2023-05-04 03:55:42.000000 libvsbsdl-20230502/libfdata/libfdata_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2023-05-04 03:55:42.000000 libvsbsdl-20230502/libfdata/libfdata_libfcache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2023-05-04 03:55:42.000000 libvsbsdl-20230502/libfdata/libfdata_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30931 2023-05-04 03:55:42.000000 libvsbsdl-20230502/libfdata/libfdata_range_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2023-05-04 03:55:42.000000 libvsbsdl-20230502/libfdata/libfdata_libcnotify.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2023-05-04 03:55:42.000000 libvsbsdl-20230502/libfdata/libfdata_notify.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3999 2023-05-04 03:55:42.000000 libvsbsdl-20230502/libfdata/libfdata_list_element.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2023-05-04 03:55:42.000000 libvsbsdl-20230502/libfdata/libfdata_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2023-05-04 03:55:42.000000 libvsbsdl-20230502/libfdata/libfdata_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31964 2023-05-04 03:55:57.000000 libvsbsdl-20230502/libfdata/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1491 2023-05-04 03:55:42.000000 libvsbsdl-20230502/libfdata/libfdata_cache.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    66203 2023-05-04 03:55:42.000000 libvsbsdl-20230502/libfdata/libfdata_stream.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21271 2023-05-04 03:55:42.000000 libvsbsdl-20230502/libfdata/libfdata_segments_array.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6826 2023-05-04 03:55:42.000000 libvsbsdl-20230502/libfdata/libfdata_mapped_range.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6533 2023-05-04 03:55:42.000000 libvsbsdl-20230502/libfdata/libfdata_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7149 2023-05-04 03:55:42.000000 libvsbsdl-20230502/libfdata/libfdata_range.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:14:31.000000 libvsbsdl-20230502/libcdata/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49968 2023-05-04 03:55:28.000000 libvsbsdl-20230502/libcdata/libcdata_array.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37549 2023-05-04 03:55:28.000000 libvsbsdl-20230502/libcdata/libcdata_btree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100501 2023-05-04 03:55:28.000000 libvsbsdl-20230502/libcdata/libcdata_tree_node.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2023-05-04 03:55:28.000000 libvsbsdl-20230502/libcdata/libcdata_libcthreads.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2789 2023-05-04 03:55:28.000000 libvsbsdl-20230502/libcdata/libcdata_range_list_value.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2023-05-04 03:55:28.000000 libvsbsdl-20230502/libcdata/libcdata_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12295 2023-05-04 03:55:28.000000 libvsbsdl-20230502/libcdata/libcdata_range_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1092 2023-05-04 03:55:28.000000 libvsbsdl-20230502/libcdata/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   122285 2023-05-04 03:55:28.000000 libvsbsdl-20230502/libcdata/libcdata_range_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2023-05-04 03:55:28.000000 libvsbsdl-20230502/libcdata/libcdata_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2023-05-04 03:55:28.000000 libvsbsdl-20230502/libcdata/libcdata_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3871 2023-05-04 03:55:28.000000 libvsbsdl-20230502/libcdata/libcdata_list_element.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5251 2023-05-04 03:55:28.000000 libvsbsdl-20230502/libcdata/libcdata_btree_values_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10647 2023-05-04 03:55:28.000000 libvsbsdl-20230502/libcdata/libcdata_range_list_value.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2023-05-04 03:55:28.000000 libvsbsdl-20230502/libcdata/libcdata_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2023-05-04 03:55:28.000000 libvsbsdl-20230502/libcdata/libcdata_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2023-05-04 03:55:28.000000 libvsbsdl-20230502/libcdata/libcdata_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2023-05-04 03:55:28.000000 libvsbsdl-20230502/libcdata/libcdata_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2960 2023-05-04 03:55:28.000000 libvsbsdl-20230502/libcdata/libcdata_btree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69515 2023-05-04 03:55:28.000000 libvsbsdl-20230502/libcdata/libcdata_list.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8365 2023-05-04 03:55:28.000000 libvsbsdl-20230502/libcdata/libcdata_tree_node.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6448 2023-05-04 03:55:28.000000 libvsbsdl-20230502/libcdata/libcdata_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2023-05-04 03:55:28.000000 libvsbsdl-20230502/libcdata/libcdata_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23846 2023-05-04 03:55:28.000000 libvsbsdl-20230502/libcdata/libcdata_list_element.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31183 2023-05-04 03:55:57.000000 libvsbsdl-20230502/libcdata/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2023-05-04 03:55:28.000000 libvsbsdl-20230502/libcdata/libcdata_btree_values_list.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5231 2023-05-04 03:55:28.000000 libvsbsdl-20230502/libcdata/libcdata_array.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3790 2023-05-04 03:55:28.000000 libvsbsdl-20230502/libcdata/libcdata_btree.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2023-05-04 03:55:28.000000 libvsbsdl-20230502/libcdata/libcdata_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22358 2023-05-04 03:55:28.000000 libvsbsdl-20230502/libcdata/libcdata_btree.c
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:14:35.000000 libvsbsdl-20230502/pyvsbsdl-python2/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1678 2023-05-02 04:08:31.000000 libvsbsdl-20230502/pyvsbsdl-python2/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41885 2023-05-04 03:55:57.000000 libvsbsdl-20230502/pyvsbsdl-python2/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1219 2023-05-02 04:08:31.000000 libvsbsdl-20230502/acinclude.m4
-drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-04 04:14:32.000000 libvsbsdl-20230502/libcsplit/
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1679 2023-05-04 03:55:37.000000 libvsbsdl-20230502/libcsplit/libcsplit_types.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1471 2023-05-04 03:55:37.000000 libvsbsdl-20230502/libcsplit/libcsplit_wide_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2023-05-04 03:55:37.000000 libvsbsdl-20230502/libcsplit/libcsplit_error.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2023-05-04 03:55:37.000000 libvsbsdl-20230502/libcsplit/libcsplit_support.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13912 2023-05-04 03:55:37.000000 libvsbsdl-20230502/libcsplit/libcsplit_narrow_split_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2849 2023-05-04 03:55:37.000000 libvsbsdl-20230502/libcsplit/libcsplit_narrow_split_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      849 2023-05-04 03:55:37.000000 libvsbsdl-20230502/libcsplit/Makefile.am
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13944 2023-05-04 03:55:37.000000 libvsbsdl-20230502/libcsplit/libcsplit_wide_split_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1386 2023-05-04 03:55:37.000000 libvsbsdl-20230502/libcsplit/libcsplit_narrow_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2023-05-04 03:55:37.000000 libvsbsdl-20230502/libcsplit/libcsplit_unused.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6206 2023-05-04 03:55:37.000000 libvsbsdl-20230502/libcsplit/libcsplit_wide_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6125 2023-05-04 03:55:37.000000 libvsbsdl-20230502/libcsplit/libcsplit_narrow_string.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29557 2023-05-04 03:55:57.000000 libvsbsdl-20230502/libcsplit/Makefile.in
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2920 2023-05-04 03:55:37.000000 libvsbsdl-20230502/libcsplit/libcsplit_wide_split_string.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1360 2023-05-04 03:55:37.000000 libvsbsdl-20230502/libcsplit/libcsplit_definitions.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2023-05-04 03:55:37.000000 libvsbsdl-20230502/libcsplit/libcsplit_error.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2023-05-04 03:55:37.000000 libvsbsdl-20230502/libcsplit/libcsplit_support.c
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2023-05-04 03:55:37.000000 libvsbsdl-20230502/libcsplit/libcsplit_libcerror.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2023-05-04 03:55:37.000000 libvsbsdl-20230502/libcsplit/libcsplit_extern.h
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7128 2023-05-02 04:08:31.000000 libvsbsdl-20230502/configure.ac
--rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      428 2023-05-04 04:14:37.635500 libvsbsdl-20230502/PKG-INFO
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 06:05:36.000000 libvsbsdl-20230506/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 06:05:35.000000 libvsbsdl-20230506/libfcache/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2023-05-06 05:35:59.000000 libvsbsdl-20230506/libfcache/libfcache_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1619 2023-05-06 05:35:59.000000 libvsbsdl-20230506/libfcache/libfcache_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3806 2023-05-06 05:35:59.000000 libvsbsdl-20230506/libfcache/libfcache_cache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2023-05-06 05:35:59.000000 libvsbsdl-20230506/libfcache/libfcache_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1178 2023-05-06 05:35:59.000000 libvsbsdl-20230506/libfcache/libfcache_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      845 2023-05-06 05:35:59.000000 libvsbsdl-20230506/libfcache/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1551 2023-05-06 05:35:59.000000 libvsbsdl-20230506/libfcache/libfcache_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2023-05-06 05:35:59.000000 libvsbsdl-20230506/libfcache/libfcache_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2023-05-06 05:35:59.000000 libvsbsdl-20230506/libfcache/libfcache_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1680 2023-05-06 05:35:59.000000 libvsbsdl-20230506/libfcache/libfcache_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3161 2023-05-06 05:35:59.000000 libvsbsdl-20230506/libfcache/libfcache_cache_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12461 2023-05-06 05:35:59.000000 libvsbsdl-20230506/libfcache/libfcache_cache_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29208 2023-05-06 05:36:29.000000 libvsbsdl-20230506/libfcache/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2023-05-06 05:35:59.000000 libvsbsdl-20230506/libfcache/libfcache_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2259 2023-05-06 05:35:59.000000 libvsbsdl-20230506/libfcache/libfcache_date_time.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26186 2023-05-06 05:35:59.000000 libvsbsdl-20230506/libfcache/libfcache_cache.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2023-05-06 05:35:59.000000 libvsbsdl-20230506/libfcache/libfcache_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1250 2023-05-06 05:35:59.000000 libvsbsdl-20230506/libfcache/libfcache_date_time.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 06:05:34.000000 libvsbsdl-20230506/common/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2023-05-05 05:07:36.000000 libvsbsdl-20230506/common/config_msc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10432 2023-05-05 05:07:36.000000 libvsbsdl-20230506/common/byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1245 2023-05-05 05:07:36.000000 libvsbsdl-20230506/common/common.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4606 2023-05-05 05:07:36.000000 libvsbsdl-20230506/common/system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      378 2023-05-05 05:07:33.000000 libvsbsdl-20230506/common/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7370 2023-05-06 05:37:04.000000 libvsbsdl-20230506/common/types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7370 2023-05-05 05:07:36.000000 libvsbsdl-20230506/common/types.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2377 2023-05-05 05:07:36.000000 libvsbsdl-20230506/common/config_winapi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3254 2023-05-05 05:07:36.000000 libvsbsdl-20230506/common/memory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16355 2023-05-06 05:37:04.000000 libvsbsdl-20230506/common/config.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5414 2023-05-05 05:07:36.000000 libvsbsdl-20230506/common/narrow_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23779 2023-05-06 05:36:28.000000 libvsbsdl-20230506/common/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3873 2023-05-05 05:07:36.000000 libvsbsdl-20230506/common/file_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      952 2023-05-05 05:07:36.000000 libvsbsdl-20230506/common/config_borlandc.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15432 2023-05-06 05:36:22.000000 libvsbsdl-20230506/common/config.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5059 2023-05-05 05:07:36.000000 libvsbsdl-20230506/common/wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      650 2023-05-05 05:07:33.000000 libvsbsdl-20230506/libvsbsdl.pc.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 06:05:36.000000 libvsbsdl-20230506/tests/
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3862 2023-05-05 05:08:27.000000 libvsbsdl-20230506/tests/test_library.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5044 2023-05-05 05:07:37.000000 libvsbsdl-20230506/tests/pyvsbsdl_test_volume.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      984 2023-05-05 05:07:37.000000 libvsbsdl-20230506/tests/vsbsdl_test_libvsbsdl.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9434 2023-05-05 05:08:20.000000 libvsbsdl-20230506/tests/vsbsdl_test_partition_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4742 2023-05-05 05:07:37.000000 libvsbsdl-20230506/tests/vsbsdl_test_memory.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1709 2023-05-05 05:07:37.000000 libvsbsdl-20230506/tests/vsbsdl_test_rwlock.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3430 2023-05-05 05:07:37.000000 libvsbsdl-20230506/tests/test_python_module.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6652 2023-05-05 05:08:20.000000 libvsbsdl-20230506/tests/vsbsdl_test_rwlock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6502 2023-05-05 05:08:20.000000 libvsbsdl-20230506/tests/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3174 2023-05-05 05:07:37.000000 libvsbsdl-20230506/tests/vsbsdl_test_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1707 2023-05-05 05:07:37.000000 libvsbsdl-20230506/tests/vsbsdl_test_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13266 2023-05-05 05:07:37.000000 libvsbsdl-20230506/tests/vsbsdl_test_functions.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23239 2023-05-05 05:08:20.000000 libvsbsdl-20230506/tests/vsbsdl_test_disklabel.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1460 2023-05-05 05:07:37.000000 libvsbsdl-20230506/tests/vsbsdl_test_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1813 2023-05-05 05:07:37.000000 libvsbsdl-20230506/tests/vsbsdl_test_getopt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4534 2023-05-05 05:07:37.000000 libvsbsdl-20230506/tests/vsbsdl_test_getopt.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2464 2023-05-05 05:07:37.000000 libvsbsdl-20230506/tests/vsbsdl_test_tools_output.c
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     3805 2023-05-05 05:08:27.000000 libvsbsdl-20230506/tests/test_tools.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8604 2023-05-05 05:07:37.000000 libvsbsdl-20230506/tests/vsbsdl_test_macros.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31469 2023-05-05 05:08:20.000000 libvsbsdl-20230506/tests/vsbsdl_test_volume.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1442 2023-05-05 05:07:37.000000 libvsbsdl-20230506/tests/vsbsdl_test_libcerror.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     1653 2023-05-05 05:07:37.000000 libvsbsdl-20230506/tests/test_manpage.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1463 2023-05-05 05:07:37.000000 libvsbsdl-20230506/tests/vsbsdl_test_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    57176 2023-05-05 05:08:20.000000 libvsbsdl-20230506/tests/vsbsdl_test_partition.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4210 2023-05-05 05:07:37.000000 libvsbsdl-20230506/tests/vsbsdl_test_tools_signal.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9140 2023-05-05 05:07:37.000000 libvsbsdl-20230506/tests/pyvsbsdl_test_partition.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37792 2023-05-05 05:07:37.000000 libvsbsdl-20230506/tests/test_runner.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1555 2023-05-05 05:07:37.000000 libvsbsdl-20230506/tests/pyvsbsdl_test_support.py
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1549 2023-05-05 05:07:37.000000 libvsbsdl-20230506/tests/vsbsdl_test_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    59388 2023-05-06 05:36:31.000000 libvsbsdl-20230506/tests/Makefile.in
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     2174 2023-05-05 05:07:37.000000 libvsbsdl-20230506/tests/test_vsbsdlinfo.sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9709 2023-05-05 05:08:20.000000 libvsbsdl-20230506/tests/vsbsdl_test_sector_data.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1708 2023-05-05 05:07:37.000000 libvsbsdl-20230506/tests/vsbsdl_test_memory.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8150 2023-05-05 05:08:20.000000 libvsbsdl-20230506/tests/vsbsdl_test_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5673 2023-05-05 05:07:37.000000 libvsbsdl-20230506/tests/vsbsdl_test_tools_info_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14574 2023-05-05 05:07:37.000000 libvsbsdl-20230506/tests/vsbsdl_test_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4365 2023-05-05 05:07:37.000000 libvsbsdl-20230506/tests/vsbsdl_test_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1740 2023-05-05 05:07:37.000000 libvsbsdl-20230506/tests/vsbsdl_test_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1816 2023-05-05 05:07:37.000000 libvsbsdl-20230506/tests/vsbsdl_test_functions.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 06:05:34.000000 libvsbsdl-20230506/libclocale/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1696 2023-05-06 05:35:47.000000 libvsbsdl-20230506/libclocale/libclocale_wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3094 2023-05-06 05:35:47.000000 libvsbsdl-20230506/libclocale/libclocale_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1717 2023-05-06 05:35:47.000000 libvsbsdl-20230506/libclocale/libclocale_locale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      744 2023-05-06 05:35:47.000000 libvsbsdl-20230506/libclocale/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10671 2023-05-06 05:35:47.000000 libvsbsdl-20230506/libclocale/libclocale_locale.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2023-05-06 05:35:47.000000 libvsbsdl-20230506/libclocale/libclocale_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2023-05-06 05:35:47.000000 libvsbsdl-20230506/libclocale/libclocale_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1412 2023-05-06 05:35:47.000000 libvsbsdl-20230506/libclocale/libclocale_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3412 2023-05-06 05:35:47.000000 libvsbsdl-20230506/libclocale/libclocale_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1961 2023-05-06 05:35:47.000000 libvsbsdl-20230506/libclocale/libclocale_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21033 2023-05-06 05:35:47.000000 libvsbsdl-20230506/libclocale/libclocale_codepage.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28735 2023-05-06 05:36:29.000000 libvsbsdl-20230506/libclocale/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1969 2023-05-06 05:35:47.000000 libvsbsdl-20230506/libclocale/libclocale_wide_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2023-05-06 05:35:47.000000 libvsbsdl-20230506/libclocale/libclocale_libcerror.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     6878 2023-05-06 05:36:27.000000 libvsbsdl-20230506/missing
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3193 2023-04-29 13:19:51.000000 libvsbsdl-20230506/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    55932 2023-05-06 05:36:19.000000 libvsbsdl-20230506/aclocal.m4
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 06:05:35.000000 libvsbsdl-20230506/libbfio/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8883 2023-05-06 05:35:22.000000 libvsbsdl-20230506/libbfio/libbfio_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1435 2023-05-06 05:35:22.000000 libvsbsdl-20230506/libbfio/libbfio_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    64816 2023-05-06 05:35:22.000000 libvsbsdl-20230506/libbfio/libbfio_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1733 2023-05-06 05:35:22.000000 libvsbsdl-20230506/libbfio/libbfio_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2708 2023-05-06 05:35:22.000000 libvsbsdl-20230506/libbfio/libbfio_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2023-05-06 05:35:22.000000 libvsbsdl-20230506/libbfio/libbfio_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2614 2023-05-06 05:35:22.000000 libvsbsdl-20230506/libbfio/libbfio_codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1545 2023-05-06 05:35:22.000000 libvsbsdl-20230506/libbfio/libbfio_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1376 2023-05-06 05:35:22.000000 libvsbsdl-20230506/libbfio/libbfio_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12186 2023-05-06 05:35:22.000000 libvsbsdl-20230506/libbfio/libbfio_file_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    27543 2023-05-06 05:35:22.000000 libvsbsdl-20230506/libbfio/libbfio_file_range_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2023-05-06 05:35:22.000000 libvsbsdl-20230506/libbfio/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10798 2023-05-06 05:35:22.000000 libvsbsdl-20230506/libbfio/libbfio_file_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10899 2023-05-06 05:35:22.000000 libvsbsdl-20230506/libbfio/libbfio_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6841 2023-05-06 05:35:22.000000 libvsbsdl-20230506/libbfio/libbfio_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2630 2023-05-06 05:35:22.000000 libvsbsdl-20230506/libbfio/libbfio_file_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2814 2023-05-06 05:35:22.000000 libvsbsdl-20230506/libbfio/libbfio_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4085 2023-05-06 05:35:22.000000 libvsbsdl-20230506/libbfio/libbfio_file_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21082 2023-05-06 05:35:22.000000 libvsbsdl-20230506/libbfio/libbfio_memory_range_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2234 2023-05-06 05:35:22.000000 libvsbsdl-20230506/libbfio/libbfio_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2324 2023-05-06 05:35:22.000000 libvsbsdl-20230506/libbfio/libbfio_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2077 2023-05-06 05:35:22.000000 libvsbsdl-20230506/libbfio/libbfio_file_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3835 2023-05-06 05:35:22.000000 libvsbsdl-20230506/libbfio/libbfio_memory_range_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1772 2023-05-06 05:35:22.000000 libvsbsdl-20230506/libbfio/libbfio_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1918 2023-05-06 05:35:22.000000 libvsbsdl-20230506/libbfio/libbfio_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25540 2023-05-06 05:35:22.000000 libvsbsdl-20230506/libbfio/libbfio_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2023-05-06 05:35:22.000000 libvsbsdl-20230506/libbfio/libbfio_memory_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4806 2023-05-06 05:35:22.000000 libvsbsdl-20230506/libbfio/libbfio_file_range_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5821 2023-05-06 05:35:22.000000 libvsbsdl-20230506/libbfio/libbfio_memory_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    32241 2023-05-06 05:36:29.000000 libvsbsdl-20230506/libbfio/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    81879 2023-05-06 05:35:22.000000 libvsbsdl-20230506/libbfio/libbfio_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1400 2023-05-06 05:35:22.000000 libvsbsdl-20230506/libbfio/libbfio_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1362 2023-05-06 05:35:22.000000 libvsbsdl-20230506/libbfio/libbfio_libcpath.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1420 2023-05-06 05:35:22.000000 libvsbsdl-20230506/libbfio/libbfio_libcfile.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2023-05-06 05:35:22.000000 libvsbsdl-20230506/libbfio/libbfio_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26845 2023-05-06 05:35:22.000000 libvsbsdl-20230506/libbfio/libbfio_file_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2896 2023-05-06 05:35:22.000000 libvsbsdl-20230506/libbfio/libbfio_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1572 2023-05-06 05:35:22.000000 libvsbsdl-20230506/libbfio/libbfio_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    35149 2023-05-05 05:07:33.000000 libvsbsdl-20230506/COPYING
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      316 2023-05-05 05:07:33.000000 libvsbsdl-20230506/README
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 06:05:34.000000 libvsbsdl-20230506/include/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      509 2023-05-05 05:07:33.000000 libvsbsdl-20230506/include/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11038 2023-05-06 05:37:04.000000 libvsbsdl-20230506/include/libvsbsdl.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26799 2023-05-06 05:36:28.000000 libvsbsdl-20230506/include/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11038 2023-05-05 05:07:36.000000 libvsbsdl-20230506/include/libvsbsdl.h.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 06:05:34.000000 libvsbsdl-20230506/include/libvsbsdl/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1813 2023-05-05 05:07:36.000000 libvsbsdl-20230506/include/libvsbsdl/definitions.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1431 2023-05-05 05:07:36.000000 libvsbsdl-20230506/include/libvsbsdl/extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4857 2023-05-06 05:37:04.000000 libvsbsdl-20230506/include/libvsbsdl/types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1558 2023-05-05 05:07:36.000000 libvsbsdl-20230506/include/libvsbsdl/features.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4988 2023-05-05 05:07:36.000000 libvsbsdl-20230506/include/libvsbsdl/types.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1494 2023-05-06 05:37:04.000000 libvsbsdl-20230506/include/libvsbsdl/features.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1811 2023-05-06 05:37:04.000000 libvsbsdl-20230506/include/libvsbsdl/definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5417 2023-05-05 05:07:36.000000 libvsbsdl-20230506/include/libvsbsdl/codepage.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6821 2023-05-05 05:07:36.000000 libvsbsdl-20230506/include/libvsbsdl/error.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    15358 2023-05-06 05:36:27.000000 libvsbsdl-20230506/install-sh
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15766 2023-05-06 05:36:27.000000 libvsbsdl-20230506/INSTALL
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 06:05:34.000000 libvsbsdl-20230506/dpkg/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      122 2023-05-05 05:07:33.000000 libvsbsdl-20230506/dpkg/changelog.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      141 2023-05-06 05:37:04.000000 libvsbsdl-20230506/dpkg/changelog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1023 2023-05-05 05:07:37.000000 libvsbsdl-20230506/dpkg/copyright
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       96 2023-05-05 05:07:33.000000 libvsbsdl-20230506/dpkg/libvsbsdl-dev.install
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 06:05:34.000000 libvsbsdl-20230506/dpkg/source/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       12 2023-05-05 05:07:33.000000 libvsbsdl-20230506/dpkg/source/format
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       22 2023-05-05 05:07:33.000000 libvsbsdl-20230506/dpkg/libvsbsdl.install
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      778 2023-05-05 05:07:33.000000 libvsbsdl-20230506/dpkg/rules
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        3 2023-05-05 05:07:33.000000 libvsbsdl-20230506/dpkg/compat
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2181 2023-05-05 05:07:33.000000 libvsbsdl-20230506/dpkg/control
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 06:05:35.000000 libvsbsdl-20230506/pyvsbsdl/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2023-05-05 05:07:37.000000 libvsbsdl-20230506/pyvsbsdl/pyvsbsdl_integer.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      976 2023-05-05 05:07:37.000000 libvsbsdl-20230506/pyvsbsdl/pyvsbsdl_libvsbsdl.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8889 2023-05-05 05:07:37.000000 libvsbsdl-20230506/pyvsbsdl/pyvsbsdl_integer.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1201 2023-04-29 13:19:51.000000 libvsbsdl-20230506/pyvsbsdl/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9366 2023-05-05 05:07:37.000000 libvsbsdl-20230506/pyvsbsdl/pyvsbsdl_partitions.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2940 2023-05-05 05:07:37.000000 libvsbsdl-20230506/pyvsbsdl/pyvsbsdl_partition.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1523 2023-05-05 05:07:37.000000 libvsbsdl-20230506/pyvsbsdl/pyvsbsdl_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9561 2023-05-05 05:07:37.000000 libvsbsdl-20230506/pyvsbsdl/pyvsbsdl_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33959 2023-05-05 05:07:37.000000 libvsbsdl-20230506/pyvsbsdl/pyvsbsdl_file_object_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1544 2023-05-05 05:07:37.000000 libvsbsdl-20230506/pyvsbsdl/pyvsbsdl_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2463 2023-05-05 05:07:37.000000 libvsbsdl-20230506/pyvsbsdl/pyvsbsdl_partitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1403 2023-05-05 05:07:37.000000 libvsbsdl-20230506/pyvsbsdl/pyvsbsdl_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22303 2023-05-05 05:08:20.000000 libvsbsdl-20230506/pyvsbsdl/pyvsbsdl_volume.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1876 2023-05-05 05:07:37.000000 libvsbsdl-20230506/pyvsbsdl/pyvsbsdl.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41530 2023-05-06 05:36:30.000000 libvsbsdl-20230506/pyvsbsdl/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14918 2023-05-05 05:07:37.000000 libvsbsdl-20230506/pyvsbsdl/pyvsbsdl.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1433 2023-05-05 05:07:37.000000 libvsbsdl-20230506/pyvsbsdl/pyvsbsdl_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2031 2023-05-05 05:07:37.000000 libvsbsdl-20230506/pyvsbsdl/pyvsbsdl_python.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1454 2023-05-05 05:07:37.000000 libvsbsdl-20230506/pyvsbsdl/pyvsbsdl_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4151 2023-05-05 05:07:37.000000 libvsbsdl-20230506/pyvsbsdl/pyvsbsdl_file_object_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2867 2023-05-05 05:07:37.000000 libvsbsdl-20230506/pyvsbsdl/pyvsbsdl_volume.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    24351 2023-05-05 05:08:20.000000 libvsbsdl-20230506/pyvsbsdl/pyvsbsdl_partition.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 06:05:35.000000 libvsbsdl-20230506/libcfile/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   105597 2023-05-06 05:35:27.000000 libvsbsdl-20230506/libcfile/libcfile_file.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2023-05-06 05:35:27.000000 libvsbsdl-20230506/libcfile/libcfile_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25753 2023-05-06 05:35:27.000000 libvsbsdl-20230506/libcfile/libcfile_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2389 2023-05-06 05:35:27.000000 libvsbsdl-20230506/libcfile/libcfile_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2023-05-06 05:35:27.000000 libvsbsdl-20230506/libcfile/libcfile_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18388 2023-05-06 05:35:27.000000 libvsbsdl-20230506/libcfile/libcfile_winapi.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      907 2023-05-06 05:35:29.000000 libvsbsdl-20230506/libcfile/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2023-05-06 05:35:27.000000 libvsbsdl-20230506/libcfile/libcfile_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2023-05-06 05:35:27.000000 libvsbsdl-20230506/libcfile/libcfile_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3107 2023-05-06 05:35:27.000000 libvsbsdl-20230506/libcfile/libcfile_winapi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1497 2023-05-06 05:35:27.000000 libvsbsdl-20230506/libcfile/libcfile_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2023-05-06 05:35:27.000000 libvsbsdl-20230506/libcfile/libcfile_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2023-05-06 05:35:27.000000 libvsbsdl-20230506/libcfile/libcfile_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2879 2023-05-06 05:35:29.000000 libvsbsdl-20230506/libcfile/libcfile_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6452 2023-05-06 05:35:27.000000 libvsbsdl-20230506/libcfile/libcfile_file.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2023-05-06 05:35:27.000000 libvsbsdl-20230506/libcfile/libcfile_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2023-05-06 05:35:27.000000 libvsbsdl-20230506/libcfile/libcfile_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29499 2023-05-06 05:36:29.000000 libvsbsdl-20230506/libcfile/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2023-05-06 05:35:27.000000 libvsbsdl-20230506/libcfile/libcfile_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2023-05-06 05:35:27.000000 libvsbsdl-20230506/libcfile/libcfile_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2023-05-06 05:35:27.000000 libvsbsdl-20230506/libcfile/libcfile_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2023-05-06 05:35:27.000000 libvsbsdl-20230506/libcfile/libcfile_notify.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 06:05:34.000000 libvsbsdl-20230506/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4175 2023-05-06 05:35:57.000000 libvsbsdl-20230506/libcthreads/libcthreads_thread_pool.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    43321 2023-05-06 05:35:57.000000 libvsbsdl-20230506/libcthreads/libcthreads_thread_pool.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17481 2023-05-06 05:35:57.000000 libvsbsdl-20230506/libcthreads/libcthreads_repeating_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2952 2023-05-06 05:35:57.000000 libvsbsdl-20230506/libcthreads/libcthreads_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1136 2023-05-06 05:35:57.000000 libvsbsdl-20230506/libcthreads/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2023-05-06 05:35:57.000000 libvsbsdl-20230506/libcthreads/libcthreads_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3040 2023-05-06 05:35:57.000000 libvsbsdl-20230506/libcthreads/libcthreads_condition.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2128 2023-05-06 05:35:57.000000 libvsbsdl-20230506/libcthreads/libcthreads_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2356 2023-05-06 05:35:57.000000 libvsbsdl-20230506/libcthreads/libcthreads_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2870 2023-05-06 05:35:57.000000 libvsbsdl-20230506/libcthreads/libcthreads_repeating_thread.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18426 2023-05-06 05:35:57.000000 libvsbsdl-20230506/libcthreads/libcthreads_read_write_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2434 2023-05-06 05:35:57.000000 libvsbsdl-20230506/libcthreads/libcthreads_mutex.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2023-05-06 05:35:57.000000 libvsbsdl-20230506/libcthreads/libcthreads_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10198 2023-05-06 05:35:57.000000 libvsbsdl-20230506/libcthreads/libcthreads_thread.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13601 2023-05-06 05:35:57.000000 libvsbsdl-20230506/libcthreads/libcthreads_mutex.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2510 2023-05-06 05:35:57.000000 libvsbsdl-20230506/libcthreads/libcthreads_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2208 2023-05-06 05:35:57.000000 libvsbsdl-20230506/libcthreads/libcthreads_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1428 2023-05-06 05:35:57.000000 libvsbsdl-20230506/libcthreads/libcthreads_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1864 2023-05-06 05:35:57.000000 libvsbsdl-20230506/libcthreads/libcthreads_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26519 2023-05-06 05:35:57.000000 libvsbsdl-20230506/libcthreads/libcthreads_queue.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18281 2023-05-06 05:35:57.000000 libvsbsdl-20230506/libcthreads/libcthreads_condition.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31589 2023-05-06 05:36:29.000000 libvsbsdl-20230506/libcthreads/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4096 2023-05-06 05:35:57.000000 libvsbsdl-20230506/libcthreads/libcthreads_thread_attributes.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2023-05-06 05:35:57.000000 libvsbsdl-20230506/libcthreads/libcthreads_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8753 2023-05-06 05:35:57.000000 libvsbsdl-20230506/libcthreads/libcthreads_lock.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1170 2023-05-06 05:35:57.000000 libvsbsdl-20230506/libcthreads/libcthreads_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3195 2023-05-06 05:35:57.000000 libvsbsdl-20230506/libcthreads/libcthreads_read_write_lock.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2138 2023-05-06 05:35:57.000000 libvsbsdl-20230506/libcthreads/libcthreads_thread_attributes.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3341 2023-05-06 05:35:57.000000 libvsbsdl-20230506/libcthreads/libcthreads_queue.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       88 2023-05-05 05:07:36.000000 libvsbsdl-20230506/AUTHORS
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    35409 2023-05-06 05:36:27.000000 libvsbsdl-20230506/config.sub
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 06:05:35.000000 libvsbsdl-20230506/libcpath/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2023-05-06 05:35:51.000000 libvsbsdl-20230506/libcpath/libcpath_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2336 2023-05-06 05:35:51.000000 libvsbsdl-20230506/libcpath/libcpath_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1459 2023-05-06 05:35:51.000000 libvsbsdl-20230506/libcpath/libcpath_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      807 2023-05-06 05:35:52.000000 libvsbsdl-20230506/libcpath/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2023-05-06 05:35:51.000000 libvsbsdl-20230506/libcpath/libcpath_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2826 2023-05-06 05:35:51.000000 libvsbsdl-20230506/libcpath/libcpath_system_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2023-05-06 05:35:51.000000 libvsbsdl-20230506/libcpath/libcpath_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1536 2023-05-06 05:35:51.000000 libvsbsdl-20230506/libcpath/libcpath_libcsplit.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7170 2023-05-06 05:35:51.000000 libvsbsdl-20230506/libcpath/libcpath_path.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28777 2023-05-06 05:36:29.000000 libvsbsdl-20230506/libcpath/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1990 2023-05-06 05:35:52.000000 libvsbsdl-20230506/libcpath/libcpath_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2023-05-06 05:35:51.000000 libvsbsdl-20230506/libcpath/libcpath_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2023-05-06 05:35:51.000000 libvsbsdl-20230506/libcpath/libcpath_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   176165 2023-05-06 05:35:51.000000 libvsbsdl-20230506/libcpath/libcpath_path.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25560 2023-05-06 05:35:51.000000 libvsbsdl-20230506/libcpath/libcpath_system_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1461 2023-05-06 05:35:51.000000 libvsbsdl-20230506/libcpath/libcpath_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1736 2023-05-06 05:35:51.000000 libvsbsdl-20230506/libcpath/libcpath_libuna.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 06:05:35.000000 libvsbsdl-20230506/vsbsdltools/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17552 2023-05-05 05:08:20.000000 libvsbsdl-20230506/vsbsdltools/info_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1549 2023-05-05 05:07:37.000000 libvsbsdl-20230506/vsbsdltools/vsbsdltools_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1305 2023-05-02 04:32:50.000000 libvsbsdl-20230506/vsbsdltools/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1211 2023-05-05 05:07:37.000000 libvsbsdl-20230506/vsbsdltools/vsbsdltools_i18n.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1746 2023-05-05 05:07:37.000000 libvsbsdl-20230506/vsbsdltools/vsbsdltools_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4534 2023-05-05 05:07:37.000000 libvsbsdl-20230506/vsbsdltools/vsbsdltools_getopt.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1779 2023-05-05 05:07:37.000000 libvsbsdl-20230506/vsbsdltools/vsbsdltools_libuna.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6634 2023-05-05 05:08:20.000000 libvsbsdl-20230506/vsbsdltools/vsbsdlinfo.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1813 2023-05-05 05:07:37.000000 libvsbsdl-20230506/vsbsdltools/vsbsdltools_getopt.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2639 2023-05-05 05:08:20.000000 libvsbsdl-20230506/vsbsdltools/info_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1476 2023-05-05 05:07:37.000000 libvsbsdl-20230506/vsbsdltools/vsbsdltools_output.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30356 2023-05-06 05:36:31.000000 libvsbsdl-20230506/vsbsdltools/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      984 2023-05-05 05:07:37.000000 libvsbsdl-20230506/vsbsdltools/vsbsdltools_libvsbsdl.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1768 2023-05-05 05:07:37.000000 libvsbsdl-20230506/vsbsdltools/vsbsdltools_signal.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1481 2023-05-05 05:07:37.000000 libvsbsdl-20230506/vsbsdltools/vsbsdltools_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5726 2023-05-05 05:07:37.000000 libvsbsdl-20230506/vsbsdltools/vsbsdltools_signal.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3458 2023-05-05 05:07:37.000000 libvsbsdl-20230506/vsbsdltools/vsbsdltools_output.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1499 2023-05-05 05:07:37.000000 libvsbsdl-20230506/vsbsdltools/vsbsdltools_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1502 2023-05-05 05:07:37.000000 libvsbsdl-20230506/vsbsdltools/vsbsdltools_libclocale.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 06:05:36.000000 libvsbsdl-20230506/manuals/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1777 2023-05-05 05:07:37.000000 libvsbsdl-20230506/manuals/vsbsdlinfo.1
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5501 2023-05-05 05:07:37.000000 libvsbsdl-20230506/manuals/libvsbsdl.3
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      166 2023-04-29 13:19:51.000000 libvsbsdl-20230506/manuals/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    25745 2023-05-06 05:36:29.000000 libvsbsdl-20230506/manuals/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       67 2023-04-29 13:20:19.000000 libvsbsdl-20230506/ABOUT-NLS
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 06:05:36.000000 libvsbsdl-20230506/msvscpp/
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 06:05:36.000000 libvsbsdl-20230506/msvscpp/vsbsdl_test_support/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6358 2023-05-05 05:08:00.000000 libvsbsdl-20230506/msvscpp/vsbsdl_test_support/vsbsdl_test_support.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 06:05:36.000000 libvsbsdl-20230506/msvscpp/vsbsdl_test_io_handle/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5693 2023-05-05 05:08:00.000000 libvsbsdl-20230506/msvscpp/vsbsdl_test_io_handle/vsbsdl_test_io_handle.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 06:05:36.000000 libvsbsdl-20230506/msvscpp/libfcache/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5237 2023-05-05 05:08:00.000000 libvsbsdl-20230506/msvscpp/libfcache/libfcache.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 06:05:36.000000 libvsbsdl-20230506/msvscpp/vsbsdl_test_volume/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6519 2023-05-05 05:08:20.000000 libvsbsdl-20230506/msvscpp/vsbsdl_test_volume/vsbsdl_test_volume.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 06:05:36.000000 libvsbsdl-20230506/msvscpp/libclocale/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4778 2023-05-05 05:08:00.000000 libvsbsdl-20230506/msvscpp/libclocale/libclocale.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 06:05:36.000000 libvsbsdl-20230506/msvscpp/vsbsdl_test_sector_data/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5952 2023-05-05 05:08:00.000000 libvsbsdl-20230506/msvscpp/vsbsdl_test_sector_data/vsbsdl_test_sector_data.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1254 2023-05-05 05:08:00.000000 libvsbsdl-20230506/msvscpp/Makefile.am
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 06:05:36.000000 libvsbsdl-20230506/msvscpp/libbfio/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7306 2023-05-05 05:08:00.000000 libvsbsdl-20230506/msvscpp/libbfio/libbfio.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 06:05:36.000000 libvsbsdl-20230506/msvscpp/vsbsdl_test_error/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5432 2023-05-05 05:08:00.000000 libvsbsdl-20230506/msvscpp/vsbsdl_test_error/vsbsdl_test_error.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    26981 2023-05-05 05:08:20.000000 libvsbsdl-20230506/msvscpp/libvsbsdl.sln
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 06:05:36.000000 libvsbsdl-20230506/msvscpp/pyvsbsdl/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6460 2023-05-05 05:08:00.000000 libvsbsdl-20230506/msvscpp/pyvsbsdl/pyvsbsdl.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 06:05:36.000000 libvsbsdl-20230506/msvscpp/libcfile/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5597 2023-05-05 05:08:00.000000 libvsbsdl-20230506/msvscpp/libcfile/libcfile.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 06:05:36.000000 libvsbsdl-20230506/msvscpp/vsbsdl_test_partition/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6192 2023-05-05 05:08:20.000000 libvsbsdl-20230506/msvscpp/vsbsdl_test_partition/vsbsdl_test_partition.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 06:05:36.000000 libvsbsdl-20230506/msvscpp/libcthreads/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6177 2023-05-05 05:08:00.000000 libvsbsdl-20230506/msvscpp/libcthreads/libcthreads.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 06:05:36.000000 libvsbsdl-20230506/msvscpp/libcpath/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5183 2023-05-05 05:08:00.000000 libvsbsdl-20230506/msvscpp/libcpath/libcpath.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 06:05:36.000000 libvsbsdl-20230506/msvscpp/vsbsdlinfo/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6349 2023-05-05 05:08:00.000000 libvsbsdl-20230506/msvscpp/vsbsdlinfo/vsbsdlinfo.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 06:05:36.000000 libvsbsdl-20230506/msvscpp/libuna/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15387 2023-05-05 05:08:00.000000 libvsbsdl-20230506/msvscpp/libuna/libuna.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 06:05:36.000000 libvsbsdl-20230506/msvscpp/vsbsdl_test_tools_info_handle/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5794 2023-05-05 05:08:00.000000 libvsbsdl-20230506/msvscpp/vsbsdl_test_tools_info_handle/vsbsdl_test_tools_info_handle.vcproj
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21989 2023-05-06 05:36:30.000000 libvsbsdl-20230506/msvscpp/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 06:05:36.000000 libvsbsdl-20230506/msvscpp/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4488 2023-05-05 05:08:00.000000 libvsbsdl-20230506/msvscpp/libcerror/libcerror.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 06:05:36.000000 libvsbsdl-20230506/msvscpp/vsbsdl_test_disklabel/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5946 2023-05-05 05:08:00.000000 libvsbsdl-20230506/msvscpp/vsbsdl_test_disklabel/vsbsdl_test_disklabel.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 06:05:36.000000 libvsbsdl-20230506/msvscpp/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4764 2023-05-05 05:08:00.000000 libvsbsdl-20230506/msvscpp/libcnotify/libcnotify.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 06:05:36.000000 libvsbsdl-20230506/msvscpp/vsbsdl_test_partition_entry/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5711 2023-05-05 05:08:00.000000 libvsbsdl-20230506/msvscpp/vsbsdl_test_partition_entry/vsbsdl_test_partition_entry.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 06:05:36.000000 libvsbsdl-20230506/msvscpp/vsbsdl_test_tools_output/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5629 2023-05-05 05:08:00.000000 libvsbsdl-20230506/msvscpp/vsbsdl_test_tools_output/vsbsdl_test_tools_output.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 06:05:36.000000 libvsbsdl-20230506/msvscpp/vsbsdl_test_tools_signal/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5629 2023-05-05 05:08:00.000000 libvsbsdl-20230506/msvscpp/vsbsdl_test_tools_signal/vsbsdl_test_tools_signal.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 06:05:36.000000 libvsbsdl-20230506/msvscpp/libvsbsdl/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8068 2023-05-05 05:08:00.000000 libvsbsdl-20230506/msvscpp/libvsbsdl/libvsbsdl.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 06:05:36.000000 libvsbsdl-20230506/msvscpp/libfdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6858 2023-05-05 05:08:00.000000 libvsbsdl-20230506/msvscpp/libfdata/libfdata.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 06:05:36.000000 libvsbsdl-20230506/msvscpp/libcdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6172 2023-05-05 05:08:00.000000 libvsbsdl-20230506/msvscpp/libcdata/libcdata.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 06:05:36.000000 libvsbsdl-20230506/msvscpp/vsbsdl_test_notify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5520 2023-05-05 05:08:00.000000 libvsbsdl-20230506/msvscpp/vsbsdl_test_notify/vsbsdl_test_notify.vcproj
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 06:05:36.000000 libvsbsdl-20230506/msvscpp/libcsplit/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5225 2023-05-05 05:08:00.000000 libvsbsdl-20230506/msvscpp/libcsplit/libcsplit.vcproj
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    11497 2023-05-05 05:08:00.000000 libvsbsdl-20230506/setup.py
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    49797 2023-05-06 05:36:27.000000 libvsbsdl-20230506/config.guess
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3435 2023-05-05 05:07:33.000000 libvsbsdl-20230506/libvsbsdl.spec.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-05 05:07:33.000000 libvsbsdl-20230506/NEWS
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 06:05:36.000000 libvsbsdl-20230506/ossfuzz/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2023-04-29 13:19:51.000000 libvsbsdl-20230506/ossfuzz/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2716 2023-05-05 05:07:37.000000 libvsbsdl-20230506/ossfuzz/partition_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2250 2023-05-05 05:07:37.000000 libvsbsdl-20230506/ossfuzz/volume_fuzzer.cc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      977 2023-05-05 05:07:37.000000 libvsbsdl-20230506/ossfuzz/ossfuzz_libvsbsdl.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33004 2023-05-06 05:36:30.000000 libvsbsdl-20230506/ossfuzz/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1739 2023-05-05 05:07:37.000000 libvsbsdl-20230506/ossfuzz/ossfuzz_libbfio.h
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     4879 2023-05-06 05:36:31.000000 libvsbsdl-20230506/test-driver
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)  1617870 2023-05-06 05:36:21.000000 libvsbsdl-20230506/configure
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 06:05:35.000000 libvsbsdl-20230506/libuna/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15532 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_url_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1801 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_mac_symbol.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1140 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1259 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_scsu.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2738 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_iso_8859_5.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3610 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_iso_8859_2.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8602 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_windows_1253.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1602 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_koi8_u.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7189 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_windows_1252.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19794 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_utf32_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_windows_1257.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9125 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_mac_cyrillic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9435 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_mac_thai.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    95123 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_utf32_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1787 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_mac_thai.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8050 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_windows_874.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1628 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_windows_1251.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1432 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   484762 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_windows_949.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1339 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_iso_8859_6.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_windows_1256.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_mac_greek.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_mac_russian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_mac_ukrainian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2540 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_iso_8859_6.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1618 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_windows_874.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8811 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_windows_1251.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10005 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_windows_1256.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2623 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_base16_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1567 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_iso_8859_2.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4162 2023-05-06 05:36:06.000000 libvsbsdl-20230506/libuna/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9076 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_windows_1257.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1627 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_windows_1254.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9211 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_windows_1255.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1392 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1625 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_windows_1253.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5908 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_unicode_character.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_mac_dingbats.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3181 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_scsu.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15485 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_byte_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_mac_celtic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_mac_croatian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1773 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_iso_8859_3.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1346 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_iso_8859_15.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9745 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_mac_roman.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9526 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_utf32_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9542 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_koi8_r.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_mac_icelandic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_windows_936.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3679 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_base64_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9871 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_mac_celtic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   360710 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_windows_950.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9666 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_utf8_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   430461 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_windows_936.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   129163 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_unicode_character.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   101951 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_utf8_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    82226 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_base32_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_windows_950.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1749 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1830 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_windows_932.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1610 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_mac_turkish.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18019 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_utf8_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9088 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_mac_ukrainian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1600 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_koi8_r.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    39461 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_base16_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1636 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_windows_1250.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1783 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_iso_8859_16.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_mac_croatian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10379 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_mac_gaelic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_utf16_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_iso_8859_10.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9394 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_mac_centraleurroman.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   286239 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_windows_932.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2993 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_utf8_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1929 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_url_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11002 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_mac_farsi.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_windows_949.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_mac_romanian.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_mac_gaelic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2629 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_iso_8859_8.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1521 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10389 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_mac_arabic.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1644 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_windows_1252.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9776 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_windows_1250.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_mac_russian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    98825 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_utf16_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1341 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_iso_8859_5.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1363 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1449 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_iso_8859_4.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2921 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_byte_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_mac_roman.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9656 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_utf16_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3561 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_iso_8859_4.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3225 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_iso_8859_10.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1622 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_mac_icelandic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    52301 2023-05-06 05:36:29.000000 libvsbsdl-20230506/libuna/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2808 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_utf7_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14020 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_mac_symbol.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3704 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_base32_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9844 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_mac_turkish.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10880 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_mac_inuit.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19595 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_utf16_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15691 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_utf7_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3106 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_utf32_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3335 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_iso_8859_3.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9078 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_mac_greek.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    16696 2023-05-06 05:36:06.000000 libvsbsdl-20230506/libuna/libuna_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1626 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_windows_1255.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2823 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_iso_8859_14.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3664 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_iso_8859_13.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_mac_centraleurroman.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1448 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_iso_8859_8.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2053 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_iso_8859_9.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8997 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_windows_1254.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1616 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_mac_cyrillic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1604 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_mac_arabic.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9116 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_windows_1258.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_mac_farsi.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1831 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_iso_8859_15.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2873 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_iso_8859_7.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10134 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_mac_dingbats.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1340 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_iso_8859_9.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1630 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_windows_1258.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    74767 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_base64_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9953 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_mac_romanian.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2882 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9984 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_koi8_u.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1455 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_iso_8859_13.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1447 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_iso_8859_7.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1563 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_iso_8859_14.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1598 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_mac_inuit.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3296 2023-05-06 05:36:04.000000 libvsbsdl-20230506/libuna/libuna_codepage_iso_8859_16.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    40587 2023-05-06 05:36:27.000000 libvsbsdl-20230506/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       53 2023-04-28 17:14:35.000000 libvsbsdl-20230506/ChangeLog
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 06:05:34.000000 libvsbsdl-20230506/m4/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23765 2023-04-29 13:19:51.000000 libvsbsdl-20230506/m4/libuna.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14488 2023-04-29 13:20:19.000000 libvsbsdl-20230506/m4/gettext.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      756 2023-04-29 13:19:51.000000 libvsbsdl-20230506/m4/tests.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11944 2023-04-29 13:20:19.000000 libvsbsdl-20230506/m4/lib-prefix.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14525 2023-05-06 05:36:15.000000 libvsbsdl-20230506/m4/ltoptions.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9379 2023-04-29 13:19:51.000000 libvsbsdl-20230506/m4/libcpath.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5370 2023-04-29 13:20:19.000000 libvsbsdl-20230506/m4/lib-ld.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11112 2023-04-29 13:19:51.000000 libvsbsdl-20230506/m4/libcthreads.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    34802 2023-04-29 13:20:19.000000 libvsbsdl-20230506/m4/lib-link.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17674 2023-04-29 13:19:51.000000 libvsbsdl-20230506/m4/python.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   307188 2023-05-06 05:36:15.000000 libvsbsdl-20230506/m4/libtool.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1234 2023-04-29 13:20:19.000000 libvsbsdl-20230506/m4/nls.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8230 2023-04-29 13:19:51.000000 libvsbsdl-20230506/m4/libclocale.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15545 2023-04-29 13:19:51.000000 libvsbsdl-20230506/m4/libfdata.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22432 2023-04-29 13:20:19.000000 libvsbsdl-20230506/m4/host-cpu-c-abi.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5638 2023-04-29 13:19:51.000000 libvsbsdl-20230506/m4/libcnotify.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      714 2023-05-06 05:36:15.000000 libvsbsdl-20230506/m4/ltversion.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    17147 2023-04-29 13:19:51.000000 libvsbsdl-20230506/m4/libcdata.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3090 2023-04-29 13:20:19.000000 libvsbsdl-20230506/m4/progtest.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6151 2023-05-06 05:36:15.000000 libvsbsdl-20230506/m4/lt~obsolete.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11498 2023-04-29 13:19:51.000000 libvsbsdl-20230506/m4/libcfile.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    18831 2023-04-29 13:20:19.000000 libvsbsdl-20230506/m4/po.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3852 2023-04-29 13:19:51.000000 libvsbsdl-20230506/m4/pthread.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    14115 2023-04-29 13:19:51.000000 libvsbsdl-20230506/m4/common.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6260 2023-04-29 13:19:51.000000 libvsbsdl-20230506/m4/libcerror.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9731 2023-04-29 13:20:19.000000 libvsbsdl-20230506/m4/iconv.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4395 2023-05-06 05:36:15.000000 libvsbsdl-20230506/m4/ltsugar.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7325 2023-04-29 13:19:51.000000 libvsbsdl-20230506/m4/libfcache.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7384 2023-04-29 13:19:51.000000 libvsbsdl-20230506/m4/libcsplit.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3229 2023-04-29 13:20:19.000000 libvsbsdl-20230506/m4/intlmacosx.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2058 2023-04-29 13:19:51.000000 libvsbsdl-20230506/m4/types.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    11692 2023-04-29 13:19:51.000000 libvsbsdl-20230506/m4/libbfio.m4
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7652 2023-05-05 05:07:33.000000 libvsbsdl-20230506/COPYING.LESSER
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 06:05:36.000000 libvsbsdl-20230506/pyvsbsdl-python3/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1678 2023-05-05 05:07:35.000000 libvsbsdl-20230506/pyvsbsdl-python3/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41885 2023-05-06 05:36:30.000000 libvsbsdl-20230506/pyvsbsdl-python3/Makefile.in
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 06:05:34.000000 libvsbsdl-20230506/libcerror/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    15420 2023-05-06 05:35:25.000000 libvsbsdl-20230506/libcerror/libcerror_system.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19408 2023-05-06 05:35:25.000000 libvsbsdl-20230506/libcerror/libcerror_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2023-05-06 05:35:25.000000 libvsbsdl-20230506/libcerror/libcerror_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      605 2023-05-06 05:35:25.000000 libvsbsdl-20230506/libcerror/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2880 2023-05-06 05:35:25.000000 libvsbsdl-20230506/libcerror/libcerror_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2023-05-06 05:35:25.000000 libvsbsdl-20230506/libcerror/libcerror_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1522 2023-05-06 05:35:25.000000 libvsbsdl-20230506/libcerror/libcerror_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7629 2023-05-06 05:35:25.000000 libvsbsdl-20230506/libcerror/libcerror_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2023-05-06 05:35:25.000000 libvsbsdl-20230506/libcerror/libcerror_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28124 2023-05-06 05:36:29.000000 libvsbsdl-20230506/libcerror/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2023-05-06 05:35:25.000000 libvsbsdl-20230506/libcerror/libcerror_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2026 2023-05-06 05:35:25.000000 libvsbsdl-20230506/libcerror/libcerror_system.h
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 06:05:34.000000 libvsbsdl-20230506/libcnotify/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1365 2023-05-06 05:35:49.000000 libvsbsdl-20230506/libcnotify/libcnotify_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1424 2023-05-06 05:35:49.000000 libvsbsdl-20230506/libcnotify/libcnotify_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1266 2023-05-06 05:35:49.000000 libvsbsdl-20230506/libcnotify/libcnotify_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1164 2023-05-06 05:35:49.000000 libvsbsdl-20230506/libcnotify/libcnotify_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      693 2023-05-06 05:35:49.000000 libvsbsdl-20230506/libcnotify/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8166 2023-05-06 05:35:49.000000 libvsbsdl-20230506/libcnotify/libcnotify_print.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1094 2023-05-06 05:35:49.000000 libvsbsdl-20230506/libcnotify/libcnotify_verbose.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2023-05-06 05:35:49.000000 libvsbsdl-20230506/libcnotify/libcnotify_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1415 2023-05-06 05:35:49.000000 libvsbsdl-20230506/libcnotify/libcnotify_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4018 2023-05-06 05:35:49.000000 libvsbsdl-20230506/libcnotify/libcnotify_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28611 2023-05-06 05:36:29.000000 libvsbsdl-20230506/libcnotify/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1722 2023-05-06 05:35:49.000000 libvsbsdl-20230506/libcnotify/libcnotify_print.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1290 2023-05-06 05:35:49.000000 libvsbsdl-20230506/libcnotify/libcnotify_verbose.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2023-05-06 05:35:49.000000 libvsbsdl-20230506/libcnotify/libcnotify_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   332808 2023-05-06 05:36:15.000000 libvsbsdl-20230506/ltmain.sh
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)     7400 2023-05-06 05:36:26.000000 libvsbsdl-20230506/compile
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    18574 2023-04-29 13:20:19.000000 libvsbsdl-20230506/config.rpath
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 06:05:35.000000 libvsbsdl-20230506/libvsbsdl/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2193 2023-05-06 05:37:04.000000 libvsbsdl-20230506/libvsbsdl/libvsbsdl_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19674 2023-05-05 05:07:36.000000 libvsbsdl-20230506/libvsbsdl/libvsbsdl_disklabel.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1813 2023-05-05 05:07:36.000000 libvsbsdl-20230506/libvsbsdl/libvsbsdl_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1457 2023-05-05 05:07:36.000000 libvsbsdl-20230506/libvsbsdl/libvsbsdl_libclocale.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4181 2023-05-05 05:07:36.000000 libvsbsdl-20230506/libvsbsdl/libvsbsdl_debug.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2200 2023-05-05 05:07:36.000000 libvsbsdl-20230506/libvsbsdl/libvsbsdl_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1439 2023-05-05 05:07:36.000000 libvsbsdl-20230506/libvsbsdl/libvsbsdl_libfcache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2162 2023-05-05 05:07:36.000000 libvsbsdl-20230506/libvsbsdl/libvsbsdl_sector_data.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2328 2023-05-05 05:07:36.000000 libvsbsdl-20230506/libvsbsdl/libvsbsdl_partition_entry.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2517 2023-05-05 05:07:36.000000 libvsbsdl-20230506/libvsbsdl/libvsbsdl_disklabel.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    28593 2023-05-06 05:17:06.000000 libvsbsdl-20230506/libvsbsdl/libvsbsdl_partition.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30229 2023-05-05 05:07:36.000000 libvsbsdl-20230506/libvsbsdl/libvsbsdl_volume.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3705 2023-05-05 05:07:36.000000 libvsbsdl-20230506/libvsbsdl/libvsbsdl_io_handle.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1603 2023-05-05 05:07:36.000000 libvsbsdl-20230506/libvsbsdl/libvsbsdl_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8423 2023-05-05 05:07:36.000000 libvsbsdl-20230506/libvsbsdl/libvsbsdl_partition_entry.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1998 2023-04-30 05:39:27.000000 libvsbsdl-20230506/libvsbsdl/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1543 2023-05-05 05:07:36.000000 libvsbsdl-20230506/libvsbsdl/libvsbsdl_libfdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1611 2023-05-05 05:07:36.000000 libvsbsdl-20230506/libvsbsdl/libvsbsdl_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1694 2023-05-05 05:07:36.000000 libvsbsdl-20230506/libvsbsdl/libvsbsdl_io_handle.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1086 2023-05-06 05:37:04.000000 libvsbsdl-20230506/libvsbsdl/libvsbsdl.rc
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1701 2023-05-05 05:07:36.000000 libvsbsdl-20230506/libvsbsdl/libvsbsdl_libbfio.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1698 2023-05-05 05:07:36.000000 libvsbsdl-20230506/libvsbsdl/vsbsdl_partition_entry.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1834 2023-05-05 05:07:36.000000 libvsbsdl-20230506/libvsbsdl/libvsbsdl.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2195 2023-05-05 05:07:36.000000 libvsbsdl-20230506/libvsbsdl/libvsbsdl_definitions.h.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1397 2023-05-05 05:07:36.000000 libvsbsdl-20230506/libvsbsdl/libvsbsdl_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3580 2023-05-05 05:07:36.000000 libvsbsdl-20230506/libvsbsdl/vsbsdl_disklabel.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1436 2023-05-05 05:07:36.000000 libvsbsdl-20230506/libvsbsdl/libvsbsdl_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1454 2023-05-05 05:07:36.000000 libvsbsdl-20230506/libvsbsdl/libvsbsdl_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1546 2023-05-05 05:07:36.000000 libvsbsdl-20230506/libvsbsdl/libvsbsdl_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1382 2023-05-05 05:07:36.000000 libvsbsdl-20230506/libvsbsdl/libvsbsdl_debug.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3800 2023-05-05 05:07:36.000000 libvsbsdl-20230506/libvsbsdl/libvsbsdl_volume.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2919 2023-05-05 05:07:36.000000 libvsbsdl-20230506/libvsbsdl/libvsbsdl_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1411 2023-05-05 05:07:36.000000 libvsbsdl-20230506/libvsbsdl/libvsbsdl_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    33451 2023-05-06 05:36:29.000000 libvsbsdl-20230506/libvsbsdl/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1927 2023-05-05 05:07:36.000000 libvsbsdl-20230506/libvsbsdl/libvsbsdl_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8830 2023-05-05 05:07:36.000000 libvsbsdl-20230506/libvsbsdl/libvsbsdl_sector_data.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9800 2023-05-05 05:07:36.000000 libvsbsdl-20230506/libvsbsdl/libvsbsdl_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     4230 2023-05-05 05:07:36.000000 libvsbsdl-20230506/libvsbsdl/libvsbsdl_partition.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2761 2023-05-05 05:07:36.000000 libvsbsdl-20230506/libvsbsdl/libvsbsdl_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1088 2023-05-05 05:07:36.000000 libvsbsdl-20230506/libvsbsdl/libvsbsdl.rc.in
+-rwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)    23568 2023-05-06 05:36:31.000000 libvsbsdl-20230506/depcomp
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 06:05:36.000000 libvsbsdl-20230506/po/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1204 2023-04-29 13:20:19.000000 libvsbsdl-20230506/po/en@quot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2395 2023-04-29 13:20:19.000000 libvsbsdl-20230506/po/Rules-quot
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       59 2023-04-29 13:19:51.000000 libvsbsdl-20230506/po/POTFILES.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      720 2023-04-29 13:20:19.000000 libvsbsdl-20230506/po/remove-potcdate.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1808 2023-04-29 13:19:51.000000 libvsbsdl-20230506/po/Makevars.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)       50 2023-04-29 13:19:51.000000 libvsbsdl-20230506/po/ChangeLog
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1338 2023-04-29 13:20:19.000000 libvsbsdl-20230506/po/en@boldquot.header
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      153 2023-04-29 13:20:19.000000 libvsbsdl-20230506/po/quot.sed
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1811 2023-05-06 05:37:04.000000 libvsbsdl-20230506/po/Makevars
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      906 2023-04-29 13:20:19.000000 libvsbsdl-20230506/po/insert-header.sin
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19571 2023-04-29 13:20:19.000000 libvsbsdl-20230506/po/Makefile.in.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      217 2023-04-29 13:20:19.000000 libvsbsdl-20230506/po/boldquot.sed
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2678 2023-05-06 05:37:04.000000 libvsbsdl-20230506/libvsbsdl.spec
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 06:05:35.000000 libvsbsdl-20230506/libfdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2804 2023-05-06 05:36:01.000000 libvsbsdl-20230506/libfdata/libfdata_segments_array.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1658 2023-05-06 05:36:01.000000 libvsbsdl-20230506/libfdata/libfdata_cache.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1172 2023-05-06 05:36:01.000000 libvsbsdl-20230506/libfdata/libfdata_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    19329 2023-05-06 05:36:01.000000 libvsbsdl-20230506/libfdata/libfdata_list_element.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1995 2023-05-06 05:36:01.000000 libvsbsdl-20230506/libfdata/libfdata_mapped_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2023-05-06 05:36:01.000000 libvsbsdl-20230506/libfdata/libfdata_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   107689 2023-05-06 05:36:01.000000 libvsbsdl-20230506/libfdata/libfdata_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1548 2023-05-06 05:36:01.000000 libvsbsdl-20230506/libfdata/libfdata_libcdata.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1593 2023-05-06 05:36:01.000000 libvsbsdl-20230506/libfdata/libfdata_notify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6013 2023-05-06 05:36:01.000000 libvsbsdl-20230506/libfdata/libfdata_range_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1256 2023-05-06 05:36:01.000000 libvsbsdl-20230506/libfdata/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2023-05-06 05:36:01.000000 libvsbsdl-20230506/libfdata/libfdata_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12090 2023-05-06 05:36:01.000000 libvsbsdl-20230506/libfdata/libfdata_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7327 2023-05-06 05:36:01.000000 libvsbsdl-20230506/libfdata/libfdata_area.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2054 2023-05-06 05:36:01.000000 libvsbsdl-20230506/libfdata/libfdata_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37893 2023-05-06 05:36:01.000000 libvsbsdl-20230506/libfdata/libfdata_area.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2092 2023-05-06 05:36:01.000000 libvsbsdl-20230506/libfdata/libfdata_range.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49670 2023-05-06 05:36:01.000000 libvsbsdl-20230506/libfdata/libfdata_vector.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     9700 2023-05-06 05:36:01.000000 libvsbsdl-20230506/libfdata/libfdata_stream.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7810 2023-05-06 05:36:01.000000 libvsbsdl-20230506/libfdata/libfdata_vector.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2023-05-06 05:36:01.000000 libvsbsdl-20230506/libfdata/libfdata_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2023-05-06 05:36:01.000000 libvsbsdl-20230506/libfdata/libfdata_libfcache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2023-05-06 05:36:01.000000 libvsbsdl-20230506/libfdata/libfdata_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    30931 2023-05-06 05:36:01.000000 libvsbsdl-20230506/libfdata/libfdata_range_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1456 2023-05-06 05:36:01.000000 libvsbsdl-20230506/libfdata/libfdata_libcnotify.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2754 2023-05-06 05:36:01.000000 libvsbsdl-20230506/libfdata/libfdata_notify.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3999 2023-05-06 05:36:01.000000 libvsbsdl-20230506/libfdata/libfdata_list_element.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2023-05-06 05:36:01.000000 libvsbsdl-20230506/libfdata/libfdata_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2023-05-06 05:36:01.000000 libvsbsdl-20230506/libfdata/libfdata_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31964 2023-05-06 05:36:29.000000 libvsbsdl-20230506/libfdata/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1491 2023-05-06 05:36:01.000000 libvsbsdl-20230506/libfdata/libfdata_cache.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    66203 2023-05-06 05:36:01.000000 libvsbsdl-20230506/libfdata/libfdata_stream.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    21271 2023-05-06 05:36:01.000000 libvsbsdl-20230506/libfdata/libfdata_segments_array.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6826 2023-05-06 05:36:01.000000 libvsbsdl-20230506/libfdata/libfdata_mapped_range.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6533 2023-05-06 05:36:01.000000 libvsbsdl-20230506/libfdata/libfdata_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7149 2023-05-06 05:36:01.000000 libvsbsdl-20230506/libfdata/libfdata_range.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 06:05:34.000000 libvsbsdl-20230506/libcdata/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    49968 2023-05-06 05:35:24.000000 libvsbsdl-20230506/libcdata/libcdata_array.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    37549 2023-05-06 05:35:24.000000 libvsbsdl-20230506/libcdata/libcdata_btree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   100501 2023-05-06 05:35:24.000000 libvsbsdl-20230506/libcdata/libcdata_tree_node.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1925 2023-05-06 05:35:24.000000 libvsbsdl-20230506/libcdata/libcdata_libcthreads.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2789 2023-05-06 05:35:24.000000 libvsbsdl-20230506/libcdata/libcdata_range_list_value.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1408 2023-05-06 05:35:24.000000 libvsbsdl-20230506/libcdata/libcdata_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    12295 2023-05-06 05:35:24.000000 libvsbsdl-20230506/libcdata/libcdata_range_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1092 2023-05-06 05:35:24.000000 libvsbsdl-20230506/libcdata/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)   122285 2023-05-06 05:35:24.000000 libvsbsdl-20230506/libcdata/libcdata_range_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1389 2023-05-06 05:35:24.000000 libvsbsdl-20230506/libcdata/libcdata_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1152 2023-05-06 05:35:24.000000 libvsbsdl-20230506/libcdata/libcdata_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3871 2023-05-06 05:35:24.000000 libvsbsdl-20230506/libcdata/libcdata_list_element.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5251 2023-05-06 05:35:24.000000 libvsbsdl-20230506/libcdata/libcdata_btree_values_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    10647 2023-05-06 05:35:24.000000 libvsbsdl-20230506/libcdata/libcdata_range_list_value.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1438 2023-05-06 05:35:24.000000 libvsbsdl-20230506/libcdata/libcdata_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2910 2023-05-06 05:35:24.000000 libvsbsdl-20230506/libcdata/libcdata_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1795 2023-05-06 05:35:24.000000 libvsbsdl-20230506/libcdata/libcdata_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1230 2023-05-06 05:35:24.000000 libvsbsdl-20230506/libcdata/libcdata_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2960 2023-05-06 05:35:24.000000 libvsbsdl-20230506/libcdata/libcdata_btree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    69515 2023-05-06 05:35:24.000000 libvsbsdl-20230506/libcdata/libcdata_list.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     8365 2023-05-06 05:35:24.000000 libvsbsdl-20230506/libcdata/libcdata_tree_node.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6448 2023-05-06 05:35:24.000000 libvsbsdl-20230506/libcdata/libcdata_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1976 2023-05-06 05:35:24.000000 libvsbsdl-20230506/libcdata/libcdata_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    23846 2023-05-06 05:35:24.000000 libvsbsdl-20230506/libcdata/libcdata_list_element.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    31183 2023-05-06 05:36:29.000000 libvsbsdl-20230506/libcdata/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1648 2023-05-06 05:35:24.000000 libvsbsdl-20230506/libcdata/libcdata_btree_values_list.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     5231 2023-05-06 05:35:24.000000 libvsbsdl-20230506/libcdata/libcdata_array.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     3790 2023-05-06 05:35:24.000000 libvsbsdl-20230506/libcdata/libcdata_btree.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2115 2023-05-06 05:35:24.000000 libvsbsdl-20230506/libcdata/libcdata_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    22358 2023-05-06 05:35:24.000000 libvsbsdl-20230506/libcdata/libcdata_btree.c
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 06:05:36.000000 libvsbsdl-20230506/pyvsbsdl-python2/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1678 2023-05-05 05:07:35.000000 libvsbsdl-20230506/pyvsbsdl-python2/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    41885 2023-05-06 05:36:30.000000 libvsbsdl-20230506/pyvsbsdl-python2/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1219 2023-05-05 05:07:33.000000 libvsbsdl-20230506/acinclude.m4
+drwxr-xr-x   0 lordyesta  (1000) lordyesta  (1000)        0 2023-05-06 06:05:35.000000 libvsbsdl-20230506/libcsplit/
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1679 2023-05-06 05:35:53.000000 libvsbsdl-20230506/libcsplit/libcsplit_types.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1471 2023-05-06 05:35:53.000000 libvsbsdl-20230506/libcsplit/libcsplit_wide_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1818 2023-05-06 05:35:53.000000 libvsbsdl-20230506/libcsplit/libcsplit_error.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1238 2023-05-06 05:35:53.000000 libvsbsdl-20230506/libcsplit/libcsplit_support.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13912 2023-05-06 05:35:53.000000 libvsbsdl-20230506/libcsplit/libcsplit_narrow_split_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2849 2023-05-06 05:35:53.000000 libvsbsdl-20230506/libcsplit/libcsplit_narrow_split_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      849 2023-05-06 05:35:53.000000 libvsbsdl-20230506/libcsplit/Makefile.am
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    13944 2023-05-06 05:35:53.000000 libvsbsdl-20230506/libcsplit/libcsplit_wide_split_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1386 2023-05-06 05:35:53.000000 libvsbsdl-20230506/libcsplit/libcsplit_narrow_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1416 2023-05-06 05:35:53.000000 libvsbsdl-20230506/libcsplit/libcsplit_unused.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6206 2023-05-06 05:35:53.000000 libvsbsdl-20230506/libcsplit/libcsplit_wide_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     6125 2023-05-06 05:35:53.000000 libvsbsdl-20230506/libcsplit/libcsplit_narrow_string.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)    29557 2023-05-06 05:36:29.000000 libvsbsdl-20230506/libcsplit/Makefile.in
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2920 2023-05-06 05:35:53.000000 libvsbsdl-20230506/libcsplit/libcsplit_wide_split_string.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1360 2023-05-06 05:35:54.000000 libvsbsdl-20230506/libcsplit/libcsplit_definitions.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     2924 2023-05-06 05:35:53.000000 libvsbsdl-20230506/libcsplit/libcsplit_error.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1158 2023-05-06 05:35:53.000000 libvsbsdl-20230506/libcsplit/libcsplit_support.c
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1441 2023-05-06 05:35:53.000000 libvsbsdl-20230506/libcsplit/libcsplit_libcerror.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     1402 2023-05-06 05:35:53.000000 libvsbsdl-20230506/libcsplit/libcsplit_extern.h
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)     7128 2023-05-06 05:18:16.000000 libvsbsdl-20230506/configure.ac
+-rw-r--r--   0 lordyesta  (1000) lordyesta  (1000)      355 2023-05-06 06:05:37.195045 libvsbsdl-20230506/PKG-INFO
```

### Comparing `libvsbsdl-20230502/libfcache/libfcache_extern.h` & `libvsbsdl-20230506/libfcache/libfcache_extern.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libfcache/libfcache_types.h` & `libvsbsdl-20230506/libfcache/libfcache_types.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libfcache/libfcache_cache.h` & `libvsbsdl-20230506/libfcache/libfcache_cache.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libfcache/libfcache_support.h` & `libvsbsdl-20230506/libfcache/libfcache_support.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libfcache/libfcache_support.c` & `libvsbsdl-20230506/libfcache/libfcache_support.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libfcache/Makefile.am` & `libvsbsdl-20230506/libfcache/Makefile.am`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libfcache/libfcache_libcdata.h` & `libvsbsdl-20230506/libfcache/libfcache_libcdata.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libfcache/libfcache_unused.h` & `libvsbsdl-20230506/libfcache/libfcache_unused.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libfcache/libfcache_libcerror.h` & `libvsbsdl-20230506/libfcache/libfcache_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libfcache/libfcache_definitions.h` & `libvsbsdl-20230506/libfcache/libfcache_definitions.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libfcache/libfcache_cache_value.h` & `libvsbsdl-20230506/libfcache/libfcache_cache_value.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libfcache/libfcache_cache_value.c` & `libvsbsdl-20230506/libfcache/libfcache_cache_value.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libfcache/Makefile.in` & `libvsbsdl-20230506/libfcache/Makefile.in`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libfcache/libfcache_error.c` & `libvsbsdl-20230506/libfcache/libfcache_error.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libfcache/libfcache_date_time.c` & `libvsbsdl-20230506/libfcache/libfcache_date_time.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libfcache/libfcache_cache.c` & `libvsbsdl-20230506/libfcache/libfcache_cache.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libfcache/libfcache_error.h` & `libvsbsdl-20230506/libfcache/libfcache_error.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libfcache/libfcache_date_time.h` & `libvsbsdl-20230506/libfcache/libfcache_date_time.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/common/config_msc.h` & `libvsbsdl-20230506/common/config_msc.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/common/byte_stream.h` & `libvsbsdl-20230506/common/byte_stream.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/common/common.h` & `libvsbsdl-20230506/common/common.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/common/system_string.h` & `libvsbsdl-20230506/common/system_string.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/common/types.h` & `libvsbsdl-20230506/common/types.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/common/types.h.in` & `libvsbsdl-20230506/common/types.h.in`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/common/config_winapi.h` & `libvsbsdl-20230506/common/config_winapi.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/common/memory.h` & `libvsbsdl-20230506/common/memory.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/common/config.h` & `libvsbsdl-20230506/common/config.h`

 * *Files 0% similar despite different names*

```diff
@@ -505,24 +505,24 @@
 /* Define to the address where bug reports for this package should be sent. */
 #define PACKAGE_BUGREPORT "joachim.metz@gmail.com"
 
 /* Define to the full name of this package. */
 #define PACKAGE_NAME "libvsbsdl"
 
 /* Define to the full name and version of this package. */
-#define PACKAGE_STRING "libvsbsdl 20230502"
+#define PACKAGE_STRING "libvsbsdl 20230506"
 
 /* Define to the one symbol short name of this package. */
 #define PACKAGE_TARNAME "libvsbsdl"
 
 /* Define to the home page for this package. */
 #define PACKAGE_URL ""
 
 /* Define to the version of this package. */
-#define PACKAGE_VERSION "20230502"
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
-#define VERSION "20230502"
+#define VERSION "20230506"
 
 /* Number of bits in a file offset, on hosts where this is settable. */
 /* #undef _FILE_OFFSET_BITS */
 
 /* Define for large files, on AIX-style hosts. */
 /* #undef _LARGE_FILES */
```

### Comparing `libvsbsdl-20230502/common/narrow_string.h` & `libvsbsdl-20230506/common/narrow_string.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/common/Makefile.in` & `libvsbsdl-20230506/common/Makefile.in`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/common/file_stream.h` & `libvsbsdl-20230506/common/file_stream.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/common/config_borlandc.h` & `libvsbsdl-20230506/common/config_borlandc.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/common/config.h.in` & `libvsbsdl-20230506/common/config.h.in`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/common/wide_string.h` & `libvsbsdl-20230506/common/wide_string.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libvsbsdl.pc.in` & `libvsbsdl-20230506/libvsbsdl.pc.in`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/tests/test_library.sh` & `libvsbsdl-20230506/tests/test_library.sh`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/tests/pyvsbsdl_test_volume.py` & `libvsbsdl-20230506/tests/pyvsbsdl_test_volume.py`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/tests/vsbsdl_test_libvsbsdl.h` & `libvsbsdl-20230506/tests/vsbsdl_test_libvsbsdl.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/tests/vsbsdl_test_partition_entry.c` & `libvsbsdl-20230506/tests/vsbsdl_test_partition_entry.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/tests/vsbsdl_test_memory.c` & `libvsbsdl-20230506/tests/vsbsdl_test_memory.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/tests/vsbsdl_test_rwlock.h` & `libvsbsdl-20230506/tests/vsbsdl_test_rwlock.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/tests/test_python_module.sh` & `libvsbsdl-20230506/tests/test_python_module.sh`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/tests/vsbsdl_test_rwlock.c` & `libvsbsdl-20230506/tests/vsbsdl_test_rwlock.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/tests/Makefile.am` & `libvsbsdl-20230506/tests/Makefile.am`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/tests/vsbsdl_test_error.c` & `libvsbsdl-20230506/tests/vsbsdl_test_error.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/tests/vsbsdl_test_libbfio.h` & `libvsbsdl-20230506/tests/vsbsdl_test_libbfio.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/tests/vsbsdl_test_functions.c` & `libvsbsdl-20230506/tests/vsbsdl_test_functions.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/tests/vsbsdl_test_disklabel.c` & `libvsbsdl-20230506/tests/vsbsdl_test_disklabel.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/tests/vsbsdl_test_libcnotify.h` & `libvsbsdl-20230506/tests/vsbsdl_test_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/tests/vsbsdl_test_getopt.h` & `libvsbsdl-20230506/tests/vsbsdl_test_getopt.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/tests/vsbsdl_test_getopt.c` & `libvsbsdl-20230506/tests/vsbsdl_test_getopt.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/tests/vsbsdl_test_tools_output.c` & `libvsbsdl-20230506/tests/vsbsdl_test_tools_output.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/tests/test_tools.sh` & `libvsbsdl-20230506/tests/test_tools.sh`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/tests/vsbsdl_test_macros.h` & `libvsbsdl-20230506/tests/vsbsdl_test_macros.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/tests/vsbsdl_test_volume.c` & `libvsbsdl-20230506/tests/vsbsdl_test_volume.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/tests/vsbsdl_test_libcerror.h` & `libvsbsdl-20230506/tests/vsbsdl_test_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/tests/test_manpage.sh` & `libvsbsdl-20230506/tests/test_manpage.sh`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/tests/vsbsdl_test_libclocale.h` & `libvsbsdl-20230506/tests/vsbsdl_test_libclocale.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/tests/vsbsdl_test_partition.c` & `libvsbsdl-20230506/tests/vsbsdl_test_partition.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/tests/vsbsdl_test_tools_signal.c` & `libvsbsdl-20230506/tests/vsbsdl_test_tools_signal.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/tests/pyvsbsdl_test_partition.py` & `libvsbsdl-20230506/tests/pyvsbsdl_test_partition.py`

 * *Files 2% similar despite different names*

```diff
@@ -258,28 +258,28 @@
 
     vsbsdl_partition.close()
 
     # Test the seek without open.
     with self.assertRaises(IOError):
       vsbsdl_partition.seek_offset(16, os.SEEK_SET)
 
-  def test_get_type(self):
-    """Tests the get_type function and type property."""
+  def test_get_entry_index(self):
+    """Tests the get_entry_index function and entry_index property."""
     test_source = unittest.source
     if not test_source:
       raise unittest.SkipTest("missing source")
 
     vsbsdl_partition = pyvsbsdl.partition()
 
     vsbsdl_partition.open(test_source)
 
-    type = vsbsdl_partition.get_type()
-    self.assertIsNotNone(type)
+    entry_index = vsbsdl_partition.get_entry_index()
+    self.assertIsNotNone(entry_index)
 
-    self.assertIsNotNone(vsbsdl_partition.type)
+    self.assertIsNotNone(vsbsdl_partition.entry_index)
 
     vsbsdl_partition.close()
 
   def test_get_volume_offset(self):
     """Tests the get_volume_offset function and volume_offset property."""
     test_source = unittest.source
     if not test_source:
```

### Comparing `libvsbsdl-20230502/tests/test_runner.sh` & `libvsbsdl-20230506/tests/test_runner.sh`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/tests/pyvsbsdl_test_support.py` & `libvsbsdl-20230506/tests/pyvsbsdl_test_support.py`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/tests/vsbsdl_test_unused.h` & `libvsbsdl-20230506/tests/vsbsdl_test_unused.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/tests/Makefile.in` & `libvsbsdl-20230506/tests/Makefile.in`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/tests/test_vsbsdlinfo.sh` & `libvsbsdl-20230506/tests/test_vsbsdlinfo.sh`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/tests/vsbsdl_test_sector_data.c` & `libvsbsdl-20230506/tests/vsbsdl_test_sector_data.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/tests/vsbsdl_test_memory.h` & `libvsbsdl-20230506/tests/vsbsdl_test_memory.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/tests/vsbsdl_test_io_handle.c` & `libvsbsdl-20230506/tests/vsbsdl_test_io_handle.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/tests/vsbsdl_test_tools_info_handle.c` & `libvsbsdl-20230506/tests/vsbsdl_test_tools_info_handle.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/tests/vsbsdl_test_support.c` & `libvsbsdl-20230506/tests/vsbsdl_test_support.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/tests/vsbsdl_test_notify.c` & `libvsbsdl-20230506/tests/vsbsdl_test_notify.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/tests/vsbsdl_test_libuna.h` & `libvsbsdl-20230506/tests/vsbsdl_test_libuna.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/tests/vsbsdl_test_functions.h` & `libvsbsdl-20230506/tests/vsbsdl_test_functions.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libclocale/libclocale_wide_string.h` & `libvsbsdl-20230506/libclocale/libclocale_wide_string.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libclocale/libclocale_support.c` & `libvsbsdl-20230506/libclocale/libclocale_support.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libclocale/libclocale_locale.h` & `libvsbsdl-20230506/libclocale/libclocale_locale.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libclocale/Makefile.am` & `libvsbsdl-20230506/libclocale/Makefile.am`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libclocale/libclocale_locale.c` & `libvsbsdl-20230506/libclocale/libclocale_locale.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libclocale/libclocale_extern.h` & `libvsbsdl-20230506/libclocale/libclocale_extern.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libclocale/libclocale_unused.h` & `libvsbsdl-20230506/libclocale/libclocale_unused.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libclocale/libclocale_support.h` & `libvsbsdl-20230506/libclocale/libclocale_support.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libclocale/libclocale_definitions.h` & `libvsbsdl-20230506/libclocale/libclocale_definitions.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libclocale/libclocale_codepage.h` & `libvsbsdl-20230506/libclocale/libclocale_codepage.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libclocale/libclocale_codepage.c` & `libvsbsdl-20230506/libclocale/libclocale_codepage.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libclocale/Makefile.in` & `libvsbsdl-20230506/libclocale/Makefile.in`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libclocale/libclocale_wide_string.c` & `libvsbsdl-20230506/libclocale/libclocale_wide_string.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libclocale/libclocale_libcerror.h` & `libvsbsdl-20230506/libclocale/libclocale_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/missing` & `libvsbsdl-20230506/missing`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/Makefile.am` & `libvsbsdl-20230506/Makefile.am`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/aclocal.m4` & `libvsbsdl-20230506/aclocal.m4`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libbfio/libbfio_handle.h` & `libvsbsdl-20230506/libbfio/libbfio_handle.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libbfio/libbfio_libcerror.h` & `libvsbsdl-20230506/libbfio/libbfio_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libbfio/libbfio_handle.c` & `libvsbsdl-20230506/libbfio/libbfio_handle.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libbfio/libbfio_libuna.h` & `libvsbsdl-20230506/libbfio/libbfio_libuna.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libbfio/libbfio_definitions.h` & `libvsbsdl-20230506/libbfio/libbfio_definitions.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libbfio/libbfio_libclocale.h` & `libvsbsdl-20230506/libbfio/libbfio_libclocale.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libbfio/libbfio_codepage.h` & `libvsbsdl-20230506/libbfio/libbfio_codepage.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libbfio/libbfio_libcdata.h` & `libvsbsdl-20230506/libbfio/libbfio_libcdata.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libbfio/libbfio_extern.h` & `libvsbsdl-20230506/libbfio/libbfio_extern.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libbfio/libbfio_file_range.c` & `libvsbsdl-20230506/libbfio/libbfio_file_range.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libbfio/libbfio_file_range_io_handle.c` & `libvsbsdl-20230506/libbfio/libbfio_file_range_io_handle.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libbfio/Makefile.am` & `libvsbsdl-20230506/libbfio/Makefile.am`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libbfio/libbfio_file_pool.c` & `libvsbsdl-20230506/libbfio/libbfio_file_pool.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libbfio/libbfio_file.c` & `libvsbsdl-20230506/libbfio/libbfio_file.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libbfio/libbfio_pool.h` & `libvsbsdl-20230506/libbfio/libbfio_pool.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libbfio/libbfio_file_range.h` & `libvsbsdl-20230506/libbfio/libbfio_file_range.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libbfio/libbfio_system_string.h` & `libvsbsdl-20230506/libbfio/libbfio_system_string.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libbfio/libbfio_file_io_handle.h` & `libvsbsdl-20230506/libbfio/libbfio_file_io_handle.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libbfio/libbfio_memory_range_io_handle.c` & `libvsbsdl-20230506/libbfio/libbfio_memory_range_io_handle.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libbfio/libbfio_file.h` & `libvsbsdl-20230506/libbfio/libbfio_file.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libbfio/libbfio_support.c` & `libvsbsdl-20230506/libbfio/libbfio_support.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libbfio/libbfio_file_pool.h` & `libvsbsdl-20230506/libbfio/libbfio_file_pool.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libbfio/libbfio_memory_range_io_handle.h` & `libvsbsdl-20230506/libbfio/libbfio_memory_range_io_handle.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libbfio/libbfio_error.h` & `libvsbsdl-20230506/libbfio/libbfio_error.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libbfio/libbfio_libcthreads.h` & `libvsbsdl-20230506/libbfio/libbfio_libcthreads.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libbfio/libbfio_system_string.c` & `libvsbsdl-20230506/libbfio/libbfio_system_string.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libbfio/libbfio_memory_range.h` & `libvsbsdl-20230506/libbfio/libbfio_memory_range.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libbfio/libbfio_file_range_io_handle.h` & `libvsbsdl-20230506/libbfio/libbfio_file_range_io_handle.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libbfio/libbfio_memory_range.c` & `libvsbsdl-20230506/libbfio/libbfio_memory_range.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libbfio/Makefile.in` & `libvsbsdl-20230506/libbfio/Makefile.in`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libbfio/libbfio_pool.c` & `libvsbsdl-20230506/libbfio/libbfio_pool.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libbfio/libbfio_unused.h` & `libvsbsdl-20230506/libbfio/libbfio_unused.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libbfio/libbfio_libcpath.h` & `libvsbsdl-20230506/libbfio/libbfio_libcpath.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libbfio/libbfio_libcfile.h` & `libvsbsdl-20230506/libbfio/libbfio_libcfile.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libbfio/libbfio_support.h` & `libvsbsdl-20230506/libbfio/libbfio_support.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libbfio/libbfio_file_io_handle.c` & `libvsbsdl-20230506/libbfio/libbfio_file_io_handle.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libbfio/libbfio_error.c` & `libvsbsdl-20230506/libbfio/libbfio_error.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libbfio/libbfio_types.h` & `libvsbsdl-20230506/libbfio/libbfio_types.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/COPYING` & `libvsbsdl-20230506/COPYING`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/include/libvsbsdl.h` & `libvsbsdl-20230506/include/libvsbsdl.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/include/Makefile.in` & `libvsbsdl-20230506/include/Makefile.in`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/include/libvsbsdl.h.in` & `libvsbsdl-20230506/include/libvsbsdl.h.in`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/include/libvsbsdl/definitions.h.in` & `libvsbsdl-20230506/include/libvsbsdl/definitions.h.in`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/include/libvsbsdl/extern.h` & `libvsbsdl-20230506/include/libvsbsdl/extern.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/include/libvsbsdl/types.h` & `libvsbsdl-20230506/include/libvsbsdl/types.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/include/libvsbsdl/features.h.in` & `libvsbsdl-20230506/include/libvsbsdl/features.h.in`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/include/libvsbsdl/types.h.in` & `libvsbsdl-20230506/include/libvsbsdl/types.h.in`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/include/libvsbsdl/features.h` & `libvsbsdl-20230506/include/libvsbsdl/features.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/include/libvsbsdl/definitions.h` & `libvsbsdl-20230506/include/libvsbsdl/definitions.h`

 * *Files 5% similar despite different names*

```diff
@@ -20,19 +20,19 @@
  */
 
 #if !defined( _LIBVSBSDL_DEFINITIONS_H )
 #define _LIBVSBSDL_DEFINITIONS_H
 
 #include <libvsbsdl/types.h>
 
-#define LIBVSBSDL_VERSION		20230502
+#define LIBVSBSDL_VERSION		20230506
 
 /* The version string
  */
-#define LIBVSBSDL_VERSION_STRING	"20230502"
+#define LIBVSBSDL_VERSION_STRING	"20230506"
 
 /* The byte order definitions
  */
 enum LIBVSBSDL_ENDIAN
 {
 	LIBVSBSDL_ENDIAN_BIG		= (int) 'b',
 	LIBVSBSDL_ENDIAN_LITTLE		= (int) 'l',
```

### Comparing `libvsbsdl-20230502/include/libvsbsdl/codepage.h` & `libvsbsdl-20230506/include/libvsbsdl/codepage.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/include/libvsbsdl/error.h` & `libvsbsdl-20230506/include/libvsbsdl/error.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/install-sh` & `libvsbsdl-20230506/install-sh`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/INSTALL` & `libvsbsdl-20230506/INSTALL`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/dpkg/copyright` & `libvsbsdl-20230506/dpkg/copyright`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/dpkg/rules` & `libvsbsdl-20230506/dpkg/rules`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/dpkg/control` & `libvsbsdl-20230506/dpkg/control`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/pyvsbsdl/pyvsbsdl_integer.h` & `libvsbsdl-20230506/pyvsbsdl/pyvsbsdl_integer.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/pyvsbsdl/pyvsbsdl_libvsbsdl.h` & `libvsbsdl-20230506/pyvsbsdl/pyvsbsdl_libvsbsdl.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/pyvsbsdl/pyvsbsdl_integer.c` & `libvsbsdl-20230506/pyvsbsdl/pyvsbsdl_integer.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/pyvsbsdl/Makefile.am` & `libvsbsdl-20230506/pyvsbsdl/Makefile.am`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/pyvsbsdl/pyvsbsdl_partitions.c` & `libvsbsdl-20230506/pyvsbsdl/pyvsbsdl_partitions.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/pyvsbsdl/pyvsbsdl_partition.h` & `libvsbsdl-20230506/pyvsbsdl/pyvsbsdl_partition.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/pyvsbsdl/pyvsbsdl_libbfio.h` & `libvsbsdl-20230506/pyvsbsdl/pyvsbsdl_libbfio.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/pyvsbsdl/pyvsbsdl_error.c` & `libvsbsdl-20230506/pyvsbsdl/pyvsbsdl_error.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/pyvsbsdl/pyvsbsdl_file_object_io_handle.c` & `libvsbsdl-20230506/pyvsbsdl/pyvsbsdl_file_object_io_handle.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/pyvsbsdl/pyvsbsdl_error.h` & `libvsbsdl-20230506/pyvsbsdl/pyvsbsdl_error.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/pyvsbsdl/pyvsbsdl_partitions.h` & `libvsbsdl-20230506/pyvsbsdl/pyvsbsdl_partitions.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/pyvsbsdl/pyvsbsdl_unused.h` & `libvsbsdl-20230506/pyvsbsdl/pyvsbsdl_unused.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/pyvsbsdl/pyvsbsdl_volume.c` & `libvsbsdl-20230506/pyvsbsdl/pyvsbsdl_volume.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/pyvsbsdl/pyvsbsdl.h` & `libvsbsdl-20230506/pyvsbsdl/pyvsbsdl.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/pyvsbsdl/Makefile.in` & `libvsbsdl-20230506/pyvsbsdl/Makefile.in`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/pyvsbsdl/pyvsbsdl.c` & `libvsbsdl-20230506/pyvsbsdl/pyvsbsdl.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/pyvsbsdl/pyvsbsdl_libcerror.h` & `libvsbsdl-20230506/pyvsbsdl/pyvsbsdl_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/pyvsbsdl/pyvsbsdl_python.h` & `libvsbsdl-20230506/pyvsbsdl/pyvsbsdl_python.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/pyvsbsdl/pyvsbsdl_libclocale.h` & `libvsbsdl-20230506/pyvsbsdl/pyvsbsdl_libclocale.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/pyvsbsdl/pyvsbsdl_file_object_io_handle.h` & `libvsbsdl-20230506/pyvsbsdl/pyvsbsdl_file_object_io_handle.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/pyvsbsdl/pyvsbsdl_volume.h` & `libvsbsdl-20230506/pyvsbsdl/pyvsbsdl_volume.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/pyvsbsdl/pyvsbsdl_partition.c` & `libvsbsdl-20230506/pyvsbsdl/pyvsbsdl_partition.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcfile/libcfile_file.c` & `libvsbsdl-20230506/libcfile/libcfile_file.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcfile/libcfile_libclocale.h` & `libvsbsdl-20230506/libcfile/libcfile_libclocale.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcfile/libcfile_support.c` & `libvsbsdl-20230506/libcfile/libcfile_support.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcfile/libcfile_support.h` & `libvsbsdl-20230506/libcfile/libcfile_support.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcfile/libcfile_error.c` & `libvsbsdl-20230506/libcfile/libcfile_error.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcfile/libcfile_winapi.c` & `libvsbsdl-20230506/libcfile/libcfile_winapi.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcfile/Makefile.am` & `libvsbsdl-20230506/libcfile/Makefile.am`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcfile/libcfile_libcerror.h` & `libvsbsdl-20230506/libcfile/libcfile_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcfile/libcfile_unused.h` & `libvsbsdl-20230506/libcfile/libcfile_unused.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcfile/libcfile_winapi.h` & `libvsbsdl-20230506/libcfile/libcfile_winapi.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcfile/libcfile_types.h` & `libvsbsdl-20230506/libcfile/libcfile_types.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcfile/libcfile_extern.h` & `libvsbsdl-20230506/libcfile/libcfile_extern.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcfile/libcfile_notify.h` & `libvsbsdl-20230506/libcfile/libcfile_notify.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcfile/libcfile_definitions.h` & `libvsbsdl-20230506/libcfile/libcfile_definitions.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcfile/libcfile_file.h` & `libvsbsdl-20230506/libcfile/libcfile_file.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcfile/libcfile_error.h` & `libvsbsdl-20230506/libcfile/libcfile_error.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcfile/libcfile_system_string.c` & `libvsbsdl-20230506/libcfile/libcfile_system_string.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcfile/Makefile.in` & `libvsbsdl-20230506/libcfile/Makefile.in`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcfile/libcfile_system_string.h` & `libvsbsdl-20230506/libcfile/libcfile_system_string.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcfile/libcfile_libcnotify.h` & `libvsbsdl-20230506/libcfile/libcfile_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcfile/libcfile_libuna.h` & `libvsbsdl-20230506/libcfile/libcfile_libuna.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcfile/libcfile_notify.c` & `libvsbsdl-20230506/libcfile/libcfile_notify.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcthreads/libcthreads_thread_pool.h` & `libvsbsdl-20230506/libcthreads/libcthreads_thread_pool.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcthreads/libcthreads_thread_pool.c` & `libvsbsdl-20230506/libcthreads/libcthreads_thread_pool.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcthreads/libcthreads_repeating_thread.c` & `libvsbsdl-20230506/libcthreads/libcthreads_repeating_thread.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcthreads/libcthreads_error.c` & `libvsbsdl-20230506/libcthreads/libcthreads_error.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcthreads/Makefile.am` & `libvsbsdl-20230506/libcthreads/Makefile.am`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcthreads/libcthreads_unused.h` & `libvsbsdl-20230506/libcthreads/libcthreads_unused.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcthreads/libcthreads_condition.h` & `libvsbsdl-20230506/libcthreads/libcthreads_condition.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcthreads/libcthreads_definitions.h` & `libvsbsdl-20230506/libcthreads/libcthreads_definitions.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcthreads/libcthreads_thread.h` & `libvsbsdl-20230506/libcthreads/libcthreads_thread.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcthreads/libcthreads_repeating_thread.h` & `libvsbsdl-20230506/libcthreads/libcthreads_repeating_thread.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcthreads/libcthreads_read_write_lock.c` & `libvsbsdl-20230506/libcthreads/libcthreads_read_write_lock.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcthreads/libcthreads_mutex.h` & `libvsbsdl-20230506/libcthreads/libcthreads_mutex.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcthreads/libcthreads_support.h` & `libvsbsdl-20230506/libcthreads/libcthreads_support.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcthreads/libcthreads_thread.c` & `libvsbsdl-20230506/libcthreads/libcthreads_thread.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcthreads/libcthreads_mutex.c` & `libvsbsdl-20230506/libcthreads/libcthreads_mutex.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcthreads/libcthreads_types.h` & `libvsbsdl-20230506/libcthreads/libcthreads_types.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcthreads/libcthreads_lock.h` & `libvsbsdl-20230506/libcthreads/libcthreads_lock.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcthreads/libcthreads_extern.h` & `libvsbsdl-20230506/libcthreads/libcthreads_extern.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcthreads/libcthreads_error.h` & `libvsbsdl-20230506/libcthreads/libcthreads_error.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcthreads/libcthreads_queue.c` & `libvsbsdl-20230506/libcthreads/libcthreads_queue.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcthreads/libcthreads_condition.c` & `libvsbsdl-20230506/libcthreads/libcthreads_condition.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcthreads/Makefile.in` & `libvsbsdl-20230506/libcthreads/Makefile.in`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcthreads/libcthreads_thread_attributes.c` & `libvsbsdl-20230506/libcthreads/libcthreads_thread_attributes.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcthreads/libcthreads_libcerror.h` & `libvsbsdl-20230506/libcthreads/libcthreads_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcthreads/libcthreads_lock.c` & `libvsbsdl-20230506/libcthreads/libcthreads_lock.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcthreads/libcthreads_support.c` & `libvsbsdl-20230506/libcthreads/libcthreads_support.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcthreads/libcthreads_read_write_lock.h` & `libvsbsdl-20230506/libcthreads/libcthreads_read_write_lock.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcthreads/libcthreads_thread_attributes.h` & `libvsbsdl-20230506/libcthreads/libcthreads_thread_attributes.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcthreads/libcthreads_queue.h` & `libvsbsdl-20230506/libcthreads/libcthreads_queue.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/config.sub` & `libvsbsdl-20230506/config.sub`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcpath/libcpath_unused.h` & `libvsbsdl-20230506/libcpath/libcpath_unused.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcpath/libcpath_support.c` & `libvsbsdl-20230506/libcpath/libcpath_support.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcpath/libcpath_libclocale.h` & `libvsbsdl-20230506/libcpath/libcpath_libclocale.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcpath/Makefile.am` & `libvsbsdl-20230506/libcpath/Makefile.am`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcpath/libcpath_error.h` & `libvsbsdl-20230506/libcpath/libcpath_error.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcpath/libcpath_system_string.h` & `libvsbsdl-20230506/libcpath/libcpath_system_string.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcpath/libcpath_error.c` & `libvsbsdl-20230506/libcpath/libcpath_error.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcpath/libcpath_libcsplit.h` & `libvsbsdl-20230506/libcpath/libcpath_libcsplit.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcpath/libcpath_path.h` & `libvsbsdl-20230506/libcpath/libcpath_path.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcpath/Makefile.in` & `libvsbsdl-20230506/libcpath/Makefile.in`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcpath/libcpath_definitions.h` & `libvsbsdl-20230506/libcpath/libcpath_definitions.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcpath/libcpath_libcerror.h` & `libvsbsdl-20230506/libcpath/libcpath_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcpath/libcpath_extern.h` & `libvsbsdl-20230506/libcpath/libcpath_extern.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcpath/libcpath_path.c` & `libvsbsdl-20230506/libcpath/libcpath_path.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcpath/libcpath_system_string.c` & `libvsbsdl-20230506/libcpath/libcpath_system_string.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcpath/libcpath_support.h` & `libvsbsdl-20230506/libcpath/libcpath_support.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcpath/libcpath_libuna.h` & `libvsbsdl-20230506/libcpath/libcpath_libuna.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/vsbsdltools/info_handle.c` & `libvsbsdl-20230506/vsbsdltools/info_handle.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/vsbsdltools/vsbsdltools_unused.h` & `libvsbsdl-20230506/vsbsdltools/vsbsdltools_unused.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/vsbsdltools/Makefile.am` & `libvsbsdl-20230506/vsbsdltools/Makefile.am`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/vsbsdltools/vsbsdltools_i18n.h` & `libvsbsdl-20230506/vsbsdltools/vsbsdltools_i18n.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/vsbsdltools/vsbsdltools_libbfio.h` & `libvsbsdl-20230506/vsbsdltools/vsbsdltools_libbfio.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/vsbsdltools/vsbsdltools_getopt.c` & `libvsbsdl-20230506/vsbsdltools/vsbsdltools_getopt.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/vsbsdltools/vsbsdltools_libuna.h` & `libvsbsdl-20230506/vsbsdltools/vsbsdltools_libuna.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/vsbsdltools/vsbsdlinfo.c` & `libvsbsdl-20230506/vsbsdltools/vsbsdlinfo.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/vsbsdltools/vsbsdltools_getopt.h` & `libvsbsdl-20230506/vsbsdltools/vsbsdltools_getopt.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/vsbsdltools/info_handle.h` & `libvsbsdl-20230506/vsbsdltools/info_handle.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/vsbsdltools/vsbsdltools_output.h` & `libvsbsdl-20230506/vsbsdltools/vsbsdltools_output.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/vsbsdltools/Makefile.in` & `libvsbsdl-20230506/vsbsdltools/Makefile.in`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/vsbsdltools/vsbsdltools_libvsbsdl.h` & `libvsbsdl-20230506/vsbsdltools/vsbsdltools_libvsbsdl.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/vsbsdltools/vsbsdltools_signal.h` & `libvsbsdl-20230506/vsbsdltools/vsbsdltools_signal.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/vsbsdltools/vsbsdltools_libcerror.h` & `libvsbsdl-20230506/vsbsdltools/vsbsdltools_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/vsbsdltools/vsbsdltools_signal.c` & `libvsbsdl-20230506/vsbsdltools/vsbsdltools_signal.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/vsbsdltools/vsbsdltools_output.c` & `libvsbsdl-20230506/vsbsdltools/vsbsdltools_output.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/vsbsdltools/vsbsdltools_libcnotify.h` & `libvsbsdl-20230506/vsbsdltools/vsbsdltools_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/vsbsdltools/vsbsdltools_libclocale.h` & `libvsbsdl-20230506/vsbsdltools/vsbsdltools_libclocale.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/manuals/vsbsdlinfo.1` & `libvsbsdl-20230506/manuals/vsbsdlinfo.1`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/manuals/libvsbsdl.3` & `libvsbsdl-20230506/manuals/libvsbsdl.3`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/manuals/Makefile.in` & `libvsbsdl-20230506/manuals/Makefile.in`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/msvscpp/vsbsdl_test_support/vsbsdl_test_support.vcproj` & `libvsbsdl-20230506/msvscpp/vsbsdl_test_support/vsbsdl_test_support.vcproj`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/msvscpp/vsbsdl_test_io_handle/vsbsdl_test_io_handle.vcproj` & `libvsbsdl-20230506/msvscpp/vsbsdl_test_io_handle/vsbsdl_test_io_handle.vcproj`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/msvscpp/libfcache/libfcache.vcproj` & `libvsbsdl-20230506/msvscpp/libfcache/libfcache.vcproj`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/msvscpp/vsbsdl_test_volume/vsbsdl_test_volume.vcproj` & `libvsbsdl-20230506/msvscpp/vsbsdl_test_volume/vsbsdl_test_volume.vcproj`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/msvscpp/libclocale/libclocale.vcproj` & `libvsbsdl-20230506/msvscpp/libclocale/libclocale.vcproj`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/msvscpp/vsbsdl_test_sector_data/vsbsdl_test_sector_data.vcproj` & `libvsbsdl-20230506/msvscpp/vsbsdl_test_sector_data/vsbsdl_test_sector_data.vcproj`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/msvscpp/Makefile.am` & `libvsbsdl-20230506/msvscpp/Makefile.am`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/msvscpp/libbfio/libbfio.vcproj` & `libvsbsdl-20230506/msvscpp/libbfio/libbfio.vcproj`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/msvscpp/vsbsdl_test_error/vsbsdl_test_error.vcproj` & `libvsbsdl-20230506/msvscpp/vsbsdl_test_error/vsbsdl_test_error.vcproj`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/msvscpp/libvsbsdl.sln` & `libvsbsdl-20230506/msvscpp/libvsbsdl.sln`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/msvscpp/pyvsbsdl/pyvsbsdl.vcproj` & `libvsbsdl-20230506/msvscpp/pyvsbsdl/pyvsbsdl.vcproj`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/msvscpp/libcfile/libcfile.vcproj` & `libvsbsdl-20230506/msvscpp/libcfile/libcfile.vcproj`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/msvscpp/vsbsdl_test_partition/vsbsdl_test_partition.vcproj` & `libvsbsdl-20230506/msvscpp/vsbsdl_test_partition/vsbsdl_test_partition.vcproj`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/msvscpp/libcthreads/libcthreads.vcproj` & `libvsbsdl-20230506/msvscpp/libcthreads/libcthreads.vcproj`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/msvscpp/libcpath/libcpath.vcproj` & `libvsbsdl-20230506/msvscpp/libcpath/libcpath.vcproj`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/msvscpp/vsbsdlinfo/vsbsdlinfo.vcproj` & `libvsbsdl-20230506/msvscpp/vsbsdlinfo/vsbsdlinfo.vcproj`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/msvscpp/libuna/libuna.vcproj` & `libvsbsdl-20230506/msvscpp/libuna/libuna.vcproj`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/msvscpp/vsbsdl_test_tools_info_handle/vsbsdl_test_tools_info_handle.vcproj` & `libvsbsdl-20230506/msvscpp/vsbsdl_test_tools_info_handle/vsbsdl_test_tools_info_handle.vcproj`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/msvscpp/Makefile.in` & `libvsbsdl-20230506/msvscpp/Makefile.in`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/msvscpp/libcerror/libcerror.vcproj` & `libvsbsdl-20230506/msvscpp/libcerror/libcerror.vcproj`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/msvscpp/vsbsdl_test_disklabel/vsbsdl_test_disklabel.vcproj` & `libvsbsdl-20230506/msvscpp/vsbsdl_test_disklabel/vsbsdl_test_disklabel.vcproj`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/msvscpp/libcnotify/libcnotify.vcproj` & `libvsbsdl-20230506/msvscpp/libcnotify/libcnotify.vcproj`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/msvscpp/vsbsdl_test_partition_entry/vsbsdl_test_partition_entry.vcproj` & `libvsbsdl-20230506/msvscpp/vsbsdl_test_partition_entry/vsbsdl_test_partition_entry.vcproj`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/msvscpp/vsbsdl_test_tools_output/vsbsdl_test_tools_output.vcproj` & `libvsbsdl-20230506/msvscpp/vsbsdl_test_tools_output/vsbsdl_test_tools_output.vcproj`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/msvscpp/vsbsdl_test_tools_signal/vsbsdl_test_tools_signal.vcproj` & `libvsbsdl-20230506/msvscpp/vsbsdl_test_tools_signal/vsbsdl_test_tools_signal.vcproj`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/msvscpp/libvsbsdl/libvsbsdl.vcproj` & `libvsbsdl-20230506/msvscpp/libvsbsdl/libvsbsdl.vcproj`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/msvscpp/libfdata/libfdata.vcproj` & `libvsbsdl-20230506/msvscpp/libfdata/libfdata.vcproj`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/msvscpp/libcdata/libcdata.vcproj` & `libvsbsdl-20230506/msvscpp/libcdata/libcdata.vcproj`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/msvscpp/vsbsdl_test_notify/vsbsdl_test_notify.vcproj` & `libvsbsdl-20230506/msvscpp/vsbsdl_test_notify/vsbsdl_test_notify.vcproj`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/msvscpp/libcsplit/libcsplit.vcproj` & `libvsbsdl-20230506/msvscpp/libcsplit/libcsplit.vcproj`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/setup.py` & `libvsbsdl-20230506/setup.py`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/config.guess` & `libvsbsdl-20230506/config.guess`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libvsbsdl.spec.in` & `libvsbsdl-20230506/libvsbsdl.spec.in`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/ossfuzz/Makefile.am` & `libvsbsdl-20230506/ossfuzz/Makefile.am`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/ossfuzz/partition_fuzzer.cc` & `libvsbsdl-20230506/ossfuzz/partition_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/ossfuzz/volume_fuzzer.cc` & `libvsbsdl-20230506/ossfuzz/volume_fuzzer.cc`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/ossfuzz/ossfuzz_libvsbsdl.h` & `libvsbsdl-20230506/ossfuzz/ossfuzz_libvsbsdl.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/ossfuzz/Makefile.in` & `libvsbsdl-20230506/ossfuzz/Makefile.in`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/ossfuzz/ossfuzz_libbfio.h` & `libvsbsdl-20230506/ossfuzz/ossfuzz_libbfio.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/test-driver` & `libvsbsdl-20230506/test-driver`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/configure` & `libvsbsdl-20230506/configure`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #! /bin/sh
 # Guess values for system-dependent variables and create Makefiles.
-# Generated by GNU Autoconf 2.71 for libvsbsdl 20230502.
+# Generated by GNU Autoconf 2.71 for libvsbsdl 20230506.
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
 PACKAGE_NAME='libvsbsdl'
 PACKAGE_TARNAME='libvsbsdl'
-PACKAGE_VERSION='20230502'
-PACKAGE_STRING='libvsbsdl 20230502'
+PACKAGE_VERSION='20230506'
+PACKAGE_STRING='libvsbsdl 20230506'
 PACKAGE_BUGREPORT='joachim.metz@gmail.com'
 PACKAGE_URL=''
 
 ac_unique_file="include/libvsbsdl.h.in"
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
-\`configure' configures libvsbsdl 20230502 to adapt to many kinds of systems.
+\`configure' configures libvsbsdl 20230506 to adapt to many kinds of systems.
 
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
-     short | recursive ) echo "Configuration of libvsbsdl 20230502:";;
+     short | recursive ) echo "Configuration of libvsbsdl 20230506:";;
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
-libvsbsdl configure 20230502
+libvsbsdl configure 20230506
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
 
-It was created by libvsbsdl $as_me 20230502, which was
+It was created by libvsbsdl $as_me 20230506, which was
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
  PACKAGE='libvsbsdl'
- VERSION='20230502'
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
-This file was extended by libvsbsdl $as_me 20230502, which was
+This file was extended by libvsbsdl $as_me 20230506, which was
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
-libvsbsdl config.status 20230502
+libvsbsdl config.status 20230506
 configured by $0, generated by GNU Autoconf 2.71,
   with options \\"\$ac_cs_config\\"
 
 Copyright (C) 2021 Free Software Foundation, Inc.
 This config.status script is free software; the Free Software Foundation
 gives unlimited permission to copy, distribute and modify it."
```

### Comparing `libvsbsdl-20230502/libuna/libuna_url_stream.c` & `libvsbsdl-20230506/libuna/libuna_url_stream.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_mac_symbol.h` & `libvsbsdl-20230506/libuna/libuna_codepage_mac_symbol.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_support.c` & `libvsbsdl-20230506/libuna/libuna_support.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_scsu.h` & `libvsbsdl-20230506/libuna/libuna_scsu.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_iso_8859_5.c` & `libvsbsdl-20230506/libuna/libuna_codepage_iso_8859_5.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_iso_8859_2.c` & `libvsbsdl-20230506/libuna/libuna_codepage_iso_8859_2.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_windows_1253.c` & `libvsbsdl-20230506/libuna/libuna_codepage_windows_1253.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_koi8_u.h` & `libvsbsdl-20230506/libuna/libuna_codepage_koi8_u.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_windows_1252.c` & `libvsbsdl-20230506/libuna/libuna_codepage_windows_1252.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_utf32_stream.c` & `libvsbsdl-20230506/libuna/libuna_utf32_stream.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_windows_1257.h` & `libvsbsdl-20230506/libuna/libuna_codepage_windows_1257.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_mac_cyrillic.c` & `libvsbsdl-20230506/libuna/libuna_codepage_mac_cyrillic.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_mac_thai.c` & `libvsbsdl-20230506/libuna/libuna_codepage_mac_thai.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_utf32_string.c` & `libvsbsdl-20230506/libuna/libuna_utf32_string.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_mac_thai.h` & `libvsbsdl-20230506/libuna/libuna_codepage_mac_thai.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_windows_874.c` & `libvsbsdl-20230506/libuna/libuna_codepage_windows_874.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_windows_1251.h` & `libvsbsdl-20230506/libuna/libuna_codepage_windows_1251.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_libcerror.h` & `libvsbsdl-20230506/libuna/libuna_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_windows_949.c` & `libvsbsdl-20230506/libuna/libuna_codepage_windows_949.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_iso_8859_6.h` & `libvsbsdl-20230506/libuna/libuna_codepage_iso_8859_6.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_windows_1256.h` & `libvsbsdl-20230506/libuna/libuna_codepage_windows_1256.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_mac_greek.h` & `libvsbsdl-20230506/libuna/libuna_codepage_mac_greek.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_mac_russian.h` & `libvsbsdl-20230506/libuna/libuna_codepage_mac_russian.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_mac_ukrainian.h` & `libvsbsdl-20230506/libuna/libuna_codepage_mac_ukrainian.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_iso_8859_6.c` & `libvsbsdl-20230506/libuna/libuna_codepage_iso_8859_6.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_windows_874.h` & `libvsbsdl-20230506/libuna/libuna_codepage_windows_874.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_windows_1251.c` & `libvsbsdl-20230506/libuna/libuna_codepage_windows_1251.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_windows_1256.c` & `libvsbsdl-20230506/libuna/libuna_codepage_windows_1256.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_base16_stream.h` & `libvsbsdl-20230506/libuna/libuna_base16_stream.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_iso_8859_2.h` & `libvsbsdl-20230506/libuna/libuna_codepage_iso_8859_2.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/Makefile.am` & `libvsbsdl-20230506/libuna/Makefile.am`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_windows_1257.c` & `libvsbsdl-20230506/libuna/libuna_codepage_windows_1257.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_windows_1254.h` & `libvsbsdl-20230506/libuna/libuna_codepage_windows_1254.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_windows_1255.c` & `libvsbsdl-20230506/libuna/libuna_codepage_windows_1255.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_unused.h` & `libvsbsdl-20230506/libuna/libuna_unused.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_windows_1253.h` & `libvsbsdl-20230506/libuna/libuna_codepage_windows_1253.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_unicode_character.h` & `libvsbsdl-20230506/libuna/libuna_unicode_character.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_mac_dingbats.h` & `libvsbsdl-20230506/libuna/libuna_codepage_mac_dingbats.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_scsu.c` & `libvsbsdl-20230506/libuna/libuna_scsu.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_byte_stream.c` & `libvsbsdl-20230506/libuna/libuna_byte_stream.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_mac_celtic.h` & `libvsbsdl-20230506/libuna/libuna_codepage_mac_celtic.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_mac_croatian.c` & `libvsbsdl-20230506/libuna/libuna_codepage_mac_croatian.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_iso_8859_3.h` & `libvsbsdl-20230506/libuna/libuna_codepage_iso_8859_3.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_iso_8859_15.h` & `libvsbsdl-20230506/libuna/libuna_codepage_iso_8859_15.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_mac_roman.c` & `libvsbsdl-20230506/libuna/libuna_codepage_mac_roman.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_utf32_string.h` & `libvsbsdl-20230506/libuna/libuna_utf32_string.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_koi8_r.c` & `libvsbsdl-20230506/libuna/libuna_codepage_koi8_r.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_mac_icelandic.c` & `libvsbsdl-20230506/libuna/libuna_codepage_mac_icelandic.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_windows_936.h` & `libvsbsdl-20230506/libuna/libuna_codepage_windows_936.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_base64_stream.h` & `libvsbsdl-20230506/libuna/libuna_base64_stream.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_mac_celtic.c` & `libvsbsdl-20230506/libuna/libuna_codepage_mac_celtic.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_windows_950.c` & `libvsbsdl-20230506/libuna/libuna_codepage_windows_950.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_utf8_string.h` & `libvsbsdl-20230506/libuna/libuna_utf8_string.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_windows_936.c` & `libvsbsdl-20230506/libuna/libuna_codepage_windows_936.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_unicode_character.c` & `libvsbsdl-20230506/libuna/libuna_unicode_character.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_utf8_string.c` & `libvsbsdl-20230506/libuna/libuna_utf8_string.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_base32_stream.c` & `libvsbsdl-20230506/libuna/libuna_base32_stream.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_windows_950.h` & `libvsbsdl-20230506/libuna/libuna_codepage_windows_950.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_error.h` & `libvsbsdl-20230506/libuna/libuna_error.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_windows_932.h` & `libvsbsdl-20230506/libuna/libuna_codepage_windows_932.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_mac_turkish.h` & `libvsbsdl-20230506/libuna/libuna_codepage_mac_turkish.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_utf8_stream.c` & `libvsbsdl-20230506/libuna/libuna_utf8_stream.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_mac_ukrainian.c` & `libvsbsdl-20230506/libuna/libuna_codepage_mac_ukrainian.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_koi8_r.h` & `libvsbsdl-20230506/libuna/libuna_codepage_koi8_r.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_base16_stream.c` & `libvsbsdl-20230506/libuna/libuna_base16_stream.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_windows_1250.h` & `libvsbsdl-20230506/libuna/libuna_codepage_windows_1250.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_iso_8859_16.h` & `libvsbsdl-20230506/libuna/libuna_codepage_iso_8859_16.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_mac_croatian.h` & `libvsbsdl-20230506/libuna/libuna_codepage_mac_croatian.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_mac_gaelic.c` & `libvsbsdl-20230506/libuna/libuna_codepage_mac_gaelic.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_utf16_stream.h` & `libvsbsdl-20230506/libuna/libuna_utf16_stream.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_iso_8859_10.h` & `libvsbsdl-20230506/libuna/libuna_codepage_iso_8859_10.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_mac_centraleurroman.c` & `libvsbsdl-20230506/libuna/libuna_codepage_mac_centraleurroman.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_windows_932.c` & `libvsbsdl-20230506/libuna/libuna_codepage_windows_932.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_utf8_stream.h` & `libvsbsdl-20230506/libuna/libuna_utf8_stream.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_url_stream.h` & `libvsbsdl-20230506/libuna/libuna_url_stream.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_mac_farsi.c` & `libvsbsdl-20230506/libuna/libuna_codepage_mac_farsi.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_windows_949.h` & `libvsbsdl-20230506/libuna/libuna_codepage_windows_949.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_mac_romanian.h` & `libvsbsdl-20230506/libuna/libuna_codepage_mac_romanian.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_mac_gaelic.h` & `libvsbsdl-20230506/libuna/libuna_codepage_mac_gaelic.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_iso_8859_8.c` & `libvsbsdl-20230506/libuna/libuna_codepage_iso_8859_8.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_types.h` & `libvsbsdl-20230506/libuna/libuna_types.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_mac_arabic.c` & `libvsbsdl-20230506/libuna/libuna_codepage_mac_arabic.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_windows_1252.h` & `libvsbsdl-20230506/libuna/libuna_codepage_windows_1252.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_windows_1250.c` & `libvsbsdl-20230506/libuna/libuna_codepage_windows_1250.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_mac_russian.c` & `libvsbsdl-20230506/libuna/libuna_codepage_mac_russian.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_utf16_string.c` & `libvsbsdl-20230506/libuna/libuna_utf16_string.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_iso_8859_5.h` & `libvsbsdl-20230506/libuna/libuna_codepage_iso_8859_5.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_extern.h` & `libvsbsdl-20230506/libuna/libuna_extern.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_iso_8859_4.h` & `libvsbsdl-20230506/libuna/libuna_codepage_iso_8859_4.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_byte_stream.h` & `libvsbsdl-20230506/libuna/libuna_byte_stream.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_mac_roman.h` & `libvsbsdl-20230506/libuna/libuna_codepage_mac_roman.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_utf16_string.h` & `libvsbsdl-20230506/libuna/libuna_utf16_string.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_iso_8859_4.c` & `libvsbsdl-20230506/libuna/libuna_codepage_iso_8859_4.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_iso_8859_10.c` & `libvsbsdl-20230506/libuna/libuna_codepage_iso_8859_10.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_mac_icelandic.h` & `libvsbsdl-20230506/libuna/libuna_codepage_mac_icelandic.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/Makefile.in` & `libvsbsdl-20230506/libuna/Makefile.in`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_utf7_stream.h` & `libvsbsdl-20230506/libuna/libuna_utf7_stream.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_mac_symbol.c` & `libvsbsdl-20230506/libuna/libuna_codepage_mac_symbol.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_base32_stream.h` & `libvsbsdl-20230506/libuna/libuna_base32_stream.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_mac_turkish.c` & `libvsbsdl-20230506/libuna/libuna_codepage_mac_turkish.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_mac_inuit.c` & `libvsbsdl-20230506/libuna/libuna_codepage_mac_inuit.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_utf16_stream.c` & `libvsbsdl-20230506/libuna/libuna_utf16_stream.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_utf7_stream.c` & `libvsbsdl-20230506/libuna/libuna_utf7_stream.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_support.h` & `libvsbsdl-20230506/libuna/libuna_support.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_utf32_stream.h` & `libvsbsdl-20230506/libuna/libuna_utf32_stream.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_iso_8859_3.c` & `libvsbsdl-20230506/libuna/libuna_codepage_iso_8859_3.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_mac_greek.c` & `libvsbsdl-20230506/libuna/libuna_codepage_mac_greek.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_definitions.h` & `libvsbsdl-20230506/libuna/libuna_definitions.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_windows_1255.h` & `libvsbsdl-20230506/libuna/libuna_codepage_windows_1255.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_iso_8859_14.c` & `libvsbsdl-20230506/libuna/libuna_codepage_iso_8859_14.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_iso_8859_13.c` & `libvsbsdl-20230506/libuna/libuna_codepage_iso_8859_13.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_mac_centraleurroman.h` & `libvsbsdl-20230506/libuna/libuna_codepage_mac_centraleurroman.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_iso_8859_8.h` & `libvsbsdl-20230506/libuna/libuna_codepage_iso_8859_8.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_iso_8859_9.c` & `libvsbsdl-20230506/libuna/libuna_codepage_iso_8859_9.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_windows_1254.c` & `libvsbsdl-20230506/libuna/libuna_codepage_windows_1254.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_mac_cyrillic.h` & `libvsbsdl-20230506/libuna/libuna_codepage_mac_cyrillic.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_mac_arabic.h` & `libvsbsdl-20230506/libuna/libuna_codepage_mac_arabic.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_windows_1258.c` & `libvsbsdl-20230506/libuna/libuna_codepage_windows_1258.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_mac_farsi.h` & `libvsbsdl-20230506/libuna/libuna_codepage_mac_farsi.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_iso_8859_15.c` & `libvsbsdl-20230506/libuna/libuna_codepage_iso_8859_15.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_iso_8859_7.c` & `libvsbsdl-20230506/libuna/libuna_codepage_iso_8859_7.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_mac_dingbats.c` & `libvsbsdl-20230506/libuna/libuna_codepage_mac_dingbats.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_iso_8859_9.h` & `libvsbsdl-20230506/libuna/libuna_codepage_iso_8859_9.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_windows_1258.h` & `libvsbsdl-20230506/libuna/libuna_codepage_windows_1258.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_base64_stream.c` & `libvsbsdl-20230506/libuna/libuna_base64_stream.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_mac_romanian.c` & `libvsbsdl-20230506/libuna/libuna_codepage_mac_romanian.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_error.c` & `libvsbsdl-20230506/libuna/libuna_error.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_koi8_u.c` & `libvsbsdl-20230506/libuna/libuna_codepage_koi8_u.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_iso_8859_13.h` & `libvsbsdl-20230506/libuna/libuna_codepage_iso_8859_13.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_iso_8859_7.h` & `libvsbsdl-20230506/libuna/libuna_codepage_iso_8859_7.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_iso_8859_14.h` & `libvsbsdl-20230506/libuna/libuna_codepage_iso_8859_14.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_mac_inuit.h` & `libvsbsdl-20230506/libuna/libuna_codepage_mac_inuit.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libuna/libuna_codepage_iso_8859_16.c` & `libvsbsdl-20230506/libuna/libuna_codepage_iso_8859_16.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/Makefile.in` & `libvsbsdl-20230506/Makefile.in`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/m4/libuna.m4` & `libvsbsdl-20230506/m4/libuna.m4`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/m4/gettext.m4` & `libvsbsdl-20230506/m4/gettext.m4`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/m4/tests.m4` & `libvsbsdl-20230506/m4/tests.m4`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/m4/lib-prefix.m4` & `libvsbsdl-20230506/m4/lib-prefix.m4`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/m4/ltoptions.m4` & `libvsbsdl-20230506/m4/ltoptions.m4`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/m4/libcpath.m4` & `libvsbsdl-20230506/m4/libcpath.m4`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/m4/lib-ld.m4` & `libvsbsdl-20230506/m4/lib-ld.m4`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/m4/libcthreads.m4` & `libvsbsdl-20230506/m4/libcthreads.m4`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/m4/lib-link.m4` & `libvsbsdl-20230506/m4/lib-link.m4`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/m4/python.m4` & `libvsbsdl-20230506/m4/python.m4`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/m4/libtool.m4` & `libvsbsdl-20230506/m4/libtool.m4`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/m4/nls.m4` & `libvsbsdl-20230506/m4/nls.m4`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/m4/libclocale.m4` & `libvsbsdl-20230506/m4/libclocale.m4`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/m4/libfdata.m4` & `libvsbsdl-20230506/m4/libfdata.m4`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/m4/host-cpu-c-abi.m4` & `libvsbsdl-20230506/m4/host-cpu-c-abi.m4`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/m4/libcnotify.m4` & `libvsbsdl-20230506/m4/libcnotify.m4`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/m4/ltversion.m4` & `libvsbsdl-20230506/m4/ltversion.m4`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/m4/libcdata.m4` & `libvsbsdl-20230506/m4/libcdata.m4`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/m4/progtest.m4` & `libvsbsdl-20230506/m4/progtest.m4`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/m4/lt~obsolete.m4` & `libvsbsdl-20230506/m4/lt~obsolete.m4`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/m4/libcfile.m4` & `libvsbsdl-20230506/m4/libcfile.m4`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/m4/po.m4` & `libvsbsdl-20230506/m4/po.m4`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/m4/pthread.m4` & `libvsbsdl-20230506/m4/pthread.m4`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/m4/common.m4` & `libvsbsdl-20230506/m4/common.m4`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/m4/libcerror.m4` & `libvsbsdl-20230506/m4/libcerror.m4`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/m4/iconv.m4` & `libvsbsdl-20230506/m4/iconv.m4`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/m4/ltsugar.m4` & `libvsbsdl-20230506/m4/ltsugar.m4`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/m4/libfcache.m4` & `libvsbsdl-20230506/m4/libfcache.m4`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/m4/libcsplit.m4` & `libvsbsdl-20230506/m4/libcsplit.m4`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/m4/intlmacosx.m4` & `libvsbsdl-20230506/m4/intlmacosx.m4`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/m4/types.m4` & `libvsbsdl-20230506/m4/types.m4`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/m4/libbfio.m4` & `libvsbsdl-20230506/m4/libbfio.m4`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/COPYING.LESSER` & `libvsbsdl-20230506/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/pyvsbsdl-python3/Makefile.am` & `libvsbsdl-20230506/pyvsbsdl-python3/Makefile.am`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/pyvsbsdl-python3/Makefile.in` & `libvsbsdl-20230506/pyvsbsdl-python3/Makefile.in`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcerror/libcerror_system.c` & `libvsbsdl-20230506/libcerror/libcerror_system.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcerror/libcerror_error.c` & `libvsbsdl-20230506/libcerror/libcerror_error.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcerror/libcerror_extern.h` & `libvsbsdl-20230506/libcerror/libcerror_extern.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcerror/Makefile.am` & `libvsbsdl-20230506/libcerror/Makefile.am`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcerror/libcerror_error.h` & `libvsbsdl-20230506/libcerror/libcerror_error.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcerror/libcerror_support.h` & `libvsbsdl-20230506/libcerror/libcerror_support.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcerror/libcerror_types.h` & `libvsbsdl-20230506/libcerror/libcerror_types.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcerror/libcerror_definitions.h` & `libvsbsdl-20230506/libcerror/libcerror_definitions.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcerror/libcerror_unused.h` & `libvsbsdl-20230506/libcerror/libcerror_unused.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcerror/Makefile.in` & `libvsbsdl-20230506/libcerror/Makefile.in`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcerror/libcerror_support.c` & `libvsbsdl-20230506/libcerror/libcerror_support.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcerror/libcerror_system.h` & `libvsbsdl-20230506/libcerror/libcerror_system.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcnotify/libcnotify_libcerror.h` & `libvsbsdl-20230506/libcnotify/libcnotify_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcnotify/libcnotify_unused.h` & `libvsbsdl-20230506/libcnotify/libcnotify_unused.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcnotify/libcnotify_support.h` & `libvsbsdl-20230506/libcnotify/libcnotify_support.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcnotify/libcnotify_support.c` & `libvsbsdl-20230506/libcnotify/libcnotify_support.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcnotify/Makefile.am` & `libvsbsdl-20230506/libcnotify/Makefile.am`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcnotify/libcnotify_print.c` & `libvsbsdl-20230506/libcnotify/libcnotify_print.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcnotify/libcnotify_verbose.c` & `libvsbsdl-20230506/libcnotify/libcnotify_verbose.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcnotify/libcnotify_stream.h` & `libvsbsdl-20230506/libcnotify/libcnotify_stream.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcnotify/libcnotify_extern.h` & `libvsbsdl-20230506/libcnotify/libcnotify_extern.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcnotify/libcnotify_stream.c` & `libvsbsdl-20230506/libcnotify/libcnotify_stream.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcnotify/Makefile.in` & `libvsbsdl-20230506/libcnotify/Makefile.in`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcnotify/libcnotify_print.h` & `libvsbsdl-20230506/libcnotify/libcnotify_print.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcnotify/libcnotify_verbose.h` & `libvsbsdl-20230506/libcnotify/libcnotify_verbose.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcnotify/libcnotify_definitions.h` & `libvsbsdl-20230506/libcnotify/libcnotify_definitions.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/ltmain.sh` & `libvsbsdl-20230506/ltmain.sh`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/compile` & `libvsbsdl-20230506/compile`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/config.rpath` & `libvsbsdl-20230506/config.rpath`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libvsbsdl/libvsbsdl_definitions.h` & `libvsbsdl-20230506/libvsbsdl/libvsbsdl_definitions.h`

 * *Files 1% similar despite different names*

```diff
@@ -29,19 +29,19 @@
 #if !defined( HAVE_LOCAL_LIBVSBSDL )
 #include <libvsbsdl/definitions.h>
 
 /* The definitions in <libvsbsdl/definitions.h> are copied here
  * for local use of libvsbsdl
  */
 #else
-#define LIBVSBSDL_VERSION			20230502
+#define LIBVSBSDL_VERSION			20230506
 
 /* The libvsbsdl version string
  */
-#define LIBVSBSDL_VERSION_STRING		"20230502"
+#define LIBVSBSDL_VERSION_STRING		"20230506"
 
 /* The endian definitions
  */
 #define LIBVSBSDL_ENDIAN_BIG			_BYTE_STREAM_ENDIAN_BIG
 #define LIBVSBSDL_ENDIAN_LITTLE			_BYTE_STREAM_ENDIAN_LITTLE
 
 /* The access flags definitions
```

### Comparing `libvsbsdl-20230502/libvsbsdl/libvsbsdl_disklabel.c` & `libvsbsdl-20230506/libvsbsdl/libvsbsdl_disklabel.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libvsbsdl/libvsbsdl_error.h` & `libvsbsdl-20230506/libvsbsdl/libvsbsdl_error.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libvsbsdl/libvsbsdl_libclocale.h` & `libvsbsdl-20230506/libvsbsdl/libvsbsdl_libclocale.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libvsbsdl/libvsbsdl_debug.c` & `libvsbsdl-20230506/libvsbsdl/libvsbsdl_debug.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libvsbsdl/libvsbsdl_support.h` & `libvsbsdl-20230506/libvsbsdl/libvsbsdl_support.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libvsbsdl/libvsbsdl_libfcache.h` & `libvsbsdl-20230506/libvsbsdl/libvsbsdl_libfcache.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libvsbsdl/libvsbsdl_sector_data.h` & `libvsbsdl-20230506/libvsbsdl/libvsbsdl_sector_data.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libvsbsdl/libvsbsdl_partition_entry.h` & `libvsbsdl-20230506/libvsbsdl/libvsbsdl_partition_entry.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libvsbsdl/libvsbsdl_disklabel.h` & `libvsbsdl-20230506/libvsbsdl/libvsbsdl_disklabel.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libvsbsdl/libvsbsdl_partition.c` & `libvsbsdl-20230506/libvsbsdl/libvsbsdl_partition.c`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,18 @@
 		libcerror_error_set(
 		 error,
 		 LIBCERROR_ERROR_DOMAIN_MEMORY,
 		 LIBCERROR_MEMORY_ERROR_SET_FAILED,
 		 "%s: unable to clear partition.",
 		 function );
 
-		goto on_error;
+		memory_free(
+		 internal_partition );
+
+		return( -1 );
 	}
 	if( libvsbsdl_partition_entry_get_start_sector(
 	     partition_entry,
 	     (uint32_t *) &partition_offset,
 	     error ) != 1 )
 	{
 		libcerror_error_set(
@@ -232,14 +235,20 @@
 	*partition = (libvsbsdl_partition_t *) internal_partition;
 
 	return( 1 );
 
 on_error:
 	if( internal_partition != NULL )
 	{
+		if( internal_partition->sectors_vector != NULL )
+		{
+			libfdata_vector_free(
+			 &( internal_partition->sectors_vector ),
+			 NULL );
+		}
 		memory_free(
 		 internal_partition );
 	}
 	return( -1 );
 }
 
 /* Frees a partition
```

### Comparing `libvsbsdl-20230502/libvsbsdl/libvsbsdl_volume.c` & `libvsbsdl-20230506/libvsbsdl/libvsbsdl_volume.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libvsbsdl/libvsbsdl_io_handle.c` & `libvsbsdl-20230506/libvsbsdl/libvsbsdl_io_handle.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libvsbsdl/libvsbsdl_notify.h` & `libvsbsdl-20230506/libvsbsdl/libvsbsdl_notify.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libvsbsdl/libvsbsdl_partition_entry.c` & `libvsbsdl-20230506/libvsbsdl/libvsbsdl_partition_entry.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libvsbsdl/Makefile.am` & `libvsbsdl-20230506/libvsbsdl/Makefile.am`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libvsbsdl/libvsbsdl_libfdata.h` & `libvsbsdl-20230506/libvsbsdl/libvsbsdl_libfdata.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libvsbsdl/libvsbsdl_types.h` & `libvsbsdl-20230506/libvsbsdl/libvsbsdl_types.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libvsbsdl/libvsbsdl_io_handle.h` & `libvsbsdl-20230506/libvsbsdl/libvsbsdl_io_handle.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libvsbsdl/libvsbsdl.rc` & `libvsbsdl-20230506/libvsbsdl/libvsbsdl.rc`

 * *Files 1% similar despite different names*

```diff
@@ -18,20 +18,20 @@
   FILESUBTYPE				0x0L
 BEGIN
   BLOCK "StringFileInfo"
   BEGIN
     BLOCK "040904E4"
     BEGIN
       VALUE "FileDescription",		"Library to access the BSD disklabel volume system format\0"
-      VALUE "FileVersion",		"20230502" "\0"
+      VALUE "FileVersion",		"20230506" "\0"
       VALUE "InternalName",		"libvsbsdl.dll\0"
       VALUE "LegalCopyright",		"(C) 2023, Joachim Metz <joachim.metz@gmail.com>\0"
       VALUE "OriginalFilename",		"libvsbsdl.dll\0"
       VALUE "ProductName",		"libvsbsdl\0"
-      VALUE "ProductVersion",		"20230502" "\0"
+      VALUE "ProductVersion",		"20230506" "\0"
       VALUE "Comments",			"For more information visit https://github.com/libyal/libvsbsdl/\0"
     END
   END
   BLOCK "VarFileInfo"
   BEGIN
     VALUE "Translation", 0x0409, 1200
   END
```

### Comparing `libvsbsdl-20230502/libvsbsdl/libvsbsdl_libbfio.h` & `libvsbsdl-20230506/libvsbsdl/libvsbsdl_libbfio.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libvsbsdl/vsbsdl_partition_entry.h` & `libvsbsdl-20230506/libvsbsdl/vsbsdl_partition_entry.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libvsbsdl/libvsbsdl.c` & `libvsbsdl-20230506/libvsbsdl/libvsbsdl.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libvsbsdl/libvsbsdl_definitions.h.in` & `libvsbsdl-20230506/libvsbsdl/libvsbsdl_definitions.h.in`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libvsbsdl/libvsbsdl_extern.h` & `libvsbsdl-20230506/libvsbsdl/libvsbsdl_extern.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libvsbsdl/vsbsdl_disklabel.h` & `libvsbsdl-20230506/libvsbsdl/vsbsdl_disklabel.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libvsbsdl/libvsbsdl_libcerror.h` & `libvsbsdl-20230506/libvsbsdl/libvsbsdl_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libvsbsdl/libvsbsdl_libcnotify.h` & `libvsbsdl-20230506/libvsbsdl/libvsbsdl_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libvsbsdl/libvsbsdl_libcdata.h` & `libvsbsdl-20230506/libvsbsdl/libvsbsdl_libcdata.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libvsbsdl/libvsbsdl_debug.h` & `libvsbsdl-20230506/libvsbsdl/libvsbsdl_debug.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libvsbsdl/libvsbsdl_volume.h` & `libvsbsdl-20230506/libvsbsdl/libvsbsdl_volume.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libvsbsdl/libvsbsdl_error.c` & `libvsbsdl-20230506/libvsbsdl/libvsbsdl_error.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libvsbsdl/libvsbsdl_unused.h` & `libvsbsdl-20230506/libvsbsdl/libvsbsdl_unused.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libvsbsdl/Makefile.in` & `libvsbsdl-20230506/libvsbsdl/Makefile.in`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libvsbsdl/libvsbsdl_libcthreads.h` & `libvsbsdl-20230506/libvsbsdl/libvsbsdl_libcthreads.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libvsbsdl/libvsbsdl_sector_data.c` & `libvsbsdl-20230506/libvsbsdl/libvsbsdl_sector_data.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libvsbsdl/libvsbsdl_support.c` & `libvsbsdl-20230506/libvsbsdl/libvsbsdl_support.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libvsbsdl/libvsbsdl_partition.h` & `libvsbsdl-20230506/libvsbsdl/libvsbsdl_partition.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libvsbsdl/libvsbsdl_notify.c` & `libvsbsdl-20230506/libvsbsdl/libvsbsdl_notify.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libvsbsdl/libvsbsdl.rc.in` & `libvsbsdl-20230506/libvsbsdl/libvsbsdl.rc.in`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/depcomp` & `libvsbsdl-20230506/depcomp`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/po/en@quot.header` & `libvsbsdl-20230506/po/en@quot.header`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/po/Rules-quot` & `libvsbsdl-20230506/po/Rules-quot`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/po/remove-potcdate.sin` & `libvsbsdl-20230506/po/remove-potcdate.sin`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/po/Makevars.in` & `libvsbsdl-20230506/po/Makevars.in`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/po/en@boldquot.header` & `libvsbsdl-20230506/po/en@boldquot.header`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/po/Makevars` & `libvsbsdl-20230506/po/Makevars`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/po/insert-header.sin` & `libvsbsdl-20230506/po/insert-header.sin`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/po/Makefile.in.in` & `libvsbsdl-20230506/po/Makefile.in.in`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libvsbsdl.spec` & `libvsbsdl-20230506/libvsbsdl.spec`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 Name: libvsbsdl
-Version: 20230502
+Version: 20230506
 Release: 1
 Summary: Library to access the BSD disklabel volume system format
 Group: System Environment/Libraries
 License: LGPLv3+
 Source: %{name}-%{version}.tar.gz
 URL: https://github.com/libyal/libvsbsdl
 BuildRoot: %{_tmppath}/%{name}-%{version}-%{release}-root-%(%{__id_u} -n)
@@ -96,10 +96,10 @@
 %defattr(644,root,root,755)
 %license COPYING COPYING.LESSER
 %doc AUTHORS README
 %attr(755,root,root) %{_bindir}/*
 %{_mandir}/man1/*
 
 %changelog
-* Thu May  4 2023 Joachim Metz <joachim.metz@gmail.com> 20230502-1
+* Sat May  6 2023 Joachim Metz <joachim.metz@gmail.com> 20230506-1
 - Auto-generated
```

### Comparing `libvsbsdl-20230502/libfdata/libfdata_segments_array.h` & `libvsbsdl-20230506/libfdata/libfdata_segments_array.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libfdata/libfdata_cache.c` & `libvsbsdl-20230506/libfdata/libfdata_cache.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libfdata/libfdata_support.c` & `libvsbsdl-20230506/libfdata/libfdata_support.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libfdata/libfdata_list_element.c` & `libvsbsdl-20230506/libfdata/libfdata_list_element.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libfdata/libfdata_mapped_range.h` & `libvsbsdl-20230506/libfdata/libfdata_mapped_range.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libfdata/libfdata_extern.h` & `libvsbsdl-20230506/libfdata/libfdata_extern.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libfdata/libfdata_list.c` & `libvsbsdl-20230506/libfdata/libfdata_list.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libfdata/libfdata_libcdata.h` & `libvsbsdl-20230506/libfdata/libfdata_libcdata.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libfdata/libfdata_notify.h` & `libvsbsdl-20230506/libfdata/libfdata_notify.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libfdata/libfdata_range_list.h` & `libvsbsdl-20230506/libfdata/libfdata_range_list.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libfdata/Makefile.am` & `libvsbsdl-20230506/libfdata/Makefile.am`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libfdata/libfdata_error.c` & `libvsbsdl-20230506/libfdata/libfdata_error.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libfdata/libfdata_list.h` & `libvsbsdl-20230506/libfdata/libfdata_list.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libfdata/libfdata_area.h` & `libvsbsdl-20230506/libfdata/libfdata_area.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libfdata/libfdata_types.h` & `libvsbsdl-20230506/libfdata/libfdata_types.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libfdata/libfdata_area.c` & `libvsbsdl-20230506/libfdata/libfdata_area.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libfdata/libfdata_range.h` & `libvsbsdl-20230506/libfdata/libfdata_range.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libfdata/libfdata_vector.c` & `libvsbsdl-20230506/libfdata/libfdata_vector.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libfdata/libfdata_stream.h` & `libvsbsdl-20230506/libfdata/libfdata_stream.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libfdata/libfdata_vector.h` & `libvsbsdl-20230506/libfdata/libfdata_vector.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libfdata/libfdata_support.h` & `libvsbsdl-20230506/libfdata/libfdata_support.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libfdata/libfdata_libfcache.h` & `libvsbsdl-20230506/libfdata/libfdata_libfcache.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libfdata/libfdata_libcerror.h` & `libvsbsdl-20230506/libfdata/libfdata_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libfdata/libfdata_range_list.c` & `libvsbsdl-20230506/libfdata/libfdata_range_list.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libfdata/libfdata_libcnotify.h` & `libvsbsdl-20230506/libfdata/libfdata_libcnotify.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libfdata/libfdata_notify.c` & `libvsbsdl-20230506/libfdata/libfdata_notify.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libfdata/libfdata_list_element.h` & `libvsbsdl-20230506/libfdata/libfdata_list_element.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libfdata/libfdata_unused.h` & `libvsbsdl-20230506/libfdata/libfdata_unused.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libfdata/libfdata_error.h` & `libvsbsdl-20230506/libfdata/libfdata_error.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libfdata/Makefile.in` & `libvsbsdl-20230506/libfdata/Makefile.in`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libfdata/libfdata_cache.h` & `libvsbsdl-20230506/libfdata/libfdata_cache.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libfdata/libfdata_stream.c` & `libvsbsdl-20230506/libfdata/libfdata_stream.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libfdata/libfdata_segments_array.c` & `libvsbsdl-20230506/libfdata/libfdata_segments_array.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libfdata/libfdata_mapped_range.c` & `libvsbsdl-20230506/libfdata/libfdata_mapped_range.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libfdata/libfdata_definitions.h` & `libvsbsdl-20230506/libfdata/libfdata_definitions.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libfdata/libfdata_range.c` & `libvsbsdl-20230506/libfdata/libfdata_range.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcdata/libcdata_array.c` & `libvsbsdl-20230506/libcdata/libcdata_array.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcdata/libcdata_btree_node.c` & `libvsbsdl-20230506/libcdata/libcdata_btree_node.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcdata/libcdata_tree_node.c` & `libvsbsdl-20230506/libcdata/libcdata_tree_node.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcdata/libcdata_libcthreads.h` & `libvsbsdl-20230506/libcdata/libcdata_libcthreads.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcdata/libcdata_range_list_value.h` & `libvsbsdl-20230506/libcdata/libcdata_range_list_value.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcdata/libcdata_unused.h` & `libvsbsdl-20230506/libcdata/libcdata_unused.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcdata/libcdata_range_list.h` & `libvsbsdl-20230506/libcdata/libcdata_range_list.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcdata/Makefile.am` & `libvsbsdl-20230506/libcdata/Makefile.am`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcdata/libcdata_range_list.c` & `libvsbsdl-20230506/libcdata/libcdata_range_list.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcdata/libcdata_extern.h` & `libvsbsdl-20230506/libcdata/libcdata_extern.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcdata/libcdata_support.c` & `libvsbsdl-20230506/libcdata/libcdata_support.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcdata/libcdata_list_element.h` & `libvsbsdl-20230506/libcdata/libcdata_list_element.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcdata/libcdata_btree_values_list.c` & `libvsbsdl-20230506/libcdata/libcdata_btree_values_list.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcdata/libcdata_range_list_value.c` & `libvsbsdl-20230506/libcdata/libcdata_range_list_value.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcdata/libcdata_libcerror.h` & `libvsbsdl-20230506/libcdata/libcdata_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcdata/libcdata_error.c` & `libvsbsdl-20230506/libcdata/libcdata_error.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcdata/libcdata_error.h` & `libvsbsdl-20230506/libcdata/libcdata_error.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcdata/libcdata_support.h` & `libvsbsdl-20230506/libcdata/libcdata_support.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcdata/libcdata_btree_node.h` & `libvsbsdl-20230506/libcdata/libcdata_btree_node.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcdata/libcdata_list.c` & `libvsbsdl-20230506/libcdata/libcdata_list.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcdata/libcdata_tree_node.h` & `libvsbsdl-20230506/libcdata/libcdata_tree_node.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcdata/libcdata_list.h` & `libvsbsdl-20230506/libcdata/libcdata_list.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcdata/libcdata_types.h` & `libvsbsdl-20230506/libcdata/libcdata_types.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcdata/libcdata_list_element.c` & `libvsbsdl-20230506/libcdata/libcdata_list_element.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcdata/Makefile.in` & `libvsbsdl-20230506/libcdata/Makefile.in`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcdata/libcdata_btree_values_list.h` & `libvsbsdl-20230506/libcdata/libcdata_btree_values_list.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcdata/libcdata_array.h` & `libvsbsdl-20230506/libcdata/libcdata_array.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcdata/libcdata_btree.h` & `libvsbsdl-20230506/libcdata/libcdata_btree.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcdata/libcdata_definitions.h` & `libvsbsdl-20230506/libcdata/libcdata_definitions.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcdata/libcdata_btree.c` & `libvsbsdl-20230506/libcdata/libcdata_btree.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/pyvsbsdl-python2/Makefile.am` & `libvsbsdl-20230506/pyvsbsdl-python2/Makefile.am`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/pyvsbsdl-python2/Makefile.in` & `libvsbsdl-20230506/pyvsbsdl-python2/Makefile.in`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/acinclude.m4` & `libvsbsdl-20230506/acinclude.m4`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcsplit/libcsplit_types.h` & `libvsbsdl-20230506/libcsplit/libcsplit_types.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcsplit/libcsplit_wide_string.h` & `libvsbsdl-20230506/libcsplit/libcsplit_wide_string.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcsplit/libcsplit_error.h` & `libvsbsdl-20230506/libcsplit/libcsplit_error.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcsplit/libcsplit_support.h` & `libvsbsdl-20230506/libcsplit/libcsplit_support.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcsplit/libcsplit_narrow_split_string.c` & `libvsbsdl-20230506/libcsplit/libcsplit_narrow_split_string.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcsplit/libcsplit_narrow_split_string.h` & `libvsbsdl-20230506/libcsplit/libcsplit_narrow_split_string.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcsplit/Makefile.am` & `libvsbsdl-20230506/libcsplit/Makefile.am`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcsplit/libcsplit_wide_split_string.c` & `libvsbsdl-20230506/libcsplit/libcsplit_wide_split_string.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcsplit/libcsplit_narrow_string.h` & `libvsbsdl-20230506/libcsplit/libcsplit_narrow_string.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcsplit/libcsplit_unused.h` & `libvsbsdl-20230506/libcsplit/libcsplit_unused.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcsplit/libcsplit_wide_string.c` & `libvsbsdl-20230506/libcsplit/libcsplit_wide_string.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcsplit/libcsplit_narrow_string.c` & `libvsbsdl-20230506/libcsplit/libcsplit_narrow_string.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcsplit/Makefile.in` & `libvsbsdl-20230506/libcsplit/Makefile.in`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcsplit/libcsplit_wide_split_string.h` & `libvsbsdl-20230506/libcsplit/libcsplit_wide_split_string.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcsplit/libcsplit_definitions.h` & `libvsbsdl-20230506/libcsplit/libcsplit_definitions.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcsplit/libcsplit_error.c` & `libvsbsdl-20230506/libcsplit/libcsplit_error.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcsplit/libcsplit_support.c` & `libvsbsdl-20230506/libcsplit/libcsplit_support.c`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcsplit/libcsplit_libcerror.h` & `libvsbsdl-20230506/libcsplit/libcsplit_libcerror.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/libcsplit/libcsplit_extern.h` & `libvsbsdl-20230506/libcsplit/libcsplit_extern.h`

 * *Files identical despite different names*

### Comparing `libvsbsdl-20230502/configure.ac` & `libvsbsdl-20230506/configure.ac`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 AC_PREREQ([2.71])
 
 AC_INIT(
  [libvsbsdl],
- [20230502],
+ [20230506],
  [joachim.metz@gmail.com])
 
 AC_CONFIG_SRCDIR(
  [include/libvsbsdl.h.in])
 
 AM_INIT_AUTOMAKE([gnu 1.6 tar-ustar])
```

