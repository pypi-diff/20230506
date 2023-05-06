# Comparing `tmp/apasswordmanager-0.1.0.tar.gz` & `tmp/apasswordmanager-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apasswordmanager-0.1.0.tar", max compression
+gzip compressed data, was "apasswordmanager-0.1.1.tar", max compression
```

## Comparing `apasswordmanager-0.1.0.tar` & `apasswordmanager-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0    26526 2023-05-05 17:01:27.677948 apasswordmanager-0.1.0/LICENSE
--rw-r--r--   0        0        0     1301 2023-05-06 08:05:40.315764 apasswordmanager-0.1.0/README.md
--rw-r--r--   0        0        0      554 2023-05-06 10:14:05.191102 apasswordmanager-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-06 01:06:36.652640 apasswordmanager-0.1.0/src/apasswordmanager/__init__.py
--rw-r--r--   0        0        0     2992 2023-05-06 10:42:35.350634 apasswordmanager-0.1.0/src/apasswordmanager/main.py
--rw-r--r--   0        0        0        0 2023-05-06 01:06:28.612643 apasswordmanager-0.1.0/src/apasswordmanager/modules/__init__.py
--rw-r--r--   0        0        0      682 2023-05-05 23:32:44.874180 apasswordmanager-0.1.0/src/apasswordmanager/modules/config.py
--rw-r--r--   0        0        0    13453 2023-05-06 07:32:23.716310 apasswordmanager-0.1.0/src/apasswordmanager/modules/encryption.py
--rw-r--r--   0        0        0      324 2023-05-05 21:26:24.146253 apasswordmanager-0.1.0/src/apasswordmanager/modules/exceptions.py
--rw-r--r--   0        0        0    13009 2023-05-06 07:33:25.356293 apasswordmanager-0.1.0/src/apasswordmanager/modules/menu.py
--rw-r--r--   0        0        0     1956 1970-01-01 00:00:00.000000 apasswordmanager-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    26526 2023-05-05 17:01:27.677948 apasswordmanager-0.1.1/LICENSE
+-rw-r--r--   0        0        0     1381 2023-05-06 11:20:53.060006 apasswordmanager-0.1.1/README.md
+-rw-r--r--   0        0        0      554 2023-05-06 12:18:24.069061 apasswordmanager-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-06 01:06:36.652640 apasswordmanager-0.1.1/src/apasswordmanager/__init__.py
+-rw-r--r--   0        0        0     3051 2023-05-06 12:17:47.059071 apasswordmanager-0.1.1/src/apasswordmanager/main.py
+-rw-r--r--   0        0        0        0 2023-05-06 01:06:28.612643 apasswordmanager-0.1.1/src/apasswordmanager/modules/__init__.py
+-rw-r--r--   0        0        0      837 2023-05-06 12:14:55.969118 apasswordmanager-0.1.1/src/apasswordmanager/modules/config.py
+-rw-r--r--   0        0        0    13453 2023-05-06 07:32:23.716310 apasswordmanager-0.1.1/src/apasswordmanager/modules/encryption.py
+-rw-r--r--   0        0        0      324 2023-05-05 21:26:24.146253 apasswordmanager-0.1.1/src/apasswordmanager/modules/exceptions.py
+-rw-r--r--   0        0        0    13009 2023-05-06 07:33:25.356293 apasswordmanager-0.1.1/src/apasswordmanager/modules/menu.py
+-rw-r--r--   0        0        0     2036 1970-01-01 00:00:00.000000 apasswordmanager-0.1.1/PKG-INFO
```

### Comparing `apasswordmanager-0.1.0/LICENSE` & `apasswordmanager-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `apasswordmanager-0.1.0/README.md` & `apasswordmanager-0.1.1/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -6,16 +6,21 @@
 - Local database, each email and passwords are encrypted with a unique code using AES encryption
 - Master key is hashed
 - Possibility to create an unlimited number of managers
 - Clipboard detected
 - Password suggestions for password generator
 
 ## Usage
+
+### Locally
 ![](./assets/How-To-Use.svg)
 
+### Package
+![](./assets/How-To-Use-Package.svg)
+
 ## Installation and setup
 APassword Manager 0.1.x can only be run locally.
 
 ### Cloning the project
 ``` bash
 git clone https://github.com/AgentPython/AdvancedPasswordManager.git
 ```
@@ -38,21 +43,21 @@
 #### poetry
 ``` bash
 poetry run app
 ```
 
 #### python
 ``` bash
-python -m app.main
+python -m src.apasswordmanager.main
 ```
 
 ## Upcoming
 *Release date : May 13, 2023 (in a week)*
 <br>
-APasswordManager 0.2.x requires `sqlcipher` to be installed on your machine.
+APasswordManager 1.0.x requires `sqlcipher` to be installed on your machine.
 APasswordManager is packaged so you can use it in your project or in your terminal.
 Which means can be installed with `pip install apasswordmanager`
 
 ### Features
 - External database with SQLite + SQLCipher
 - Adding unique salt for every passwords, emails, and notes.
 - Import or export in JSON
```

### Comparing `apasswordmanager-0.1.0/pyproject.toml` & `apasswordmanager-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "apasswordmanager"
-version = "0.1.0"
+version = "0.1.1"
 description = ""
 authors = ["jo-project <jo.project.0911@gmail.com>"]
 readme = "README.md"
 license = "LGPL-2.1-or-later"
 packages = [{include = "apasswordmanager", from = "src"}]
 
 [tool.poetry.dependencies]
```

### Comparing `apasswordmanager-0.1.0/src/apasswordmanager/main.py` & `apasswordmanager-0.1.1/src/apasswordmanager/main.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,48 +6,50 @@
 from hashlib import sha256
 from sys import exit
 from pyperclip import copy 
 
 from .modules.exceptions import *
 from .modules.encryption import DataManipulation
 from .modules.menu import Manager
+from .modules.config import config_path_default, password_path_default, dir_
 
 from rich.console import Console
 
 console = Console()
 
 def exit_program():
     print("\n")
     print(colored("❯", "red"))
     exit()
 
+
 obj = DataManipulation()
 def main():
     try:
 
-        if path.isfile('db/masterpassword.json'):
-            with open('db/masterpassword.json') as jsondata:
+        if path.isfile(config_path_default):
+            with open(config_path_default) as jsondata:
                 jfile = load(jsondata)
 
             stored_master_password = jfile['Master']
             master_password = Prompt.ask("Enter master password", password=True)
             if sha256(master_password.encode('utf-8')).hexdigest() == stored_master_password:
                 print(colored(f"{obj.checkmark_} Thank you!", "green"))
-                menu = Manager(obj, "db/passwords.json", "db/masterpassword.json", master_password)
+                menu = Manager(obj, password_path_default, config_path_default, master_password)
                 try:
                     menu.begin()
                 except UserExits:
                     exit_program()
                 except PasswordFileDoesNotExist:
                     print(colored(f"{obj.x_mark} DB not found. Try adding a password {obj.x_mark}", "red"))
             else:
                 print(colored(f"{obj.x_mark} Master password is incorrect, please try again!", "red"))
         else:
             try:
-                mkdir('db/')
+                mkdir(dir_)
             except FileExistsError:
                 pass
     
             master_password = Prompt.ask("Enter master password", password=True)
             master_password_verification = Prompt.ask("Verify your master password", password=True)
 
             if master_password == master_password_verification:
@@ -59,15 +61,15 @@
 
                 spinner = Halo(text=colored('Initializing base...', 'green'), spinner=obj.dots_, color="green")
                 spinner.start()
                 hash_master = sha256(master_password.encode('utf-8')).hexdigest()
                 jfile = {
                     "Master": hash_master
                 }
-                with open('db/masterpassword.json', 'w') as jsondata:
+                with open(config_path_default, 'w') as jsondata:
                     dump(jfile, jsondata, sort_keys=True, indent=4)
                 spinner.stop()
                 print(colored(f"{obj.checkmark_} Thank you! please restart the program", 'green'))
             else:
                 print(colored(f"{obj.x_mark} Password do not match, please try again!", "red"))
     except KeyboardInterrupt:
         exit_program()
```

### Comparing `apasswordmanager-0.1.0/src/apasswordmanager/modules/encryption.py` & `apasswordmanager-0.1.1/src/apasswordmanager/modules/encryption.py`

 * *Files identical despite different names*

### Comparing `apasswordmanager-0.1.0/src/apasswordmanager/modules/menu.py` & `apasswordmanager-0.1.1/src/apasswordmanager/modules/menu.py`

 * *Files identical despite different names*

### Comparing `apasswordmanager-0.1.0/PKG-INFO` & `apasswordmanager-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apasswordmanager
-Version: 0.1.0
+Version: 0.1.1
 Summary: 
 License: LGPL-2.1-or-later
 Author: jo-project
 Author-email: jo.project.0911@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved
 Classifier: Programming Language :: Python :: 3
@@ -26,16 +26,21 @@
 - Local database, each email and passwords are encrypted with a unique code using AES encryption
 - Master key is hashed
 - Possibility to create an unlimited number of managers
 - Clipboard detected
 - Password suggestions for password generator
 
 ## Usage
+
+### Locally
 ![](./assets/How-To-Use.svg)
 
+### Package
+![](./assets/How-To-Use-Package.svg)
+
 ## Installation and setup
 APassword Manager 0.1.x can only be run locally.
 
 ### Cloning the project
 ``` bash
 git clone https://github.com/AgentPython/AdvancedPasswordManager.git
 ```
@@ -58,21 +63,21 @@
 #### poetry
 ``` bash
 poetry run app
 ```
 
 #### python
 ``` bash
-python -m app.main
+python -m src.apasswordmanager.main
 ```
 
 ## Upcoming
 *Release date : May 13, 2023 (in a week)*
 <br>
-APasswordManager 0.2.x requires `sqlcipher` to be installed on your machine.
+APasswordManager 1.0.x requires `sqlcipher` to be installed on your machine.
 APasswordManager is packaged so you can use it in your project or in your terminal.
 Which means can be installed with `pip install apasswordmanager`
 
 ### Features
 - External database with SQLite + SQLCipher
 - Adding unique salt for every passwords, emails, and notes.
 - Import or export in JSON
```

