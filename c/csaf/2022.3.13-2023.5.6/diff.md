# Comparing `tmp/csaf-2022.3.13.tar.gz` & `tmp/csaf-2023.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csaf-2022.3.13.tar", last modified: Sun Mar 13 20:18:03 2022, max compression
+gzip compressed data, was "csaf-2023.5.6.tar", last modified: Sat May  6 14:40:24 2023, max compression
```

## Comparing `csaf-2022.3.13.tar` & `csaf-2023.5.6.tar`

### file list

```diff
@@ -1,67 +1,64 @@
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2022-03-13 20:18:03.615086 csaf-2022.3.13/
--rw-r--r--   0 ruth       (501) staff       (20)     1075 2022-03-13 12:11:14.000000 csaf-2022.3.13/LICENSE
--rw-r--r--   0 ruth       (501) staff       (20)        1 2021-05-01 18:01:04.000000 csaf-2022.3.13/MANIFEST.in
--rw-r--r--   0 ruth       (501) staff       (20)     2299 2022-03-13 20:18:03.615192 csaf-2022.3.13/PKG-INFO
--rw-r--r--   0 ruth       (501) staff       (20)     1195 2022-03-13 16:41:38.000000 csaf-2022.3.13/README.md
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2022-03-13 20:18:03.581128 csaf-2022.3.13/csaf/
--rw-r--r--   0 ruth       (501) staff       (20)     1985 2022-03-13 20:17:16.000000 csaf-2022.3.13/csaf/__init__.py
--rw-r--r--   0 ruth       (501) staff       (20)      246 2022-03-13 14:31:06.000000 csaf-2022.3.13/csaf/__main__.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:28:57.000000 csaf-2022.3.13/csaf/category.py
--rw-r--r--   0 ruth       (501) staff       (20)     4192 2022-03-13 19:21:31.000000 csaf-2022.3.13/csaf/cli.py
--rw-r--r--   0 ruth       (501) staff       (20)      639 2022-03-13 19:18:56.000000 csaf-2022.3.13/csaf/config.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:29:02.000000 csaf-2022.3.13/csaf/cpe.py
--rw-r--r--   0 ruth       (501) staff       (20)    16570 2022-03-13 19:46:29.000000 csaf-2022.3.13/csaf/csaf.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:29:06.000000 csaf-2022.3.13/csaf/cve.py
--rw-r--r--   0 ruth       (501) staff       (20)    10903 2022-03-13 19:26:24.000000 csaf-2022.3.13/csaf/cvss.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:29:10.000000 csaf-2022.3.13/csaf/cwe.py
--rw-r--r--   0 ruth       (501) staff       (20)    12337 2021-12-31 17:31:07.000000 csaf-2022.3.13/csaf/definitions.py
--rw-r--r--   0 ruth       (501) staff       (20)    14907 2022-03-13 16:02:41.000000 csaf-2022.3.13/csaf/document.py
--rw-r--r--   0 ruth       (501) staff       (20)     1284 2022-03-13 20:11:44.000000 csaf-2022.3.13/csaf/env.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:28:45.000000 csaf-2022.3.13/csaf/hash.py
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2022-03-13 20:18:03.591574 csaf-2022.3.13/csaf/mandatory/
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-02-14 21:10:09.000000 csaf-2022.3.13/csaf/mandatory/__init__.py
--rw-r--r--   0 ruth       (501) staff       (20)     1325 2021-12-16 11:48:56.000000 csaf-2022.3.13/csaf/mandatory/acyclic_product_ids.py
--rw-r--r--   0 ruth       (501) staff       (20)     2023 2021-12-16 11:48:42.000000 csaf-2022.3.13/csaf/mandatory/consistent_product_status.py
--rw-r--r--   0 ruth       (501) staff       (20)     1435 2022-02-13 17:11:58.000000 csaf-2022.3.13/csaf/mandatory/defined_group_ids.py
--rw-r--r--   0 ruth       (501) staff       (20)     2548 2022-02-13 17:04:26.000000 csaf-2022.3.13/csaf/mandatory/defined_product_ids.py
--rw-r--r--   0 ruth       (501) staff       (20)     5204 2022-03-13 19:26:24.000000 csaf-2022.3.13/csaf/mandatory/rules.py
--rw-r--r--   0 ruth       (501) staff       (20)      981 2022-02-13 16:48:33.000000 csaf-2022.3.13/csaf/mandatory/translator_and_source_lang.py
--rw-r--r--   0 ruth       (501) staff       (20)     1267 2022-02-13 20:44:51.000000 csaf-2022.3.13/csaf/mandatory/unique_group_ids.py
--rw-r--r--   0 ruth       (501) staff       (20)     1192 2022-02-13 20:40:08.000000 csaf-2022.3.13/csaf/mandatory/unique_product_ids.py
--rw-r--r--   0 ruth       (501) staff       (20)     2390 2022-02-13 16:48:33.000000 csaf-2022.3.13/csaf/mandatory/valid_category_name.py
--rw-r--r--   0 ruth       (501) staff       (20)    16398 2022-03-13 19:26:24.000000 csaf-2022.3.13/csaf/product.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:29:21.000000 csaf-2022.3.13/csaf/purl.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:28:33.000000 csaf-2022.3.13/csaf/terminal.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:28:41.000000 csaf-2022.3.13/csaf/tlp.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:28:29.000000 csaf-2022.3.13/csaf/version.py
--rw-r--r--   0 ruth       (501) staff       (20)     3354 2022-03-13 16:02:22.000000 csaf-2022.3.13/csaf/vuln_types.py
--rw-r--r--   0 ruth       (501) staff       (20)    13398 2022-03-13 19:26:24.000000 csaf-2022.3.13/csaf/vulnerability.py
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2022-03-13 20:18:03.585621 csaf-2022.3.13/csaf.egg-info/
--rw-r--r--   0 ruth       (501) staff       (20)     2299 2022-03-13 20:18:03.000000 csaf-2022.3.13/csaf.egg-info/PKG-INFO
--rw-r--r--   0 ruth       (501) staff       (20)     1274 2022-03-13 20:18:03.000000 csaf-2022.3.13/csaf.egg-info/SOURCES.txt
--rw-r--r--   0 ruth       (501) staff       (20)        1 2022-03-13 20:18:03.000000 csaf-2022.3.13/csaf.egg-info/dependency_links.txt
--rw-r--r--   0 ruth       (501) staff       (20)       38 2022-03-13 20:18:03.000000 csaf-2022.3.13/csaf.egg-info/entry_points.txt
--rw-r--r--   0 ruth       (501) staff       (20)      145 2022-03-13 20:18:03.000000 csaf-2022.3.13/csaf.egg-info/requires.txt
--rw-r--r--   0 ruth       (501) staff       (20)       11 2022-03-13 20:18:03.000000 csaf-2022.3.13/csaf.egg-info/top_level.txt
--rw-r--r--   0 ruth       (501) staff       (20)      433 2022-03-13 20:14:55.000000 csaf-2022.3.13/pyproject.toml
--rw-r--r--   0 ruth       (501) staff       (20)     1944 2022-03-13 20:18:03.616699 csaf-2022.3.13/setup.cfg
--rw-r--r--   0 ruth       (501) staff       (20)       38 2022-02-26 15:38:11.000000 csaf-2022.3.13/setup.py
-drwxr-xr-x   0 ruth       (501) staff       (20)        0 2022-03-13 20:18:03.614982 csaf-2022.3.13/tests/
--rw-r--r--   0 ruth       (501) staff       (20)      130 2022-03-13 13:37:12.000000 csaf-2022.3.13/tests/__init__.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:34:16.000000 csaf-2022.3.13/tests/context.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:34:24.000000 csaf-2022.3.13/tests/test_category.py
--rw-r--r--   0 ruth       (501) staff       (20)      659 2022-03-13 19:31:15.000000 csaf-2022.3.13/tests/test_cli.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:34:47.000000 csaf-2022.3.13/tests/test_config.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:34:50.000000 csaf-2022.3.13/tests/test_cpe.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:34:53.000000 csaf-2022.3.13/tests/test_csaf.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:35:20.000000 csaf-2022.3.13/tests/test_cve.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:35:23.000000 csaf-2022.3.13/tests/test_cvss.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:35:26.000000 csaf-2022.3.13/tests/test_cwe.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:35:29.000000 csaf-2022.3.13/tests/test_document.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:33:14.000000 csaf-2022.3.13/tests/test_env.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:35:43.000000 csaf-2022.3.13/tests/test_product.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:35:46.000000 csaf-2022.3.13/tests/test_purl.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:35:49.000000 csaf-2022.3.13/tests/test_terminal.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:35:52.000000 csaf-2022.3.13/tests/test_tlp.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:35:55.000000 csaf-2022.3.13/tests/test_version.py
--rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:35:59.000000 csaf-2022.3.13/tests/test_vulnerability.py
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-05-06 14:40:24.128668 csaf-2023.5.6/
+-rw-r--r--   0 ruth       (501) staff       (20)     1069 2023-01-01 14:50:10.000000 csaf-2023.5.6/LICENSE
+-rw-r--r--   0 ruth       (501) staff       (20)       34 2021-05-12 16:52:51.000000 csaf-2023.5.6/MANIFEST.in
+-rw-r--r--   0 ruth       (501) staff       (20)     3732 2023-05-06 14:40:24.128510 csaf-2023.5.6/PKG-INFO
+-rw-r--r--   0 ruth       (501) staff       (20)     2576 2023-05-06 13:23:15.000000 csaf-2023.5.6/README.md
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-05-06 14:40:24.109374 csaf-2023.5.6/csaf/
+-rw-r--r--   0 ruth       (501) staff       (20)     1984 2023-05-06 14:37:47.000000 csaf-2023.5.6/csaf/__init__.py
+-rw-r--r--   0 ruth       (501) staff       (20)      246 2022-03-13 14:31:06.000000 csaf-2023.5.6/csaf/__main__.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:28:57.000000 csaf-2023.5.6/csaf/category.py
+-rw-r--r--   0 ruth       (501) staff       (20)     4112 2023-01-02 18:40:21.000000 csaf-2023.5.6/csaf/cli.py
+-rw-r--r--   0 ruth       (501) staff       (20)      647 2022-12-21 15:07:30.000000 csaf-2023.5.6/csaf/config.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:29:02.000000 csaf-2023.5.6/csaf/cpe.py
+-rw-r--r--   0 ruth       (501) staff       (20)    16866 2022-12-21 15:35:09.000000 csaf-2023.5.6/csaf/csaf.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:29:06.000000 csaf-2023.5.6/csaf/cve.py
+-rw-r--r--   0 ruth       (501) staff       (20)    11239 2023-05-06 14:07:29.000000 csaf-2023.5.6/csaf/cvss.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:29:10.000000 csaf-2023.5.6/csaf/cwe.py
+-rw-r--r--   0 ruth       (501) staff       (20)    12425 2023-05-06 13:11:03.000000 csaf-2023.5.6/csaf/definitions.py
+-rw-r--r--   0 ruth       (501) staff       (20)    14924 2022-07-31 13:30:33.000000 csaf-2023.5.6/csaf/document.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1284 2022-03-13 20:11:44.000000 csaf-2023.5.6/csaf/env.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:28:45.000000 csaf-2023.5.6/csaf/hash.py
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-05-06 14:40:24.118487 csaf-2023.5.6/csaf/mandatory/
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-02-14 21:10:09.000000 csaf-2023.5.6/csaf/mandatory/__init__.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1325 2021-12-16 11:48:56.000000 csaf-2023.5.6/csaf/mandatory/acyclic_product_ids.py
+-rw-r--r--   0 ruth       (501) staff       (20)     2023 2021-12-16 11:48:42.000000 csaf-2023.5.6/csaf/mandatory/consistent_product_status.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1435 2022-02-13 17:11:58.000000 csaf-2023.5.6/csaf/mandatory/defined_group_ids.py
+-rw-r--r--   0 ruth       (501) staff       (20)     2548 2022-02-13 17:04:26.000000 csaf-2023.5.6/csaf/mandatory/defined_product_ids.py
+-rw-r--r--   0 ruth       (501) staff       (20)     5288 2022-06-19 10:04:43.000000 csaf-2023.5.6/csaf/mandatory/rules.py
+-rw-r--r--   0 ruth       (501) staff       (20)      981 2022-02-13 16:48:33.000000 csaf-2023.5.6/csaf/mandatory/translator_and_source_lang.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1267 2022-02-13 20:44:51.000000 csaf-2023.5.6/csaf/mandatory/unique_group_ids.py
+-rw-r--r--   0 ruth       (501) staff       (20)     1192 2022-02-13 20:40:08.000000 csaf-2023.5.6/csaf/mandatory/unique_product_ids.py
+-rw-r--r--   0 ruth       (501) staff       (20)     2390 2022-02-13 16:48:33.000000 csaf-2023.5.6/csaf/mandatory/valid_category_name.py
+-rw-r--r--   0 ruth       (501) staff       (20)    16500 2022-07-31 13:32:20.000000 csaf-2023.5.6/csaf/product.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:29:21.000000 csaf-2023.5.6/csaf/purl.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:28:33.000000 csaf-2023.5.6/csaf/terminal.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:28:41.000000 csaf-2023.5.6/csaf/tlp.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:28:29.000000 csaf-2023.5.6/csaf/version.py
+-rw-r--r--   0 ruth       (501) staff       (20)     3354 2022-03-13 16:02:22.000000 csaf-2023.5.6/csaf/vuln_types.py
+-rw-r--r--   0 ruth       (501) staff       (20)    13432 2022-07-31 13:30:55.000000 csaf-2023.5.6/csaf/vulnerability.py
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-05-06 14:40:24.111520 csaf-2023.5.6/csaf.egg-info/
+-rw-r--r--   0 ruth       (501) staff       (20)     3732 2023-05-06 14:40:24.000000 csaf-2023.5.6/csaf.egg-info/PKG-INFO
+-rw-r--r--   0 ruth       (501) staff       (20)     1204 2023-05-06 14:40:24.000000 csaf-2023.5.6/csaf.egg-info/SOURCES.txt
+-rw-r--r--   0 ruth       (501) staff       (20)        1 2023-05-06 14:40:24.000000 csaf-2023.5.6/csaf.egg-info/dependency_links.txt
+-rw-r--r--   0 ruth       (501) staff       (20)       38 2023-05-06 14:40:24.000000 csaf-2023.5.6/csaf.egg-info/entry_points.txt
+-rw-r--r--   0 ruth       (501) staff       (20)      222 2023-05-06 14:40:24.000000 csaf-2023.5.6/csaf.egg-info/requires.txt
+-rw-r--r--   0 ruth       (501) staff       (20)        5 2023-05-06 14:40:24.000000 csaf-2023.5.6/csaf.egg-info/top_level.txt
+-rw-r--r--   0 ruth       (501) staff       (20)     3004 2023-05-06 14:31:45.000000 csaf-2023.5.6/pyproject.toml
+-rw-r--r--   0 ruth       (501) staff       (20)       38 2023-05-06 14:40:24.128708 csaf-2023.5.6/setup.cfg
+drwxr-xr-x   0 ruth       (501) staff       (20)        0 2023-05-06 14:40:24.128279 csaf-2023.5.6/test/
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:34:24.000000 csaf-2023.5.6/test/test_category.py
+-rw-r--r--   0 ruth       (501) staff       (20)      544 2023-05-06 14:12:39.000000 csaf-2023.5.6/test/test_cli.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:34:47.000000 csaf-2023.5.6/test/test_config.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:34:50.000000 csaf-2023.5.6/test/test_cpe.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:34:53.000000 csaf-2023.5.6/test/test_csaf.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:35:20.000000 csaf-2023.5.6/test/test_cve.py
+-rw-r--r--   0 ruth       (501) staff       (20)     8576 2023-05-06 14:28:48.000000 csaf-2023.5.6/test/test_cvss.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:35:26.000000 csaf-2023.5.6/test/test_cwe.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:35:29.000000 csaf-2023.5.6/test/test_document.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:33:14.000000 csaf-2023.5.6/test/test_env.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:35:43.000000 csaf-2023.5.6/test/test_product.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:35:46.000000 csaf-2023.5.6/test/test_purl.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:35:49.000000 csaf-2023.5.6/test/test_terminal.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:35:52.000000 csaf-2023.5.6/test/test_tlp.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:35:55.000000 csaf-2023.5.6/test/test_version.py
+-rw-r--r--   0 ruth       (501) staff       (20)        0 2022-03-13 13:35:59.000000 csaf-2023.5.6/test/test_vulnerability.py
```

### Comparing `csaf-2022.3.13/LICENSE` & `csaf-2023.5.6/LICENSE`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2021, 2022 Stefan Hagen
+Copyright (c) 2023 Stefan Hagen
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `csaf-2022.3.13/csaf/__init__.py` & `csaf-2023.5.6/csaf/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -47,13 +47,13 @@
 
 
 init_logger(name=APP_ENV, level=logging.DEBUG if DEBUG else None)
 
 from csaf.csaf import is_valid  # noqa
 
 # [[[fill git_describe()]]]
-__version__ = '2022.3.13+parent.a9f32152'
-# [[[end]]] (checksum: 84b6ae9dc99ae644ee5450c1bd533e4b)
+__version__ = '2023.5.6+parent.75eb2ed8'
+# [[[end]]] (checksum: 68f0baf39732daf74a5084a1979c2fad)
 __version_info__ = tuple(
     e if '-' not in e else e.split('-')[0] for part in __version__.split('+') for e in part.split('.') if e != 'parent'
 )
 __all__ = ['is_valid', 'log']
```

### Comparing `csaf-2022.3.13/csaf/cli.py` & `csaf-2023.5.6/csaf/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-#! /usr/bin/env python3
-# -*- coding: utf-8 -*-
-# pylint: disable=line-too-long
 """Commandline API gateway for csaf."""
 import sys
 from typing import List, Mapping
 
 import typer
 
 import csaf
```

### Comparing `csaf-2022.3.13/csaf/csaf.py` & `csaf-2023.5.6/csaf/csaf.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from __future__ import annotations
 
 import pathlib
 from itertools import chain
 from typing import Annotated, Dict, Iterator, List, Mapping, Optional, Tuple, no_type_check
 
 import jmespath
-import orjson
+import msgspec
 from langcodes import tag_is_valid
 from lazr.uri import URI, InvalidURIError  # type: ignore
 from pydantic import BaseModel, Field, validator
 
 import csaf
 from csaf import log
 from csaf.document import Document
@@ -32,14 +32,15 @@
     is_valid_unique_product_ids,
 )
 from csaf.product import ProductTree
 from csaf.vulnerability import Vulnerability
 
 ENCODING_ERRORS_POLICY = 'ignore'
 CSAF_MIN_BYTES = 92
+CSAF_WARN_MAX_BYTES = 15 << 20
 CSAF_VERSION_STRING = '2.0'
 
 
 class CSAF(BaseModel):
     """
     Representation of security advisory information as a JSON document.
     """
@@ -67,14 +68,15 @@
             min_items=1,
             title='Vulnerabilities',
         ),
     ]
 
     @no_type_check
     @validator('vulnerabilities')
+    @classmethod
     def check_len(cls, v):
         if not v:
             raise ValueError('vulnerabilities present but empty')
         return v
 
 
 @no_type_check
@@ -333,17 +335,19 @@
             yield line
 
 
 def peek(data: str) -> str:
     """Determine trivial format of data."""
     if len(data) < CSAF_MIN_BYTES:
         return 'TOO_SHORT'
+
     sample = data[:CSAF_MIN_BYTES].strip()
     if sample.startswith('{'):
-        return 'JSON'
+        warn_size = '_MAYBE_TOO_LARGE' if len(data) > CSAF_WARN_MAX_BYTES else ''
+        return f'JSON{warn_size}'
     if sample.startswith('<'):
         return 'XML'
     return 'UNKNOWN'
 
 
 def verify_request(argv: Optional[List[str]]) -> Tuple[int, str, List[str]]:
     """Fail with grace."""
@@ -370,16 +374,16 @@
 
     return 0, '', argv
 
 
 def verify_json(data: str) -> Tuple[int, str, List[str], Dict[str, object]]:
     """Verify the JSON as CSAF."""
     try:
-        doc = orjson.loads(data)
-    except orjson.JSONDecodeError:
+        doc = msgspec.json.decode(data)
+    except msgspec.DecodeError:
         return 1, 'advisory is no valid JSON', [], {}
 
     error, message = level_zero(doc)
     if error:
         return error, message, [], {}
     return 0, 'OK', [], doc
 
@@ -445,15 +449,17 @@
 
     if guess == 'TOO_SHORT':
         return 1, 'advisory is too short to be valid'
 
     if guess == 'UNKNOWN':
         return 1, 'advisory is of unknown format'
 
-    if guess == 'JSON':
+    if guess.startswith('JSON'):
+        if guess.endswith('_MAYBE_TOO_LARGE'):
+            log.warning('File of %d bytes may be above known file size limits' % len(data))
         error, message, strings, doc = verify_json(data)
         if error:
             log.error(message)
             return error, message
         # Later post process the business rules (spec tests) here
         # Like that:
         if is_valid(doc) is False:  # For now, we return NotImplemented, sorry
```

### Comparing `csaf-2022.3.13/csaf/cvss.py` & `csaf-2023.5.6/csaf/cvss.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """CSAF CVSS 2/3.0/3.1 proxy implementation."""
 
 from __future__ import annotations
 
 from enum import Enum
-from typing import Annotated, Optional
+from typing import Annotated, Optional, no_type_check
 
 from pydantic import BaseModel, Field
 
 from csaf.vuln_types import (
     AccessComplexityType,
     AccessVectorType,
     AttackComplexityType,
@@ -57,152 +57,163 @@
 
 
 class CVSS2(BaseModel):
     version: Annotated[Version, Field(description='CVSS Version')] = Version.two
     vector_string: Annotated[
         str,
         Field(
-            alias='vector_string',
+            alias='vectorString',
             regex=(
                 '^((AV:[NAL]|AC:[LMH]|Au:[MSN]|[CIA]:[NPC]|E:(U|POC|F|H|ND)|RL:(OF|TF|W|U|ND)|RC:(UC|UR|C|ND)|CDP:'
                 '(N|L|LM|MH|H|ND)|TD:(N|L|M|H|ND)|[CIA]R:(L|M|H|ND))/)*(AV:[NAL]|AC:[LMH]|Au:[MSN]|[CIA]:[NPC]|E:'
                 '(U|POC|F|H|ND)|RL:(OF|TF|W|U|ND)|RC:(UC|UR|C|ND)|CDP:(N|L|LM|MH|H|ND)|TD:(N|L|M|H|ND)|[CIA]R:'
                 '(L|M|H|ND))$'
             ),
         ),
     ]
-    access_vector: Annotated[Optional[AccessVectorType], Field(alias='access_vector')] = None
-    access_complexity: Annotated[Optional[AccessComplexityType], Field(alias='access_complexity')] = None
+    access_vector: Annotated[Optional[AccessVectorType], Field(alias='accessVector')] = None
+    access_complexity: Annotated[Optional[AccessComplexityType], Field(alias='accessComplexity')] = None
     authentication: Optional[AuthenticationType] = None
-    confidentiality_impact: Annotated[Optional[CiaType], Field(alias='confidentiality_impact')] = None
-    integrity_impact: Annotated[Optional[CiaType], Field(alias='integrity_impact')] = None
-    availability_impact: Annotated[Optional[CiaType], Field(alias='availability_impact')] = None
-    base_score: Annotated[ScoreType, Field(alias='base_score')]
+    confidentiality_impact: Annotated[Optional[CiaType], Field(alias='confidentialityImpact')] = None
+    integrity_impact: Annotated[Optional[CiaType], Field(alias='integrityImpact')] = None
+    availability_impact: Annotated[Optional[CiaType], Field(alias='availabilityImpact')] = None
+    base_score: Annotated[ScoreType, Field(alias='baseScore')]
     exploitability: Optional[ExploitabilityType] = None
-    remediation_level: Annotated[Optional[RemediationLevelType], Field(alias='remediation_level')] = None
-    report_confidence: Annotated[Optional[ReportConfidenceType], Field(alias='report_confidence')] = None
-    temporal_score: Annotated[Optional[ScoreType], Field(alias='temporal_score')] = None
+    remediation_level: Annotated[Optional[RemediationLevelType], Field(alias='remediationLevel')] = None
+    report_confidence: Annotated[Optional[ReportConfidenceType], Field(alias='reportConfidence')] = None
+    temporal_score: Annotated[Optional[ScoreType], Field(alias='temporalScore')] = None
     collateral_damage_potential: Annotated[
         Optional[CollateralDamagePotentialType],
-        Field(alias='collateral_damage_potential'),
+        Field(alias='collateralDamagePotential'),
     ] = None
-    target_distribution: Annotated[Optional[TargetDistributionType], Field(alias='target_distribution')] = None
+    target_distribution: Annotated[Optional[TargetDistributionType], Field(alias='targetDistribution')] = None
     confidentiality_requirement: Annotated[
-        Optional[CiaRequirementType], Field(alias='confidentiality_requirement')
+        Optional[CiaRequirementType], Field(alias='confidentialityRequirement')
     ] = None
-    integrity_requirement: Annotated[Optional[CiaRequirementType], Field(alias='integrity_requirement')] = None
-    availability_requirement: Annotated[Optional[CiaRequirementType], Field(alias='availability_requirement')] = None
-    environmental_score: Annotated[Optional[ScoreType], Field(alias='environmental_score')] = None
+    integrity_requirement: Annotated[Optional[CiaRequirementType], Field(alias='integrityRequirement')] = None
+    availability_requirement: Annotated[Optional[CiaRequirementType], Field(alias='availabilityRequirement')] = None
+    environmental_score: Annotated[Optional[ScoreType], Field(alias='environmentalScore')] = None
+
+    @no_type_check
+    def json(self, *args, **kwargs):
+        kwargs.setdefault('by_alias', True)
+        return super().json(*args, **kwargs)
 
 
 class CVSS30(BaseModel):
     version: Annotated[Version, Field(description='CVSS Version')] = Version.three_zero
     vector_string: Annotated[
         str,
         Field(
-            alias='vector_string',
+            alias='vectorString',
             regex=(
                 '^CVSS:3[.]0/((AV:[NALP]|AC:[LH]|PR:[UNLH]|UI:[NR]|S:[UC]|[CIA]:[NLH]|E:[XUPFH]|RL:[XOTWU]|RC:[XURC]|'
                 '[CIA]R:[XLMH]|MAV:[XNALP]|MAC:[XLH]|MPR:[XUNLH]|MUI:[XNR]|MS:[XUC]|M[CIA]:[XNLH])/)*(AV:[NALP]|'
                 'AC:[LH]|PR:[UNLH]|UI:[NR]|S:[UC]|[CIA]:[NLH]|E:[XUPFH]|RL:[XOTWU]|RC:[XURC]|[CIA]R:[XLMH]|'
                 'MAV:[XNALP]|MAC:[XLH]|MPR:[XUNLH]|MUI:[XNR]|MS:[XUC]|M[CIA]:[XNLH])$'
             ),
         ),
     ]
-    attack_vector: Annotated[Optional[AttackVectorType], Field(alias='attack_vector')] = None
-    attack_complexity: Annotated[Optional[AttackComplexityType], Field(alias='attack_complexity')] = None
-    privileges_required: Annotated[Optional[PrivilegesRequiredType], Field(alias='privileges_required')] = None
-    user_interaction: Annotated[Optional[UserInteractionType], Field(alias='user_interaction')] = None
+    attack_vector: Annotated[Optional[AttackVectorType], Field(alias='attackVector')] = None
+    attack_complexity: Annotated[Optional[AttackComplexityType], Field(alias='attackComplexity')] = None
+    privileges_required: Annotated[Optional[PrivilegesRequiredType], Field(alias='privilegesRequired')] = None
+    user_interaction: Annotated[Optional[UserInteractionType], Field(alias='userInteraction')] = None
     scope: Optional[ScopeType] = None
-    confidentiality_impact: Annotated[Optional[CiaType], Field(alias='confidentiality_impact')] = None
-    integrity_impact: Annotated[Optional[CiaType], Field(alias='integrity_impact')] = None
-    availability_impact: Annotated[Optional[CiaType], Field(alias='availability_impact')] = None
-    base_score: Annotated[ScoreType, Field(alias='base_score')]
-    base_severity: Annotated[SeverityType, Field(alias='base_severity')]
-    exploit_code_maturity: Annotated[Optional[ExploitCodeMaturityType], Field(alias='exploit_code_maturity')] = None
-    remediation_level: Annotated[Optional[RemediationLevelType], Field(alias='remediation_level')] = None
-    report_confidence: Annotated[Optional[ConfidenceType], Field(alias='report_confidence')] = None
-    temporal_score: Annotated[Optional[ScoreType], Field(alias='temporal_score')] = None
-    temporal_severity: Annotated[Optional[SeverityType], Field(alias='temporal_severity')] = None
+    confidentiality_impact: Annotated[Optional[CiaType], Field(alias='confidentialityImpact')] = None
+    integrity_impact: Annotated[Optional[CiaType], Field(alias='integrityImpact')] = None
+    availability_impact: Annotated[Optional[CiaType], Field(alias='availabilityImpact')] = None
+    base_score: Annotated[ScoreType, Field(alias='baseScore')]
+    base_severity: Annotated[SeverityType, Field(alias='baseSeverity')]
+    exploit_code_maturity: Annotated[Optional[ExploitCodeMaturityType], Field(alias='exploitCodeMaturity')] = None
+    remediation_level: Annotated[Optional[RemediationLevelType], Field(alias='remediationLevel')] = None
+    report_confidence: Annotated[Optional[ConfidenceType], Field(alias='reportConfidence')] = None
+    temporal_score: Annotated[Optional[ScoreType], Field(alias='temporalScore')] = None
+    temporal_severity: Annotated[Optional[SeverityType], Field(alias='temporalSeverity')] = None
     confidentiality_requirement: Annotated[
-        Optional[CiaRequirementType], Field(alias='confidentiality_requirement')
+        Optional[CiaRequirementType], Field(alias='confidentialityRequirement')
     ] = None
-    integrity_requirement: Annotated[Optional[CiaRequirementType], Field(alias='integrity_requirement')] = None
-    availability_requirement: Annotated[Optional[CiaRequirementType], Field(alias='availability_requirement')] = None
-    modified_attack_vector: Annotated[Optional[ModifiedAttackVectorType], Field(alias='modified_attack_vector')] = None
+    integrity_requirement: Annotated[Optional[CiaRequirementType], Field(alias='integrityRequirement')] = None
+    availability_requirement: Annotated[Optional[CiaRequirementType], Field(alias='availabilityRequirement')] = None
+    modified_attack_vector: Annotated[Optional[ModifiedAttackVectorType], Field(alias='modifiedAttackVector')] = None
     modified_attack_complexity: Annotated[
-        Optional[ModifiedAttackComplexityType], Field(alias='modified_attack_complexity')
+        Optional[ModifiedAttackComplexityType], Field(alias='modifiedAttackComplexity')
     ] = None
     modified_privileges_required: Annotated[
         Optional[ModifiedPrivilegesRequiredType],
-        Field(alias='modified_privileges_required'),
+        Field(alias='modifiedPrivilegesRequired'),
     ] = None
     modified_user_interaction: Annotated[
-        Optional[ModifiedUserInteractionType], Field(alias='modified_user_interaction')
+        Optional[ModifiedUserInteractionType], Field(alias='modifiedUserInteraction')
     ] = None
-    modified_scope: Annotated[Optional[ModifiedScopeType], Field(alias='modified_scope')] = None
+    modified_scope: Annotated[Optional[ModifiedScopeType], Field(alias='modifiedScope')] = None
     modified_confidentiality_impact: Annotated[
-        Optional[ModifiedCiaType], Field(alias='modified_confidentiality_impact')
+        Optional[ModifiedCiaType], Field(alias='modifiedConfidentialityImpact')
     ] = None
-    modified_integrity_impact: Annotated[Optional[ModifiedCiaType], Field(alias='modified_integrity_impact')] = None
-    modified_availability_impact: Annotated[
-        Optional[ModifiedCiaType], Field(alias='modified_availability_impact')
-    ] = None
-    environmental_score: Annotated[Optional[ScoreType], Field(alias='environmental_score')] = None
-    environmental_severity: Annotated[Optional[SeverityType], Field(alias='environmental_severity')] = None
+    modified_integrity_impact: Annotated[Optional[ModifiedCiaType], Field(alias='modifiedIntegrityImpact')] = None
+    modified_availability_impact: Annotated[Optional[ModifiedCiaType], Field(alias='modifiedAvailabilityImpact')] = None
+    environmental_score: Annotated[Optional[ScoreType], Field(alias='environmentalScore')] = None
+    environmental_severity: Annotated[Optional[SeverityType], Field(alias='environmentalSeverity')] = None
+
+    @no_type_check
+    def json(self, *args, **kwargs):
+        kwargs.setdefault('by_alias', True)
+        return super().json(*args, **kwargs)
 
 
 class CVSS31(BaseModel):
     version: Annotated[Version, Field(description='CVSS Version')] = Version.three_wun
     vector_string: Annotated[
         str,
         Field(
-            alias='vector_string',
+            alias='vectorString',
             regex=(
                 '^CVSS:3[.]1/((AV:[NALP]|AC:[LH]|PR:[NLH]|UI:[NR]|S:[UC]|[CIA]:[NLH]|E:[XUPFH]|RL:[XOTWU]|RC:'
                 '[XURC]|[CIA]R:[XLMH]|MAV:[XNALP]|MAC:[XLH]|MPR:[XNLH]|MUI:[XNR]|MS:[XUC]|M[CIA]:[XNLH])/)*'
                 '(AV:[NALP]|AC:[LH]|PR:[NLH]|UI:[NR]|S:[UC]|[CIA]:[NLH]|E:[XUPFH]|RL:[XOTWU]|RC:[XURC]|[CIA]R:'
                 '[XLMH]|MAV:[XNALP]|MAC:[XLH]|MPR:[XNLH]|MUI:[XNR]|MS:[XUC]|M[CIA]:[XNLH])$'
             ),
         ),
     ]
-    attack_vector: Annotated[Optional[AttackVectorType], Field(alias='attack_vector')] = None
-    attack_complexity: Annotated[Optional[AttackComplexityType], Field(alias='attack_complexity')] = None
-    privileges_required: Annotated[Optional[PrivilegesRequiredType], Field(alias='privileges_required')] = None
-    user_interaction: Annotated[Optional[UserInteractionType], Field(alias='user_interaction')] = None
+    attack_vector: Annotated[Optional[AttackVectorType], Field(alias='attackVector')] = None
+    attack_complexity: Annotated[Optional[AttackComplexityType], Field(alias='attackComplexity')] = None
+    privileges_required: Annotated[Optional[PrivilegesRequiredType], Field(alias='privilegesRequired')] = None
+    user_interaction: Annotated[Optional[UserInteractionType], Field(alias='userInteraction')] = None
     scope: Optional[ScopeType] = None
-    confidentiality_impact: Annotated[Optional[CiaType], Field(alias='confidentiality_impact')] = None
-    integrity_impact: Annotated[Optional[CiaType], Field(alias='integrity_impact')] = None
-    availability_impact: Annotated[Optional[CiaType], Field(alias='availability_impact')] = None
-    base_score: Annotated[ScoreType, Field(alias='base_score')]
-    base_severity: Annotated[SeverityType, Field(alias='base_severity')]
-    exploit_code_maturity: Annotated[Optional[ExploitCodeMaturityType], Field(alias='exploit_code_maturity')] = None
-    remediation_level: Annotated[Optional[RemediationLevelType], Field(alias='remediation_level')] = None
-    report_confidence: Annotated[Optional[ConfidenceType], Field(alias='report_confidence')] = None
-    temporal_score: Annotated[Optional[ScoreType], Field(alias='temporal_score')] = None
-    temporal_severity: Annotated[Optional[SeverityType], Field(alias='temporal_severity')] = None
+    confidentiality_impact: Annotated[Optional[CiaType], Field(alias='confidentialityImpact')] = None
+    integrity_impact: Annotated[Optional[CiaType], Field(alias='integrityImpact')] = None
+    availability_impact: Annotated[Optional[CiaType], Field(alias='availabilityImpact')] = None
+    base_score: Annotated[ScoreType, Field(alias='baseScore')]
+    base_severity: Annotated[SeverityType, Field(alias='baseSeverity')]
+    exploit_code_maturity: Annotated[Optional[ExploitCodeMaturityType], Field(alias='exploitCodeMaturity')] = None
+    remediation_level: Annotated[Optional[RemediationLevelType], Field(alias='remediationLevel')] = None
+    report_confidence: Annotated[Optional[ConfidenceType], Field(alias='reportConfidence')] = None
+    temporal_score: Annotated[Optional[ScoreType], Field(alias='temporalScore')] = None
+    temporal_severity: Annotated[Optional[SeverityType], Field(alias='temporalSeverity')] = None
     confidentiality_requirement: Annotated[
-        Optional[CiaRequirementType], Field(alias='confidentiality_requirement')
+        Optional[CiaRequirementType], Field(alias='confidentialityRequirement')
     ] = None
-    integrity_requirement: Annotated[Optional[CiaRequirementType], Field(alias='integrity_requirement')] = None
-    availability_requirement: Annotated[Optional[CiaRequirementType], Field(alias='availability_requirement')] = None
-    modified_attack_vector: Annotated[Optional[ModifiedAttackVectorType], Field(alias='modified_attack_vector')] = None
+    integrity_requirement: Annotated[Optional[CiaRequirementType], Field(alias='integrityRequirement')] = None
+    availability_requirement: Annotated[Optional[CiaRequirementType], Field(alias='availabilityRequirement')] = None
+    modified_attack_vector: Annotated[Optional[ModifiedAttackVectorType], Field(alias='modifiedAttackVector')] = None
     modified_attack_complexity: Annotated[
-        Optional[ModifiedAttackComplexityType], Field(alias='modified_attack_complexity')
+        Optional[ModifiedAttackComplexityType], Field(alias='modifiedAttackComplexity')
     ] = None
     modified_privileges_required: Annotated[
         Optional[ModifiedPrivilegesRequiredType],
-        Field(alias='modified_privileges_required'),
+        Field(alias='modifiedPrivilegesRequired'),
     ] = None
     modified_user_interaction: Annotated[
-        Optional[ModifiedUserInteractionType], Field(alias='modified_user_interaction')
+        Optional[ModifiedUserInteractionType], Field(alias='modifiedUserInteraction')
     ] = None
-    modified_scope: Annotated[Optional[ModifiedScopeType], Field(alias='modified_scope')] = None
+    modified_scope: Annotated[Optional[ModifiedScopeType], Field(alias='modifiedScope')] = None
     modified_confidentiality_impact: Annotated[
-        Optional[ModifiedCiaType], Field(alias='modified_confidentiality_impact')
-    ] = None
-    modified_integrity_impact: Annotated[Optional[ModifiedCiaType], Field(alias='modified_integrity_impact')] = None
-    modified_availability_impact: Annotated[
-        Optional[ModifiedCiaType], Field(alias='modified_availability_impact')
+        Optional[ModifiedCiaType], Field(alias='modifiedConfidentialityImpact')
     ] = None
-    environmental_score: Annotated[Optional[ScoreType], Field(alias='environmental_score')] = None
-    environmental_severity: Annotated[Optional[SeverityType], Field(alias='environmental_severity')] = None
+    modified_integrity_impact: Annotated[Optional[ModifiedCiaType], Field(alias='modifiedIntegrityImpact')] = None
+    modified_availability_impact: Annotated[Optional[ModifiedCiaType], Field(alias='modifiedAvailabilityImpact')] = None
+    environmental_score: Annotated[Optional[ScoreType], Field(alias='environmentalScore')] = None
+    environmental_severity: Annotated[Optional[SeverityType], Field(alias='environmentalSeverity')] = None
+
+    @no_type_check
+    def json(self, *args, **kwargs):
+        kwargs.setdefault('by_alias', True)
+        return super().json(*args, **kwargs)
```

### Comparing `csaf-2022.3.13/csaf/definitions.py` & `csaf-2023.5.6/csaf/definitions.py`

 * *Files 3% similar despite different names*

```diff
@@ -85,14 +85,15 @@
             min_items=1,
             title='List of URLs',
         ),
     ]
 
     @no_type_check
     @validator('names', 'organization', 'summary', 'urls')
+    @classmethod
     def check_len(cls, v):
         if not v:
             raise ValueError('optional element present but empty')
         return v
 
 
 class Acknowledgments(BaseModel):
@@ -107,14 +108,15 @@
             min_items=1,
             title='List of acknowledgments',
         ),
     ]
 
     @no_type_check
     @validator('__root__')
+    @classmethod
     def check_len(cls, v):
         if not v:
             raise ValueError('optional element present but empty')
         return v
 
 
 class ReferenceTokenForProductGroupInstance(BaseModel):
@@ -160,14 +162,15 @@
             min_items=1,
             title='List of product_group_ids',
         ),
     ]
 
     @no_type_check
     @validator('__root__')
+    @classmethod
     def check_len(cls, v):
         if not v:
             raise ValueError('mandatory element present but empty')
         return v
 
 
 class ProductId(BaseModel):
@@ -196,15 +199,15 @@
             min_items=1,
             title='List of product_ids',
         ),
     ]
 
 
 class ReferenceTokenForProductInstance(BaseModel):
-    value: Annotated[
+    __root__: Annotated[
         str,
         Field(
             description=(
                 'Token required to identify a full_product_name so that it can be referred to from other'
                 ' parts in the document.'
                 ' There is no predefined or required format for the product_id as long as it uniquely'
                 ' identifies a product in the context of the current document.'
@@ -228,14 +231,15 @@
             # min_items=1,
             title='List of product_ids',
         ),
     ]
 
     @no_type_check
     @validator('product_ids')
+    @classmethod
     def check_len(cls, v):
         if not v:
             raise ValueError('mandatory element present but empty')
         return v
 
 
 class Lang(BaseModel):
@@ -327,14 +331,15 @@
             min_items=1,
             title='List of notes',
         ),
     ]
 
     @no_type_check
     @validator('__root__')
+    @classmethod
     def check_len(cls, v):
         if not v:
             raise ValueError('mandatory element present but empty')
         return v
 
 
 class ReferenceCategory(Enum):
```

### Comparing `csaf-2022.3.13/csaf/document.py` & `csaf-2023.5.6/csaf/document.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,14 +97,15 @@
             title='Document status',
         ),
     ]
     version: Version
 
     @no_type_check
     @validator('revision_history')
+    @classmethod
     def check_len(cls, v):
         if not v:
             raise ValueError('mandatory element present but empty')
         return v
 
 
 class AggregateSeverity(BaseModel):
```

### Comparing `csaf-2022.3.13/csaf/env.py` & `csaf-2023.5.6/csaf/env.py`

 * *Files identical despite different names*

### Comparing `csaf-2022.3.13/csaf/mandatory/acyclic_product_ids.py` & `csaf-2023.5.6/csaf/mandatory/acyclic_product_ids.py`

 * *Files identical despite different names*

### Comparing `csaf-2022.3.13/csaf/mandatory/consistent_product_status.py` & `csaf-2023.5.6/csaf/mandatory/consistent_product_status.py`

 * *Files identical despite different names*

### Comparing `csaf-2022.3.13/csaf/mandatory/defined_group_ids.py` & `csaf-2023.5.6/csaf/mandatory/defined_group_ids.py`

 * *Files identical despite different names*

### Comparing `csaf-2022.3.13/csaf/mandatory/defined_product_ids.py` & `csaf-2023.5.6/csaf/mandatory/defined_product_ids.py`

 * *Files identical despite different names*

### Comparing `csaf-2022.3.13/csaf/mandatory/rules.py` & `csaf-2023.5.6/csaf/mandatory/rules.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,14 +84,15 @@
     return True
 
 
 @no_type_check
 def is_valid_defined_product_ids(document: dict) -> bool:
     """Temporary implementation of rule for defined product ids."""
     defined_prod_ids = jmespath.search(def_pro_ids.TRIGGER_JMES_PATH, document)
+    # TODO(sthagen) too shallow tree visiting # print("DEBUG>>>", defined_prod_ids)
     if defined_prod_ids is None:
         defined_prod_ids = []
     known_prod_ids = set(defined_prod_ids)
     for path in def_pro_ids.CONDITION_JMES_PATHS:
         claim_prod_ids = jmespath.search(path, document)
         if claim_prod_ids is not None:
             if any(claim_prod_id not in known_prod_ids for claim_prod_id in claim_prod_ids):
```

### Comparing `csaf-2022.3.13/csaf/mandatory/translator_and_source_lang.py` & `csaf-2023.5.6/csaf/mandatory/translator_and_source_lang.py`

 * *Files identical despite different names*

### Comparing `csaf-2022.3.13/csaf/mandatory/unique_group_ids.py` & `csaf-2023.5.6/csaf/mandatory/unique_group_ids.py`

 * *Files identical despite different names*

### Comparing `csaf-2022.3.13/csaf/mandatory/unique_product_ids.py` & `csaf-2023.5.6/csaf/mandatory/unique_product_ids.py`

 * *Files identical despite different names*

### Comparing `csaf-2022.3.13/csaf/mandatory/valid_category_name.py` & `csaf-2023.5.6/csaf/mandatory/valid_category_name.py`

 * *Files identical despite different names*

### Comparing `csaf-2022.3.13/csaf/product.py` & `csaf-2023.5.6/csaf/product.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,14 +65,15 @@
             # min_length=1,
             title='Filename',
         ),
     ]
 
     @no_type_check
     @validator('file_hashes', 'filename')
+    @classmethod
     def check_len(cls, v):
         if not v:
             raise ValueError('mandatory element present but empty')
         return v
 
 
 class GenericUri(BaseModel):
@@ -196,21 +197,23 @@
             # min_items=1,
             title='List of generic URIs',
         ),
     ] = None
 
     @no_type_check
     @validator('hashes', 'sbom_urls', 'serial_numbers', 'skus', 'x_generic_uris')
+    @classmethod
     def check_len(cls, v):
         if not v:
             raise ValueError('optional element present but empty')
         return v
 
     @no_type_check
     @validator('purl')
+    @classmethod
     def check_purl(cls, v):
         if not v or len(v) < 7:
             raise ValueError('optional purl element present but too short')
         if not re.match('^pkg:[A-Za-z\\.\\-\\+][A-Za-z0-9\\.\\-\\+]*/.+', v):
             raise ValueError('optional purl element present but is no purl (regex does not match)')
         return v
 
@@ -271,14 +274,15 @@
             min_length=1,
             title='Summary of the product group',
         ),
     ] = None
 
     @no_type_check
     @validator('product_ids')
+    @classmethod
     def check_len(cls, v):
         if len(v) < 2:
             raise ValueError('mandatory element present but too few items')
         return v
 
 
 class ProductStatus(BaseModel):
@@ -428,14 +432,15 @@
             min_items=1,
             title='List of relationships',
         ),
     ]
 
     @no_type_check
     @validator('full_product_names', 'product_groups', 'relationships')
+    @classmethod
     def check_len(cls, v):
         if not v:
             raise ValueError('optional element present but empty')
         return v
 
 
 class BranchCategory(Enum):
@@ -502,14 +507,15 @@
             min_items=1,
             title='List of branches',
         ),
     ]
 
     @no_type_check
     @validator('__root__')
+    @classmethod
     def check_len(cls, v):
         if not v:
             raise ValueError('mandatory element present but empty')
         return v
 
 
 Branch.update_forward_refs()
```

### Comparing `csaf-2022.3.13/csaf/vuln_types.py` & `csaf-2023.5.6/csaf/vuln_types.py`

 * *Files identical despite different names*

### Comparing `csaf-2022.3.13/csaf/vulnerability.py` & `csaf-2023.5.6/csaf/vulnerability.py`

 * *Files 0% similar despite different names*

```diff
@@ -328,14 +328,15 @@
             description='Contains the URL where to obtain the remediation.',
             title='URL to the remediation',
         ),
     ]
 
     @no_type_check
     @validator('entitlements')
+    @classmethod
     def check_len(cls, v):
         if not v:
             raise ValueError('optional element present but empty')
         return v
 
 
 class Threat(BaseModel):
@@ -493,11 +494,12 @@
             min_length=1,
             title='Title',
         ),
     ]
 
     @no_type_check
     @validator('involvements', 'remediations', 'scores', 'threats')
+    @classmethod
     def check_len(cls, v):
         if not v:
             raise ValueError('optional element present but empty')
         return v
```

### Comparing `csaf-2022.3.13/csaf.egg-info/SOURCES.txt` & `csaf-2023.5.6/csaf.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
-setup.cfg
-setup.py
 csaf/__init__.py
 csaf/__main__.py
 csaf/category.py
 csaf/cli.py
 csaf/config.py
 csaf/cpe.py
 csaf/csaf.py
@@ -37,25 +35,23 @@
 csaf/mandatory/defined_group_ids.py
 csaf/mandatory/defined_product_ids.py
 csaf/mandatory/rules.py
 csaf/mandatory/translator_and_source_lang.py
 csaf/mandatory/unique_group_ids.py
 csaf/mandatory/unique_product_ids.py
 csaf/mandatory/valid_category_name.py
-tests/__init__.py
-tests/context.py
-tests/test_category.py
-tests/test_cli.py
-tests/test_config.py
-tests/test_cpe.py
-tests/test_csaf.py
-tests/test_cve.py
-tests/test_cvss.py
-tests/test_cwe.py
-tests/test_document.py
-tests/test_env.py
-tests/test_product.py
-tests/test_purl.py
-tests/test_terminal.py
-tests/test_tlp.py
-tests/test_version.py
-tests/test_vulnerability.py
+test/test_category.py
+test/test_cli.py
+test/test_config.py
+test/test_cpe.py
+test/test_csaf.py
+test/test_cve.py
+test/test_cvss.py
+test/test_cwe.py
+test/test_document.py
+test/test_env.py
+test/test_product.py
+test/test_purl.py
+test/test_terminal.py
+test/test_tlp.py
+test/test_version.py
+test/test_vulnerability.py
```

