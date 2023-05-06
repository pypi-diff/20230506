# Comparing `tmp/hypercli-0.1.7.tar.gz` & `tmp/hypercli-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypercli-0.1.7.tar", last modified: Mon Feb  6 23:52:24 2023, max compression
+gzip compressed data, was "hypercli-0.1.8.tar", last modified: Sat May  6 18:11:10 2023, max compression
```

## Comparing `hypercli-0.1.7.tar` & `hypercli-0.1.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-02-06 23:52:24.008995 hypercli-0.1.7/
--rw-rw-rw-   0        0        0     1082 2022-12-24 15:57:36.000000 hypercli-0.1.7/LICENSE
--rw-rw-rw-   0        0        0     2076 2023-02-06 23:52:24.009930 hypercli-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0     1790 2023-02-06 23:52:17.000000 hypercli-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-02-06 23:52:23.991252 hypercli-0.1.7/hypercli/
--rw-rw-rw-   0        0        0       25 2022-12-30 20:26:33.000000 hypercli-0.1.7/hypercli/__init__.py
--rw-rw-rw-   0        0        0     9821 2023-02-06 23:47:48.000000 hypercli-0.1.7/hypercli/core.py
-drwxrwxrwx   0        0        0        0 2023-02-06 23:52:24.007932 hypercli-0.1.7/hypercli.egg-info/
--rw-rw-rw-   0        0        0     2076 2023-02-06 23:52:23.000000 hypercli-0.1.7/hypercli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2023-02-06 23:52:23.000000 hypercli-0.1.7/hypercli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-06 23:52:23.000000 hypercli-0.1.7/hypercli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-12-24 19:45:36.000000 hypercli-0.1.7/hypercli.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       24 2023-02-06 23:52:23.000000 hypercli-0.1.7/hypercli.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-02-06 23:52:23.000000 hypercli-0.1.7/hypercli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       88 2022-12-24 19:57:58.000000 hypercli-0.1.7/pyproject.toml
--rw-rw-rw-   0        0        0      111 2023-02-06 23:52:24.010925 hypercli-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0      605 2023-02-06 23:50:37.000000 hypercli-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 18:11:10.962369 hypercli-0.1.8/
+-rw-rw-rw-   0        0        0     1082 2022-12-24 15:57:36.000000 hypercli-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0     2770 2023-05-06 18:11:10.962369 hypercli-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0     2484 2023-05-06 17:43:51.000000 hypercli-0.1.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-06 18:11:10.932858 hypercli-0.1.8/hypercli/
+-rw-rw-rw-   0        0        0       52 2023-05-04 13:21:59.000000 hypercli-0.1.8/hypercli/__init__.py
+-rw-rw-rw-   0        0        0    10094 2023-05-06 17:57:47.000000 hypercli-0.1.8/hypercli/core.py
+drwxrwxrwx   0        0        0        0 2023-05-06 18:11:10.961375 hypercli-0.1.8/hypercli.egg-info/
+-rw-rw-rw-   0        0        0     2770 2023-05-06 18:11:10.000000 hypercli-0.1.8/hypercli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2023-05-06 18:11:10.000000 hypercli-0.1.8/hypercli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 18:11:10.000000 hypercli-0.1.8/hypercli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-12-24 19:45:36.000000 hypercli-0.1.8/hypercli.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       24 2023-05-06 18:11:10.000000 hypercli-0.1.8/hypercli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-06 18:11:10.000000 hypercli-0.1.8/hypercli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       88 2022-12-24 19:57:58.000000 hypercli-0.1.8/pyproject.toml
+-rw-rw-rw-   0        0        0      111 2023-05-06 18:11:10.968376 hypercli-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0      605 2023-05-06 17:49:57.000000 hypercli-0.1.8/setup.py
```

### Comparing `hypercli-0.1.7/LICENSE` & `hypercli-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `hypercli-0.1.7/PKG-INFO` & `hypercli-0.1.8/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,130 +1,156 @@
-00000000: 4d65 7461 6461 7461 2d56 6572 7369 6f6e  Metadata-Version
-00000010: 3a20 322e 310d 0a4e 616d 653a 2068 7970  : 2.1..Name: hyp
-00000020: 6572 636c 690d 0a56 6572 7369 6f6e 3a20  ercli..Version: 
-00000030: 302e 312e 370d 0a53 756d 6d61 7279 3a20  0.1.7..Summary: 
-00000040: 456e 6861 6e63 6564 204d 656e 7520 616e  Enhanced Menu an
-00000050: 6420 434c 4920 6765 6e65 7261 746f 720d  d CLI generator.
-00000060: 0a48 6f6d 652d 7061 6765 3a20 6874 7470  .Home-page: http
-00000070: 733a 2f2f 6769 7468 7562 2e63 6f6d 2f74  s://github.com/t
-00000080: 6865 2d68 7970 6572 6f6f 742f 6879 7065  he-hyperoot/hype
-00000090: 725f 636c 690d 0a41 7574 686f 723a 2048  r_cli..Author: H
-000000a0: 5950 3352 3030 540d 0a41 7574 686f 722d  YP3R00T..Author-
-000000b0: 656d 6169 6c3a 2063 6f6e 7461 6374 4068  email: contact@h
-000000c0: 7970 6572 6f6f 742e 6c69 7665 0d0a 4c69  yperoot.live..Li
-000000d0: 6365 6e73 653a 204d 4954 0d0a 4465 7363  cense: MIT..Desc
-000000e0: 7269 7074 696f 6e2d 436f 6e74 656e 742d  ription-Content-
-000000f0: 5479 7065 3a20 7465 7874 2f6d 6172 6b64  Type: text/markd
-00000100: 6f77 6e0d 0a4c 6963 656e 7365 2d46 696c  own..License-Fil
-00000110: 653a 204c 4943 454e 5345 0d0a 0d0a 6060  e: LICENSE....``
-00000120: 600d 0a20 5f20 2020 2020 2020 2020 2020  `.. _           
-00000130: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000140: 2020 2020 5f20 5f0d 0a7c 207c 2020 2020      _ _..| |    
-00000150: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00000160: 2020 2020 2020 2020 207c 2028 5f29 0d0a           | (_)..
-00000170: 7c20 7c5f 5f20 205f 2020 205f 205f 205f  | |__  _   _ _ _
-00000180: 5f20 2020 5f5f 5f20 5f20 5f5f 205f 5f5f  _   ___ _ __ ___
-00000190: 7c20 7c5f 0d0a 7c20 275f 205c 7c20 7c20  | |_..| '_ \| | 
-000001a0: 7c20 7c20 275f 205c 202f 205f 205c 2027  | | '_ \ / _ \ '
-000001b0: 5f5f 2f20 5f5f 7c20 7c20 7c0d 0a7c 207c  __/ __| | |..| |
-000001c0: 207c 207c 207c 5f7c 207c 207c 5f29 207c   | | |_| | |_) |
-000001d0: 2020 5f5f 2f20 7c20 7c20 285f 5f7c 207c    __/ | | (__| |
-000001e0: 207c 0d0a 7c5f 7c20 7c5f 7c5c 5f5f 2c20   |..|_| |_|\__, 
-000001f0: 7c20 2e5f 5f2f 205c 5f5f 5f7c 5f7c 2020  | .__/ \___|_|  
-00000200: 5c5f 5f5f 7c5f 7c5f 7c0d 0a20 2020 2020  \___|_|_|..     
-00000210: 2020 205f 5f2f 207c 207c 0d0a 2020 2020     __/ | |..    
-00000220: 2020 207c 5f5f 5f2f 7c5f 7c20 2020 2020     |___/|_|     
-00000230: 2020 2020 2020 2020 2020 7620 302e 312e            v 0.1.
-00000240: 370d 0a60 6060 0d0a 0d0a 0d0a 2320 6879  7..```......# hy
-00000250: 7065 7263 6c69 0d0a 0d0a 6068 7970 6572  percli....`hyper
-00000260: 636c 6960 2069 7320 6120 5079 7468 6f6e  cli` is a Python
-00000270: 206c 6962 7261 7279 2066 6f72 2063 7265   library for cre
-00000280: 6174 696e 6720 6120 676f 6f64 206c 6f6f  ating a good loo
-00000290: 6b69 6e67 2063 6f6d 6d61 6e64 206c 696e  king command lin
-000002a0: 6520 696e 7465 7266 6163 652e 2050 7269  e interface. Pri
-000002b0: 6d61 7269 6c79 2069 7420 6361 6e20 6765  marily it can ge
-000002c0: 6e65 7261 7465 206d 656e 7520 7769 7468  nerate menu with
-000002d0: 2076 6572 7920 7369 6d70 6c65 2073 7465   very simple ste
-000002e0: 7073 2e20 5765 2063 616e 2061 6c73 6f20  ps. We can also 
-000002f0: 6372 6561 7465 2073 6f6d 6520 6261 6e6e  create some bann
-00000300: 6572 7320 6173 2077 656c 6c2e 2045 7665  ers as well. Eve
-00000310: 7279 7468 696e 6720 6f6e 6520 6e65 6564  rything one need
-00000320: 2074 6f20 6372 6561 7465 2063 7265 6174   to create creat
-00000330: 6520 696e 7465 7261 6374 6976 6520 636f  e interactive co
-00000340: 6d6d 616e 6420 6c69 6e65 2069 6e74 6572  mmand line inter
-00000350: 6661 6365 2e20 0d0a 0d0a 2323 2049 6e73  face. ....## Ins
-00000360: 7461 6c6c 6174 696f 6e0d 0a0d 0a55 7365  tallation....Use
-00000370: 2074 6865 2070 6163 6b61 6765 206d 616e   the package man
-00000380: 6167 6572 205b 7069 705d 2868 7474 7073  ager [pip](https
-00000390: 3a2f 2f70 7970 692e 6f72 672f 7072 6f6a  ://pypi.org/proj
-000003a0: 6563 742f 6879 7065 7263 6c69 2f29 2074  ect/hypercli/) t
-000003b0: 6f20 696e 7374 616c 6c20 6068 7970 6572  o install `hyper
-000003c0: 636c 6960 2e0d 0a0d 0a60 6060 6261 7368  cli`.....```bash
-000003d0: 0d0a 7069 7020 696e 7374 616c 6c20 6879  ..pip install hy
-000003e0: 7065 7263 6c69 0d0a 6060 600d 0a0d 0a23  percli..```....#
-000003f0: 2320 4465 6d6f 6e73 7472 6174 696f 6e0d  # Demonstration.
-00000400: 0a0d 0a60 6060 7079 7468 6f6e 0d0a 6672  ...```python..fr
-00000410: 6f6d 2068 7970 6572 636c 6920 696d 706f  om hypercli impo
-00000420: 7274 2063 6c69 0d0a 696d 706f 7274 2077  rt cli..import w
-00000430: 6562 6272 6f77 7365 720d 0a0d 0a0d 0a64  ebbrowser......d
-00000440: 6566 2061 7574 686f 725f 6e61 6d65 2829  ef author_name()
-00000450: 3a0d 0a20 2020 2070 7269 6e74 2822 4859  :..    print("HY
-00000460: 5033 5230 3054 2229 0d0a 0d0a 0d0a 6465  P3R00T")......de
-00000470: 6620 6f70 656e 5f77 6562 7369 7465 2829  f open_website()
-00000480: 3a0d 0a20 2020 2077 6562 6272 6f77 7365  :..    webbrowse
-00000490: 722e 6f70 656e 2822 6874 7470 733a 2f2f  r.open("https://
-000004a0: 6879 7065 726f 6f74 2e6c 6976 6522 290d  hyperoot.live").
-000004b0: 0a0d 0a0d 0a68 7970 6572 203d 2063 6c69  .....hyper = cli
-000004c0: 2829 0d0a 0d0a 6879 7065 722e 6372 6561  ()....hyper.crea
-000004d0: 7465 5f62 616e 6e65 7228 2268 7970 6572  te_banner("hyper
-000004e0: 636c 6922 290d 0a68 7970 6572 2e63 7265  cli")..hyper.cre
-000004f0: 6174 655f 696e 7472 6f28 2249 6e74 726f  ate_intro("Intro
-00000500: 222c 2022 416e 2065 6c65 6761 6e74 2073  ", "An elegant s
-00000510: 6f6c 7574 696f 6e20 746f 2069 6e74 6572  olution to inter
-00000520: 6163 745c 6e20 7769 7468 2063 6f6d 6d61  act\n with comma
-00000530: 6e64 206c 696e 6520 746f 6f6c 7322 290d  nd line tools").
-00000540: 0a0d 0a68 7970 6572 2e63 7265 6174 655f  ...hyper.create_
-00000550: 6d65 6e75 2822 4d61 696e 204d 656e 7522  menu("Main Menu"
-00000560: 2c20 2245 6e74 6572 2079 6f75 7220 6368  , "Enter your ch
-00000570: 6f69 6365 2229 0d0a 6879 7065 722e 6164  oice")..hyper.ad
-00000580: 645f 6f70 7469 6f6e 2822 4d61 696e 204d  d_option("Main M
-00000590: 656e 7522 2c20 2243 6865 636b 6f75 7420  enu", "Checkout 
-000005a0: 7468 6520 5375 6220 4d65 6e75 222c 2022  the Sub Menu", "
-000005b0: 5375 6220 4d65 6e75 2229 0d0a 6879 7065  Sub Menu")..hype
-000005c0: 722e 6164 645f 6f70 7469 6f6e 2822 4d61  r.add_option("Ma
-000005d0: 696e 204d 656e 7522 2c20 2250 7269 6e74  in Menu", "Print
-000005e0: 2041 7574 686f 7220 4e61 6d65 222c 2061   Author Name", a
-000005f0: 7574 686f 725f 6e61 6d65 290d 0a0d 0a68  uthor_name)....h
-00000600: 7970 6572 2e63 7265 6174 655f 6d65 6e75  yper.create_menu
-00000610: 2822 5375 6220 4d65 6e75 222c 2022 456e  ("Sub Menu", "En
-00000620: 7465 7220 796f 7572 2063 686f 6963 6522  ter your choice"
-00000630: 290d 0a68 7970 6572 2e61 6464 5f6f 7074  )..hyper.add_opt
-00000640: 696f 6e28 2253 7562 204d 656e 7522 2c20  ion("Sub Menu", 
-00000650: 2247 6f20 4261 636b 2074 6f20 4d61 696e  "Go Back to Main
-00000660: 204d 656e 7522 2c20 224d 6169 6e20 4d65   Menu", "Main Me
-00000670: 6e75 2229 0d0a 6879 7065 722e 6164 645f  nu")..hyper.add_
-00000680: 6f70 7469 6f6e 2822 5375 6220 4d65 6e75  option("Sub Menu
-00000690: 222c 2022 4368 6563 6b6f 7574 2074 6865  ", "Checkout the
-000006a0: 2057 6562 7369 7465 2028 6879 7065 726f   Website (hypero
-000006b0: 6f74 2e6c 6976 6529 222c 206f 7065 6e5f  ot.live)", open_
-000006c0: 7765 6273 6974 6529 0d0a 0d0a 7265 7370  website)....resp
-000006d0: 6f6e 7365 203d 2068 7970 6572 2e73 686f  onse = hyper.sho
-000006e0: 775f 636c 6928 290d 0a72 6573 706f 6e73  w_cli()..respons
-000006f0: 6528 290d 0a60 6060 0d0a 0d0a 215b 5d28  e()..```....![](
-00000700: 646f 6373 2f61 7373 6573 7473 2f62 6173  docs/assests/bas
-00000710: 6963 5f64 656d 6f2e 6769 6629 0d0a 0d0a  ic_demo.gif)....
-00000720: 2323 2043 6f6e 7472 6962 7574 696e 670d  ## Contributing.
-00000730: 0a0d 0a50 756c 6c20 7265 7175 6573 7473  ...Pull requests
-00000740: 2061 7265 2077 656c 636f 6d65 2e20 466f   are welcome. Fo
-00000750: 7220 6d61 6a6f 7220 6368 616e 6765 732c  r major changes,
-00000760: 2070 6c65 6173 6520 6f70 656e 2061 6e20   please open an 
-00000770: 6973 7375 6520 6669 7273 7420 746f 2064  issue first to d
-00000780: 6973 6375 7373 2077 6861 7420 796f 7520  iscuss what you 
-00000790: 776f 756c 6420 6c69 6b65 2074 6f20 6368  would like to ch
-000007a0: 616e 6765 2e0d 0a0d 0a50 6c65 6173 6520  ange.....Please 
-000007b0: 6d61 6b65 2073 7572 6520 746f 2075 7064  make sure to upd
-000007c0: 6174 6520 7465 7374 7320 6173 2061 7070  ate tests as app
-000007d0: 726f 7072 6961 7465 2e0d 0a0d 0a23 2320  ropriate.....## 
-000007e0: 4c69 6365 6e73 650d 0a0d 0a5b 4d49 545d  License....[MIT]
-000007f0: 2868 7474 7073 3a2f 2f63 686f 6f73 6561  (https://choosea
-00000800: 6c69 6365 6e73 652e 636f 6d2f 6c69 6365  license.com/lice
-00000810: 6e73 6573 2f6d 6974 2f29 0d0a            nses/mit/)..
+00000000: 6060 600d 0a20 5f20 2020 2020 2020 2020  ```.. _         
+00000010: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000020: 2020 2020 2020 5f20 5f0d 0a7c 207c 2020        _ _..| |  
+00000030: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00000040: 2020 2020 2020 2020 2020 207c 2028 5f29             | (_)
+00000050: 0d0a 7c20 7c5f 5f20 205f 2020 205f 205f  ..| |__  _   _ _
+00000060: 205f 5f20 2020 5f5f 5f20 5f20 5f5f 205f   __   ___ _ __ _
+00000070: 5f5f 7c20 7c5f 0d0a 7c20 275f 205c 7c20  __| |_..| '_ \| 
+00000080: 7c20 7c20 7c20 275f 205c 202f 205f 205c  | | | '_ \ / _ \
+00000090: 2027 5f5f 2f20 5f5f 7c20 7c20 7c0d 0a7c   '__/ __| | |..|
+000000a0: 207c 207c 207c 207c 5f7c 207c 207c 5f29   | | | |_| | |_)
+000000b0: 207c 2020 5f5f 2f20 7c20 7c20 285f 5f7c   |  __/ | | (__|
+000000c0: 207c 207c 0d0a 7c5f 7c20 7c5f 7c5c 5f5f   | |..|_| |_|\__
+000000d0: 2c20 7c20 2e5f 5f2f 205c 5f5f 5f7c 5f7c  , | .__/ \___|_|
+000000e0: 2020 5c5f 5f5f 7c5f 7c5f 7c0d 0a20 2020    \___|_|_|..   
+000000f0: 2020 2020 205f 5f2f 207c 207c 0d0a 2020       __/ | |..  
+00000100: 2020 2020 207c 5f5f 5f2f 7c5f 7c20 2020       |___/|_|   
+00000110: 2020 2020 2020 2020 2020 2020 7620 302e              v 0.
+00000120: 312e 380d 0a60 6060 0d0a 0d0a 2320 6879  1.8..```....# hy
+00000130: 7065 7263 6c69 0d0a 0d0a 2a2a 6879 7065  percli....**hype
+00000140: 7263 6c69 2a2a 2069 7320 6120 5079 7468  rcli** is a Pyth
+00000150: 6f6e 2070 6163 6b61 6765 2074 6861 7420  on package that 
+00000160: 7072 6f76 6964 6573 2061 6e20 656c 6567  provides an eleg
+00000170: 616e 7420 736f 6c75 7469 6f6e 2066 6f72  ant solution for
+00000180: 2069 6e74 6572 6163 7469 6e67 2077 6974   interacting wit
+00000190: 6820 636f 6d6d 616e 6420 6c69 6e65 2074  h command line t
+000001a0: 6f6f 6c73 2e20 4974 206f 6666 6572 7320  ools. It offers 
+000001b0: 6120 6d65 6e75 2d62 6173 6564 2063 6f6d  a menu-based com
+000001c0: 6d61 6e64 206c 696e 6520 696e 7465 7266  mand line interf
+000001d0: 6163 6520 2843 4c49 2920 7468 6174 2061  ace (CLI) that a
+000001e0: 6c6c 6f77 7320 7573 6572 7320 746f 206e  llows users to n
+000001f0: 6176 6967 6174 6520 7468 726f 7567 6820  avigate through 
+00000200: 6469 6666 6572 656e 7420 6f70 7469 6f6e  different option
+00000210: 7320 616e 6420 6578 6563 7574 6520 6675  s and execute fu
+00000220: 6e63 7469 6f6e 7320 6261 7365 6420 6f6e  nctions based on
+00000230: 2074 6865 6972 2063 686f 6963 6573 2e0d   their choices..
+00000240: 0a0d 0a23 2320 4665 6174 7572 6573 0d0a  ...## Features..
+00000250: 0d0a 2d20 496e 7465 7261 6374 6976 6520  ..- Interactive 
+00000260: 6d65 6e75 2d62 6173 6564 2043 4c49 0d0a  menu-based CLI..
+00000270: 2d20 4375 7374 6f6d 697a 6162 6c65 2062  - Customizable b
+00000280: 616e 6e65 7273 2061 6e64 2069 6e74 726f  anners and intro
+00000290: 730d 0a2d 2053 7570 706f 7274 2066 6f72  s..- Support for
+000002a0: 2064 6966 6665 7265 6e74 2076 6973 7561   different visua
+000002b0: 6c20 7374 796c 6573 2061 6e64 2063 6f6c  l styles and col
+000002c0: 6f72 730d 0a2d 2045 6173 7920 696e 7465  ors..- Easy inte
+000002d0: 6772 6174 696f 6e20 7769 7468 2065 7869  gration with exi
+000002e0: 7374 696e 6720 5079 7468 6f6e 2073 6372  sting Python scr
+000002f0: 6970 7473 0d0a 0d0a 2323 2049 6e73 7461  ipts....## Insta
+00000300: 6c6c 6174 696f 6e0d 0a0d 0a59 6f75 2063  llation....You c
+00000310: 616e 2069 6e73 7461 6c6c 202a 2a68 7970  an install **hyp
+00000320: 6572 636c 692a 2a20 7573 696e 6720 7069  ercli** using pi
+00000330: 702e 204f 7065 6e20 796f 7572 2074 6572  p. Open your ter
+00000340: 6d69 6e61 6c20 616e 6420 7275 6e20 7468  minal and run th
+00000350: 6520 666f 6c6c 6f77 696e 6720 636f 6d6d  e following comm
+00000360: 616e 643a 0d0a 0d0a 6060 600d 0a70 6970  and:....```..pip
+00000370: 2069 6e73 7461 6c6c 2068 7970 6572 636c   install hypercl
+00000380: 690d 0a60 6060 0d0a 0d0a 2323 2055 7361  i..```....## Usa
+00000390: 6765 0d0a 0d0a 546f 2075 7365 202a 2a68  ge....To use **h
+000003a0: 7970 6572 636c 692a 2a2c 2069 6d70 6f72  ypercli**, impor
+000003b0: 7420 7468 6520 6063 6c69 6020 6d6f 6475  t the `cli` modu
+000003c0: 6c65 2066 726f 6d20 7468 6520 6068 7970  le from the `hyp
+000003d0: 6572 636c 6960 2070 6163 6b61 6765 2061  ercli` package a
+000003e0: 6e64 2063 7265 6174 6520 616e 2069 6e73  nd create an ins
+000003f0: 7461 6e63 6520 6f66 2074 6865 2060 636c  tance of the `cl
+00000400: 6960 2063 6c61 7373 2e20 596f 7520 6361  i` class. You ca
+00000410: 6e20 7468 656e 2064 6566 696e 6520 796f  n then define yo
+00000420: 7572 206d 656e 7573 2c20 6f70 7469 6f6e  ur menus, option
+00000430: 732c 2061 6e64 2066 756e 6374 696f 6e73  s, and functions
+00000440: 2074 6f20 6265 2065 7865 6375 7465 642e   to be executed.
+00000450: 2046 696e 616c 6c79 2c20 6361 6c6c 2074   Finally, call t
+00000460: 6865 2060 7368 6f77 5f63 6c69 2829 6020  he `show_cli()` 
+00000470: 6d65 7468 6f64 2074 6f20 7374 6172 7420  method to start 
+00000480: 7468 6520 434c 4920 696e 7465 7266 6163  the CLI interfac
+00000490: 652e 0d0a 0d0a 4865 7265 2773 2061 6e20  e.....Here's an 
+000004a0: 6578 616d 706c 6520 6f66 2068 6f77 2074  example of how t
+000004b0: 6f20 7573 6520 2a2a 6879 7065 7263 6c69  o use **hypercli
+000004c0: 2a2a 3a0d 0a0d 0a60 6060 7079 7468 6f6e  **:....```python
+000004d0: 0d0a 6672 6f6d 2068 7970 6572 636c 6920  ..from hypercli 
+000004e0: 696d 706f 7274 2063 6c69 0d0a 696d 706f  import cli..impo
+000004f0: 7274 2077 6562 6272 6f77 7365 720d 0a0d  rt webbrowser...
+00000500: 0a64 6566 2061 7574 686f 725f 6e61 6d65  .def author_name
+00000510: 2829 3a0d 0a20 2020 2070 7269 6e74 2822  ():..    print("
+00000520: 4859 5033 5230 3054 2229 0d0a 0d0a 6465  HYP3R00T")....de
+00000530: 6620 6f70 656e 5f77 6562 7369 7465 2829  f open_website()
+00000540: 3a0d 0a20 2020 2077 6562 6272 6f77 7365  :..    webbrowse
+00000550: 722e 6f70 656e 2822 6874 7470 733a 2f2f  r.open("https://
+00000560: 6879 7065 726f 6f74 2e64 6576 2229 0d0a  hyperoot.dev")..
+00000570: 0d0a 6465 6620 6772 6565 7428 6e61 6d65  ..def greet(name
+00000580: 293a 0d0a 2020 2020 7072 696e 7428 6622  ):..    print(f"
+00000590: 4865 6c6c 6f2c 207b 6e61 6d65 7d21 2229  Hello, {name}!")
+000005a0: 0d0a 0d0a 6879 7065 7220 3d20 636c 6928  ....hyper = cli(
+000005b0: 290d 0a0d 0a68 7970 6572 2e63 7265 6174  )....hyper.creat
+000005c0: 655f 6261 6e6e 6572 2822 6879 7065 7263  e_banner("hyperc
+000005d0: 6c69 2229 0d0a 6879 7065 722e 6372 6561  li")..hyper.crea
+000005e0: 7465 5f69 6e74 726f 2822 496e 7472 6f22  te_intro("Intro"
+000005f0: 2c20 2241 6e20 656c 6567 616e 7420 736f  , "An elegant so
+00000600: 6c75 7469 6f6e 2074 6f20 696e 7465 7261  lution to intera
+00000610: 6374 5c6e 2077 6974 6820 636f 6d6d 616e  ct\n with comman
+00000620: 6420 6c69 6e65 2074 6f6f 6c73 2229 0d0a  d line tools")..
+00000630: 0d0a 6879 7065 722e 6372 6561 7465 5f6d  ..hyper.create_m
+00000640: 656e 7528 224d 6169 6e20 4d65 6e75 222c  enu("Main Menu",
+00000650: 2022 456e 7465 7220 796f 7572 2063 686f   "Enter your cho
+00000660: 6963 6522 290d 0a68 7970 6572 2e61 6464  ice")..hyper.add
+00000670: 5f6f 7074 696f 6e28 224d 6169 6e20 4d65  _option("Main Me
+00000680: 6e75 222c 2022 4368 6563 6b6f 7574 2074  nu", "Checkout t
+00000690: 6865 2053 7562 204d 656e 7522 2c20 2253  he Sub Menu", "S
+000006a0: 7562 204d 656e 7522 290d 0a68 7970 6572  ub Menu")..hyper
+000006b0: 2e61 6464 5f6f 7074 696f 6e28 224d 6169  .add_option("Mai
+000006c0: 6e20 4d65 6e75 222c 2022 4772 6565 7422  n Menu", "Greet"
+000006d0: 2c20 6772 6565 742c 2022 4a6f 686e 2229  , greet, "John")
+000006e0: 0d0a 6879 7065 722e 6164 645f 6f70 7469  ..hyper.add_opti
+000006f0: 6f6e 2822 4d61 696e 204d 656e 7522 2c20  on("Main Menu", 
+00000700: 2250 7269 6e74 2041 7574 686f 7220 4e61  "Print Author Na
+00000710: 6d65 222c 2061 7574 686f 725f 6e61 6d65  me", author_name
+00000720: 290d 0a0d 0a68 7970 6572 2e63 7265 6174  )....hyper.creat
+00000730: 655f 6d65 6e75 2822 5375 6220 4d65 6e75  e_menu("Sub Menu
+00000740: 222c 2022 456e 7465 7220 796f 7572 2063  ", "Enter your c
+00000750: 686f 6963 6522 290d 0a68 7970 6572 2e61  hoice")..hyper.a
+00000760: 6464 5f6f 7074 696f 6e28 2253 7562 204d  dd_option("Sub M
+00000770: 656e 7522 2c20 2247 6f20 4261 636b 2074  enu", "Go Back t
+00000780: 6f20 4d61 696e 204d 656e 7522 2c20 224d  o Main Menu", "M
+00000790: 6169 6e20 4d65 6e75 2229 0d0a 6879 7065  ain Menu")..hype
+000007a0: 722e 6164 645f 6f70 7469 6f6e 2822 5375  r.add_option("Su
+000007b0: 6220 4d65 6e75 222c 2022 4368 6563 6b6f  b Menu", "Checko
+000007c0: 7574 2074 6865 2057 6562 7369 7465 2028  ut the Website (
+000007d0: 6879 7065 726f 6f74 2e64 6576 2922 2c20  hyperoot.dev)", 
+000007e0: 6f70 656e 5f77 6562 7369 7465 290d 0a0d  open_website)...
+000007f0: 0a72 6573 706f 6e73 6520 3d20 6879 7065  .response = hype
+00000800: 722e 7368 6f77 5f63 6c69 2829 0d0a 6060  r.show_cli()..``
+00000810: 600d 0a0d 0a54 6865 2061 626f 7665 2073  `....The above s
+00000820: 6372 6970 7420 6465 6d6f 6e73 7472 6174  cript demonstrat
+00000830: 6573 2074 6865 2075 7361 6765 206f 6620  es the usage of 
+00000840: 2a2a 6879 7065 7263 6c69 2a2a 2e20 4974  **hypercli**. It
+00000850: 2063 7265 6174 6573 2061 2043 4c49 2077   creates a CLI w
+00000860: 6974 6820 7477 6f20 6d65 6e75 733a 2022  ith two menus: "
+00000870: 4d61 696e 204d 656e 7522 2061 6e64 2022  Main Menu" and "
+00000880: 5375 6220 4d65 6e75 222e 2045 6163 6820  Sub Menu". Each 
+00000890: 6d65 6e75 2068 6173 2069 7473 206f 776e  menu has its own
+000008a0: 206f 7074 696f 6e73 2061 6e64 2066 756e   options and fun
+000008b0: 6374 696f 6e73 2074 6f20 6265 2065 7865  ctions to be exe
+000008c0: 6375 7465 642e 2059 6f75 2063 616e 2063  cuted. You can c
+000008d0: 7573 746f 6d69 7a65 2074 6865 206d 656e  ustomize the men
+000008e0: 7573 2c20 6f70 7469 6f6e 732c 2061 6e64  us, options, and
+000008f0: 2076 6973 7561 6c20 7374 796c 6573 2061   visual styles a
+00000900: 6363 6f72 6469 6e67 2074 6f20 796f 7572  ccording to your
+00000910: 2072 6571 7569 7265 6d65 6e74 732e 0d0a   requirements...
+00000920: 0d0a 2323 204c 6963 656e 7365 0d0a 0d0a  ..## License....
+00000930: 5468 6973 2070 726f 6a65 6374 2069 7320  This project is 
+00000940: 6c69 6365 6e73 6564 2075 6e64 6572 2074  licensed under t
+00000950: 6865 204d 4954 204c 6963 656e 7365 2e20  he MIT License. 
+00000960: 5365 6520 7468 6520 5b4d 4954 5d28 6874  See the [MIT](ht
+00000970: 7470 733a 2f2f 6368 6f6f 7365 616c 6963  tps://choosealic
+00000980: 656e 7365 2e63 6f6d 2f6c 6963 656e 7365  ense.com/license
+00000990: 732f 6d69 742f 2920 6669 6c65 2066 6f72  s/mit/) file for
+000009a0: 206d 6f72 6520 696e 666f 726d 6174 696f   more informatio
+000009b0: 6e2e 0d0a                                n...
```

### Comparing `hypercli-0.1.7/hypercli/core.py` & `hypercli-0.1.8/hypercli/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -76,23 +76,25 @@
         self.visual[f"{menu_name}"] = {}
         self.visual[f"{menu_name}"]["context_color"] = context_color
         self.visual[f"{menu_name}"]["option_color"] = option_color
         self.visual[f"{menu_name}"]["exit_color"] = exit_color
         self.visual[f"{menu_name}"]["show_border"] = show_border
         self.visual[f"{menu_name}"]["show_exit"] = show_exit
 
-    def add_option(self, menu_name, option, function=None):
+    def add_option(self, menu_name, option, function=None, *args, **kwargs):
         """
         It adds an option to a menu
         
         :param menu_name: The name of the menu you want to add the option to
         :param option: The name of the option to add to the menu
         :param function: The function to be called when the option is selected
+        :param args: Additional positional arguments for the function
+        :param kwargs: Additional keyword arguments for the function
         """
-        self.menu[menu_name][option] = function
+        self.menu[menu_name][option] = (function, args, kwargs)
 
     def show_cli(self, menu_name=None):
         """
         It prints a menu to the console
         
         :param menu_name: The name of the menu to show
         :return: The return value is the value of the option that was selected.
@@ -134,26 +136,28 @@
         :param show_exit: If True, the user can exit the menu by entering 0
         :return: The return value is the function that is being called.
         """
         choice = input("\u279D ")
         for (index, (k, v)) in enumerate(self.menu[menu_name].items()):
             if int(choice) <= len(self.menu[menu_name]):
                 if int(choice) == index + 1:
-                    if isinstance(v, str):
-                        return self.show_cli(v)
-                    elif v != None:
-                        return v
+                    function, args, kwargs = v
+                    if isinstance(function, str):
+                        return self.show_cli(function)
+                    elif function is not None:
+                        return function(*args, **kwargs)
                     else:
                         return self.common_func.error()
                 elif int(choice) == 0 and show_exit == True:
                     return self.common_func.exit()
             else:
                 return self.common_func.error()
 
 
+
 class Banner:
     def __init__(self, banner, figlet_font, banner_color, justify) -> None:
         """
         This function is used to print a banner in the terminal
         
         :param banner: The text you want to display
         :param figlet_font: The font you want to use
```

### Comparing `hypercli-0.1.7/setup.py` & `hypercli-0.1.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("./README.md", "r") as readme:
     desc = readme.read()
 
 setuptools.setup(
     name="hypercli",
-    version="0.1.7",
+    version="0.1.8",
     author="HYP3R00T",
     author_email="contact@hyperoot.live",
     description="Enhanced Menu and CLI generator",
     url="https://github.com/the-hyperoot/hyper_cli",
     long_description=desc,
     long_description_content_type='text/markdown',
     license='MIT',
```

