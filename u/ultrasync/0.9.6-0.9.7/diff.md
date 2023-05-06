# Comparing `tmp/ultrasync-0.9.6.tar.gz` & `tmp/ultrasync-0.9.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ultrasync-0.9.6.tar", last modified: Sat Mar 25 17:53:14 2023, max compression
+gzip compressed data, was "ultrasync-0.9.7.tar", last modified: Sat May  6 17:20:32 2023, max compression
```

## Comparing `ultrasync-0.9.6.tar` & `ultrasync-0.9.7.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-03-25 17:53:14.353669 ultrasync-0.9.6/
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     1090 2020-11-22 16:33:46.000000 ultrasync-0.9.6/LICENSE
--rw-rw-r--   0 l2g       (1000) l2g       (1000)      191 2020-11-22 16:33:46.000000 ultrasync-0.9.6/MANIFEST.in
--rw-r--r--   0 l2g       (1000) l2g       (1000)     7208 2023-03-25 17:53:14.353669 ultrasync-0.9.6/PKG-INFO
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     6235 2021-09-20 21:40:13.000000 ultrasync-0.9.6/README.md
--rw-rw-r--   0 l2g       (1000) l2g       (1000)       43 2020-11-22 16:33:46.000000 ultrasync-0.9.6/dev-requirements.txt
--rw-rw-r--   0 l2g       (1000) l2g       (1000)       15 2020-11-22 16:33:46.000000 ultrasync-0.9.6/requirements.txt
--rw-rw-r--   0 l2g       (1000) l2g       (1000)      335 2023-03-25 17:53:14.354669 ultrasync-0.9.6/setup.cfg
--rwxrwxr-x   0 l2g       (1000) l2g       (1000)     3031 2023-03-25 17:52:58.000000 ultrasync-0.9.6/setup.py
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-03-25 17:53:14.325669 ultrasync-0.9.6/tests/
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     5121 2020-11-22 16:33:46.000000 ultrasync-0.9.6/tests/test_cli.py
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     7424 2021-01-25 19:18:33.000000 ultrasync-0.9.6/tests/test_comnav_0_106.py
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     6360 2021-01-25 19:18:33.000000 ultrasync-0.9.6/tests/test_comnav_0_108-zone-check.py
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     6635 2021-01-25 19:18:33.000000 ultrasync-0.9.6/tests/test_comnav_0_108.py
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     4922 2021-01-25 19:18:33.000000 ultrasync-0.9.6/tests/test_comnav_0_108_burglar_alarm_on.py
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     3873 2020-11-22 16:33:46.000000 ultrasync-0.9.6/tests/test_config.py
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     4828 2022-07-01 13:18:56.000000 ultrasync-0.9.6/tests/test_xgen8_bypass.py
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     7289 2021-09-20 21:40:13.000000 ultrasync-0.9.6/tests/test_xgen8_nxg8zbo.py
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     7984 2021-09-19 13:53:23.000000 ultrasync-0.9.6/tests/test_xgen_general.py
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     4590 2021-01-25 19:18:33.000000 ultrasync-0.9.6/tests/test_zerowire_armed.py
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     6543 2021-01-25 19:18:33.000000 ultrasync-0.9.6/tests/test_zerowire_general.py
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-03-25 17:53:14.317669 ultrasync-0.9.6/tests/var/
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-03-25 17:53:14.317669 ultrasync-0.9.6/tests/var/comnav/
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-03-25 17:53:14.329669 ultrasync-0.9.6/tests/var/comnav/0.106/
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     1892 2020-11-22 16:33:46.000000 ultrasync-0.9.6/tests/var/comnav/0.106/area.htm
--rw-rw-r--   0 l2g       (1000) l2g       (1000)    36123 2020-11-22 16:33:46.000000 ultrasync-0.9.6/tests/var/comnav/0.106/master.js
--rw-rw-r--   0 l2g       (1000) l2g       (1000)       96 2020-11-22 16:33:46.000000 ultrasync-0.9.6/tests/var/comnav/0.106/seq.w.update.xml
--rw-rw-r--   0 l2g       (1000) l2g       (1000)       96 2020-11-22 16:33:46.000000 ultrasync-0.9.6/tests/var/comnav/0.106/seq.xml
--rw-rw-r--   0 l2g       (1000) l2g       (1000)    21526 2020-11-22 16:33:46.000000 ultrasync-0.9.6/tests/var/comnav/0.106/status.js
--rw-rw-r--   0 l2g       (1000) l2g       (1000)      436 2020-11-22 16:33:46.000000 ultrasync-0.9.6/tests/var/comnav/0.106/status.xml
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     1832 2020-11-22 16:33:46.000000 ultrasync-0.9.6/tests/var/comnav/0.106/zones.htm
--rw-rw-r--   0 l2g       (1000) l2g       (1000)       82 2020-11-22 16:33:46.000000 ultrasync-0.9.6/tests/var/comnav/0.106/zstate.bank0.w.update.xml
--rw-rw-r--   0 l2g       (1000) l2g       (1000)       81 2020-11-22 16:33:46.000000 ultrasync-0.9.6/tests/var/comnav/0.106/zstate.bank4.w.update.xml
--rw-rw-r--   0 l2g       (1000) l2g       (1000)       82 2020-11-22 16:33:46.000000 ultrasync-0.9.6/tests/var/comnav/0.106/zstate.xml
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-03-25 17:53:14.332669 ultrasync-0.9.6/tests/var/comnav/0.108/
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     1971 2020-11-22 16:33:46.000000 ultrasync-0.9.6/tests/var/comnav/0.108/area.htm
--rw-rw-r--   0 l2g       (1000) l2g       (1000)    23023 2020-11-22 16:33:46.000000 ultrasync-0.9.6/tests/var/comnav/0.108/master.js
--rw-rw-r--   0 l2g       (1000) l2g       (1000)       92 2020-11-22 16:33:46.000000 ultrasync-0.9.6/tests/var/comnav/0.108/seq.w.update.xml
--rw-rw-r--   0 l2g       (1000) l2g       (1000)       92 2020-11-22 16:33:46.000000 ultrasync-0.9.6/tests/var/comnav/0.108/seq.xml
--rw-rw-r--   0 l2g       (1000) l2g       (1000)    18114 2020-11-22 16:33:46.000000 ultrasync-0.9.6/tests/var/comnav/0.108/status.js
--rw-rw-r--   0 l2g       (1000) l2g       (1000)      436 2020-11-22 16:33:46.000000 ultrasync-0.9.6/tests/var/comnav/0.108/status.xml
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     2793 2020-11-22 16:33:46.000000 ultrasync-0.9.6/tests/var/comnav/0.108/zones.htm
--rw-rw-r--   0 l2g       (1000) l2g       (1000)       98 2020-11-22 16:33:46.000000 ultrasync-0.9.6/tests/var/comnav/0.108/zstate.xml
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-03-25 17:53:14.335669 ultrasync-0.9.6/tests/var/comnav/0.108-burglar-alarm-on/
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     1983 2020-12-06 19:13:13.000000 ultrasync-0.9.6/tests/var/comnav/0.108-burglar-alarm-on/area.htm
--rw-rw-r--   0 l2g       (1000) l2g       (1000)    23026 2020-12-06 19:13:13.000000 ultrasync-0.9.6/tests/var/comnav/0.108-burglar-alarm-on/master.js
--rw-rw-r--   0 l2g       (1000) l2g       (1000)       92 2020-12-06 19:13:13.000000 ultrasync-0.9.6/tests/var/comnav/0.108-burglar-alarm-on/seq.xml
--rw-rw-r--   0 l2g       (1000) l2g       (1000)    18114 2020-12-06 19:13:13.000000 ultrasync-0.9.6/tests/var/comnav/0.108-burglar-alarm-on/status.js
--rw-rw-r--   0 l2g       (1000) l2g       (1000)      447 2020-12-06 19:13:13.000000 ultrasync-0.9.6/tests/var/comnav/0.108-burglar-alarm-on/status.xml
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     2791 2020-12-06 19:13:13.000000 ultrasync-0.9.6/tests/var/comnav/0.108-burglar-alarm-on/zones.htm
--rw-rw-r--   0 l2g       (1000) l2g       (1000)       96 2020-12-06 19:13:13.000000 ultrasync-0.9.6/tests/var/comnav/0.108-burglar-alarm-on/zstate.xml
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-03-25 17:53:14.337669 ultrasync-0.9.6/tests/var/comnav/0.108-zone-test/
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     2044 2021-01-25 19:18:33.000000 ultrasync-0.9.6/tests/var/comnav/0.108-zone-test/area.htm
--rw-rw-r--   0 l2g       (1000) l2g       (1000)       97 2021-01-25 19:18:33.000000 ultrasync-0.9.6/tests/var/comnav/0.108-zone-test/seq.w.update.xml
--rw-rw-r--   0 l2g       (1000) l2g       (1000)       97 2021-01-25 19:18:33.000000 ultrasync-0.9.6/tests/var/comnav/0.108-zone-test/seq.xml
--rw-rw-r--   0 l2g       (1000) l2g       (1000)      458 2021-01-25 19:18:33.000000 ultrasync-0.9.6/tests/var/comnav/0.108-zone-test/status.xml
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     2327 2021-01-25 19:18:33.000000 ultrasync-0.9.6/tests/var/comnav/0.108-zone-test/zones.htm
--rw-rw-r--   0 l2g       (1000) l2g       (1000)       91 2021-01-25 19:18:33.000000 ultrasync-0.9.6/tests/var/comnav/0.108-zone-test/zstate.xml
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-03-25 17:53:14.317669 ultrasync-0.9.6/tests/var/xgen/
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-03-25 17:53:14.341669 ultrasync-0.9.6/tests/var/xgen/general/
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     1862 2021-01-18 21:01:58.000000 ultrasync-0.9.6/tests/var/xgen/general/area.htm
--rw-rw-r--   0 l2g       (1000) l2g       (1000)    13088 2021-01-18 21:01:58.000000 ultrasync-0.9.6/tests/var/xgen/general/master.js
--rw-rw-r--   0 l2g       (1000) l2g       (1000)      130 2021-01-18 21:01:58.000000 ultrasync-0.9.6/tests/var/xgen/general/seq.json
--rw-rw-r--   0 l2g       (1000) l2g       (1000)      130 2021-01-18 21:01:58.000000 ultrasync-0.9.6/tests/var/xgen/general/seq.w.update.json
--rw-rw-r--   0 l2g       (1000) l2g       (1000)    18618 2021-01-18 21:01:58.000000 ultrasync-0.9.6/tests/var/xgen/general/status.js
--rw-rw-r--   0 l2g       (1000) l2g       (1000)      188 2021-01-18 21:01:58.000000 ultrasync-0.9.6/tests/var/xgen/general/status.json
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     2071 2021-01-18 21:01:58.000000 ultrasync-0.9.6/tests/var/xgen/general/zones.htm
--rw-rw-r--   0 l2g       (1000) l2g       (1000)       76 2021-01-18 21:01:58.000000 ultrasync-0.9.6/tests/var/xgen/general/zstate.json
--rw-rw-r--   0 l2g       (1000) l2g       (1000)       76 2021-01-18 21:01:58.000000 ultrasync-0.9.6/tests/var/xgen/general/zstate.w.update.json
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-03-25 17:53:14.317669 ultrasync-0.9.6/tests/var/xgen8/
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-03-25 17:53:14.343669 ultrasync-0.9.6/tests/var/xgen8/bypass/
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     2217 2022-07-01 13:18:56.000000 ultrasync-0.9.6/tests/var/xgen8/bypass/area.htm
--rw-rw-r--   0 l2g       (1000) l2g       (1000)      326 2022-07-01 13:18:56.000000 ultrasync-0.9.6/tests/var/xgen8/bypass/seq.json
--rw-rw-r--   0 l2g       (1000) l2g       (1000)       73 2022-07-01 13:18:56.000000 ultrasync-0.9.6/tests/var/xgen8/bypass/zonefunction.json
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     2054 2022-07-01 13:18:56.000000 ultrasync-0.9.6/tests/var/xgen8/bypass/zones.htm
--rw-rw-r--   0 l2g       (1000) l2g       (1000)       73 2022-07-01 13:18:56.000000 ultrasync-0.9.6/tests/var/xgen8/bypass/zstate.json
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-03-25 17:53:14.345669 ultrasync-0.9.6/tests/var/xgen8/nxg8zbo/
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     2282 2021-09-20 21:43:45.000000 ultrasync-0.9.6/tests/var/xgen8/nxg8zbo/area.htm
--rw-rw-r--   0 l2g       (1000) l2g       (1000)      321 2021-09-20 21:43:45.000000 ultrasync-0.9.6/tests/var/xgen8/nxg8zbo/seq.json
--rw-rw-r--   0 l2g       (1000) l2g       (1000)      321 2021-09-20 21:43:45.000000 ultrasync-0.9.6/tests/var/xgen8/nxg8zbo/seq.w.update.json
--rw-rw-r--   0 l2g       (1000) l2g       (1000)      563 2021-09-20 21:43:45.000000 ultrasync-0.9.6/tests/var/xgen8/nxg8zbo/status.json
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     2088 2021-09-20 21:43:45.000000 ultrasync-0.9.6/tests/var/xgen8/nxg8zbo/zones.htm
--rw-rw-r--   0 l2g       (1000) l2g       (1000)       75 2021-09-20 21:43:45.000000 ultrasync-0.9.6/tests/var/xgen8/nxg8zbo/zstate.json
--rw-rw-r--   0 l2g       (1000) l2g       (1000)       75 2021-09-20 21:43:45.000000 ultrasync-0.9.6/tests/var/xgen8/nxg8zbo/zstate.w.update.json
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-03-25 17:53:14.317669 ultrasync-0.9.6/tests/var/zerowire/
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-03-25 17:53:14.347669 ultrasync-0.9.6/tests/var/zerowire/armed/
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     1848 2020-11-22 16:33:46.000000 ultrasync-0.9.6/tests/var/zerowire/armed/area.htm
--rw-rw-r--   0 l2g       (1000) l2g       (1000)      165 2020-11-22 16:33:46.000000 ultrasync-0.9.6/tests/var/zerowire/armed/seq.json
--rw-rw-r--   0 l2g       (1000) l2g       (1000)      196 2020-11-22 16:33:46.000000 ultrasync-0.9.6/tests/var/zerowire/armed/status.json
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     2582 2020-11-22 16:33:46.000000 ultrasync-0.9.6/tests/var/zerowire/armed/zones.htm
--rw-rw-r--   0 l2g       (1000) l2g       (1000)       94 2020-11-22 16:33:46.000000 ultrasync-0.9.6/tests/var/zerowire/armed/zstate.json
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-03-25 17:53:14.348669 ultrasync-0.9.6/tests/var/zerowire/general/
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     1848 2020-11-22 16:33:46.000000 ultrasync-0.9.6/tests/var/zerowire/general/area.htm
--rw-rw-r--   0 l2g       (1000) l2g       (1000)      160 2021-01-18 21:01:58.000000 ultrasync-0.9.6/tests/var/zerowire/general/seq.json
--rw-rw-r--   0 l2g       (1000) l2g       (1000)      196 2021-01-18 21:01:58.000000 ultrasync-0.9.6/tests/var/zerowire/general/status.json
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     2574 2020-11-22 16:33:46.000000 ultrasync-0.9.6/tests/var/zerowire/general/zones.htm
--rw-rw-r--   0 l2g       (1000) l2g       (1000)       94 2020-11-22 16:33:46.000000 ultrasync-0.9.6/tests/var/zerowire/general/zstate.json
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-03-25 17:53:14.351669 ultrasync-0.9.6/ultrasync/
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     1793 2023-03-25 17:52:39.000000 ultrasync-0.9.6/ultrasync/__init__.py
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     8954 2022-07-01 13:18:56.000000 ultrasync-0.9.6/ultrasync/cli.py
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     8351 2021-09-20 21:40:13.000000 ultrasync-0.9.6/ultrasync/common.py
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     6747 2021-09-12 19:13:27.000000 ultrasync-0.9.6/ultrasync/config.py
--rw-rw-r--   0 l2g       (1000) l2g       (1000)     2282 2020-12-06 19:13:13.000000 ultrasync-0.9.6/ultrasync/logger.py
--rw-rw-r--   0 l2g       (1000) l2g       (1000)    81936 2022-07-01 13:18:56.000000 ultrasync-0.9.6/ultrasync/main.py
-drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-03-25 17:53:14.353669 ultrasync-0.9.6/ultrasync.egg-info/
--rw-r--r--   0 l2g       (1000) l2g       (1000)     7208 2023-03-25 17:53:14.000000 ultrasync-0.9.6/ultrasync.egg-info/PKG-INFO
--rw-r--r--   0 l2g       (1000) l2g       (1000)     3085 2023-03-25 17:53:14.000000 ultrasync-0.9.6/ultrasync.egg-info/SOURCES.txt
--rw-r--r--   0 l2g       (1000) l2g       (1000)        1 2023-03-25 17:53:14.000000 ultrasync-0.9.6/ultrasync.egg-info/dependency_links.txt
--rw-r--r--   0 l2g       (1000) l2g       (1000)       50 2023-03-25 17:53:14.000000 ultrasync-0.9.6/ultrasync.egg-info/entry_points.txt
--rw-r--r--   0 l2g       (1000) l2g       (1000)       15 2023-03-25 17:53:14.000000 ultrasync-0.9.6/ultrasync.egg-info/requires.txt
--rw-r--r--   0 l2g       (1000) l2g       (1000)       10 2023-03-25 17:53:14.000000 ultrasync-0.9.6/ultrasync.egg-info/top_level.txt
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-05-06 17:20:32.856993 ultrasync-0.9.7/
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)     1090 2020-11-22 16:33:46.000000 ultrasync-0.9.7/LICENSE
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)      191 2020-11-22 16:33:46.000000 ultrasync-0.9.7/MANIFEST.in
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     7208 2023-05-06 17:20:32.856993 ultrasync-0.9.7/PKG-INFO
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)     6235 2021-09-20 21:40:13.000000 ultrasync-0.9.7/README.md
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)       43 2020-11-22 16:33:46.000000 ultrasync-0.9.7/dev-requirements.txt
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)       15 2020-11-22 16:33:46.000000 ultrasync-0.9.7/requirements.txt
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)      335 2023-05-06 17:20:32.857993 ultrasync-0.9.7/setup.cfg
+-rwxr-xr-x   0 l2g       (1000) l2g       (1000)     3031 2023-05-06 17:19:41.000000 ultrasync-0.9.7/setup.py
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-05-06 17:20:32.830993 ultrasync-0.9.7/tests/
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)     5121 2020-11-22 16:33:46.000000 ultrasync-0.9.7/tests/test_cli.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     7424 2023-03-25 17:53:36.000000 ultrasync-0.9.7/tests/test_comnav_0_106.py
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)     6360 2021-01-25 19:18:33.000000 ultrasync-0.9.7/tests/test_comnav_0_108-zone-check.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     6635 2023-03-25 17:53:36.000000 ultrasync-0.9.7/tests/test_comnav_0_108.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     4922 2023-03-25 17:53:36.000000 ultrasync-0.9.7/tests/test_comnav_0_108_burglar_alarm_on.py
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)     3873 2020-11-22 16:33:46.000000 ultrasync-0.9.7/tests/test_config.py
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)     4828 2022-07-01 13:18:56.000000 ultrasync-0.9.7/tests/test_xgen8_bypass.py
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)     7289 2021-09-20 21:40:13.000000 ultrasync-0.9.7/tests/test_xgen8_nxg8zbo.py
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)     7984 2021-09-19 13:53:23.000000 ultrasync-0.9.7/tests/test_xgen_general.py
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)     4590 2021-01-25 19:18:33.000000 ultrasync-0.9.7/tests/test_zerowire_armed.py
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)     6543 2021-01-25 19:18:33.000000 ultrasync-0.9.7/tests/test_zerowire_general.py
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-05-06 17:20:32.823993 ultrasync-0.9.7/tests/var/
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-05-06 17:20:32.823993 ultrasync-0.9.7/tests/var/comnav/
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-05-06 17:20:32.833993 ultrasync-0.9.7/tests/var/comnav/0.106/
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)     1892 2020-11-22 16:33:46.000000 ultrasync-0.9.7/tests/var/comnav/0.106/area.htm
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)    36123 2020-11-22 16:33:46.000000 ultrasync-0.9.7/tests/var/comnav/0.106/master.js
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)       96 2020-11-22 16:33:46.000000 ultrasync-0.9.7/tests/var/comnav/0.106/seq.w.update.xml
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)       96 2020-11-22 16:33:46.000000 ultrasync-0.9.7/tests/var/comnav/0.106/seq.xml
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)    21526 2020-11-22 16:33:46.000000 ultrasync-0.9.7/tests/var/comnav/0.106/status.js
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)      436 2020-11-22 16:33:46.000000 ultrasync-0.9.7/tests/var/comnav/0.106/status.xml
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)     1832 2020-11-22 16:33:46.000000 ultrasync-0.9.7/tests/var/comnav/0.106/zones.htm
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)       82 2020-11-22 16:33:46.000000 ultrasync-0.9.7/tests/var/comnav/0.106/zstate.bank0.w.update.xml
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)       81 2020-11-22 16:33:46.000000 ultrasync-0.9.7/tests/var/comnav/0.106/zstate.bank4.w.update.xml
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)       82 2020-11-22 16:33:46.000000 ultrasync-0.9.7/tests/var/comnav/0.106/zstate.xml
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-05-06 17:20:32.837993 ultrasync-0.9.7/tests/var/comnav/0.108/
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)     1971 2020-11-22 16:33:46.000000 ultrasync-0.9.7/tests/var/comnav/0.108/area.htm
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)    23023 2020-11-22 16:33:46.000000 ultrasync-0.9.7/tests/var/comnav/0.108/master.js
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)       92 2020-11-22 16:33:46.000000 ultrasync-0.9.7/tests/var/comnav/0.108/seq.w.update.xml
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)       92 2020-11-22 16:33:46.000000 ultrasync-0.9.7/tests/var/comnav/0.108/seq.xml
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)    18114 2020-11-22 16:33:46.000000 ultrasync-0.9.7/tests/var/comnav/0.108/status.js
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)      436 2020-11-22 16:33:46.000000 ultrasync-0.9.7/tests/var/comnav/0.108/status.xml
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)     2793 2020-11-22 16:33:46.000000 ultrasync-0.9.7/tests/var/comnav/0.108/zones.htm
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)       98 2020-11-22 16:33:46.000000 ultrasync-0.9.7/tests/var/comnav/0.108/zstate.xml
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-05-06 17:20:32.839993 ultrasync-0.9.7/tests/var/comnav/0.108-burglar-alarm-on/
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)     1983 2020-12-06 19:13:13.000000 ultrasync-0.9.7/tests/var/comnav/0.108-burglar-alarm-on/area.htm
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)    23026 2020-12-06 19:13:13.000000 ultrasync-0.9.7/tests/var/comnav/0.108-burglar-alarm-on/master.js
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)       92 2020-12-06 19:13:13.000000 ultrasync-0.9.7/tests/var/comnav/0.108-burglar-alarm-on/seq.xml
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)    18114 2020-12-06 19:13:13.000000 ultrasync-0.9.7/tests/var/comnav/0.108-burglar-alarm-on/status.js
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)      447 2020-12-06 19:13:13.000000 ultrasync-0.9.7/tests/var/comnav/0.108-burglar-alarm-on/status.xml
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)     2791 2020-12-06 19:13:13.000000 ultrasync-0.9.7/tests/var/comnav/0.108-burglar-alarm-on/zones.htm
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)       96 2020-12-06 19:13:13.000000 ultrasync-0.9.7/tests/var/comnav/0.108-burglar-alarm-on/zstate.xml
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-05-06 17:20:32.841993 ultrasync-0.9.7/tests/var/comnav/0.108-zone-test/
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)     2044 2021-01-25 19:18:33.000000 ultrasync-0.9.7/tests/var/comnav/0.108-zone-test/area.htm
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)       97 2021-01-25 19:18:33.000000 ultrasync-0.9.7/tests/var/comnav/0.108-zone-test/seq.w.update.xml
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)       97 2021-01-25 19:18:33.000000 ultrasync-0.9.7/tests/var/comnav/0.108-zone-test/seq.xml
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)      458 2021-01-25 19:18:33.000000 ultrasync-0.9.7/tests/var/comnav/0.108-zone-test/status.xml
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)     2327 2021-01-25 19:18:33.000000 ultrasync-0.9.7/tests/var/comnav/0.108-zone-test/zones.htm
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)       91 2021-01-25 19:18:33.000000 ultrasync-0.9.7/tests/var/comnav/0.108-zone-test/zstate.xml
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-05-06 17:20:32.823993 ultrasync-0.9.7/tests/var/xgen/
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-05-06 17:20:32.845993 ultrasync-0.9.7/tests/var/xgen/general/
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)     1862 2021-01-18 21:01:58.000000 ultrasync-0.9.7/tests/var/xgen/general/area.htm
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)    13088 2021-01-18 21:01:58.000000 ultrasync-0.9.7/tests/var/xgen/general/master.js
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)      130 2021-01-18 21:01:58.000000 ultrasync-0.9.7/tests/var/xgen/general/seq.json
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)      130 2021-01-18 21:01:58.000000 ultrasync-0.9.7/tests/var/xgen/general/seq.w.update.json
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)    18618 2021-01-18 21:01:58.000000 ultrasync-0.9.7/tests/var/xgen/general/status.js
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)      188 2021-01-18 21:01:58.000000 ultrasync-0.9.7/tests/var/xgen/general/status.json
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)     2071 2021-01-18 21:01:58.000000 ultrasync-0.9.7/tests/var/xgen/general/zones.htm
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)       76 2021-01-18 21:01:58.000000 ultrasync-0.9.7/tests/var/xgen/general/zstate.json
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)       76 2021-01-18 21:01:58.000000 ultrasync-0.9.7/tests/var/xgen/general/zstate.w.update.json
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-05-06 17:20:32.823993 ultrasync-0.9.7/tests/var/xgen8/
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-05-06 17:20:32.847993 ultrasync-0.9.7/tests/var/xgen8/bypass/
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)     2217 2022-07-01 13:18:56.000000 ultrasync-0.9.7/tests/var/xgen8/bypass/area.htm
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)      326 2022-07-01 13:18:56.000000 ultrasync-0.9.7/tests/var/xgen8/bypass/seq.json
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)       73 2022-07-01 13:18:56.000000 ultrasync-0.9.7/tests/var/xgen8/bypass/zonefunction.json
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)     2054 2022-07-01 13:18:56.000000 ultrasync-0.9.7/tests/var/xgen8/bypass/zones.htm
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)       73 2022-07-01 13:18:56.000000 ultrasync-0.9.7/tests/var/xgen8/bypass/zstate.json
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-05-06 17:20:32.849993 ultrasync-0.9.7/tests/var/xgen8/nxg8zbo/
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)     2282 2021-09-20 21:43:45.000000 ultrasync-0.9.7/tests/var/xgen8/nxg8zbo/area.htm
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)      321 2021-09-20 21:43:45.000000 ultrasync-0.9.7/tests/var/xgen8/nxg8zbo/seq.json
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)      321 2021-09-20 21:43:45.000000 ultrasync-0.9.7/tests/var/xgen8/nxg8zbo/seq.w.update.json
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)      563 2021-09-20 21:43:45.000000 ultrasync-0.9.7/tests/var/xgen8/nxg8zbo/status.json
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)     2088 2021-09-20 21:43:45.000000 ultrasync-0.9.7/tests/var/xgen8/nxg8zbo/zones.htm
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)       75 2021-09-20 21:43:45.000000 ultrasync-0.9.7/tests/var/xgen8/nxg8zbo/zstate.json
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)       75 2021-09-20 21:43:45.000000 ultrasync-0.9.7/tests/var/xgen8/nxg8zbo/zstate.w.update.json
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-05-06 17:20:32.824993 ultrasync-0.9.7/tests/var/zerowire/
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-05-06 17:20:32.851993 ultrasync-0.9.7/tests/var/zerowire/armed/
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)     1848 2020-11-22 16:33:46.000000 ultrasync-0.9.7/tests/var/zerowire/armed/area.htm
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)      165 2020-11-22 16:33:46.000000 ultrasync-0.9.7/tests/var/zerowire/armed/seq.json
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)      196 2020-11-22 16:33:46.000000 ultrasync-0.9.7/tests/var/zerowire/armed/status.json
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)     2582 2020-11-22 16:33:46.000000 ultrasync-0.9.7/tests/var/zerowire/armed/zones.htm
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)       94 2020-11-22 16:33:46.000000 ultrasync-0.9.7/tests/var/zerowire/armed/zstate.json
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-05-06 17:20:32.852993 ultrasync-0.9.7/tests/var/zerowire/general/
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)     1848 2020-11-22 16:33:46.000000 ultrasync-0.9.7/tests/var/zerowire/general/area.htm
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)      160 2021-01-18 21:01:58.000000 ultrasync-0.9.7/tests/var/zerowire/general/seq.json
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)      196 2021-01-18 21:01:58.000000 ultrasync-0.9.7/tests/var/zerowire/general/status.json
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)     2574 2020-11-22 16:33:46.000000 ultrasync-0.9.7/tests/var/zerowire/general/zones.htm
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)       94 2020-11-22 16:33:46.000000 ultrasync-0.9.7/tests/var/zerowire/general/zstate.json
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-05-06 17:20:32.855993 ultrasync-0.9.7/ultrasync/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     1793 2023-05-06 17:19:51.000000 ultrasync-0.9.7/ultrasync/__init__.py
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)     8954 2022-07-01 13:18:56.000000 ultrasync-0.9.7/ultrasync/cli.py
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)     8351 2021-09-20 21:40:13.000000 ultrasync-0.9.7/ultrasync/common.py
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)     6747 2021-09-12 19:13:27.000000 ultrasync-0.9.7/ultrasync/config.py
+-rw-rw-r--   0 l2g       (1000) l2g       (1000)     2282 2020-12-06 19:13:13.000000 ultrasync-0.9.7/ultrasync/logger.py
+-rw-r--r--   0 l2g       (1000) l2g       (1000)    83078 2023-05-06 17:19:29.000000 ultrasync-0.9.7/ultrasync/main.py
+drwxr-xr-x   0 l2g       (1000) l2g       (1000)        0 2023-05-06 17:20:32.856993 ultrasync-0.9.7/ultrasync.egg-info/
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     7208 2023-05-06 17:20:32.000000 ultrasync-0.9.7/ultrasync.egg-info/PKG-INFO
+-rw-r--r--   0 l2g       (1000) l2g       (1000)     3085 2023-05-06 17:20:32.000000 ultrasync-0.9.7/ultrasync.egg-info/SOURCES.txt
+-rw-r--r--   0 l2g       (1000) l2g       (1000)        1 2023-05-06 17:20:32.000000 ultrasync-0.9.7/ultrasync.egg-info/dependency_links.txt
+-rw-r--r--   0 l2g       (1000) l2g       (1000)       50 2023-05-06 17:20:32.000000 ultrasync-0.9.7/ultrasync.egg-info/entry_points.txt
+-rw-r--r--   0 l2g       (1000) l2g       (1000)       15 2023-05-06 17:20:32.000000 ultrasync-0.9.7/ultrasync.egg-info/requires.txt
+-rw-r--r--   0 l2g       (1000) l2g       (1000)       10 2023-05-06 17:20:32.000000 ultrasync-0.9.7/ultrasync.egg-info/top_level.txt
```

### Comparing `ultrasync-0.9.6/LICENSE` & `ultrasync-0.9.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.6/PKG-INFO` & `ultrasync-0.9.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ultrasync
-Version: 0.9.6
+Version: 0.9.7
 Summary: Wrapper to XGen/XGen8/Hills/Interlogix NX-595E/UltraSync ZeroWire
 Home-page: https://github.com/caronc/ultrasync
 Author: Chris Caron
 Author-email: lead2gold@gmail.com
 License: MIT
 Keywords: XGen XGen8 Hills ComNav Interlogix UltraSync NX-595E ZeroWire Security Panel
 Platform: UNKNOWN
```

### Comparing `ultrasync-0.9.6/README.md` & `ultrasync-0.9.7/README.md`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.6/setup.py` & `ultrasync-0.9.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
 else:
     # Load our CLI
     console_scripts = ['ultrasync = ultrasync.cli:main']
 
 setup(
     name='ultrasync',
-    version='0.9.6',
+    version='0.9.7',
     description='Wrapper to XGen/XGen8/Hills/Interlogix NX-595E/UltraSync '
                 'ZeroWire',
     license='MIT',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/caronc/ultrasync',
     keywords='XGen XGen8 Hills ComNav Interlogix UltraSync NX-595E ZeroWire '
```

### Comparing `ultrasync-0.9.6/tests/test_cli.py` & `ultrasync-0.9.7/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.6/tests/test_comnav_0_106.py` & `ultrasync-0.9.7/tests/test_comnav_0_106.py`

 * *Files 1% similar despite different names*

```diff
@@ -132,15 +132,15 @@
     for entry in zone_map:
         assert entry['bank'] in uobj.zones
         assert uobj.zones[entry['bank']]['bank'] == entry['bank']
         assert uobj.zones[entry['bank']]['name'] == entry['name']
         assert uobj.zones[entry['bank']]['sequence'] == 1
         assert uobj.zones[entry['bank']]['status'] == \
             entry.get('status', 'Ready')
-        assert uobj.zones[entry['bank']]['can_bypass'] is None
+        assert uobj.zones[entry['bank']]['can_bypass'] is True
 
     # A call to login.cgi (which fetches area.html) and then zones.htm
     assert mock_post.call_count == 2
     assert mock_post.call_args_list[0][0][0] == \
         'http://zerowire/login.cgi'
     assert mock_post.call_args_list[1][0][0] == \
         'http://zerowire/user/zones.htm'
```

### Comparing `ultrasync-0.9.6/tests/test_comnav_0_108-zone-check.py` & `ultrasync-0.9.7/tests/test_comnav_0_108-zone-check.py`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.6/tests/test_comnav_0_108.py` & `ultrasync-0.9.7/tests/test_comnav_0_108.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,15 @@
     for entry in zone_map:
         assert entry['bank'] in uobj.zones
         assert uobj.zones[entry['bank']]['bank'] == entry['bank']
         assert uobj.zones[entry['bank']]['name'] == entry['name']
         assert uobj.zones[entry['bank']]['sequence'] == 1
         assert uobj.zones[entry['bank']]['status'] == \
             entry.get('status', 'Ready')
-        assert uobj.zones[entry['bank']]['can_bypass'] is None
+        assert uobj.zones[entry['bank']]['can_bypass'] is True
 
     # A call to login.cgi (which fetches area.html) and then zones.htm
     assert mock_post.call_count == 2
     assert mock_post.call_args_list[0][0][0] == \
         'http://zerowire/login.cgi'
     assert mock_post.call_args_list[1][0][0] == \
         'http://zerowire/user/zones.htm'
```

### Comparing `ultrasync-0.9.6/tests/test_comnav_0_108_burglar_alarm_on.py` & `ultrasync-0.9.7/tests/test_comnav_0_108_burglar_alarm_on.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,15 @@
     for entry in zone_map:
         assert entry['bank'] in uobj.zones
         assert uobj.zones[entry['bank']]['bank'] == entry['bank']
         assert uobj.zones[entry['bank']]['name'] == entry['name']
         assert uobj.zones[entry['bank']]['sequence'] == 1
         assert uobj.zones[entry['bank']]['status'] == \
             entry.get('status', 'Ready')
-        assert uobj.zones[entry['bank']]['can_bypass'] is None
+        assert uobj.zones[entry['bank']]['can_bypass'] is True
 
     # A call to login.cgi (which fetches area.html) and then zones.htm
     assert mock_post.call_count == 2
     assert mock_post.call_args_list[0][0][0] == \
         'http://zerowire/login.cgi'
     assert mock_post.call_args_list[1][0][0] == \
         'http://zerowire/user/zones.htm'
```

### Comparing `ultrasync-0.9.6/tests/test_config.py` & `ultrasync-0.9.7/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.6/tests/test_xgen8_bypass.py` & `ultrasync-0.9.7/tests/test_xgen8_bypass.py`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.6/tests/test_xgen8_nxg8zbo.py` & `ultrasync-0.9.7/tests/test_xgen8_nxg8zbo.py`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.6/tests/test_xgen_general.py` & `ultrasync-0.9.7/tests/test_xgen_general.py`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.6/tests/test_zerowire_armed.py` & `ultrasync-0.9.7/tests/test_zerowire_armed.py`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.6/tests/test_zerowire_general.py` & `ultrasync-0.9.7/tests/test_zerowire_general.py`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.6/tests/var/comnav/0.106/area.htm` & `ultrasync-0.9.7/tests/var/comnav/0.106/area.htm`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.6/tests/var/comnav/0.106/master.js` & `ultrasync-0.9.7/tests/var/comnav/0.106/master.js`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.6/tests/var/comnav/0.106/status.js` & `ultrasync-0.9.7/tests/var/comnav/0.106/status.js`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.6/tests/var/comnav/0.106/zones.htm` & `ultrasync-0.9.7/tests/var/comnav/0.106/zones.htm`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.6/tests/var/comnav/0.108/area.htm` & `ultrasync-0.9.7/tests/var/comnav/0.108/area.htm`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.6/tests/var/comnav/0.108/master.js` & `ultrasync-0.9.7/tests/var/comnav/0.108/master.js`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.6/tests/var/comnav/0.108/status.js` & `ultrasync-0.9.7/tests/var/comnav/0.108/status.js`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.6/tests/var/comnav/0.108/zones.htm` & `ultrasync-0.9.7/tests/var/comnav/0.108/zones.htm`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.6/tests/var/comnav/0.108-burglar-alarm-on/area.htm` & `ultrasync-0.9.7/tests/var/comnav/0.108-burglar-alarm-on/area.htm`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.6/tests/var/comnav/0.108-burglar-alarm-on/master.js` & `ultrasync-0.9.7/tests/var/comnav/0.108-burglar-alarm-on/master.js`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.6/tests/var/comnav/0.108-burglar-alarm-on/status.js` & `ultrasync-0.9.7/tests/var/comnav/0.108-burglar-alarm-on/status.js`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.6/tests/var/comnav/0.108-burglar-alarm-on/zones.htm` & `ultrasync-0.9.7/tests/var/comnav/0.108-burglar-alarm-on/zones.htm`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.6/tests/var/comnav/0.108-zone-test/area.htm` & `ultrasync-0.9.7/tests/var/comnav/0.108-zone-test/area.htm`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.6/tests/var/comnav/0.108-zone-test/zones.htm` & `ultrasync-0.9.7/tests/var/comnav/0.108-zone-test/zones.htm`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.6/tests/var/xgen/general/area.htm` & `ultrasync-0.9.7/tests/var/xgen/general/area.htm`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.6/tests/var/xgen/general/master.js` & `ultrasync-0.9.7/tests/var/xgen/general/master.js`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.6/tests/var/xgen/general/status.js` & `ultrasync-0.9.7/tests/var/xgen/general/status.js`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.6/tests/var/xgen/general/zones.htm` & `ultrasync-0.9.7/tests/var/xgen/general/zones.htm`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.6/tests/var/xgen8/bypass/area.htm` & `ultrasync-0.9.7/tests/var/xgen8/bypass/area.htm`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.6/tests/var/xgen8/bypass/zones.htm` & `ultrasync-0.9.7/tests/var/xgen8/bypass/zones.htm`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.6/tests/var/xgen8/nxg8zbo/area.htm` & `ultrasync-0.9.7/tests/var/xgen8/nxg8zbo/area.htm`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.6/tests/var/xgen8/nxg8zbo/status.json` & `ultrasync-0.9.7/tests/var/xgen8/nxg8zbo/status.json`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.6/tests/var/xgen8/nxg8zbo/zones.htm` & `ultrasync-0.9.7/tests/var/xgen8/nxg8zbo/zones.htm`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.6/tests/var/zerowire/armed/area.htm` & `ultrasync-0.9.7/tests/var/zerowire/armed/area.htm`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.6/tests/var/zerowire/armed/zones.htm` & `ultrasync-0.9.7/tests/var/zerowire/armed/zones.htm`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.6/tests/var/zerowire/general/area.htm` & `ultrasync-0.9.7/tests/var/zerowire/general/area.htm`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.6/tests/var/zerowire/general/zones.htm` & `ultrasync-0.9.7/tests/var/zerowire/general/zones.htm`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.6/ultrasync/__init__.py` & `ultrasync-0.9.7/ultrasync/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT.IN NO EVENT SHALL THE
 # AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 # OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
 # THE SOFTWARE.
 
 __title__ = 'ultrasync'
-__version__ = '0.9.6'
+__version__ = '0.9.7'
 __author__ = 'Chris Caron'
 __license__ = 'MIT'
 __copywrite__ = 'Copyright (C) 2023 Chris Caron <lead2gold@gmail.com>'
 __email__ = 'lead2gold@gmail.com'
 __status__ = 'Production'
 
 from .main import UltraSync
```

### Comparing `ultrasync-0.9.6/ultrasync/cli.py` & `ultrasync-0.9.7/ultrasync/cli.py`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.6/ultrasync/common.py` & `ultrasync-0.9.7/ultrasync/common.py`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.6/ultrasync/config.py` & `ultrasync-0.9.7/ultrasync/config.py`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.6/ultrasync/logger.py` & `ultrasync-0.9.7/ultrasync/logger.py`

 * *Files identical despite different names*

### Comparing `ultrasync-0.9.6/ultrasync/main.py` & `ultrasync-0.9.7/ultrasync/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -589,22 +589,49 @@
         has_error = False
 
         # Start our payload off with our session identifier
         payload = {
             'sess': self.session_id,
         }
 
-        if self.vendor in (NX595EVendor.XGEN8):
-            payload.update({
+        if self.vendor in (NX595EVendor.ZEROWIRE, NX595EVendor.XGEN8):
+                payload.update({
                 'cmd': 5,
                 'opt': int(state),
                 'zone': zone - 1,
             })
-
-        else:  # self.vendor is NX595EVendor.{COMNAV, ZEROWIRE, XGEN}
+            
+                # Send our response
+                response = self.__get(
+                    '/user/zonefunction.cgi', payload=payload)
+
+        elif self.vendor in (NX595EVendor.COMNAV):
+            # Call comnav_process_zones to update can_bypass attribute
+            self.comnav_process_zones
+
+            # Get the current can_bypass state of the zone
+            can_bypass = self.zones[zone - 1]['can_bypass']
+
+            # If the current can_bypass state does not match the desired bypass state,
+            # toggle the bypass state
+            if can_bypass == state:
+                # Start our payload off with our session identifier
+                payload = {
+                    'sess': self.session_id,
+                    'comm': 82,
+                    'data0': zone - 1,
+                }
+            else: 
+                payload = {}
+
+            # Send our response
+            response = self.__get(
+                '/user/zonefunction.cgi', payload=payload)
+ 
+        else:   # self.vendor is NX595EVendor.{ZEROWIRE, XGEN}
 
             logger.error(
                 'Bypass not implemented for vendor {}'.format(self.vendor))
             return False
 
         # Send our response
         response = self.__get(
@@ -1468,14 +1495,17 @@
             vbank = [bool(int(self._zbank[s][idx]) & mask)
                      for s in range(0, len(self._zbank))]
 
             # Update our zone virtual bank
             self._zvbank[bank] = ''.join(
                 [str(1 if b else 0) for b in vbank])
 
+            # Track whether or not element is part of things
+            can_bypass = not vbank[ZoneBank.UNKWN_03]
+
             if vbank[ZoneBank.UNKWN_05]:
                 # red
                 priority = 1
 
             elif vbank[ZoneBank.UNKWN_01] or vbank[ZoneBank.UNKWN_02] or \
                     vbank[ZoneBank.UNKWN_06] or vbank[ZoneBank.UNKWN_07]:
 
@@ -1508,15 +1538,15 @@
                 zone.get('sequence', 0)) \
                 if zone.get('bank_state') != self._zvbank[bank] \
                 else zone.get('sequence', 0)
 
             zone.update({
                 'priority': priority,
                 'status': status,
-                'can_bypass': None,
+                'can_bypass': can_bypass,
                 'bank_state': self._zvbank[bank],
                 'sequence': sequence,
             })
 
         return True
 
     def _zones(self):
```

### Comparing `ultrasync-0.9.6/ultrasync.egg-info/PKG-INFO` & `ultrasync-0.9.7/ultrasync.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ultrasync
-Version: 0.9.6
+Version: 0.9.7
 Summary: Wrapper to XGen/XGen8/Hills/Interlogix NX-595E/UltraSync ZeroWire
 Home-page: https://github.com/caronc/ultrasync
 Author: Chris Caron
 Author-email: lead2gold@gmail.com
 License: MIT
 Keywords: XGen XGen8 Hills ComNav Interlogix UltraSync NX-595E ZeroWire Security Panel
 Platform: UNKNOWN
```

### Comparing `ultrasync-0.9.6/ultrasync.egg-info/SOURCES.txt` & `ultrasync-0.9.7/ultrasync.egg-info/SOURCES.txt`

 * *Files identical despite different names*

