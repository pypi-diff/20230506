# Comparing `tmp/simple_aws_ec2-0.1.3.tar.gz` & `tmp/simple_aws_ec2-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simple_aws_ec2-0.1.3.tar", last modified: Wed May  3 17:17:59 2023, max compression
+gzip compressed data, was "simple_aws_ec2-0.1.4.tar", last modified: Sat May  6 21:10:40 2023, max compression
```

## Comparing `simple_aws_ec2-0.1.3.tar` & `simple_aws_ec2-0.1.4.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-03 17:17:59.298587 simple_aws_ec2-0.1.3/
--rw-r--r--   0 sanhehu    (501) staff       (20)      509 2023-05-03 14:52:18.000000 simple_aws_ec2-0.1.3/AUTHORS.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)     1124 2023-05-03 14:52:18.000000 simple_aws_ec2-0.1.3/LICENSE.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      322 2023-05-03 14:52:18.000000 simple_aws_ec2-0.1.3/MANIFEST.in
--rw-r--r--   0 sanhehu    (501) staff       (20)     4922 2023-05-03 17:17:59.298389 simple_aws_ec2-0.1.3/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)     3860 2023-05-03 16:06:52.000000 simple_aws_ec2-0.1.3/README.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)      903 2023-05-03 17:17:41.000000 simple_aws_ec2-0.1.3/release-history.rst
--rw-r--r--   0 sanhehu    (501) staff       (20)      284 2023-05-03 14:52:18.000000 simple_aws_ec2-0.1.3/requirements-dev.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      621 2023-05-03 14:52:18.000000 simple_aws_ec2-0.1.3/requirements-doc.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      193 2023-05-03 14:53:32.000000 simple_aws_ec2-0.1.3/requirements-test.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       76 2023-05-03 14:58:41.000000 simple_aws_ec2-0.1.3/requirements.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-05-03 17:17:59.298642 simple_aws_ec2-0.1.3/setup.cfg
--rw-r--r--   0 sanhehu    (501) staff       (20)     7513 2023-05-03 14:54:47.000000 simple_aws_ec2-0.1.3/setup.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-03 17:17:59.289245 simple_aws_ec2-0.1.3/simple_aws_ec2/
--rw-r--r--   0 sanhehu    (501) staff       (20)      398 2023-05-03 16:05:44.000000 simple_aws_ec2-0.1.3/simple_aws_ec2/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-05-03 17:17:00.000000 simple_aws_ec2-0.1.3/simple_aws_ec2/_version.py
--rw-r--r--   0 sanhehu    (501) staff       (20)      116 2023-05-03 16:04:16.000000 simple_aws_ec2-0.1.3/simple_aws_ec2/api.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-03 17:17:59.289972 simple_aws_ec2-0.1.3/simple_aws_ec2/docs/
--rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-05-03 14:52:18.000000 simple_aws_ec2-0.1.3/simple_aws_ec2/docs/__init__.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     6621 2023-05-03 17:16:12.000000 simple_aws_ec2-0.1.3/simple_aws_ec2/ec2.py
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-03 17:17:59.289839 simple_aws_ec2-0.1.3/simple_aws_ec2.egg-info/
--rw-r--r--   0 sanhehu    (501) staff       (20)     4922 2023-05-03 17:17:59.000000 simple_aws_ec2-0.1.3/simple_aws_ec2.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (501) staff       (20)      511 2023-05-03 17:17:59.000000 simple_aws_ec2-0.1.3/simple_aws_ec2.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-05-03 17:17:59.000000 simple_aws_ec2-0.1.3/simple_aws_ec2.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)      257 2023-05-03 17:17:59.000000 simple_aws_ec2-0.1.3/simple_aws_ec2.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (501) staff       (20)       15 2023-05-03 17:17:59.000000 simple_aws_ec2-0.1.3/simple_aws_ec2.egg-info/top_level.txt
-drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-03 17:17:59.297126 simple_aws_ec2-0.1.3/tests/
--rw-r--r--   0 sanhehu    (501) staff       (20)      315 2023-05-03 16:04:16.000000 simple_aws_ec2-0.1.3/tests/test_api.py
--rw-r--r--   0 sanhehu    (501) staff       (20)     3457 2023-05-03 15:15:52.000000 simple_aws_ec2-0.1.3/tests/test_ec2.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-06 21:10:40.511444 simple_aws_ec2-0.1.4/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      509 2023-05-03 14:52:18.000000 simple_aws_ec2-0.1.4/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1124 2023-05-03 14:52:18.000000 simple_aws_ec2-0.1.4/LICENSE.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      322 2023-05-03 14:52:18.000000 simple_aws_ec2-0.1.4/MANIFEST.in
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4922 2023-05-06 21:10:40.511266 simple_aws_ec2-0.1.4/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3860 2023-05-03 16:06:52.000000 simple_aws_ec2-0.1.4/README.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)     1165 2023-05-06 21:09:45.000000 simple_aws_ec2-0.1.4/release-history.rst
+-rw-r--r--   0 sanhehu    (501) staff       (20)      284 2023-05-03 14:52:18.000000 simple_aws_ec2-0.1.4/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      621 2023-05-03 14:52:18.000000 simple_aws_ec2-0.1.4/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      193 2023-05-03 14:53:32.000000 simple_aws_ec2-0.1.4/requirements-test.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       76 2023-05-03 14:58:41.000000 simple_aws_ec2-0.1.4/requirements.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       38 2023-05-06 21:10:40.511500 simple_aws_ec2-0.1.4/setup.cfg
+-rw-r--r--   0 sanhehu    (501) staff       (20)     7513 2023-05-03 14:54:47.000000 simple_aws_ec2-0.1.4/setup.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-06 21:10:40.508868 simple_aws_ec2-0.1.4/simple_aws_ec2/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      398 2023-05-03 16:05:44.000000 simple_aws_ec2-0.1.4/simple_aws_ec2/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)       93 2023-05-06 21:06:30.000000 simple_aws_ec2-0.1.4/simple_aws_ec2/_version.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)      116 2023-05-03 16:04:16.000000 simple_aws_ec2-0.1.4/simple_aws_ec2/api.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-06 21:10:40.510024 simple_aws_ec2-0.1.4/simple_aws_ec2/docs/
+-rw-r--r--   0 sanhehu    (501) staff       (20)       43 2023-05-03 14:52:18.000000 simple_aws_ec2-0.1.4/simple_aws_ec2/docs/__init__.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     6864 2023-05-06 21:10:23.000000 simple_aws_ec2-0.1.4/simple_aws_ec2/ec2.py
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-06 21:10:40.509872 simple_aws_ec2-0.1.4/simple_aws_ec2.egg-info/
+-rw-r--r--   0 sanhehu    (501) staff       (20)     4922 2023-05-06 21:10:40.000000 simple_aws_ec2-0.1.4/simple_aws_ec2.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (501) staff       (20)      511 2023-05-06 21:10:40.000000 simple_aws_ec2-0.1.4/simple_aws_ec2.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)        1 2023-05-06 21:10:40.000000 simple_aws_ec2-0.1.4/simple_aws_ec2.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)      257 2023-05-06 21:10:40.000000 simple_aws_ec2-0.1.4/simple_aws_ec2.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (501) staff       (20)       15 2023-05-06 21:10:40.000000 simple_aws_ec2-0.1.4/simple_aws_ec2.egg-info/top_level.txt
+drwxr-xr-x   0 sanhehu    (501) staff       (20)        0 2023-05-06 21:10:40.510903 simple_aws_ec2-0.1.4/tests/
+-rw-r--r--   0 sanhehu    (501) staff       (20)      315 2023-05-03 16:04:16.000000 simple_aws_ec2-0.1.4/tests/test_api.py
+-rw-r--r--   0 sanhehu    (501) staff       (20)     3457 2023-05-03 15:15:52.000000 simple_aws_ec2-0.1.4/tests/test_ec2.py
```

### Comparing `simple_aws_ec2-0.1.3/LICENSE.txt` & `simple_aws_ec2-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `simple_aws_ec2-0.1.3/PKG-INFO` & `simple_aws_ec2-0.1.4/simple_aws_ec2.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: simple_aws_ec2
-Version: 0.1.3
+Name: simple-aws-ec2
+Version: 0.1.4
 Summary: Simple AWS EC2 devtool.
 Home-page: https://github.com/MacHu-GWU/simple_aws_ec2-project
-Download-URL: https://pypi.python.org/pypi/simple_aws_ec2/0.1.3#downloads
+Download-URL: https://pypi.python.org/pypi/simple_aws_ec2/0.1.4#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Unknown
 License: MIT
 Platform: Windows
 Platform: MacOS
 Platform: Unix
```

### Comparing `simple_aws_ec2-0.1.3/README.rst` & `simple_aws_ec2-0.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `simple_aws_ec2-0.1.3/release-history.rst` & `simple_aws_ec2-0.1.4/release-history.rst`

 * *Files 25% similar despite different names*

```diff
@@ -11,14 +11,21 @@
 **Minor Improvements**
 
 **Bugfixes**
 
 **Miscellaneous**
 
 
+0.1.4 (2023-05-06)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+**Bugfixes**
+
+- fix a bug that the :meth:`~simple_aws_ec2.ec2.Ec2Instance._yield_dict_from_describe_instances_response` method failed to yield instances objects.
+
+
 0.1.3 (2023-05-03)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Bugfixes**
 
 - fix a bug that when you describe ec2 instances with instance ids, we should not use any paginator configuration.
```

### Comparing `simple_aws_ec2-0.1.3/requirements-doc.txt` & `simple_aws_ec2-0.1.4/requirements-doc.txt`

 * *Files identical despite different names*

### Comparing `simple_aws_ec2-0.1.3/setup.py` & `simple_aws_ec2-0.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `simple_aws_ec2-0.1.3/simple_aws_ec2/ec2.py` & `simple_aws_ec2-0.1.4/simple_aws_ec2/ec2.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,14 +28,20 @@
     Get the EC2 instance id from the AWS EC2 metadata API.
     """
     url = "http://169.254.169.254/latest/meta-data/instance-id"
     return get_response(url).strip()
 
 
 class EC2InstanceStatusEnum(str, enum.Enum):
+    """
+    EC2 instance status enumerations.
+
+    See also: https://docs.aws.amazon.com/AWSEC2/latest/UserGuide/monitoring-instance-state-changes.html
+    """
+
     pending = "pending"
     running = "running"
     shutting_down = "shutting-down"
     terminated = "terminated"
     stopping = "stopping"
     stopped = "stopped"
 
@@ -132,29 +138,28 @@
     # --------------------------------------------------------------------------
     # more constructor methods
     # --------------------------------------------------------------------------
     @classmethod
     def _yield_dict_from_describe_instances_response(
         cls, res: dict
     ) -> T.Iterable["Ec2Instance"]:
-        reservations = res.get("Reservations", [])
-        if len(reservations):
-            instances = reservations[0].get("Instances", [])
-            if len(instances):
-                for instance_dict in instances:
-                    yield cls.from_dict(instance_dict)
+        for reservation in res.get("Reservations", []):
+            for instance_dict in reservation.get("Instances", []):
+                yield cls.from_dict(instance_dict)
 
     @classmethod
     def query(
         cls,
         bsm: "BotoSesManager",
         filters: T.List[dict] = NOTHING,
         instance_ids: T.List[str] = NOTHING,
     ) -> "Ec2InstanceIterProxy":
-        """ """
+        """
+        TODO: docstring
+        """
 
         def run():
             paginator = bsm.ec2_client.get_paginator("describe_instances")
             kwargs = resolve_kwargs(
                 Filters=filters,
                 InstanceIds=instance_ids,
                 PaginationConfig={
@@ -168,53 +173,63 @@
             for response in response_iterator:
                 yield from cls._yield_dict_from_describe_instances_response(response)
 
         return Ec2InstanceIterProxy(run())
 
     @classmethod
     def from_id(cls, bsm: "BotoSesManager", inst_id: str) -> T.Optional["Ec2Instance"]:
-        """ """
+        """
+        TODO: docstring
+        """
         return cls.query(
             bsm,
             instance_ids=[inst_id],
         ).one_or_none()
 
     @classmethod
     def from_ec2_inside(
         cls, bsm: "BotoSesManager"
     ) -> T.Optional["Ec2Instance"]:  # pragma: no cover
-        """ """
+        """
+        TODO: docstring
+        """
         instance_id = get_instance_id()
         return cls.query(
             bsm,
             instance_ids=[instance_id],
         ).one()
 
     @classmethod
     def from_tag_key_value(
         cls,
         bsm: "BotoSesManager",
         key: str,
         value: str,
     ) -> "Ec2InstanceIterProxy":
-        """ """
+        """
+        TODO: docstring
+        """
         return cls.query(
             bsm,
             filters=[
                 dict(Name=f"tag:{key}", Values=[value]),
             ],
         )
 
     @classmethod
     def from_ec2_name(
         cls,
         bsm: "BotoSesManager",
         name: str,
     ) -> "Ec2InstanceIterProxy":
-        """ """
+        """
+        TODO: docstring
+        """
         return cls.from_tag_key_value(bsm, key="Name", value=name)
 
 
 class Ec2InstanceIterProxy(IterProxy[Ec2Instance]):
-    """ """
+    """
+    TODO: docstring
+    """
 
     pass
```

### Comparing `simple_aws_ec2-0.1.3/simple_aws_ec2.egg-info/PKG-INFO` & `simple_aws_ec2-0.1.4/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
-Name: simple-aws-ec2
-Version: 0.1.3
+Name: simple_aws_ec2
+Version: 0.1.4
 Summary: Simple AWS EC2 devtool.
 Home-page: https://github.com/MacHu-GWU/simple_aws_ec2-project
-Download-URL: https://pypi.python.org/pypi/simple_aws_ec2/0.1.3#downloads
+Download-URL: https://pypi.python.org/pypi/simple_aws_ec2/0.1.4#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Unknown
 License: MIT
 Platform: Windows
 Platform: MacOS
 Platform: Unix
```

### Comparing `simple_aws_ec2-0.1.3/tests/test_ec2.py` & `simple_aws_ec2-0.1.4/tests/test_ec2.py`

 * *Files identical despite different names*

