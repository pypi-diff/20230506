# Comparing `tmp/polymatica_api-0.0.9.tar.gz` & `tmp/polymatica_api-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polymatica_api-0.0.9.tar", last modified: Wed May  3 13:20:10 2023, max compression
+gzip compressed data, was "polymatica_api-0.1.0.tar", last modified: Sat May  6 17:32:07 2023, max compression
```

## Comparing `polymatica_api-0.0.9.tar` & `polymatica_api-0.1.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 leggnom    (501) staff       (20)        0 2023-05-03 13:20:10.833235 polymatica_api-0.0.9/
--rw-r--r--   0 leggnom    (501) staff       (20)     1076 2023-05-02 01:53:27.000000 polymatica_api-0.0.9/LICENSE
--rw-r--r--   0 leggnom    (501) staff       (20)      870 2023-05-03 13:20:10.833053 polymatica_api-0.0.9/PKG-INFO
--rw-r--r--   0 leggnom    (501) staff       (20)      677 2023-05-03 07:03:34.000000 polymatica_api-0.0.9/README.md
-drwxr-xr-x   0 leggnom    (501) staff       (20)        0 2023-05-03 13:20:10.831435 polymatica_api-0.0.9/polymatica_api/
--rw-r--r--   0 leggnom    (501) staff       (20)     1573 2023-05-03 06:42:47.000000 polymatica_api-0.0.9/polymatica_api/__init__.py
--rw-r--r--   0 leggnom    (501) staff       (20)      320 2023-05-03 06:52:44.000000 polymatica_api-0.0.9/polymatica_api/data.py
--rw-r--r--   0 leggnom    (501) staff       (20)     3874 2023-05-03 13:19:54.000000 polymatica_api-0.0.9/polymatica_api/data_option.py
--rw-r--r--   0 leggnom    (501) staff       (20)     1258 2023-05-03 06:46:48.000000 polymatica_api-0.0.9/polymatica_api/types.py
-drwxr-xr-x   0 leggnom    (501) staff       (20)        0 2023-05-03 13:20:10.832755 polymatica_api-0.0.9/polymatica_api.egg-info/
--rw-r--r--   0 leggnom    (501) staff       (20)      870 2023-05-03 13:20:10.000000 polymatica_api-0.0.9/polymatica_api.egg-info/PKG-INFO
--rw-r--r--   0 leggnom    (501) staff       (20)      319 2023-05-03 13:20:10.000000 polymatica_api-0.0.9/polymatica_api.egg-info/SOURCES.txt
--rw-r--r--   0 leggnom    (501) staff       (20)        1 2023-05-03 13:20:10.000000 polymatica_api-0.0.9/polymatica_api.egg-info/dependency_links.txt
--rw-r--r--   0 leggnom    (501) staff       (20)       34 2023-05-03 13:20:10.000000 polymatica_api-0.0.9/polymatica_api.egg-info/requires.txt
--rw-r--r--   0 leggnom    (501) staff       (20)       15 2023-05-03 13:20:10.000000 polymatica_api-0.0.9/polymatica_api.egg-info/top_level.txt
--rw-r--r--   0 leggnom    (501) staff       (20)       38 2023-05-03 13:20:10.833315 polymatica_api-0.0.9/setup.cfg
--rw-r--r--   0 leggnom    (501) staff       (20)      569 2023-05-03 13:19:54.000000 polymatica_api-0.0.9/setup.py
+drwxr-xr-x   0 leggnom    (501) staff       (20)        0 2023-05-06 17:32:07.320909 polymatica_api-0.1.0/
+-rw-r--r--   0 leggnom    (501) staff       (20)     1076 2023-05-02 01:53:27.000000 polymatica_api-0.1.0/LICENSE
+-rw-r--r--   0 leggnom    (501) staff       (20)     1141 2023-05-06 17:32:07.320717 polymatica_api-0.1.0/PKG-INFO
+-rw-r--r--   0 leggnom    (501) staff       (20)      948 2023-05-06 17:31:41.000000 polymatica_api-0.1.0/README.md
+drwxr-xr-x   0 leggnom    (501) staff       (20)        0 2023-05-06 17:32:07.319233 polymatica_api-0.1.0/polymatica_api/
+-rw-r--r--   0 leggnom    (501) staff       (20)     2474 2023-05-06 17:26:38.000000 polymatica_api-0.1.0/polymatica_api/__init__.py
+-rw-r--r--   0 leggnom    (501) staff       (20)      320 2023-05-03 06:52:44.000000 polymatica_api-0.1.0/polymatica_api/data.py
+-rw-r--r--   0 leggnom    (501) staff       (20)     5825 2023-05-06 15:46:48.000000 polymatica_api-0.1.0/polymatica_api/data_option.py
+-rw-r--r--   0 leggnom    (501) staff       (20)     2370 2023-05-06 15:20:02.000000 polymatica_api-0.1.0/polymatica_api/types.py
+drwxr-xr-x   0 leggnom    (501) staff       (20)        0 2023-05-06 17:32:07.320453 polymatica_api-0.1.0/polymatica_api.egg-info/
+-rw-r--r--   0 leggnom    (501) staff       (20)     1141 2023-05-06 17:32:07.000000 polymatica_api-0.1.0/polymatica_api.egg-info/PKG-INFO
+-rw-r--r--   0 leggnom    (501) staff       (20)      319 2023-05-06 17:32:07.000000 polymatica_api-0.1.0/polymatica_api.egg-info/SOURCES.txt
+-rw-r--r--   0 leggnom    (501) staff       (20)        1 2023-05-06 17:32:07.000000 polymatica_api-0.1.0/polymatica_api.egg-info/dependency_links.txt
+-rw-r--r--   0 leggnom    (501) staff       (20)       34 2023-05-06 17:32:07.000000 polymatica_api-0.1.0/polymatica_api.egg-info/requires.txt
+-rw-r--r--   0 leggnom    (501) staff       (20)       15 2023-05-06 17:32:07.000000 polymatica_api-0.1.0/polymatica_api.egg-info/top_level.txt
+-rw-r--r--   0 leggnom    (501) staff       (20)       38 2023-05-06 17:32:07.320973 polymatica_api-0.1.0/setup.cfg
+-rw-r--r--   0 leggnom    (501) staff       (20)      569 2023-05-06 14:49:31.000000 polymatica_api-0.1.0/setup.py
```

### Comparing `polymatica_api-0.0.9/LICENSE` & `polymatica_api-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `polymatica_api-0.0.9/PKG-INFO` & `polymatica_api-0.1.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,34 +1,40 @@
 Metadata-Version: 2.1
 Name: polymatica_api
-Version: 0.0.9
+Version: 0.1.0
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 This is a simple example of getting data from a server Polymatica Platform
 
 ```python
 from polymatica_api import PolymaticaAPI
-from polymatica_api.types import DataOptionMethod
+from polymatica_api.data_option import FilterAnd
+from polymatica_api.types import DataOptionMethod, FilterMethod, SortDirection
 import pandas as pd
 
 
 p = PolymaticaAPI('{SERVER_URL}', 'Token {TOKEN}')
 response = p.get_data([
     p.from_dataset('world_population.csv').
     method(DataOptionMethod.Aggregate).
     group("Country/Territory").
     sum(
         '2000 Population', 
         '2010 Population', 
         '2015 Population',
         '2020 Population',
         '2022 Population',
+    ).
+    sort("Country/Territory", SortDirection.Desc).
+    sort("2010 Population", SortDirection.Desc).
+    set_filter(
+        FilterAnd("Country/Territory", FilterMethod.Equal, "Jamaica")
     )
 ])
 
 data = response.get('default')
 frame = pd.DataFrame(data.rows)
 frame.rename(columns=data.column_map, inplace=True)
 print(frame)
```

### Comparing `polymatica_api-0.0.9/polymatica_api/__init__.py` & `polymatica_api-0.1.0/polymatica_api/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,14 +5,18 @@
 import requests
 import urllib.parse
 
 
 HOST_ROUTE = dict(
     dataset='/proxy/manager/api/v1/dataset',
     data_dataset='/proxy/manager/api/v1/data/dataset',
+    write_line='/api/v1/data-line/{id}',
+    write_lines='/api/v1/data-line/{id}/rows',
+    delete_line='/api/v1/data-line/{id}/{uid}',
+    update_line='/api/v1/data-line/{id}/{uid}'
 )
 
 
 class PolymaticaAPI:
     _host: str
     _session: requests.Session
 
@@ -22,26 +26,38 @@
         self._session.headers = {
             "Authorization": token
         }
 
     def from_dataset(self, name) -> DataOption:
         return DataOption(name, self)
 
+    def delete_line(self, dataset_id: int, line_id: str):
+        return self._session.delete(self.route('delete_line').format(id=dataset_id, uid=line_id)).json()
+
+    def update_line(self, dataset_id: int, line_id: str, row: typing.Dict):
+        return self._session.put(self.route('update_line').format(id=dataset_id, uid=line_id), json=row).json()
+
+    def write_line(self, dataset_id: int, row: typing.Dict):
+        return self._session.post(self.route('write_line').format(id=dataset_id), json=row).json()
+
+    def write_lines(self, dataset_id: int, rows: typing.List[typing.Dict]):
+        return self._session.post(self.route('write_lines').format(id=dataset_id), json=rows).json()
+
     def get_dataset(self, name) -> typing.Optional[Dataset]:
         data = self._session.get(self.route('dataset'), params=dict(
             name=name
         )).json()
 
         for item in data.get('rows'):
             dataset = Dataset.parse_obj(item)
             if dataset.name == name:
                 return dataset
         return None
 
-    def get_data(self, options, get_columns: bool = True, get_dataset: bool = False):
+    def get_data(self, options, get_columns: bool = True, get_dataset: bool = False) -> typing.Dict[str, Data]:
         data = self._session.post(self.route('data_dataset'), json=dict(
             data_options=list(map(lambda item: item.make(), options)),
             get_columns=get_columns,
             get_dataset=get_dataset
         )).json()
 
         result = dict()
```

### Comparing `polymatica_api-0.0.9/setup.py` & `polymatica_api-0.1.0/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 requires = [
     "pydantic==1.10.7",
     "requests==2.29.0"
 ]
 
 setuptools.setup(
     name="polymatica_api",
-    version="0.0.9",
+    version="0.1.0",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3"
     ],
     python_requires='>=3.7',
```

