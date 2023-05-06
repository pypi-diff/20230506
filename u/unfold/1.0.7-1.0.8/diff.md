# Comparing `tmp/unfold-1.0.7.tar.gz` & `tmp/unfold-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unfold-1.0.7.tar", last modified: Fri Apr 21 12:39:45 2023, max compression
+gzip compressed data, was "unfold-1.0.8.tar", last modified: Sat May  6 16:58:57 2023, max compression
```

## Comparing `unfold-1.0.7.tar` & `unfold-1.0.8.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:39:45.065472 unfold-1.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-04-21 12:39:34.000000 unfold-1.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-04-21 12:39:34.000000 unfold-1.0.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    45662 2023-04-21 12:39:45.065472 unfold-1.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-04-21 12:39:34.000000 unfold-1.0.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 12:39:45.065472 unfold-1.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-04-21 12:39:34.000000 unfold-1.0.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:39:45.061472 unfold-1.0.7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-04-21 12:39:34.000000 unfold-1.0.7/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-04-21 12:39:34.000000 unfold-1.0.7/tests/test_reproducing_db.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:39:45.061472 unfold-1.0.7/unfold/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-21 12:39:34.000000 unfold-1.0.7/unfold/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:39:45.061472 unfold-1.0.7/unfold/data/
--rw-r--r--   0 runner    (1001) docker     (123)   395147 2023-04-21 12:39:34.000000 unfold-1.0.7/unfold/data/flows_biosphere_38.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-04-21 12:39:34.000000 unfold-1.0.7/unfold/data/outdated_flows.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    12590 2023-04-21 12:39:34.000000 unfold-1.0.7/unfold/data_cleaning.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-21 12:39:34.000000 unfold-1.0.7/unfold/export.py
--rw-r--r--   0 runner    (1001) docker     (123)    31043 2023-04-21 12:39:34.000000 unfold-1.0.7/unfold/fold.py
--rw-r--r--   0 runner    (1001) docker     (123)    45022 2023-04-21 12:39:34.000000 unfold-1.0.7/unfold/unfold.py
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-04-21 12:39:34.000000 unfold-1.0.7/unfold/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:39:45.061472 unfold-1.0.7/unfold.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    45662 2023-04-21 12:39:45.000000 unfold-1.0.7/unfold.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-04-21 12:39:45.000000 unfold-1.0.7/unfold.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 12:39:45.000000 unfold-1.0.7/unfold.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-21 12:39:45.000000 unfold-1.0.7/unfold.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-21 12:39:45.000000 unfold-1.0.7/unfold.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:58:57.442960 unfold-1.0.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    34523 2023-05-06 16:58:49.000000 unfold-1.0.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-06 16:58:49.000000 unfold-1.0.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    45662 2023-05-06 16:58:57.442960 unfold-1.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-05-06 16:58:49.000000 unfold-1.0.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-06 16:58:57.442960 unfold-1.0.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2294 2023-05-06 16:58:49.000000 unfold-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:58:57.438959 unfold-1.0.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-05-06 16:58:49.000000 unfold-1.0.8/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1771 2023-05-06 16:58:49.000000 unfold-1.0.8/tests/test_reproducing_db.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:58:57.442960 unfold-1.0.8/unfold/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-06 16:58:49.000000 unfold-1.0.8/unfold/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:58:57.442960 unfold-1.0.8/unfold/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   395147 2023-05-06 16:58:49.000000 unfold-1.0.8/unfold/data/flows_biosphere_38.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3815 2023-05-06 16:58:49.000000 unfold-1.0.8/unfold/data/outdated_flows.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    12912 2023-05-06 16:58:49.000000 unfold-1.0.8/unfold/data_cleaning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-06 16:58:49.000000 unfold-1.0.8/unfold/export.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31043 2023-05-06 16:58:49.000000 unfold-1.0.8/unfold/fold.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45629 2023-05-06 16:58:49.000000 unfold-1.0.8/unfold/unfold.py
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-06 16:58:49.000000 unfold-1.0.8/unfold/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 16:58:57.442960 unfold-1.0.8/unfold.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    45662 2023-05-06 16:58:57.000000 unfold-1.0.8/unfold.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-06 16:58:57.000000 unfold-1.0.8/unfold.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 16:58:57.000000 unfold-1.0.8/unfold.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-06 16:58:57.000000 unfold-1.0.8/unfold.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-06 16:58:57.000000 unfold-1.0.8/unfold.egg-info/top_level.txt
```

### Comparing `unfold-1.0.7/LICENSE` & `unfold-1.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `unfold-1.0.7/PKG-INFO` & `unfold-1.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unfold
-Version: 1.0.7
+Version: 1.0.8
 Summary: Unpacks LCA scenario databases.
 Home-page: https://github.com/polca/premise
 Author: Romain Sacchi <romain.sacchi@psi.ch>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

### Comparing `unfold-1.0.7/README.md` & `unfold-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `unfold-1.0.7/setup.py` & `unfold-1.0.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         for filename in filenames:
             paths.append(os.path.join("..", path, filename))
     return paths
 
 
 setup(
     name="unfold",
-    version="1.0.7",
+    version="1.0.8",
     python_requires=">=3.9",
     packages=packages,
     author="Romain Sacchi <romain.sacchi@psi.ch>",
     license=open("LICENSE").read(),
     # Only if you have non-python data (CSV, etc.). Might need to change the directory name as well.
     include_package_data=True,
     install_requires=[
```

### Comparing `unfold-1.0.7/tests/test_reproducing_db.py` & `unfold-1.0.8/tests/test_reproducing_db.py`

 * *Files identical despite different names*

### Comparing `unfold-1.0.7/unfold/data/flows_biosphere_38.csv` & `unfold-1.0.8/unfold/data/flows_biosphere_38.csv`

 * *Files identical despite different names*

### Comparing `unfold-1.0.7/unfold/data/outdated_flows.yaml` & `unfold-1.0.8/unfold/data/outdated_flows.yaml`

 * *Files identical despite different names*

### Comparing `unfold-1.0.7/unfold/data_cleaning.py` & `unfold-1.0.8/unfold/data_cleaning.py`

 * *Files 4% similar despite different names*

```diff
@@ -178,15 +178,22 @@
 
     # Add a `product` field to technosphere exchanges
     for dataset in data:
         for exchange in dataset["exchanges"]:
             if exchange["type"] == "technosphere":
                 # Check if the field 'product' is present
                 if "product" not in exchange:
-                    exchange["product"] = correct_product_field(exchange, data, db)
+                    try:
+                        exchange["product"] = correct_product_field(exchange, data, db)
+                    except KeyError:
+                        print(
+                            "No activity found for exchange {}{} in: {}".format(
+                                exchange["name"], exchange["location"], dataset["name"]
+                            )
+                        )
 
     # Add a `code` field if missing
     for dataset in data:
         if "code" not in dataset:
             dataset["code"] = str(uuid.uuid4().hex)
 
     return data
```

### Comparing `unfold-1.0.7/unfold/export.py` & `unfold-1.0.8/unfold/export.py`

 * *Files identical despite different names*

### Comparing `unfold-1.0.7/unfold/fold.py` & `unfold-1.0.8/unfold/fold.py`

 * *Files identical despite different names*

### Comparing `unfold-1.0.7/unfold/unfold.py` & `unfold-1.0.8/unfold/unfold.py`

 * *Files 8% similar despite different names*

```diff
@@ -296,15 +296,18 @@
         remove_categories_for_technosphere_flows(data)
         return data
 
     def extract_additional_inventories(self) -> None:
         """Extracts additional inventories."""
         print("Extracting additional inventories...")
         with HiddenPrints():
-            i = bw2io.CSVImporter(self.package.get_resource("inventories").source)
+            filepath = self.package.get_resource("inventories").source
+            # ensure that all slashes in filepath are forward slashes
+            filepath = filepath.replace("\\", "/")
+            i = bw2io.CSVImporter(filepath)
             i.strategies = i.strategies[:4]
             i.apply_strategies()
             i.data = self.clean_imported_inventory(i.data)
 
         self.database.extend(i.data)
         self.database = change_db_name(self.database, self.package.descriptor["name"])
         self.build_mapping_for_dependencies(self.database)
@@ -386,14 +389,63 @@
         reference product, and location.
         """
         if (name, ref, loc, None) in self.dependency_mapping:
             return self.dependency_mapping[(name, ref, loc, None)][1]
         else:
             return str(uuid.uuid4().hex)
 
+    def find_correct_id(self, key: tuple) -> [tuple, None]:
+        if key[0] in self.outdated_flows:
+            if (
+                self.outdated_flows[key[0]],
+                key[1],
+                key[2],
+                key[3],
+            ) in self.dependency_mapping:
+                return self.outdated_flows[key[0]], key[1], key[2], key[3]
+
+            elif (
+                self.outdated_flows[key[0]].replace(", ion", ""),
+                key[1],
+                key[2],
+                key[3],
+            ) in self.dependency_mapping:
+                return (
+                    self.outdated_flows[key[0]].replace(", ion", ""),
+                    key[1],
+                    key[2],
+                    key[3],
+                )
+
+            elif (
+                self.outdated_flows[key[0]] + ", ion",
+                key[1],
+                key[2],
+                key[3],
+            ) in self.dependency_mapping:
+                return self.outdated_flows[key[0]] + ", ion", key[1], key[2], key[3]
+
+            elif (
+                key[0] + ", in ground",
+                key[1],
+                key[2],
+                key[3],
+            ) in self.dependency_mapping:
+                return key[0] + ", in ground", key[1], key[2], key[3]
+
+            else:
+                print("Could not find key", key)
+                return key
+
+    def fix_key(self, key: tuple) -> tuple:
+        if key in self.dependency_mapping:
+            return self.dependency_mapping[key]
+        else:
+            return self.dependency_mapping[self.find_correct_id(key)]
+
     def get_exchange(
         self,
         ind: int,
         amount: float = 1.0,
         scenario_name: str = None,
     ):
         """
@@ -405,78 +457,23 @@
         :param amount: amount of the exchange
         :param scenario_name: name of the scenario
         :return: dictionary of the exchange
         """
         name, ref, cat, loc, unit, flow_type = self.acts_indices[ind]
         _ = lambda x: x if x != 0 else 1.0
 
-        def fix_key(key: tuple) -> tuple:
-            if key in self.dependency_mapping:
-                return self.dependency_mapping[key]
-            else:
-                if key[0] in self.outdated_flows:
-                    if (
-                        self.outdated_flows[key[0]],
-                        key[1],
-                        key[2],
-                        key[3],
-                    ) in self.dependency_mapping:
-                        return self.dependency_mapping[
-                            (self.outdated_flows[key[0]], key[1], key[2], key[3])
-                        ]
-                    elif (
-                        self.outdated_flows[key[0]].replace(", ion", ""),
-                        key[1],
-                        key[2],
-                        key[3],
-                    ) in self.dependency_mapping:
-                        return self.dependency_mapping[
-                            (
-                                self.outdated_flows[key[0]].replace(", ion", ""),
-                                key[1],
-                                key[2],
-                                key[3],
-                            )
-                        ]
-                    elif (
-                        self.outdated_flows[key[0]] + ", ion",
-                        key[1],
-                        key[2],
-                        key[3],
-                    ) in self.dependency_mapping:
-                        return self.dependency_mapping[
-                            (
-                                self.outdated_flows[key[0]] + ", ion",
-                                key[1],
-                                key[2],
-                                key[3],
-                            )
-                        ]
-                    elif (
-                        key[0] + ", in ground",
-                        key[1],
-                        key[2],
-                        key[3],
-                    ) in self.dependency_mapping:
-                        return self.dependency_mapping[
-                            (key[0] + ", in ground", key[1], key[2], key[3])
-                        ]
-                    else:
-                        print("Could not find key", key)
-                        return key
-
         return {
             "name": name,
             "product": ref,
             "unit": unit,
             "location": loc,
             "categories": cat,
             "type": flow_type,
             "amount": amount if flow_type != "production" else _(amount),
-            "input": fix_key((name, ref, loc, cat))
+            "input": self.fix_key((name, ref, loc, cat))
             if flow_type == "biosphere"
             else (
                 scenario_name,
                 self.fetch_exchange_code(name, ref, loc),
             ),
         }
 
@@ -556,41 +553,50 @@
         # Iterate over the scaling factors defined in `self.factors`.
         for flow_id, factor in self.factors.items():
             # Extract the components of the flow ID, which are used to look up the indices in the matrix.
             c_name, c_prod, c_loc, c_unit = list(flow_id)[:4]
             s_name, s_prod, s_loc, s_cat, s_unit, s_type = list(flow_id)[4:]
 
             # Look up the index of the consumer activity in the reversed activities index.
-            consumer_idx = self.reversed_acts_indices[
+            consumer_idx = self.reversed_acts_indices.get(
                 (
                     c_name,
                     c_prod,
                     None,
                     c_loc,
                     c_unit,
                     "production",
-                )
-            ]
+                ),
+                None,
+            )
 
             # Look up the index of the supplier activity in the reversed activities index.
             supplier_id = (
                 s_name,
                 s_prod,
                 s_cat,
                 s_loc,
                 s_unit,
                 s_type,
             )
-            supplier_idx = self.reversed_acts_indices[supplier_id]
+            supplier_idx = self.reversed_acts_indices.get(
+                supplier_id,
+                None,
+            )
 
             # Multiply the appropriate element of the matrix by the scaling factor for the given scenario.
             # Use the lambda function defined above to avoid multiplying by zero.
-            matrix[supplier_idx, consumer_idx] = factor[scenario_name] * _(
-                matrix[supplier_idx, consumer_idx]
-            )
+            if supplier_idx is not None and consumer_idx is not None:
+                matrix[supplier_idx, consumer_idx] = factor[scenario_name] * _(
+                    matrix[supplier_idx, consumer_idx]
+                )
+            else:
+                print(
+                    f"Could not find activity for flow {flow_id} in scenario {scenario_name}."
+                )
 
         # Return the scaled matrix.
         return matrix
 
     def get_act_dict_structure(self, ind: int, scenario_name: str) -> dict:
         """
         Get the structure of the activity/dataset dictionary.
@@ -849,17 +855,18 @@
 
         # Find the scenarios to leave out of the scenario dataframe.
         scenarios_to_leave_out = list(
             set(s["name"] for s in self.scenarios) - set(scenarios_to_keep)
         )
 
         # Load the scenario dataframe from the `scenario_data` resource.
-        self.scenario_df = pd.DataFrame(
-            self.package.get_resource("scenario_data").read(keyed=True)
-        )
+        filepath = self.package.get_resource("scenario_data").source
+        # ensure that all slashes in filepath are forward slashes
+        filepath = filepath.replace("\\", "/")
+        self.scenario_df = pd.read_csv(filepath, keep_default_na=False, na_values="")
 
         # Remove rows corresponding to production flows.
         self.scenario_df = self.scenario_df.loc[
             (self.scenario_df["flow type"] != "production")
         ]
 
         # Drop columns corresponding to scenarios that were removed.
@@ -872,17 +879,19 @@
         # Convert strings to Python objects in columns that contain lists or tuples.
         self.scenario_df["from categories"] = self.scenario_df["from categories"].apply(
             lambda x: literal_eval(str(x))
         )
         self.scenario_df["to categories"] = self.scenario_df["to categories"].apply(
             lambda x: literal_eval(str(x))
         )
+
         self.scenario_df["from key"] = self.scenario_df["from key"].apply(
             lambda x: literal_eval(str(x))
         )
+
         self.scenario_df["to key"] = self.scenario_df["to key"].apply(
             lambda x: literal_eval(str(x))
         )
 
         # Convert columns corresponding to scenario exchange amounts to float dtype.
         self.scenario_df[scenarios_to_keep] = self.scenario_df[
             scenarios_to_keep
@@ -931,22 +940,44 @@
                     c_prod,
                     None,
                     c_loc,
                     c_unit,
                     "production",
                 )
             ]
+
             supplier_id = (
                 s_name,
                 s_prod,
                 s_cat,
                 s_loc,
                 s_unit,
                 s_type,
             )
+
+            if supplier_id not in self.reversed_acts_indices:
+                try:
+                    (
+                        s_name,
+                        s_prod,
+                        s_loc,
+                        s_cat,
+                    ) = self.find_correct_id((s_name, s_prod, s_loc, s_cat))
+
+                    supplier_id = (
+                        s_name,
+                        s_prod,
+                        s_cat,
+                        s_loc,
+                        s_unit,
+                        s_type,
+                    )
+                except TypeError:
+                    print("not found key for", supplier_id)
+
             supplier_idx = self.reversed_acts_indices[supplier_id]
 
             # Update the factor values for each scenario by multiplying with the corresponding matrix value
             for scenario, val in factor.items():
                 factor[scenario] = val * _(matrix[consumer_idx, supplier_idx])
 
         # Create a new scenario dataframe from the updated factors dictionary
```

### Comparing `unfold-1.0.7/unfold.egg-info/PKG-INFO` & `unfold-1.0.8/unfold.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unfold
-Version: 1.0.7
+Version: 1.0.8
 Summary: Unpacks LCA scenario databases.
 Home-page: https://github.com/polca/premise
 Author: Romain Sacchi <romain.sacchi@psi.ch>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
```

