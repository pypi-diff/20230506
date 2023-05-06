# Comparing `tmp/apollo-sdk-0.1.4.tar.gz` & `tmp/apollo-sdk-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apollo-sdk-0.1.4.tar", last modified: Thu May  4 23:15:11 2023, max compression
+gzip compressed data, was "apollo-sdk-0.1.6.tar", last modified: Sat May  6 03:15:36 2023, max compression
```

## Comparing `apollo-sdk-0.1.4.tar` & `apollo-sdk-0.1.6.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-04 23:15:11.390741 apollo-sdk-0.1.4/
--rw-r--r--   0 abpyguru   (501) staff       (20)     3793 2023-04-29 17:42:09.000000 apollo-sdk-0.1.4/LICENSE
--rw-r--r--   0 abpyguru   (501) staff       (20)      605 2023-05-04 23:15:11.390840 apollo-sdk-0.1.4/PKG-INFO
--rw-r--r--   0 abpyguru   (501) staff       (20)     5509 2023-04-29 17:42:09.000000 apollo-sdk-0.1.4/README.md
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-04 23:15:11.378208 apollo-sdk-0.1.4/apollo/
--rw-r--r--   0 abpyguru   (501) staff       (20)     1403 2023-04-30 05:02:07.000000 apollo-sdk-0.1.4/apollo/__init__.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     3608 2023-04-30 05:02:07.000000 apollo-sdk-0.1.4/apollo/client.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-04 23:15:11.378683 apollo-sdk-0.1.4/apollo/connectors/
--rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.1.4/apollo/connectors/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-04 23:15:11.379119 apollo-sdk-0.1.4/apollo/connectors/aws/
--rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.1.4/apollo/connectors/aws/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-04 23:15:11.379497 apollo-sdk-0.1.4/apollo/connectors/google/
--rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.1.4/apollo/connectors/google/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-04 23:15:11.380866 apollo-sdk-0.1.4/apollo/connectors/microsoft/
--rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.1.4/apollo/connectors/microsoft/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-04 23:15:11.382199 apollo-sdk-0.1.4/apollo/connectors/openai/
--rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.1.4/apollo/connectors/openai/__init__.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     1450 2023-05-03 17:36:48.000000 apollo-sdk-0.1.4/apollo/const.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-04 23:15:11.383118 apollo-sdk-0.1.4/apollo/database/
--rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.1.4/apollo/database/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-04 23:15:11.385133 apollo-sdk-0.1.4/apollo/database/firebase/
--rw-r--r--   0 abpyguru   (501) staff       (20)      770 2023-04-30 05:02:07.000000 apollo-sdk-0.1.4/apollo/database/firebase/__init__.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     1488 2023-04-30 05:02:07.000000 apollo-sdk-0.1.4/apollo/database/firebase/base.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     3494 2023-04-30 05:02:07.000000 apollo-sdk-0.1.4/apollo/database/firebase/cloud.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     1438 2023-04-30 05:02:07.000000 apollo-sdk-0.1.4/apollo/database/firebase/local.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-04 23:15:11.385352 apollo-sdk-0.1.4/apollo/database/mongo/
--rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.1.4/apollo/database/mongo/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-04 23:15:11.385588 apollo-sdk-0.1.4/apollo/database/mysql/
--rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.1.4/apollo/database/mysql/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-04 23:15:11.385790 apollo-sdk-0.1.4/apollo/database/postgres/
--rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.1.4/apollo/database/postgres/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-04 23:15:11.386601 apollo-sdk-0.1.4/apollo/database/supabase/
--rw-r--r--   0 abpyguru   (501) staff       (20)      770 2023-04-30 05:02:07.000000 apollo-sdk-0.1.4/apollo/database/supabase/__init__.py
--rw-r--r--   0 abpyguru   (501) staff       (20)      739 2023-04-30 05:02:07.000000 apollo-sdk-0.1.4/apollo/database/supabase/base.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     1553 2023-04-30 05:02:07.000000 apollo-sdk-0.1.4/apollo/database/supabase/cloud.py
--rw-r--r--   0 abpyguru   (501) staff       (20)      810 2023-04-30 05:02:07.000000 apollo-sdk-0.1.4/apollo/database/supabase/local.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     4197 2023-04-30 05:02:07.000000 apollo-sdk-0.1.4/apollo/exceptions.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     1375 2023-04-30 05:02:07.000000 apollo-sdk-0.1.4/apollo/manager.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     1194 2023-04-30 05:02:07.000000 apollo-sdk-0.1.4/apollo/resource.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-04 23:15:11.386837 apollo-sdk-0.1.4/apollo/service/
--rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.1.4/apollo/service/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-04 23:15:11.387026 apollo-sdk-0.1.4/apollo/service/graphql/
--rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.1.4/apollo/service/graphql/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-04 23:15:11.388657 apollo-sdk-0.1.4/apollo/service/json/
--rw-r--r--   0 abpyguru   (501) staff       (20)      754 2023-04-30 05:02:07.000000 apollo-sdk-0.1.4/apollo/service/json/__init__.py
--rw-r--r--   0 abpyguru   (501) staff       (20)      859 2023-04-30 05:02:07.000000 apollo-sdk-0.1.4/apollo/service/json/base.py
--rw-r--r--   0 abpyguru   (501) staff       (20)     1154 2023-05-03 17:37:51.000000 apollo-sdk-0.1.4/apollo/service/json/cloud.py
--rw-r--r--   0 abpyguru   (501) staff       (20)      888 2023-04-30 05:02:07.000000 apollo-sdk-0.1.4/apollo/service/json/local.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-04 23:15:11.388886 apollo-sdk-0.1.4/apollo/tests/
--rw-r--r--   0 abpyguru   (501) staff       (20)      645 2023-04-30 05:02:07.000000 apollo-sdk-0.1.4/apollo/tests/__init__.py
-drwxr-xr-x   0 abpyguru   (501) staff       (20)        0 2023-05-04 23:15:11.390551 apollo-sdk-0.1.4/apollo_sdk.egg-info/
--rw-r--r--   0 abpyguru   (501) staff       (20)      605 2023-05-04 23:15:11.000000 apollo-sdk-0.1.4/apollo_sdk.egg-info/PKG-INFO
--rw-r--r--   0 abpyguru   (501) staff       (20)     1107 2023-05-04 23:15:11.000000 apollo-sdk-0.1.4/apollo_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 abpyguru   (501) staff       (20)        1 2023-05-04 23:15:11.000000 apollo-sdk-0.1.4/apollo_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 abpyguru   (501) staff       (20)      266 2023-05-04 23:15:11.000000 apollo-sdk-0.1.4/apollo_sdk.egg-info/requires.txt
--rw-r--r--   0 abpyguru   (501) staff       (20)        7 2023-05-04 23:15:11.000000 apollo-sdk-0.1.4/apollo_sdk.egg-info/top_level.txt
--rw-r--r--   0 abpyguru   (501) staff       (20)      103 2023-05-04 23:15:11.391117 apollo-sdk-0.1.4/setup.cfg
--rw-r--r--   0 abpyguru   (501) staff       (20)     1872 2023-05-04 23:13:04.000000 apollo-sdk-0.1.4/setup.py
+drwxr-xr-x   0 adrianbrown   (501) staff       (20)        0 2023-05-06 03:15:36.622763 apollo-sdk-0.1.6/
+-rw-r--r--   0 adrianbrown   (501) staff       (20)     3793 2023-04-29 00:08:01.000000 apollo-sdk-0.1.6/LICENSE
+-rw-r--r--   0 adrianbrown   (501) staff       (20)     5909 2023-05-06 03:15:36.622834 apollo-sdk-0.1.6/PKG-INFO
+-rw-r--r--   0 adrianbrown   (501) staff       (20)     5259 2023-05-06 02:32:52.000000 apollo-sdk-0.1.6/README.md
+drwxr-xr-x   0 adrianbrown   (501) staff       (20)        0 2023-05-06 03:15:36.618934 apollo-sdk-0.1.6/apollo/
+-rw-r--r--   0 adrianbrown   (501) staff       (20)     1419 2023-05-06 01:22:11.000000 apollo-sdk-0.1.6/apollo/__init__.py
+-rw-r--r--   0 adrianbrown   (501) staff       (20)     3778 2023-05-06 01:22:11.000000 apollo-sdk-0.1.6/apollo/client.py
+drwxr-xr-x   0 adrianbrown   (501) staff       (20)        0 2023-05-06 03:15:36.619058 apollo-sdk-0.1.6/apollo/connectors/
+-rw-r--r--   0 adrianbrown   (501) staff       (20)      645 2023-05-06 01:22:11.000000 apollo-sdk-0.1.6/apollo/connectors/__init__.py
+drwxr-xr-x   0 adrianbrown   (501) staff       (20)        0 2023-05-06 03:15:36.619182 apollo-sdk-0.1.6/apollo/connectors/aws/
+-rw-r--r--   0 adrianbrown   (501) staff       (20)      645 2023-05-06 01:22:11.000000 apollo-sdk-0.1.6/apollo/connectors/aws/__init__.py
+drwxr-xr-x   0 adrianbrown   (501) staff       (20)        0 2023-05-06 03:15:36.619347 apollo-sdk-0.1.6/apollo/connectors/google/
+-rw-r--r--   0 adrianbrown   (501) staff       (20)      645 2023-05-06 01:22:11.000000 apollo-sdk-0.1.6/apollo/connectors/google/__init__.py
+drwxr-xr-x   0 adrianbrown   (501) staff       (20)        0 2023-05-06 03:15:36.619480 apollo-sdk-0.1.6/apollo/connectors/microsoft/
+-rw-r--r--   0 adrianbrown   (501) staff       (20)      645 2023-05-06 01:22:11.000000 apollo-sdk-0.1.6/apollo/connectors/microsoft/__init__.py
+drwxr-xr-x   0 adrianbrown   (501) staff       (20)        0 2023-05-06 03:15:36.619597 apollo-sdk-0.1.6/apollo/connectors/openai/
+-rw-r--r--   0 adrianbrown   (501) staff       (20)      645 2023-05-06 01:22:11.000000 apollo-sdk-0.1.6/apollo/connectors/openai/__init__.py
+-rw-r--r--   0 adrianbrown   (501) staff       (20)     1450 2023-05-06 01:22:11.000000 apollo-sdk-0.1.6/apollo/const.py
+drwxr-xr-x   0 adrianbrown   (501) staff       (20)        0 2023-05-06 03:15:36.619728 apollo-sdk-0.1.6/apollo/database/
+-rw-r--r--   0 adrianbrown   (501) staff       (20)      645 2023-04-29 00:08:01.000000 apollo-sdk-0.1.6/apollo/database/__init__.py
+drwxr-xr-x   0 adrianbrown   (501) staff       (20)        0 2023-05-06 03:15:36.620233 apollo-sdk-0.1.6/apollo/database/firebase/
+-rw-r--r--   0 adrianbrown   (501) staff       (20)      770 2023-04-29 00:08:01.000000 apollo-sdk-0.1.6/apollo/database/firebase/__init__.py
+-rw-r--r--   0 adrianbrown   (501) staff       (20)     1488 2023-04-29 00:08:01.000000 apollo-sdk-0.1.6/apollo/database/firebase/base.py
+-rw-r--r--   0 adrianbrown   (501) staff       (20)     3494 2023-04-29 00:08:01.000000 apollo-sdk-0.1.6/apollo/database/firebase/cloud.py
+-rw-r--r--   0 adrianbrown   (501) staff       (20)     1438 2023-04-29 00:08:01.000000 apollo-sdk-0.1.6/apollo/database/firebase/local.py
+drwxr-xr-x   0 adrianbrown   (501) staff       (20)        0 2023-05-06 03:15:36.620361 apollo-sdk-0.1.6/apollo/database/mongo/
+-rw-r--r--   0 adrianbrown   (501) staff       (20)      645 2023-04-29 00:08:01.000000 apollo-sdk-0.1.6/apollo/database/mongo/__init__.py
+drwxr-xr-x   0 adrianbrown   (501) staff       (20)        0 2023-05-06 03:15:36.620490 apollo-sdk-0.1.6/apollo/database/mysql/
+-rw-r--r--   0 adrianbrown   (501) staff       (20)      645 2023-04-29 00:08:01.000000 apollo-sdk-0.1.6/apollo/database/mysql/__init__.py
+drwxr-xr-x   0 adrianbrown   (501) staff       (20)        0 2023-05-06 03:15:36.620645 apollo-sdk-0.1.6/apollo/database/postgres/
+-rw-r--r--   0 adrianbrown   (501) staff       (20)      645 2023-04-29 00:08:01.000000 apollo-sdk-0.1.6/apollo/database/postgres/__init__.py
+drwxr-xr-x   0 adrianbrown   (501) staff       (20)        0 2023-05-06 03:15:36.621161 apollo-sdk-0.1.6/apollo/database/supabase/
+-rw-r--r--   0 adrianbrown   (501) staff       (20)      770 2023-04-29 00:08:01.000000 apollo-sdk-0.1.6/apollo/database/supabase/__init__.py
+-rw-r--r--   0 adrianbrown   (501) staff       (20)      739 2023-04-29 00:08:01.000000 apollo-sdk-0.1.6/apollo/database/supabase/base.py
+-rw-r--r--   0 adrianbrown   (501) staff       (20)     1553 2023-04-29 00:08:01.000000 apollo-sdk-0.1.6/apollo/database/supabase/cloud.py
+-rw-r--r--   0 adrianbrown   (501) staff       (20)      810 2023-04-29 00:08:01.000000 apollo-sdk-0.1.6/apollo/database/supabase/local.py
+-rw-r--r--   0 adrianbrown   (501) staff       (20)     4197 2023-04-29 00:08:01.000000 apollo-sdk-0.1.6/apollo/exceptions.py
+-rw-r--r--   0 adrianbrown   (501) staff       (20)     1389 2023-05-06 01:22:11.000000 apollo-sdk-0.1.6/apollo/manager.py
+-rw-r--r--   0 adrianbrown   (501) staff       (20)     1230 2023-05-06 01:22:11.000000 apollo-sdk-0.1.6/apollo/resource.py
+drwxr-xr-x   0 adrianbrown   (501) staff       (20)        0 2023-05-06 03:15:36.621294 apollo-sdk-0.1.6/apollo/service/
+-rw-r--r--   0 adrianbrown   (501) staff       (20)      645 2023-04-29 00:08:01.000000 apollo-sdk-0.1.6/apollo/service/__init__.py
+drwxr-xr-x   0 adrianbrown   (501) staff       (20)        0 2023-05-06 03:15:36.621417 apollo-sdk-0.1.6/apollo/service/graphql/
+-rw-r--r--   0 adrianbrown   (501) staff       (20)      645 2023-04-29 00:08:01.000000 apollo-sdk-0.1.6/apollo/service/graphql/__init__.py
+drwxr-xr-x   0 adrianbrown   (501) staff       (20)        0 2023-05-06 03:15:36.621919 apollo-sdk-0.1.6/apollo/service/json/
+-rw-r--r--   0 adrianbrown   (501) staff       (20)      754 2023-04-29 00:08:01.000000 apollo-sdk-0.1.6/apollo/service/json/__init__.py
+-rw-r--r--   0 adrianbrown   (501) staff       (20)      859 2023-04-29 00:08:01.000000 apollo-sdk-0.1.6/apollo/service/json/base.py
+-rw-r--r--   0 adrianbrown   (501) staff       (20)     1209 2023-05-06 01:22:11.000000 apollo-sdk-0.1.6/apollo/service/json/cloud.py
+-rw-r--r--   0 adrianbrown   (501) staff       (20)      888 2023-04-29 00:08:01.000000 apollo-sdk-0.1.6/apollo/service/json/local.py
+drwxr-xr-x   0 adrianbrown   (501) staff       (20)        0 2023-05-06 03:15:36.622036 apollo-sdk-0.1.6/apollo/tests/
+-rw-r--r--   0 adrianbrown   (501) staff       (20)      645 2023-04-29 00:08:01.000000 apollo-sdk-0.1.6/apollo/tests/__init__.py
+drwxr-xr-x   0 adrianbrown   (501) staff       (20)        0 2023-05-06 03:15:36.622647 apollo-sdk-0.1.6/apollo_sdk.egg-info/
+-rw-r--r--   0 adrianbrown   (501) staff       (20)     5909 2023-05-06 03:15:36.000000 apollo-sdk-0.1.6/apollo_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 adrianbrown   (501) staff       (20)     1107 2023-05-06 03:15:36.000000 apollo-sdk-0.1.6/apollo_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 adrianbrown   (501) staff       (20)        1 2023-05-06 03:15:36.000000 apollo-sdk-0.1.6/apollo_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 adrianbrown   (501) staff       (20)      266 2023-05-06 03:15:36.000000 apollo-sdk-0.1.6/apollo_sdk.egg-info/requires.txt
+-rw-r--r--   0 adrianbrown   (501) staff       (20)        7 2023-05-06 03:15:36.000000 apollo-sdk-0.1.6/apollo_sdk.egg-info/top_level.txt
+-rw-r--r--   0 adrianbrown   (501) staff       (20)      103 2023-05-06 03:15:36.623064 apollo-sdk-0.1.6/setup.cfg
+-rw-r--r--   0 adrianbrown   (501) staff       (20)     2092 2023-05-06 03:15:18.000000 apollo-sdk-0.1.6/setup.py
```

### Comparing `apollo-sdk-0.1.4/LICENSE` & `apollo-sdk-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.4/README.md` & `apollo-sdk-0.1.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,116 +1,120 @@
+Metadata-Version: 2.1
+Name: apollo-sdk
+Version: 0.1.6
+Summary: Build automated decision making workflows by aggregating your AI models and data into one api.
+Home-page: https://github.com/apolloapi/apolloapi
+Author: Apollo API, Inc.
+Author-email: adrbrownx@gmail.com
+License: Elastic License v2
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 <div align="center">
 
-![ApolloLogo](https://uploads-ssl.webflow.com/640ca38ad086fde245b76c9d/643fffb82419ac18d39e3e4e_Screenshot%202023-04-19%20at%2010.50.13%20AM.png)
+![ApolloLogo](https://uploads-ssl.webflow.com/640ca38ad086fde245b76c9d/6455b1fd3d8642575f793c94_header.png)
 
 </div>
 
-<h1 align="center">The easiest way to build custom decision making workflows</h1>
+<h1 align="center">Open-source Task Automation</h1>
 
 <div align="center">
-Apollo gives you access to custom machine learning models, no-code platform and continuously syncs data from any API or Database to centralize investigations and allow you to automate the detection of harm in images, videos, audio and text.
+Apollo is an open-source no-code platform that helps you build automated workflows in minutes. Our SDK allows you to automate tasks such as; onboarding, compliance, trust & safety, fraud detection, code generation and more.
 </div>
 
 <p align="center">
     <br />
-    <a href="https://apolloapi-doc.vercel.app/" rel="dofollow"><strong>Docs »</strong></a>
+    <a href="https://docs.apolloapi.io/" rel="dofollow"><strong>Docs »</strong></a>
     <br />
 
   <br/>
-    <a href="https://apolloapi-doc.vercel.app/">Examples</a>
     <a href="https://www.apolloapi.io/">Join the waitlist</a>
     ·
     <a href="https://github.com/apolloapi/apolloapi/issues">Report Bug</a>
     ·
     <a href="https://discord.gg/ZUH7f7AzUY">Community Discord</a>
 </p>
 
-## ⭐ Can you show me an example?
-
-In your code you can write:
-
-```ts
-Apollo.connect('postgres://username:password@hostnam...', ...) // Starts syncing content forever!
-
-Apollo.use('OpenAI', "moderation", ...) // Connect to existing providers!
-
-Apollo.rule('Phrase1', '>=', '0.8') // Create custom rules!
-
-Apollo.use('Apollo', "violence", ...) // Connect with our internal models!
-
-// Detect bad actors at scale!
-Apollo.detectImage('Image1', 'contains', 'VERY_LIKELY') // Image Analysis/OCR
-Apollo.detectSpeech('Audio1', 'contains', 'UNLIKELY') // Audio Processing
-Apollo.detectVideo('Video1', 'contains', 'POSSIBLE') // Video Analysis
-Apollo.detectText('Phrase1', 'contains', 'UNKNOWN') // Text Analysis
-
-```
-
-Apollo then takes care of:
-
-- Detecting real-time changes in user experience
-- Automated detection against image, video, audio or text
-- Connecting policy to product
-- Making sure your integration is robust, so you never again have to worry about stuck/stale data or false-positives
+## Why Apollo API?
 
-## 🧑‍💻 Cool, what can I build with it?
-
-- Trust & Safety teams in companies use Apollo to **build native in-app connections** related to active response, content moderation, fraud detection, etc.
-- Some **automate their personal lives** with Apollo by integrating against discord communities or other decentralized networks for safety
-- Apollo can help you **quickly build trust** for hobby projects, communities or business
+Before Apollo, integrating AI models and building automated workflows could be time-consuming and complex, with Apollo, teams can simplify and accelerate the process, making it easier to deploy AI models, sync data, and develop insights in minutes.
 
 ## 🚀 Interesting, how can I try it?
 
-Let's setup your first Integration in 2 minutes!
-
-It will pull from your local database (and keep it in sync).
-
-To start:
+Lets install the SDK first...
 
 ```bash
-# install the cli-toolkit
 pip install apollo-sdk
-
-# enter a python repl or create a python file, up to you! (repl is easiest)
-python3
 ```
 
+Let's setup your first Integration!
+
+It will pull from your local database (and keep it in sync).
+
 ```python
 # import the package
 from apollo.client import Apollo
 
 # sync data from your database instance
 # (we support supabase at the current moment or postgresql via uri format)
 Apollo.connect("postgres://username:password@hostname:port/database_name")
 
 # If you want to test out operation on your external connection
 Apollo.fetch_tables()
 Apollo.query("desc", "table", "column")
 ```
 
-Test sending your content to our API!
-
 ...and create a workflow with a simple command:
 
+_Note: you can obtain a Auth token [here](https://docs.apolloapi.io/docs/api/authentication), sign up today on our [Site](https://app.apolloapi.io/)_
+
 ```python
 # import the package
 from apollo.client import Apollo
 
 # Use our custom model to test building decisions
-Apollo.use("Apollo")
+Apollo.use("apollo", token="YOUR_API_TOKEN_HERE")
 
-# We support video, speech, image and text. Try text!
+# Lets check to see if a phrase contains threats
 Apollo.detectText("Phrase1", "contains", "Threats")
+
+# Create custom rules which creates a task!
+Apollo.rule('Phrase1', '>=', '0.8')
+
+# Connect with other models!
+Apollo.use('Google', "violence", ...)
+
+Apollo.detectImage('Image1', 'contains', 'VERY_LIKELY') # Image Analysis/OCR
+Apollo.detectSpeech('Audio1', 'contains', 'UNLIKELY') # Audio Processing
+Apollo.detectVideo('Video1', 'contains', 'POSSIBLE') # Video Analysis
+Apollo.detectText('Phrase1', 'contains', 'UNKNOWN') # Text Analysis
 ```
 
 That's all it takes!
 
-That's all it takes! You can check out [more on our notion page](https://cloudguruab.notion.site/Apollo-e5e347745c1e43798d849d79cce90aba).
+## Apollo then takes care of:
+
+- Detecting real-time changes in your data
+- Automating tasks against image, video, audio or text
+- Simplifying the process of deploying AI models
+- Making sure your integration is robust, so you never again have to worry about stuck/stale data or false-positives
+
+In practice, you probably want to use one of our native SDKs to interact with Apollo's API or use our custom browser client so you dont have to write code. If so, sign up at [Apollo API](https://app.apolloapi.io/signup)!
+
+## 🧑‍💻 Cool, what can I build with it?
 
-In practice, you probably want to use one of our native SDKs to interact with Apollo's API or use our custom browser client so you dont have to write code. If so, ping us at adrian@apolloapi.io!
+- Trust & Safety teams can use Apollo to **build native in-app connections** related to active response, content moderation, fraud detection, etc.
+- Some **automate their personal lives** with Apollo by integrating against discord communities or their personal lives
+- Apollo can help you **quickly automate tasks** for hobby projects, communities or business
 
 ## Contributing
 
 ### 📦 pre-commit config
 
 As an open source project, Apollo welcomes contributions from the community at large. This isn’t an exhaustive reference and is a living document subject to change as needed when the project formalizes any practice or pattern.
 
@@ -136,14 +140,15 @@
 ```
 <type>: <summary>
 
 <body>
 ```
 
 Accepted `<type>` values:
+
 - new = newly implemented user-facing features
 - chg = changes in existing user-facing features
 - fix = user-facing bugfixes
 - oth = other changes which users should know about
 - dev = any developer-facing changes, regardless of new/chg/fix status
 
 #### Summary (The first line)
```

#### html2text {}

```diff
@@ -1,66 +1,73 @@
+Metadata-Version: 2.1 Name: apollo-sdk Version: 0.1.6 Summary: Build automated
+decision making workflows by aggregating your AI models and data into one api.
+Home-page: https://github.com/apolloapi/apolloapi Author: Apollo API, Inc.
+Author-email: adrbrownx@gmail.com License: Elastic License v2 Classifier:
+Intended Audience :: Developers Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
+Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9 Description-Content-Type:
+text/markdown License-File: LICENSE
     ![ApolloLogo](https://uploads-ssl.webflow.com/640ca38ad086fde245b76c9d/
-  643fffb82419ac18d39e3e4e_Screenshot%202023-04-19%20at%2010.50.13%20AM.png)
-    ****** The easiest way to build custom decision making workflows ******
-Apollo gives you access to custom machine learning models, no-code platform and
- continuously syncs data from any API or Database to centralize investigations
- and allow you to automate the detection of harm in images, videos, audio and
-                                     text.
+                     6455b1fd3d8642575f793c94_header.png)
+                   ****** Open-source Task Automation ******
+   Apollo is an open-source no-code platform that helps you build automated
+workflows in minutes. Our SDK allows you to automate tasks such as; onboarding,
+    compliance, trust & safety, fraud detection, code generation and more.
 
                                    Docs_Â»
 
-         Examples Join_the_waitlist Â· Report_Bug Â· Community_Discord
-## â­ Can you show me an example? In your code you can write: ```ts
-Apollo.connect('postgres://username:password@hostnam...', ...) // Starts
-syncing content forever! Apollo.use('OpenAI', "moderation", ...) // Connect to
-existing providers! Apollo.rule('Phrase1', '>=', '0.8') // Create custom rules!
-Apollo.use('Apollo', "violence", ...) // Connect with our internal models! /
-/ Detect bad actors at scale! Apollo.detectImage('Image1', 'contains',
-'VERY_LIKELY') // Image Analysis/OCR Apollo.detectSpeech('Audio1', 'contains',
-'UNLIKELY') // Audio Processing Apollo.detectVideo('Video1', 'contains',
-'POSSIBLE') // Video Analysis Apollo.detectText('Phrase1', 'contains',
-'UNKNOWN') // Text Analysis ``` Apollo then takes care of: - Detecting real-
-time changes in user experience - Automated detection against image, video,
-audio or text - Connecting policy to product - Making sure your integration is
-robust, so you never again have to worry about stuck/stale data or false-
-positives ## ð§âð» Cool, what can I build with it? - Trust & Safety teams
-in companies use Apollo to **build native in-app connections** related to
-active response, content moderation, fraud detection, etc. - Some **automate
-their personal lives** with Apollo by integrating against discord communities
-or other decentralized networks for safety - Apollo can help you **quickly
-build trust** for hobby projects, communities or business ## ð Interesting,
-how can I try it? Let's setup your first Integration in 2 minutes! It will pull
-from your local database (and keep it in sync). To start: ```bash # install the
-cli-toolkit pip install apollo-sdk # enter a python repl or create a python
-file, up to you! (repl is easiest) python3 ``` ```python # import the package
-from apollo.client import Apollo # sync data from your database instance # (we
-support supabase at the current moment or postgresql via uri format)
-Apollo.connect("postgres://username:password@hostname:port/database_name") # If
-you want to test out operation on your external connection Apollo.fetch_tables
-() Apollo.query("desc", "table", "column") ``` Test sending your content to our
-API! ...and create a workflow with a simple command: ```python # import the
+             Join_the_waitlist Â· Report_Bug Â· Community_Discord
+## Why Apollo API? Before Apollo, integrating AI models and building automated
+workflows could be time-consuming and complex, with Apollo, teams can simplify
+and accelerate the process, making it easier to deploy AI models, sync data,
+and develop insights in minutes. ## ð Interesting, how can I try it? Lets
+install the SDK first... ```bash pip install apollo-sdk ``` Let's setup your
+first Integration! It will pull from your local database (and keep it in sync).
+```python # import the package from apollo.client import Apollo # sync data
+from your database instance # (we support supabase at the current moment or
+postgresql via uri format) Apollo.connect("postgres://username:
+password@hostname:port/database_name") # If you want to test out operation on
+your external connection Apollo.fetch_tables() Apollo.query("desc", "table",
+"column") ``` ...and create a workflow with a simple command: _Note: you can
+obtain a Auth token [here](https://docs.apolloapi.io/docs/api/authentication),
+sign up today on our [Site](https://app.apolloapi.io/)_ ```python # import the
 package from apollo.client import Apollo # Use our custom model to test
-building decisions Apollo.use("Apollo") # We support video, speech, image and
-text. Try text! Apollo.detectText("Phrase1", "contains", "Threats") ``` That's
-all it takes! That's all it takes! You can check out [more on our notion page]
-(https://cloudguruab.notion.site/Apollo-e5e347745c1e43798d849d79cce90aba). In
-practice, you probably want to use one of our native SDKs to interact with
-Apollo's API or use our custom browser client so you dont have to write code.
-If so, ping us at adrian@apolloapi.io! ## Contributing ### ð¦ pre-commit
-config As an open source project, Apollo welcomes contributions from the
-community at large. This isnât an exhaustive reference and is a living
-document subject to change as needed when the project formalizes any practice
-or pattern. Clone the repo and start Apollo locally... ```bash git clone https:
-//github.com/apolloapi/apolloapi.git cd apolloapi && python3 -m venv env &&
-source env/bin/activate && pip install -r requirements.txt ``` - After
-installing system dependencies be sure to install pre-commit for lint checks
-```bash pip install pre-commit pre-commit install pre-commit run --all-files
-``` Apollo uses commit messages for automated generation of project changelog.
-For every pull request we request contributors to be compliant with the
-following commit message notation. ``` :
+building decisions Apollo.use("apollo", token="YOUR_API_TOKEN_HERE") # Lets
+check to see if a phrase contains threats Apollo.detectText("Phrase1",
+"contains", "Threats") # Create custom rules which creates a task! Apollo.rule
+('Phrase1', '>=', '0.8') # Connect with other models! Apollo.use('Google',
+"violence", ...) Apollo.detectImage('Image1', 'contains', 'VERY_LIKELY') #
+Image Analysis/OCR Apollo.detectSpeech('Audio1', 'contains', 'UNLIKELY') #
+Audio Processing Apollo.detectVideo('Video1', 'contains', 'POSSIBLE') # Video
+Analysis Apollo.detectText('Phrase1', 'contains', 'UNKNOWN') # Text Analysis
+``` That's all it takes! ## Apollo then takes care of: - Detecting real-time
+changes in your data - Automating tasks against image, video, audio or text -
+Simplifying the process of deploying AI models - Making sure your integration
+is robust, so you never again have to worry about stuck/stale data or false-
+positives In practice, you probably want to use one of our native SDKs to
+interact with Apollo's API or use our custom browser client so you dont have to
+write code. If so, sign up at [Apollo API](https://app.apolloapi.io/signup)! ##
+ð§âð» Cool, what can I build with it? - Trust & Safety teams can use
+Apollo to **build native in-app connections** related to active response,
+content moderation, fraud detection, etc. - Some **automate their personal
+lives** with Apollo by integrating against discord communities or their
+personal lives - Apollo can help you **quickly automate tasks** for hobby
+projects, communities or business ## Contributing ### ð¦ pre-commit config As
+an open source project, Apollo welcomes contributions from the community at
+large. This isnât an exhaustive reference and is a living document subject to
+change as needed when the project formalizes any practice or pattern. Clone the
+repo and start Apollo locally... ```bash git clone https://github.com/
+apolloapi/apolloapi.git cd apolloapi && python3 -m venv env && source env/bin/
+activate && pip install -r requirements.txt ``` - After installing system
+dependencies be sure to install pre-commit for lint checks ```bash pip install
+pre-commit pre-commit install pre-commit run --all-files ``` Apollo uses commit
+messages for automated generation of project changelog. For every pull request
+we request contributors to be compliant with the following commit message
+notation. ``` :
 ``` Accepted `` values: - new = newly implemented user-facing features - chg =
 changes in existing user-facing features - fix = user-facing bugfixes - oth =
 other changes which users should know about - dev = any developer-facing
 changes, regardless of new/chg/fix status #### Summary (The first line) The
 first line should not be longer than 75 characters, the second line is always
 blank and other lines should be wrapped at 80 characters. ## ð Neat, I would
 like to learn more â­ Follow our development by starring us here on GitHub â­
```

### Comparing `apollo-sdk-0.1.4/apollo/__init__.py` & `apollo-sdk-0.1.6/apollo/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,10 +27,10 @@
 
 
 def get_firebase_client(service_account_key) -> AbstractFirebaseClient:
     client = import_string(FIREBASE_CLIENT_CLASS)
     return client(service_account_key)
 
 
-def get_json_client() -> AbstractRestClient:
+def get_json_client(api_key) -> AbstractRestClient:
     client = import_string(REST_CLIENT_CLASS)
-    return client
+    return client(api_key)
```

### Comparing `apollo-sdk-0.1.4/apollo/client.py` & `apollo-sdk-0.1.6/apollo/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,22 +97,26 @@
             1. Apollo.fetch_tables()
             2. Apollo.query([desc/asc], [table], [column])
         """
         cls.psql_curs = cls._manager.connect_to_prefix(db_url)
         return "Syncing data with Apollo"
 
     @classmethod
-    def use(cls, provider, *args, **kwargs):
-        if provider == "Apollo":
+    def use(cls, provider, token=None, *args, **kwargs):
+        if provider.lower() == "apollo":
             cls.model = "Apollo"
-            return f"Connected to {provider} provider, using Safety model"
+            if token:
+                cls._auth_token = token
+                print(f"Connected to {provider} provider, using Safety model")
+            else:
+                print("Please set a auth token")
         else:
             return f"Provider {provider} not found"
 
     @classmethod
     def detectText(cls, text, operator, threshold):
         if cls.model:
-            print(cls.model)
-            conn = cls._service_manager.connect()
+            # print(cls.model)
+            conn = cls._service_manager.connect(cls._auth_token)
             return conn.make_https_request({"rule": f"{text} {operator} {threshold}"})
         else:
             return "No provider connected"
```

### Comparing `apollo-sdk-0.1.4/apollo/connectors/__init__.py` & `apollo-sdk-0.1.6/apollo/connectors/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.4/apollo/connectors/aws/__init__.py` & `apollo-sdk-0.1.6/apollo/connectors/aws/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.4/apollo/connectors/google/__init__.py` & `apollo-sdk-0.1.6/apollo/connectors/google/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.4/apollo/connectors/microsoft/__init__.py` & `apollo-sdk-0.1.6/apollo/connectors/microsoft/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.4/apollo/connectors/openai/__init__.py` & `apollo-sdk-0.1.6/apollo/connectors/openai/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.4/apollo/const.py` & `apollo-sdk-0.1.6/apollo/const.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.4/apollo/database/__init__.py` & `apollo-sdk-0.1.6/apollo/database/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.4/apollo/database/firebase/__init__.py` & `apollo-sdk-0.1.6/apollo/database/firebase/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.4/apollo/database/firebase/base.py` & `apollo-sdk-0.1.6/apollo/database/firebase/base.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.4/apollo/database/firebase/cloud.py` & `apollo-sdk-0.1.6/apollo/database/firebase/cloud.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.4/apollo/database/firebase/local.py` & `apollo-sdk-0.1.6/apollo/database/firebase/local.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.4/apollo/database/mongo/__init__.py` & `apollo-sdk-0.1.6/apollo/database/mongo/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.4/apollo/database/mysql/__init__.py` & `apollo-sdk-0.1.6/apollo/database/mysql/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.4/apollo/database/postgres/__init__.py` & `apollo-sdk-0.1.6/apollo/database/postgres/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.4/apollo/database/supabase/__init__.py` & `apollo-sdk-0.1.6/apollo/database/supabase/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.4/apollo/database/supabase/base.py` & `apollo-sdk-0.1.6/apollo/database/supabase/base.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.4/apollo/database/supabase/cloud.py` & `apollo-sdk-0.1.6/apollo/database/supabase/cloud.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.4/apollo/database/supabase/local.py` & `apollo-sdk-0.1.6/apollo/database/supabase/local.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.4/apollo/exceptions.py` & `apollo-sdk-0.1.6/apollo/exceptions.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.4/apollo/manager.py` & `apollo-sdk-0.1.6/apollo/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,9 +39,9 @@
     @staticmethod
     def connect_to_prefix(service_account_key):
         return get_firebase_client(service_account_key)
 
 
 class JSONConnectionManager:
     @staticmethod
-    def connect():
-        return get_json_client()
+    def connect(api_key):
+        return get_json_client(api_key)
```

### Comparing `apollo-sdk-0.1.4/apollo/resource.py` & `apollo-sdk-0.1.6/apollo/resource.py`

 * *Files 3% similar despite different names*

```diff
@@ -38,12 +38,15 @@
 
 
 class JSON:
 
     # Service utility class
     _service_manager = JSONConnectionManager()
 
+    # Token
+    _auth_token = None
+
 
 class General(Postgres, JSON):
 
     # Current LLM to be used
     model = None
```

### Comparing `apollo-sdk-0.1.4/apollo/service/__init__.py` & `apollo-sdk-0.1.6/apollo/service/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.4/apollo/service/graphql/__init__.py` & `apollo-sdk-0.1.6/apollo/service/graphql/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.4/apollo/service/json/__init__.py` & `apollo-sdk-0.1.6/apollo/service/json/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.4/apollo/service/json/base.py` & `apollo-sdk-0.1.6/apollo/service/json/base.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.4/apollo/service/json/cloud.py` & `apollo-sdk-0.1.6/apollo/service/json/cloud.py`

 * *Files 7% similar despite different names*

```diff
@@ -16,20 +16,22 @@
 import requests
 
 from apollo.service.json.base import AbstractRestClient
 from apollo.const import test_token
 
 
 class RestClient(AbstractRestClient):
+    def __init__(self, api_key):
+        self.api_key = api_key
+
     @staticmethod
     def make_http_request():
         return None
 
-    @staticmethod
-    def make_https_request(body):
+    def make_https_request(self, body):
         response = requests.post(
             "https://api.apolloapi.io/api/v1/apollo/",
-            headers={"Authorization": f"Token {test_token}"},
+            headers={"Authorization": f"Token {self.api_key}"},
             json=body,
             timeout=10,
         )
         return response.json()
```

### Comparing `apollo-sdk-0.1.4/apollo/service/json/local.py` & `apollo-sdk-0.1.6/apollo/service/json/local.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.4/apollo/tests/__init__.py` & `apollo-sdk-0.1.6/apollo/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `apollo-sdk-0.1.4/apollo_sdk.egg-info/SOURCES.txt` & `apollo-sdk-0.1.6/apollo_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

