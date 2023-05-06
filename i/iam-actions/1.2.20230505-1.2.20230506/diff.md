# Comparing `tmp/iam_actions-1.2.20230505.tar.gz` & `tmp/iam_actions-1.2.20230506.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20230505.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20230506.tar", max compression
```

## Comparing `iam_actions-1.2.20230505.tar` & `iam_actions-1.2.20230506.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2023-05-05 02:23:24.642775 iam_actions-1.2.20230505/LICENSE
--rw-r--r--   0        0        0     2302 2023-05-05 02:23:24.642775 iam_actions-1.2.20230505/README.md
--rw-r--r--   0        0        0      228 2023-05-05 02:23:24.642775 iam_actions-1.2.20230505/iam_actions/__init__.py
--rw-r--r--   0        0        0  4244693 2023-05-05 02:25:19.316170 iam_actions-1.2.20230505/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2023-05-05 02:23:24.642775 iam_actions-1.2.20230505/iam_actions/data.py
--rw-r--r--   0        0        0       80 2023-05-05 02:23:24.642775 iam_actions-1.2.20230505/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2023-05-05 02:23:24.642775 iam_actions-1.2.20230505/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2023-05-05 02:23:24.642775 iam_actions-1.2.20230505/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2023-05-05 02:23:24.642775 iam_actions-1.2.20230505/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2023-05-05 02:23:24.642775 iam_actions-1.2.20230505/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2023-05-05 02:23:24.642775 iam_actions-1.2.20230505/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2023-05-05 02:23:24.642775 iam_actions-1.2.20230505/iam_actions/generate/services.py
--rw-r--r--   0        0        0   545743 2023-05-05 02:25:19.316170 iam_actions-1.2.20230505/iam_actions/policies.json
--rw-r--r--   0        0        0   193571 2023-05-05 02:25:19.316170 iam_actions-1.2.20230505/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   529274 2023-05-05 02:25:19.316170 iam_actions-1.2.20230505/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2023-05-05 02:25:20.072179 iam_actions-1.2.20230505/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230505/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230505/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-06 02:21:51.531170 iam_actions-1.2.20230506/LICENSE
+-rw-r--r--   0        0        0     2302 2023-05-06 02:21:51.531170 iam_actions-1.2.20230506/README.md
+-rw-r--r--   0        0        0      228 2023-05-06 02:21:51.531170 iam_actions-1.2.20230506/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4245819 2023-05-06 02:23:45.447431 iam_actions-1.2.20230506/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2023-05-06 02:21:51.531170 iam_actions-1.2.20230506/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2023-05-06 02:21:51.531170 iam_actions-1.2.20230506/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2023-05-06 02:21:51.531170 iam_actions-1.2.20230506/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2023-05-06 02:21:51.531170 iam_actions-1.2.20230506/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2023-05-06 02:21:51.531170 iam_actions-1.2.20230506/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2023-05-06 02:21:51.531170 iam_actions-1.2.20230506/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2023-05-06 02:21:51.531170 iam_actions-1.2.20230506/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2023-05-06 02:21:51.531170 iam_actions-1.2.20230506/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   545884 2023-05-06 02:23:45.447431 iam_actions-1.2.20230506/iam_actions/policies.json
+-rw-r--r--   0        0        0   193571 2023-05-06 02:23:45.447431 iam_actions-1.2.20230506/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   529410 2023-05-06 02:23:45.447431 iam_actions-1.2.20230506/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2023-05-06 02:23:46.267462 iam_actions-1.2.20230506/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20230506/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20230506/PKG-INFO
```

### Comparing `iam_actions-1.2.20230505/LICENSE` & `iam_actions-1.2.20230506/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230505/README.md` & `iam_actions-1.2.20230506/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230505/iam_actions/actions.json` & `iam_actions-1.2.20230506/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999339122441429%*

 * *Differences: {"'appsync'": "{'CreateGraphqlApi': {'condition_keys': {insert: [(0, 'appsync:Visibility')]}}}",*

 * * "'elasticfilesystem'": "{'TagResource': {'condition_keys': {insert: [(2, "*

 * *                        "'elasticfilesystem:CreateAction')]}}}",*

 * * "'quicksight'": "{'UpdateVPCConnection': OrderedDict([('access_level', 'Undocumented'), "*

 * *                 "('action', 'UpdateVPCConnection'), ('condition_keys', []), ('description', 'Not "*

 * *                 "Documented by AWS'), ('orphan', False), ('resources', [])]), "*

 * *   […]*

```diff
@@ -6908,14 +6908,15 @@
             "orphan": false,
             "resources": []
         },
         "CreateGraphqlApi": {
             "access_level": "Write",
             "action": "CreateGraphqlApi",
             "condition_keys": [
+                "appsync:Visibility",
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
             ],
             "description": "Grants permission to create a GraphQL API, which is the top level AppSync resource",
             "orphan": false,
             "resources": []
         },
@@ -55311,15 +55312,16 @@
             ]
         },
         "TagResource": {
             "access_level": "Tagging",
             "action": "TagResource",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
-                "aws:TagKeys"
+                "aws:TagKeys",
+                "elasticfilesystem:CreateAction"
             ],
             "description": "Grants permission to create or overwrite tags associated with the specified Amazon EFS resource",
             "orphan": false,
             "resources": [
                 "access-point",
                 "file-system"
             ]
@@ -109011,14 +109013,22 @@
             "condition_keys": [],
             "description": "Grants permission to describe a QuickSight user given the user name",
             "orphan": false,
             "resources": [
                 "user"
             ]
         },
+        "DescribeVPCConnection": {
+            "access_level": "Undocumented",
+            "action": "DescribeVPCConnection",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "GenerateEmbedUrlForAnonymousUser": {
             "access_level": "Write",
             "action": "GenerateEmbedUrlForAnonymousUser",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys",
                 "quicksight:AllowedEmbeddingDomains"
@@ -109324,14 +109334,22 @@
             "condition_keys": [],
             "description": "Grants permission to list all of the QuickSight users belonging to this account",
             "orphan": false,
             "resources": [
                 "user"
             ]
         },
+        "ListVPCConnections": {
+            "access_level": "Undocumented",
+            "action": "ListVPCConnections",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "PassDataSet": {
             "access_level": "Read",
             "action": "PassDataSet",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
             ],
@@ -109809,14 +109827,22 @@
             "action": "UpdateUser",
             "condition_keys": [],
             "description": "Grants permission to update an Amazon QuickSight user",
             "orphan": false,
             "resources": [
                 "user"
             ]
+        },
+        "UpdateVPCConnection": {
+            "access_level": "Undocumented",
+            "action": "UpdateVPCConnection",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
         }
     },
     "ram": {
         "AcceptResourceShareInvitation": {
             "access_level": "Undocumented",
             "action": "AcceptResourceShareInvitation",
             "condition_keys": [],
@@ -128140,14 +128166,22 @@
             "condition_keys": [],
             "description": "Grants permission to enable standards in Security Hub",
             "orphan": false,
             "resources": [
                 "hub"
             ]
         },
+        "BatchGetControlEvaluations": {
+            "access_level": "Undocumented",
+            "action": "BatchGetControlEvaluations",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "BatchGetSecurityControls": {
             "access_level": "Read",
             "action": "BatchGetSecurityControls",
             "condition_keys": [],
             "description": "Grants permission to get details about specific security controls identified by ID or ARN",
             "orphan": false,
             "resources": []
@@ -128489,14 +128523,22 @@
             "condition_keys": [],
             "description": "Grants permission to retrieve details for a finding aggregator, which configures finding aggregation across Regions",
             "orphan": false,
             "resources": [
                 "finding-aggregator"
             ]
         },
+        "GetFindingHistory": {
+            "access_level": "Undocumented",
+            "action": "GetFindingHistory",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "GetFindings": {
             "access_level": "Read",
             "action": "GetFindings",
             "condition_keys": [],
             "description": "Grants permission to retrieve a list of findings from Security Hub",
             "orphan": false,
             "resources": [
```

### Comparing `iam_actions-1.2.20230505/iam_actions/generate/action_map.py` & `iam_actions-1.2.20230506/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230505/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20230506/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230505/iam_actions/generate/generate.py` & `iam_actions-1.2.20230506/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230505/iam_actions/generate/notifier.py` & `iam_actions-1.2.20230506/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230505/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20230506/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230505/iam_actions/generate/services.py` & `iam_actions-1.2.20230506/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230505/iam_actions/policies.json` & `iam_actions-1.2.20230506/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999994816424044%*

 * *Differences: {"'serviceMap'": "{'Amazon QuickSight': {'Actions': {insert: [(80, 'DescribeVPCConnection'), (112, "*

 * *                 "'ListVPCConnections'), (159, 'UpdateVPCConnection')]}}, 'AWS Security Hub': "*

 * *                 "{'Actions': {insert: [(4, 'BatchGetControlEvaluations'), (40, "*

 * *                 "'GetFindingHistory')]}}}"}*

```diff
@@ -7676,14 +7676,15 @@
             "ARNFormat": "arn:aws:securityhub:${Region}:${Account}:.+",
             "ARNRegex": "^arn:aws:securityhub:.+",
             "Actions": [
                 "AcceptAdministratorInvitation",
                 "AcceptInvitation",
                 "BatchDisableStandards",
                 "BatchEnableStandards",
+                "BatchGetControlEvaluations",
                 "BatchGetSecurityControls",
                 "BatchGetStandardsControlAssociations",
                 "BatchImportFindings",
                 "BatchUpdateFindings",
                 "BatchUpdateStandardsControlAssociations",
                 "CreateActionTarget",
                 "CreateFindingAggregator",
@@ -7711,14 +7712,15 @@
                 "EnableOrganizationAdminAccount",
                 "EnableSecurityHub",
                 "GetAdhocInsightResults",
                 "GetAdministratorAccount",
                 "GetControlFindingSummary",
                 "GetEnabledStandards",
                 "GetFindingAggregator",
+                "GetFindingHistory",
                 "GetFindings",
                 "GetFreeTrialEndDate",
                 "GetFreeTrialUsage",
                 "GetInsightFindingTrend",
                 "GetInsightResults",
                 "GetInsights",
                 "GetInvitationsCount",
@@ -16634,14 +16636,15 @@
                 "DescribeTemplate",
                 "DescribeTemplateAlias",
                 "DescribeTemplatePermissions",
                 "DescribeTheme",
                 "DescribeThemeAlias",
                 "DescribeThemePermissions",
                 "DescribeUser",
+                "DescribeVPCConnection",
                 "GenerateEmbedUrlForAnonymousUser",
                 "GenerateEmbedUrlForRegisteredUser",
                 "GetAnonymousUserEmbedUrl",
                 "GetAuthCode",
                 "GetDashboardEmbedUrl",
                 "GetGroupMapping",
                 "GetSessionEmbedUrl",
@@ -16665,14 +16668,15 @@
                 "ListTemplateVersions",
                 "ListTemplates",
                 "ListThemeAliases",
                 "ListThemeVersions",
                 "ListThemes",
                 "ListUserGroups",
                 "ListUsers",
+                "ListVPCConnections",
                 "PassDataSet",
                 "PassDataSource",
                 "PutDataSetRefreshProperties",
                 "RegisterUser",
                 "RestoreAnalysis",
                 "ScopeDownPolicy",
                 "SearchAnalyses",
@@ -16710,15 +16714,16 @@
                 "UpdateResourcePermissions",
                 "UpdateTemplate",
                 "UpdateTemplateAlias",
                 "UpdateTemplatePermissions",
                 "UpdateTheme",
                 "UpdateThemeAlias",
                 "UpdateThemePermissions",
-                "UpdateUser"
+                "UpdateUser",
+                "UpdateVPCConnection"
             ],
             "HasResource": true,
             "StringPrefix": "quicksight",
             "conditionKeys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:ResourceTag/${TagKey}",
                 "aws:TagKeys",
```

### Comparing `iam_actions-1.2.20230505/iam_actions/resourcetypes.json` & `iam_actions-1.2.20230506/iam_actions/resourcetypes.json`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20230505/iam_actions/services.json` & `iam_actions-1.2.20230506/iam_actions/services.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999945695870942%*

 * *Differences: {"'quicksight'": "{'Actions': {insert: [(80, 'DescribeVPCConnection'), (112, "*

 * *                 "'ListVPCConnections'), (159, 'UpdateVPCConnection')]}}",*

 * * "'securityhub'": "{'Actions': {insert: [(4, 'BatchGetControlEvaluations'), (40, "*

 * *                  "'GetFindingHistory')]}}"}*

```diff
@@ -15319,14 +15319,15 @@
             "DescribeTemplate",
             "DescribeTemplateAlias",
             "DescribeTemplatePermissions",
             "DescribeTheme",
             "DescribeThemeAlias",
             "DescribeThemePermissions",
             "DescribeUser",
+            "DescribeVPCConnection",
             "GenerateEmbedUrlForAnonymousUser",
             "GenerateEmbedUrlForRegisteredUser",
             "GetAnonymousUserEmbedUrl",
             "GetAuthCode",
             "GetDashboardEmbedUrl",
             "GetGroupMapping",
             "GetSessionEmbedUrl",
@@ -15350,14 +15351,15 @@
             "ListTemplateVersions",
             "ListTemplates",
             "ListThemeAliases",
             "ListThemeVersions",
             "ListThemes",
             "ListUserGroups",
             "ListUsers",
+            "ListVPCConnections",
             "PassDataSet",
             "PassDataSource",
             "PutDataSetRefreshProperties",
             "RegisterUser",
             "RestoreAnalysis",
             "ScopeDownPolicy",
             "SearchAnalyses",
@@ -15395,15 +15397,16 @@
             "UpdateResourcePermissions",
             "UpdateTemplate",
             "UpdateTemplateAlias",
             "UpdateTemplatePermissions",
             "UpdateTheme",
             "UpdateThemeAlias",
             "UpdateThemePermissions",
-            "UpdateUser"
+            "UpdateUser",
+            "UpdateVPCConnection"
         ],
         "ConditionKeys": [
             "aws:RequestTag/${TagKey}",
             "aws:ResourceTag/${TagKey}",
             "aws:TagKeys",
             "quicksight:AllowedEmbeddingDomains",
             "quicksight:DirectoryType",
@@ -17799,14 +17802,15 @@
             "^arn:aws:securityhub:.+"
         ],
         "Actions": [
             "AcceptAdministratorInvitation",
             "AcceptInvitation",
             "BatchDisableStandards",
             "BatchEnableStandards",
+            "BatchGetControlEvaluations",
             "BatchGetSecurityControls",
             "BatchGetStandardsControlAssociations",
             "BatchImportFindings",
             "BatchUpdateFindings",
             "BatchUpdateStandardsControlAssociations",
             "CreateActionTarget",
             "CreateFindingAggregator",
@@ -17834,14 +17838,15 @@
             "EnableOrganizationAdminAccount",
             "EnableSecurityHub",
             "GetAdhocInsightResults",
             "GetAdministratorAccount",
             "GetControlFindingSummary",
             "GetEnabledStandards",
             "GetFindingAggregator",
+            "GetFindingHistory",
             "GetFindings",
             "GetFreeTrialEndDate",
             "GetFreeTrialUsage",
             "GetInsightFindingTrend",
             "GetInsightResults",
             "GetInsights",
             "GetInvitationsCount",
```

### Comparing `iam_actions-1.2.20230505/pyproject.toml` & `iam_actions-1.2.20230506/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20230505"
+version = "1.2.20230506"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20230505/setup.py` & `iam_actions-1.2.20230506/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20230505',
+    'version': '1.2.20230506',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20230505/PKG-INFO` & `iam_actions-1.2.20230506/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20230505
+Version: 1.2.20230506
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

