# Comparing `tmp/Flask-Helper-2.0.3.tar.gz` & `tmp/Flask-Helper-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\Flask-Helper-2.0.3.tar", last modified: Fri Apr 28 00:13:00 2023, max compression
+gzip compressed data, was "dist\Flask-Helper-2.0.4.tar", last modified: Sat May  6 10:04:41 2023, max compression
```

## Comparing `Flask-Helper-2.0.3.tar` & `Flask-Helper-2.0.4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-04-28 00:13:00.242320 Flask-Helper-2.0.3/
-drwxrwxrwx   0        0        0        0 2023-04-28 00:12:59.957903 Flask-Helper-2.0.3/Flask_Helper.egg-info/
--rw-rw-rw-   0        0        0      297 2023-04-28 00:12:59.000000 Flask-Helper-2.0.3/Flask_Helper.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1150 2023-04-28 00:12:59.000000 Flask-Helper-2.0.3/Flask_Helper.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-28 00:12:59.000000 Flask-Helper-2.0.3/Flask_Helper.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-04-28 00:12:59.000000 Flask-Helper-2.0.3/Flask_Helper.egg-info/requires.txt
--rw-rw-rw-   0        0        0       51 2023-04-28 00:12:59.000000 Flask-Helper-2.0.3/Flask_Helper.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      297 2023-04-28 00:13:00.242320 Flask-Helper-2.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      920 2023-04-28 00:12:17.000000 Flask-Helper-2.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-28 00:13:00.097074 Flask-Helper-2.0.3/flask_helper/
--rw-rw-rw-   0        0        0      260 2023-03-29 02:48:52.000000 Flask-Helper-2.0.3/flask_helper/__init__.py
--rw-rw-rw-   0        0        0     5592 2021-03-06 08:22:26.000000 Flask-Helper-2.0.3/flask_helper/_flask.py
--rw-rw-rw-   0        0        0      323 2020-06-16 06:22:00.000000 Flask-Helper-2.0.3/flask_helper/ctx.py
--rw-rw-rw-   0        0        0     1014 2020-09-16 00:12:06.000000 Flask-Helper-2.0.3/flask_helper/exception.py
--rw-rw-rw-   0        0        0     4756 2023-04-10 10:54:48.000000 Flask-Helper-2.0.3/flask_helper/flask2.py
--rw-rw-rw-   0        0        0      478 2020-09-15 10:53:03.000000 Flask-Helper-2.0.3/flask_helper/flask_hook.py
-drwxrwxrwx   0        0        0        0 2023-04-28 00:13:00.162228 Flask-Helper-2.0.3/flask_helper/hooks/
--rw-rw-rw-   0        0        0       72 2020-06-16 06:47:11.000000 Flask-Helper-2.0.3/flask_helper/hooks/__init__.py
--rw-rw-rw-   0        0        0      693 2020-06-16 08:35:29.000000 Flask-Helper-2.0.3/flask_helper/hooks/cors_hook.py
--rw-rw-rw-   0        0        0     1028 2020-06-16 08:36:48.000000 Flask-Helper-2.0.3/flask_helper/hooks/handle_30x_hook.py
--rw-rw-rw-   0        0        0     1285 2021-04-07 00:23:23.000000 Flask-Helper-2.0.3/flask_helper/hooks/real_ip_hook.py
--rw-rw-rw-   0        0        0     1827 2021-03-10 08:03:58.000000 Flask-Helper-2.0.3/flask_helper/hooks/user_agent_hook.py
--rw-rw-rw-   0        0        0     2129 2023-04-28 00:10:28.000000 Flask-Helper-2.0.3/flask_helper/sessions.py
--rw-rw-rw-   0        0        0      558 2020-06-16 06:22:00.000000 Flask-Helper-2.0.3/flask_helper/template.py
--rw-rw-rw-   0        0        0     3739 2020-06-19 00:00:52.000000 Flask-Helper-2.0.3/flask_helper/upload.py
--rw-rw-rw-   0        0        0     1346 2020-06-16 06:22:00.000000 Flask-Helper-2.0.3/flask_helper/url_rule.py
-drwxrwxrwx   0        0        0        0 2023-04-28 00:13:00.235334 Flask-Helper-2.0.3/flask_helper/utils/
--rw-rw-rw-   0        0        0       72 2020-06-17 02:26:04.000000 Flask-Helper-2.0.3/flask_helper/utils/__init__.py
--rw-rw-rw-   0        0        0      522 2020-06-16 06:22:00.000000 Flask-Helper-2.0.3/flask_helper/utils/folder.py
--rw-rw-rw-   0        0        0     1240 2020-06-16 06:22:00.000000 Flask-Helper-2.0.3/flask_helper/utils/ip.py
--rw-rw-rw-   0        0        0     3167 2020-07-03 00:18:51.000000 Flask-Helper-2.0.3/flask_helper/utils/loader.py
--rw-rw-rw-   0        0        0     1493 2021-12-13 03:19:57.000000 Flask-Helper-2.0.3/flask_helper/utils/log.py
--rw-rw-rw-   0        0        0     4304 2021-04-30 02:14:59.000000 Flask-Helper-2.0.3/flask_helper/utils/registry.py
--rw-rw-rw-   0        0        0     1190 2021-04-04 02:42:29.000000 Flask-Helper-2.0.3/flask_helper/view.py
--rw-rw-rw-   0        0        0       42 2023-04-28 00:13:00.243281 Flask-Helper-2.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1094 2023-04-28 00:11:14.000000 Flask-Helper-2.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-06 10:04:41.796387 Flask-Helper-2.0.4/
+drwxrwxrwx   0        0        0        0 2023-05-06 10:04:41.287502 Flask-Helper-2.0.4/Flask_Helper.egg-info/
+-rw-rw-rw-   0        0        0      297 2023-05-06 10:04:40.000000 Flask-Helper-2.0.4/Flask_Helper.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1150 2023-05-06 10:04:40.000000 Flask-Helper-2.0.4/Flask_Helper.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-06 10:04:40.000000 Flask-Helper-2.0.4/Flask_Helper.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-05-06 10:04:40.000000 Flask-Helper-2.0.4/Flask_Helper.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       51 2023-05-06 10:04:40.000000 Flask-Helper-2.0.4/Flask_Helper.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      297 2023-05-06 10:04:41.795389 Flask-Helper-2.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      952 2023-05-06 10:03:51.000000 Flask-Helper-2.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-06 10:04:41.543128 Flask-Helper-2.0.4/flask_helper/
+-rw-rw-rw-   0        0        0      260 2023-03-29 02:48:52.000000 Flask-Helper-2.0.4/flask_helper/__init__.py
+-rw-rw-rw-   0        0        0     5592 2021-03-06 08:22:26.000000 Flask-Helper-2.0.4/flask_helper/_flask.py
+-rw-rw-rw-   0        0        0      323 2020-06-16 06:22:00.000000 Flask-Helper-2.0.4/flask_helper/ctx.py
+-rw-rw-rw-   0        0        0     1014 2020-09-16 00:12:06.000000 Flask-Helper-2.0.4/flask_helper/exception.py
+-rw-rw-rw-   0        0        0     4207 2023-05-06 10:02:23.000000 Flask-Helper-2.0.4/flask_helper/flask2.py
+-rw-rw-rw-   0        0        0      478 2020-09-15 10:53:03.000000 Flask-Helper-2.0.4/flask_helper/flask_hook.py
+drwxrwxrwx   0        0        0        0 2023-05-06 10:04:41.648106 Flask-Helper-2.0.4/flask_helper/hooks/
+-rw-rw-rw-   0        0        0       72 2020-06-16 06:47:11.000000 Flask-Helper-2.0.4/flask_helper/hooks/__init__.py
+-rw-rw-rw-   0        0        0      693 2020-06-16 08:35:29.000000 Flask-Helper-2.0.4/flask_helper/hooks/cors_hook.py
+-rw-rw-rw-   0        0        0     1028 2020-06-16 08:36:48.000000 Flask-Helper-2.0.4/flask_helper/hooks/handle_30x_hook.py
+-rw-rw-rw-   0        0        0     1285 2021-04-07 00:23:23.000000 Flask-Helper-2.0.4/flask_helper/hooks/real_ip_hook.py
+-rw-rw-rw-   0        0        0     1827 2021-03-10 08:03:58.000000 Flask-Helper-2.0.4/flask_helper/hooks/user_agent_hook.py
+-rw-rw-rw-   0        0        0     2129 2023-04-28 00:10:28.000000 Flask-Helper-2.0.4/flask_helper/sessions.py
+-rw-rw-rw-   0        0        0      558 2020-06-16 06:22:00.000000 Flask-Helper-2.0.4/flask_helper/template.py
+-rw-rw-rw-   0        0        0     3739 2020-06-19 00:00:52.000000 Flask-Helper-2.0.4/flask_helper/upload.py
+-rw-rw-rw-   0        0        0     1346 2020-06-16 06:22:00.000000 Flask-Helper-2.0.4/flask_helper/url_rule.py
+drwxrwxrwx   0        0        0        0 2023-05-06 10:04:41.781311 Flask-Helper-2.0.4/flask_helper/utils/
+-rw-rw-rw-   0        0        0       72 2020-06-17 02:26:04.000000 Flask-Helper-2.0.4/flask_helper/utils/__init__.py
+-rw-rw-rw-   0        0        0      522 2020-06-16 06:22:00.000000 Flask-Helper-2.0.4/flask_helper/utils/folder.py
+-rw-rw-rw-   0        0        0     1240 2020-06-16 06:22:00.000000 Flask-Helper-2.0.4/flask_helper/utils/ip.py
+-rw-rw-rw-   0        0        0     3167 2020-07-03 00:18:51.000000 Flask-Helper-2.0.4/flask_helper/utils/loader.py
+-rw-rw-rw-   0        0        0     1493 2021-12-13 03:19:57.000000 Flask-Helper-2.0.4/flask_helper/utils/log.py
+-rw-rw-rw-   0        0        0     4304 2021-04-30 02:14:59.000000 Flask-Helper-2.0.4/flask_helper/utils/registry.py
+-rw-rw-rw-   0        0        0     1190 2021-04-04 02:42:29.000000 Flask-Helper-2.0.4/flask_helper/view.py
+-rw-rw-rw-   0        0        0       42 2023-05-06 10:04:41.797397 Flask-Helper-2.0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1094 2023-05-06 10:03:51.000000 Flask-Helper-2.0.4/setup.py
```

### Comparing `Flask-Helper-2.0.3/Flask_Helper.egg-info/SOURCES.txt` & `Flask-Helper-2.0.4/Flask_Helper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Flask-Helper-2.0.3/README.md` & `Flask-Helper-2.0.4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 # Flask-Heler
 
+## 2.0.4
+删除_packet_data
+
 ## 2.0.3
 修复
 'Flask2' object has no attribute 'session_cookie_name'
 
 ## 2.0.2
 修复
 TypeError: send_file() got an unexpected keyword argument 'cache_timeout'
```

### Comparing `Flask-Helper-2.0.3/flask_helper/_flask.py` & `Flask-Helper-2.0.4/flask_helper/_flask.py`

 * *Files identical despite different names*

### Comparing `Flask-Helper-2.0.3/flask_helper/exception.py` & `Flask-Helper-2.0.4/flask_helper/exception.py`

 * *Files identical despite different names*

### Comparing `Flask-Helper-2.0.3/flask_helper/flask2.py` & `Flask-Helper-2.0.4/flask_helper/flask2.py`

 * *Files 8% similar despite different names*

```diff
@@ -79,38 +79,23 @@
 
     session_interface = SecureCookieSessionInterface2()
 
     @staticmethod
     def _assign_default_g():
         pass
 
-    @staticmethod
-    def _packet_data():
-        # if request.method == "OPTIONS":
-        #     return make_response("success", 204)
-        if request.method != "GET":
-            if request.json is None:
-                g.request_data = {}
-            else:
-                g.request_data = request.json
-            if type(g.request_data) != dict:
-                return make_response("访问受限", 400)
-        else:
-            g.request_args = request.args
-
     def ping_func(self):
         ping_msg = "Ping %s success. App run at %s" % (request.path, self.run_time)
         return jsonify({"status": self.config.get("MSG_STATUS", 2), "message": ping_msg})
 
     def __init__(self, import_name, **kwargs):
         self.blues = []
         super(Flask2, self).__init__(import_name, **kwargs)
         self.add_url_rule("/ping/", endpoint="app_ping", view_func=self.ping_func)
         self.before_request_funcs.setdefault(None, []).append(self._assign_default_g)
-        self.before_request_funcs[None].append(self._packet_data)
         self.after_authorization_funcs = []
         self.extend_functions = dict()
 
     def register_blues(self):
         self.log.warning('register_blues is about to be abandoned')
         for blue_item in self.blues:
             if hasattr(blue_item, "static_routes") is True:
```

### Comparing `Flask-Helper-2.0.3/flask_helper/hooks/cors_hook.py` & `Flask-Helper-2.0.4/flask_helper/hooks/cors_hook.py`

 * *Files identical despite different names*

### Comparing `Flask-Helper-2.0.3/flask_helper/hooks/handle_30x_hook.py` & `Flask-Helper-2.0.4/flask_helper/hooks/handle_30x_hook.py`

 * *Files identical despite different names*

### Comparing `Flask-Helper-2.0.3/flask_helper/hooks/real_ip_hook.py` & `Flask-Helper-2.0.4/flask_helper/hooks/real_ip_hook.py`

 * *Files identical despite different names*

### Comparing `Flask-Helper-2.0.3/flask_helper/hooks/user_agent_hook.py` & `Flask-Helper-2.0.4/flask_helper/hooks/user_agent_hook.py`

 * *Files identical despite different names*

### Comparing `Flask-Helper-2.0.3/flask_helper/sessions.py` & `Flask-Helper-2.0.4/flask_helper/sessions.py`

 * *Files identical despite different names*

### Comparing `Flask-Helper-2.0.3/flask_helper/template.py` & `Flask-Helper-2.0.4/flask_helper/template.py`

 * *Files identical despite different names*

### Comparing `Flask-Helper-2.0.3/flask_helper/upload.py` & `Flask-Helper-2.0.4/flask_helper/upload.py`

 * *Files identical despite different names*

### Comparing `Flask-Helper-2.0.3/flask_helper/url_rule.py` & `Flask-Helper-2.0.4/flask_helper/url_rule.py`

 * *Files identical despite different names*

### Comparing `Flask-Helper-2.0.3/flask_helper/utils/folder.py` & `Flask-Helper-2.0.4/flask_helper/utils/folder.py`

 * *Files identical despite different names*

### Comparing `Flask-Helper-2.0.3/flask_helper/utils/ip.py` & `Flask-Helper-2.0.4/flask_helper/utils/ip.py`

 * *Files identical despite different names*

### Comparing `Flask-Helper-2.0.3/flask_helper/utils/loader.py` & `Flask-Helper-2.0.4/flask_helper/utils/loader.py`

 * *Files identical despite different names*

### Comparing `Flask-Helper-2.0.3/flask_helper/utils/log.py` & `Flask-Helper-2.0.4/flask_helper/utils/log.py`

 * *Files identical despite different names*

### Comparing `Flask-Helper-2.0.3/flask_helper/utils/registry.py` & `Flask-Helper-2.0.4/flask_helper/utils/registry.py`

 * *Files identical despite different names*

### Comparing `Flask-Helper-2.0.3/flask_helper/view.py` & `Flask-Helper-2.0.4/flask_helper/view.py`

 * *Files identical despite different names*

### Comparing `Flask-Helper-2.0.3/setup.py` & `Flask-Helper-2.0.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 
 if sys.version_info <= (3, 7):
     sys.stderr.write("ERROR: flask_helper requires Python Version 3.7 or above.\n")
     sys.stderr.write("Your Python Version is %s.%s.%s.\n" % sys.version_info[:3])
     sys.exit(1)
 
 name = "Flask-Helper"
-version = "2.0.3"
+version = "2.0.4"
 url = "https://github.com/meisanggou/Flask-Helper"
 license = "MIT"
 author = "meisanggou"
 short_description = "Flask Helper"
 long_description = """Some Tools For Help You Use Flask"""
 keywords = "flask_helper"
 install_requires = ["Flask"]
```

