# Comparing `tmp/f5-openstack-lbaasv2-inventory-1.0.1.tar.gz` & `tmp/f5-openstack-lbaasv2-inventory-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/f5-openstack-lbaasv2-inventory-1.0.1.tar", last modified: Sun Apr 23 06:51:43 2023, max compression
+gzip compressed data, was "dist/f5-openstack-lbaasv2-inventory-1.1.0.tar", last modified: Sat May  6 02:53:08 2023, max compression
```

## Comparing `f5-openstack-lbaasv2-inventory-1.0.1.tar` & `f5-openstack-lbaasv2-inventory-1.1.0.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 qzhao     (1001) users      (100)        0 2023-04-23 06:51:43.000000 f5-openstack-lbaasv2-inventory-1.0.1/
--rw-r--r--   0 qzhao     (1001) users      (100)      680 2023-04-23 06:51:43.000000 f5-openstack-lbaasv2-inventory-1.0.1/PKG-INFO
--rw-r--r--   0 qzhao     (1001) users      (100)     6279 2023-03-30 07:52:56.000000 f5-openstack-lbaasv2-inventory-1.0.1/README.md
-drwxr-xr-x   0 qzhao     (1001) users      (100)        0 2023-04-23 06:51:43.000000 f5-openstack-lbaasv2-inventory-1.0.1/etc/
-drwxr-xr-x   0 qzhao     (1001) users      (100)        0 2023-04-23 06:51:43.000000 f5-openstack-lbaasv2-inventory-1.0.1/etc/neutron/
-drwxr-xr-x   0 qzhao     (1001) users      (100)        0 2023-04-23 06:51:43.000000 f5-openstack-lbaasv2-inventory-1.0.1/etc/neutron/policy.d/
--rw-r--r--   0 qzhao     (1001) users      (100)      484 2023-04-23 06:39:33.000000 f5-openstack-lbaasv2-inventory-1.0.1/etc/neutron/policy.d/lbaas_device.json
--rw-r--r--   0 qzhao     (1001) users      (100)       46 2023-03-30 07:52:56.000000 f5-openstack-lbaasv2-inventory-1.0.1/MANIFEST.in
-drwxr-xr-x   0 qzhao     (1001) users      (100)        0 2023-04-23 06:51:43.000000 f5-openstack-lbaasv2-inventory-1.0.1/neutron_lbaas_inventory/
-drwxr-xr-x   0 qzhao     (1001) users      (100)        0 2023-04-23 06:51:43.000000 f5-openstack-lbaasv2-inventory-1.0.1/neutron_lbaas_inventory/common/
--rw-r--r--   0 qzhao     (1001) users      (100)      136 2023-03-30 07:52:56.000000 f5-openstack-lbaasv2-inventory-1.0.1/neutron_lbaas_inventory/common/constants.py
--rw-r--r--   0 qzhao     (1001) users      (100)      591 2023-04-23 06:39:33.000000 f5-openstack-lbaasv2-inventory-1.0.1/neutron_lbaas_inventory/common/exceptions.py
--rw-r--r--   0 qzhao     (1001) users      (100)        0 2023-03-30 07:52:56.000000 f5-openstack-lbaasv2-inventory-1.0.1/neutron_lbaas_inventory/common/__init__.py
-drwxr-xr-x   0 qzhao     (1001) users      (100)        0 2023-04-23 06:51:43.000000 f5-openstack-lbaasv2-inventory-1.0.1/neutron_lbaas_inventory/plugins/
--rw-r--r--   0 qzhao     (1001) users      (100)     3068 2023-04-23 06:39:33.000000 f5-openstack-lbaasv2-inventory-1.0.1/neutron_lbaas_inventory/plugins/lbaasdevice.py
--rw-r--r--   0 qzhao     (1001) users      (100)        0 2023-03-30 07:52:56.000000 f5-openstack-lbaasv2-inventory-1.0.1/neutron_lbaas_inventory/plugins/__init__.py
-drwxr-xr-x   0 qzhao     (1001) users      (100)        0 2023-04-23 06:51:43.000000 f5-openstack-lbaasv2-inventory-1.0.1/neutron_lbaas_inventory/extensions/
--rw-r--r--   0 qzhao     (1001) users      (100)     8462 2023-04-23 06:39:33.000000 f5-openstack-lbaasv2-inventory-1.0.1/neutron_lbaas_inventory/extensions/lbaasdevice.py
--rw-r--r--   0 qzhao     (1001) users      (100)        0 2023-03-30 07:52:56.000000 f5-openstack-lbaasv2-inventory-1.0.1/neutron_lbaas_inventory/extensions/__init__.py
-drwxr-xr-x   0 qzhao     (1001) users      (100)        0 2023-04-23 06:51:43.000000 f5-openstack-lbaasv2-inventory-1.0.1/neutron_lbaas_inventory/db/
-drwxr-xr-x   0 qzhao     (1001) users      (100)        0 2023-04-23 06:51:43.000000 f5-openstack-lbaasv2-inventory-1.0.1/neutron_lbaas_inventory/db/models/
--rw-r--r--   0 qzhao     (1001) users      (100)      110 2023-03-30 07:52:56.000000 f5-openstack-lbaasv2-inventory-1.0.1/neutron_lbaas_inventory/db/models/head.py
--rw-r--r--   0 qzhao     (1001) users      (100)     1289 2023-04-23 06:39:33.000000 f5-openstack-lbaasv2-inventory-1.0.1/neutron_lbaas_inventory/db/models/inventory.py
--rw-r--r--   0 qzhao     (1001) users      (100)        0 2023-03-30 07:52:56.000000 f5-openstack-lbaasv2-inventory-1.0.1/neutron_lbaas_inventory/db/models/__init__.py
-drwxr-xr-x   0 qzhao     (1001) users      (100)        0 2023-04-23 06:51:43.000000 f5-openstack-lbaasv2-inventory-1.0.1/neutron_lbaas_inventory/db/migration/
-drwxr-xr-x   0 qzhao     (1001) users      (100)        0 2023-04-23 06:51:43.000000 f5-openstack-lbaasv2-inventory-1.0.1/neutron_lbaas_inventory/db/migration/alembic_migrations/
--rw-r--r--   0 qzhao     (1001) users      (100)     1483 2023-04-23 06:39:33.000000 f5-openstack-lbaasv2-inventory-1.0.1/neutron_lbaas_inventory/db/migration/alembic_migrations/inventory_init_ops.py
--rw-r--r--   0 qzhao     (1001) users      (100)     2076 2023-03-30 07:52:56.000000 f5-openstack-lbaasv2-inventory-1.0.1/neutron_lbaas_inventory/db/migration/alembic_migrations/env.py
--rw-r--r--   0 qzhao     (1001) users      (100)        0 2023-03-30 07:52:56.000000 f5-openstack-lbaasv2-inventory-1.0.1/neutron_lbaas_inventory/db/migration/alembic_migrations/__init__.py
-drwxr-xr-x   0 qzhao     (1001) users      (100)        0 2023-04-23 06:51:43.000000 f5-openstack-lbaasv2-inventory-1.0.1/neutron_lbaas_inventory/db/migration/alembic_migrations/versions/
--rw-r--r--   0 qzhao     (1001) users      (100)        0 2023-03-30 07:52:56.000000 f5-openstack-lbaasv2-inventory-1.0.1/neutron_lbaas_inventory/db/migration/alembic_migrations/versions/__init__.py
--rw-r--r--   0 qzhao     (1001) users      (100)      281 2023-03-30 07:52:56.000000 f5-openstack-lbaasv2-inventory-1.0.1/neutron_lbaas_inventory/db/migration/alembic_migrations/versions/pike_initial.py
--rw-r--r--   0 qzhao     (1001) users      (100)        0 2023-03-30 07:52:56.000000 f5-openstack-lbaasv2-inventory-1.0.1/neutron_lbaas_inventory/db/migration/__init__.py
--rw-r--r--   0 qzhao     (1001) users      (100)        0 2023-03-30 07:52:56.000000 f5-openstack-lbaasv2-inventory-1.0.1/neutron_lbaas_inventory/db/__init__.py
--rw-r--r--   0 qzhao     (1001) users      (100)     9972 2023-04-23 06:39:33.000000 f5-openstack-lbaasv2-inventory-1.0.1/neutron_lbaas_inventory/db/inventory_db.py
--rw-r--r--   0 qzhao     (1001) users      (100)       22 2023-04-23 06:51:22.000000 f5-openstack-lbaasv2-inventory-1.0.1/neutron_lbaas_inventory/__init__.py
--rw-r--r--   0 qzhao     (1001) users      (100)     1239 2023-03-30 07:52:56.000000 f5-openstack-lbaasv2-inventory-1.0.1/setup.py
--rw-r--r--   0 qzhao     (1001) users      (100)       38 2023-04-23 06:51:43.000000 f5-openstack-lbaasv2-inventory-1.0.1/setup.cfg
-drwxr-xr-x   0 qzhao     (1001) users      (100)        0 2023-04-23 06:51:43.000000 f5-openstack-lbaasv2-inventory-1.0.1/f5_openstack_lbaasv2_inventory.egg-info/
--rw-r--r--   0 qzhao     (1001) users      (100)      680 2023-04-23 06:51:43.000000 f5-openstack-lbaasv2-inventory-1.0.1/f5_openstack_lbaasv2_inventory.egg-info/PKG-INFO
--rw-r--r--   0 qzhao     (1001) users      (100)      219 2023-04-23 06:51:43.000000 f5-openstack-lbaasv2-inventory-1.0.1/f5_openstack_lbaasv2_inventory.egg-info/entry_points.txt
--rw-r--r--   0 qzhao     (1001) users      (100)     1331 2023-04-23 06:51:43.000000 f5-openstack-lbaasv2-inventory-1.0.1/f5_openstack_lbaasv2_inventory.egg-info/SOURCES.txt
--rw-r--r--   0 qzhao     (1001) users      (100)       24 2023-04-23 06:51:43.000000 f5-openstack-lbaasv2-inventory-1.0.1/f5_openstack_lbaasv2_inventory.egg-info/top_level.txt
--rw-r--r--   0 qzhao     (1001) users      (100)        1 2023-04-23 06:51:43.000000 f5-openstack-lbaasv2-inventory-1.0.1/f5_openstack_lbaasv2_inventory.egg-info/dependency_links.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 02:53:08.000000 f5-openstack-lbaasv2-inventory-1.1.0/
+-rw-rw-rw-   0 root         (0) root         (0)       46 2023-05-06 02:52:43.000000 f5-openstack-lbaasv2-inventory-1.1.0/MANIFEST.in
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 02:53:08.000000 f5-openstack-lbaasv2-inventory-1.1.0/etc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 02:53:08.000000 f5-openstack-lbaasv2-inventory-1.1.0/etc/neutron/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 02:53:08.000000 f5-openstack-lbaasv2-inventory-1.1.0/etc/neutron/policy.d/
+-rw-rw-rw-   0 root         (0) root         (0)      484 2023-05-06 02:52:43.000000 f5-openstack-lbaasv2-inventory-1.1.0/etc/neutron/policy.d/lbaas_device.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 02:53:08.000000 f5-openstack-lbaasv2-inventory-1.1.0/neutron_lbaas_inventory/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 02:53:08.000000 f5-openstack-lbaasv2-inventory-1.1.0/neutron_lbaas_inventory/db/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 02:53:08.000000 f5-openstack-lbaasv2-inventory-1.1.0/neutron_lbaas_inventory/db/migration/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-06 02:52:43.000000 f5-openstack-lbaasv2-inventory-1.1.0/neutron_lbaas_inventory/db/migration/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 02:53:08.000000 f5-openstack-lbaasv2-inventory-1.1.0/neutron_lbaas_inventory/db/migration/alembic_migrations/
+-rw-rw-rw-   0 root         (0) root         (0)     1482 2023-05-06 02:52:43.000000 f5-openstack-lbaasv2-inventory-1.1.0/neutron_lbaas_inventory/db/migration/alembic_migrations/inventory_init_ops.py
+-rw-rw-rw-   0 root         (0) root         (0)     2076 2023-05-06 02:52:43.000000 f5-openstack-lbaasv2-inventory-1.1.0/neutron_lbaas_inventory/db/migration/alembic_migrations/env.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-06 02:52:43.000000 f5-openstack-lbaasv2-inventory-1.1.0/neutron_lbaas_inventory/db/migration/alembic_migrations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 02:53:08.000000 f5-openstack-lbaasv2-inventory-1.1.0/neutron_lbaas_inventory/db/migration/alembic_migrations/versions/
+-rw-rw-rw-   0 root         (0) root         (0)      281 2023-05-06 02:52:43.000000 f5-openstack-lbaasv2-inventory-1.1.0/neutron_lbaas_inventory/db/migration/alembic_migrations/versions/pike_initial.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-06 02:52:43.000000 f5-openstack-lbaasv2-inventory-1.1.0/neutron_lbaas_inventory/db/migration/alembic_migrations/versions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-06 02:52:43.000000 f5-openstack-lbaasv2-inventory-1.1.0/neutron_lbaas_inventory/db/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     9885 2023-05-06 02:52:43.000000 f5-openstack-lbaasv2-inventory-1.1.0/neutron_lbaas_inventory/db/inventory_db.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 02:53:08.000000 f5-openstack-lbaasv2-inventory-1.1.0/neutron_lbaas_inventory/db/models/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-06 02:52:43.000000 f5-openstack-lbaasv2-inventory-1.1.0/neutron_lbaas_inventory/db/models/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1288 2023-05-06 02:52:43.000000 f5-openstack-lbaasv2-inventory-1.1.0/neutron_lbaas_inventory/db/models/inventory.py
+-rw-rw-rw-   0 root         (0) root         (0)      110 2023-05-06 02:52:43.000000 f5-openstack-lbaasv2-inventory-1.1.0/neutron_lbaas_inventory/db/models/head.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 02:53:08.000000 f5-openstack-lbaasv2-inventory-1.1.0/neutron_lbaas_inventory/plugins/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-06 02:52:43.000000 f5-openstack-lbaasv2-inventory-1.1.0/neutron_lbaas_inventory/plugins/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3073 2023-05-06 02:52:43.000000 f5-openstack-lbaasv2-inventory-1.1.0/neutron_lbaas_inventory/plugins/lbaasdevice.py
+-rw-rw-rw-   0 root         (0) root         (0)       22 2023-05-06 02:52:43.000000 f5-openstack-lbaasv2-inventory-1.1.0/neutron_lbaas_inventory/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 02:53:08.000000 f5-openstack-lbaasv2-inventory-1.1.0/neutron_lbaas_inventory/extensions/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-06 02:52:43.000000 f5-openstack-lbaasv2-inventory-1.1.0/neutron_lbaas_inventory/extensions/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8467 2023-05-06 02:52:43.000000 f5-openstack-lbaasv2-inventory-1.1.0/neutron_lbaas_inventory/extensions/lbaasdevice.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 02:53:08.000000 f5-openstack-lbaasv2-inventory-1.1.0/neutron_lbaas_inventory/common/
+-rw-rw-rw-   0 root         (0) root         (0)      136 2023-05-06 02:52:43.000000 f5-openstack-lbaasv2-inventory-1.1.0/neutron_lbaas_inventory/common/constants.py
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-05-06 02:52:43.000000 f5-openstack-lbaasv2-inventory-1.1.0/neutron_lbaas_inventory/common/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      591 2023-05-06 02:52:43.000000 f5-openstack-lbaasv2-inventory-1.1.0/neutron_lbaas_inventory/common/exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     6279 2023-05-06 02:52:43.000000 f5-openstack-lbaasv2-inventory-1.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-06 02:53:08.000000 f5-openstack-lbaasv2-inventory-1.1.0/f5_openstack_lbaasv2_inventory.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      219 2023-05-06 02:53:08.000000 f5-openstack-lbaasv2-inventory-1.1.0/f5_openstack_lbaasv2_inventory.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)     1331 2023-05-06 02:53:08.000000 f5-openstack-lbaasv2-inventory-1.1.0/f5_openstack_lbaasv2_inventory.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)       24 2023-05-06 02:53:08.000000 f5-openstack-lbaasv2-inventory-1.1.0/f5_openstack_lbaasv2_inventory.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-06 02:53:08.000000 f5-openstack-lbaasv2-inventory-1.1.0/f5_openstack_lbaasv2_inventory.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      680 2023-05-06 02:53:08.000000 f5-openstack-lbaasv2-inventory-1.1.0/f5_openstack_lbaasv2_inventory.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     1239 2023-05-06 02:52:43.000000 f5-openstack-lbaasv2-inventory-1.1.0/setup.py
+-rw-r--r--   0 root         (0) root         (0)      680 2023-05-06 02:53:08.000000 f5-openstack-lbaasv2-inventory-1.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-06 02:53:08.000000 f5-openstack-lbaasv2-inventory-1.1.0/setup.cfg
```

### Comparing `f5-openstack-lbaasv2-inventory-1.0.1/PKG-INFO` & `f5-openstack-lbaasv2-inventory-1.1.0/f5_openstack_lbaasv2_inventory.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: f5-openstack-lbaasv2-inventory
-Version: 1.0.1
+Version: 1.1.0
 Summary: F5 Networks device inventory for OpenStack services
 Home-page: UNKNOWN
 Author: F5 Networks
 Author-email: openstack@f5.com
 License: Apache License, Version 2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `f5-openstack-lbaasv2-inventory-1.0.1/README.md` & `f5-openstack-lbaasv2-inventory-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `f5-openstack-lbaasv2-inventory-1.0.1/neutron_lbaas_inventory/common/exceptions.py` & `f5-openstack-lbaasv2-inventory-1.1.0/neutron_lbaas_inventory/common/exceptions.py`

 * *Files identical despite different names*

### Comparing `f5-openstack-lbaasv2-inventory-1.0.1/neutron_lbaas_inventory/plugins/lbaasdevice.py` & `f5-openstack-lbaasv2-inventory-1.1.0/neutron_lbaas_inventory/plugins/lbaasdevice.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,11 +58,11 @@
         return self.inventory_db.create_member(context, device_id, member)
 
     def update_device_member(self, context, id, device_id, member):
         LOG.debug("Update lbaas device member, device_id: {}, id: {}"
                   .format(device_id, id))
         return self.inventory_db.update_member(context, id, member)
 
-    def delete_device_member(self, context, id, device_id):
+    def delete_device_member(self, context, id, device_id=None):
         LOG.debug("Delete lbaas device member, device_id: {}, id: {}"
                   .format(device_id, id))
         self.inventory_db.delete_member(context, id)
```

### Comparing `f5-openstack-lbaasv2-inventory-1.0.1/neutron_lbaas_inventory/extensions/lbaasdevice.py` & `f5-openstack-lbaasv2-inventory-1.1.0/neutron_lbaas_inventory/extensions/lbaasdevice.py`

 * *Files 1% similar despite different names*

```diff
@@ -218,9 +218,9 @@
         pass
 
     @abc.abstractmethod
     def update_device_member(self, context, id, device_id, member):
         pass
 
     @abc.abstractmethod
-    def delete_device_member(self, context, id, device_id):
+    def delete_device_member(self, context, id, device_id=None):
         pass
```

### Comparing `f5-openstack-lbaasv2-inventory-1.0.1/neutron_lbaas_inventory/db/models/inventory.py` & `f5-openstack-lbaasv2-inventory-1.1.0/neutron_lbaas_inventory/db/models/inventory.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,12 +23,12 @@
 
     __tablename__ = "lbaas_device_members"
 
     device_id = sa.Column(sa.String(36),
                           sa.ForeignKey("lbaas_devices.id"),
                           nullable=False)
     type = sa.Column(sa.String(16), nullable=False)
-    mgmt_ipv4 = sa.Column(sa.String(255), nullable=False)
+    mgmt_ipv4 = sa.Column(sa.String(255), nullable=True)
     mgmt_ipv6 = sa.Column(sa.String(255), nullable=True)
     device_info = sa.Column(sa.String(4095), nullable=False)
     operating_status = sa.Column(sa.String(255), nullable=True)
     last_error = sa.Column(sa.String(4095), nullable=True)
```

### Comparing `f5-openstack-lbaasv2-inventory-1.0.1/neutron_lbaas_inventory/db/migration/alembic_migrations/inventory_init_ops.py` & `f5-openstack-lbaasv2-inventory-1.1.0/neutron_lbaas_inventory/db/migration/alembic_migrations/inventory_init_ops.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     )
 
     op.create_table(
         u'lbaas_device_members',
         sa.Column(u'id', sa.String(36), nullable=False),
         sa.Column(u'device_id', sa.String(36), nullable=False),
         sa.Column(u'type', sa.String(16), nullable=False),
-        sa.Column(u'mgmt_ipv4', sa.String(255), nullable=False),
+        sa.Column(u'mgmt_ipv4', sa.String(255), nullable=True),
         sa.Column(u'mgmt_ipv6', sa.String(255), nullable=True),
         sa.Column(u'device_info', sa.String(4095), nullable=False),
         sa.Column(u'operating_status', sa.String(255), nullable=True),
         sa.Column(u'last_error', sa.String(4095), nullable=True),
         sa.PrimaryKeyConstraint(u'id'),
         sa.ForeignKeyConstraint([u'device_id'], [u'lbaas_devices.id']),
     )
```

### Comparing `f5-openstack-lbaasv2-inventory-1.0.1/neutron_lbaas_inventory/db/migration/alembic_migrations/env.py` & `f5-openstack-lbaasv2-inventory-1.1.0/neutron_lbaas_inventory/db/migration/alembic_migrations/env.py`

 * *Files identical despite different names*

### Comparing `f5-openstack-lbaasv2-inventory-1.0.1/neutron_lbaas_inventory/db/inventory_db.py` & `f5-openstack-lbaasv2-inventory-1.1.0/neutron_lbaas_inventory/db/inventory_db.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,17 +75,15 @@
         device = self._device_dict(self._get_device(context, id))
         return self._populate_member_info(context, device, id)
 
     @db_api.retry_if_session_inactive()
     def update_device(self, context, id, payload):
         json_keys = [
             "provisioning_status",
-            "operating_status",
             "device_info",
-            "last_error"
         ]
         device = payload["device"]
         for key in json_keys:
             if key in device:
                 device[key] = jsonutils.dumps(device[key])
 
         with context.session.begin(subtransactions=True):
@@ -127,15 +125,15 @@
         ]
 
         device = dict((k, device_db[k])
                       for k in device_db.keys() if k not in json_keys)
         for k in json_keys:
             device[k] = self._get_dict(device_db, k)
 
-        return db_utils.resource_fields(device, fields)
+        return device
 
     def _get_dict(self, device_db, dict_name, ignore_missing=False):
         json_string = None
         try:
             json_string = getattr(device_db, dict_name)
             json_dict = jsonutils.loads(json_string)
         except Exception:
@@ -178,15 +176,15 @@
         member = payload["member"]
 
         with db_api.context_manager.writer.using(context):
             args = {
                 "id": uuidutils.generate_uuid(),
                 "device_id": device_id,
                 "type": member["type"],
-                "mgmt_ipv4": member["mgmt_ipv4"],
+                "mgmt_ipv4": member.get("mgmt_ipv4"),
                 "mgmt_ipv6": member.get("mgmt_ipv6"),
                 "device_info": jsonutils.dumps(member["device_info"]),
                 "operating_status": jsonutils.dumps(
                     member["operating_status"]),
                 "last_error": jsonutils.dumps({})
             }
             member_db = models.DeviceMember(**args)
```

### Comparing `f5-openstack-lbaasv2-inventory-1.0.1/setup.py` & `f5-openstack-lbaasv2-inventory-1.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `f5-openstack-lbaasv2-inventory-1.0.1/f5_openstack_lbaasv2_inventory.egg-info/PKG-INFO` & `f5-openstack-lbaasv2-inventory-1.1.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: f5-openstack-lbaasv2-inventory
-Version: 1.0.1
+Version: 1.1.0
 Summary: F5 Networks device inventory for OpenStack services
 Home-page: UNKNOWN
 Author: F5 Networks
 Author-email: openstack@f5.com
 License: Apache License, Version 2.0
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `f5-openstack-lbaasv2-inventory-1.0.1/f5_openstack_lbaasv2_inventory.egg-info/SOURCES.txt` & `f5-openstack-lbaasv2-inventory-1.1.0/f5_openstack_lbaasv2_inventory.egg-info/SOURCES.txt`

 * *Files identical despite different names*

