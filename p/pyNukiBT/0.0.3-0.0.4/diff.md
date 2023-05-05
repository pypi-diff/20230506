# Comparing `tmp/pynukibt-0.0.3.tar.gz` & `tmp/pynukibt-0.0.4.tar.gz`

## Comparing `pynukibt-0.0.3.tar` & `pynukibt-0.0.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 pynukibt-0.0.3/requirements.txt
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 pynukibt-0.0.3/setup.py
--rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pynukibt-0.0.3/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 pynukibt-0.0.3/pyNukiBT/__init__.py
--rw-r--r--   0        0        0    39005 2020-02-02 00:00:00.000000 pynukibt-0.0.3/pyNukiBT/const.py
--rw-r--r--   0        0        0    24671 2020-02-02 00:00:00.000000 pynukibt-0.0.3/pyNukiBT/nuki.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pynukibt-0.0.3/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 pynukibt-0.0.3/LICENSE
--rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 pynukibt-0.0.3/README.md
--rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 pynukibt-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     2005 2020-02-02 00:00:00.000000 pynukibt-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 pynukibt-0.0.4/requirements.txt
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 pynukibt-0.0.4/setup.py
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pynukibt-0.0.4/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 pynukibt-0.0.4/pyNukiBT/__init__.py
+-rw-r--r--   0        0        0    39005 2020-02-02 00:00:00.000000 pynukibt-0.0.4/pyNukiBT/const.py
+-rw-r--r--   0        0        0    24728 2020-02-02 00:00:00.000000 pynukibt-0.0.4/pyNukiBT/nuki.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pynukibt-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 pynukibt-0.0.4/LICENSE
+-rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 pynukibt-0.0.4/README.md
+-rw-r--r--   0        0        0      658 2020-02-02 00:00:00.000000 pynukibt-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2005 2020-02-02 00:00:00.000000 pynukibt-0.0.4/PKG-INFO
```

### Comparing `pynukibt-0.0.3/setup.py` & `pynukibt-0.0.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="pyNukiBT",
-    version="0.0.3",
+    version="0.0.4",
     author="Ronen Gruengras",
     author_email="ronengr@gmail.com",
     description="Nuki Bluetooth API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/ronengr/pyNukiBT",
     packages=find_packages(),
```

### Comparing `pynukibt-0.0.3/.github/workflows/python-publish.yml` & `pynukibt-0.0.4/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `pynukibt-0.0.3/pyNukiBT/const.py` & `pynukibt-0.0.4/pyNukiBT/const.py`

 * *Files identical despite different names*

### Comparing `pynukibt-0.0.3/pyNukiBT/nuki.py` & `pynukibt-0.0.4/pyNukiBT/nuki.py`

 * *Files 0% similar despite different names*

```diff
@@ -304,14 +304,15 @@
                 != msg.payload["config_update_count"]
             )
             self.last_state = msg.payload
             logger.debug(f"State: {self.last_state}")
             if update_config:
                 # todo: update config directly?
                 self.poll_needed = True
+            self._fire_callbacks()
 
         elif msg.command == self._const.NukiCommand.STATUS:
             logger.info(f"Last action: {msg.payload.status}")
 
         else:
             logger.error("%s: Received unsolicited notification: %s", self._name, msg)
             logger.error("was expecting %s", self._expected_response)
@@ -430,15 +431,14 @@
                 != msg["config_update_count"]
             )
             self.last_state = msg
             logger.debug(f"State: {self.last_state}")
             self._poll_needed = False
         if update_config:
             await self.update_config()
-        self._fire_callbacks()
 
     async def lock(self):
         return await self.lock_action(
             self._const.LockAction.LOCK, self._const.LockState.LOCKING
         )
 
     async def unlock(self):
@@ -578,24 +578,24 @@
             except NukiErrorException as ex:
                 if ex.error_code == self._const.ErrorCode.K_ERROR_BAD_PIN:
                     return False
                 else:
                     raise
             return msg.status == self._const.StatusCode.COMPLETED
 
-    async def request_log_entry(self, security_pin, sort_order=0x01, count=1):
-        logger.info(f"request last log entry")
+    async def request_log_entries(self, security_pin, sort_order=0x01, count=1, start_index=0):
+        logger.info(f"request {count} log entries, start={start_index}")
         async with self._operation_lock:
             msg = await self._send_encrtypted_command(
                 self._const.NukiCommand.REQUEST_DATA,
                 {"command": self._const.NukiCommand.CHALLENGE},
                 expected_response=self._const.NukiCommand.CHALLENGE,
             )
             payload = {
-                "start_index": 0,
+                "start_index": start_index,
                 "count": count,
                 "sort_order": sort_order,
                 "total_count": 0,
                 "nonce": msg.nonce,
                 "security_pin": security_pin,
             }
             msg = await self._send_encrtypted_command(
```

### Comparing `pynukibt-0.0.3/.gitignore` & `pynukibt-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `pynukibt-0.0.3/LICENSE` & `pynukibt-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pynukibt-0.0.3/README.md` & `pynukibt-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pynukibt-0.0.3/pyproject.toml` & `pynukibt-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pyNukiBT"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Ronen Gruengras", email="ronengr@gmail.com" },
 ]
 description = "Nuki Bluetooth API"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `pynukibt-0.0.3/PKG-INFO` & `pynukibt-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyNukiBT
-Version: 0.0.3
+Version: 0.0.4
 Summary: Nuki Bluetooth API
 Project-URL: Homepage, https://github.com/ronengr/pyNukiBT
 Project-URL: Bug Tracker, https://github.com/ronengr/pyNukiBT/issues
 Author-email: Ronen Gruengras <ronengr@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

