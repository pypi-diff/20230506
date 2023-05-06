# Comparing `tmp/aws_lambda_mess-0.0.6.tar.gz` & `tmp/aws_lambda_mess-0.0.7.tar.gz`

## Comparing `aws_lambda_mess-0.0.6.tar` & `aws_lambda_mess-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.6/aws_lambda_mess/__about__.py
--rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.6/aws_lambda_mess/cli.py
--rw-r--r--   0        0        0     1056 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.6/aws_lambda_mess/framework/Route.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.6/aws_lambda_mess/framework/failures.py
--rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.6/aws_lambda_mess/framework/lambda_dispatcher.py
--rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.6/aws_lambda_mess/framework/server.py
--rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.6/aws_lambda_mess/framework/success.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.6/aws_lambda_mess/init_files/.aws_lambda_mess.json
--rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.6/aws_lambda_mess/init_files/.gitignore
--rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.6/aws_lambda_mess/init_files/app.py
--rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.6/aws_lambda_mess/init_files/requirements.txt
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.6/.gitignore
--rw-r--r--   0        0        0     4986 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.6/README.md
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.6/pyproject.toml
--rw-r--r--   0        0        0     5193 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.6/PKG-INFO
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.7/aws_lambda_mess/__about__.py
+-rw-r--r--   0        0        0     2250 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.7/aws_lambda_mess/cli.py
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.7/aws_lambda_mess/framework/Route.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.7/aws_lambda_mess/framework/failures.py
+-rw-r--r--   0        0        0      509 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.7/aws_lambda_mess/framework/lambda_dispatcher.py
+-rw-r--r--   0        0        0     1554 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.7/aws_lambda_mess/framework/server.py
+-rw-r--r--   0        0        0      239 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.7/aws_lambda_mess/framework/success.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.7/aws_lambda_mess/init_files/.aws_lambda_mess.json
+-rw-r--r--   0        0        0       20 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.7/aws_lambda_mess/init_files/.gitignore
+-rw-r--r--   0        0        0      816 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.7/aws_lambda_mess/init_files/app.py
+-rw-r--r--   0        0        0       15 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.7/aws_lambda_mess/init_files/requirements.txt
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.7/.gitignore
+-rw-r--r--   0        0        0     5033 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.7/README.md
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.7/pyproject.toml
+-rw-r--r--   0        0        0     5238 2020-02-02 00:00:00.000000 aws_lambda_mess-0.0.7/PKG-INFO
```

### Comparing `aws_lambda_mess-0.0.6/aws_lambda_mess/cli.py` & `aws_lambda_mess-0.0.7/aws_lambda_mess/cli.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_mess-0.0.6/aws_lambda_mess/framework/Route.py` & `aws_lambda_mess-0.0.7/aws_lambda_mess/framework/Route.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This routine replaces <variable> with a regex to extract the variable into a named group
 # somethinmg like this f"(?P<{key}>[a-zA-Z0-9]*)"
 #
 def replace_with_regex(pattern):
     match = re.findall("<([a-zA-Z0-9_]*)>", pattern)
     for key in match:
         pattern = pattern.replace(f"<{key}>", f"(?P<{key}>[a-zA-Z0-9\\-_]*)")
-    return pattern + ("?" if pattern.endswith("/") else "/?")
+    return "(/.*?)?" + pattern + ("?" if pattern.endswith("/") else "/?")
 
 
 class Route:
     def __init__(self, method_pattern, path_pattern, handler):
         self.method_pattern = method_pattern
         self.path_pattern = replace_with_regex(path_pattern)
         self.handler = handler
```

### Comparing `aws_lambda_mess-0.0.6/aws_lambda_mess/framework/server.py` & `aws_lambda_mess-0.0.7/aws_lambda_mess/framework/server.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_mess-0.0.6/aws_lambda_mess/init_files/app.py` & `aws_lambda_mess-0.0.7/aws_lambda_mess/init_files/app.py`

 * *Files identical despite different names*

### Comparing `aws_lambda_mess-0.0.6/README.md` & `aws_lambda_mess-0.0.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,16 @@
 * Does not support non json responses
 * Query variables not supported yet
 * Headers not exposed in route handlers
 * Many others
 
 Please raise issues for any enhancements or bugs. 
 
+The [FAQ](FAQ.md), always the [FAQ](FAQ.md).
+
 # Index
 1. [Workflow in a nutshell](#Workflow-in-a-nutshell)
 2. [Installing](#Installing)
 3. [Create and run a new project](#Create-and-run-a-new-project)
 4. [Build the aws lambda zip](#Build-the-aws-lambda-zip)
 5. [Install the zip as a lambda](#Install-the-zip-as-a-lambda)
 6. [Configure the api gateway](#Configure-the-api-gateway)
@@ -136,15 +138,15 @@
 ## Test /
 ```json
 {
   "body": "{}",
   "resource": "/{proxy+}",
   "path": "/",
   "httpMethod": "GET",
-  "isBase64Encoded": true,
+  "isBase64Encoded": true
 }
 ```
 Returns 
 ```json
 {
   "isBase64Encoded": false,
   "statusCode": 200,
```

### Comparing `aws_lambda_mess-0.0.6/pyproject.toml` & `aws_lambda_mess-0.0.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aws_lambda_mess-0.0.6/PKG-INFO` & `aws_lambda_mess-0.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aws_lambda_mess
-Version: 0.0.6
+Version: 0.0.7
 Project-URL: Documentation, https://github.com/johanjordaan/aws_lambda_mess#readme
 Project-URL: Issues, https://github.com/johanjordaan/aws_lambda_mess/issues
 Project-URL: Source, https://github.com/johanjordaan/aws_lambda_mess
 Author-email: johan jordaan <djjordaan@gmail.com>
 License-Expression: MIT
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
@@ -23,14 +23,16 @@
 * Does not support non json responses
 * Query variables not supported yet
 * Headers not exposed in route handlers
 * Many others
 
 Please raise issues for any enhancements or bugs. 
 
+The [FAQ](FAQ.md), always the [FAQ](FAQ.md).
+
 # Index
 1. [Workflow in a nutshell](#Workflow-in-a-nutshell)
 2. [Installing](#Installing)
 3. [Create and run a new project](#Create-and-run-a-new-project)
 4. [Build the aws lambda zip](#Build-the-aws-lambda-zip)
 5. [Install the zip as a lambda](#Install-the-zip-as-a-lambda)
 6. [Configure the api gateway](#Configure-the-api-gateway)
@@ -147,15 +149,15 @@
 ## Test /
 ```json
 {
   "body": "{}",
   "resource": "/{proxy+}",
   "path": "/",
   "httpMethod": "GET",
-  "isBase64Encoded": true,
+  "isBase64Encoded": true
 }
 ```
 Returns 
 ```json
 {
   "isBase64Encoded": false,
   "statusCode": 200,
```

