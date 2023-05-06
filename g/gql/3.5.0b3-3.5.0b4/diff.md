# Comparing `tmp/gql-3.5.0b3.tar.gz` & `tmp/gql-3.5.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gql-3.5.0b3.tar", last modified: Thu Feb 23 22:06:15 2023, max compression
+gzip compressed data, was "gql-3.5.0b4.tar", last modified: Sat May  6 19:36:59 2023, max compression
```

## Comparing `gql-3.5.0b3.tar` & `gql-3.5.0b4.tar`

### file list

```diff
@@ -1,189 +1,190 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 22:06:15.198130 gql-3.5.0b3/
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-02-23 22:06:12.000000 gql-3.5.0b3/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-02-23 22:06:12.000000 gql-3.5.0b3/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)     4069 2023-02-23 22:06:12.000000 gql-3.5.0b3/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)     1081 2023-02-23 22:06:12.000000 gql-3.5.0b3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-02-23 22:06:12.000000 gql-3.5.0b3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-02-23 22:06:12.000000 gql-3.5.0b3/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-02-23 22:06:15.198130 gql-3.5.0b3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4276 2023-02-23 22:06:12.000000 gql-3.5.0b3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 22:06:15.182130 gql-3.5.0b3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 22:06:15.182130 gql-3.5.0b3/docs/advanced/
--rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/advanced/async_advanced_usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3907 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/advanced/async_permanent_session.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11000 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/advanced/dsl_module.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3143 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/advanced/error_handling.rst
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/advanced/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/advanced/local_schema.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1444 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/advanced/logging.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 22:06:15.182130 gql-3.5.0b3/docs/async/
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/async/async_intro.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/async/async_usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/async/index.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 22:06:15.186130 gql-3.5.0b3/docs/code_examples/
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/code_examples/aiohttp_async.py
--rw-r--r--   0 runner    (1001) docker     (123)     1783 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/code_examples/aiohttp_async_dsl.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/code_examples/aiohttp_sync.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 22:06:15.186130 gql-3.5.0b3/docs/code_examples/appsync/
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/code_examples/appsync/mutation_api_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/code_examples/appsync/mutation_iam.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/code_examples/appsync/subscription_api_key.py
--rw-r--r--   0 runner    (1001) docker     (123)      941 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/code_examples/appsync/subscription_iam.py
--rw-r--r--   0 runner    (1001) docker     (123)     1846 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/code_examples/console_async.py
--rw-r--r--   0 runner    (1001) docker     (123)     2033 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/code_examples/fastapi_async.py
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/code_examples/httpx_async.py
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/code_examples/httpx_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)      734 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/code_examples/phoenix_channel_async.py
--rw-r--r--   0 runner    (1001) docker     (123)     1084 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/code_examples/reconnecting_mutation_http.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/code_examples/reconnecting_mutation_ws.py
--rw-r--r--   0 runner    (1001) docker     (123)      771 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/code_examples/reconnecting_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/code_examples/requests_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/code_examples/requests_sync_dsl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/code_examples/websockets_async.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 22:06:15.186130 gql-3.5.0b3/docs/gql-cli/
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/gql-cli/intro.rst
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4166 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/intro.rst
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 22:06:15.186130 gql-3.5.0b3/docs/modules/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/modules/client.rst
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/modules/dsl.rst
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/modules/gql.rst
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/modules/transport.rst
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/modules/transport_aiohttp.rst
--rw-r--r--   0 runner    (1001) docker     (123)      173 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/modules/transport_appsync_auth.rst
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/modules/transport_appsync_websockets.rst
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/modules/transport_exceptions.rst
--rw-r--r--   0 runner    (1001) docker     (123)      145 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/modules/transport_httpx.rst
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/modules/transport_phoenix_channel_websockets.rst
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/modules/transport_requests.rst
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/modules/transport_websockets.rst
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/modules/transport_websockets_base.rst
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/modules/utilities.rst
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 22:06:15.186130 gql-3.5.0b3/docs/transports/
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/transports/aiohttp.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5965 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/transports/appsync.rst
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/transports/async_transports.rst
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/transports/httpx.rst
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/transports/httpx_async.rst
--rw-r--r--   0 runner    (1001) docker     (123)      277 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/transports/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      600 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/transports/phoenix.rst
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/transports/requests.rst
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/transports/sync_transports.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5481 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/transports/websockets.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 22:06:15.190130 gql-3.5.0b3/docs/usage/
--rw-r--r--   0 runner    (1001) docker     (123)      774 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/usage/basic_usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)    10061 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/usage/custom_scalars_and_enums.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/usage/extensions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5898 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/usage/file_upload.rst
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/usage/headers.rst
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/usage/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      708 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/usage/subscriptions.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/usage/validation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-02-23 22:06:12.000000 gql-3.5.0b3/docs/usage/variables.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 22:06:15.190130 gql-3.5.0b3/gql/
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-02-23 22:06:12.000000 gql-3.5.0b3/gql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-02-23 22:06:12.000000 gql-3.5.0b3/gql/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14738 2023-02-23 22:06:12.000000 gql-3.5.0b3/gql/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    51634 2023-02-23 22:06:12.000000 gql-3.5.0b3/gql/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    35952 2023-02-23 22:06:12.000000 gql-3.5.0b3/gql/dsl.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-02-23 22:06:12.000000 gql-3.5.0b3/gql/gql.py
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-02-23 22:06:12.000000 gql-3.5.0b3/gql/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 22:06:15.190130 gql-3.5.0b3/gql/transport/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-02-23 22:06:12.000000 gql-3.5.0b3/gql/transport/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13451 2023-02-23 22:06:12.000000 gql-3.5.0b3/gql/transport/aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     7515 2023-02-23 22:06:12.000000 gql-3.5.0b3/gql/transport/appsync_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     7093 2023-02-23 22:06:12.000000 gql-3.5.0b3/gql/transport/appsync_websockets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1723 2023-02-23 22:06:12.000000 gql-3.5.0b3/gql/transport/async_transport.py
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-02-23 22:06:12.000000 gql-3.5.0b3/gql/transport/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    10439 2023-02-23 22:06:12.000000 gql-3.5.0b3/gql/transport/httpx.py
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-02-23 22:06:12.000000 gql-3.5.0b3/gql/transport/local_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    15179 2023-02-23 22:06:12.000000 gql-3.5.0b3/gql/transport/phoenix_channel_websockets.py
--rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-02-23 22:06:12.000000 gql-3.5.0b3/gql/transport/requests.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-02-23 22:06:12.000000 gql-3.5.0b3/gql/transport/transport.py
--rw-r--r--   0 runner    (1001) docker     (123)    19190 2023-02-23 22:06:12.000000 gql-3.5.0b3/gql/transport/websockets.py
--rw-r--r--   0 runner    (1001) docker     (123)    24466 2023-02-23 22:06:12.000000 gql-3.5.0b3/gql/transport/websockets_base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 22:06:15.194130 gql-3.5.0b3/gql/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-02-23 22:06:12.000000 gql-3.5.0b3/gql/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-02-23 22:06:12.000000 gql-3.5.0b3/gql/utilities/build_client_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     3865 2023-02-23 22:06:12.000000 gql-3.5.0b3/gql/utilities/get_introspection_query_ast.py
--rw-r--r--   0 runner    (1001) docker     (123)    14304 2023-02-23 22:06:12.000000 gql-3.5.0b3/gql/utilities/parse_result.py
--rw-r--r--   0 runner    (1001) docker     (123)     4261 2023-02-23 22:06:12.000000 gql-3.5.0b3/gql/utilities/serialize_variable_values.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-02-23 22:06:12.000000 gql-3.5.0b3/gql/utilities/update_schema_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-02-23 22:06:12.000000 gql-3.5.0b3/gql/utilities/update_schema_scalars.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-02-23 22:06:12.000000 gql-3.5.0b3/gql/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 22:06:15.190130 gql-3.5.0b3/gql.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6152 2023-02-23 22:06:15.000000 gql-3.5.0b3/gql.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4901 2023-02-23 22:06:15.000000 gql-3.5.0b3/gql.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 22:06:15.000000 gql-3.5.0b3/gql.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-02-23 22:06:15.000000 gql-3.5.0b3/gql.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 22:06:15.000000 gql-3.5.0b3/gql.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-02-23 22:06:15.000000 gql-3.5.0b3/gql.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-02-23 22:06:15.000000 gql-3.5.0b3/gql.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-02-23 22:06:15.198130 gql-3.5.0b3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-02-23 22:06:12.000000 gql-3.5.0b3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 22:06:15.194130 gql-3.5.0b3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15031 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 22:06:15.198130 gql-3.5.0b3/tests/custom_scalars/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/custom_scalars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6593 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/custom_scalars/test_datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     6960 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/custom_scalars/test_enum_colors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5153 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/custom_scalars/test_json.py
--rw-r--r--   0 runner    (1001) docker     (123)    20717 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/custom_scalars/test_money.py
--rw-r--r--   0 runner    (1001) docker     (123)     2546 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/custom_scalars/test_parse_results.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 22:06:15.198130 gql-3.5.0b3/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/fixtures/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 22:06:15.198130 gql-3.5.0b3/tests/fixtures/aws/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/fixtures/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/fixtures/aws/fake_credentials.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/fixtures/aws/fake_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/fixtures/aws/fake_session.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/fixtures/aws/fake_signer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 22:06:15.198130 gql-3.5.0b3/tests/fixtures/graphql/
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/fixtures/graphql/sample.graphql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 22:06:15.198130 gql-3.5.0b3/tests/fixtures/vcr_cassettes/
--rw-r--r--   0 runner    (1001) docker     (123)     5340 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/fixtures/vcr_cassettes/client.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    78820 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/fixtures/vcr_cassettes/queries.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 22:06:15.198130 gql-3.5.0b3/tests/nested_input/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/nested_input/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      856 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/nested_input/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/nested_input/test_nested_input.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 22:06:15.198130 gql-3.5.0b3/tests/starwars/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/starwars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/starwars/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     7790 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/starwars/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    22874 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/starwars/test_dsl.py
--rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/starwars/test_parse_results.py
--rw-r--r--   0 runner    (1001) docker     (123)     7529 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/starwars/test_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     2594 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/starwars/test_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/starwars/test_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    43147 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/test_aiohttp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/test_aiohttp_online.py
--rw-r--r--   0 runner    (1001) docker     (123)     6588 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/test_appsync_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/test_appsync_http.py
--rw-r--r--   0 runner    (1001) docker     (123)    23922 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/test_appsync_websockets.py
--rw-r--r--   0 runner    (1001) docker     (123)     7303 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/test_async_client_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10785 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     7011 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7525 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/test_graphqlws_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    27257 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/test_graphqlws_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     4008 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/test_http_async_sync.py
--rw-r--r--   0 runner    (1001) docker     (123)    26413 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/test_httpx.py
--rw-r--r--   0 runner    (1001) docker     (123)    38462 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/test_httpx_async.py
--rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/test_httpx_online.py
--rw-r--r--   0 runner    (1001) docker     (123)      264 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/test_localhost.cnf
--rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/test_localhost.pem
--rw-r--r--   0 runner    (1001) docker     (123)    15131 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/test_phoenix_channel_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4079 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/test_phoenix_channel_query.py
--rw-r--r--   0 runner    (1001) docker     (123)    12704 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/test_phoenix_channel_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)    26692 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/test_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/test_transport.py
--rw-r--r--   0 runner    (1001) docker     (123)    11402 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/test_websocket_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6236 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/test_websocket_online.py
--rw-r--r--   0 runner    (1001) docker     (123)    17431 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/test_websocket_query.py
--rw-r--r--   0 runner    (1001) docker     (123)    18656 2023-02-23 22:06:12.000000 gql-3.5.0b3/tests/test_websocket_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-02-23 22:06:12.000000 gql-3.5.0b3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 19:36:59.502615 gql-3.5.0b4/
+-rw-r--r--   0 runner    (1001) docker     (122)      603 2023-05-06 19:36:54.000000 gql-3.5.0b4/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-05-06 19:36:54.000000 gql-3.5.0b4/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (122)     4069 2023-05-06 19:36:54.000000 gql-3.5.0b4/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1081 2023-05-06 19:36:54.000000 gql-3.5.0b4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      464 2023-05-06 19:36:54.000000 gql-3.5.0b4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      875 2023-05-06 19:36:54.000000 gql-3.5.0b4/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)     6203 2023-05-06 19:36:59.502615 gql-3.5.0b4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4276 2023-05-06 19:36:54.000000 gql-3.5.0b4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 19:36:59.474614 gql-3.5.0b4/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)      634 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 19:36:59.474614 gql-3.5.0b4/docs/advanced/
+-rw-r--r--   0 runner    (1001) docker     (122)     1895 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/advanced/async_advanced_usage.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3907 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/advanced/async_permanent_session.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    11000 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/advanced/dsl_module.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3143 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/advanced/error_handling.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      159 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/advanced/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      612 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/advanced/local_schema.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1445 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/advanced/logging.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 19:36:59.478614 gql-3.5.0b4/docs/async/
+-rw-r--r--   0 runner    (1001) docker     (122)     1164 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/async/async_intro.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1251 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/async/async_usage.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      116 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/async/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 19:36:59.478614 gql-3.5.0b4/docs/code_examples/
+-rw-r--r--   0 runner    (1001) docker     (122)      784 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/code_examples/aiohttp_async.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1783 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/code_examples/aiohttp_async_dsl.py
+-rw-r--r--   0 runner    (1001) docker     (122)      552 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/code_examples/aiohttp_sync.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 19:36:59.478614 gql-3.5.0b4/docs/code_examples/appsync/
+-rw-r--r--   0 runner    (1001) docker     (122)     1332 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/code_examples/appsync/mutation_api_key.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1238 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/code_examples/appsync/mutation_iam.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1254 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/code_examples/appsync/subscription_api_key.py
+-rw-r--r--   0 runner    (1001) docker     (122)      941 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/code_examples/appsync/subscription_iam.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1846 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/code_examples/console_async.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2033 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/code_examples/fastapi_async.py
+-rw-r--r--   0 runner    (1001) docker     (122)      788 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/code_examples/httpx_async.py
+-rw-r--r--   0 runner    (1001) docker     (122)      377 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/code_examples/httpx_sync.py
+-rw-r--r--   0 runner    (1001) docker     (122)      734 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/code_examples/phoenix_channel_async.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1084 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/code_examples/reconnecting_mutation_http.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1093 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/code_examples/reconnecting_mutation_ws.py
+-rw-r--r--   0 runner    (1001) docker     (122)      771 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/code_examples/reconnecting_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (122)      433 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/code_examples/requests_sync.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1070 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/code_examples/requests_sync_dsl.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1148 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/code_examples/websockets_async.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2625 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 19:36:59.478614 gql-3.5.0b4/docs/gql-cli/
+-rw-r--r--   0 runner    (1001) docker     (122)     2057 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/gql-cli/intro.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      316 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     4166 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/intro.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      764 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 19:36:59.482615 gql-3.5.0b4/docs/modules/
+-rw-r--r--   0 runner    (1001) docker     (122)       81 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/modules/client.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       97 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/modules/dsl.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      489 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/modules/gql.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      237 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/modules/transport.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      153 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/modules/transport_aiohttp.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      173 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/modules/transport_appsync_auth.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      197 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/modules/transport_appsync_websockets.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      165 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/modules/transport_exceptions.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      145 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/modules/transport_httpx.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      229 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/modules/transport_phoenix_channel_websockets.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      157 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/modules/transport_requests.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      165 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/modules/transport_websockets.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      185 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/modules/transport_websockets_base.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       93 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/modules/utilities.rst
+-rw-r--r--   0 runner    (1001) docker     (122)       85 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 19:36:59.482615 gql-3.5.0b4/docs/transports/
+-rw-r--r--   0 runner    (1001) docker     (122)     1474 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/transports/aiohttp.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     5965 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/transports/appsync.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      301 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/transports/async_transports.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      332 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/transports/httpx.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      997 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/transports/httpx_async.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      277 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/transports/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      600 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/transports/phoenix.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      378 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/transports/requests.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/transports/sync_transports.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     5481 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/transports/websockets.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 19:36:59.486615 gql-3.5.0b4/docs/usage/
+-rw-r--r--   0 runner    (1001) docker     (122)      774 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/usage/basic_usage.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10061 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/usage/custom_scalars_and_enums.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1125 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/usage/extensions.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     5898 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/usage/file_upload.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      344 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/usage/headers.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      170 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/usage/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      708 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/usage/subscriptions.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1603 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/usage/validation.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      790 2023-05-06 19:36:54.000000 gql-3.5.0b4/docs/usage/variables.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 19:36:59.486615 gql-3.5.0b4/gql/
+-rw-r--r--   0 runner    (1001) docker     (122)      463 2023-05-06 19:36:54.000000 gql-3.5.0b4/gql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       24 2023-05-06 19:36:54.000000 gql-3.5.0b4/gql/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16695 2023-05-06 19:36:54.000000 gql-3.5.0b4/gql/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)    52066 2023-05-06 19:36:54.000000 gql-3.5.0b4/gql/client.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36033 2023-05-06 19:36:54.000000 gql-3.5.0b4/gql/dsl.py
+-rw-r--r--   0 runner    (1001) docker     (122)      667 2023-05-06 19:36:54.000000 gql-3.5.0b4/gql/gql.py
+-rw-r--r--   0 runner    (1001) docker     (122)       62 2023-05-06 19:36:54.000000 gql-3.5.0b4/gql/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 19:36:59.490615 gql-3.5.0b4/gql/transport/
+-rw-r--r--   0 runner    (1001) docker     (122)      120 2023-05-06 19:36:54.000000 gql-3.5.0b4/gql/transport/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13451 2023-05-06 19:36:54.000000 gql-3.5.0b4/gql/transport/aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7515 2023-05-06 19:36:54.000000 gql-3.5.0b4/gql/transport/appsync_auth.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7093 2023-05-06 19:36:54.000000 gql-3.5.0b4/gql/transport/appsync_websockets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1723 2023-05-06 19:36:54.000000 gql-3.5.0b4/gql/transport/async_transport.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1744 2023-05-06 19:36:54.000000 gql-3.5.0b4/gql/transport/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10440 2023-05-06 19:36:54.000000 gql-3.5.0b4/gql/transport/httpx.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2030 2023-05-06 19:36:54.000000 gql-3.5.0b4/gql/transport/local_schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15179 2023-05-06 19:36:54.000000 gql-3.5.0b4/gql/transport/phoenix_channel_websockets.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10021 2023-05-06 19:36:54.000000 gql-3.5.0b4/gql/transport/requests.py
+-rw-r--r--   0 runner    (1001) docker     (122)      991 2023-05-06 19:36:54.000000 gql-3.5.0b4/gql/transport/transport.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19190 2023-05-06 19:36:54.000000 gql-3.5.0b4/gql/transport/websockets.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24466 2023-05-06 19:36:54.000000 gql-3.5.0b4/gql/transport/websockets_base.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 19:36:59.490615 gql-3.5.0b4/gql/utilities/
+-rw-r--r--   0 runner    (1001) docker     (122)      609 2023-05-06 19:36:54.000000 gql-3.5.0b4/gql/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3165 2023-05-06 19:36:54.000000 gql-3.5.0b4/gql/utilities/build_client_schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3865 2023-05-06 19:36:54.000000 gql-3.5.0b4/gql/utilities/get_introspection_query_ast.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14304 2023-05-06 19:36:54.000000 gql-3.5.0b4/gql/utilities/parse_result.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4261 2023-05-06 19:36:54.000000 gql-3.5.0b4/gql/utilities/serialize_variable_values.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2392 2023-05-06 19:36:54.000000 gql-3.5.0b4/gql/utilities/update_schema_enum.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2280 2023-05-06 19:36:54.000000 gql-3.5.0b4/gql/utilities/update_schema_scalars.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1850 2023-05-06 19:36:54.000000 gql-3.5.0b4/gql/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 19:36:59.490615 gql-3.5.0b4/gql.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     6203 2023-05-06 19:36:59.000000 gql-3.5.0b4/gql.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4938 2023-05-06 19:36:59.000000 gql-3.5.0b4/gql.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-06 19:36:59.000000 gql-3.5.0b4/gql.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       45 2023-05-06 19:36:59.000000 gql-3.5.0b4/gql.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-06 19:36:59.000000 gql-3.5.0b4/gql.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)     1303 2023-05-06 19:36:59.000000 gql-3.5.0b4/gql.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        4 2023-05-06 19:36:59.000000 gql-3.5.0b4/gql.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      369 2023-05-06 19:36:59.502615 gql-3.5.0b4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     3262 2023-05-06 19:36:54.000000 gql-3.5.0b4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 19:36:59.494614 gql-3.5.0b4/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15031 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 19:36:59.498615 gql-3.5.0b4/tests/custom_scalars/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/custom_scalars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6593 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/custom_scalars/test_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6960 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/custom_scalars/test_enum_colors.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5153 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/custom_scalars/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20717 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/custom_scalars/test_money.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2546 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/custom_scalars/test_parse_results.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 19:36:59.498615 gql-3.5.0b4/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/fixtures/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 19:36:59.498615 gql-3.5.0b4/tests/fixtures/aws/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/fixtures/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      885 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/fixtures/aws/fake_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (122)      604 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/fixtures/aws/fake_request.py
+-rw-r--r--   0 runner    (1001) docker     (122)      678 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/fixtures/aws/fake_session.py
+-rw-r--r--   0 runner    (1001) docker     (122)      678 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/fixtures/aws/fake_signer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 19:36:59.498615 gql-3.5.0b4/tests/fixtures/graphql/
+-rw-r--r--   0 runner    (1001) docker     (122)      180 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/fixtures/graphql/sample.graphql
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 19:36:59.498615 gql-3.5.0b4/tests/fixtures/vcr_cassettes/
+-rw-r--r--   0 runner    (1001) docker     (122)     5340 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/fixtures/vcr_cassettes/client.yaml
+-rw-r--r--   0 runner    (1001) docker     (122)    78820 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/fixtures/vcr_cassettes/queries.yaml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 19:36:59.498615 gql-3.5.0b4/tests/nested_input/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/nested_input/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      856 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/nested_input/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1006 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/nested_input/test_nested_input.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-06 19:36:59.502615 gql-3.5.0b4/tests/starwars/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/starwars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3914 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/starwars/fixtures.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7990 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/starwars/schema.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23843 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/starwars/test_dsl.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2050 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/starwars/test_introspection.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3587 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/starwars/test_parse_results.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7529 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/starwars/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2594 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/starwars/test_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5441 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/starwars/test_validation.py
+-rw-r--r--   0 runner    (1001) docker     (122)    43147 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/test_aiohttp.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3320 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/test_aiohttp_online.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6588 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/test_appsync_auth.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2139 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/test_appsync_http.py
+-rw-r--r--   0 runner    (1001) docker     (122)    23922 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/test_appsync_websockets.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7303 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/test_async_client_validation.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12020 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7011 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7525 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/test_graphqlws_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    27257 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/test_graphqlws_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4008 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/test_http_async_sync.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26413 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/test_httpx.py
+-rw-r--r--   0 runner    (1001) docker     (122)    38462 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/test_httpx_async.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3320 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/test_httpx_online.py
+-rw-r--r--   0 runner    (1001) docker     (122)      264 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/test_localhost.cnf
+-rw-r--r--   0 runner    (1001) docker     (122)     2908 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/test_localhost.pem
+-rw-r--r--   0 runner    (1001) docker     (122)    15131 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/test_phoenix_channel_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4079 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/test_phoenix_channel_query.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12704 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/test_phoenix_channel_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26692 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/test_requests.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3517 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/test_transport.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11402 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/test_websocket_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6236 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/test_websocket_online.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17431 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/test_websocket_query.py
+-rw-r--r--   0 runner    (1001) docker     (122)    18656 2023-05-06 19:36:54.000000 gql-3.5.0b4/tests/test_websocket_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1528 2023-05-06 19:36:54.000000 gql-3.5.0b4/tox.ini
```

### Comparing `gql-3.5.0b3/.readthedocs.yaml` & `gql-3.5.0b4/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/CONTRIBUTING.md` & `gql-3.5.0b4/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/LICENSE` & `gql-3.5.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/Makefile` & `gql-3.5.0b4/Makefile`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/PKG-INFO` & `gql-3.5.0b4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gql
-Version: 3.5.0b3
+Version: 3.5.0b4
 Summary: GraphQL client for Python
 Home-page: https://github.com/graphql-python/gql
 Author: Syrus Akbary
 Author-email: me@syrusakbary.com
 License: MIT
 Description: # GQL
         
@@ -115,14 +115,15 @@
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: test
 Provides-Extra: test_no_transport
 Provides-Extra: dev
 Provides-Extra: aiohttp
```

### Comparing `gql-3.5.0b3/README.md` & `gql-3.5.0b4/README.md`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/docs/Makefile` & `gql-3.5.0b4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/docs/advanced/async_advanced_usage.rst` & `gql-3.5.0b4/docs/advanced/async_advanced_usage.rst`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/docs/advanced/async_permanent_session.rst` & `gql-3.5.0b4/docs/advanced/async_permanent_session.rst`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/docs/advanced/dsl_module.rst` & `gql-3.5.0b4/docs/advanced/dsl_module.rst`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/docs/advanced/error_handling.rst` & `gql-3.5.0b4/docs/advanced/error_handling.rst`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/docs/advanced/local_schema.rst` & `gql-3.5.0b4/docs/advanced/local_schema.rst`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/docs/advanced/logging.rst` & `gql-3.5.0b4/docs/advanced/logging.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Logging
 =======
 
-GQL use the python `logging`_ module.
+GQL uses the python `logging`_ module.
 
 In order to debug a problem, you can enable logging to see the messages exchanged between the client and the server.
 To do that, set the loglevel at **INFO** at the beginning of your code:
 
 .. code-block:: python
 
     import logging
```

### Comparing `gql-3.5.0b3/docs/async/async_intro.rst` & `gql-3.5.0b4/docs/async/async_intro.rst`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/docs/async/async_usage.rst` & `gql-3.5.0b4/docs/async/async_usage.rst`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/docs/code_examples/aiohttp_async.py` & `gql-3.5.0b4/docs/code_examples/aiohttp_async.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/docs/code_examples/aiohttp_async_dsl.py` & `gql-3.5.0b4/docs/code_examples/aiohttp_async_dsl.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/docs/code_examples/aiohttp_sync.py` & `gql-3.5.0b4/docs/code_examples/aiohttp_sync.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/docs/code_examples/appsync/mutation_api_key.py` & `gql-3.5.0b4/docs/code_examples/appsync/mutation_api_key.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/docs/code_examples/appsync/mutation_iam.py` & `gql-3.5.0b4/docs/code_examples/appsync/mutation_iam.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/docs/code_examples/appsync/subscription_api_key.py` & `gql-3.5.0b4/docs/code_examples/appsync/subscription_api_key.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/docs/code_examples/appsync/subscription_iam.py` & `gql-3.5.0b4/docs/code_examples/appsync/subscription_iam.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/docs/code_examples/console_async.py` & `gql-3.5.0b4/docs/code_examples/console_async.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/docs/code_examples/fastapi_async.py` & `gql-3.5.0b4/docs/code_examples/fastapi_async.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/docs/code_examples/httpx_async.py` & `gql-3.5.0b4/docs/code_examples/httpx_async.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/docs/code_examples/phoenix_channel_async.py` & `gql-3.5.0b4/docs/code_examples/phoenix_channel_async.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/docs/code_examples/reconnecting_mutation_http.py` & `gql-3.5.0b4/docs/code_examples/reconnecting_mutation_http.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/docs/code_examples/reconnecting_mutation_ws.py` & `gql-3.5.0b4/docs/code_examples/reconnecting_mutation_ws.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/docs/code_examples/reconnecting_subscription.py` & `gql-3.5.0b4/docs/code_examples/reconnecting_subscription.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/docs/code_examples/requests_sync_dsl.py` & `gql-3.5.0b4/docs/code_examples/requests_sync_dsl.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/docs/code_examples/websockets_async.py` & `gql-3.5.0b4/docs/code_examples/websockets_async.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/docs/conf.py` & `gql-3.5.0b4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/docs/gql-cli/intro.rst` & `gql-3.5.0b4/docs/gql-cli/intro.rst`

 * *Files 17% similar despite different names*

```diff
@@ -74,7 +74,17 @@
 
 Print the GraphQL schema in a file
 ^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^^
 
 .. code-block:: shell
 
     $ gql-cli https://countries.trevorblades.com/graphql --print-schema > schema.graphql
+
+.. note::
+
+    By default, deprecated input fields are not requested from the backend.
+    You can add :code:`--schema-download input_value_deprecation:true` to request them.
+
+.. note::
+
+    You can add :code:`--schema-download descriptions:false` to request a compact schema
+    without comments.
```

### Comparing `gql-3.5.0b3/docs/intro.rst` & `gql-3.5.0b4/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/docs/make.bat` & `gql-3.5.0b4/docs/make.bat`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/docs/transports/aiohttp.rst` & `gql-3.5.0b4/docs/transports/aiohttp.rst`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/docs/transports/appsync.rst` & `gql-3.5.0b4/docs/transports/appsync.rst`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/docs/transports/httpx_async.rst` & `gql-3.5.0b4/docs/transports/httpx_async.rst`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/docs/transports/phoenix.rst` & `gql-3.5.0b4/docs/transports/phoenix.rst`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/docs/transports/websockets.rst` & `gql-3.5.0b4/docs/transports/websockets.rst`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/docs/usage/basic_usage.rst` & `gql-3.5.0b4/docs/usage/basic_usage.rst`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/docs/usage/custom_scalars_and_enums.rst` & `gql-3.5.0b4/docs/usage/custom_scalars_and_enums.rst`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/docs/usage/extensions.rst` & `gql-3.5.0b4/docs/usage/extensions.rst`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/docs/usage/file_upload.rst` & `gql-3.5.0b4/docs/usage/file_upload.rst`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/docs/usage/subscriptions.rst` & `gql-3.5.0b4/docs/usage/subscriptions.rst`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/docs/usage/validation.rst` & `gql-3.5.0b4/docs/usage/validation.rst`

 * *Files 7% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         schema_str = f.read()
 
     client = Client(schema=schema_str)
 
 .. note::
     You can download a schema from a server by using :ref:`gql-cli <gql_cli>`
 
-    :code:`$ gql-cli https://SERVER_URL/graphql --print-schema > schema.graphql`
+    :code:`$ gql-cli https://SERVER_URL/graphql --print-schema --schema-download input_value_deprecation:true > schema.graphql`
 
 OR can be created using python classes:
 
 .. code-block:: python
 
     from .someSchema import SampleSchema
     # SampleSchema is an instance of GraphQLSchema
```

### Comparing `gql-3.5.0b3/docs/usage/variables.rst` & `gql-3.5.0b4/docs/usage/variables.rst`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/gql/cli.py` & `gql-3.5.0b4/gql/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import asyncio
 import json
 import logging
 import signal as signal_module
 import sys
-from argparse import ArgumentParser, Namespace, RawDescriptionHelpFormatter
+import textwrap
+from argparse import ArgumentParser, Namespace, RawTextHelpFormatter
 from typing import Any, Dict, Optional
 
 from graphql import GraphQLError, print_schema
 from yarl import URL
 
 from gql import Client, __version__, gql
 from gql.transport import AsyncTransport
@@ -74,15 +75,15 @@
                           present in the sphinx docs (they are put there with
                           a different layout)
     """
 
     parser = ArgumentParser(
         description=description,
         epilog=examples if with_examples else None,
-        formatter_class=RawDescriptionHelpFormatter,
+        formatter_class=RawTextHelpFormatter,
     )
     parser.add_argument(
         "server", help="the server url starting with http://, https://, ws:// or wss://"
     )
     parser.add_argument(
         "-V",
         "--variables",
@@ -119,14 +120,35 @@
     parser.add_argument(
         "--print-schema",
         help="get the schema from instrospection and print it",
         action="store_true",
         dest="print_schema",
     )
     parser.add_argument(
+        "--schema-download",
+        nargs="*",
+        help=textwrap.dedent(
+            """select the introspection query arguments to download the schema.
+            Only useful if --print-schema is used.
+            By default, it will:
+
+             - request field descriptions
+             - not request deprecated input fields
+
+            Possible options:
+
+             - descriptions:false             for a compact schema without comments
+             - input_value_deprecation:true   to download deprecated input fields
+             - specified_by_url:true
+             - schema_description:true
+             - directive_is_repeatable:true"""
+        ),
+        dest="schema_download",
+    )
+    parser.add_argument(
         "--execute-timeout",
         help="set the execute_timeout argument of the Client (default: 10)",
         type=positive_int_or_none,
         default=10,
         dest="execute_timeout",
     )
     parser.add_argument(
@@ -358,14 +380,50 @@
             try:
                 return AppSyncWebsocketsTransport(url=args.server, **transport_args)
             except Exception:
                 # This is for the NoCredentialsError but we cannot import it here
                 return None
 
 
+def get_introspection_args(args: Namespace) -> Dict:
+    """Get the introspection args depending on the schema_download argument"""
+
+    # Parse the headers argument
+    introspection_args = {}
+
+    possible_args = [
+        "descriptions",
+        "specified_by_url",
+        "directive_is_repeatable",
+        "schema_description",
+        "input_value_deprecation",
+    ]
+
+    if args.schema_download is not None:
+        for arg in args.schema_download:
+
+            try:
+                # Split only the first colon (throw a ValueError if no colon is present)
+                arg_key, arg_value = arg.split(":", 1)
+
+                if arg_key not in possible_args:
+                    raise ValueError(f"Invalid schema_download: {args.schema_download}")
+
+                arg_value = arg_value.lower()
+                if arg_value not in ["true", "false"]:
+                    raise ValueError(f"Invalid schema_download: {args.schema_download}")
+
+                introspection_args[arg_key] = arg_value == "true"
+
+            except ValueError:
+                raise ValueError(f"Invalid schema_download: {args.schema_download}")
+
+    return introspection_args
+
+
 async def main(args: Namespace) -> int:
     """Main entrypoint of the gql-cli script
 
     :param args: The parsed command line arguments
     :return: The script exit code (0 = ok, 1 = error)
     """
 
@@ -391,14 +449,15 @@
     # By default, the exit_code is 0 (everything is ok)
     exit_code = 0
 
     # Connect to the backend and provide a session
     async with Client(
         transport=transport,
         fetch_schema_from_transport=args.print_schema,
+        introspection_args=get_introspection_args(args),
         execute_timeout=args.execute_timeout,
     ) as session:
 
         if args.print_schema:
             schema_str = print_schema(session.client.schema)
             print(schema_str)
```

### Comparing `gql-3.5.0b3/gql/client.py` & `gql-3.5.0b4/gql/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,25 +72,28 @@
 
     def __init__(
         self,
         schema: Optional[Union[str, GraphQLSchema]] = None,
         introspection: Optional[IntrospectionQuery] = None,
         transport: Optional[Union[Transport, AsyncTransport]] = None,
         fetch_schema_from_transport: bool = False,
+        introspection_args: Optional[Dict] = None,
         execute_timeout: Optional[Union[int, float]] = 10,
         serialize_variables: bool = False,
         parse_results: bool = False,
     ):
         """Initialize the client with the given parameters.
 
         :param schema: an optional GraphQL Schema for local validation
                 See :ref:`schema_validation`
         :param transport: The provided :ref:`transport <Transports>`.
         :param fetch_schema_from_transport: Boolean to indicate that if we want to fetch
-                the schema from the transport using an introspection query
+                the schema from the transport using an introspection query.
+        :param introspection_args: arguments passed to the get_introspection_query
+                method of graphql-core.
         :param execute_timeout: The maximum time in seconds for the execution of a
                 request before a TimeoutError is raised. Only used for async transports.
                 Passing None results in waiting forever for a response.
         :param serialize_variables: whether the variable values should be
             serialized. Used for custom scalars and/or enums. Default: False.
         :param parse_results: Whether gql will try to parse the serialized output
                 sent by the backend. Can be used to unserialize custom scalars or enums.
@@ -128,14 +131,17 @@
 
         # GraphQL transport chosen
         self.transport: Optional[Union[Transport, AsyncTransport]] = transport
 
         # Flag to indicate that we need to fetch the schema from the transport
         # On async transports, we fetch the schema before executing the first query
         self.fetch_schema_from_transport: bool = fetch_schema_from_transport
+        self.introspection_args = (
+            {} if introspection_args is None else introspection_args
+        )
 
         # Enforced timeout of the execute function (only for async transports)
         self.execute_timeout = execute_timeout
 
         self.serialize_variables = serialize_variables
         self.parse_results = parse_results
 
@@ -875,15 +881,16 @@
         return result.data
 
     def fetch_schema(self) -> None:
         """Fetch the GraphQL schema explicitly using introspection.
 
         Don't use this function and instead set the fetch_schema_from_transport
         attribute to True"""
-        execution_result = self.transport.execute(parse(get_introspection_query()))
+        introspection_query = get_introspection_query(**self.client.introspection_args)
+        execution_result = self.transport.execute(parse(introspection_query))
 
         self.client._build_schema_from_introspection(execution_result)
 
     @property
     def transport(self):
         return self.client.transport
 
@@ -1246,17 +1253,16 @@
         return result.data
 
     async def fetch_schema(self) -> None:
         """Fetch the GraphQL schema explicitly using introspection.
 
         Don't use this function and instead set the fetch_schema_from_transport
         attribute to True"""
-        execution_result = await self.transport.execute(
-            parse(get_introspection_query())
-        )
+        introspection_query = get_introspection_query(**self.client.introspection_args)
+        execution_result = await self.transport.execute(parse(introspection_query))
 
         self.client._build_schema_from_introspection(execution_result)
 
     @property
     def transport(self):
         return self.client.transport
```

### Comparing `gql-3.5.0b3/gql/dsl.py` & `gql-3.5.0b4/gql/dsl.py`

 * *Files 2% similar despite different names*

```diff
@@ -291,15 +291,19 @@
     def __getattr__(self, name: str) -> "DSLType":
 
         type_def: Optional[GraphQLNamedType] = self._schema.get_type(name)
 
         if type_def is None:
             raise AttributeError(f"Type '{name}' not found in the schema!")
 
-        assert isinstance(type_def, (GraphQLObjectType, GraphQLInterfaceType))
+        if not isinstance(type_def, (GraphQLObjectType, GraphQLInterfaceType)):
+            raise AttributeError(
+                f'Type "{name} ({type_def!r})" is not valid as an attribute of'
+                " DSLSchema. Only Object types or Interface types are accepted."
+            )
 
         return DSLType(type_def, self)
 
 
 class DSLSelector(ABC):
     """DSLSelector is an abstract class which defines the
     :meth:`select <gql.dsl.DSLSelector.select>` method to select
@@ -920,20 +924,14 @@
         try:
             field = self.meta_type.fields[name]
         except KeyError:
             raise GraphQLError(f'Invalid meta-field "{name}"')
 
         super().__init__(name, self.meta_type, field)
 
-    def alias(self, alias: str) -> "DSLSelectableWithAlias":
-        """
-        :meta private:
-        """
-        return self
-
 
 class DSLInlineFragment(DSLSelectable, DSLFragmentSelector):
     """DSLInlineFragment represents an inline fragment for the DSL code."""
 
     _type: Union[GraphQLObjectType, GraphQLInterfaceType]
     ast_field: InlineFragmentNode
```

### Comparing `gql-3.5.0b3/gql/gql.py` & `gql-3.5.0b4/gql/gql.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/gql/transport/aiohttp.py` & `gql-3.5.0b4/gql/transport/aiohttp.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/gql/transport/appsync_auth.py` & `gql-3.5.0b4/gql/transport/appsync_auth.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/gql/transport/appsync_websockets.py` & `gql-3.5.0b4/gql/transport/appsync_websockets.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/gql/transport/async_transport.py` & `gql-3.5.0b4/gql/transport/async_transport.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/gql/transport/exceptions.py` & `gql-3.5.0b4/gql/transport/exceptions.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/gql/transport/httpx.py` & `gql-3.5.0b4/gql/transport/httpx.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 
 log = logging.getLogger(__name__)
 
 
 class _HTTPXTransport:
     file_classes: Tuple[Type[Any], ...] = (io.IOBase,)
 
-    reponse_headers: Optional[httpx.Headers] = None
+    response_headers: Optional[httpx.Headers] = None
 
     def __init__(
         self,
         url: Union[str, httpx.URL],
         json_serialize: Callable = json.dumps,
         **kwargs,
     ):
```

### Comparing `gql-3.5.0b3/gql/transport/local_schema.py` & `gql-3.5.0b4/gql/transport/local_schema.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/gql/transport/phoenix_channel_websockets.py` & `gql-3.5.0b4/gql/transport/phoenix_channel_websockets.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/gql/transport/requests.py` & `gql-3.5.0b4/gql/transport/requests.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/gql/transport/transport.py` & `gql-3.5.0b4/gql/transport/transport.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/gql/transport/websockets.py` & `gql-3.5.0b4/gql/transport/websockets.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/gql/transport/websockets_base.py` & `gql-3.5.0b4/gql/transport/websockets_base.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/gql/utilities/__init__.py` & `gql-3.5.0b4/gql/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/gql/utilities/build_client_schema.py` & `gql-3.5.0b4/gql/utilities/build_client_schema.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/gql/utilities/get_introspection_query_ast.py` & `gql-3.5.0b4/gql/utilities/get_introspection_query_ast.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/gql/utilities/parse_result.py` & `gql-3.5.0b4/gql/utilities/parse_result.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/gql/utilities/serialize_variable_values.py` & `gql-3.5.0b4/gql/utilities/serialize_variable_values.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/gql/utilities/update_schema_enum.py` & `gql-3.5.0b4/gql/utilities/update_schema_enum.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/gql/utilities/update_schema_scalars.py` & `gql-3.5.0b4/gql/utilities/update_schema_scalars.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/gql/utils.py` & `gql-3.5.0b4/gql/utils.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/gql.egg-info/PKG-INFO` & `gql-3.5.0b4/gql.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gql
-Version: 3.5.0b3
+Version: 3.5.0b4
 Summary: GraphQL client for Python
 Home-page: https://github.com/graphql-python/gql
 Author: Syrus Akbary
 Author-email: me@syrusakbary.com
 License: MIT
 Description: # GQL
         
@@ -115,14 +115,15 @@
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Description-Content-Type: text/markdown
 Provides-Extra: all
 Provides-Extra: test
 Provides-Extra: test_no_transport
 Provides-Extra: dev
 Provides-Extra: aiohttp
```

### Comparing `gql-3.5.0b3/gql.egg-info/SOURCES.txt` & `gql-3.5.0b4/gql.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -156,11 +156,12 @@
 tests/nested_input/__init__.py
 tests/nested_input/schema.py
 tests/nested_input/test_nested_input.py
 tests/starwars/__init__.py
 tests/starwars/fixtures.py
 tests/starwars/schema.py
 tests/starwars/test_dsl.py
+tests/starwars/test_introspection.py
 tests/starwars/test_parse_results.py
 tests/starwars/test_query.py
 tests/starwars/test_subscription.py
 tests/starwars/test_validation.py
```

### Comparing `gql-3.5.0b3/gql.egg-info/requires.txt` & `gql-3.5.0b4/gql.egg-info/requires.txt`

 * *Files 3% similar despite different names*

```diff
@@ -5,27 +5,27 @@
 [aiohttp]
 aiohttp<3.9.0,>=3.8.0
 
 [all]
 aiohttp<3.9.0,>=3.8.0
 requests<3,>=2.26
 requests_toolbelt<1,>=0.9.1
-urllib3>=1.26
+urllib3<2,>=1.26
 httpx<1,>=0.23.1
 websockets<11,>=10
 botocore<2,>=1.21
 
 [botocore]
 botocore<2,>=1.21
 
 [dev]
 aiohttp<3.9.0,>=3.8.0
 requests<3,>=2.26
 requests_toolbelt<1,>=0.9.1
-urllib3>=1.26
+urllib3<2,>=1.26
 httpx<1,>=0.23.1
 websockets<11,>=10
 botocore<2,>=1.21
 black==22.3.0
 check-manifest<1,>=0.42
 flake8==3.8.1
 isort==4.3.21
@@ -47,21 +47,21 @@
 
 [httpx]
 httpx<1,>=0.23.1
 
 [requests]
 requests<3,>=2.26
 requests_toolbelt<1,>=0.9.1
-urllib3>=1.26
+urllib3<2,>=1.26
 
 [test]
 aiohttp<3.9.0,>=3.8.0
 requests<3,>=2.26
 requests_toolbelt<1,>=0.9.1
-urllib3>=1.26
+urllib3<2,>=1.26
 httpx<1,>=0.23.1
 websockets<11,>=10
 botocore<2,>=1.21
 parse==1.15.0
 pytest==6.2.5
 pytest-asyncio==0.16.0
 pytest-console-scripts==1.3.1
```

### Comparing `gql-3.5.0b3/setup.py` & `gql-3.5.0b4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 install_aiohttp_requires = [
     "aiohttp>=3.8.0,<3.9.0",
 ]
 
 install_requests_requires = [
     "requests>=2.26,<3",
     "requests_toolbelt>=0.9.1,<1",
-    "urllib3>=1.26",
+    "urllib3>=1.26,<2",
 ]
 
 install_httpx_requires = [
     "httpx>=0.23.1,<1",
 ]
 
 install_websockets_requires = [
@@ -85,14 +85,15 @@
         "Topic :: Software Development :: Libraries",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation :: PyPy",
     ],
     keywords="api graphql protocol rest relay gql client",
     packages=find_packages(include=["gql*"]),
     # PEP-561: https://www.python.org/dev/peps/pep-0561/
     package_data={"gql": ["py.typed"]},
     install_requires=install_requires,
```

### Comparing `gql-3.5.0b3/tests/conftest.py` & `gql-3.5.0b4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/tests/custom_scalars/test_datetime.py` & `gql-3.5.0b4/tests/custom_scalars/test_datetime.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/tests/custom_scalars/test_enum_colors.py` & `gql-3.5.0b4/tests/custom_scalars/test_enum_colors.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/tests/custom_scalars/test_json.py` & `gql-3.5.0b4/tests/custom_scalars/test_json.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/tests/custom_scalars/test_money.py` & `gql-3.5.0b4/tests/custom_scalars/test_money.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/tests/custom_scalars/test_parse_results.py` & `gql-3.5.0b4/tests/custom_scalars/test_parse_results.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/tests/fixtures/aws/fake_credentials.py` & `gql-3.5.0b4/tests/fixtures/aws/fake_credentials.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/tests/fixtures/aws/fake_request.py` & `gql-3.5.0b4/tests/fixtures/aws/fake_request.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/tests/fixtures/aws/fake_session.py` & `gql-3.5.0b4/tests/fixtures/aws/fake_session.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/tests/fixtures/aws/fake_signer.py` & `gql-3.5.0b4/tests/fixtures/aws/fake_signer.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/tests/fixtures/vcr_cassettes/client.yaml` & `gql-3.5.0b4/tests/fixtures/vcr_cassettes/client.yaml`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/tests/fixtures/vcr_cassettes/queries.yaml` & `gql-3.5.0b4/tests/fixtures/vcr_cassettes/queries.yaml`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/tests/nested_input/schema.py` & `gql-3.5.0b4/tests/nested_input/schema.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/tests/nested_input/test_nested_input.py` & `gql-3.5.0b4/tests/nested_input/test_nested_input.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/tests/starwars/fixtures.py` & `gql-3.5.0b4/tests/starwars/fixtures.py`

 * *Files 19% similar despite different names*

```diff
@@ -140,7 +140,49 @@
     return droidData.get(id)
 
 
 def create_review(episode, review):
     reviews[episode].append(review)
     review["episode"] = episode
     return review
+
+
+async def make_starwars_backend(aiohttp_server):
+    from aiohttp import web
+    from .schema import StarWarsSchema
+    from graphql import graphql_sync
+
+    async def handler(request):
+        data = await request.json()
+        source = data["query"]
+
+        try:
+            variables = data["variables"]
+        except KeyError:
+            variables = None
+
+        result = graphql_sync(StarWarsSchema, source, variable_values=variables)
+
+        return web.json_response(
+            {
+                "data": result.data,
+                "errors": [str(e) for e in result.errors] if result.errors else None,
+            }
+        )
+
+    app = web.Application()
+    app.router.add_route("POST", "/", handler)
+    server = await aiohttp_server(app)
+
+    return server
+
+
+async def make_starwars_transport(aiohttp_server):
+    from gql.transport.aiohttp import AIOHTTPTransport
+
+    server = await make_starwars_backend(aiohttp_server)
+
+    url = server.make_url("/")
+
+    transport = AIOHTTPTransport(url=url, timeout=10)
+
+    return transport
```

### Comparing `gql-3.5.0b3/tests/starwars/schema.py` & `gql-3.5.0b4/tests/starwars/schema.py`

 * *Files 5% similar despite different names*

```diff
@@ -151,14 +151,19 @@
 review_input_type = GraphQLInputObjectType(
     "ReviewInput",
     lambda: {
         "stars": GraphQLInputField(GraphQLInt, description="0-5 stars"),
         "commentary": GraphQLInputField(
             GraphQLString, description="Comment about the movie, optional"
         ),
+        "deprecated_input_field": GraphQLInputField(
+            GraphQLString,
+            description="deprecated field example",
+            deprecation_reason="deprecated for testing",
+        ),
     },
     description="The input object sent when someone is creating a new review",
 )
 
 query_type = GraphQLObjectType(
     "Query",
     lambda: {
```

### Comparing `gql-3.5.0b3/tests/starwars/test_dsl.py` & `gql-3.5.0b4/tests/starwars/test_dsl.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,16 @@
     IntValueNode,
     ListTypeNode,
     NamedTypeNode,
     NameNode,
     NonNullTypeNode,
     NullValueNode,
     Undefined,
+    build_ast_schema,
+    parse,
     print_ast,
 )
 from graphql.utilities import get_introspection_query
 
 from gql import Client, gql
 from gql.dsl import (
     DSLFragment,
@@ -770,16 +772,14 @@
     assert ("Invalid field for <DSLQuery>: <DSLField Character::name>") in str(
         excinfo.value
     )
 
 
 def test_dsl_root_type_not_default():
 
-    from graphql import parse, build_ast_schema
-
     schema_str = """
 schema {
   query: QueryNotDefault
 }
 
 type QueryNotDefault {
   version: String
@@ -823,14 +823,49 @@
 def test_invalid_type(ds):
     with pytest.raises(
         AttributeError, match="Type 'invalid_type' not found in the schema!"
     ):
         ds.invalid_type
 
 
+def test_invalid_type_union():
+    schema_str = """
+    type FloatValue {
+        floatValue: Float!
+    }
+
+    type IntValue {
+        intValue: Int!
+    }
+
+    union Value = FloatValue | IntValue
+
+    type Entry {
+        name: String!
+        value: Value
+    }
+
+    type Query {
+        values: [Entry!]!
+    }
+    """
+
+    schema = build_ast_schema(parse(schema_str))
+    ds = DSLSchema(schema)
+
+    with pytest.raises(
+        AttributeError,
+        match=(
+            "Type \"Value \\(<GraphQLUnionType 'Value'>\\)\" is not valid as an "
+            "attribute of DSLSchema. Only Object types or Interface types are accepted."
+        ),
+    ):
+        ds.Value
+
+
 def test_hero_name_query_with_typename(ds):
     query = """
 hero {
   name
   __typename
 }
     """.strip()
@@ -866,19 +901,14 @@
     DSLQuery(DSLMetaField("__typename"))
     DSLQuery(DSLMetaField("__schema"))
     DSLQuery(DSLMetaField("__type"))
 
     metafield = DSLMetaField("__typename")
     assert metafield.name == "__typename"
 
-    # alias does not work
-    metafield.alias("test")
-
-    assert metafield.name == "__typename"
-
     with pytest.raises(GraphQLError):
         DSLMetaField("__invalid_meta_field")
 
     DSLMutation(DSLMetaField("__typename"))
 
     with pytest.raises(GraphQLError):
         DSLMutation(DSLMetaField("__schema"))
@@ -932,7 +962,26 @@
         descriptions=option,
         specified_by_url=option,
         directive_is_repeatable=option,
         schema_description=option,
     )
 
     assert print_ast(gql(introspection_query)) == print_ast(dsl_introspection_query)
+
+
+def test_typename_aliased(ds):
+    query = """
+hero {
+  name
+  typenameField: __typename
+}
+""".strip()
+
+    query_dsl = ds.Query.hero.select(
+        ds.Character.name, typenameField=DSLMetaField("__typename")
+    )
+    assert query == str(query_dsl)
+
+    query_dsl = ds.Query.hero.select(
+        ds.Character.name, DSLMetaField("__typename").alias("typenameField")
+    )
+    assert query == str(query_dsl)
```

### Comparing `gql-3.5.0b3/tests/starwars/test_parse_results.py` & `gql-3.5.0b4/tests/starwars/test_parse_results.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/tests/starwars/test_query.py` & `gql-3.5.0b4/tests/starwars/test_query.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/tests/starwars/test_subscription.py` & `gql-3.5.0b4/tests/starwars/test_subscription.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/tests/starwars/test_validation.py` & `gql-3.5.0b4/tests/starwars/test_validation.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/tests/test_aiohttp.py` & `gql-3.5.0b4/tests/test_aiohttp.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/tests/test_aiohttp_online.py` & `gql-3.5.0b4/tests/test_aiohttp_online.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/tests/test_appsync_auth.py` & `gql-3.5.0b4/tests/test_appsync_auth.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/tests/test_appsync_http.py` & `gql-3.5.0b4/tests/test_appsync_http.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/tests/test_appsync_websockets.py` & `gql-3.5.0b4/tests/test_appsync_websockets.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/tests/test_async_client_validation.py` & `gql-3.5.0b4/tests/test_async_client_validation.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/tests/test_cli.py` & `gql-3.5.0b4/tests/test_cli.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
 
 import pytest
 
 from gql import __version__
 from gql.cli import (
     get_execute_args,
+    get_introspection_args,
     get_parser,
     get_transport,
     get_transport_args,
     main,
 )
 
 
@@ -372,7 +373,50 @@
 def test_cli_ep_version(script_runner):
     ret = script_runner.run("gql-cli", "--version")
 
     assert ret.success
 
     assert ret.stdout == f"v{__version__}\n"
     assert ret.stderr == ""
+
+
+def test_cli_parse_schema_download(parser):
+
+    args = parser.parse_args(
+        [
+            "https://your_server.com",
+            "--schema-download",
+            "descriptions:false",
+            "input_value_deprecation:true",
+            "specified_by_url:True",
+            "schema_description:true",
+            "directive_is_repeatable:true",
+            "--print-schema",
+        ]
+    )
+
+    introspection_args = get_introspection_args(args)
+
+    expected_args = {
+        "descriptions": False,
+        "input_value_deprecation": True,
+        "specified_by_url": True,
+        "schema_description": True,
+        "directive_is_repeatable": True,
+    }
+
+    assert introspection_args == expected_args
+
+
+@pytest.mark.parametrize(
+    "invalid_args",
+    [
+        ["https://your_server.com", "--schema-download", "ArgWithoutColon"],
+        ["https://your_server.com", "--schema-download", "blahblah:true"],
+        ["https://your_server.com", "--schema-download", "descriptions:invalid_bool"],
+    ],
+)
+def test_cli_parse_schema_download_invalid_arg(parser, invalid_args):
+    args = parser.parse_args(invalid_args)
+
+    with pytest.raises(ValueError):
+        get_introspection_args(args)
```

### Comparing `gql-3.5.0b3/tests/test_client.py` & `gql-3.5.0b4/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/tests/test_graphqlws_exceptions.py` & `gql-3.5.0b4/tests/test_graphqlws_exceptions.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/tests/test_graphqlws_subscription.py` & `gql-3.5.0b4/tests/test_graphqlws_subscription.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/tests/test_http_async_sync.py` & `gql-3.5.0b4/tests/test_http_async_sync.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/tests/test_httpx.py` & `gql-3.5.0b4/tests/test_httpx.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/tests/test_httpx_async.py` & `gql-3.5.0b4/tests/test_httpx_async.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/tests/test_httpx_online.py` & `gql-3.5.0b4/tests/test_httpx_online.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/tests/test_localhost.pem` & `gql-3.5.0b4/tests/test_localhost.pem`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/tests/test_phoenix_channel_exceptions.py` & `gql-3.5.0b4/tests/test_phoenix_channel_exceptions.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/tests/test_phoenix_channel_query.py` & `gql-3.5.0b4/tests/test_phoenix_channel_query.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/tests/test_phoenix_channel_subscription.py` & `gql-3.5.0b4/tests/test_phoenix_channel_subscription.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/tests/test_requests.py` & `gql-3.5.0b4/tests/test_requests.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/tests/test_transport.py` & `gql-3.5.0b4/tests/test_transport.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/tests/test_websocket_exceptions.py` & `gql-3.5.0b4/tests/test_websocket_exceptions.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/tests/test_websocket_online.py` & `gql-3.5.0b4/tests/test_websocket_online.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/tests/test_websocket_query.py` & `gql-3.5.0b4/tests/test_websocket_query.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/tests/test_websocket_subscription.py` & `gql-3.5.0b4/tests/test_websocket_subscription.py`

 * *Files identical despite different names*

### Comparing `gql-3.5.0b3/tox.ini` & `gql-3.5.0b4/tox.ini`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 [tox]
 envlist =
     black,flake8,import-order,mypy,manifest,
-    py{37,38,39,310,py3}
+    py{37,38,39,310,311,py3}
 
 [gh-actions]
 python =
     3.7: py37
     3.8: py38
     3.9: py39
     3.10: py310
+    3.11: py311
     pypy-3: pypy3
 
 [testenv]
 conda_channels = conda-forge
 passenv = *
 setenv =
     PYTHONPATH = {toxinidir}
@@ -23,15 +24,15 @@
 whitelist_externals =
     python
 deps = -e.[test]
 ; Prevent installing issues: https://github.com/ContinuumIO/anaconda-issues/issues/542
 commands =
     pip install -U setuptools
     ; run "tox -- tests -s" to show output for debugging
-    py{37,39,310,py3}: pytest {posargs:tests}
+    py{37,39,310,311,py3}: pytest {posargs:tests}
     py{38}: pytest {posargs:tests --cov-report=term-missing --cov=gql}
 
 [testenv:black]
 basepython = python3.8
 deps = -e.[dev]
 commands =
     black --check gql tests
```

