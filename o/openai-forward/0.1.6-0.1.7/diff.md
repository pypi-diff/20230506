# Comparing `tmp/openai_forward-0.1.6.tar.gz` & `tmp/openai_forward-0.1.7.tar.gz`

## Comparing `openai_forward-0.1.6.tar` & `openai_forward-0.1.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 openai_forward-0.1.6/openai_forward/__init__.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 openai_forward-0.1.6/openai_forward/__main__.py
--rw-r--r--   0        0        0     3963 2020-02-02 00:00:00.000000 openai_forward-0.1.6/openai_forward/_base.py
--rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 openai_forward-0.1.6/openai_forward/app.py
--rw-r--r--   0        0        0     3475 2020-02-02 00:00:00.000000 openai_forward-0.1.6/openai_forward/config.py
--rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 openai_forward-0.1.6/openai_forward/openai.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.1.6/openai_forward/content/__init__.py
--rw-r--r--   0        0        0     3421 2020-02-02 00:00:00.000000 openai_forward-0.1.6/openai_forward/content/chat.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.1.6/openai_forward/content/image.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.1.6/openai_forward/routers/__init__.py
--rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 openai_forward-0.1.6/openai_forward/routers/openai_v1.py
--rw-r--r--   0        0        0     2272 2020-02-02 00:00:00.000000 openai_forward-0.1.6/openai_forward/routers/schemas.py
--rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 openai_forward-0.1.6/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 openai_forward-0.1.6/LICENSE
--rw-r--r--   0        0        0     6493 2020-02-02 00:00:00.000000 openai_forward-0.1.6/README.md
--rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 openai_forward-0.1.6/pyproject.toml
--rw-r--r--   0        0        0     7783 2020-02-02 00:00:00.000000 openai_forward-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 openai_forward-0.1.7/openai_forward/__init__.py
+-rw-r--r--   0        0        0     1499 2020-02-02 00:00:00.000000 openai_forward-0.1.7/openai_forward/__main__.py
+-rw-r--r--   0        0        0     4576 2020-02-02 00:00:00.000000 openai_forward-0.1.7/openai_forward/_base.py
+-rw-r--r--   0        0        0      677 2020-02-02 00:00:00.000000 openai_forward-0.1.7/openai_forward/app.py
+-rw-r--r--   0        0        0     3109 2020-02-02 00:00:00.000000 openai_forward-0.1.7/openai_forward/config.py
+-rw-r--r--   0        0        0      699 2020-02-02 00:00:00.000000 openai_forward-0.1.7/openai_forward/openai.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.1.7/openai_forward/content/__init__.py
+-rw-r--r--   0        0        0     3418 2020-02-02 00:00:00.000000 openai_forward-0.1.7/openai_forward/content/chat.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.1.7/openai_forward/content/image.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 openai_forward-0.1.7/openai_forward/routers/__init__.py
+-rw-r--r--   0        0        0      508 2020-02-02 00:00:00.000000 openai_forward-0.1.7/openai_forward/routers/openai_v1.py
+-rw-r--r--   0        0        0     2272 2020-02-02 00:00:00.000000 openai_forward-0.1.7/openai_forward/routers/schemas.py
+-rw-r--r--   0        0        0     1897 2020-02-02 00:00:00.000000 openai_forward-0.1.7/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 openai_forward-0.1.7/LICENSE
+-rw-r--r--   0        0        0     7067 2020-02-02 00:00:00.000000 openai_forward-0.1.7/README.md
+-rw-r--r--   0        0        0     1646 2020-02-02 00:00:00.000000 openai_forward-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0     8357 2020-02-02 00:00:00.000000 openai_forward-0.1.7/PKG-INFO
```

### Comparing `openai_forward-0.1.6/openai_forward/_base.py` & `openai_forward-0.1.7/openai_forward/_base.py`

 * *Files 12% similar despite different names*

```diff
@@ -44,15 +44,15 @@
         bytes_ = b''
         async for chunk in r.aiter_bytes():
             bytes_ += chunk
             yield chunk
         try:
             cls.log_chat_completions(bytes_)
         except Exception as e:
-            logger.warning(f"small log chat error:\n{e=}")
+            logger.debug(f"log chat (not) error:\n{e=}")
 
     @classmethod
     async def _reverse_proxy(cls, request: Request):
         client: httpx.AsyncClient = request.app.state.client
         url_path = request.url.path
         url_path = url_path[len(cls._ROUTE_PREFIX):]
         url = httpx.URL(path=url_path, query=request.url.query.encode('utf-8'))
@@ -74,21 +74,33 @@
                 msgs = input_info['messages']
                 cls.chatsaver.add_chat({
                     "host": request.client.host,
                     "model": input_info['model'],
                     "messages": [{msg['role']: msg['content']} for msg in msgs],
                 })
             except Exception as e:
-                logger.warning(f"small log chat error:\n{request.client.host=}: {e}")
+                logger.debug(f"log chat (not) error:\n{request.client.host=}: {e}")
         req = client.build_request(
             request.method, url, headers=headers,
             content=request.stream(),
             timeout=cls.timeout,
         )
-        r = await client.send(req, stream=True)
+        logger.warning(f"{url=}")
+
+        try:
+            r = await client.send(req, stream=True)
+        except httpx.ConnectError as e:
+            error_info = f"{type(e)}: {e} | " \
+                         f"Please check if host={request.client.host} can access [{cls._base_url}] successfully."
+            logger.error(error_info)
+            raise HTTPException(status_code=status.HTTP_504_GATEWAY_TIMEOUT, detail=error_info)
+        except Exception as e:
+            error_info = f"{type(e)}: {str(e)}"
+            logger.error(error_info)
+            raise HTTPException(status_code=status.HTTP_500_INTERNAL_SERVER_ERROR, detail=error_info)
 
         aiter_bytes = cls.aiter_bytes(r) if cls._LOG_CHAT else r.aiter_bytes()
         return StreamingResponse(
             aiter_bytes,
             status_code=r.status_code,
             # headers=r.headers, # do not use r.headers, it will cause error
             media_type=r.headers.get("content-type"),
```

### Comparing `openai_forward-0.1.6/openai_forward/app.py` & `openai_forward-0.1.7/openai_forward/app.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.1.6/openai_forward/config.py` & `openai_forward-0.1.7/openai_forward/config.py`

 * *Files 23% similar despite different names*

```diff
@@ -23,25 +23,16 @@
             frame = frame.f_back
             depth += 1
         logger.opt(depth=depth, exception=record.exc_info).log(level, record.getMessage())
 
 
 def setting_log(log_name, multi_process=True):
     # TODO 修复时区配置
-    time_zone = os.environ.get("TZ")
-    print(f"{time_zone=}")
-    if time_zone == "Asia/Shanghai":
-        import datetime
-        tz = pytz.timezone(time_zone)
-        loc_dt = tz.localize(datetime.datetime.now())
-        offset = loc_dt.utcoffset()
-        # tzname, offset = loc_dt.strftime("%Z::%z").split("::")
-        # offset = loc_dt.strftime("%z")
-        # os.environ['TZ'] = f"UTC-{offset}"
-        os.environ['TZ'] = f"UTC-8"
+    if os.environ.get("TZ") == "Asia/Shanghai":
+        os.environ['TZ'] = "UTC-8"
         if hasattr(time, 'tzset'):
             print(os.environ['TZ'])
             time.tzset()
 
     logging.root.handlers = [InterceptHandler()]
     for name in logging.root.manager.loggerDict.keys():
         logging.getLogger(name).handlers = []
```

### Comparing `openai_forward-0.1.6/openai_forward/openai.py` & `openai_forward-0.1.7/openai_forward/openai.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.1.6/openai_forward/content/chat.py` & `openai_forward-0.1.7/openai_forward/content/chat.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,15 +72,15 @@
         self._cur_chat_file_size += 1
         self._save_chat()
 
     def _save_chat(self):
         if len(self._chat_list) >= self._save_interval:
             logger.info(f"save chat to {self.chat_file}")
             if self._cur_chat_file_size > self._max_chat_file_size:
-                logger.warning(f"{self._cur_chat_file_size} is too large, create new file")
+                logger.info(f"{self._cur_chat_file_size} is too large, create new file")
                 self._file_idx += 1
                 self._cur_chat_file_size = 1
             self.dump_chat_list(self._chat_list, self.chat_file, mode='a+', _end='\n')
             self._chat_list = []
 
     @staticmethod
     def dump_chat_list(data: List[Dict], filepath: str, rel=False, mode='w', _sep='\n', _end="\n"):
```

### Comparing `openai_forward-0.1.6/openai_forward/routers/schemas.py` & `openai_forward-0.1.7/openai_forward/routers/schemas.py`

 * *Files identical despite different names*

### Comparing `openai_forward-0.1.6/.gitignore` & `openai_forward-0.1.7/.gitignore`

 * *Files identical despite different names*

### Comparing `openai_forward-0.1.6/LICENSE` & `openai_forward-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `openai_forward-0.1.6/README.md` & `openai_forward-0.1.7/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -26,28 +26,32 @@
     </a>
     <a href="https://github.com/beidongjiedeguang/openai-forward/actions/workflows/run_tests.yaml">
         <img alt="tests" src="https://img.shields.io/github/actions/workflow/status/beidongjiedeguang/openai-forward/run_tests.yml?label=tests">
     </a>
     <a href="https://pypi.org/project/openai_forward/">
         <img alt="pypi downloads" src="https://img.shields.io/pypi/dm/openai_forward">
     </a>
+    <a href="https://codecov.io/gh/beidongjiedeguang/openai-forward">
+        <img alt="codecov" src="https://codecov.io/gh/beidongjiedeguang/openai-forward/branch/dev/graph/badge.svg">
+    </a>
 
 </p>
 This project is designed to solve the problem of some regions being unable to directly access OpenAI. The service is deployed on a server that can access the OpenAI API, and OpenAI requests are forwarded through the service, i.e. a reverse proxy service is set up. 
 
 Test access: https://caloi.top/openai/v1/chat/completions is equivalent to https://api.openai.com/v1/chat/completions  
 Or, to put it another way, https://caloi.top/openai is equivalent to https://api.openai.com.
 
 # Table of Contents
 
 - [Features](#Features)
 - [Usage](#Usage)
 - [Deploy](#Deploy)
 - [Service Usage](#Service-Usage)
 - [Configuration](#Configuration)
+- [Chat Log](#Chat-log)
 
 # Features
 
 - [x] Supports forwarding of all OpenAI interfaces
 - [x] Request IP verification
 - [x] Streaming Response
 - [x] Supports default API key (cyclic call with multiple API keys)
@@ -186,7 +190,21 @@
 |-----------------|------------|:------------------------:|
 | OPENAI_API_KEY  | Default API key, supports multiple default API keys separated by space. | None |
 | OPENAI_BASE_URL | Forwarding base URL | `https://api.openai.com` |
 |LOG_CHAT| Whether to log chat content | `true` |
 |ROUTE_PREFIX| Route prefix | None |
 | IP_WHITELIST    | IP whitelist, separated by space. | None |
 | IP_BLACKLIST    | IP blacklist, separated by space. | None |
+
+# Chat Log
+The saved path is in the `Log/` directory under the current directory.  
+The chat log starts with `chat_` and is written to the file every 5 rounds by default.  
+The recording format is as follows:
+```text
+{'host': xxx, 'model': xxx, 'message': [{'user': xxx}, {'assistant': xxx}]}
+{'assistant': xxx}
+
+{'host': ...}
+{'assistant': ...}
+
+...
+```
```

#### html2text {}

```diff
@@ -1,32 +1,32 @@
 [**ä¸­æ**](./README_ZH.md) | **English**
                                     ******
                                 OpenAI Forward
                                      ******
                         OpenAI API æ¥å£è½¬åæå¡
                 The fastest way to deploy openai api forwarding
  [PyPI_version] [License] [Release_(latest_by_date)] [GitHub_repo_size] [docer
-                     image_size] [tests] [pypi_downloads]
+                image_size] [tests] [pypi_downloads] [codecov]
 This project is designed to solve the problem of some regions being unable to
 directly access OpenAI. The service is deployed on a server that can access the
 OpenAI API, and OpenAI requests are forwarded through the service, i.e. a
 reverse proxy service is set up. Test access: https://caloi.top/openai/v1/chat/
 completions is equivalent to https://api.openai.com/v1/chat/completions Or, to
 put it another way, https://caloi.top/openai is equivalent to https://
 api.openai.com. # Table of Contents - [Features](#Features) - [Usage](#Usage) -
 [Deploy](#Deploy) - [Service Usage](#Service-Usage) - [Configuration]
-(#Configuration) # Features - [x] Supports forwarding of all OpenAI interfaces
-- [x] Request IP verification - [x] Streaming Response - [x] Supports default
-API key (cyclic call with multiple API keys) - [x] pip installation and
-deployment - [x] Docker deployment - [x] Support for multiple worker processes
-- [x] Support for specifying the forwarding routing prefix # Usage > Here, the
-proxy address set up by the individual, https://caloi.top/openai, is used as an
-example ### Using in a module **Python** ```diff import openai +
-openai.api_base = "https://caloi.top/openai/v1" openai.api_key = "sk-******"
-``` **JS/TS** ```diff import { Configuration } from "openai"; const
+(#Configuration) - [Chat Log](#Chat-log) # Features - [x] Supports forwarding
+of all OpenAI interfaces - [x] Request IP verification - [x] Streaming Response
+- [x] Supports default API key (cyclic call with multiple API keys) - [x] pip
+installation and deployment - [x] Docker deployment - [x] Support for multiple
+worker processes - [x] Support for specifying the forwarding routing prefix #
+Usage > Here, the proxy address set up by the individual, https://caloi.top/
+openai, is used as an example ### Using in a module **Python** ```diff import
+openai + openai.api_base = "https://caloi.top/openai/v1" openai.api_key = "sk-
+******" ``` **JS/TS** ```diff import { Configuration } from "openai"; const
 configuration = new Configuration({ + basePath: "https://caloi.top/openai/v1",
 apiKey: "sk-******", }); ``` ### Image Generation (DALL-E): ```bash curl --
 location 'https://caloi.top/openai/v1/images/generations' \ --header
 'Authorization: Bearer sk-******' \ --header 'Content-Type: application/json' \
 --data '{ "prompt": "A photo of a cat", "n": 1, "size": "512x512" }' ``` ###
 [chatgpt-web](https://github.com/Chanzhaoyu/chatgpt-web) Modify the
 `OPENAI_API_BASE_URL` in [Docker Compose](https://github.com/Chanzhaoyu/
@@ -63,8 +63,13 @@
 **Environment Variable Configuration Options** refer to the `.env` file in the
 project root directory | Environment Variable | Description | Default Value |
 |-----------------|------------|:------------------------:| | OPENAI_API_KEY |
 Default API key, supports multiple default API keys separated by space. | None
 | | OPENAI_BASE_URL | Forwarding base URL | `https://api.openai.com` |
 |LOG_CHAT| Whether to log chat content | `true` | |ROUTE_PREFIX| Route prefix |
 None | | IP_WHITELIST | IP whitelist, separated by space. | None | |
-IP_BLACKLIST | IP blacklist, separated by space. | None |
+IP_BLACKLIST | IP blacklist, separated by space. | None | # Chat Log The saved
+path is in the `Log/` directory under the current directory. The chat log
+starts with `chat_` and is written to the file every 5 rounds by default. The
+recording format is as follows: ```text {'host': xxx, 'model': xxx, 'message':
+[{'user': xxx}, {'assistant': xxx}]} {'assistant': xxx} {'host': ...}
+{'assistant': ...} ... ```
```

### Comparing `openai_forward-0.1.6/pyproject.toml` & `openai_forward-0.1.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `openai_forward-0.1.6/PKG-INFO` & `openai_forward-0.1.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openai_forward
-Version: 0.1.6
+Version: 0.1.7
 Summary: 🚀 Openai api forward · OpenAI 接口转发服务 · streaming forward
 Project-URL: Homepage, https://github.com/beidongjiedeguang/openai-forward
 Project-URL: Documentation, https://github.com/beidongjiedeguang/openai-forward#openai-forward
 Project-URL: Issues, https://github.com/beidongjiedeguang/openai-forward/issues
 Project-URL: Source, https://github.com/beidongjiedeguang/openai-forward
 Author-email: kunyuan <beidongjiedeguang@gmail.com>
 License-File: LICENSE
@@ -59,28 +59,32 @@
     </a>
     <a href="https://github.com/beidongjiedeguang/openai-forward/actions/workflows/run_tests.yaml">
         <img alt="tests" src="https://img.shields.io/github/actions/workflow/status/beidongjiedeguang/openai-forward/run_tests.yml?label=tests">
     </a>
     <a href="https://pypi.org/project/openai_forward/">
         <img alt="pypi downloads" src="https://img.shields.io/pypi/dm/openai_forward">
     </a>
+    <a href="https://codecov.io/gh/beidongjiedeguang/openai-forward">
+        <img alt="codecov" src="https://codecov.io/gh/beidongjiedeguang/openai-forward/branch/dev/graph/badge.svg">
+    </a>
 
 </p>
 This project is designed to solve the problem of some regions being unable to directly access OpenAI. The service is deployed on a server that can access the OpenAI API, and OpenAI requests are forwarded through the service, i.e. a reverse proxy service is set up. 
 
 Test access: https://caloi.top/openai/v1/chat/completions is equivalent to https://api.openai.com/v1/chat/completions  
 Or, to put it another way, https://caloi.top/openai is equivalent to https://api.openai.com.
 
 # Table of Contents
 
 - [Features](#Features)
 - [Usage](#Usage)
 - [Deploy](#Deploy)
 - [Service Usage](#Service-Usage)
 - [Configuration](#Configuration)
+- [Chat Log](#Chat-log)
 
 # Features
 
 - [x] Supports forwarding of all OpenAI interfaces
 - [x] Request IP verification
 - [x] Streaming Response
 - [x] Supports default API key (cyclic call with multiple API keys)
@@ -219,7 +223,21 @@
 |-----------------|------------|:------------------------:|
 | OPENAI_API_KEY  | Default API key, supports multiple default API keys separated by space. | None |
 | OPENAI_BASE_URL | Forwarding base URL | `https://api.openai.com` |
 |LOG_CHAT| Whether to log chat content | `true` |
 |ROUTE_PREFIX| Route prefix | None |
 | IP_WHITELIST    | IP whitelist, separated by space. | None |
 | IP_BLACKLIST    | IP blacklist, separated by space. | None |
+
+# Chat Log
+The saved path is in the `Log/` directory under the current directory.  
+The chat log starts with `chat_` and is written to the file every 5 rounds by default.  
+The recording format is as follows:
+```text
+{'host': xxx, 'model': xxx, 'message': [{'user': xxx}, {'assistant': xxx}]}
+{'assistant': xxx}
+
+{'host': ...}
+{'assistant': ...}
+
+...
+```
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: openai_forward Version: 0.1.6 Summary: ð Openai
+Metadata-Version: 2.1 Name: openai_forward Version: 0.1.7 Summary: ð Openai
 api forward Â· OpenAI æ¥å£è½¬åæå¡ Â· streaming forward Project-URL:
 Homepage, https://github.com/beidongjiedeguang/openai-forward Project-URL:
 Documentation, https://github.com/beidongjiedeguang/openai-forward#openai-
 forward Project-URL: Issues, https://github.com/beidongjiedeguang/openai-
 forward/issues Project-URL: Source, https://github.com/beidongjiedeguang/
 openai-forward Author-email: kunyuan
 gmail.com> License-File: LICENSE Keywords:
@@ -19,32 +19,32 @@
 README_ZH.md) | **English**
                                     ******
                                 OpenAI Forward
                                      ******
                         OpenAI API æ¥å£è½¬åæå¡
                 The fastest way to deploy openai api forwarding
  [PyPI_version] [License] [Release_(latest_by_date)] [GitHub_repo_size] [docer
-                     image_size] [tests] [pypi_downloads]
+                image_size] [tests] [pypi_downloads] [codecov]
 This project is designed to solve the problem of some regions being unable to
 directly access OpenAI. The service is deployed on a server that can access the
 OpenAI API, and OpenAI requests are forwarded through the service, i.e. a
 reverse proxy service is set up. Test access: https://caloi.top/openai/v1/chat/
 completions is equivalent to https://api.openai.com/v1/chat/completions Or, to
 put it another way, https://caloi.top/openai is equivalent to https://
 api.openai.com. # Table of Contents - [Features](#Features) - [Usage](#Usage) -
 [Deploy](#Deploy) - [Service Usage](#Service-Usage) - [Configuration]
-(#Configuration) # Features - [x] Supports forwarding of all OpenAI interfaces
-- [x] Request IP verification - [x] Streaming Response - [x] Supports default
-API key (cyclic call with multiple API keys) - [x] pip installation and
-deployment - [x] Docker deployment - [x] Support for multiple worker processes
-- [x] Support for specifying the forwarding routing prefix # Usage > Here, the
-proxy address set up by the individual, https://caloi.top/openai, is used as an
-example ### Using in a module **Python** ```diff import openai +
-openai.api_base = "https://caloi.top/openai/v1" openai.api_key = "sk-******"
-``` **JS/TS** ```diff import { Configuration } from "openai"; const
+(#Configuration) - [Chat Log](#Chat-log) # Features - [x] Supports forwarding
+of all OpenAI interfaces - [x] Request IP verification - [x] Streaming Response
+- [x] Supports default API key (cyclic call with multiple API keys) - [x] pip
+installation and deployment - [x] Docker deployment - [x] Support for multiple
+worker processes - [x] Support for specifying the forwarding routing prefix #
+Usage > Here, the proxy address set up by the individual, https://caloi.top/
+openai, is used as an example ### Using in a module **Python** ```diff import
+openai + openai.api_base = "https://caloi.top/openai/v1" openai.api_key = "sk-
+******" ``` **JS/TS** ```diff import { Configuration } from "openai"; const
 configuration = new Configuration({ + basePath: "https://caloi.top/openai/v1",
 apiKey: "sk-******", }); ``` ### Image Generation (DALL-E): ```bash curl --
 location 'https://caloi.top/openai/v1/images/generations' \ --header
 'Authorization: Bearer sk-******' \ --header 'Content-Type: application/json' \
 --data '{ "prompt": "A photo of a cat", "n": 1, "size": "512x512" }' ``` ###
 [chatgpt-web](https://github.com/Chanzhaoyu/chatgpt-web) Modify the
 `OPENAI_API_BASE_URL` in [Docker Compose](https://github.com/Chanzhaoyu/
@@ -81,8 +81,13 @@
 **Environment Variable Configuration Options** refer to the `.env` file in the
 project root directory | Environment Variable | Description | Default Value |
 |-----------------|------------|:------------------------:| | OPENAI_API_KEY |
 Default API key, supports multiple default API keys separated by space. | None
 | | OPENAI_BASE_URL | Forwarding base URL | `https://api.openai.com` |
 |LOG_CHAT| Whether to log chat content | `true` | |ROUTE_PREFIX| Route prefix |
 None | | IP_WHITELIST | IP whitelist, separated by space. | None | |
-IP_BLACKLIST | IP blacklist, separated by space. | None |
+IP_BLACKLIST | IP blacklist, separated by space. | None | # Chat Log The saved
+path is in the `Log/` directory under the current directory. The chat log
+starts with `chat_` and is written to the file every 5 rounds by default. The
+recording format is as follows: ```text {'host': xxx, 'model': xxx, 'message':
+[{'user': xxx}, {'assistant': xxx}]} {'assistant': xxx} {'host': ...}
+{'assistant': ...} ... ```
```

