# Comparing `tmp/vents-0.1.0.tar.gz` & `tmp/vents-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vents-0.1.0.tar", last modified: Fri May  5 08:50:41 2023, max compression
+gzip compressed data, was "vents-0.1.1.tar", last modified: Fri May  5 18:42:21 2023, max compression
```

## Comparing `vents-0.1.0.tar` & `vents-0.1.1.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-05-05 08:50:41.985060 vents-0.1.0/
--rw-r--r--   0 mourad     (501) staff       (20)      172 2023-05-05 08:48:57.000000 vents-0.1.0/MANIFEST.in
--rw-r--r--   0 mourad     (501) staff       (20)     1568 2023-05-05 08:50:41.985153 vents-0.1.0/PKG-INFO
--rw-r--r--   0 mourad     (501) staff       (20)     1031 2023-05-05 08:50:41.985680 vents-0.1.0/setup.cfg
--rw-r--r--   0 mourad     (501) staff       (20)     2695 2023-05-05 08:48:57.000000 vents-0.1.0/setup.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-05-05 08:50:41.978065 vents-0.1.0/vents/
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-05-05 08:48:57.000000 vents-0.1.0/vents/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)     4857 2023-05-05 08:48:57.000000 vents-0.1.0/vents/config.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-05-05 08:50:41.980359 vents-0.1.0/vents/connections/
--rw-r--r--   0 mourad     (501) staff       (20)      335 2023-05-05 08:48:57.000000 vents-0.1.0/vents/connections/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)     2485 2023-05-05 08:48:57.000000 vents-0.1.0/vents/connections/catalog.py
--rw-r--r--   0 mourad     (501) staff       (20)     2916 2023-05-05 08:48:57.000000 vents-0.1.0/vents/connections/connection.py
--rw-r--r--   0 mourad     (501) staff       (20)      513 2023-05-05 08:48:57.000000 vents-0.1.0/vents/connections/connection_resource.py
--rw-r--r--   0 mourad     (501) staff       (20)     3301 2023-05-05 08:48:57.000000 vents-0.1.0/vents/connections/connection_schema.py
--rw-r--r--   0 mourad     (501) staff       (20)       37 2023-05-05 08:48:57.000000 vents-0.1.0/vents/exceptions.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-05-05 08:50:41.982107 vents-0.1.0/vents/notifiers/
--rw-r--r--   0 mourad     (501) staff       (20)      866 2023-05-05 08:48:57.000000 vents-0.1.0/vents/notifiers/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)     4589 2023-05-05 08:48:57.000000 vents-0.1.0/vents/notifiers/base.py
--rw-r--r--   0 mourad     (501) staff       (20)     1303 2023-05-05 08:48:57.000000 vents-0.1.0/vents/notifiers/discord_webhook.py
--rw-r--r--   0 mourad     (501) staff       (20)     1277 2023-05-05 08:48:57.000000 vents-0.1.0/vents/notifiers/hipchat_webhook.py
--rw-r--r--   0 mourad     (501) staff       (20)     1764 2023-05-05 08:48:57.000000 vents-0.1.0/vents/notifiers/mattermost_webhook.py
--rw-r--r--   0 mourad     (501) staff       (20)     1723 2023-05-05 08:48:57.000000 vents-0.1.0/vents/notifiers/pagerduty_webhook.py
--rw-r--r--   0 mourad     (501) staff       (20)     2051 2023-05-05 08:48:57.000000 vents-0.1.0/vents/notifiers/slack_webhook.py
--rw-r--r--   0 mourad     (501) staff       (20)      372 2023-05-05 08:48:57.000000 vents-0.1.0/vents/notifiers/spec.py
--rw-r--r--   0 mourad     (501) staff       (20)     1847 2023-05-05 08:48:57.000000 vents-0.1.0/vents/notifiers/webhook.py
--rw-r--r--   0 mourad     (501) staff       (20)      233 2023-05-05 08:48:57.000000 vents-0.1.0/vents/pkg.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-05-05 08:50:41.982685 vents-0.1.0/vents/providers/
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-05-05 08:48:57.000000 vents-0.1.0/vents/providers/__init__.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-05-05 08:50:41.983410 vents-0.1.0/vents/providers/aws/
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-05-05 08:48:57.000000 vents-0.1.0/vents/providers/aws/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)     3724 2023-05-05 08:48:57.000000 vents-0.1.0/vents/providers/aws/base.py
--rw-r--r--   0 mourad     (501) staff       (20)     1656 2023-05-05 08:48:57.000000 vents-0.1.0/vents/providers/aws/s3.py
--rw-r--r--   0 mourad     (501) staff       (20)     3456 2023-05-05 08:48:57.000000 vents-0.1.0/vents/providers/aws/service.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-05-05 08:50:41.984146 vents-0.1.0/vents/providers/azure/
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-05-05 08:48:57.000000 vents-0.1.0/vents/providers/azure/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)     2609 2023-05-05 08:48:57.000000 vents-0.1.0/vents/providers/azure/base.py
--rw-r--r--   0 mourad     (501) staff       (20)     1831 2023-05-05 08:48:57.000000 vents-0.1.0/vents/providers/azure/blob_storage.py
--rw-r--r--   0 mourad     (501) staff       (20)     2251 2023-05-05 08:48:57.000000 vents-0.1.0/vents/providers/azure/service.py
--rw-r--r--   0 mourad     (501) staff       (20)     1620 2023-05-05 08:48:57.000000 vents-0.1.0/vents/providers/base.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-05-05 08:50:41.984877 vents-0.1.0/vents/providers/gcp/
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-05-05 08:48:57.000000 vents-0.1.0/vents/providers/gcp/__init__.py
--rw-r--r--   0 mourad     (501) staff       (20)     3750 2023-05-05 08:48:57.000000 vents-0.1.0/vents/providers/gcp/base.py
--rw-r--r--   0 mourad     (501) staff       (20)      995 2023-05-05 08:48:57.000000 vents-0.1.0/vents/providers/gcp/gcs.py
--rw-r--r--   0 mourad     (501) staff       (20)     2513 2023-05-05 08:48:57.000000 vents-0.1.0/vents/providers/gcp/service.py
--rw-r--r--   0 mourad     (501) staff       (20)     2337 2023-05-05 08:48:57.000000 vents-0.1.0/vents/providers/kinds.py
--rw-r--r--   0 mourad     (501) staff       (20)        0 2023-05-05 08:48:57.000000 vents-0.1.0/vents/py.typed
--rw-r--r--   0 mourad     (501) staff       (20)      256 2023-05-05 08:48:57.000000 vents-0.1.0/vents/settings.py
-drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-05-05 08:50:41.979106 vents-0.1.0/vents.egg-info/
--rw-r--r--   0 mourad     (501) staff       (20)     1568 2023-05-05 08:50:41.000000 vents-0.1.0/vents.egg-info/PKG-INFO
--rw-r--r--   0 mourad     (501) staff       (20)     1216 2023-05-05 08:50:41.000000 vents-0.1.0/vents.egg-info/SOURCES.txt
--rw-r--r--   0 mourad     (501) staff       (20)        1 2023-05-05 08:50:41.000000 vents-0.1.0/vents.egg-info/dependency_links.txt
--rw-r--r--   0 mourad     (501) staff       (20)       66 2023-05-05 08:50:41.000000 vents-0.1.0/vents.egg-info/requires.txt
--rw-r--r--   0 mourad     (501) staff       (20)        6 2023-05-05 08:50:41.000000 vents-0.1.0/vents.egg-info/top_level.txt
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-05-05 18:42:21.761314 vents-0.1.1/
+-rw-r--r--   0 mourad     (501) staff       (20)      172 2023-05-05 18:39:27.000000 vents-0.1.1/MANIFEST.in
+-rw-r--r--   0 mourad     (501) staff       (20)     1568 2023-05-05 18:42:21.761429 vents-0.1.1/PKG-INFO
+-rw-r--r--   0 mourad     (501) staff       (20)     1031 2023-05-05 18:42:21.761975 vents-0.1.1/setup.cfg
+-rw-r--r--   0 mourad     (501) staff       (20)     2695 2023-05-05 18:39:27.000000 vents-0.1.1/setup.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-05-05 18:42:21.754849 vents-0.1.1/vents/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-05-05 18:39:27.000000 vents-0.1.1/vents/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)     4857 2023-05-05 18:39:27.000000 vents-0.1.1/vents/config.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-05-05 18:42:21.756823 vents-0.1.1/vents/connections/
+-rw-r--r--   0 mourad     (501) staff       (20)      335 2023-05-05 18:39:27.000000 vents-0.1.1/vents/connections/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2485 2023-05-05 18:39:27.000000 vents-0.1.1/vents/connections/catalog.py
+-rw-r--r--   0 mourad     (501) staff       (20)     3813 2023-05-05 18:39:27.000000 vents-0.1.1/vents/connections/connection.py
+-rw-r--r--   0 mourad     (501) staff       (20)      513 2023-05-05 18:39:27.000000 vents-0.1.1/vents/connections/connection_resource.py
+-rw-r--r--   0 mourad     (501) staff       (20)     3301 2023-05-05 18:39:27.000000 vents-0.1.1/vents/connections/connection_schema.py
+-rw-r--r--   0 mourad     (501) staff       (20)       37 2023-05-05 18:39:27.000000 vents-0.1.1/vents/exceptions.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-05-05 18:42:21.758514 vents-0.1.1/vents/notifiers/
+-rw-r--r--   0 mourad     (501) staff       (20)      866 2023-05-05 18:39:27.000000 vents-0.1.1/vents/notifiers/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)     4589 2023-05-05 18:39:27.000000 vents-0.1.1/vents/notifiers/base.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1303 2023-05-05 18:39:27.000000 vents-0.1.1/vents/notifiers/discord_webhook.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1277 2023-05-05 18:39:27.000000 vents-0.1.1/vents/notifiers/hipchat_webhook.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1764 2023-05-05 18:39:27.000000 vents-0.1.1/vents/notifiers/mattermost_webhook.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1723 2023-05-05 18:39:27.000000 vents-0.1.1/vents/notifiers/pagerduty_webhook.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2051 2023-05-05 18:39:27.000000 vents-0.1.1/vents/notifiers/slack_webhook.py
+-rw-r--r--   0 mourad     (501) staff       (20)      372 2023-05-05 18:39:27.000000 vents-0.1.1/vents/notifiers/spec.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1847 2023-05-05 18:39:27.000000 vents-0.1.1/vents/notifiers/webhook.py
+-rw-r--r--   0 mourad     (501) staff       (20)      233 2023-05-05 18:39:27.000000 vents-0.1.1/vents/pkg.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-05-05 18:42:21.759060 vents-0.1.1/vents/providers/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-05-05 18:39:27.000000 vents-0.1.1/vents/providers/__init__.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-05-05 18:42:21.759734 vents-0.1.1/vents/providers/aws/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-05-05 18:39:27.000000 vents-0.1.1/vents/providers/aws/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)     3724 2023-05-05 18:39:27.000000 vents-0.1.1/vents/providers/aws/base.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1656 2023-05-05 18:39:27.000000 vents-0.1.1/vents/providers/aws/s3.py
+-rw-r--r--   0 mourad     (501) staff       (20)     3456 2023-05-05 18:39:27.000000 vents-0.1.1/vents/providers/aws/service.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-05-05 18:42:21.760441 vents-0.1.1/vents/providers/azure/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-05-05 18:39:27.000000 vents-0.1.1/vents/providers/azure/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2609 2023-05-05 18:39:27.000000 vents-0.1.1/vents/providers/azure/base.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1831 2023-05-05 18:39:27.000000 vents-0.1.1/vents/providers/azure/blob_storage.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2251 2023-05-05 18:39:27.000000 vents-0.1.1/vents/providers/azure/service.py
+-rw-r--r--   0 mourad     (501) staff       (20)     1620 2023-05-05 18:39:27.000000 vents-0.1.1/vents/providers/base.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-05-05 18:42:21.761124 vents-0.1.1/vents/providers/gcp/
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-05-05 18:39:27.000000 vents-0.1.1/vents/providers/gcp/__init__.py
+-rw-r--r--   0 mourad     (501) staff       (20)     3750 2023-05-05 18:39:27.000000 vents-0.1.1/vents/providers/gcp/base.py
+-rw-r--r--   0 mourad     (501) staff       (20)      995 2023-05-05 18:39:27.000000 vents-0.1.1/vents/providers/gcp/gcs.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2513 2023-05-05 18:39:27.000000 vents-0.1.1/vents/providers/gcp/service.py
+-rw-r--r--   0 mourad     (501) staff       (20)     2337 2023-05-05 18:39:27.000000 vents-0.1.1/vents/providers/kinds.py
+-rw-r--r--   0 mourad     (501) staff       (20)        0 2023-05-05 18:39:27.000000 vents-0.1.1/vents/py.typed
+-rw-r--r--   0 mourad     (501) staff       (20)      256 2023-05-05 18:39:27.000000 vents-0.1.1/vents/settings.py
+drwxr-xr-x   0 mourad     (501) staff       (20)        0 2023-05-05 18:42:21.755858 vents-0.1.1/vents.egg-info/
+-rw-r--r--   0 mourad     (501) staff       (20)     1568 2023-05-05 18:42:21.000000 vents-0.1.1/vents.egg-info/PKG-INFO
+-rw-r--r--   0 mourad     (501) staff       (20)     1216 2023-05-05 18:42:21.000000 vents-0.1.1/vents.egg-info/SOURCES.txt
+-rw-r--r--   0 mourad     (501) staff       (20)        1 2023-05-05 18:42:21.000000 vents-0.1.1/vents.egg-info/dependency_links.txt
+-rw-r--r--   0 mourad     (501) staff       (20)       66 2023-05-05 18:42:21.000000 vents-0.1.1/vents.egg-info/requires.txt
+-rw-r--r--   0 mourad     (501) staff       (20)        6 2023-05-05 18:42:21.000000 vents-0.1.1/vents.egg-info/top_level.txt
```

### Comparing `vents-0.1.0/PKG-INFO` & `vents-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vents
-Version: 0.1.0
+Version: 0.1.1
 Summary: Open source integrations, alerting, and notification library.
 Home-page: https://github.com/mmourafiq/vents
 Author: Mourad Mourafiq
 Author-email: mourad.mourafiq@gmail.com
 Maintainer: Mourad Mourafiq
 Maintainer-email: mourad.mourafiq@gmail.com
 License: Apache 2.0
```

### Comparing `vents-0.1.0/setup.cfg` & `vents-0.1.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `vents-0.1.0/setup.py` & `vents-0.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.0/vents/config.py` & `vents-0.1.1/vents/config.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.0/vents/connections/catalog.py` & `vents-0.1.1/vents/connections/catalog.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.0/vents/connections/connection.py` & `vents-0.1.1/vents/connections/connection.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Dict, List, Optional, Union
+from typing import Dict, List, Literal, Optional, Union
 
 from clipped.config.schema import BaseSchemaModel
 from clipped.types.ref_or_obj import RefField
 from pydantic import Field, StrictStr
 
 from vents.connections.connection_resource import ConnectionResource
 from vents.connections.connection_schema import ConnectionSchema
@@ -88,7 +88,29 @@
     @property
     def is_s3(self) -> bool:
         return self.kind == ProviderKind.S3
 
     @property
     def is_wasb(self) -> bool:
         return ProviderKind.is_wasb(self.kind)
+
+    @staticmethod
+    def get_requested_resources(
+        resources: List[ConnectionResource],
+        connections: List["Connection"],
+        resource_key: Literal["secret", "config_map"],
+    ) -> List[ConnectionResource]:
+        resources = resources or []
+
+        connections = connections or []
+        # Create a set of all resources:
+        #   * resources request by non managed connections
+        #   * resources requested directly by the user
+        requested_resources = [r for r in resources if r.is_requested]
+        resource_ids = {s.name for s in requested_resources}
+        for connection in connections:
+            resource = getattr(connection, resource_key)
+            if resource and resource.name not in resource_ids:
+                resource_ids.add(resource.name)
+                requested_resources.append(resource)
+
+        return requested_resources
```

### Comparing `vents-0.1.0/vents/connections/connection_resource.py` & `vents-0.1.1/vents/connections/connection_resource.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.0/vents/connections/connection_schema.py` & `vents-0.1.1/vents/connections/connection_schema.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.0/vents/notifiers/__init__.py` & `vents-0.1.1/vents/notifiers/__init__.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.0/vents/notifiers/base.py` & `vents-0.1.1/vents/notifiers/base.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.0/vents/notifiers/discord_webhook.py` & `vents-0.1.1/vents/notifiers/discord_webhook.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.0/vents/notifiers/hipchat_webhook.py` & `vents-0.1.1/vents/notifiers/hipchat_webhook.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.0/vents/notifiers/mattermost_webhook.py` & `vents-0.1.1/vents/notifiers/mattermost_webhook.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.0/vents/notifiers/pagerduty_webhook.py` & `vents-0.1.1/vents/notifiers/pagerduty_webhook.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.0/vents/notifiers/slack_webhook.py` & `vents-0.1.1/vents/notifiers/slack_webhook.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.0/vents/notifiers/webhook.py` & `vents-0.1.1/vents/notifiers/webhook.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.0/vents/providers/aws/base.py` & `vents-0.1.1/vents/providers/aws/base.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.0/vents/providers/aws/s3.py` & `vents-0.1.1/vents/providers/aws/s3.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.0/vents/providers/aws/service.py` & `vents-0.1.1/vents/providers/aws/service.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.0/vents/providers/azure/base.py` & `vents-0.1.1/vents/providers/azure/base.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.0/vents/providers/azure/blob_storage.py` & `vents-0.1.1/vents/providers/azure/blob_storage.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.0/vents/providers/azure/service.py` & `vents-0.1.1/vents/providers/azure/service.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.0/vents/providers/base.py` & `vents-0.1.1/vents/providers/base.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.0/vents/providers/gcp/base.py` & `vents-0.1.1/vents/providers/gcp/base.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.0/vents/providers/gcp/gcs.py` & `vents-0.1.1/vents/providers/gcp/gcs.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.0/vents/providers/gcp/service.py` & `vents-0.1.1/vents/providers/gcp/service.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.0/vents/providers/kinds.py` & `vents-0.1.1/vents/providers/kinds.py`

 * *Files identical despite different names*

### Comparing `vents-0.1.0/vents.egg-info/PKG-INFO` & `vents-0.1.1/vents.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vents
-Version: 0.1.0
+Version: 0.1.1
 Summary: Open source integrations, alerting, and notification library.
 Home-page: https://github.com/mmourafiq/vents
 Author: Mourad Mourafiq
 Author-email: mourad.mourafiq@gmail.com
 Maintainer: Mourad Mourafiq
 Maintainer-email: mourad.mourafiq@gmail.com
 License: Apache 2.0
```

### Comparing `vents-0.1.0/vents.egg-info/SOURCES.txt` & `vents-0.1.1/vents.egg-info/SOURCES.txt`

 * *Files identical despite different names*

