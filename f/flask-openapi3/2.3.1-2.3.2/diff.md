# Comparing `tmp/flask-openapi3-2.3.1.tar.gz` & `tmp/flask-openapi3-2.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask-openapi3-2.3.1.tar", last modified: Mon Feb 13 06:08:35 2023, max compression
+gzip compressed data, was "flask-openapi3-2.3.2.tar", last modified: Mon Apr  3 02:25:04 2023, max compression
```

## Comparing `flask-openapi3-2.3.1.tar` & `flask-openapi3-2.3.2.tar`

### file list

```diff
@@ -1,77 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 06:08:35.864249 flask-openapi3-2.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)     5991 2023-02-13 06:08:24.000000 flask-openapi3-2.3.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-02-13 06:08:24.000000 flask-openapi3-2.3.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-02-13 06:08:24.000000 flask-openapi3-2.3.1/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)      164 2023-02-13 06:08:24.000000 flask-openapi3-2.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7524 2023-02-13 06:08:35.864249 flask-openapi3-2.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6432 2023-02-13 06:08:24.000000 flask-openapi3-2.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 06:08:35.856249 flask-openapi3-2.3.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-02-13 06:08:24.000000 flask-openapi3-2.3.1/examples/api_blueprint_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-02-13 06:08:24.000000 flask-openapi3-2.3.1/examples/api_view_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-02-13 06:08:24.000000 flask-openapi3-2.3.1/examples/async_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-02-13 06:08:24.000000 flask-openapi3-2.3.1/examples/custom_ui_templates_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-02-13 06:08:24.000000 flask-openapi3-2.3.1/examples/enum_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      662 2023-02-13 06:08:24.000000 flask-openapi3-2.3.1/examples/header_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-02-13 06:08:24.000000 flask-openapi3-2.3.1/examples/image_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-02-13 06:08:24.000000 flask-openapi3-2.3.1/examples/init_oauth_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-02-13 06:08:24.000000 flask-openapi3-2.3.1/examples/just_flask.py
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-02-13 06:08:24.000000 flask-openapi3-2.3.1/examples/nested_apiblueprint_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-02-13 06:08:24.000000 flask-openapi3-2.3.1/examples/orjson_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-02-13 06:08:24.000000 flask-openapi3-2.3.1/examples/pydantic_custom_root_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-02-13 06:08:24.000000 flask-openapi3-2.3.1/examples/response_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-02-13 06:08:24.000000 flask-openapi3-2.3.1/examples/rest_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-02-13 06:08:24.000000 flask-openapi3-2.3.1/examples/servers_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-02-13 06:08:24.000000 flask-openapi3-2.3.1/examples/simple_demo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-02-13 06:08:24.000000 flask-openapi3-2.3.1/examples/upload_file_demo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 06:08:35.856249 flask-openapi3-2.3.1/flask_openapi3/
--rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-02-13 06:08:24.000000 flask-openapi3-2.3.1/flask_openapi3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-02-13 06:08:24.000000 flask-openapi3-2.3.1/flask_openapi3/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6902 2023-02-13 06:08:24.000000 flask-openapi3-2.3.1/flask_openapi3/blueprint.py
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-02-13 06:08:24.000000 flask-openapi3-2.3.1/flask_openapi3/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-02-13 06:08:24.000000 flask-openapi3-2.3.1/flask_openapi3/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-02-13 06:08:24.000000 flask-openapi3-2.3.1/flask_openapi3/markdown.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 06:08:35.860249 flask-openapi3-2.3.1/flask_openapi3/models/
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-02-13 06:08:24.000000 flask-openapi3-2.3.1/flask_openapi3/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-02-13 06:08:24.000000 flask-openapi3-2.3.1/flask_openapi3/models/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-02-13 06:08:24.000000 flask-openapi3-2.3.1/flask_openapi3/models/component.py
--rw-r--r--   0 runner    (1001) docker     (123)      987 2023-02-13 06:08:24.000000 flask-openapi3-2.3.1/flask_openapi3/models/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      723 2023-02-13 06:08:24.000000 flask-openapi3-2.3.1/flask_openapi3/models/info.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-02-13 06:08:24.000000 flask-openapi3-2.3.1/flask_openapi3/models/oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-02-13 06:08:24.000000 flask-openapi3-2.3.1/flask_openapi3/models/path.py
--rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-02-13 06:08:24.000000 flask-openapi3-2.3.1/flask_openapi3/models/security.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-02-13 06:08:24.000000 flask-openapi3-2.3.1/flask_openapi3/models/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      407 2023-02-13 06:08:24.000000 flask-openapi3-2.3.1/flask_openapi3/models/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)      823 2023-02-13 06:08:24.000000 flask-openapi3-2.3.1/flask_openapi3/models/validation_error.py
--rw-r--r--   0 runner    (1001) docker     (123)    12633 2023-02-13 06:08:24.000000 flask-openapi3-2.3.1/flask_openapi3/openapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     4394 2023-02-13 06:08:24.000000 flask-openapi3-2.3.1/flask_openapi3/request.py
--rw-r--r--   0 runner    (1001) docker     (123)    19080 2023-02-13 06:08:24.000000 flask-openapi3-2.3.1/flask_openapi3/scaffold.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 06:08:35.860249 flask-openapi3-2.3.1/flask_openapi3/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-02-13 06:08:24.000000 flask-openapi3-2.3.1/flask_openapi3/templates/openapi.html
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-02-13 06:08:24.000000 flask-openapi3-2.3.1/flask_openapi3/templates/rapidoc.html
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-02-13 06:08:24.000000 flask-openapi3-2.3.1/flask_openapi3/templates/redoc.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 06:08:35.856249 flask-openapi3-2.3.1/flask_openapi3/templates/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 06:08:35.860249 flask-openapi3-2.3.1/flask_openapi3/templates/static/css/
--rw-r--r--   0 runner    (1001) docker     (123)   144726 2023-02-13 06:08:24.000000 flask-openapi3-2.3.1/flask_openapi3/templates/static/css/swagger-ui.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 06:08:35.860249 flask-openapi3-2.3.1/flask_openapi3/templates/static/images/
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-02-13 06:08:24.000000 flask-openapi3-2.3.1/flask_openapi3/templates/static/images/apidoc.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-02-13 06:08:24.000000 flask-openapi3-2.3.1/flask_openapi3/templates/static/images/rapidoc.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-02-13 06:08:24.000000 flask-openapi3-2.3.1/flask_openapi3/templates/static/images/redoc.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-02-13 06:08:24.000000 flask-openapi3-2.3.1/flask_openapi3/templates/static/images/swagger.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 06:08:35.864249 flask-openapi3-2.3.1/flask_openapi3/templates/static/js/
--rw-r--r--   0 runner    (1001) docker     (123)   620595 2023-02-13 06:08:24.000000 flask-openapi3-2.3.1/flask_openapi3/templates/static/js/rapidoc-min.js
--rw-r--r--   0 runner    (1001) docker     (123)  1042510 2023-02-13 06:08:24.000000 flask-openapi3-2.3.1/flask_openapi3/templates/static/js/redoc.standalone.js
--rw-r--r--   0 runner    (1001) docker     (123)  1061567 2023-02-13 06:08:24.000000 flask-openapi3-2.3.1/flask_openapi3/templates/static/js/swagger-ui-bundle.js
--rw-r--r--   0 runner    (1001) docker     (123)   312217 2023-02-13 06:08:24.000000 flask-openapi3-2.3.1/flask_openapi3/templates/static/js/swagger-ui-standalone-preset.js
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-02-13 06:08:24.000000 flask-openapi3-2.3.1/flask_openapi3/templates/swagger.html
--rw-r--r--   0 runner    (1001) docker     (123)    15442 2023-02-13 06:08:24.000000 flask-openapi3-2.3.1/flask_openapi3/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7502 2023-02-13 06:08:24.000000 flask-openapi3-2.3.1/flask_openapi3/view.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-13 06:08:35.856249 flask-openapi3-2.3.1/flask_openapi3.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7524 2023-02-13 06:08:35.000000 flask-openapi3-2.3.1/flask_openapi3.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2054 2023-02-13 06:08:35.000000 flask-openapi3-2.3.1/flask_openapi3.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-13 06:08:35.000000 flask-openapi3-2.3.1/flask_openapi3.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-13 06:08:35.000000 flask-openapi3-2.3.1/flask_openapi3.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-02-13 06:08:35.000000 flask-openapi3-2.3.1/flask_openapi3.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-02-13 06:08:35.000000 flask-openapi3-2.3.1/flask_openapi3.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-02-13 06:08:24.000000 flask-openapi3-2.3.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-13 06:08:35.864249 flask-openapi3-2.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-02-13 06:08:24.000000 flask-openapi3-2.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 02:25:04.696719 flask-openapi3-2.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     6111 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      164 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7542 2023-04-03 02:25:04.696719 flask-openapi3-2.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6450 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 02:25:04.692719 flask-openapi3-2.3.2/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     1704 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/examples/api_blueprint_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/examples/api_view_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/examples/async_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2489 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/examples/custom_ui_templates_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/examples/enum_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/examples/header_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/examples/image_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/examples/init_oauth_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/examples/just_flask.py
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/examples/nested_apiblueprint_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/examples/orjson_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1392 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/examples/pydantic_custom_root_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/examples/response_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4546 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/examples/rest_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/examples/servers_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/examples/simple_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/examples/upload_file_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 02:25:04.692719 flask-openapi3-2.3.2/flask_openapi3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1839 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/flask_openapi3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/flask_openapi3/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6905 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/flask_openapi3/blueprint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/flask_openapi3/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/flask_openapi3/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/flask_openapi3/markdown.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 02:25:04.692719 flask-openapi3-2.3.2/flask_openapi3/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/flask_openapi3/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/flask_openapi3/models/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/flask_openapi3/models/component.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/flask_openapi3/models/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      723 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/flask_openapi3/models/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/flask_openapi3/models/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3874 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/flask_openapi3/models/path.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1885 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/flask_openapi3/models/security.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/flask_openapi3/models/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/flask_openapi3/models/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)      823 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/flask_openapi3/models/validation_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11733 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/flask_openapi3/openapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/flask_openapi3/request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19084 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/flask_openapi3/scaffold.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 02:25:04.692719 flask-openapi3-2.3.2/flask_openapi3/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     5814 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/flask_openapi3/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 02:25:04.688719 flask-openapi3-2.3.2/flask_openapi3/templates/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 02:25:04.692719 flask-openapi3-2.3.2/flask_openapi3/templates/static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)   144726 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/flask_openapi3/templates/static/css/swagger-ui.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 02:25:04.696719 flask-openapi3-2.3.2/flask_openapi3/templates/static/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/flask_openapi3/templates/static/images/apidoc.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/flask_openapi3/templates/static/images/rapidoc.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/flask_openapi3/templates/static/images/redoc.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2551 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/flask_openapi3/templates/static/images/swagger.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 02:25:04.696719 flask-openapi3-2.3.2/flask_openapi3/templates/static/js/
+-rw-r--r--   0 runner    (1001) docker     (123)   620595 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/flask_openapi3/templates/static/js/rapidoc-min.js
+-rw-r--r--   0 runner    (1001) docker     (123)  1042510 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/flask_openapi3/templates/static/js/redoc.standalone.js
+-rw-r--r--   0 runner    (1001) docker     (123)  1061567 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/flask_openapi3/templates/static/js/swagger-ui-bundle.js
+-rw-r--r--   0 runner    (1001) docker     (123)   312217 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/flask_openapi3/templates/static/js/swagger-ui-standalone-preset.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15444 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/flask_openapi3/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7503 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/flask_openapi3/view.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-03 02:25:04.692719 flask-openapi3-2.3.2/flask_openapi3.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7542 2023-04-03 02:25:04.000000 flask-openapi3-2.3.2/flask_openapi3.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-04-03 02:25:04.000000 flask-openapi3-2.3.2/flask_openapi3.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 02:25:04.000000 flask-openapi3-2.3.2/flask_openapi3.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-03 02:25:04.000000 flask-openapi3-2.3.2/flask_openapi3.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-03 02:25:04.000000 flask-openapi3-2.3.2/flask_openapi3.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-03 02:25:04.000000 flask-openapi3-2.3.2/flask_openapi3.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-03 02:25:04.696719 flask-openapi3-2.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2362 2023-04-03 02:24:50.000000 flask-openapi3-2.3.2/setup.py
```

### Comparing `flask-openapi3-2.3.1/CHANGELOG.md` & `flask-openapi3-2.3.2/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,11 @@
+## v2.3.2 2023-04-03
+
+- [#61](https://github.com/luolingchun/flask-openapi3/issues/61) Fix headers with pydantic alias
+
 ## v2.3.1 2023-02-13
 
 - remove * in install_requires for setuptools 67+
 
 ## v2.3.0 2023-02-12
 
 - Support custom UI templates (#55)
```

### Comparing `flask-openapi3-2.3.1/CONTRIBUTING.md` & `flask-openapi3-2.3.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.3.1/LICENSE.rst` & `flask-openapi3-2.3.2/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.3.1/PKG-INFO` & `flask-openapi3-2.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-openapi3
-Version: 2.3.1
+Version: 2.3.2
 Summary: Generate REST API and OpenAPI documentation for your Flask project.
 Home-page: https://github.com/luolingchun/flask-openapi3
 Author: llc
 Author-email: luolingchun@outlook.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -67,15 +67,15 @@
 
 - **Authorization:** Support to reload authorizations in Swagger UI
 
 ## Requirements
 
 Python 3.7+
 
-flask-openapi3 be dependent on the following libraries:
+flask-openapi3 is dependent on the following libraries:
 
 - [Flask](https://github.com/pallets/flask) for the web app.
 - [Pydantic](https://github.com/pydantic/pydantic) for the data validation.
 
 ## Installation
 
 ```bash
@@ -130,18 +130,18 @@
 
 
 class BookQuery(BaseModel):
     age: int
     author: str
 
 
-@app.get("/book", tags=[book_tag])
+@app.get("/book", summary="get books", tags=[book_tag])
 def get_book(query: BookQuery):
-    """get books
-    get all books
+    """
+    to get all books
     """
     return {
         "code": 0,
         "message": "ok",
         "data": [
             {"bid": 1, "age": query.age, "author": query.author},
             {"bid": 2, "age": query.age, "author": query.author}
@@ -190,15 +190,15 @@
     @api_view.doc(summary="get book list")
     def get(self, query: BookQuery):
         print(self.a)
         return query.json()
 
     @api_view.doc(summary="create book")
     def post(self, body: BookBody):
-        """description for create book"""
+        """description for a created book"""
         return body.json()
 
 
 @api_view.route("/book/<id>")
 class BookAPIView:
     @api_view.doc(summary="get book")
     def get(self, path: BookPath):
```

### Comparing `flask-openapi3-2.3.1/README.md` & `flask-openapi3-2.3.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 
 - **Authorization:** Support to reload authorizations in Swagger UI
 
 ## Requirements
 
 Python 3.7+
 
-flask-openapi3 be dependent on the following libraries:
+flask-openapi3 is dependent on the following libraries:
 
 - [Flask](https://github.com/pallets/flask) for the web app.
 - [Pydantic](https://github.com/pydantic/pydantic) for the data validation.
 
 ## Installation
 
 ```bash
@@ -100,18 +100,18 @@
 
 
 class BookQuery(BaseModel):
     age: int
     author: str
 
 
-@app.get("/book", tags=[book_tag])
+@app.get("/book", summary="get books", tags=[book_tag])
 def get_book(query: BookQuery):
-    """get books
-    get all books
+    """
+    to get all books
     """
     return {
         "code": 0,
         "message": "ok",
         "data": [
             {"bid": 1, "age": query.age, "author": query.author},
             {"bid": 2, "age": query.age, "author": query.author}
@@ -160,15 +160,15 @@
     @api_view.doc(summary="get book list")
     def get(self, query: BookQuery):
         print(self.a)
         return query.json()
 
     @api_view.doc(summary="create book")
     def post(self, body: BookBody):
-        """description for create book"""
+        """description for a created book"""
         return body.json()
 
 
 @api_view.route("/book/<id>")
 class BookAPIView:
     @api_view.doc(summary="get book")
     def get(self, path: BookPath):
```

### Comparing `flask-openapi3-2.3.1/examples/api_blueprint_demo.py` & `flask-openapi3-2.3.2/examples/api_blueprint_demo.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.3.1/examples/api_view_demo.py` & `flask-openapi3-2.3.2/examples/api_view_demo.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.3.1/examples/async_demo.py` & `flask-openapi3-2.3.2/examples/async_demo.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.3.1/examples/custom_ui_templates_demo.py` & `flask-openapi3-2.3.2/examples/custom_ui_templates_demo.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.3.1/examples/enum_demo.py` & `flask-openapi3-2.3.2/examples/enum_demo.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.3.1/examples/header_demo.py` & `flask-openapi3-2.3.2/examples/header_demo.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 book_tag = Tag(name='book', description='Some Book')
 
 
 class Headers(BaseModel):
     hello: str = Field("what's up", max_length=12, description='sds')
     # required
     # hello: str = Field(..., max_length=12, description='sds')
+    x_hello: str = Field(..., max_length=12, description='Header with alias to support dash', alias="x-hello")
 
 
 @app.get('/book', tags=[book_tag])
 def get_book(header: Headers):
     print(header)
     return header.hello
```

### Comparing `flask-openapi3-2.3.1/examples/init_oauth_demo.py` & `flask-openapi3-2.3.2/examples/init_oauth_demo.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.3.1/examples/nested_apiblueprint_demo.py` & `flask-openapi3-2.3.2/examples/nested_apiblueprint_demo.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.3.1/examples/orjson_demo.py` & `flask-openapi3-2.3.2/examples/orjson_demo.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.3.1/examples/pydantic_custom_root_types.py` & `flask-openapi3-2.3.2/examples/pydantic_custom_root_types.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.3.1/examples/response_demo.py` & `flask-openapi3-2.3.2/examples/response_demo.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.3.1/examples/rest_demo.py` & `flask-openapi3-2.3.2/examples/rest_demo.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.3.1/examples/servers_demo.py` & `flask-openapi3-2.3.2/examples/servers_demo.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.3.1/examples/simple_demo.py` & `flask-openapi3-2.3.2/examples/simple_demo.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,35 +2,35 @@
 # @Author  : llc
 # @Time    : 2021/5/10 17:01
 from pydantic import BaseModel
 
 from flask_openapi3 import Info, Tag
 from flask_openapi3 import OpenAPI
 
-info = Info(title='book API', version='1.0.0')
+info = Info(title="book API", version="1.0.0")
 app = OpenAPI(__name__, info=info)
 
-book_tag = Tag(name='book', description='Some Book')
+book_tag = Tag(name="book", description="Some Book")
 
 
 class BookQuery(BaseModel):
     age: int
     author: str
 
 
-@app.get('/book', tags=[book_tag])
+@app.get("/book", summary="get books", tags=[book_tag])
 def get_book(query: BookQuery):
-    """get books
+    """
     get all books
     """
     return {
         "code": 0,
         "message": "ok",
         "data": [
             {"bid": 1, "age": query.age, "author": query.author},
             {"bid": 2, "age": query.age, "author": query.author}
         ]
     }
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     app.run(debug=True)
```

### Comparing `flask-openapi3-2.3.1/examples/upload_file_demo.py` & `flask-openapi3-2.3.2/examples/upload_file_demo.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.3.1/flask_openapi3/__init__.py` & `flask-openapi3-2.3.2/flask_openapi3/__init__.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.3.1/flask_openapi3/blueprint.py` & `flask-openapi3-2.3.2/flask_openapi3/blueprint.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
             doc_ui: bool = True,
             **kwargs: Any
     ) -> None:
         """
         Based on Flask Blueprint
 
         Arguments:
-            name: The name of the blueprint. Will be prepended to each endpoint name.
+            name: The name of the blueprint. It Will be prepared to each endpoint name.
             import_name: The name of the blueprint package, usually
                          ``__name__``. This helps locate the ``root_path`` for the blueprint.
             abp_tags: APIBlueprint tags for every api
             abp_security: APIBlueprint security for every api
             abp_responses: APIBlueprint response model
             doc_ui: Add openapi document UI(swagger, rapidoc and redoc). Defaults to True.
             **kwargs: Flask Blueprint kwargs
@@ -99,16 +99,16 @@
         Collect openapi specification information
         :param rule: flask route
         :param func: flask view_func
         :param tags: api tag
         :param responses: response model
         :param extra_responses: extra response dict
         :param security: security name
-        :param doc_ui: add openapi document UI(swagger and redoc). Defaults to True.
-        :param deprecated: mark as deprecated support. Default to not True.
+        :param doc_ui: adds openapi document UI(swagger and redoc). defaults to True.
+        :param deprecated: mark as deprecated support. default to not True.
         :param operation_id: unique string used to identify the operation.
         :param method: api method
         :return:
         """
         if self.doc_ui is True and doc_ui is True:
             if responses is None:
                 responses = {}
```

### Comparing `flask-openapi3-2.3.1/flask_openapi3/commands.py` & `flask-openapi3-2.3.2/flask_openapi3/commands.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.3.1/flask_openapi3/http.py` & `flask-openapi3-2.3.2/flask_openapi3/http.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.3.1/flask_openapi3/markdown.py` & `flask-openapi3-2.3.2/flask_openapi3/markdown.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.3.1/flask_openapi3/models/__init__.py` & `flask-openapi3-2.3.2/flask_openapi3/models/__init__.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.3.1/flask_openapi3/models/common.py` & `flask-openapi3-2.3.2/flask_openapi3/models/common.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.3.1/flask_openapi3/models/component.py` & `flask-openapi3-2.3.2/flask_openapi3/models/component.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.3.1/flask_openapi3/models/file.py` & `flask-openapi3-2.3.2/flask_openapi3/models/file.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.3.1/flask_openapi3/models/info.py` & `flask-openapi3-2.3.2/flask_openapi3/models/info.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.3.1/flask_openapi3/models/oauth.py` & `flask-openapi3-2.3.2/flask_openapi3/models/oauth.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.3.1/flask_openapi3/models/path.py` & `flask-openapi3-2.3.2/flask_openapi3/models/path.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.3.1/flask_openapi3/models/security.py` & `flask-openapi3-2.3.2/flask_openapi3/models/security.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.3.1/flask_openapi3/models/server.py` & `flask-openapi3-2.3.2/flask_openapi3/models/server.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.3.1/flask_openapi3/models/validation_error.py` & `flask-openapi3-2.3.2/flask_openapi3/models/validation_error.py`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.3.1/flask_openapi3/openapi.py` & `flask-openapi3-2.3.2/flask_openapi3/openapi.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,25 +3,26 @@
 # @Time    : 2021/4/30 14:25
 import json
 import os
 import re
 from copy import deepcopy
 from typing import Optional, List, Dict, Union, Any, Type, Callable, Tuple
 
-from flask import Flask, Blueprint, render_template, render_template_string
+from flask import Flask, Blueprint, render_template_string
 from pydantic import BaseModel
 
 from .blueprint import APIBlueprint
 from .commands import openapi_command
 from .http import HTTPMethod
 from .models import Info, APISpec, Tag, Components, Server
 from .models.common import Reference, ExternalDocumentation, ExtraRequestBody
 from .models.oauth import OAuthConfig
 from .models.security import SecurityScheme
 from .scaffold import APIScaffold
+from .templates import openapi_html_string, redoc_html_string, rapidoc_html_string, swagger_html_string
 from .utils import get_operation, get_responses, parse_and_store_tags, parse_parameters, parse_method, \
     get_operation_id_for_path
 from .view import APIView
 
 
 class OpenAPI(APIScaffold, Flask):
     def __init__(
@@ -61,57 +62,48 @@
                          "full" (expands the tags and operations) or "none" (expands nothing).
                          see https://github.com/swagger-api/swagger-ui/blob/master/docs/usage/configuration.md
             doc_prefix: URL prefix used for OpenAPI document and UI. Defaults to "/openapi".
             api_doc_url: The OpenAPI Spec documentation. Defaults to "/openapi.json".
             swagger_url: The Swagger UI documentation. Defaults to `/swagger`.
             redoc_url: The Redoc UI documentation. Defaults to `/redoc`.
             rapidoc_url: The RapiDoc UI documentation. Defaults to `/rapidoc`.
-            ui_templates: Custom UI templates, which used to overwrite or add UI documents.
+            ui_templates: Custom UI templates, which are used to overwrite or add UI documents.
             servers: An array of Server Objects, which provide connectivity information to a target server.
             external_docs: Allows referencing an external resource for extended documentation.
                            See: https://spec.openapis.org/oas/v3.0.3#external-documentation-object
             **kwargs: Flask kwargs
         """
         super(OpenAPI, self).__init__(import_name, **kwargs)
-
         self.openapi_version = "3.0.3"
-        if info is None:
-            info = Info(title="OpenAPI", version="1.0.0")
-        assert isinstance(info, Info), f"Info is required (got type {type(info)})"
-        self.info = info
+        self.info = info or Info(title="OpenAPI", version="1.0.0")
         self.security_schemes = security_schemes
         self.responses = responses or {}
         self.paths: Dict = dict()
         self.components_schemas: Dict = dict()
         self.components = Components()
         self.tags: List[Tag] = []
         self.tag_names: List[str] = []
         self.doc_prefix = doc_prefix
         self.api_doc_url = api_doc_url
         self.swagger_url = swagger_url
         self.redoc_url = redoc_url
         self.rapidoc_url = rapidoc_url
-        if oauth_config:
-            if not isinstance(oauth_config, OAuthConfig):
-                raise TypeError("`initOAuth` must be `OAuthConfig`")
         self.oauth_config = oauth_config
         self.doc_expansion = doc_expansion
-        if ui_templates is None:
-            ui_templates = dict()
-        self.ui_templates = ui_templates
+        self.ui_templates = ui_templates or dict()
         self.severs = servers
         self.external_docs = external_docs
         if doc_ui:
             self._init_doc()
         # add openapi command
         self.cli.add_command(openapi_command)
 
     def _init_doc(self) -> None:
         """
-        Provide Swagger UI, Redoc and Rapidoc
+        Provide Swagger UI, Redoc, and Rapidoc
         """
         _here = os.path.dirname(__file__)
         template_folder = os.path.join(_here, "templates")
         static_folder = os.path.join(template_folder, "static")
 
         blueprint = Blueprint(
             "openapi",
@@ -121,59 +113,41 @@
             static_folder=static_folder
         )
         blueprint.add_url_rule(
             rule=self.api_doc_url,
             endpoint="api_doc",
             view_func=lambda: self.api_doc
         )
-        # iter ui_templates
-        for key, value in self.ui_templates.items():
+        builtins_templates = {
+            self.swagger_url.strip("/"): swagger_html_string,
+            self.redoc_url.strip("/"): redoc_html_string,
+            self.rapidoc_url.strip("/"): rapidoc_html_string
+        }
+        # update builtins_templates
+        builtins_templates.update(**self.ui_templates)
+        # iter builtins_templates
+        for key, value in builtins_templates.items():
             blueprint.add_url_rule(
                 rule=f"/{key}",
                 endpoint=key,
                 # pass default value to source
                 view_func=lambda source=value: render_template_string(
                     source,
-                    api_doc_url=self.api_doc_url.lstrip("/")
-                )
-            )
-        if self.swagger_url.strip("/") not in self.ui_templates.keys():
-            blueprint.add_url_rule(
-                rule=self.swagger_url,
-                endpoint="swagger",
-                view_func=lambda: render_template(
-                    "swagger.html",
                     api_doc_url=self.api_doc_url.lstrip("/"),
+                    # The following parameters are only for swagger ui
                     doc_expansion=self.doc_expansion,
                     oauth_config=self.oauth_config.dict() if self.oauth_config else None
                 )
             )
-        if self.redoc_url.strip("/") not in self.ui_templates.keys():
-            blueprint.add_url_rule(
-                rule=self.redoc_url,
-                endpoint="redoc",
-                view_func=lambda: render_template(
-                    "redoc.html",
-                    api_doc_url=self.api_doc_url.lstrip("/")
-                )
-            )
-        if self.rapidoc_url.strip("/") not in self.ui_templates.keys():
-            blueprint.add_url_rule(
-                rule=self.rapidoc_url,
-                endpoint="rapidoc",
-                view_func=lambda: render_template(
-                    "rapidoc.html",
-                    api_doc_url=self.api_doc_url.lstrip("/")
-                )
-            )
+        # home page
         blueprint.add_url_rule(
             rule="/",
             endpoint="openapi",
-            view_func=lambda: render_template(
-                "openapi.html",
+            view_func=lambda: render_template_string(
+                openapi_html_string,
                 swagger_url=self.swagger_url.lstrip("/"),
                 redoc_url=self.redoc_url.lstrip("/"),
                 rapidoc_url=self.rapidoc_url.lstrip("/")
             )
         )
         self.register_blueprint(blueprint)
```

### Comparing `flask-openapi3-2.3.1/flask_openapi3/request.py` & `flask-openapi3-2.3.2/flask_openapi3/request.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from flask.wrappers import Response
 from pydantic import ValidationError, BaseModel
 from pydantic.error_wrappers import ErrorWrapper
 
 
 def _do_header(header, request_kwargs):
     request_headers = dict(request.headers) or {}
-    for key, value in header.__annotations__.items():
+    for key, value in header.schema().get("properties", {}).items():
         key_title = key.replace("_", "-").title()
         # add original key
         if key_title in request_headers.keys():
             request_headers[key] = request_headers[key_title]
     request_kwargs.update({"header": header(**request_headers)})
```

### Comparing `flask-openapi3-2.3.1/flask_openapi3/scaffold.py` & `flask-openapi3-2.3.2/flask_openapi3/scaffold.py`

 * *Files 4% similar despite different names*

```diff
@@ -137,15 +137,15 @@
             tags: Adds metadata to a single tag.
             summary: A short summary of what the operation does.
             description: A verbose explanation of the operation behavior.
             external_docs: Additional external documentation for this operation.
             operation_id: Unique string used to identify the operation.
             extra_form: Extra information describing the request body(application/form).
             extra_body: Extra information describing the request body(application/json).
-            responses: Responses model, must be pydantic BaseModel.
+            responses: response's model must be pydantic BaseModel.
             extra_responses: Extra information for responses.
             deprecated: Declares this operation to be deprecated.
             security: A declaration of which security mechanisms can be used for this operation.
             servers: An alternative server array to service this operation.
             doc_ui: Add openapi document UI(swagger, rapidoc and redoc). Defaults to True.
         """
 
@@ -206,20 +206,20 @@
             tags: Adds metadata to a single tag.
             summary: A short summary of what the operation does.
             description: A verbose explanation of the operation behavior.
             external_docs: Additional external documentation for this operation.
             operation_id: Unique string used to identify the operation.
             extra_form: Extra information describing the request body(application/form).
             extra_body: Extra information describing the request body(application/json).
-            responses: Responses model, must be pydantic BaseModel.
+            responses: response's model must be pydantic BaseModel.
             extra_responses: Extra information for responses.
             deprecated: Declares this operation to be deprecated.
             security: A declaration of which security mechanisms can be used for this operation.
             servers: An alternative server array to service this operation.
-            doc_ui: Declares this operation to be show.
+            doc_ui: Declares this operation to be shown.
         """
 
         def decorator(func) -> Callable:
             header, cookie, path, query, form, body = \
                 self._do_decorator(
                     rule,
                     func,
@@ -275,20 +275,20 @@
             tags: Adds metadata to a single tag.
             summary: A short summary of what the operation does.
             description: A verbose explanation of the operation behavior.
             external_docs: Additional external documentation for this operation.
             operation_id: Unique string used to identify the operation.
             extra_form: Extra information describing the request body(application/form).
             extra_body: Extra information describing the request body(application/json).
-            responses: Responses model, must be pydantic BaseModel.
+            responses: response's model must be pydantic BaseModel.
             extra_responses: Extra information for responses.
             deprecated: Declares this operation to be deprecated.
             security: A declaration of which security mechanisms can be used for this operation.
             servers: An alternative server array to service this operation.
-            doc_ui: Declares this operation to be show.
+            doc_ui: Declares this operation to be shown.
         """
 
         def decorator(func) -> Callable:
             header, cookie, path, query, form, body = \
                 self._do_decorator(
                     rule,
                     func,
@@ -344,20 +344,20 @@
             tags: Adds metadata to a single tag.
             summary: A short summary of what the operation does.
             description: A verbose explanation of the operation behavior.
             external_docs: Additional external documentation for this operation.
             operation_id: Unique string used to identify the operation.
             extra_form: Extra information describing the request body(application/form).
             extra_body: Extra information describing the request body(application/json).
-            responses: Responses model, must be pydantic BaseModel.
+            responses: response's model must be pydantic BaseModel.
             extra_responses: Extra information for responses.
             deprecated: Declares this operation to be deprecated.
             security: A declaration of which security mechanisms can be used for this operation.
             servers: An alternative server array to service this operation.
-            doc_ui: Declares this operation to be show.
+            doc_ui: Declares this operation to be shown.
         """
 
         def decorator(func) -> Callable:
             header, cookie, path, query, form, body = \
                 self._do_decorator(
                     rule,
                     func,
@@ -413,20 +413,20 @@
             tags: Adds metadata to a single tag.
             summary: A short summary of what the operation does.
             description: A verbose explanation of the operation behavior.
             external_docs: Additional external documentation for this operation.
             operation_id: Unique string used to identify the operation.
             extra_form: Extra information describing the request body(application/form).
             extra_body: Extra information describing the request body(application/json).
-            responses: Responses model, must be pydantic BaseModel.
+            responses: response's model must be pydantic BaseModel.
             extra_responses: Extra information for responses.
             deprecated: Declares this operation to be deprecated.
             security: A declaration of which security mechanisms can be used for this operation.
             servers: An alternative server array to service this operation.
-            doc_ui: Declares this operation to be show.
+            doc_ui: Declares this operation to be shown.
         """
 
         def decorator(func) -> Callable:
             header, cookie, path, query, form, body = \
                 self._do_decorator(
                     rule,
                     func,
```

### Comparing `flask-openapi3-2.3.1/flask_openapi3/templates/static/css/swagger-ui.css` & `flask-openapi3-2.3.2/flask_openapi3/templates/static/css/swagger-ui.css`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.3.1/flask_openapi3/templates/static/images/apidoc.svg` & `flask-openapi3-2.3.2/flask_openapi3/templates/static/images/apidoc.svg`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.3.1/flask_openapi3/templates/static/images/rapidoc.svg` & `flask-openapi3-2.3.2/flask_openapi3/templates/static/images/rapidoc.svg`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.3.1/flask_openapi3/templates/static/images/redoc.svg` & `flask-openapi3-2.3.2/flask_openapi3/templates/static/images/redoc.svg`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.3.1/flask_openapi3/templates/static/images/swagger.svg` & `flask-openapi3-2.3.2/flask_openapi3/templates/static/images/swagger.svg`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.3.1/flask_openapi3/templates/static/js/rapidoc-min.js` & `flask-openapi3-2.3.2/flask_openapi3/templates/static/js/rapidoc-min.js`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.3.1/flask_openapi3/templates/static/js/redoc.standalone.js` & `flask-openapi3-2.3.2/flask_openapi3/templates/static/js/redoc.standalone.js`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.3.1/flask_openapi3/templates/static/js/swagger-ui-bundle.js` & `flask-openapi3-2.3.2/flask_openapi3/templates/static/js/swagger-ui-bundle.js`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.3.1/flask_openapi3/templates/static/js/swagger-ui-standalone-preset.js` & `flask-openapi3-2.3.2/flask_openapi3/templates/static/js/swagger-ui-standalone-preset.js`

 * *Files identical despite different names*

### Comparing `flask-openapi3-2.3.1/flask_openapi3/utils.py` & `flask-openapi3-2.3.2/flask_openapi3/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -370,15 +370,15 @@
         parameters.extend(_parameters)
         components_schemas.update(**_components_schemas)
     if cookie:
         _parameters, _components_schemas = parse_cookie(cookie)
         parameters.extend(_parameters)
         components_schemas.update(**_components_schemas)
     if path:
-        # get args from route path
+        # get args from a route path
         _parameters, _components_schemas = parse_path(path)
         parameters.extend(_parameters)
         components_schemas.update(**_components_schemas)
     if query:
         # get args from route query
         _parameters, _components_schemas = parse_query(query)
         parameters.extend(_parameters)
```

### Comparing `flask-openapi3-2.3.1/flask_openapi3/view.py` & `flask-openapi3-2.3.2/flask_openapi3/view.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,20 +116,20 @@
             tags: Adds metadata to a single tag.
             summary: A short summary of what the operation does.
             description: A verbose explanation of the operation behavior.
             external_docs: Additional external documentation for this operation.
             operation_id: Unique string used to identify the operation.
             extra_form: Extra information describing the request body(application/form).
             extra_body: Extra information describing the request body(application/json).
-            responses: Responses model, must be pydantic BaseModel.
+            responses: response's model must be pydantic BaseModel.
             extra_responses: Extra information for responses.
             deprecated: Declares this operation to be deprecated.
             security: A declaration of which security mechanisms can be used for this operation.
             servers: An alternative server array to service this operation.
-            doc_ui: Declares this operation to be show.
+            doc_ui: Declares this operation to be shown.
         """
 
         if responses is None:
             responses = {}
         if extra_responses is None:
             extra_responses = {}
         if security is None:
```

### Comparing `flask-openapi3-2.3.1/flask_openapi3.egg-info/PKG-INFO` & `flask-openapi3-2.3.2/flask_openapi3.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-openapi3
-Version: 2.3.1
+Version: 2.3.2
 Summary: Generate REST API and OpenAPI documentation for your Flask project.
 Home-page: https://github.com/luolingchun/flask-openapi3
 Author: llc
 Author-email: luolingchun@outlook.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
@@ -67,15 +67,15 @@
 
 - **Authorization:** Support to reload authorizations in Swagger UI
 
 ## Requirements
 
 Python 3.7+
 
-flask-openapi3 be dependent on the following libraries:
+flask-openapi3 is dependent on the following libraries:
 
 - [Flask](https://github.com/pallets/flask) for the web app.
 - [Pydantic](https://github.com/pydantic/pydantic) for the data validation.
 
 ## Installation
 
 ```bash
@@ -130,18 +130,18 @@
 
 
 class BookQuery(BaseModel):
     age: int
     author: str
 
 
-@app.get("/book", tags=[book_tag])
+@app.get("/book", summary="get books", tags=[book_tag])
 def get_book(query: BookQuery):
-    """get books
-    get all books
+    """
+    to get all books
     """
     return {
         "code": 0,
         "message": "ok",
         "data": [
             {"bid": 1, "age": query.age, "author": query.author},
             {"bid": 2, "age": query.age, "author": query.author}
@@ -190,15 +190,15 @@
     @api_view.doc(summary="get book list")
     def get(self, query: BookQuery):
         print(self.a)
         return query.json()
 
     @api_view.doc(summary="create book")
     def post(self, body: BookBody):
-        """description for create book"""
+        """description for a created book"""
         return body.json()
 
 
 @api_view.route("/book/<id>")
 class BookAPIView:
     @api_view.doc(summary="get book")
     def get(self, path: BookPath):
```

### Comparing `flask-openapi3-2.3.1/flask_openapi3.egg-info/SOURCES.txt` & `flask-openapi3-2.3.2/flask_openapi3.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -46,18 +46,15 @@
 flask_openapi3/models/info.py
 flask_openapi3/models/oauth.py
 flask_openapi3/models/path.py
 flask_openapi3/models/security.py
 flask_openapi3/models/server.py
 flask_openapi3/models/tag.py
 flask_openapi3/models/validation_error.py
-flask_openapi3/templates/openapi.html
-flask_openapi3/templates/rapidoc.html
-flask_openapi3/templates/redoc.html
-flask_openapi3/templates/swagger.html
+flask_openapi3/templates/__init__.py
 flask_openapi3/templates/static/css/swagger-ui.css
 flask_openapi3/templates/static/images/apidoc.svg
 flask_openapi3/templates/static/images/rapidoc.svg
 flask_openapi3/templates/static/images/redoc.svg
 flask_openapi3/templates/static/images/swagger.svg
 flask_openapi3/templates/static/js/rapidoc-min.js
 flask_openapi3/templates/static/js/redoc.standalone.js
```

### Comparing `flask-openapi3-2.3.1/setup.py` & `flask-openapi3-2.3.2/setup.py`

 * *Files identical despite different names*

