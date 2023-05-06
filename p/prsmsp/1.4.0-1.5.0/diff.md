# Comparing `tmp/prsmsp-1.4.0.tar.gz` & `tmp/prsmsp-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prsmsp-1.4.0.tar", last modified: Fri Apr 14 09:28:58 2023, max compression
+gzip compressed data, was "prsmsp-1.5.0.tar", last modified: Sat May  6 18:52:46 2023, max compression
```

## Comparing `prsmsp-1.4.0.tar` & `prsmsp-1.5.0.tar`

### file list

```diff
@@ -1,41 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:28:58.336466 prsmsp-1.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-04-14 09:28:58.336466 prsmsp-1.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-04-14 09:28:47.000000 prsmsp-1.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:28:58.332466 prsmsp-1.4.0/prsmsp/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-14 09:28:47.000000 prsmsp-1.4.0/prsmsp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:28:58.336466 prsmsp-1.4.0/prsmsp/abstracts/
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-04-14 09:28:47.000000 prsmsp-1.4.0/prsmsp/abstracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-14 09:28:47.000000 prsmsp-1.4.0/prsmsp/abstracts/abcpanel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:28:58.336466 prsmsp-1.4.0/prsmsp/exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:28:47.000000 prsmsp-1.4.0/prsmsp/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:28:47.000000 prsmsp-1.4.0/prsmsp/exceptions/abstracts.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-14 09:28:47.000000 prsmsp-1.4.0/prsmsp/exceptions/models.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:28:47.000000 prsmsp-1.4.0/prsmsp/exceptions/panels.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:28:58.336466 prsmsp-1.4.0/prsmsp/factories/
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-04-14 09:28:47.000000 prsmsp-1.4.0/prsmsp/factories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      739 2023-04-14 09:28:47.000000 prsmsp-1.4.0/prsmsp/factories/auth_factory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:28:58.336466 prsmsp-1.4.0/prsmsp/models/
--rw-r--r--   0 runner    (1001) docker     (123)       75 2023-04-14 09:28:47.000000 prsmsp-1.4.0/prsmsp/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-14 09:28:47.000000 prsmsp-1.4.0/prsmsp/models/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-04-14 09:28:47.000000 prsmsp-1.4.0/prsmsp/models/response.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:28:58.336466 prsmsp-1.4.0/prsmsp/panels/
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-14 09:28:47.000000 prsmsp-1.4.0/prsmsp/panels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-04-14 09:28:47.000000 prsmsp-1.4.0/prsmsp/panels/farazsms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-04-14 09:28:47.000000 prsmsp-1.4.0/prsmsp/panels/ghasedaksms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-04-14 09:28:47.000000 prsmsp-1.4.0/prsmsp/panels/kavenegar.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-04-14 09:28:47.000000 prsmsp-1.4.0/prsmsp/panels/mediana.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-04-14 09:28:47.000000 prsmsp-1.4.0/prsmsp/panels/melipayamak.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-04-14 09:28:47.000000 prsmsp-1.4.0/prsmsp/panels/niksms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-04-14 09:28:47.000000 prsmsp-1.4.0/prsmsp/panels/smsdotir.py
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-04-14 09:28:47.000000 prsmsp-1.4.0/prsmsp/panels/webonesms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:28:58.336466 prsmsp-1.4.0/prsmsp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2177 2023-04-14 09:28:58.000000 prsmsp-1.4.0/prsmsp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-04-14 09:28:58.000000 prsmsp-1.4.0/prsmsp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 09:28:58.000000 prsmsp-1.4.0/prsmsp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 09:28:58.000000 prsmsp-1.4.0/prsmsp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-14 09:28:58.000000 prsmsp-1.4.0/prsmsp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-14 09:28:58.000000 prsmsp-1.4.0/prsmsp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-14 09:28:58.336466 prsmsp-1.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-04-14 09:28:47.000000 prsmsp-1.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 09:28:58.336466 prsmsp-1.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 09:28:47.000000 prsmsp-1.4.0/tests/test_app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:52:46.213863 prsmsp-1.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-05-06 18:52:46.213863 prsmsp-1.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2484 2023-05-06 18:52:35.000000 prsmsp-1.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:52:46.209863 prsmsp-1.5.0/prsmsp/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-06 18:52:35.000000 prsmsp-1.5.0/prsmsp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:52:46.209863 prsmsp-1.5.0/prsmsp/abstracts/
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-06 18:52:35.000000 prsmsp-1.5.0/prsmsp/abstracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-06 18:52:35.000000 prsmsp-1.5.0/prsmsp/abstracts/abcpanel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:52:46.209863 prsmsp-1.5.0/prsmsp/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 18:52:35.000000 prsmsp-1.5.0/prsmsp/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 18:52:35.000000 prsmsp-1.5.0/prsmsp/exceptions/abstracts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-06 18:52:35.000000 prsmsp-1.5.0/prsmsp/exceptions/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 18:52:35.000000 prsmsp-1.5.0/prsmsp/exceptions/panels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:52:46.209863 prsmsp-1.5.0/prsmsp/factories/
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-06 18:52:35.000000 prsmsp-1.5.0/prsmsp/factories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      739 2023-05-06 18:52:35.000000 prsmsp-1.5.0/prsmsp/factories/auth_factory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:52:46.209863 prsmsp-1.5.0/prsmsp/models/
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-06 18:52:35.000000 prsmsp-1.5.0/prsmsp/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-06 18:52:35.000000 prsmsp-1.5.0/prsmsp/models/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-06 18:52:35.000000 prsmsp-1.5.0/prsmsp/models/response.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:52:46.209863 prsmsp-1.5.0/prsmsp/panels/
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-06 18:52:35.000000 prsmsp-1.5.0/prsmsp/panels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-05-06 18:52:35.000000 prsmsp-1.5.0/prsmsp/panels/farazsms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1653 2023-05-06 18:52:35.000000 prsmsp-1.5.0/prsmsp/panels/ghasedaksms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 2023-05-06 18:52:35.000000 prsmsp-1.5.0/prsmsp/panels/kavenegar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-05-06 18:52:35.000000 prsmsp-1.5.0/prsmsp/panels/mediana.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-05-06 18:52:35.000000 prsmsp-1.5.0/prsmsp/panels/melipayamak.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-05-06 18:52:35.000000 prsmsp-1.5.0/prsmsp/panels/niksms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1731 2023-05-06 18:52:35.000000 prsmsp-1.5.0/prsmsp/panels/smsdotir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1573 2023-05-06 18:52:35.000000 prsmsp-1.5.0/prsmsp/panels/smsone.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-05-06 18:52:35.000000 prsmsp-1.5.0/prsmsp/panels/webonesms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:52:46.209863 prsmsp-1.5.0/prsmsp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-05-06 18:52:46.000000 prsmsp-1.5.0/prsmsp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      817 2023-05-06 18:52:46.000000 prsmsp-1.5.0/prsmsp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 18:52:46.000000 prsmsp-1.5.0/prsmsp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 18:52:46.000000 prsmsp-1.5.0/prsmsp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-06 18:52:46.000000 prsmsp-1.5.0/prsmsp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-06 18:52:46.000000 prsmsp-1.5.0/prsmsp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-05-06 18:52:46.213863 prsmsp-1.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-06 18:52:35.000000 prsmsp-1.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 18:52:46.213863 prsmsp-1.5.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 18:52:35.000000 prsmsp-1.5.0/tests/test_app.py
```

### Comparing `prsmsp-1.4.0/PKG-INFO` & `prsmsp-1.5.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7072 736d  : 2.1.Name: prsm
-00000020: 7370 0a56 6572 7369 6f6e 3a20 312e 342e  sp.Version: 1.4.
+00000020: 7370 0a56 6572 7369 6f6e 3a20 312e 352e  sp.Version: 1.5.
 00000030: 300a 5375 6d6d 6172 793a 2050 6163 6b61  0.Summary: Packa
 00000040: 6765 2074 6f20 776f 726b 2077 6974 6820  ge to work with 
 00000050: 736d 7320 7061 6e65 6c73 0a48 6f6d 652d  sms panels.Home-
 00000060: 7061 6765 3a20 6874 7470 733a 2f2f 6769  page: https://gi
 00000070: 7468 7562 2e63 6f6d 2f70 6172 7361 7269  thub.com/parsari
 00000080: 7961 6869 2f70 7273 6d73 700a 4175 7468  yahi/prsmsp.Auth
 00000090: 6f72 3a20 5061 7273 6120 5269 7961 6869  or: Parsa Riyahi
@@ -45,93 +45,164 @@
 000002c0: 3a20 546f 7069 6320 3a3a 2053 6f66 7477  : Topic :: Softw
 000002d0: 6172 6520 4465 7665 6c6f 706d 656e 7420  are Development 
 000002e0: 3a3a 204c 6962 7261 7269 6573 203a 3a20  :: Libraries :: 
 000002f0: 5079 7468 6f6e 204d 6f64 756c 6573 0a52  Python Modules.R
 00000300: 6571 7569 7265 732d 5079 7468 6f6e 3a20  equires-Python: 
 00000310: 3e3d 332e 360a 4465 7363 7269 7074 696f  >=3.6.Descriptio
 00000320: 6e2d 436f 6e74 656e 742d 5479 7065 3a20  n-Content-Type: 
-00000330: 7465 7874 2f6d 6172 6b64 6f77 6e0a 0a23  text/markdown..#
-00000340: 2320 5375 7070 6f72 7465 6420 7061 6e65  # Supported pane
-00000350: 6c73 0a0a 2a20 5b4b 6176 656e 6567 6172  ls..* [Kavenegar
-00000360: 5d28 6874 7470 3a2f 2f6b 6176 656e 6567  ](http://kaveneg
-00000370: 6172 2e63 6f6d 290a 2a20 5b53 6d73 2e69  ar.com).* [Sms.i
-00000380: 725d 2868 7474 703a 2f2f 736d 732e 6972  r](http://sms.ir
-00000390: 290a 2a20 5b57 6562 206f 6e65 5d28 6874  ).* [Web one](ht
-000003a0: 7470 3a2f 2f77 6562 6f6e 652d 736d 732e  tp://webone-sms.
-000003b0: 6972 290a 2a20 5b4d 656c 6920 5061 7961  ir).* [Meli Paya
-000003c0: 6d61 6b5d 2868 7474 7073 3a2f 2f77 7777  mak](https://www
-000003d0: 2e6d 656c 6970 6179 616d 616b 2e63 6f6d  .melipayamak.com
-000003e0: 290a 2a20 5b4d 6564 6961 6e61 5d28 6874  ).* [Mediana](ht
-000003f0: 7470 733a 2f2f 6d65 6469 616e 612e 6972  tps://mediana.ir
-00000400: 290a 2a20 5b47 6861 7365 6461 6b20 536d  ).* [Ghasedak Sm
-00000410: 735d 2868 7474 7073 3a2f 2f67 6861 7365  s](https://ghase
-00000420: 6461 6b2e 6d65 290a 2a20 5b46 6172 617a  dak.me).* [Faraz
-00000430: 2053 6d73 5d28 6874 7470 733a 2f2f 6661   Sms](https://fa
-00000440: 7261 7a73 6d73 2e63 6f6d 2f29 0a0a 2323  razsms.com/)..##
-00000450: 2057 6879 2075 7365 2074 6869 7320 7061   Why use this pa
-00000460: 636b 6167 653f 0a0a 312e 2020 596f 7520  ckage?..1.  You 
-00000470: 6861 7665 2061 6c6c 2074 6865 2066 616d  have all the fam
-00000480: 6f75 7320 616e 6420 7765 6c6c 2064 6573  ous and well des
-00000490: 6967 6e65 6420 736d 7320 7061 6e65 6c73  igned sms panels
-000004a0: 2072 6561 6479 2074 6f20 676f 2e0a 322e   ready to go..2.
-000004b0: 2020 5768 656e 2079 6f75 2068 6176 6520    When you have 
-000004c0: 746f 2077 6f72 6b20 7769 7468 2073 6576  to work with sev
-000004d0: 6572 616c 2073 6d73 2070 616e 656c 732e  eral sms panels.
-000004e0: 0a33 2e20 2044 6f6e 2774 206e 6565 6420  .3.  Don't need 
-000004f0: 746f 2062 7569 6c64 2074 6865 2077 6865  to build the whe
-00000500: 656c 206f 6620 796f 7572 2062 6963 7963  el of your bicyc
-00000510: 6c65 2065 6163 6820 7469 6d65 20e2 98ba  le each time ...
-00000520: 2e0a 0a23 2320 486f 7720 746f 2075 7365  ...## How to use
-00000530: 0a0a 4669 7273 7420 6c65 7473 2069 6e73  ..First lets ins
-00000540: 7461 6c6c 2074 6865 2070 6163 6b61 6765  tall the package
-00000550: 0a60 6060 7368 656c 6c0a 7069 7020 696e  .```shell.pip in
-00000560: 7374 616c 6c20 7072 736d 7370 0a60 6060  stall prsmsp.```
-00000570: 0a0a 5468 6973 2062 6c6f 636b 206f 6620  ..This block of 
-00000580: 636f 6465 2069 7320 666f 7220 2a2a 6b61  code is for **ka
-00000590: 7665 6e65 6761 722a 2a20 736d 7320 7061  venegar** sms pa
-000005a0: 6e65 6c2e 0a0a 4561 6368 206f 6620 736d  nel...Each of sm
-000005b0: 7320 7061 6e65 6c73 2068 6173 2069 7473  s panels has its
-000005c0: 206f 776e 2070 6172 616d 6574 6572 732e   own parameters.
-000005d0: 2050 6c65 6173 6520 7265 6164 2074 6865   Please read the
-000005e0: 6972 2064 6f63 7320 6669 7273 742e 0a0a  ir docs first...
-000005f0: 6060 6070 7974 686f 6e0a 6672 6f6d 2070  ```python.from p
-00000600: 7273 6d73 702e 7061 6e65 6c73 2069 6d70  rsmsp.panels imp
-00000610: 6f72 7420 4b61 7665 6e65 6761 720a 0a61  ort Kavenegar..a
-00000620: 7069 5f6b 6579 203d 2022 796f 7572 2061  pi_key = "your a
-00000630: 7069 206b 6579 220a 7061 6e65 6c20 3d20  pi key".panel = 
-00000640: 4b61 7665 6e65 6761 7228 6170 695f 6b65  Kavenegar(api_ke
-00000650: 7929 2020 2320 6175 7468 0a0a 7265 6365  y)  # auth..rece
-00000660: 7074 6f72 203d 2022 796f 7572 2072 6563  ptor = "your rec
-00000670: 6570 746f 7222 0a6d 7367 203d 2022 796f  eptor".msg = "yo
-00000680: 7572 206d 6573 7361 6765 220a 7061 6e65  ur message".pane
-00000690: 6c2e 7365 6e64 5f73 6d73 2872 6563 6570  l.send_sms(recep
-000006a0: 746f 722c 206d 7367 290a 6060 600a 2323  tor, msg).```.##
-000006b0: 2320 5265 6164 205b 446f 6373 5d28 6874  # Read [Docs](ht
-000006c0: 7470 733a 2f2f 7072 736d 7370 2e72 6561  tps://prsmsp.rea
-000006d0: 6474 6865 646f 6373 2e69 6f2f 290a 0a0a  dthedocs.io/)...
-000006e0: 2323 2048 6f77 2074 6f20 7375 7070 6f72  ## How to suppor
-000006f0: 7420 7468 6973 2070 726f 6a65 6374 0a66  t this project.f
-00000700: 6f72 2074 6869 7320 7072 6f6a 6563 7420  or this project 
-00000710: 746f 2062 6520 6265 7474 6572 2061 6e64  to be better and
-00000720: 2062 6967 6765 7220 7468 616e 2077 6861   bigger than wha
-00000730: 7420 6974 2069 7320 6e6f 772e 0a77 6520  t it is now..we 
-00000740: 6e65 6564 2074 6f20 7375 7070 6f72 7420  need to support 
-00000750: 6d6f 7265 2070 616e 656c 7320 616e 6420  more panels and 
-00000760: 6576 656e 2074 6573 7420 6120 7265 616c  even test a real
-00000770: 2073 656e 6420 736d 7320 7768 6963 6820   send sms which 
-00000780: 6e65 6564 7320 6120 7375 6273 6372 6970  needs a subscrip
-00000790: 7469 6f6e 2066 6f72 2065 6163 6820 736d  tion for each sm
-000007a0: 7320 7072 6f76 6964 6572 200a 6966 2079  s provider .if y
-000007b0: 6f75 2068 6176 6520 7375 6273 2066 6f72  ou have subs for
-000007c0: 2061 6e79 2073 6d73 2070 616e 656c 206f   any sms panel o
-000007d0: 7220 646f 6373 206f 6620 616e 7920 736d  r docs of any sm
-000007e0: 7320 7061 6e65 6c20 616e 6420 796f 7520  s panel and you 
-000007f0: 7468 696e 6b20 6974 2077 6f75 6c64 2062  think it would b
-00000800: 6520 676f 6f64 2066 6f72 2074 6869 7320  e good for this 
-00000810: 7061 6361 6b67 6520 746f 2068 6176 6520  pacakge to have 
-00000820: 7375 7070 6f72 7420 7468 6174 2073 6d73  support that sms
-00000830: 2070 616e 656c 2070 6c65 6173 6520 6f70   panel please op
-00000840: 656e 2061 6e20 6973 7375 6520 6f72 2063  en an issue or c
-00000850: 6f6e 7461 6374 206d 650a 4d79 2065 6d61  ontact me.My ema
-00000860: 696c 2069 7320 7061 6e79 2e70 6172 7361  il is pany.parsa
-00000870: 7269 7961 6869 4067 6d61 696c 2e63 6f6d  riyahi@gmail.com
-00000880: 0a                                       .
+00000330: 7465 7874 2f6d 6172 6b64 6f77 6e0a 0a3c  text/markdown..<
+00000340: 6469 7620 616c 6967 6e3d 2263 656e 7465  div align="cente
+00000350: 7222 3e0a 2020 2020 3c68 313e 203c 696d  r">.    <h1> <im
+00000360: 6720 7372 633d 2268 7474 7073 3a2f 2f75  g src="https://u
+00000370: 706c 6f61 642e 7769 6b69 6d65 6469 612e  pload.wikimedia.
+00000380: 6f72 672f 7769 6b69 7065 6469 612f 636f  org/wikipedia/co
+00000390: 6d6d 6f6e 732f 7468 756d 622f 352f 3531  mmons/thumb/5/51
+000003a0: 2f49 4d65 7373 6167 655f 6c6f 676f 2e73  /IMessage_logo.s
+000003b0: 7667 2f32 3034 3870 782d 494d 6573 7361  vg/2048px-IMessa
+000003c0: 6765 5f6c 6f67 6f2e 7376 672e 706e 6722  ge_logo.svg.png"
+000003d0: 2077 6964 7468 3d22 3830 7078 223e 3c62   width="80px"><b
+000003e0: 722f 3e70 7273 6d73 703c 2f68 313e 0a3c  r/>prsmsp</h1>.<
+000003f0: 2f64 6976 3e0a 3c70 2061 6c69 676e 3d22  /div>.<p align="
+00000400: 6365 6e74 6572 223e 203c 6120 6872 6566  center"> <a href
+00000410: 3d22 6874 7470 733a 2f2f 7072 736d 7370  ="https://prsmsp
+00000420: 2e72 6561 6474 6865 646f 6373 2e69 6f22  .readthedocs.io"
+00000430: 2074 6172 6765 743d 225f 626c 616e 6b22   target="_blank"
+00000440: 3e3c 696d 6720 616c 743d 2222 2073 7263  ><img alt="" src
+00000450: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
+00000460: 6965 6c64 732e 696f 2f62 6164 6765 2f57  ields.io/badge/W
+00000470: 6562 7369 7465 2d45 4134 4338 393f 7374  ebsite-EA4C89?st
+00000480: 796c 653d 6e6f 726d 616c 266c 6f67 6f3d  yle=normal&logo=
+00000490: 6472 6962 6262 6c65 266c 6f67 6f43 6f6c  dribbble&logoCol
+000004a0: 6f72 3d77 6869 7465 2220 7374 796c 653d  or=white" style=
+000004b0: 2276 6572 7469 6361 6c2d 616c 6967 6e3a  "vertical-align:
+000004c0: 6365 6e74 6572 2220 2f3e 3c2f 613e 0a20  center" /></a>. 
+000004d0: 2020 200a 2020 200a 2320 4465 7363 7269     .   .# Descri
+000004e0: 7074 696f 6e0a 5079 7468 6f6e 204c 6962  ption.Python Lib
+000004f0: 7261 7279 2066 6f72 2073 656e 6469 6e67  rary for sending
+00000500: 2053 4d53 2077 6974 6820 7375 7070 6f72   SMS with suppor
+00000510: 7465 6420 534d 5320 7365 7276 6963 6520  ted SMS service 
+00000520: 7072 6f76 6964 6572 732c 2054 6869 7320  providers, This 
+00000530: 7072 6f6a 6563 7420 776f 726b 7320 6173  project works as
+00000540: 2061 6e20 4150 4920 6265 7477 6565 6e20   an API between 
+00000550: 796f 7520 616e 6420 796f 7572 2053 4d53  you and your SMS
+00000560: 2070 726f 7669 6465 722c 2072 6561 6420   provider, read 
+00000570: 6d6f 7265 2061 626f 7574 2074 6869 7320  more about this 
+00000580: 7072 6f6a 6563 7420 6174 205b 5265 6164  project at [Read
+00000590: 2054 6865 2044 6f63 735d 2868 7474 7073   The Docs](https
+000005a0: 3a2f 2f70 7273 6d73 702e 7265 6164 7468  ://prsmsp.readth
+000005b0: 6564 6f63 732e 696f 2f29 2e0a 0a3c 6272  edocs.io/)...<br
+000005c0: 3e0a 0a23 2046 6561 7475 7265 730a 5768  >..# Features.Wh
+000005d0: 656e 2079 6f75 2075 7365 2061 2053 4d53  en you use a SMS
+000005e0: 2070 616e 656c 2066 726f 6d20 6120 7072   panel from a pr
+000005f0: 6f76 6964 6572 2c20 796f 7520 696d 706c  ovider, you impl
+00000600: 656d 656e 7420 6974 2066 726f 6d20 7a65  ement it from ze
+00000610: 726f 2c20 616e 6420 6966 2079 6f75 2077  ro, and if you w
+00000620: 616e 7420 746f 2063 6861 6e67 6520 7468  ant to change th
+00000630: 6520 7061 6e65 6c2c 2079 6f75 206e 6565  e panel, you nee
+00000640: 6420 746f 2072 6566 6163 746f 7220 616c  d to refactor al
+00000650: 6c20 6f66 2079 6f75 7220 636f 6465 2e0a  l of your code..
+00000660: 616e 6420 666f 7220 696d 706c 656d 656e  and for implemen
+00000670: 7469 6e67 2061 2070 616e 656c 2066 726f  ting a panel fro
+00000680: 6d20 7a65 726f 2079 6f75 206e 6565 6420  m zero you need 
+00000690: 7469 6d65 2074 6f20 7265 6164 2074 6865  time to read the
+000006a0: 6972 2064 6f63 756d 656e 7420 616e 6420  ir document and 
+000006b0: 7472 7920 746f 2075 7365 2069 7420 616e  try to use it an
+000006c0: 6420 696d 706c 656d 656e 7420 6974 2e0a  d implement it..
+000006d0: 7468 6973 2070 726f 6a65 6374 2073 6176  this project sav
+000006e0: 6520 796f 7520 7469 6d65 2066 6f72 2069  e you time for i
+000006f0: 6d70 6c65 6d65 6e74 696e 6720 7061 6e65  mplementing pane
+00000700: 6c73 2061 6e64 2066 6f72 2072 6566 6163  ls and for refac
+00000710: 746f 7269 6e67 2079 6f75 7220 636f 6465  toring your code
+00000720: 2e0a 0a23 2320 5768 7920 7573 6520 7468  ...## Why use th
+00000730: 6973 2070 726f 6a65 6374 3f0a 2d20 596f  is project?.- Yo
+00000740: 7520 6861 7665 2061 6c6c 2074 6865 2066  u have all the f
+00000750: 616d 6f75 7320 616e 6420 7765 6c6c 2064  amous and well d
+00000760: 6573 6967 6e65 6420 534d 5320 7061 6e65  esigned SMS pane
+00000770: 6c73 2072 6561 6479 2074 6f20 676f 2e0a  ls ready to go..
+00000780: 2d20 596f 7520 6361 6e20 6861 7665 2073  - You can have s
+00000790: 6576 6572 616c 2053 4d53 2070 616e 656c  everal SMS panel
+000007a0: 7320 6174 2074 6865 2073 616d 6520 7469  s at the same ti
+000007b0: 6d65 2e0a 2d20 446f 6e27 7420 6e65 6564  me..- Don't need
+000007c0: 2074 6f20 6275 696c 6420 7468 6520 7768   to build the wh
+000007d0: 6565 6c20 6f66 2079 6f75 7220 6269 6379  eel of your bicy
+000007e0: 636c 6520 6561 6368 2074 696d 6520 e298  cle each time ..
+000007f0: ba2e 0a2d 2046 6173 7420 616e 6420 536d  ...- Fast and Sm
+00000800: 616c 6c0a 2d20 4561 7379 2074 6f20 696d  all.- Easy to im
+00000810: 706c 656d 656e 7420 616e 6420 7573 650a  plement and use.
+00000820: 0a3c 6272 3e0a 0a23 2053 7570 706f 7274  .<br>..# Support
+00000830: 6564 2070 616e 656c 730a 0a2a 205b 4b61  ed panels..* [Ka
+00000840: 7665 6e65 6761 725d 2868 7474 703a 2f2f  venegar](http://
+00000850: 6b61 7665 6e65 6761 722e 636f 6d29 0a2a  kavenegar.com).*
+00000860: 205b 536d 732e 6972 5d28 6874 7470 3a2f   [Sms.ir](http:/
+00000870: 2f73 6d73 2e69 7229 0a2a 205b 5765 6220  /sms.ir).* [Web 
+00000880: 6f6e 655d 2868 7474 703a 2f2f 7765 626f  one](http://webo
+00000890: 6e65 2d73 6d73 2e69 7229 0a2a 205b 4d65  ne-sms.ir).* [Me
+000008a0: 6c69 2050 6179 616d 616b 5d28 6874 7470  li Payamak](http
+000008b0: 733a 2f2f 7777 772e 6d65 6c69 7061 7961  s://www.melipaya
+000008c0: 6d61 6b2e 636f 6d29 0a2a 205b 4d65 6469  mak.com).* [Medi
+000008d0: 616e 615d 2868 7474 7073 3a2f 2f6d 6564  ana](https://med
+000008e0: 6961 6e61 2e69 7229 0a2a 205b 4768 6173  iana.ir).* [Ghas
+000008f0: 6564 616b 2053 6d73 5d28 6874 7470 733a  edak Sms](https:
+00000900: 2f2f 6768 6173 6564 616b 2e6d 6529 0a2a  //ghasedak.me).*
+00000910: 205b 4661 7261 7a20 536d 735d 2868 7474   [Faraz Sms](htt
+00000920: 7073 3a2f 2f66 6172 617a 736d 732e 636f  ps://farazsms.co
+00000930: 6d2f 290a 2a20 5b4e 696b 2053 6d73 5d28  m/).* [Nik Sms](
+00000940: 6874 7470 733a 2f2f 6e69 6b73 6d73 2e63  https://niksms.c
+00000950: 6f6d 2f29 0a2a 205b 536d 7331 5d28 6874  om/).* [Sms1](ht
+00000960: 7470 733a 2f2f 736d 7331 2e69 722f 290a  tps://sms1.ir/).
+00000970: 0a3c 6272 3e0a 0a23 2048 6f77 2074 6f20  .<br>..# How to 
+00000980: 7573 653f 0a46 6972 7374 206c 6574 7320  use?.First lets 
+00000990: 696e 7374 616c 6c20 7468 6520 7061 636b  install the pack
+000009a0: 6167 650a 6060 6073 6865 6c6c 0a70 6970  age.```shell.pip
+000009b0: 2069 6e73 7461 6c6c 2070 7273 6d73 700a   install prsmsp.
+000009c0: 6060 600a 0a54 6869 7320 626c 6f63 6b20  ```..This block 
+000009d0: 6f66 2063 6f64 6520 6973 2066 6f72 202a  of code is for *
+000009e0: 2a6b 6176 656e 6567 6172 2a2a 2073 6d73  *kavenegar** sms
+000009f0: 2070 616e 656c 2e0a 0a45 6163 6820 6f66   panel...Each of
+00000a00: 2073 6d73 2070 616e 656c 7320 6861 7320   sms panels has 
+00000a10: 6974 7320 6f77 6e20 7061 7261 6d65 7465  its own paramete
+00000a20: 7273 2e20 506c 6561 7365 2072 6561 6420  rs. Please read 
+00000a30: 7468 6569 7220 646f 6373 2066 6972 7374  their docs first
+00000a40: 2e0a 0a60 6060 7079 7468 6f6e 0a66 726f  ...```python.fro
+00000a50: 6d20 7072 736d 7370 2e70 616e 656c 7320  m prsmsp.panels 
+00000a60: 696d 706f 7274 204b 6176 656e 6567 6172  import Kavenegar
+00000a70: 0a0a 6170 695f 6b65 7920 3d20 2279 6f75  ..api_key = "you
+00000a80: 7220 6170 6920 6b65 7922 0a70 616e 656c  r api key".panel
+00000a90: 203d 204b 6176 656e 6567 6172 2861 7069   = Kavenegar(api
+00000aa0: 5f6b 6579 2920 2023 2061 7574 680a 0a72  _key)  # auth..r
+00000ab0: 6563 6570 746f 7220 3d20 2279 6f75 7220  eceptor = "your 
+00000ac0: 7265 6365 7074 6f72 220a 6d73 6720 3d20  receptor".msg = 
+00000ad0: 2279 6f75 7220 6d65 7373 6167 6522 0a70  "your message".p
+00000ae0: 616e 656c 2e73 656e 645f 736d 7328 7265  anel.send_sms(re
+00000af0: 6365 7074 6f72 2c20 6d73 6729 0a60 6060  ceptor, msg).```
+00000b00: 0a0a 2323 2323 205b 446f 6373 5d28 6874  ..#### [Docs](ht
+00000b10: 7470 733a 2f2f 7072 736d 7370 2e72 6561  tps://prsmsp.rea
+00000b20: 6474 6865 646f 6373 2e69 6f2f 656e 2f6c  dthedocs.io/en/l
+00000b30: 6174 6573 742f 7061 6e65 6c73 2f70 616e  atest/panels/pan
+00000b40: 656c 732e 6874 6d6c 290a 0a3c 6272 3e0a  els.html)..<br>.
+00000b50: 0a23 2048 6f77 2074 6f20 7375 7070 6f72  .# How to suppor
+00000b60: 7420 7468 6973 2070 726f 6a65 6374 3f0a  t this project?.
+00000b70: 666f 7220 7468 6973 2070 726f 6a65 6374  for this project
+00000b80: 2074 6f20 6265 2062 6574 7465 7220 616e   to be better an
+00000b90: 6420 6269 6767 6572 2074 6861 6e20 7768  d bigger than wh
+00000ba0: 6174 2069 7420 6973 206e 6f77 2e0a 7765  at it is now..we
+00000bb0: 206e 6565 6420 746f 2073 7570 706f 7274   need to support
+00000bc0: 206d 6f72 6520 7061 6e65 6c73 2061 6e64   more panels and
+00000bd0: 2065 7665 6e20 7465 7374 2061 2072 6561   even test a rea
+00000be0: 6c20 7365 6e64 2073 6d73 2077 6869 6368  l send sms which
+00000bf0: 206e 6565 6473 2061 2073 7562 7363 7269   needs a subscri
+00000c00: 7074 696f 6e20 666f 7220 6561 6368 2073  ption for each s
+00000c10: 6d73 2070 726f 7669 6465 7220 0a69 6620  ms provider .if 
+00000c20: 796f 7520 6861 7665 2073 7562 7320 666f  you have subs fo
+00000c30: 7220 616e 7920 736d 7320 7061 6e65 6c20  r any sms panel 
+00000c40: 6f72 2064 6f63 7320 6f66 2061 6e79 2073  or docs of any s
+00000c50: 6d73 2070 616e 656c 2061 6e64 2079 6f75  ms panel and you
+00000c60: 2074 6869 6e6b 2069 7420 776f 756c 6420   think it would 
+00000c70: 6265 2067 6f6f 6420 666f 7220 7468 6973  be good for this
+00000c80: 2070 6163 616b 6765 2074 6f20 6861 7665   pacakge to have
+00000c90: 2073 7570 706f 7274 2074 6861 7420 736d   support that sm
+00000ca0: 7320 7061 6e65 6c20 706c 6561 7365 206f  s panel please o
+00000cb0: 7065 6e20 616e 2069 7373 7565 206f 7220  pen an issue or 
+00000cc0: 636f 6e74 6163 7420 6d65 0a4d 7920 656d  contact me.My em
+00000cd0: 6169 6c20 6973 2070 616e 792e 7061 7273  ail is pany.pars
+00000ce0: 6172 6979 6168 6940 676d 6169 6c2e 636f  ariyahi@gmail.co
+00000cf0: 6d0a 0a                                  m..
```

### Comparing `prsmsp-1.4.0/prsmsp/factories/auth_factory.py` & `prsmsp-1.5.0/prsmsp/factories/auth_factory.py`

 * *Files identical despite different names*

### Comparing `prsmsp-1.4.0/prsmsp/models/response.py` & `prsmsp-1.5.0/prsmsp/models/response.py`

 * *Files identical despite different names*

### Comparing `prsmsp-1.4.0/prsmsp/panels/farazsms.py` & `prsmsp-1.5.0/prsmsp/panels/farazsms.py`

 * *Files identical despite different names*

### Comparing `prsmsp-1.4.0/prsmsp/panels/ghasedaksms.py` & `prsmsp-1.5.0/prsmsp/panels/ghasedaksms.py`

 * *Files identical despite different names*

### Comparing `prsmsp-1.4.0/prsmsp/panels/kavenegar.py` & `prsmsp-1.5.0/prsmsp/panels/kavenegar.py`

 * *Files identical despite different names*

### Comparing `prsmsp-1.4.0/prsmsp/panels/mediana.py` & `prsmsp-1.5.0/prsmsp/panels/mediana.py`

 * *Files identical despite different names*

### Comparing `prsmsp-1.4.0/prsmsp/panels/melipayamak.py` & `prsmsp-1.5.0/prsmsp/panels/melipayamak.py`

 * *Files identical despite different names*

### Comparing `prsmsp-1.4.0/prsmsp/panels/niksms.py` & `prsmsp-1.5.0/prsmsp/panels/niksms.py`

 * *Files identical despite different names*

### Comparing `prsmsp-1.4.0/prsmsp/panels/smsdotir.py` & `prsmsp-1.5.0/prsmsp/panels/smsdotir.py`

 * *Files identical despite different names*

### Comparing `prsmsp-1.4.0/prsmsp/panels/webonesms.py` & `prsmsp-1.5.0/prsmsp/panels/webonesms.py`

 * *Files identical despite different names*

### Comparing `prsmsp-1.4.0/prsmsp.egg-info/PKG-INFO` & `prsmsp-1.5.0/prsmsp.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
 00000010: 3a20 322e 310a 4e61 6d65 3a20 7072 736d  : 2.1.Name: prsm
-00000020: 7370 0a56 6572 7369 6f6e 3a20 312e 342e  sp.Version: 1.4.
+00000020: 7370 0a56 6572 7369 6f6e 3a20 312e 352e  sp.Version: 1.5.
 00000030: 300a 5375 6d6d 6172 793a 2050 6163 6b61  0.Summary: Packa
 00000040: 6765 2074 6f20 776f 726b 2077 6974 6820  ge to work with 
 00000050: 736d 7320 7061 6e65 6c73 0a48 6f6d 652d  sms panels.Home-
 00000060: 7061 6765 3a20 6874 7470 733a 2f2f 6769  page: https://gi
 00000070: 7468 7562 2e63 6f6d 2f70 6172 7361 7269  thub.com/parsari
 00000080: 7961 6869 2f70 7273 6d73 700a 4175 7468  yahi/prsmsp.Auth
 00000090: 6f72 3a20 5061 7273 6120 5269 7961 6869  or: Parsa Riyahi
@@ -45,93 +45,164 @@
 000002c0: 3a20 546f 7069 6320 3a3a 2053 6f66 7477  : Topic :: Softw
 000002d0: 6172 6520 4465 7665 6c6f 706d 656e 7420  are Development 
 000002e0: 3a3a 204c 6962 7261 7269 6573 203a 3a20  :: Libraries :: 
 000002f0: 5079 7468 6f6e 204d 6f64 756c 6573 0a52  Python Modules.R
 00000300: 6571 7569 7265 732d 5079 7468 6f6e 3a20  equires-Python: 
 00000310: 3e3d 332e 360a 4465 7363 7269 7074 696f  >=3.6.Descriptio
 00000320: 6e2d 436f 6e74 656e 742d 5479 7065 3a20  n-Content-Type: 
-00000330: 7465 7874 2f6d 6172 6b64 6f77 6e0a 0a23  text/markdown..#
-00000340: 2320 5375 7070 6f72 7465 6420 7061 6e65  # Supported pane
-00000350: 6c73 0a0a 2a20 5b4b 6176 656e 6567 6172  ls..* [Kavenegar
-00000360: 5d28 6874 7470 3a2f 2f6b 6176 656e 6567  ](http://kaveneg
-00000370: 6172 2e63 6f6d 290a 2a20 5b53 6d73 2e69  ar.com).* [Sms.i
-00000380: 725d 2868 7474 703a 2f2f 736d 732e 6972  r](http://sms.ir
-00000390: 290a 2a20 5b57 6562 206f 6e65 5d28 6874  ).* [Web one](ht
-000003a0: 7470 3a2f 2f77 6562 6f6e 652d 736d 732e  tp://webone-sms.
-000003b0: 6972 290a 2a20 5b4d 656c 6920 5061 7961  ir).* [Meli Paya
-000003c0: 6d61 6b5d 2868 7474 7073 3a2f 2f77 7777  mak](https://www
-000003d0: 2e6d 656c 6970 6179 616d 616b 2e63 6f6d  .melipayamak.com
-000003e0: 290a 2a20 5b4d 6564 6961 6e61 5d28 6874  ).* [Mediana](ht
-000003f0: 7470 733a 2f2f 6d65 6469 616e 612e 6972  tps://mediana.ir
-00000400: 290a 2a20 5b47 6861 7365 6461 6b20 536d  ).* [Ghasedak Sm
-00000410: 735d 2868 7474 7073 3a2f 2f67 6861 7365  s](https://ghase
-00000420: 6461 6b2e 6d65 290a 2a20 5b46 6172 617a  dak.me).* [Faraz
-00000430: 2053 6d73 5d28 6874 7470 733a 2f2f 6661   Sms](https://fa
-00000440: 7261 7a73 6d73 2e63 6f6d 2f29 0a0a 2323  razsms.com/)..##
-00000450: 2057 6879 2075 7365 2074 6869 7320 7061   Why use this pa
-00000460: 636b 6167 653f 0a0a 312e 2020 596f 7520  ckage?..1.  You 
-00000470: 6861 7665 2061 6c6c 2074 6865 2066 616d  have all the fam
-00000480: 6f75 7320 616e 6420 7765 6c6c 2064 6573  ous and well des
-00000490: 6967 6e65 6420 736d 7320 7061 6e65 6c73  igned sms panels
-000004a0: 2072 6561 6479 2074 6f20 676f 2e0a 322e   ready to go..2.
-000004b0: 2020 5768 656e 2079 6f75 2068 6176 6520    When you have 
-000004c0: 746f 2077 6f72 6b20 7769 7468 2073 6576  to work with sev
-000004d0: 6572 616c 2073 6d73 2070 616e 656c 732e  eral sms panels.
-000004e0: 0a33 2e20 2044 6f6e 2774 206e 6565 6420  .3.  Don't need 
-000004f0: 746f 2062 7569 6c64 2074 6865 2077 6865  to build the whe
-00000500: 656c 206f 6620 796f 7572 2062 6963 7963  el of your bicyc
-00000510: 6c65 2065 6163 6820 7469 6d65 20e2 98ba  le each time ...
-00000520: 2e0a 0a23 2320 486f 7720 746f 2075 7365  ...## How to use
-00000530: 0a0a 4669 7273 7420 6c65 7473 2069 6e73  ..First lets ins
-00000540: 7461 6c6c 2074 6865 2070 6163 6b61 6765  tall the package
-00000550: 0a60 6060 7368 656c 6c0a 7069 7020 696e  .```shell.pip in
-00000560: 7374 616c 6c20 7072 736d 7370 0a60 6060  stall prsmsp.```
-00000570: 0a0a 5468 6973 2062 6c6f 636b 206f 6620  ..This block of 
-00000580: 636f 6465 2069 7320 666f 7220 2a2a 6b61  code is for **ka
-00000590: 7665 6e65 6761 722a 2a20 736d 7320 7061  venegar** sms pa
-000005a0: 6e65 6c2e 0a0a 4561 6368 206f 6620 736d  nel...Each of sm
-000005b0: 7320 7061 6e65 6c73 2068 6173 2069 7473  s panels has its
-000005c0: 206f 776e 2070 6172 616d 6574 6572 732e   own parameters.
-000005d0: 2050 6c65 6173 6520 7265 6164 2074 6865   Please read the
-000005e0: 6972 2064 6f63 7320 6669 7273 742e 0a0a  ir docs first...
-000005f0: 6060 6070 7974 686f 6e0a 6672 6f6d 2070  ```python.from p
-00000600: 7273 6d73 702e 7061 6e65 6c73 2069 6d70  rsmsp.panels imp
-00000610: 6f72 7420 4b61 7665 6e65 6761 720a 0a61  ort Kavenegar..a
-00000620: 7069 5f6b 6579 203d 2022 796f 7572 2061  pi_key = "your a
-00000630: 7069 206b 6579 220a 7061 6e65 6c20 3d20  pi key".panel = 
-00000640: 4b61 7665 6e65 6761 7228 6170 695f 6b65  Kavenegar(api_ke
-00000650: 7929 2020 2320 6175 7468 0a0a 7265 6365  y)  # auth..rece
-00000660: 7074 6f72 203d 2022 796f 7572 2072 6563  ptor = "your rec
-00000670: 6570 746f 7222 0a6d 7367 203d 2022 796f  eptor".msg = "yo
-00000680: 7572 206d 6573 7361 6765 220a 7061 6e65  ur message".pane
-00000690: 6c2e 7365 6e64 5f73 6d73 2872 6563 6570  l.send_sms(recep
-000006a0: 746f 722c 206d 7367 290a 6060 600a 2323  tor, msg).```.##
-000006b0: 2320 5265 6164 205b 446f 6373 5d28 6874  # Read [Docs](ht
-000006c0: 7470 733a 2f2f 7072 736d 7370 2e72 6561  tps://prsmsp.rea
-000006d0: 6474 6865 646f 6373 2e69 6f2f 290a 0a0a  dthedocs.io/)...
-000006e0: 2323 2048 6f77 2074 6f20 7375 7070 6f72  ## How to suppor
-000006f0: 7420 7468 6973 2070 726f 6a65 6374 0a66  t this project.f
-00000700: 6f72 2074 6869 7320 7072 6f6a 6563 7420  or this project 
-00000710: 746f 2062 6520 6265 7474 6572 2061 6e64  to be better and
-00000720: 2062 6967 6765 7220 7468 616e 2077 6861   bigger than wha
-00000730: 7420 6974 2069 7320 6e6f 772e 0a77 6520  t it is now..we 
-00000740: 6e65 6564 2074 6f20 7375 7070 6f72 7420  need to support 
-00000750: 6d6f 7265 2070 616e 656c 7320 616e 6420  more panels and 
-00000760: 6576 656e 2074 6573 7420 6120 7265 616c  even test a real
-00000770: 2073 656e 6420 736d 7320 7768 6963 6820   send sms which 
-00000780: 6e65 6564 7320 6120 7375 6273 6372 6970  needs a subscrip
-00000790: 7469 6f6e 2066 6f72 2065 6163 6820 736d  tion for each sm
-000007a0: 7320 7072 6f76 6964 6572 200a 6966 2079  s provider .if y
-000007b0: 6f75 2068 6176 6520 7375 6273 2066 6f72  ou have subs for
-000007c0: 2061 6e79 2073 6d73 2070 616e 656c 206f   any sms panel o
-000007d0: 7220 646f 6373 206f 6620 616e 7920 736d  r docs of any sm
-000007e0: 7320 7061 6e65 6c20 616e 6420 796f 7520  s panel and you 
-000007f0: 7468 696e 6b20 6974 2077 6f75 6c64 2062  think it would b
-00000800: 6520 676f 6f64 2066 6f72 2074 6869 7320  e good for this 
-00000810: 7061 6361 6b67 6520 746f 2068 6176 6520  pacakge to have 
-00000820: 7375 7070 6f72 7420 7468 6174 2073 6d73  support that sms
-00000830: 2070 616e 656c 2070 6c65 6173 6520 6f70   panel please op
-00000840: 656e 2061 6e20 6973 7375 6520 6f72 2063  en an issue or c
-00000850: 6f6e 7461 6374 206d 650a 4d79 2065 6d61  ontact me.My ema
-00000860: 696c 2069 7320 7061 6e79 2e70 6172 7361  il is pany.parsa
-00000870: 7269 7961 6869 4067 6d61 696c 2e63 6f6d  riyahi@gmail.com
-00000880: 0a                                       .
+00000330: 7465 7874 2f6d 6172 6b64 6f77 6e0a 0a3c  text/markdown..<
+00000340: 6469 7620 616c 6967 6e3d 2263 656e 7465  div align="cente
+00000350: 7222 3e0a 2020 2020 3c68 313e 203c 696d  r">.    <h1> <im
+00000360: 6720 7372 633d 2268 7474 7073 3a2f 2f75  g src="https://u
+00000370: 706c 6f61 642e 7769 6b69 6d65 6469 612e  pload.wikimedia.
+00000380: 6f72 672f 7769 6b69 7065 6469 612f 636f  org/wikipedia/co
+00000390: 6d6d 6f6e 732f 7468 756d 622f 352f 3531  mmons/thumb/5/51
+000003a0: 2f49 4d65 7373 6167 655f 6c6f 676f 2e73  /IMessage_logo.s
+000003b0: 7667 2f32 3034 3870 782d 494d 6573 7361  vg/2048px-IMessa
+000003c0: 6765 5f6c 6f67 6f2e 7376 672e 706e 6722  ge_logo.svg.png"
+000003d0: 2077 6964 7468 3d22 3830 7078 223e 3c62   width="80px"><b
+000003e0: 722f 3e70 7273 6d73 703c 2f68 313e 0a3c  r/>prsmsp</h1>.<
+000003f0: 2f64 6976 3e0a 3c70 2061 6c69 676e 3d22  /div>.<p align="
+00000400: 6365 6e74 6572 223e 203c 6120 6872 6566  center"> <a href
+00000410: 3d22 6874 7470 733a 2f2f 7072 736d 7370  ="https://prsmsp
+00000420: 2e72 6561 6474 6865 646f 6373 2e69 6f22  .readthedocs.io"
+00000430: 2074 6172 6765 743d 225f 626c 616e 6b22   target="_blank"
+00000440: 3e3c 696d 6720 616c 743d 2222 2073 7263  ><img alt="" src
+00000450: 3d22 6874 7470 733a 2f2f 696d 672e 7368  ="https://img.sh
+00000460: 6965 6c64 732e 696f 2f62 6164 6765 2f57  ields.io/badge/W
+00000470: 6562 7369 7465 2d45 4134 4338 393f 7374  ebsite-EA4C89?st
+00000480: 796c 653d 6e6f 726d 616c 266c 6f67 6f3d  yle=normal&logo=
+00000490: 6472 6962 6262 6c65 266c 6f67 6f43 6f6c  dribbble&logoCol
+000004a0: 6f72 3d77 6869 7465 2220 7374 796c 653d  or=white" style=
+000004b0: 2276 6572 7469 6361 6c2d 616c 6967 6e3a  "vertical-align:
+000004c0: 6365 6e74 6572 2220 2f3e 3c2f 613e 0a20  center" /></a>. 
+000004d0: 2020 200a 2020 200a 2320 4465 7363 7269     .   .# Descri
+000004e0: 7074 696f 6e0a 5079 7468 6f6e 204c 6962  ption.Python Lib
+000004f0: 7261 7279 2066 6f72 2073 656e 6469 6e67  rary for sending
+00000500: 2053 4d53 2077 6974 6820 7375 7070 6f72   SMS with suppor
+00000510: 7465 6420 534d 5320 7365 7276 6963 6520  ted SMS service 
+00000520: 7072 6f76 6964 6572 732c 2054 6869 7320  providers, This 
+00000530: 7072 6f6a 6563 7420 776f 726b 7320 6173  project works as
+00000540: 2061 6e20 4150 4920 6265 7477 6565 6e20   an API between 
+00000550: 796f 7520 616e 6420 796f 7572 2053 4d53  you and your SMS
+00000560: 2070 726f 7669 6465 722c 2072 6561 6420   provider, read 
+00000570: 6d6f 7265 2061 626f 7574 2074 6869 7320  more about this 
+00000580: 7072 6f6a 6563 7420 6174 205b 5265 6164  project at [Read
+00000590: 2054 6865 2044 6f63 735d 2868 7474 7073   The Docs](https
+000005a0: 3a2f 2f70 7273 6d73 702e 7265 6164 7468  ://prsmsp.readth
+000005b0: 6564 6f63 732e 696f 2f29 2e0a 0a3c 6272  edocs.io/)...<br
+000005c0: 3e0a 0a23 2046 6561 7475 7265 730a 5768  >..# Features.Wh
+000005d0: 656e 2079 6f75 2075 7365 2061 2053 4d53  en you use a SMS
+000005e0: 2070 616e 656c 2066 726f 6d20 6120 7072   panel from a pr
+000005f0: 6f76 6964 6572 2c20 796f 7520 696d 706c  ovider, you impl
+00000600: 656d 656e 7420 6974 2066 726f 6d20 7a65  ement it from ze
+00000610: 726f 2c20 616e 6420 6966 2079 6f75 2077  ro, and if you w
+00000620: 616e 7420 746f 2063 6861 6e67 6520 7468  ant to change th
+00000630: 6520 7061 6e65 6c2c 2079 6f75 206e 6565  e panel, you nee
+00000640: 6420 746f 2072 6566 6163 746f 7220 616c  d to refactor al
+00000650: 6c20 6f66 2079 6f75 7220 636f 6465 2e0a  l of your code..
+00000660: 616e 6420 666f 7220 696d 706c 656d 656e  and for implemen
+00000670: 7469 6e67 2061 2070 616e 656c 2066 726f  ting a panel fro
+00000680: 6d20 7a65 726f 2079 6f75 206e 6565 6420  m zero you need 
+00000690: 7469 6d65 2074 6f20 7265 6164 2074 6865  time to read the
+000006a0: 6972 2064 6f63 756d 656e 7420 616e 6420  ir document and 
+000006b0: 7472 7920 746f 2075 7365 2069 7420 616e  try to use it an
+000006c0: 6420 696d 706c 656d 656e 7420 6974 2e0a  d implement it..
+000006d0: 7468 6973 2070 726f 6a65 6374 2073 6176  this project sav
+000006e0: 6520 796f 7520 7469 6d65 2066 6f72 2069  e you time for i
+000006f0: 6d70 6c65 6d65 6e74 696e 6720 7061 6e65  mplementing pane
+00000700: 6c73 2061 6e64 2066 6f72 2072 6566 6163  ls and for refac
+00000710: 746f 7269 6e67 2079 6f75 7220 636f 6465  toring your code
+00000720: 2e0a 0a23 2320 5768 7920 7573 6520 7468  ...## Why use th
+00000730: 6973 2070 726f 6a65 6374 3f0a 2d20 596f  is project?.- Yo
+00000740: 7520 6861 7665 2061 6c6c 2074 6865 2066  u have all the f
+00000750: 616d 6f75 7320 616e 6420 7765 6c6c 2064  amous and well d
+00000760: 6573 6967 6e65 6420 534d 5320 7061 6e65  esigned SMS pane
+00000770: 6c73 2072 6561 6479 2074 6f20 676f 2e0a  ls ready to go..
+00000780: 2d20 596f 7520 6361 6e20 6861 7665 2073  - You can have s
+00000790: 6576 6572 616c 2053 4d53 2070 616e 656c  everal SMS panel
+000007a0: 7320 6174 2074 6865 2073 616d 6520 7469  s at the same ti
+000007b0: 6d65 2e0a 2d20 446f 6e27 7420 6e65 6564  me..- Don't need
+000007c0: 2074 6f20 6275 696c 6420 7468 6520 7768   to build the wh
+000007d0: 6565 6c20 6f66 2079 6f75 7220 6269 6379  eel of your bicy
+000007e0: 636c 6520 6561 6368 2074 696d 6520 e298  cle each time ..
+000007f0: ba2e 0a2d 2046 6173 7420 616e 6420 536d  ...- Fast and Sm
+00000800: 616c 6c0a 2d20 4561 7379 2074 6f20 696d  all.- Easy to im
+00000810: 706c 656d 656e 7420 616e 6420 7573 650a  plement and use.
+00000820: 0a3c 6272 3e0a 0a23 2053 7570 706f 7274  .<br>..# Support
+00000830: 6564 2070 616e 656c 730a 0a2a 205b 4b61  ed panels..* [Ka
+00000840: 7665 6e65 6761 725d 2868 7474 703a 2f2f  venegar](http://
+00000850: 6b61 7665 6e65 6761 722e 636f 6d29 0a2a  kavenegar.com).*
+00000860: 205b 536d 732e 6972 5d28 6874 7470 3a2f   [Sms.ir](http:/
+00000870: 2f73 6d73 2e69 7229 0a2a 205b 5765 6220  /sms.ir).* [Web 
+00000880: 6f6e 655d 2868 7474 703a 2f2f 7765 626f  one](http://webo
+00000890: 6e65 2d73 6d73 2e69 7229 0a2a 205b 4d65  ne-sms.ir).* [Me
+000008a0: 6c69 2050 6179 616d 616b 5d28 6874 7470  li Payamak](http
+000008b0: 733a 2f2f 7777 772e 6d65 6c69 7061 7961  s://www.melipaya
+000008c0: 6d61 6b2e 636f 6d29 0a2a 205b 4d65 6469  mak.com).* [Medi
+000008d0: 616e 615d 2868 7474 7073 3a2f 2f6d 6564  ana](https://med
+000008e0: 6961 6e61 2e69 7229 0a2a 205b 4768 6173  iana.ir).* [Ghas
+000008f0: 6564 616b 2053 6d73 5d28 6874 7470 733a  edak Sms](https:
+00000900: 2f2f 6768 6173 6564 616b 2e6d 6529 0a2a  //ghasedak.me).*
+00000910: 205b 4661 7261 7a20 536d 735d 2868 7474   [Faraz Sms](htt
+00000920: 7073 3a2f 2f66 6172 617a 736d 732e 636f  ps://farazsms.co
+00000930: 6d2f 290a 2a20 5b4e 696b 2053 6d73 5d28  m/).* [Nik Sms](
+00000940: 6874 7470 733a 2f2f 6e69 6b73 6d73 2e63  https://niksms.c
+00000950: 6f6d 2f29 0a2a 205b 536d 7331 5d28 6874  om/).* [Sms1](ht
+00000960: 7470 733a 2f2f 736d 7331 2e69 722f 290a  tps://sms1.ir/).
+00000970: 0a3c 6272 3e0a 0a23 2048 6f77 2074 6f20  .<br>..# How to 
+00000980: 7573 653f 0a46 6972 7374 206c 6574 7320  use?.First lets 
+00000990: 696e 7374 616c 6c20 7468 6520 7061 636b  install the pack
+000009a0: 6167 650a 6060 6073 6865 6c6c 0a70 6970  age.```shell.pip
+000009b0: 2069 6e73 7461 6c6c 2070 7273 6d73 700a   install prsmsp.
+000009c0: 6060 600a 0a54 6869 7320 626c 6f63 6b20  ```..This block 
+000009d0: 6f66 2063 6f64 6520 6973 2066 6f72 202a  of code is for *
+000009e0: 2a6b 6176 656e 6567 6172 2a2a 2073 6d73  *kavenegar** sms
+000009f0: 2070 616e 656c 2e0a 0a45 6163 6820 6f66   panel...Each of
+00000a00: 2073 6d73 2070 616e 656c 7320 6861 7320   sms panels has 
+00000a10: 6974 7320 6f77 6e20 7061 7261 6d65 7465  its own paramete
+00000a20: 7273 2e20 506c 6561 7365 2072 6561 6420  rs. Please read 
+00000a30: 7468 6569 7220 646f 6373 2066 6972 7374  their docs first
+00000a40: 2e0a 0a60 6060 7079 7468 6f6e 0a66 726f  ...```python.fro
+00000a50: 6d20 7072 736d 7370 2e70 616e 656c 7320  m prsmsp.panels 
+00000a60: 696d 706f 7274 204b 6176 656e 6567 6172  import Kavenegar
+00000a70: 0a0a 6170 695f 6b65 7920 3d20 2279 6f75  ..api_key = "you
+00000a80: 7220 6170 6920 6b65 7922 0a70 616e 656c  r api key".panel
+00000a90: 203d 204b 6176 656e 6567 6172 2861 7069   = Kavenegar(api
+00000aa0: 5f6b 6579 2920 2023 2061 7574 680a 0a72  _key)  # auth..r
+00000ab0: 6563 6570 746f 7220 3d20 2279 6f75 7220  eceptor = "your 
+00000ac0: 7265 6365 7074 6f72 220a 6d73 6720 3d20  receptor".msg = 
+00000ad0: 2279 6f75 7220 6d65 7373 6167 6522 0a70  "your message".p
+00000ae0: 616e 656c 2e73 656e 645f 736d 7328 7265  anel.send_sms(re
+00000af0: 6365 7074 6f72 2c20 6d73 6729 0a60 6060  ceptor, msg).```
+00000b00: 0a0a 2323 2323 205b 446f 6373 5d28 6874  ..#### [Docs](ht
+00000b10: 7470 733a 2f2f 7072 736d 7370 2e72 6561  tps://prsmsp.rea
+00000b20: 6474 6865 646f 6373 2e69 6f2f 656e 2f6c  dthedocs.io/en/l
+00000b30: 6174 6573 742f 7061 6e65 6c73 2f70 616e  atest/panels/pan
+00000b40: 656c 732e 6874 6d6c 290a 0a3c 6272 3e0a  els.html)..<br>.
+00000b50: 0a23 2048 6f77 2074 6f20 7375 7070 6f72  .# How to suppor
+00000b60: 7420 7468 6973 2070 726f 6a65 6374 3f0a  t this project?.
+00000b70: 666f 7220 7468 6973 2070 726f 6a65 6374  for this project
+00000b80: 2074 6f20 6265 2062 6574 7465 7220 616e   to be better an
+00000b90: 6420 6269 6767 6572 2074 6861 6e20 7768  d bigger than wh
+00000ba0: 6174 2069 7420 6973 206e 6f77 2e0a 7765  at it is now..we
+00000bb0: 206e 6565 6420 746f 2073 7570 706f 7274   need to support
+00000bc0: 206d 6f72 6520 7061 6e65 6c73 2061 6e64   more panels and
+00000bd0: 2065 7665 6e20 7465 7374 2061 2072 6561   even test a rea
+00000be0: 6c20 7365 6e64 2073 6d73 2077 6869 6368  l send sms which
+00000bf0: 206e 6565 6473 2061 2073 7562 7363 7269   needs a subscri
+00000c00: 7074 696f 6e20 666f 7220 6561 6368 2073  ption for each s
+00000c10: 6d73 2070 726f 7669 6465 7220 0a69 6620  ms provider .if 
+00000c20: 796f 7520 6861 7665 2073 7562 7320 666f  you have subs fo
+00000c30: 7220 616e 7920 736d 7320 7061 6e65 6c20  r any sms panel 
+00000c40: 6f72 2064 6f63 7320 6f66 2061 6e79 2073  or docs of any s
+00000c50: 6d73 2070 616e 656c 2061 6e64 2079 6f75  ms panel and you
+00000c60: 2074 6869 6e6b 2069 7420 776f 756c 6420   think it would 
+00000c70: 6265 2067 6f6f 6420 666f 7220 7468 6973  be good for this
+00000c80: 2070 6163 616b 6765 2074 6f20 6861 7665   pacakge to have
+00000c90: 2073 7570 706f 7274 2074 6861 7420 736d   support that sm
+00000ca0: 7320 7061 6e65 6c20 706c 6561 7365 206f  s panel please o
+00000cb0: 7065 6e20 616e 2069 7373 7565 206f 7220  pen an issue or 
+00000cc0: 636f 6e74 6163 7420 6d65 0a4d 7920 656d  contact me.My em
+00000cd0: 6169 6c20 6973 2070 616e 792e 7061 7273  ail is pany.pars
+00000ce0: 6172 6979 6168 6940 676d 6169 6c2e 636f  ariyahi@gmail.co
+00000cf0: 6d0a 0a                                  m..
```

### Comparing `prsmsp-1.4.0/prsmsp.egg-info/SOURCES.txt` & `prsmsp-1.5.0/prsmsp.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -23,9 +23,10 @@
 prsmsp/panels/farazsms.py
 prsmsp/panels/ghasedaksms.py
 prsmsp/panels/kavenegar.py
 prsmsp/panels/mediana.py
 prsmsp/panels/melipayamak.py
 prsmsp/panels/niksms.py
 prsmsp/panels/smsdotir.py
+prsmsp/panels/smsone.py
 prsmsp/panels/webonesms.py
 tests/test_app.py
```

### Comparing `prsmsp-1.4.0/setup.cfg` & `prsmsp-1.5.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = prsmsp
-version = 1.4.0
+version = 1.5.0
 author = Parsa Riyahi
 author_email = pany.parsariyahi@gmail.com
 description = Package to work with sms panels
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT License
 license_files = file: LICENSE
```

