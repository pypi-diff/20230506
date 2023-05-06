# Comparing `tmp/klarity-connector-0.1.3.tar.gz` & `tmp/klarity-connector-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klarity-connector-0.1.3.tar", last modified: Thu Oct 27 07:25:48 2022, max compression
+gzip compressed data, was "klarity-connector-0.1.4.tar", last modified: Sat May  6 17:53:35 2023, max compression
```

## Comparing `klarity-connector-0.1.3.tar` & `klarity-connector-0.1.4.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxr-xr-x   0 kacper.szczepanek   (503) staff       (20)        0 2022-10-27 07:25:48.349400 klarity-connector-0.1.3/
--rw-r--r--   0 kacper.szczepanek   (503) staff       (20)     1902 2022-10-27 07:25:48.349173 klarity-connector-0.1.3/PKG-INFO
-drwxr-xr-x   0 kacper.szczepanek   (503) staff       (20)        0 2022-10-27 07:25:48.348162 klarity-connector-0.1.3/klarity_connector/
--rw-r--r--   0 kacper.szczepanek   (503) staff       (20)       57 2022-10-17 13:14:52.000000 klarity-connector-0.1.3/klarity_connector/__init__.py
--rw-r--r--   0 kacper.szczepanek   (503) staff       (20)     2078 2022-10-17 10:29:25.000000 klarity-connector-0.1.3/klarity_connector/connector.py
-drwxr-xr-x   0 kacper.szczepanek   (503) staff       (20)        0 2022-10-27 07:25:48.348992 klarity-connector-0.1.3/klarity_connector.egg-info/
--rw-r--r--   0 kacper.szczepanek   (503) staff       (20)     1902 2022-10-27 07:25:48.000000 klarity-connector-0.1.3/klarity_connector.egg-info/PKG-INFO
--rw-r--r--   0 kacper.szczepanek   (503) staff       (20)      273 2022-10-27 07:25:48.000000 klarity-connector-0.1.3/klarity_connector.egg-info/SOURCES.txt
--rw-r--r--   0 kacper.szczepanek   (503) staff       (20)        1 2022-10-27 07:25:48.000000 klarity-connector-0.1.3/klarity_connector.egg-info/dependency_links.txt
--rw-r--r--   0 kacper.szczepanek   (503) staff       (20)        9 2022-10-27 07:25:48.000000 klarity-connector-0.1.3/klarity_connector.egg-info/requires.txt
--rw-r--r--   0 kacper.szczepanek   (503) staff       (20)       18 2022-10-27 07:25:48.000000 klarity-connector-0.1.3/klarity_connector.egg-info/top_level.txt
--rw-r--r--   0 kacper.szczepanek   (503) staff       (20)       38 2022-10-27 07:25:48.349476 klarity-connector-0.1.3/setup.cfg
--rw-r--r--   0 kacper.szczepanek   (503) staff       (20)     1445 2022-10-27 07:25:40.000000 klarity-connector-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 17:53:35.332884 klarity-connector-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-06 17:53:23.000000 klarity-connector-0.1.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-05-06 17:53:35.332884 klarity-connector-0.1.4/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 17:53:35.332884 klarity-connector-0.1.4/klarity_connector/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-06 17:53:23.000000 klarity-connector-0.1.4/klarity_connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2185 2023-05-06 17:53:23.000000 klarity-connector-0.1.4/klarity_connector/connector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 17:53:35.332884 klarity-connector-0.1.4/klarity_connector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1958 2023-05-06 17:53:35.000000 klarity-connector-0.1.4/klarity_connector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-06 17:53:35.000000 klarity-connector-0.1.4/klarity_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 17:53:35.000000 klarity-connector-0.1.4/klarity_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-06 17:53:35.000000 klarity-connector-0.1.4/klarity_connector.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-06 17:53:35.000000 klarity-connector-0.1.4/klarity_connector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 17:53:35.332884 klarity-connector-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1495 2023-05-06 17:53:23.000000 klarity-connector-0.1.4/setup.py
```

### Comparing `klarity-connector-0.1.3/PKG-INFO` & `klarity-connector-0.1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: klarity-connector
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python connector to GraphQL API of Klarity
 Home-page: https://github.com/Kacperek0/klarity-connector
 Author: Kacper Szczepanek
 Author-email: pypi@szczepanek.dev
 License: MIT
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
 
 ### Klarity Connector
 Python connector for Klarity API
 
 #### Installation
 ```bash
 pip install klarity-connector
@@ -71,9 +72,7 @@
 
 response = connector.graphql_request(mutation, variables)
 
 ```
 
 ### Official product documentation
 [docs](https://docs.klarity.nordcloudapp.com)
-
-
```

### Comparing `klarity-connector-0.1.3/klarity_connector/connector.py` & `klarity-connector-0.1.4/klarity_connector/connector.py`

 * *Files 9% similar despite different names*

```diff
@@ -13,20 +13,21 @@
     :param region: Region to connect to. Valid values are 'us', 'eu' and 'uk'.
     :type region: str
 
     :param api_key: API key for Klarity.
     :type api_key: str
 
     """
-    def __init__(self, region: str, api_key: str):
+    def __init__(self, region: str, api_key: str, billing_period: str = 'current'):
         """
         Establish Klarity connection
         """
         self.region = region
         self.api_key = api_key
+        self.billing_period = billing_period
         self.url = self.__get_url(region)
 
         self.retry_strategy = Retry(
             total=10,
             status_forcelist=[500, 502, 503, 504],
             allowed_methods=['POST'],
             backoff_factor=3
@@ -39,36 +40,36 @@
         self.session.mount('https://', self.adapter)
 
 
     def __get_url(self, region) -> str:
         """
         Get url for region
         """
-        match region:
-            case 'us':
-                return 'https://api.cnop-int.us.nordcloudapp.com/graphql'
-            case 'eu':
-                return 'https://api.cnop-int.nordcloudapp.com/graphql'
-            case 'uk':
-                return 'https://api.cnop-int.uk.nordcloudapp.com/graphql'
-            case _:
-                raise ValueError(f'Invalid region: {region}')
+        if region == 'us':
+            return 'https://api.cnop-int.us.nordcloudapp.com/graphql'
+        elif region == 'eu':
+            return 'https://api.cnop-int.nordcloudapp.com/graphql'
+        elif region == 'uk':
+            return 'https://api.cnop-int.uk.nordcloudapp.com/graphql'
+        else:
+            raise ValueError(f'Invalid region: {region}')
 
     def graphql_request(self, query: str, variables: dict = None) -> dict:
         """
         Send GraphQL request
         """
 
         response = self.session.post(
             self.url,
             json={
                 'query': query,
                 'variables': variables
             }, headers={
-                'x-api-key': self.api_key
+                'x-api-key': self.api_key,
+                'x-billing-period': self.billing_period
             }
         )
 
         if response.status_code != 200:
             print(f'GraphQL request failed with status code {response.status_code} and response body {response.text}')
 
         return json.loads(response.text)
```

### Comparing `klarity-connector-0.1.3/klarity_connector.egg-info/PKG-INFO` & `klarity-connector-0.1.4/klarity_connector.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 Metadata-Version: 2.1
 Name: klarity-connector
-Version: 0.1.3
+Version: 0.1.4
 Summary: Python connector to GraphQL API of Klarity
 Home-page: https://github.com/Kacperek0/klarity-connector
 Author: Kacper Szczepanek
 Author-email: pypi@szczepanek.dev
 License: MIT
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
+License-File: LICENSE.md
 
 ### Klarity Connector
 Python connector for Klarity API
 
 #### Installation
 ```bash
 pip install klarity-connector
@@ -71,9 +72,7 @@
 
 response = connector.graphql_request(mutation, variables)
 
 ```
 
 ### Official product documentation
 [docs](https://docs.klarity.nordcloudapp.com)
-
-
```

### Comparing `klarity-connector-0.1.3/setup.py` & `klarity-connector-0.1.4/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # Get the long description from the README file
 with open(path.join(HERE, 'readme.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 # This call to setup() does all the work
 setup(
     name="klarity-connector",
-    version="0.1.3",
+    version="0.1.4",
     description="Python connector to GraphQL API of Klarity",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Kacperek0/klarity-connector",
     author="Kacper Szczepanek",
     author_email="pypi@szczepanek.dev",
     license="MIT",
@@ -29,14 +29,15 @@
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Topic :: Software Development :: Libraries",
         "Operating System :: OS Independent"
     ],
     packages=["klarity_connector"],
     include_package_data=True,
     install_requires=["requests"]
 )
```

