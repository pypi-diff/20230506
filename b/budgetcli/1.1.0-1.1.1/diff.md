# Comparing `tmp/budgetcli-1.1.0.tar.gz` & `tmp/budgetcli-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "budgetcli-1.1.0.tar", last modified: Fri May  5 21:50:23 2023, max compression
+gzip compressed data, was "budgetcli-1.1.1.tar", last modified: Sat May  6 19:35:07 2023, max compression
```

## Comparing `budgetcli-1.1.0.tar` & `budgetcli-1.1.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:50:23.655035 budgetcli-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-05 21:49:55.000000 budgetcli-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-05-05 21:50:23.655035 budgetcli-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-05-05 21:49:55.000000 budgetcli-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-05 21:49:55.000000 budgetcli-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-05 21:50:23.655035 budgetcli-1.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:50:23.651034 budgetcli-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:50:23.655035 budgetcli-1.1.0/src/budgetcli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 21:49:55.000000 budgetcli-1.1.0/src/budgetcli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-05-05 21:49:55.000000 budgetcli-1.1.0/src/budgetcli/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:50:23.655035 budgetcli-1.1.0/src/budgetcli/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 21:49:55.000000 budgetcli-1.1.0/src/budgetcli/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-05-05 21:49:55.000000 budgetcli-1.1.0/src/budgetcli/cli/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-05 21:49:55.000000 budgetcli-1.1.0/src/budgetcli/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-05-05 21:49:55.000000 budgetcli-1.1.0/src/budgetcli/cli/display.py
--rw-r--r--   0 runner    (1001) docker     (123)     3910 2023-05-05 21:49:55.000000 budgetcli-1.1.0/src/budgetcli/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)    11705 2023-05-05 21:49:55.000000 budgetcli-1.1.0/src/budgetcli/data_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-05 21:49:55.000000 budgetcli-1.1.0/src/budgetcli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-05-05 21:49:55.000000 budgetcli-1.1.0/src/budgetcli/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-05 21:49:55.000000 budgetcli-1.1.0/src/budgetcli/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:50:23.655035 budgetcli-1.1.0/src/budgetcli/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 21:49:55.000000 budgetcli-1.1.0/src/budgetcli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-05 21:49:55.000000 budgetcli-1.1.0/src/budgetcli/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-05 21:49:55.000000 budgetcli-1.1.0/src/budgetcli/utils/dates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-05 21:49:55.000000 budgetcli-1.1.0/src/budgetcli/utils/display.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:50:23.655035 budgetcli-1.1.0/src/budgetcli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-05-05 21:50:23.000000 budgetcli-1.1.0/src/budgetcli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-05 21:50:23.000000 budgetcli-1.1.0/src/budgetcli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 21:50:23.000000 budgetcli-1.1.0/src/budgetcli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-05 21:50:23.000000 budgetcli-1.1.0/src/budgetcli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-05 21:50:23.000000 budgetcli-1.1.0/src/budgetcli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-05 21:50:23.000000 budgetcli-1.1.0/src/budgetcli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 19:35:07.095886 budgetcli-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-06 19:34:41.000000 budgetcli-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-05-06 19:35:07.095886 budgetcli-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-05-06 19:34:41.000000 budgetcli-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-06 19:34:41.000000 budgetcli-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-06 19:35:07.095886 budgetcli-1.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 19:35:07.091886 budgetcli-1.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 19:35:07.091886 budgetcli-1.1.1/src/budgetcli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 19:34:41.000000 budgetcli-1.1.1/src/budgetcli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-05-06 19:34:41.000000 budgetcli-1.1.1/src/budgetcli/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 19:35:07.095886 budgetcli-1.1.1/src/budgetcli/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 19:34:41.000000 budgetcli-1.1.1/src/budgetcli/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-05-06 19:34:41.000000 budgetcli-1.1.1/src/budgetcli/cli/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1325 2023-05-06 19:34:41.000000 budgetcli-1.1.1/src/budgetcli/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1754 2023-05-06 19:34:41.000000 budgetcli-1.1.1/src/budgetcli/cli/display.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-05-06 19:34:41.000000 budgetcli-1.1.1/src/budgetcli/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11907 2023-05-06 19:34:41.000000 budgetcli-1.1.1/src/budgetcli/data_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-06 19:34:41.000000 budgetcli-1.1.1/src/budgetcli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-05-06 19:34:41.000000 budgetcli-1.1.1/src/budgetcli/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-05-06 19:34:41.000000 budgetcli-1.1.1/src/budgetcli/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 19:35:07.095886 budgetcli-1.1.1/src/budgetcli/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-06 19:34:41.000000 budgetcli-1.1.1/src/budgetcli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-06 19:34:41.000000 budgetcli-1.1.1/src/budgetcli/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      681 2023-05-06 19:34:41.000000 budgetcli-1.1.1/src/budgetcli/utils/dates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-05-06 19:34:41.000000 budgetcli-1.1.1/src/budgetcli/utils/display.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 19:35:07.095886 budgetcli-1.1.1/src/budgetcli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-05-06 19:35:07.000000 budgetcli-1.1.1/src/budgetcli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-06 19:35:07.000000 budgetcli-1.1.1/src/budgetcli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 19:35:07.000000 budgetcli-1.1.1/src/budgetcli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-06 19:35:07.000000 budgetcli-1.1.1/src/budgetcli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-06 19:35:07.000000 budgetcli-1.1.1/src/budgetcli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-06 19:35:07.000000 budgetcli-1.1.1/src/budgetcli.egg-info/top_level.txt
```

### Comparing `budgetcli-1.1.0/LICENSE` & `budgetcli-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `budgetcli-1.1.0/PKG-INFO` & `budgetcli-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: budgetcli
-Version: 1.1.0
+Version: 1.1.1
 Summary: A simple async budgeting app to manage expenses and budgets in google spreadsheets
 Author: Code Rustle
 Author-email: coderustle@gmail.com
 License: MIT
 Classifier: Topic :: Utilities
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `budgetcli-1.1.0/README.md` & `budgetcli-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `budgetcli-1.1.0/pyproject.toml` & `budgetcli-1.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `budgetcli-1.1.0/setup.cfg` & `budgetcli-1.1.1/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = budgetcli
-version = 1.1.0
+version = 1.1.1
 author = Code Rustle
 author_email = coderustle@gmail.com
 description = A simple async budgeting app to manage expenses and budgets in google spreadsheets
 long_description = file: README.md
 long_description_content_type = text/markdown
 license = MIT
 license_file = LICENSE
```

### Comparing `budgetcli-1.1.0/src/budgetcli/auth.py` & `budgetcli-1.1.1/src/budgetcli/auth.py`

 * *Files identical despite different names*

### Comparing `budgetcli-1.1.0/src/budgetcli/cli/add.py` & `budgetcli-1.1.1/src/budgetcli/cli/add.py`

 * *Files identical despite different names*

### Comparing `budgetcli-1.1.0/src/budgetcli/cli/config.py` & `budgetcli-1.1.1/src/budgetcli/cli/config.py`

 * *Files identical despite different names*

### Comparing `budgetcli-1.1.0/src/budgetcli/cli/display.py` & `budgetcli-1.1.1/src/budgetcli/cli/display.py`

 * *Files 15% similar despite different names*

```diff
@@ -24,25 +24,26 @@
 
 RowsOption = typer.Option(
     100,
     min=1,
     max=100,
     help="Number of transaction rows to display",
 )
+NameOption = typer.Option("", help="The name of category")
 MonthOption = typer.Option(
     "",
     help="The name of the month eg: April or Apr",
     callback=validate_month,
 )
 
 
 @app.command()
-def categories(rows: int = RowsOption):
+def categories(rows: int = RowsOption, name: str = NameOption):
     """List all categories from spreadsheet"""
-    command = ListCategoryCommand(rows=rows)
+    command = ListCategoryCommand(rows=rows, name=name)
     command.execute()
 
 
 @app.command()
 def transactions(rows: int = RowsOption, month: str = MonthOption):
     """List all transactions from spreadsheet"""
     month_number = dates.get_month_number(month)
```

### Comparing `budgetcli-1.1.0/src/budgetcli/commands.py` & `budgetcli-1.1.1/src/budgetcli/commands.py`

 * *Files 5% similar despite different names*

```diff
@@ -64,21 +64,19 @@
         self.manager = ManagerFactory.create_manager_for("transactions")
 
     def execute(self):
         table = get_transaction_table()
         if self.manager is not None:
             with task_progress(description="Processing.."):
                 if self.month:
-                    transactions = asyncio.run(
-                        self.manager.get_records_for_month(self.month)
-                    )
+                    get = self.manager.get_records_for_month(self.month)
+                    transactions = asyncio.run(get)
                 else:
-                    transactions = asyncio.run(
-                        self.manager.get_records(self.rows)
-                    )
+                    get = self.manager.get_records(self.rows)
+                    transactions = asyncio.run(get)
                 for row in transactions:
                     income = f"{CURRENCY} {row[3]}"
                     outcome = f"{CURRENCY} {row[4]}"
                     table.add_row(row[0], row[1], row[2], income, outcome)
         print(table)
 
 
@@ -94,24 +92,27 @@
                 asyncio.run(self.manager.append(row))
                 print(":heavy_check_mark: Category was added successfully")
         except AttributeError:
             print("Init factory manager error")
 
 
 class ListCategoryCommand(Command):
-    def __init__(self, rows: int):
+    def __init__(self, rows: int, name: str):
         self.rows = rows
+        self.name = name
         self.manager = ManagerFactory.create_manager_for("categories")
 
     def execute(self) -> None:
         table = get_category_table()
         try:
             with task_progress(description="Processing"):
-                if self.rows:
-                    categories = asyncio.run(
-                        self.manager.get_records(rows=self.rows)
-                    )
-                    for row in categories:
-                        table.add_row(row[0])
+                if self.name:
+                    get = self.manager.get_records_by_name(name=self.name)
+                    categories = asyncio.run(get)
+                else:
+                    get = self.manager.get_records(rows=self.rows)
+                    categories = asyncio.run(get)
+                for row in categories:
+                    table.add_row(row[0])
         except AttributeError:
             print("Init factory manager error")
         print(table)
```

### Comparing `budgetcli-1.1.0/src/budgetcli/data_manager.py` & `budgetcli-1.1.1/src/budgetcli/data_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -121,17 +121,18 @@
         params = "fields=sheets.properties"
         url = f"{self.base_url}?{params}"
         response = await self.session.get(url)
         try:
             response.raise_for_status()
             data = response.json()
             sheets = data.get("sheets")
-            for sheet in sheets:
-                if sheet["properties"]["title"] == title:
-                    return sheet["properties"]
+            if sheets:
+                for sheet in sheets:
+                    if sheet["properties"]["title"] == title:
+                        return sheet["properties"]
         except httpx.HTTPStatusError as err:
             req_url = err.request.url
             status = err.response.status_code
             pprint(f"Error calling {req_url}, http status: {status}")
         return None
 
     async def _create_sheet(self, title: str) -> dict[str, str] | None:
@@ -165,14 +166,28 @@
                 if properties:
                     return properties
         except asyncio.TimeoutError:
             pass
         return {}
 
     @staticmethod
+    def _process_row(row: dict[str, list]) -> list[str]:
+        """Helper function to process transaction rows"""
+        records = []
+        for cel in row.get("c", []):
+            if cel and "Date(" in str(cel.get("v")):
+                date = cel.get("f")
+                records.append(date)
+            elif cel:
+                records.append(cel.get("v"))
+            else:
+                records.append("")
+        return records
+
+    @staticmethod
     def get_auth_headers() -> dict:
         """Get the authentication headers from Google credentials"""
         headers: dict[str, str] = {}
         credentials: Credentials | None = load_user_token()
         if credentials:
             credentials.apply(headers=headers)
         return headers
@@ -219,34 +234,22 @@
         result: list[list[str]] = await self._list(a1=transaction_range)
         return result if result else []
 
     async def get_records_for_month(self, month: int) -> list[list[str]]:
         """Query the transactions for current month"""
         month -= 1  # month query starts from 0 to 11
         query = f"select A,B,C,D,E where month(A)={month}"
-
-        sheet_index = get_config("transactions_sheet_index")
-        index = int(sheet_index) if sheet_index else 1
-        rows = await self._query(query, index)
-        transactions = [self._process_row(row) for row in rows] if rows else []
-        return transactions
-
-    @staticmethod
-    def _process_row(row: dict[str, list]) -> list[str]:
-        """Helper function to process transaction rows"""
-        transaction = []
-        for cel in row.get("c", []):
-            if cel and "Date(" in str(cel.get("v")):
-                date = cel.get("f")
-                transaction.append(date)
-            elif cel:
-                transaction.append(cel.get("v"))
-            else:
-                transaction.append("")
-        return transaction
+        index = get_config("transactions_sheet_index")
+        if index:
+            rows = await self._query(query, int(index))
+            transactions = [self._process_row(i) for i in rows] if rows else []
+            return transactions
+        else:
+            pprint(":warning: Transactions sheet index is missing")
+        return []
 
 
 class CategoryDataManager(AbstractDataManager):
     SHEET_NAME = "CATEGORIES"
     FIRST_COLUMN = "A"
     LAST_COLUMN = "A"
     ROW_START = 2
@@ -279,24 +282,26 @@
 
     async def get_records(self, rows: int = 100):
         """Return all categories"""
         category_range = f"{self.CATEGORY_RANGE}{rows + 1}"
         result: list[list[str]] = await self._list(a1=category_range)
         return result if result else []
 
-    async def get_records_by_name(self, name: str) -> None:
+    async def get_records_by_name(self, name: str) -> list[list[str]]:
         """Return a category by a given name"""
         name = name.lower()
         query = f"select A where A='{name}'"
         index = get_config("categories_sheet_index")
-        print("index is", index)
         if index:
             rows = await self._query(query, int(index))
-            pprint(rows, expand_all=True)
-            return rows
+            categories = [self._process_row(i) for i in rows] if rows else []
+            return categories
+        else:
+            pprint(":warning: Categories sheet index is missing")
+        return []
 
 
 class ManagerFactory:
     @staticmethod
     def create_manager_for(manager_name: str) -> T | None:
         match manager_name:
             case "transactions":
```

### Comparing `budgetcli-1.1.0/src/budgetcli/main.py` & `budgetcli-1.1.1/src/budgetcli/main.py`

 * *Files identical despite different names*

### Comparing `budgetcli-1.1.0/src/budgetcli/models.py` & `budgetcli-1.1.1/src/budgetcli/models.py`

 * *Files identical despite different names*

### Comparing `budgetcli-1.1.0/src/budgetcli/settings.py` & `budgetcli-1.1.1/src/budgetcli/settings.py`

 * *Files identical despite different names*

### Comparing `budgetcli-1.1.0/src/budgetcli/utils/config.py` & `budgetcli-1.1.1/src/budgetcli/utils/config.py`

 * *Files identical despite different names*

### Comparing `budgetcli-1.1.0/src/budgetcli/utils/dates.py` & `budgetcli-1.1.1/src/budgetcli/utils/dates.py`

 * *Files identical despite different names*

### Comparing `budgetcli-1.1.0/src/budgetcli/utils/display.py` & `budgetcli-1.1.1/src/budgetcli/utils/display.py`

 * *Files identical despite different names*

### Comparing `budgetcli-1.1.0/src/budgetcli.egg-info/PKG-INFO` & `budgetcli-1.1.1/src/budgetcli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: budgetcli
-Version: 1.1.0
+Version: 1.1.1
 Summary: A simple async budgeting app to manage expenses and budgets in google spreadsheets
 Author: Code Rustle
 Author-email: coderustle@gmail.com
 License: MIT
 Classifier: Topic :: Utilities
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `budgetcli-1.1.0/src/budgetcli.egg-info/SOURCES.txt` & `budgetcli-1.1.1/src/budgetcli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

