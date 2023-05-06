# Comparing `tmp/tremolo-0.0.86.tar.gz` & `tmp/tremolo-0.0.88.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tremolo-0.0.86.tar", last modified: Mon Apr 17 02:09:06 2023, max compression
+gzip compressed data, was "dist/tremolo-0.0.88.tar", last modified: Sat May  6 12:13:04 2023, max compression
```

## Comparing `tremolo-0.0.86.tar` & `tremolo-0.0.88.tar`

### file list

```diff
@@ -1,27 +1,31 @@
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-04-17 02:09:06.000000 tremolo-0.0.86/
--rw-r--r--   0 tux       (1000) users      (100)     3487 2023-04-17 02:09:06.000000 tremolo-0.0.86/PKG-INFO
--rw-r--r--   0 tux       (1000) users      (100)     2202 2023-04-12 13:07:35.000000 tremolo-0.0.86/README.md
--rw-r--r--   0 tux       (1000) users      (100)       38 2023-04-17 02:09:06.000000 tremolo-0.0.86/setup.cfg
--rwxr-xr-x   0 tux       (1000) users      (100)      973 2023-04-17 02:04:05.000000 tremolo-0.0.86/setup.py
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-04-17 02:09:06.000000 tremolo-0.0.86/tremolo/
--rwxr-xr-x   0 tux       (1000) users      (100)       54 2023-04-12 13:07:35.000000 tremolo-0.0.86/tremolo/__init__.py
--rw-r--r--   0 tux       (1000) users      (100)      321 2023-04-12 13:07:35.000000 tremolo-0.0.86/tremolo/exceptions.py
--rw-r--r--   0 tux       (1000) users      (100)    11623 2023-04-16 23:50:01.000000 tremolo-0.0.86/tremolo/http_server.py
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-04-17 02:09:06.000000 tremolo-0.0.86/tremolo/lib/
--rwxr-xr-x   0 tux       (1000) users      (100)        0 2023-04-12 13:07:35.000000 tremolo-0.0.86/tremolo/lib/__init__.py
--rw-r--r--   0 tux       (1000) users      (100)      846 2023-04-12 13:07:35.000000 tremolo-0.0.86/tremolo/lib/connection_pool.py
--rw-r--r--   0 tux       (1000) users      (100)     1665 2023-04-12 13:07:35.000000 tremolo-0.0.86/tremolo/lib/http_exception.py
--rwxr-xr-x   0 tux       (1000) users      (100)    13753 2023-04-17 02:02:16.000000 tremolo-0.0.86/tremolo/lib/http_protocol.py
--rwxr-xr-x   0 tux       (1000) users      (100)     8775 2023-04-16 23:20:22.000000 tremolo-0.0.86/tremolo/lib/http_request.py
--rwxr-xr-x   0 tux       (1000) users      (100)    10732 2023-04-14 02:53:02.000000 tremolo-0.0.86/tremolo/lib/http_response.py
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-04-17 02:09:06.000000 tremolo-0.0.86/tremolo/lib/parsed/
--rw-r--r--   0 tux       (1000) users      (100)       31 2023-04-12 13:07:35.000000 tremolo-0.0.86/tremolo/lib/parsed/__init__.py
--rwxr-xr-x   0 tux       (1000) users      (100)     4954 2023-04-16 22:37:48.000000 tremolo-0.0.86/tremolo/lib/parsed/parse.py
--rwxr-xr-x   0 tux       (1000) users      (100)     1259 2023-04-12 13:07:35.000000 tremolo-0.0.86/tremolo/lib/request.py
--rwxr-xr-x   0 tux       (1000) users      (100)      810 2023-04-12 13:07:35.000000 tremolo-0.0.86/tremolo/lib/response.py
--rwxr-xr-x   0 tux       (1000) users      (100)    13668 2023-04-16 23:28:28.000000 tremolo-0.0.86/tremolo/tremolo.py
-drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-04-17 02:09:06.000000 tremolo-0.0.86/tremolo.egg-info/
--rw-r--r--   0 tux       (1000) users      (100)     3487 2023-04-17 02:09:05.000000 tremolo-0.0.86/tremolo.egg-info/PKG-INFO
--rw-r--r--   0 tux       (1000) users      (100)      503 2023-04-17 02:09:05.000000 tremolo-0.0.86/tremolo.egg-info/SOURCES.txt
--rw-r--r--   0 tux       (1000) users      (100)        1 2023-04-17 02:09:05.000000 tremolo-0.0.86/tremolo.egg-info/dependency_links.txt
--rw-r--r--   0 tux       (1000) users      (100)        8 2023-04-17 02:09:05.000000 tremolo-0.0.86/tremolo.egg-info/top_level.txt
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-06 12:13:04.000000 tremolo-0.0.88/
+-rw-r--r--   0 tux       (1000) users      (100)     4740 2023-05-06 12:13:04.000000 tremolo-0.0.88/PKG-INFO
+-rw-r--r--   0 tux       (1000) users      (100)     3143 2023-05-06 12:12:19.000000 tremolo-0.0.88/README.md
+-rw-r--r--   0 tux       (1000) users      (100)       38 2023-05-06 12:13:04.000000 tremolo-0.0.88/setup.cfg
+-rwxr-xr-x   0 tux       (1000) users      (100)      973 2023-05-06 12:12:19.000000 tremolo-0.0.88/setup.py
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-06 12:13:04.000000 tremolo-0.0.88/tremolo/
+-rwxr-xr-x   0 tux       (1000) users      (100)       54 2023-05-06 12:12:19.000000 tremolo-0.0.88/tremolo/__init__.py
+-rw-r--r--   0 tux       (1000) users      (100)     4465 2023-05-06 12:12:19.000000 tremolo-0.0.88/tremolo/__main__.py
+-rw-r--r--   0 tux       (1000) users      (100)     2278 2023-05-06 12:12:19.000000 tremolo-0.0.88/tremolo/asgi_lifespan.py
+-rw-r--r--   0 tux       (1000) users      (100)     5300 2023-05-06 12:12:19.000000 tremolo-0.0.88/tremolo/asgi_server.py
+-rw-r--r--   0 tux       (1000) users      (100)      542 2023-05-06 12:12:19.000000 tremolo-0.0.88/tremolo/contexts.py
+-rw-r--r--   0 tux       (1000) users      (100)      586 2023-05-06 12:12:19.000000 tremolo-0.0.88/tremolo/exceptions.py
+-rw-r--r--   0 tux       (1000) users      (100)    11243 2023-05-06 12:12:19.000000 tremolo-0.0.88/tremolo/http_server.py
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-06 12:13:04.000000 tremolo-0.0.88/tremolo/lib/
+-rwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-06 12:12:19.000000 tremolo-0.0.88/tremolo/lib/__init__.py
+-rw-r--r--   0 tux       (1000) users      (100)      846 2023-05-06 12:12:19.000000 tremolo-0.0.88/tremolo/lib/connection_pool.py
+-rw-r--r--   0 tux       (1000) users      (100)     1798 2023-05-06 12:12:19.000000 tremolo-0.0.88/tremolo/lib/http_exception.py
+-rwxr-xr-x   0 tux       (1000) users      (100)    13709 2023-05-06 12:12:19.000000 tremolo-0.0.88/tremolo/lib/http_protocol.py
+-rwxr-xr-x   0 tux       (1000) users      (100)     9155 2023-05-06 12:12:19.000000 tremolo-0.0.88/tremolo/lib/http_request.py
+-rwxr-xr-x   0 tux       (1000) users      (100)    10924 2023-05-06 12:12:19.000000 tremolo-0.0.88/tremolo/lib/http_response.py
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-06 12:13:04.000000 tremolo-0.0.88/tremolo/lib/parsed/
+-rw-r--r--   0 tux       (1000) users      (100)       31 2023-05-06 12:12:19.000000 tremolo-0.0.88/tremolo/lib/parsed/__init__.py
+-rwxr-xr-x   0 tux       (1000) users      (100)     4954 2023-05-06 12:12:19.000000 tremolo-0.0.88/tremolo/lib/parsed/parse.py
+-rwxr-xr-x   0 tux       (1000) users      (100)     1259 2023-05-06 12:12:19.000000 tremolo-0.0.88/tremolo/lib/request.py
+-rwxr-xr-x   0 tux       (1000) users      (100)      810 2023-05-06 12:12:19.000000 tremolo-0.0.88/tremolo/lib/response.py
+-rwxr-xr-x   0 tux       (1000) users      (100)    15012 2023-05-06 12:12:19.000000 tremolo-0.0.88/tremolo/tremolo.py
+drwxr-xr-x   0 tux       (1000) users      (100)        0 2023-05-06 12:13:04.000000 tremolo-0.0.88/tremolo.egg-info/
+-rw-r--r--   0 tux       (1000) users      (100)     4740 2023-05-06 12:13:04.000000 tremolo-0.0.88/tremolo.egg-info/PKG-INFO
+-rw-r--r--   0 tux       (1000) users      (100)      591 2023-05-06 12:13:04.000000 tremolo-0.0.88/tremolo.egg-info/SOURCES.txt
+-rw-r--r--   0 tux       (1000) users      (100)        1 2023-05-06 12:13:04.000000 tremolo-0.0.88/tremolo.egg-info/dependency_links.txt
+-rw-r--r--   0 tux       (1000) users      (100)        8 2023-05-06 12:13:04.000000 tremolo-0.0.88/tremolo.egg-info/top_level.txt
```

### Comparing `tremolo-0.0.86/PKG-INFO` & `tremolo-0.0.88/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tremolo
-Version: 0.0.86
+Version: 0.0.88
 Summary: Tremolo is a stream-oriented, asynchronous web server/framework written in pure Python
 Home-page: https://github.com/nggit/tremolo
 Author: nggit
 Author-email: contact@anggit.com
 License: MIT
 Description: # Tremolo
         
@@ -54,14 +54,53 @@
         
         Well, `latin-1` on the right side is not required. The default is `utf-8`.
         
         You can save it as `hello.py` and just run it with `python3 hello.py`.
         
         Your first *hello world* page with Tremolo will be at http://localhost:8000/hello.
         
+        ## ASGI Server
+        Tremolo is an HTTP Server framework. You can build abstractions on top of it, say an ASGI server.
+        
+        In fact, Tremolo already has ASGI server implementation.
+        
+        So you can immediately use existing [ASGI applications / frameworks](https://asgi.readthedocs.io/en/latest/implementations.html#application-frameworks), behind Tremolo (ASGI server).
+        
+        For example, If a minimal ASGI application with the name `example.py`:
+        
+        ```python
+        async def app(scope, receive, send):
+            assert scope['type'] == 'http'
+        
+            await send({
+                'type': 'http.response.start',
+                'status': 200,
+                'headers': [
+                    (b'content-type', b'text/plain'),
+                ]
+            })
+        
+            await send({
+                'type': 'http.response.body',
+                'body': b'Hello world!'
+            })
+        ```
+        
+        Then you can run as follows:
+        
+        ```
+        python3 -m tremolo --debug --bind 127.0.0.1:8000 example:app
+        ```
+        
+        To see more available options:
+        
+        ```
+        python3 -m tremolo --help
+        ```
+        
         ## Misc
         Tremolo utilizes `SO_REUSEPORT` (Linux 3.9+) to load balance worker processes.
         
         ```python
         app.run('0.0.0.0', 8000, worker_num=2)
         ```
```

### Comparing `tremolo-0.0.86/README.md` & `tremolo-0.0.88/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -46,14 +46,53 @@
 
 Well, `latin-1` on the right side is not required. The default is `utf-8`.
 
 You can save it as `hello.py` and just run it with `python3 hello.py`.
 
 Your first *hello world* page with Tremolo will be at http://localhost:8000/hello.
 
+## ASGI Server
+Tremolo is an HTTP Server framework. You can build abstractions on top of it, say an ASGI server.
+
+In fact, Tremolo already has ASGI server implementation.
+
+So you can immediately use existing [ASGI applications / frameworks](https://asgi.readthedocs.io/en/latest/implementations.html#application-frameworks), behind Tremolo (ASGI server).
+
+For example, If a minimal ASGI application with the name `example.py`:
+
+```python
+async def app(scope, receive, send):
+    assert scope['type'] == 'http'
+
+    await send({
+        'type': 'http.response.start',
+        'status': 200,
+        'headers': [
+            (b'content-type', b'text/plain'),
+        ]
+    })
+
+    await send({
+        'type': 'http.response.body',
+        'body': b'Hello world!'
+    })
+```
+
+Then you can run as follows:
+
+```
+python3 -m tremolo --debug --bind 127.0.0.1:8000 example:app
+```
+
+To see more available options:
+
+```
+python3 -m tremolo --help
+```
+
 ## Misc
 Tremolo utilizes `SO_REUSEPORT` (Linux 3.9+) to load balance worker processes.
 
 ```python
 app.run('0.0.0.0', 8000, worker_num=2)
 ```
```

### Comparing `tremolo-0.0.86/setup.py` & `tremolo-0.0.88/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setup(
     name='tremolo',
     packages=['tremolo'],
     package_data={'': ['lib/*', 'lib/parsed/*']},
-    version='0.0.86',
+    version='0.0.88',
     license='MIT',
     author='nggit',
     author_email='contact@anggit.com',
     description='Tremolo is a stream-oriented, asynchronous web server/framework written in pure Python',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/nggit/tremolo',
```

### Comparing `tremolo-0.0.86/tremolo/http_server.py` & `tremolo-0.0.88/tremolo/http_server.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,43 +1,18 @@
 # Copyright (c) 2023 nggit
 
 __all__ = ('HTTPServer',)
 
 from datetime import datetime
 from urllib.parse import parse_qs
 
+from .contexts import ServerContext
 from .exceptions import ExpectationFailed
 from .lib.http_protocol import HTTPProtocol
 
-class ServerContext:
-    def __init__(self):
-        self.__dict__ = {
-            'options': {},
-            'tasks': [],
-            'data': {}
-        }
-
-    def __repr__(self):
-        return self.__dict__.__repr__()
-
-    @property
-    def options(self):
-        return self.__dict__['options']
-
-    @property
-    def tasks(self):
-        return self.__dict__['tasks']
-
-    @property
-    def data(self):
-        return self.__dict__['data']
-
-    def set(self, name, value):
-        self.__dict__[name] = value
-
 class HTTPServer(HTTPProtocol):
     def __init__(self, **kwargs):
         self._route_handlers = kwargs['_handlers']
         self._middlewares = kwargs['_middlewares']
         self._server = {
             'loop': kwargs['loop'],
             'logger': kwargs['logger'],
@@ -184,16 +159,22 @@
         if is_agen:
             if no_content:
                 self._server['response'].append_header(b'Connection: close\r\n\r\n')
             else:
                 if not self._server['response'].http_chunked:
                     self._server['request'].http_keepalive = False
 
-                self._server['response'].append_header(b'Content-Type: %s\r\nConnection: keep-alive\r\n\r\n' %
-                                                       self._server['response'].get_content_type())
+                if status[0] == 101:
+                    self._server['request'].http_upgrade = True
+
+                self._server['response'].append_header(
+                    b'Content-Type: %s\r\nConnection: %s\r\n\r\n' %
+                    (self._server['response'].get_content_type(), {False: b'keep-alive',
+                                                                   True: b'upgrade'}[status[0] in (101, 426)])
+                )
 
             if self._server['request'].method == b'HEAD' or no_content:
                 await self._server['response'].write(None)
                 return
 
             self.set_watermarks(high=options['buffer_size'] * 4, low=options['buffer_size'] // 2)
             await self._server['response'].write(
@@ -255,62 +236,63 @@
 
         for middleware in self._middlewares['request']:
             options = await self._handle_middleware(middleware[0], {**middleware[1], **options})
 
             if not isinstance(options, dict):
                 return
 
-        if request.is_valid:
-            if request.query_string != b'':
-                self._server['request'].query = parse_qs(request.query_string.decode(encoding='latin-1'))
+        if not request.is_valid:
+            # bad request
+            await self._handle_response(self._route_handlers[0][0][1], {**self._route_handlers[0][0][2], **options})
+            return
 
-            p = request.path.strip(b'/')
+        if request.query_string != b'':
+            self._server['request'].query = parse_qs(request.query_string.decode(encoding='latin-1'))
 
-            if p == b'':
-                ri = 1
-            else:
-                ri = b'%d#%s' % (p.count(b'/') + 2, p[:(p + b'/').find(b'/')])
+        p = request.path.strip(b'/')
+
+        if p == b'':
+            ri = 1
+        else:
+            ri = b'%d#%s' % (p.count(b'/') + 2, p[:(p + b'/').find(b'/')])
 
-            if ri in self._route_handlers:
-                for (pattern, func, kwargs) in self._route_handlers[ri]:
-                    m = pattern.search(request.url)
+        if ri in self._route_handlers:
+            for (pattern, func, kwargs) in self._route_handlers[ri]:
+                m = pattern.search(request.url)
 
-                    if m:
-                        await self._handle_continue()
+                if m:
+                    await self._handle_continue()
 
-                        matches = m.groupdict()
+                    matches = m.groupdict()
 
-                        if not matches:
-                            matches = m.groups()
+                    if not matches:
+                        matches = m.groups()
 
-                        self._server['request'].params['path'] = matches
+                    self._server['request'].params['path'] = matches
 
-                        await self._handle_response(func, {**kwargs, **options})
-                        return
-            else:
-                for i, (pattern, func, kwargs) in enumerate(self._route_handlers[-1]):
-                    m = pattern.search(request.url)
+                    await self._handle_response(func, {**kwargs, **options})
+                    return
+        else:
+            for i, (pattern, func, kwargs) in enumerate(self._route_handlers[-1]):
+                m = pattern.search(request.url)
 
-                    if m:
-                        if ri in self._route_handlers:
-                            self._route_handlers[ri].append((pattern, func, kwargs))
-                        else:
-                            self._route_handlers[ri] = [(pattern, func, kwargs)]
+                if m:
+                    if ri in self._route_handlers:
+                        self._route_handlers[ri].append((pattern, func, kwargs))
+                    else:
+                        self._route_handlers[ri] = [(pattern, func, kwargs)]
 
-                        await self._handle_continue()
+                    await self._handle_continue()
 
-                        matches = m.groupdict()
+                    matches = m.groupdict()
 
-                        if not matches:
-                            matches = m.groups()
+                    if not matches:
+                        matches = m.groups()
 
-                        self._server['request'].params['path'] = matches
+                    self._server['request'].params['path'] = matches
 
-                        await self._handle_response(func, {**kwargs, **options})
-                        del self._route_handlers[-1][i]
-                        return
+                    await self._handle_response(func, {**kwargs, **options})
+                    del self._route_handlers[-1][i]
+                    return
 
-            # not found
-            await self._handle_response(self._route_handlers[0][1][1], {**self._route_handlers[0][1][2], **options})
-        else:
-            # bad request
-            await self._handle_response(self._route_handlers[0][0][1], {**self._route_handlers[0][0][2], **options})
+        # not found
+        await self._handle_response(self._route_handlers[0][1][1], {**self._route_handlers[0][1][2], **options})
```

### Comparing `tremolo-0.0.86/tremolo/lib/connection_pool.py` & `tremolo-0.0.88/tremolo/lib/connection_pool.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.86/tremolo/lib/http_exception.py` & `tremolo-0.0.88/tremolo/lib/http_exception.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,22 @@
 # Copyright (c) 2023 nggit
 
-class HTTPException(Exception):
+class TremoloException(Exception):
+    message = 'TremoloException'
+
+    def __init__(self, *args):
+        self.args = args
+
+    def __str__(self):
+        if self.args:
+            return ' '.join(self.args)
+
+        return self.message
+
+class HTTPException(TremoloException):
     code = 500
     message = 'Internal Server Error'
     content_type = 'text/html; charset=utf-8'
 
     def __init__(self, *args, code=None, message=None, content_type=None, cause=None):
         self.args = args
 
@@ -16,20 +28,14 @@
 
         if isinstance(content_type, str):
             self.content_type = content_type
 
         if isinstance(cause, Exception):
             self.__cause__ = cause
 
-    def __str__(self):
-        if self.args:
-            return ' '.join(self.args)
-
-        return self.message
-
 class BadRequest(HTTPException):
     code = 400
     message = 'Bad Request'
 
 class Unauthorized(HTTPException):
     code = 401
     message = 'Unauthorized'
```

### Comparing `tremolo-0.0.86/tremolo/lib/http_protocol.py` & `tremolo-0.0.88/tremolo/lib/http_protocol.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,15 +110,16 @@
         if transport is not None and self._request is not None:
             if self._request.http_upgrade:
                 transport.resume_reading()
                 return
 
             self._request.body_size += data_size
 
-            if self._request.content_length > -1 and self._request.body_size >= self._request.content_length and queue is not None:
+            if (b'content-length' in self._request.headers and self._request.body_size >= self._request.content_length
+                    and queue is not None):
                 queue.put_nowait(None)
             elif self._request.body_size < self._options['client_max_body_size']:
                 transport.resume_reading()
             else:
                 if self._queue[1] is not None:
                     self._request.http_keepalive = False
                     self._queue[1].put_nowait(None)
@@ -189,15 +190,15 @@
         try:
             if b'connection' in self._request.headers:
                 if self._request.headers[b'connection'].lower().find(b'close') == -1:
                     self._request.http_keepalive = True
             elif self._request.version == b'1.1':
                 self._request.http_keepalive = True
 
-            if self._request.method in (b'POST', b'PUT', b'PATCH'):
+            if b'transfer-encoding' in self._request.headers or b'content-length' in self._request.headers:
                 if b'content-type' in self._request.headers:
                     self._request.content_type = self._request.headers[b'content-type'].lower()
 
                 if b'transfer-encoding' in self._request.headers:
                     if self._request.version == b'1.0':
                         raise BadRequest
 
@@ -326,16 +327,15 @@
 
                 self._transport.write(data)
             except asyncio.CancelledError:
                 pass
             except Exception as exc:
                 if self._transport is not None:
                     self._transport.abort()
-
-                self.print_exception(exc)
+                    self.print_exception(exc)
 
     def connection_lost(self, exc):
         for task in self.tasks:
             if callable(task):
                 task()
                 continue
 
@@ -343,21 +343,16 @@
                 exc = task.exception()
 
                 if exc:
                     self.print_exception(exc)
             except asyncio.InvalidStateError:
                 task.cancel()
 
-        for queue in self._queue:
-            while not queue.empty():
-                queue.get_nowait()
-                queue.task_done()
-
         self._options['_pool'].put({
-            'queue': self._queue,
+            'queue': (asyncio.Queue(), asyncio.Queue()),
             'header': self._header
         })
 
         self._transport = None
         self._queue = (None, None)
         self._request = None
         self._response = None
```

### Comparing `tremolo-0.0.86/tremolo/lib/http_request.py` & `tremolo-0.0.88/tremolo/lib/http_request.py`

 * *Files 7% similar despite different names*

```diff
@@ -76,15 +76,15 @@
 
             while buf != b'0\r\n\r\n':
                 if not paused:
                     try:
                         buf.extend(await agen.__anext__())
                     except StopAsyncIteration:
                         if not buf.endswith(b'0\r\n\r\n'):
-                            return
+                            raise BadRequest('bad chunked encoding: incomplete read')
 
                 if tobe_read > 0:
                     data = buf[:tobe_read]
 
                     yield data
                     del buf[:tobe_read]
 
@@ -95,19 +95,22 @@
 
                     paused = True
                     del buf[:2]
                 else:
                     i = buf.find(b'\r\n')
 
                     if i == -1:
+                        if len(buf) > self.protocol.options['buffer_size'] * 4:
+                            raise BadRequest('bad chunked encoding: no chunk size')
+
                         paused = False
                         continue
 
                     try:
-                        chunk_size = int(buf[:i].split(b';')[0], 16)
+                        chunk_size = int(buf[:i].split(b';', 1)[0], 16)
                     except ValueError:
                         del buf[:]
                         raise BadRequest('bad chunked encoding')
 
                     data = buf[i + 2:i + 2 + chunk_size]
                     tobe_read = chunk_size - len(data)
 
@@ -237,21 +240,24 @@
             data = b''
 
             if not paused:
                 try:
                     data = await agen.__anext__()
                 except StopAsyncIteration:
                     if header_size == -1 or body_size == -1:
-                        return
+                        raise BadRequest('malformed multipart/form-data')
 
             if isinstance(header, bytearray):
                 header.extend(data)
                 header_size = header.find(b'\r\n\r\n')
 
                 if header_size == -1:
+                    if len(header) > 8192:
+                        raise BadRequest('malformed multipart/form-data')
+
                     paused = False
                 else:
                     body = header[header_size + 4:]
                     info = {}
 
                     if header_size <= 8192 and header.startswith(b'--%s\r\n' % boundary):
                         header = self.protocol.header.parse(header, header_size=header_size).getheaders()
```

### Comparing `tremolo-0.0.86/tremolo/lib/http_response.py` & `tremolo-0.0.88/tremolo/lib/http_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -135,16 +135,21 @@
 
                 if no_content:
                     self.append_header(b'Connection: close\r\n\r\n')
                 else:
                     if not self._http_chunked and not (self._request.version == b'1.1' and b'range' in self._request.headers):
                         self._request.http_keepalive = False
 
-                    self.append_header(b'Content-Type: %s\r\nConnection: keep-alive\r\n\r\n' %
-                                       self.get_content_type())
+                    if status[0] == 101:
+                        self._request.http_upgrade = True
+
+                    self.append_header(
+                        b'Content-Type: %s\r\nConnection: %s\r\n\r\n' %
+                        (self.get_content_type(), {False: b'keep-alive', True: b'upgrade'}[status[0] in (101, 426)])
+                    )
 
                 if self._request.method == b'HEAD' or no_content:
                     self._request.http_keepalive = False
                     data = None
                 else:
                     self._request.protocol.set_watermarks(high=buffer_size * 4, low=buffer_size // 2)
```

### Comparing `tremolo-0.0.86/tremolo/lib/parsed/parse.py` & `tremolo-0.0.88/tremolo/lib/parsed/parse.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.86/tremolo/lib/request.py` & `tremolo-0.0.88/tremolo/lib/request.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.86/tremolo/lib/response.py` & `tremolo-0.0.88/tremolo/lib/response.py`

 * *Files identical despite different names*

### Comparing `tremolo-0.0.86/tremolo/tremolo.py` & `tremolo-0.0.88/tremolo/tremolo.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,18 +12,18 @@
 import ssl
 import sys
 import time
 
 from copy import deepcopy
 from datetime import datetime
 from functools import wraps
+from importlib import import_module
 
 from .lib.connection_pool import ConnectionPool
 from .exceptions import BadRequest
-from .http_server import HTTPServer
 
 class Tremolo:
     def __init__(self):
         self._ports = []
 
         self._route_handlers = {
             0: [
@@ -184,47 +184,84 @@
                 sock.listen(backlog)
                 options['conn'].send(True)
             except Exception:
                 options['conn'].send(False)
                 sock = options['conn'].recv()
                 sock.listen(backlog)
 
-        if 'ssl' in options and isinstance(options['ssl'], dict):
+        if 'ssl' in options and options['ssl'] and isinstance(options['ssl'], dict):
             ssl_context = ssl.create_default_context(ssl.Purpose.CLIENT_AUTH)
-            ssl_context.load_cert_chain(certfile=options['ssl'].get('cert'),
+            ssl_context.load_cert_chain(certfile=options['ssl'].get('cert', ''),
                                         keyfile=options['ssl'].get('key'),
                                         password=options['ssl'].get('password'))
         else:
             ssl_context = None
 
         server_name = options.get('server_name', b'Tremolo')
 
         if isinstance(server_name, str):
             server_name = server_name.encode(encoding='latin-1')
 
         if isinstance(host, str):
             host = host.encode(encoding='latin-1')
 
         pool = ConnectionPool(1024, self._logger)
+        lifespan = None
+
+        if 'app' in options and isinstance(options['app'], str):
+            from .asgi_lifespan import ASGILifespan
+            from .asgi_server import ASGIServer as Server
+
+            # 'module:app'               -> 'module:app'   (dir: os.getcwd())
+            # '/path/to/module.py'       -> 'module:app'   (dir: '/path/to')
+            # '/path/to/module.py:myapp' -> 'module:myapp' (dir: '/path/to')
+
+            path, attr_name = (options['app'] + ':app').split(':')[:2]
+            dir_name, base_name = os.path.split(path)
+            module_name = os.path.splitext(base_name)[0]
+
+            if dir_name == '':
+                dir_name = os.getcwd()
+
+            sys.path.insert(0, dir_name)
+
+            options['app'] = getattr(import_module(module_name), attr_name)
+
+            if server_name != b'':
+                server_name = server_name + b' (ASGI)'
+
+            lifespan = ASGILifespan(options['app'], loop=self._loop, logger=self._logger)
+
+            lifespan.startup()
+            exc = await lifespan.exception()
+
+            if exc:
+                raise exc
+        else:
+            from .http_server import HTTPServer as Server
+
+            options['app'] = None
+            self._compile_handlers(options['handlers'])
 
         server = await self._loop.create_server(
-            lambda : HTTPServer(loop=self._loop,
-                                logger=self._logger,
-                                sock=sock,
-                                debug=options.get('debug', False),
-                                download_rate=options.get('download_rate', 1048576),
-                                upload_rate=options.get('upload_rate', 1048576),
-                                buffer_size=options.get('buffer_size', 16 * 1024),
-                                client_max_body_size=options.get('client_max_body_size', 2 * 1048576),
-                                request_timeout=options.get('request_timeout', 30),
-                                keepalive_timeout=options.get('keepalive_timeout', 30),
-                                server_name=server_name,
-                                _pool=pool,
-                                _handlers=options['handlers'],
-                                _middlewares=options['middlewares']), sock=sock, backlog=backlog, ssl=ssl_context)
+            lambda : Server(loop=self._loop,
+                            logger=self._logger,
+                            sock=sock,
+                            debug=options.get('debug', False),
+                            download_rate=options.get('download_rate', 1048576),
+                            upload_rate=options.get('upload_rate', 1048576),
+                            buffer_size=options.get('buffer_size', 16 * 1024),
+                            client_max_body_size=options.get('client_max_body_size', 2 * 1048576),
+                            request_timeout=options.get('request_timeout', 30),
+                            keepalive_timeout=options.get('keepalive_timeout', 30),
+                            server_name=server_name,
+                            _pool=pool,
+                            _app=options['app'],
+                            _handlers=options['handlers'],
+                            _middlewares=options['middlewares']), sock=sock, backlog=backlog, ssl=ssl_context)
 
         print(datetime.now().strftime('[%Y-%m-%d %H:%M:%S]'), end=' ')
         sys.stdout.flush()
         sys.stdout.buffer.write(b'%s (pid %d) is started at %s port %d' % (server_name, os.getpid(), host, port))
 
         if ssl_context is not None:
             sys.stdout.buffer.write(b' (https)')
@@ -246,17 +283,19 @@
                         break
 
                 process_num = options['conn'].recv()
             except (BrokenPipeError, ConnectionResetError, EOFError):
                 server.close()
                 break
 
-    def _worker(self, host, port, **kwargs):
-        self._compile_handlers(kwargs['handlers'])
+        if lifespan is not None:
+            lifespan.shutdown()
+            await lifespan.exception()
 
+    def _worker(self, host, port, **kwargs):
         self._logger = logging.getLogger(mp.current_process().name)
         self._logger.setLevel(getattr(logging, kwargs.get('log_level', 'DEBUG'), logging.DEBUG))
 
         handler = logging.StreamHandler()
         formatter = logging.Formatter('[%(asctime)s] %(levelname)s: %(message)s')
 
         handler.setFormatter(formatter)
```

### Comparing `tremolo-0.0.86/tremolo.egg-info/PKG-INFO` & `tremolo-0.0.88/tremolo.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tremolo
-Version: 0.0.86
+Version: 0.0.88
 Summary: Tremolo is a stream-oriented, asynchronous web server/framework written in pure Python
 Home-page: https://github.com/nggit/tremolo
 Author: nggit
 Author-email: contact@anggit.com
 License: MIT
 Description: # Tremolo
         
@@ -54,14 +54,53 @@
         
         Well, `latin-1` on the right side is not required. The default is `utf-8`.
         
         You can save it as `hello.py` and just run it with `python3 hello.py`.
         
         Your first *hello world* page with Tremolo will be at http://localhost:8000/hello.
         
+        ## ASGI Server
+        Tremolo is an HTTP Server framework. You can build abstractions on top of it, say an ASGI server.
+        
+        In fact, Tremolo already has ASGI server implementation.
+        
+        So you can immediately use existing [ASGI applications / frameworks](https://asgi.readthedocs.io/en/latest/implementations.html#application-frameworks), behind Tremolo (ASGI server).
+        
+        For example, If a minimal ASGI application with the name `example.py`:
+        
+        ```python
+        async def app(scope, receive, send):
+            assert scope['type'] == 'http'
+        
+            await send({
+                'type': 'http.response.start',
+                'status': 200,
+                'headers': [
+                    (b'content-type', b'text/plain'),
+                ]
+            })
+        
+            await send({
+                'type': 'http.response.body',
+                'body': b'Hello world!'
+            })
+        ```
+        
+        Then you can run as follows:
+        
+        ```
+        python3 -m tremolo --debug --bind 127.0.0.1:8000 example:app
+        ```
+        
+        To see more available options:
+        
+        ```
+        python3 -m tremolo --help
+        ```
+        
         ## Misc
         Tremolo utilizes `SO_REUSEPORT` (Linux 3.9+) to load balance worker processes.
         
         ```python
         app.run('0.0.0.0', 8000, worker_num=2)
         ```
```

