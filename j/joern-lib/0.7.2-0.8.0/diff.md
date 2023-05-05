# Comparing `tmp/joern_lib-0.7.2.tar.gz` & `tmp/joern_lib-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "joern_lib-0.7.2.tar", max compression
+gzip compressed data, was "joern_lib-0.8.0.tar", max compression
```

## Comparing `joern_lib-0.7.2.tar` & `joern_lib-0.8.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11357 2023-04-02 22:16:36.336281 joern_lib-0.7.2/LICENSE
--rw-r--r--   0        0        0     3722 2023-05-04 20:26:07.824853 joern_lib-0.7.2/README.md
--rw-r--r--   0        0        0       86 2023-05-04 21:19:10.842784 joern_lib-0.7.2/joern_lib/__init__.py
--rw-r--r--   0        0        0     9514 2023-05-04 23:50:46.832580 joern_lib-0.7.2/joern_lib/client.py
--rw-r--r--   0        0        0       61 2023-05-04 21:19:10.842784 joern_lib-0.7.2/joern_lib/detectors/__init__.py
--rw-r--r--   0        0        0      627 2023-04-28 20:22:02.075618 joern_lib-0.7.2/joern_lib/detectors/c.py
--rw-r--r--   0        0        0     8445 2023-05-04 23:14:53.536043 joern_lib-0.7.2/joern_lib/detectors/common.py
--rw-r--r--   0        0        0     2814 2023-05-04 20:09:52.512192 joern_lib-0.7.2/joern_lib/detectors/java.py
--rw-r--r--   0        0        0     3914 2023-04-02 22:16:36.347281 joern_lib-0.7.2/joern_lib/detectors/js.py
--rw-r--r--   0        0        0    11061 2023-05-04 22:05:54.090370 joern_lib-0.7.2/joern_lib/utils.py
--rw-r--r--   0        0        0     4535 2023-04-28 20:22:02.075618 joern_lib-0.7.2/joern_lib/workspace.py
--rw-r--r--   0        0        0     1206 2023-05-05 00:13:27.557001 joern_lib-0.7.2/pyproject.toml
--rw-r--r--   0        0        0     5068 1970-01-01 00:00:00.000000 joern_lib-0.7.2/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-05 22:17:31.777335 joern_lib-0.8.0/LICENSE
+-rw-r--r--   0        0        0     3909 2023-05-05 22:17:31.777335 joern_lib-0.8.0/README.md
+-rw-r--r--   0        0        0       86 2023-05-05 22:17:31.805335 joern_lib-0.8.0/joern_lib/__init__.py
+-rw-r--r--   0        0        0    11860 2023-05-05 22:17:31.805335 joern_lib-0.8.0/joern_lib/client.py
+-rw-r--r--   0        0        0       61 2023-05-05 22:17:31.805335 joern_lib-0.8.0/joern_lib/detectors/__init__.py
+-rw-r--r--   0        0        0      627 2023-05-05 22:17:31.805335 joern_lib-0.8.0/joern_lib/detectors/c.py
+-rw-r--r--   0        0        0     9096 2023-05-05 22:17:31.805335 joern_lib-0.8.0/joern_lib/detectors/common.py
+-rw-r--r--   0        0        0     2841 2023-05-05 22:17:31.805335 joern_lib-0.8.0/joern_lib/detectors/java.py
+-rw-r--r--   0        0        0     3914 2023-05-05 22:17:31.805335 joern_lib-0.8.0/joern_lib/detectors/js.py
+-rw-r--r--   0        0        0    12485 2023-05-05 22:17:31.805335 joern_lib-0.8.0/joern_lib/utils.py
+-rw-r--r--   0        0        0     4535 2023-05-05 22:17:31.809336 joern_lib-0.8.0/joern_lib/workspace.py
+-rw-r--r--   0        0        0     1206 2023-05-05 22:17:31.809336 joern_lib-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0     5255 1970-01-01 00:00:00.000000 joern_lib-0.8.0/PKG-INFO
```

### Comparing `joern_lib-0.7.2/LICENSE` & `joern_lib-0.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `joern_lib-0.7.2/README.md` & `joern_lib-0.8.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -189,7 +189,16 @@
 
 If Joern server stops responding after a while restart docker.
 
 ```
 docker compose down
 docker compose up -d
 ```
+
+### Websockets connection closed error
+
+Adding asyncio.sleep(0) seems to fix such errors.
+
+```
+# Workaround to fix websockets.exceptions.ConnectionClosedError
+await asyncio.sleep(0)
+```
```

### Comparing `joern_lib-0.7.2/joern_lib/client.py` & `joern_lib-0.8.0/joern_lib/client.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,15 +5,21 @@
 import orjson
 import uvloop
 
 asyncio.set_event_loop_policy(uvloop.EventLoopPolicy())
 
 import websockets
 
-from joern_lib.utils import print_flows, print_md, print_table
+from joern_lib.utils import (
+    check_labels_list,
+    expand_search_str,
+    print_flows,
+    print_md,
+    print_table,
+)
 
 headers = {"Content-Type": "application/json", "Accept-Encoding": "gzip"}
 CLIENT_TIMEOUT = os.getenv("HTTP_CLIENT_TIMEOUT")
 
 
 class Connection:
     """
@@ -63,14 +69,16 @@
     ws_url = f"""{base_url.replace("http://", "ws://").replace("https://", "wss://")}/connect"""
     websocket = await websockets.connect(ws_url, ping_timeout=None)
     connected_msg = await websocket.recv()
     if connected_msg != "connected":
         raise websockets.exceptions.InvalidState(
             "Didn't receive connected message from Joern server"
         )
+    # Workaround to fix websockets.exceptions.ConnectionClosedError
+    await asyncio.sleep(0)
     return Connection(cpggenclient, client, websocket)
 
 
 async def send(connection, message):
     """Send message to the joern server via websocket"""
     await connection.websocket.send(message)
 
@@ -156,26 +164,29 @@
     client = connection.httpclient
     response = await client.post(
         url="/query", headers=headers, json={"query": fix_query(query_str)}
     )
     if response.status_code == httpx.codes.OK:
         j = response.json()
         res_uuid = j.get("uuid")
-        completed_uuid = await receive(connection)
-        if completed_uuid == res_uuid:
-            response = await client.get(
-                url=f"/result/{completed_uuid}", headers=headers
-            )
-            if response.status_code == httpx.codes.OK:
-                j = response.json()
-                sout = j.get("stdout", "")
-                serr = j.get("stderr", "")
-                if sout:
-                    return fix_json(sout)
-                return parse_error(serr)
+        try:
+            completed_uuid = await receive(connection)
+            if completed_uuid == res_uuid:
+                response = await client.get(
+                    url=f"/result/{completed_uuid}", headers=headers
+                )
+                if response.status_code == httpx.codes.OK:
+                    j = response.json()
+                    sout = j.get("stdout", "")
+                    serr = j.get("stderr", "")
+                    if sout:
+                        return fix_json(sout)
+                    return parse_error(serr)
+        except Exception:
+            return None
     return None
 
 
 async def bulk_query(connection, query_list):
     """Bulk query joern server"""
     client = connection.httpclient
     websocket = connection.websocket
@@ -237,32 +248,66 @@
 
 
 async def df(
     connection,
     source,
     sink,
     print_result=True if os.getenv("POLYNOTE_VERSION") else False,
+    filter=None,
+    check_labels=check_labels_list,
 ):
-    """Execute reachableByFlows query"""
+    """
+    Execute reachableByFlows query. Optionally accepts filters which could be a raw conditional string or predefined keywords such as skip_control_structures, skip_cfg and skip_checks
+    skip_control_structures: This adds a control structure filter `filter(m => m.elements.isControlStructure.size > 0)` to skip flows with control statements such if condition or break
+    skip_cfg: This adds a cfg filter `filter(m => m.elements.isCfgNode.size > 0)` to skip flows with control flow graph nodes
+    skip_checks: When used with check_labels parameter, this could filter flows containing known validation and sanitization code in the flow. Has a default list.
+    """
+    filter_str = ""
+    if isinstance(check_labels, str):
+        check_labels = check_labels.split("|")
     if isinstance(source, dict):
         for k, v in source.items():
-            source = f"""cpg.tag.name("{v}").{k}"""
+            if k in ("parameter", "tag"):
+                source = f"""cpg.tag.name("{v}").{k}"""
+            elif k in ("method", "call", "annotation"):
+                source = f"""cpg.{k}{expand_search_str(v)}"""
     if isinstance(sink, dict):
         for k, v in sink.items():
-            sink = f"""cpg.tag.name("{v}").{k}"""
+            if k in ("parameter", "tag"):
+                sink = f"""cpg.tag.name("{v}").{k}"""
+            elif k in ("method", "call", "annotation"):
+                sink = f"""cpg.{k}{expand_search_str(v)}"""
     if not source.startswith("def"):
         source = f"def source = {source}"
     if not sink.startswith("def"):
         sink = f"def sink = {sink}"
+    if filter:
+        if isinstance(filter, str):
+            if filter == "skip_checks":
+                filter_str = f""".filter(m => m.elements.code(".*({'|'.join(check_labels)}).*").size == 0)"""
+            elif not filter.startswith("."):
+                filter_str = f".filter({filter})"
+        elif isinstance(filter, list):
+            for k in filter:
+                if k == "skip_control_structures":
+                    filter_str = f"{filter_str}.filter(m => m.elements.isControlStructure.size > 0)"
+                elif k == "skip_cfg":
+                    filter_str = (
+                        f"{filter_str}.filter(m => m.elements.isCfgNode.size > 0)"
+                    )
+                elif k == "skip_checks":
+                    filter_str = f"""{filter_str}.filter(m => m.elements.code(".*({'|'.join(check_labels)}).*").size == 0)"""
+                else:
+                    filter_str = f"""{filter_str}.filter({k})"""
     results = await query(
         connection,
         f"""
         {source}
         {sink}
-        sink.reachableByFlows(source).map(m => (m, m.elements.location.l)).toJson
+        sink.reachableByFlows(source){filter_str}.map(m => (m, m.elements.location.l)).toJson
         """,
     )
     if print_result:
         print_flows(results)
     return results
```

### Comparing `joern_lib-0.7.2/joern_lib/detectors/c.py` & `joern_lib-0.8.0/joern_lib/detectors/c.py`

 * *Files identical despite different names*

### Comparing `joern_lib-0.7.2/joern_lib/detectors/common.py` & `joern_lib-0.8.0/joern_lib/detectors/common.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,31 @@
 from joern_lib import client
+from joern_lib.utils import expand_search_str
 
 
-async def list_files(connection):
-    return await client.q(connection, "cpg.file")
+async def list_files(connection, search_descriptor=None):
+    search_str = expand_search_str(search_descriptor)
+    return await client.q(connection, f"cpg.file{search_str}")
 
 
 async def list_annotations(connection):
     return await client.q(connection, "cpg.annotation")
 
 
 async def list_arguments(connection):
     return await client.q(connection, "cpg.argument")
 
 
 async def list_assignments(connection):
     return await client.q(connection, "cpg.assignment")
 
 
-async def list_calls(connection):
-    return await client.q(connection, "cpg.call")
+async def list_calls(connection, search_descriptor=None):
+    search_str = expand_search_str(search_descriptor)
+    return await client.q(connection, f"cpg.call{search_str}")
 
 
 async def list_config_files(connection):
     return await client.q(connection, "cpg.configFile")
 
 
 async def list_control_structures(connection):
@@ -64,18 +67,21 @@
     return await client.q(connection, "cpg.member")
 
 
 async def list_metadatas(connection):
     return await client.q(connection, "cpg.metaData")
 
 
-async def list_methods(connection):
-    return await client.q(
-        connection, """cpg.method.whereNot(_.name(".*<operator>.*"))"""
-    )
+async def list_methods(connection, search_descriptor=None, skip_operators=True):
+    search_str = expand_search_str(search_descriptor)
+    filter_str = ""
+    if skip_operators:
+        filter_str = '.whereNot(_.name(".*<operator>.*"))'
+
+    return await client.q(connection, f"""cpg.method{search_str}{filter_str}""")
 
 
 async def list_constructors(connection):
     return await client.q(connection, """cpg.method.internal.name("<init>")""")
 
 
 async def list_external_methods(connection):
@@ -119,35 +125,42 @@
         return await client.q(connection, f"""cpg.tag.name("{name}"){suffix}""")
     elif value:
         return await client.q(connection, f"""cpg.tag.value("{value}"){suffix}""")
     return await client.q(connection, "cpg.tag{suffix}")
 
 
 async def create_tags(connection, query=None, call=None, method=None, tags=[]):
+    """
+    Method to create custom tags on nodes. Nodes could be selected based on a query, or call or method name.
+
+    Tags could be a list of string or dictionary of key, value pairs
+    """
     if not query and call:
         query = f"""cpg.call.name("{call}")"""
     elif not query and method:
         query = f"""cpg.method.name("{method}")"""
     if query and tags:
         for tag in tags:
             if isinstance(tag, dict):
                 for k, v in tag.items():
                     await client.q(
                         connection,
                         f"""
                         {query}.newTagNodePair("{k}", "{v}").store
                         run.commit
+                        save
                         """,
                     )
             if isinstance(tag, str):
                 await client.q(
                     connection,
                     f"""
                 {query}.newTagNode("{tag}").store
                 run.commit
+                save
                 """,
                 )
 
 
 async def list_types(connection):
     return await client.q(connection, "cpg.typ")
```

### Comparing `joern_lib-0.7.2/joern_lib/detectors/java.py` & `joern_lib-0.8.0/joern_lib/detectors/java.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 FILTER_ANNOTATIONS = "javax\\.servlet\\.annotation\\.WebFilter"
 
 
 def expand_annotations(rows):
     ret_rows = []
     for r in rows:
         m = {}
-        if not r:
+        if not r or not isinstance(r, dict):
             continue
         if r.get("_1"):
             method_data = r.get("_1")
             for k, v in method_data.items():
                 m[k] = v
         if r.get("_2"):
             annotation_list = r.get("_2")
```

### Comparing `joern_lib-0.7.2/joern_lib/detectors/js.py` & `joern_lib-0.8.0/joern_lib/detectors/js.py`

 * *Files identical despite different names*

### Comparing `joern_lib-0.7.2/joern_lib/utils.py` & `joern_lib-0.8.0/joern_lib/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import os
-
+import re
 from hashlib import blake2b
 
 from rich.console import Console
 from rich.json import JSON
 from rich.syntax import Syntax
 from rich.table import Table
 from rich.tree import Tree
@@ -179,14 +179,22 @@
                 code = (
                     loc.get("node", {})
                     .get("code", "")
                     .encode()
                     .decode("unicode_escape")
                     .strip()
                 )
+                methodFullName = loc.get("methodFullName", "").replace("<init>", "")
+                methodShortName = loc.get("methodShortName", "").replace("<init>", "")
+                class_name = loc.get("className")
+                # If there is no class name but there is a method full name try to recover
+                if not class_name and methodFullName:
+                    class_name = methodFullName.split(":")[0]
+                    if class_name.endswith("." + methodShortName):
+                        class_name = re.sub(f".{methodShortName}$", "", class_name)
                 node_name = loc.get("node", {}).get("name")
                 # Highlight potential check methods
                 if node_name and node_name in code and check_highlight_color:
                     for check_label in check_labels_list:
                         if check_label in node_name.lower():
                             code = code.replace(
                                 node_name,
@@ -212,18 +220,19 @@
                             nextfloc = (
                                 f"{nextloc.get('filename')}:{nextloc.get('lineNumber')}"
                             )
                             nextfloc_key = f"""{nextfloc}|{nextloc.get("symbol")}"""
                             if floc == nextfloc and len(floc_key) < len(nextfloc_key):
                                 continue
                     if loc.get("filename") == "<empty>":
+                        class_method_sep = "" if not methodShortName else "."
                         if symbol_highlight_color:
-                            floc = f"{loc.get('className')}.{loc.get('methodShortName')}( [{symbol_highlight_color}]{code}[/{symbol_highlight_color}] )"
+                            floc = f"{class_name}{class_method_sep}{methodShortName}( [{symbol_highlight_color}]{code}[/{symbol_highlight_color}] )"
                         else:
-                            floc = f"{loc.get('className')}.{loc.get('methodShortName')}( {code} )"
+                            floc = f"{class_name}{class_method_sep}{methodShortName}( {code} )"
                     if floc_key not in floc_list:
                         if symbol == code and last_symbol and last_symbol != code:
                             symbol = last_symbol
                         if (
                             symbol
                             and symbol_highlight_color
                             and symbol in code
@@ -260,7 +269,26 @@
                     last_symbol = symbol
         if ftree:
             flow_fingerprint_key = "-".join(flow_fingerprint_list)
             if flow_fingerprint_key not in parsed_flows_list:
                 console.print(ftree)
                 console.print("")
                 parsed_flows_list.append(flow_fingerprint_key)
+
+
+def expand_search_str(search_descriptor):
+    """Given a descriptor string or dict, this method converts into equivalent cpgql method"""
+    search_str = ""
+    if isinstance(search_descriptor, str):
+        if "." in search_descriptor:
+            if (
+                ":" in search_descriptor or "(" in search_descriptor
+            ) and ".*" not in search_descriptor:
+                search_str = f'.fullNameExact("{search_descriptor}")'
+            else:
+                search_str = f'.fullName("{search_descriptor}")'
+        else:
+            search_str = f'.name("{search_descriptor}")'
+    elif isinstance(search_descriptor, dict):
+        for k, v in search_descriptor.items():
+            search_str = f'{search_str}.{k}("{v}")'
+    return search_str
```

### Comparing `joern_lib-0.7.2/joern_lib/workspace.py` & `joern_lib-0.8.0/joern_lib/workspace.py`

 * *Files identical despite different names*

### Comparing `joern_lib-0.7.2/pyproject.toml` & `joern_lib-0.8.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "joern-lib"
-version = "0.7.2"
+version = "0.8.0"
 description = "Python library to interact with Joern server"
 authors = ["Team AppThreat <cloud@appthreat.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 packages = [{include = "joern_lib"}]
 homepage = "https://github.com/AppThreat/joern-lib"
 repository = "https://github.com/AppThreat/joern-lib"
```

### Comparing `joern_lib-0.7.2/PKG-INFO` & `joern_lib-0.8.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: joern-lib
-Version: 0.7.2
+Version: 0.8.0
 Summary: Python library to interact with Joern server
 Home-page: https://github.com/AppThreat/joern-lib
 License: Apache-2.0
 Keywords: joern,code analysis,static analysis
 Author: Team AppThreat
 Author-email: cloud@appthreat.com
 Requires-Python: >=3.7,<3.11
@@ -223,7 +223,16 @@
 If Joern server stops responding after a while restart docker.
 
 ```
 docker compose down
 docker compose up -d
 ```
 
+### Websockets connection closed error
+
+Adding asyncio.sleep(0) seems to fix such errors.
+
+```
+# Workaround to fix websockets.exceptions.ConnectionClosedError
+await asyncio.sleep(0)
+```
+
```

