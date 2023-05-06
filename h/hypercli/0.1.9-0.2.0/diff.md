# Comparing `tmp/hypercli-0.1.9.tar.gz` & `tmp/hypercli-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hypercli-0.1.9.tar", last modified: Sat May  6 18:18:44 2023, max compression
+gzip compressed data, was "hypercli-0.2.0.tar", last modified: Sat May  6 18:30:47 2023, max compression
```

## Comparing `hypercli-0.1.9.tar` & `hypercli-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-06 18:18:44.279898 hypercli-0.1.9/
--rw-rw-rw-   0        0        0     1082 2022-12-24 15:57:36.000000 hypercli-0.1.9/LICENSE
--rw-rw-rw-   0        0        0     2837 2023-05-06 18:18:44.279898 hypercli-0.1.9/PKG-INFO
--rw-rw-rw-   0        0        0     2551 2023-05-06 18:15:31.000000 hypercli-0.1.9/README.md
-drwxrwxrwx   0        0        0        0 2023-05-06 18:18:44.229134 hypercli-0.1.9/hypercli/
--rw-rw-rw-   0        0        0       52 2023-05-04 13:21:59.000000 hypercli-0.1.9/hypercli/__init__.py
--rw-rw-rw-   0        0        0    10094 2023-05-06 17:57:47.000000 hypercli-0.1.9/hypercli/core.py
-drwxrwxrwx   0        0        0        0 2023-05-06 18:18:44.277898 hypercli-0.1.9/hypercli.egg-info/
--rw-rw-rw-   0        0        0     2837 2023-05-06 18:18:44.000000 hypercli-0.1.9/hypercli.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      279 2023-05-06 18:18:44.000000 hypercli-0.1.9/hypercli.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-06 18:18:44.000000 hypercli-0.1.9/hypercli.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-12-24 19:45:36.000000 hypercli-0.1.9/hypercli.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       24 2023-05-06 18:18:44.000000 hypercli-0.1.9/hypercli.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-06 18:18:44.000000 hypercli-0.1.9/hypercli.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       88 2022-12-24 19:57:58.000000 hypercli-0.1.9/pyproject.toml
--rw-rw-rw-   0        0        0      111 2023-05-06 18:18:44.281892 hypercli-0.1.9/setup.cfg
--rw-rw-rw-   0        0        0      605 2023-05-06 18:15:40.000000 hypercli-0.1.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 18:30:47.327772 hypercli-0.2.0/
+-rw-rw-rw-   0        0        0     1082 2022-12-24 15:57:36.000000 hypercli-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     2875 2023-05-06 18:30:47.328723 hypercli-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2589 2023-05-06 18:29:54.000000 hypercli-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-06 18:30:47.307437 hypercli-0.2.0/hypercli/
+-rw-rw-rw-   0        0        0       52 2023-05-04 13:21:59.000000 hypercli-0.2.0/hypercli/__init__.py
+-rw-rw-rw-   0        0        0    10094 2023-05-06 17:57:47.000000 hypercli-0.2.0/hypercli/core.py
+drwxrwxrwx   0        0        0        0 2023-05-06 18:30:47.327772 hypercli-0.2.0/hypercli.egg-info/
+-rw-rw-rw-   0        0        0     2875 2023-05-06 18:30:47.000000 hypercli-0.2.0/hypercli.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      279 2023-05-06 18:30:47.000000 hypercli-0.2.0/hypercli.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 18:30:47.000000 hypercli-0.2.0/hypercli.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-12-24 19:45:36.000000 hypercli-0.2.0/hypercli.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       24 2023-05-06 18:30:47.000000 hypercli-0.2.0/hypercli.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-06 18:30:47.000000 hypercli-0.2.0/hypercli.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       88 2022-12-24 19:57:58.000000 hypercli-0.2.0/pyproject.toml
+-rw-rw-rw-   0        0        0      111 2023-05-06 18:30:47.329722 hypercli-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      605 2023-05-06 18:30:23.000000 hypercli-0.2.0/setup.py
```

### Comparing `hypercli-0.1.9/LICENSE` & `hypercli-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hypercli-0.1.9/PKG-INFO` & `hypercli-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypercli
-Version: 0.1.9
+Version: 0.2.0
 Summary: Enhanced Menu and CLI generator
 Home-page: https://github.com/the-hyperoot/hyper_cli
 Author: HYP3R00T
 Author-email: contact@hyperoot.live
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -13,15 +13,15 @@
  _                               _ _
 | |                             | (_)
 | |__  _   _ _ __   ___ _ __ ___| |_
 | '_ \| | | | '_ \ / _ \ '__/ __| | |
 | | | | |_| | |_) |  __/ | | (__| | |
 |_| |_|\__, | .__/ \___|_|  \___|_|_|
         __/ | |
-       |___/|_|               v 0.1.9
+       |___/|_|               v 0.2.0
 ```
 
 # hypercli
 
 **hypercli** is a Python package that provides an elegant solution for interacting with command line tools. It offers a menu-based command line interface (CLI) that allows users to navigate through different options and execute functions based on their choices.
 
 ## Features
@@ -71,12 +71,14 @@
 hyper.create_menu("Sub Menu", "Enter your choice")
 hyper.add_option("Sub Menu", "Go Back to Main Menu", "Main Menu")
 hyper.add_option("Sub Menu", "Checkout the Website (hyperoot.dev)", open_website)
 
 response = hyper.show_cli()
 ```
 
+![](docs/assests/example_demo.gif)
+
 The above script demonstrates the usage of **hypercli**. It creates a CLI with two menus: "Main Menu" and "Sub Menu". Each menu has its own options and functions to be executed. You can customize the menus, options, and visual styles according to your requirements. To check out more complex example, refer to `Example_revamped.py`.
 
 ## License
 
 This project is licensed under the MIT License. See the [MIT](https://choosealicense.com/licenses/mit/) file for more information.
```

### Comparing `hypercli-0.1.9/README.md` & `hypercli-0.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 000000b0: 207c 2020 5f5f 2f20 7c20 7c20 285f 5f7c   |  __/ | | (__|
 000000c0: 207c 207c 0d0a 7c5f 7c20 7c5f 7c5c 5f5f   | |..|_| |_|\__
 000000d0: 2c20 7c20 2e5f 5f2f 205c 5f5f 5f7c 5f7c  , | .__/ \___|_|
 000000e0: 2020 5c5f 5f5f 7c5f 7c5f 7c0d 0a20 2020    \___|_|_|..   
 000000f0: 2020 2020 205f 5f2f 207c 207c 0d0a 2020       __/ | |..  
 00000100: 2020 2020 207c 5f5f 5f2f 7c5f 7c20 2020       |___/|_|   
 00000110: 2020 2020 2020 2020 2020 2020 7620 302e              v 0.
-00000120: 312e 390d 0a60 6060 0d0a 0d0a 2320 6879  1.9..```....# hy
+00000120: 322e 300d 0a60 6060 0d0a 0d0a 2320 6879  2.0..```....# hy
 00000130: 7065 7263 6c69 0d0a 0d0a 2a2a 6879 7065  percli....**hype
 00000140: 7263 6c69 2a2a 2069 7320 6120 5079 7468  rcli** is a Pyth
 00000150: 6f6e 2070 6163 6b61 6765 2074 6861 7420  on package that 
 00000160: 7072 6f76 6964 6573 2061 6e20 656c 6567  provides an eleg
 00000170: 616e 7420 736f 6c75 7469 6f6e 2066 6f72  ant solution for
 00000180: 2069 6e74 6572 6163 7469 6e67 2077 6974   interacting wit
 00000190: 6820 636f 6d6d 616e 6420 6c69 6e65 2074  h command line t
@@ -123,38 +123,40 @@
 000007a0: 722e 6164 645f 6f70 7469 6f6e 2822 5375  r.add_option("Su
 000007b0: 6220 4d65 6e75 222c 2022 4368 6563 6b6f  b Menu", "Checko
 000007c0: 7574 2074 6865 2057 6562 7369 7465 2028  ut the Website (
 000007d0: 6879 7065 726f 6f74 2e64 6576 2922 2c20  hyperoot.dev)", 
 000007e0: 6f70 656e 5f77 6562 7369 7465 290d 0a0d  open_website)...
 000007f0: 0a72 6573 706f 6e73 6520 3d20 6879 7065  .response = hype
 00000800: 722e 7368 6f77 5f63 6c69 2829 0d0a 6060  r.show_cli()..``
-00000810: 600d 0a0d 0a54 6865 2061 626f 7665 2073  `....The above s
-00000820: 6372 6970 7420 6465 6d6f 6e73 7472 6174  cript demonstrat
-00000830: 6573 2074 6865 2075 7361 6765 206f 6620  es the usage of 
-00000840: 2a2a 6879 7065 7263 6c69 2a2a 2e20 4974  **hypercli**. It
-00000850: 2063 7265 6174 6573 2061 2043 4c49 2077   creates a CLI w
-00000860: 6974 6820 7477 6f20 6d65 6e75 733a 2022  ith two menus: "
-00000870: 4d61 696e 204d 656e 7522 2061 6e64 2022  Main Menu" and "
-00000880: 5375 6220 4d65 6e75 222e 2045 6163 6820  Sub Menu". Each 
-00000890: 6d65 6e75 2068 6173 2069 7473 206f 776e  menu has its own
-000008a0: 206f 7074 696f 6e73 2061 6e64 2066 756e   options and fun
-000008b0: 6374 696f 6e73 2074 6f20 6265 2065 7865  ctions to be exe
-000008c0: 6375 7465 642e 2059 6f75 2063 616e 2063  cuted. You can c
-000008d0: 7573 746f 6d69 7a65 2074 6865 206d 656e  ustomize the men
-000008e0: 7573 2c20 6f70 7469 6f6e 732c 2061 6e64  us, options, and
-000008f0: 2076 6973 7561 6c20 7374 796c 6573 2061   visual styles a
-00000900: 6363 6f72 6469 6e67 2074 6f20 796f 7572  ccording to your
-00000910: 2072 6571 7569 7265 6d65 6e74 732e 2054   requirements. T
-00000920: 6f20 6368 6563 6b20 6f75 7420 6d6f 7265  o check out more
-00000930: 2063 6f6d 706c 6578 2065 7861 6d70 6c65   complex example
-00000940: 2c20 7265 6665 7220 746f 2060 4578 616d  , refer to `Exam
-00000950: 706c 655f 7265 7661 6d70 6564 2e70 7960  ple_revamped.py`
-00000960: 2e0d 0a0d 0a23 2320 4c69 6365 6e73 650d  .....## License.
-00000970: 0a0d 0a54 6869 7320 7072 6f6a 6563 7420  ...This project 
-00000980: 6973 206c 6963 656e 7365 6420 756e 6465  is licensed unde
-00000990: 7220 7468 6520 4d49 5420 4c69 6365 6e73  r the MIT Licens
-000009a0: 652e 2053 6565 2074 6865 205b 4d49 545d  e. See the [MIT]
-000009b0: 2868 7474 7073 3a2f 2f63 686f 6f73 6561  (https://choosea
-000009c0: 6c69 6365 6e73 652e 636f 6d2f 6c69 6365  license.com/lice
-000009d0: 6e73 6573 2f6d 6974 2f29 2066 696c 6520  nses/mit/) file 
-000009e0: 666f 7220 6d6f 7265 2069 6e66 6f72 6d61  for more informa
-000009f0: 7469 6f6e 2e0d 0a                        tion...
+00000810: 600d 0a0d 0a21 5b5d 2864 6f63 732f 6173  `....![](docs/as
+00000820: 7365 7374 732f 6578 616d 706c 655f 6465  sests/example_de
+00000830: 6d6f 2e67 6966 290d 0a0d 0a54 6865 2061  mo.gif)....The a
+00000840: 626f 7665 2073 6372 6970 7420 6465 6d6f  bove script demo
+00000850: 6e73 7472 6174 6573 2074 6865 2075 7361  nstrates the usa
+00000860: 6765 206f 6620 2a2a 6879 7065 7263 6c69  ge of **hypercli
+00000870: 2a2a 2e20 4974 2063 7265 6174 6573 2061  **. It creates a
+00000880: 2043 4c49 2077 6974 6820 7477 6f20 6d65   CLI with two me
+00000890: 6e75 733a 2022 4d61 696e 204d 656e 7522  nus: "Main Menu"
+000008a0: 2061 6e64 2022 5375 6220 4d65 6e75 222e   and "Sub Menu".
+000008b0: 2045 6163 6820 6d65 6e75 2068 6173 2069   Each menu has i
+000008c0: 7473 206f 776e 206f 7074 696f 6e73 2061  ts own options a
+000008d0: 6e64 2066 756e 6374 696f 6e73 2074 6f20  nd functions to 
+000008e0: 6265 2065 7865 6375 7465 642e 2059 6f75  be executed. You
+000008f0: 2063 616e 2063 7573 746f 6d69 7a65 2074   can customize t
+00000900: 6865 206d 656e 7573 2c20 6f70 7469 6f6e  he menus, option
+00000910: 732c 2061 6e64 2076 6973 7561 6c20 7374  s, and visual st
+00000920: 796c 6573 2061 6363 6f72 6469 6e67 2074  yles according t
+00000930: 6f20 796f 7572 2072 6571 7569 7265 6d65  o your requireme
+00000940: 6e74 732e 2054 6f20 6368 6563 6b20 6f75  nts. To check ou
+00000950: 7420 6d6f 7265 2063 6f6d 706c 6578 2065  t more complex e
+00000960: 7861 6d70 6c65 2c20 7265 6665 7220 746f  xample, refer to
+00000970: 2060 4578 616d 706c 655f 7265 7661 6d70   `Example_revamp
+00000980: 6564 2e70 7960 2e0d 0a0d 0a23 2320 4c69  ed.py`.....## Li
+00000990: 6365 6e73 650d 0a0d 0a54 6869 7320 7072  cense....This pr
+000009a0: 6f6a 6563 7420 6973 206c 6963 656e 7365  oject is license
+000009b0: 6420 756e 6465 7220 7468 6520 4d49 5420  d under the MIT 
+000009c0: 4c69 6365 6e73 652e 2053 6565 2074 6865  License. See the
+000009d0: 205b 4d49 545d 2868 7474 7073 3a2f 2f63   [MIT](https://c
+000009e0: 686f 6f73 6561 6c69 6365 6e73 652e 636f  hoosealicense.co
+000009f0: 6d2f 6c69 6365 6e73 6573 2f6d 6974 2f29  m/licenses/mit/)
+00000a00: 2066 696c 6520 666f 7220 6d6f 7265 2069   file for more i
+00000a10: 6e66 6f72 6d61 7469 6f6e 2e0d 0a         nformation...
```

### Comparing `hypercli-0.1.9/hypercli/core.py` & `hypercli-0.2.0/hypercli/core.py`

 * *Files identical despite different names*

### Comparing `hypercli-0.1.9/hypercli.egg-info/PKG-INFO` & `hypercli-0.2.0/hypercli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hypercli
-Version: 0.1.9
+Version: 0.2.0
 Summary: Enhanced Menu and CLI generator
 Home-page: https://github.com/the-hyperoot/hyper_cli
 Author: HYP3R00T
 Author-email: contact@hyperoot.live
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -13,15 +13,15 @@
  _                               _ _
 | |                             | (_)
 | |__  _   _ _ __   ___ _ __ ___| |_
 | '_ \| | | | '_ \ / _ \ '__/ __| | |
 | | | | |_| | |_) |  __/ | | (__| | |
 |_| |_|\__, | .__/ \___|_|  \___|_|_|
         __/ | |
-       |___/|_|               v 0.1.9
+       |___/|_|               v 0.2.0
 ```
 
 # hypercli
 
 **hypercli** is a Python package that provides an elegant solution for interacting with command line tools. It offers a menu-based command line interface (CLI) that allows users to navigate through different options and execute functions based on their choices.
 
 ## Features
@@ -71,12 +71,14 @@
 hyper.create_menu("Sub Menu", "Enter your choice")
 hyper.add_option("Sub Menu", "Go Back to Main Menu", "Main Menu")
 hyper.add_option("Sub Menu", "Checkout the Website (hyperoot.dev)", open_website)
 
 response = hyper.show_cli()
 ```
 
+![](docs/assests/example_demo.gif)
+
 The above script demonstrates the usage of **hypercli**. It creates a CLI with two menus: "Main Menu" and "Sub Menu". Each menu has its own options and functions to be executed. You can customize the menus, options, and visual styles according to your requirements. To check out more complex example, refer to `Example_revamped.py`.
 
 ## License
 
 This project is licensed under the MIT License. See the [MIT](https://choosealicense.com/licenses/mit/) file for more information.
```

### Comparing `hypercli-0.1.9/setup.py` & `hypercli-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("./README.md", "r") as readme:
     desc = readme.read()
 
 setuptools.setup(
     name="hypercli",
-    version="0.1.9",
+    version="0.2.0",
     author="HYP3R00T",
     author_email="contact@hyperoot.live",
     description="Enhanced Menu and CLI generator",
     url="https://github.com/the-hyperoot/hyper_cli",
     long_description=desc,
     long_description_content_type='text/markdown',
     license='MIT',
```

