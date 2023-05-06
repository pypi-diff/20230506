# Comparing `tmp/xhs-0.1.5.tar.gz` & `tmp/xhs-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xhs-0.1.5.tar", last modified: Tue Apr 25 14:08:23 2023, max compression
+gzip compressed data, was "xhs-0.1.6.tar", last modified: Sat May  6 07:52:41 2023, max compression
```

## Comparing `xhs-0.1.5.tar` & `xhs-0.1.6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:08:23.763887 xhs-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-04-25 14:08:10.000000 xhs-0.1.5/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-25 14:08:10.000000 xhs-0.1.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-25 14:08:10.000000 xhs-0.1.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-04-25 14:08:23.763887 xhs-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-04-25 14:08:10.000000 xhs-0.1.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-25 14:08:10.000000 xhs-0.1.5/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-25 14:08:23.763887 xhs-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-04-25 14:08:10.000000 xhs-0.1.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:08:23.759887 xhs-0.1.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-04-25 14:08:10.000000 xhs-0.1.5/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-04-25 14:08:10.000000 xhs-0.1.5/tests/test_help.py
--rw-r--r--   0 runner    (1001) docker     (123)     5010 2023-04-25 14:08:10.000000 xhs-0.1.5/tests/test_xhs.py
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-25 14:08:10.000000 xhs-0.1.5/tests/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:08:23.763887 xhs-0.1.5/xhs/
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-25 14:08:10.000000 xhs-0.1.5/xhs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-04-25 14:08:10.000000 xhs-0.1.5/xhs/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20212 2023-04-25 14:08:10.000000 xhs-0.1.5/xhs/core.py
--rw-r--r--   0 runner    (1001) docker     (123)       91 2023-04-25 14:08:10.000000 xhs-0.1.5/xhs/exception.py
--rw-r--r--   0 runner    (1001) docker     (123)     2709 2023-04-25 14:08:10.000000 xhs-0.1.5/xhs/help.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 14:08:23.763887 xhs-0.1.5/xhs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-04-25 14:08:23.000000 xhs-0.1.5/xhs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-04-25 14:08:23.000000 xhs-0.1.5/xhs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 14:08:23.000000 xhs-0.1.5/xhs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 14:08:23.000000 xhs-0.1.5/xhs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-25 14:08:23.000000 xhs-0.1.5/xhs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-25 14:08:23.000000 xhs-0.1.5/xhs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 07:52:41.367742 xhs-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1507 2023-05-06 07:52:29.000000 xhs-0.1.6/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-06 07:52:29.000000 xhs-0.1.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-06 07:52:29.000000 xhs-0.1.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-05-06 07:52:41.367742 xhs-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-05-06 07:52:29.000000 xhs-0.1.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-06 07:52:29.000000 xhs-0.1.6/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-06 07:52:41.367742 xhs-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-05-06 07:52:29.000000 xhs-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 07:52:41.367742 xhs-0.1.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-06 07:52:29.000000 xhs-0.1.6/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2845 2023-05-06 07:52:29.000000 xhs-0.1.6/tests/test_help.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5663 2023-05-06 07:52:29.000000 xhs-0.1.6/tests/test_xhs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-06 07:52:29.000000 xhs-0.1.6/tests/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 07:52:41.367742 xhs-0.1.6/xhs/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-06 07:52:29.000000 xhs-0.1.6/xhs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      448 2023-05-06 07:52:29.000000 xhs-0.1.6/xhs/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22296 2023-05-06 07:52:29.000000 xhs-0.1.6/xhs/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-06 07:52:29.000000 xhs-0.1.6/xhs/exception.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9719 2023-05-06 07:52:29.000000 xhs-0.1.6/xhs/help.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-06 07:52:41.367742 xhs-0.1.6/xhs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-05-06 07:52:41.000000 xhs-0.1.6/xhs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-06 07:52:41.000000 xhs-0.1.6/xhs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 07:52:41.000000 xhs-0.1.6/xhs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-06 07:52:41.000000 xhs-0.1.6/xhs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-06 07:52:41.000000 xhs-0.1.6/xhs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-06 07:52:41.000000 xhs-0.1.6/xhs.egg-info/top_level.txt
```

### Comparing `xhs-0.1.5/CHANGELOG.md` & `xhs-0.1.6/CHANGELOG.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,26 @@
 # Changelog
 
 ## dev
 
 - Improve documentation
 - Add more test function
 
+## 0.1.6
+
+### Fixed
+
+- client init without cookie will casue a exception
+
+### Added
+
+- add get note by id from html api
+- add ip block error exception
+- add x-s-common sign
+
 ## 0.1.5
 
 ### Fixed
 
 - fix get_user_all_notes lose note time and last_update_time
 
 ## 0.1.4
```

### Comparing `xhs-0.1.5/LICENSE` & `xhs-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `xhs-0.1.5/PKG-INFO` & `xhs-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xhs
-Version: 0.1.5
+Version: 0.1.6
 Summary: xiaohongshu crawl sdk.
 Home-page: https://github.com/ReaJason/xhs
 Author: ReaJason
 Author-email: reajason1225@gmail.com
 License: MIT
 Keywords: xhs crawl
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `xhs-0.1.5/README.md` & `xhs-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `xhs-0.1.5/setup.py` & `xhs-0.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `xhs-0.1.5/tests/test_help.py` & `xhs-0.1.6/tests/test_help.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,20 @@
         "cookie": test_cookie,
         "user-agent": ("Mozilla/5.0 (Windows NT 10.0; Win64; x64)"
                        "AppleWebKit/537.36 (KHTML, like Gecko)"
                        "Chrome/111.0.0.0 Safari/537.36")
     }
 
 
+def test_sign():
+    sign = help.sign("/api/sns/web/v1/user/otherinfo?"
+                     "target_user_id=5ff0e6410000000001008400")
+    print(sign)
+
+
 def test_sign_get(header):
     uri = ("/api/sns/web/v1/user/otherinfo?"
            "target_user_id=5ff0e6410000000001008400")
     sign = help.sign(uri=uri)
 
     url = f"https://edith.xiaohongshu.com{uri}"
```

### Comparing `xhs-0.1.5/tests/test_xhs.py` & `xhs-0.1.6/tests/test_xhs.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import pytest
+import requests
 
-from xhs import FeedType, XhsClient
+from xhs import FeedType, IPBlockError, XhsClient
 
 from . import test_cookie
 from .utils import beauty_print
 
 
 @pytest.fixture
 def xhs_client():
@@ -13,29 +14,36 @@
 
 def test_xhs_client_init():
     xhs_client = XhsClient()
     assert xhs_client
 
 
 def test_cookie_setter_getter():
-    cookie = "web_session=123"
-    xhs_client = XhsClient(cookie)
-    assert xhs_client.cookie == cookie
-    new_cookie = "web_session=456"
-    xhs_client.cookie = new_cookie
-    assert xhs_client.cookie == new_cookie
+    xhs_client = XhsClient()
+    cd = requests.utils.dict_from_cookiejar(xhs_client.session.cookies)
+    beauty_print(cd)
+    assert "web_session" in cd
 
 
 def test_get_note_by_id(xhs_client: XhsClient):
     note_id = "6413cf6b00000000270115b5"
     data = xhs_client.get_note_by_id(note_id)
     beauty_print(data)
     assert data["note_id"] == note_id
 
 
+def test_get_note_by_id_from_html(xhs_client: XhsClient):
+    note_id = "6413cf6b00000000270115b5"
+    data = xhs_client.get_note_by_id_from_html(note_id)
+    # pre_data = xhs_client.get_note_by_id(note_id)
+    beauty_print(data)
+    # assert pre_data == data
+    assert data["note_id"] == note_id
+
+
 def test_get_self_info(xhs_client: XhsClient):
     data = xhs_client.get_self_info()
     beauty_print(data)
     assert isinstance(data, dict)
 
 
 def test_get_user_info(xhs_client: XhsClient):
@@ -150,21 +158,35 @@
     "635d06790000000015020497"
 ])
 @pytest.mark.skip()
 def test_save_files_from_note_id_invalid_title(xhs_client: XhsClient, note_id):
     xhs_client.save_files_from_note_id(note_id, r"C:\Users\ReaJason\Desktop")
 
 
-# @pytest.mark.skip()
+@pytest.mark.skip()
 def test_get_user_collect_notes(xhs_client: XhsClient):
     notes = xhs_client.get_user_collect_notes(
         user_id="63273a77000000002303cc9b")["notes"]
     beauty_print(notes)
     assert len(notes) == 1
 
 
-# @pytest.mark.skip()
+@pytest.mark.skip()
 def test_get_user_like_notes(xhs_client: XhsClient):
     notes = xhs_client.get_user_like_notes(
         user_id="63273a77000000002303cc9b")["notes"]
     beauty_print(notes)
     assert len(notes) == 2
+
+
+@pytest.mark.skip(reason="i don't want to block by ip")
+def test_ip_block_error(xhs_client: XhsClient):
+    with pytest.raises(IPBlockError):
+        note_id = "6413cf6b00000000270115b5"
+        for _ in range(150):
+            xhs_client.get_note_by_id(note_id)
+
+
+def test_activate(xhs_client: XhsClient):
+    info = xhs_client.activate()
+    beauty_print(info)
+    assert info["session"]
```

### Comparing `xhs-0.1.5/xhs/core.py` & `xhs-0.1.6/xhs/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,18 +3,18 @@
 import re
 import time
 from enum import Enum
 from typing import NamedTuple
 
 import requests
 
-from xhs.exception import DataFetchError
+from xhs.exception import DataFetchError, IPBlockError
 
-from .help import (cookie_jar_to_cookie_str, get_search_id, sign,
-                   update_session_cookies_from_cookie)
+from .help import (cookie_jar_to_cookie_str, cookie_str_to_cookie_dict,
+                   get_search_id, sign, update_session_cookies_from_cookie)
 
 
 class FeedType(Enum):
     # 推荐
     RECOMMEND = "homefeed_recommend"
     # 穿搭
     FASION = "homefeed.fashion_v3"
@@ -101,35 +101,40 @@
                  cookie=None,
                  user_agent=None,
                  timeout=10,
                  proxies=None):
         """constructor"""
         self.proxies = proxies
         self.__session: requests.Session = requests.session()
-        if cookie:
-            update_session_cookies_from_cookie(self.__session, cookie)
         self.timeout = timeout
         self._host = "https://edith.xiaohongshu.com"
+        self.home = "https://www.xiaohongshu.com"
         user_agent = user_agent or ("Mozilla/5.0 "
                                     "(Windows NT 10.0; Win64; x64) "
                                     "AppleWebKit/537.36 "
                                     "(KHTML, like Gecko) "
                                     "Chrome/111.0.0.0 Safari/537.36")
         self.__session.headers = {
             "user-agent": user_agent,
             "Content-Type": "application/json"
         }
+        self.IP_ERROR_STR = "网络连接异常，请检查网络设置或重启试试"
+        self.IP_ERROR_CODE = 300012
+        self.cookie = cookie
 
     @property
     def cookie(self):
         return cookie_jar_to_cookie_str(self.__session)
 
     @cookie.setter
     def cookie(self, cookie: str):
         update_session_cookies_from_cookie(self.__session, cookie)
+        cookie_dict = cookie_str_to_cookie_dict(self.cookie)
+        if "web_session" not in cookie_dict:
+            self.activate()
 
     @property
     def session(self):
         return self.__session
 
     @property
     def user_agent(self):
@@ -139,22 +144,25 @@
     def user_agent(self, user_agent: str):
         self.__session.headers.update({"user-agent": user_agent})
 
     def _pre_headers(self, url: str, data=None):
         signs = sign(url, data)
         self.__session.headers.update({"x-s": signs["x-s"]})
         self.__session.headers.update({"x-t": signs["x-t"]})
+        self.__session.headers.update({"x-s-common": signs["x-s-common"]})
 
     def request(self, method, url, **kwargs):
         response = self.__session.request(
-            method, url, timeout=self.timeout,
-            proxies=self.proxies, **kwargs)
+                        method, url, timeout=self.timeout,
+                        proxies=self.proxies, **kwargs)
         data = response.json()
         if data["success"]:
             return data.get("data", data.get("success"))
+        elif data["code"] == self.IP_ERROR_CODE:
+            raise IPBlockError(self.IP_ERROR_STR)
         else:
             raise DataFetchError(data.get("msg", None))
 
     def get(self, uri: str, params=None):
         final_uri = uri
         if isinstance(params, dict):
             final_uri = (f"{uri}?"
@@ -176,14 +184,51 @@
         :rtype: dict
         """
         data = {"source_note_id": note_id}
         uri = "/api/sns/web/v1/feed"
         res = self.post(uri, data)
         return res["items"][0]["note_card"]
 
+    def get_note_by_id_from_html(self, note_id: str):
+        """get note info from "https://www.xiaohongshu.com/explore/" + note_id, and the return obj is equal to get_note_by_id
+
+        :param note_id: note_id you want to fetch
+        :type note_id: str
+        """
+
+        def camel_to_underscore(key):
+            return re.sub(r'(?<!^)(?=[A-Z])', '_', key).lower()
+
+        def transform_json_keys(json_data):
+            data_dict = json.loads(json_data)
+            new_dict = {}
+            for key, value in data_dict.items():
+                new_key = camel_to_underscore(key)
+                if not value:
+                    new_dict[new_key] = value
+                elif isinstance(value, dict):
+                    new_dict[new_key] = transform_json_keys(json.dumps(value))
+                elif isinstance(value, list):
+                    new_dict[new_key] = [transform_json_keys(json.dumps(
+                        item)) if item else item for item in value]
+                else:
+                    new_dict[new_key] = value
+            return new_dict
+
+        url = "https://www.xiaohongshu.com/explore/" + note_id
+        res = self.session.get(url, headers={"user-agent": self.user_agent})
+        html = res.text
+        state = re.findall(r'window.__INITIAL_STATE__=({.*})</script>', html)[0].replace("undefined", '""')
+        if state != "{}":
+            new_dict = transform_json_keys(state)
+            return new_dict["note"]["note"]
+        elif self.IP_ERROR_STR in html:
+            raise IPBlockError(self.IP_ERROR_STR)
+        raise DataFetchError()
+
     def save_files_from_note_id(self, note_id: str, dir_path: str):
         """this function will fetch note and save file in dir_path/note_title
 
         :param note_id: note_id that you want to fetch
         :type note_id: str
         :param dir_path: in fact, files will be stored in your dir_path/note_title directory
         :type dir_path: str
@@ -413,21 +458,19 @@
         while comments_has_more:
             comments_res = self.get_note_comments(note_id, comments_cursor)
             comments_has_more = comments_res.get("has_more", False)
             comments_cursor = comments_res.get("cursor", "")
             comments = comments_res["comments"]
             for comment in comments:
                 result.append(comment)
-                print(comment)
                 cur_sub_comment_count = int(comment["sub_comment_count"])
                 cur_sub_comments = comment["sub_comments"]
                 result.extend(cur_sub_comments)
                 sub_comments_has_more = comment["sub_comment_has_more"] and len(cur_sub_comments) < cur_sub_comment_count
                 sub_comment_cursor = comment["sub_comment_cursor"]
-                print(comment["content"] + str(sub_comments_has_more))
                 while sub_comments_has_more:
                     page_num = 30
                     sub_comments_res = self.get_note_sub_comments(note_id, comment["id"], num=page_num, cursor=sub_comment_cursor)
                     sub_comments = sub_comments_res["comments"]
                     sub_comments_has_more = sub_comments_res["has_more"] and len(sub_comments) == page_num
                     sub_comment_cursor = sub_comments_res["cursor"]
                     result.extend(sub_comments)
@@ -542,14 +585,18 @@
         uri = "/api/sns/web/v1/login/qrcode/status"
         params = {
             "qr_id": qr_id,
             "code": code
         }
         return self.get(uri, params)
 
+    def activate(self):
+        uri = "/api/sns/web/v1/login/activate"
+        return self.post(uri, data={})
+
     def get_user_collect_notes(self, user_id: str, num: int = 30, cursor: str = ""):
         uri = "/api/sns/web/v2/note/collect/page"
         params = {
             "user_id": user_id,
             "num": num,
             "cursor": cursor
         }
```

### Comparing `xhs-0.1.5/xhs.egg-info/PKG-INFO` & `xhs-0.1.6/xhs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xhs
-Version: 0.1.5
+Version: 0.1.6
 Summary: xiaohongshu crawl sdk.
 Home-page: https://github.com/ReaJason/xhs
 Author: ReaJason
 Author-email: reajason1225@gmail.com
 License: MIT
 Keywords: xhs crawl
 Classifier: Development Status :: 3 - Alpha
```

