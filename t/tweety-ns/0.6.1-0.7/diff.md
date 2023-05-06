# Comparing `tmp/tweety-ns-0.6.1.tar.gz` & `tmp/tweety-ns-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tweety-ns-0.6.1.tar", last modified: Sat Apr  8 16:41:00 2023, max compression
+gzip compressed data, was "tweety-ns-0.7.tar", last modified: Sat May  6 13:43:03 2023, max compression
```

## Comparing `tweety-ns-0.6.1.tar` & `tweety-ns-0.7.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxrwxrwx   0 kharltayyab  (1000) kharltayyab  (1000)        0 2023-04-08 16:41:00.881770 tweety-ns-0.6.1/
--rwxrwxrwx   0 kharltayyab  (1000) kharltayyab  (1000)      995 2023-04-08 16:41:00.882073 tweety-ns-0.6.1/PKG-INFO
--rwxrwxrwx   0 kharltayyab  (1000) kharltayyab  (1000)      302 2022-10-22 17:49:03.000000 tweety-ns-0.6.1/README.md
--rwxrwxrwx   0 kharltayyab  (1000) kharltayyab  (1000)      108 2021-11-15 09:32:36.000000 tweety-ns-0.6.1/pyproject.toml
--rwxrwxrwx   0 kharltayyab  (1000) kharltayyab  (1000)      671 2023-04-08 16:41:00.883072 tweety-ns-0.6.1/setup.cfg
--rwxrwxrwx   0 kharltayyab  (1000) kharltayyab  (1000)      767 2023-04-08 16:40:37.000000 tweety-ns-0.6.1/setup.py
-drwxrwxrwx   0 kharltayyab  (1000) kharltayyab  (1000)        0 2023-04-08 16:41:00.851381 tweety-ns-0.6.1/src/
-drwxrwxrwx   0 kharltayyab  (1000) kharltayyab  (1000)        0 2023-04-08 16:41:00.866647 tweety-ns-0.6.1/src/tweety/
--rwxrwxrwx   0 kharltayyab  (1000) kharltayyab  (1000)       54 2023-04-08 16:39:18.000000 tweety-ns-0.6.1/src/tweety/__init__.py
--rwxrwxrwx   0 kharltayyab  (1000) kharltayyab  (1000)     7599 2023-02-17 05:07:11.000000 tweety-ns-0.6.1/src/tweety/bot.py
--rwxrwxrwx   0 kharltayyab  (1000) kharltayyab  (1000)    14608 2023-04-08 16:31:32.000000 tweety-ns-0.6.1/src/tweety/builder.py
--rwxrwxrwx   0 kharltayyab  (1000) kharltayyab  (1000)    18861 2023-02-16 11:46:04.000000 tweety-ns-0.6.1/src/tweety/exceptions_.py
--rwxrwxrwx   0 kharltayyab  (1000) kharltayyab  (1000)      282 2022-03-04 06:53:48.000000 tweety-ns-0.6.1/src/tweety/filters.py
--rwxrwxrwx   0 kharltayyab  (1000) kharltayyab  (1000)     2261 2023-04-03 14:41:39.000000 tweety-ns-0.6.1/src/tweety/http.py
-drwxrwxrwx   0 kharltayyab  (1000) kharltayyab  (1000)        0 2023-04-08 16:41:00.873328 tweety-ns-0.6.1/src/tweety/types/
--rwxrwxrwx   0 kharltayyab  (1000) kharltayyab  (1000)       58 2023-03-12 12:43:32.000000 tweety-ns-0.6.1/src/tweety/types/__init__.py
--rwxrwxrwx   0 kharltayyab  (1000) kharltayyab  (1000)     4906 2023-04-03 14:44:27.000000 tweety-ns-0.6.1/src/tweety/types/search.py
--rwxrwxrwx   0 kharltayyab  (1000) kharltayyab  (1000)    31494 2023-04-08 16:37:09.000000 tweety-ns-0.6.1/src/tweety/types/twDataTypes.py
--rwxrwxrwx   0 kharltayyab  (1000) kharltayyab  (1000)     3271 2023-04-03 14:44:51.000000 tweety-ns-0.6.1/src/tweety/types/usertweet.py
--rwxrwxrwx   0 kharltayyab  (1000) kharltayyab  (1000)       96 2023-03-13 06:35:02.000000 tweety-ns-0.6.1/src/tweety/utils.py
-drwxrwxrwx   0 kharltayyab  (1000) kharltayyab  (1000)        0 2023-04-08 16:41:00.880563 tweety-ns-0.6.1/src/tweety_ns.egg-info/
--rwxrwxrwx   0 kharltayyab  (1000) kharltayyab  (1000)      995 2023-04-08 16:41:00.000000 tweety-ns-0.6.1/src/tweety_ns.egg-info/PKG-INFO
--rwxrwxrwx   0 kharltayyab  (1000) kharltayyab  (1000)      495 2023-04-08 16:41:00.000000 tweety-ns-0.6.1/src/tweety_ns.egg-info/SOURCES.txt
--rwxrwxrwx   0 kharltayyab  (1000) kharltayyab  (1000)        1 2023-04-08 16:41:00.000000 tweety-ns-0.6.1/src/tweety_ns.egg-info/dependency_links.txt
--rwxrwxrwx   0 kharltayyab  (1000) kharltayyab  (1000)       40 2023-04-08 16:41:00.000000 tweety-ns-0.6.1/src/tweety_ns.egg-info/requires.txt
--rwxrwxrwx   0 kharltayyab  (1000) kharltayyab  (1000)        7 2023-04-08 16:41:00.000000 tweety-ns-0.6.1/src/tweety_ns.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-06 13:43:03.005410 tweety-ns-0.7/
+-rw-rw-rw-   0        0        0     1017 2023-05-06 13:43:03.005410 tweety-ns-0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      302 2022-10-22 17:49:03.000000 tweety-ns-0.7/README.md
+-rw-rw-rw-   0        0        0      108 2021-11-15 09:32:36.000000 tweety-ns-0.7/pyproject.toml
+-rw-rw-rw-   0        0        0      699 2023-05-06 13:43:03.007511 tweety-ns-0.7/setup.cfg
+-rw-rw-rw-   0        0        0      782 2023-05-06 10:32:37.000000 tweety-ns-0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:43:02.980972 tweety-ns-0.7/src/
+drwxrwxrwx   0        0        0        0 2023-05-06 13:43:02.991439 tweety-ns-0.7/src/tweety/
+-rw-rw-rw-   0        0        0       52 2023-05-06 10:37:02.000000 tweety-ns-0.7/src/tweety/__init__.py
+-rw-rw-rw-   0        0        0     7069 2023-05-06 13:18:33.000000 tweety-ns-0.7/src/tweety/bot.py
+-rw-rw-rw-   0        0        0    15562 2023-04-24 21:35:55.000000 tweety-ns-0.7/src/tweety/builder.py
+-rw-rw-rw-   0        0        0    18251 2023-04-24 18:05:20.000000 tweety-ns-0.7/src/tweety/exceptions_.py
+-rw-rw-rw-   0        0        0      282 2022-03-04 06:53:48.000000 tweety-ns-0.7/src/tweety/filters.py
+-rw-rw-rw-   0        0        0     5347 2023-05-06 13:19:25.000000 tweety-ns-0.7/src/tweety/http.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:43:02.998535 tweety-ns-0.7/src/tweety/types/
+-rw-rw-rw-   0        0        0       58 2023-03-12 12:43:32.000000 tweety-ns-0.7/src/tweety/types/__init__.py
+-rw-rw-rw-   0        0        0     2145 2023-04-24 19:05:27.000000 tweety-ns-0.7/src/tweety/types/n_types.py
+-rw-rw-rw-   0        0        0     4929 2023-04-24 20:14:22.000000 tweety-ns-0.7/src/tweety/types/search.py
+-rw-rw-rw-   0        0        0    27837 2023-05-06 13:08:01.000000 tweety-ns-0.7/src/tweety/types/twDataTypes.py
+-rw-rw-rw-   0        0        0     3584 2023-05-06 13:10:36.000000 tweety-ns-0.7/src/tweety/types/usertweet.py
+-rw-rw-rw-   0        0        0       96 2023-03-13 06:35:02.000000 tweety-ns-0.7/src/tweety/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-06 13:43:03.004403 tweety-ns-0.7/src/tweety_ns.egg-info/
+-rw-rw-rw-   0        0        0     1017 2023-05-06 13:43:02.000000 tweety-ns-0.7/src/tweety_ns.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      523 2023-05-06 13:43:02.000000 tweety-ns-0.7/src/tweety_ns.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 13:43:02.000000 tweety-ns-0.7/src/tweety_ns.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       45 2023-05-06 13:43:02.000000 tweety-ns-0.7/src/tweety_ns.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-06 13:43:02.000000 tweety-ns-0.7/src/tweety_ns.egg-info/top_level.txt
```

### Comparing `tweety-ns-0.6.1/PKG-INFO` & `tweety-ns-0.7/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1
-Name: tweety-ns
-Version: 0.6.1
-Summary: An easy Twitter Scraper
-Home-page: https://github.com/mahrtayyab/tweety
-Author: Tayyab Kharl
-Author-email: tayyabmahr@gmail.com
-License: MIT
-Project-URL: Bug Tracker, https://github.com/mahrtayyab/tweety/issues
-Project-URL: Documentation, https://github.com/mahrtayyab/tweety
-Keywords: TWITTER,TWITTER SCRAPE,SCRAPE TWEETS
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
-# tweety
-Twitter's API is annoying to work with, and has lots of limitations — luckily their frontend (JavaScript) has it's own API, which I reverse–engineered. No API rate limits. No restrictions.
-
-## Documentation:
-You can check documentation at  [here](https://mahrtayyab.github.io/tweety_docs/)
+Metadata-Version: 2.1
+Name: tweety-ns
+Version: 0.7
+Summary: An easy Twitter Scraper
+Home-page: https://github.com/mahrtayyab/tweety
+Author: Tayyab Kharl
+Author-email: tayyabmahr@gmail.com
+License: MIT
+Project-URL: Bug Tracker, https://github.com/mahrtayyab/tweety/issues
+Project-URL: Documentation, https://github.com/mahrtayyab/tweety
+Keywords: TWITTER,TWITTER SCRAPE,SCRAPE TWEETS
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+
+# tweety
+Twitter's API is annoying to work with, and has lots of limitations — luckily their frontend (JavaScript) has it's own API, which I reverse–engineered. No API rate limits. No restrictions.
+
+## Documentation:
+You can check documentation at  [here](https://mahrtayyab.github.io/tweety_docs/)
```

### Comparing `tweety-ns-0.6.1/setup.cfg` & `tweety-ns-0.7/setup.cfg`

 * *Files 25% similar despite different names*

```diff
@@ -1,42 +1,44 @@
-00000000: 5b6d 6574 6164 6174 615d 0a6e 616d 6520  [metadata].name 
-00000010: 3d20 7477 6565 7479 2d6e 730a 7665 7273  = tweety-ns.vers
-00000020: 696f 6e20 3d20 302e 362e 310a 6175 7468  ion = 0.6.1.auth
-00000030: 6f72 203d 2054 6179 7961 6220 4b68 6172  or = Tayyab Khar
-00000040: 6c0a 6175 7468 6f72 5f65 6d61 696c 203d  l.author_email =
-00000050: 2074 6179 7961 626d 6168 7240 676d 6169   tayyabmahr@gmai
-00000060: 6c2e 636f 6d0a 6465 7363 7269 7074 696f  l.com.descriptio
-00000070: 6e20 3d20 416e 2065 6173 7920 5477 6974  n = An easy Twit
-00000080: 7465 7220 5363 7261 7065 720a 6c6f 6e67  ter Scraper.long
-00000090: 5f64 6573 6372 6970 7469 6f6e 203d 2066  _description = f
-000000a0: 696c 653a 2052 4541 444d 452e 6d64 0a6c  ile: README.md.l
-000000b0: 6f6e 675f 6465 7363 7269 7074 696f 6e5f  ong_description_
-000000c0: 636f 6e74 656e 745f 7479 7065 203d 2074  content_type = t
-000000d0: 6578 742f 6d61 726b 646f 776e 0a75 726c  ext/markdown.url
-000000e0: 203d 2068 7474 7073 3a2f 2f67 6974 6875   = https://githu
-000000f0: 622e 636f 6d2f 6d61 6872 7461 7979 6162  b.com/mahrtayyab
-00000100: 2f74 7765 6574 790a 7072 6f6a 6563 745f  /tweety.project_
-00000110: 7572 6c73 203d 200a 0942 7567 2054 7261  urls = ..Bug Tra
-00000120: 636b 6572 203d 2068 7474 7073 3a2f 2f67  cker = https://g
-00000130: 6974 6875 622e 636f 6d2f 6d61 6872 7461  ithub.com/mahrta
-00000140: 7979 6162 2f74 7765 6574 792f 6973 7375  yyab/tweety/issu
-00000150: 6573 0a09 446f 6375 6d65 6e74 6174 696f  es..Documentatio
-00000160: 6e20 3d20 6874 7470 733a 2f2f 6769 7468  n = https://gith
-00000170: 7562 2e63 6f6d 2f6d 6168 7274 6179 7961  ub.com/mahrtayya
-00000180: 622f 7477 6565 7479 0a63 6c61 7373 6966  b/tweety.classif
-00000190: 6965 7273 203d 200a 0950 726f 6772 616d  iers = ..Program
-000001a0: 6d69 6e67 204c 616e 6775 6167 6520 3a3a  ming Language ::
-000001b0: 2050 7974 686f 6e20 3a3a 2033 0a09 4c69   Python :: 3..Li
-000001c0: 6365 6e73 6520 3a3a 204f 5349 2041 7070  cense :: OSI App
-000001d0: 726f 7665 6420 3a3a 204d 4954 204c 6963  roved :: MIT Lic
-000001e0: 656e 7365 0a09 4f70 6572 6174 696e 6720  ense..Operating 
-000001f0: 5379 7374 656d 203a 3a20 4f53 2049 6e64  System :: OS Ind
-00000200: 6570 656e 6465 6e74 0a0a 5b6f 7074 696f  ependent..[optio
-00000210: 6e73 5d0a 7061 636b 6167 655f 6469 7220  ns].package_dir 
-00000220: 3d20 0a09 3d20 7372 630a 7061 636b 6167  = ..= src.packag
-00000230: 6573 203d 2066 696e 643a 0a70 7974 686f  es = find:.pytho
-00000240: 6e5f 7265 7175 6972 6573 203d 203e 3d33  n_requires = >=3
-00000250: 2e36 0a0a 5b6f 7074 696f 6e73 2e70 6163  .6..[options.pac
-00000260: 6b61 6765 732e 6669 6e64 5d0a 7768 6572  kages.find].wher
-00000270: 6520 3d20 7372 630a 0a5b 6567 675f 696e  e = src..[egg_in
-00000280: 666f 5d0a 7461 675f 6275 696c 6420 3d20  fo].tag_build = 
-00000290: 0a74 6167 5f64 6174 6520 3d20 300a 0a    .tag_date = 0..
+00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
+00000010: 203d 2074 7765 6574 792d 6e73 0d0a 7665   = tweety-ns..ve
+00000020: 7273 696f 6e20 3d20 302e 370d 0a61 7574  rsion = 0.7..aut
+00000030: 686f 7220 3d20 5461 7979 6162 204b 6861  hor = Tayyab Kha
+00000040: 726c 0d0a 6175 7468 6f72 5f65 6d61 696c  rl..author_email
+00000050: 203d 2074 6179 7961 626d 6168 7240 676d   = tayyabmahr@gm
+00000060: 6169 6c2e 636f 6d0d 0a64 6573 6372 6970  ail.com..descrip
+00000070: 7469 6f6e 203d 2041 6e20 6561 7379 2054  tion = An easy T
+00000080: 7769 7474 6572 2053 6372 6170 6572 0d0a  witter Scraper..
+00000090: 6c6f 6e67 5f64 6573 6372 6970 7469 6f6e  long_description
+000000a0: 203d 2066 696c 653a 2052 4541 444d 452e   = file: README.
+000000b0: 6d64 0d0a 6c6f 6e67 5f64 6573 6372 6970  md..long_descrip
+000000c0: 7469 6f6e 5f63 6f6e 7465 6e74 5f74 7970  tion_content_typ
+000000d0: 6520 3d20 7465 7874 2f6d 6172 6b64 6f77  e = text/markdow
+000000e0: 6e0d 0a75 726c 203d 2068 7474 7073 3a2f  n..url = https:/
+000000f0: 2f67 6974 6875 622e 636f 6d2f 6d61 6872  /github.com/mahr
+00000100: 7461 7979 6162 2f74 7765 6574 790d 0a70  tayyab/tweety..p
+00000110: 726f 6a65 6374 5f75 726c 7320 3d20 0d0a  roject_urls = ..
+00000120: 0942 7567 2054 7261 636b 6572 203d 2068  .Bug Tracker = h
+00000130: 7474 7073 3a2f 2f67 6974 6875 622e 636f  ttps://github.co
+00000140: 6d2f 6d61 6872 7461 7979 6162 2f74 7765  m/mahrtayyab/twe
+00000150: 6574 792f 6973 7375 6573 0d0a 0944 6f63  ety/issues...Doc
+00000160: 756d 656e 7461 7469 6f6e 203d 2068 7474  umentation = htt
+00000170: 7073 3a2f 2f67 6974 6875 622e 636f 6d2f  ps://github.com/
+00000180: 6d61 6872 7461 7979 6162 2f74 7765 6574  mahrtayyab/tweet
+00000190: 790d 0a63 6c61 7373 6966 6965 7273 203d  y..classifiers =
+000001a0: 200d 0a09 5072 6f67 7261 6d6d 696e 6720   ...Programming 
+000001b0: 4c61 6e67 7561 6765 203a 3a20 5079 7468  Language :: Pyth
+000001c0: 6f6e 203a 3a20 330d 0a09 4c69 6365 6e73  on :: 3...Licens
+000001d0: 6520 3a3a 204f 5349 2041 7070 726f 7665  e :: OSI Approve
+000001e0: 6420 3a3a 204d 4954 204c 6963 656e 7365  d :: MIT License
+000001f0: 0d0a 094f 7065 7261 7469 6e67 2053 7973  ...Operating Sys
+00000200: 7465 6d20 3a3a 204f 5320 496e 6465 7065  tem :: OS Indepe
+00000210: 6e64 656e 740d 0a0d 0a5b 6f70 7469 6f6e  ndent....[option
+00000220: 735d 0d0a 7061 636b 6167 655f 6469 7220  s]..package_dir 
+00000230: 3d20 0d0a 093d 2073 7263 0d0a 7061 636b  = ...= src..pack
+00000240: 6167 6573 203d 2066 696e 643a 0d0a 7079  ages = find:..py
+00000250: 7468 6f6e 5f72 6571 7569 7265 7320 3d20  thon_requires = 
+00000260: 3e3d 332e 360d 0a0d 0a5b 6f70 7469 6f6e  >=3.6....[option
+00000270: 732e 7061 636b 6167 6573 2e66 696e 645d  s.packages.find]
+00000280: 0d0a 7768 6572 6520 3d20 7372 630d 0a0d  ..where = src...
+00000290: 0a5b 6567 675f 696e 666f 5d0d 0a74 6167  .[egg_info]..tag
+000002a0: 5f62 7569 6c64 203d 200d 0a74 6167 5f64  _build = ..tag_d
+000002b0: 6174 6520 3d20 300d 0a0d 0a              ate = 0....
```

### Comparing `tweety-ns-0.6.1/setup.py` & `tweety-ns-0.7/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 from distutils.core import setup
 
 setup(
     name='tweety-ns',
     packages=['tweety', 'tweety.types'],
-    version='0.6.1',
+    version='0.7',
     license='MIT',
     description='An easy Twitter Scraper',
     author='Tayyab Kharl',
     author_email='tayyabmahr@gmail.com',
     url='https://github.com/mahrtayyab/tweety',
     keywords=['TWITTER', 'TWITTER SCRAPE', 'SCRAPE TWEETS'],
     install_requires=[
         'beautifulsoup4',
         'openpyxl',
         'httpx',
-        'dateutils'
+        'dateutils',
+        'tqdm'
     ],
     classifiers=[
         'Development Status :: 4 - Beta',
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Build Tools',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3'
```

### Comparing `tweety-ns-0.6.1/src/tweety/bot.py` & `tweety-ns-0.7/src/tweety/bot.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,130 +1,110 @@
 import functools
+from typing import Union
+
+from .types.n_types import Proxy
 from .exceptions_ import *
 from .http import Request
 from .types.usertweet import UserTweets
 from .types.search import Search
 from .types.twDataTypes import User, Trends, Tweet
 
 
-def valid_profile(f):
+def AuthRequired(f):
     @functools.wraps(f)
     def wrapper(self, *args, **kwargs):
-        if self.profile_url is None:
-            raise ValueError("No Username Provided , Please initiate the class using a username or profile URL")
-
-        if self.user.protected:
-            username = self.profile_url.split("/")[-1]
-            raise UserProtected(f"User {username} is Protected")
+        if self.user is None:
+            raise AuthenticationRequired(200, "GenericForbidden", None)
 
-        try:
-            return f(self, *args, **kwargs)
-        except (UserProtected, UserNotFound) as e:
-            raise e
-        except Exception as e:
-            raise UnknownError(e)
+        return f(self, *args, **kwargs)
 
     return wrapper
 
 
 class Twitter:
-    def __init__(self, profile_name: str = None, max_retires: int = 10, proxy: dict = None):
+    def __init__(self, max_retires: int = 10, proxy: Union[dict, Proxy] = None, cookies: Union[str, dict] = None):
         """
-        Initialize the Twitter Class
+        Constructor of the Twitter Public class
 
-        :param profile_name: (`str`) Profile URL or The Username of the user you are dealing with
         :param max_retires: (`int`) Number of retries the script would make , if the guest token wasn't found
-        :param proxy: (`dict`) Provide the proxy you want to use while making a request
+        :param proxy: (`dict` or `Proxy`) Provide the proxy you want to use while making a request
+        :param cookies: (`str` or `dict`) Cookies which will be used for user authentication
         """
-        if profile_name:
-            if profile_name.startswith("https://"):
-                self.profile_url = profile_name
-            else:
-                self.profile_url = f"https://twitter.com/{profile_name}"
-        else:
-            self.profile_url = None
 
-        if proxy and proxy is not None:
-            if proxy.get("http") and proxy.get("https"):
-                self.proxy = dict(http=proxy['http'], https=proxy['https'])
-            else:
-                raise ProxyParseError()
-        else:
-            self.proxy = None
+        self.request = Request(max_retries=max_retires, proxy=proxy, cookies=cookies)
+        self.user = self.get_user_info() if cookies is not None else None
 
-        self.request = Request(self.profile_url, max_retries=max_retires, proxy=self.proxy)
-        self.user = self.get_user_info() if self.profile_url is not None else None
-
-    def __verify_user(self):
+    def get_user_info(self, username: str = None, banner_extensions: bool = False, image_extensions: bool = False):
         """
-        Protected method to Verify the User
-
-        :return: User Json
-        """
-        username = self.profile_url.split("/")[-1]
-        return self.request.verify_user(username)
-
-    def get_user_info(self, banner_extensions: bool = False, image_extensions: bool = False):
-        """
-        Get the user available info
+        Get the User Info of the specified username or ``self`` if user is authenticated using ``cookies``
 
+        :param username: (`str`) username to get information of
         :param banner_extensions: (`boolean`) Get the Banner extension on the user page
         :param image_extensions: (`boolean`) Get the Image extension on the user page
 
         :return: .types.twDataTypes.User
         """
-        if not self.profile_url:
-            raise ValueError("No Username Provided , Please initiate the class using a username or profile URL")
+        if not username:
+            if not self.user:
+                raise ValueError("You need to specify 'username' ")
 
-        user_raw = self.__verify_user()
+            return self.user
 
-        if not user_raw:
-            raise UserNotFound("User {} not Found".format(self.profile_url.split("/")[-1]))
+        user_raw = self.request.get_user(username)
 
         if not banner_extensions or banner_extensions is False:
             try:
                 del user_raw['data']['user']['result']['legacy']['profile_banner_extensions']
             except KeyError:
                 pass
 
         if not image_extensions or image_extensions is False:
             try:
                 del user_raw['data']['user']['result']['legacy']['profile_image_extensions']
             except KeyError:
                 pass
 
-        return User(user_raw)
+        return User(user_raw['data']['user']['result'])
 
     @property
     def user_id(self):
         """
         Get the user unique twitter id
 
         :return: int
         """
 
-        return self.user.rest_id
+        return self.user.rest_id if self.user else None
 
-    @valid_profile
-    def get_tweets(self, pages: int = 1, replies: bool = False, wait_time: int = 2, cursor: str = None):
+    def get_tweets(self, username: Union[str, int, User], pages: int = 1, replies: bool = False, wait_time: int = 2, cursor: str = None):
         """
         Get the tweets from a user
 
-        :param pages: (`int`) number of pages to be scraped
-        :param replies: (`boolean`) get the replied tweets of the user too
-        :param wait_time: (`int`) seconds to wait between multiple requests
-        :param cursor: Pagination cursor if you want to get the pages from that cursor up-to (This cursor is different from actual API cursor)
+        :param: username: (`str` | `int` | `User`) username of the user whom to get the tweets of
+        :param: pages: (`int`) number of pages to be scraped
+        :param: replies: (`boolean`) get the replied tweets of the user too
+        :param: wait_time: (`int`) seconds to wait between multiple requests
+        :param: cursor: Pagination cursor if you want to get the pages from that cursor up-to (This cursor is different from actual API cursor)
 
 
         :return: .types.usertweet.UserTweets
         """
         if wait_time is None:
             wait_time = 0
 
-        return UserTweets(self.user_id, self.request, pages, replies, wait_time, cursor)
+        if isinstance(username, User):
+            user_id = username.rest_id
+        elif isinstance(username, int):
+            user_id = username
+        elif isinstance(username, str) and str(username).isdigit():
+            user_id = int(username)
+        else:
+            user_id = self.get_user_info(username).rest_id
+
+        return UserTweets(user_id, self.request, pages, replies, wait_time, cursor)
 
     def get_trends(self):
         """
         Get the Trends from you locale
 
         :return:list of .types.twDataTypes.Trends
         """
@@ -141,14 +121,15 @@
                 if i['item']['content']['trend']['trendMetadata']['metaDescription']:
                     data['tweet_count'] = i['item']['content']['trend']['trendMetadata']['metaDescription']
             except:
                 pass
             trends.append(Trends(data))
         return trends
 
+    @AuthRequired
     def search(self, keyword: str, pages: int = 1, filter_: str = None, wait_time: int = 2, cursor: str = None):
         """
         Search for a keyword or hashtag on Twitter
 
         :param keyword: (`str`) The keyword which is supposed to be searched
         :param pages: (`int`) The number of pages to get
         :param filter_: (
@@ -177,20 +158,18 @@
         if str(identifier).startswith("https://"):
             if str(identifier).endswith("/"):
                 tweetId = str(identifier)[:-1].split("/")[-1]
             else:
                 tweetId = str(identifier).split("/")[-1]
         else:
             tweetId = identifier
-
         r = self.request.get_tweet_detail(tweetId)
-
         try:
-            for entry in r.json()['data']['threaded_conversation_with_injections_v2']['instructions'][0]['entries']:
+            for entry in r['data']['threaded_conversation_with_injections_v2']['instructions'][0]['entries']:
                 if str(entry['entryId']).split("-")[0] == "tweet":
                     raw_tweet = entry['content']['itemContent']['tweet_results']['result']
-                    if raw_tweet['rest_id'] == str(identifier):
+
+                    if raw_tweet['rest_id'] == str(tweetId):
                         return Tweet(r, raw_tweet, self.request, True, False, True)
 
-            raise InvalidTweetIdentifier()
         except KeyError:
-            raise InvalidTweetIdentifier()
+            raise InvalidTweetIdentifier(144, "StatusNotFound", r)
```

### Comparing `tweety-ns-0.6.1/src/tweety/builder.py` & `tweety-ns-0.7/src/tweety/builder.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,35 +4,35 @@
 from functools import wraps
 
 REQUEST_USER_AGENT = 'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/109.0.0.0 Safari/537.36'
 REQUEST_PLATFORMS = ['Linux', 'Windows']
 
 
 def return_with_headers(func):
-
     @wraps(func)
     def wrapper(self, *arg, **kw):
-        url = func(self, *arg, **kw)
-        return dict(headers=self._get_headers(), url=url)
+        method, url = func(self, *arg, **kw)
+        return dict(method=method, headers=self._get_headers(), url=url)
 
     return wrapper
 
 
 class UrlBuilder:
     URL_GUEST_TOKEN = "https://api.twitter.com/1.1/guest/activate.json"
     URL_API_INIT = "https://twitter.com/i/api/1.1/branch/init.json"
     URL_USER_BY_SCREEN_NAME = "https://api.twitter.com/graphql/rePnxwe9LZ51nQ7Sn_xN_A/UserByScreenName"
     URL_USER_TWEETS = "https://twitter.com/i/api/graphql/OXXUyHfKYZ-xLx4NcL9-_Q/UserTweets"
     URL_USER_TWEETS_WITH_REPLIES = "https://twitter.com/i/api/graphql/nrdle2catTyGnTyj1Qa7wA/UserTweetsAndReplies"
     URL_TRENDS = "https://twitter.com/i/api/2/guide.json"
     URL_SEARCH = "https://twitter.com/i/api/2/search/adaptive.json"
     URL_TWEET_DETAILS = "https://twitter.com/i/api/graphql/1oIoGPTOJN2mSjbbXlQifA/TweetDetail"
+    URL_AUSER_SETTINGS = "https://api.twitter.com/1.1/account/settings.json" # noqa
 
-    def __init__(self, profile_url):
-        self.username = profile_url.split("/")[-1] if profile_url else None
+    def __init__(self, cookies=None):
+        self.cookies = cookies
         self.user_id = None
         self.guest_token = None
 
     def _get_headers(self):
         headers = {
             'authority': 'twitter.com',
             'accept': '*/*',
@@ -48,45 +48,49 @@
             'sec-fetch-site': 'same-site',
             'user-agent': REQUEST_USER_AGENT,
             'x-csrf-token': self._get_csrf(),
             'x-twitter-active-user': 'yes',
             'x-twitter-client-language': 'en',
         }
 
-        if self.guest_token:
+        if self.guest_token or self.cookies:
             headers['content-type'] = 'application/json'
-            headers['referer'] = f'https://twitter.com/{self.username}'
+            # headers['referer'] = f'https://twitter.com/{self.username}'
             headers['sec-fetch-site'] = 'same-origin'
-            headers['x-guest-token'] = self.guest_token
+
+            if self.guest_token:
+                headers['x-guest-token'] = self.guest_token
 
         return headers
 
-    @staticmethod
-    def _get_csrf():
+    def _get_csrf(self):
+        if self.cookies and self.cookies.get("ct0"):
+            return self.cookies.get("ct0")
+
         return ''.join(random.choices(string.ascii_letters + string.digits, k=32))
 
     @staticmethod
     def _build(url, params):
         return "?".join([url, params])
 
     @return_with_headers
     def get_guest_token(self):
-        return self.URL_GUEST_TOKEN
+        return "POST", self.URL_GUEST_TOKEN
 
     @return_with_headers
     def init_api(self):
-        return self.URL_API_INIT
+        return "POST", self.URL_API_INIT
 
     @return_with_headers
     def user_by_screen_name(self, username):
         params = {
             'variables': f'{{"screen_name":"{username}","withSafetyModeUserFields":true,"withSuperFollowsUserFields":true}}',
             'features': '{"responsive_web_twitter_blue_verified_badge_is_enabled":true,"responsive_web_graphql_exclude_directive_enabled":false,"verified_phone_label_enabled":false,"responsive_web_graphql_skip_user_profile_image_extensions_enabled":false,"responsive_web_graphql_timeline_navigation_enabled":true}',
         }
-        return self._build(self.URL_USER_BY_SCREEN_NAME, urlencode(params))
+        return "GET", self._build(self.URL_USER_BY_SCREEN_NAME, urlencode(params))
 
     @return_with_headers
     def user_tweets(self, user_id, replies=False, cursor=None):
         if replies:
             if not cursor:
                 params = {
                     'variables': f'{{"userId":"{user_id}","count":40,"includePromotedContent":true,"withCommunity":true,"withSuperFollowsUserFields":true,"withDownvotePerspective":false,"withReactionsMetadata":false,"withReactionsPerspective":false,"withSuperFollowsTweetFields":true,"withVoice":true,"withV2Timeline":true}}',
@@ -105,15 +109,15 @@
                 'features': '{"responsive_web_twitter_blue_verified_badge_is_enabled":true,"responsive_web_graphql_exclude_directive_enabled":false,"verified_phone_label_enabled":false,"responsive_web_graphql_timeline_navigation_enabled":true,"responsive_web_graphql_skip_user_profile_image_extensions_enabled":false,"tweetypie_unmention_optimization_enabled":true,"vibe_api_enabled":true,"responsive_web_edit_tweet_api_enabled":true,"graphql_is_translatable_rweb_tweet_is_translatable_enabled":true,"view_counts_everywhere_api_enabled":true,"longform_notetweets_consumption_enabled":true,"tweet_awards_web_tipping_enabled":false,"freedom_of_speech_not_reach_fetch_enabled":false,"standardized_nudges_misinfo":true,"tweet_with_visibility_results_prefer_gql_limited_actions_policy_enabled":false,"interactive_text_enabled":true,"responsive_web_text_conversations_enabled":false,"responsive_web_enhance_cards_enabled":false}',
             }
         else:
             params = {
                 'variables': f'{{"userId":"{user_id}","count":40,"cursor":"{cursor}","includePromotedContent":true,"withQuickPromoteEligibilityTweetFields":true,"withSuperFollowsUserFields":true,"withDownvotePerspective":false,"withReactionsMetadata":false,"withReactionsPerspective":false,"withSuperFollowsTweetFields":true,"withVoice":true,"withV2Timeline":true}}',
                 'features': '{"responsive_web_twitter_blue_verified_badge_is_enabled":true,"responsive_web_graphql_exclude_directive_enabled":false,"verified_phone_label_enabled":false,"responsive_web_graphql_timeline_navigation_enabled":true,"responsive_web_graphql_skip_user_profile_image_extensions_enabled":false,"tweetypie_unmention_optimization_enabled":true,"vibe_api_enabled":true,"responsive_web_edit_tweet_api_enabled":true,"graphql_is_translatable_rweb_tweet_is_translatable_enabled":true,"view_counts_everywhere_api_enabled":true,"longform_notetweets_consumption_enabled":true,"tweet_awards_web_tipping_enabled":false,"freedom_of_speech_not_reach_fetch_enabled":false,"standardized_nudges_misinfo":true,"tweet_with_visibility_results_prefer_gql_limited_actions_policy_enabled":false,"interactive_text_enabled":true,"responsive_web_text_conversations_enabled":false,"responsive_web_enhance_cards_enabled":false}',
             }
-        return self._build(self.URL_USER_TWEETS, urlencode(params))
+        return "GET", self._build(self.URL_USER_TWEETS, urlencode(params))
 
     @return_with_headers
     def trends(self):
         params = {
             'include_profile_interstitial_type': '1',
             'include_blocking': '1',
             'include_blocked_by': '1',
@@ -146,15 +150,15 @@
             'count': '20',
             'requestContext': 'launch',
             'candidate_source': 'trends',
             'include_page_configuration': 'false',
             'entity_tokens': 'false',
             'ext': 'mediaStats,highlightedLabel,hasNftAvatar,voiceInfo,enrichments,superFollowMetadata,unmentionInfo,editControl,collab_control,vibe',
         }
-        return self._build(self.URL_TRENDS, urlencode(params))
+        return "GET", self._build(self.URL_TRENDS, urlencode(params))
 
     @return_with_headers
     def search(self, keyword, cursor, filter_):
         params = {
             'include_profile_interstitial_type': '1',
             'include_blocking': '1',
             'include_blocked_by': '1',
@@ -162,14 +166,15 @@
             'include_want_retweets': '1',
             'include_mute_edge': '1',
             'include_can_dm': '1',
             'include_can_media_tag': '1',
             'include_ext_has_nft_avatar': '1',
             'include_ext_is_blue_verified': '1',
             'include_ext_verified_type': '1',
+            'include_ext_profile_image_shape': '1',
             'skip_status': '1',
             'cards_platform': 'Web-12',
             'include_cards': '1',
             'include_ext_alt_text': 'true',
             'include_ext_limited_action_results': 'false',
             'include_quote_count': 'true',
             'include_reply_count': '1',
@@ -180,37 +185,52 @@
             'include_ext_media_color': 'true',
             'include_ext_media_availability': 'true',
             'include_ext_sensitive_media_warning': 'true',
             'include_ext_trusted_friends_metadata': 'true',
             'send_error_codes': 'true',
             'simple_quoted_tweet': 'true',
             'q': keyword,
-            'query_source': '',
-            'count': '20',
+            'query_source': 'typeahead_click',
+            'count': '40',
             'requestContext': 'launch',
             'pc': '1',
             'spelling_corrections': '1',
             'include_ext_edit_control': 'true',
-            'ext': 'mediaStats,highlightedLabel,hasNftAvatar,voiceInfo,enrichments,superFollowMetadata,unmentionInfo,editControl,vibe',
+            'ext': 'mediaStats,highlightedLabel,hasNftAvatar,voiceInfo,birdwatchPivot,enrichments,superFollowMetadata,unmentionInfo,editControl,vibe',
         }
 
         if filter_ and filter_ == "latest":
             params['tweet_search_mode'] = "live"
         elif filter_ and filter_ == "users":
             params['result_filter'] = "user"
         elif filter_ and filter_ == "photos":
             params['result_filter'] = "image"
         elif filter_ and filter_ == "videos":
             params['result_filter'] = "video"
 
         if cursor:
             params['cursor'] = cursor
 
-        return self._build(self.URL_SEARCH, urlencode(params))
+        return "GET", self._build(self.URL_SEARCH, urlencode(params))
 
     @return_with_headers
     def tweet_detail(self, tweet_id):
         params = {
             'variables': f'{{"focalTweetId":"{tweet_id}","with_rux_injections":false,"includePromotedContent":true,"withCommunity":true,"withQuickPromoteEligibilityTweetFields":true,"withBirdwatchNotes":true,"withDownvotePerspective":false,"withReactionsMetadata":false,"withReactionsPerspective":false,"withVoice":true,"withV2Timeline":true}}',
             'features': '{"blue_business_profile_image_shape_enabled":false,"responsive_web_graphql_exclude_directive_enabled":true,"verified_phone_label_enabled":false,"responsive_web_graphql_timeline_navigation_enabled":true,"responsive_web_graphql_skip_user_profile_image_extensions_enabled":false,"tweetypie_unmention_optimization_enabled":true,"vibe_api_enabled":true,"responsive_web_edit_tweet_api_enabled":true,"graphql_is_translatable_rweb_tweet_is_translatable_enabled":true,"view_counts_everywhere_api_enabled":true,"longform_notetweets_consumption_enabled":true,"tweet_awards_web_tipping_enabled":false,"freedom_of_speech_not_reach_fetch_enabled":false,"standardized_nudges_misinfo":true,"tweet_with_visibility_results_prefer_gql_limited_actions_policy_enabled":false,"interactive_text_enabled":true,"responsive_web_text_conversations_enabled":false,"longform_notetweets_richtext_consumption_enabled":false,"responsive_web_enhance_cards_enabled":false}',
         }
-        return self._build(self.URL_TWEET_DETAILS, urlencode(params))
+        return "GET", self._build(self.URL_TWEET_DETAILS, urlencode(params))
+
+    @return_with_headers
+    def aUser_settings(self):
+        params = {
+            'include_mention_filter': 'true',
+            'include_nsfw_user_flag': 'true',
+            'include_nsfw_admin_flag': 'true',
+            'include_ranked_timeline': 'true',
+            'include_alt_text_compose': 'true',
+            'ext': 'ssoConnections',
+            'include_country_code': 'true',
+            'include_ext_dm_nsfw_media_filter': 'true',
+            'include_ext_sharing_audiospaces_listening_data_with_followers': 'true',
+        }
+        return "GET", self._build(self.URL_AUSER_SETTINGS, urlencode(params))
```

### Comparing `tweety-ns-0.6.1/src/tweety/types/search.py` & `tweety-ns-0.7/src/tweety/types/search.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import time
+import traceback
+
 from . import Tweet, Excel, User, deprecated
 
 
 class Search(dict):
     def __init__(self, keyword, http, pages=1, filter_=None, wait_time=2, cursor=None):
         super().__init__()
         self.tweets = []
@@ -21,61 +23,61 @@
             self.filter
         )
 
     def get_next_page(self):
         _tweets = []
         if self.is_next_page:
             response = self.http.perform_search(self.keyword, self.cursor, self.filter)
-
             thisTweets = self._parse_response(response)
 
             self['is_next_page'] = self.is_next_page
             self['cursor'] = self.cursor
 
             return thisTweets
 
     def _parse_response(self, response):
         thisObjects = []
         if self.filter == "users":
-            for raw_user in response.json()['globalObjects']['users'].values():
+            for raw_user in response['globalObjects']['users'].values():
                 try:
-                    user = User(raw_user, 2)
+                    user = User(raw_user)
                     self.users.append(user)
                     thisObjects.append(user)
                 except:
                     pass
             self['users'] = self.users
         else:
-            users = response.json()['globalObjects']['users']
-            for tweet_id, raw_tweet in response.json()['globalObjects']['tweets'].items():
+            users = response['globalObjects']['users']
+            for tweet_id, raw_tweet in response['globalObjects']['tweets'].items():
                 try:
-                    raw_tweet['rest_id'], raw_tweet['core'] = tweet_id, users.get(str(raw_tweet['user_id']))
+                    raw_tweet['rest_id'], raw_tweet['author'] = tweet_id, users.get(str(raw_tweet['user_id']))
                     tweet = Tweet(response, raw_tweet, self.http, False, True)
                     self.tweets.append(tweet)
                     thisObjects.append(tweet)
                 except:
+                    traceback.print_exc()
                     pass
 
             self['tweets'] = self.tweets
 
         self.is_next_page = self._get_cursor(response)
         return thisObjects
 
     def _get_cursor(self, response):
         if self.filter == "users":
-            for i in response.json()['timeline']['instructions'][-1]['addEntries']['entries']:
+            for i in response['timeline']['instructions'][-1]['addEntries']['entries']:
                 if str(i['entryId']).split("-")[0] == "cursor":
                     if i['content']['operation']['cursor']['cursorType'] == "Bottom":
                         newCursor = i['content']['operation']['cursor']['value']
                         if newCursor == self.cursor:
                             return False
                         self.cursor = newCursor
                         return True
         else:
-            for i in response.json()['timeline']['instructions'][0]['addEntries']['entries']:
+            for i in response['timeline']['instructions'][0]['addEntries']['entries']:
                 try:
                     if i['content']['operation']:
                         if i['content']['operation']['cursor']['cursorType'] == "Bottom":
                             newCursor = i['content']['operation']['cursor']['value']
                             if newCursor == self.cursor:
                                 return False
                             self.cursor = newCursor
```

### Comparing `tweety-ns-0.6.1/src/tweety/types/twDataTypes.py` & `tweety-ns-0.7/src/tweety/types/twDataTypes.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,21 +1,28 @@
+import base64
+import os.path
+import re
 import sys
 import warnings
 from dateutil import parser
 import openpyxl
 import dateutil
 
 try:
     import wget
 except ModuleNotFoundError:
     warnings.warn(' "wget" not found in system ,you will not be able to download the medias')
 WORKBOOK_HEADERS = ['Created on', 'author', 'is_retweet', 'is_reply', 'tweet_id', 'tweet_body', 'language', 'likes',
                     'retweet_count', 'source', 'medias', 'user_mentioned', 'urls', 'hashtags', 'symbols']
 
 
+def decodeBase64(encoded_string):
+    return str(base64.b64decode(bytes(encoded_string, "utf-8")))[2:-1]
+
+
 def deprecated(func):
     """
 
     This is a decorator which can be used to mark functions
     as deprecated. It will result in a warning being emitted
     when the function is used.
 
@@ -86,89 +93,62 @@
         super().__init__()
         self.http = http
         self.__raw_response = raw_response
         self.__raw_tweet = raw_tweet
         self.__is_legacy_user = is_legacy_user
         self.__replied_to = None
         self._get_reply = get_reply
-        self.__formatted_tweet = self._format_tweet()
-        self.id = None
+        self._format_tweet()
 
         if get_threads:
             self._get_threads()
 
-        for key, value in self.__formatted_tweet.items():
-            setattr(self, key, value)
-            self[key] = value
+        for key, value in vars(self).items():
+            if not str(key).startswith("_"):
+                self[key] = value
 
     def __repr__(self):
         return f"Tweet(id={self.id}, author={self.author}, created_on={self.created_on}, threads={len(self.threads) if self.threads else None})"  # noqa
 
     def __iter__(self):
         if self.threads:  # noqa
             for thread_ in self.threads:  # noqa
                 yield thread_
 
-    @deprecated
-    def to_dict(self):
-        return self.__formatted_tweet
-
     def _format_tweet(self):
         original_tweet = self._get_original_tweet()
-        self.id = tweet_rest_id = self._get_id()
-        tweet_author = self.__raw_tweet['core']
-
-        created_on = dateutil.parser.parse(original_tweet.get("created_at"))
-        author = UserLegacy(tweet_author) if self.__is_legacy_user else User(tweet_author, 3)
-        is_retweet = self._is_retweet(original_tweet)
-        retweeted_tweet = self._get_retweeted_tweet(is_retweet,original_tweet)
-        text = self._get_tweet_text(original_tweet, is_retweet)
-        is_quoted = self._is_quoted(original_tweet)
-        quoted_tweet = self._get_quoted_tweet(is_quoted)
-        is_reply = self._is_reply(original_tweet)
-        is_sensitive = self._is_sensitive(original_tweet)
-        reply_counts = self._get_reply_counts(original_tweet)
-        quote_counts = self._get_quote_counts(original_tweet)
-        replied_to = self.__replied_to = self._get_reply_to(is_reply, original_tweet)
-        bookmark_count = self._get_bookmark_count(original_tweet)
-        vibe = self._get_vibe()
-        views = self._get_views()
-
-        return {
-            "created_on": created_on,
-            "author": author,
-            "is_quoted": is_quoted,
-            "quoted_tweet": quoted_tweet,
-            "quote_counts": quote_counts,
-            "is_retweet": is_retweet,
-            "retweeted_tweet": retweeted_tweet,
-            "is_reply": is_reply,
-            "vibe": vibe,
-            "reply_counts": reply_counts,
-            "is_possibly_sensitive": is_sensitive,
-            "id": tweet_rest_id,
-            "tweet_body": text,
-            "text": text,
-            "language": self._get_language(original_tweet),
-            "likes": self._get_likes(original_tweet),
-            "card": self._get_card(),
-            "place": self._get_place(original_tweet),
-            "retweet_counts": self._get_retweet_counts(original_tweet),
-            "source": self._get_source(self.__raw_tweet),
-            "media": self._get_tweet_media(original_tweet),
-            "user_mentions": self._get_tweet_mentions(original_tweet),
-            "urls": self._get_tweet_urls(original_tweet),
-            "hashtags": self._get_tweet_hashtags(original_tweet),
-            "symbols": self._get_tweet_symbols(original_tweet),
-            "views": views,
-            "reply_to": replied_to,
-            "bookmark_count": bookmark_count,
-            "threads": [],
-            "comments": []
-        }
+        self.id = self._get_id()
+        self.created_on = dateutil.parser.parse(original_tweet["created_at"])
+        self.author = self._get_author()
+        self.is_retweet = self._is_retweet(original_tweet)
+        self.retweeted_tweet = self._get_retweeted_tweet(self.is_retweet, original_tweet)
+        self.text = self.tweet_body = self._get_tweet_text(original_tweet, self.is_retweet)
+        self.is_quoted = self._is_quoted(original_tweet)
+        self.quoted_tweet = self._get_quoted_tweet(self.is_quoted)
+        self.is_reply = self._is_reply(original_tweet)
+        self.is_sensitive = self._is_sensitive(original_tweet)
+        self.reply_counts = self._get_reply_counts(original_tweet)
+        self.quote_counts = self._get_quote_counts(original_tweet)
+        self.replied_to = self.__replied_to = self._get_reply_to(self.is_reply, original_tweet)
+        self.bookmark_count = self._get_bookmark_count(original_tweet)
+        self.vibe = self._get_vibe()
+        self.views = self._get_views()
+        self.language = self._get_language(original_tweet)
+        self.likes = self._get_likes(original_tweet)
+        self.card = self._get_card()
+        self.place = self._get_place(original_tweet)
+        self.retweet_counts = self._get_retweet_counts(original_tweet)
+        self.source = self._get_source(self.__raw_tweet)
+        self.media = self._get_tweet_media(original_tweet)
+        self.user_mentions = self._get_tweet_mentions(original_tweet)
+        self.urls = self._get_tweet_urls(original_tweet)
+        self.hashtags = self._get_tweet_hashtags(original_tweet)
+        self.symbols = self._get_tweet_symbols(original_tweet)
+        self.threads = []
+        self.comments = []
 
     def _get_id(self):
         if self.__raw_tweet.get("rest_id"):
             return self.__raw_tweet['rest_id']
 
         if self.__raw_tweet.get("tweet"):
             return self.__raw_tweet['tweet']['rest_id']
@@ -178,46 +158,57 @@
             self.__raw_tweet = self.__raw_tweet['tweet']
 
         if self.__raw_tweet.get("legacy"):
             return self.__raw_tweet['legacy']
 
         return self.__raw_tweet
 
+    def _get_author(self):
+        if self.__raw_tweet.get("core"):
+            return User(self.__raw_tweet['core']['user_results']['result'])
+
+        if self.__raw_tweet.get("author"):
+            return User(self.__raw_tweet['author'])
+        return None
+
     def _get_retweeted_tweet(self, is_retweet, original_tweet):
-        if is_retweet:
+        if is_retweet and original_tweet.get("retweeted_status_result"):
             retweet = original_tweet['retweeted_status_result']['result']
             return Tweet(None, retweet, self.http)
 
         return None
 
     def _get_threads(self):
         if not self.__raw_response:
             self.__raw_response = self.http.get_tweet_detail(self.id)  # noqa
 
-        for entry in self.__raw_response.json()['data']['threaded_conversation_with_injections_v2']['instructions'][0]['entries']:
+        for entry in self.__raw_response['data']['threaded_conversation_with_injections_v2']['instructions'][0]['entries']:
             if str(entry['entryId']).split("-")[0] == "conversationthread":
                 for item in entry['content']['items']:
                     try:
                         tweetType = item["item"]["itemContent"]["tweetDisplayType"]
                         tweet = item['item']['itemContent']['tweet_results']['result']
 
                         if not self.__replied_to or self.__replied_to.id != tweet['rest_id']:
-                            self.__formatted_tweet['threads' if tweetType == "SelfThread" else 'comments'].append(
-                                Tweet(None, tweet, self.http))
+                            if tweetType == "SelfThread":
+                                self.threads.append(Tweet(None, tweet, self.http))
+                            else:
+                                self.comments.append(Tweet(None, tweet, self.http))
                     except KeyError as e:
                         pass
 
     def _get_quoted_tweet(self, is_quoted):
         raw_tweet = None
         if is_quoted:
             raw_response = self.__raw_response
-            if self.__raw_tweet.get("quoted_status_result"):
-                raw_tweet = self.__raw_tweet['quoted_status_result']['result']
-                return Tweet(raw_response, raw_tweet, self.http)
             try:
+                if self.__raw_tweet.get("quoted_status_result"):
+                    raw_tweet = self.__raw_tweet['quoted_status_result']['result']
+                    return Tweet(raw_response, raw_tweet, self.http)
+
                 if not raw_tweet and self.__raw_tweet.get("legacy"):
                     raw_tweet = self.__raw_tweet['legacy']['retweeted_status_result']['result']['quoted_status_result']['result']
                     return Tweet(raw_response, raw_tweet, self.http)
             except:
                 return None
 
         return None
@@ -316,31 +307,34 @@
         if original_tweet.get('source'):
             return str(original_tweet['source']).split(">")[1].split("<")[0]
 
         return ""
 
     @staticmethod
     def _get_tweet_text(original_tweet, is_retweet):
-        if is_retweet:
+        if is_retweet and original_tweet.get("retweeted_status_result"):
+
+            if not original_tweet['retweeted_status_result']['result'].get("legacy"):
+                return original_tweet['retweeted_status_result']['result']['tweet']['legacy']['full_text']
+
             return original_tweet['retweeted_status_result']['result']['legacy']['full_text']
 
         if original_tweet.get('full_text'):
             return original_tweet['full_text']
 
         return ""
 
-    @staticmethod
-    def _get_tweet_media(original_tweet):
+    def _get_tweet_media(self, original_tweet):
         if not original_tweet.get("extended_entities"):
             return []
 
         if not original_tweet['extended_entities'].get("media"):
             return []
 
-        return [Media(media) for media in original_tweet['extended_entities']['media']]
+        return [Media(media, self.http) for media in original_tweet['extended_entities']['media']]
 
     @staticmethod
     def _get_tweet_mentions(original_tweet):
         if not original_tweet.get("entities"):
             return []
 
         if not original_tweet['entities'].get("user_mentions"):
@@ -380,129 +374,121 @@
         if not original_tweet['entities'].get("symbols"):
             return []
 
         return [symbol for symbol in original_tweet['entities']['symbols']]
 
 
 class Media(dict):
-    def __init__(self, media_dict):
+    def __init__(self, media_dict, http):
         super().__init__()
         self.__dictionary = media_dict
+        self.__http = http
         self.display_url = self.__dictionary.get("display_url")
         self.expanded_url = self.__dictionary.get("expanded_url")
         self.id = self.__dictionary.get("id_str")
         self.indices = self.__dictionary.get("indices")
-        self.media_url_https = self.__dictionary.get("media_url_https")
+        self.media_url_https = self.direct_url = self.__dictionary.get("media_url_https")
         self.type = self.__dictionary.get("type")
         self.url = self.__dictionary.get("url")
         self.features = self.__dictionary.get("features")
         self.media_key = self.__dictionary.get("media_key")
         self.mediaStats = self.__dictionary.get("mediaStats")
-        self.sizes = self.__dictionary.get("sizes")
+        self.sizes = [MediaSize(k, v) for k, v in self.__dictionary.get("sizes").items() if self.__dictionary.get('sizes')]
         self.original_info = self.__dictionary.get("original_info")
-        self.file_format = self.media_url_https.split(".")[-1] if self.type == "photo" else None
+        self.file_format = self._get_file_format()
         self.streams = []
         if self.type == "video" or self.type == "animated_gif":
             self.__parse_video_streams()
 
         for k, v in vars(self).items():
             if not k.startswith("_"):
                 self[k] = v
 
+    def _get_file_format(self):
+        filename = os.path.basename(self.media_url_https).split("?")[0]
+        return filename.split(".")[-1] if self.type == "photo" else "mp4"
+
     def __parse_video_streams(self):
         videoDict = self.__dictionary.get("video_info")
-        if videoDict:
-            for i in videoDict.get("variants"):
-                if not i.get("content_type").split("/")[-1] == "x-mpegURL":
-                    self.streams.append(
-                        Stream(i, videoDict.get("duration_millis", 0), videoDict.get("aspect_ratio"))
-                    )
+        if not videoDict:
+            return
+
+        for i in videoDict.get("variants"):
+            if not i.get("content_type").split("/")[-1] == "x-mpegURL":
+                self.streams.append(Stream(i, videoDict.get("duration_millis", 0), videoDict.get("aspect_ratio"), self.__http))
 
     def __repr__(self):
         return f"Media(id={self.id}, type={self.type})"
 
-    def download(self, filename_, show_progress=True):
-        if show_progress:
-            show_progress = bar_progress
-        else:
-            show_progress = None
-
+    def download(self, filename=None, show_progress=True):
         if self.type == "photo":
-            filename = f"{filename_}.{self.file_format}"
-            wget.download(url=self.media_url_https, out=filename, bar=show_progress)
-            if show_progress:
-                sys.stdout.write("\n")
-            return filename
-
+            return self.__http.download_media(self.direct_url, filename, show_progress)
         elif self.type == "video":
-            _res = [int(stream.res) for stream in self.streams if stream.res]
+            _res = [eval(stream.res) for stream in self.streams if stream.res]
             max_res = max(_res)
             for stream in self.streams:
-                if int(stream.res) == max_res:
+                if eval(stream.res) == max_res:
                     file_format = stream.content_type.split("/")[-1]
                     if not file_format == "x-mpegURL":
-                        filename = f"{filename_}.{file_format}"
-                        wget.download(url=stream.url, out=filename, bar=show_progress)
-                        if show_progress:
-                            sys.stdout.write("\n")
-                        return filename
-
+                        return self.__http.download_media(stream.url, filename, show_progress)
         elif self.type == "animated_gif":
             file_format = self.streams[0].content_type.split("/")[-1]
             if not file_format == "x-mpegURL":
-                filename = f"{filename_}.{file_format}"
-                wget.download(url=self.streams[0].url, out=filename, bar=show_progress)
-                if show_progress:
-                    sys.stdout.write("\n")
-                return filename
+                return self.__http.download_media(self.streams[0].url, filename, show_progress)
         return None
 
     @deprecated
     def to_dict(self):
         return self.__dictionary
 
 
 class Stream(dict):
-    def __init__(self, videoDict, length, ratio):
+    def __init__(self, videoDict, length, ratio, http):
         super().__init__()
         self.__dictionary = videoDict
+        self.__http = http
         self.bitrate = self.__dictionary.get("bitrate")
         self.content_type = self.__dictionary.get("content_type")
-        self.url = self.__dictionary.get("url")
+        self.url = self.direct_url = self.__dictionary.get("url")
         self.length = length
         self.aspect_ratio = ratio
-        try:
-            self.res = int(self.url.split("/")[7].split("x")[0]) * int(self.url.split("/")[7].split("x")[1])
-        except (ValueError, IndexError):
-            try:
-                self.res = int(self.url.split("/")[6].split("x")[0]) * int(self.url.split("/")[6].split("x")[1])
-            except (ValueError, IndexError):
-                self.res = None
+        self.res = self._get_resolution()
 
         for k, v in vars(self).items():
             if not k.startswith("_"):
                 self[k] = v
 
+    def _get_resolution(self):
+        result = re.findall("/(\d+)x(\d+)/", self.url)
+        if result:
+            result = result[0]
+            return f"{result[0]}*{result[1]}"
+
+        return None
+
     def __repr__(self):
         return f"Stream(content_type={self.content_type}, length={self.length}, bitrate={self.bitrate}, res={self.res})"
 
     def download(self, filename_=None, show_progress=False):
-        if show_progress:
-            show_progress = bar_progress
-        else:
-            show_progress = None
-        file_format = self.content_type.split("/")[-1]
-        if filename_:
-            filename = f"{filename_}.{file_format}"
-        else:
-            filename = None
-        wget.download(url=self.url, out=filename, bar=show_progress)
-        if show_progress:
-            sys.stdout.write("\n")
-        return filename
+        return self.__http.download_media(self.url, filename_, show_progress)
+
+
+class MediaSize(dict):
+    def __init__(self, name, data):
+        super().__init__()
+        self._json = data
+        self.name = self['name'] = name
+        self.width = self['width'] = self._json['w']
+        self.height = self['height'] = self._json['h']
+        self.resize = self['resize'] = self._json['resize']
+
+    def __repr__(self):
+        return "MediaSize(name={}, width={}, height={}, resize={})".format(
+            self.name, self.width, self.height, self.resize
+        )
 
 
 class ShortUser(dict):
     def __init__(self, user_dict):
         super().__init__()
         self.__dictionary = user_dict
         self.id = self.__dictionary.get("id_str")
@@ -516,172 +502,40 @@
     def __repr__(self):
         return f"ShortUser(id={self.id}, name={self.name})"
 
     def to_dict(self):
         return self.__dictionary
 
 
-class User(dict):
-    def __init__(self, user_dict, type_=1):
-        super().__init__()
-        if type_ == 1:
-            self.__dictionary = user_dict['data']['user']['result']
-        elif type_ == 2:
-            self.__dictionary = user_dict
-        else:
-            self.__dictionary = user_dict['user_results']['result']
-
-        self.id = self.__dictionary.get("id")
-        self.rest_id = self._get_rest_id(self.__dictionary)
-        self.created_at = self._get_created_at(self.__dictionary)
-        self.default_profile = self._get_key(self.__dictionary, "default_profile")
-        self.default_profile_image = self._get_key(self.__dictionary, "default_profile_image")
-        self.description = self._get_key(self.__dictionary, "description")
-        self.entities = self._get_key(self.__dictionary, "entities")
-        self.fast_followers_count = self._get_key(self.__dictionary, "fast_followers_count")
-        self.favourites_count = self._get_key(self.__dictionary, "favourites_count")
-        self.followers_count = self._get_key(self.__dictionary, "followers_count")
-        self.friends_count = self._get_key(self.__dictionary, "friends_count")
-        self.has_custom_timelines = self._get_key(self.__dictionary, "has_custom_timelines")
-        self.is_translator = self._get_key(self.__dictionary, "is_translator")
-        self.listed_count = self._get_key(self.__dictionary, "listed_count")
-        self.location = self._get_key(self.__dictionary, "location")
-        self.media_count = self._get_key(self.__dictionary, "media_count")
-        self.name = self._get_key(self.__dictionary, "name")
-        self.normal_followers_count = self._get_key(self.__dictionary, "normal_followers_count")
-        self.profile_banner_url = self._get_key(self.__dictionary, "profile_banner_url")
-        self.profile_image_url_https = self._get_key(self.__dictionary, "profile_image_url_https")
-        self.profile_interstitial_type = self._get_key(self.__dictionary, "profile_interstitial_type")
-        self.protected = self._get_key(self.__dictionary, "protected")
-        self.screen_name = self.username = self._get_key(self.__dictionary, "screen_name")
-        self.statuses_count = self._get_key(self.__dictionary, "statuses_count")
-        self.translator_type = self._get_key(self.__dictionary, "translator_type")
-        self.verified = self._get_key(self.__dictionary, "verified")
-        # self.verified_type = self._get_key(self.__dictionary, "verified_type")
-        self.possibly_sensitive = self._get_key(self.__dictionary, "possibly_sensitive")
-        self.pinned_tweets = self._get_key(self.__dictionary, "pinned_tweet_ids_str")
-
-        self.profile_url = "https://twitter.com/{}".format(self.screen_name)
-
-        for k, v in vars(self).items():
-            if not k.startswith("_"):
-                self[k] = v
-
-    def __repr__(self):
-        return f"User(id={self.rest_id}, name={self.name}, username={self.screen_name}, followers={self.followers_count}, verified={self.verified})"
-
-    @deprecated
-    def to_dict(self):
-        return self.__dictionary
-
-    @staticmethod
-    def _get_rest_id(user):
-        if user.get("rest_id"):
-            return user['rest_id']
-
-        if user.get("id_str"):
-            return user['id_str']
-
-        return None
-
-    @staticmethod
-    def _get_created_at(user):
-        date = None
-        if user.get("legacy"):
-            date = user['legacy']['created_at']
-
-        if not date and user.get("created_at"):
-            date = user["created_at"]
-
-        return parser.parse(date) if date else None
-
-    @staticmethod
-    def _get_key(user, key):
-        keyValue = None
-        if user.get("legacy"):
-            keyValue = user['legacy'].get(key)
-
-        if not keyValue and user.get(key):
-            keyValue = user[key]
-
-        return keyValue
-
-
 class Trends:
     def __init__(self, trends_dict):
         self.__dictionary = trends_dict
         self.name = self.__dictionary.get("name")
         self.url = self.__dictionary.get("url")
         self.tweet_count = self.__dictionary.get("tweet_count")
 
     def __repr__(self):
         return f"Trends(name={self.name})"
 
     def to_dict(self):
         return self.__dictionary
 
 
-class UserLegacy(dict):
-    def __init__(self, user_dict):
-        super().__init__()
-        self.__dictionary = user_dict
-        self.id = self.__dictionary.get("id")
-        self.rest_id = self.__dictionary.get("id")
-        self.created_at = parser.parse(self.__dictionary.get("created_at")) if self.__dictionary.get("created_at") else None
-        self.default_profile = self.__dictionary.get("default_profile")
-        self.default_profile_image = self.__dictionary.get("default_profile_image")
-        self.description = self.__dictionary.get("description")
-        self.entities = self.__dictionary.get("entities")
-        self.fast_followers_count = self.__dictionary.get("fast_followers_count")
-        self.favourites_count = self.__dictionary.get("favourites_count")
-        self.followers_count = self.__dictionary.get("followers_count")
-        self.friends_count = self.__dictionary.get("friends_count")
-        self.has_custom_timelines = self.__dictionary.get("has_custom_timelines")
-        self.is_translator = self.__dictionary.get("is_translator")
-        self.listed_count = self.__dictionary.get("listed_count")
-        self.location = self.__dictionary.get("location")
-        self.media_count = self.__dictionary.get("media_count")
-        self.name = self.__dictionary.get("name")
-        self.normal_followers_count = self.__dictionary.get("normal_followers_count")
-        self.profile_banner_url = self.__dictionary.get("profile_banner_url")
-        self.profile_image_url_https = self.__dictionary.get("profile_image_url_https")
-        self.profile_interstitial_type = self.__dictionary.get("profile_interstitial_type")
-        self.protected = self.__dictionary.get("protected")
-        self.screen_name = self.__dictionary.get("screen_name")
-        self.statuses_count = self.__dictionary.get("statuses_count")
-        self.translator_type = self.__dictionary.get("translator_type")
-        self.verified = self.__dictionary.get("verified")
-        # self.verified_type = self.__dictionary.get("verified_type")
-        self.possibly_sensitive = self.__dictionary.get("possibly_sensitive")
-        self.pinned_tweets = self.__dictionary.get("pinned_tweet_ids_str")
-        self.profile_url = "https://twitter.com/{}".format(self.screen_name)
-
-        for k, v in vars(self).items():
-            if not k.startswith("_"):
-                self[k] = v
-
-    def __repr__(self):
-        return f"User(id={self.rest_id}, name={self.name}, followers={self.followers_count} , verified={self.verified})"
-
-    def to_dict(self):
-        return self.__dictionary
-
-
 class Card(dict):
     def __init__(self, card_dict):
         super().__init__()
         self._dict = card_dict
         self._bindings = self._dict['legacy'].get("binding_values")
         self.rest_id = self._dict.get("rest_id")
         self.name = self._dict['legacy'].get("name")
         self.choices = []
         self.end_time = None
         self.last_updated_time = None
         self.duration = None
-        self.user_ref = [User(user, 2) for user in self._dict['legacy']["user_refs"]] if self._dict['legacy'].get("user_refs") else []
+        self.user_ref = [User(user) for user in self._dict['legacy']["user_refs"]] if self._dict['legacy'].get("user_refs") else []
         self.__parse_choices()
 
         for k, v in vars(self).items():
             if not k.startswith("_"):
                 self[k] = v
 
     def __parse_choices(self):
@@ -751,14 +605,17 @@
 
         for k, v in vars(self).items():
             if not k.startswith("_"):
                 self[k] = v
 
     def parse_coordinates(self):
         results = []
+        if not self.__dict.get("bounding_box"):
+            return results
+
         for i in self.__dict['bounding_box'].get("coordinates"):
             for p in i:
                 coordinates = [p[1], p[0]]
                 if coordinates not in results:
                     results.append([coordinates[0], coordinates[1]])
 
         return [Coordinates(i[0], i[1]) for i in results]
@@ -776,7 +633,85 @@
         for k, v in vars(self).items():
             if not k.startswith("_"):
                 self[k] = v
 
     def __repr__(self):
         return f"Coordinates(latitude={self.latitude}, longitude={self.longitude})"
 
+
+class User(dict):
+    def __init__(self, user_data):
+        super().__init__()
+        self._json = user_data
+        self.id = self.rest_id = self.get_id()
+        self.created_at = self.get_created_at()
+        self.description = self._get_key("description")
+        self.fast_followers_count = self._get_key("fast_followers_count")
+        self.favourites_count = self._get_key("favourites_count")
+        self.followers_count = self._get_key("followers_count")
+        self.friends_count = self._get_key("friends_count")
+        self.has_custom_timelines = self._get_key("has_custom_timelines")
+        self.is_translator = self._get_key("is_translator")
+        self.listed_count = self._get_key("listed_count")
+        self.location = self._get_key("location")
+        self.media_count = self._get_key("media_count")
+        self.name = self._get_key("name")
+        self.normal_followers_count = self._get_key("normal_followers_count")
+        self.profile_banner_url = self._get_key("profile_banner_url")
+        self.profile_image_url_https = self._get_key("profile_image_url_https")
+        self.profile_interstitial_type = self._get_key("profile_interstitial_type")
+        self.protected = self._get_key("protected")
+        self.screen_name = self.username = self._get_key("screen_name")
+        self.statuses_count = self._get_key("statuses_count")
+        self.translator_type = self._get_key("translator_type")
+        self.verified = self._get_verified()
+        # self.verified_type = self._get_key("verified_type")
+        self.possibly_sensitive = self._get_key("possibly_sensitive")
+        self.pinned_tweets = self._get_key("pinned_tweet_ids_str")
+        self.profile_url = "https://twitter.com/{}".format(self.screen_name)
+
+    def __repr__(self):
+        return "User(id={}, username={}, name={}, verified={})".format(
+            self.id, self.username, self.name, self.verified
+        )
+
+    def _get_verified(self):
+        verified = self._get_key("verified", False)
+        if verified is False:
+            verified = self._get_key("is_blue_verified", False)
+
+        if verified is False:
+            verified = self._get_key("ext_is_blue_verified", False)
+
+        return False if verified in (None, False) else True
+
+    def get_id(self):
+        raw_id = self._json.get("id")
+        if not str(raw_id).isdigit():
+            raw_id = decodeBase64(raw_id).split(":")[-1]
+
+        return int(raw_id)
+
+    def get_created_at(self):
+        date = None
+        if self._json.get("legacy"):
+            date = self._json['legacy']['created_at']
+
+        if not date and self._json.get("created_at"):
+            date = self._json["created_at"]
+
+        return parser.parse(date) if date else None
+
+    def _get_key(self, key, default=None):
+        user = self._json
+        keyValue = default
+        if user.get("legacy"):
+            keyValue = user['legacy'].get(key)
+
+        if not keyValue and user.get(key):
+            keyValue = user[key]
+
+        if str(keyValue).isdigit():
+            keyValue = int(keyValue)
+
+        return keyValue
+
```

### Comparing `tweety-ns-0.6.1/src/tweety_ns.egg-info/PKG-INFO` & `tweety-ns-0.7/src/tweety_ns.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-Metadata-Version: 2.1
-Name: tweety-ns
-Version: 0.6.1
-Summary: An easy Twitter Scraper
-Home-page: https://github.com/mahrtayyab/tweety
-Author: Tayyab Kharl
-Author-email: tayyabmahr@gmail.com
-License: MIT
-Project-URL: Bug Tracker, https://github.com/mahrtayyab/tweety/issues
-Project-URL: Documentation, https://github.com/mahrtayyab/tweety
-Keywords: TWITTER,TWITTER SCRAPE,SCRAPE TWEETS
-Classifier: Development Status :: 4 - Beta
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: Build Tools
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-
-# tweety
-Twitter's API is annoying to work with, and has lots of limitations — luckily their frontend (JavaScript) has it's own API, which I reverse–engineered. No API rate limits. No restrictions.
-
-## Documentation:
-You can check documentation at  [here](https://mahrtayyab.github.io/tweety_docs/)
+Metadata-Version: 2.1
+Name: tweety-ns
+Version: 0.7
+Summary: An easy Twitter Scraper
+Home-page: https://github.com/mahrtayyab/tweety
+Author: Tayyab Kharl
+Author-email: tayyabmahr@gmail.com
+License: MIT
+Project-URL: Bug Tracker, https://github.com/mahrtayyab/tweety/issues
+Project-URL: Documentation, https://github.com/mahrtayyab/tweety
+Keywords: TWITTER,TWITTER SCRAPE,SCRAPE TWEETS
+Classifier: Development Status :: 4 - Beta
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: Build Tools
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+
+# tweety
+Twitter's API is annoying to work with, and has lots of limitations — luckily their frontend (JavaScript) has it's own API, which I reverse–engineered. No API rate limits. No restrictions.
+
+## Documentation:
+You can check documentation at  [here](https://mahrtayyab.github.io/tweety_docs/)
```

