# Comparing `tmp/Flask-JSON-0.3.5.tar.gz` & `tmp/Flask-JSON-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/Flask-JSON-0.3.5.tar", last modified: Sat Nov 19 14:49:49 2022, max compression
+gzip compressed data, was "Flask-JSON-0.4.0.tar", last modified: Sat May  6 07:02:40 2023, max compression
```

## Comparing `Flask-JSON-0.3.5.tar` & `Flask-JSON-0.4.0.tar`

### file list

```diff
@@ -1,15 +1,25 @@
-drwxrwxr-x   0 skozlovf  (1000) skozlovf  (1000)        0 2022-11-19 14:49:49.000000 Flask-JSON-0.3.5/
-drwxrwxr-x   0 skozlovf  (1000) skozlovf  (1000)        0 2022-11-19 14:49:49.000000 Flask-JSON-0.3.5/Flask_JSON.egg-info/
--rw-r--r--   0 skozlovf  (1000) skozlovf  (1000)     3099 2022-11-19 14:49:49.000000 Flask-JSON-0.3.5/Flask_JSON.egg-info/PKG-INFO
--rw-r--r--   0 skozlovf  (1000) skozlovf  (1000)      265 2022-11-19 14:49:49.000000 Flask-JSON-0.3.5/Flask_JSON.egg-info/SOURCES.txt
--rw-r--r--   0 skozlovf  (1000) skozlovf  (1000)        1 2022-11-19 14:49:49.000000 Flask-JSON-0.3.5/Flask_JSON.egg-info/dependency_links.txt
--rw-r--r--   0 skozlovf  (1000) skozlovf  (1000)        1 2016-10-02 06:46:16.000000 Flask-JSON-0.3.5/Flask_JSON.egg-info/not-zip-safe
--rw-r--r--   0 skozlovf  (1000) skozlovf  (1000)       12 2022-11-19 14:49:49.000000 Flask-JSON-0.3.5/Flask_JSON.egg-info/requires.txt
--rw-r--r--   0 skozlovf  (1000) skozlovf  (1000)       11 2022-11-19 14:49:49.000000 Flask-JSON-0.3.5/Flask_JSON.egg-info/top_level.txt
--rw-r--r--   0 skozlovf  (1000) skozlovf  (1000)     1445 2016-10-02 06:36:50.000000 Flask-JSON-0.3.5/LICENSE
--rw-r--r--   0 skozlovf  (1000) skozlovf  (1000)       27 2016-10-02 06:36:50.000000 Flask-JSON-0.3.5/MANIFEST.in
--rw-rw-r--   0 skozlovf  (1000) skozlovf  (1000)     3099 2022-11-19 14:49:49.000000 Flask-JSON-0.3.5/PKG-INFO
--rw-r--r--   0 skozlovf  (1000) skozlovf  (1000)     1664 2022-11-19 14:46:20.000000 Flask-JSON-0.3.5/README.rst
--rw-rw-r--   0 skozlovf  (1000) skozlovf  (1000)    22118 2022-11-19 14:34:53.000000 Flask-JSON-0.3.5/flask_json.py
--rw-r--r--   0 skozlovf  (1000) skozlovf  (1000)       63 2022-11-19 14:49:49.000000 Flask-JSON-0.3.5/setup.cfg
--rw-rw-r--   0 skozlovf  (1000) skozlovf  (1000)     1426 2022-11-19 14:34:19.000000 Flask-JSON-0.3.5/setup.py
+drwxrwxr-x   0 skozlovf  (1000) skozlovf  (1000)        0 2023-05-06 07:02:40.956604 Flask-JSON-0.4.0/
+-rw-r--r--   0 skozlovf  (1000) skozlovf  (1000)     1445 2016-10-02 06:36:50.000000 Flask-JSON-0.4.0/LICENSE
+-rw-r--r--   0 skozlovf  (1000) skozlovf  (1000)       27 2016-10-02 06:36:50.000000 Flask-JSON-0.4.0/MANIFEST.in
+-rw-rw-r--   0 skozlovf  (1000) skozlovf  (1000)     3051 2023-05-06 07:02:40.956604 Flask-JSON-0.4.0/PKG-INFO
+-rw-r--r--   0 skozlovf  (1000) skozlovf  (1000)     1664 2022-11-19 14:46:20.000000 Flask-JSON-0.4.0/README.rst
+-rw-r--r--   0 skozlovf  (1000) skozlovf  (1000)       63 2023-05-06 07:02:40.956604 Flask-JSON-0.4.0/setup.cfg
+-rw-rw-r--   0 skozlovf  (1000) skozlovf  (1000)     1415 2023-05-03 06:19:42.000000 Flask-JSON-0.4.0/setup.py
+drwxrwxr-x   0 skozlovf  (1000) skozlovf  (1000)        0 2023-05-06 07:02:40.956604 Flask-JSON-0.4.0/src/
+drwxrwxr-x   0 skozlovf  (1000) skozlovf  (1000)        0 2023-05-06 07:02:40.956604 Flask-JSON-0.4.0/src/Flask_JSON.egg-info/
+-rw-rw-r--   0 skozlovf  (1000) skozlovf  (1000)     3051 2023-05-06 07:02:40.000000 Flask-JSON-0.4.0/src/Flask_JSON.egg-info/PKG-INFO
+-rw-rw-r--   0 skozlovf  (1000) skozlovf  (1000)      477 2023-05-06 07:02:40.000000 Flask-JSON-0.4.0/src/Flask_JSON.egg-info/SOURCES.txt
+-rw-rw-r--   0 skozlovf  (1000) skozlovf  (1000)        1 2023-05-06 07:02:40.000000 Flask-JSON-0.4.0/src/Flask_JSON.egg-info/dependency_links.txt
+-rw-rw-r--   0 skozlovf  (1000) skozlovf  (1000)        1 2023-05-03 06:19:47.000000 Flask-JSON-0.4.0/src/Flask_JSON.egg-info/not-zip-safe
+-rw-rw-r--   0 skozlovf  (1000) skozlovf  (1000)       13 2023-05-06 07:02:40.000000 Flask-JSON-0.4.0/src/Flask_JSON.egg-info/requires.txt
+-rw-rw-r--   0 skozlovf  (1000) skozlovf  (1000)       11 2023-05-06 07:02:40.000000 Flask-JSON-0.4.0/src/Flask_JSON.egg-info/top_level.txt
+-rw-rw-r--   0 skozlovf  (1000) skozlovf  (1000)    20666 2023-05-06 06:54:21.000000 Flask-JSON-0.4.0/src/flask_json.py
+drwxrwxr-x   0 skozlovf  (1000) skozlovf  (1000)        0 2023-05-06 07:02:40.956604 Flask-JSON-0.4.0/tests/
+-rw-r--r--   0 skozlovf  (1000) skozlovf  (1000)     9356 2023-04-15 18:22:37.000000 Flask-JSON-0.4.0/tests/test_as_json.py
+-rw-r--r--   0 skozlovf  (1000) skozlovf  (1000)     9912 2017-06-24 20:14:40.000000 Flask-JSON-0.4.0/tests/test_as_json_p.py
+-rw-r--r--   0 skozlovf  (1000) skozlovf  (1000)     2400 2022-11-19 19:46:24.000000 Flask-JSON-0.4.0/tests/test_decode.py
+-rw-r--r--   0 skozlovf  (1000) skozlovf  (1000)     7447 2023-04-29 18:18:18.000000 Flask-JSON-0.4.0/tests/test_encode.py
+-rw-r--r--   0 skozlovf  (1000) skozlovf  (1000)     2337 2017-06-24 19:39:46.000000 Flask-JSON-0.4.0/tests/test_error.py
+-rw-rw-r--   0 skozlovf  (1000) skozlovf  (1000)     2749 2022-11-19 19:39:10.000000 Flask-JSON-0.4.0/tests/test_init.py
+-rw-rw-r--   0 skozlovf  (1000) skozlovf  (1000)     2596 2022-11-20 07:06:43.000000 Flask-JSON-0.4.0/tests/test_jsonify_http_errors.py
+-rw-r--r--   0 skozlovf  (1000) skozlovf  (1000)     4800 2023-04-29 18:28:55.000000 Flask-JSON-0.4.0/tests/test_response.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `Flask-JSON-0.3.5/Flask_JSON.egg-info/PKG-INFO` & `Flask-JSON-0.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: Flask-JSON
-Version: 0.3.5
+Version: 0.4.0
 Summary: Better JSON support for Flask
 Home-page: https://github.com/skozlovf/flask-json
 Author: Sergey Kozlov
 Author-email: skozlovf@gmail.com
 License: BSD
 Description: Flask-JSON
         ==========
@@ -94,11 +94,10 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Flask
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `Flask-JSON-0.3.5/LICENSE` & `Flask-JSON-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `Flask-JSON-0.3.5/PKG-INFO` & `Flask-JSON-0.4.0/src/Flask_JSON.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: Flask-JSON
-Version: 0.3.5
+Version: 0.4.0
 Summary: Better JSON support for Flask
 Home-page: https://github.com/skozlovf/flask-json
 Author: Sergey Kozlov
 Author-email: skozlovf@gmail.com
 License: BSD
 Description: Flask-JSON
         ==========
@@ -94,11 +94,10 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Flask
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `Flask-JSON-0.3.5/README.rst` & `Flask-JSON-0.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `Flask-JSON-0.3.5/flask_json.py` & `Flask-JSON-0.4.0/src/flask_json.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,46 +1,28 @@
 """
     flask_json
     ~~~~~~~~~~
 
     A Flask extension providing better JSON support.
 
-    :copyright: (c) 2015 - 2017 by Sergey Kozlov
+    :copyright: (c) 2015 - 2022 by Sergey Kozlov
     :license: BSD, see LICENSE for more details.
 """
-from __future__ import absolute_import
-import sys
-try:
-    import collections.abc as collections_abc  # python 3.3+
-except ImportError:
-    import collections as collections_abc
+from collections.abc import Iterable
 from functools import partial, wraps
 from datetime import datetime, date, time
 try:
     from speaklater import _LazyString
-# Don't cover since simulated in test_encoder_nospeaklater().
 except ImportError:  # pragma: no cover
     _LazyString = None
 from werkzeug.exceptions import default_exceptions, BadRequest, HTTPException
-from flask import current_app, jsonify, request, Request, Response
-from flask import json
-
-__version__ = '0.3.5'
-
-
-if sys.version_info[0] == 2:
-    text_type = unicode
+from flask import current_app, jsonify, request, Request, Response, Flask
+from flask.json.provider import DefaultJSONProvider
 
-    def _is_str(value):
-        return isinstance(value, str) or isinstance(value, unicode)
-else:
-    text_type = str
-
-    def _is_str(value):
-        return isinstance(value, str)
+__version__ = '0.4.0'
 
 
 def json_response(status_=200, headers_=None, add_status_=None, data_=None,
                   **kwargs):
     """Helper function to build JSON response
     with the given HTTP status and fields(``kwargs``).
 
@@ -104,49 +86,48 @@
         `data_`: Data to put in result JSON. It can be used instead of
             ``kwargs`` or if you want to pass non-dictionary value.
         `kwargs`: keyword arguments to put in result JSON.
 
     Returns:
         flask.Response: Response with the JSON content.
 
-    Note:
-        Only ``data_`` or ``kwargs`` is allowed.
+    Notes:
+        If both ``data_`` and ``kwargs`` are passed then ``data_`` should be a
+        :class:`dict` (``kwargs`` will be merged into ``data_``).
 
         If ``data_`` is not a :class:`dict` then ``add_status_`` and
         :ref:`JSON_ADD_STATUS <opt_add_status>` are ignored and no status
         is stored in the result JSON.
 
-        If :class:`dict` is passed via ``data_`` then behaviour is like you
-        pass data in the keyword arguments.
+        Doesn't work for numeric keys if ``add_status_=True`` and
+        ``app.json.sort_keys=True``.
 
     .. versionchanged:: 0.3.2
        Added ``data_`` and non-dictionary values support.
     """
-    assert data_ is None or not kwargs
+    if data_ is None:
+        data_ = kwargs
+    elif isinstance(data_, dict):
+        if kwargs:
+            data_.update(kwargs)
+    else:
+        assert not kwargs
+        add_status_ = False
 
-    if isinstance(data_, dict):
-        kwargs = data_
-        data_ = None
-
-    if data_ is not None:
-        add_status = False
-    elif add_status_ is not None:
+    if add_status_ is not None:
         add_status = add_status_
     else:
         add_status = current_app.config['JSON_ADD_STATUS']
 
     if add_status:
         field = current_app.config['JSON_STATUS_FIELD_NAME']
         if field not in kwargs:
-            kwargs[field] = status_
+            data_[field] = status_
 
-    if data_ is None and not kwargs:
-        data_ = {}
-
-    response = jsonify(data_) if data_ is not None else jsonify(**kwargs)
+    response = jsonify(data_)
     response.status_code = status_
 
     if headers_ is not None:
         response.headers.extend(headers_)
 
     return response
 
@@ -169,15 +150,15 @@
 # Raises an error if the data is not convertible to JSON.
 def _build_response(data, add_status=None):
     if data is None:
         return json_response(add_status_=add_status)
     elif isinstance(data, dict):
         return json_response(add_status_=add_status, **data)
     elif isinstance(data, Response):
-        assert 'application/json' in data.mimetype
+        assert current_app.json.mimetype == data.mimetype
         return data
     elif isinstance(data, tuple):
         d, status, headers = _normalize_view_tuple(data)
         if isinstance(d, dict):
             return json_response(status_=status or 200, headers_=headers,
                                  add_status_=add_status, **d)
         else:
@@ -260,27 +241,27 @@
         if optional:
             return _build_response(rv)
         else:
             raise BadRequest('Missing JSONP callback parameter.')
 
     # NOTE: flask 0.11 adds '\n' to the end but we don't need it here.
 
-    if _is_str(rv):
+    if isinstance(rv, str):
         if rv.endswith('\n'):  # pragma: no cover
             rv = rv[:-1]
         if add_quotes:
             data = '"%s"' % rv.replace('"', '\\"')
         else:
             data = '%s' % rv
     else:
         data = _build_response(rv, add_status=False).get_data(as_text=True)
         if data.endswith('\n'):  # pragma: no cover
             data = data[:-1]
 
-    data = text_type('%s(%s);') % (callback, data)
+    data = str('%s(%s);') % (callback, data)
     response = current_app.response_class(
         data, status=200, content_type='application/javascript')
     return response
 
 
 def as_json_p(f=None, callbacks=None, optional=None, add_quotes=None):
     """This decorator acts like :func:`@as_json <flask_json.as_json>` but
@@ -387,15 +368,15 @@
         super(JsonError, self).__init__()
         assert status_ != 200
         self.status = status_
         self.headers = headers_
         self.data = kwargs
 
 
-class JsonRequest(Request):
+class FlaskJSONRequest(Request):
     """This class changes :class:`flask.Request` behaviour on JSON parse
     errors.
 
     :meth:`flask.Request.get_json` will raise :class:`.JsonError`
     by default on invalid JSON content.
 
     See Also:
@@ -406,126 +387,39 @@
         # Try decoder error hook firstly; see FlaskJSON.invalid_json_error().
         func = current_app.extensions['json']._decoder_error_func
         if func is not None:
             response = func(e)
             if response is not None:
                 return response
 
-        # By default we raise json error with description.
+        # By default, we raise json error with description.
         # If there is no description config or it's text is empty then
         # raise without a description.
         desc = current_app.config.get('JSON_DECODE_ERROR_MESSAGE')
         if desc:
             raise JsonError(description=desc)
         else:
             raise JsonError()
 
 
-class JSONEncoderEx(json.JSONEncoder):
-    """Extends default Flask JSON encoder with more types:
-
-    * iterable;
-    * :class:`~datetime.datetime`;
-    * :class:`~datetime.date`;
-    * :class:`~datetime.time`;
-    * `speaklater <https://pypi.python.org/pypi/speaklater>`_ lazy strings;
-    * objects with ``__json__()`` or ``for_json()`` methods.
-
-    Time related values will be converted to ISO 8601 format by default.
-
-    See Also:
-        :ref:`JSON_DATETIME_FORMAT <opt_fmt_datetime>`,
-        :ref:`JSON_DATE_FORMAT <opt_fmt_date>`,
-        :ref:`JSON_TIME_FORMAT <opt_fmt_time>`,
-        :ref:`JSON_USE_ENCODE_METHODS <opt_use_enc_methods>`.
-    """
-    def default(self, o):
-        # We have to test _LazyString before Iterable to prevent
-        # converting string to list of chars, since string is iterable too.
-        if _LazyString is not None and isinstance(o, _LazyString):
-            return text_type(o)
-        elif isinstance(o, collections_abc.Iterable):
-            # All iterables will be converted to list.
-            return list(o)
-        elif isinstance(o, datetime):
-            fmt = current_app.config.get('JSON_DATETIME_FORMAT')
-            return o.strftime(fmt) if fmt else o.isoformat()
-        elif isinstance(o, date):
-            fmt = current_app.config.get('JSON_DATE_FORMAT')
-            return o.strftime(fmt) if fmt else o.isoformat()
-        elif isinstance(o, time):
-            fmt = current_app.config.get('JSON_TIME_FORMAT')
-            return o.strftime(fmt) if fmt else o.isoformat()
-        elif current_app.config.get('JSON_USE_ENCODE_METHODS'):
-            if hasattr(o, '__json__'):
-                return o.__json__()
-            elif hasattr(o, 'for_json'):
-                return o.for_json()
-        return super(JSONEncoderEx, self).default(o)
-
-
-class JsonTestResponse(Response):
-    """JSON Response class for testing.
-
-    It provides convenient access to JSON content without explicit response
-    data decoding.
-
-    Flask-JSON replaces Flask's response class with this one
-    on initialization if testing mode enabled.
-
-    Usage:
-
-    .. code-block:: py
-
-        app = Flask()
-        app.config['TESTING'] = True
-        FlaskJSON(app)
-        ...
-        client = app.test_client()
-        r = client.get('/view')  # suppose it returns json_response(param='12)
-        assert r.json['param'] == 12
-
-    If you enable testing after Flask-JSON initialization the you have to
-    set :class:`.JsonTestResponse` by yourself:
-
-    .. code-block:: py
-
-        app = Flask()
-        FlaskJSON(app)
-        app.config['TESTING'] = True
-        app.response_class = JsonTestResponse
-
-    """
-    _json_cache = None
-
-    @property
-    def json(self):
-        """Response JSON content."""
-        if self._json_cache is None:
-            assert self.mimetype == 'application/json'
-            self._json_cache = json.loads(self.data)
-        return self._json_cache
-
-
 class FlaskJSON(object):
     """Flask-JSON extension class."""
-    def __init__(self, app=None):
-        self._app = app
+    def __init__(self, app: Flask = None):
         self._error_handler_func = None
         self._decoder_error_func = None
-        self._encoder_class = JSONEncoderEx
+        self._encoders = [_encoder, DefaultJSONProvider.default]
         if app is not None:
             self.init_app(app)
 
     def _error_handler(self, e):
         if self._error_handler_func is not None:
             return self._error_handler_func(e)
         return json_response(e.status, e.headers, **e.data)
 
-    def init_app(self, app):
+    def init_app(self, app: Flask):
         """Initializes the application with the extension.
 
         Args:
             app: Flask application object.
         """
         app.config.setdefault('JSON_ADD_STATUS', True)
         app.config.setdefault('JSON_STATUS_FIELD_NAME', 'status')
@@ -534,29 +428,24 @@
             'JSON_JSONIFY_HTTP_ERRORS', False)
 
         app.config.setdefault('JSON_JSONP_STRING_QUOTES', True)
         app.config.setdefault('JSON_JSONP_OPTIONAL', True)
         app.config.setdefault('JSON_JSONP_QUERY_CALLBACKS',
                               ['callback', 'jsonp'])
 
-        if not hasattr(app, 'extensions'):
-            app.extensions = dict()
         app.extensions['json'] = self
 
-        self._app = app
-        app.request_class = JsonRequest
-        app.json_encoder = self._encoder_class
+        app.json_provider_class = FlaskJSONProvider
+        app.json = FlaskJSONProvider(app)
+        app.request_class = FlaskJSONRequest
         app.errorhandler(JsonError)(self._error_handler)
 
         if jsonify_errors:
             self._jsonify_http_errors(app)
 
-        if app.testing:
-            app.response_class = JsonTestResponse
-
     def _jsonify_http_errors(self, app):
         """Force HTTP errors returned as JSON instead of default HTML."""
         status_field = app.config['JSON_STATUS_FIELD_NAME']
 
         def _handler(error, status_code, reason, default_description):
             response = {
                 'reason': reason,
@@ -622,56 +511,114 @@
                 json = FlaskJson(app)
                 ...
 
                 @json.invalid_json_error
                 def invalid_json_error(e):
                     raise SomeException
 
-        By default JSON response will be generated with HTTP 400::
+        By default, JSON response will be generated with HTTP 400::
 
             {"status": 400, "description": "Not a JSON."}
 
         You also may return a value from the handler then it will be used as
         :meth:`request.get_json() <flask.Request.get_json>` result on errors.
 
         See Also:
             :ref:`JSON_DECODE_ERROR_MESSAGE <opt_decode_error_msg>`
         """
         self._decoder_error_func = func
         return func
 
     def encoder(self, func):
-        """This decorator allows to set extra JSON encoding step on response
-        building.
+        """Add extra JSON encoding step on response building.
 
         JSON encoding order:
 
         * User defined encoding.
         * Flask-JSON encoding.
         * Flask encoding.
 
         If user defined encoder returns None then default encoders takes place
         (Flask-JSON and then Flask).
 
-        Example:
+        Examples:
 
             ::
 
                 json = FlaskJson(app)
                 ...
 
                 @json.encoder
                 def custom_encoder(o):
                     if isinstance(o, MyClass):
                         return o.to_string()
+
         """
-        class JSONEncoderWithHook(JSONEncoderEx):
-            def default(self, o):
-                result = func(o)
-                if result is not None:
-                    return result
-                return JSONEncoderEx.default(self, o)
-        if self._app is not None:
-            self._app.json_encoder = JSONEncoderWithHook
-        else:
-            self._encoder_class = JSONEncoderWithHook
+        self._encoders.insert(0, func)
         return func
+
+
+def _encoder(o):
+    # We have to test _LazyString before Iterable to prevent
+    # converting string to list of chars, since string is iterable too.
+    if _LazyString is not None and isinstance(o, _LazyString):
+        return str(o)
+    elif isinstance(o, Iterable):
+        # All iterables will be converted to list.
+        return list(o)
+    elif isinstance(o, datetime):
+        fmt = current_app.config.get('JSON_DATETIME_FORMAT')
+        if fmt == 'iso':
+            return o.isoformat()
+        elif fmt:
+            return o.strftime(fmt)
+    elif isinstance(o, date):
+        fmt = current_app.config.get('JSON_DATE_FORMAT')
+        if fmt == 'iso':
+            return o.isoformat()
+        elif fmt:
+            return o.strftime(fmt)
+    elif isinstance(o, time):
+        fmt = current_app.config.get('JSON_TIME_FORMAT')
+        return o.strftime(fmt) if fmt else o.isoformat()
+    elif current_app.config.get('JSON_USE_ENCODE_METHODS'):
+        try:
+            m = o.__json__
+        except AttributeError:
+            try:
+                m = o.for_json
+            except AttributeError:
+                return
+        return m()
+
+
+class FlaskJSONProvider(DefaultJSONProvider):
+    """Extends default Flask JSON provider with more types.
+
+    * iterable;
+    * :class:`~datetime.datetime`;
+    * :class:`~datetime.date`;
+    * :class:`~datetime.time`;
+    * `speaklater <https://pypi.python.org/pypi/speaklater>`_ lazy strings;
+    * objects with ``__json__()`` or ``for_json()`` methods.
+
+    Time related values will be converted to ISO 8601 format by default.
+
+    See Also:
+        :ref:`JSON_DATETIME_FORMAT <opt_fmt_datetime>`,
+        :ref:`JSON_DATE_FORMAT <opt_fmt_date>`,
+        :ref:`JSON_TIME_FORMAT <opt_fmt_time>`,
+        :ref:`JSON_USE_ENCODE_METHODS <opt_use_enc_methods>`.
+    """
+
+    @staticmethod
+    def default(o):
+        for func in current_app.extensions['json']._encoders:
+            val = func(o)
+            if val is not None:
+                return val
+        # NOTE: flask's converter raises an error, so this line is unreachable.
+        raise TypeError(f"Object of type {type(o).__name__} is not JSON serializable")  # pragma: no cover
+
+    def _prepare_response_obj(self, args, kwargs):
+        obj = super(FlaskJSONProvider, self)._prepare_response_obj(args, kwargs)
+        return obj if obj is not None else {}
```

### Comparing `Flask-JSON-0.3.5/setup.py` & `Flask-JSON-0.4.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 def read(name, only_open=False):
     f = open(op.join(op.dirname(__file__), name))
     return f if only_open else f.read()
 
 
 ext_version = None
-with read('flask_json.py', only_open=True) as f:
+with read('src/flask_json.py', only_open=True) as f:
     for line in f:
         if line.startswith('__version__'):
             ext_version,  = re.findall(r"__version__\W*=\W*'([^']+)'", line)
             break
 
 
 setup(
@@ -21,27 +21,27 @@
     version=ext_version,
     url='https://github.com/skozlovf/flask-json',
     license='BSD',
     author='Sergey Kozlov',
     author_email='skozlovf@gmail.com',
     description='Better JSON support for Flask',
     long_description=read('README.rst'),
+    package_dir = {"": "src"},
     py_modules=['flask_json'],
     zip_safe=False,
     include_package_data=True,
     platforms='any',
-    install_requires=['Flask>=0.10'],
+    install_requires=['Flask>=2.2.0'],
     classifiers=[
         'Development Status :: 4 - Beta',
         'Environment :: Web Environment',
         'Framework :: Flask',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: BSD License',
         'Operating System :: OS Independent',
         'Programming Language :: Python',
-        'Programming Language :: Python :: 2',
         'Programming Language :: Python :: 3',
         'Topic :: Internet :: WWW/HTTP :: Dynamic Content',
         'Topic :: Software Development :: Libraries :: Python Modules'
     ],
     tests_require=['pytest', 'pytest-cov']
 )
```

