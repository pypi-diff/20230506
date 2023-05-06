# Comparing `tmp/age-0.4.1.tar.gz` & `tmp/age-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/age-0.4.1.tar", last modified: Sun Dec 27 22:50:38 2020, max compression
+gzip compressed data, was "age-0.5.1.tar", last modified: Sat May  6 13:08:21 2023, max compression
```

## Comparing `age-0.4.1.tar` & `age-0.5.1.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-27 22:50:38.252519 age-0.4.1/
--rw-r--r--   0 runner    (1001) docker     (116)     1055 2020-12-27 22:50:30.000000 age-0.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      156 2020-12-27 22:50:30.000000 age-0.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     3356 2020-12-27 22:50:38.252519 age-0.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1905 2020-12-27 22:50:30.000000 age-0.4.1/README.md
--rw-r--r--   0 runner    (1001) docker     (116)      153 2020-12-27 22:50:30.000000 age-0.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (116)     2419 2020-12-27 22:50:38.252519 age-0.4.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     1246 2020-12-27 22:50:30.000000 age-0.4.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-27 22:50:38.244519 age-0.4.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-27 22:50:38.252519 age-0.4.1/src/age/
--rw-r--r--   0 runner    (1001) docker     (116)       93 2020-12-27 22:50:30.000000 age-0.4.1/src/age/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      497 2020-12-27 22:50:38.252519 age-0.4.1/src/age/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-27 22:50:38.248519 age-0.4.1/src/age/algorithms/
--rw-r--r--   0 runner    (1001) docker     (116)      489 2020-12-27 22:50:30.000000 age-0.4.1/src/age/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1257 2020-12-27 22:50:30.000000 age-0.4.1/src/age/algorithms/scrypt.py
--rw-r--r--   0 runner    (1001) docker     (116)     2124 2020-12-27 22:50:30.000000 age-0.4.1/src/age/algorithms/ssh_ed25519.py
--rw-r--r--   0 runner    (1001) docker     (116)     1012 2020-12-27 22:50:30.000000 age-0.4.1/src/age/algorithms/ssh_rsa.py
--rw-r--r--   0 runner    (1001) docker     (116)     3460 2020-12-27 22:50:30.000000 age-0.4.1/src/age/algorithms/x25519.py
--rw-r--r--   0 runner    (1001) docker     (116)     7411 2020-12-27 22:50:30.000000 age-0.4.1/src/age/cli.py
--rw-r--r--   0 runner    (1001) docker     (116)      416 2020-12-27 22:50:30.000000 age-0.4.1/src/age/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (116)     4122 2020-12-27 22:50:30.000000 age-0.4.1/src/age/file.py
--rw-r--r--   0 runner    (1001) docker     (116)     2204 2020-12-27 22:50:30.000000 age-0.4.1/src/age/format.py
--rw-r--r--   0 runner    (1001) docker     (116)     5122 2020-12-27 22:50:30.000000 age-0.4.1/src/age/keyloader.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-27 22:50:38.248519 age-0.4.1/src/age/keys/
--rw-r--r--   0 runner    (1001) docker     (116)      248 2020-12-27 22:50:30.000000 age-0.4.1/src/age/keys/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3596 2020-12-27 22:50:30.000000 age-0.4.1/src/age/keys/agekey.py
--rw-r--r--   0 runner    (1001) docker     (116)       97 2020-12-27 22:50:30.000000 age-0.4.1/src/age/keys/base.py
--rw-r--r--   0 runner    (1001) docker     (116)     4742 2020-12-27 22:50:30.000000 age-0.4.1/src/age/keys/ed25519.py
--rw-r--r--   0 runner    (1001) docker     (116)      289 2020-12-27 22:50:30.000000 age-0.4.1/src/age/keys/password.py
--rw-r--r--   0 runner    (1001) docker     (116)     3771 2020-12-27 22:50:30.000000 age-0.4.1/src/age/keys/rsa.py
--rw-r--r--   0 runner    (1001) docker     (116)    10059 2020-12-27 22:50:30.000000 age-0.4.1/src/age/openssh_keys.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-27 22:50:38.248519 age-0.4.1/src/age/primitives/
--rw-r--r--   0 runner    (1001) docker     (116)      589 2020-12-27 22:50:30.000000 age-0.4.1/src/age/primitives/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     6544 2020-12-27 22:50:30.000000 age-0.4.1/src/age/primitives/bech32.py
--rw-r--r--   0 runner    (1001) docker     (116)      912 2020-12-27 22:50:30.000000 age-0.4.1/src/age/primitives/encode.py
--rw-r--r--   0 runner    (1001) docker     (116)      936 2020-12-27 22:50:30.000000 age-0.4.1/src/age/primitives/encrypt.py
--rw-r--r--   0 runner    (1001) docker     (116)      361 2020-12-27 22:50:30.000000 age-0.4.1/src/age/primitives/hashes.py
--rw-r--r--   0 runner    (1001) docker     (116)      744 2020-12-27 22:50:30.000000 age-0.4.1/src/age/primitives/hkdf.py
--rw-r--r--   0 runner    (1001) docker     (116)     2035 2020-12-27 22:50:30.000000 age-0.4.1/src/age/primitives/hmac.py
--rw-r--r--   0 runner    (1001) docker     (116)      281 2020-12-27 22:50:30.000000 age-0.4.1/src/age/primitives/random.py
--rw-r--r--   0 runner    (1001) docker     (116)     1418 2020-12-27 22:50:30.000000 age-0.4.1/src/age/primitives/rsa_oaep.py
--rw-r--r--   0 runner    (1001) docker     (116)      533 2020-12-27 22:50:30.000000 age-0.4.1/src/age/primitives/scrypt.py
--rw-r--r--   0 runner    (1001) docker     (116)     2001 2020-12-27 22:50:30.000000 age-0.4.1/src/age/primitives/x25519.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-27 22:50:38.248519 age-0.4.1/src/age/recipients/
--rw-r--r--   0 runner    (1001) docker     (116)      292 2020-12-27 22:50:30.000000 age-0.4.1/src/age/recipients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      713 2020-12-27 22:50:30.000000 age-0.4.1/src/age/recipients/base.py
--rw-r--r--   0 runner    (1001) docker     (116)     2095 2020-12-27 22:50:30.000000 age-0.4.1/src/age/recipients/helpers.py
--rw-r--r--   0 runner    (1001) docker     (116)     1493 2020-12-27 22:50:30.000000 age-0.4.1/src/age/recipients/scrypt.py
--rw-r--r--   0 runner    (1001) docker     (116)     1795 2020-12-27 22:50:30.000000 age-0.4.1/src/age/recipients/ssh_ed25519.py
--rw-r--r--   0 runner    (1001) docker     (116)     1429 2020-12-27 22:50:30.000000 age-0.4.1/src/age/recipients/ssh_rsa.py
--rw-r--r--   0 runner    (1001) docker     (116)     1493 2020-12-27 22:50:30.000000 age-0.4.1/src/age/recipients/x25519.py
--rw-r--r--   0 runner    (1001) docker     (116)     1509 2020-12-27 22:50:30.000000 age-0.4.1/src/age/stream.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-27 22:50:38.252519 age-0.4.1/src/age/utils/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2020-12-27 22:50:30.000000 age-0.4.1/src/age/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     4299 2020-12-27 22:50:30.000000 age-0.4.1/src/age/utils/asciiarmor.py
--rw-r--r--   0 runner    (1001) docker     (116)      231 2020-12-27 22:50:30.000000 age-0.4.1/src/age/utils/copy_doc.py
--rw-r--r--   0 runner    (1001) docker     (116)      224 2020-12-27 22:50:30.000000 age-0.4.1/src/age/utils/env.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2020-12-27 22:50:38.248519 age-0.4.1/src/age.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     3356 2020-12-27 22:50:38.000000 age-0.4.1/src/age.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1361 2020-12-27 22:50:38.000000 age-0.4.1/src/age.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2020-12-27 22:50:38.000000 age-0.4.1/src/age.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       40 2020-12-27 22:50:38.000000 age-0.4.1/src/age.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)      244 2020-12-27 22:50:38.000000 age-0.4.1/src/age.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        4 2020-12-27 22:50:38.000000 age-0.4.1/src/age.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)    68611 2020-12-27 22:50:30.000000 age-0.4.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 13:08:21.557603 age-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-06 13:08:10.000000 age-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      156 2023-05-06 13:08:10.000000 age-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-05-06 13:08:21.557603 age-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1905 2023-05-06 13:08:10.000000 age-0.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-06 13:08:10.000000 age-0.5.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-05-06 13:08:21.557603 age-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-05-06 13:08:10.000000 age-0.5.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 13:08:21.545603 age-0.5.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 13:08:21.557603 age-0.5.1/src/age/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-06 13:08:10.000000 age-0.5.1/src/age/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-06 13:08:21.557603 age-0.5.1/src/age/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 13:08:21.549603 age-0.5.1/src/age/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-06 13:08:10.000000 age-0.5.1/src/age/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1189 2023-05-06 13:08:10.000000 age-0.5.1/src/age/algorithms/scrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2123 2023-05-06 13:08:10.000000 age-0.5.1/src/age/algorithms/ssh_ed25519.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-05-06 13:08:10.000000 age-0.5.1/src/age/algorithms/ssh_rsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3460 2023-05-06 13:08:10.000000 age-0.5.1/src/age/algorithms/x25519.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7554 2023-05-06 13:08:10.000000 age-0.5.1/src/age/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-06 13:08:10.000000 age-0.5.1/src/age/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4122 2023-05-06 13:08:10.000000 age-0.5.1/src/age/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2283 2023-05-06 13:08:10.000000 age-0.5.1/src/age/format.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5156 2023-05-06 13:08:10.000000 age-0.5.1/src/age/keyloader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 13:08:21.549603 age-0.5.1/src/age/keys/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-06 13:08:10.000000 age-0.5.1/src/age/keys/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3596 2023-05-06 13:08:10.000000 age-0.5.1/src/age/keys/agekey.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-06 13:08:10.000000 age-0.5.1/src/age/keys/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4773 2023-05-06 13:08:10.000000 age-0.5.1/src/age/keys/ed25519.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-06 13:08:10.000000 age-0.5.1/src/age/keys/password.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-05-06 13:08:10.000000 age-0.5.1/src/age/keys/rsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10098 2023-05-06 13:08:10.000000 age-0.5.1/src/age/openssh_keys.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 13:08:21.553603 age-0.5.1/src/age/primitives/
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-06 13:08:10.000000 age-0.5.1/src/age/primitives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6544 2023-05-06 13:08:10.000000 age-0.5.1/src/age/primitives/bech32.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-06 13:08:10.000000 age-0.5.1/src/age/primitives/encode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-06 13:08:10.000000 age-0.5.1/src/age/primitives/encrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-05-06 13:08:10.000000 age-0.5.1/src/age/primitives/hashes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-06 13:08:10.000000 age-0.5.1/src/age/primitives/hkdf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-06 13:08:10.000000 age-0.5.1/src/age/primitives/hmac.py
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-05-06 13:08:10.000000 age-0.5.1/src/age/primitives/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-06 13:08:10.000000 age-0.5.1/src/age/primitives/rsa_oaep.py
+-rw-r--r--   0 runner    (1001) docker     (123)      533 2023-05-06 13:08:10.000000 age-0.5.1/src/age/primitives/scrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2001 2023-05-06 13:08:10.000000 age-0.5.1/src/age/primitives/x25519.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 13:08:21.553603 age-0.5.1/src/age/recipients/
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-05-06 13:08:10.000000 age-0.5.1/src/age/recipients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-06 13:08:10.000000 age-0.5.1/src/age/recipients/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-05-06 13:08:10.000000 age-0.5.1/src/age/recipients/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-05-06 13:08:10.000000 age-0.5.1/src/age/recipients/scrypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1795 2023-05-06 13:08:10.000000 age-0.5.1/src/age/recipients/ssh_ed25519.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-06 13:08:10.000000 age-0.5.1/src/age/recipients/ssh_rsa.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1493 2023-05-06 13:08:10.000000 age-0.5.1/src/age/recipients/x25519.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-05-06 13:08:10.000000 age-0.5.1/src/age/stream.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 13:08:21.557603 age-0.5.1/src/age/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 13:08:10.000000 age-0.5.1/src/age/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5016 2023-05-06 13:08:10.000000 age-0.5.1/src/age/utils/asciiarmor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-06 13:08:10.000000 age-0.5.1/src/age/utils/copy_doc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-06 13:08:10.000000 age-0.5.1/src/age/utils/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 13:08:21.549603 age-0.5.1/src/age.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3140 2023-05-06 13:08:21.000000 age-0.5.1/src/age.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-05-06 13:08:21.000000 age-0.5.1/src/age.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 13:08:21.000000 age-0.5.1/src/age.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-06 13:08:21.000000 age-0.5.1/src/age.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-06 13:08:21.000000 age-0.5.1/src/age.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-06 13:08:21.000000 age-0.5.1/src/age.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    68611 2023-05-06 13:08:10.000000 age-0.5.1/versioneer.py
```

### Comparing `age-0.4.1/LICENSE` & `age-0.5.1/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright 2019-2020 Jonas Lieb
+Copyright 2019-2023 Jonas Lieb
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
 use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
 the Software, and to permit persons to whom the Software is furnished to do so,
 subject to the following conditions:
```

### Comparing `age-0.4.1/PKG-INFO` & `age-0.5.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,71 +1,75 @@
 Metadata-Version: 2.1
 Name: age
-Version: 0.4.1
+Version: 0.5.1
 Summary: Actually good encryption. In Python.
 Home-page: https://github.com/jojonas/pyage
 Author: Jonas Lieb
 License: MIT
 Project-URL: Repository, https://github.com/jojonas/pyage
 Project-URL: Documentation, https://pyage.readthedocs.io/
 Project-URL: Specification, https://age-encryption.org/
-Description: # pyage
-        
-        [![Build and Test](https://github.com/jojonas/pyage/workflows/Build%20and%20Test/badge.svg)](https://github.com/jojonas/pyage/actions?workflow=Build+and+Test)
-        [![Compatibility Check](https://github.com/jojonas/pyage/workflows/Compatibility%20with%20FiloSottile/age/badge.svg)](https://github.com/jojonas/pyage/actions?workflow=Compatibility%20with%20FiloSottile/age)
-        [![Documentation Status](https://readthedocs.org/projects/pyage/badge/?version=latest)](https://pyage.readthedocs.io/en/latest/?badge=latest)
-        ![License](https://img.shields.io/github/license/jojonas/pyage)
-        
-        ![pyage screenshot](https://raw.githubusercontent.com/jojonas/pyage/master/docs/source/_static/carbon.png)
-        
-        pyage is an experimental implementation of @FiloSottile and @Benjojo12 's project "age".
-        The spec is currently available as seven-page Google doc at [age-encryption.org/v1](https://age-encryption.org/v1).
-        
-        This project is still work-in-progress.
-        
-        ⚠️ pyage is not intended to be a secure age implementation!
-        My original intention was to better understand the spec, find mistakes early and provide a redundant implementation for validation. I'm not a cryptographer (IANAC) and did not (yet) find the time to address  implementation-specific security issues (such as DoS attacks or side-channel attacks).
-        
-        So:
-        *Use at your own risk.*
-        
-        ## Quick Start
-        Install from pip:
-        
-            pip install age
-        
-        Generate a key pair:
-        
-            mkdir -p ~/.config/age
-            pyage generate > ~/.config/age/keys.txt
-        
-        Encrypt a file:
-        
-            pyage encrypt -i hello.txt -o hello.age pubkey:<recipient public key>
-        
-        Decrypt a file (uses `~/.config/age/keys.txt`):
-        
-            pyage decrypt -i hello.age
-        
-        For a real tutorial, see [the Tutorial section in the documentation](https://pyage.readthedocs.io/en/latest/tutorials.html).
-        
-        ## Documentation
-        The full documentation can be found at [pyage.readthedocs.io](https://pyage.readthedocs.io/en/latest/index.html).
 Keywords: age encryption privacy experimental
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: Console
 Classifier: Topic :: Security :: Cryptography
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: <4,>=3.6
 Description-Content-Type: text/markdown; charset=UTF-8
 Provides-Extra: dev
 Provides-Extra: test
 Provides-Extra: docs
+License-File: LICENSE
+
+# pyage
+
+[![Build and Test](https://github.com/jojonas/pyage/workflows/Build%20and%20Test/badge.svg)](https://github.com/jojonas/pyage/actions?workflow=Build+and+Test)
+[![Compatibility Check](https://github.com/jojonas/pyage/workflows/Compatibility%20with%20FiloSottile/age/badge.svg)](https://github.com/jojonas/pyage/actions?workflow=Compatibility%20with%20FiloSottile/age)
+[![Documentation Status](https://readthedocs.org/projects/pyage/badge/?version=latest)](https://pyage.readthedocs.io/en/latest/?badge=latest)
+![License](https://img.shields.io/github/license/jojonas/pyage)
+
+![pyage screenshot](https://raw.githubusercontent.com/jojonas/pyage/master/docs/source/_static/carbon.png)
+
+pyage is an experimental implementation of @FiloSottile and @Benjojo12 's project "age".
+The spec is currently available as seven-page Google doc at [age-encryption.org/v1](https://age-encryption.org/v1).
+
+This project is still work-in-progress.
+
+⚠️ pyage is not intended to be a secure age implementation!
+My original intention was to better understand the spec, find mistakes early and provide a redundant implementation for validation. I'm not a cryptographer (IANAC) and did not (yet) find the time to address  implementation-specific security issues (such as DoS attacks or side-channel attacks).
+
+So:
+*Use at your own risk.*
+
+## Quick Start
+Install from pip:
+
+    pip install age
+
+Generate a key pair:
+
+    mkdir -p ~/.config/age
+    pyage generate > ~/.config/age/keys.txt
+
+Encrypt a file:
+
+    pyage encrypt -i hello.txt -o hello.age pubkey:<recipient public key>
+
+Decrypt a file (uses `~/.config/age/keys.txt`):
+
+    pyage decrypt -i hello.age
+
+For a real tutorial, see [the Tutorial section in the documentation](https://pyage.readthedocs.io/en/latest/tutorials.html).
+
+## Documentation
+The full documentation can be found at [pyage.readthedocs.io](https://pyage.readthedocs.io/en/latest/index.html).
```

### Comparing `age-0.4.1/README.md` & `age-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `age-0.4.1/setup.cfg` & `age-0.5.1/setup.cfg`

 * *Files 16% similar despite different names*

```diff
@@ -20,17 +20,19 @@
 	Intended Audience :: Science/Research
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Environment :: Console
 	Topic :: Security :: Cryptography
 	Programming Language :: Python
 	Programming Language :: Python :: 3 :: Only
-	Programming Language :: Python :: 3.6
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
+	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 
 [options]
 package_dir = 
 	=src
 packages = find:
 install_requires = 
 	setuptools>=38.3
@@ -49,14 +51,15 @@
 [options.extras_require]
 dev = 
 	black
 	flake8
 	mypy
 	isort
 	versioneer
+	types-requests
 test = 
 	pytest
 	pyfakefs
 	coverage
 	pytest-cov
 docs = 
 	sphinx
@@ -93,15 +96,15 @@
 line_length = 100
 multi_line_output = 3
 include_trailing_comma = True
 use_parentheses = True
 skip = versioneer.py,src/age/__init__.py,src/age/version.py
 
 [versioneer]
-vcs = git
+VCS = git
 style = pep440
 versionfile_source = src/age/_version.py
 versionfile_build = age/_version.py
 tag_prefix = v
 parentdir_prefix = age-
 
 [tool:pytest]
```

### Comparing `age-0.4.1/setup.py` & `age-0.5.1/setup.py`

 * *Files identical despite different names*

### Comparing `age-0.4.1/src/age/algorithms/scrypt.py` & `age-0.5.1/src/age/algorithms/scrypt.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,21 +8,18 @@
 __all__ = ["scrypt_encrypt_file_key", "scrypt_decrypt_file_key"]
 
 MAX_LOG_COST = 22
 AGE_SCRYPT_LABEL = b"age-encryption.org/v1/scrypt"
 
 
 def scrypt_encrypt_file_key(
-    password: PasswordKey, file_key: bytes, log_cost: int = None
+    password: PasswordKey, file_key: bytes, log_cost: int = 18
 ) -> typing.Tuple[bytes, int, bytes]:
     # https://blog.filippo.io/the-scrypt-parameters/
 
-    if log_cost is None:
-        log_cost = 18  # about 1 second
-
     if not (0 <= log_cost <= MAX_LOG_COST):
         raise ValueError("Invalid scrypt cost")
 
     salt = random(16)
     cost = 1 << log_cost
 
     key = scrypt(AGE_SCRYPT_LABEL + salt, cost, password.value)
```

### Comparing `age-0.4.1/src/age/algorithms/ssh_ed25519.py` & `age-0.5.1/src/age/algorithms/ssh_ed25519.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 def _tweak(ssh_key: bytes) -> ECScalar:
     return x25519_reduce(ECScalar(hkdf(salt=ssh_key, label=AGE_ED25519_LABEL, key=b"", len=64)))
 
 
 def ssh_ed25519_encrypt_file_key(
     ed25519_public_key: Ed25519PublicKey, file_key: bytes
 ) -> typing.Tuple[bytes, ECPoint, bytes]:
-
     ssh_key = ed25519_public_key.binary_encoding()
     public_key_fingerprint = sha256(ssh_key)[:4]
 
     age_public_key = ed25519_public_key.to_age_public_key()
 
     pk_conv: ECPoint = age_public_key.public_bytes()
     pk_conv_tweak: ECPoint = x25519_scalarmult(_tweak(ssh_key), pk_conv)
```

### Comparing `age-0.4.1/src/age/algorithms/ssh_rsa.py` & `age-0.5.1/src/age/algorithms/ssh_rsa.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 
 AGE_RSA_PADDING_LABEL = b"age-encryption.org/v1/ssh-rsa"
 
 
 def ssh_rsa_encrypt_file_key(
     public_key: RSAPublicKey, file_key: bytes
 ) -> typing.Tuple[bytes, bytes]:
-
     public_key_fingerprint = sha256(public_key.binary_encoding())[:4]
     encrypted_file_key = rsa_encrypt(
         public_key=public_key, label=AGE_RSA_PADDING_LABEL, plaintext=file_key
     )
 
     return public_key_fingerprint, encrypted_file_key
```

### Comparing `age-0.4.1/src/age/algorithms/x25519.py` & `age-0.5.1/src/age/algorithms/x25519.py`

 * *Files identical despite different names*

### Comparing `age-0.4.1/src/age/cli.py` & `age-0.5.1/src/age/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,17 +16,17 @@
 from age.keys.base import DecryptionKey
 from age.keys.password import PasswordKey
 from age.utils.asciiarmor import AGE_PEM_LABEL, AsciiArmoredInput, AsciiArmoredOutput
 from age.utils.copy_doc import copy_doc
 
 
 def encrypt(
-    recipients: typing.List[str] = None,
-    infile: typing.BinaryIO = None,
-    outfile: typing.BinaryIO = None,
+    recipients: typing.Optional[typing.List[str]] = None,
+    infile: typing.Optional[typing.BinaryIO] = None,
+    outfile: typing.Optional[typing.BinaryIO] = None,
     ask_password: bool = False,
     ascii_armored: bool = False,
 ) -> None:
     """Encrypt data for the given recipients.
 
     \b
     RECIPIENTS can be a list of either:
@@ -46,19 +46,19 @@
 
     Note that in this case, anyone in possession of the password can tamper
     with the message, therefore it is recommended to not mix password- and
     public key recipients.
 
     """
 
-    if not infile:
+    if infile is None:
         infile = sys.stdin.buffer
-    if not outfile:
+    if outfile is None:
         outfile = sys.stdout.buffer
-    if not recipients:
+    if recipients is None:
         recipients = []
 
     if outfile is sys.stdout.buffer and sys.stdout.isatty():
         print("Refusing to encrypt to a TTY.", file=sys.stderr)
         sys.exit(1)
 
     aliases = load_aliases()
@@ -87,18 +87,18 @@
         outfile = AsciiArmoredOutput(AGE_PEM_LABEL, outfile)  # type: ignore
 
     with Encryptor(keys, outfile) as encryptor:
         encryptor.write(infile.read())
 
 
 def decrypt(
-    infile: typing.BinaryIO = None,
-    outfile: typing.BinaryIO = None,
+    infile: typing.Optional[typing.BinaryIO] = None,
+    outfile: typing.Optional[typing.BinaryIO] = None,
     ask_password: bool = False,
-    keyfiles: typing.List[str] = None,
+    keyfiles: typing.Optional[typing.List[str]] = None,
     ascii_armored: bool = False,
 ) -> None:
     """Decrypt a file encrypted with 'age encrypt'.
 
     Ciphertext can be passed from the standard input stream and from a file.
     Plaintext will by default be written to the standard output stream, but
     a filename can be specified.
@@ -109,19 +109,19 @@
     - Private SSH keys at ~/.ssh/id_*
     - Age private keys in files passed via KEYFILES.
 
     If the '-p' switch is provided, age will prompt for a password and also
     attempt to decrypt the message with the given password.
     """
 
-    if not infile:
+    if infile is None:
         infile = sys.stdin.buffer
-    if not outfile:
+    if outfile is None:
         outfile = sys.stdout.buffer
-    if not keyfiles:
+    if keyfiles is None:
         keyfiles = []
 
     keys: typing.List[DecryptionKey] = []
     keys.extend(load_keys_txt())
     keys.extend(load_ssh_keys())
     for keyfile in keyfiles:
         keys.extend(load_keys_txt(keyfile))
@@ -138,15 +138,15 @@
         # ignoring mypy error because RawIOBase satisfies BinaryIO (doesn't it?)
         infile = AsciiArmoredInput(AGE_PEM_LABEL, infile)  # type: ignore
 
     with Decryptor(keys, infile) as decryptor:
         outfile.write(decryptor.read())
 
 
-def generate(outfile: typing.TextIO = None) -> None:
+def generate(outfile: typing.Optional[typing.TextIO] = None) -> None:
     """Generate a new age private/public key pair.
 
     If no FILENAME is given, the command outputs the key pair to the standard output stream.
 
     If FILENAME exists, age will warn if the file permissions allow others to read, write or
     execute the file.
     """
```

### Comparing `age-0.4.1/src/age/file.py` & `age-0.5.1/src/age/file.py`

 * *Files identical despite different names*

### Comparing `age-0.4.1/src/age/format.py` & `age-0.5.1/src/age/format.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,25 +4,27 @@
 from age.exceptions import ParserError
 from age.primitives.encode import decode, encode
 
 __all__ = ["Recipient", "Header", "load_header", "dump_header"]
 
 
 class Recipient:
-    def __init__(self, type: str = "", arguments: typing.List[str] = None, body: str = ""):
+    def __init__(
+        self, type: str = "", arguments: typing.Optional[typing.List[str]] = None, body: str = ""
+    ):
         if arguments is None:
             arguments = []
 
         self.type: str = type
         self.arguments: typing.List[str] = arguments
         self.body: str = body
 
 
 class Header:
-    def __init__(self, recipients: typing.List[Recipient] = None):
+    def __init__(self, recipients: typing.Optional[typing.List[Recipient]] = None):
         if recipients is None:
             recipients = []
 
         self.recipients: typing.List[Recipient] = recipients
 
 
 AGE_INTRO = "age-encryption.org/v1"
@@ -35,14 +37,15 @@
     first_line = stream.readline().strip()
 
     if first_line.decode("utf-8", "replace") != AGE_INTRO:
         raise ParserError("File signature not found.")
 
     header = Header()
 
+    line = ""
     for raw_line in stream:
         line = raw_line.decode("utf-8")
 
         if line.startswith(RECIPIENT_PREFIX):
             type, *args = line[len(RECIPIENT_PREFIX) :].split()
             header.recipients.append(Recipient(type, args))
         elif line.startswith(FOOTER_PREFIX):
@@ -54,15 +57,15 @@
     prefix, encoded_mac = line.split()
     assert prefix == FOOTER_PREFIX
     mac = decode(encoded_mac)
 
     return header, mac
 
 
-def dump_header(header: Header, stream: typing.BinaryIO, mac: bytes = None):
+def dump_header(header: Header, stream: typing.BinaryIO, mac: typing.Optional[bytes] = None):
     stream.write(AGE_INTRO.encode("utf-8") + b"\n")
 
     for recipient in header.recipients:
         line = RECIPIENT_PREFIX + " " + recipient.type + " " + " ".join(recipient.arguments) + "\n"
         stream.write(line.encode("utf-8"))
         if recipient.body:
             wrapped = textwrap.fill(recipient.body, break_on_hyphens=False, width=64)
```

### Comparing `age-0.4.1/src/age/keyloader.py` & `age-0.5.1/src/age/keyloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,15 +96,19 @@
                 public_keys = values.split()
                 aliases[label].extend(public_keys)
 
     return dict(aliases)
 
 
 def resolve_public_key(
-    keystr: str, aliases: AliasDict = None, read_aliases=True, read_files=True, read_urls=True
+    keystr: str,
+    aliases: typing.Optional[AliasDict] = None,
+    read_aliases=True,
+    read_files=True,
+    read_urls=True,
 ) -> typing.List[EncryptionKey]:
     # none of the key types like leading/trailing whitespace
     keystr = keystr.strip()
 
     # First: resolve aliases
     if read_aliases and aliases is not None and keystr in aliases:
         resolved_from_alias: typing.List[EncryptionKey] = []
```

### Comparing `age-0.4.1/src/age/keys/agekey.py` & `age-0.5.1/src/age/keys/agekey.py`

 * *Files identical despite different names*

### Comparing `age-0.4.1/src/age/keys/ed25519.py` & `age-0.5.1/src/age/keys/ed25519.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import base64
 import hashlib
+import typing
 
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives.asymmetric.ed25519 import (
     Ed25519PrivateKey as Ed25519PrivateKey_,
 )
 from cryptography.hazmat.primitives.asymmetric.ed25519 import Ed25519PublicKey as Ed25519PublicKey_
 from cryptography.hazmat.primitives.asymmetric.x25519 import X25519PrivateKey, X25519PublicKey
@@ -39,15 +40,15 @@
         return f"<{clsname} {self.public_key().fingerprint()}>"
 
     @classmethod
     def generate(cls):
         return cls(Ed25519PrivateKey_.generate())
 
     @classmethod
-    def from_pem(cls, pem_data: bytes, password: bytes = None):
+    def from_pem(cls, pem_data: bytes, password: typing.Optional[bytes] = None):
         try:
             private_key = load_pem_private_key(
                 pem_data, password=password, backend=default_backend()
             )
         except ValueError:
             # OpenSSH private keys are special snowflakes
             private_key = load_openssh_private_key(pem_data, passphrase=password)
```

### Comparing `age-0.4.1/src/age/keys/rsa.py` & `age-0.5.1/src/age/keys/rsa.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import base64
 import hashlib
+import typing
 
 from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives.asymmetric.rsa import RSAPrivateKey as RSAPrivateKey_
 from cryptography.hazmat.primitives.asymmetric.rsa import RSAPublicKey as RSAPublicKey_
 from cryptography.hazmat.primitives.asymmetric.rsa import generate_private_key
 from cryptography.hazmat.primitives.serialization import (
     Encoding,
@@ -36,15 +37,15 @@
     def generate(cls, key_size: int = 4096):
         generated_key = generate_private_key(
             RSA_DEFAULT_PUBLIC_EXPONENT, key_size, backend=default_backend()
         )
         return cls(generated_key)
 
     @classmethod
-    def from_pem(cls, pem_data: bytes, password: bytes = None):
+    def from_pem(cls, pem_data: bytes, password: typing.Optional[bytes] = None):
         try:
             private_key = load_pem_private_key(
                 pem_data, password=password, backend=default_backend()
             )
         except ValueError:
             # OpenSSH private keys are special snowflakes
             private_key = load_openssh_private_key(pem_data, passphrase=password)
```

### Comparing `age-0.4.1/src/age/openssh_keys.py` & `age-0.5.1/src/age/openssh_keys.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,20 +128,19 @@
     assert len(private_key_bytes) == 64
     assert private_key_bytes[32:] == public_key_bytes
     return ed25519.Ed25519PrivateKey.from_private_bytes(private_key_bytes[:32])
 
 
 def _decrypt_key(
     encrypted: bytes,
-    passphrase: bytes = None,
+    passphrase: typing.Optional[bytes] = None,
     ciphername: bytes = b"none",
     kdfname: bytes = b"none",
     kdf_metadata: bytes = b"",
 ) -> bytes:
-
     if ciphername == b"none":
         return encrypted
 
     if not passphrase:
         raise WrongPassphrase("Passphrase needed for decryption")
 
     if kdfname == b"none":
@@ -178,15 +177,17 @@
     cipher = Cipher(algorithm=suite.algorithm(key), mode=suite.mode(iv), backend=default_backend())
     decryptor = cipher.decryptor()
     decrypted = decryptor.update(encrypted) + decryptor.finalize()
 
     return decrypted
 
 
-def load_openssh_private_key(openssh_data: bytes, passphrase: bytes = None) -> AnyPrivateKey:
+def load_openssh_private_key(
+    openssh_data: bytes, passphrase: typing.Optional[bytes] = None
+) -> AnyPrivateKey:
     """Load OpenSSH key in ""PEM"" format.
 
     The files look like PEM, but aren't. OpenSSH keys are "proprietary" and
     can be identified by the line "-----BEGIN OPENSSH PRIVATE KEY-----".
     """
 
     # Format documentation:
```

### Comparing `age-0.4.1/src/age/primitives/__init__.py` & `age-0.5.1/src/age/primitives/__init__.py`

 * *Files identical despite different names*

### Comparing `age-0.4.1/src/age/primitives/bech32.py` & `age-0.5.1/src/age/primitives/bech32.py`

 * *Files identical despite different names*

### Comparing `age-0.4.1/src/age/primitives/encode.py` & `age-0.5.1/src/age/primitives/encode.py`

 * *Files identical despite different names*

### Comparing `age-0.4.1/src/age/primitives/encrypt.py` & `age-0.5.1/src/age/primitives/encrypt.py`

 * *Files identical despite different names*

### Comparing `age-0.4.1/src/age/primitives/hkdf.py` & `age-0.5.1/src/age/primitives/hkdf.py`

 * *Files identical despite different names*

### Comparing `age-0.4.1/src/age/primitives/hmac.py` & `age-0.5.1/src/age/primitives/hmac.py`

 * *Files identical despite different names*

### Comparing `age-0.4.1/src/age/primitives/rsa_oaep.py` & `age-0.5.1/src/age/primitives/rsa_oaep.py`

 * *Files identical despite different names*

### Comparing `age-0.4.1/src/age/primitives/scrypt.py` & `age-0.5.1/src/age/primitives/scrypt.py`

 * *Files identical despite different names*

### Comparing `age-0.4.1/src/age/primitives/x25519.py` & `age-0.5.1/src/age/primitives/x25519.py`

 * *Files identical despite different names*

### Comparing `age-0.4.1/src/age/recipients/base.py` & `age-0.5.1/src/age/recipients/base.py`

 * *Files identical despite different names*

### Comparing `age-0.4.1/src/age/recipients/helpers.py` & `age-0.5.1/src/age/recipients/helpers.py`

 * *Files identical despite different names*

### Comparing `age-0.4.1/src/age/recipients/scrypt.py` & `age-0.5.1/src/age/recipients/scrypt.py`

 * *Files identical despite different names*

### Comparing `age-0.4.1/src/age/recipients/ssh_ed25519.py` & `age-0.5.1/src/age/recipients/ssh_ed25519.py`

 * *Files identical despite different names*

### Comparing `age-0.4.1/src/age/recipients/ssh_rsa.py` & `age-0.5.1/src/age/recipients/ssh_rsa.py`

 * *Files identical despite different names*

### Comparing `age-0.4.1/src/age/recipients/x25519.py` & `age-0.5.1/src/age/recipients/x25519.py`

 * *Files identical despite different names*

### Comparing `age-0.4.1/src/age/stream.py` & `age-0.5.1/src/age/stream.py`

 * *Files identical despite different names*

### Comparing `age-0.4.1/src/age/utils/asciiarmor.py` & `age-0.5.1/src/age/utils/asciiarmor.py`

 * *Files 10% similar despite different names*

```diff
@@ -76,15 +76,15 @@
     for i in range(0, len(encoded), 64):
         chunk = encoded[i : i + 64]
         file.write(chunk)
         file.write("\n")
     file.write(f"-----END {label}-----\n")
 
 
-class AsciiArmoredOutput(io.RawIOBase):
+class AsciiArmoredOutput(io.RawIOBase, typing.BinaryIO):
     def __init__(self, label: str, stream: typing.BinaryIO):
         self._stream: typing.BinaryIO = stream
         self._text_stream: typing.TextIO = io.TextIOWrapper(stream, "utf-8")
         self._plaintext_buffer: bytes = b""
         self._label: str = label
 
     def writable(self):
@@ -95,20 +95,32 @@
         return len(data)
 
     def close(self):
         if not self.closed:
             self._encode_buffer()
             super().close()
 
+    def read(self, n):
+        # Needed to implement typing.BinaryIO
+        raise NotImplementedError()
+
+    def writelines(self, lines):
+        # Needed to implement typing.BinaryIO
+        raise NotImplementedError()
+
+    def __enter__(self):
+        # Needed to implement typing.BinaryIO
+        raise NotImplementedError()
+
     def _encode_buffer(self):
         write_ascii_armored(self._text_stream, self._label, self._plaintext_buffer)
         self._plaintext_buffer = b""
 
 
-class AsciiArmoredInput(io.RawIOBase):
+class AsciiArmoredInput(io.RawIOBase, typing.BinaryIO):
     def __init__(self, label: str, stream: typing.BinaryIO):
         self._stream: typing.BinaryIO = stream
         self._text_stream: typing.TextIO = io.TextIOWrapper(stream, "utf-8")
         self._plaintext_stream: typing.Optional[typing.BinaryIO] = None
         self._label: str = label
 
         self._decode_body()
@@ -116,18 +128,32 @@
     def readable(self):
         return True
 
     def read(self, size=-1):
         assert self._plaintext_stream is not None
         return self._plaintext_stream.read(size)
 
+    def write(self, data):
+        # Needed to implement typing.BinaryIO
+        raise NotImplementedError()
+
+    def writelines(self, lines):
+        # Needed to implement typing.BinaryIO
+        raise NotImplementedError()
+
+    def __enter__(self):
+        # Needed to implement typing.BinaryIO
+        raise NotImplementedError()
+
     def _decode_body(self):
         count = 0
 
-        data = None
+        data = b""
+        label = ""
+
         for label, decoded in read_ascii_armored(self._text_stream):
             if label == self._label:
                 data = decoded
                 count += 1
 
         if count == 0:
             raise ValueError(f"label {label} not found")
```

### Comparing `age-0.4.1/src/age.egg-info/PKG-INFO` & `age-0.5.1/src/age.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,71 +1,75 @@
 Metadata-Version: 2.1
 Name: age
-Version: 0.4.1
+Version: 0.5.1
 Summary: Actually good encryption. In Python.
 Home-page: https://github.com/jojonas/pyage
 Author: Jonas Lieb
 License: MIT
 Project-URL: Repository, https://github.com/jojonas/pyage
 Project-URL: Documentation, https://pyage.readthedocs.io/
 Project-URL: Specification, https://age-encryption.org/
-Description: # pyage
-        
-        [![Build and Test](https://github.com/jojonas/pyage/workflows/Build%20and%20Test/badge.svg)](https://github.com/jojonas/pyage/actions?workflow=Build+and+Test)
-        [![Compatibility Check](https://github.com/jojonas/pyage/workflows/Compatibility%20with%20FiloSottile/age/badge.svg)](https://github.com/jojonas/pyage/actions?workflow=Compatibility%20with%20FiloSottile/age)
-        [![Documentation Status](https://readthedocs.org/projects/pyage/badge/?version=latest)](https://pyage.readthedocs.io/en/latest/?badge=latest)
-        ![License](https://img.shields.io/github/license/jojonas/pyage)
-        
-        ![pyage screenshot](https://raw.githubusercontent.com/jojonas/pyage/master/docs/source/_static/carbon.png)
-        
-        pyage is an experimental implementation of @FiloSottile and @Benjojo12 's project "age".
-        The spec is currently available as seven-page Google doc at [age-encryption.org/v1](https://age-encryption.org/v1).
-        
-        This project is still work-in-progress.
-        
-        ⚠️ pyage is not intended to be a secure age implementation!
-        My original intention was to better understand the spec, find mistakes early and provide a redundant implementation for validation. I'm not a cryptographer (IANAC) and did not (yet) find the time to address  implementation-specific security issues (such as DoS attacks or side-channel attacks).
-        
-        So:
-        *Use at your own risk.*
-        
-        ## Quick Start
-        Install from pip:
-        
-            pip install age
-        
-        Generate a key pair:
-        
-            mkdir -p ~/.config/age
-            pyage generate > ~/.config/age/keys.txt
-        
-        Encrypt a file:
-        
-            pyage encrypt -i hello.txt -o hello.age pubkey:<recipient public key>
-        
-        Decrypt a file (uses `~/.config/age/keys.txt`):
-        
-            pyage decrypt -i hello.age
-        
-        For a real tutorial, see [the Tutorial section in the documentation](https://pyage.readthedocs.io/en/latest/tutorials.html).
-        
-        ## Documentation
-        The full documentation can be found at [pyage.readthedocs.io](https://pyage.readthedocs.io/en/latest/index.html).
 Keywords: age encryption privacy experimental
 Platform: any
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Environment :: Console
 Classifier: Topic :: Security :: Cryptography
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: <4,>=3.6
 Description-Content-Type: text/markdown; charset=UTF-8
 Provides-Extra: dev
 Provides-Extra: test
 Provides-Extra: docs
+License-File: LICENSE
+
+# pyage
+
+[![Build and Test](https://github.com/jojonas/pyage/workflows/Build%20and%20Test/badge.svg)](https://github.com/jojonas/pyage/actions?workflow=Build+and+Test)
+[![Compatibility Check](https://github.com/jojonas/pyage/workflows/Compatibility%20with%20FiloSottile/age/badge.svg)](https://github.com/jojonas/pyage/actions?workflow=Compatibility%20with%20FiloSottile/age)
+[![Documentation Status](https://readthedocs.org/projects/pyage/badge/?version=latest)](https://pyage.readthedocs.io/en/latest/?badge=latest)
+![License](https://img.shields.io/github/license/jojonas/pyage)
+
+![pyage screenshot](https://raw.githubusercontent.com/jojonas/pyage/master/docs/source/_static/carbon.png)
+
+pyage is an experimental implementation of @FiloSottile and @Benjojo12 's project "age".
+The spec is currently available as seven-page Google doc at [age-encryption.org/v1](https://age-encryption.org/v1).
+
+This project is still work-in-progress.
+
+⚠️ pyage is not intended to be a secure age implementation!
+My original intention was to better understand the spec, find mistakes early and provide a redundant implementation for validation. I'm not a cryptographer (IANAC) and did not (yet) find the time to address  implementation-specific security issues (such as DoS attacks or side-channel attacks).
+
+So:
+*Use at your own risk.*
+
+## Quick Start
+Install from pip:
+
+    pip install age
+
+Generate a key pair:
+
+    mkdir -p ~/.config/age
+    pyage generate > ~/.config/age/keys.txt
+
+Encrypt a file:
+
+    pyage encrypt -i hello.txt -o hello.age pubkey:<recipient public key>
+
+Decrypt a file (uses `~/.config/age/keys.txt`):
+
+    pyage decrypt -i hello.age
+
+For a real tutorial, see [the Tutorial section in the documentation](https://pyage.readthedocs.io/en/latest/tutorials.html).
+
+## Documentation
+The full documentation can be found at [pyage.readthedocs.io](https://pyage.readthedocs.io/en/latest/index.html).
```

### Comparing `age-0.4.1/src/age.egg-info/SOURCES.txt` & `age-0.5.1/src/age.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `age-0.4.1/versioneer.py` & `age-0.5.1/versioneer.py`

 * *Files identical despite different names*

